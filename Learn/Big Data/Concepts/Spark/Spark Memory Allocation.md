##### Tags: #spark

##### Spark Driver Memory
To setup the drive memory there 2  [[Spark Configuration Properties]] the total sum of the Driver container is equal to the requested memory plus its **10%** or **384 MB** what ever is higher.


##### Spark Executor Memory
The total executor memory is the result of the sum of this [[Spark Configuration Properties]]:
 - spark.executor.memory.OverHead
- spark.executor.memory 
- spark.memory.offHeap.size 
- spark.executor.pyspark.memory 

Please do a deep look at **memory fractions** in spark, noticed you wont be able to allocate more memory than the default allow by the [[Resource Mangers]]


