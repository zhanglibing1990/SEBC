#Test HDFS Snapshots

Create a precious directory in HDFS; copy the ZIP course file into it.
```sh
sudo -u hdfs hdfs dfs -mkdir precious
```

Enable snapshots for precious

```sh
[hdfs@ip-172-31-27-157 home]$ hdfs dfsadmin -allowSnapshot /precious
Allowing snaphot on /precious succeeded
```

Create a snapshot called sebc-hdfs-test

```sh
[hdfs@ip-172-31-27-157 home]$ hadoop fs -createSnapshot /precious sebc-hdfs-test
Created snapshot /precious/.snapshot/sebc-hdfs-test
```

Delete the directory
```sh
hdfs dfs -rm -r /precious
rm: Failed to move to trash: hdfs://ip-172-31-20-132:8020/precious: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```
Delete the ZIP file

Restore the deleted file
