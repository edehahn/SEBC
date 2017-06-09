```
[root@ip-172-31-23-176 java]# kinit jeremy
Password for jeremy@EDEHAHN.CO.UK:
[root@ip-172-31-23-176 java]# hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 10 100
Number of Maps  = 10
Samples per Map = 100
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Starting Job
17/06/09 06:33:46 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-23-176.eu-central-1.compute.internal/172.31.23.176:8032
17/06/09 06:33:46 INFO hdfs.DFSClient: Created token for jeremy: HDFS_DELEGATION_TOKEN owner=jeremy@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004426244, maxDate=1497609226244, sequenceNumber=2, masterKeyId=2 on 172.31.23.176:8020
17/06/09 06:33:46 INFO security.TokenCache: Got dt for hdfs://ip-172-31-23-176.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.23.176:8020, Ident: (token for jeremy: HDFS_DELEGATION_TOKEN owner=jeremy@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004426244, maxDate=1497609226244, sequenceNumber=2, masterKeyId=2)
17/06/09 06:33:46 INFO input.FileInputFormat: Total input paths to process : 10
17/06/09 06:33:46 INFO mapreduce.JobSubmitter: number of splits:10
17/06/09 06:33:46 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1497003883313_0002
17/06/09 06:33:46 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.23.176:8020, Ident: (token for jeremy: HDFS_DELEGATION_TOKEN owner=jeremy@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004426244, maxDate=1497609226244, sequenceNumber=2, masterKeyId=2)
17/06/09 06:33:47 INFO impl.YarnClientImpl: Submitted application application_1497003883313_0002
17/06/09 06:33:47 INFO mapreduce.Job: The url to track the job: http://ip-172-31-23-176.eu-central-1.compute.internal:8088/proxy/application_1497003883313_0002/
17/06/09 06:33:47 INFO mapreduce.Job: Running job: job_1497003883313_0002
17/06/09 06:33:56 INFO mapreduce.Job: Job job_1497003883313_0002 running in uber mode : false
17/06/09 06:33:56 INFO mapreduce.Job:  map 0% reduce 0%
17/06/09 06:34:03 INFO mapreduce.Job:  map 20% reduce 0%
17/06/09 06:34:06 INFO mapreduce.Job:  map 60% reduce 0%
17/06/09 06:34:13 INFO mapreduce.Job:  map 100% reduce 0%
17/06/09 06:34:19 INFO mapreduce.Job:  map 100% reduce 100%
17/06/09 06:34:19 INFO mapreduce.Job: Job job_1497003883313_0002 completed successfully
17/06/09 06:34:19 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=96
                FILE: Number of bytes written=1391342
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=3030
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=43
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=10
                Launched reduce tasks=1
                Data-local map tasks=9
                Rack-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=104914
                Total time spent by all reduces in occupied slots (ms)=3820
                Total time spent by all map tasks (ms)=104914
                Total time spent by all reduce tasks (ms)=3820
                Total vcore-seconds taken by all map tasks=104914
                Total vcore-seconds taken by all reduce tasks=3820
                Total megabyte-seconds taken by all map tasks=107431936
                Total megabyte-seconds taken by all reduce tasks=3911680
        Map-Reduce Framework
                Map input records=10
                Map output records=20
                Map output bytes=180
                Map output materialized bytes=340
                Input split bytes=1850
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=340
                Reduce input records=20
                Reduce output records=0
                Spilled Records=40
                Shuffled Maps =10
                Failed Shuffles=0
                Merged Map outputs=10
                GC time elapsed (ms)=529
                CPU time spent (ms)=8230
                Physical memory (bytes) snapshot=4970151936
                Virtual memory (bytes) snapshot=17280757760
                Total committed heap usage (bytes)=5644484608
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1180
        File Output Format Counters
                Bytes Written=97
Job Finished in 33.629 seconds
Estimated value of Pi is 3.14800000000000000000
```