# TeraGen

hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D mapreduce.job.maps=4 -D dfs.blocksize=32M  104857600 /user/zlb/terasort-input

Output:

```sh
	File System Counters
		FILE: Number of bytes read=276514
		FILE: Number of bytes written=575070
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=0
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=4
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Input split bytes=83
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=2620
		Total committed heap usage (bytes)=123207680
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=225186913807133164
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10485760000

real	4m20.384s
user	2m11.756s
sys	0m16.600s

```

# Terasort

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort \
/user/zlb/terasort-input /user/zlb/terasort-output

output:

```
	File System Counters
		FILE: Number of bytes read=4714474004
		FILE: Number of bytes written=9342353680
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10485800690
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=948
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=6
	Job Counters 
		Launched map tasks=313
		Launched reduce tasks=3
		Data-local map tasks=290
		Rack-local map tasks=23
		Total time spent by all maps in occupied slots (ms)=2485242
		Total time spent by all reduces in occupied slots (ms)=802663
		Total time spent by all map tasks (ms)=2485242
		Total time spent by all reduce tasks (ms)=802663
		Total vcore-milliseconds taken by all map tasks=2485242
		Total vcore-milliseconds taken by all reduce tasks=802663
		Total megabyte-milliseconds taken by all map tasks=2544887808
		Total megabyte-milliseconds taken by all reduce tasks=821926912
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Map output bytes=10695475200
		Map output materialized bytes=4587244331
		Input split bytes=40690
		Combine input records=0
		Combine output records=0
		Reduce input groups=104857600
		Reduce shuffle bytes=4587244331
		Reduce input records=104857600
		Reduce output records=104857600
		Spilled Records=209715200
		Shuffled Maps =939
		Failed Shuffles=0
		Merged Map outputs=939
		GC time elapsed (ms)=41398
		CPU time spent (ms)=1479530
		Physical memory (bytes) snapshot=161915736064
		Virtual memory (bytes) snapshot=493245456384
		Total committed heap usage (bytes)=152796921856
		Peak Map Physical memory (bytes)=523591680
		Peak Map Virtual memory (bytes)=1575759872
		Peak Reduce Physical memory (bytes)=1001086976
		Peak Reduce Virtual memory (bytes)=1583112192
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10485760000
	File Output Format Counters 
		Bytes Written=10485760000
17/05/10 05:13:25 INFO terasort.TeraSort: done

real	31m26.922s
user	0m15.658s
sys	0m2.394s
```

