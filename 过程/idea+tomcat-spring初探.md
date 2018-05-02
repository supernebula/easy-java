

# 教程

## Tomcat

### 下载tomcat

官网下载地址： http://tomcat.apache.org/

### 安装tomcat

1. 将下载的文件解压，复制到 /Library/Tomcat目录下：

```sh
cp -r /Users/jikukalun/Downloads/apache-tomcat-8.0.39/ /Library/Tomcat/tomcat8
```
2. 配置文件权限

安装后，startup.sh 没有运行权限，如下命令配置：
```sh

chmod -R 777  [FolderName]

chmod 777 *.sh  //将文件改为最高权限

```
 startup.sh 就拥有读写运行所有权限了

### 运行

启动命令

```sh
./startup.sh
```

停止命令

```sh
./shutdown.sh
```

## Tomcat相关问题

org.apache.jasper.JasperException: java.lang.IllegalStateException: No output folder: 

关于这个原因主要是权限的问题，在tomcat/work/Catalina/localhost/，主要是这个目录没有被读写的权限，导致文件不能被编译到该指定的工作目录中，此时我们就要针对与这个目录做一些权限的修改权限至少要达到755或者以上，同时注意此处修改权限必须用root身份进行操作，否则不能进行修改，修改完后编译好的jsp文件就在localhost的目录当中了

```sh

chmod -R 777  localhost

```

# 参考资料




[IntelliJ IDEA 教程](https://blog.csdn.net/qq_35246620/article/details/61191375)