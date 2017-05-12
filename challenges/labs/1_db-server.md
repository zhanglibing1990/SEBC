The hostname of your db server node
  ```
  ip-172-31-23-52  
  ```
    

The command and output for display your database server's version
  ```
 [root@ip-172-31-23-52 home]#  mysql -uroot -p123456 -v
 Warning: Using a password on the command line interface can be insecure.
 Welcome to the MySQL monitor.  Commands end with ; or \g.
 Your MySQL connection id is 4
 Server version: 5.6.36 MySQL Community Server (GPL)
 
 Copyright (c) 2000, 2017, Oracle and/or its affiliates. All rights reserved.
 
 Oracle is a registered trademark of Oracle Corporation and/or its
 affiliates. Other names may be trademarks of their respective
 owners.
 
 Reading history-file /root/.mysql_history
  
  ```

The command and output for listing your created databases
  ```
  mysql> show databases;
  --------------
  show databases
  --------------
  
  +--------------------+
  | Database           |
  +--------------------+
  | information_schema |
  | amon               |
  | hue                |
  | metastore          |
  | mysql              |
  | nav                |
  | navms              |
  | oozie              |
  | performance_schema |
  | rman               |
  | sentry             |
  +--------------------+
  11 rows in set (0.00 sec)
  ```