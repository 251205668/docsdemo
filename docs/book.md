# 追书神器API 接口文档 -- 仅供学习使用！！！


```

API域名: http://api.zhuishushenqi.com

图片域名: http://statics.zhuishushenqi.com

章节域名: http://chapterup.zhuishushenqi.com

```


 

## 接口列表：

----

### 获取所有排行榜</h3>

 请求URL:  
```
http://api.zhuishushenqi.com/ranking/gender
```

 示例：
 [http://api.zhuishushenqi.com/ranking/gender](http://api.zhuishushenqi.com/ranking/gender)

 请求方式: `GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|无      |无       |无   |无  |

 返回示例：

```json
{
    "male": [
        {
            "_id": "54d42d92321052167dfb75e3",
            "title": "追书最热榜 Top100",
            "cover": "/ranking-cover/142319144267827",
            "collapse": false,
            "monthRank": "564d820bc319238a644fb408",
            "totalRank": "564d8494fe996c25652644d2",
            "shortTitle": "最热榜"
        }...
    ],
    "female": [
        {
            "_id": "54d43437d47d13ff21cad58b",
            "title": "追书最热榜 Top100",
            "cover": "/ranking-cover/142319314350435",
            "collapse": false,
            "monthRank": "564d853484665f97662d0810",
            "totalRank": "564d85b6dd2bd1ec660ea8e2",
            "shortTitle": "最热榜"
        }...
    ]
}
```

---

### 获取单一排行榜

 请求URL：
```
http://api.zhuishushenqi.com/ranking/{rankingId}
```

 示例：
[http://api.zhuishushenqi.com/ranking/54d43437d47d13ff21cad58b](http://api.zhuishushenqi.com/ranking/54d43437d47d13ff21cad58b)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|rankingId      |Y       |string   | 周榜：_id,月榜：monthRank,总榜：totalRank |

 返回示例：
```json
{
    "ranking": {
        "_id": "54d43437d47d13ff21cad58b",
        "updated": "2017-09-10T21:20:06.740Z",
        "title": "追书最热榜 Top100",
        "tag": "manualRank",
        "cover": "/ranking-cover/142319314350435",
        "icon": "/cover/148945782817557",
        "__v": 1194,
        "monthRank": "564d853484665f97662d0810",
        "totalRank": "564d85b6dd2bd1ec660ea8e2",
        "shortTitle": "最热榜",
        "created": "2017-09-11T13:20:35.079Z",
        "isSub": false,
        "collapse": false,
        "new": true,
        "gender": "female",
        "priority": 250,
        "books": [
            {
                "_id": "578f718209013c307e2c71c0",
                "title": "隐婚100分：惹火娇妻嫁一送一",
                "author": "囧囧有妖",
                "shortIntro": "“你救了我，我让我爹地以身相许！”宁夕意外救了只小包子，结果被附赠了一只大包子。婚后，陆霆骁宠妻如命千依百顺，虐起狗来连亲儿子都不放过。“老板，公司真给夫人拿去玩？难道夫人要卖公司您也不管？”“卖你家公司了？”“大少爷，不好了！夫人说要把屋顶掀了！”“还不去帮夫人扶梯子。”“粑粑，谢谢你给小宝买的大熊！”“那是买给你妈妈的。”“老公，这个剧本我特别喜欢，只是床戏有点多，我可以接吗？”陆霆骁神色淡定：“可以。”当天晚上，宁夕扶着腰连滚带爬逃下床。陆霆骁！可以你大爷！！！",
                "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F86590%2F86590_9ec02fe59dbd40b999c420fcc43a75b0.jpg%2F",
                "site": "zhuishuvip",
                "banned": 0,
                "latelyFollower": 82377,
                "retentionRatio": "45.82"
            }...
        ],
        "id": "54d43437d47d13ff21cad58b",
        "total": 98
    },
    "ok": true
}
```

---

### 获取书单列表

 请求URL：
```
http://api.zhuishushenqi.com/book-list
```

 示例：
[http://api.zhuishushenqi.com/book-list?duration=all&sort=collectorCount&start=0&limit=20&tag=古代&gender=male](http://api.zhuishushenqi.com/book-list?duration=all&sort=collectorCount&start=0&limit=20&tag=古代&gender=male)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|duration      |Y       |string   | 本周最热：duration=last-seven-days&sort=collectorCount,最新发布：duration=all&sort=created,最多收藏：duration=all&sort=collectorCount |
|sort      |Y       |string   | 看上个参数 |
|start      |Y       |string   | 起始位置从0开始 |
|limit      |Y       |string   | 20 |
|tag      |Y       |string   | 都市、古代、架空、重生、玄幻、网游 |
|gender      |Y       |string   | male、female |

 返回示例：
```json
{
    "total": 1916,
    "bookLists": [
        {
            "_id": "5659f9c28498cf236a508b08",
            "title": "无敌爽文🐎",
            "author": "原罪&七罪",
            "desc": "本人很,懒喜欢的收藏  经典📚无限📘  粮草&储备   ♞♞ 挑灯💡夜读📖   🌙",
            "gender": "male",
            "collectorCount": 31459,
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F1183975%2F_1183975_531140.jpg%2F",
            "bookCount": 437
        }...
    ],
    "ok": true
}
```
---

### 获取书单标签列表

 请求URL:  
```
http://api.zhuishushenqi.com/book-list/tagType
```

 示例：
 [http://api.zhuishushenqi.com/book-list/tagType](http://api.zhuishushenqi.com/book-list/tagType)

 请求方式: `GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|无      |无       |无   |无  |

 返回示例：

```json
{
    "data": [
        {
            "name": "时空",
            "tags": [
                "都市",
                "古代",
                "科幻",
                "架空",
                "重生",
                "未来",
                "穿越",
                "历史",
                "快穿",
                "末世",
                "异界位面"
            ]
        }...
    ],
    "ok":true
}
```


---

### 获取书单详情

 请求URL：
```
http://api.zhuishushenqi.com/book-list/{bookListId}
```

 示例：
[http://api.zhuishushenqi.com/book-list/5659f9c28498cf236a508b08](http://api.zhuishushenqi.com/book-list/5659f9c28498cf236a508b08)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|bookListId      |Y       |string   | 书单Id |

 返回示例：
```json
{
    "total": 1916,
    "bookLists": [
        {
            "_id": "5659f9c28498cf236a508b08",
            "title": "无敌爽文🐎",
            "author": "原罪&七罪",
            "desc": "本人很,懒喜欢的收藏  经典📚无限📘  粮草&储备   ♞♞ 挑灯💡夜读📖   🌙",
            "gender": "male",
            "collectorCount": 31459,
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F1183975%2F_1183975_531140.jpg%2F",
            "bookCount": 437
        }...
    "ok": true
}
```


---

### 获取分类

 请求URL:  
```
http://api.zhuishushenqi.com/cats/lv2/statistics
```

 示例：
 [http://api.zhuishushenqi.com/cats/lv2/statistics](http://api.zhuishushenqi.com/cats/lv2/statistics)

 请求方式: `GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|无      |无       |无   |无  |

 返回示例：

```json
{
    "male": [
        {
            "name": "玄幻",
            "bookCount": 475245,
            "monthlyCount": 13366,
            "icon": "/icon/玄幻_.png"
        }...
    ],
    "female": [
        {
            "name": "古代言情",
            "bookCount": 427554,
            "monthlyCount": 9293,
            "icon": "/icon/古代言情_.png"
        }...
    ],
    "picture": [
        {
            "name": "热血",
            "bookCount": 330,
            "monthlyCount": 0,
            "icon": "/icon/热血_.png"
        }...
    ],
    "press": [
        {
            "name": "传记名著",
            "bookCount": 2801,
            "monthlyCount": 0,
            "icon": "/icon/传记名著_.png"
        }...
    ],
    "ok": true
}
```

---

### 获取二级分类

 请求URL:  
```
http://api.zhuishushenqi.com/cats/lv2
```

 示例：
 [http://api.zhuishushenqi.com/cats/lv2](http://api.zhuishushenqi.com/cats/lv2)

 请求方式: `GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|无      |无       |无   |无  |

 返回示例：

```json
{
    "male": [
        {
            "major": "玄幻",
            "mins": [
                "东方玄幻",
                "异界大陆",
                "异界争霸",
                "远古神话"
            ]
        }...
    ],
    "female": [
        {
            "major": "古代言情",
            "mins": [
                "穿越时空",
                "古代历史",
                "古典架空",
                "宫闱宅斗",
                "经商种田"
            ]
        }...
    ],
    "picture": [
        {
            "major": "热血",
            "mins": []
        }...
    ],
    "press": [
        {
            "major": "出版小说",
            "mins": []
        }...
    ],
    "ok": true
}
```


---

### 按分类获取书籍列表

 请求URL：
```
http://api.zhuishushenqi.com/book/by-categories
```

 示例：
[http://api.zhuishushenqi.com/book/by-categories?gender=male&type=hot&major=玄幻&minor=东方玄幻&start=0&limit=20](http://api.zhuishushenqi.com/book/by-categories?gender=male&type=hot&major=玄幻&minor=东方玄幻&start=0&limit=20)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|type      |Y       |string   | 热门:`hot` 新书:`new ` 好评:`repulation ` 完结:`over ` 包月: `month `|
|major      |Y       |string   | 大类别 从接口[6、获取分类](#6)获取 |
| minor      |N       |string   | 小类别 从接口[7、获取二级分类](#7)获取 |
|start      |Y       |string   | 分页开始位置，起始位置从0开始 |
|limit      |Y       |string   | 分页条数 |
|gender      |Y       |string   | 男生:`mael ` 女生:`female ` 出版:`press ` |


 返回示例：

```json
{
    "total": 40215,
    "books": [
        {
            "_id": "5816b415b06d1d32157790b1",
            "title": "圣墟",
            "author": "辰东",
            "shortIntro": "在破败中崛起，在寂灭中复苏。沧海成尘，雷电枯竭，那一缕幽雾又一次临近大地，世间的枷锁被打开了，一个全新的世界就此揭开神秘的一角……",
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F1228859%2F_1228859_441552.jpg%2F",
            "site": "zhuishuvip",
            "majorCate": "玄幻",
            "minorCate": "东方玄幻",
            "sizetype": -1,
            "superscript": "",
            "contentType": "txt",
            "allowMonthly": false,
            "banned": 0,
            "latelyFollower": 305266,
            "retentionRatio": 72.08,
            "lastChapter": "第629章 闷棍镇压昆仑",
            "tags": [
                "玄幻",
                "东方玄幻"
            ]
        }...
    ],
    "ok": true
}
```


---

### 获取综合讨论区帖子列表

 请求URL：
```
http://api.zhuishushenqi.com/post/by-block
```

 全部、默认排序：
[http://api.zhuishushenqi.com/post/by-block?block=ramble&duration=all&sort=updated&type=all&start=0&limit=20&distillate=](http://api.zhuishushenqi.com/post/by-block?block=ramble&duration=all&sort=updated&type=all&start=0&limit=20&distillate=)

 精品、默认排序：
[http://api.zhuishushenqi.com/post/by-block?block=ramble&duration=all&sort=updated&type=all&start=0&limit=20&distillate=true](http://api.zhuishushenqi.com/post/by-block?block=ramble&duration=all&sort=updated&type=all&start=0&limit=20&distillate=true)
     *

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|block      |Y       |string   | ramble:综合讨论区  original：原创区 |
|duration      |Y       |string   | all |
|start      |Y       |string   | 起始位置从0开始 |
|limit      |Y       |string   | 20 |
|sort      |Y       |string   | updated(默认排序) created(最新发布) comment-count(最多评论) |
|type      |Y       |string   | all |
|distillate      |Y       |string   | true(精品) |

 返回示例：
```json
{
    "posts": [
        {
            "_id": "59b5edbfe41bc82033773be9",
            "author": {
                "_id": "56e903c1febd4661455a0692",
                "avatar": "/avatar/7b/e1/7be142f47d8ef8834727b1dd2c7bbbc1",
                "nickname": "追书家的眼镜娘",
                "activityAvatar": "/activities/20170120/4.jpg",
                "type": "official",
                "lv": 9,
                "gender": "female"
            },
            "type": "normal",
            "likeCount": 222,
            "block": "ramble",
            "haveImage": false,
            "state": "normal",
            "updated": "2017-09-11T14:05:59.568Z",
            "created": "2017-09-11T01:58:23.843Z",
            "commentCount": 1470,
            "voteCount": 0,
            "title": "【话题】你最希望哪本小说出番外/续集？"
        }...
    ]
    "ok": true
}
```


---

### 获取综合讨论区帖子详情

 请求URL：
```
http://api.zhuishushenqi.com/post/{disscussionId}
```

 示例：
[http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9](http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|disscussionId      |Y       |string   | disscussionId->_id 帖子的id |

 返回示例：
```json
{
    "post": {
        "_id": "59b5edbfe41bc82033773be9",
        "author": {
            "_id": "56e903c1febd4661455a0692",
            "avatar": "/avatar/7b/e1/7be142f47d8ef8834727b1dd2c7bbbc1",
            "nickname": "追书家的眼镜娘",
            "activityAvatar": "/activities/20170120/4.jpg",
            "type": "official",
            "lv": 9,
            "gender": "female",
            "rank": null,
            "created": "2016-03-16T06:57:05.000Z",
            "id": "56e903c1febd4661455a0692"
        },
        "type": "normal",
        "isStopPriority": false,
        "deleted": false,
        "likeCount": 355,
        "isStick": true,
        "block": "ramble",
        "state": "normal",
        "updated": "2017-09-12T13:06:51.586Z",
        "created": "2017-09-11T01:58:23.843Z",
        "commentCount": 2330,
        "voteCount": 0,
        "votes": [],
        "content": "(-@y@) [扶眼镜] 说起完结文，总会有基本你超想让作者出番外/续集的吧！不仅仅是小说主线人物的番外，其他人物也有TA精彩的故事想要知道。那对于你们来，你们最希望哪本小说出番外/续集呢？\r\n\r\n《↘↘↘直接本帖回帖格式：》\r\n#希望#+______（书名/电视剧/动漫）出番外/续集+______（想看什么剧情等相关话题内容）\r\n【周三（9月13日） 抽奖，随机选择符合要求的评论奖励666追书券】\n\n--------------------------------\r\n*请回复讨论与本期话题相关的内容，与其无关的楼层会被官方V删除。\r\n*《相关功能问题请到反馈区发帖》\r\n*如果有小伙伴发现问题解决不了（比如闪退问题），请第一时间先关注微信公众号【zssqxs】输入【RG】和客服反馈！\r\n*书架上有书籍丢失问题：①在微信公众号找在线客服清理书架缓存；②向在线客服进行登记。\r\n\r\n--------------------------------\r\n你们不赚点书券在追更完之后看看漫画咩~\r\n（安卓3.115.1版本 、IOS 2.26.24版本及以上版本有【漫画专区】哦！）\r\n--------------------------------\r\n《敲黑板》\r\n不符合回帖格式一律没奖励机会。每次镜娘的活动和话题，只有认真互动，都是有几率找到自己感兴趣的小说，解决书荒问题。\r\n--------------------------------\r\n另外，天蚕土豆新书9月14日，全网发布！你们猜这次的书名会是什么呢？",
        "title": "【话题】你最希望哪本小说出番外/续集？",
        "shareLink": "http://share.zhuishushenqi.com/post/59b5edbfe41bc82033773be9",
        "id": "59b5edbfe41bc82033773be9"
    },
    "ok": true
}
```


---

### 获取神评论列表(综合讨论区、书评区、书荒区皆为同一接口

 请求URL：
```
http://api.zhuishushenqi.com/post/{disscussionId}/comment/best
```

 示例：
[http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9/comment/best](http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9/comment/best)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|disscussionId      |Y       |string   | disscussionId->_id 帖子的id |

 返回示例：
```json
{
    "comments": [
        {
            "_id": "59b5f3a7a17d25ad324e20c8",
            "content": "(-@y@) [扶眼镜] 本帖回复“签到”一律没有奖励！\r\n想要回“签到”的一律左拐去“活动福利”专区找@追书家的Benny的帖子！\r\n想要认真互动和交流的\r\n小火们请回复#希望#+_____（自己希望看番外的小说名/动漫/影视）进行互动。\r\n*可以说说想看什么样的番外剧情？或者哪些小说里还有疑点没有说明想要作者可以写番外说明的？",
            "author": {
                "_id": "56e903c1febd4661455a0692",
                "avatar": "/avatar/7b/e1/7be142f47d8ef8834727b1dd2c7bbbc1",
                "nickname": "追书家的眼镜娘",
                "activityAvatar": "/activities/20170120/4.jpg",
                "type": "official",
                "lv": 9,
                "gender": "female"
            },
            "floor": 71,
            "likeCount": 279,
            "created": "2017-09-11T02:23:35.884Z",
            "replyTo": null
        }...
    ],
    "ok": true
}
```


---

### 获取综合讨论区帖子详情内的评论列表

 请求URL：
```
http://api.zhuishushenqi.com/post/{disscussionId}/comment
```

 示例：
[http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9/comment?start=0&limit=30](http://api.zhuishushenqi.com/post/59b5edbfe41bc82033773be9/comment?start=0&limit=30)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|disscussionId      |Y       |string   | disscussionId->_id 帖子的id |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-30 |

 返回示例：
```json
{
    "comments": [
        {
            "_id": "59b7ddfdd822483251569709",
            "content": "＃希望＃+《超级包裹》出番外感觉叶小雷最后成为黑帝之后应该还有没完成的事，希望沉默不是低调能把写个番外或者续集",
            "author": {
                "_id": "55435746298389ad01e402a5",
                "avatar": "/avatar/15/a8/15a8c8b41bc9ccedbdc06d14de944292",
                "nickname": "Psxoh或许已忘记",
                "activityAvatar": "",
                "type": "normal",
                "lv": 8,
                "gender": "male"
            },
            "floor": 2434,
            "likeCount": 0,
            "created": "2017-09-12T13:15:41.425Z",
            "replyTo": null
        }...
    ],
    "ok": true
}
```


---

### 获取书评区帖子列表

 请求URL：
```
http://api.zhuishushenqi.com/post/review
```

 示例：
###   精品、玄幻奇幻、默认排序
[http://api.zhuishushenqi.com/post/review?duration=all&sort=updated&type=xhqh&start=0&limit=20&distillate=true](http://api.zhuishushenqi.com/post/review?duration=all&sort=updated&type=xhqh&start=0&limit=20&distillate=true)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|duration      |Y       |string   | all |
|sort      |Y       |string   | updated(默认排序) created(最新发布) helpful(最有用的) comment-count(最多评论) |
|type      |Y       |string   |  all(全部类型)、xhqh(玄幻奇幻)、dsyn(都市异能)... |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-20 |
|distillate      |Y       |string   | true(精品) 、空字符（全部） |

 返回示例：
```json
{
    "reviews": [
        {
            "_id": "59a7b98e48a3b73d6ea55e25",
            "book": {
                "_id": "50ac662fde1233e062000001",
                "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F23794%2F_23794_790294.jpg%2F",
                "title": "问镜",
                "site": "zhuishuvip",
                "type": "xhqh",
                "latelyFollower": null,
                "retentionRatio": null
            },
            "helpful": {
                "total": 20,
                "yes": 22,
                "no": 2
            },
            "likeCount": 4,
            "haveImage": false,
            "state": "distillate",
            "updated": "2017-09-12T07:40:16.298Z",
            "created": "2017-08-31T07:23:58.843Z",
            "title": "关于仙侠，随便谈谈"
        }...
    ],
    "ok": true
}
```


---

### 获取书评区帖子详情

 请求URL：

```
http://api.zhuishushenqi.com/post/review/{bookReviewId}
```

 示例：

[http://api.zhuishushenqi.com/post/review/59a7b98e48a3b73d6ea55e25](http://api.zhuishushenqi.com/post/review/59a7b98e48a3b73d6ea55e25)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|bookReviewId      |Y       |string   | bookReviewId->_id 帖子的id |

 返回示例：
```json
{
    "review": {
        "_id": "59a7b98e48a3b73d6ea55e25",
        "rating": 4,
        "type": "review",
        "book": {
            "_id": "50ac662fde1233e062000001",
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F23794%2F_23794_790294.jpg%2F",
            "title": "问镜",
            "id": "50ac662fde1233e062000001",
            "latelyFollower": null,
            "retentionRatio": null
        },
        "author": {
            "_id": "569f912ed40269362795ed9e",
            "avatar": "/avatar/4b/76/4b76378e01b9cffda17e1b34378b7d31",
            "nickname": "脱缰的哈士奇",
            "activityAvatar": "/activities/20170120/5.jpg",
            "type": "normal",
            "lv": 8,
            "gender": "male",
            "rank": null,
            "created": "2016-01-20T13:52:46.000Z",
            "id": "569f912ed40269362795ed9e"
        },
        "helpful": {
            "total": 20,
            "yes": 22,
            "no": 2
        },
        "state": "distillate",
        "updated": "2017-09-12T07:40:16.298Z",
        "created": "2017-08-31T07:23:58.843Z",
        "commentCount": 18,
        "content": "先说《问镜》，本书延续《幽冥仙途》（以下简称幽）的某些特点，世界恢弘，布局精妙又不失大气，文字古色古香，行文间自有一番韵味，随主角的成长作者逐步为我们揭开了一片波澜壮阔的天地，虽以主角为切入视觉，总体上却是多线同时进行，当线与线交汇矛盾激化时迸发出的冲击感就显得格外强烈，私以为作者还是最擅长人物刻画，尤擅人心（这点之后再谈），往往寥寥几笔一人便跃然纸上，性格鲜明在很多书里往往只是一个标签，在网文里能做到这点并不容易，如果你将两人性格互换相较其言行依旧合理，那便是不鲜明的代表了，关于《问镜》这里举两点例子:陆沉，全书未曾正面出现一次，然而几次借他人之口勾勒出一位行事无忌，豪情万丈的大能;湛水澄，不据小节而古灵精怪的一只“猫”，登场方式别具一格，让人印象深刻，这两位花费笔墨都不多，但是人物性格都可说展现得淋漓尽致，其余重要配角等自不必说。\n        再说说和《幽》的不同之处，最明显的一点，本文着重写设定，即世界观的构架，以仙侠之基修出了一个圆融自洽的内核，其中还夹杂着一些乱七八糟(深奥莫测？)的思辨，好吧确实有点别扭，而《幽》着重写人心，李珣的心路历程，其中的奇诡变化只有读过之人才能体会，减肥专家描绘时常化虚为实，将人心鬼蜮刻画得入木三分，当初读《幽》时正读高中，每两个礼拜回家读一点，断断续续看了许久，因为一些事情压力很大，看得也很累，但读完之时宛若一个溺水之人浮上水面，有一种异样的酣畅之感，对我来说算是一段特殊的经历，也算是本人最喜欢的一本网文，扯远了；第二点，虽然两本书的主角都求长生，但鱼刺贯而始终的是一股豪气，算是正面的感情，这在书里的其他方面也有体现，如羽清玄，如剑修，而李珣心里充塞的，应算是某种意义上的心魔，在这点上《亵渎》虽然整书的风格上相近于《幽》的压抑，罗格内心却应与鱼刺更贴近；第三点，可能与发表方式不同有关(《幽》是实体书出版有字数限制)，神主写得兴起时就有点收不住，其中还夹杂大量不明觉厉的设定，导致某些情节显得冗长，特别是高潮时过于拖延会使人感觉后气不足，有碍于阅读体验，当然冗长并不等于废话连篇，比起某些作者的强行灌水还是要良心的；第四点，神主本人也说过《幽》的布局都是贯穿全篇的，《问镜》是通过一个个小布局逐步展开，感觉并无孰优孰劣；第五点，《问镜》里时常冒出一些现代感十足的词汇，减肥专家在写《幽》时貌似是没这个习惯的，有好处也有坏处，作为一本以设定为卖点的书，这些词更有利于读者理解，而坏处很明显，特别出戏，最后提一句，《问镜》里多了许多玩笑话，格调虽是不高，嵌入也略显生硬，读来仍让人莞尔。就我个人来说还是喜欢《幽》多过于《问镜》。\n        《尘缘》，一直拿来和《幽》比较，文笔上各有风格，《幽》阴暗奇诡，初读可能略显晦涩，习惯之后别有一般滋味，可谓剑走偏锋，独辟蹊径，《尘缘》缥缈隽永，对烟男的文笔还是没话说的（不得不说他的书一本不如一本，层次分明得很，难得文笔一贯保持），人物感觉《幽》更胜一筹，我读《幽》先于《尘缘》，但如今有印象的《尘缘》中远少于《幽》，顾清为一大亮点增色不少，情节方面，个人以为一部完成度撑死百分之七十的书与《幽》是没有可比性的，而作为《尘缘》全书核心的楔子在后文中亦没有交代清楚也算一大败笔，总体上《尘缘》劣于《幽》，与《问镜》伯仲之间，就这样。\n        顺便提一下《搜神记》，这本书差不多是和《幽》同一时期读的，是高中舍友以前在地摊上买的那种很老的厚得一匹的盗版书，还是不全的，最后网上补完（高中时在学校没啥娱乐，就到处借书看，有点饥不择食，记得当时还看了不少三流言情小说，现在回想起来真是辣眼睛），看完深感名不副实，除了大段华丽而空洞的环境描写几乎没留下啥别的印象，有匠气过重之嫌，作者想将神话融进传统武侠中，却是画虎不成反类犬，既没让背景显得宏大也失去了武侠的江湖味儿，踩在金老先生的肩上依旧矮了人家何止一截。至于感情戏，原谅我真的对要死要活，感天动地的琼瑶式爱情没感觉，而且这书实在是没啥内涵，表面华丽，内里干瘪，哪怕是以言情出名的《诛仙》还有一句“天地不仁，以万物为刍狗”的口号，好像《搜神记》被我吐槽得有点一无是处，但好歹是树下野狐对仙侠（当时可能连这个概念都没有，确实是早）的某种开拓意义的尝试，只是在绝大多数人眼里他是成功的英雄，而我觉得他是个“烈士”。\n        神主曾在求票时说起有人问他《问镜》算不算凡人流，这是自嘲？忘语是个有想法的人，《凡人修仙传》也确是出名，但真正把凡人流发扬光大的却是耳根，以爽文的方式，讲真，凡人流已和仙侠两个字没啥关系了，既不仙，也无侠，基本上是对大刘的黑暗森林法则模仿了个瓜瓢子（这里只是打个比喻，不是说忘语抄袭《三体》），忘语也算是对冷酷无情类主角的流行起了一个助推的作用，刚入坑的新人普遍喜欢这类的，别问我怎么知道的，《凡人》里韩老魔一步一个脚印可谓迈得无比扎实，从不跳级，不乱开金手指，很合理，太合理了，和玩游戏似的，以至于显得僵硬死板，毫无灵性，这点甚至比不上模仿者《仙逆》(《凡人》总体上还是比《仙逆》强的，虽然我不喜欢它)，当初还是小白的时候《仙逆》好是把我迷了一段时间，同样的还有《神墓》，可是我口味越养越叼，他们却越写越，咳咳。忘语算是处在一个比较尴尬的位置，比上不足比下有余，然而他下面的人赚的还比他多，果然要挣钱还是要爽文，现在很多作者都因此转型了，唉。\n        说到仙侠不得不谈下徐公子，很难想象写出《神游》这样书的人是个证券分析师，出于凡俗之间却不带一丝烟火气，他笔下的世界真实又缥缈，一幅人世间的仙家气象，没有浑厚的积累不足以为之，仿佛山水泼墨画，意境深远，但对于意境的过度重视导致除了着重描摹的风君子其他人物都沦为远方的背景，难以留下深刻的印象（也许这就是作者的目的？），而飘逸的仙气也冲淡了情节的转折，当然作为一本满是私货的书如果你能接受足以掩盖住这些缺点，不是很感冒的如我就是另外一回事了，通过风君子的超脱可以看出作者内心的骄傲，以至于其给出私货的方式都是高高在上的说教形式，让人心里难以舒坦，这里同样以私货闻名的教主做得就比他好很多（对于私货的内容同样不是怎么感冒，可能是因为我本身就是个俗人），徐公子的书对于某些读者来说应是十成十仙草。给我同样感受的还有《仙葫》，说来惭愧，我没有读完，也许是少年人心性，对于情节平淡的书缺乏阅读动力。\n        最后说句题外话，同一作者的书之间往往有一些相似点，比如老猫的主角基本都是隐藏的太子党，烟男的书总会有一个楔子，当然并不是每本书的楔子都有用，而神主就比较有意思了，他的书里往往有人头顶绿光，手动滑稽。\n\nPS：写得比较乱，评价也未必中肯，纯属个人观点\n\nPSS:本人读得书少，算是半个文盲，喷子别和文盲一般计较",
        "title": "关于仙侠，随便谈谈",
        "shareLink": "http://share.zhuishushenqi.com/post/59a7b98e48a3b73d6ea55e25",
        "id": "59a7b98e48a3b73d6ea55e25"
    },
    "ok": true
}
```


---

### 获取书评区、书荒区帖子详情内的评论列表

 请求URL：
```
http://api.zhuishushenqi.com/post/review/{bookReviewId}/comment
```

 示例：
[http://api.zhuishushenqi.com/post/review/59a7b98e48a3b73d6ea55e25/comment?start=0&limit=30](http://api.zhuishushenqi.com/post/review/59a7b98e48a3b73d6ea55e25/comment?start=0&limit=30)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|bookReviewId      |Y       |string   | bookReviewId->_id 帖子的id |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-30 |

 返回示例：
```json
{
    "comments": [
        {
            "_id": "59b78f607b3522c8163b2cd2",
            "content": "仙逆我是真的看到400章看不下去了，虽然它很有名，",
            "author": {
                "_id": "545239b7e2f91081741adae1",
                "avatar": "/avatar/69/97/699742e197a041981d2627ad03648b08",
                "nickname": "十二月的萧邦ゼ",
                "activityAvatar": "",
                "type": "normal",
                "lv": 8,
                "gender": "male"
            },
            "floor": 18,
            "replyAuthor": null,
            "likeCount": 0,
            "created": "2017-09-12T07:40:16.263Z",
            "replyTo": null
        }...
    ],
    "ok": true
}
```


---
### 获取书荒区帖子列表

 请求URL：
```
http://api.zhuishushenqi.com/post/help
```

 示例：
**精品、默认排序**

[http://api.zhuishushenqi.com/post/help?duration=all&sort=updated&start=0&limit=20&distillate=true](http://api.zhuishushenqi.com/post/help?duration=all&sort=updated&start=0&limit=20&distillate=true)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|duration      |Y       |string   | all |
|sort      |Y       |string   | updated(默认排序) created(最新发布) comment-count(最多评论) |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-30 |
|distillate      |Y       |string   | true(精品) 、空字符（全部） |

 返回示例：

```json
{
    "helps": [
        {
            "_id": "59ad0c510682e12f518c2b89",
            "author": {
                "_id": "581ac04dce4c6fe105ce767c",
                "avatar": "/avatar/4a/50/4a50aeee8ea934532fcc7ecfdd81d9ff",
                "nickname": "追书家的Benny",
                "activityAvatar": "/activities/20170120/5.jpg",
                "type": "official",
                "lv": 8,
                "gender": "female"
            },
            "likeCount": 3824,
            "haveImage": false,
            "state": "distillate",
            "updated": "2017-09-12T11:39:51.367Z",
            "created": "2017-09-04T08:18:25.285Z",
            "commentCount": 14246,
            "title": "【追书读书会】第十期：9月开学季，让我们一起玩嗨社区！！！"
        }...
    ],
    "ok": true
}
```


---


### 获取书荒区帖子详情

 请求URL：

```
http://api.zhuishushenqi.com/post/help/{helpId}
```

 示例：

[http://api.zhuishushenqi.com/post/help/59ad0c510682e12f518c2b89](http://api.zhuishushenqi.com/post/help/59ad0c510682e12f518c2b89)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|helpId      |Y       |string   | helpId->_id 帖子的id |

 返回示例：

```json
{
    "help": {
        "_id": "59ad0c510682e12f518c2b89",
        "author": {
            "_id": "581ac04dce4c6fe105ce767c",
            "avatar": "/avatar/4a/50/4a50aeee8ea934532fcc7ecfdd81d9ff",
            "nickname": "追书家的Benny",
            "activityAvatar": "/activities/20170120/5.jpg",
            "type": "official",
            "lv": 8,
            "gender": "female",
            "rank": null,
            "created": "2016-11-03T04:42:53.000Z",
            "id": "581ac04dce4c6fe105ce767c"
        },
        "type": "normal",
        "state": "distillate",
        "updated": "2017-09-12T11:39:51.367Z",
        "created": "2017-09-04T08:18:25.285Z",
        "commentCount": 14246,
        "content": "暑假悄然无声的结束，新的学期也接踵而来；也许刚结束的假期没能让你玩的happy，那么开学社区继续陪你玩；\r\n\r\n《不管你是老书虫，还是小萌新；只要你够活跃你够努力，你就是那个获奖者！》\r\n\r\n【本期要求】\r\n《「晒出你认为的粮草」在书评区或者书荒区，晒出你心里理想的书》\r\n\r\n▶▶▶参与方式：\r\n\r\n一：《发表书评（预计5分钟，奖大）》\r\n1,在『社区』-『精彩书评』专区发布书评\r\n2,标题带有【读书会】标签，字数≥50，不可水，即可参与\r\n人气书评奖：3000书劵 + 《永久书评人勋章 + 追书神秘福袋1名》（“有用”值最高）；\r\n参与奖：666书劵+30天免广告，15名 （优选合格书评）；\r\n努力奖：《原创书评≥1000字，你将会获得1000书券》；\r\n\r\n二：《发书单贴（预计20分钟，奖大，竞争少） 》；\r\n1,在『社区』-『书荒互助』专区按以下格式发布书单贴即可参与；\r\n2,书单贴里的推荐书籍须≥5本，每本书的短评字数≥30字；\r\n标题：【读书会-XXX】______________\r\n❤《福利来了~~》\r\n点同感并在本帖回复前500名，可以获得30追书券（本福利在9月30日系统统一发放）\r\n\r\n❤开学季：9月社区活动依然待你如初恋，点击『社区』—『活动福利』，这里有史上最全的活动汇总，如果想获得书券就请到这里来，也可以关注『官方V』,下面是官方V活动传现场；\r\n[[post:599ab84d4fde17027f045e5a  【9月福利】书籍区有券参与活动，期待你的到来！！！]]",
        "title": "【追书读书会】第十期：9月开学季，让我们一起玩嗨社区！！！",
        "shareLink": "http://share.zhuishushenqi.com/post/59ad0c510682e12f518c2b89",
        "id": "59ad0c510682e12f518c2b89"
    },
    "ok": true
}
```


---

### 第三方登陆

 请求URL：
```
http://api.zhuishushenqi.com/user/login
```

 示例：
[http://api.zhuishushenqi.com/user/login](http://api.zhuishushenqi.com/user/login)

 请求方式：`POST`


 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|platform_uid      |Y       |string   |  |
|platform_token      |Y       |string   |  |
|platform_code      |Y       |string   |  |

 返回示例：
```json
{
    "ok": true
}
```


---


### 获取作者粉丝相关信息

 请求URL：
```
http://api.zhuishushenqi.com/user/followings/{userid}
```

 示例：
[http://api.zhuishushenqi.com/user/followings/xxx](http://api.zhuishushenqi.com/user/followings/xxx)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|userid      |Y       |string   | 用户id |

 返回示例：

```json
{
    "ok": true
}
```


---


### 获取书籍讨论列表

 请求URL：

```
http://api.zhuishushenqi.com/post/by-book
```

 示例：

###   精品、玄幻奇幻、默认排序
[http://api.zhuishushenqi.com/post/by-book?book=5816b415b06d1d32157790b1&sort=updated&type=normal&start=0&limit=20](http://api.zhuishushenqi.com/post/by-book?book=5816b415b06d1d32157790b1&sort=updated&type=normal&start=0&limit=20)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|book      |Y       |string   | bookId |
|sort      |Y       |string   | updated(默认排序) created(最新发布) comment-count(最高热度) |
|type      |Y       |string   |  normal vote |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-20 |


 返回示例：

```json
{
    "posts": [
        {
            "_id": "59b0f120930ffa032c9176d4",
            "author": {
                "_id": "5559b73846fb7ff0496ccc97",
                "avatar": "/avatar/e9/0d/e90d9e4bbd80560961a2f9b043025f2d",
                "nickname": "追书家的小姝姝",
                "activityAvatar": "/activities/20170120/3.jpg",
                "type": "official",
                "lv": 6,
                "gender": "female"
            },
            "type": "normal",
            "likeCount": 197,
            "block": "ramble",
            "haveImage": true,
            "state": "normal",
            "updated": "2017-09-12T13:38:20.752Z",
            "created": "2017-09-07T07:11:28.602Z",
            "commentCount": 751,
            "voteCount": 0,
            "title": "舞长空形象大比拼，漫画与游戏中的他谁更帅"
        }...
    ],
    "ok": true
}
```


---

### 获取书籍书评列表

 请求URL：
```
http://api.zhuishushenqi.com/post/review/by-book
```

 示例：
[http://api.zhuishushenqi.com/post/review/by-book?book=5816b415b06d1d32157790b1&sort=updated&start=0&limit=20](http://api.zhuishushenqi.com/post/review/by-book?book=5816b415b06d1d32157790b1&sort=updated&start=0&limit=20)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|book      |Y       |string   | bookId |
|sort      |Y       |string   | updated(默认排序) created(最新发布) helpful(最有用的) comment-count(最高热度) |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-20 |

 返回示例：
```json
{
    "total": 2727,
    "reviews": [
        {
            "_id": "581b3700be9018985f28e6de",
            "rating": 5,
            "author": {
                "_id": "570a6d6d641a4b1d7b93efd1",
                "avatar": "/avatar/2a/37/2a37cbbf61d3c61313dfd59a147f14e5",
                "nickname": "羽",
                "activityAvatar": "",
                "type": "normal",
                "lv": 8,
                "gender": "male"
            },
            "helpful": {
                "total": 18057,
                "yes": 18780,
                "no": 723
            },
            "likeCount": 1019,
            "state": "normal",
            "updated": "2017-09-12T13:39:59.263Z",
            "created": "2016-11-03T13:09:20.553Z",
            "commentCount": 2983,
            "content": "东哥写书名套路满满的，恋爱时期书名为不死不灭，迈入婚姻殿堂（坟墓）时书名为神墓。生孩子时，便写下了长生界。因为婚后东嫂一手遮天，所以有了遮天，等到孩子生下后发现世界完美了，便有了完美世界，如今运动过度肾虚了，圣墟就出来了。（辰东：“媳妇求放过！😭”）",
            "title": "东哥真会玩"
        }...
    ],
    "ok": true
}
```


---


### 获取综合讨论列表

 请求URL：
```
http://api.zhuishushenqi.com/post/original
```

 示例：
[http://api.zhuishushenqi.com/post/original?book=5816b415b06d1d32157790b1&sort=updated&start=0&limit=20&duration=all&type=all&distillate=](http://api.zhuishushenqi.com/post/original?book=5816b415b06d1d32157790b1&sort=updated&start=0&limit=20&duration=all&type=all&distillate=)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|block      |Y       |string   |  |
|duration      |Y       |string   | all |
|sort      |Y       |string   | updated(默认排序) created(最新发布) helpful(最有用的) comment-count(最多评论) |
|type      |Y       |string   |  all(全部类型)、xhqh(玄幻奇幻)、dsyn(都市异能)... |
|start      |Y       |string   | 评论位置-0 |
|limit      |Y       |string   | 页大小-20 |
|distillate      |Y       |string   | true(精品) 、空字符（全部） |


 返回示例：
```json
{
    "total": 2727,
    "reviews": [
        {
            "_id": "581b3700be9018985f28e6de",
            "rating": 5,
            "author": {
                "_id": "570a6d6d641a4b1d7b93efd1",
                "avatar": "/avatar/2a/37/2a37cbbf61d3c61313dfd59a147f14e5",
                "nickname": "羽",
                "activityAvatar": "",
                "type": "normal",
                "lv": 8,
                "gender": "male"
            },
            "helpful": {
                "total": 18057,
                "yes": 18780,
                "no": 723
            },
            "likeCount": 1019,
            "state": "normal",
            "updated": "2017-09-12T13:39:59.263Z",
            "created": "2016-11-03T13:09:20.553Z",
            "commentCount": 2983,
            "content": "东哥写书名套路满满的，恋爱时期书名为不死不灭，迈入婚姻殿堂（坟墓）时书名为神墓。生孩子时，便写下了长生界。因为婚后东嫂一手遮天，所以有了遮天，等到孩子生下后发现世界完美了，便有了完美世界，如今运动过度肾虚了，圣墟就出来了。（辰东：“媳妇求放过！😭”）",
            "title": "东哥真会玩"
        }...
    ],
    "ok": true
}
```


---



### 获取搜索热词

 请求URL：
```
http://api.zhuishushenqi.com/book/search-hotwords
```

 示例：
[http://api.zhuishushenqi.com/book/search-hotwords](http://api.zhuishushenqi.com/book/search-hotwords)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| 无      |无      |无   | 无 |


 返回示例：
```json
{
    "searchHotWords": [
        {
            "word": "全职高手",
            "times": 116,
            "isNew": 0,
            "soaring": 2
        },
        {
            "word": "上门狂婿",
            "times": 80,
            "isNew": 0,
            "soaring": 2
        },
        {
            "word": "斗罗大陆",
            "times": 79,
            "isNew": 0,
            "soaring": -2
        }
        ...
    ],
    "ok": true
}
```

---


### 搜索自动补充

 请求URL：
```
http://api.zhuishushenqi.com/book/auto-complete
```

 示例：
[http://api.zhuishushenqi.com/book/auto-complete?query=斗罗](http://api.zhuishushenqi.com/book/auto-complete?query=斗罗)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| query      |Y      |string   | 待补充的关键词 |


 返回示例：
```json
{
    "keywords": [
        "斗罗大陆",
        "斗罗大陆之王者归来",
        "斗罗大陆之七怪成神之路",
        "斗罗大陆之七绝",
        "斗罗大陆前传",
        "斗罗大陆之再踏巅峰",
        "斗罗大陆之秩序神传",
        "斗罗大陆之武魂极限",
        "斗罗大陆之黄金圣龙",
        "斗罗强少在学院"
    ],
    "ok": true
}
```

---


### 模糊搜索书籍

 请求URL：
```
http://api.zhuishushenqi.com/book/fuzzy-search
```

 示例：
[http://api.zhuishushenqi.com/book/fuzzy-search?query=斗破苍穹&start=1&limit=20](http://api.zhuishushenqi.com/book/fuzzy-search?query=斗破苍穹&start=1&limit=20)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| query      |Y       |string   | 搜索关键字 |
| start      |Y       |int   | 开始位置（从1开始） |
| limit      |Y       |int   |每页条数|


 返回示例：
```json
{
    "books": [
        {
            "_id": "54bb7cf5dc0b372756005509",
            "hasCp": true,
            "title": "斗破苍穹之破帝成神",
            "aliases": "",
            "cat": "玄幻",
            "author": "夜晚的晨风",
            "site": "zhuishuvip",
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F2033313%2F2033313_e6745e80b68b4f4c822b769cd5cd659f.jpg%2F",
            "shortIntro": "眨眼间，数百年的时光悄然而过，曾今那个彻响中州大陆无人不知无人不晓的男人离开了这里，拼尽了全力保全了大陆，虽然他离开了这里，但是这么多年过去了，人们仍然无法忘记他，只因为，他是炎帝萧炎。没错，心没冷，血还热，战斗又怎会停止？",
            "lastChapter": "第三十五章  交锋",
            "retentionRatio": 18.31,
            "banned": 0,
            "allowMonthly": false,
            "latelyFollower": 1013,
            "wordCount": 128755,
            "contentType": "txt",
            "superscript": "",
            "sizetype": 0,
            "highlight": {
                "title": [
                    "斗",
                    "破",
                    "苍",
                    "穹"
                ]
            }
        }
    ],
    "total": 103,
    "ok": true
}
```
---


### 书籍详情

 请求URL：
```
http://api.zhuishushenqi.com/book/{bookid}
```

 示例：
[http://api.zhuishushenqi.com/book/5816b415b06d1d32157790b1](http://api.zhuishushenqi.com/book/5816b415b06d1d32157790b1)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|bookid      |Y       |string   |书籍id  |


 返回示例：
```json
{
    "_id": "5816b415b06d1d32157790b1",
    "title": "圣墟",
    "author": "辰东",
    "longIntro": "在破败中崛起，在寂灭中复苏。沧海成尘，雷电枯竭，那一缕幽雾又一次临近大地，世间的枷锁被打开了，一个全新的世界就此揭开神秘的一角……",
    "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F1228859%2F_1228859_441552.jpg%2F",
    "majorCate": "玄幻",
    "minorCate": "东方玄幻",
    "creater": "iPhone 5s (UK+Europe+Asis+China)",
    "rating": {
        "count": 17432,
        "score": 8.686,
        "isEffect": true
    },
    "sizetype": -1,
    "superscript": "",
    "currency": 0,
    "contentType": "txt",
    "_le": false,
    "allowMonthly": false,
    "allowVoucher": true,
    "allowBeanVoucher": false,
    "hasCp": true,
    "postCount": 49851,
    "latelyFollower": 293174,
    "followerCount": 0,
    "wordCount": 2748484,
    "serializeWordCount": 8232,
    "retentionRatio": "71.08",
    "updated": "2017-10-25T12:28:56.605Z",
    "isSerial": true,
    "chaptersCount": 716,
    "lastChapter": "第716章 严肃表态负责",
    "gender": [
        "male"
    ],
    "tags": [
        "玄幻",
        "东方玄幻"
    ],
    "cat": "东方玄幻",
    "donate": false,
    "copyright": "阅文集团正版授权",
    "_gg": false,
    "discount": null
}
```


---

### 获取小说源（正版）

 请求URL：
```
http://api.zhuishushenqi.com/btoc
```

 示例：
[http://api.zhuishushenqi.com/btoc?book=54bb7cf5dc0b372756005509&view=summary](http://api.zhuishushenqi.com/btoc?book=54bb7cf5dc0b372756005509&view=summary)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| book      |Y       |string   | 书籍ID |
| view      |Y       |string   | 固定值 |


 返回示例：
```json
[
    {
        "_id": "5982d0baa047e3f0682c86e8",
        "name": "优质书源",
        "lastChapter": "第三十五章  交锋",
        "source": "zhuishuvip",
        "link": "http://vip.zhuishushenqi.com/toc/5982d0baa047e3f0682c86e8",
        "isCharge": false,
        "chaptersCount": 36,
        "updated": "2018-10-08T08:22:34.276Z",
        "starting": true,
        "host": "vip.zhuishushenqi.com"
    }
]
```

---



### 书籍章节列表（正版）

 请求URL：
```
http://api.zhuishushenqi.com/atoc/{sourceid}?view=chapters
```

 示例：
[http://api.zhuishushenqi.com/atoc/595ce4a9d6da39c156adc97f?view=chapters](http://api.zhuishushenqi.com/atoc/595ce4a9d6da39c156adc97f?view=chapters)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| sourceid      |Y       |string   | 小说源id（此处的ID为接口[27、获取小说源（正版）](#27)返回的`_id`） |
|view|Y|string|固定值|


 返回示例：

```json
{
    "_id": "595ce4a9d6da39c156adc97f",
    "name": "优质书源",
    "source": "zhuishuvip",
    "book": "592fe687c60e3c4926b040ca",
    "link": "http://vip.zhuishushenqi.com/toc/595ce4a9d6da39c156adc97f",
    "chapters": [
        {
            "title": "第一章 惊蛰",
            "link": "http://vip.zhuishushenqi.com/chapter/595ce4a9c9f6f6b3439bfb30?cv=1555034201195",
            "id": "595ce4a9c9f6f6b3439bfb30",
            "time": 0,
            "chapterCover": "",
            "totalpage": 0,
            "partsize": 0,
            "order": 1,
            "currency": 15,
            "unreadble": false,
            "isVip": false
        },
        ...
    ],
    "updated": "2019-08-20T14:03:05.681Z",
    "host": "vip.zhuishushenqi.com"
}
```


---



### 获取小说源（正版、盗版混合）

 请求URL：
```
http://api.zhuishushenqi.com/atoc
```

 示例：
[http://api.zhuishushenqi.com/atoc?view=summary&book=548d9c17eb0337ee6df738f5](http://api.zhuishushenqi.com/atoc?view=summary&book=548d9c17eb0337ee6df738f5)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| book      |Y       |string   | 书籍ID |
| view      |Y       |string   | 固定值`summary ` |


 返回示例：
```json
[
    {
        "_id": "568fef99adb27bfb4b3a58dc",
        "name": "优质书源",
        "lastChapter": "正文 第3926章 一往无前！",
        "source": "zhuishuvip",
        "link": "http://vip.zhuishushenqi.com/toc/568fef99adb27bfb4b3a58dc",
        "isCharge": false,
        "chaptersCount": 3927,
        "updated": "2019-08-23T11:21:49.450Z",
        "starting": true,
        "host": "vip.zhuishushenqi.com"
    },
    {
        "_id": "5cc749c58c59f97450b8a8b1",
        "lastChapter": "正文 第3916章 白凌川！",
        "link": "http://book.xbiquge.com/getBooks.aspx?method=chapterList&bookId=683354",
        "source": "xbiquge",
        "name": "xbiquge",
        "isCharge": false,
        "chaptersCount": 3917,
        "updated": "2019-08-19T17:04:42.809Z",
        "starting": false,
        "host": "book.xbiquge.com"
    }
	...
]
```

---



### 书籍章节列表（正版、盗版混合）

 请求URL：
```
http://api.zhuishushenqi.com/mix-atoc/{bookid}?view=chapters
```

 示例：
[http://api.zhuishushenqi.com/mix-atoc/595ce4a9d6da39c156adc97f?view=chapters](http://api.zhuishushenqi.com/mix-atoc/595ce4a9d6da39c156adc97f?view=chapters)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|bookid      |Y       |string   | 书籍id（此处的ID为接口[29、获取小说源（正版、盗版混合）](#29)返回的`_id`） |
|view|Y|string|固定值`chapters `|


 返回示例：

```json
{
    "_id": "595ce4a9d6da39c156adc97f",
    "name": "优质书源",
    "source": "zhuishuvip",
    "book": "592fe687c60e3c4926b040ca",
    "link": "http://vip.zhuishushenqi.com/toc/595ce4a9d6da39c156adc97f",
    "chapters": [
        {
            "title": "第一章 惊蛰",
            "link": "http://vip.zhuishushenqi.com/chapter/595ce4a9c9f6f6b3439bfb30?cv=1555034201195",
            "id": "595ce4a9c9f6f6b3439bfb30",
            "time": 0,
            "chapterCover": "",
            "totalpage": 0,
            "partsize": 0,
            "order": 1,
            "currency": 15,
            "unreadble": false,
            "isVip": false
        },
        ...
    ],
    "updated": "2019-08-20T14:03:05.681Z",
    "host": "vip.zhuishushenqi.com"
}
```


---


### 章节内容详情

 请求URL：
```
http://chapterup.zhuishushenqi.com/chapter/{link}
```

 示例：
[http://chapterup.zhuishushenqi.com/chapter/http://vip.zhuishushenqi.com/chapter/595ce4a9c9f6f6b3439bfb30?cv=1555034201195](http://chapterup.zhuishushenqi.com/chapter/http://vip.zhuishushenqi.com/chapter/595ce4a9c9f6f6b3439bfb30?cv=1555034201195)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|link      |Y       |string   | 接口[28、书籍章节列表（正版）](#28)中返回的`link` |


 返回示例：

```json
{
    "ok": true,
    "chapter": {
        "title": "第一章 惊蛰",
        "body": "\n\r\n\r\n\r请安装最新版追书 以便使用优质资源",
        "isVip": false,
        "order": 1,
        "currency": 15,
        "id": "595ce4a9c9f6f6b3439bfb30",
        "created": "2017-07-05T13:07:53.680Z",
        "updated": "2019-04-12T01:56:41.195Z",
        "cpContent": "二月二，龙抬头。\r\n暮色里，小镇名叫泥瓶巷的僻静地方，有位孤苦伶仃的清瘦少年，此时他正按照习俗，一手持蜡烛，一手持桃枝，照耀房梁、墙壁、木床等处，用桃枝敲敲打打，试图借此驱赶蛇蝎、蜈蚣等，嘴里念念有词，是这座小镇祖祖辈辈传下来的老话：二月二，烛照梁，桃打墙，人间蛇虫无处藏。\r\n少年姓陈，名平安，爹娘早逝。小镇的瓷器极负盛名，本朝开国以来，就担当起“奉诏监烧献陵祭器”的重任，有朝廷官员常年驻扎此地，监理官窑事务。无依无靠的少年，很早就当起了烧瓷的窑匠，起先只能做些杂事粗活，跟着一个脾气糟糕的半路师傅，辛苦熬了几年，刚刚琢磨到一点烧瓷的门道，结果世事无常，小镇突然失去了官窑造办这张护身符，小镇周边数十座形若卧龙的窑炉，一夜之间全部被官府勒令关闭熄火。\r\n陈平安放下新折的那根桃枝，吹灭蜡烛，走出屋子后，坐在台阶上，仰头望去，星空璀璨。\r\n少年至今仍然清晰记得，那个只肯认自己做半个徒弟的老师傅，姓姚，在去年暮秋时分的清晨，被人发现坐在一张小竹椅子上，正对着窑头方向，闭眼了。\r\n不过如姚老头这般钻牛角尖的人，终究少数。\r\n世世代代都只会烧瓷一事的小镇匠人，既不敢僭越烧制贡品官窑，也不敢将库藏瓷器私自贩卖给百姓，只得纷纷另谋出路，十四岁的陈平安也被扫地出门，回到泥瓶巷后，继续守着这栋早已破败不堪的老宅，差不多是家徒四壁的惨淡场景，便是陈平安想要当败家子，也无从下手。\r\n当了一段时间飘来荡去的孤魂野鬼，少年实在找不到挣钱的营生，靠着那点微薄积蓄，少年勉强填饱肚子，前几天听说几条街外的骑龙巷，来了个姓阮的外乡老铁匠，对外宣称要收七八个打铁的学徒，不给工钱，但管饭，陈平安就赶紧跑去碰运气，不曾想老人只是斜瞥了他一眼，就把他拒之门外，当时陈平安就纳闷，难道打铁这门活计，不是看臂力大小，而是看面相好坏？\r\n要知道陈平安虽然看着孱弱，但力气不容小觑，这是少年那些年烧瓷拉坯锻炼出来的身体底子，除此之外，陈平安还跟着姓姚的老人，跑遍了小镇方圆百里的山山水水，尝遍了四周各种土壤的滋味，任劳任怨，什么脏活累活都愿意做，毫不拖泥带水。可惜老姚始终不喜欢陈平安，嫌弃少年没有悟性，是榆木疙瘩不开窍，远远不如大徒弟刘羡阳，这也怪不得老人偏心，师父领进门，修行在个人，例如同样是枯燥乏味的拉坯，刘羡阳短短半年的功力，就抵得上陈平安辛苦三年的水准。\r\n虽然这辈子都未必用得着这门手艺，但陈平安仍是像以往一般，闭上眼睛，想象自己身前搁置有青石板和轱辘车，开始练习拉坯，熟能生巧。\r\n大概每过一刻钟，少年就会歇息稍许时分，抖抖手腕，如此循环反复，直到整个人彻底精疲力尽，陈平安这才起身，一边在院中散步，一边缓缓舒展筋骨。从来没有人教过陈平安这些，是他自己瞎琢磨出来的门道。\r\n天地间原本万籁寂静，陈平安听到一声刺耳的讥讽笑声，停下脚步，果不其然，看到那个同龄人蹲在墙头上，咧着嘴，毫不掩饰他的鄙夷神色。\r\n此人是陈平安的老邻居，据说更是前任监造大人的私生子，那位大人唯恐清流非议、言官弹劾，最后孤身返回京城述职，把孩子交由颇有私交情谊的接任官员，帮着看管照拂。如今小镇莫名其妙地失去官窑烧制资格，负责替朝廷监理窑务的督造大人，自己都泥菩萨过江自身难保了，哪里还顾得上官场同僚的私生子，丢下一些银钱，就火急火燎赶往京城打点关系。\r\n不知不觉已经沦为弃子的邻居少年，日子倒是依旧过得优哉游哉，成天带着他的贴身丫鬟，在小镇内外逛荡，一年到头游手好闲，也从来不曾为银子发过愁。\r\n泥瓶巷家家户户的黄土院墙都很低矮，其实邻居少年完全不用踮起脚跟，就可以看到这边院子的景象，可每次跟陈平安说话，偏偏喜欢蹲在墙头上。\r\n相比陈平安这个名字的粗浅俗气，邻居少年就要雅致许多，叫宋集薪，就连与他相依为命的婢女，也有个文绉绉的称呼，稚圭。\r\n少女此时就站在院墙那边，她有一双杏眼，怯怯弱弱。\r\n院门那边，有个嗓音响起，“你这婢女卖不卖？”\r\n宋集薪愣了愣，循着声音转头望去，是个眉眼含笑的锦衣少年，站在院外，一张全然陌生的面孔。\r\n锦衣少年身边站着一位身材高大的老者，面容白皙，脸色和蔼，轻轻眯眼打量着两座毗邻院落的少年少女。\r\n老者的视线在陈平安一扫而过，并无停滞，但是在宋集薪和婢女身上，多有停留，笑意渐渐浓郁。\r\n宋集薪斜眼道：“卖！怎么不卖！”\r\n那少年微笑道：“那你说个价。”\r\n少女瞪大眼眸，满脸匪夷所思，像一头惊慌失措的年幼麋鹿。\r\n宋集薪翻了个白眼，伸出一根手指，晃了晃，“白银一万两！”\r\n锦衣少年脸色如常，点头道：“好。”\r\n宋集薪见那少年不像是开玩笑的样子，连忙改口道：“是黄金万两！”\r\n锦衣少年嘴角翘起，道：“逗你玩的。”\r\n宋集薪脸色阴沉。\r\n锦衣少年不再理睬宋集薪，偏移视线，望向陈平安，“今天多亏了你，我才能买到那条鲤鱼，买回去后，我越看越欢喜，想着一定要当面跟你道一声谢，于是就让吴爷爷带我连夜来找你。”\r\n他丢出一只沉甸甸的绣袋，抛给陈平安，笑脸灿烂道：“这是酬谢，你我就算两清了。”\r\n陈平安刚想要说话，锦衣少年已经转身离去。\r\n陈平安皱了皱眉头。\r\n白天自己无意间看到有个中年人，提着只鱼篓走在大街上，捕获了一尾巴掌长短的金黄鲤鱼，它在竹篓里蹦跳得厉害，陈平安只瞥了一眼，就觉得很喜庆，于是开口询问，能不能用十文钱买下它，中年人本来只是想着犒劳犒劳自己的五脏庙，眼见有利可图，就坐地起价，狮子大开口，非要三十文钱才肯卖。囊中羞涩的陈平安哪里有这么多闲钱，又实在舍不得那条金灿灿的鲤鱼，就眼馋跟着中年人，软磨硬泡，想着把价格砍到十五文，哪怕是二十文也行，就在中年人有松口迹象的时候，锦衣少年和高大老人正好路过，他们二话不说，用五十文钱买走了鲤鱼和鱼篓，陈平安只能眼睁睁看着他们扬长而去，无可奈何。\r\n死死盯住那对爷孙愈行愈远的背影，宋集薪收回恶狠狠的眼神后，跳下墙头，似乎记起什么，对陈平安说道：“你还记得正月里的那条四脚吗？”\r\n陈平安点了点头。\r\n怎么会不记得，简直就是记忆犹新。\r\n按照这座小镇传承数百年的风俗，如果有蛇类往自家屋子钻，是好兆头，主人绝对不要将其驱逐打杀。宋集薪在正月初一的时候，坐在门槛上晒太阳，然后就有只俗称四脚蛇的小玩意儿，在他的眼皮子底下往屋里窜，宋集薪一把抓住就往院子里摔出去，不曾想那条已经摔得七荤八素的四脚蛇，愈挫愈勇，一次次，把从来不信鬼神之说的宋集薪给气得不行，一怒之下就把它甩到了陈平安院子，哪里想到，宋集薪第二天就在自己床底下，看到了那条盘踞蜷缩起来的四脚蛇。\r\n宋集薪察觉到少女扯了扯自己袖子。\r\n少年与她心有灵犀，下意识就将已经到了嘴边的话语，重新咽回肚子。\r\n他想说的是，那条奇丑无比的四脚蛇，最近额头上有隆起，如头顶生角。\r\n宋集薪换了一句话说出口，“我和稚圭可能下个月就要离开这里了。”\r\n陈平安叹了口气，“路上小心。”\r\n宋集薪半真半假道：“有些物件我肯定搬不走，你可别趁我家没人，就肆无忌惮地偷东西。”\r\n陈平安摇了摇头。\r\n宋集薪蓦然哈哈大笑，用手指点了点陈平安，嬉皮笑脸道：“胆小如鼠，难怪寒门无贵子，莫说是这辈子贫贱任人欺，说不定下辈子也逃不掉。”\r\n陈平安默不作声。\r\n各自返回屋子，陈平安关上门，躺在坚硬的木板床上，贫寒少年闭上眼睛，小声呢喃道：“碎碎平，岁岁安，碎碎平安，岁岁平安……”\r\n \r\n\r\n"
    }
}
```

---


### 获取小说最新章节

 请求URL：

```
http://api.zhuishushenqi.com/book
```

 示例：

[http://api.zhuishushenqi.com/book?view=updated&id=531169b3173bfacb4904ca67](http://api.zhuishushenqi.com/book?view=updated&id=531169b3173bfacb4904ca67)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| id      |Y      |string   |书籍ID|
| view      |Y      |string   |固定值`updated`|


 返回示例：

```json
[
    {
        "_id": "531169b3173bfacb4904ca67",
        "author": "耳根",
        "isMakeMoneyLimit": false,
        "isFineBook": false,
        "allowMonthly": false,
        "referenceSource": "sogou",
        "updated": "2017-11-24T01:42:04.150Z",
        "chaptersCount": 1609,
        "lastChapter": "第十卷 我看沧海化桑田 第1614章 孤帆一片日边来！（终）"
    }
]

```

---


### 根据某小说Id获取推荐小说

 请求URL：

```
http://api.zhuishushenqi.com/book/{id}/recommend
```

 示例：

[http://api.zhuishushenqi.com/book/531169b3173bfacb4904ca67/recommend](http://api.zhuishushenqi.com/book/531169b3173bfacb4904ca67/recommend)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| id      |Y      |string   |书籍ID|


 返回示例：

```json
{
    "books": [
        {
            "_id": "597b3573628661b94bbd205f",
            "title": "藏锋",
            "author": "他曾是少年",
            "site": "zhuishuvip",
            "cover": "/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F2177015%2F2177015_86dae9882c2145569cff58ef290c5e22.jpg%2F",
            "shortIntro": "太子弑父，天降灾祸饿殍遍野。\r\n乞儿命苦，数九寒冬家破人亡。\r\n是谁说生死有命富贵在天？\r\n是谁说善恶有报因果轮回？\r\n尽是荒唐！\r\n弱肉强食，何来道义！\r\n物竞天择，何来公平！\r\n倒不如杀他个天昏地暗！\r\n倒不如杀他个天下太平！\r\n ",
            "lastChapter": "第五卷 十九 新书发布，请多支持！",
            "retentionRatio": 53.27,
            "latelyFollower": 9132,
            "majorCate": "玄幻",
            "minorCate": "东方玄幻",
            "allowMonthly": true,
            "isSerial": false,
            "contentType": "txt",
            "allowFree": false,
            "otherReadRatio": 77.61
        }
		 ...
    ],
    "ok": true
}
```

---


### 热门搜索

 请求URL：

```
http://api.zhuishushenqi.com/book/hot-word
```

 示例：

[http://api.zhuishushenqi.com/book/hot-word](http://api.zhuishushenqi.com/book/hot-word)

 请求方式：`GET`

 参数类型：

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
| 无      | 无      | 无   | 无 |


 返回示例：

```json
{
    "hotWords": [
        "元后传",
        "都市之最强狂兵",
        ...
    ],
    "newHotWords": [
        {
            "word": "元后传",
            "book": "5d3e83e76c77f36c4a76baa5"
        },
        {
            "word": "都市之最强狂兵",
            "book": "59305ea9eeecff1975986572"
        }
		 ...
    ],
    "ok": true
}

```

---
