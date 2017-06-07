What is ubertask optimization?
Whether to enable ubertask optimization, which runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings.

Where in CM is the Kerberos Security Realm value displayed?
Administration -> Settings -> Kerberos -> default_realm

Which CDH service(s) host a property for enabling Kerberos authentication?
every service

How do you upgrade the CM agents?
in CM: upgrade the server and follow the wizard to update agents
or in shell, using the OS package manager commands

Give the tsquery statement used to chart Hue's CPU utilization?
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=$SERVICENAME

Name all the roles that make up the Hive service
HiveServer2, Hive Metastore Server, Gateway

What steps must be completed before integrating Cloudera Manager with Kerberos?
1) have a KDC or AD
2) secured communication between the Cloudera Manager Server and Agents 
3) installed the Kerberos client packages on all cluster hosts and hosts that will be used to access the cluster
4) If You are Using AES-256 Encryption, Install the JCE Policy File
5) Get or Create a Kerberos Principal for the Cloudera Manager Server