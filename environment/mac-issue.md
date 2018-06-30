## mac 安装 tomcat 8.x

下载 https://tomcat.apache.org/

新建 Finder，按快捷键 shift + command + g 打开前往指定目录对话框

输入 ~／Library 进入当前用户Library目录，解压tomcat压缩包并复制到该目录；

进入 Users/user1/Library/tomcat/bin

运行 startup.sh 启动Tomcat

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

浏览器访问： http://http://127.0.0.1:8080/

命令行访问：curl http://127.0.0.1:8080
