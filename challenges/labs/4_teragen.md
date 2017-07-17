```
time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=33554432 51200000  tgen512m
```
```
real    1m32.856s
user    0m6.402s
sys     0m0.362s
```
<i><strong>The output below should show seven files: one `_SUCCESS` and six mapped output files.</strong></i> 
```
[theresa@ip-172-31-23-252 yum.repos.d]$ hdfs dfs -ls /user/theresa/tgen512m
Found 3 items
-rw-r--r--   3 theresa theresa          0 2017-06-09 06:01 /user/theresa/tgen512m/_SUCCESS
-rw-r--r--   3 theresa theresa 2560000000 2017-06-09 06:01 /user/theresa/tgen512m/part-m-00000
-rw-r--r--   3 theresa theresa 2560000000 2017-06-09 06:01 /user/theresa/tgen512m/part-m-00001
```

```
[theresa@ip-172-31-23-252 yum.repos.d]$ hdfs fsck -blocks /user/theresa/tgen512m
Connecting to namenode via http://ip-172-31-23-176.eu-central-1.compute.internal:50070
FSCK started by theresa (auth:SIMPLE) from /172.31.23.252 for path /user/theresa/tgen512m at Fri Jun 09 06:03:47 EDT 2017
...Status: HEALTHY
 Total size:    5120000000 B
 Total dirs:    1
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      154 (avg. block size 33246753 B)
 Minimally replicated blocks:   154 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Fri Jun 09 06:03:47 EDT 2017 in 7 milliseconds


The filesystem under path '/user/theresa/tgen512m' is HEALTHY
```
