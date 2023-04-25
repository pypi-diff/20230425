# Comparing `tmp/DXR-1.7.6.tar.gz` & `tmp/DXR-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.7.6.tar", last modified: Tue Apr 25 05:22:19 2023, max compression
+gzip compressed data, was "DXR-1.7.7.tar", last modified: Tue Apr 25 10:47:03 2023, max compression
```

## Comparing `DXR-1.7.6.tar` & `DXR-1.7.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.386927 DXR-1.7.6/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.318770 DXR-1.7.6/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1381 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-04-25 05:22:19.000000 DXR-1.7.6/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.321027 DXR-1.7.6/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.6/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.6/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.6/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.323706 DXR-1.7.6/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.6/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.329331 DXR-1.7.6/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.6/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.6/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-04-24 05:32:08.000000 DXR-1.7.6/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2524 2023-04-24 05:49:44.000000 DXR-1.7.6/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.7.6/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.6/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.336552 DXR-1.7.6/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.6/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.6/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.6/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.6/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.6/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.6/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.6/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.6/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.342947 DXR-1.7.6/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.6/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-04-25 05:13:27.000000 DXR-1.7.6/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.6/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.6/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.6/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.345835 DXR-1.7.6/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.351297 DXR-1.7.6/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.6/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.6/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.358410 DXR-1.7.6/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.6/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.362736 DXR-1.7.6/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.377409 DXR-1.7.6/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.380068 DXR-1.7.6/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.6/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.6/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.381609 DXR-1.7.6/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.6/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.6/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 05:22:19.385513 DXR-1.7.6/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.6/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 05:22:19.383546 DXR-1.7.6/dxr_cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.7.6/dxr_cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1840 2023-04-25 05:20:15.000000 DXR-1.7.6/dxr_cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-25 05:22:19.388261 DXR-1.7.6/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-04-25 05:22:12.000000 DXR-1.7.6/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.497001 DXR-1.7.7/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.409408 DXR-1.7.7/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1381 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.411276 DXR-1.7.7/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.7/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.7/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.7/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.413560 DXR-1.7.7/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.7/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.422153 DXR-1.7.7/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-04-24 05:32:08.000000 DXR-1.7.7/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2524 2023-04-24 05:49:44.000000 DXR-1.7.7/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.7.7/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.442240 DXR-1.7.7/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.7/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.7/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.7/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.7/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.450584 DXR-1.7.7/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.7/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-04-25 05:13:27.000000 DXR-1.7.7/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.7/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.7/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.7/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.454039 DXR-1.7.7/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.461112 DXR-1.7.7/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.7/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.7/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.465935 DXR-1.7.7/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.7/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.471959 DXR-1.7.7/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.488099 DXR-1.7.7/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.490619 DXR-1.7.7/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.7/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.7/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.492544 DXR-1.7.7/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.7/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 10:47:03.496336 DXR-1.7.7/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.7/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.494964 DXR-1.7.7/dxr_cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.7.7/dxr_cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2794 2023-04-25 10:46:49.000000 DXR-1.7.7/dxr_cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-25 10:47:03.497494 DXR-1.7.7/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-04-25 10:46:56.000000 DXR-1.7.7/setup.py
```

### Comparing `DXR-1.7.6/DXR.egg-info/SOURCES.txt` & `DXR-1.7.7/DXR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_Chat/ChatGPT.py` & `DXR-1.7.7/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_Chat/utils.py` & `DXR-1.7.7/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_bytes/Dxr_bytes.py` & `DXR-1.7.7/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_file/dxr_file.py` & `DXR-1.7.7/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_file/dxr_request.py` & `DXR-1.7.7/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_file/dxr_request_ros.py` & `DXR-1.7.7/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_file/dxr_requests.py` & `DXR-1.7.7/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_file/dxr_ssh.py` & `DXR-1.7.7/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/Datas_pb2.py` & `DXR-1.7.7/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.7.7/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/audios_pb2.py` & `DXR-1.7.7/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.7.7/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.7.7/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.7.7/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_isapi/api.py` & `DXR-1.7.7/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_isapi/error.py` & `DXR-1.7.7/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_isapi/ir_client.py` & `DXR-1.7.7/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_log/log.py` & `DXR-1.7.7/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.7.7/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.7.7/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_mqtt/msg.py` & `DXR-1.7.7/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_serial/Dxr_serial.py` & `DXR-1.7.7/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_utils/dxr_ftp.py` & `DXR-1.7.7/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_utils/dxr_utils.py` & `DXR-1.7.7/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/Datas_pb2.py` & `DXR-1.7.7/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.7.7/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/HCNetSDK.py` & `DXR-1.7.7/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/PlayCtrl.py` & `DXR-1.7.7/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/test_main.py` & `DXR-1.7.7/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/video.py` & `DXR-1.7.7/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/video_hk.py` & `DXR-1.7.7/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_video/video_server.py` & `DXR-1.7.7/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_voice/dxr_tts.py` & `DXR-1.7.7/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/Dxr_yaml/Dxr_yaml.py` & `DXR-1.7.7/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/README.md` & `DXR-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.7.6/dxr_cli/cli.py` & `DXR-1.7.7/dxr_cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,47 +27,77 @@
 
 def get_bash_script(script, sub_script):
     url = f'http://39.101.69.111:4000/bash/{script}/{sub_script}'
     r = requests.get(url)
     script = r.text
     return script
 
-def choose_script(scripts):
+def choose_script(scripts, step=1):
     script_index = 0
     while True:
         click.clear()
         click.echo('Select a script:')
         for i, script in enumerate(scripts):
             if i == script_index:
                 click.echo(f'> {script}')
             else:
                 click.echo(f'  {script}')
         key = click.getchar()
+        # 上下键选择，左键返回，右键进入
         if key == '\r':
-            return scripts[script_index]
+            return scripts[script_index], step + 1
         elif key == '\x1b[A':
             script_index = (script_index - 1) % len(scripts)
         elif key == '\x1b[B':
             script_index = (script_index + 1) % len(scripts)
+        elif key == '\x1b[D':
+            return None, step - 1
+        elif key == '\x1b[C':
+            return scripts[script_index], step + 1
+            
 
 @dxr.command()
 def bash():
     """Bash scripts"""
     import os
-    scripts = get_bash_scripts()
-    script = choose_script(scripts)
-    sub_scripts = get_bash_script_dir(script)
-    sub_script = choose_script(sub_scripts)
-    bash_script = get_bash_script(script, sub_script)
-    print("=" * 80)
-    click.echo(bash_script)
-    print("=" * 80)
-    click.echo('Run this script?')
-    if click.confirm('Continue?'):
-        os.system(bash_script)
+    # scripts = get_bash_scripts()
+    # script = choose_script(scripts)
+    # sub_scripts = get_bash_script_dir(script)
+    # sub_script = choose_script(sub_scripts)
+    # bash_script = get_bash_script(script, sub_script)
+    # print("=" * 80)
+    # click.echo(bash_script)
+    # print("=" * 80)
+    # click.echo('Run this script?')
+    # if click.confirm('Continue?'):
+    #     os.system(bash_script)
+    step = 1
+    while True:
+        if step == 0:
+            break
+        if step == 1:
+            scripts = get_bash_scripts()
+            script, step = choose_script(scripts, step)
+        elif step == 2:
+            sub_scripts = get_bash_script_dir(script)
+            sub_script, step = choose_script(sub_scripts, step)
+        elif step == 3:
+            bash_script = get_bash_script(script, sub_script)
+            print("=" * 80)
+            click.echo(bash_script)
+            print("=" * 80)
+            click.echo('Run this script?')
+            if click.confirm('Continue?'):
+                os.system(bash_script)
+                break
+            step = 2
+        
+    
+    
+    
    
     
 
 
 def main():
     print("Hello world!")
```

### Comparing `DXR-1.7.6/setup.py` & `DXR-1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.7.6',
+    version='1.7.7',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'dxr_cli'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

