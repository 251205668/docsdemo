## java8语法

### 类和对象

#### 变量

一个类可以包含三种变量:`局部变量`，`成员变量`,`类变量`

```java
public class Dog{
    // 成员变量
    String breed;
    int age;
    String color;
    // 局部变量
    public Dog(String name){
       String dogName;  
    }
    // 类变量
    static final username = 'ZhangSan'
    void barking(){}
    void hungry(){}
    void sleep(){}
}
```

#### 构造方法

用来初始化对象，一个对象必须要有一个构造方法

```java
public class Pub{
    public Pub(String name){
        System.out.println("")
    }
}
```

#### 创建对象

- 声明
- 实例化
- 初始化属性

```java
public class Car{
    public Car(String name){
        System.out.println("汽车名字:"+name);
    }
    public static void main(String[] args){
        Car car1 = new Car("BMW")
            // 汽车名字:BMW
    }
}
```

#### 访问成员变量

```java
public class Car{
    String name;
    public Car(String name){
        
    }
    public String getName(){
        return name;
    }
    public void setName(name){
        this.name = name;
    }
  public static void main(String[] args){
      Car car1 = new Car('bmw');
      // 设置成员变量
      car1.setName('')
      // 获取
      car1.getName()
  }
}
```

#### 继承 重写

##### 继承

公共类

```java
public class Animal { 
    private String name;  
    private int id; 
    public Animal(String myName, int myid) { 
        name = myName; 
        id = myid;
    } 
    public void eat(){ 
        System.out.println(name+"正在吃"); 
    }
    public void sleep(){
        System.out.println(name+"正在睡");
    }
    public void introduction() { 
        System.out.println("大家好！我是"         + id + "号" + name + "."); 
    } 
}
```

子类

```java
public class Penguin extends Animal { 
    public Penguin(String myName, int myid) { 
        super(myName, myid); 
    } 
}
```

> 如果父类的构造器带有参数，则必须在子类的构造器中显式地通过 **super** 关键字调用父类的构造器并配以适当的参数列表。
>
> 如果父类构造器没有参数，则在子类的构造器中不需要使用 **super** 关键字调用父类构造器，系统会自动调用父类的无参构造器。

多继承接口

```java
public interface A {
    public void eat();
    public void sleep();
}
 
public interface B {
    public void show();
}
 
public class C implements A,B {
}
```

子类调用父类方法

```java
class Dog extends Animal {
  void eat() {
    System.out.println("dog : eat");
  }
  void eatTest() {
    this.eat();   // this 调用自己的方法
    super.eat();  // super 调用父类方法
  }
}
```

##### 重写

子类对父类允许访问的方法进行重新编写， **即外壳不变，核心重写！** 

![](https://image.yangxiansheng.top/img/20200424233112.png?imagelist)

例:

```java
class Animal{
   public void move(){
      System.out.println("动物可以移动");
   }
}
 
class Dog extends Animal{
   public void move(){
      System.out.println("狗可以跑和走");
   }
}
 
public class TestDog{
   public static void main(String args[]){
      Animal a = new Animal(); // Animal 对象
      Animal b = new Dog(); // Dog 对象
 
      a.move();// 执行 Animal 类的方法
 
      b.move();//执行 Dog 类的方法
   }
}
```

#### 多态 抽象类

##### 多态

同一个行为不同的实例进行不同操作

多态例子：英雄分为 近战，射手 都可以进行杀敌行为

#### 接口

 接口（英文：Interface），在JAVA编程语言中是一个抽象类型，是抽象方法的集合，接口通常以interface来声明。一个类通过继承接口的方式，从而来继承接口的抽象方法。 

>  接口支持多继承 
>
>  接口中的方法是不能在接口中实现的，只能由实现接口的类来实现接口中的方法。 

例：

```java
interface Animal {
   public void eat();
   public void travel();
}
```

实现类

```java
/* 文件名 : MammalInt.java */
public class MammalInt implements Animal{
 
   public void eat(){
      System.out.println("Mammal eats");
   }
 
   public void travel(){
      System.out.println("Mammal travels");
   } 
 
   public int noOfLegs(){
      return 0;
   }
 
   public static void main(String args[]){
      MammalInt m = new MammalInt();
      m.eat();
      m.travel();
   }
}
```





### 数据类型

#### 基本类型

- byte/8
- char/16
- short/16
- int/32
- float/32
- long/64
- double/64
- boolean/~

#### 装箱拆箱

```java
Integer x = 2;//装箱
int y = x;    // 拆箱
```

#### 引用类型

对象，数组都是引用类型，引用类型指向一个对象，状态可以保存

 例子：Site site = new Site("Runoob")。 

#### 常量

```java
final double PI = 3.14
```

#### 类型转换

- 自动类型转换

  必须满足规则

  ```java
  低  ------------------------------------>  高
  
  byte,short,char—> int —> long—> float —> double 
  ```

  

  ```java
  char c1 = 'a';
  int a = c1;
  // a =97
  ```

- 强制转换

  语法：`(type)value type`

  ```java
  int i = 123;
  byte b = (byte)i
  ```

  

#### 字符串

常用转义字符

![](https://image.yangxiansheng.top/img/20200424214323.png?imagelist)

```java
String name = 'runoob.com'
```
##### API
- concat 连接
-  compareTo 比较是否相等 返回0
- endsWith 结尾
- indexOf 返回第一次出现索引
- lastIndexOf

#### 数组

##### 基础

- 声明

  ```java
  dateType []arrayName;
  ```

- 创建

  ```java
  1. int []array = new int[size]
  2. int []array = {1,2,3...};
  ```

- 遍历

  ```java
  int []array = {1,2,3,4,5,6};
  
  for(int i = 0;i < array.length;i++){
      
  }
  
  // 加强for
  for(int item:array){
      System.out.println(item)
  }
  ```
  
- 数组作为函数参数，和函数返回数组

  ```java
  public static void printArray(int[] array){
      
  }
  
  public void int[] reverse(int[] array){
      int[] result = new int[array.length];
       return result;
  }
  ```

  

- 多维数组
  
  ```java
  int a[][] = new int[2][3]
  ```

##### API

![](https://image.yangxiansheng.top/img/20200424231317.png?imagelist)



### 修饰符

#### 访问修饰符

- default 默认
- private 私有
- public 共有
- protected 同一包内可见，不能修饰外部类（接口）

####  非访问修饰符

- static 静态方法，静态变量
- final 保持不变
- abstract 抽象类， 声明抽象类的唯一目的是为了将来对该类进行扩充 。
- synchronized 同一时间只能被一个线程访问

### Number,Math,Date

#### Number，Math

```java
Integer x = 7 // 创建Number
    
x.equals(params) //判断相等
    
valueOf() //返回数据类型
    
x.toString() //转为字符串

x.parseInt() // 转int

Math.abs()  // 绝对值
 
Math.ceil()
Math.floor() //取整

Math.round  // 四舍五入
 
Math.min
Math.max

Math.random // 取随机数 0-1
// 去区间随机数
Math.floor(Math.random() * (max - min + 1) + min)
 
```

#### **Date**

```java
Date date = new Date()
date.toString() // 日期时间

SimpleDtaeFormat ft = new SimpleDateFormat("yyyy-MM-dd hh:mm:ss")// 格式化类
ft.format(new Date())
    
   DateTimeFormatter formatter = DateTimeFormatter.ofPattern("yyyy年MM月dd日 HH:mm:ss");
   LocalDateTime localDateTime = LocalDateTime.now();


```

#### Calendar

```java
Calendar c1 = Calendar.getInstance();
// 获得年份
int year = c1.get(Calendar.YEAR);
// 获得月份
int month = c1.get(Calendar.MONTH) + 1;
// 获得日期
int date = c1.get(Calendar.DATE);
// 获得小时
int hour = c1.get(Calendar.HOUR_OF_DAY);
// 获得分钟
int minute = c1.get(Calendar.MINUTE);
// 获得秒
int second = c1.get(Calendar.SECOND);
// 获得星期几（注意（这个与Date类是不同的）：1代表星期日、2代表星期1、3代表星期二，以此类推）
int day = c1.get(Calendar.DAY_OF_WEEK);
```

### 枚举 集合 泛型 

#### 概念

枚举:参考文章   [地址]( https://www.runoob.com/java/java-enumeration-interface.html )

集合

- Collection 接口

- List 接口

- Set 接口

- Map  键值队

- Enumeration

  ![](https://image.yangxiansheng.top/img/20200424234934.png?imagelist)

#### 使用实例

```java
List<String> list = new ArrayList<String>();// 声明数组集合
list.add("1");
list.add("2");

// 遍历方法

for - Each循环
for(String item :list){
  
}

迭代器循环
Iterator<String> ite = list.iterator();
while(ite.hasNext()){
    
}


Map
Map<String, String> map = new HashMap<String, String>();
      map.put("1", "value1");
      map.put("2", "value2");
      map.put("3", "value3");
      
      //第一种：普遍使用，二次取值
      System.out.println("通过Map.keySet遍历key和value：");
      for (String key : map.keySet()) {
       System.out.println("key= "+ key + " and value= " + map.get(key));
      }
      
      //第二种
      System.out.println("通过Map.entrySet使用iterator遍历key和value：");
      Iterator<Map.Entry<String, String>> it = map.entrySet().iterator();
      while (it.hasNext()) {
       Map.Entry<String, String> entry = it.next();
       System.out.println("key= " + entry.getKey() + " and value= " + entry.getValue());
      }
      
      //第三种：推荐，尤其是容量大时
      System.out.println("通过Map.entrySet遍历key和value");
      for (Map.Entry<String, String> entry : map.entrySet()) {
       System.out.println("key= " + entry.getKey() + " and value= " + entry.getValue());
      }
    
      //第四种
      System.out.println("通过Map.values()遍历所有的value，但不能遍历key");
      for (String v : map.values()) {
       System.out.println("value= " + v);
      }
```

## Springboot

### 理解IOC 依赖注入

#### IOC

`IOC`- 控制反转，在传统`SE`阶段如果`A`类需要使用到`B`类，需要在`A`的内部`new`一个`B`的实例出来，进而控制对象内部。**而`IOC`专门有一个`容器`来创建这些依赖的对象**，然后控制要交给`A`类哪些依赖。至于为什么叫`反转`,因为传统的获取依赖对象是`对象主动去控制`，而`IOC`的控制交给了容器，容器帮忙创建注入依赖对象，此时`A`对象只是`被动的接收依赖的注入`。

- `IOC`容器控制对象，主要控制外部资源获取
- 容器帮忙创建并注入依赖对象，程序被动接受`依赖对象`

#### DI

`DI`-依赖注入，容器将某个依赖关系注入到组件中去。依赖注入组件`重用`的频率，依赖注入是`IOC`思想最好的表现形式。

- **谁依赖谁**：`应用程序`依赖于`IOC`容器

- **为什么要使用`DI`**：应用程序需要`IOC`提供提供对象外部资源

- **谁注入谁**:`IOC`注入应用程序的对象

#### 我的理解

> `IOC`的出现解决了传统java开发应用程序，对象与对象之间耦合性，`A`需要`B`，`A`就要主动创建`B`对象，进行控制，这样`A`和`B`就产生了依赖，而且是紧密耦合性。`IOC`则不同，我们只需要吧需要的依赖在`容器`中创建好，然后要的时候由`容器`进行注入,`A`对象根本不用去管`B`以及更多依赖的问题，只需要交给容器处理，二者协作进行即可。

### springboot阶段学习

#### 版本号

2.2.1 RELEASE

```markdown
2 主版本
2 次版本 新特性 发布新特性 要保证兼容
1 增量版本 bug修复
RELEASE 发布版本 、 里程碑版本


RC 
Alpha 内测
Beta 发行 但不稳定
GA （General Availability） 官方通用
SHAPSHOT
```

#### 运行springboot项目

在官网中创建项目然后用idea打开，或者直接创建`springboot项目`

```markdown
- 打开 idea -> create project
- 选择左侧 Spring Initializr
  - 选择你的 java版本 如 8
  - next
- Group: com.公司名
- artifact : 你的项目名
- Type: 选 maven
- Language: Java
- Packaging: Jar
- java version:8
- 点击最下方的 Next
- Spring Boot 选择 2.2.x
- Dependencies 选择 web 下的 spring web 
- Next
- Finish
```

修改默认端口

> resources/application.properties 下添加
>
> server.port = 端口号

#### 编写第一个接口

创建`api.v1/api.v2`文件夹管理`api`，然后创建一个控制器类.

```java
分为三步
1. 编写返回方法
2. 插入注解
3. 返回结果

// 控制器注解
@Controller 
public class BannerController{
    // 路由注解
    @GetMapping("/test")
    // 处理返回结果注解 相当于操作了 HttpServletresponse 的打印器方法
    @ResponseBody  
    public String test(){
        return "hello,springboot"
    }
}
```

#### 配置热重启

安装`devtools`，然后配置idea

- 搜索 Compiler
- 勾选 build project automatically

#### 常见注解

- 请求method限定

    ```java
  @GetMapping("/test")
  @PostMapping("/test")
  @PutMapping("/test")
  @RequestMapping("/test") // 全方法都支持
  @RequestMapping(value = "/test",method = {RequestMethod.DELETE,RequestMethod.GET}) // method传递支持的方法
  ```

-  Springboot 提供的 简化注解

  `@RestController` 意思就是

  ```
  @Controller
  @ResponseBody
  ```

#### 统一路径管理

```java
@RestController
@RequestMapping("/v1")
public class BannerController {
    @GetMapping("/test")
    public String test(){
        return "七月,牛逼";
    }
}

```

#### 深刻理解springboot

##### 开闭原则-OCP

软件，函数，类是扩展开发的，修改是封闭的。举例说明：修改业务最好是通过新增业务模块进行处理，API的`v1`和`v2`版本的使用。



##### 面向抽象编程

`interface` ，设计模式:`工厂模式`，`IOC/DI`

如果是具体类的话，修改是灾难性的。面向抽象的话，只需要调方法即可。**真正的目的就是实现开闭原则从而达到代码可维护性。**



> springboot和springframework的区别
>
> springboot 借助springframework开发的

#####  Spring、SpringMVC与SpringBoot的关系与区别

> SSM `Spring + SpringMVC + MyBatis`

Spring 全称是 Spring Framework

- SpringBoot 是 Spring Framework 的应用

#####  什么是SpringBoot核心优势-自动配置

#####  Springboot意义性(死记)

> OCP -> IOC

- IOC实现： 容器，把控制类加入 容器 ，在你需要时把对象注入你所需要的代码里去

-  抽象意义：控制权交给用户

##### 如何将对象加入容器,并注入

- xml

- 注解

  - `stereotype annotations` 模式注解,`两步`

    ```java
    加入容器
    @Component  
    扫描加入容器注解
    @service 
    加入服务层容器
        
    使用的时候，注入,已经实例化
    @Autowired
    
    1.成员变量注入
    private Diana diana
    
    2.推荐注入方式：构造器，不需要加入注解@Autowired
     private final Diana diana;
      public BannerController(Diana diana) {
            this.diana = diana;
       }
    ```
```
    
    - `@Component` 最基础的模式注解
  - 把一个组件/类/bean加入到容器中
    
> 以下都是以 `@Component` 为基础的衍生注解
    
    - `@Service` 标明是种服务
    - `@Controller` 标明是个控制器
    - `@RestController` 标明是个restful 的 控制器 
    - `@Repository` 标明是个仓储
    - `@Configuration` 更灵活的方式 把一组bean加入到容器里
      - 跟上面的有些不同
      - 具体参考[@Configuration 注解介绍](

##### 实例化时机和延时实例化

> 如何允许 未添加 `@Component` 注解的类 为空值

```
@Autowired(required = false)
private Diana diana;
```

> IOC 对象实例化注入时机

- 在Spring启动的时候就开始 对象的实例化 并注入
- 这是一个默认的机制 **立即/提前 实例化**
  
    - 延迟实例化 `@Lazy`
    
      

##### @Autowired 类型注入方式

预设环境，多个类实现接口，并且加入到容器，使用`@Autowired`注入会加载哪一个实现

<h2>被动注入</h2>
- **bytype** 默认注入形式

  - 根据类型推断到底应该注入谁

  - 比如上面的如果注入 ISkill 就会去所有加入到容器里的bean去寻找实现ISkill的类 加入进来

```
    @Autowired
    private ISkill iSkill;
    ```
    
    - **如果仅仅有一个实现类 Diana 那就会加载它**
    - **如果有多个bean时候，字段找不到对应的`bean`， spring就不知道到底该注入谁。就会报错**

- **byname**

<h2>主动注入</h2>
强制设置注入的`value`

```java
@Autowired
@Qualifier("irelia")
private ISkill iSkill;

// 这样它就会 按你要求注入 Irelia
```

##### 如何应对变化

1. **制定一个 interface ,然后多个类实现同一个 interface.** 

   - 策略模式
   - 只能选一个策略  

2. **一个类，属性 解决变化**

   ```java
   // 比如你只有一个实现类 Diana ，但你想打印 irelia
   
   package com.lin.missyou.sample.hero;
   
   import com.lin.missyou.sample.ISkill;
   import org.springframework.stereotype.Component;
   
   @Component
   public class Diana  implements ISkill {
       private String skillName = "Irelia"
       public Diana() { System.out.println("hello,Diana"); }
       public void q(){ System.out.println("Diana Q"); }
       public void w(){ System.out.println("Diana W"); }
       public void e(){ System.out.println("Diana E"); }
       
       public void r(){ System.out.println(this.skillName + "r"); }
       
   }
   ```

   - 像这样实际上是不好的，因为在代码里了。
   - 如果你要用这样方式： **应该用读取配置的方式** 这样才不违背 OCP 原则
     - 比如 spring boot 默认 8080 端口，你可以通过修改配置文件 让他启动在其他端口
     - 这种方式不具备 扩展性，如果未来你想添加新的属性，就要改这个类了，也不够灵活。除非你保证以后这个类不再变了

   

##### @configuration注解使用方法

- 新建 HeroConfiguration.java
    1. 在 HeroConfiguration上 使用 `@Configuration`
    
    2. 对注入的对象 Camille 使用`@Bean`，返回一个`bean`实例

```
@Configuration
public class HeroConfiguration {
    @Bean
    public ISkill camille(){
        return new Camille();
    }
}
```

- 控制器类里稍微修改下

```
@RestController
@RequestMapping("/v1/banner")
public class BannerController {

    @Autowired
    private ISkill camille;

    @GetMapping("/test")
    public String test2() {
        camille.q();
        return "Hello,亚瑟";
    }
}
```

**优势**

>  如果我们的 hero 类 新增了属性那么如何初始化

- `@Component` 是**无法做到把 类的属性进行初始化的**
- `@Configuration` 则可以
- `@Configuration` 还能同时初始化多个 bean

Camille.java

- 新增了 name / age 字段 并在构造器里赋值

```java
public class Camille implements ISkill {

    private String name;
    private Integer age;

    public Camille(String name, Integer age) {
        this.name = name;
        this.age = age;
    }

    public void setName(String name) {
        this.name = name;
    }

    public void setAge(Integer age) {
        this.age = age;
    }

    public Camille() { System.out.println("hello,Camille"); }
    public void q(){ System.out.println("Camille Q"); }
    public void w(){ System.out.println("Camille W"); }
    public void e(){ System.out.println("Camille E"); }
    public void r(){ System.out.println("Camille r"); }
}
```

HeroConfiguration.java 里只需要这样就可以实现

- 即使你想调用无参构造器 ，也可用通过 setName / setAge 在 return camille

```java
@Configuration
public class HeroConfiguration {

    @Bean
    public ISkill camille(){
        return new Camille("camille",18);
    }
    
     @Bean
    public ISkill diana(){
        return new Diana();
    }
}
```

##### springboot扫描注解

默认是与程序主入口文件夹下

`@ComponentScan("path")`

> 手动指定你想要加载其他位置的包

- 如果手动指定的路径 已经在默认路径里会标红
- 新增的扫描位置是不影响原来的扫描位置，是可以叠加的

```
@SpringBootApplication
@ComponentScan("com.lin")
public class MissyouApplication {
    public static void main(String[] args) {
        SpringApplication.run(MissyouApplication.class, args);
    }
}
```

##### 策略模式实现的几种方式

1. `byname 方式` 切换 bean的 name

    ```java
    @Autowired
    private Iskill diana
    ```

    

2. `@Qualifier` 指定 bean

    ```java
    多个bean情况下
    
    @Autowired
    @Qualifier("diana")
    private Isskill isskill
    ```

    

3. **有选择的只注入一个 bean 注释掉某个 bean的 @Component**

4. `@Primary` 

    - 如果同时 Diana 和 Irelia 同时加上了 @Component
    - 如果定义的时候是 ISkill iskill 那么会报错
    - 可以想让 Diana 生效则 额外添加`@Primary`
    ```java
    @Component
    @Primary
    public class Diana  implements ISkill {
        ...
    }
    ```

##### 条件注解

配置类

```java
@configuarition
public class HeroConfiguarition {
    @bean
    public ISkill iskill(){
        return new Dinaa()
    }
    // 可以有多个bean
}
```

> 自定义条件注解

**`@Conditional` + 实现Condition 接口的元类**

- 分别注释掉 Diana 和 Irelia 里的 `@Component`

- 修改 HeroConfiguration.java 
    ```
    @Configuration
    public class HeroConfiguration {
    
        @Bean
        @Conditional(DianaCondition.class)
        public ISkill diana(){
            return new Diana();
        }
    
        @Bean
        @Conditional(IreliaCondition.class)
        public ISkill irelia(){
            return new Irelia();
        }
    }
    ```
- DianaCondition.java / IreliaCondition.java
```
// 注意 java 很多类都有 Condition 这里引入 spring framework的
import org.springframework.context.annotation.Condition;

public class DianaCondition implements Condition {
    @Override
    public boolean matches(ConditionContext conditionContext, AnnotatedTypeMetadata annotatedTypeMetadata) {
        // 判断条件
        return true;
    }
}


public class IreliaCondition implements Condition {
    @Override
    public boolean matches(ConditionContext conditionContext, AnnotatedTypeMetadata annotatedTypeMetadata) {
        // 判断条件
        return false;
    }
}
```

#### 二次封装springboot框架机制

##### 异常处理概念

统一异常捕获

```java
@ControllerAdvice
public class GlobalException {
    @ExceptionHandler(value = Exception.class)
    public void handleException(HttpServletRequest req,Exception e){
        System.out.println("hello");
    }
}
```

**异常分类**

> **`CheckedException`** 受检异常  (可以处理，比如是A类调用B类的方法，但是B类没有方法)

- 编译阶段进行处理，否则编译通不过.
- 必须程序里主动处理

> **`RuntimeException`** 运行时异常（不能处理，比如数据库记录查询结果为空）

- 可以不处理

> 对于web如果有全局的异常处理

- 可以不区分





##### 全局异常处理步骤

>  处理的异常分为**已知异常或者未知异常**

###### 1. 定义`HttpException类`，继承`RuntimeException`

   ```java
   public class HttpException extends RuntimeException{
       protected Integer code;
       protected Integer HttpstatusCode;
   }
   
   ```

###### 2. 基类子异常，比如`NotFoundException`

   ```java
   public class NotFoundException extends HttpException{
       public NotFoundException(int code){
           this.HttpstatusCode = 404;
           this.code = code;
       }
   }
   ```

###### 3. 定义统一异常返回格式类 ，构造函数初始化属性，并且一定要有`getter`方法，否则无法访问

   ```java
   public class UnifyException {
       private int code;
       private String message;
       private String request;
   
       public UnifyException(int code, String message, String request) {
           this.code = code;
           this.message = message;
           this.request = request;
       }
   
       public int getCode() {
           return code;
       }
   
       public void setCode(int code) {
           this.code = code;
       }
   
       public String getMessage() {
           return message;
       }
   
       public void setMessage(String message) {
           this.message = message;
       }
   
       public String getRequest() {
           return request;
       }
   
       public void setRequest(String request) {
           this.request = request;
       }
   }
   ```

   

###### 4. 全局捕捉异常类`GlobalException`，分为`已知异常`和`未知异常`

   `@ControllerAdvice`捕获异常注解

` @ExceptionHandler(value = Exception.class)`捕获到进行处理的注解

   `@ResponseStatus(code = HttpStatus.INTERNAL_SERVER_ERROR)`设置状态码

   可以通过`req`获取`method`,`url`,

   - 已知异常: 处理`Exception`，设置HttpstatusCode为500，然后返回`UnifyException`
   - 未知异常: 使用 `ResponseEntity<UnifyException>`定义一个泛型，然后返回这个泛型，需要传入三个参数，`message`,`header`，`HttpStatusCode`

   ```java
   @ControllerAdvice
   @ResponseBody
   public class GlobalException {
       // 加载配置文件关联的类 处理message
       @Autowired
       private ExceptionCodeConfiguration codeConfiguration;
       // 未知异常
       @ExceptionHandler(value = Exception.class)
       @ResponseStatus(code = HttpStatus.INTERNAL_SERVER_ERROR)
       public UnifyException handleException(HttpServletRequest req,Exception e){
           // 当有checkedException异常抛出,加上这两个方法,会在全局捕捉到异常,并运行方法
           String url = req.getRequestURI();
           String method =req.getMethod();
           UnifyException message = new UnifyException(999,"服务器异常",method+" "+url);
           // 返回对象序列化
           return message;
       }
      
       // 已知异常
      @ExceptionHandler(HttpException.class)
       public ResponseEntity<UnifyException> handleHttpException(HttpServletRequest req, HttpException e){
           String url = req.getRequestURI();
           String method = req.getMethod();
           UnifyException message = new UnifyException(e.getCode(),codeConfiguration.getMessage(e.getCode()),method+" "+url);
           // 设置已知异常的Httpstatus 利用泛型设置
           //ResponseEntity<UnifyResponse> r = new ResponseEntity<>(message,header,httpStatus);
           // 处理返回的 header httpstatus
           HttpHeaders header = new HttpHeaders();
           header.setContentType(MediaType.APPLICATION_JSON);
   
           HttpStatus httpStatus = HttpStatus.resolve(e.getHttpstatusCode());
           ResponseEntity<UnifyException> r = new ResponseEntity<>(message,header,httpStatus);
           return r;
       }
   
   }
   ```

   ![](https://image.yangxiansheng.top/img/20200429000523.png?imagelist)

![1588089946065](C:\Users\努力中的杨先生\AppData\Roaming\Typora\typora-user-images\1588089946065.png)

###### 自定义错误码，统一返回格式

首先定义一个文件管理`code`码对应的`message`,俗称错误码清单

```java
lin.codes[10000] = 通用异常
lin.codes[10001]= 通用参数异常
```

然后，定义一个`configuration`类对配置文件进行关联，将`codes`看做是`Map`数据结构，然后定义方法获取到`message`

>@ConfigurationProperties(prefix = "lin")  配置前缀
>@PropertySource(value = "classpath:config/exception-code.properties") 加载配置文件路径
>@Component 

```java
@ConfigurationProperties(prefix = "lin")
@PropertySource(value = "classpath:config/exception-code.properties")
@Component
public class ExceptionCodeConfiguration {
/*
  codes看做是 Map数据结构，键值对应
 */
    private Map<Integer, String>codes;

    public Map<Integer, String> getCodes() {
        return codes;
    }
    public void setCodes(Map<Integer, String> codes) {
        this.codes = codes;
    }

    public String getMessage(int code){
        String message = codes.get(code);
        return message;
    }

}
```

然后将之前写死的`message`替换成方法即可

##### 构建校验层

###### 获取参数

`@PathVariable`获取路径中的参数 `param`

`@RequestParam` 获取`query`参数

`@RequestHeader`

`@RequestBody`

```java
@GetMapping("/test/{id}")
    public String test(@PathVariable Integer id,@RequestParam String name){
        iSkill.r();
        throw new NotFoundException(10001);
//        return "七月,牛逼";
    }
```

获取`POST`请求的`body`

定义一个`DTO`类，数据传输类

```java
public class PersonDTO {
    private String name;
    private Integer age;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public Integer getAge() {
        return age;
    }

    public void setAge(Integer age) {
        this.age = age;
    }
}

```



然后用`@RequestBody PersonDTO person`获取对象

```java
 @PostMapping("/test")
    public String test(@RequestBody PersonDTO personDTO){
        iSkill.r();
        throw new NotFoundException(10001);
//        return "七月,牛逼";
    }
```

###### 使用lomBok

-   生成`getter,setter`

  `@Getter`

  `@Setter`

-  生辰有参数构造函数和无参构造函数 `@AllArgsConstructor`,`@NoArgsConstructor`

  ```
  @AllArgsConstructor  全参数构造函数
  @NoArgsConstructor   无参数构造函数
  ```

-  生成必填参数的构造函数 `@RequiredArgsConstructor`

  ```java
  @Getter
  @Setter
  @NoArgsConstructor
  @RequiredArgsConstructor
  public class PersonDTO {
      @NonNull
      private String name;
      private Integer age;
  }
  // 生成了必填name的构造函数
  ```

-  创建对象实例化

  ```java
  import lombok.Builder;
  
  @Builder
  public class PersonDTO {
      private String name;
      private Integer age;
  }
  ```

  创建对象的时候就可以这样


  ```java
  PersonDTO.builder()
      .name("abc")
      .age(19)
      .build();
  ```

-   `@Builder` 的坑

  - 一旦加上这个注解，就不能用构造器的方式 实例化了
  - 即使你加了 @Getter/@Setter

  ```java
  也不能这样了
  PersonDTO p = new PersonDTO();
  p.setName("abc");
  p.setAge(19)
  ```

  **因为 @Builder 之后会生成 私有的无参构造函数**

  你只能在手动添加`@NoArgsConstructor` 注解生成共有的无参构造器，或者手动写一个 共有的构造器

  ```java
  @Builder
  @Setter
  @NoArgsConstructor
  public class PersonDTO {
      private String name;
      private Integer age;
  }
  ```
  
- **对象实例化最佳用法**

  使用`@builder`实例化对象，必须要添加`@Getter`,否则无法序列化。

  ```java
  @PostMapping("/test5/{id}")
  public PersonDTO test5(@PathVariable Integer id,
                      @RequestParam String name,
                      @RequestBody PersonDTO person){
       PersonDTO dto = PersonDTO.builder()
            .name("abc")
            .age(19)
            .build();              
      return dto;
  }
  ```

###### 使用校验器注解校验

- 验证简单参数,在`class`头部添加`validated`

`@Range`

`Max`

`Min`

```java
 public PersonDTO test(@PathVariable @Range(min = 0,max = 10,message = "id不合法") Integer id){
        iSkill.r();
        PersonDTO personDTO1 = PersonDTO.builder().age(10).name("7yue").build();
        return personDTO1;
    }
```

- 验证`DTO`参数，然后再方法前面加上`@Validated`

```java
public class PersonDTO {
    @Length(min = 1,max = 8,message = "长度应该在1到8之间")
    private String name;
    private Integer age;
}

```

- 级联校验：如果`DTO`中还有一个对象需要校验，必须要加上`@Valid`注解关联

  ```java
     @Valid
      private SchoolDTO schoolDTO;
  ```

  ```java
  @Getter
  public class SchoolDTO {
      @Min(value = 2)
      String schoolName;
  }
  
  ```

  

###### 编写自定义校验注解

1. 自定义注解写法 ，定义注解class

```java
@Documented // 注释文档加入
@Retention(RetentionPolicy.RUNTIME) //选择保留在运行阶段
@Target({ElementType.TYPE}) // 选择作用的目标  如果作用方法 ElementType.METHOD
@Constraint(validatedBy = PasswordValidator.class) // 关联的校验类

public @interface PasswordEqual {
    String message() default "password is not equal"; // 定义返回的message
    Class<?>[] groups() default {};
    Class<? extends Payload>[] payload() default {};

}
```

2. 编写自定义校验注解的关联类,继承` ConstraintValidator<PasswordEqual, PersonDTO>`

   >ConstraintValidator<> 是一个泛型接口
   >    接受两个参数
   >        第一个是 自定义注解类型 PasswordEqual
   >        第二个是 这个自定义注解 PasswordEqual 修饰的 目标类型，`你要校验哪个DTO 你就加在谁身上`（PersonDTO）
   >    实现` isValid 方法` 具体的校验逻辑

   定义关联类

   ```java
   public class PasswordValidator implements ConstraintValidator<PasswordEqual, PersonDTO> {
       @Override
       public boolean isValid(PersonDTO personDTO, ConstraintValidatorContext constraintValidatorContext) {
       String password1 = personDTO.getPassword1();
       String passwword2 = personDTO.getPassword2();
           return password1.equals(passwword2);
       }
   }
   ```

3. 将校验注解添加上即可

4. 给注解添加参数，然后再关联类获取注解信息

   ```java
      int min() default 4;
       int max() default 8;
   ```

   

   ```java
   重写方法 获取到注解的参数
   @Override
       public void initialize(PasswordEqual constraintAnnotation) {
           // 获取注解的最大值和最小值参数
           min = constraintAnnotation.min();
           max = constraintAnnotation.max();
       }
   ```

5. 返回错误信息给前端

   改造全局异常处理类  校验异常`MethodArgumentNotValidException ` 一个是`body`校验，一个是`url`传递

   ```java
    // 参数异常
   
       @ExceptionHandler(MethodArgumentNotValidException.class)
       @ResponseStatus(code = HttpStatus.BAD_REQUEST)
       public UnifyException hanldeMethodArgumentNotValidException(HttpServletRequest req, MethodArgumentNotValidException e){
           String url = req.getRequestURI();
           String method = req.getMethod();
           // 拿到所有的验证异常
           List<ObjectError> errors = e.getBindingResult().getAllErrors();
           String messages = format(errors);
           return new UnifyException(10001,messages,method+" "+url);
       }
       private String format(List<ObjectError> errors){
           // 获取错误信息数组 将数组拼接成字符串
           StringBuffer errorMsg = new StringBuffer();
           errors.forEach(error-> errorMsg.append(error.getDefaultMessage()).append(";"));;
           return errorMsg.toString();
       }
   
       @ExceptionHandler(value= ConstraintViolationException.class)
       @ResponseStatus(code= HttpStatus.BAD_REQUEST)
       @ResponseBody
       public UnifyException handlerConstrainException(HttpServletRequest req, ConstraintViolationException e) {
           String requestUrl = req.getRequestURI();
           String method = req.getMethod();
   
           //这里如果有多个错误 是拼接好的，但是如果需要特殊处理，就不能用它了
           String message = e.getMessage();
           /*
           // 自定义错误信息时
           for (ConstraintViolation error:e.getConstraintViolations()) {
               ConstraintViolation a = error;
           }
           */
           return new UnifyException(10001,message,method + " " + requestUrl);
       }
   ```

   至此，异常处理和验证信息层全部封装完毕，只需要简单的添加注解或者主动抛出异常类即可使用。
   
 ###### 返回成功时

   正常返回时也应该有状态码显示

   ```java
   public Map<String, Object> getByName(@PathVariable @NotBlank String name){
           Banner banner = bannerService.getByName(name);
           if(banner == null){
               throw new NotFoundException(30005);
           }
           Map<String, Object>results = new HashMap<String, Object>();
           results.put("code",0);
           results.put("message","返回成功");
           results.put("data",banner);
           return results;
       }
   ```

   

#### JPA

##### 业务层

> 一般都是用`接口`来进行层与层的调用,首先定义`BannerService`接口，然后实现接口方法，然后将接口加入容器`@Service`,但是这样非常`繁琐`,可以直接实现类



##### 启动命令启动我们的程序(不同的环境)

```java
spring:
  profiles:
    active: dev

missyou:
  api-package: com.lin.missyou.api
```



配置文件的区分，在全部的环境下`application.yml`,在开发环境`application-dev.yml`,在上生产环境`application-prod.yml`

- 服务器上实际是一个 jar包，没有 idea工具，所以要通过命令启动

- 执行打包命令 `mvn clean package` 就会在 target目录下生成一个 jar文件

- 通过 命令 `java -jar xxx.jar --spring.profiles.active=dev` 指定读取哪个配置文件




##### 新建表

安装好部分依赖后，配置`application.yml`,`url`中指定数据库和端口号和配置字符，使用`jpa`，一般都是这样配置

```yml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/missyou?characterEncoding=utf-8&serverTimezone=GMT%2B8
    username: root
    password: wohenpi0918
  jpa:
    hibernate:
      ddl-auto: update
```

然后新建模型类`Banner`,一定要打上`@Entity`实体注解，然后指定主键

```java
@Entity
@Table(name="banner1") // 修改表名
public class Banner {
    @Id
    private Integer id;
    @Column() // 配置限制
    private String name;
    private String description;
    private String img;
    private String title;
}

```

##### **表与表的关系**
```markdown
 一对一: 人 身份证

 一对多: 班级 学生

 多对多: 老师  学生
```
> 一对一

- 一张表字段过多，有意识的拆成多个表
- 设计一对一考虑：
    - 查询效率，避免一个表字段太多
    - 业务的角度，不同的业务归类在不同的表里
    
> 一对多

- 最简单的一种关系

> 多对多

- 至少三张表才能表示 多对多
    - student (sid,name)
    - teacher (tid,name)
    - student_teacher (id,sid,tid) 老师学生关系表
- 多对多复杂性：
    - 难点在于 表实际上有很多，每个表和其他表可能也有关系，这样问题就会变得复杂了
    - 第三张表是不是一个毫无意义的表？
        - 比如student_teacher 它只是用来记录关系 ，这就是无实际业务意义的表
    - **有意义的第三张表** 
        - `用户-优惠券` user_coupon(id,uid,cid,status,order_id,update_time) 有 业务字段
            - status 为 优惠券状态
            - 只有 status = 2的时候代表 使用了优惠券，order_id 记录是那笔订单
            - 这样保存在第三张表的 status,order_id 就是记录 实际的业务意义

##### 设计数据库的步骤

1. 把业务对象抽离出来，比如:`Coupon优惠券`,`banner`,`order`
2. 思考对象与对象之间的关系，比如`外键`
3. 细化：`字段限制`,`长度`,`小数点`,`唯一索引`

解决性能问题:

1. 表的记录不能过多
2. 建立索引，水平垂直分表
3. 加入缓存机制

#####  层与层之间的关系(重点)
在编写业务之前，理清楚各层之间的关系
- model 层  对象实体层，我们最终要返回的结果基本上都是以model对象的形式返回的。例如在`service`层定义接口
```java
public interface BannerService {
    Banner getByName(String name);
}

或者实现接口
 @Override
    public Banner getByName(String name) {
        return bannerRepository.findOneByName(name);
    }
```
- service层 业务层,通常不能将处理业务的方法定义在`控制器层`，都是定义在`service`,然后标准的定义方法就是先定义`接口`,再实现接口，当要操作数据库时,调用`repository`层的`JPA`接口

接口实现类,记得要导出`@service`
```java
@Service
public class BannerServiceImpl implements BannerService {
    @Autowired
    private BannerRepository bannerRepository;
    @Override
    public Banner getByName(String name) {
        return bannerRepository.findOneByName(name);
    }
}
```
- controller层 控制层，通常接口定义在这一层，并且这一层负责调用`service`层方法，进行相关业务，然后返回结果。
```java
   @GetMapping("/name/{name}")
    public Banner getByName(@PathVariable @NotBlank String name){
        Banner banner = bannerService.getByName(name);
        return banner;
    }
```




##### 编写JPA业务的常用知识

###### 设置关联表

加入一个`BannerItem`模型，一个banner对应多个`BannerItem`

```java
@Entity
public class BannerItem {
    @Id
    private long id;
    private String img;
    // 跳转spu 需要携带一个 id 如果是 专题 则是 专题的标识
    private String keyword;
    // 首页banner 点击可能是 商品详情 可能是其他 专题
    private String type;
    private String name;
}

```

但是发现这样运行程序，`JPA`会生成三张表,我们并不需要第三张表

![](https://image.yangxiansheng.top/img/20200503130825.png?imagelist)

###### 单向一对多

```java
@Entity
@Table(name = "banner")
public class Banner {
    @GeneratedValue(strategy = GenerationType.IDENTITY)  // 自动增长注解
    @Id
    private long id;
    @Column(length = 16)
    private String name;
    @Transient
    private String description;
    private String img;
    private String title;
   
    // 一对多关系 外键是banenrId
    @OneToMany
    @JoinColumn(name="bannerId")
    private List<BannerItem> items;
}
```

###### 建立repository层

建立操作数据库的仓储层,新建`repository`包，再新建接口，**这里不需要实现接口**,只需要引入方法自动生成sql语句，`service`层调用

```java
public interface BannerRepository extends JpaRepository<Banner,Long> {
/*
 * 继承JpaRepository传入的参数是  1.操作的实体类 2.实体类主键类型
 */
    
    Banner findOneById(Long id);
    Banner findOneByName(String name);
}

```

###### 执行业务(调用repository接口)

然后在`service`层调用

```java
@Service
public class BannerServiceImpl implements BannerService {
    @Autowired
    private BannerRepository bannerRepository;
    @Override
    public Banner getByName(String name) {
        return bannerRepository.findOneByName(name);
    }
}
```

最后在`controller`层调用业务层方法，返回数据.



###### 设置sql打印在控制台

>```yml
>jpa: 
>  hibernate:    
>   ddl-auto: update  
>  properties:    
>    hibernate:      
>      show_sql:true      
>      format_sql:true
>```

这里会发现默认是`懒加载`，只有当你去展开`banner-item`时才去查询另一张表。

**设置急加载模式**:`@OneToMany(fetch = FetchType.EAGER)`

###### 双向一对多配置

有时候，我们需要在查询`bannerItem`时同时查询到`banner`导航,这里就需要设置双向一对多关系，分为两个方：`一方`，`多方`

1. 设置`BannerItem`多对一关系,这里是多方,**记住双向一对多关系中`@JoinColumn`一定是打在多端的**

   ```java
    @ManyToOne
       @JoinColumn(insertable = false,updatable = false,name = "bannerId")
       private Banner banner;
   ```

2. 设置`Banner`一方的`mappedBy`,值是多方导航属性的名字，也就是上面定义的`banner`

   ```java
   @OneToMany(mappedBy = "banner",fetch = FetchType.EAGER)
       private List<BannerItem> items;
   ```

   这里可能要注释掉定义的`bannerId`,

   如果要显示添加`bannerId`字段，就要设置外键

   ```java
    private Long bannerId;
       @ManyToOne
       @JoinColumn(insertable = false,updatable = false,name = "bannerId")
       private Banner banner;
   ```

   `BannerItem`

   ```java
   @Entity
   public class BannerItem {
       @Id
       @GeneratedValue(strategy = GenerationType.IDENTITY)
       private long id;
       private String img;
       private String keyword;
       private String type;
       private String name;
       private Long bannerId;
   
       @ManyToOne
       @JoinColumn(insertable = false,updatable = false,name = "bannerId")
       private Banner banner;
   }
   ```

   `Banner`

   ```java
   @Entity
   @Table(name = "banner")
   public class Banner {
       @Id
       @GeneratedValue(strategy = GenerationType.IDENTITY)
       private long id;
   
       @Column(length = 16)
       private String name;
   
       private String description;
       private String img;
       private String title;
   
       // 双向一对多关系 查询结果中会有bannerItem数组
   
       @OneToMany(mappedBy = "banner",fetch = FetchType.EAGER)
       private List<BannerItem> items;
   }
   ```

   

###### 多对多配置
- 单向多对多关系
**创建两个实体类，主题和SPU的多对多关系，只需要在一方设置注解**
Spu.java

```java
@Entity
public class Spu {
    @Id
    private Long id;
    private String title;
    private String subtitle;
}
```

Theme.java

```java
@Entity
public class Theme {
    @Id
    private Long id;
    private String title;
    private String name;

    // 导航属性
    @ManyToMany
    private List<Spu> spuList;
}
```

此时生成三个表

```markdown
spu
theme
theme_spu_list(theme_id,spu_list_id)  关系表
```

> 我们不想要生成的关系表叫做 theme_spu_list 而是 theme_spu 才对
> 而且 theme_spu_list 里的字段 spu_list_id 应该是 spu_id 才对

这里我使用到`@JoinTable`这个注解,**指定外键和第二个外键名称和第三张表名**

```java
@Entity
public class Theme {
    @Id
    private Long id;
    private String title;
    private String name;

    // 导航属性
    @ManyToMany
    @JoinTable(name="theme_spu",joinColumns = @JoinColumn(name = "theme_id"),
    inverseJoinColumns = @JoinColumn(name="spu_id"))
    private List<Spu> spuList;
}
```
这样生成的关系表就是 `theme_spu(theme_id,spu_id)`

- 双向多对多关系
双向多对多关系需要配置`被维护端`，哪一方有` mappedBy` 那一方就是 被维护端
  
> Spu.java

  ```
  @Entity
  public class Spu {
      @Id
      private Long id;
      private String title;
      private String subtitle;
  
      //导航属性
      @ManyToMany(mappedBy = "spuList") 
      private List<Theme> themeList;
  }
  ```
> Theme.java

  ```
  @Entity
  public class Theme {
      @Id
      private Long id;
      private String title;
    private String name;
  
      // 导航属性
      @ManyToMany
      @JoinTable(name="theme_spu",joinColumns = @JoinColumn(name = "theme_id"),
      inverseJoinColumns = @JoinColumn(name="spu_id"))
      private List<Spu> spuList;
  }
  ```

针对我们这个 spu / theme 关系维护端和被维护端可以相互颠倒。

  针对**查询**来说，无论谁是 关系维护端还是被维护端都没有关系。

###### 禁止JPA生成物理外键

```java
 	@OneToMany(mappedBy = "banner",fetch = FetchType.EAGER)
    @org.hibernate.annotations.ForeignKey(name = "null")
    private List<BannerItem> items;
```

但这是一个过时废用的注解，新注解有`bug`

使用`idea`反向生成`Entity`模型类

#### 编写业务

##### banner(/banenr)

###### 创建一对多关系

首先反向生成模型，然后简化，之后编写`service`层实现方法，然后在`service`层操作数据库调用`repository`

层，最后在控制器层调用实现的方法返回数据即可

###### 优化返回的三个时间

首先提取基类`baseEntity`,然后模型继承该类，处理事件问题,一定要打上`@MappedSuperclass`这个注解，表示映射类，这样才能显示正确时间

```java
@Getter
@Setter
@MappedSuperclass
public abstract class BaseEntity {
    private Date create_time;
    private Date update_time;
    private Date delete_time;
}
```

然后访问之前写过的`Banner`接口

![](https://image.yangxiansheng.top/img/20200503204037.png?imagelist)

###### 配置默认的jachson优化返回结果

```yml
 jackson:
    property-naming-strategy: SNAKE_CASE // 默认将驼峰转为下划线形式
    serialization:
      WRITE_DATES_AS_TIMESTAMPS: true  // 将时间转为时间戳
```

然后控制某个字段不序列化，打上`@Jonignore`即可

```java
@Getter
@Setter
@MappedSuperclass
public abstract class BaseEntity {
    @JsonIgnore
    private Date create_time;
    @JsonIgnore
    private Date update_time;
    @JsonIgnore
    private Date delete_time;
}
```

然后返回结果

![](https://image.yangxiansheng.top/img/20200503205512.png?imagelist)

###### 附加where的查询语句

```java
@Entity
@Getter
@Setter
@Where(clause = "delete_time is null")
public class Banner extends BaseEntity{}
```

##### Theme

##### spu

###### 详情(/{id}/detail)

spu的简单的单表查询就常规写法即可，创建`service`层，然后调用`repositrty`层，定义返回的结果是`Spu`即可

后面需要配置一下导航属性 查看`detail-img`和`spu_img`

```java
 // 配置导航关系
    @OneToMany(fetch = FetchType.LAZY)
    @JoinColumn(name = "spuId")
    private List<Sku> skuList;

    @OneToMany(fetch = FetchType.LAZY)
    @JoinColumn(name = "spuId")
    private List<SpuDetailImg> spuDetailImgList;

    @OneToMany(fetch = FetchType.LAZY)
    @JoinColumn(name = "spuId")
    private List<SpuImg> spuImgList;
```

 ###### 序列化和反序列化(改变spec返回格式)

> 然后会碰到一个问题，我们读取`spec`时需要一个`json`数组对象，但是数据库中存放的时字符串
> 然后读取的时候要将对象转换成字符串
>
> 我们要做的就是将json字符串 转为json对象 ，json字符串分为List 和单体的 Map

编写`ListAndjson`和`MapAndjson`工具类

单体`MapAndjson` 继承`AttributeConverter`接口，实现两个方法 然后传入的参数是 `希望序列化的实体属性类型`,`数据库json类型`这里json我们通常写成String

这里使用到了序列化工具`ObjectMapper`

```java
@Convert
public class MapAndjson implements AttributeConverter<Map<String, Object>,String> {
@Autowired
    private ObjectMapper mapper;

    @Override
    public String convertToDatabaseColumn(Map<String, Object> stringObjectMap) {
        try {
            return mapper.writeValueAsString(stringObjectMap);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
            throw new ServerExcetion(999);
        }
    }
    @Override
    @SuppressWarnings("unchecked")
    public Map<String, Object> convertToEntityAttribute(String s) {
        try {
            /*
            将数据库的json对象 转换成Map结构的字段
             */
            return mapper.readValue(s, HashedMap.class);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
            throw new ServerExcetion(999);
        }
    }
}
```

同理将`json`字符串返回数组类型json格式

```java
public class ListAndjson implements AttributeConverter<List<Object>,String> {

    @Autowired
    private ObjectMapper mapper;
    @Override
    public String convertToDatabaseColumn(List<Object> objects) {
        try {
            return mapper.writeValueAsString(objects);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
            throw new ServerExcetion(999);
        }
    }

    @Override
    @SuppressWarnings("unchecked")
    public List<Object> convertToEntityAttribute(String s) {
/*
反序列化 将数据库字段读取 转换成数组集合
 */
        try {
            if(s == null){
                return null;
            }
            List<Object> t = mapper.readValue(s,List.class);
            return t;
        } catch (JsonProcessingException e) {
            e.printStackTrace();
            throw new ServerExcetion(999);
        }
    }
}
```

使用这两个序列化类在实体属性上打上注解`@convert(@converter=ListAndjson.class)`

> 但是失去了业务能力 就是不能调用model下的方法





###### 获取最新商品列表（/latest）

直接返回全部`latest`列表，在`spuService`定义方法调用`getAll()`即可返回，但是这种方式太捞了，要增加`分页`和`排序`的功能。

######  vo层自定义返回数据格式(简化数据)

- 单个vo对象

```java
@Getter
@Setter
public class SpuSimplifyVO {
    private Long id;
    private String title;
    private String subtitle;
    private String img;
    private String forThemeImg;
    private String price;
    private String discountPrice;
    private String description;
    private String tags;
    private String sketchSpecId;

}

```

然后拷贝属性,返回`vo`格式的数据,做这一步的目的是为了简化这样的写法

`vo.setTitle(spu.getTitle());`

```java
 Spu spu = this.spuService.getSpuById(id);
 SpuSimplifyVo vo =new SpuSimplifyVo();
        /*
         * 工具集拷贝对象属性 参数是源和对象
         */
  BeanUtils.copyProperties(spu,vo);
  return vo;
```

- 一组vo对象

如果是一个数组，需要借助一个库`dozer-core`

```java
// 引入 mapper
Mapper mapper = DozerBeanMapperBuilder.buildDefault();
// 定义两个数组
 List<Spu> spuList = this.spuService.getLatestSpuList();
 List<SpuSimplifyVo>vos = new ArrayList<>();
// 通过map方法，参数是源和目标的class 遍历拿到vo然后加入数组集合
  spuList.forEach(s->{
            SpuSimplifyVo vo = mapper.map(s,SpuSimplifyVo.class);
            vos.add(vo);
    });
   return vos;
```

###### 分页

`传统web端`： 分页参数一般为 `pageSize`,`page`

`移动端`: 分页参数一般为`start`,`count`

> 具体实现思路：
>
> 1. 设置默认的参数
> 2. 创建分页业务对象(bo层) 将`start`和`count`转化成`page`和`count`
> 3. `service`传入`page`和`count`，利用JPA查询出`pageable`对象，然后返回
> 4. 利用`dozer-core`创建`pagingDozerVo`和`pagingVo`层简化数据对象

```java
getLatestSpuList(@RequestParam(defaultValue="0") Integer start,@RequestParam(defaultValue="10") Integer count)
```

`pageCounter`搭配编写的`CommonUtil`方法类处理接收的参数

```java
@Setter
@Getter
@Builder
public class pageCounter {
    private Integer page;
    private Integer count;
}
```

```java
public class CommonUtil {
    public static pageCounter convertStartToPage(Integer start,Integer count){
        int page = start/count;
        return  pageCounter.builder().page(page).count(count).build();
    }
}

```

`service`查询分页数据,**这里返回的数据是`Page<>`泛型**，查询API:`findAll(pageable)`

```java
 public Page<Spu> getLatestPagingSpu(Integer pageNum, Integer size){
     // 创建分页对象 参数为当前页 size 和排序规则
        Pageable pageable = PageRequest.of(pageNum,size, Sort.by("createTime").descending());
        return this.spuRepositpry.findAll(pageable);
    }
```

简化数据层`pagingVo`,封装简化数据层和初始化数据`PagingDozer` 

> 这两个类均是泛型类

```java
@Getter
@Setter
@NoArgsConstructor
public class PaggingVo<T> {
    private Long total;
    private Integer count;
    private Integer page;
    private Integer total_page;
    // 使用到泛型 因为不止spu一处使用到这个vo 使用泛型要将类名上也要打上泛型
    private List<T> items;
    public PaggingVo(Page<T> pageT) {
        /*
        传入service获取到的Page对象 初始化参数
         */
        this.initPageParamters(pageT);
        this.items = pageT.getContent();
    }
    void initPageParamters(Page<T> pageT){
        this.total = pageT.getTotalElements();
        this.count= pageT.getSize();
        this.page = pageT.getNumber();
        this.total_page = pageT.getTotalPages();
    }

}
```

封装过后的`vo`层

```java
public class PagingDozerVo<T,K> extends PaggingVo {
    @SuppressWarnings("unchecked")//解决错误检查
    public PagingDozerVo(Page<T> pageT,Class<K> classk) {
        /*
          泛型类 构造函数需要完成初始化参数 并且简化JPA返回的items
         */
        this.initPageParamters(pageT);
        // 获取分页返回内容
        List<T> tList = pageT.getContent();
        // 仿造之前写的简化返回值
        Mapper mapper = DozerBeanMapperBuilder.buildDefault();
        // 目标对象voList 这里也应该定义成泛型
        List<K> voList = new ArrayList<>();
        tList.forEach(t->{
            // map接收参数 源 目标元类
             K vo= mapper.map(t,classk);
             voList.add(vo);
        });
        this.setItems(voList);
    }
}
```

最后`controller`依次调用

```java
 @GetMapping("/latest")
    public PagingDozerVo<Spu,SpuSimplifyVo> getLatestSpuList(@RequestParam(defaultValue = "0") Integer start,@RequestParam(defaultValue = "10") Integer count){
        pageCounter pageCounter = CommonUtil.convertStartToPage(start,count);
        Page<Spu> spuPage = spuService.getLatestPagingSpu(pageCounter.getPage(),pageCounter.getCount());
        return new PagingDozerVo(spuPage,SpuSimplifyVo.class);
    }
```

![](https://image.yangxiansheng.top/img/20200506171835.png?imagelist)






###### 根据分类id获取商品

前面铺垫好了方法，就比之前好写多了。这个接口同样是返回分页数据，需要通过传递参数`isroot`判断返回数据是返回一级分类还是二级分类

`jpa`的语法

```markdown
 /*
    JPA 规范 findBy 查找 orderBy 排序  Desc 升序  参数中加入Pageable 返回分页结果前提是定义成Page泛型
    containing 添加模糊查找
     */
```

![](https://image.yangxiansheng.top/img/20200507164608.png?imagelist)

`service`层

```java
public Page<Spu> getListByCid(Integer pageNum,Integer size,Long cid,Boolean isroot){
    Pageable pageable = PageRequest.of(PageNum,size);
    Page<spu> page = null;
    if(isroot){
        page = this.SpuRepository.findAllByCategoryIdOrderByCreateTimeDesc(cid,pageable);
    }{
        page = this.SpuRepository.findAllByRootcategoryIdOrderByCreateTimeDesc(cid,pageable);
    }
    return page;
}
```

```java
 @Positive(message = "{id.positive}")
// 创建ValidationMessageProperties 
写入 id.poisitive = id必须是正整数 
```

###### 关键词搜索商品（/search）

这里就相对简单的多，只需要书写正确的`Jpa`方法即可

```java
// 传入keyword
page<Spu> findByTitleContainingorBySubtitleContainingorByTagsContaining(String keword1,String keyword2,String keyword3,pageable)
```

##### 分类(/category)

##### sku

数据表设计

```
SPU（有多种规格 多个sku）

Spu - Spec_key 多对多  一个Spu规定了多个规格名
    为什么？ 因为  standard 定义这个规格是不是一个标准规格 
    如 颜色， spu1,spu2,spu3 都可以有颜色， 颜色不是单独属于某个spu的，所以是多对多 
    
Sku - Spec_Value 多对多
Spu - Sku 一对多
Sku - Spec_Key  多对多    
Spec_key - Spec_Value 一对多
```

