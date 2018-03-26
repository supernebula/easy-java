# 关键字：

## [JAVA 10](https://docs.oracle.com/javase/specs/jls/se10/html/jls-3.html#jls-3.9)和[C# 7.0](https://docs.microsoft.com/zh-cn/dotnet/csharp/language-reference/keywords/index)语言规范-基础关键字比较:

| JAVA   |<font color=green>C#</font>| JAVA   |<font color=green>C#</font>| JAVA     |<font color=green>C#</font> | JAVA   |<font color=green>C#</font>| JAVA       |<font color=green>C#</font> |
|:-------|-------:|:-------|-------:|:---------|----------:|:-------|--------:|:-----------|----------:|
|abstract|*<font color=green>abstract</font>*|continue|*<font color=green>continue*|for     |*for*     |new     |*new*      |switch      |*switch*|
|assert  |System.Diagnostics.Assert(bool)|default |*<font color=green>default</font>* |if        |*<font color=green>if</font>*      |package |*<font color=green>namespace</font>*|synchronized|*<font color=green>lock</font>*  |
|boolean |*<font color=green>bool</font>*  |do      |*<font color=green>do</font>*      |goto      |*<font color=green>goto</font>*    |private |*<font color=green>private</font>*  |this        |*<font color=green>this</font>*  |
|break   |*<font color=green>break</font>* |double  |*<font color=green>double</font>*  |implements|*<font color=green>:(实现接口)</font>*|protected|*<font color=green>protected</font>*|throw       |*<font color=green>throw</font>*|
|byte    |*<font color=green>byte</font>*  |else    |*<font color=green>else</font>*    |import    |*<font color=green>using</font>*   |public  |*<font color=green>public</font>*   |throws      |方法注释：<br/>&lt;exception cref="Exception"&gt;注释&lt;/exception&gt;         |
|case    |*<font color=green>case</font>*  |enum    |*<font color=green>enum</font>*    |instanceof|*<font color=green>is</font>*      |return  |*<font color=green>return</font>*   |transient   |[Serialization.XmlIgnore]或[JsonIgnore]等特性|
|catch   |*<font color=green>catch</font>* |extends |*<font color=green>:(继承类)</font>*|int       |*<font color=green>int</font>*     |short  |*<font color=green>short</font>*    |try         |*<font color=green>try</font>*     |
|char    |*<font color=green>char</font>* |final   |*<font color=green>const</font>*|interface|*<font color=green>interface</font>*|static  |*<font color=green>static</font>*   |void        |*<font color=green>void</font>*  |
|class   |*<font color=green>class</font>* |finally |*<font color=green>finally</font>* |long      |*<font color=green>long</font>*     |strictfp|         |volatile    |*<font color=green>volatile</font>*|
|const   |*<font color=green>保留字</font></font>*|float   |*<font color=green>float</font>*   |native    |extern?    |super   |*<font color=green>base</font>*     |while       |*<font color=green>while</font>*  |
|_       |_       |        |        |          |          |        |         |           |            |


### JAVA关键字：

| 关键字     |   等价           |   含义      |
|:----------|:-----------------|:------------|
|strictfp   |strict float point|精确浮点      |




## [C#独有关键字:](https://docs.microsoft.com/zh-cn/dotnet/csharp/language-reference/keywords/index)

| C#     |   JAVA       |   C#      |   JAVA       |   C#      |   JAVA     |   C#      |   JAVA     |
|:-------|:-------------|:----------|:-------------|:----------|:-----------|:----------|:-----------|
|abstract|              |as         |              | base       |           |bool       |            |
|break  |               |byte       |              | case       |           |catch      |            |
|char    |              |checked    |              | class      |           |const      |            |
|continue|              |decimal    |              | default    |           |delegate   |            |
|do      |              |double     |              | else       |           |enum       |            |
|event   |              |explicit   |              | extern     |           |false      |            |
|finally |              |fixed      |              | float      |           |for        |            |
|foreach |              |goto       |              | if         |           |implicit   |            |
|in      |              |int        |              | interface  |           |internal   |            |
|is      |              |lock       |              | long       |           |namespace  |            |
|new     |              |null       |              | object     |           |operator   |            |
|out     |              |override   |              | params     |           |private    |            |
|protected|             |public     |              | readonly   |           |ref        |            |
|return  |              |sbyte      |              | sealed     |           |short      |            |
|sizeof  |              |stackalloc |              | static     |           |string     |            |
|struct  |              |switch     |              | this       |           |throw      |            |
|true    |              |try        |              | typeof     |           |uint       |            |
|ulong   |              |unchecked  |              | unsafe     |           |ushort     |            |
|using   |              |using static|             |virtual     |           |void       |            |
|abstract|              |as         |              | base       |           |bool       |            |
|volatile|              |while      |              |            |           |           |            |


## [C#上下文关键字:](https://docs.microsoft.com/zh-cn/dotnet/csharp/language-reference/keywords/index)

| C#                            |   JAVA       |   C#               |   JAVA       |   C#           |   JAVA    |
|:------------------------------|:-------------|:-------------------|:-------------|:---------------|:----------|
|add                            |              |alias               |              | ascending      |           |
|async                          |              |await               |              | descending     |           |
|dynamic                        |              |from                |              | get            |           |
|global                         |              |group               |              | into           |           |
|join                           |              |let                 |              | nameof         |           |
|orderby                        |              |partial (type)      |              | partial(method)|           |
|remove                         |              |select              |              | set            |           |
|value                          |              |var                 |              | yield          |           |
|when (filter condition)        |              |                    |              |                |           |
|where (generic type constraint)|              |                    |              |                |           |
|where (query clause)           |              |                    |              |                |           |

