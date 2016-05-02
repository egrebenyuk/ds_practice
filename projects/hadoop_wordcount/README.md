## <a href="https://amodernstory.com/2014/09/23/hadoop-on-mac-osx-yosemite-part-2/">Creating Hadoop’s Wordcount Program</a>

---


### compile
javac WordCount.java

### create jar (http://www.skylit.com/javamethods/faqs/createjar.html):
jar cvfe WordCount.jar WordCount *.class

### upload
hadoop fs -copyFromLocal book.txt hdfs:/inputA
hadoop fs -ls hdfs:/inputA

### count
hadoop jar WordCount.jar hdfs:/inputA hdfs:/outputA
hadoop fs -ls hdfs:/outputA

### download result
hadoop fs -copyToLocal hdfs:/outputA/part-00000 
