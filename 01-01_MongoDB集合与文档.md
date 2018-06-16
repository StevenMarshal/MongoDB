# 1 MongoDB集合与文档

## 1.1 命令“cls”

清屏命令。

## 1.2.	命令“show dbs;”

显示MongoDB有哪些数据库。数据库下放集合，集合下面放文档。  

例如：  

    > show dbs;
    admin   0.000GB
    config  0.000GB
    local   0.000GB

## 1.3 命令“use mydb”  

创建和使用新的数据库“mydb”。  

例如：  

    > use mydb
    switched to db mydb

## 1.4 命令“db;”

显示当前是哪个数据库。  

例如：  

    > db;
    mydb

以上提示当前数据库已经是“mydb”

## 1.5 命令“db.user.insert({})”

其中的“user”在MongoDB中叫集合（collection），而每行数据被叫做一个文档。每条数据插入的是一个“bson”串。  

例如：  

    >db.user.insert({uname:"Jack",pwd:"abc123",height:173,birthday:ISODate("1980-06-28")});
    WriteResult({ "nInserted" : 1 })

## 3.6 命令“show collections;”  

显示数据库中集合的意思。  

例如：  

    > show collections;
    user

## 3.7 命令“db.user.find()”  

查看集合中的数据。  

例如：  

    > db.user.find()
    { "_id" : ObjectId("5b2462fc3dfc34a24def2c28"), "uname" : "Tom", "pwd" : "abc123", "height" : 173, "birthday" : ISODate("1980-06-28T00:00:00Z") }
    { "_id" : ObjectId("5b24637a3dfc34a24def2c29"), "uname" : "Jack", "pwd" : "abc123", "height" : 173, "birthday" : ISODate("1980-06-28T00:00:00Z") }
  