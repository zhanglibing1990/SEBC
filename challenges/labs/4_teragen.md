### The full teragen command and job output
```
[zhou@ip-172-31-23-52 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar  teragen -Dmapreduce.job.maps=6 -Ddfs.blocksize=64M -D mapreduce.map.memory.mb=1024  65536000 /user/zhou/tgen
17/05/12 03:16:43 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-145/172.31.17.145:8032
17/05/12 03:16:44 INFO terasort.TeraSort: Generating 65536000 using 6
17/05/12 03:16:44 INFO mapreduce.JobSubmitter: number of splits:6
17/05/12 03:16:44 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494555249148_0001
17/05/12 03:16:45 INFO impl.YarnClientImpl: Submitted application application_1494555249148_0001
17/05/12 03:16:45 INFO mapreduce.Job: The url to track the job: http://ip-172-31-3-172:8088/proxy/application_1494555249148_0001/
17/05/12 03:16:45 INFO mapreduce.Job: Running job: job_1494555249148_0001
17/05/12 03:16:51 INFO mapreduce.Job: Job job_1494555249148_0001 running in uber mode : false
17/05/12 03:16:51 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 03:17:03 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 03:17:06 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 03:17:09 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 03:17:12 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 03:17:15 INFO mapreduce.Job:  map 59% reduce 0%
17/05/12 03:17:17 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 03:17:18 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 03:17:25 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 03:17:27 INFO mapreduce.Job:  map 81% reduce 0%
17/05/12 03:17:28 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 03:17:30 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 03:17:31 INFO mapreduce.Job:  map 93% reduce 0%
17/05/12 03:17:32 INFO mapreduce.Job:  map 94% reduce 0%
17/05/12 03:17:33 INFO mapreduce.Job:  map 100% reduce 0%
17/05/12 03:17:35 INFO mapreduce.Job: Job job_1494555249148_0001 completed successfully
17/05/12 03:17:36 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=733560
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=511
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=24
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=12
	Job Counters 
		Launched map tasks=6
		Other local map tasks=6
		Total time spent by all maps in occupied slots (ms)=125846
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=125846
		Total vcore-seconds taken by all map tasks=125846
		Total megabyte-seconds taken by all map tasks=128866304
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=511
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=704
		CPU time spent (ms)=102620
		Physical memory (bytes) snapshot=1807962112
		Virtual memory (bytes) snapshot=9429188608
		Total committed heap usage (bytes)=1872756736
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000

real	0m54.658s
user	0m4.863s
sys	0m0.585s
```
### The result of the time command
```
real	0m54.658s
user	0m4.863s
sys	0m0.585s
```

### he command and output of hdfs dfs -ls /user/zhou/tgen
```
[hdfs@ip-172-31-23-52 yum.repos.d]$ hdfs dfs -ls /user/zhou/tgen
Found 7 items
-rw-r--r--   3 zhou supergroup          0 2017-05-12 03:17 /user/zhou/tgen/_SUCCESS
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 03:17 /user/zhou/tgen/part-m-00000
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 03:17 /user/zhou/tgen/part-m-00001
-rw-r--r--   3 zhou supergroup 1092266600 2017-05-12 03:17 /user/zhou/tgen/part-m-00002
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 03:17 /user/zhou/tgen/part-m-00003
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 03:17 /user/zhou/tgen/part-m-00004
-rw-r--r--   3 zhou supergroup 1092266600 2017-05-12 03:17 /user/zhou/tgen/part-m-00005
```
