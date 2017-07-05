DFSIO enhanced test code from HiBench github with updates to run on ADLS

Sample Run:

hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=adl://dfsiotest.azuredatalakestore.net/dfsio -write -nrFiles 30 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal
