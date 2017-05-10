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

```

