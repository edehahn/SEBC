```
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170608081313_be171c80-77c1-405b-b07b-f948decc9e1a): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170608081313_be171c80-77c1-405b-b07b-f948decc9e1a); Time taken: 0.144 seconds
INFO  : Executing command(queryId=hive_20170608081313_be171c80-77c1-405b-b07b-f948decc9e1a): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608081313_be171c80-77c1-405b-b07b-f948decc9e1a); Time taken: 30.277 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (30.441 seconds)
0: jdbc:hive2://localhost:10000/default> CREATE ROLE sentry_admin;
INFO  : Compiling command(queryId=hive_20170608081313_12ad3bda-2f47-4c67-a20e-79c07787b195): CREATE ROLE sentry_admin
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608081313_12ad3bda-2f47-4c67-a20e-79c07787b195); Time taken: 0.095 seconds
INFO  : Executing command(queryId=hive_20170608081313_12ad3bda-2f47-4c67-a20e-79c07787b195): CREATE ROLE sentry_admin
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608081313_12ad3bda-2f47-4c67-a20e-79c07787b195); Time taken: 0.705 seconds
INFO  : OK
No rows affected (0.814 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ALL ON SERVER server1 TO ROLE sentry_admin;
INFO  : Compiling command(queryId=hive_20170608081313_fd410f8b-5107-44a5-80a8-ed61570fa2fc): GRANT ALL ON SERVER server1 TO ROLE sentry_admin
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608081313_fd410f8b-5107-44a5-80a8-ed61570fa2fc); Time taken: 0.081 seconds
INFO  : Executing command(queryId=hive_20170608081313_fd410f8b-5107-44a5-80a8-ed61570fa2fc): GRANT ALL ON SERVER server1 TO ROLE sentry_admin
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608081313_fd410f8b-5107-44a5-80a8-ed61570fa2fc); Time taken: 0.103 seconds
INFO  : OK
No rows affected (0.193 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ROLE sentry_admin TO GROUP edehahn;
INFO  : Compiling command(queryId=hive_20170608081414_e776bf38-7a79-4b83-b4eb-d6d3e5985a77): GRANT ROLE sentry_admin TO GROUP edehahn
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608081414_e776bf38-7a79-4b83-b4eb-d6d3e5985a77); Time taken: 0.064 seconds
INFO  : Executing command(queryId=hive_20170608081414_e776bf38-7a79-4b83-b4eb-d6d3e5985a77): GRANT ROLE sentry_admin TO GROUP edehahn
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608081414_e776bf38-7a79-4b83-b4eb-d6d3e5985a77); Time taken: 0.102 seconds
INFO  : OK
No rows affected (0.177 seconds)
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170608084545_2836a45b-0dbe-4616-88db-7b24316a5145): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084545_2836a45b-0dbe-4616-88db-7b24316a5145); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20170608084545_2836a45b-0dbe-4616-88db-7b24316a5145): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084545_2836a45b-0dbe-4616-88db-7b24316a5145); Time taken: 0.131 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| test       |
| web_logs   |
+------------+--+
5 rows selected (0.316 seconds)
```
```
0: jdbc:hive2://localhost:10000/default> CREATE ROLE reads;
INFO  : Compiling command(queryId=hive_20170608082727_b8b4460b-579f-4da0-9677-d4cf7f42e805): CREATE ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608082727_b8b4460b-579f-4da0-9677-d4cf7f42e805); Time taken: 0.068 seconds
INFO  : Executing command(queryId=hive_20170608082727_b8b4460b-579f-4da0-9677-d4cf7f42e805): CREATE ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608082727_b8b4460b-579f-4da0-9677-d4cf7f42e805); Time taken: 0.045 seconds
INFO  : OK
No rows affected (0.184 seconds)
0: jdbc:hive2://localhost:10000/default> CREATE ROLE writes;
INFO  : Compiling command(queryId=hive_20170608082727_cafeeaba-85f3-46ce-9061-12a5c28397c0): CREATE ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608082727_cafeeaba-85f3-46ce-9061-12a5c28397c0); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20170608082727_cafeeaba-85f3-46ce-9061-12a5c28397c0): CREATE ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608082727_cafeeaba-85f3-46ce-9061-12a5c28397c0); Time taken: 0.027 seconds
INFO  : OK
No rows affected (0.094 seconds)
```
```
0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON DATABASE default TO ROLE reads;
INFO  : Compiling command(queryId=hive_20170608084747_6a46cf68-6a0e-43a8-83c3-c293ef759f5a): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084747_6a46cf68-6a0e-43a8-83c3-c293ef759f5a); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20170608084747_6a46cf68-6a0e-43a8-83c3-c293ef759f5a): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084747_6a46cf68-6a0e-43a8-83c3-c293ef759f5a); Time taken: 0.034 seconds
INFO  : OK
No rows affected (0.099 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ROLE reads TO GROUP selector;
INFO  : Compiling command(queryId=hive_20170608084747_5cd7973f-7abb-458e-81ba-ee8d37d493d7): GRANT ROLE reads TO GROUP selector
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084747_5cd7973f-7abb-458e-81ba-ee8d37d493d7); Time taken: 0.065 seconds
INFO  : Executing command(queryId=hive_20170608084747_5cd7973f-7abb-458e-81ba-ee8d37d493d7): GRANT ROLE reads TO GROUP selector
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084747_5cd7973f-7abb-458e-81ba-ee8d37d493d7); Time taken: 0.023 seconds
INFO  : OK
No rows affected (0.099 seconds)
0: jdbc:hive2://localhost:10000/default> REVOKE ALL ON DATABASE default FROM ROLE writes;
INFO  : Compiling command(queryId=hive_20170608084848_cca24ef1-3b4f-446a-a684-1638b08b9d63): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084848_cca24ef1-3b4f-446a-a684-1638b08b9d63); Time taken: 0.07 seconds
INFO  : Executing command(queryId=hive_20170608084848_cca24ef1-3b4f-446a-a684-1638b08b9d63): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084848_cca24ef1-3b4f-446a-a684-1638b08b9d63); Time taken: 0.045 seconds
INFO  : OK
No rows affected (0.13 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON default.sample_07 TO ROLE writes;
INFO  : Compiling command(queryId=hive_20170608084848_188f47ff-91c4-4938-8891-92bfe87eac6a): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084848_188f47ff-91c4-4938-8891-92bfe87eac6a); Time taken: 0.055 seconds
INFO  : Executing command(queryId=hive_20170608084848_188f47ff-91c4-4938-8891-92bfe87eac6a): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084848_188f47ff-91c4-4938-8891-92bfe87eac6a); Time taken: 0.031 seconds
INFO  : OK
No rows affected (0.095 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ROLE writes TO GROUP inserters;
INFO  : Compiling command(queryId=hive_20170608084848_b1e3e53b-fcce-4758-8cd1-149ef1552d5d): GRANT ROLE writes TO GROUP inserters
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170608084848_b1e3e53b-fcce-4758-8cd1-149ef1552d5d); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20170608084848_b1e3e53b-fcce-4758-8cd1-149ef1552d5d): GRANT ROLE writes TO GROUP inserters
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608084848_b1e3e53b-fcce-4758-8cd1-149ef1552d5d); Time taken: 0.023 seconds
INFO  : OK
No rows affected (0.09 seconds)
```
```
[root@ip-172-31-16-139 pki]# kinit george
Password for george@edehahn:
[root@ip-172-31-16-139 pki]# beeline
Beeline version 1.1.0-cdh5.8.3 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn
scan complete in 4ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn
Enter username for jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn: george
Enter password for jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn: *******
Connected to: Apache Hive (version 1.1.0-cdh5.8.3)
Driver: Hive JDBC (version 1.1.0-cdh5.8.3)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170608091212_bb1fceb1-237e-48e4-8177-727fadad1e1f): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170608091212_bb1fceb1-237e-48e4-8177-727fadad1e1f); Time taken: 0.063 seconds
INFO  : Executing command(queryId=hive_20170608091212_bb1fceb1-237e-48e4-8177-727fadad1e1f): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608091212_bb1fceb1-237e-48e4-8177-727fadad1e1f); Time taken: 0.133 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| test       |
| web_logs   |
+------------+--+
5 rows selected (0.327 seconds)
```
```
[root@ip-172-31-16-139 pki]# kinit ferdinand
Password for ferdinand@edehahn:
[root@ip-172-31-16-139 pki]# beeline
Beeline version 1.1.0-cdh5.8.3 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn
scan complete in 3ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn
Enter username for jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn: ferdinand
Enter password for jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-16-139.eu-central-1.compute.internal@edehahn: *******
Connected to: Apache Hive (version 1.1.0-cdh5.8.3)
Driver: Hive JDBC (version 1.1.0-cdh5.8.3)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170608091212_6d732c00-c839-415a-94a4-6864094b29c3): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170608091212_6d732c00-c839-415a-94a4-6864094b29c3); Time taken: 0.067 seconds
INFO  : Executing command(queryId=hive_20170608091212_6d732c00-c839-415a-94a4-6864094b29c3): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170608091212_6d732c00-c839-415a-94a4-6864094b29c3); Time taken: 0.134 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.324 seconds)
```