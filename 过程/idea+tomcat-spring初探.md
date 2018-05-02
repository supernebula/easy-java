

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

# 参考资料




[IntelliJ IDEA 教程](https://blog.csdn.net/qq_35246620/article/details/61191375)