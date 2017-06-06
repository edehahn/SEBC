```
[edehahn@ip-172-31-24-190 mm]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.block.size=33554432 -D mapred.map.tasks=4 100000000  /user/edehahn/teragen
real    2m31.842s
user    0m6.407s
sys     0m0.347s
```

```
[edehahn@ip-172-31-24-190 mm]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/edehahn/teragen /user/edehahn/terasort
real    5m54.074s
user    0m9.626s
sys     0m0.426s
```