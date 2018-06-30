# 对比 [C# 7.0](https://docs.microsoft.com/zh-cn/dotnet/csharp/language-reference/keywords/index) 和 [JAVA 10](https://docs.oracle.com/javase/specs/jls/se10/html/jls-3.html#jls-3.9) 语言规范

## 关键字 JAVA --> C#:

| JAVA   |<font color=green>C#等价</font>| JAVA   |<font color=green>C#等价</font>| JAVA     |<font color=green>C#等价</font> | JAVA   |<font color=green>C#等价</font>| JAVA       |<font color=green>C#等价</font> |
|:-------|-------:|:-------|-------:|:---------|----------:|:-------|--------:|:-----------|----------:|
|abstract|*<font color=green>abstract</font>*|continue|*<font color=green>continue*|for     |*for*     |new     |*new*      |switch      |*switch*|
|assert  |System.Diagnostics.Assert(bool)|default |*<font color=green>default</font>* |if        |*<font color=green>if</font>*      |package |*<font color=green>namespace</font>*|synchronized|*<font color=green>lock</font>*  |
|boolean |*<font color=green>bool</font>*  |do      |*<font color=green>do</font>*      |goto(不支持)|*<font color=green>goto</font>*    |private |*<font color=green>private</font>*  |this        |*<font color=green>this</font>*  |
|break   |*<font color=green>break</font>* |double  |*<font color=green>double</font>*  |implements|*<font color=green>:(实现接口)</font>*|protected|*<font color=green>protected</font>*|throw       |*<font color=green>throw</font>*|
|byte    |*<font color=green>byte</font>*  |else    |*<font color=green>else</font>*    |import    |*<font color=green>using</font>*   |public  |*<font color=green>public</font>*   |throws      |方法注释：<br/>&lt;exception cref="Exception"&gt;注释&lt;/exception&gt;         |
|case    |*<font color=green>case</font>*  |enum    |*<font color=green>enum</font>*    |instanceof|*<font color=green>is</font>*      |return  |*<font color=green>return</font>*   |transient   |[Serialization.XmlIgnore]或[JsonIgnore]等特性|
|catch   |*<font color=green>catch</font>* |extends |*<font color=green>:(继承类)</font>*|int       |*<font color=green>int</font>*     |short  |*<font color=green>short</font>*    |try         |*<font color=green>try</font>*     |
|char    |*<font color=green>char</font>* |final   |*<font color=green>const</font>*|interface|*<font color=green>interface</font>*|static  |*<font color=green>static</font>*   |void        |*<font color=green>void</font>*  |
|class   |*<font color=green>class</font>* |finally |*<font color=green>finally</font>* |long      |*<font color=green>long</font>*     |strictfp|         |volatile    |*<font color=green>volatile</font>*|
|const   |*<font color=green>保留字</font></font>*|float   |*<font color=green>float</font>*   |native    |extern?    |super   |*<font color=green>base</font>*     |while       |*<font color=green>while</font>*  |
|_       |_       |        |        |          |          |        |         |           |            |


JAVA关键字：

strictfp 即  strict float point //精确浮点

## 关键字 C# 7.0 --> JAVA 10

| C#     |   JAVA等价   |   C#      |   JAVA等价   |   C#       |   JAVA等价  |   C#      |   JAVA等价 |
|:-------|-------------:|:----------|-------------:|:-----------|-----------:|:----------|----------:|
|abstract|abstract      |as         |无            | base       |super      |bool       |boolean     |
|break   |break         |byte       |byte          | case       |case       |catch      |catch       |
|char    |char          |checked    |              | class      |class      |const      |final       |
|continue|continue      |decimal    |BigDecimal?   | default    |default    |delegate   |Delegate?   |
|do      |do            |double     |double        | else       |else       |enum       |enum        |
|event   |              |explicit   |              | extern     |native?    |false      |false?      |
|finally |finally       |fixed      |              | float      |float      |for        |for         |
|foreach |              |goto       |goto          | if         |if         |implicit   |            |
|in      |              |int        |int           | interface  |interface  |internal   |            |
|is      |instanceof    |lock       |synchronized  | long       |long       |namespace  |package     |
|new     |new           |null       |              | object     |           |operator   |            |
|out     |              |override   |              | params     |           |private    |private     |
|protected|protected    |public     |public        | readonly   |           |ref        |            |
|return  |return        |sbyte      |              | sealed     |           |short      |short       |
|sizeof  |              |stackalloc |              | static     |static     |string     |            |
|struct  |              |switch     |switch        | this       |this       |throw      |throw       |
|true    |true          |try        |try           | typeof     |           |uint       |            |
|ulong   |              |unchecked  |              | unsafe     |           |ushort     |            |
|using   |import        |using static|             |virtual     |           |void       |void        |
|volatile|volatile      |while      |while         |            |           |           |            |


## C#上下文关键字: C# 7.0 --> JAVA 10

| C#                            |   JAVA       |   C#               |   JAVA       |   C#           |   JAVA    |
|:------------------------------|:-------------|:-------------------|:-------------|:----------------|:----------|
|add (+=)                       |              |alias               |              | ascending (linq)|           |
|async                          |              |await               |              | descending (linq)|           |
|dynamic                        |              |from (linq)         |              | get             |           |
|global                         |              |group (linq)        |              | into (linq)     |           |
|join (linq)                    |              |let                 |              | nameof          |           |
|orderby (linq)                 |              |partial (type)      |              | partial(method) |           |
|remove (-=)                    |              |select (linq)       |              | set             |           |
|value                          |              |var                 |              | yield           |           |
|when (filter condition)        |              |                    |              |                 |           |
|where (generic type constraint)|              |                    |              |                 |           |
|where (query clause)           |              |                    |              |                 |           |



## 参考：C#（针对 Java 开发人员）

[MSDN C# 编程语言（针对 Java 开发人员）](https://docs.microsoft.com/zh-cn/previous-versions/visualstudio/visual-studio-2008/ms228602%28v%3dvs.90%29)

[MSDN C# 代码示例（针对 Java 开发人员）](https://docs.microsoft.com/zh-cn/previous-versions/visualstudio/visual-studio-2008/ms228363%28v%3dvs.90%29)

[MSDN C# 应用程序类型（针对 Java 开发人员）](https://docs.microsoft.com/zh-cn/previous-versions/visualstudio/visual-studio-2008/ms228501%28v%3dvs.90%29)