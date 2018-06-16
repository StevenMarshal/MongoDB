# 2 bson与json对比

* json  

英文全称：JavaScript Object Notation。  
key:value结构的字符串。  
json与 XML对应，是网络传输的重要数据格式。  

* bson  

Binary Serialized Document Format。  
json所有数据都是字符型，bson有整型、日期型等。   
bson有三个特点：轻量型、可遍历性、高效性。  

最大的区别就是bson串中是有数据类型的，而且bson是无模式的，也就是说在原有基础上可以很轻易的加上一列数据。另外在读取bson串时的读写效率非常高。
