#Test HDFS Snapshots

Create a precious directory in HDFS; copy the ZIP course file into it.
```sh
sudo -u hdfs hdfs dfs -mkdir precious
sudo -u hdfs hdfs dfs -put /tmp/SEBC-Shanghai.zip /precious/
```

Enable snapshots for precious

```sh
[hdfs@ip-172-31-27-157 home]$ hdfs dfsadmin -allowSnapshot /precious
Allowing snaphot on /precious succeeded
```

Create a snapshot called sebc-hdfs-test

```sh
[hdfs@ip-172-31-29-79 root]$ hadoop fs -createSnapshot /precious hdfs-test
Created snapshot /precious/.snapshot/hdfs-test
```

Delete the directory
```sh
hdfs dfs -rm -r /precious
rm: Failed to move to trash: hdfs://ip-172-31-20-132:8020/precious: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```

Delete the ZIP file
```
[hdfs@ip-172-31-29-79 root]$ hdfs dfs -rm -r /precious/*
17/05/10 05:17:37 INFO fs.TrashPolicyDefault: Moved: 'hdfs://ip-172-31-20-132:8020/precious/SEBC-Shanghai.zip' to trash at: hdfs://ip-172-31-20-132:8020/user/hdfs/.Trash/Current/precious/SEBC-Shanghai.zip
```

Restore the deleted file
```
[hdfs@ip-172-31-29-79 root]$ hadoop fs -cp /precious/.snapshot/hdfs-test/SEBC-Shanghai.zip /precious/
```
