# Comparing `tmp/nope_py-1.7.1a1.tar.gz` & `tmp/nope_py-1.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nope_py-1.7.1a1.tar", last modified: Tue Apr 25 06:41:09 2023, max compression
+gzip compressed data, was "nope_py-1.7.1a2.tar", last modified: Tue Apr 25 06:48:37 2023, max compression
```

## Comparing `nope_py-1.7.1a1.tar` & `nope_py-1.7.1a2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.778884 nope_py-1.7.1a1/
--rw-rw-rw-   0        0        0     1083 2023-04-24 13:45:45.000000 nope_py-1.7.1a1/LICENSE
--rw-rw-rw-   0        0        0      649 2023-04-25 06:41:09.779891 nope_py-1.7.1a1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-24 13:51:19.000000 nope_py-1.7.1a1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.541712 nope_py-1.7.1a1/nope/
--rw-rw-rw-   0        0        0      525 2023-03-02 06:33:24.000000 nope_py-1.7.1a1/nope/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.552195 nope_py-1.7.1a1/nope/cli/
--rw-rw-rw-   0        0        0      439 2023-01-19 15:25:53.000000 nope_py-1.7.1a1/nope/cli/__init__.py
--rw-rw-rw-   0        0        0      128 2022-10-08 04:53:36.000000 nope_py-1.7.1a1/nope/cli/__main__.py
--rw-rw-rw-   0        0        0      707 2022-10-10 06:55:18.000000 nope_py-1.7.1a1/nope/cli/main.py
--rw-rw-rw-   0        0        0     7118 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/cli/run.py
--rw-rw-rw-   0        0        0     3651 2023-03-02 06:52:49.000000 nope_py-1.7.1a1/nope/cli/scan.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.560151 nope_py-1.7.1a1/nope/communication/
--rw-rw-rw-   0        0        0      130 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/communication/__init__.py
--rw-rw-rw-   0        0        0     1154 2022-11-02 06:36:13.000000 nope_py-1.7.1a1/nope/communication/abstractBridgePlugin.py
--rw-rw-rw-   0        0        0     5498 2022-11-11 21:37:48.000000 nope_py-1.7.1a1/nope/communication/bridge.py
--rw-rw-rw-   0        0        0      943 2023-02-09 15:29:20.000000 nope_py-1.7.1a1/nope/communication/getLayer.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.573104 nope_py-1.7.1a1/nope/communication/layers/
--rw-rw-rw-   0        0        0     2522 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/communication/layers/EventCommunicationInterface.py
--rw-rw-rw-   0        0        0     2896 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/communication/layers/IoSocketClientLayer.py
--rw-rw-rw-   0        0        0      200 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/communication/layers/__init__.py
--rw-rw-rw-   0        0        0      903 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/communication/layers/abstractLayer.py
--rw-rw-rw-   0        0        0     6117 2022-11-22 20:19:24.000000 nope_py-1.7.1a1/nope/communication/layers/mqttLayer.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.578101 nope_py-1.7.1a1/nope/decorators/
--rw-rw-rw-   0        0        0       83 2022-10-28 12:27:33.000000 nope_py-1.7.1a1/nope/decorators/__init__.py
--rw-rw-rw-   0        0        0     1327 2022-11-22 20:12:50.000000 nope_py-1.7.1a1/nope/decorators/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.580109 nope_py-1.7.1a1/nope/demo/
--rw-rw-rw-   0        0        0       95 2022-11-02 15:37:57.000000 nope_py-1.7.1a1/nope/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.586811 nope_py-1.7.1a1/nope/demo/instances/
--rw-rw-rw-   0        0        0     1524 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/instances/DecoratedHelloWorld.py
--rw-rw-rw-   0        0        0     1510 2023-03-02 07:08:18.000000 nope_py-1.7.1a1/nope/demo/instances/HelloWorld.py
--rw-rw-rw-   0        0        0     1243 2022-11-11 07:20:50.000000 nope_py-1.7.1a1/nope/demo/instances/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.599027 nope_py-1.7.1a1/nope/demo/plugins/
--rw-rw-rw-   0        0        0      977 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/plugins/00-load-hello.py
--rw-rw-rw-   0        0        0     2597 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/plugins/01-dynamic.py
--rw-rw-rw-   0        0        0     3031 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/plugins/02-multiple.py
--rw-rw-rw-   0        0        0     3284 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/plugins/03-different-items.py
--rw-rw-rw-   0        0        0     1264 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/demo/plugins/04-fix.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.607025 nope_py-1.7.1a1/nope/dispatcher/
--rw-rw-rw-   0        0        0      362 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/dispatcher/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.611023 nope_py-1.7.1a1/nope/dispatcher/baseServices/
--rw-rw-rw-   0        0        0      943 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/dispatcher/baseServices/__init__.py
--rw-rw-rw-   0        0        0     2772 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/dispatcher/baseServices/connectivy.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.615024 nope_py-1.7.1a1/nope/dispatcher/connectivityManager/
--rw-rw-rw-   0        0        0       57 2022-10-10 11:28:42.000000 nope_py-1.7.1a1/nope/dispatcher/connectivityManager/__init__.py
--rw-rw-rw-   0        0        0    12774 2023-03-02 07:08:18.000000 nope_py-1.7.1a1/nope/dispatcher/connectivityManager/connectivityManager.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.619027 nope_py-1.7.1a1/nope/dispatcher/core/
--rw-rw-rw-   0        0        0      115 2022-10-28 20:55:28.000000 nope_py-1.7.1a1/nope/dispatcher/core/__init__.py
--rw-rw-rw-   0        0        0     4711 2022-11-11 07:20:50.000000 nope_py-1.7.1a1/nope/dispatcher/core/nopeCore.py
--rw-rw-rw-   0        0        0     2175 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/dispatcher/getDispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.628026 nope_py-1.7.1a1/nope/dispatcher/instanceManager/
--rw-rw-rw-   0        0        0      108 2022-10-29 19:35:08.000000 nope_py-1.7.1a1/nope/dispatcher/instanceManager/__init__.py
--rw-rw-rw-   0        0        0      929 2022-10-10 06:40:15.000000 nope_py-1.7.1a1/nope/dispatcher/instanceManager/assignmentChecker.py
--rw-rw-rw-   0        0        0    39458 2023-04-24 14:24:50.000000 nope_py-1.7.1a1/nope/dispatcher/instanceManager/instanceManager.py
--rw-rw-rw-   0        0        0     4399 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/dispatcher/nopeDispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.637150 nope_py-1.7.1a1/nope/dispatcher/rpcManager/
--rw-rw-rw-   0        0        0       81 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/dispatcher/rpcManager/__init__.py
--rw-rw-rw-   0        0        0    24360 2023-04-24 14:26:18.000000 nope_py-1.7.1a1/nope/dispatcher/rpcManager/rpcManager.py
--rw-rw-rw-   0        0        0     3309 2023-01-19 08:26:09.000000 nope_py-1.7.1a1/nope/dispatcher/rpcManager/selectors.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.642035 nope_py-1.7.1a1/nope/eventEmitter/
--rw-rw-rw-   0        0        0       82 2022-10-10 11:28:51.000000 nope_py-1.7.1a1/nope/eventEmitter/__init__.py
--rw-rw-rw-   0        0        0     6698 2022-11-11 07:20:52.000000 nope_py-1.7.1a1/nope/eventEmitter/nopeEventEmitter.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.693747 nope_py-1.7.1a1/nope/helpers/
--rw-rw-rw-   0        0        0     2457 2023-01-25 06:14:09.000000 nope_py-1.7.1a1/nope/helpers/__init__.py
--rw-rw-rw-   0        0        0    13549 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/helpers/asyncHelpers.py
--rw-rw-rw-   0        0        0    12446 2022-11-11 07:20:53.000000 nope_py-1.7.1a1/nope/helpers/dictMethods.py
--rw-rw-rw-   0        0        0      720 2022-11-23 09:03:26.000000 nope_py-1.7.1a1/nope/helpers/dispatcherPathes.py
--rw-rw-rw-   0        0        0     4166 2023-03-02 07:08:47.000000 nope_py-1.7.1a1/nope/helpers/dottedDict.py
--rw-rw-rw-   0        0        0     3933 2022-10-10 11:28:37.000000 nope_py-1.7.1a1/nope/helpers/emitter.py
--rw-rw-rw-   0        0        0      836 2022-11-15 16:15:46.000000 nope_py-1.7.1a1/nope/helpers/files.py
--rw-rw-rw-   0        0        0    12428 2023-03-02 07:08:18.000000 nope_py-1.7.1a1/nope/helpers/hashable.py
--rw-rw-rw-   0        0        0      793 2022-11-11 20:53:45.000000 nope_py-1.7.1a1/nope/helpers/idMethods.py
--rw-rw-rw-   0        0        0      617 2022-10-10 06:40:15.000000 nope_py-1.7.1a1/nope/helpers/importing.py
--rw-rw-rw-   0        0        0     2821 2023-01-19 08:26:10.000000 nope_py-1.7.1a1/nope/helpers/jsonMethods.py
--rw-rw-rw-   0        0        0     2411 2023-01-19 08:26:10.000000 nope_py-1.7.1a1/nope/helpers/listMethods.py
--rw-rw-rw-   0        0        0    14752 2022-11-11 07:20:54.000000 nope_py-1.7.1a1/nope/helpers/objectMethods.py
--rw-rw-rw-   0        0        0     5206 2023-02-25 07:40:18.000000 nope_py-1.7.1a1/nope/helpers/path.py
--rw-rw-rw-   0        0        0    10739 2023-04-24 14:30:38.000000 nope_py-1.7.1a1/nope/helpers/pathMatchingMethods.py
--rw-rw-rw-   0        0        0      610 2022-10-10 06:40:15.000000 nope_py-1.7.1a1/nope/helpers/prints.py
--rw-rw-rw-   0        0        0     1459 2022-10-04 06:04:14.000000 nope_py-1.7.1a1/nope/helpers/runtime.py
--rw-rw-rw-   0        0        0      778 2022-10-10 11:28:32.000000 nope_py-1.7.1a1/nope/helpers/setMethods.py
--rw-rw-rw-   0        0        0     4995 2023-03-07 19:13:14.000000 nope_py-1.7.1a1/nope/helpers/stringMethods.py
--rw-rw-rw-   0        0        0     1894 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/helpers/timers.py
--rw-rw-rw-   0        0        0      119 2022-10-10 06:55:23.000000 nope_py-1.7.1a1/nope/helpers/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.704746 nope_py-1.7.1a1/nope/loader/
--rw-rw-rw-   0        0        0      241 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/loader/__init__.py
--rw-rw-rw-   0        0        0      777 2023-03-06 11:45:58.000000 nope_py-1.7.1a1/nope/loader/getPackageLoader.py
--rw-rw-rw-   0        0        0     2743 2023-03-02 08:45:55.000000 nope_py-1.7.1a1/nope/loader/loadPackages.py
--rw-rw-rw-   0        0        0     6529 2023-02-25 07:40:18.000000 nope_py-1.7.1a1/nope/loader/nopePackkageLoader.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.708751 nope_py-1.7.1a1/nope/logger/
--rw-rw-rw-   0        0        0      100 2022-10-10 06:40:15.000000 nope_py-1.7.1a1/nope/logger/__init__.py
--rw-rw-rw-   0        0        0     2505 2023-03-02 07:08:18.000000 nope_py-1.7.1a1/nope/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.712745 nope_py-1.7.1a1/nope/merging/
--rw-rw-rw-   0        0        0       53 2022-10-10 11:29:50.000000 nope_py-1.7.1a1/nope/merging/__init__.py
--rw-rw-rw-   0        0        0     2359 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/merging/mergeData.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.718877 nope_py-1.7.1a1/nope/modules/
--rw-rw-rw-   0        0        0      214 2022-10-10 11:30:28.000000 nope_py-1.7.1a1/nope/modules/__init__.py
--rw-rw-rw-   0        0        0    18241 2023-03-02 07:08:18.000000 nope_py-1.7.1a1/nope/modules/baseModule.py
--rw-rw-rw-   0        0        0     7829 2023-02-25 07:40:18.000000 nope_py-1.7.1a1/nope/modules/genericModule.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.723893 nope_py-1.7.1a1/nope/observable/
--rw-rw-rw-   0        0        0      157 2022-10-10 11:30:26.000000 nope_py-1.7.1a1/nope/observable/__init__.py
--rw-rw-rw-   0        0        0     3097 2023-01-26 07:25:35.000000 nope_py-1.7.1a1/nope/observable/nopeObservable.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.736897 nope_py-1.7.1a1/nope/plugins/
--rw-rw-rw-   0        0        0      129 2022-11-11 20:52:06.000000 nope_py-1.7.1a1/nope/plugins/__init__.py
--rw-rw-rw-   0        0        0     6213 2022-11-11 07:20:56.000000 nope_py-1.7.1a1/nope/plugins/ack_messages.py
--rw-rw-rw-   0        0        0      946 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/plugins/hello.py
--rw-rw-rw-   0        0        0    22410 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/plugins/plugin.py
--rw-rw-rw-   0        0        0    16526 2022-11-15 16:15:53.000000 nope_py-1.7.1a1/nope/plugins/rpc_with_callbacks.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.742885 nope_py-1.7.1a1/nope/pubSub/
--rw-rw-rw-   0        0        0       96 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/nope/pubSub/__init__.py
--rw-rw-rw-   0        0        0     3810 2022-10-10 11:30:55.000000 nope_py-1.7.1a1/nope/pubSub/nopeDataPubSubSystem.py
--rw-rw-rw-   0        0        0    18864 2023-04-24 14:53:00.000000 nope_py-1.7.1a1/nope/pubSub/nopePubSubSystem.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.745888 nope_py-1.7.1a1/nope/types/
--rw-rw-rw-   0        0        0     3468 2022-11-22 16:51:58.000000 nope_py-1.7.1a1/nope/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.763892 nope_py-1.7.1a1/nope_py.egg-info/
--rw-rw-rw-   0        0        0      649 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3070 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 06:41:09.000000 nope_py-1.7.1a1/nope_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-04-25 06:41:09.780885 nope_py-1.7.1a1/setup.cfg
--rw-rw-rw-   0        0        0     2596 2023-04-25 06:40:31.000000 nope_py-1.7.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:09.777093 nope_py-1.7.1a1/test/
--rw-rw-rw-   0        0        0     1427 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/test/test.py
--rw-rw-rw-   0        0        0     2144 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/test/test_communicator.py
--rw-rw-rw-   0        0        0     3047 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/test/test_plugin.py
--rw-rw-rw-   0        0        0     1606 2022-11-11 07:20:58.000000 nope_py-1.7.1a1/test/test_plugin_bridge.py
--rw-rw-rw-   0        0        0     1454 2022-11-15 16:15:55.000000 nope_py-1.7.1a1/test/test_plugin_rpc_callbacks.py
--rw-rw-rw-   0        0        0      682 2023-01-19 08:26:15.000000 nope_py-1.7.1a1/test/test_pub_sub.py
--rw-rw-rw-   0        0        0     3254 2022-11-07 07:10:33.000000 nope_py-1.7.1a1/test/test_rpc_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.191940 nope_py-1.7.1a2/
+-rw-rw-rw-   0        0        0     1083 2023-04-24 13:45:45.000000 nope_py-1.7.1a2/LICENSE
+-rw-rw-rw-   0        0        0      649 2023-04-25 06:48:37.193079 nope_py-1.7.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-24 13:51:19.000000 nope_py-1.7.1a2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.964985 nope_py-1.7.1a2/nope/
+-rw-rw-rw-   0        0        0      525 2023-03-02 06:33:24.000000 nope_py-1.7.1a2/nope/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.977691 nope_py-1.7.1a2/nope/cli/
+-rw-rw-rw-   0        0        0      439 2023-01-19 15:25:53.000000 nope_py-1.7.1a2/nope/cli/__init__.py
+-rw-rw-rw-   0        0        0      128 2022-10-08 04:53:36.000000 nope_py-1.7.1a2/nope/cli/__main__.py
+-rw-rw-rw-   0        0        0      707 2022-10-10 06:55:18.000000 nope_py-1.7.1a2/nope/cli/main.py
+-rw-rw-rw-   0        0        0     7118 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/cli/run.py
+-rw-rw-rw-   0        0        0     3651 2023-03-02 06:52:49.000000 nope_py-1.7.1a2/nope/cli/scan.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.987690 nope_py-1.7.1a2/nope/communication/
+-rw-rw-rw-   0        0        0      130 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/communication/__init__.py
+-rw-rw-rw-   0        0        0     1154 2022-11-02 06:36:13.000000 nope_py-1.7.1a2/nope/communication/abstractBridgePlugin.py
+-rw-rw-rw-   0        0        0     5498 2022-11-11 21:37:48.000000 nope_py-1.7.1a2/nope/communication/bridge.py
+-rw-rw-rw-   0        0        0      943 2023-02-09 15:29:20.000000 nope_py-1.7.1a2/nope/communication/getLayer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.998690 nope_py-1.7.1a2/nope/communication/layers/
+-rw-rw-rw-   0        0        0     2522 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/communication/layers/EventCommunicationInterface.py
+-rw-rw-rw-   0        0        0     2896 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/communication/layers/IoSocketClientLayer.py
+-rw-rw-rw-   0        0        0      200 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/communication/layers/__init__.py
+-rw-rw-rw-   0        0        0      903 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/communication/layers/abstractLayer.py
+-rw-rw-rw-   0        0        0     6117 2022-11-22 20:19:24.000000 nope_py-1.7.1a2/nope/communication/layers/mqttLayer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.002802 nope_py-1.7.1a2/nope/decorators/
+-rw-rw-rw-   0        0        0       83 2022-10-28 12:27:33.000000 nope_py-1.7.1a2/nope/decorators/__init__.py
+-rw-rw-rw-   0        0        0     1327 2022-11-22 20:12:50.000000 nope_py-1.7.1a2/nope/decorators/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.005794 nope_py-1.7.1a2/nope/demo/
+-rw-rw-rw-   0        0        0       95 2022-11-02 15:37:57.000000 nope_py-1.7.1a2/nope/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.010818 nope_py-1.7.1a2/nope/demo/instances/
+-rw-rw-rw-   0        0        0     1524 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/instances/DecoratedHelloWorld.py
+-rw-rw-rw-   0        0        0     1510 2023-03-02 07:08:18.000000 nope_py-1.7.1a2/nope/demo/instances/HelloWorld.py
+-rw-rw-rw-   0        0        0     1243 2022-11-11 07:20:50.000000 nope_py-1.7.1a2/nope/demo/instances/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.023791 nope_py-1.7.1a2/nope/demo/plugins/
+-rw-rw-rw-   0        0        0      977 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/plugins/00-load-hello.py
+-rw-rw-rw-   0        0        0     2597 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/plugins/01-dynamic.py
+-rw-rw-rw-   0        0        0     3031 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/plugins/02-multiple.py
+-rw-rw-rw-   0        0        0     3284 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/plugins/03-different-items.py
+-rw-rw-rw-   0        0        0     1264 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/demo/plugins/04-fix.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.029792 nope_py-1.7.1a2/nope/dispatcher/
+-rw-rw-rw-   0        0        0      362 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/dispatcher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.035795 nope_py-1.7.1a2/nope/dispatcher/baseServices/
+-rw-rw-rw-   0        0        0      943 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/dispatcher/baseServices/__init__.py
+-rw-rw-rw-   0        0        0     2772 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/dispatcher/baseServices/connectivy.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.041794 nope_py-1.7.1a2/nope/dispatcher/connectivityManager/
+-rw-rw-rw-   0        0        0       57 2022-10-10 11:28:42.000000 nope_py-1.7.1a2/nope/dispatcher/connectivityManager/__init__.py
+-rw-rw-rw-   0        0        0    12774 2023-03-02 07:08:18.000000 nope_py-1.7.1a2/nope/dispatcher/connectivityManager/connectivityManager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.047792 nope_py-1.7.1a2/nope/dispatcher/core/
+-rw-rw-rw-   0        0        0      115 2022-10-28 20:55:28.000000 nope_py-1.7.1a2/nope/dispatcher/core/__init__.py
+-rw-rw-rw-   0        0        0     4711 2022-11-11 07:20:50.000000 nope_py-1.7.1a2/nope/dispatcher/core/nopeCore.py
+-rw-rw-rw-   0        0        0     2175 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/dispatcher/getDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.053801 nope_py-1.7.1a2/nope/dispatcher/instanceManager/
+-rw-rw-rw-   0        0        0      108 2022-10-29 19:35:08.000000 nope_py-1.7.1a2/nope/dispatcher/instanceManager/__init__.py
+-rw-rw-rw-   0        0        0      929 2022-10-10 06:40:15.000000 nope_py-1.7.1a2/nope/dispatcher/instanceManager/assignmentChecker.py
+-rw-rw-rw-   0        0        0    39458 2023-04-24 14:24:50.000000 nope_py-1.7.1a2/nope/dispatcher/instanceManager/instanceManager.py
+-rw-rw-rw-   0        0        0     4399 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/dispatcher/nopeDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.061349 nope_py-1.7.1a2/nope/dispatcher/rpcManager/
+-rw-rw-rw-   0        0        0       81 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/dispatcher/rpcManager/__init__.py
+-rw-rw-rw-   0        0        0    24360 2023-04-24 14:26:18.000000 nope_py-1.7.1a2/nope/dispatcher/rpcManager/rpcManager.py
+-rw-rw-rw-   0        0        0     3309 2023-01-19 08:26:09.000000 nope_py-1.7.1a2/nope/dispatcher/rpcManager/selectors.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.066179 nope_py-1.7.1a2/nope/eventEmitter/
+-rw-rw-rw-   0        0        0       82 2022-10-10 11:28:51.000000 nope_py-1.7.1a2/nope/eventEmitter/__init__.py
+-rw-rw-rw-   0        0        0     6698 2022-11-11 07:20:52.000000 nope_py-1.7.1a2/nope/eventEmitter/nopeEventEmitter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.110939 nope_py-1.7.1a2/nope/helpers/
+-rw-rw-rw-   0        0        0     2457 2023-01-25 06:14:09.000000 nope_py-1.7.1a2/nope/helpers/__init__.py
+-rw-rw-rw-   0        0        0    13549 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/helpers/asyncHelpers.py
+-rw-rw-rw-   0        0        0    12446 2022-11-11 07:20:53.000000 nope_py-1.7.1a2/nope/helpers/dictMethods.py
+-rw-rw-rw-   0        0        0      720 2022-11-23 09:03:26.000000 nope_py-1.7.1a2/nope/helpers/dispatcherPathes.py
+-rw-rw-rw-   0        0        0     4166 2023-03-02 07:08:47.000000 nope_py-1.7.1a2/nope/helpers/dottedDict.py
+-rw-rw-rw-   0        0        0     3933 2022-10-10 11:28:37.000000 nope_py-1.7.1a2/nope/helpers/emitter.py
+-rw-rw-rw-   0        0        0      836 2022-11-15 16:15:46.000000 nope_py-1.7.1a2/nope/helpers/files.py
+-rw-rw-rw-   0        0        0    12428 2023-03-02 07:08:18.000000 nope_py-1.7.1a2/nope/helpers/hashable.py
+-rw-rw-rw-   0        0        0      793 2022-11-11 20:53:45.000000 nope_py-1.7.1a2/nope/helpers/idMethods.py
+-rw-rw-rw-   0        0        0      617 2022-10-10 06:40:15.000000 nope_py-1.7.1a2/nope/helpers/importing.py
+-rw-rw-rw-   0        0        0     2821 2023-01-19 08:26:10.000000 nope_py-1.7.1a2/nope/helpers/jsonMethods.py
+-rw-rw-rw-   0        0        0     2411 2023-01-19 08:26:10.000000 nope_py-1.7.1a2/nope/helpers/listMethods.py
+-rw-rw-rw-   0        0        0    14752 2022-11-11 07:20:54.000000 nope_py-1.7.1a2/nope/helpers/objectMethods.py
+-rw-rw-rw-   0        0        0     5206 2023-02-25 07:40:18.000000 nope_py-1.7.1a2/nope/helpers/path.py
+-rw-rw-rw-   0        0        0    10739 2023-04-24 14:30:38.000000 nope_py-1.7.1a2/nope/helpers/pathMatchingMethods.py
+-rw-rw-rw-   0        0        0      610 2022-10-10 06:40:15.000000 nope_py-1.7.1a2/nope/helpers/prints.py
+-rw-rw-rw-   0        0        0     1459 2022-10-04 06:04:14.000000 nope_py-1.7.1a2/nope/helpers/runtime.py
+-rw-rw-rw-   0        0        0      778 2022-10-10 11:28:32.000000 nope_py-1.7.1a2/nope/helpers/setMethods.py
+-rw-rw-rw-   0        0        0     4995 2023-03-07 19:13:14.000000 nope_py-1.7.1a2/nope/helpers/stringMethods.py
+-rw-rw-rw-   0        0        0     1894 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/helpers/timers.py
+-rw-rw-rw-   0        0        0      119 2022-10-10 06:55:23.000000 nope_py-1.7.1a2/nope/helpers/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.117940 nope_py-1.7.1a2/nope/loader/
+-rw-rw-rw-   0        0        0      241 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/loader/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-03-06 11:45:58.000000 nope_py-1.7.1a2/nope/loader/getPackageLoader.py
+-rw-rw-rw-   0        0        0     2743 2023-03-02 08:45:55.000000 nope_py-1.7.1a2/nope/loader/loadPackages.py
+-rw-rw-rw-   0        0        0     6529 2023-02-25 07:40:18.000000 nope_py-1.7.1a2/nope/loader/nopePackkageLoader.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.121939 nope_py-1.7.1a2/nope/logger/
+-rw-rw-rw-   0        0        0      100 2022-10-10 06:40:15.000000 nope_py-1.7.1a2/nope/logger/__init__.py
+-rw-rw-rw-   0        0        0     2505 2023-03-02 07:08:18.000000 nope_py-1.7.1a2/nope/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.126522 nope_py-1.7.1a2/nope/merging/
+-rw-rw-rw-   0        0        0       53 2022-10-10 11:29:50.000000 nope_py-1.7.1a2/nope/merging/__init__.py
+-rw-rw-rw-   0        0        0     2359 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/merging/mergeData.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.133941 nope_py-1.7.1a2/nope/modules/
+-rw-rw-rw-   0        0        0      214 2022-10-10 11:30:28.000000 nope_py-1.7.1a2/nope/modules/__init__.py
+-rw-rw-rw-   0        0        0    18241 2023-03-02 07:08:18.000000 nope_py-1.7.1a2/nope/modules/baseModule.py
+-rw-rw-rw-   0        0        0     7829 2023-02-25 07:40:18.000000 nope_py-1.7.1a2/nope/modules/genericModule.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.138939 nope_py-1.7.1a2/nope/observable/
+-rw-rw-rw-   0        0        0      157 2022-10-10 11:30:26.000000 nope_py-1.7.1a2/nope/observable/__init__.py
+-rw-rw-rw-   0        0        0     3097 2023-01-26 07:25:35.000000 nope_py-1.7.1a2/nope/observable/nopeObservable.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.148939 nope_py-1.7.1a2/nope/plugins/
+-rw-rw-rw-   0        0        0      129 2022-11-11 20:52:06.000000 nope_py-1.7.1a2/nope/plugins/__init__.py
+-rw-rw-rw-   0        0        0     6213 2022-11-11 07:20:56.000000 nope_py-1.7.1a2/nope/plugins/ack_messages.py
+-rw-rw-rw-   0        0        0      946 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/plugins/hello.py
+-rw-rw-rw-   0        0        0    22410 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/plugins/plugin.py
+-rw-rw-rw-   0        0        0    16526 2022-11-15 16:15:53.000000 nope_py-1.7.1a2/nope/plugins/rpc_with_callbacks.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.154939 nope_py-1.7.1a2/nope/pubSub/
+-rw-rw-rw-   0        0        0       96 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/nope/pubSub/__init__.py
+-rw-rw-rw-   0        0        0     3810 2022-10-10 11:30:55.000000 nope_py-1.7.1a2/nope/pubSub/nopeDataPubSubSystem.py
+-rw-rw-rw-   0        0        0    18864 2023-04-24 14:53:00.000000 nope_py-1.7.1a2/nope/pubSub/nopePubSubSystem.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.156939 nope_py-1.7.1a2/nope/types/
+-rw-rw-rw-   0        0        0     3468 2022-11-22 16:51:58.000000 nope_py-1.7.1a2/nope/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.176939 nope_py-1.7.1a2/nope_py.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3070 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 06:48:36.000000 nope_py-1.7.1a2/nope_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-04-25 06:48:37.194474 nope_py-1.7.1a2/setup.cfg
+-rw-rw-rw-   0        0        0     2596 2023-04-25 06:44:10.000000 nope_py-1.7.1a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:37.190940 nope_py-1.7.1a2/test/
+-rw-rw-rw-   0        0        0     1427 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/test/test.py
+-rw-rw-rw-   0        0        0     2144 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/test/test_communicator.py
+-rw-rw-rw-   0        0        0     3047 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/test/test_plugin.py
+-rw-rw-rw-   0        0        0     1606 2022-11-11 07:20:58.000000 nope_py-1.7.1a2/test/test_plugin_bridge.py
+-rw-rw-rw-   0        0        0     1454 2022-11-15 16:15:55.000000 nope_py-1.7.1a2/test/test_plugin_rpc_callbacks.py
+-rw-rw-rw-   0        0        0      682 2023-01-19 08:26:15.000000 nope_py-1.7.1a2/test/test_pub_sub.py
+-rw-rw-rw-   0        0        0     3254 2022-11-07 07:10:33.000000 nope_py-1.7.1a2/test/test_rpc_manager.py
```

### Comparing `nope_py-1.7.1a1/LICENSE` & `nope_py-1.7.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/PKG-INFO` & `nope_py-1.7.1a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope_py
-Version: 1.7.1a1
+Version: 1.7.1a2
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.7.1a1/nope/__init__.py` & `nope_py-1.7.1a2/nope/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/cli/main.py` & `nope_py-1.7.1a2/nope/cli/main.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/cli/run.py` & `nope_py-1.7.1a2/nope/cli/run.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/cli/scan.py` & `nope_py-1.7.1a2/nope/cli/scan.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/abstractBridgePlugin.py` & `nope_py-1.7.1a2/nope/communication/abstractBridgePlugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/bridge.py` & `nope_py-1.7.1a2/nope/communication/bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/getLayer.py` & `nope_py-1.7.1a2/nope/communication/getLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/layers/EventCommunicationInterface.py` & `nope_py-1.7.1a2/nope/communication/layers/EventCommunicationInterface.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/layers/IoSocketClientLayer.py` & `nope_py-1.7.1a2/nope/communication/layers/IoSocketClientLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/layers/abstractLayer.py` & `nope_py-1.7.1a2/nope/communication/layers/abstractLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/communication/layers/mqttLayer.py` & `nope_py-1.7.1a2/nope/communication/layers/mqttLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/decorators/classes.py` & `nope_py-1.7.1a2/nope/decorators/classes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/instances/DecoratedHelloWorld.py` & `nope_py-1.7.1a2/nope/demo/instances/DecoratedHelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/instances/HelloWorld.py` & `nope_py-1.7.1a2/nope/demo/instances/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/instances/__init__.py` & `nope_py-1.7.1a2/nope/demo/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/plugins/00-load-hello.py` & `nope_py-1.7.1a2/nope/demo/plugins/00-load-hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/plugins/01-dynamic.py` & `nope_py-1.7.1a2/nope/demo/plugins/01-dynamic.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/plugins/02-multiple.py` & `nope_py-1.7.1a2/nope/demo/plugins/02-multiple.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/plugins/03-different-items.py` & `nope_py-1.7.1a2/nope/demo/plugins/03-different-items.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/demo/plugins/04-fix.py` & `nope_py-1.7.1a2/nope/demo/plugins/04-fix.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/baseServices/__init__.py` & `nope_py-1.7.1a2/nope/dispatcher/baseServices/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/baseServices/connectivy.py` & `nope_py-1.7.1a2/nope/dispatcher/baseServices/connectivy.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/connectivityManager/connectivityManager.py` & `nope_py-1.7.1a2/nope/dispatcher/connectivityManager/connectivityManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/core/nopeCore.py` & `nope_py-1.7.1a2/nope/dispatcher/core/nopeCore.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/getDispatcher.py` & `nope_py-1.7.1a2/nope/dispatcher/getDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/instanceManager/assignmentChecker.py` & `nope_py-1.7.1a2/nope/dispatcher/instanceManager/assignmentChecker.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/instanceManager/instanceManager.py` & `nope_py-1.7.1a2/nope/dispatcher/instanceManager/instanceManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/nopeDispatcher.py` & `nope_py-1.7.1a2/nope/dispatcher/nopeDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/rpcManager/rpcManager.py` & `nope_py-1.7.1a2/nope/dispatcher/rpcManager/rpcManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/dispatcher/rpcManager/selectors.py` & `nope_py-1.7.1a2/nope/dispatcher/rpcManager/selectors.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/eventEmitter/nopeEventEmitter.py` & `nope_py-1.7.1a2/nope/eventEmitter/nopeEventEmitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/__init__.py` & `nope_py-1.7.1a2/nope/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/asyncHelpers.py` & `nope_py-1.7.1a2/nope/helpers/asyncHelpers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/dictMethods.py` & `nope_py-1.7.1a2/nope/helpers/dictMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/dispatcherPathes.py` & `nope_py-1.7.1a2/nope/helpers/dispatcherPathes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/dottedDict.py` & `nope_py-1.7.1a2/nope/helpers/dottedDict.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/emitter.py` & `nope_py-1.7.1a2/nope/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/files.py` & `nope_py-1.7.1a2/nope/helpers/files.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/hashable.py` & `nope_py-1.7.1a2/nope/helpers/hashable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/idMethods.py` & `nope_py-1.7.1a2/nope/helpers/idMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/importing.py` & `nope_py-1.7.1a2/nope/helpers/importing.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/jsonMethods.py` & `nope_py-1.7.1a2/nope/helpers/jsonMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/listMethods.py` & `nope_py-1.7.1a2/nope/helpers/listMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/objectMethods.py` & `nope_py-1.7.1a2/nope/helpers/objectMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/path.py` & `nope_py-1.7.1a2/nope/helpers/path.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/pathMatchingMethods.py` & `nope_py-1.7.1a2/nope/helpers/pathMatchingMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/prints.py` & `nope_py-1.7.1a2/nope/helpers/prints.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/runtime.py` & `nope_py-1.7.1a2/nope/helpers/runtime.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/setMethods.py` & `nope_py-1.7.1a2/nope/helpers/setMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/stringMethods.py` & `nope_py-1.7.1a2/nope/helpers/stringMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/helpers/timers.py` & `nope_py-1.7.1a2/nope/helpers/timers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/loader/getPackageLoader.py` & `nope_py-1.7.1a2/nope/loader/getPackageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/loader/loadPackages.py` & `nope_py-1.7.1a2/nope/loader/loadPackages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/loader/nopePackkageLoader.py` & `nope_py-1.7.1a2/nope/loader/nopePackkageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/logger/logger.py` & `nope_py-1.7.1a2/nope/logger/logger.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/merging/mergeData.py` & `nope_py-1.7.1a2/nope/merging/mergeData.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/modules/baseModule.py` & `nope_py-1.7.1a2/nope/modules/baseModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/modules/genericModule.py` & `nope_py-1.7.1a2/nope/modules/genericModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/observable/nopeObservable.py` & `nope_py-1.7.1a2/nope/observable/nopeObservable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/plugins/ack_messages.py` & `nope_py-1.7.1a2/nope/plugins/ack_messages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/plugins/hello.py` & `nope_py-1.7.1a2/nope/plugins/hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/plugins/plugin.py` & `nope_py-1.7.1a2/nope/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/plugins/rpc_with_callbacks.py` & `nope_py-1.7.1a2/nope/plugins/rpc_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/pubSub/nopeDataPubSubSystem.py` & `nope_py-1.7.1a2/nope/pubSub/nopeDataPubSubSystem.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/pubSub/nopePubSubSystem.py` & `nope_py-1.7.1a2/nope/pubSub/nopePubSubSystem.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope/types/__init__.py` & `nope_py-1.7.1a2/nope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/nope_py.egg-info/PKG-INFO` & `nope_py-1.7.1a2/nope_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope-py
-Version: 1.7.1a1
+Version: 1.7.1a2
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.7.1a1/nope_py.egg-info/SOURCES.txt` & `nope_py-1.7.1a2/nope_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/setup.py` & `nope_py-1.7.1a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 try:
     long_description = open("README").read()
 except BaseException:
     long_description = """NOPE-Python Backend. A Generic Backend for Python"""
 
 if __name__ == "__main__":
     setup(name="nope_py",
-          version="1.7.1a1",
+          version="1.7.1a2",
           description="NOPE-Lib represents the No Programming Environment Library for python.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Martin Karkowski",
           author_email="m.karkowski@zema.de",
           maintainer="Martin Karkowski",
           maintainer_email="m.karkowski@zema.de",
           install_requires=['paho-mqtt',
+                            'multidict',
                             'python-socketio[asyncio_client]',
                             'aiohttp',
-                            'multidict',
                             'psutil'],
           url="https://github.com/ZeMA-gGmbH/NoPE-PY.git",
           packages=["nope",
                     "nope.cli",
                     "nope.communication",
                     "nope.communication.layers",
                     "nope.decorators",
```

### Comparing `nope_py-1.7.1a1/test/test.py` & `nope_py-1.7.1a2/test/test.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_communicator.py` & `nope_py-1.7.1a2/test/test_communicator.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_plugin.py` & `nope_py-1.7.1a2/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_plugin_bridge.py` & `nope_py-1.7.1a2/test/test_plugin_bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_plugin_rpc_callbacks.py` & `nope_py-1.7.1a2/test/test_plugin_rpc_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_pub_sub.py` & `nope_py-1.7.1a2/test/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.1a1/test/test_rpc_manager.py` & `nope_py-1.7.1a2/test/test_rpc_manager.py`

 * *Files identical despite different names*

