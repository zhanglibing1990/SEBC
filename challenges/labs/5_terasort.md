````
[root@ip-172-31-23-52 krb5kdc]# kinit zhou
Password for zhou@ZHANGLIBING1990.CN: 
[root@ip-172-31-23-52 krb5kdc]# time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/zhou/tgen /user/zhou/tsort
17/05/12 03:56:34 INFO terasort.TeraSort: starting
17/05/12 03:56:36 INFO hdfs.DFSClient: Created token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561396338, maxDate=1495166196338, sequenceNumber=4, masterKeyId=2 on 172.31.17.145:8020
17/05/12 03:56:36 INFO security.TokenCache: Got dt for hdfs://ip-172-31-17-145:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.145:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561396338, maxDate=1495166196338, sequenceNumber=4, masterKeyId=2)
17/05/12 03:56:36 INFO input.FileInputFormat: Total input paths to process : 6
Spent 328ms computing base-splits.
Spent 3ms computing TeraScheduler splits.
Computing input splits took 332ms
Sampling 10 splits of 102
Making 6 from 100000 sampled records
Computing parititions took 863ms
Spent 1198ms computing partitions.
17/05/12 03:56:37 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-145/172.31.17.145:8032
17/05/12 03:56:37 INFO mapreduce.JobSubmitter: number of splits:102
17/05/12 03:56:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494560708137_0001
17/05/12 03:56:38 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.145:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561396338, maxDate=1495166196338, sequenceNumber=4, masterKeyId=2)
17/05/12 03:56:39 INFO impl.YarnClientImpl: Submitted application application_1494560708137_0001
17/05/12 03:56:39 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-145:8088/proxy/application_1494560708137_0001/
17/05/12 03:56:39 INFO mapreduce.Job: Running job: job_1494560708137_0001
17/05/12 03:56:49 INFO mapreduce.Job: Job job_1494560708137_0001 running in uber mode : false
17/05/12 03:56:49 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 03:56:58 INFO mapreduce.Job:  map 1% reduce 0%
17/05/12 03:57:05 INFO mapreduce.Job:  map 5% reduce 0%
17/05/12 03:57:06 INFO mapreduce.Job:  map 6% reduce 0%
17/05/12 03:57:14 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 03:57:15 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 03:57:21 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 03:57:24 INFO mapreduce.Job:  map 14% reduce 0%
17/05/12 03:57:25 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 03:57:28 INFO mapreduce.Job:  map 17% reduce 0%
17/05/12 03:57:33 INFO mapreduce.Job:  map 19% reduce 0%
17/05/12 03:57:34 INFO mapreduce.Job:  map 21% reduce 0%
17/05/12 03:57:35 INFO mapreduce.Job:  map 22% reduce 0%
17/05/12 03:57:43 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 03:57:44 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 03:57:45 INFO mapreduce.Job:  map 26% reduce 0%
17/05/12 03:57:49 INFO mapreduce.Job:  map 27% reduce 0%
17/05/12 03:57:52 INFO mapreduce.Job:  map 29% reduce 0%
17/05/12 03:57:53 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 03:57:54 INFO mapreduce.Job:  map 31% reduce 0%
17/05/12 03:57:57 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 03:58:01 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 03:58:02 INFO mapreduce.Job:  map 35% reduce 0%
17/05/12 03:58:03 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 03:58:10 INFO mapreduce.Job:  map 40% reduce 0%
17/05/12 03:58:11 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 03:58:12 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 03:58:17 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 03:58:20 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 03:58:21 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 03:58:24 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 03:58:29 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 03:58:30 INFO mapreduce.Job:  map 52% reduce 0%
17/05/12 03:58:31 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 03:58:38 INFO mapreduce.Job:  map 57% reduce 0%
17/05/12 03:58:39 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 03:58:45 INFO mapreduce.Job:  map 59% reduce 0%
17/05/12 03:58:47 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 03:58:48 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 03:58:52 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 03:58:56 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 03:58:57 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 03:58:59 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 03:59:05 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 03:59:06 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 03:59:13 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 03:59:15 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 03:59:20 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 03:59:23 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 03:59:24 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 03:59:28 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 03:59:32 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 03:59:33 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 03:59:35 INFO mapreduce.Job:  map 86% reduce 4%
17/05/12 03:59:36 INFO mapreduce.Job:  map 87% reduce 4%
17/05/12 03:59:37 INFO mapreduce.Job:  map 87% reduce 8%
17/05/12 03:59:40 INFO mapreduce.Job:  map 87% reduce 9%
17/05/12 03:59:41 INFO mapreduce.Job:  map 88% reduce 9%
17/05/12 03:59:43 INFO mapreduce.Job:  map 89% reduce 10%
17/05/12 03:59:44 INFO mapreduce.Job:  map 89% reduce 14%
17/05/12 03:59:47 INFO mapreduce.Job:  map 89% reduce 15%
17/05/12 03:59:50 INFO mapreduce.Job:  map 91% reduce 15%
17/05/12 03:59:58 INFO mapreduce.Job:  map 93% reduce 15%
17/05/12 04:00:01 INFO mapreduce.Job:  map 93% reduce 16%
17/05/12 04:00:05 INFO mapreduce.Job:  map 95% reduce 16%
17/05/12 04:00:11 INFO mapreduce.Job:  map 96% reduce 16%
17/05/12 04:00:12 INFO mapreduce.Job:  map 97% reduce 16%
17/05/12 04:00:17 INFO mapreduce.Job:  map 98% reduce 16%
17/05/12 04:00:18 INFO mapreduce.Job:  map 99% reduce 16%
17/05/12 04:00:21 INFO mapreduce.Job:  map 99% reduce 17%
17/05/12 04:00:23 INFO mapreduce.Job:  map 100% reduce 17%
17/05/12 04:00:24 INFO mapreduce.Job:  map 100% reduce 22%
17/05/12 04:00:25 INFO mapreduce.Job:  map 100% reduce 28%
17/05/12 04:00:27 INFO mapreduce.Job:  map 100% reduce 35%
17/05/12 04:00:29 INFO mapreduce.Job:  map 100% reduce 40%
17/05/12 04:00:30 INFO mapreduce.Job:  map 100% reduce 41%
17/05/12 04:00:31 INFO mapreduce.Job:  map 100% reduce 42%
17/05/12 04:00:32 INFO mapreduce.Job:  map 100% reduce 43%
17/05/12 04:00:33 INFO mapreduce.Job:  map 100% reduce 45%
17/05/12 04:00:34 INFO mapreduce.Job:  map 100% reduce 46%
17/05/12 04:00:35 INFO mapreduce.Job:  map 100% reduce 55%
17/05/12 04:00:36 INFO mapreduce.Job:  map 100% reduce 57%
17/05/12 04:00:37 INFO mapreduce.Job:  map 100% reduce 59%
17/05/12 04:00:38 INFO mapreduce.Job:  map 100% reduce 60%
17/05/12 04:00:39 INFO mapreduce.Job:  map 100% reduce 62%
17/05/12 04:00:40 INFO mapreduce.Job:  map 100% reduce 64%
17/05/12 04:00:41 INFO mapreduce.Job:  map 100% reduce 66%
17/05/12 04:00:42 INFO mapreduce.Job:  map 100% reduce 68%
17/05/12 04:00:44 INFO mapreduce.Job:  map 100% reduce 76%
17/05/12 04:00:47 INFO mapreduce.Job:  map 100% reduce 79%
17/05/12 04:00:53 INFO mapreduce.Job:  map 100% reduce 80%
17/05/12 04:00:56 INFO mapreduce.Job:  map 100% reduce 84%
17/05/12 04:00:59 INFO mapreduce.Job:  map 100% reduce 87%
17/05/12 04:01:02 INFO mapreduce.Job:  map 100% reduce 89%
17/05/12 04:01:05 INFO mapreduce.Job:  map 100% reduce 95%
17/05/12 04:01:08 INFO mapreduce.Job:  map 100% reduce 96%
17/05/12 04:01:11 INFO mapreduce.Job:  map 100% reduce 97%
17/05/12 04:01:14 INFO mapreduce.Job:  map 100% reduce 99%
17/05/12 04:01:17 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 04:01:17 INFO mapreduce.Job: Job job_1494560708137_0001 completed successfully
17/05/12 04:01:17 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=2934292533
		FILE: Number of bytes written=5820815178
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=6553612342
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=324
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=12
	Job Counters 
		Launched map tasks=102
		Launched reduce tasks=6
		Data-local map tasks=102
		Total time spent by all maps in occupied slots (ms)=785144
		Total time spent by all reduces in occupied slots (ms)=324118
		Total time spent by all map tasks (ms)=785144
		Total time spent by all reduce tasks (ms)=324118
		Total vcore-seconds taken by all map tasks=785144
		Total vcore-seconds taken by all reduce tasks=324118
		Total megabyte-seconds taken by all map tasks=803987456
		Total megabyte-seconds taken by all reduce tasks=331896832
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Map output bytes=6684672000
		Map output materialized bytes=2873057831
		Input split bytes=12342
		Combine input records=0
		Combine output records=0
		Reduce input groups=65536000
		Reduce shuffle bytes=2873057831
		Reduce input records=65536000
		Reduce output records=65536000
		Spilled Records=131072000
		Shuffled Maps =612
		Failed Shuffles=0
		Merged Map outputs=612
		GC time elapsed (ms)=12390
		CPU time spent (ms)=671960
		Physical memory (bytes) snapshot=56906203136
		Virtual memory (bytes) snapshot=169203363840
		Total committed heap usage (bytes)=66351792128
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=6553600000
	File Output Format Counters 
		Bytes Written=6553600000
17/05/12 04:01:17 INFO terasort.TeraSort: done

real	4m43.873s
user	0m8.743s
sys	0m0.847s
```