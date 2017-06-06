```
[ec2-user@ip-172-31-24-190 mm]$ sudo -u hdfs hdfs fsck /edehahn/ -files -blocks
Connecting to namenode via http://ip-172-31-16-139.eu-central-1.compute.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.24.190 for path /edehahn/ at Tue Jun 06 10:37:07 EDT 2017
/edehahn/ <dir>
/edehahn/_SUCCESS 0 bytes, 0 block(s):  OK

/edehahn/part-m-00000 256000000 bytes, 2 block(s):  OK
0. BP-668188234-172.31.16.139-1496753320751:blk_1073742828_2004 len=134217728 Live_repl=3
1. BP-668188234-172.31.16.139-1496753320751:blk_1073742830_2006 len=121782272 Live_repl=3

/edehahn/part-m-00001 256000000 bytes, 2 block(s):  OK
0. BP-668188234-172.31.16.139-1496753320751:blk_1073742827_2003 len=134217728 Live_repl=3
1. BP-668188234-172.31.16.139-1496753320751:blk_1073742829_2005 len=121782272 Live_repl=3

Status: HEALTHY
 Total size:    512000000 B
 Total dirs:    1
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      4 (avg. block size 128000000 B)
 Minimally replicated blocks:   4 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Tue Jun 06 10:37:07 EDT 2017 in 3 milliseconds


The filesystem under path '/edehahn/' is HEALTHY
```

```
[ec2-user@ip-172-31-24-190 mm]$ sudo -u hdfs hdfs fsck /egruppioni/ -files -blocks
Connecting to namenode via http://ip-172-31-16-139.eu-central-1.compute.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.24.190 for path /egruppioni/ at Tue Jun 06 10:37:18 EDT 2017
/egruppioni/ <dir>
/egruppioni/_SUCCESS 0 bytes, 0 block(s):  OK

/egruppioni/part-m-00000 256000000 bytes, 2 block(s):  OK
0. BP-668188234-172.31.16.139-1496753320751:blk_1073742867_2043 len=134217728 Live_repl=3
1. BP-668188234-172.31.16.139-1496753320751:blk_1073742868_2044 len=121782272 Live_repl=3

/egruppioni/part-m-00001 256000000 bytes, 2 block(s):  OK
0. BP-668188234-172.31.16.139-1496753320751:blk_1073742862_2038 len=134217728 Live_repl=3
1. BP-668188234-172.31.16.139-1496753320751:blk_1073742863_2039 len=121782272 Live_repl=3

Status: HEALTHY
 Total size:    512000000 B
 Total dirs:    1
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      4 (avg. block size 128000000 B)
 Minimally replicated blocks:   4 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Tue Jun 06 10:37:18 EDT 2017 in 1 milliseconds


The filesystem under path '/egruppioni/' is HEALTHY
```