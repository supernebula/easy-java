## 1.在MAC上.sh command not found
场景：下载并运行tomcat/bin/, 在终端运行startup.sh，显示无权限：

``` java
user1$ ./startup.sh
-bash: ./startup.sh: Permission denied
```

解决办法：修改startup.sh文件的权限

```java
user1$  cd /tomcat8.5/bin
user1$  chmod u+x *.sh
```
执行后

```java
pctel:bin evol$ chmod u+x *sh
pctel:bin evol$ ./startup.sh 
Using CATALINA_BASE:   /Users/evol/Library/Tomcat/tomcat8.5
Using CATALINA_HOME:   /Users/evol/Library/Tomcat/tomcat8.5
Using CATALINA_TMPDIR: /Users/evol/Library/Tomcat/tomcat8.5/temp
Using JRE_HOME:        /Library/Java/JavaVirtualMachines/jdk1.8.0_152.jdk/Contents/Home
Using CLASSPATH:       /Users/evol/Library/Tomcat/tomcat8.5/bin/bootstrap.jar:/Users/evol/Library/Tomcat/tomcat8.5/bin/tomcat-juli.jar
Tomcat started.
```

启动Tomcat成功！
