When I installed CM at the beginning of the course, I used yum without indicating which version to install. So my CM is 5.11 (and CDH 5.8.3)
I should have edited the repo file and modify the baseurl:
```
[root@ip-172-31-24-190 cloudera]# vi /etc/yum.repos.d/cloudera-manager.repo
[cloudera-manager]
name = Cloudera Manager, Version 5.11.0
baseurl = https://archive.cloudera.com/cm5/redhat/6/x86_64/cm/5.11.0/
gpgkey = https://archive.cloudera.com/redhat/cdh/RPM-GPG-KEY-cloudera
gpgcheck = 1
```

```
[root@ip-172-31-24-190 cloudera]# curl -u edehahn:cloudera -X GET http://localhost:7180/api/version/
v16
```

```
[root@ip-172-31-24-190 cloudera]# curl -u edehahn:cloudera -X GET http://localhost:7180/api/v16/users
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "edehahn",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```

```
[root@ip-172-31-24-190 cloudera]# curl -u edehahn:cloudera -X GET http://localhost:7180/api/v16/cm/scmDbInfo
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```