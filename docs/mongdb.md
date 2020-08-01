### MongoDB

- [文档](https://docs.mongodb.com/)

#### 常用数据库

> 关系型数据库

- mysql
    - 被收购了，开源数据库，说不定那天就收费了
- oracle
    - 稳定，性能强，可定制可优化，容灾
- PostgreSQL
    - 传统 sql类型语言
    - 支持json
    - 适合分布式系统

> nosql数据库(key/value数据库)

- mongodb
    - 分布式系统有良好的兼容性
    - 对机器的要求高一点，但是能承受的并发量，和读写单表的数据大小要比mysql好很多
    - 在老一点版本mysql 5.7之前，单表数据1000万的时候，进行插入和加索引查询比较慢，而mongoDB到达1亿左右的数据都不会有明显的下降
- redis
- memocache


### mongoDB 使用

- 推荐docker 方式
    - https://www.runoob.com/docker/docker-install-mongodb.html

```
docker run -p 27017:27017 -v $PWD/db:/data/db -d mongo:3.6.15
docker ps -a 查看 mongo id编号
# 进入 容器内部
docker exec -it id编号 bash 
# 开启 mongodb
mongo

# 使用方式
# 使用我们的数据库 不存在则创建
use what_i_love

# 查看表
show collections;

# 插入数据 同时创建表
db.users.insert({name:"hjx",age:100})

# 查询数据
db.users.find()

# 查询数据 查看数据方式美化
db.users.find().pretty()

# 更改数据
db.users.update({name:"hjx"},{name:"hjx",age:20})

# 删除数据
db.users.remove({})

# 查看帮助文档
db.users.help()

# 创建索引
db.users.createIndex({name:1})

# 获取索引
db.users.getIndexes({name:1})
```

#### ObjectId 问题

```
# 插入单条数据,他会把插入后的 id返回给你
db.users.insertOne({name:'hjx',age:29})
# 返回内容如下
{
	"acknowledged" : true,
	"insertedId" : ObjectId("5e8e8c929f5bb82134fad5db")
}
```

- mongoDB对分布式的系统设计非常友好

> 特别是你想生成一个自增长的主键，在分布式你会遇到问题

- 如何保证唯一性，如 mysql 的主键状态同步问题
    - 一个表我分了表，数据会被同时存到两张不同的表里去，或者10多台不同的服务器上去
        - 你就不能通过某一台服务器某一个数据库让它 +1，你必须问其他数据库 现在加到几了

- mongodb的处理
    - 首先有这个自增长的数字
    - 其次时间戳
    - 加上 机器编码
    - 最后每个 mongo开启会有一个 进程号
- `ObjectId = 自增长id + 时间戳 + 机器编码 + mongoDB的进程号`
- 有效避免了 mysql需要 全局维护一个自增长的变量来存储当前表里状态的情况
    - 你始终要有一个地方 去存现在 id到底是几
    - 如果这个业务中心这个服务挂掉了，你在其他地方想要恢复它是一个困难的问题
    - 结论：最好不要有这个中心化的东西管理系统 处理这个 主键id


#### 如果对数据有强烈要求(准确性)

- 电商/订单等问题 **不要用mongoDB，而是mysql**

#### mongoDB 添加字段问题

- 可方便的添加新的字段，不用像 mysql 那样设计的时候 定义扩展字段 (name,age,city ,extra1 , extra2, extra3)

```
db.users.insert({name:"hjx",age:100})

db.users.insert({name:"aaa",age:33,city:"tj"})
db.users.insert({name:"aaa",age:22,city:"bj"})

# 查询的时候
> db.users.find()
{ "_id" : ObjectId("5e8e8c929f5bb82134fad5db"), "name" : "hjx", "age" : 29 }
{ "_id" : ObjectId("5e8e97129f5bb82134fad5dc"), "name" : "aaa", "age" : 33, "city" : "tj" }
{ "_id" : ObjectId("5e8e97169f5bb82134fad5dd"), "name" : "aaa", "age" : 22, "city" : "bj" }
```

#### find条件筛选

```
# 查找 age = 30的
db.users.find({age:30})

# 操作符 大于12的
db.users.find({age: {$gt:12}})

# 操作符 大于等于12的
db.users.find({age: {$gte:12}})

# 操作符 小于等于12的
db.users.find({age: {$lte:12}})

# 大于等于12 小于等于30
db.users.find({age: {$lte:30 , $gte:12}})

# 是否存在 city
db.users.find({city: {$exists:true}})
```

> 只要某些字段

```
# 默认会返回id 如果你不设置的话
# 查询所有数据 返回 id,age
db.users.find({},{age:true})
db.users.find({},{age:1})

# 除了age其他字段都查出来
db.users.find({},{age:0})
```

#### update 的大惊喜

```
# 把你 name=hjx 的数据 改的只有 id 和 age
db.users.update({name:'hjx'},{age:57}) 

# 务必用 $set 更新某一个字段的时候
db.users.update({name:'hjx'},{$set:{age:57}}) 
```

#### `$unset` 滞空值

```
# 去除 age字段
db.users.update({name:'hjx'},{$unset:{age:true}}) 
```

#### `findOneAndUpdate`

```
更新并返回
db.users.findOneAndUpdate({name:'hjx'},{$set:{age:11}},{returnNewDockment:true}) 
```

# 查询不到就新增

- 原子操作

```
db.users.findOneAndUpdate({name:'hjx'},{$set:{age:11}},{upsert:true}) 
```

#### deleteOne

```
# 删除 name= aa city不存在的
db.users.deleteOne({name:'aa',city:{$exists:false}})
```

### 字段重命名

- https://blog.csdn.net/shellching/article/details/7651721

```
db.test.update({}, {$rename : {"abc" : "def"}}, false, true)
```

### 聚合操作

```
db.users.aggregate([
    {
        $match:{
            age:{
                $exists:true
            },
            name:{
                $exists:true
            }
        }
    },
    {
        $group:{
            _id:"$name",
            avgName:{
                $avg:'$age'
            }
        }
    }
])
```

### 索引问题

```
# name 根据升序排列
db.users.createIndex({name:1})

# 删除索引
db.users.dropIndex({name:1})

# 添加name唯一索引
db.users.createIndex({name:1},{unique:1})

# 获取索引
db.users.getIndexes()
```

> 各种操作参考

- [mongoDb入门一](https://sltrust.github.io/2018/05/10/MONGODB_001_%E5%85%A5%E9%97%A81/)
- [mongoDb练习一](https://sltrust.github.io/2018/05/10/MONGODB_002_%E7%BB%83%E4%B9%A01/)
- [mongoDb练习二](https://sltrust.github.io/2018/05/10/MONGODB_003_%E7%BB%83%E4%B9%A02/)
- [mongoDb文档之间的关系](https://sltrust.github.io/2018/05/10/MONGODB_004%E6%96%87%E6%A1%A3%E9%97%B4%E7%9A%84%E5%85%B3%E7%B3%BB/)
- [mongoDb练习三](https://sltrust.github.io/2018/05/10/MONGODB_005_%E7%BB%83%E4%B9%A03/)
- [mongoose是什么鬼](https://sltrust.github.io/2018/05/10/MONGODB_006_mongoose/)
- [Schema和Model](https://sltrust.github.io/2018/05/10/MONGODB_007_Schema%E5%92%8CModel/)

### MongoDB

MongoDB作为最流行的NoSQL数据库之一，运用灰常广泛，其友好的JSON支持和灵活的表单结构，使其在使用Node.js开发的诸多Web应用中非常受欢迎
在高性能分布式存储领域，MongoDB也有一席之地，然而MongoDB对事务的不友好和过于灵活的特性也带来了一些问题

#### mongoose

mongoose是MongoDB的Node.js框架，在处理MongoDB表管理、验证方面有方便之处

**hello world**

```
const mongoose = require('mongoose');

mongoose.Promise = Promise;

const uri = `mongodb://localhost:27017/what_i_love`;
mongoose.connect(uri, { useMongoClient: true });
const db = mongoose.connection;

const Schema = mongoose.Schema;

const ObjectId = Schema.Types.ObjectId;

const UserSchema = new Schema({
  name: { type: String, required: true, unique: true, index: 1 },
  age: { type: Number, max: 188, min: 0 },
});

const UserModel = mongoose.model('user', UserSchema);

(async (params) => {

  const filter = {};
  if (params.name) filter.name = params.name;

  const flow = UserModel.find(filter);

  if(params.projection) flow.select(params.projection);

  if(params.sort) flow.sort(params.sort);

  const users = await flow.exec();

  return users;

})({
  name:"xiaoli",
  projection: {age:1},
  // sort:{age:-1},
  sort:'-age'
})
  .then(r => {
    console.log(r);
  })
  .catch(e => {
    console.log(e);
  });

db.on('open', () => {
  console.log('db connected!');
});

db.on('error', (e) => {
  console.log(e);
});
```

#### Schema属性和验证

```
{
    name:{
        type: String,
        required: true
    }, //存储之前会验证
    age:{
        type:Number,
        min:1,
        max:[12, 'Growned are not welcome!'],
    },
    address:[new Schema({
      city:String,
      province:String,
    })]
}
```

#### 查询（流）

```
const query = Model.find({name:{$regex:"a"}});
query.where('age').lte(2);
if(params.limit) query.limit(params.limit);
query.sort('-age');

const result = await query.then();
```

使用Schema.statics和Schema.method可以定义用于查询的方法