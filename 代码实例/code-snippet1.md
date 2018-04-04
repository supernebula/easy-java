# JAVA基础

## 第三章JAVA集成程序设计结构

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

#### 通用注释

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



