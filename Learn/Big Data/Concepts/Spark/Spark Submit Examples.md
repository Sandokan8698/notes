##### Tags: #spark, #spark-submit

`spark-submit --master  spark://192.168.100.79:7077 --deploy-mode cluster \ 
`--conf spark.executor.memory=3g \
`--conf spark.driver.memory=6g --conf spark.driver.maxResultSize=10g \`
`--conf spark.driver.extraJavaOptions=-XX:+HeapDumpOnOutOfMemoryError \`
`--class org.damg.agiledatacode.examples.DriverOOm ./processor/target/processor-1.0-SNAPSHOT.jar On_Time_On_Time_Performance_2015.csv`