```sh
curl -u admin:admin 'http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:7180/api/v2/cm/deployment'output
```
output 

```sh
{
  "timestamp" : "2017-05-10T08:56:10.388Z",
  "clusters" : [ {
    "name" : "zhanglibing1990",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "569376768"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "569376768"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1181850009"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "198"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "172.31.29.79"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "321321"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-43d7887adfd629b58e03716e4736a97f",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-61088494e21f9eec59374a7881f72c71",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "bd1bd54e-bbb7-4500-951d-59b821ae41f1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d0f0dbohcx73oscs2uc4rajpv"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ob2fycuk6zkp03fvtqzzyub0"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "WEBHCAT",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_webhcat_secret_key",
            "value" : "tVYF3n5MbnkUICyfqtVGW88JtrfCXw"
          }, {
            "name" : "role_health_suppression_webhcat_heap_dump_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_webhcat_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "6e1xceizqacj29qp8mtss249x"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "569376768"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-43d7887adfd629b58e03716e4736a97f",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dw3swhfm5m5wftd2dmnu8668y"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2sby2mlhvcdfz69niyi4mntjr"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-dab003a31053136c1a33efade2d483bc",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "280c42d7-871e-4288-a321-4e2a36805712"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_zookeeper_server_data_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_zookeeper_server_data_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_zookeeper_server_heap_dump_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_zookeeper_server_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "e3oni8z8aeg46xnrnnca67sk7"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-29-79"
        }, {
          "name" : "database_password",
          "value" : "321321"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-4400e98cf7929bcb34dc99893dbeebd1"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bi9l46vizj31nq42q5f0kk1pb"
          }, {
            "name" : "secret_key",
            "value" : "8oNQTAb4nCsZnZOsgfO23giWEUv2uq"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-29-79"
          }, {
            "name" : "oozie_database_password",
            "value" : "321321"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "569376768"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_oozie_server_shared_lib_version_health",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "8m19w3kt1oxqgwpccqkbewg9x"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "3"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "569376768"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "2"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1655"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "569376768"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "1655"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "2"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "5G3kXKC7HRxrYqhwDPnyL1kwsUQQeP"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1j6f0cagt12opoydx8cyhru8r"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-43d7887adfd629b58e03716e4736a97f",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1f3t9rx4pm2frvw2rimh5croo"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_node_manager_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "7h78ox3uvfh6x8ul2nsy58g59"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-61088494e21f9eec59374a7881f72c71",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "bd1bd54e-bbb7-4500-951d-59b821ae41f1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b3rdbqswuhyy3q5qpntqiw00f"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "49"
          }, {
            "name" : "role_jceks_password",
            "value" : "9tgky4r1pszy9kjjyj0ttwtp0"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "569376768"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "4227576627"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1735393280"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/home/Hadoop/journaldata/"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "569376768"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "QQOJOC31LzwdJILQb8DSfyUEXUx1F7"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "ZWsIgCGU4MuX8vFKWO15ytYZ3ddOaB"
        }, {
          "name" : "hdfs_under_replicated_blocks_thresholds",
          "value" : "{\"warning\":10,\"critical\":30}"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "ZonEBiUgG7dZivCSUGyX7xH8QhR1YL"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "service_config_suppression_nameservice_namenodes_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-43d7887adfd629b58e03716e4736a97f",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3s2hrp0bu59pgu2b5fstmmq4k"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_data_node_heap_dump_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_data_node_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_datanode_data_directories_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "1xa3cwjmy6l95v4layiu7bvo8"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-61088494e21f9eec59374a7881f72c71",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "bd1bd54e-bbb7-4500-951d-59b821ae41f1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7npqm5quwepdm67ifctodmypn"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-dab003a31053136c1a33efade2d483bc",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "280c42d7-871e-4288-a321-4e2a36805712"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_data_node_free_space_remaining",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_data_node_heap_dump_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_data_node_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_datanode_data_directories_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "7ihaaefq9xdrqjm7ulrycp26h"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_health_suppression_httpfs_heap_dump_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_health_suppression_httpfs_log_directory_free_space",
            "value" : "true"
          }, {
            "name" : "role_jceks_password",
            "value" : "5s5och6f8rt9sf3j8o0o0dvvt"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-43d7887adfd629b58e03716e4736a97f",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "95xxkvwogep0sn6bsmck1vfwk"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-4400e98cf7929bcb34dc99893dbeebd1",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bk4ey8wt6xr0nc74q9b8nwecg"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2omtw9fk2o9ierm9kpth0qawj"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "52"
          }, {
            "name" : "role_jceks_password",
            "value" : "c6zgamrmq7wgl5m9g91zv1h98"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-b72964ad5a6e9f0f2bf708b1085e3ca3",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4mbjy2uncrt192sbh8q4gq7lh"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd",
    "ipAddress" : "172.31.20.132",
    "hostname" : "ip-172-31-20-132",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_config_suppression_memory_overcommitted_validator",
        "value" : "true"
      }, {
        "name" : "memory_overcommit_threshold",
        "value" : "0.5"
      } ]
    }
  }, {
    "hostId" : "acc501df-48fe-4a94-b2e6-15b0b8211d0d",
    "ipAddress" : "172.31.22.117",
    "hostname" : "ip-172-31-22-117",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_health_suppression_host_agent_parcel_directory_free_space",
        "value" : "true"
      } ]
    }
  }, {
    "hostId" : "2ca8fa2b-5fe2-4a00-bfef-909d71a42ed2",
    "ipAddress" : "172.31.27.157",
    "hostname" : "ip-172-31-27-157",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_config_suppression_memory_overcommitted_validator",
        "value" : "true"
      } ]
    }
  }, {
    "hostId" : "280c42d7-871e-4288-a321-4e2a36805712",
    "ipAddress" : "172.31.29.79",
    "hostname" : "ip-172-31-29-79",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_health_suppression_host_agent_parcel_directory_free_space",
        "value" : "true"
      } ]
    }
  }, {
    "hostId" : "bd1bd54e-bbb7-4500-951d-59b821ae41f1",
    "ipAddress" : "172.31.30.89",
    "hostname" : "ip-172-31-30-89",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0a166ab285a6fe949902c5290121a08c3c8180598959143e53eb50ac6777785a",
    "pwSalt" : 4275765790038672206,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-b72964ad5a6e9f0f2bf708b1085e3ca3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a0d24dd4fc2ce0f137548e8d4e6357676bdd45cb834e7acfdaeff339e57a435f",
    "pwSalt" : 5770569793160314490,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c98630b339d42cb62decc6b2070fd2e59d317444257a0693a987c5d91306dfb9",
    "pwSalt" : -962332722182698373,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-b72964ad5a6e9f0f2bf708b1085e3ca3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "cf0da4200f7abc17065b6ed5d3b5c8c55268cdfc696cd9759af138dcc9ce8bb3",
    "pwSalt" : -1430614618441316609,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "8342105e2f619fc73dd83e47e5fff09ba5de0b6d62c46a061038cd6b5abca309",
    "pwSalt" : -6275762790365587063,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "0e9dbe8e426522a175e977be6216dcd07bd7a90bae4e59f031e6554ee3efb720",
    "pwSalt" : -802302176750344420,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "7552f21eae9fb66e52cac4b815886248f6775e6230bef974548acd5bc4e5f3ce",
    "pwSalt" : 7272299803245586374,
    "pwLogin" : true
  }, {
    "name" : "zhanglibing1990",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "12ce1978490226cc2c00b2a7ed88f25589e66da243d1451e09536f60bf3dfe31",
    "pwSalt" : -6588400345483994344,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170412-1249",
    "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-29-79"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "321321"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "569376768"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "569376768"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "569376768"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-29-79"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "321321"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "569376768"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "569376768"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "8giwssgbvz6kkskdtgpnq6fdg"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ro325bxs5mawqdbqglme1iu9"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "e0q6zpko9lyhsso4cgzmf2f9w"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ccx95yf93s7r21bjxw51rhojb"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "1hiu5w7y1tti6zev0ce55bzc9"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-b72964ad5a6e9f0f2bf708b1085e3ca3",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "d9744a01-7b8c-4588-befe-3781e3de75cd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "7egeglldgp0wjr120taekd3cl"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/27/2012 17:10"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://ec2-54-178-175-207.ap-northeast-1.compute.amazonaws.com:80/cdh5.9/"
    } ]
  }
}
```