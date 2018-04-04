
# 《JAVA核心技术 卷1 基础知识》读书笔记

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



