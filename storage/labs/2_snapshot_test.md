I uploaded the course-zip using Hue and took tbe snapshot in CM; so no evidence in terms of commands for those parts;

```
[root@ip-172-31-21-158 ec2-user]# sudo -u hdfs hadoop fs -mkdir /precious
[root@ip-172-31-21-158 ec2-user]# sudo -u hdfs hadoop fs -cp /user/admin/precious/* /precious/.
```


```
[root@ip-172-31-21-158 ec2-user]# sudo -u hdfs hadoop fs -rm /precious/*
17/06/06 11:24:17 INFO fs.TrashPolicyDefault: Moved: 'hdfs://ip-172-31-16-139.eu-central-1.compute.internal:8020/precious/SEBC-master.zip' to trash at: hdfs://ip-172-31-16-139.eu-central-1.compute.internal:8020/user/hdfs/.Trash/Current/precious/SEBC-master.zip
[root@ip-172-31-21-158 ec2-user]# sudo -u hdfs hadoop fs -rmdir /precious
rmdir: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```