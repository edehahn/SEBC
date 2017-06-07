```
[root@ip-172-31-24-190 cloudera-scm-server]# curl -u edehahn:cloudera -X POST http://localhost:7180/api/v2/clusters/edehahn/services/hive/commands/stop
{
  "id" : 810,
  "name" : "Stop",
  "startTime" : "2017-06-07T13:12:47.735Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

```
[root@ip-172-31-24-190 cloudera-scm-server]# curl -u edehahn:cloudera -X POST http://localhost:7180/api/v2/clusters/edehahn/services/hive/commands/start
{
  "id" : 813,
  "name" : "Start",
  "startTime" : "2017-06-07T13:13:10.810Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

```
[root@ip-172-31-24-190 cloudera-scm-server]# curl -u edehahn:cloudera -X GET http://localhost:7180/api/v2/clusters/edehahn/services/hive/
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-24-190.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD"
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD"
  } ],
  "configStale" : false,
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive"
}
```