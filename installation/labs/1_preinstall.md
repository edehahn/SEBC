```
[root@ip-172-31-18-209 ~]# cat /proc/sys/vm/swappiness
1
[root@ip-172-31-18-209 ~]# grep swap /etc/sysctl.conf
vm.swappiness = 1
```

```
[root@ip-172-31-18-209 ~]# cat /etc/fstab

#
# /etc/fstab
# Created by anaconda on Mon Sep 29 22:18:18 2014
#
# Accessible filesystems, by reference, are maintained under '/dev/disk'
# See man pages fstab(5), findfs(8), mount(8) and/or blkid(8) for more info
#
LABEL=_         /                       ext4    defaults        1 1
/dev/xvde2              /data           ext4    defaults        1 1
tmpfs                   /dev/shm                tmpfs   defaults        0 0
devpts                  /dev/pts                devpts  gid=5,mode=620  0 0
sysfs                   /sys                    sysfs   defaults        0 0
proc                    /proc                   proc    defaults        0 0
```

```
[root@ip-172-31-18-209 ~]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde1      7.9G  1.1G  6.4G  15% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvde2       22G  172M   21G   1% /data
```

```
[root@ip-172-31-18-209 ~]# sysctl -a |grep huge
vm.nr_hugepages = 0
vm.nr_hugepages_mempolicy = 0
vm.hugetlb_shm_group = 0
vm.hugepages_treat_as_movable = 0
vm.nr_overcommit_hugepages = 0
```

```
[root@ip-172-31-18-209 ~]# ifconfig -a
eth0      Link encap:Ethernet  HWaddr 06:6D:10:B9:CD:F1
          inet addr:172.31.18.209  Bcast:172.31.31.255  Mask:255.255.240.0
          inet6 addr: fe80::46d:10ff:feb9:cdf1/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:2901 errors:0 dropped:0 overruns:0 frame:0
          TX packets:1300 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000
          RX bytes:1286258 (1.2 MiB)  TX bytes:193939 (189.3 KiB)
          Interrupt:24

lo        Link encap:Local Loopback
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0
          RX bytes:0 (0.0 b)  TX bytes:0 (0.0 b)
```

```
[root@ip-172-31-18-209 ~]# nslookup ip-172-31-18-209
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   ip-172-31-18-209.eu-central-1.compute.internal
Address: 172.31.18.209

[root@ip-172-31-18-209 ~]# nslookup 172.31.18.209
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
209.18.31.172.in-addr.arpa      name = ip-172-31-18-209.eu-central-1.compute.internal.

Authoritative answers can be found from:
```

```
[root@ip-172-31-18-209 ~]# pidof nscd
777
[root@ip-172-31-18-209 ~]# pidof ntpd
807
```

