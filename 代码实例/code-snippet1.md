
# JAVA核心技术 卷1 基础知识

参考C#，只记录重点部分

#### 大数值(任意长度／精度数值序列)

```java
import java.mach;
//BigInteger
//BigDecimal
///普通数值转大数值
BigInteger num = BigInteger.ValOf(100);

//JAVA不提供运算重载，所有不能使用+ 、 - 、*符号
Biglnteger c = a.add(b); // c = a + b
Biglnteger d = c.nultipiy(b.add(Biglnteger.valueOf(2))); // d = c * (b + 2)
```

#### for each

```java
//简化版,collection必须实现Iterable接口
for (int element : collection) 
    System.out.println(element);

//完整版
for (int i = 0; i < collect.length; i++)
 System,out.println(collect[i]);

```

#### 静态导入

``` java
import static java.lang.*;
//缺陷！不利于代码清晰度
//就可以使用 System 类的静态方法和静态域， 而不必加类名前缀:
out.println("Goodbye, World!"); // i.e., System.out
exit(9); //i.

```

#### 注释

```java

public class TestClass{
    /**
    * Raises the salary of an employee.
    * @param byPercent the percentage by which to raise the salary (e.g. 10 means 10%) 
    * ©return the amount of the ra
    * ©return the amount of the raise
    *／

    public double raiseSalary(double byPercent) {
        double raise = salary * byPercent / 100; salary += raise;
        return raise;
    }
}
```

#### 通用注释

@author 

作者姓名

@version 

版本

@sinee 

始于， 例如 ©since version 1.7.10

@deprecated

这个标记将对类、方法或变量添加一个不再使用的注释。 文本中给出了取代的建议。 例如，
@deprecated Use <code> setVIsible(true) </code> instead

@see 

引用

@link 

标记， 可以使用超级链接， 链接到 javadoc 文档的相关部分或外
部文档


#### 继承类  和 实现接口

```java

public class Manager extends Employee implements Iinterface{
    //添加方法和域 
}

```

#### lambda表达式

```java

(String first, String second) ->
{ 
    if (first.length() < second.length()) 
        return -1; 
    else if (first.length() > second.length()) 
        return 1;
//即使 lambda 表达式没有参数， 仍然要提供空括号， 就像无参数方法一样:
    else 
        return 0; 
}

```

#### 异常

所有的异常都是由 Throwable 继承而来， 但在下一层立即分解为两个分 支:Error 和 Exception

Throwable

 |-----Error  : 描述了 Java 运行时系统的内部错误和资源耗尽错误

 |-----Exception (RuntimeException、 其他异常)

 ```java
//throws关键字，声明受查异常
public Fi1elnputStream(String name) throws FileNotFoundException
 ```

#### JAVA断言

```java
//断言方式一  assert 条件;

assert x >= 0;

//断言方式二  assert 条件 : 表达式; 例如：
assert x >= 0 : x;
//如果结果为 false, 则抛出一个 AssertionError 异常,将 x 的实际值传递给 AssertionError 对象
```

启用和禁用断言

在默认情况下， 断言被禁用。可以在运行程序时用 -enableassertions 或 -ea 选项启用: java -enableassertions MyApp

#### 日志？

保留疑问？

#### 范型-通配符类型

通配符类型中， 允许类型参数变化。 

```java
//例如，通配符类型,?是 Employee 的子类
Pair<? extends Employee〉

//通配符的超类型限定
//指定一个超 类型限定(supertypebound), 如下所亦:
? super Manager

 //例如， Pair<? super Manager> 有方法
void setFirst(? super Manager) 

? super Manager getFirst()

```

#### 范型-无限定通配符

````java
//还可以使用无限定的通配符， 例如，Pair<?>
? getFirst() 
void setFirst(?)

//可以调用 setFirst(null)
````

#### 通配符捕获？

保留疑问？


#### 反射和范型？

保留疑问？


#### 集合 - 接口 - 队列 Queue<>

```java
// a simplified form of the interface in the standard library
public interface Queue<E> 
{
    void add(E element); E remove();
    int size();
}

//队列通常有两种实现方式: 一种是使用循环数组; 另一种是使用链表
```

#### 集合 - 接口 - 集合 Collection<>

```java
public interface Collection<E>
{
    boolean add(E element); 
    Iterator<E> iterator(); //Iterator 迭代器接口
    ...
}
```

#### 集合 - 接口 - 迭代器 Iterator<>

```java
public interface Iterator<E>
{
    E next();
    boolean hasNext();
    void remove();
    //传入lambda 表达式,依次处理每一个元素
    default void forEachRemaining(Consumer<? super E> action);
}
```

#### 集合 - 接口 - 泛型实用方法

```java

public static <E> boolean contains(Collection<E> c, Object obj)
{
    for (E element : c)
        if (element,equals(obj)) 
            return true;
    return false; 
}
```

#### 集合 - 集合框架中的接口 ？

保留疑问？


#### 集合 - 链表 ？

保留疑问？

#### 集合 - 散列集合 ？

保留疑问？

#### 集合 - 树集 ？

保留疑问？

#### 集合 - 队列和双端队列 ？

保留疑问？


#### 集合 - 优先级队列 ？

保留疑问？

#### 集合 - 映射 - HashMap？

保留疑问？

#### 集合 - 映射 - TreeMap ？

保留疑问？

#### 集合 - 算法？

保留疑问？

排序与混排、二分查找、简单算法、批操作、集合与数组的转换

#### 遗留的集合

Hashtable、枚举 Enumeration、栈 Stack、位集、BitSet

#### 图形程序设计、Swing用户界面组件？

Swing、处理2D图形..... 保留疑问？

#### 事件处理

主要：图形见面处理，保留疑问？

#### 部署JAVA应用程序

#### 部署 - JAR文件

JAR : java归档文件。包含：类文件，图像、声音等其他类型的文件；

JAR文件是压缩的，zip格式。

#### 部署 - JAR - 创建JAR文件

命令格式：

```java

 jar cvf JARFileNameFile File2 . . . :

 例如：
jar cvf CalculatorClasses.jar *.class icon.gif

通常，jar 命令的格式如下: 

jar options File File2 . . .

 ```


#### 部署 - JAR - 清单文件

除了类文件、图像和其他资源外， 每个 JAR 文件还包含一个用于描述归档特征的清单文 件 (manifest。)

被命名为 MANIFEST.MF , 它位于 JAR 文件的一个特殊 META-INF 子目录中.

#### 部署 - JAR - 可执行JAR包？

保留疑问？


#### 部署 - 资源？

保留疑问

#### 部署 - 应用首选项的存储？

保留疑问？

#### 部署 - 服务加载器？

保留疑问？

#### 并发？

保留疑问？
线程、中断线程、线程状态、线程属性、同步、阻塞队列、线程安全的集合、Callable与Future

#### 并发 - 线程安全集合

所属包

```java
import java.util.concurrent;

//java.util.concurrent 包提供了映射、 有序集和队列的高效实现: 
ConcurrentHashMap
ConcurrentSkipListMap
ConcurrentSkipListSet
ConcurrentLinkedQueue

//JavaSE 8 引入了一个 mappingCount 方法可以把大小作为 long 返回


```













