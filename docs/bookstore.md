## 前端

前端项目目录结构

```js

```



### 音乐播放器部分

#### 需求分析

![](https://image.yangxiansheng.top/img/20200804204948.png?imagelist)

#### 榜单歌曲列表获取

首先调用服务器上网易云的API获取榜单数据，进入播放器页面进行调用，用解构的方式取出需要的数据，组成一个新对象。最后push到定义的数组里面去

```js
 const {id, name, ar: [{name: singer}], al: {name: album, picUrl}} = item
      this.playMusicItem = {
        id,
        name,
        singer,
        picUrl,
        album,
        index,
        src: `https://music.163.com/song/media/outer/url?id=${id}.mp3`
      }

```



#### 音乐播放器主要功能实现

 **第一步就是用vuex存放数据**,比如**歌曲暂停还是播放**,播放列表数组,当前歌曲,**当前播放模式**等。然后就是开始写业务，**首先在created钩子里面new一个后台音乐播放器实例**(getBackgroundAudioManager)。然后将页面骨架初步写完。**点击模式**时通过computed改变图标，然后调用不同的Action生成不同模式下的歌曲列表,比如随机播放,这个时候我就需要书写一个洗牌算法把里面的歌曲列表打乱，最后再提交修改。

然后最重要的是**监听点击上一首下一首或者播放暂停的时候**先去调用微信的audio暂停播放这些API，然后要去实时修改vuex里面数据，**比如我点击下一首**,这个要做的事: 1.将歌曲当前时间置为0 2.将歌曲在播放列表里面的index+1,然后修改vuex的currentSong,最后是调用微信API封装的播放方法，监听到歌曲能够播放就讲isPlay设为true,调用播放钩子，然后设置一下显示的时间 



洗牌算法

```js
function getRandomInt (min, max) {
  // 取min-max的数据
  return Math.floor(Math.random() * (max - min + 1) + min)
}
export function shuffle (arr) {
  // 当前数组值与取到的随机数组值交换 从而打乱数据
  let _arr = arr.slice()
  for (let i = 0; i < _arr.length; i++) {
    let j = getRandomInt(0, i)
    let t = _arr[i]
    _arr[i] = _arr[j]
    _arr[j] = t
  }
  return _arr
}
```

切换播放模式部分代码

```js
 changeMode () {
      const mode = (this.mode + 1) % 3
      this.setPlayMode(mode)
      let list = null
      if (this.mode === playMode.random) {
        list = shuffle(this.sequencelist)
        setTimeout(() => {
          this.setPlaylist(list)
        }, 300)
      } else {
        list = this.sequencelist
        this.setPlaylist(list)
      }
    }
```





### 阅读器部分

#### 需求分析

![](https://image.yangxiansheng.top/img/QQ截图20200312141124.png?imagelist)



#### **渲染和解析电子书**

首先要访问在`nginx`上存放的`epub`资源,然后通过`epubjs`进行解析渲染

```js
<script>
  //引入epubjs库  
import { mapMutations, mapGetters } from "vuex";
import Epub from "epubjs";
global.ePub = Epub;
export default {
  name: "",
  props: [""],
  data() {
    return {
      Bookfilename: ""
    };
  },
//首次渲染时将参数传递 然后设置vuex数据 之后调用init方法
  mounted() {
    this.Bookfilename = this.$route.params.fileName;
    this.setFileName(this.Bookfilename);
    this.initEpub();
  },

  methods: {
    ...mapGetters(["fileName"]),
    ...mapMutations({
      setFileName: "SET_FILENAME"
    }),
    initEpub() {
      //拼接字符串  
      const url = "https://store.yangxiansheng.top/epub/";
      let BookUrl = url + `${this.Bookfilename}.epub`;
      window.console.log(BookUrl);
      // 解析电子书路径
      this.book = new Epub(BookUrl);
      // 渲染关键钩子 拿到rendition对象
      this.redition = this.book.renderTo("read", {
        //宽高为书籍宽高  
        width: innerWidth,
        height: innerHeight,
        //兼容微信  
        method: "default"
      });
      this.redition.display();
    }
  }
};
```

**使用epubjs解析关键**

> 1. dom上挂载read节点
> 2. 创建epub实例 ，渲染API为`rederTo('dom',attribute)`
> 3. 显示渲染内容  `display()`

#### **设置字号和字体**

<h3>字号</h3>
引入vant-slide帮助快速搭建滑块,监听`@change`事件,设置字号大小阈值为`12`到`24`

```js
 <Slider
              :min="12"
              :max="24"
              bar-height="4px"
              active-color="#5f5f56"
              button-size="15"
              v-model="value"
              inactive-color="#d4d4cf"
              @change="onChange"
            ></Slider>     
```

在监听事件中拿到`value`,改变图书字体大小,关键函数:`this.rendition.themes.fontSize(fontsize)`

```js
onChange(value) {
      this.CurrentBook.rendition.themes.fontSize(value);
      saveFontSize(this.fileName, value);//保存字体大小进入缓存
    }
```

设置字体大小后，发现了一个问题,那就是当我们再次进入阅读器时，之前设置的字体大小重新刷新了,所以我根据此问题引入了缓存`web-storage-cache`

使用该方法书写业务代码

例: 在刚开始加载图书信息时`（this.book.redition.display().then(()=>{})）` 初始化加载

```js
 loadingFontsize() {
      // 取到fontSize
      let fontSize = getFontSize(this.fileName);
      // 没有就写入当前默认的值
      if (!fontSize) {
        fontSize = 16;
        saveFontSize(this.fileName, fontSize);
        this.redition.themes.fontSize(fontSize);
      }
      // 读取到就更改字体大小
      this.redition.themes.fontSize(fontSize);
      saveFontSize(this.fileName, fontSize);
    },
```

改变值的时候也要存入



<h3>字体</h3>
首先根据w3c规则 css3开始可以引入外部样式文件来引入自定义字体文件,所以添加了这个功能。

第一步在阿里巴巴图标库下载字体文件，然后放入自己服务器上通过nginx访问

![](https://image.yangxiansheng.top/img/QQ截图20200314221348.png?imagelist)

第二步 书写设置字体面板组件，这里引入vant-poup组件弹出层，再弹出层里填写内容

同样通过vuex变量来控制弹出层面板显示

![](https://image.yangxiansheng.top/img/QQ截图20200314221551.png?imagelist)



然后就是设置字体了,同样epubjs的钩子要使用到`this.rendition.themes.font()`

注: `defaultFontFamily`:默认字体 `CurrentBook`书籍对象 都是之前初始化设置的vuex全局变量

**初始化注册字体文件**

```js
this.redition.hook.content.register((contents)=>{
    contents.addStylesheet() //添加字体样式文件  
})  //epubjs钩子注册方法 添加样式文件
```

> addStylesheet() 方法必须存入url, 可以将url换成nginx服务器样式文件路径

**切换字体事件**

```js
setfamily(font) {
      // 设置 不同的字体 关键函数 但还需要注册字体文件 使用hook钩子
      this.setfontfamily(font);
      if (this.defaultFontFamily === "Default") {
        this.CurrentBook.rendition.themes.font("Times New Roman");
        saveFontFamily(this.fileName, "Default");
      } else {
        this.CurrentBook.rendition.themes.font(font);
        saveFontFamily(this.fileName, font);
      }
    },
```

这样就完成了字体的切换，这里也需要设置storage初始化，同理。



#### **更换主题**

更换主题这里思路大致这样：

> 通过点击面板选择主题的名字，初始化阅读器时注册主题文件，然后通过动态添加css文件覆盖样式的方式实现主题切换

<h3>注册主题文件

```js
 initTheme() {
      let themelist = themeList();
      let Currenttheme = getTheme(this.fileName);
      if (!Currenttheme) {
          //如果缓存中没有就设置为default的主题
        saveTheme(this.fileName, "Default");
        this.settheme("Default");
        this.redition.themes.select("Default");
      }
      // 注册主题属性
      themelist.forEach(theme => {
        this.redition.themes.register(theme.name, theme.style);
      });
      this.settheme(Currenttheme);
      this.redition.themes.select(Currenttheme);
    },
```

<h3>动态添加样式</h3>
添加css文件方法:创建link的dom，注入属性，然后添加到借点树中

```js
export function addLink(href) {
  const link = document.createElement("link");
  link.setAttribute("rel", "stylesheet");
  link.setAttribute("type", "text/css");
  link.setAttribute("href", href);
  document.getElementsByTagName("head")[0].appendChild(link);
}
```

**发现问题: 点击事件创建了很多css文件**

分析问题:创建css文件我们应该去遍历之前的创建的文件，然后进行删除,写完删除的逻辑之后基本上切换主题就能够实现了。

监听面板点击事件

```js
 setTheme(theme) {
      this.settheme(theme);//vuex设置theme
      this.CurrentBook.rendition.themes.select(theme);//更换主题
      saveTheme(this.fileName, theme);
      this.initGlobaltheme();//初始化主题 动态添加css文件
    },
```

每次点击时，都将之前创建的css文件删除，然后添加点击的主题css文件

```js
 initGlobaltheme() {
      removeAllCss();
      switch (this.defaultTheme) {
        case "Default":
          addLink(`https://store.yangxiansheng.top/theme/theme_default.css`);
          break;
        case "Eye":
          addLink(`https://store.yangxiansheng.top/theme/theme_eye.css`);
          break;
        case "Gold":
          addLink(`https://store.yangxiansheng.top/theme/theme_gold.css`);
          break;
        case "Night":
          addLink(`https://store.yangxiansheng.top/theme/theme_night.css`);
          break;
        default:
          this.saveTheme(this.defaultTheme);
          addLink(`https://store.yangxiansheng.top/theme/theme_default.css`);
          break;
      }
    }
```

这样切换主题功能就实现了。

![](https://image.yangxiansheng.top/img/QQ截图20200314223526.png?imagelist)

#### 切换进度条

切换进度条关键分页算法(简易) 设置750个字符一页,书一行的宽度大于375,那么这也页就大于750个字    `this.book.loctions.generate`拿到页数

```js
this.book.ready(),then(()=>{
    return this.book.locations.generate(750*(window.innerWidth/375)*(getFontsize(this.fileName) / 16))
}).then(()=>{
    this.setProgressFinished(true) //加载完cif的标志设为true
})
```

<h3>
    拖动换章
</h3>

监听滑块的时间中 拿到`cfifromPercentage(vaule/100)`当前进度条内容，然后就display()出页面即可

![](https://image.yangxiansheng.top/img/QQ截图20200315104639.png?imagelist)





<h3>上一章</h3>
定义vuex守卫 `section`，默认为零，通过epub的`this.book.section(vaule).href`获取到章节内容对象,然后进行显示.  

```js
  preveSection(){
      if(this.BookValiable && this.section > 0){  
        this.setSection(this.section - 1).then(()=>{
            // 拿到sectionInfo对象 对象里的href就是对应章节内容
            const sectioninfo = this.Currentbook.section(this.section)
            if(this.section && this.section.href)
            this.CurrentBook.rendition.display(sectioninfo.href)
        })
      }
  }
```

<h3>下一章</h3>
```js
nextSection(){
    // this.Currentbook.spine 对应章节的信息对象
    if(this.BookValiable && this.section < this.Currentbook.spine.length - 1){  
      this.setSection(this.section + 1).then(()=>{
          const sectioninfo = this.Currentbook.section(this.section)
          if(this.section && this.section.href)
          this.CurrentBook.rendition.display(sectioninfo.href)
      })
    }
}
```

#### 目录

<h3>获取图片封面</h3>
`this.book.loaded.cover` `this.book.archive.createUrl`

通过这两个函数获取

```js
this.book.loaded.cover.then((cover)=>{
    this.book.archive.createUrl(cover).then(url=>{
        this.setCover(url)
        console.log(url)
    })
})
```

<h3>获取书籍的基本信息</h3>
`this.book.loaded.metadata.then((meta)=>{})`

```js
metadata.title 标题
metadata.creator 作者
```



<h3>获取目录</h3>
`this.book.`loaded.navigation.then(())

`重点算法`: 将树状的结构数组拆分然后 合并到一个数组

`...[array]`  扩展运算符拆分数组

`[].concat(...[array])` 合并拆分后的数组



拿到的数组结构

```json
[
	 {
         id:1,
         subitems:[
             {
                 id:2,
            	 subitems:[
             				{
             					id:3,subitems:[]
             				},
    						{
                                id:4,subitems:[]
                            }
         					]
             },
             {
                 id:5,
                 subitems:[]
             }
        			 ]
     },
    {
        id:6,
        subitems:[]
    }
]
```

期待拿到的值 

```json
[
    {
    id:1,
    subitems:[{id:2,subitems:[{},{}]},{id:6,subitems:[{},{}]}]
    },
    {
    id:2,
    subitems:[{id:3,subitems:[]},{id:4,subitems:[]}]
    },
    {
    id:3,
    subitems:[]
    },
    {
    id:4,
    subitems:[]
    },
    {
    id:5,
    subitems:[]
    },
    {
    id:6,
    subitems:[]
    },
]
```





```js
function flaten(array){
    // 先遍历数组 然后将一级item 二级item(拆分先)合并 组成新的数组
    return [].concat(array.map(item=>[].concat[item,...item.subitem]))
}

//递归优化 遍历深层树
function flaten(array){
    return [].concat(...arr.map(item=>[].concat(item,...flaten(item.subitem))))
}
```

拿到 目录数组后判断字段`parent` 如果是`undefined`---一级目录



拿到了一维数组的目录结构后，接下来要定义层级结构显示

```js
let nav = flaten(navigation)
function find(item,level = 0){
    if(!item.parent){
        // 一级
        return level
    }else{
        // subitems里面有parent:parentid
        //过滤筛选出 item.id = item.parent 拿到父元素 层级加一
        return find(nav.filter(parentItem => parentItem.id===item.parent)[0],++level)
    }
}
//添加属性 得到层级数组
nav.forEach((item)=>{
    item.level = find(item)
})
```



### epubAPI

```js
初始化epubjs
global.ePub = Epub

解析一本电子书
new Epub(url)
 this.rendition = this.book.renderTo("read", {
        //宽高为书籍宽高  
        width: innerWidth,
        height: innerHeight,
        //兼容微信  
        method: "default"
      });

渲染一本电子书
this.rendition.display()

监听touch事件,控制翻页动作
this.rendition.on('touchstart',e=>{
    
})

拿到手指的触摸位置和触碰时间
touchStartX = e.changeedTouches[0].clientX
time = e.timeStamp

上一页
this.rendition.prev()

下一页
this.rendition.next()

设置字体大小
this.rendition.themes.fontSize(value)

设置字体family (需要注册)
this.renditio.themes.font(fontfamilyName)

注册字体文件
this.rendition.hooks.conetnt.register((contents)=>{
    Promise.all([
        contents.addStylesheet(url)
        ...
    ])
})

注册主题文件 (themelist---提前准备好的themelist)
themelist.forEach(theme =>{
  this.rendition.themes.register(theme.name,theme.style)  
})

设置主题
this.redition.themes.select(theme.name)

粗略分出一本书的总页数(做进度条)
this.book.ready().then(()=>{
    return this.book.locations.generate(rules)
    例：
    return this.book.locations.generate(750*(window.innerWidth / 375) * (getFontsize(this,filename)/16))
    这里 一页的宽度和字体大小决定一页是否超过750字 默认750字一屏
})

获取当前页的位置信息
this.currentBook.rendition.currentLocation()
可以用到的(start.cfi end.cfi ...)

获取cfi(当前页的内容)信息
value: 当前的进度百分比
this.book.locations.cfiFromPercentage(value)，可以直接渲染到页面

通过进度条获取当前页面cfi 页面内容
this.book.locations.percentageFromCfi(percentage)


获取章节信息
section 获取的章节数
sectionInfo = this.book.section(section)
sectionInfo.href  章节内容

上一章下一章 
sectionInfo = this.book.section(section) | section-1|section + 1
显示切换后的章节内容 （跳到指定章节）
this.book.rendition.display(sectionInfo.href)

获取书籍章节信息
this.book.spine (length ...等信息)

获取当前章节信息
this,book.navigation.get(sectionInfo.href)

获取当前章节名称
this,book.navigation.get(sectionInfo.href).label

获取封面
this.book.loaded.cover
this.book.archive.createUrl(cover=>{})
this.setCover(url)

this.book.loaded.cover.then((cover)=>{
    this.book.archive.createUrl(cover).then(url=>{
        this.setCover(url)
        console.log(url)
    })
})
```



## 后端

### 后端部署文档

#### 上传资源文件到服务器上,并利用nginx访问index目录

![](https://image.yangxiansheng.top/img/QQ截图20200311212743.png?imagelist)

配置nginx服务器访问目录文件

```bash

server
{
	listen 80;
    server_name store.yangxiansheng.top;
    root /www/server/nginx/upload;
    autoindex on;
    add_header Cache-Control "no-cache,must-revalidate";
    location / {
    ## 解决跨域问题
    
    add_header Access-Control-Allow-Origin *;
    }
}
```
配置完成后可以通过http://store.yangxiansheng.top访问文件根目录

####  部署后端代码

 1. app.js上修改 数据库相关信息

![](https://image.yangxiansheng.top/img/QQ截图20200311213354.png?imagelist)
 2. 修改const.js

![](https://image.yangxiansheng.top/img/QQ截图20200311213434.png?imagelist)

3.启动服务 node app.js 或者pm2 start app.js

##  接口文档

###  首页数据

**必选参数** : 无

**接口地址 :** `/book/home`

**调用例子 :**  [https://book.yangxiansheng.top/book/home](https://book.yangxiansheng.top/book/home)


###  首页数据

**必选参数** : 无

**接口地址 :** `/book/home`

**调用例子 :**  [https://book.yangxiansheng.top/book/home](https://book.yangxiansheng.top/book/home)

**返回数据:** 
      
```markdown
        guessYouLike --- 猜你喜欢
        banner       --- 导航
        recommend    --- 推荐
        featured     --- 精选
        categoryList --- 几个分类下的图书列表
        categories   --- 分类列表
        random       --- 随机一本图书
```

![](https://image.yangxiansheng.top/img/QQ截图20200311230928.png?imagelist)

###  图书全部分类下的全部书籍列表

**必选参数** : 无

**接口地址 :** `/book/list`

**调用例子 :**  [https://book.yangxiansheng.top/book/list](https://book.yangxiansheng.top/book/list)

**返回数据:**  每个分类下的所有书籍列表

![](https://image.yangxiansheng.top/img/QQ截图20200311231137.png?imagelist)


###  图书详情

**接口地址 :** `/book/detail`

**请求参数 :** `fileName`

**调用例子 :**  [https://book.yangxiansheng.top/book/detail?fileName=2015_Book_TheImpactOfFoodBioactivesOnHea](https://book.yangxiansheng.top/book/detail?fileName=2015_Book_TheImpactOfFoodBioactivesOnHea)

**返回数据:**  每个分类下的所有书籍列表

![](https://image.yangxiansheng.top/img/QQ截图20200311231640.png?imagelist)

###  所有图书

**接口地址 :** `/book/flat-list`

**请求参数 :** 无

**调用例子 :**  [https://book.yangxiansheng.top/book/flat-list](https://book.yangxiansheng.top/book/flat-list)

**返回数据:**  所有图书信息

![](https://image.yangxiansheng.top/img/QQ截图20200311231920.png?imagelist)

## nginx书籍地址

[https://store.yangxiansheng.top](https://store.yangxiansheng.top)





## 播放器组件

### 获取播放列表

### 将播放列表封装成一个规范的数组

### 点击事件触发vuex的action播放歌曲

  // *todo:1.控制面板的显示与隐藏 2.设置显示字号设置时面板阴影消失 3.点击隐藏时设置num为-1 4.混入minx使用vuex 5.this.book写入vuex中 6.填写fontsize数组 ,实现字号更换功能，默认字体大小写入vuex 7 .更改vuex默认字号 8.添加设置字体的wrapper 占三分之一份,定义vuex字体值 8。定义弹出层 书写样式 添加动画 9.添加点击事件 更改字体，翻页时隐藏面板*

  // *(this.currentBook.rendition.themes.fontSize() this.currnetBook.rendition.themes.font())*

  // *更换字体时需要使用钩子函数*

  // *todo: 书写样式代码 定义themList方法返回them数组 1.定义vuex theme 点击事件设置当前vuex theme 删除border 和设置item.name匹配选中项*

  // *注册 initTheme(){this.themelist.forEach((theme)=>{this.rendition.themes.register(theme.name,theme.style)})}*

  // *设置默认样式 this.rendition.themes.select(defaulttheme)*

  // *设置主题方法: 点击事件异步调用select() 选中时preview设置一个阴影 保存storage 全局引如css文件到head 动态主题切换（switch case 实现） 点击事件设置全局主题 书写清除css文件方法*

  // *todo: 总结:1.完成了电子书的翻页(通过监听touchstart touchend事件) 2.完成了电子书面板样式代码和基本逻辑 3.完成了电子书的字号 字体设置 这里主要使用到了this.rendition的方法 4.主题更改 5.进度更改 6.目录显示与跳转 8.书签 9.完善 缓存处理*



  // *todo: 1.math.ceil(time/60) 取到分钟 2.获取进度 3. 获取封面 解析电子书时获取封面图（）*





