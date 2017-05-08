
1.Check vm.swappiness on all your nodes

Current VMSwappiness is 60 

```
$ cat /proc/sys/vm/swappiness
60
```
Change VMSwappiness to 1

```
$ sudo sysctl vm.swappiness=1
$ cat /proc/sys/vm/swappiness
>> 1
```

2.Show the mount attributes of your volume(s)
```
df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  656M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
```

3.If you have ext-based volumes, list the reserve space setting
```
cat /proc/mounts | grep ext4
/dev/xvde / ext4 rw,seclabel,relatime,barrier=1,data=ordered 0 0
```

4.Disable transparent hugepage support
```
#  grep -i Hugepages_Total /proc/meminfo

HugePages_Total:       0
```

5.List your network interface configuration
```
 ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 16436 qdisc noqueue state UNKNOWN 
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
    inet6 ::1/128 scope host 
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP qlen 1000
    link/ether 06:a5:06:6e:b7:5b brd ff:ff:ff:ff:ff:ff
    inet 172.31.24.109/20 brd 172.31.31.255 scope global eth0
    inet6 fe80::4a5:6ff:fe6e:b75b/64 scope link 
       valid_lft forever preferred_lft forever
```

6.Show that forward and reverse host lookups are correctly resolved
```
$ getent hosts 
127.0.0.1       localhost.localdomain localhost
127.0.0.1       localhost6.localdomain6 localhost6
172.31.18.221   ip-172.31.18.221 cdh2
172.31.24.109   ip-172.31.24.109 cdh3
172.31.22.93    ip-172.31.22.93 cdh4
172.31.21.24    ip-172.31.21.24 cdh5
172.31.20.132   ip-172-31-20-132 cdh5
```

7.Show the nscd service is running
```
# service nscd status
nscd (pid 4523) is running...
```

8.Show the ntpd service is running
```
service ntpd status
ntpd (pid  4521) is running...
```



