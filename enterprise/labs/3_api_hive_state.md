curl statement that stop Hive service

```
[admin@localhost Desktop]$ curl -u "zhanglibing1990:cloudera" -XPOST 'http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:7180/api/v16/clusters/zhanglibing190/services/hive/commands/stop'
{
  "id" : 424,
  "name" : "Stop",
  "startTime" : "2017-05-10T09:42:36.432Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
```

check the status of the previous stop command
```
[admin@localhost Desktop]$ curl -u "zhanglibing1990:cloudera" 'http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:7180/api/v16/commands/424'{
  "id" : 424,
  "name" : "Stop",
  "startTime" : "2017-05-10T09:47:24.368Z",
  "endTime" : "2017-05-10T09:47:26.505Z",
  "active" : false,
  "success" : true,
  "resultMessage" : "Successfully stopped service.",
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  },
  "children" : {
    "items" : [ {
      "id" : 426,
      "name" : "Stop",
      "startTime" : "2017-05-10T09:47:24.372Z",
      "endTime" : "2017-05-10T09:47:26.505Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVEMETASTORE-b72964ad5a6e9f0f2bf708b1085e3ca3"
      }
    }, {
      "id" : 427,
      "name" : "Stop",
      "startTime" : "2017-05-10T09:47:24.373Z",
      "endTime" : "2017-05-10T09:47:26.484Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVESERVER2-b72964ad5a6e9f0f2bf708b1085e3ca3"
      }
    }, {
      "id" : 425,
      "name" : "Stop",
      "startTime" : "2017-05-10T09:47:24.370Z",
      "endTime" : "2017-05-10T09:47:26.212Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-WEBHCAT-4400e98cf7929bcb34dc99893dbeebd1"
      }
    } ]
  },
  "canRetry" : false
}
```
curl statement that start Hive service
```
[admin@localhost Desktop]$ curl -u "zhanglibing1990:cloudera" -XPOST 'http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:7180/api/v16/clusters/zhanglibing190/services/hive/commands/start'
{
  "id" : 418,
  "name" : "Start",
  "startTime" : "2017-05-10T09:43:58.382Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

curl statement to check the current state of Hive service
```
[admin@localhost Desktop]$ curl -u "zhanglibing1990:cloudera" 'http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:7180/api/v16/clusters/zhanglibing1990/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-29-79:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-29-79:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_WEBHCATS_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "FRESH",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
```