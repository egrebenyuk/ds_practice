## <a href="https://amodernstory.com/2014/09/23/hadoop-on-mac-osx-yosemite-part-2/">Creating Hadoop’s Wordcount Program</a>

---


### compile
javac WordCount.java

### create jar (http://www.skylit.com/javamethods/faqs/createjar.html):
jar cvfe WordCount.jar WordCount *.class

### upload
hadoop fs -copyFromLocal book.txt hdfs:/input
hadoop fs -ls hdfs:/input

### count
hadoop jar WordCount.jar hdfs:/input hdfs:/output
hadoop fs -ls hdfs:/output

### download result
hadoop fs -copyToLocal hdfs:/output/part-00000 
