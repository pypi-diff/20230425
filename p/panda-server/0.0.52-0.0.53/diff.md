# Comparing `tmp/panda-server-0.0.52.tar.gz` & `tmp/panda-server-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.52.tar", last modified: Mon Apr 24 06:51:18 2023, max compression
+gzip compressed data, was "panda-server-0.0.53.tar", last modified: Tue Apr 25 06:52:21 2023, max compression
```

## Comparing `panda-server-0.0.52.tar` & `panda-server-0.0.53.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-24 06:51:06.000000 panda-server-0.0.52/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 06:51:06.000000 panda-server-0.0.52/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 06:51:06.000000 panda-server-0.0.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 06:51:18.824622 panda-server-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 06:51:06.000000 panda-server-0.0.52/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 06:51:06.000000 panda-server-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.800620 panda-server-0.0.52/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.800620 panda-server-0.0.52/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.812621 panda-server-0.0.52/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1229216 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 06:51:18.824622 panda-server-0.0.52/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-24 06:51:06.000000 panda-server-0.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/logrotate.d/panda_server.logrotate.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-add_main.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-add_sub.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-backupJobArch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-boostUser.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-callback.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-configurator.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-copyArchive.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-datasetManager.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-esPreemption.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-evpPD2P.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-frontier_retagging.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-network_configurator.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-pilot_streaming.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-priority.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-proxyCache.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-schedconfig_json.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-sw_tags.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-tmpwatch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server.cfg.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/pandasrv.cron.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-25 06:52:10.000000 panda-server-0.0.53/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 06:52:10.000000 panda-server-0.0.53/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 06:52:10.000000 panda-server-0.0.53/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 06:52:21.168215 panda-server-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 06:52:10.000000 panda-server-0.0.53/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 06:52:10.000000 panda-server-0.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:52:20.000000 panda-server-0.0.53/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/master.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.132214 panda-server-0.0.53/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.136214 panda-server-0.0.53/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40218 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.152214 panda-server-0.0.53/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1229216 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.164214 panda-server-0.0.53/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 06:52:21.168215 panda-server-0.0.53/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-25 06:52:10.000000 panda-server-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/logrotate.d/panda_server.logrotate.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-add_main.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-add_sub.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-backupJobArch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-boostUser.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-callback.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-configurator.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-copyArchive.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-datasetManager.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-esPreemption.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-evpPD2P.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-frontier_retagging.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-network_configurator.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-pilot_streaming.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-priority.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-proxyCache.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-schedconfig_json.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-sw_tags.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-tmpwatch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server.cfg.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/pandasrv.cron.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/sysconfig/panda_server.sysconfig.rpmnew.template
```

### Comparing `panda-server-0.0.52/ChangeLog.txt` & `panda-server-0.0.53/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/LICENSE.txt` & `panda-server-0.0.53/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.53/panda_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.53/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/brokerage/broker.py` & `panda-server-0.0.53/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/config/daemon_config.py` & `panda-server-0.0.53/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/config/panda_config.py` & `panda-server-0.0.53/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/configurator/Carbon.py` & `panda-server-0.0.53/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/configurator/Configurator.py` & `panda-server-0.0.53/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/configurator/aux.py` & `panda-server-0.0.53/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/master.py` & `panda-server-0.0.53/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/add_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pandaserver.dataservice.AdderGen import AdderGen
 
 # logger
 _logger = PandaLogger().getLogger('add_main')
 
 
 # main
-def main(argv=tuple(), tbuf=None, **kwargs):
+def main(argv=tuple(), tbuf=None, lock_pool=None, **kwargs):
 
     try:
         long
     except NameError:
         long = int
 
     prelock_pid = GenericThread().get_pid()
@@ -57,19 +57,20 @@
     aSiteMapper = SiteMapper(taskBuffer)
 
 
     # thread for adder
     class AdderThread(GenericThread):
 
         def __init__(self, taskBuffer, aSiteMapper,
-                        job_output_reports):
+                        job_output_reports, lock_pool):
             GenericThread.__init__(self)
             self.taskBuffer = taskBuffer
             self.aSiteMapper = aSiteMapper
             self.job_output_reports = job_output_reports
+            self.lock_pool = lock_pool
 
         # main loop
         def run(self):
             # initialize
             taskBuffer = self.taskBuffer
             aSiteMapper = self.aSiteMapper
             # get file list
@@ -107,15 +108,16 @@
                         # usual add
                         tmpLog.debug("pid={0} : add job={1}.{2} st={3}".format(uniq_pid, panda_id,
                                                                                attempt_nr, job_status))
                         ignoreTmpError = True
                     # get adder
                     adder_gen = AdderGen(taskBuffer, panda_id, job_status, attempt_nr,
                                          ignoreTmpError=ignoreTmpError, siteMapper=aSiteMapper, pid=uniq_pid,
-                                         prelock_pid=uniq_pid, lock_offset=lock_interval-retry_interval)
+                                         prelock_pid=uniq_pid, lock_offset=lock_interval-retry_interval,
+                                         lock_pool=lock_pool)
                     n_processed += 1
                     # execute
                     adder_gen.run()
                     del adder_gen
                 except Exception as e:
                     tmpLog.error("pid={} : failed to run with {} {}".format(uniq_pid, str(e), traceback.format_exc()))
             # stats
@@ -172,17 +174,17 @@
         tbuf_list = []
         tmpLog.debug("got {} job reports".format(len(jor_lists)))
         for i in range(nThr):
             if i < _n_thr_with_tbuf:
                 tbuf = TaskBuffer()
                 tbuf_list.append(tbuf)
                 tbuf.init(panda_config.dbhost, panda_config.dbpasswd, nDBConnection=1, useTimeout=True)
-                thr = AdderThread(tbuf, aSiteMapper, jor_lists)
+                thr = AdderThread(tbuf, aSiteMapper, jor_lists, lock_pool)
             else:
-                thr = AdderThread(taskBufferIF.getInterface(), aSiteMapper, jor_lists)
+                thr = AdderThread(taskBufferIF.getInterface(), aSiteMapper, jor_lists, lock_pool)
             adderThrList.append(thr)
         # start all threads
         for thr in adderThrList:
             # thr.start()
             thr.proc_launch()
             time.sleep(0.25)
```

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.53/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/daemons/utils.py` & `panda-server-0.0.53/pandaserver/daemons/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import traceback
 import signal
 import gc
 
 import psutil
 
 from pandacommon.pandalogger import logger_utils
+from pandacommon.pandautils.thread_utils import LockPool
 from pandaserver.config import panda_config, daemon_config
 
 
 # list of signals accepted to end the main process
 END_SIGNALS = [
         signal.SIGINT,
         signal.SIGHUP,
@@ -59,15 +60,15 @@
             pass
     gone, alive = psutil.wait_procs(children, timeout=timeout,
                                     callback=on_terminate)
     return (gone, alive)
 
 
 # worker process loop of daemon
-def daemon_loop(dem_config, msg_queue, pipe_conn, worker_lifetime, tbuf=None):
+def daemon_loop(dem_config, msg_queue, pipe_conn, worker_lifetime, tbuf=None, lock_pool=None):
     # pid of the worker
     my_pid = os.getpid()
     my_full_pid = '{0}-{1}-{2}'.format(socket.getfqdn().split('.')[0], os.getpgrp(), my_pid)
     # logger to log in file
     base_logger = logger_utils.setup_logger('daemons')
     tmp_log = logger_utils.make_logger(base_logger, 'worker_pid={pid}'.format(pid=my_pid))
     tmp_log.info('daemon worker start')
@@ -198,27 +199,27 @@
                 pipe_conn.send(status_tuple)
                 try:
                     if is_loop:
                         # go looping the script until reaching daemon period
                         tmp_log.info('{dem} start looping'.format(dem=dem_name))
                         start_ts = time.time()
                         while True:
-                            ret_val = the_module.main(argv=mod_argv, tbuf=tbuf)
+                            ret_val = the_module.main(argv=mod_argv, tbuf=tbuf, lock_pool=lock_pool)
                             now_ts = time.time()
                             if not ret_val:
                                 # daemon main function says stop the loop
                                 break
                             if now_ts > start_ts + dem_period:
                                 # longer than the period, stop the loop
                                 break
                         tmp_log.info('{dem} finish looping'.format(dem=dem_name))
                     else:
                         # execute the module script with arguments
                         tmp_log.info('{dem} start'.format(dem=dem_name))
-                        the_module.main(argv=mod_argv, tbuf=tbuf)
+                        the_module.main(argv=mod_argv, tbuf=tbuf, lock_pool=lock_pool)
                         tmp_log.info('{dem} finish'.format(dem=dem_name))
                 except Exception as e:
                     # with error
                     tb = traceback.format_exc()
                     tmp_log.error('failed to run daemon {dem} with {err} ; stop this worker'.format(
                                     dem=dem_name, err='{0}: {1}\n{2}\n'.format(e.__class__.__name__, e, tb)))
                     # daemon has run but failed
@@ -258,35 +259,36 @@
             'dem_ts',
         )
 
     # class lock
     _lock = threading.Lock()
 
     # constructor
-    def __init__(self, dem_config, msg_queue, worker_lifetime, tbuf=None):
+    def __init__(self, dem_config, msg_queue, worker_lifetime, tbuf=None, lock_pool=None):
         # synchronized with lock
         with self._lock:
             self._make_pipe()
             self._make_process( dem_config=dem_config,
                                 msg_queue=msg_queue,
                                 worker_lifetime=worker_lifetime,
-                                tbuf=tbuf)
+                                tbuf=tbuf,
+                                lock_pool=lock_pool)
 
     # make pipe connection pairs for the worker
     def _make_pipe(self):
         self.parent_conn, self.child_conn = multiprocessing.Pipe()
 
     # close pipe connections
     def _close_pipe(self):
         self.parent_conn.close()
         self.child_conn.close()
 
     # make associated process
-    def _make_process(self, dem_config, msg_queue, worker_lifetime, tbuf):
-        args = (dem_config, msg_queue, self.child_conn, worker_lifetime, tbuf)
+    def _make_process(self, dem_config, msg_queue, worker_lifetime, tbuf, lock_pool):
+        args = (dem_config, msg_queue, self.child_conn, worker_lifetime, tbuf, lock_pool)
         self.process = multiprocessing.Process(target=daemon_loop, args=args)
 
     # start worker process
     def start(self):
         self.unset_dem()
         self.process.start()
         self.pid = self.process.pid
@@ -347,14 +349,16 @@
         self._parse_config()
         # map of run status of daemons
         self.dem_run_map = {}
         self._make_dem_run_map()
         # shared taskBufferIF
         self.tbif = None
         self._make_tbif()
+        # shared lock pool
+        self.lock_pool = LockPool()
         # spawn workers
         self._spawn_workers(self.n_workers)
 
     # make common taskBuffer interface for daemon workers
     def _make_tbif(self):
         try:
             # import is always required to have reserveChangedState consistent in *Spec
@@ -382,15 +386,16 @@
                 if self.use_tbif:
                     tbuf = self.tbif.getInterface()
                 else:
                     tbuf = None
                 worker = DaemonWorker(  dem_config=self.dem_config,
                                         msg_queue=self.msg_queue,
                                         worker_lifetime=self.worker_lifetime,
-                                        tbuf=tbuf)
+                                        tbuf=tbuf,
+                                        lock_pool=self.lock_pool)
                 self.worker_pool.add(worker)
                 if auto_start:
                     worker.start()
                     self.logger.debug('launched new worker_pid={worker_pid}'.format(worker_pid=worker.pid))
 
     # remove a worker from pool
     def _remove_worker(self, worker):
```

### Comparing `panda-server-0.0.52/pandaserver/dataservice/Activator.py` & `panda-server-0.0.53/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.53/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.53/pandaserver/dataservice/AdderGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,29 @@
 
 panda_config.setupPlugin()
 
 
 class AdderGen(object):
     # constructor
     def __init__(self, taskBuffer, jobID, jobStatus, attemptNr, ignoreTmpError=True, siteMapper=None,
-                 pid=None, prelock_pid=None, lock_offset=10):
+                 pid=None, prelock_pid=None, lock_offset=10, lock_pool=None):
         self.job = None
         self.jobID = jobID
         self.jobStatus = jobStatus
         self.taskBuffer = taskBuffer
         self.ignoreTmpError = ignoreTmpError
         self.lock_offset = lock_offset
         self.siteMapper = siteMapper
         self.datasetMap = {}
         self.extraInfo = {'surl':{},'nevents':{},'lbnr':{},'endpoint':{}, 'guid':{}}
         self.attemptNr = attemptNr
         self.pid = pid
         self.prelock_pid = prelock_pid
         self.data = None
+        self.lock_pool = lock_pool
         # logger
         self.logger = LogWrapper(_logger,str(self.jobID))
 
 
     # dump file report
     def dumpFileReport(self, fileCatalog, attemptNr):
         self.logger.debug("dump file report")
@@ -300,21 +301,33 @@
                 maxOutputFileBytes = 99999999999
                 if self.job.outputFileBytes > maxOutputFileBytes:
                     self.job.outputFileBytes = maxOutputFileBytes
                 # set cancelled state
                 if self.job.commandToPilot == 'tobekilled' and self.job.jobStatus == 'failed':
                     self.job.jobStatus = 'cancelled'
                 # update job
-                if oldJobStatus in ['cancelled','closed']:
+                if oldJobStatus in ['cancelled', 'closed']:
                     pass
                 else:
+                    db_lock = None
+                    if self.job.jediTaskID not in [0, None, 'NULL'] and self.lock_pool:
+                        db_lock = self.lock_pool.get(self.job.jediTaskID)
+                        if db_lock:
+                            db_lock.acquire()
+                            self.logger.debug("got DB lock for jediTaskID={}".format(self.job.jediTaskID))
+                        else:
+                            self.logger.debug("couldn't get DB lock for jediTaskID={}".format(self.job.jediTaskID))
                     self.logger.debug("updating DB")
                     retU = self.taskBuffer.updateJobs([self.job],False,oldJobStatusList=[oldJobStatus],
                                                       extraInfo=self.extraInfo)
                     self.logger.debug("retU: %s" % retU)
+                    if db_lock:
+                        self.logger.debug("release DB lock for jediTaskID={}".format(self.job.jediTaskID))
+                        db_lock.release()
+                        self.lock_pool.release(self.job.jediTaskID)
                     # failed
                     if not retU[0]:
                         self.logger.error('failed to update DB for pandaid={0}'.format(self.job.PandaID))
                         # unlock job output report
                         self.taskBuffer.unlockJobOutputReport(
                                         panda_id=self.jobID, attempt_nr=self.attemptNr, pid=self.pid,
                                         lock_offset=self.lock_offset)
```

### Comparing `panda-server-0.0.52/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.53/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.53/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/Closer.py` & `panda-server-0.0.53/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.53/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/DDM.py` & `panda-server-0.0.53/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.53/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/DataService.py` & `panda-server-0.0.53/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.53/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.53/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.53/pandaserver/dataservice/EventPicker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.53/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.53/pandaserver/dataservice/Notifier.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.53/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.53/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.53/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.53/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.53/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.53/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.53/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.53/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.53/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.53/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.53/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.53/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.53/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.53/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.53/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/server/panda.py` & `panda-server-0.0.53/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.53/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.53/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.53/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.53/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.53/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.53/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.53/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.53/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.53/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.53/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.53/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.53/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.53/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.53/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.53/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.53/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.53/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.53/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.53/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.53/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.53/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.53/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.53/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.53/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.53/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/banUser.py` & `panda-server-0.0.53/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/boostPrio.py` & `panda-server-0.0.53/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/boostUser.py` & `panda-server-0.0.53/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/callbackDDM.py` & `panda-server-0.0.53/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/finishJob.py` & `panda-server-0.0.53/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.53/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/getJobs.py` & `panda-server-0.0.53/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killJob.py` & `panda-server-0.0.53/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.53/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.53/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killProdJobs.py` & `panda-server-0.0.53/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killTask.py` & `panda-server-0.0.53/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/killUser.py` & `panda-server-0.0.53/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/reassignSite.py` & `panda-server-0.0.53/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/reassignTask.py` & `panda-server-0.0.53/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.53/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.53/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.53/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/setDebugMode.py` & `panda-server-0.0.53/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/setPriority.py` & `panda-server-0.0.53/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testEvgen.py` & `panda-server-0.0.53/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testEvgen17.py` & `panda-server-0.0.53/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testG4sim.py` & `panda-server-0.0.53/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testG4sim17.py` & `panda-server-0.0.53/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.53/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.53/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.53/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testReco.py` & `panda-server-0.0.53/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.53/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testSiteMap.py` & `panda-server-0.0.53/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/test/testutils.py` & `panda-server-0.0.53/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/userinterface/Client.py` & `panda-server-0.0.53/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.53/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.53/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.53/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.53/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.53/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.53/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.53/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.53/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.53/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/setup.py` & `panda-server-0.0.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     description=' PanDA Server Package',
     long_description='''This package contains PanDA Server Components''',
     license='GPL',
     author='Panda Team',
     author_email='atlas-adc-panda@cern.ch',
     url='https://twiki.cern.ch/twiki/bin/view/Atlas/PanDA',
     zip_safe=False,
-    install_requires=['panda-common>=0.0.31',
+    install_requires=['panda-common>=0.0.34',
                       'panda-client',
                       'pyOpenSSL',
                       'python-daemon',
                       'mod_wsgi',
                       'six',
                       'sqlalchemy',
                       'stomp.py',
```

### Comparing `panda-server-0.0.52/templates/conda_meta.yaml.template` & `panda-server-0.0.53/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.53/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.53/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/init.d/panda_server.exe.template` & `panda-server-0.0.53/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.53/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.53/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.53/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.53/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.53/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.53/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/pandasrv.cron.template` & `panda-server-0.0.53/templates/pandasrv.cron.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.52/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.53/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

