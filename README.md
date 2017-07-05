DFSIO tests from HiBench github (https://github.com/intel-hadoop/HiBench)  with updates to run on ADLS and WASB

Compile:
mvn clean package

Sample Runs:

ADLS

Write:
hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=adl://dfsiotest.azuredatalakestore.net/dfsio -write -nrFiles 10 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal -bufferSize 4096

Read: 
hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=adl://dfsiotest.azuredatalakestore.net/dfsio -read -nrFiles 10 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal -buff
erSize 4096 

WASB

Write:
hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=wasb://dfsiotest@dfsio.blob.core.windows.net/dfsio -write -nrFiles 10 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal -bufferSize 4096

Read:
hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=wasb://dfsiotest@dfsio.blob.core.windows.net/dfsio -read -nrFiles 10 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal -bufferSize 4096
