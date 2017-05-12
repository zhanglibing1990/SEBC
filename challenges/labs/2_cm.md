List the command and output for `ls /etc/yum.repos.d` 

  ```
  [root@ip-172-31-17-254 yum.repos.d]#  ls /etc/yum.repos.d
  CentOS-Base.repo  CentOS-Debuginfo.repo  CentOS-Media.repo  CentOS-Vault.repo  cloudera-manager.repo
   ```
   Connect Cloudera Manager Server to its database
   
  ```
   [root@ip-172-31-17-254 java]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-30-30 -utemp -ptemp --scm-host ip-172-31-17-254 scm scm scm
   JAVA_HOME=/usr/java/default
   Verifying that we can write to /etc/cloudera-scm-server
   Creating SCM configuration file in /etc/cloudera-scm-server
   Executing:  /usr/java/default/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
   [                          main] DbCommandExecutor              INFO  Successfully connected to database.
   All done, your SCM database is configured correctly!
   ```

