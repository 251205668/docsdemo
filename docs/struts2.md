# javaEE考试复习
## jsp相关知识点
### 内置对象
1. request(继承于Httprequest) 
2. response(继承于Httpresponse)
3. out(继承于JSPWritter)
   ```java
   <%
   out.println("jsp我不喜欢");
   response.getWritter.println("jsp我最喜爱")
   %>
   //打印结果：jsp我最喜爱 jsp我不喜欢
   out打印出结果是等jsp页面结束后才进行
   ```
   
4. session(继承HttpSession,保存会话)
5. application(包装了servletContext类的实例)
6. config(配置信息 继承servletConfig)
7. pageContext(代表整个jsp页面 相当于object)
8. page(相当于this)
9. Exception(异常抛出对象 常用:exception.getMessage)
```java
<% =exception.getMessage %>
```
具体用法啥的在jsp书上 都可以查到

### Tomcat的目录及作用

```markdown

--bin:**存放启动和停止服务器和其他脚本文件**(tomcat6.exe tomcat6w.exe)
--conf:**存放服务器的配置文件(server.xml 配置服务器文件 tomcatusers.xml 存储用户文件 web.xml 部署描述文件 context.xml 上下文)**
--lib:**存放Tomact jar包(依赖包)**
--logs:**存放Tomcat的日志文件**
--temp:**存放Tomcat的临时文件**
--webapps:**部署目录**
--work:**Tomcat工作目录**

```

## struts2 部分

`Struts2` 是 Apache 软件组织推出的一个基于 MVC 模式的轻量级 Web 框架，自问世以来，就受到了广大 Web 开发者的欢迎。目前，Struts2 在 Java Web 开发领域中已占据了十分重要的地位

优点:
- 项目开源，使用及拓展方便。
- 通过简单、集中的配置调度业务类，使配置和修改都非常容易。
- 提供简单、统一的表达式语言访问所有可供访问的数据。
- 提供标准、强大的验证框架和国际化框架。
- 提供强大、可以有效减少页面代码的标签。
- 提供 `Exception` 处理机制，并且具有良好的 `Ajax` 支持。
- Result 方式的页面导航，通过 `Result` 标签很方便地实现重定向和页面跳转。
- 拥有智能的默认设置，不需要另外进行繁琐的设置。使用默认设置就可以完成大多数项目程序开发所需要的功能。

## 第一个struts2程序
### 过程
接下来创建一个struts2程序了解struts运行机制
1. 创建web项目,将struts2依赖包build在WEB-INF/lib
   ![QQ截图20200104141408.png](https://i.loli.net/2020/01/04/AhrzLQPVcvGiKYu.png)

2. web.xml配置struts2核心过滤器
  ```xml
     <!-- 配置Struts2核心过滤器 -->
    <filter>
    <!-- 过滤器名称 -->
        <filter-name>struts2</filter-name>
        <!-- 过滤器类 -->
        <filter-class>
            org.apache.struts2.dispatcher.ng.filter.StrutsPrepareAndExecuteFilter
        </filter-class>
    </filter>
    <!-- 映射 -->
    <filter-mapping>
        <filter-name>struts2</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
  ```
3. 编写**action**类
创建一个com.java.action包 然后在里面新建一个Helloworld类, **ActionSupport**（struts2提供的类）
   ```java
   package com.java.action;
   import com.opensymphony.xwork2.ActionSupport;
   public class Helloworld extends ActionSupport {
     public String execute() throws Exception{
      //  父类继承来的常量 返回成功
       return SUCCESS;
     }

   }
   
   ```
  4. src下面创建并配置**struts.xml**
这里的**重点**是配置`action`(请求路径 映射action类) `result` (映射视图路径)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!-- 指定 Struts2 配置文件的 DTD 信息 -->
<!DOCTYPE struts PUBLIC
    "-//Apache Software Foundation//DTD Struts Configuration 2.3//EN"
    "http://struts.apache.org/dtds/struts-2.3.dtd">
<!-- Struts2配置文件的根元素 -->
<struts>
    <package name="hello" namespace="/" extends="struts-default">
        <!-- 定义 action，该 action 对应的类为 com.mengma.action.HelloWorldAction 类-->
        <action name="helloworld" class="com.java.action.Helloworld">
            <!-- 定义处理结果和视图资源之间的映射关系 -->
            <result name="success">/success.jsp</result>
        </action>
    </package>
</struts>

```
5. **视图层创建** 显示结果 index.jsp
超链接跳转helloworld action类
```java
<% @page language="java" contentType="text/html" charset="UTF-8" %>
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>首页</title>
</head>
<body>
    <a href="${pageContext.request.contextPath }/helloWorld.action">
            第一个 Struts2 程序！
    </a>
</body>
</html>
```

因为返回值是SUCESS,所以到跳转成功页
```java
<%@ page language="java" contentType="text/html; charset=utf-8"
    pageEncoding="utf-8"%>
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>成功页面</title>
</head>
<body>
    您的第一个小程序执行成功，欢迎来到Struts2的世界！
</body>
</html>
```
### 总结
基本的调用机制如下图

![QQ截图20200104144436.png](https://i.loli.net/2020/01/04/GcNY34HdSsfekDb.png)

> 首先配置好了核心过滤器(web.xml)后,写action类 然后再配置struts.xml文件(重点是action(映射包下面的action类) 和 result(映射请求页面)) **那两行配置代码记住  **

> 1. 发送action请求
> 2. 配置文件加载(struts.xml)
> 3. 调用action类 执行方法 
> 4. 转发到视图层
> 5. 生成响应内容
> 6. 输出响应

综上，这就是struts运行机制的基本内容，掌握了基本上考试就不用慌 😆😆😆

## struts配置
### struts配置基础
一个典型的struts.xml
```java
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE struts PUBLIC
  "-//Apache Software Foundation//DTD Struts Configuration 2.3//EN"
  "http://struts.apache.org/dtds/struts-2.3.dtd">
<struts>
    <!--<constant>元素用常量的配置-->
    <constant name="struts.enable.DynamicMethodInvocation" value="false" />
    <constant name="struts.devMode" value="true" />
    <!--<package>元素用于包配置-->
    <package name="default" namespace="/" extends="struts-default">
        <!--配置Action-->
        <action name="index" class="Xxx"/>
            <!--配置Result-->
            <result type="dispatcher">
                <param name="location">/index.jsp</param>
            </result>
        </action>
    </package>
    <!-- <include>元素用于包含配置 -->
    <include file="example.xml"/>
</struts>

```
### 相关配置详解
1. `<constant>`常量配置 了解一下即可
2. `<package>` 包配置 
  - **name** 包名 必须 一个struts.xml可以有多个package映射
  - **namespace** 定义包的命名空间 非必选，通常是'/*' 如果配置了namespace,对应的请求路径也要改变
  ```xml
  没有配置
  <action name="login" class="or.action.LOginAction" namespace="/"></action>


  如果配置了namespace的情况
  <action name='user/login' class="or.action.LoginAction"
  namespace ='/user'
  >
  </action>
  ```
  -  **extends** 配置这个就是继承某个包,一般为`struts-default` 因为这个包具有stuts基本属性(拦截器过滤器)

<h2>配置重点</h2>

3. `<action>`配置
- 常规配置
  - name:对应请求的Action的名称
  - class:不是必须类 指明处理类的具体路径 'org.action.LoginAction'
  - method:不是必需 Action类中不同的方法 对应的指定请求的哪个方法
  - converter: 指定Action的类型转换器

```xml
<action name="login" class="org.action.LoginAction" namespace="/">

</action>
```
- 使用通配符
  - action配置中使用
当发送一个userAction_login.action请求,{1}的作用就是取'*'值,这里就是将userAction_*换成userAction_login
    ```xml
    <package name="user" namespace="/user" extends="struts-default">
    <action name="userAction_*" class="org.action.UserAction" method={1}>
    <result>/index.jsp</result>
    </action>
    </package>
    ```
  - result里面配置
  ```xml
  <action name="*" class="org.action.loginAction" method='{1}'>
  <result name="error">
  {1}.jsp
  </result>
  </action>
  ```


4. `<result>`配置
可选的result配置:`name`,`type`(默认值:dispatcher)
```xml
<action name="loginAction" class="com.mengma.action.LoginAction">
    <result name="success" type="dispatcher">
        <param name="location">/success.jsp</param>
    </result>
</action>
```
- name
param的name有两个值:一个是location 一个是parse
通常这里的代码会简化写成
```xml
<action name="loginAction" class="com.mengma.action.LoginAction">
<result>/success.jsp</result>
</action>
```
- type(默认的type:dispatcher)
  - dispatcher
默认配置即可转发到指定资源
  - redirect(重新发一个请求,重定向)
```xml
<action name="login" class="com.mengma.action.LoginAction">
    <result name="success" type="redirect">/success.jsp</result>
    <result name="error" type="dispatcher">/error.jsp</result>
</action>
```
1) 浏览器发出一个请求，`Struts2`框架调用对应的`Action`实例对请求进行处理。

2) `Action`返回`success`结果字符串，`Struts2`框架根据这个结果选择对应的结果类型，这里使用的是`redirect`结果类型。

3) `ServletRedirectResult`在内部使用`HttpServletResponse`的`sendRedirect()`方法将请求重新定向到目标资源。

4) 浏览器重新发起一个针对目标资源的新请求。

5) 目标资源作为响应呈现给用户。

**类型作用范围**

![QQ截图20200104173255.png](https://i.loli.net/2020/01/04/jQMOiulD1FIdPr2.png)






## 标签库
### 总括
标签库表
![QQ截图20200104200515.png](https://i.loli.net/2020/01/04/GhwzVNospru2ZjA.png)

### data标签
#### `<s:action>` 
主要属性:
-  id(可选 引用标志)
-  name(必选 用来指定是哪一个action请求)
-  namespace(命名空间 与前面相似)
-  executeResult(设置为true 表示页面请求参数包含本页面)
-  ignoreContext(请求参数传入action)

这里假设配置好了struts.xml映射 success.jsp
当运行这个jsp文件 请求成功后会跳转到success.jsp去
```java
<s:action name="action" executeResult="true"></s:action>
<s:action name="action"></s:action>
```
#### `<s:propetry>`
主要属性:
- default (默认值)
- escape(是否转义)
- value(输出的属性值)
```java
<s:propetry value="我爱javaee"></s:propetry>
//忽略html代码 将html转义
<s:propetry value="'<h2>我讨厌jsp</h2>'" escape="true">
//不忽略
```
#### `<s:param>`
给标签提供参数
主要属性:
- name(参数名)
- value(参数值)

```java
//这里是设置杨先生对象值
<s:param name="author" value="杨先生"></s:param>
<s:param name="author" >杨先生</s:param>
```
反正这个标签包在其他标签里面提供参数就行

#### `<s:bean>`
javaBean实例 用于运用公共类(类似于pojo类)
例:一个简单的运用`<s:bean>`的实例
student bean
```java
package orh.vo;
public class Student {
  private String name;
  public String name(){
    return name;
  }
  public void setName(String name) {
    this.name=name;
  }
}
```
脚本运用
```jsp
<!-- name指定bean类 var定义实例 -->
<s:bean name="org.vo.Student" var="stu">
<s:param name=="name" value="杨先生"></s:param>
</s:bean>
<br/>
<!-- #实例名称调用函数 -->
<s:propetry value="#stu.name"></s:propetry>
```
#### `<s:date>`
格式化日期
主要属性:
- format(定义日期格式化格式)
- nice(如果显示时差 就设为true)
- name(必选 要格式化的日期值)

几个例子
```jsp
<%
Date bir=new Date(122,1,4,20,54,00);
request.setAttribute("bir",bir)
%>

<s:date name="#request.bir" format="yyyy-MM-dd" nice="false"/>
//2022-02-04
<s:date name="#request.bir" format="yyyy-MM-dd" nice="true"/>
//4 years 82 days

不指定格式 就会输出完整的时间信息
2022-2-4 10:54:00
```

#### `<s:debug>`
这个标签会输出当前值栈的所有信息

#### `<s:include>`
不带参数
```jsp
<s:include value="XXXX.jsp/>
```
带参数
```jsp
<s:include calue="xxxx.jsp">
<s:param name="java" value="javaee真好"/>
</s:include>
```
xxxx.jsp
```jsp
S{param.java}
```
<br/>>
剩下两个`<s:set>` `<s:url>`自己看 都很简单

```jsp
<s:set name="java" value="javaee真不是个东西"/>
<s:propetry value="java"/>

url输出字符串形式的字符串地址
<s:url value="xxx.jsp"></s:url>
...
```

### 控制标签
#### `<s:if> <s:elseif> <s:else>`
```jsp
<s:if test=""false>javaee哈巴狗</s:if>
<s:elseif test="false">javaee真好</s:elseif>
<s:else>java真不好</s:else>
```
#### `<s:iterator>`
主要属性:
- value 要遍历迭代的集合的值
- status 判断当前迭代元素的属性
    - getCount()返回元素个数
    - getIndex()返回元素索引
    - isEven()偶数真假
    - isOdd()奇数真假
```jsp
<s:iterator value="{'A','B','C'}" var="book" status="st">
<s:property var="book"/>
<s:propetry value="#st.getindex()"/>
<s:propetry value="#st.getCount()">
</s:iterator>
```

#### `<s:append>`
拼接标签
```jsp
<!-- 一定要定义books实例 不然拿不到上下文 -->
<s:append var="books">
<s:param value="{'A'}"/>
<s:param value="{B}"/>
</s:append>


<s:iterator value="#books" status>
<s:propetry value="books">
</s:iterator>
```

#### `<s:merge>` `<s:generator>` `<s:sort>` `<s:subset>`

1. 拼接集合(选每个集合第一个元素 第二个然后依次下去拼接)
2. 分隔符
3. 排序(comparator-排序规则 
```jsp
javabean 排序规则类

sort.jsp
<s:bean name="org.test" var="testdemo"/>
<s:sort comparator="testdemo" source="{'A','B','C'}"/>
<s:iterator value="#attr.sort">
<s:propetry/>
</s:iterator>

```
4. 生成新集合

### 表单标签
常用的表单标签都一样改写成`<s:formname/>`即可

#### 撸一个例子
```jsp
<s:form action="login.jsp">
<s:textfield value="javaee真狗" name="textfield" label="文本" requiredLabel="true"></s:textfield>
<s:password name="passowrd" label="密码" requiredLabel="true"></s:passowrd>
<s:hidden value="hidden"></s:hidden>
<s:textarea value="javaee我最喜欢" label="文本域"></s:textarea>
<s:checkbox value="true" label="篮球" name="checkbox"></s:checkbox>
<s:radio list="#{1:'男',2:'女'}"></s:radio>
<s:submit value="提交"></s:submit>
</s:form>
```

#### struts独有表单标签
1. `<s:checkboxlist>`
**复选框列表**
- list 集合
- listkey 集合元素key
- listValue 复选框内容
```jsp
<%@ taglib uri="/struts-tags" prefix="s"%>
<s:checkboxlist list="{'A','B','C'}" label="list复选框" name="java" lavelposition="top"/>
<s:checkboxlist list="#{1:'A',2:'B',3:'C'}" listkey="key" listValue="value" label="map集合的复选框" name="java" lavelposition="top"/>
```
2. `<s:doubleselect>`
级联选择框**
```jsp
<s:doubleselect list="" doubleName="" doublelist=""></s:doubleselect>
```
3. `<s:updownselect>`
**列表框**
list:指定集合
listkey:集合元素key
listValue：复选框内容
4. `<s:combobox>`
```jsp
<s:form>
<!-- 下拉菜单文本框 -->
<s:combobox list="{'A','B','C','D'}" name="combox"/>
</s:form>
```
5. `<s:optiontransferselect>`
  两个列表选择框 组合框 
6. `<s:optgroup>`
选项组

## Hibernate
Hibernate就是把关系与对象映射起来，通过控制对象来操作数据库
![QQ截图20200105183557.png](https://i.loli.net/2020/01/05/hpkQsgUcuRy4mdX.png)

<h3>编写pojo类 </h3>

```java
package org.vo;
public class UserTable implements java.io.Serializable{
  //Fields
  private Integer id;
  private String username;
  private String password;
  //default constructor
  public UserTable(){}
  public UserTable(String username,String password) {
    this.username=username;
    this.passowrd=password;
  }
  // gettters setters
  public Integer getid() {
    return this.id;
  }
  public void serId(String id){
    this.id=id;
  }
  public String getUsername (){
    return this.username;
  }
  public void setUsername(String username) {
    this.username=username;
  }
  public String getPassword(){
    return this.password;
  }
  public void setPassword (String password) {
    this.passowrd=password;
  }
}
```

<h3>配置映射文件</h3>
*.hbm.xml

```xml
<hibernate-mapping>
<!-- class name(pojo类) -->
<class name="org.vo.UserTable" table="userTable">
<!-- name(主键) type(主键类型) -->
<id name="id" type="java.lang.Integer">
<column name="id"/>
<generator class="native"/>
</id>
<!-- pojo属性与表中字段对应 -->
<propetry name="username" type="java.lang.String">
<column name="username" length="20" not-null="true">
</propetry>
<propetry name="password" type="java.lang.String">
<column name="password" length="20" no-null="true">
</propetry>

</class>

</hobernate-mapping>
```

主键映射
1. 代理主键映射
代理主键是自定义的,用来标识表记录的,不具有任何意义
2. 自然主键映射
自然主键映射充当数据成分
3. 复合主键映射
自然主键由两个或两个以上的字段组成

数据类型映射
type由原来的java数据类型变为Hibernate数据类型

对象关系映射
1. 继承关系映射

2. 关联关系映射
