```
{
  "timestamp" : "2017-06-07T13:03:14.357Z",
  "clusters" : [ {
    "name" : "edehahn",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "654311424"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "2363700019"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "397"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-24-190"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0390eb9fb8045b828714d18686f8d649",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4b22fdee-98ac-4951-9102-cabbfb568b47"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6713afb5d787582c49868496433e663a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6d201661aaf2541c91ef85379d02d48a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2fc5ee67-2268-4396-87c0-5420eaaa8b56"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-d93742ab4da24e3102520cc7378c1313",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "431tbjk2hl89ckci8onbgt9tb"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8expgm1m2de10obtbyer2vc3j"
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
            "value" : "654311424"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dzf647x7kmcfvescyvzkl4bsv"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-6713afb5d787582c49868496433e663a",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "530teix5ghy765ldpldg1wymq"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-d93742ab4da24e3102520cc7378c1313",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "abr5tgafq9oqmu2sjvn1t8zz1"
          }, {
            "name" : "serverId",
            "value" : "3"
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
          "value" : "ip-172-31-24-190"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-6d201661aaf2541c91ef85379d02d48a"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1kw62ntucxb6dqluylnddixeu"
          }, {
            "name" : "secret_key",
            "value" : "D6j49AsZVRbaUUfXuyeu7M9hYjO6Qp"
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
            "value" : "ip-172-31-24-190"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "654311424"
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
        "name" : "oozie-OOZIE_SERVER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3ydt221mnty4vjvt8dbezrgel"
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
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
          }, {
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
            "value" : "3"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5192"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "654311424"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5192"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "fLot4ncFMF2kNM8DlmTORl6JPyh9wy"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "eq0f57jo2n7h1f5whh11hxd3e"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0390eb9fb8045b828714d18686f8d649",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "4b22fdee-98ac-4951-9102-cabbfb568b47"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "pzf96766jdwkm3nfgez4gw3v"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6713afb5d787582c49868496433e663a",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ee8jmhdcidxcfotz3b25cyw7k"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6d201661aaf2541c91ef85379d02d48a",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2fc5ee67-2268-4396-87c0-5420eaaa8b56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c612jlxpnz5q364npoxvyil92"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-d93742ab4da24e3102520cc7378c1313",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "an1plpicollji6fpqyzvii4yz"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "ddig6f4an12frduo4gv8djavg"
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
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3157155020"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
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
            "value" : "/opt/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "fs_trash_checkpoint_interval",
            "value" : "10"
          }, {
            "name" : "fs_trash_interval",
            "value" : "10"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "f4AYXgPyBn94weCxQZTkIUIID6vQ0S"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "NkGCRpgLxf873RxLVus4neYMmqFJ95"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "kqndC0bN7rA2EvjWSLFhtZYU2yHN77"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0390eb9fb8045b828714d18686f8d649",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "4b22fdee-98ac-4951-9102-cabbfb568b47"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8evnq1lczf39b112mug5ykoou"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6713afb5d787582c49868496433e663a",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6n4uf2nrgoy8lxdemr8arpnf6"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6d201661aaf2541c91ef85379d02d48a",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2fc5ee67-2268-4396-87c0-5420eaaa8b56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ekrb2g3uxt8itmxqg7e8ihjd6"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-d93742ab4da24e3102520cc7378c1313",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "59gj14l54v9zwkhto6ojcbs6y"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7nnz2zulhhjg9qf4b405ptrt"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-6713afb5d787582c49868496433e663a",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bc4zlq3if415th0y17vvx9yv2"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-6d201661aaf2541c91ef85379d02d48a",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "2fc5ee67-2268-4396-87c0-5420eaaa8b56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "57lavag6krd6bs2lvlghmpy1p"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dha4oseykvwlkvpbg8607usij"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-6713afb5d787582c49868496433e663a",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "99kr13v59lcuupax6qov4fugi"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-d93742ab4da24e3102520cc7378c1313",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4purhx3wqw40j39127osfwvy"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-124665e9c74b9109cd1490f1fbf015c2",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "9odqb70fja6y8kzh3ffbdywqc"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-6713afb5d787582c49868496433e663a",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "62"
          }, {
            "name" : "role_jceks_password",
            "value" : "77sc3la818xsl079rzf59fpxb"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893",
    "ipAddress" : "172.31.16.139",
    "hostname" : "ip-172-31-16-139.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "bb06debf-e8f4-4ef7-b12c-d630a3f46155",
    "ipAddress" : "172.31.21.158",
    "hostname" : "ip-172-31-21-158.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "de0336f5-6200-40a4-a329-9df37be3eb31",
    "ipAddress" : "172.31.22.48",
    "hostname" : "ip-172-31-22-48.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2fc5ee67-2268-4396-87c0-5420eaaa8b56",
    "ipAddress" : "172.31.24.190",
    "hostname" : "ip-172-31-24-190.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "4b22fdee-98ac-4951-9102-cabbfb568b47",
    "ipAddress" : "172.31.30.107",
    "hostname" : "ip-172-31-30-107.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-124665e9c74b9109cd1490f1fbf015c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "2e767ccca0e8a866a3cb16534c4c04dfc87a644b23eafd782eb798da49c72c97",
    "pwSalt" : 8404668125985491369,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-124665e9c74b9109cd1490f1fbf015c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "ecf0f12e0606489031f901fd591bd5b7714122ff08d1a5a181db586290cc1dd9",
    "pwSalt" : 1770792772689730269,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-124665e9c74b9109cd1490f1fbf015c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b0757be25cfb7224a37ecefca994e10b40995b314e2d3f00b787197f9d87a862",
    "pwSalt" : 6863227532958630706,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-124665e9c74b9109cd1490f1fbf015c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "53a972debda2c11e3bf5bfee1edac2925ddd87a004d55f2162ba02b4e60393df",
    "pwSalt" : 3876540829447726753,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "26875b0ac2c74415bc57cdacc3e0e5a6e487c8fb5544d8459bc4816d0a5ea889",
    "pwSalt" : -5006857356008527915,
    "pwLogin" : true
  }, {
    "name" : "edehahn",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "1fbe42350ed367d327e3cec7ab5edc7330f254090917f73f32a80d2409da72b8",
    "pwSalt" : 4053175003458574010,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "9d8d97091d989dc081fd068b8b8070d89657d66f85a6fb76a9549a3a916f6187",
    "pwSalt" : 675913380970600053,
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
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "654311424"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-24-190"
        }, {
          "name" : "headlamp_database_name",
          "value" : "reports"
        }, {
          "name" : "headlamp_database_password",
          "value" : "reports_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "reports"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "654311424"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-124665e9c74b9109cd1490f1fbf015c2",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "bt1x3y31ln6nhxadhoejzncrz"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-124665e9c74b9109cd1490f1fbf015c2",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "4bjbuj1s6mbj1ec2sjtobuusi"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-124665e9c74b9109cd1490f1fbf015c2",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2pylfqplwogx5gqedia6q2mg"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-124665e9c74b9109cd1490f1fbf015c2",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "81gws9two028vwhc7wio7zidq"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-124665e9c74b9109cd1490f1fbf015c2",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "5fd18af5-0255-4e99-9de1-60cc877e4893"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "55juidkxgn8aauirr0vce2hz1"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/23/2012 5:10"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/5.8.3/,https://archive.cloudera.com/cdh5/parcels/5.9/,http://ip-172-31-24-190/cdh5.8.3/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
```