C#和JAVA语言规范比较

JAVA关键字，引用自[Java10](https://docs.oracle.com/javase/specs/jls/se10/html/jls-3.html#jls-3.9)

| java   | c#     | java   | c#     | java     | c#        | java   | c#      | java       | c#       |
|:-------|:-------|:-------|:-------|:---------|:----------|:-------|:--------|:-----------|:----------|
|abstract|abstract|continue|continue|for       |for       |new     |new      |switch      |switch     |
|assert  |        |default |default |if        |if        |package |namespace|synchronized|lock       |
|boolean |bool    |do      |do      |goto      |goto      |private |private  |this        |this       |
|break   |break   |double  |double  |implements|: 实现接口|protected|protected|throw       |throw      |
|byte    |byte    |else    |else    |import    |using     |public  |public   |throws      |           |
|case    |case    |enum    |enum    |instanceof|as        |return  |return   |transient   |           |
|catch   |catch   |extends |:(继承类)|int       |int       |short  |short    |try         |try        |
|char    |char    |final   |readonly?|interface|interface |static  |static   |void        |void       |
|class   |class   |finally |finally |long      |long      |strictfp|         |volatile    |volatile?  |
|const   |const?  |float   |float   |native    |          |super   |base     |while       |while      |
|_       |_       |        |        |          |          |        |         |           |            |

JAVA另外：
strictfp, 即 strict float point (精确浮点)
