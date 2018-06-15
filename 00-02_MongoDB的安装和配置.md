# 2 MongoDB的安装和配置

## 2.1 MongoDB下载和安装

MongoDB的官方网址：  

    https://www.mongodb.com  

MongoDB的下载地址：  

    https://www.mongodb.com/download-center?jmp=nav  

安装完成以后，在安装目录的版本号文件夹中创建两个新文件夹：  
1：“data”文件夹用来放置将来的数据文件。  
2：“log”文件夹用来存放日志文件。  
在“log”文件夹中可以新建一个文件“MongoDB.log”。  

## 2.2 启动MongoDB服务

两个非常重要的启动服务命令：  

    mongod ——dbpath “C:\MongoDB\Server\3.6\data”

    mongod ——bind_ip 127.0.0.1 ——port 27017 ——logpath “C:\ MongoDB\Server\3.6\log\MongoDB.log” ——serviceName “MongoDB” ——install  

注：在安装目录的bin目录下执行该两条命令。

## 2.3 启动MongoDB客户端  

在命令行窗口中进入MongoDB的bin目录下，执行“mongo”命令则进入MongoDB的客户端服务。  

## 2.4 安装成功验证  

安装成功验证命令为：“show dbs:”  
利用Ctrl + c 进行退出。
