````
[root@ip-172-31-23-52 krb5kdc]# time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 100 100000000
Number of Maps  = 100
Samples per Map = 100000000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Wrote input for Map #16
Wrote input for Map #17
Wrote input for Map #18
Wrote input for Map #19
Wrote input for Map #20
Wrote input for Map #21
Wrote input for Map #22
Wrote input for Map #23
Wrote input for Map #24
Wrote input for Map #25
Wrote input for Map #26
Wrote input for Map #27
Wrote input for Map #28
Wrote input for Map #29
Wrote input for Map #30
Wrote input for Map #31
Wrote input for Map #32
Wrote input for Map #33
Wrote input for Map #34
Wrote input for Map #35
Wrote input for Map #36
Wrote input for Map #37
Wrote input for Map #38
Wrote input for Map #39
Wrote input for Map #40
Wrote input for Map #41
Wrote input for Map #42
Wrote input for Map #43
Wrote input for Map #44
Wrote input for Map #45
Wrote input for Map #46
Wrote input for Map #47
Wrote input for Map #48
Wrote input for Map #49
Wrote input for Map #50
Wrote input for Map #51
Wrote input for Map #52
Wrote input for Map #53
Wrote input for Map #54
Wrote input for Map #55
Wrote input for Map #56
Wrote input for Map #57
Wrote input for Map #58
Wrote input for Map #59
Wrote input for Map #60
Wrote input for Map #61
Wrote input for Map #62
Wrote input for Map #63
Wrote input for Map #64
Wrote input for Map #65
Wrote input for Map #66
Wrote input for Map #67
Wrote input for Map #68
Wrote input for Map #69
Wrote input for Map #70
Wrote input for Map #71
Wrote input for Map #72
Wrote input for Map #73
Wrote input for Map #74
Wrote input for Map #75
Wrote input for Map #76
Wrote input for Map #77
Wrote input for Map #78
Wrote input for Map #79
Wrote input for Map #80
Wrote input for Map #81
Wrote input for Map #82
Wrote input for Map #83
Wrote input for Map #84
Wrote input for Map #85
Wrote input for Map #86
Wrote input for Map #87
Wrote input for Map #88
Wrote input for Map #89
Wrote input for Map #90
Wrote input for Map #91
Wrote input for Map #92
Wrote input for Map #93
Wrote input for Map #94
Wrote input for Map #95
Wrote input for Map #96
Wrote input for Map #97
Wrote input for Map #98
Wrote input for Map #99
Starting Job
17/05/12 04:02:26 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-145/172.31.17.145:8032
17/05/12 04:02:26 INFO hdfs.DFSClient: Created token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561746900, maxDate=1495166546900, sequenceNumber=5, masterKeyId=2 on 172.31.17.145:8020
17/05/12 04:02:26 INFO security.TokenCache: Got dt for hdfs://ip-172-31-17-145:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.145:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561746900, maxDate=1495166546900, sequenceNumber=5, masterKeyId=2)
17/05/12 04:02:27 INFO input.FileInputFormat: Total input paths to process : 100
17/05/12 04:02:27 INFO mapreduce.JobSubmitter: number of splits:100
17/05/12 04:02:27 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494560708137_0002
17/05/12 04:02:27 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.145:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@ZHANGLIBING1990.CN, renewer=yarn, realUser=, issueDate=1494561746900, maxDate=1495166546900, sequenceNumber=5, masterKeyId=2)
17/05/12 04:02:27 INFO impl.YarnClientImpl: Submitted application application_1494560708137_0002
17/05/12 04:02:27 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-145:8088/proxy/application_1494560708137_0002/
17/05/12 04:02:27 INFO mapreduce.Job: Running job: job_1494560708137_0002
17/05/12 04:02:37 INFO mapreduce.Job: Job job_1494560708137_0002 running in uber mode : false
17/05/12 04:02:37 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 04:02:45 INFO mapreduce.Job:  map 1% reduce 0%
17/05/12 04:02:51 INFO mapreduce.Job:  map 4% reduce 0%
17/05/12 04:02:52 INFO mapreduce.Job:  map 6% reduce 0%
17/05/12 04:02:59 INFO mapreduce.Job:  map 9% reduce 0%
17/05/12 04:03:00 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 04:03:06 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 04:03:07 INFO mapreduce.Job:  map 13% reduce 0%
17/05/12 04:03:08 INFO mapreduce.Job:  map 14% reduce 0%
17/05/12 04:03:09 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 04:03:13 INFO mapreduce.Job:  map 17% reduce 0%
17/05/12 04:03:15 INFO mapreduce.Job:  map 18% reduce 0%
17/05/12 04:03:16 INFO mapreduce.Job:  map 19% reduce 0%
17/05/12 04:03:18 INFO mapreduce.Job:  map 21% reduce 0%
17/05/12 04:03:20 INFO mapreduce.Job:  map 22% reduce 0%
17/05/12 04:03:23 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 04:03:24 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 04:03:27 INFO mapreduce.Job:  map 27% reduce 0%
17/05/12 04:03:32 INFO mapreduce.Job:  map 29% reduce 0%
17/05/12 04:03:34 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 04:03:36 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 04:03:40 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 04:03:41 INFO mapreduce.Job:  map 35% reduce 0%
17/05/12 04:03:44 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 04:03:45 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 04:03:48 INFO mapreduce.Job:  map 39% reduce 0%
17/05/12 04:03:49 INFO mapreduce.Job:  map 40% reduce 0%
17/05/12 04:03:52 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 04:03:53 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 04:03:55 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 04:03:56 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 04:03:57 INFO mapreduce.Job:  map 45% reduce 0%
17/05/12 04:04:00 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 04:04:01 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 04:04:02 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 04:04:05 INFO mapreduce.Job:  map 49% reduce 0%
17/05/12 04:04:06 INFO mapreduce.Job:  map 50% reduce 0%
17/05/12 04:04:08 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 04:04:09 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 04:04:14 INFO mapreduce.Job:  map 54% reduce 0%
17/05/12 04:04:15 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 04:04:16 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 04:04:17 INFO mapreduce.Job:  map 57% reduce 0%
17/05/12 04:04:18 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 04:04:23 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 04:04:24 INFO mapreduce.Job:  map 61% reduce 0%
17/05/12 04:04:25 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 04:04:27 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 04:04:30 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 04:04:32 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 04:04:33 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 04:04:34 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 04:04:35 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 04:04:37 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 04:04:40 INFO mapreduce.Job:  map 70% reduce 0%
17/05/12 04:04:42 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 04:04:43 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 04:04:44 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 04:04:49 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 04:04:50 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 04:04:51 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 04:04:52 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 04:04:58 INFO mapreduce.Job:  map 81% reduce 0%
17/05/12 04:04:59 INFO mapreduce.Job:  map 82% reduce 0%
17/05/12 04:05:00 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 04:05:05 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 04:05:06 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 04:05:09 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 04:05:11 INFO mapreduce.Job:  map 88% reduce 29%
17/05/12 04:05:12 INFO mapreduce.Job:  map 89% reduce 29%
17/05/12 04:05:13 INFO mapreduce.Job:  map 90% reduce 29%
17/05/12 04:05:14 INFO mapreduce.Job:  map 90% reduce 30%
17/05/12 04:05:18 INFO mapreduce.Job:  map 92% reduce 30%
17/05/12 04:05:19 INFO mapreduce.Job:  map 93% reduce 30%
17/05/12 04:05:20 INFO mapreduce.Job:  map 94% reduce 31%
17/05/12 04:05:26 INFO mapreduce.Job:  map 97% reduce 31%
17/05/12 04:05:27 INFO mapreduce.Job:  map 98% reduce 31%
17/05/12 04:05:29 INFO mapreduce.Job:  map 98% reduce 33%
17/05/12 04:05:35 INFO mapreduce.Job:  map 100% reduce 33%
17/05/12 04:05:36 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 04:05:36 INFO mapreduce.Job: Job job_1494560708137_0002 completed successfully
17/05/12 04:05:37 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=864
		FILE: Number of bytes written=12519000
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=27090
		HDFS: Number of bytes written=215
		HDFS: Number of read operations=403
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Job Counters 
		Launched map tasks=100
		Launched reduce tasks=1
		Data-local map tasks=100
		Total time spent by all maps in occupied slots (ms)=729101
		Total time spent by all reduces in occupied slots (ms)=36015
		Total time spent by all map tasks (ms)=729101
		Total time spent by all reduce tasks (ms)=36015
		Total vcore-seconds taken by all map tasks=729101
		Total vcore-seconds taken by all reduce tasks=36015
		Total megabyte-seconds taken by all map tasks=746599424
		Total megabyte-seconds taken by all reduce tasks=36879360
	Map-Reduce Framework
		Map input records=100
		Map output records=200
		Map output bytes=1800
		Map output materialized bytes=3700
		Input split bytes=15290
		Combine input records=0
		Combine output records=0
		Reduce input groups=2
		Reduce shuffle bytes=3700
		Reduce input records=200
		Reduce output records=0
		Spilled Records=400
		Shuffled Maps =100
		Failed Shuffles=0
		Merged Map outputs=100
		GC time elapsed (ms)=4871
		CPU time spent (ms)=339910
		Physical memory (bytes) snapshot=47207591936
		Virtual memory (bytes) snapshot=158057132032
		Total committed heap usage (bytes)=57026281472
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=11800
	File Output Format Counters 
		Bytes Written=97
Job Finished in 190.418 seconds
Estimated value of Pi is 3.14159264920000000000

real	3m15.635s
user	0m6.869s
sys	0m0.883s

````