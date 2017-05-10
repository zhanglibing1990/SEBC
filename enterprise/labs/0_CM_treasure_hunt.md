* What is ubertask optimization?
  ```
  Whether to enable ubertask optimization, which runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings.
  ```
* Where in CM is the Kerberos Security Realm value displayed?
  ```
  Administration -> Settings ->  Category -> Kerberos -> security_realm
  ```
* Which CDH service(s) host a property for enabling Kerberos authentication?
  ```
HDFS	Kerberos, SPNEGO (HttpFS)
MapReduce	Kerberos (also see HDFS)
YARN	Kerberos (also see HDFS)
Accumulo	Kerberos (partial)
Flume	Kerberos (starting CDH 5.4)
HBase	Kerberos (HBase Thrift and REST clients must perform their own user authentication)
HiveServer	None
HiveServer2	Kerberos, LDAP, Custom/pluggable authentication
Hive Metastore	Kerberos
Hue	Kerberos, LDAP, SAML, Custom/pluggable authentication
Impala	Kerberos, LDAP, SPNEGO (Impala Web Console)
Oozie	Kerberos, SPNEGO
Pig	Kerberos
Search	Kerberos, SPNEGO
Sentry	Kerberos
Spark	Kerberos
Sqoop	Kerberos
Sqoop2	Kerberos (starting CDH 5.4)
Zookeeper	Kerberos
  ```
 
* How do you upgrade the CM agents?
  ```
  
  ```
* Give the `tsquery` statement used to chart Hue's CPU utilization?
  ```
  SELECT cpu_percent WHERE roleType=HUE_SERVER
  ```
* Name all the roles that make up the Hive service
  ```
  hiveserver2
  hive metastore
  hive gateway
  ```
* What steps must be completed before integrating Cloudera Manager with Kerberos?
  ```
  Install KDC and kerberos libs
  ```
