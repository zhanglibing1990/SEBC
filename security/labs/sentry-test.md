### Verify user privileges
```
[root@ip-172-31-20-132 cloudera-scm-server]# beeline
Beeline version 1.1.0-cdh5.11.0 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
scan complete in 3ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
Connected to: Apache Hive (version 1.1.0-cdh5.11.0)
Driver: Hive JDBC (version 1.1.0-cdh5.11.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170511044848_ec65c242-dce7-4b5c-ae79-2065e19d367a): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170511044848_ec65c242-dce7-4b5c-ae79-2065e19d367a); Time taken: 1.044 seconds
INFO  : Executing command(queryId=hive_20170511044848_ec65c242-dce7-4b5c-ae79-2065e19d367a): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170511044848_ec65c242-dce7-4b5c-ae79-2065e19d367a); Time taken: 0.65 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (3.326 seconds)
```

### kinit as george, login to beeline, and use SHOW TABLES;
```
[root@ip-172-31-20-132 ~]# su george
[george@ip-172-31-20-132 root]$ kinit george
Password for george@ZHANGLIBING.COM: 
[george@ip-172-31-20-132 root]$ beeline
Beeline version 1.1.0-cdh5.11.0 by Apache Hive
beeline> 
beeline> !connect jdbc:hive2://locahost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
scan complete in 3ms
Connecting to jdbc:hive2://locahost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
Could not open connection to the HS2 server. Please check the server URI and if the URI is correct, then ask the administrator to check the server status.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://locahost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM: java.net.UnknownHostException: locahost (state=08S01,code=0)
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
Connected to: Apache Hive (version 1.1.0-cdh5.11.0)
Driver: Hive JDBC (version 1.1.0-cdh5.11.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170511070909_6bfa5efd-7796-4f1f-aec3-2762f85faeb1): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170511070909_6bfa5efd-7796-4f1f-aec3-2762f85faeb1); Time taken: 0.109 seconds
INFO  : Executing command(queryId=hive_20170511070909_6bfa5efd-7796-4f1f-aec3-2762f85faeb1): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170511070909_6bfa5efd-7796-4f1f-aec3-2762f85faeb1); Time taken: 0.347 seconds
INFO  : OK
+-------------+--+
|  tab_name   |
+-------------+--+
| example_01  |
| example_02  |
| example_03  |
| sample07    |
+-------------+--+
4 rows selected (0.608 seconds)
```


### kinit as ferdinand, login to beeline, and use SHOW TABLES
```
[ferdinand@ip-172-31-20-132 root]$ kinit ferdinand
Password for ferdinand@ZHANGLIBING.COM: 
[ferdinand@ip-172-31-20-132 root]$ beeline
Beeline version 1.1.0-cdh5.11.0 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
scan complete in 3ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-20-132@ZHANGLIBING.COM
Connected to: Apache Hive (version 1.1.0-cdh5.11.0)
Driver: Hive JDBC (version 1.1.0-cdh5.11.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170511071717_ea2ac2ab-a017-4005-9890-f31b2971c068): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170511071717_ea2ac2ab-a017-4005-9890-f31b2971c068); Time taken: 0.101 seconds
INFO  : Executing command(queryId=hive_20170511071717_ea2ac2ab-a017-4005-9890-f31b2971c068): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170511071717_ea2ac2ab-a017-4005-9890-f31b2971c068); Time taken: 0.179 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
| sample07  |
+-----------+--+
1 row selected (0.43 seconds)
```









