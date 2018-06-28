## 3.5 Java开发MongoDB驱动  

MongoDB的Java开发相关下载地址：  

    http://mongodb.github.io/mongo-java-driver/

选择相应的驱动和版本后，点击左上角的“download”。

![下载图示](images/xiazaitushi.jpg)
 
在下载驱动列表中选择相应的驱动：

    “mongo-java-driver-3.6.4.jar”
 
相关的两个jar包为：

    mongo-java-driver-3.6.4.jar
    mongodb-driver-core-3.6.4.jar

编写Java普通项目的main方法进行连接验证如下：  

    public class Test {

	    public static void main(String[] args){
		
		    MongoClientURI uri = new MongoClientURI("mongodb://xiaohp:123456@localhost:27017/mydb");
		    MongoClient client = new MongoClient(uri);
		    MongoDatabase db = client.getDatabase("mydb");
		    MongoCollection<Document> collection = db.getCollection("user");
		
		    System.out.println(collection.count());
		
		    client.close();
	    }
    }
