# Comparing `tmp/FastCNN2-1.23.424.1637.tar.gz` & `tmp/FastCNN2-1.23.425.1716.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FastCNN2-1.23.424.1637.tar", last modified: Mon Apr 24 08:37:24 2023, max compression
+gzip compressed data, was "dist\FastCNN2-1.23.425.1716.tar", last modified: Tue Apr 25 09:16:50 2023, max compression
```

## Comparing `FastCNN2-1.23.424.1637.tar` & `FastCNN2-1.23.425.1716.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/api/
--rw-rw-rw-   0        0        0     5922 2022-07-25 09:49:16.000000 FastCNN2-1.23.424.1637/FastCNN/api/camera_.py
--rw-rw-rw-   0        0        0     2527 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/api/fastcnn_.py
--rw-rw-rw-   0        0        0     7638 2023-04-24 08:35:52.000000 FastCNN2-1.23.424.1637/FastCNN/api/pytorchfastcnn_.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/datasets/
--rw-rw-rw-   0        0        0     4588 2022-06-01 11:01:02.000000 FastCNN2-1.23.424.1637/FastCNN/datasets/fastcsv.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/entry/
--rw-rw-rw-   0        0        0      943 2022-07-13 02:13:51.000000 FastCNN2-1.23.424.1637/FastCNN/entry/camera.py
--rw-rw-rw-   0        0        0     3133 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/gongda.py
--rw-rw-rw-   0        0        0      143 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/intergrate.py
--rw-rw-rw-   0        0        0      987 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/server.py
--rw-rw-rw-   0        0        0      951 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/server2.py
--rw-rw-rw-   0        0        0     1354 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/train.py
--rw-rw-rw-   0        0        0     1355 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/train2.py
--rw-rw-rw-   0        0        0     1318 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/entry/trainvisiable.py
--rw-rw-rw-   0        0        0     1338 2022-06-01 12:50:39.000000 FastCNN2-1.23.424.1637/FastCNN/entry/trainyolov5.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/models/
--rw-rw-rw-   0        0        0    36119 2022-06-01 19:52:23.000000 FastCNN2-1.23.424.1637/FastCNN/models/common.py
--rw-rw-rw-   0        0        0     4238 2022-06-01 14:26:38.000000 FastCNN2-1.23.424.1637/FastCNN/models/experimental.py
--rw-rw-rw-   0        0        0    15741 2022-06-01 14:27:01.000000 FastCNN2-1.23.424.1637/FastCNN/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/nn/
--rw-rw-rw-   0        0        0     1925 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/alexnet.py
--rw-rw-rw-   0        0        0     3697 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/efficientnets.py
--rw-rw-rw-   0        0        0     4222 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/nn/experimental.py
--rw-rw-rw-   0        0        0     1128 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/lenet.py
--rw-rw-rw-   0        0        0      777 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/neuralnets.py
--rw-rw-rw-   0        0        0     1122 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/standard.py
--rw-rw-rw-   0        0        0     3713 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/torchnn.py
--rw-rw-rw-   0        0        0     4843 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/nn/vgg.py
--rw-rw-rw-   0        0        0    15693 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/nn/yolo.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/prx/
--rw-rw-rw-   0        0        0     2952 2022-07-27 06:32:53.000000 FastCNN2-1.23.424.1637/FastCNN/prx/CameraProxy.py
--rw-rw-rw-   0        0        0     1190 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/prx/DatasetProxy.py
--rw-rw-rw-   0        0        0    14401 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/prx/GongDaProxy.py
--rw-rw-rw-   0        0        0    14149 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/prx/GongDaProxy1.py
--rw-rw-rw-   0        0        0     6584 2022-07-14 02:49:05.000000 FastCNN2-1.23.424.1637/FastCNN/prx/PathProxy.py
--rw-rw-rw-   0        0        0     6100 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/prx/TrainProxy.py
--rw-rw-rw-   0        0        0     6484 2022-06-01 10:08:55.000000 FastCNN2-1.23.424.1637/FastCNN/prx/TrainProxy2.py
--rw-rw-rw-   0        0        0     7938 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/prx/ValidProxy.py
--rw-rw-rw-   0        0        0     5316 2023-04-24 07:47:37.000000 FastCNN2-1.23.424.1637/FastCNN/prx/ValidProxy2.py
--rw-rw-rw-   0        0        0    21109 2023-04-24 08:31:59.000000 FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5DetectProxy.py
--rw-rw-rw-   0        0        0     2406 2022-06-01 12:39:44.000000 FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5Proxy.py
--rw-rw-rw-   0        0        0    43732 2022-06-02 00:45:04.000000 FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5TrainProxy.py
--rw-rw-rw-   0        0        0    20311 2022-06-01 17:08:57.000000 FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5ValidProxy.py
--rw-rw-rw-   0        0        0    30570 2022-06-01 19:53:11.000000 FastCNN2-1.23.424.1637/FastCNN/prx/export.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/utils/
--rw-rw-rw-   0        0        0     8413 2022-06-01 18:18:09.000000 FastCNN2-1.23.424.1637/FastCNN/utils/CallBacks.py
--rw-rw-rw-   0        0        0     1542 2022-06-01 09:36:12.000000 FastCNN2-1.23.424.1637/FastCNN/utils/Logs.py
--rw-rw-rw-   0        0        0    12210 2022-06-01 12:08:37.000000 FastCNN2-1.23.424.1637/FastCNN/utils/augmentations.py
--rw-rw-rw-   0        0        0     7613 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/autoanchor.py
--rw-rw-rw-   0        0        0     2256 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/autobatch.py
--rw-rw-rw-   0        0        0    67782 2022-06-01 17:32:09.000000 FastCNN2-1.23.424.1637/FastCNN/utils/dataloaders.py
--rw-rw-rw-   0        0        0     7289 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/downloads.py
--rw-rw-rw-   0        0        0    42735 2022-06-01 12:07:38.000000 FastCNN2-1.23.424.1637/FastCNN/utils/general.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/
--rw-rw-rw-   0        0        0     8282 2023-04-24 08:37:18.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/
--rw-rw-rw-   0        0        0       30 2023-04-24 08:37:18.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/__init__.py
--rw-rw-rw-   0        0        0     1059 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/log_dataset.py
--rw-rw-rw-   0        0        0     1254 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/sweep.py
--rw-rw-rw-   0        0        0    28163 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/wandb_utils.py
--rw-rw-rw-   0        0        0    10145 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/loss.py
--rw-rw-rw-   0        0        0    14716 2022-05-28 09:10:50.000000 FastCNN2-1.23.424.1637/FastCNN/utils/metrics.py
--rw-rw-rw-   0        0        0    21526 2022-06-01 12:09:58.000000 FastCNN2-1.23.424.1637/FastCNN/utils/plots.py
--rw-rw-rw-   0        0        0    13884 2022-06-01 12:09:30.000000 FastCNN2-1.23.424.1637/FastCNN/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1740 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      309 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/FastCNN2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2022-04-08 05:42:42.000000 FastCNN2-1.23.424.1637/LICENSE
--rw-rw-rw-   0        0        0      219 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/PKG-INFO
--rw-rw-rw-   0        0        0        2 2022-04-08 05:42:42.000000 FastCNN2-1.23.424.1637/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 08:37:24.000000 FastCNN2-1.23.424.1637/setup.cfg
--rw-rw-rw-   0        0        0     1530 2023-04-24 08:37:18.000000 FastCNN2-1.23.424.1637/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/api/
+-rw-rw-rw-   0        0        0     5922 2022-07-25 09:49:16.000000 FastCNN2-1.23.425.1716/FastCNN/api/camera_.py
+-rw-rw-rw-   0        0        0     2527 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/api/fastcnn_.py
+-rw-rw-rw-   0        0        0     7638 2023-04-24 08:35:52.000000 FastCNN2-1.23.425.1716/FastCNN/api/pytorchfastcnn_.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/datasets/
+-rw-rw-rw-   0        0        0     4588 2022-06-01 11:01:02.000000 FastCNN2-1.23.425.1716/FastCNN/datasets/fastcsv.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/entry/
+-rw-rw-rw-   0        0        0      943 2022-07-13 02:13:51.000000 FastCNN2-1.23.425.1716/FastCNN/entry/camera.py
+-rw-rw-rw-   0        0        0     3133 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/gongda.py
+-rw-rw-rw-   0        0        0      143 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/intergrate.py
+-rw-rw-rw-   0        0        0      987 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/server.py
+-rw-rw-rw-   0        0        0      951 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/server2.py
+-rw-rw-rw-   0        0        0     1354 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/train.py
+-rw-rw-rw-   0        0        0     1355 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/train2.py
+-rw-rw-rw-   0        0        0     1318 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/entry/trainvisiable.py
+-rw-rw-rw-   0        0        0     1338 2022-06-01 12:50:39.000000 FastCNN2-1.23.425.1716/FastCNN/entry/trainyolov5.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/models/
+-rw-rw-rw-   0        0        0    36119 2022-06-01 19:52:23.000000 FastCNN2-1.23.425.1716/FastCNN/models/common.py
+-rw-rw-rw-   0        0        0     4238 2022-06-01 14:26:38.000000 FastCNN2-1.23.425.1716/FastCNN/models/experimental.py
+-rw-rw-rw-   0        0        0    15741 2022-06-01 14:27:01.000000 FastCNN2-1.23.425.1716/FastCNN/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/nn/
+-rw-rw-rw-   0        0        0     1925 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/alexnet.py
+-rw-rw-rw-   0        0        0     3697 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/efficientnets.py
+-rw-rw-rw-   0        0        0     4222 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/nn/experimental.py
+-rw-rw-rw-   0        0        0     1128 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/lenet.py
+-rw-rw-rw-   0        0        0      777 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/neuralnets.py
+-rw-rw-rw-   0        0        0     1122 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/standard.py
+-rw-rw-rw-   0        0        0     3713 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/torchnn.py
+-rw-rw-rw-   0        0        0     4843 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/nn/vgg.py
+-rw-rw-rw-   0        0        0    15693 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/nn/yolo.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/prx/
+-rw-rw-rw-   0        0        0     2952 2022-07-27 06:32:53.000000 FastCNN2-1.23.425.1716/FastCNN/prx/CameraProxy.py
+-rw-rw-rw-   0        0        0     1190 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/prx/DatasetProxy.py
+-rw-rw-rw-   0        0        0    14401 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/prx/GongDaProxy.py
+-rw-rw-rw-   0        0        0    14149 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/prx/GongDaProxy1.py
+-rw-rw-rw-   0        0        0     6745 2023-04-25 09:16:27.000000 FastCNN2-1.23.425.1716/FastCNN/prx/PathProxy.py
+-rw-rw-rw-   0        0        0     6100 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/prx/TrainProxy.py
+-rw-rw-rw-   0        0        0     6484 2022-06-01 10:08:55.000000 FastCNN2-1.23.425.1716/FastCNN/prx/TrainProxy2.py
+-rw-rw-rw-   0        0        0     7938 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/prx/ValidProxy.py
+-rw-rw-rw-   0        0        0     5316 2023-04-24 07:47:37.000000 FastCNN2-1.23.425.1716/FastCNN/prx/ValidProxy2.py
+-rw-rw-rw-   0        0        0    21109 2023-04-24 08:31:59.000000 FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5DetectProxy.py
+-rw-rw-rw-   0        0        0     2406 2022-06-01 12:39:44.000000 FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5Proxy.py
+-rw-rw-rw-   0        0        0    43732 2022-06-02 00:45:04.000000 FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5TrainProxy.py
+-rw-rw-rw-   0        0        0    20311 2022-06-01 17:08:57.000000 FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5ValidProxy.py
+-rw-rw-rw-   0        0        0    30570 2022-06-01 19:53:11.000000 FastCNN2-1.23.425.1716/FastCNN/prx/export.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/
+-rw-rw-rw-   0        0        0     8413 2022-06-01 18:18:09.000000 FastCNN2-1.23.425.1716/FastCNN/utils/CallBacks.py
+-rw-rw-rw-   0        0        0     1542 2022-06-01 09:36:12.000000 FastCNN2-1.23.425.1716/FastCNN/utils/Logs.py
+-rw-rw-rw-   0        0        0    12210 2022-06-01 12:08:37.000000 FastCNN2-1.23.425.1716/FastCNN/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7613 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2256 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/autobatch.py
+-rw-rw-rw-   0        0        0    67782 2022-06-01 17:32:09.000000 FastCNN2-1.23.425.1716/FastCNN/utils/dataloaders.py
+-rw-rw-rw-   0        0        0     7289 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/downloads.py
+-rw-rw-rw-   0        0        0    42735 2022-06-01 12:07:38.000000 FastCNN2-1.23.425.1716/FastCNN/utils/general.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/
+-rw-rw-rw-   0        0        0     8282 2023-04-25 09:16:42.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/
+-rw-rw-rw-   0        0        0       30 2023-04-25 09:16:42.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/__init__.py
+-rw-rw-rw-   0        0        0     1059 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/log_dataset.py
+-rw-rw-rw-   0        0        0     1254 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/sweep.py
+-rw-rw-rw-   0        0        0    28163 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/wandb_utils.py
+-rw-rw-rw-   0        0        0    10145 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/loss.py
+-rw-rw-rw-   0        0        0    14716 2022-05-28 09:10:50.000000 FastCNN2-1.23.425.1716/FastCNN/utils/metrics.py
+-rw-rw-rw-   0        0        0    21526 2022-06-01 12:09:58.000000 FastCNN2-1.23.425.1716/FastCNN/utils/plots.py
+-rw-rw-rw-   0        0        0    13884 2022-06-01 12:09:30.000000 FastCNN2-1.23.425.1716/FastCNN/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1740 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      309 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/FastCNN2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2022-04-08 05:42:42.000000 FastCNN2-1.23.425.1716/LICENSE
+-rw-rw-rw-   0        0        0      219 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2022-04-08 05:42:42.000000 FastCNN2-1.23.425.1716/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 09:16:50.000000 FastCNN2-1.23.425.1716/setup.cfg
+-rw-rw-rw-   0        0        0     1530 2023-04-25 09:16:42.000000 FastCNN2-1.23.425.1716/setup.py
```

### Comparing `FastCNN2-1.23.424.1637/FastCNN/api/camera_.py` & `FastCNN2-1.23.425.1716/FastCNN/api/camera_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/api/fastcnn_.py` & `FastCNN2-1.23.425.1716/FastCNN/api/fastcnn_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/api/pytorchfastcnn_.py` & `FastCNN2-1.23.425.1716/FastCNN/api/pytorchfastcnn_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/datasets/fastcsv.py` & `FastCNN2-1.23.425.1716/FastCNN/datasets/fastcsv.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/camera.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/camera.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/gongda.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/gongda.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/server.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/server.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/server2.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/server2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/train.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/train.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/train2.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/train2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/trainvisiable.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/trainvisiable.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/entry/trainyolov5.py` & `FastCNN2-1.23.425.1716/FastCNN/entry/trainyolov5.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/models/common.py` & `FastCNN2-1.23.425.1716/FastCNN/models/common.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/models/experimental.py` & `FastCNN2-1.23.425.1716/FastCNN/models/experimental.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/models/yolo.py` & `FastCNN2-1.23.425.1716/FastCNN/models/yolo.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/alexnet.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/alexnet.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/efficientnets.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/efficientnets.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/experimental.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/experimental.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/lenet.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/lenet.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/neuralnets.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/neuralnets.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/standard.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/standard.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/torchnn.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/torchnn.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/vgg.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/vgg.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/nn/yolo.py` & `FastCNN2-1.23.425.1716/FastCNN/nn/yolo.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/CameraProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/CameraProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/DatasetProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/DatasetProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/GongDaProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/GongDaProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/GongDaProxy1.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/GongDaProxy1.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/PathProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/PathProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 import sys
 
 def getRoot(sec=[r"C:/"]):
     for r in sec:
         if os.path.exists(r):
             return r
 
+def getDataPath():
+    rtn = r"{}FastCNN/Data".format(getRoot([r"d:/","c:/"]))
+    if not os.path.exists(rtn):
+        rtn = r"{}FastCNN/Data".format(getRoot([r"e:/",r"d:/","c:/"]))
+    return rtn
+
 app_path = r"{}FastCNN/Coach".format(getRoot([r"d:/","c:/"]))
-data_path = r"{}FastCNN/Data".format(getRoot([r"e:/",r"d:/","c:/"]))
+data_path = getDataPath()
 
 if sys.platform == "linux":
     app_path = "/usr/local/App/Coach"
     data_path = "usr/local/Data/"
 
 class PathProxy:
     """
```

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/TrainProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/TrainProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/TrainProxy2.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/TrainProxy2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/ValidProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/ValidProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/ValidProxy2.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/ValidProxy2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5DetectProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5DetectProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5Proxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5Proxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5TrainProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5TrainProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/YoloV5ValidProxy.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/YoloV5ValidProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/prx/export.py` & `FastCNN2-1.23.425.1716/FastCNN/prx/export.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/CallBacks.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/CallBacks.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/Logs.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/Logs.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/augmentations.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/autoanchor.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/autobatch.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/dataloaders.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/downloads.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/general.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/general.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/loggers/__init__.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/log_dataset.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/log_dataset.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/sweep.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/sweep.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/loggers/wandb/wandb_utils.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/loss.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/loss.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/metrics.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/plots.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/plots.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN/utils/torch_utils.py` & `FastCNN2-1.23.425.1716/FastCNN/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/FastCNN2.egg-info/SOURCES.txt` & `FastCNN2-1.23.425.1716/FastCNN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/LICENSE` & `FastCNN2-1.23.425.1716/LICENSE`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.424.1637/setup.py` & `FastCNN2-1.23.425.1716/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 
 """
 set App Name
 """
 name = "FastCNN2"
-version = '1.23.0424.1637'
+version = '1.23.0425.1716'
 
 author = "Iuty"
 author_email = "dfdfggg@126.com"
 
 """
 set entry_points
 """
```

