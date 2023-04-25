# Comparing `tmp/nope_py-1.6.7.tar.gz` & `tmp/nope_py-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nope_py-1.6.7.tar", last modified: Mon Apr 24 14:02:39 2023, max compression
+gzip compressed data, was "nope_py-1.7.1.tar", last modified: Tue Apr 25 06:32:29 2023, max compression
```

## Comparing `nope_py-1.6.7.tar` & `nope_py-1.7.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:39.038529 nope_py-1.6.7/
--rw-rw-rw-   0        0        0     1083 2023-04-24 13:45:45.000000 nope_py-1.6.7/LICENSE
--rw-rw-rw-   0        0        0      650 2023-04-24 14:02:39.038529 nope_py-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-24 13:51:19.000000 nope_py-1.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.786698 nope_py-1.6.7/nope/
--rw-rw-rw-   0        0        0      525 2023-03-02 06:33:24.000000 nope_py-1.6.7/nope/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.798124 nope_py-1.6.7/nope/cli/
--rw-rw-rw-   0        0        0      439 2023-01-19 15:25:53.000000 nope_py-1.6.7/nope/cli/__init__.py
--rw-rw-rw-   0        0        0      128 2022-10-08 04:53:36.000000 nope_py-1.6.7/nope/cli/__main__.py
--rw-rw-rw-   0        0        0      707 2022-10-10 06:55:18.000000 nope_py-1.6.7/nope/cli/main.py
--rw-rw-rw-   0        0        0     7118 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/cli/run.py
--rw-rw-rw-   0        0        0     3651 2023-03-02 06:52:49.000000 nope_py-1.6.7/nope/cli/scan.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.808118 nope_py-1.6.7/nope/communication/
--rw-rw-rw-   0        0        0      130 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/communication/__init__.py
--rw-rw-rw-   0        0        0     1154 2022-11-02 06:36:13.000000 nope_py-1.6.7/nope/communication/abstractBridgePlugin.py
--rw-rw-rw-   0        0        0     5498 2022-11-11 21:37:48.000000 nope_py-1.6.7/nope/communication/bridge.py
--rw-rw-rw-   0        0        0      943 2023-02-09 15:29:20.000000 nope_py-1.6.7/nope/communication/getLayer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.820118 nope_py-1.6.7/nope/communication/layers/
--rw-rw-rw-   0        0        0     2522 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/communication/layers/EventCommunicationInterface.py
--rw-rw-rw-   0        0        0     2896 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/communication/layers/IoSocketClientLayer.py
--rw-rw-rw-   0        0        0      200 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/communication/layers/__init__.py
--rw-rw-rw-   0        0        0      903 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/communication/layers/abstractLayer.py
--rw-rw-rw-   0        0        0     6117 2022-11-22 20:19:24.000000 nope_py-1.6.7/nope/communication/layers/mqttLayer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.825119 nope_py-1.6.7/nope/decorators/
--rw-rw-rw-   0        0        0       83 2022-10-28 12:27:33.000000 nope_py-1.6.7/nope/decorators/__init__.py
--rw-rw-rw-   0        0        0     1327 2022-11-22 20:12:50.000000 nope_py-1.6.7/nope/decorators/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.827532 nope_py-1.6.7/nope/demo/
--rw-rw-rw-   0        0        0       95 2022-11-02 15:37:57.000000 nope_py-1.6.7/nope/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.835535 nope_py-1.6.7/nope/demo/instances/
--rw-rw-rw-   0        0        0     1524 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/instances/DecoratedHelloWorld.py
--rw-rw-rw-   0        0        0     1510 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/demo/instances/HelloWorld.py
--rw-rw-rw-   0        0        0     1243 2022-11-11 07:20:50.000000 nope_py-1.6.7/nope/demo/instances/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.847534 nope_py-1.6.7/nope/demo/plugins/
--rw-rw-rw-   0        0        0      977 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/plugins/00-load-hello.py
--rw-rw-rw-   0        0        0     2597 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/plugins/01-dynamic.py
--rw-rw-rw-   0        0        0     3031 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/plugins/02-multiple.py
--rw-rw-rw-   0        0        0     3284 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/plugins/03-different-items.py
--rw-rw-rw-   0        0        0     1264 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/demo/plugins/04-fix.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.854534 nope_py-1.6.7/nope/dispatcher/
--rw-rw-rw-   0        0        0      362 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/dispatcher/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.857602 nope_py-1.6.7/nope/dispatcher/baseServices/
--rw-rw-rw-   0        0        0      943 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/dispatcher/baseServices/__init__.py
--rw-rw-rw-   0        0        0     2772 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/dispatcher/baseServices/connectivy.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.863437 nope_py-1.6.7/nope/dispatcher/connectivityManager/
--rw-rw-rw-   0        0        0       57 2022-10-10 11:28:42.000000 nope_py-1.6.7/nope/dispatcher/connectivityManager/__init__.py
--rw-rw-rw-   0        0        0    12774 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/dispatcher/connectivityManager/connectivityManager.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.867836 nope_py-1.6.7/nope/dispatcher/core/
--rw-rw-rw-   0        0        0      115 2022-10-28 20:55:28.000000 nope_py-1.6.7/nope/dispatcher/core/__init__.py
--rw-rw-rw-   0        0        0     4711 2022-11-11 07:20:50.000000 nope_py-1.6.7/nope/dispatcher/core/nopeCore.py
--rw-rw-rw-   0        0        0     2175 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/dispatcher/getDispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.875836 nope_py-1.6.7/nope/dispatcher/instanceManager/
--rw-rw-rw-   0        0        0      108 2022-10-29 19:35:08.000000 nope_py-1.6.7/nope/dispatcher/instanceManager/__init__.py
--rw-rw-rw-   0        0        0      929 2022-10-10 06:40:15.000000 nope_py-1.6.7/nope/dispatcher/instanceManager/assignmentChecker.py
--rw-rw-rw-   0        0        0    34789 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/dispatcher/instanceManager/instanceManager.py
--rw-rw-rw-   0        0        0     4399 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/dispatcher/nopeDispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.883847 nope_py-1.6.7/nope/dispatcher/rpcManager/
--rw-rw-rw-   0        0        0       81 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/dispatcher/rpcManager/__init__.py
--rw-rw-rw-   0        0        0    24194 2023-01-19 16:28:00.000000 nope_py-1.6.7/nope/dispatcher/rpcManager/rpcManager.py
--rw-rw-rw-   0        0        0     3309 2023-01-19 08:26:09.000000 nope_py-1.6.7/nope/dispatcher/rpcManager/selectors.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.888839 nope_py-1.6.7/nope/eventEmitter/
--rw-rw-rw-   0        0        0       82 2022-10-10 11:28:51.000000 nope_py-1.6.7/nope/eventEmitter/__init__.py
--rw-rw-rw-   0        0        0     6698 2022-11-11 07:20:52.000000 nope_py-1.6.7/nope/eventEmitter/nopeEventEmitter.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.932765 nope_py-1.6.7/nope/helpers/
--rw-rw-rw-   0        0        0     2457 2023-01-25 06:14:09.000000 nope_py-1.6.7/nope/helpers/__init__.py
--rw-rw-rw-   0        0        0    13549 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/helpers/asyncHelpers.py
--rw-rw-rw-   0        0        0    12446 2022-11-11 07:20:53.000000 nope_py-1.6.7/nope/helpers/dictMethods.py
--rw-rw-rw-   0        0        0      720 2022-11-23 09:03:26.000000 nope_py-1.6.7/nope/helpers/dispatcherPathes.py
--rw-rw-rw-   0        0        0     4166 2023-03-02 07:08:47.000000 nope_py-1.6.7/nope/helpers/dottedDict.py
--rw-rw-rw-   0        0        0     3933 2022-10-10 11:28:37.000000 nope_py-1.6.7/nope/helpers/emitter.py
--rw-rw-rw-   0        0        0      836 2022-11-15 16:15:46.000000 nope_py-1.6.7/nope/helpers/files.py
--rw-rw-rw-   0        0        0    12428 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/helpers/hashable.py
--rw-rw-rw-   0        0        0      793 2022-11-11 20:53:45.000000 nope_py-1.6.7/nope/helpers/idMethods.py
--rw-rw-rw-   0        0        0      617 2022-10-10 06:40:15.000000 nope_py-1.6.7/nope/helpers/importing.py
--rw-rw-rw-   0        0        0     2821 2023-01-19 08:26:10.000000 nope_py-1.6.7/nope/helpers/jsonMethods.py
--rw-rw-rw-   0        0        0     2411 2023-01-19 08:26:10.000000 nope_py-1.6.7/nope/helpers/listMethods.py
--rw-rw-rw-   0        0        0    14752 2022-11-11 07:20:54.000000 nope_py-1.6.7/nope/helpers/objectMethods.py
--rw-rw-rw-   0        0        0     5206 2023-02-25 07:40:18.000000 nope_py-1.6.7/nope/helpers/path.py
--rw-rw-rw-   0        0        0    10286 2022-10-10 11:28:33.000000 nope_py-1.6.7/nope/helpers/pathMatchingMethods.py
--rw-rw-rw-   0        0        0      610 2022-10-10 06:40:15.000000 nope_py-1.6.7/nope/helpers/prints.py
--rw-rw-rw-   0        0        0     1459 2022-10-04 06:04:14.000000 nope_py-1.6.7/nope/helpers/runtime.py
--rw-rw-rw-   0        0        0      778 2022-10-10 11:28:32.000000 nope_py-1.6.7/nope/helpers/setMethods.py
--rw-rw-rw-   0        0        0     4995 2023-03-07 19:13:14.000000 nope_py-1.6.7/nope/helpers/stringMethods.py
--rw-rw-rw-   0        0        0     1894 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/helpers/timers.py
--rw-rw-rw-   0        0        0      119 2022-10-10 06:55:23.000000 nope_py-1.6.7/nope/helpers/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.942947 nope_py-1.6.7/nope/loader/
--rw-rw-rw-   0        0        0      241 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/loader/__init__.py
--rw-rw-rw-   0        0        0      777 2023-03-06 11:45:58.000000 nope_py-1.6.7/nope/loader/getPackageLoader.py
--rw-rw-rw-   0        0        0     2743 2023-03-02 08:45:55.000000 nope_py-1.6.7/nope/loader/loadPackages.py
--rw-rw-rw-   0        0        0     6529 2023-02-25 07:40:18.000000 nope_py-1.6.7/nope/loader/nopePackkageLoader.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.948244 nope_py-1.6.7/nope/logger/
--rw-rw-rw-   0        0        0      100 2022-10-10 06:40:15.000000 nope_py-1.6.7/nope/logger/__init__.py
--rw-rw-rw-   0        0        0     2505 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.952627 nope_py-1.6.7/nope/merging/
--rw-rw-rw-   0        0        0       53 2022-10-10 11:29:50.000000 nope_py-1.6.7/nope/merging/__init__.py
--rw-rw-rw-   0        0        0     2359 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/merging/mergeData.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.959548 nope_py-1.6.7/nope/modules/
--rw-rw-rw-   0        0        0      214 2022-10-10 11:30:28.000000 nope_py-1.6.7/nope/modules/__init__.py
--rw-rw-rw-   0        0        0    18241 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/modules/baseModule.py
--rw-rw-rw-   0        0        0     7829 2023-02-25 07:40:18.000000 nope_py-1.6.7/nope/modules/genericModule.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.964560 nope_py-1.6.7/nope/observable/
--rw-rw-rw-   0        0        0      157 2022-10-10 11:30:26.000000 nope_py-1.6.7/nope/observable/__init__.py
--rw-rw-rw-   0        0        0     3097 2023-01-26 07:25:35.000000 nope_py-1.6.7/nope/observable/nopeObservable.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.985548 nope_py-1.6.7/nope/plugins/
--rw-rw-rw-   0        0        0      129 2022-11-11 20:52:06.000000 nope_py-1.6.7/nope/plugins/__init__.py
--rw-rw-rw-   0        0        0     6213 2022-11-11 07:20:56.000000 nope_py-1.6.7/nope/plugins/ack_messages.py
--rw-rw-rw-   0        0        0      946 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/plugins/hello.py
--rw-rw-rw-   0        0        0    22410 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/plugins/plugin.py
--rw-rw-rw-   0        0        0    16526 2022-11-15 16:15:53.000000 nope_py-1.6.7/nope/plugins/rpc_with_callbacks.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:38.998550 nope_py-1.6.7/nope/pubSub/
--rw-rw-rw-   0        0        0       96 2022-11-07 07:10:33.000000 nope_py-1.6.7/nope/pubSub/__init__.py
--rw-rw-rw-   0        0        0     3810 2022-10-10 11:30:55.000000 nope_py-1.6.7/nope/pubSub/nopeDataPubSubSystem.py
--rw-rw-rw-   0        0        0    20054 2023-03-02 07:08:18.000000 nope_py-1.6.7/nope/pubSub/nopePubSubSystem.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:39.000549 nope_py-1.6.7/nope/types/
--rw-rw-rw-   0        0        0     3468 2022-11-22 16:51:58.000000 nope_py-1.6.7/nope/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:39.019551 nope_py-1.6.7/nope_py.egg-info/
--rw-rw-rw-   0        0        0      650 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3070 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-24 14:02:38.000000 nope_py-1.6.7/nope_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-04-24 14:02:39.038529 nope_py-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2578 2023-04-24 14:02:36.000000 nope_py-1.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:02:39.037440 nope_py-1.6.7/test/
--rw-rw-rw-   0        0        0     1427 2022-11-07 07:10:33.000000 nope_py-1.6.7/test/test.py
--rw-rw-rw-   0        0        0     2144 2022-11-07 07:10:33.000000 nope_py-1.6.7/test/test_communicator.py
--rw-rw-rw-   0        0        0     3047 2022-11-07 07:10:33.000000 nope_py-1.6.7/test/test_plugin.py
--rw-rw-rw-   0        0        0     1606 2022-11-11 07:20:58.000000 nope_py-1.6.7/test/test_plugin_bridge.py
--rw-rw-rw-   0        0        0     1454 2022-11-15 16:15:55.000000 nope_py-1.6.7/test/test_plugin_rpc_callbacks.py
--rw-rw-rw-   0        0        0      682 2023-01-19 08:26:15.000000 nope_py-1.6.7/test/test_pub_sub.py
--rw-rw-rw-   0        0        0     3254 2022-11-07 07:10:33.000000 nope_py-1.6.7/test/test_rpc_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.489349 nope_py-1.7.1/
+-rw-rw-rw-   0        0        0     1083 2023-04-24 13:45:45.000000 nope_py-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-04-25 06:32:29.490349 nope_py-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-24 13:51:19.000000 nope_py-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.178944 nope_py-1.7.1/nope/
+-rw-rw-rw-   0        0        0      525 2023-03-02 06:33:24.000000 nope_py-1.7.1/nope/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.192231 nope_py-1.7.1/nope/cli/
+-rw-rw-rw-   0        0        0      439 2023-01-19 15:25:53.000000 nope_py-1.7.1/nope/cli/__init__.py
+-rw-rw-rw-   0        0        0      128 2022-10-08 04:53:36.000000 nope_py-1.7.1/nope/cli/__main__.py
+-rw-rw-rw-   0        0        0      707 2022-10-10 06:55:18.000000 nope_py-1.7.1/nope/cli/main.py
+-rw-rw-rw-   0        0        0     7118 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/cli/run.py
+-rw-rw-rw-   0        0        0     3651 2023-03-02 06:52:49.000000 nope_py-1.7.1/nope/cli/scan.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.203944 nope_py-1.7.1/nope/communication/
+-rw-rw-rw-   0        0        0      130 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/communication/__init__.py
+-rw-rw-rw-   0        0        0     1154 2022-11-02 06:36:13.000000 nope_py-1.7.1/nope/communication/abstractBridgePlugin.py
+-rw-rw-rw-   0        0        0     5498 2022-11-11 21:37:48.000000 nope_py-1.7.1/nope/communication/bridge.py
+-rw-rw-rw-   0        0        0      943 2023-02-09 15:29:20.000000 nope_py-1.7.1/nope/communication/getLayer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.220059 nope_py-1.7.1/nope/communication/layers/
+-rw-rw-rw-   0        0        0     2522 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/communication/layers/EventCommunicationInterface.py
+-rw-rw-rw-   0        0        0     2896 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/communication/layers/IoSocketClientLayer.py
+-rw-rw-rw-   0        0        0      200 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/communication/layers/__init__.py
+-rw-rw-rw-   0        0        0      903 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/communication/layers/abstractLayer.py
+-rw-rw-rw-   0        0        0     6117 2022-11-22 20:19:24.000000 nope_py-1.7.1/nope/communication/layers/mqttLayer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.226060 nope_py-1.7.1/nope/decorators/
+-rw-rw-rw-   0        0        0       83 2022-10-28 12:27:33.000000 nope_py-1.7.1/nope/decorators/__init__.py
+-rw-rw-rw-   0        0        0     1327 2022-11-22 20:12:50.000000 nope_py-1.7.1/nope/decorators/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.229060 nope_py-1.7.1/nope/demo/
+-rw-rw-rw-   0        0        0       95 2022-11-02 15:37:57.000000 nope_py-1.7.1/nope/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.238193 nope_py-1.7.1/nope/demo/instances/
+-rw-rw-rw-   0        0        0     1524 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/instances/DecoratedHelloWorld.py
+-rw-rw-rw-   0        0        0     1510 2023-03-02 07:08:18.000000 nope_py-1.7.1/nope/demo/instances/HelloWorld.py
+-rw-rw-rw-   0        0        0     1243 2022-11-11 07:20:50.000000 nope_py-1.7.1/nope/demo/instances/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.254202 nope_py-1.7.1/nope/demo/plugins/
+-rw-rw-rw-   0        0        0      977 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/plugins/00-load-hello.py
+-rw-rw-rw-   0        0        0     2597 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/plugins/01-dynamic.py
+-rw-rw-rw-   0        0        0     3031 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/plugins/02-multiple.py
+-rw-rw-rw-   0        0        0     3284 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/plugins/03-different-items.py
+-rw-rw-rw-   0        0        0     1264 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/demo/plugins/04-fix.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.262204 nope_py-1.7.1/nope/dispatcher/
+-rw-rw-rw-   0        0        0      362 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/dispatcher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.268206 nope_py-1.7.1/nope/dispatcher/baseServices/
+-rw-rw-rw-   0        0        0      943 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/dispatcher/baseServices/__init__.py
+-rw-rw-rw-   0        0        0     2772 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/dispatcher/baseServices/connectivy.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.275236 nope_py-1.7.1/nope/dispatcher/connectivityManager/
+-rw-rw-rw-   0        0        0       57 2022-10-10 11:28:42.000000 nope_py-1.7.1/nope/dispatcher/connectivityManager/__init__.py
+-rw-rw-rw-   0        0        0    12774 2023-03-02 07:08:18.000000 nope_py-1.7.1/nope/dispatcher/connectivityManager/connectivityManager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.281931 nope_py-1.7.1/nope/dispatcher/core/
+-rw-rw-rw-   0        0        0      115 2022-10-28 20:55:28.000000 nope_py-1.7.1/nope/dispatcher/core/__init__.py
+-rw-rw-rw-   0        0        0     4711 2022-11-11 07:20:50.000000 nope_py-1.7.1/nope/dispatcher/core/nopeCore.py
+-rw-rw-rw-   0        0        0     2175 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/dispatcher/getDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.290928 nope_py-1.7.1/nope/dispatcher/instanceManager/
+-rw-rw-rw-   0        0        0      108 2022-10-29 19:35:08.000000 nope_py-1.7.1/nope/dispatcher/instanceManager/__init__.py
+-rw-rw-rw-   0        0        0      929 2022-10-10 06:40:15.000000 nope_py-1.7.1/nope/dispatcher/instanceManager/assignmentChecker.py
+-rw-rw-rw-   0        0        0    39458 2023-04-24 14:24:50.000000 nope_py-1.7.1/nope/dispatcher/instanceManager/instanceManager.py
+-rw-rw-rw-   0        0        0     4399 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/dispatcher/nopeDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.300452 nope_py-1.7.1/nope/dispatcher/rpcManager/
+-rw-rw-rw-   0        0        0       81 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/dispatcher/rpcManager/__init__.py
+-rw-rw-rw-   0        0        0    24360 2023-04-24 14:26:18.000000 nope_py-1.7.1/nope/dispatcher/rpcManager/rpcManager.py
+-rw-rw-rw-   0        0        0     3309 2023-01-19 08:26:09.000000 nope_py-1.7.1/nope/dispatcher/rpcManager/selectors.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.306466 nope_py-1.7.1/nope/eventEmitter/
+-rw-rw-rw-   0        0        0       82 2022-10-10 11:28:51.000000 nope_py-1.7.1/nope/eventEmitter/__init__.py
+-rw-rw-rw-   0        0        0     6698 2022-11-11 07:20:52.000000 nope_py-1.7.1/nope/eventEmitter/nopeEventEmitter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.371168 nope_py-1.7.1/nope/helpers/
+-rw-rw-rw-   0        0        0     2457 2023-01-25 06:14:09.000000 nope_py-1.7.1/nope/helpers/__init__.py
+-rw-rw-rw-   0        0        0    13549 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/helpers/asyncHelpers.py
+-rw-rw-rw-   0        0        0    12446 2022-11-11 07:20:53.000000 nope_py-1.7.1/nope/helpers/dictMethods.py
+-rw-rw-rw-   0        0        0      720 2022-11-23 09:03:26.000000 nope_py-1.7.1/nope/helpers/dispatcherPathes.py
+-rw-rw-rw-   0        0        0     4166 2023-03-02 07:08:47.000000 nope_py-1.7.1/nope/helpers/dottedDict.py
+-rw-rw-rw-   0        0        0     3933 2022-10-10 11:28:37.000000 nope_py-1.7.1/nope/helpers/emitter.py
+-rw-rw-rw-   0        0        0      836 2022-11-15 16:15:46.000000 nope_py-1.7.1/nope/helpers/files.py
+-rw-rw-rw-   0        0        0    12428 2023-03-02 07:08:18.000000 nope_py-1.7.1/nope/helpers/hashable.py
+-rw-rw-rw-   0        0        0      793 2022-11-11 20:53:45.000000 nope_py-1.7.1/nope/helpers/idMethods.py
+-rw-rw-rw-   0        0        0      617 2022-10-10 06:40:15.000000 nope_py-1.7.1/nope/helpers/importing.py
+-rw-rw-rw-   0        0        0     2821 2023-01-19 08:26:10.000000 nope_py-1.7.1/nope/helpers/jsonMethods.py
+-rw-rw-rw-   0        0        0     2411 2023-01-19 08:26:10.000000 nope_py-1.7.1/nope/helpers/listMethods.py
+-rw-rw-rw-   0        0        0    14752 2022-11-11 07:20:54.000000 nope_py-1.7.1/nope/helpers/objectMethods.py
+-rw-rw-rw-   0        0        0     5206 2023-02-25 07:40:18.000000 nope_py-1.7.1/nope/helpers/path.py
+-rw-rw-rw-   0        0        0    10739 2023-04-24 14:30:38.000000 nope_py-1.7.1/nope/helpers/pathMatchingMethods.py
+-rw-rw-rw-   0        0        0      610 2022-10-10 06:40:15.000000 nope_py-1.7.1/nope/helpers/prints.py
+-rw-rw-rw-   0        0        0     1459 2022-10-04 06:04:14.000000 nope_py-1.7.1/nope/helpers/runtime.py
+-rw-rw-rw-   0        0        0      778 2022-10-10 11:28:32.000000 nope_py-1.7.1/nope/helpers/setMethods.py
+-rw-rw-rw-   0        0        0     4995 2023-03-07 19:13:14.000000 nope_py-1.7.1/nope/helpers/stringMethods.py
+-rw-rw-rw-   0        0        0     1894 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/helpers/timers.py
+-rw-rw-rw-   0        0        0      119 2022-10-10 06:55:23.000000 nope_py-1.7.1/nope/helpers/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.383112 nope_py-1.7.1/nope/loader/
+-rw-rw-rw-   0        0        0      241 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/loader/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-03-06 11:45:58.000000 nope_py-1.7.1/nope/loader/getPackageLoader.py
+-rw-rw-rw-   0        0        0     2743 2023-03-02 08:45:55.000000 nope_py-1.7.1/nope/loader/loadPackages.py
+-rw-rw-rw-   0        0        0     6529 2023-02-25 07:40:18.000000 nope_py-1.7.1/nope/loader/nopePackkageLoader.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.389114 nope_py-1.7.1/nope/logger/
+-rw-rw-rw-   0        0        0      100 2022-10-10 06:40:15.000000 nope_py-1.7.1/nope/logger/__init__.py
+-rw-rw-rw-   0        0        0     2505 2023-03-02 07:08:18.000000 nope_py-1.7.1/nope/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.396281 nope_py-1.7.1/nope/merging/
+-rw-rw-rw-   0        0        0       53 2022-10-10 11:29:50.000000 nope_py-1.7.1/nope/merging/__init__.py
+-rw-rw-rw-   0        0        0     2359 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/merging/mergeData.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.407283 nope_py-1.7.1/nope/modules/
+-rw-rw-rw-   0        0        0      214 2022-10-10 11:30:28.000000 nope_py-1.7.1/nope/modules/__init__.py
+-rw-rw-rw-   0        0        0    18241 2023-03-02 07:08:18.000000 nope_py-1.7.1/nope/modules/baseModule.py
+-rw-rw-rw-   0        0        0     7829 2023-02-25 07:40:18.000000 nope_py-1.7.1/nope/modules/genericModule.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.413282 nope_py-1.7.1/nope/observable/
+-rw-rw-rw-   0        0        0      157 2022-10-10 11:30:26.000000 nope_py-1.7.1/nope/observable/__init__.py
+-rw-rw-rw-   0        0        0     3097 2023-01-26 07:25:35.000000 nope_py-1.7.1/nope/observable/nopeObservable.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.428734 nope_py-1.7.1/nope/plugins/
+-rw-rw-rw-   0        0        0      129 2022-11-11 20:52:06.000000 nope_py-1.7.1/nope/plugins/__init__.py
+-rw-rw-rw-   0        0        0     6213 2022-11-11 07:20:56.000000 nope_py-1.7.1/nope/plugins/ack_messages.py
+-rw-rw-rw-   0        0        0      946 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/plugins/hello.py
+-rw-rw-rw-   0        0        0    22410 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/plugins/plugin.py
+-rw-rw-rw-   0        0        0    16526 2022-11-15 16:15:53.000000 nope_py-1.7.1/nope/plugins/rpc_with_callbacks.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.438735 nope_py-1.7.1/nope/pubSub/
+-rw-rw-rw-   0        0        0       96 2022-11-07 07:10:33.000000 nope_py-1.7.1/nope/pubSub/__init__.py
+-rw-rw-rw-   0        0        0     3810 2022-10-10 11:30:55.000000 nope_py-1.7.1/nope/pubSub/nopeDataPubSubSystem.py
+-rw-rw-rw-   0        0        0    18864 2023-04-24 14:53:00.000000 nope_py-1.7.1/nope/pubSub/nopePubSubSystem.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.441736 nope_py-1.7.1/nope/types/
+-rw-rw-rw-   0        0        0     3468 2022-11-22 16:51:58.000000 nope_py-1.7.1/nope/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.466313 nope_py-1.7.1/nope_py.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-04-25 06:32:28.000000 nope_py-1.7.1/nope_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3070 2023-04-25 06:32:29.000000 nope_py-1.7.1/nope_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:32:28.000000 nope_py-1.7.1/nope_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-25 06:32:28.000000 nope_py-1.7.1/nope_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-25 06:32:28.000000 nope_py-1.7.1/nope_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 06:32:28.000000 nope_py-1.7.1/nope_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-04-25 06:32:29.493110 nope_py-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2555 2023-04-25 06:32:12.000000 nope_py-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:32:29.486986 nope_py-1.7.1/test/
+-rw-rw-rw-   0        0        0     1427 2022-11-07 07:10:33.000000 nope_py-1.7.1/test/test.py
+-rw-rw-rw-   0        0        0     2144 2022-11-07 07:10:33.000000 nope_py-1.7.1/test/test_communicator.py
+-rw-rw-rw-   0        0        0     3047 2022-11-07 07:10:33.000000 nope_py-1.7.1/test/test_plugin.py
+-rw-rw-rw-   0        0        0     1606 2022-11-11 07:20:58.000000 nope_py-1.7.1/test/test_plugin_bridge.py
+-rw-rw-rw-   0        0        0     1454 2022-11-15 16:15:55.000000 nope_py-1.7.1/test/test_plugin_rpc_callbacks.py
+-rw-rw-rw-   0        0        0      682 2023-01-19 08:26:15.000000 nope_py-1.7.1/test/test_pub_sub.py
+-rw-rw-rw-   0        0        0     3254 2022-11-07 07:10:33.000000 nope_py-1.7.1/test/test_rpc_manager.py
```

### Comparing `nope_py-1.6.7/LICENSE` & `nope_py-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/PKG-INFO` & `nope_py-1.7.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope_py
-Version: 1.6.7
+Version: 1.7.1
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/anti-held-333/nope-py.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.6.7/nope/__init__.py` & `nope_py-1.7.1/nope/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/cli/main.py` & `nope_py-1.7.1/nope/cli/main.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/cli/run.py` & `nope_py-1.7.1/nope/cli/run.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/cli/scan.py` & `nope_py-1.7.1/nope/cli/scan.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/abstractBridgePlugin.py` & `nope_py-1.7.1/nope/communication/abstractBridgePlugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/bridge.py` & `nope_py-1.7.1/nope/communication/bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/getLayer.py` & `nope_py-1.7.1/nope/communication/getLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/layers/EventCommunicationInterface.py` & `nope_py-1.7.1/nope/communication/layers/EventCommunicationInterface.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/layers/IoSocketClientLayer.py` & `nope_py-1.7.1/nope/communication/layers/IoSocketClientLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/layers/abstractLayer.py` & `nope_py-1.7.1/nope/communication/layers/abstractLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/communication/layers/mqttLayer.py` & `nope_py-1.7.1/nope/communication/layers/mqttLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/decorators/classes.py` & `nope_py-1.7.1/nope/decorators/classes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/instances/DecoratedHelloWorld.py` & `nope_py-1.7.1/nope/demo/instances/DecoratedHelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/instances/HelloWorld.py` & `nope_py-1.7.1/nope/demo/instances/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/instances/__init__.py` & `nope_py-1.7.1/nope/demo/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/plugins/00-load-hello.py` & `nope_py-1.7.1/nope/demo/plugins/00-load-hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/plugins/01-dynamic.py` & `nope_py-1.7.1/nope/demo/plugins/01-dynamic.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/plugins/02-multiple.py` & `nope_py-1.7.1/nope/demo/plugins/02-multiple.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/plugins/03-different-items.py` & `nope_py-1.7.1/nope/demo/plugins/03-different-items.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/demo/plugins/04-fix.py` & `nope_py-1.7.1/nope/demo/plugins/04-fix.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/baseServices/__init__.py` & `nope_py-1.7.1/nope/dispatcher/baseServices/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/baseServices/connectivy.py` & `nope_py-1.7.1/nope/dispatcher/baseServices/connectivy.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/connectivityManager/connectivityManager.py` & `nope_py-1.7.1/nope/dispatcher/connectivityManager/connectivityManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/core/nopeCore.py` & `nope_py-1.7.1/nope/dispatcher/core/nopeCore.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/getDispatcher.py` & `nope_py-1.7.1/nope/dispatcher/getDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/instanceManager/assignmentChecker.py` & `nope_py-1.7.1/nope/dispatcher/instanceManager/assignmentChecker.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/instanceManager/instanceManager.py` & `nope_py-1.7.1/nope/dispatcher/instanceManager/instanceManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,18 +113,17 @@
 
         if self._logger:
             self._logger.info('core.instance-manager online')
 
         self.reset()
         EXECUTOR.callParallel(self._init)
 
-    def _sendAvailableInstances(self):
+    async def _sendAvailableInstances(self):
         # Update the Instances provided by this module.
-        EXECUTOR.callParallel(
-            self._communicator.emit,
+        await self._communicator.emit(
             "instancesChanged",
             {
                 "dispatcher": self._id,
                 # We will send the descriptions.
                 # Generate the Module Description for every identifier:
                 "instances": list(
                     map(lambda item: self._instances[item]["instance"].toDescription(), self._internalInstances))
@@ -157,24 +156,27 @@
         def _onDispatchersChanged(changes, *args):
             """ Callback which will handle new and offline Dispatchers.
             """
 
             if len(changes.added):
                 # If there are dispatchers online,
                 # We will emit our available services.
-                self._sendAvailableInstances()
+                EXECUTOR.callParallel(self._sendAvailableInstances)
 
             if len(changes.removed):
                 # Remove the dispatchers.
                 for removedId in changes.removed:
                     self.removeDispatcher(removedId)
 
         # We will use our status-manager to listen to changes.
         self._connectivityManager.dispatchers.onChange.subscribe(
             _onDispatchersChanged)
+        
+        # Make shure we are emitting the instances provided.
+        self._communicator.on("bonjour", lambda *args : EXECUTOR.callParallel(self._sendAvailableInstances))
 
         def _onInstancesChanged(message, *args):
             """ Callback which will be called if the commincator receives a Message
                 that some instances has been changed.
 
             Args:
                 message: The Message from the System.
@@ -333,15 +335,15 @@
                                         # Remove the Instance.
                                         await _instance.dispose()
                                         # Removes the instances
                                         self._instances.pop(data.identifier)
                                         # Remove the Function itself
                                         await self._rpcManager.unregisterService(self.getServiceName(data.identifier, 'dispose'))
                                         # Emit the instances again
-                                        self._sendAvailableInstances()
+                                        await self._sendAvailableInstances()
 
                                 except ValueError:
                                     pass
 
                         # A Function is registered, taking care of removing
                         # an instances, if it isnt needed any more.
                         await self._rpcManager.registerService(
@@ -359,15 +361,15 @@
                             'instance': _instance,
                             'usedBy': [data.dispatcherId]
                         })
 
                         self._internalInstances.add(data.identifier)
 
                         # Update the available instances:
-                        self._sendAvailableInstances()
+                        await self._sendAvailableInstances()
 
                         # Make shure, we remove this instance.hash
                         self._initializingInstance.pop(data.identifier)
 
                     except BaseException as E:
                         # Make shure, we remove this instance.hash
                         self._initializingInstance.pop(data.identifier)
@@ -477,44 +479,45 @@
         Args:
             identifier (str):  identifier of the instance.
             externalOnly (bool, optional): If set to true we will only look for external instances in the external dispatchers. Defaults to True.
 
         Returns:
             bool: The Testresult
         """
+        if identifier not in self.instances.simplified:
+            return False
+
         if externalOnly:
-            return identifier in self._externalInstances
-        else:
-            return identifier in self._externalInstances or identifier in self._instances
+            manager = self.getManagerOfInstance(identifier)
+            return manager["id"] != self._id
+        
+        return True
 
     def getManagerOfInstance(self, identifier: str):
         """ Returns the hosting dispatcher for the given instance.
 
         Args:
             identifier (str): The identifier for instance (its name)
 
         Returns:
             INopeStatusInfo | False: The Status or false if not present.
         """
-        # Check if the instance exists in general
-        if not self.instanceExists(identifier, False):
-            return None
-
         # First we will check if the instance is available internally
         if identifier in self._internalInstances:
             return self._connectivityManager.info
 
         # If that isnt the case, we will check all dispatchers and search the
         # instance.
         for iter_item in self._mappingOfRemoteDispatchersAndInstances.items():
             dispatcher = iter_item[0]
             msg = iter_item[1]
             for instance in msg.instances:
                 if instance.identifier == identifier:
                     return self._connectivityManager.getStatus(dispatcher)
+                
         return None
 
     def getInstanceDescription(self, instanceIdentifier: str):
         """ Returns the instance Description for a specific instance. It is just a simplified wrapper
             for the "instances"-property.
 
         Args:
@@ -677,14 +680,114 @@
             if self._logger:
                 self._logger.error(
                     'During creating an Instance, the following error Occurd')
                 self._logger.error(formatException(e))
 
             raise e
 
+    
+    async def generateWrapper(self, description):
+        # Define the Default Description
+        # which will lead to an error.
+        description = ensureDottedAccess(description)
+
+        # Assign the provided Description
+        _description = ensureDottedAccess({
+            'dispatcherId': self._id,
+            'identifier': 'error',
+            'params': [],
+            'type': 'unkown'
+        })
+        _description.update(description)
+        _description.update({'dispatcherId': self._id})
+
+        # Check if the Description is complete
+        if (_description.type == 'unkown' or _description.identifier) == 'error':
+            raise Exception(
+                'Please Provide at least a "type" and "identifier" in the paremeters')
+
+        # Use the varified Name (removes the invalid chars.)
+        _description.identifier = varifyPath(
+            _description.identifier) if self.options.forceUsingValidVarNames else _description.identifier
+        if self._logger:
+            self._logger.debug('Requesting an Instance of type: "' + _description.type +
+                               '" with the identifier: "' + _description.identifier + '"')
+
+        try:
+            _type = _description.type
+            if _type not in self._internalWrapperGenerators:
+                _type = '*'
+
+            if not self.constructorExists(_description.type):
+                # No default type is present for a remote
+                # => assing the default type which is "*""
+                raise Exception('Generator "' + _description.type +
+                                '" isnt present in the network!')
+            if _type in self._internalWrapperGenerators:
+                if self._logger:
+                    self._logger.debug('No instance with the identifiert: "' + _description.identifier +
+                                       '" found, but an internal generator is available. Using the internal one for creating the instance and requesting the "real" instance externally')
+
+                # Now test if there is allready an instance with this name and type.
+                # If so, we check if we have the correct type etc. Additionally we
+                # try to extract its dispatcher-id and will use that as selector
+                # to allow the function be called.
+
+                _instanceDetails = self._getInstanceInfo(
+                    _description.identifier)
+
+
+                if _instanceDetails is not None and _instanceDetails.description.type != _description.type:
+                    raise Exception(
+                        "There exists an Instance named: '" + _description.identifier + "' but it uses a different type. Requested type: '" +
+                        _description.type + "', given type: '" + _instanceDetails.description.type + "'")
+
+                elif _instanceDetails is None:
+                    raise Exception(
+                        'No instance known with the idenfitier "' + _description.identifier +'" !')
+
+                definedInstance = _instanceDetails.description
+
+                # Create the Wrapper for our instance.
+                wrapper = await self._internalWrapperGenerators.get(_type)(self._core, definedInstance.description)
+                if self._logger:
+                    self._logger.debug(
+                        f'Created a Wrapper for the instance "{definedInstance.description.identifier}"')
+
+                originalDispose = wrapper.dispose
+
+                async def dispose():
+                    await self.deleteInstance(wrapper.indentifier)
+
+                    await originalDispose()
+
+                setattr(wrapper, "dispose", dispose)
+
+                self._instances[_description.identifier] = ensureDottedAccess({
+                    'instance': wrapper,
+                    'usedBy': [
+                        _description.dispatcherId
+                    ]
+                }
+                )
+
+                return wrapper
+
+            raise Exception('No internal generator Available!')
+
+        except Exception as e:
+
+            if self._logger:
+                self._logger.error(
+                    'During creating an Instance, the following error Occurd')
+                self._logger.error(formatException(e))
+
+            raise e
+    
+    
     async def registerInstance(self, instance):
         """ Option, to statically register an instance, without using an specific generator etc.
             This instance is just present in the network.
 
         Args:
             instance (INopeInstance): The Instnce to register
 
@@ -693,14 +796,19 @@
         """
         self._instances[instance.identifier] = ensureDottedAccess({
             'instance': instance,
             'usedBy': [],
             'manual': True
         }
         )
+
+        self._internalInstances.add(instance.identifier)
+        
+        await self._sendAvailableInstances()
+
         return instance
 
     async def deleteInstance(self, instance, preventSendingUpdate=False) -> bool:
         """ Disposes an instance and removes it. Thereby the Instance wont be available for other
             InstanceManagers in the system.
 
         Args:
@@ -758,15 +866,15 @@
 
                 # Delete the Identifier
                 self._instances.pop(_instance.instance.identifier)
 
                 # Check if an update should be emitted or not.
                 if not preventSendingUpdate:
                     # Update the Instances provided by this module.
-                    self._sendAvailableInstances()
+                    await self._sendAvailableInstances()
 
                 await _instance.instance.dispose()
             return True
         return False
 
     async def getInstancesOfType(self, typeToGet: str):
         """ Creates Wrappers for the Type of the given element.
@@ -832,15 +940,15 @@
         self._externalInstances = dict()
         self._internalInstances = set()
         self._initializingInstance = dict()
         self._externalInstancesNames = set()
         self.internalInstances.setContent([])
 
         if self._communicator.connected.getContent():
-            self._sendAvailableInstances()
+            EXECUTOR.callParallel(self._sendAvailableInstances)
 
     async def dispose(self):
         self.reset()
         self.instances.dispose()
 
     def __del__(self):
         EXECUTOR.callParallel(self.dispose, target=self)
```

### Comparing `nope_py-1.6.7/nope/dispatcher/nopeDispatcher.py` & `nope_py-1.7.1/nope/dispatcher/nopeDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/dispatcher/rpcManager/rpcManager.py` & `nope_py-1.7.1/nope/dispatcher/rpcManager/rpcManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,17 @@
 
         def on_unregister(msg):
             if msg.identifier in self._registeredServices:
                 self.unregisterService(msg.identifier)
 
         await self._communicator.on("rpcUnregister", on_unregister)
 
+        # We are now listening on these changes!
+        await self._communicator.on("bonjour", lambda *args: EXECUTOR.callParallel(self._sendAvailableServices))
+
         def onDispatchersChanged(changes, *args):
             if len(changes.added):
                 # If there are dispatchers online,
                 # We will emit our available services.
                 EXECUTOR.callParallel(self._sendAvailableServices)
             if len(changes.removed):
                 for rm in changes.removed:
```

### Comparing `nope_py-1.6.7/nope/dispatcher/rpcManager/selectors.py` & `nope_py-1.7.1/nope/dispatcher/rpcManager/selectors.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/eventEmitter/nopeEventEmitter.py` & `nope_py-1.7.1/nope/eventEmitter/nopeEventEmitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/__init__.py` & `nope_py-1.7.1/nope/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/asyncHelpers.py` & `nope_py-1.7.1/nope/helpers/asyncHelpers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/dictMethods.py` & `nope_py-1.7.1/nope/helpers/dictMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/dispatcherPathes.py` & `nope_py-1.7.1/nope/helpers/dispatcherPathes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/dottedDict.py` & `nope_py-1.7.1/nope/helpers/dottedDict.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/emitter.py` & `nope_py-1.7.1/nope/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/files.py` & `nope_py-1.7.1/nope/helpers/files.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/hashable.py` & `nope_py-1.7.1/nope/helpers/hashable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/idMethods.py` & `nope_py-1.7.1/nope/helpers/idMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/importing.py` & `nope_py-1.7.1/nope/helpers/importing.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/jsonMethods.py` & `nope_py-1.7.1/nope/helpers/jsonMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/listMethods.py` & `nope_py-1.7.1/nope/helpers/listMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/objectMethods.py` & `nope_py-1.7.1/nope/helpers/objectMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/path.py` & `nope_py-1.7.1/nope/helpers/path.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/pathMatchingMethods.py` & `nope_py-1.7.1/nope/helpers/pathMatchingMethods.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,14 +173,23 @@
                     DottedDict({
                         'affectedByParent': True,
                         'patternToExtractData': pathPattern,
                         'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
                         'containsWildcards': _containsWildcards
                     })
                 )
+            elif patternLengthComparedToPathLength == ">":
+                return generateResult(
+                    DottedDict({
+                        'affectedByParent': True,
+                        'patternToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
             else:
                 raise Exception('Implementation Error! This should not happen')
         elif currentPath == currentPattern:
             # The Patterns Match
             # We now store the correct path of our segment.
             partialPath = f'{partialPath}{SPLITCHAR}{currentPath}' if len(
                 partialPath) > 0 else currentPath
@@ -231,12 +240,12 @@
             return generateResult(DottedDict({
                 'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
                 'containsWildcards': _containsWildcards
             }))
     diff = contentPath[len(partialPath):]
     return generateResult(DottedDict({
         'affectedOnSameLevel': len(diff) == 0,
-        'affectedByChild': len(diff) > 1,
+        'affectedByChild': len(diff) >= 1,
         'pathToExtractData': partialPath,
         'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
         'containsWildcards': _containsWildcards
     }))
```

### Comparing `nope_py-1.6.7/nope/helpers/prints.py` & `nope_py-1.7.1/nope/helpers/prints.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/runtime.py` & `nope_py-1.7.1/nope/helpers/runtime.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/setMethods.py` & `nope_py-1.7.1/nope/helpers/setMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/stringMethods.py` & `nope_py-1.7.1/nope/helpers/stringMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/helpers/timers.py` & `nope_py-1.7.1/nope/helpers/timers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/loader/getPackageLoader.py` & `nope_py-1.7.1/nope/loader/getPackageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/loader/loadPackages.py` & `nope_py-1.7.1/nope/loader/loadPackages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/loader/nopePackkageLoader.py` & `nope_py-1.7.1/nope/loader/nopePackkageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/logger/logger.py` & `nope_py-1.7.1/nope/logger/logger.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/merging/mergeData.py` & `nope_py-1.7.1/nope/merging/mergeData.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/modules/baseModule.py` & `nope_py-1.7.1/nope/modules/baseModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/modules/genericModule.py` & `nope_py-1.7.1/nope/modules/genericModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/observable/nopeObservable.py` & `nope_py-1.7.1/nope/observable/nopeObservable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/plugins/ack_messages.py` & `nope_py-1.7.1/nope/plugins/ack_messages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/plugins/hello.py` & `nope_py-1.7.1/nope/plugins/hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/plugins/plugin.py` & `nope_py-1.7.1/nope/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/plugins/rpc_with_callbacks.py` & `nope_py-1.7.1/nope/plugins/rpc_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/pubSub/nopeDataPubSubSystem.py` & `nope_py-1.7.1/nope/pubSub/nopeDataPubSubSystem.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope/pubSub/nopePubSubSystem.py` & `nope_py-1.7.1/nope/pubSub/nopePubSubSystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
             # Register the emitter. This will be used during topic matching.
             self._emitters[emitter] = ensureDottedAccess(
                 {'options': options, 'pubTopic': pubTopic, 'subTopic': subTopic, 'callback': callback,
                  'observer': observer})
 
             # Update the Matching Rules.
-            self._updatePartialMatching('add', emitter, pubTopic, subTopic)
+            self.updateMatching()
 
             if callback:
                 # If necessary. Add the Callback.
                 observer = emitter.subscribe(callback, ensureDottedAccess(
                     {'skipCurrent': not self._sendCurrentDataOnSubscription}))
                 # Now lets store our binding.
                 self._emittersToObservers[emitter] = observer
@@ -184,23 +184,22 @@
 
     def updateOptions(self, emitter, options):
         # We will adapat the Options, for dotted access.
         options = ensureDottedAccess(options)
         if emitter in self._emitters:
             subTopic, pubTopic = _extractPubAndSubTopic(options)
             data = self._emitters.get(emitter)
-            self._updatePartialMatching(
-                'remove', emitter, data.pubTopic, data.subTopic)
-
+            
             data.options = options
             data.subTopic = subTopic
             data.pubTopic = pubTopic
 
             self._emitters[emitter] = data
-            self._updatePartialMatching('add', emitter, pubTopic, subTopic)
+            
+            self.updateMatching()
         else:
             raise Exception('Emitter is not registered')
 
     def unregister(self, emitter):
         if emitter in self._emitters:
             options = self._emitters.pop(emitter)
             subTopic, pubTopic = _extractPubAndSubTopic(options["options"])
@@ -218,36 +217,26 @@
 
     @property
     def emitters(self):
         # TODO:
         pass
 
     def updateMatching(self):
+
         self._matched.clear()
-        for emitter, item in self._emitters.items():
-            # Extract the topic
-            subTopic = item.get("subTopic", False)
+
+        for item in self._emitters.values():
+            # Extract the publisher topic
             pubTopic = item.get("pubTopic", False)
 
-            if pubTopic:
+            if pubTopic is not False:
                 self._updateMatchingForTopic(pubTopic)
 
-            if subTopic:
-                self._addMatchingEntryIfRequired(subTopic, subTopic, emitter)
-                self.publishers.update()
-
-            self.subscriptions.update()
-
-    def _deleteMatchingEntry(self, pubTopic, subTopic, emitter):
-        if pubTopic in self._matched:
-            data = self._matched.get(pubTopic)
-            if subTopic in data.dataPull:
-                data.dataPull.get(subTopic).remove(emitter)
-            if subTopic in data.dataQuery:
-                data.dataQuery.get(subTopic).remove(emitter)
+        self.subscriptions.update()
+        self.publishers.update()
 
     def _addMatchingEntryIfRequired(self, pubTopic, subTopic, emitter):
         result = self._comparePatternAndPath(subTopic, pubTopic)
         if result.affected:
             if not result.containsWildcards and ((result.affectedByChild and not self.options.forwardChildData) or
                                                  (
                 result.affectedByParent and not self.options.forwardParentData)
@@ -261,58 +250,36 @@
             #    - child based change => content
             # 2) subscription doesnt contains a pattern:
             #    We more or less want the data on the path.
             #    - direct change (topic = path) => content
             #    - parent based change => a super change
             if result.containsWildcards:
                 if self.options.mqttPatternBasedSubscriptions:
-                    if result.patternToExtractData:
+                    if result.patternToExtractData is not False:
                         self._addToMatchingStructure(
                             'dataQuery', pubTopic, result.patternToExtractData, emitter)
-                    elif result.pathToExtractData:
+                    elif result.pathToExtractData is not False:
                         self._addToMatchingStructure(
                             'dataPull', pubTopic, result.pathToExtractData, emitter)
                     else:
                         raise Exception(
                             'Implementation Error. Either the patternToExtractData or the pathToExtractData must be provided')
                 else:
                     self._addToMatchingStructure(
                         'dataQuery', pubTopic, pubTopic, emitter)
             else:
                 if result.affectedByChild and not self.options.forwardChildData or result.affectedByParent and not self.options.forwardParentData:
                     return
-                if result.pathToExtractData:
+                if result.pathToExtractData is not False:
                     self._addToMatchingStructure(
                         'dataPull', pubTopic, result.pathToExtractData, emitter)
                 else:
                     raise Exception(
                         "Implementation Error. The 'pathToExtractData' must be provided")
 
-    def _updatePartialMatching(
-            self, mode: str, _emitter, _pubTopic: str, _subTopic: str):
-        for item in self._emitters.values():
-            pubTopic = item.pubTopic
-            if mode == 'remove' and pubTopic and _subTopic:
-                self._deleteMatchingEntry(pubTopic, _subTopic, _emitter)
-            elif mode == 'add' and pubTopic and _subTopic:
-                self._addMatchingEntryIfRequired(
-                    pubTopic, _subTopic, _emitter)
-        if mode == 'add':
-            if _pubTopic:
-                self._updateMatchingForTopic(_pubTopic)
-            if _subTopic and not containsWildcards(_subTopic):
-                self._addMatchingEntryIfRequired(
-                    _subTopic, _subTopic, _emitter)
-        elif mode == 'remove':
-            if _subTopic:
-                self._deleteMatchingEntry(_subTopic, _subTopic, _emitter)
-
-        self.publishers.update()
-        self.subscriptions.update()
-
     def emit(self, eventName, data, options=None):
         return self._pushData(eventName, eventName, data,
                               ensureDottedAccess(options))
 
     async def dispose(self):
         self._disposing = True
 
@@ -333,17 +300,23 @@
 
         self._matched.get(topicOfChange)[entry].get(
             path_or_pattern).add(emitter)
 
     def _updateMatchingForTopic(self, topicOfChange):
         if topicOfChange not in self._matched:
             self._matched[topicOfChange] = ensureDottedAccess(
-                {'dataPull': {}, 'dataQuery': {}})
+                {
+                    'dataPull': {}, 
+                    'dataQuery': {}
+                }
+            )
+
+        # Find all matches
         for emitter, item in self._emitters.items():
-            if item.subTopic:
+            if item.subTopic is not False:
                 self._addMatchingEntryIfRequired(
                     topicOfChange, item.subTopic, emitter)
 
     def _notify(self, topicOfContent: str, topicOfChange: str,
                 options, emitterCausingUpdate=None):
         """ Internal Function to _notify all subscribers
 
@@ -362,47 +335,55 @@
             self._updateMatchingForTopic(topicOfContent)
 
         referenceToMatch = self._matched[topicOfContent]
 
         for path_to_pull, emitters in referenceToMatch.dataPull.items():
 
             for emitter in emitters:
-                data = self._pullData(path_to_pull, None)
-
                 # Only if we want to _notify an exclusive emitter we
                 # have to continue, if our emitter isnt matched.
                 if emitterCausingUpdate is not None and emitterCausingUpdate == emitter:
                     continue
 
+                data = self._pullData(path_to_pull, None)
+
                 emitter.emit(
                     data,
                     ensureDottedAccess({
                         **options,
                         'topicOfChange': topicOfChange,
                         'topicOfContent': topicOfContent,
                         'topicOfSubscription': self._emitters[emitter].subTopic
                     })
                 )
 
         for pattern, emitters in referenceToMatch.dataQuery.items():
-
-            for emitter in emitters:
-                data = self._pullData(pattern, None)
-                if emitter is not None and emitter != emitter:
-                    continue
-                emitter.emit(
-                    data,
-                    ensureDottedAccess({
-                        **options,
-                        'mode': 'direct',
-                        'topicOfChange': topicOfChange,
-                        'topicOfContent': topicOfContent,
-                        'topicOfSubscription': self._emitters.get(emitter).subTopic
-                    })
-                )
+            
+            # Get a copy of the filtered items.
+            data = self._pullData(pattern, None)
+
+            # Filter the items.
+            data = filter(lambda item: self._comparePatternAndPath(topicOfChange, item.path).affected, data)
+
+            if len(data) > 0:
+
+                for emitter in emitters:
+                    if emitter is not None and emitter != emitter:
+                        continue
+                    
+                    emitter.emit(
+                        data,
+                        ensureDottedAccess({
+                            **options,
+                            'mode': 'direct',
+                            'topicOfChange': topicOfChange,
+                            'topicOfContent': topicOfContent,
+                            'topicOfSubscription': self._emitters.get(emitter).subTopic
+                        })
+                    )
 
     def _updateOptions(self, options):
         if not options.timestamp:
             options.timestamp = getTimestamp()
         if not isinstance(options.forced, bool):
             options.forced = False
         if not isIterable(options.args):
```

### Comparing `nope_py-1.6.7/nope/types/__init__.py` & `nope_py-1.7.1/nope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/nope_py.egg-info/PKG-INFO` & `nope_py-1.7.1/nope_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope-py
-Version: 1.6.7
+Version: 1.7.1
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/anti-held-333/nope-py.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.6.7/nope_py.egg-info/SOURCES.txt` & `nope_py-1.7.1/nope_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/setup.py` & `nope_py-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     long_description = open("README").read()
 except BaseException:
     long_description = """NOPE-Python Backend. A Generic Backend for Python"""
 
 if __name__ == "__main__":
     setup(name="nope_py",
-          version=open("VERSION").read().strip(),
+          version="1.7.1",
           description="NOPE-Lib represents the No Programming Environment Library for python.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Martin Karkowski",
           author_email="m.karkowski@zema.de",
           maintainer="Martin Karkowski",
           maintainer_email="m.karkowski@zema.de",
```

### Comparing `nope_py-1.6.7/test/test.py` & `nope_py-1.7.1/test/test.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_communicator.py` & `nope_py-1.7.1/test/test_communicator.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_plugin.py` & `nope_py-1.7.1/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_plugin_bridge.py` & `nope_py-1.7.1/test/test_plugin_bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_plugin_rpc_callbacks.py` & `nope_py-1.7.1/test/test_plugin_rpc_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_pub_sub.py` & `nope_py-1.7.1/test/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.6.7/test/test_rpc_manager.py` & `nope_py-1.7.1/test/test_rpc_manager.py`

 * *Files identical despite different names*

