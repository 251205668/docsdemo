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