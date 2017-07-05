DFSIO enhanced test code from HiBench github with updates to run on ADLS

Sample Run:

hadoop jar dfs-tests-1.0-SNAPSHOT-jar-with-dependencies.jar org.apache.dfs.test.TestDFSIOEnh -Dtest.build.data=adl://dfsiotest.azuredatalakestore.net/dfsio -write -nrFiles 30 -fileSize 2000  -plotInteval 1000 -sampleUnit m -sampleInteval 200 -sumThreshold 0.5 -tputReportTotal
TestFDSIO.0.0.4 Enhanced Version
17/07/05 16:13:59 INFO test.TestDFSIOEnh: nrFiles = 30
17/07/05 16:13:59 INFO test.TestDFSIOEnh: fileSize (MB) = 2000
17/07/05 16:13:59 INFO test.TestDFSIOEnh: bufferSize = 4000000
17/07/05 16:13:59 INFO test.DfsioeConfig: Found 'test.build.data' in Hadoop configuration, value is 'adl://dfsiotest.azuredatalakestore.net/dfsio'
17/07/05 16:13:59 INFO test.DfsioeConfig: Setting testRootDir to 'adl://dfsiotest.azuredatalakestore.net/dfsio'
17/07/05 16:14:00 INFO client.AHSProxy: Connecting to Application History server at headnodehost/10.0.0.24:10200
17/07/05 16:14:00 INFO client.RequestHedgingRMFailoverProxyProvider: Looking for the active RM in [rm1, rm2]...
17/07/05 16:14:00 INFO client.RequestHedgingRMFailoverProxyProvider: Found active RM [rm1]
17/07/05 16:14:00 INFO test.TestDFSIOEnh: maximum concurrent maps = 20
17/07/05 16:14:00 INFO test.TestDFSIOEnh: creating control file: 2000 mega bytes, 30 files
17/07/05 16:14:01 INFO zlib.ZlibFactory: Successfully loaded & initialized native-zlib library
17/07/05 16:14:01 INFO compress.CodecPool: Got brand-new compressor [.deflate]
17/07/05 16:14:10 INFO test.TestDFSIOEnh: created control files for: 30 files
17/07/05 16:14:10 INFO client.AHSProxy: Connecting to Application History server at headnodehost/10.0.0.24:10200
17/07/05 16:14:10 INFO client.AHSProxy: Connecting to Application History server at headnodehost/10.0.0.24:10200
17/07/05 16:14:10 INFO client.RequestHedgingRMFailoverProxyProvider: Looking for the active RM in [rm1, rm2]...
17/07/05 16:14:10 INFO client.RequestHedgingRMFailoverProxyProvider: Found active RM [rm1]
17/07/05 16:14:12 INFO mapred.FileInputFormat: Total input paths to process : 30
17/07/05 16:14:12 INFO mapreduce.JobSubmitter: number of splits:30
17/07/05 16:14:12 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1498841784082_0024
17/07/05 16:14:13 INFO impl.YarnClientImpl: Submitted application application_1498841784082_0024
17/07/05 16:14:13 INFO mapreduce.Job: The url to track the job: http://hn0-testdfsio.riw1dcq23.gx.internal.cloudapp.net:8088/proxy/application_1498841784082_0024/
17/07/05 16:14:13 INFO mapreduce.Job: Running job: job_1498841784082_0024
17/07/05 16:14:21 INFO mapreduce.Job: Job job_1498841784082_0024 running in uber mode : false
17/07/05 16:14:21 INFO mapreduce.Job:  map 0% reduce 0%
17/07/05 16:14:33 INFO mapreduce.Job:  map 13% reduce 0%
17/07/05 16:14:34 INFO mapreduce.Job:  map 22% reduce 0%
17/07/05 16:14:35 INFO mapreduce.Job:  map 24% reduce 0%
17/07/05 16:14:36 INFO mapreduce.Job:  map 27% reduce 0%
17/07/05 16:14:37 INFO mapreduce.Job:  map 29% reduce 0%
17/07/05 16:14:38 INFO mapreduce.Job:  map 33% reduce 0%
17/07/05 16:14:39 INFO mapreduce.Job:  map 36% reduce 0%
17/07/05 16:14:40 INFO mapreduce.Job:  map 40% reduce 0%
17/07/05 16:14:41 INFO mapreduce.Job:  map 44% reduce 0%
17/07/05 16:14:42 INFO mapreduce.Job:  map 47% reduce 0%
17/07/05 16:14:43 INFO mapreduce.Job:  map 56% reduce 0%
17/07/05 16:14:50 INFO mapreduce.Job:  map 60% reduce 0%
17/07/05 16:14:51 INFO mapreduce.Job:  map 61% reduce 0%
17/07/05 16:14:52 INFO mapreduce.Job:  map 67% reduce 0%
17/07/05 16:14:53 INFO mapreduce.Job:  map 72% reduce 0%
17/07/05 16:14:54 INFO mapreduce.Job:  map 73% reduce 0%
17/07/05 16:14:57 INFO mapreduce.Job:  map 74% reduce 0%
17/07/05 16:14:58 INFO mapreduce.Job:  map 77% reduce 0%
17/07/05 16:15:00 INFO mapreduce.Job:  map 78% reduce 0%
17/07/05 16:15:01 INFO mapreduce.Job:  map 81% reduce 0%
17/07/05 16:15:05 INFO mapreduce.Job:  map 81% reduce 14%
17/07/05 16:15:13 INFO mapreduce.Job:  map 83% reduce 14%
17/07/05 16:15:14 INFO mapreduce.Job:  map 88% reduce 17%
17/07/05 16:15:15 INFO mapreduce.Job:  map 91% reduce 17%
17/07/05 16:15:16 INFO mapreduce.Job:  map 92% reduce 17%
17/07/05 16:15:17 INFO mapreduce.Job:  map 94% reduce 26%
17/07/05 16:15:19 INFO mapreduce.Job:  map 99% reduce 26%
17/07/05 16:15:20 INFO mapreduce.Job:  map 100% reduce 30%
17/07/05 16:15:23 INFO mapreduce.Job:  map 100% reduce 70%
17/07/05 16:15:26 INFO mapreduce.Job:  map 100% reduce 75%
17/07/05 16:15:29 INFO mapreduce.Job:  map 100% reduce 82%
17/07/05 16:15:32 INFO mapreduce.Job:  map 100% reduce 87%
17/07/05 16:15:35 INFO mapreduce.Job:  map 100% reduce 92%
17/07/05 16:15:38 INFO mapreduce.Job:  map 100% reduce 97%
17/07/05 16:15:40 INFO mapreduce.Job:  map 100% reduce 100%
17/07/05 16:15:41 INFO mapreduce.Job: Job job_1498841784082_0024 completed successfully
17/07/05 16:15:42 INFO mapreduce.Job: Counters: 54
	File System Counters
		ADL: Number of bytes read=4820
		ADL: Number of bytes written=386084352
		ADL: Number of read operations=95
		ADL: Number of large read operations=0
		ADL: Number of write operations=2
		FILE: Number of bytes read=387620799
		FILE: Number of bytes written=780106253
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		WASB: Number of bytes read=59730
		WASB: Number of bytes written=62914560000
		WASB: Number of read operations=0
		WASB: Number of large read operations=0
		WASB: Number of write operations=0
	Job Counters
		Launched map tasks=30
		Launched reduce tasks=1
		Rack-local map tasks=30
		Total time spent by all maps in occupied slots (ms)=5367516
		Total time spent by all reduces in occupied slots (ms)=182364
		Total time spent by all map tasks (ms)=1341879
		Total time spent by all reduce tasks (ms)=45591
		Total vcore-milliseconds taken by all map tasks=1341879
		Total vcore-milliseconds taken by all reduce tasks=45591
		Total megabyte-milliseconds taken by all map tasks=10992672768
		Total megabyte-milliseconds taken by all reduce tasks=373481472
	Map-Reduce Framework
		Map input records=30
		Map output records=306911
		Map output bytes=386393677
		Map output materialized bytes=387620973
		Input split bytes=3860
		Combine input records=0
		Combine output records=0
		Reduce input groups=306737
		Reduce shuffle bytes=387620973
		Reduce input records=306911
		Reduce output records=306737
		Spilled Records=613822
		Shuffled Maps =30
		Failed Shuffles=0
		Merged Map outputs=30
		GC time elapsed (ms)=323093
		CPU time spent (ms)=2104200
		Physical memory (bytes) snapshot=102345031680
		Virtual memory (bytes) snapshot=275412520960
		Total committed heap usage (bytes)=115232735232
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters
		Bytes Read=4820
	File Output Format Counters
		Bytes Written=386084352
17/07/05 16:15:42 INFO test.TestDFSIOEnh: ----- TestDFSIO ----- : write
17/07/05 16:15:42 INFO test.TestDFSIOEnh:            Date & time: Wed Jul 05 16:15:42 UTC 2017
17/07/05 16:15:42 INFO test.TestDFSIOEnh:        Number of files: 30
17/07/05 16:15:42 INFO test.TestDFSIOEnh: Total MBytes processed: 60000
17/07/05 16:15:42 INFO test.TestDFSIOEnh:      Throughput mb/sec: 52.39094824123587
17/07/05 16:15:42 INFO test.TestDFSIOEnh: Average IO rate mb/sec: 57.26332092285156
17/07/05 16:15:42 INFO test.TestDFSIOEnh:  IO rate std deviation: 18.106745029363655
17/07/05 16:15:42 INFO test.TestDFSIOEnh:     Test exec time sec: 92.024
17/07/05 16:15:42 INFO test.TestDFSIOEnh:
17/07/05 16:15:42 INFO test.TestDFSIOEnh: -- Extended Metrics --   : write
17/07/05 16:15:42 INFO test.TestDFSIOEnh: Result file name         : TestDFSIOEnh_Tput.csv
17/07/05 16:15:42 INFO test.TestDFSIOEnh: Sampling overhead        : 2.8440428%
17/07/05 16:15:42 INFO test.TestDFSIOEnh: Reference Start Time     : 1499271250145
17/07/05 16:15:42 INFO client.AHSProxy: Connecting to Application History server at headnodehost/10.0.0.24:10200
17/07/05 16:15:42 INFO client.RequestHedgingRMFailoverProxyProvider: Looking for the active RM in [rm1, rm2]...
17/07/05 16:15:42 INFO client.RequestHedgingRMFailoverProxyProvider: Found active RM [rm1]
17/07/05 16:15:44 INFO input.FileInputFormat: Total input paths to process : 1
17/07/05 16:15:44 INFO mapreduce.JobSubmitter: number of splits:2
17/07/05 16:15:44 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1498841784082_0025
17/07/05 16:15:44 INFO impl.YarnClientImpl: Submitted application application_1498841784082_0025
17/07/05 16:15:44 INFO mapreduce.Job: The url to track the job: http://hn0-testdfsio.riw1dcq23.gx.internal.cloudapp.net:8088/proxy/application_1498841784082_0025/
17/07/05 16:15:44 INFO mapreduce.Job: Running job: job_1498841784082_0025
17/07/05 16:15:52 INFO mapreduce.Job: Job job_1498841784082_0025 running in uber mode : false
17/07/05 16:15:52 INFO mapreduce.Job:  map 0% reduce 0%
17/07/05 16:16:02 INFO mapreduce.Job:  map 29% reduce 0%
17/07/05 16:16:05 INFO mapreduce.Job:  map 50% reduce 0%
17/07/05 16:16:06 INFO mapreduce.Job:  map 66% reduce 0%
17/07/05 16:16:08 INFO mapreduce.Job:  map 74% reduce 0%
17/07/05 16:16:11 INFO mapreduce.Job:  map 82% reduce 0%
17/07/05 16:16:14 INFO mapreduce.Job:  map 83% reduce 0%
17/07/05 16:16:18 INFO mapreduce.Job:  map 100% reduce 0%
17/07/05 16:16:19 INFO mapreduce.Job:  map 100% reduce 17%
17/07/05 16:16:22 INFO mapreduce.Job:  map 100% reduce 44%
17/07/05 16:16:25 INFO mapreduce.Job:  map 100% reduce 61%
17/07/05 16:16:28 INFO mapreduce.Job:  map 100% reduce 69%
17/07/05 16:16:31 INFO mapreduce.Job:  map 100% reduce 73%
17/07/05 16:16:34 INFO mapreduce.Job:  map 100% reduce 77%
17/07/05 16:16:37 INFO mapreduce.Job:  map 100% reduce 81%
17/07/05 16:16:40 INFO mapreduce.Job:  map 100% reduce 86%
17/07/05 16:16:43 INFO mapreduce.Job:  map 100% reduce 89%
17/07/05 16:16:46 INFO mapreduce.Job:  map 100% reduce 93%
17/07/05 16:16:49 INFO mapreduce.Job:  map 100% reduce 98%
17/07/05 16:16:50 INFO mapreduce.Job:  map 100% reduce 100%
17/07/05 16:16:52 INFO mapreduce.Job: Job job_1498841784082_0025 completed successfully
17/07/05 16:16:52 INFO mapreduce.Job: Counters: 54
	File System Counters
		ADL: Number of bytes read=386215424
		ADL: Number of bytes written=100246
		ADL: Number of read operations=9
		ADL: Number of large read operations=0
		ADL: Number of write operations=2
		FILE: Number of bytes read=569396046
		FILE: Number of bytes written=1139264078
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		WASB: Number of bytes read=396
		WASB: Number of bytes written=0
		WASB: Number of read operations=0
		WASB: Number of large read operations=0
		WASB: Number of write operations=0
	Job Counters
		Launched map tasks=2
		Launched reduce tasks=1
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=144812
		Total time spent by all reduces in occupied slots (ms)=165096
		Total time spent by all map tasks (ms)=36203
		Total time spent by all reduce tasks (ms)=41274
		Total vcore-milliseconds taken by all map tasks=36203
		Total vcore-milliseconds taken by all reduce tasks=41274
		Total megabyte-milliseconds taken by all map tasks=296574976
		Total megabyte-milliseconds taken by all reduce tasks=338116608
	Map-Reduce Framework
		Map input records=306737
		Map output records=15332281
		Map output bytes=538731478
		Map output materialized bytes=569396052
		Input split bytes=264
		Combine input records=0
		Combine output records=0
		Reduce input groups=30
		Reduce shuffle bytes=569396052
		Reduce input records=15332281
		Reduce output records=2820
		Spilled Records=30664562
		Shuffled Maps =2
		Failed Shuffles=0
		Merged Map outputs=2
		GC time elapsed (ms)=1462
		CPU time spent (ms)=75470
		Physical memory (bytes) snapshot=7219798016
		Virtual memory (bytes) snapshot=26651701248
		Total committed heap usage (bytes)=8231845888
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters
		Bytes Read=386215424
	File Output Format Counters
		Bytes Written=100246
17/07/05 16:16:52 INFO test.TestDFSIOEnh: remote report file adl://dfsiotest.azuredatalakestore.net/dfsio/_merged_reports.txt merged.
17/07/05 16:16:52 INFO test.TestDFSIOEnh: 0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,21,29,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,29,26,25,24,24,24,23,21,21,19,18,17,17,17,17,17,17,17,17,17,17,17,15,13,8,7,5,5,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
17/07/05 16:16:52 INFO test.TestDFSIOEnh: Average of Aggregated Throughput : 1212.0171601073416 mb/sec
17/07/05 16:16:52 INFO test.TestDFSIOEnh:               Standard Deviation : 877.3716200982295 mb/sec
17/07/05 16:16:52 INFO test.TestDFSIOEnh:    Time spots Counted in Average : ..................111111111111111111111111111111111111111111111...............................
