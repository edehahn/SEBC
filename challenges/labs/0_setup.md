AWS
```
[root@ip-172-31-23-252 yum.repos.d]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 6.7 (Santiago)
```
```
[root@ip-172-31-23-252 yum.repos.d]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       40G  2.1G   36G   6% /
tmpfs           7.3G     0  7.3G   0% /dev/shm

[root@ip-172-31-23-176 yum.repos.d]#  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       40G  2.1G   36G   6% /
tmpfs           7.3G     0  7.3G   0% /dev/shm

[root@ip-172-31-27-22 yum.repos.d]#  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       40G  2.1G   36G   6% /
tmpfs           7.3G     0  7.3G   0% /dev/shm

[root@ip-172-31-25-95 yum.repos.d]#  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       40G  2.1G   36G   6% /
tmpfs           7.3G     0  7.3G   0% /dev/shm

[root@ip-172-31-24-201 yum.repos.d]#  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       40G  2.1G   36G   6% /
tmpfs           7.3G     0  7.3G   0% /dev/shm
```

```
[root@ip-172-31-23-252 yum.repos.d]# grep theresa /etc/passwd
theresa:x:2000:501::/home/theresa:/bin/bash
[root@ip-172-31-23-252 yum.repos.d]# grep theresa /etc/passwd
theresa:x:2000:501::/home/theresa:/bin/bash
[root@ip-172-31-23-252 yum.repos.d]# grep conservative /etc/group
conservative:x:501:
[root@ip-172-31-23-252 yum.repos.d]# grep labour /etc/group
labour:x:502:
```