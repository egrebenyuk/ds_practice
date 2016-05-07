## <a href="https://amodernstory.com/2014/09/23/hadoop-on-mac-osx-yosemite-part-2/">Creating Hadoop’s Wordcount Program</a>

---


### compile
<code>javac WordCount.java</code>

### create jar (http://www.skylit.com/javamethods/faqs/createjar.html):
<code>jar cvfe WordCount.jar WordCount *.class</code>

### upload
<code>hadoop fs -copyFromLocal book.txt hdfs:/input</code>
<code>hadoop fs -ls hdfs:/input</code>

### count
<code>hadoop jar WordCount.jar hdfs:/input hdfs:/output</code>
<code>hadoop fs -ls hdfs:/output</code>

### download result
<code>hadoop fs -copyToLocal hdfs:/output/part-00000</code>
