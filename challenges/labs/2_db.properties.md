```
[root@ip-172-31-23-176 java]# head -n 1 /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-06-09 05:17:09,957 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.10.1 (#6 built by jenkins on 20170319-2001 git: f226435f6fa5f545543c00245900ae43bea7a29c)
```

```
[root@ip-172-31-23-176 java]# grep "Started Jetty server" /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-06-09 05:18:32,020 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
```

```
[root@ip-172-31-23-176 java]# cat /etc/cloudera-scm-server/db.properties
# Auto-generated by scm_prepare_database.sh on Fri Jun  9 05:15:17 EDT 2017
#
# For information describing how to configure the Cloudera Manager Server
# to connect to databases, see the "Cloudera Manager Installation Guide."
#
com.cloudera.cmf.db.type=mysql
com.cloudera.cmf.db.host=ip-172-31-23-252
com.cloudera.cmf.db.name=scm
com.cloudera.cmf.db.user=scm
com.cloudera.cmf.db.setupType=EXTERNAL
com.cloudera.cmf.db.password=scm
```