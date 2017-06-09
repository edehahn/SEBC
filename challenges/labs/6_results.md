```
[root@ip-172-31-23-176 java]# kinit theresa
Password for theresa@EDEHAHN.CO.UK:
[root@ip-172-31-23-176 java]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hiv
login as: ec2-user
Authenticating with public key "imported-openssh-key" from agent
Last login: Fri Jun  9 06:59:02 2017 from 135.196.42.4
[ec2-user@ip-172-31-23-176 ~]$ sudo su
[root@ip-172-31-23-176 ec2-user]# kinit theresa
Password for theresa@EDEHAHN.CO.UK:
[root@ip-172-31-23-176 ec2-user]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-23-176.eu-central-1.compute.internal@EDEHAHN.CO.UK
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-23-176.eu-central-1.compute.internal@EDEHAHN.CO.UK
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> Display all 560 possibilities? (y or n)
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170609070000_473b3ec6-9283-45aa-b1d1-c9abb11ac57c): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170609070000_473b3ec6-9283-45aa-b1d1-c9abb11ac57c); Time taken: 0.065 seconds
INFO  : Executing command(queryId=hive_20170609070000_473b3ec6-9283-45aa-b1d1-c9abb11ac57c): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170609070000_473b3ec6-9283-45aa-b1d1-c9abb11ac57c); Time taken: 0.145 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.32 seconds)
```

```
[root@ip-172-31-23-176 ec2-user]# kinit jeremy
Password for jeremy@EDEHAHN.CO.UK:
[root@ip-172-31-23-176 ec2-user]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-23-176.eu-central-1.compute.internal@EDEHAHN.CO.UK
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-23-176.eu-central-1.compute.internal@EDEHAHN.CO.UK
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170609070101_151f6660-b79e-419b-aaf8-664364c6bbcc): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170609070101_151f6660-b79e-419b-aaf8-664364c6bbcc); Time taken: 0.067 seconds
INFO  : Executing command(queryId=hive_20170609070101_151f6660-b79e-419b-aaf8-664364c6bbcc): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170609070101_151f6660-b79e-419b-aaf8-664364c6bbcc); Time taken: 0.155 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.325 seconds)
```