List the cloud provider you are using (AWS, GCE, Azure, other)
AWS

List the nodes you are using by IP address and name
  ```
52.193.68.171 SEBC-1
13.113.115.206 SEBC-2
52.199.233.190 SEBC-3
52.198.72.162 SEBC-4
13.112.248.26 SEBC-5
  ```
List the Linux release you are using
  ```
CentOS 6-5 -x86_64- - Release Media-6-5 
  ```
Demonstrate the disk capacity available on each node is >= 30 GB
  ```
[root@ip-172-31-23-52 yum.repos.d]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  847M   28G   3% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
  ```
  
List the command and output for yum repolist enabled
  ```
[root@ip-172-31-17-145 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
Loading mirror speeds from cached hostfile
 * base: ftp.iij.ad.jp
 * extras: ftp.iij.ad.jp
 * updates: ftp.iij.ad.jp
repo id                                                   repo name                                                             status
base                                                      CentOS-6 - Base                                                       6,706
extras                                                    CentOS-6 - Extras                                                        64
updates                                                   CentOS-6 - Updates                                                      270
repolist: 7,040
  ```
  
  Add the following Linux accounts to all nodes
  ```
useradd -u 2800 zhou 
useradd -u 2900 chen
groupadd shanghai
groupadd beijing
usermod -G shanghai  chen 
usermod -G beijing zhou  
  ```
  List the /etc/passwd entries for zhou and chen
  ```
[root@ip-172-31-23-52 ~]# cat /etc/passwd |grep zhou
zhou:x:2800:2800::/home/zhou:/bin/bash
  
[root@ip-172-31-23-52 ~]# cat /etc/passwd |grep chen
chen:x:2900:2900::/home/chen:/bin/bash
  
  ```
  List the /etc/group entries for kiwis and aussies
  ```
[root@ip-172-31-23-52 ~]# cat /etc/group |grep shanghai
shanghai:x:2903:chen
  
[root@ip-172-31-23-52 ~]# cat /etc/group |grep beijing
beijing:x:2904:zhou
  ```
