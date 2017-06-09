```
[root@ip-172-31-23-176 ~]# ls -l /etc/yum.repos.d/
total 36
-rw-r--r--. 1 root root  293 Jun  9 04:02 cloudera-manager.repo
-rw-r--r--. 1 root root 1836 Jun  9 04:16 mysql-community.repo
-rw-r--r--. 1 root root 1885 Apr 27 05:04 mysql-community-source.repo
-rw-r--r--. 1 root root  358 Jul 14  2015 redhat.repo
-rw-r--r--  1 root root  606 Jun  9 04:22 redhat-rhui-client-config.repo
-rw-r--r--. 1 root root 6300 Jun  9 04:22 redhat-rhui.repo
-rw-r--r--. 1 root root  529 Jun 12  2015 rhel-source.repo
-rw-r--r--  1 root root   86 Jun  9 04:22 rhui-load-balancers.conf
```

```
[root@ip-172-31-23-176 java]# /usr/share/cmf/schema/scm_prepare_database.sh mysql --force -h ip-172-31-23-252 -uroot -p --scm-host ip-172-31-23-252 scm scm scm
```

