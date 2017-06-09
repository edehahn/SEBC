```
[root@ip-172-31-23-252 yum.repos.d]# kinit theresa
Password for theresa@EDEHAHN.CO.UK:
[root@ip-172-31-23-252 yum.repos.d]# time hadoop jar /opt/cloudera/parcels/CDH/l                                                                                             ib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort tgen512m tsrt512m
17/06/09 06:30:32 INFO terasort.TeraSort: starting
17/06/09 06:30:34 INFO hdfs.DFSClient: Created token for theresa: HDFS_DELEGATION_TOKEN owner=theresa@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004234058, maxDate=1497609034058, sequenceNumber=1, masterKeyId=2 on 172.31.23.176:8020
17/06/09 06:30:34 INFO security.TokenCache: Got dt for hdfs://ip-172-31-23-176.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.23.176:8020, Ident: (token for theresa: HDFS_DELEGATION_TOKEN owner=theresa@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004234058, maxDate=1497609034058, sequenceNumber=1, masterKeyId=2)
17/06/09 06:30:34 INFO input.FileInputFormat: Total input paths to process : 2
Spent 449ms computing base-splits.
Spent 4ms computing TeraScheduler splits.
Computing input splits took 454ms
Sampling 10 splits of 154
Making 8 from 100000 sampled records
Computing parititions took 1144ms
Spent 1600ms computing partitions.
17/06/09 06:30:35 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-23-176.eu-central-1.compute.internal/172.31.23.176:8032
17/06/09 06:30:36 INFO mapreduce.JobSubmitter: number of splits:154
17/06/09 06:30:36 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1497003883313_0001
17/06/09 06:30:36 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.23.176:8020, Ident: (token for theresa: HDFS_DELEGATION_TOKEN owner=theresa@EDEHAHN.CO.UK, renewer=yarn, realUser=, issueDate=1497004234058, maxDate=1497609034058, sequenceNumber=1, masterKeyId=2)
17/06/09 06:30:38 INFO impl.YarnClientImpl: Submitted application application_1497003883313_0001
17/06/09 06:30:38 INFO mapreduce.Job: The url to track the job: http://ip-172-31-23-176.eu-central-1.compute.internal:8088/proxy/application_1497003883313_0001/
17/06/09 06:30:38 INFO mapreduce.Job: Running job: job_1497003883313_0001
17/06/09 06:30:49 INFO mapreduce.Job: Job job_1497003883313_0001 running in uber mode : false
17/06/09 06:30:49 INFO mapreduce.Job:  map 0% reduce 0%
17/06/09 06:30:59 INFO mapreduce.Job:  map 1% reduce 0%
17/06/09 06:31:01 INFO mapreduce.Job:  map 2% reduce 0%
17/06/09 06:31:06 INFO mapreduce.Job:  map 6% reduce 0%
17/06/09 06:31:09 INFO mapreduce.Job:  map 7% reduce 0%
17/06/09 06:31:10 INFO mapreduce.Job:  map 8% reduce 0%
17/06/09 06:31:11 INFO mapreduce.Job:  map 10% reduce 0%
17/06/09 06:31:15 INFO mapreduce.Job:  map 11% reduce 0%
17/06/09 06:31:16 INFO mapreduce.Job:  map 12% reduce 0%
17/06/09 06:31:17 INFO mapreduce.Job:  map 14% reduce 0%
17/06/09 06:31:20 INFO mapreduce.Job:  map 15% reduce 0%
17/06/09 06:31:21 INFO mapreduce.Job:  map 17% reduce 0%
17/06/09 06:31:22 INFO mapreduce.Job:  map 18% reduce 0%
17/06/09 06:31:23 INFO mapreduce.Job:  map 19% reduce 0%
17/06/09 06:31:26 INFO mapreduce.Job:  map 21% reduce 0%
17/06/09 06:31:27 INFO mapreduce.Job:  map 22% reduce 0%
17/06/09 06:31:28 INFO mapreduce.Job:  map 23% reduce 0%
17/06/09 06:31:31 INFO mapreduce.Job:  map 24% reduce 0%
17/06/09 06:31:32 INFO mapreduce.Job:  map 25% reduce 0%
17/06/09 06:31:35 INFO mapreduce.Job:  map 27% reduce 0%
17/06/09 06:31:36 INFO mapreduce.Job:  map 29% reduce 0%
17/06/09 06:31:37 INFO mapreduce.Job:  map 31% reduce 0%
17/06/09 06:31:40 INFO mapreduce.Job:  map 32% reduce 0%
17/06/09 06:31:42 INFO mapreduce.Job:  map 33% reduce 0%
17/06/09 06:31:45 INFO mapreduce.Job:  map 34% reduce 0%
17/06/09 06:31:46 INFO mapreduce.Job:  map 36% reduce 0%
17/06/09 06:31:48 INFO mapreduce.Job:  map 39% reduce 0%
17/06/09 06:31:49 INFO mapreduce.Job:  map 40% reduce 0%
17/06/09 06:31:52 INFO mapreduce.Job:  map 42% reduce 0%
17/06/09 06:31:56 INFO mapreduce.Job:  map 43% reduce 0%
17/06/09 06:31:57 INFO mapreduce.Job:  map 45% reduce 0%
17/06/09 06:31:58 INFO mapreduce.Job:  map 46% reduce 0%
17/06/09 06:32:00 INFO mapreduce.Job:  map 47% reduce 0%
17/06/09 06:32:02 INFO mapreduce.Job:  map 50% reduce 0%
17/06/09 06:32:05 INFO mapreduce.Job:  map 51% reduce 0%
17/06/09 06:32:07 INFO mapreduce.Job:  map 54% reduce 0%
17/06/09 06:32:08 INFO mapreduce.Job:  map 55% reduce 0%
17/06/09 06:32:11 INFO mapreduce.Job:  map 56% reduce 0%
17/06/09 06:32:14 INFO mapreduce.Job:  map 57% reduce 0%
17/06/09 06:32:15 INFO mapreduce.Job:  map 59% reduce 0%
17/06/09 06:32:16 INFO mapreduce.Job:  map 60% reduce 0%
17/06/09 06:32:18 INFO mapreduce.Job:  map 62% reduce 0%
17/06/09 06:32:19 INFO mapreduce.Job:  map 63% reduce 0%
17/06/09 06:32:20 INFO mapreduce.Job:  map 64% reduce 0%
17/06/09 06:32:22 INFO mapreduce.Job:  map 65% reduce 0%
17/06/09 06:32:24 INFO mapreduce.Job:  map 66% reduce 0%
17/06/09 06:32:26 INFO mapreduce.Job:  map 67% reduce 0%
17/06/09 06:32:27 INFO mapreduce.Job:  map 68% reduce 0%
17/06/09 06:32:28 INFO mapreduce.Job:  map 71% reduce 0%
17/06/09 06:32:31 INFO mapreduce.Job:  map 72% reduce 0%
17/06/09 06:32:33 INFO mapreduce.Job:  map 73% reduce 0%
17/06/09 06:32:34 INFO mapreduce.Job:  map 74% reduce 0%
17/06/09 06:32:37 INFO mapreduce.Job:  map 75% reduce 0%
17/06/09 06:32:38 INFO mapreduce.Job:  map 76% reduce 0%
17/06/09 06:32:39 INFO mapreduce.Job:  map 77% reduce 0%
17/06/09 06:32:40 INFO mapreduce.Job:  map 78% reduce 0%
17/06/09 06:32:42 INFO mapreduce.Job:  map 80% reduce 0%
17/06/09 06:32:43 INFO mapreduce.Job:  map 81% reduce 0%
17/06/09 06:32:44 INFO mapreduce.Job:  map 82% reduce 0%
17/06/09 06:32:46 INFO mapreduce.Job:  map 83% reduce 0%
17/06/09 06:32:47 INFO mapreduce.Job:  map 84% reduce 0%
17/06/09 06:32:48 INFO mapreduce.Job:  map 85% reduce 0%
17/06/09 06:32:49 INFO mapreduce.Job:  map 86% reduce 0%
17/06/09 06:32:53 INFO mapreduce.Job:  map 88% reduce 0%
17/06/09 06:32:55 INFO mapreduce.Job:  map 90% reduce 0%
17/06/09 06:32:56 INFO mapreduce.Job:  map 91% reduce 0%
17/06/09 06:32:59 INFO mapreduce.Job:  map 92% reduce 0%
17/06/09 06:33:05 INFO mapreduce.Job:  map 92% reduce 8%
17/06/09 06:33:07 INFO mapreduce.Job:  map 93% reduce 12%
17/06/09 06:33:08 INFO mapreduce.Job:  map 95% reduce 15%
17/06/09 06:33:09 INFO mapreduce.Job:  map 95% reduce 19%
17/06/09 06:33:10 INFO mapreduce.Job:  map 96% reduce 19%
17/06/09 06:33:12 INFO mapreduce.Job:  map 96% reduce 28%
17/06/09 06:33:13 INFO mapreduce.Job:  map 97% reduce 28%
17/06/09 06:33:20 INFO mapreduce.Job:  map 98% reduce 28%
17/06/09 06:33:21 INFO mapreduce.Job:  map 99% reduce 28%
17/06/09 06:33:22 INFO mapreduce.Job:  map 100% reduce 28%
17/06/09 06:33:23 INFO mapreduce.Job:  map 100% reduce 30%
17/06/09 06:33:24 INFO mapreduce.Job:  map 100% reduce 36%
17/06/09 06:33:25 INFO mapreduce.Job:  map 100% reduce 40%
17/06/09 06:33:27 INFO mapreduce.Job:  map 100% reduce 49%
17/06/09 06:33:29 INFO mapreduce.Job:  map 100% reduce 61%
17/06/09 06:33:30 INFO mapreduce.Job:  map 100% reduce 70%
17/06/09 06:33:31 INFO mapreduce.Job:  map 100% reduce 72%
17/06/09 06:33:33 INFO mapreduce.Job:  map 100% reduce 75%
17/06/09 06:33:35 INFO mapreduce.Job:  map 100% reduce 82%
17/06/09 06:33:36 INFO mapreduce.Job:  map 100% reduce 88%
17/06/09 06:33:38 INFO mapreduce.Job:  map 100% reduce 90%
17/06/09 06:33:39 INFO mapreduce.Job:  map 100% reduce 94%
17/06/09 06:33:40 INFO mapreduce.Job:  map 100% reduce 95%
17/06/09 06:33:41 INFO mapreduce.Job:  map 100% reduce 100%
17/06/09 06:33:41 INFO mapreduce.Job: Job job_1497003883313_0001 completed successfully
17/06/09 06:33:41 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2285320503
                FILE: Number of bytes written=4545961611
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=5120024332
                HDFS: Number of bytes written=5120000000
                HDFS: Number of read operations=486
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=154
                Launched reduce tasks=8
                Data-local map tasks=153
                Rack-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=1558678
                Total time spent by all reduces in occupied slots (ms)=367885
                Total time spent by all map tasks (ms)=1558678
                Total time spent by all reduce tasks (ms)=367885
                Total vcore-seconds taken by all map tasks=1558678
                Total vcore-seconds taken by all reduce tasks=367885
                Total megabyte-seconds taken by all map tasks=1596086272
                Total megabyte-seconds taken by all reduce tasks=376714240
        Map-Reduce Framework
                Map input records=51200000
                Map output records=51200000
                Map output bytes=5222400000
                Map output materialized bytes=2240024986
                Input split bytes=24332
                Combine input records=0
                Combine output records=0
                Reduce input groups=51200000
                Reduce shuffle bytes=2240024986
                Reduce input records=51200000
                Reduce output records=51200000
                Spilled Records=102400000
                Shuffled Maps =1232
                Failed Shuffles=0
                Merged Map outputs=1232
                GC time elapsed (ms)=21316
                CPU time spent (ms)=786860
                Physical memory (bytes) snapshot=81498849280
                Virtual memory (bytes) snapshot=253592850432
                Total committed heap usage (bytes)=92284125184
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5120000000
        File Output Format Counters
                Bytes Written=5120000000
17/06/09 06:33:41 INFO terasort.TeraSort: done

real    3m10.294s
user    0m9.587s
sys     0m0.405s
```