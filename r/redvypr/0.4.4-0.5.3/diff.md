# Comparing `tmp/redvypr-0.4.4.tar.gz` & `tmp/redvypr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvypr-0.4.4.tar", last modified: Fri Jun 17 04:28:00 2022, max compression
+gzip compressed data, was "redvypr-0.5.3.tar", last modified: Tue Apr 25 09:49:25 2023, max compression
```

## Comparing `redvypr-0.4.4.tar` & `redvypr-0.5.3.tar`

### file list

```diff
@@ -1,77 +1,99 @@
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.760525 redvypr-0.4.4/
--rw-r--r--   0 holterma  (1000) holterma  (1000)    35149 2022-03-17 04:29:20.000000 redvypr-0.4.4/LICENSE
--rw-r--r--   0 holterma  (1000) holterma  (1000)      795 2022-06-17 04:28:00.760525 redvypr-0.4.4/PKG-INFO
--rw-r--r--   0 holterma  (1000) holterma  (1000)     3030 2022-06-17 04:23:43.000000 redvypr-0.4.4/README.md
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr/
--rw-r--r--   0 holterma  (1000) holterma  (1000)        5 2022-06-17 04:17:16.000000 redvypr-0.4.4/redvypr/VERSION
--rw-r--r--   0 holterma  (1000) holterma  (1000)      237 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    13252 2022-06-15 14:40:53.000000 redvypr-0.4.4/redvypr/data_packets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5631 2022-06-11 04:14:22.000000 redvypr-0.4.4/redvypr/device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr/devices/
--rw-r--r--   0 holterma  (1000) holterma  (1000)      448 2022-06-16 11:21:11.000000 redvypr-0.4.4/redvypr/devices/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)   119101 2022-06-10 14:57:05.000000 redvypr-0.4.4/redvypr/devices/calibration.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    12876 2022-06-17 04:23:06.000000 redvypr-0.4.4/redvypr/devices/csvlogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6141 2022-05-31 03:52:46.000000 redvypr-0.4.4/redvypr/devices/exampledevice.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2038 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/exampledevice_bare.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    11954 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/gps_device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr/devices/manufacturer/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       52 2022-05-06 08:56:37.000000 redvypr-0.4.4/redvypr/devices/manufacturer/__init__.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       84 2022-05-21 14:30:40.000000 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    14671 2022-05-24 11:14:57.000000 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/ads124s0x.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    16864 2022-04-27 12:52:56.000000 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/datalogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    21024 2022-05-29 12:55:54.000000 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/datalogger_rpi.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    18927 2022-04-26 17:42:52.000000 redvypr-0.4.4/redvypr/devices/manufacturer/ce_sensors/heatflow_sensor.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr/devices/manufacturer/leitenberger/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       28 2022-05-02 13:01:30.000000 redvypr-0.4.4/redvypr/devices/manufacturer/leitenberger/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    21420 2022-05-26 04:22:21.000000 redvypr-0.4.4/redvypr/devices/manufacturer/leitenberger/lrcal_Tfluid.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     4192 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/mergedata.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    51819 2022-06-03 18:07:49.000000 redvypr-0.4.4/redvypr/devices/netcdflogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    31589 2022-06-03 18:05:32.000000 redvypr-0.4.4/redvypr/devices/network_device.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    11367 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/nmea_logbook.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    10179 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/nmea_sensor.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    50328 2022-06-10 04:09:11.000000 redvypr-0.4.4/redvypr/devices/plot.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    14515 2022-06-14 14:52:15.000000 redvypr-0.4.4/redvypr/devices/randdata.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     4347 2022-04-26 17:37:26.000000 redvypr-0.4.4/redvypr/devices/rawdatadisp.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    16343 2022-06-15 08:42:58.000000 redvypr-0.4.4/redvypr/devices/rawdatalogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    15941 2022-06-16 04:03:00.000000 redvypr-0.4.4/redvypr/devices/rawdatareplay.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    12414 2022-05-06 04:02:41.000000 redvypr-0.4.4/redvypr/devices/serial_device.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    17078 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/devices/textlogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      990 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/files.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    29237 2022-06-09 13:10:07.000000 redvypr-0.4.4/redvypr/gui.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.760525 redvypr-0.4.4/redvypr/icon/
--rw-r--r--   0 holterma  (1000) holterma  (1000)    11374 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v02.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    10980 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v02.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    39662 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v03.1.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5924 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v03.1.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    34925 2022-06-05 18:16:36.000000 redvypr-0.4.4/redvypr/icon/icon_v03.1_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    38644 2022-06-06 07:01:58.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    38680 2022-06-06 07:01:15.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6006 2022-06-06 07:00:49.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1150 2022-06-06 13:10:10.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2_favicon.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    24079 2022-06-06 09:05:14.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    16110 2022-06-06 09:07:27.000000 redvypr-0.4.4/redvypr/icon/icon_v03.2_verysmall.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    25790 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v03.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5560 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/icon_v03.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    28999 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/logo_merged.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     4997 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/logo_v01.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5197 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/logo_v02.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    45795 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/logo_v03.1.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6585 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/logo_v03.1.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6498 2022-06-06 06:59:44.000000 redvypr-0.4.4/redvypr/icon/logo_v03.2.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    27174 2022-06-05 18:22:35.000000 redvypr-0.4.4/redvypr/icon/logo_v03.2_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    27301 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/icon/redvypr_logo_v02.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    82128 2022-06-15 04:55:18.000000 redvypr-0.4.4/redvypr/redvypr.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      288 2022-03-17 04:29:20.000000 redvypr-0.4.4/redvypr/standard_device_widgets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5585 2022-06-09 13:12:35.000000 redvypr-0.4.4/redvypr/utils.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      516 2022-04-19 05:07:55.000000 redvypr-0.4.4/redvypr/version.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2022-06-17 04:28:00.756525 redvypr-0.4.4/redvypr.egg-info/
--rw-r--r--   0 holterma  (1000) holterma  (1000)      795 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/PKG-INFO
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2051 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/SOURCES.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/dependency_links.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)       50 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/entry_points.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2022-03-17 04:32:33.000000 redvypr-0.4.4/redvypr.egg-info/not-zip-safe
--rw-r--r--   0 holterma  (1000) holterma  (1000)       33 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/requires.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        8 2022-06-17 04:28:00.000000 redvypr-0.4.4/redvypr.egg-info/top_level.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)       38 2022-06-17 04:28:00.760525 redvypr-0.4.4/setup.cfg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1546 2022-06-17 04:27:38.000000 redvypr-0.4.4/setup.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.692566 redvypr-0.5.3/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    35149 2022-03-17 04:29:20.000000 redvypr-0.5.3/LICENSE
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-25 09:49:25.692566 redvypr-0.5.3/PKG-INFO
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     3030 2022-06-17 04:23:43.000000 redvypr-0.5.3/README.md
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.680566 redvypr-0.5.3/redvypr/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        5 2023-04-25 09:36:55.000000 redvypr-0.5.3/redvypr/VERSION
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      286 2023-04-25 09:31:02.000000 redvypr-0.5.3/redvypr/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    26761 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/config.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    10726 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/configdata.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    40720 2023-03-26 03:39:27.000000 redvypr-0.5.3/redvypr/data_packets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27230 2023-04-25 04:44:39.000000 redvypr-0.5.3/redvypr/device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.680566 redvypr-0.5.3/redvypr/devices/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      135 2023-04-10 17:52:06.000000 redvypr-0.5.3/redvypr/devices/__init__.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.680566 redvypr-0.5.3/redvypr/devices/db/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2023-03-29 11:49:05.000000 redvypr-0.5.3/redvypr/devices/db/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1872 2022-12-11 06:19:03.000000 redvypr-0.5.3/redvypr/devices/db/influxdb_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/develop/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       24 2023-04-19 10:29:29.000000 redvypr-0.5.3/redvypr/devices/develop/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    37708 2023-03-26 05:06:47.000000 redvypr-0.5.3/redvypr/devices/develop/csvlogger.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/fileio/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       56 2023-04-19 10:29:41.000000 redvypr-0.5.3/redvypr/devices/fileio/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28729 2023-04-06 05:28:30.000000 redvypr-0.5.3/redvypr/devices/fileio/rawdatalogger.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    16771 2023-04-05 18:41:57.000000 redvypr-0.5.3/redvypr/devices/fileio/rawdatareplay.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/interface/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       28 2023-04-10 17:40:41.000000 redvypr-0.5.3/redvypr/devices/interface/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    15186 2023-04-17 11:51:35.000000 redvypr-0.5.3/redvypr/devices/interface/serial_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/network/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       77 2023-03-29 11:42:45.000000 redvypr-0.5.3/redvypr/devices/network/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)   101562 2023-04-25 04:50:06.000000 redvypr-0.5.3/redvypr/devices/network/iored.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    33337 2023-01-09 05:25:09.000000 redvypr-0.5.3/redvypr/devices/network/network_device.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     8771 2023-04-17 17:53:48.000000 redvypr-0.5.3/redvypr/devices/network/zeromq_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/plot/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       72 2023-04-10 17:41:27.000000 redvypr-0.5.3/redvypr/devices/plot/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    31897 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/devices/plot/plot.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    23149 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/devices/plot/plot_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2907 2023-04-17 17:53:38.000000 redvypr-0.5.3/redvypr/devices/plot/rawdatadisp.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/processing/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       79 2023-04-10 17:58:08.000000 redvypr-0.5.3/redvypr/devices/processing/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2121 2023-04-17 17:54:15.000000 redvypr-0.5.3/redvypr/devices/processing/csvparser.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6499 2023-04-19 04:26:46.000000 redvypr-0.5.3/redvypr/devices/processing/nmeaparser.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5761 2023-04-17 17:54:15.000000 redvypr-0.5.3/redvypr/devices/processing/sensor_raw2unit.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.684566 redvypr-0.5.3/redvypr/devices/test/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       26 2023-03-29 11:50:28.000000 redvypr-0.5.3/redvypr/devices/test/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2156 2023-04-05 10:52:52.000000 redvypr-0.5.3/redvypr/devices/test/test_device.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      990 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/files.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28218 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/gui.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.688566 redvypr-0.5.3/redvypr/icon/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    11374 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v02.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    10980 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v02.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    39662 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v03.1.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5924 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v03.1.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    34925 2022-06-05 18:16:36.000000 redvypr-0.5.3/redvypr/icon/icon_v03.1_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    38644 2022-06-06 07:01:58.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    38680 2022-06-06 07:01:15.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6006 2022-06-06 07:00:49.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1150 2022-06-06 13:10:10.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2_favicon.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    24079 2022-06-06 09:05:14.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    16110 2022-06-06 09:07:27.000000 redvypr-0.5.3/redvypr/icon/icon_v03.2_verysmall.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    25790 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v03.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5560 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/icon_v03.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28999 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/logo_merged.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     4997 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/logo_v01.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5197 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/logo_v02.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    45795 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/logo_v03.1.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6585 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/logo_v03.1.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6498 2022-06-06 06:59:44.000000 redvypr-0.5.3/redvypr/icon/logo_v03.2.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27174 2022-06-05 18:22:35.000000 redvypr-0.5.3/redvypr/icon/logo_v03.2_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27301 2022-03-17 04:29:20.000000 redvypr-0.5.3/redvypr/icon/redvypr_logo_v02.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    84616 2023-04-25 09:07:34.000000 redvypr-0.5.3/redvypr/redvypr.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.688566 redvypr-0.5.3/redvypr/utils/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       23 2023-04-25 09:30:22.000000 redvypr-0.5.3/redvypr/utils/__init__.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.688566 redvypr-0.5.3/redvypr/utils/csv2dict/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1077 2023-04-25 09:29:49.000000 redvypr-0.5.3/redvypr/utils/csv2dict/NMEA_functions.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        5 2023-04-25 09:29:49.000000 redvypr-0.5.3/redvypr/utils/csv2dict/VERSION
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      215 2023-04-25 09:29:49.000000 redvypr-0.5.3/redvypr/utils/csv2dict/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     9932 2023-04-25 09:29:49.000000 redvypr-0.5.3/redvypr/utils/csv2dict/csv2dict.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      516 2022-04-19 05:07:55.000000 redvypr-0.5.3/redvypr/version.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.688566 redvypr-0.5.3/redvypr/widgets/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2022-12-02 05:59:19.000000 redvypr-0.5.3/redvypr/widgets/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     7664 2023-03-24 16:08:24.000000 redvypr-0.5.3/redvypr/widgets/datastream_widget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    32322 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/widgets/gui_config_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5964 2023-02-20 13:31:35.000000 redvypr-0.5.3/redvypr/widgets/standard_device_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    53424 2023-04-25 09:24:41.000000 redvypr-0.5.3/redvypr/widgets/tmp.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.680566 redvypr-0.5.3/redvypr.egg-info/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/PKG-INFO
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2399 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/SOURCES.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/dependency_links.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       49 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/entry_points.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2022-03-17 04:32:33.000000 redvypr-0.5.3/redvypr.egg-info/not-zip-safe
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       55 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/requires.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        8 2023-04-25 09:49:25.000000 redvypr-0.5.3/redvypr.egg-info/top_level.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       38 2023-04-25 09:49:25.692566 redvypr-0.5.3/setup.cfg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1623 2023-04-25 09:49:23.000000 redvypr-0.5.3/setup.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 09:49:25.692566 redvypr-0.5.3/test/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     8082 2023-01-05 11:46:21.000000 redvypr-0.5.3/test/test_config.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     4749 2023-02-18 13:42:06.000000 redvypr-0.5.3/test/test_configwidget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      705 2023-03-29 03:33:18.000000 redvypr-0.5.3/test/test_devicescanwidget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      383 2023-03-28 10:24:09.000000 redvypr-0.5.3/test/test_find_devices.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      221 2023-01-14 15:22:49.000000 redvypr-0.5.3/test/test_iored_1.py
```

### Comparing `redvypr-0.4.4/LICENSE` & `redvypr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/PKG-INFO` & `redvypr-0.5.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: redvypr
-Version: 0.4.4
+Version: 0.5.3
 Summary: redvypr: REaltime Data Viewer and PRocessor (in PYthon)
 Home-page: https://github.com/redvypr/redvypr
 Author: Peter Holtermann
-Author-email: peter.holtermann@systemausfall.org
+Author-email: peter.holtermann@io-warnemuende.de
 License: GPLv03
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 redvypr: REaltime Data Viewer and PRocessor (in PYthon). Python based software to read, process, fuse, distribute, save and visualize data from various sensors.
-
```

### Comparing `redvypr-0.4.4/README.md` & `redvypr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/device.py` & `redvypr-0.5.3/redvypr/widgets/standard_device_widgets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,168 +1,191 @@
-"""
-
-redvypr device class
-
-
-
-"""
-
 import datetime
 import logging
 import queue
 from PyQt5 import QtWidgets, QtCore, QtGui
 import time
 import logging
 import sys
 import yaml
+from redvypr.device import redvypr_device
+from redvypr.widgets.gui_config_widgets import configWidget
 
 logging.basicConfig(stream=sys.stderr)
-logger = logging.getLogger('device')
+logger = logging.getLogger('redvypr')
 logger.setLevel(logging.DEBUG)
 
 
-class redvypr_device():
-    def __init__(self,dataqueue=None,comqueue=None,datainqueue=None,config = [],publish=False,subscribe=False):
-        """
-        """
-        self.publish     = publish   # publishes data, a typical device is doing this
-        self.subscribe   = suscribe  # subscribing data, a typical datalogger is doing this
-        self.datainqueue = datainqueue
-        self.dataqueue   = dataqueue        
-        self.comqueue    = comqueue
-        self.config      = config # Please note that this is typically a placeholder, the config structure will be written by redvypr and the yaml
-
-    def start(self):
-        start(self.datainqueue,self.dataqueue,self.comqueue)
-        
-    def __str__(self):
-        sstr = 'redvypr_device'
-        return sstr
-    
-    
-    def get_datakeys(self):
-        """ Returns a list of datakey that the device has in their data dictionary
-        datakeys = ['t','data','?data','temperature']
-        """
-        
-        return []
-
-    def get_info(self):
-        """This a example function displaying information about the device
-
-        """
-        print('get_info():')
-        print('Name' + self.name)
-        print('redvypr' + self.redvypr)        
-
-
-
-class initDeviceWidget(QtWidgets.QWidget):
-    device_start = QtCore.pyqtSignal(Device) # Signal requesting a start of the device (starting the thread)
-    device_stop  = QtCore.pyqtSignal(Device) # Signal requesting a stop of device
-    connect      = QtCore.pyqtSignal(Device) # Signal requesting a connect of the datainqueue with available dataoutqueues of other devices
-    def __init__(self,device=None):
-        super(QtWidgets.QWidget, self).__init__()
-        layout        = QtWidgets.QFormLayout(self)
-        self.device   = device
-        self.label    = QtWidgets.QLabel("Rawdatadisplay setup")
-        self.conbtn = QtWidgets.QPushButton("Connect logger to devices")
-        self.conbtn.clicked.connect(self.con_clicked)        
-        self.startbtn = QtWidgets.QPushButton("Start logging")
-        self.startbtn.clicked.connect(self.start_clicked)
-        self.startbtn.setCheckable(True)
-
-        self.infobtn = QtWidgets.QPushButton("Get some information")
-        self.infobtn.clicked.connect(self.info_clicked)                
-
-        layout.addRow(self.label)
-        layout.addRow(self.infobtn)        
-        layout.addRow(self.conbtn)
-        layout.addRow(self.startbtn)
-
-    def finalize_init(self):
-        """ This function is called after the configuration is parsed
-        """
-        print('Finalize init')
-
-    def info_clicked(self):
-        # This is the entry of the redvypr devicelist, giving full
-        # access to all widgets related to this device
-        print(self.redvyprdevicelistentry)
-    def con_clicked(self):
-        button = self.sender()
-        self.connect.emit(self.device)        
-            
-    def start_clicked(self):
-        button = self.sender()
-        if button.isChecked():
-            print("button pressed")
-            self.device_start.emit(self.device)
-            button.setText("Stop logging")
-            self.conbtn.setEnabled(False)
-        else:
-            print('button released')
-            self.device_stop.emit(self.device)
-            button.setText("Start logging")
-            self.conbtn.setEnabled(True)
-            
-            
-    def thread_status(self,status):
-        """ This function is called by redvypr whenever the thread is started/stopped
-        """   
-        self.update_buttons(status['threadalive'])
-
-       
-    def update_buttons(self,thread_status):
-            """ Updating all buttons depending on the thread status (if its alive, graying out things)
-            """
-            if(thread_status):
-                self.startbtn.setText('Stop logging')
-                self.startbtn.setChecked(True)
-                #self.conbtn.setEnabled(False)
-            else:
-                self.startbtn.setText('Start logging')
-                #self.conbtn.setEnabled(True)
-
-
-
-
-class displayDeviceWidget(QtWidgets.QWidget):
-    """ Widget is plotting realtimedata using the pyqtgraph functionality
-    This widget can be configured with a configuration dictionary 
+class displayDeviceWidget_standard(QtWidgets.QWidget):
+    """ Widget is displaying incoming data as text
     """
-    def __init__(self,device=None,tabwidget=None):
+
+    def __init__(self, device=None, tabwidget=None):
         """
         device [optional]
         tabwidget [optional]
-        
+
         """
         funcname = __name__ + '.start()'
         super(QtWidgets.QWidget, self).__init__()
-        layout        = QtWidgets.QGridLayout(self)
+        layout = QtWidgets.QGridLayout(self)
         self.device = device
-        self.tabname = 'exampledevice plot' # This name is taken as the tabname [optional], otherwise "Display data" is used
+        # A timer that is regularly calling the device.status function
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update_status)
+        self.statustimer.start(2000)
+
+        self.text = QtWidgets.QPlainTextEdit(self)
+        self.text.setReadOnly(True)
+        self.text.setMaximumBlockCount(10000)
+        layout.addWidget(self.text, 0, 0)
 
-                
-    def thread_status(self,status):
+    def thread_status(self, status):
         """ This function is regularly called by redvypr whenever the thread is started/stopped
         """
-        pass        
-        #self.update_buttons(status['threadalive'])
-        
-
-        
-    def update(self,data):
-        """ 
+        pass
+        # self.update_buttons(status['threadalive'])
+
+    def update_status(self):
+        """
+        """
+        funcname = __name__ + 'update_status():'
+        try:
+            statusdata = self.device.status()
+            # print(funcname + str(statusdata))
+            self.text.clear()
+            self.text.insertPlainText(str(statusdata))
+        except Exception as e:
+            # logger.debug(funcname + str(e) + 'hallo')
+            pass
+
+    def update(self, data):
+        """
         """
         funcname = __name__ + '.update()'
         tnow = time.time()
-        #print('got data',data)
+        # print('got data',data)
 
         devicename = data['device']
         # Only plot the data in intervals of dt_update length, this prevents high CPU loads for fast devices
         update = (tnow - self.config['last_update']) > self.config['dt_update']
-        
-        if(update):
+
+        if (update):
             self.config['last_update'] = tnow
-            
 
+
+
+
+
+#
+#
+#
+#
+#
+class redvypr_deviceInitWidget(QtWidgets.QWidget):
+    connect = QtCore.pyqtSignal(
+        redvypr_device)  # Signal requesting a connect of the datainqueue with available dataoutqueues of other devices
+
+    def __init__(self, device=None):
+        """
+        Standard deviceinitwidget if the device is not providing one by itself.
+
+        Args:
+            device:
+        """
+        funcname = __name__ + '.__init__():'
+        logger.debug(funcname)
+        super().__init__()
+        self.layout = QtWidgets.QGridLayout(self)
+        self.config_widgets = []
+        self.device = device
+        self.config_widget = configWidget(device.config,redvypr_instance=self.device.redvypr)
+
+        self.config_widgets.append(self.config_widget)
+
+        # Start-button
+        self.startbutton = QtWidgets.QPushButton('Start')
+        self.startbutton.clicked.connect(self.start_clicked)
+        self.startbutton.setCheckable(True)
+        # Process kill button (if thread)
+        if (self.device.mp == 'multiprocess'):
+            # Killbutton
+            self.killbutton = QtWidgets.QPushButton('Kill process')
+            self.killbutton.clicked.connect(self.kill_clicked)
+
+        # Connect button
+        self.conbutton = QtWidgets.QPushButton("Connect")
+        self.conbutton.clicked.connect(self.connect_clicked)
+        self.config_widgets.append(self.conbutton)
+
+        self.layout.addWidget(self.config_widget, 0, 0, 1, 4)
+        self.layout.addWidget(self.conbutton, 1, 0, 1, 4)
+        if (self.device.mp == 'multiprocess'):
+            self.layout.addWidget(self.startbutton, 2, 0, 1, 3)
+            self.layout.addWidget(self.killbutton, 2, 3)
+        else:
+            self.layout.addWidget(self.startbutton, 2, 0, 1, 4)
+
+        # If the config is changed, update the device widget
+
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update_buttons)
+        self.statustimer.start(500)
+
+        self.config_widget.config_changed_flag.connect(self.config_changed)
+
+    def config_changed(self):
+        """
+
+
+        Args:
+            config:
+
+        Returns:
+
+        """
+        funcname = __name__ + '.config_changed():'
+        logger.debug(funcname)
+
+    def kill_clicked(self):
+        button = self.sender()
+        logger.debug("Kill device {:s}".format(self.device.name))
+        self.device.kill_process()
+
+    def start_clicked(self):
+        button = self.sender()
+        if button.isChecked():
+            logger.debug("button pressed")
+            button.setText('Starting')
+            self.device.thread_start()
+            # self.device_start.emit(self.device)
+        else:
+            logger.debug('button released')
+            # button.setText('Stopping')
+            self.startbutton.setChecked(True)
+            self.device.thread_stop()
+
+    def update_buttons(self):
+        """ Updating all buttons depending on the thread status (if its alive, graying out things)
+        """
+
+        status = self.device.get_thread_status()
+        thread_status = status['thread_status']
+        # Running
+        if (thread_status):
+            self.startbutton.setText('Stop')
+            self.startbutton.setChecked(True)
+            for w in self.config_widgets:
+                w.setEnabled(False)
+        # Not running
+        else:
+            self.startbutton.setText('Start')
+            for w in self.config_widgets:
+                w.setEnabled(True)
+
+            # Check if an error occured and the startbutton
+            if (self.startbutton.isChecked()):
+                self.startbutton.setChecked(False)
+            # self.conbtn.setEnabled(True)
+
+    def connect_clicked(self):
+        button = self.sender()
+        self.connect.emit(self.device)
```

### Comparing `redvypr-0.4.4/redvypr/devices/gps_device.py` & `redvypr-0.5.3/redvypr/devices/interface/serial_device.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,306 +1,365 @@
-"""
-.
-
-The gps device converts stadard nmea messages used in marine navigation into redvypr format 
-
-
-Configuration options for the gps device:
-
-.. code-block::
-
-    - deviceconfig:
-    name: gps
-    config:
-      key: 'data' # The dictionary key of the raw NMEA string, defaults to 'data'
-      append: True # If the raw message is tranported in pieces, append data until a valid message was found
-      maxlen: 10000 # The maximum length of text buffer to search for NMEA messages
-      #sentences: all Set sentences to all, or a list of sentences (see next line)
-      sentences: # Filter for the NMEA sentences 
-          - RMC
-          - GGA
-                     
-
-  devicemodulename: gps_device
-
-
-"""
-
 import datetime
 import logging
 import queue
 from PyQt5 import QtWidgets, QtCore, QtGui
 import time
 import numpy as np
 import serial
 import serial.tools.list_ports
 import logging
 import sys
-import pynmea2
+from redvypr.data_packets import do_data_statistics, create_data_statistic_dict,check_for_command
+
+
+description = 'Reading data from a serial device'
+
 
 logging.basicConfig(stream=sys.stderr)
-logger = logging.getLogger('gps_device')
+logger = logging.getLogger('serial_device')
 logger.setLevel(logging.DEBUG)
 
-def parse_nmea(nmea_data):
-    try:
-        msg = pynmea2.parse(nmea_data)
-        logger.debug('Valid message:' + str(msg))
-        data_nmea = {'valid_nmea':True}
-        data_nmea['nmea'] = str(msg) + '\n'
-        data_nmea['lat'] = msg.latitude
-        data_nmea['lon'] = msg.longitude
-        try: # If there is a date
-            data_nmea['date'] = msg.datestamp.strftime("%m%d%y")
-        except:
-            pass
-        try: # If there is a date
-            data_nmea['time'] = msg.timestamp.strftime("%H%M%S.%f")[:-4]
-        except:
-            pass    
-        
-        data_nmea['sentence_type'] = msg.sentence_type
-        return data_nmea
-    except Exception as e:
-        data_nmea = {'valid_nmea':False}
-        return data_nmea
 
+config_template              = {}
+config_template['comport']   = {'type':'str'}
+config_template['baud']      = {'type':'int','default':4800}
+config_template['parity']    = {'type':'int','default':serial.PARITY_NONE}
+config_template['stopbits']  = {'type':'int','default':serial.STOPBITS_ONE}
+config_template['bytesize']  = {'type':'int','default':serial.EIGHTBITS}
+config_template['dt_poll']   = {'type':'float','default':0.05}
+config_template['chunksize'] = {'type':'int','default':1000} # The maximum amount of bytes read with one chunk
+config_template['packetdelimiter'] = {'type':'str','default':'\n'} # The maximum amount of bytes read with one chunk
+config_template['redvypr_device'] = {}
+config_template['redvypr_device']['publishes']   = True
+config_template['redvypr_device']['subscribes'] = False
+config_template['redvypr_device']['description'] = description
+
+
+def start(device_info, config={}, dataqueue=None, datainqueue=None, statusqueue=None):
+    """
+
+    """
+    funcname = __name__ + '.start()'
+    logger.debug(funcname + ':Starting reading serial data')
+    chunksize   = config['chunksize'] #The maximum amount of bytes read with one chunk    
+    serial_name = config['comport']
+    baud        = config['baud']
+    parity      = config['parity']    
+    stopbits    = config['stopbits']    
+    bytesize    = config['bytesize']    
+    dt_poll     = config['dt_poll']
+
+    print('Starting',config)
     
-def start(dataqueue,comqueue,datainqueue,devicename,config):
-    funcname = __name__ + '.start()'        
-    logger.debug(funcname + ':Starting reading NMEA data')        
-    nmea_sentence = ''
-    sentences = 0
-    try:
-        nmea_key = config['key']
-    except:
-        nmea_key = 'data'
-        
-    try:
-        config['append']
-    except:
-        config['append'] = False
-        
-    try:
-        config['sentences']
-    except:
-        config['sentences'] = 'all'
+    newpacket   = config['packetdelimiter']
+    # Check if a delimiter shall be used (\n, \r\n, etc ...)
+    if(len(newpacket)>0):
+        FLAG_DELIMITER = True
+    else:
+        FLAG_DELIMITER = False
+    if(type(newpacket) is not bytes):
+        newpacket = newpacket.encode('utf-8')
         
-    try:
-        config['maxlen']
-    except:
-        config['maxlen'] = 10000
-        
-    logger.debug(funcname + ': config {:s}'.format(str(config)))
-    nmea_sentence_append = '' # Only used for append
-    while True:
-        data = datainqueue.get() # This is a blocking read
-        if('command' in data.keys()):
-            if(data['command'] == 'stop'):
-                logger.info(funcname + ': received stop command, stopping now')
-                break    
-        if True:
-            if(nmea_key in data.keys()):
-                nmea_sentence_raw = data[nmea_key]
-                if(config['append']):
-                    #print('appending')
-                    nmea_sentence_append += nmea_sentence_raw
-                    # Precheck if there is at all valid data
-                    if(('\n' in nmea_sentence_append) and ('$' in nmea_sentence_append)):
-                        nmea_sentence_all = nmea_sentence_append.split('\n')
-                        nmea_last = nmea_sentence_all[-1]
-                    else:
-                        nmea_sentence_all = []
-                else:
-                    nmea_sentence_all = [nmea_sentence_raw]
-                    nmea_last = nmea_sentence_all[-1]
-                # save the last sentence 
-                
-                if(len(nmea_sentence_all)>0):
-                    if(len(nmea_sentence_all[-1])>0): # This happens if the last character is not a \n
-                        nmea_sentence_append = nmea_sentence_all[-1]
-                        
-                    nmea_sentence_all.pop(-1) # Remove last sentence (either '' or rest)
-                    
-                # loop over all NMEA sentences 
-                for nmea_sentence in nmea_sentence_all:  
-                    data_parse = parse_nmea(nmea_sentence)  
-                    #print(data_parse)
-                    #print(nmea_sentence_all)
-                    
-                    data_parse['device']  = devicename
-                    if(data_parse['valid_nmea']):
-                        nmea_sentence_all.remove(nmea_sentence)
-                        sentence_right = config['sentences'] == 'all'
-                        sentence_right = sentence_right or (data_parse['sentence_type'] in config['sentences'])
-                        if(sentence_right): # Which message shall be used?
-                            dataqueue.put(data_parse)
-                            data_parse['host'] = data['host']
-                            data_parse['t'] = data['t']
-                            sentences += 1
-                                
-                            
+    rawdata_all    = b''
+    dt_update      = 1 # Update interval in seconds
+    bytes_read     = 0
+    sentences_read = 0
+    bytes_read_old = 0 # To calculate the amount of bytes read per second
+    t_update       = time.time()
+    serial_device = False
+    if True:
+        try:
+            serial_device = serial.Serial(serial_name,baud,parity=parity,stopbits=stopbits,bytesize=bytesize,timeout=0)
+            #print('Serial device 0',serial_device)
+            #serial_device.timeout(0.05)
+            #print('Serial device 1',serial_device)                        
+        except Exception as e:
+            #print('Serial device 2',serial_device)
+            logger.debug(funcname + ': Exception open_serial_device {:s} {:d}: '.format(serial_name,baud) + str(e))
+            return False
 
+    got_dollar = False    
+    while True:
+        # TODO, here commands could be send as well
+        try:
+            data = datainqueue.get(block=False)
+        except:
+            data = None
+        if (data is not None):
+            command = check_for_command(data, thread_uuid=device_info['thread_uuid'])
+            # logger.debug('Got a command: {:s}'.format(str(data)))
+            if (command is not None):
+                if command == 'stop':
+                    serial_device.close()
+                    sstr = funcname + ': Command is for me: {:s}'.format(str(command))
+                    logger.debug(sstr)
+                    try:
+                        statusqueue.put_nowait(sstr)
+                    except:
+                        pass
+                    return
+
+
+        time.sleep(dt_poll)
+        ndata = serial_device.inWaiting()
+        try:
+            rawdata_tmp = serial_device.read(ndata)
+        except Exception as e:
+            print(e)
+            #print('rawdata_tmp', rawdata_tmp)
 
-class Device():
-    def __init__(self,dataqueue=None,comqueue=None,datainqueue=None):
-        """
-        """
-        self.publish     = True # publishes data, a typical device is doing this
-        self.subscribe   = True  # subscribing data, a typical datalogger is doing this
-        self.datainqueuestop  = True  # Send the stop command into the dataqueuue
-        self.autostart   = True # Start the thread directly after initialization
-        self.datainqueue = datainqueue
-        self.dataqueue   = dataqueue        
-        self.comqueue    = comqueue
-        self.config = {}
+        nread = len(rawdata_tmp)
+        if True:
+            if nread > 0:
+                bytes_read  += nread
+                rawdata_all += rawdata_tmp
+                #print('rawdata_all',rawdata_all)
+                FLAG_CHUNK = len(rawdata_all) > chunksize
+                if(FLAG_CHUNK):
+                    data               = {'t':time.time()}
+                    data['data']       = rawdata_all
+                    data['comport']    = serial_device.name
+                    data['bytes_read'] = bytes_read
+                    dataqueue.put(data)
+                    rawdata_all = b''
+
+                # Check if the newpacket character in the data
+                if(FLAG_DELIMITER):
+                    FLAG_CHAR = newpacket in rawdata_all
+                    if(FLAG_CHAR):
+                        rawdata_split = rawdata_all.split(newpacket)
+                        #print('rawdata_all', rawdata_all)
+                        if(len(rawdata_split)>1): # If len==0 then character was not found
+                            for ind in range(len(rawdata_split)-1): # The last packet does not have the split character
+                                sentences_read += 1
+                                raw = rawdata_split[ind] + newpacket # reconstruct the data
+                                #print('raw', raw)
+                                data               = {'t':time.time()}
+                                data['data']       = raw
+                                data['comport']    = serial_device.name
+                                data['bytes_read'] = bytes_read
+                                data['sentences_read'] = sentences_read
+                                dataqueue.put(data)
 
-    def start(self):
-        start(self.dataqueue,self.comqueue,self.datainqueue,devicename=self.name,config=self.config)
+                            rawdata_all = rawdata_split[-1]
         
+            
+            
+        if((time.time() - t_update) > dt_update):
+            dbytes = bytes_read - bytes_read_old
+            bytes_read_old = bytes_read
+            bps = dbytes/dt_update# bytes per second
+            #print('ndata',len(rawdata_all),'rawdata',rawdata_all,type(rawdata_all))
+            #print('bps',bps)
+            t_update = time.time()
+            
+                
+
 
-    def __str__(self):
-        sstr = 'GPS device'
-        return sstr
 
 
 
 class initDeviceWidget(QtWidgets.QWidget):
-    device_start = QtCore.pyqtSignal(Device)
-    device_stop = QtCore.pyqtSignal(Device)        
     def __init__(self,device=None):
         super(QtWidgets.QWidget, self).__init__()
         layout        = QtWidgets.QVBoxLayout(self)
         self.device   = device
-        self.inputtabs = QtWidgets.QTabWidget() # Create tabs for different connection types
         self.serialwidget = QtWidgets.QWidget()
-        #self.init_serialwidget()
-        #self.networkwidget = QtWidgets.QWidget()        
-        #self.inputtabs.addTab(self.serialwidget,'Serial')
-        #self.inputtabs.addTab(self.networkwidget,'Network')                
-        self.label    = QtWidgets.QLabel("GPS device")
+        self.init_serialwidget()
+        self.label    = QtWidgets.QLabel("Serial device")
         #self.startbtn = QtWidgets.QPushButton("Open device")
         #self.startbtn.clicked.connect(self.start_clicked)
         #self.stopbtn = QtWidgets.QPushButton("Close device")
         #self.stopbtn.clicked.connect(self.stop_clicked)
         layout.addWidget(self.label)        
-        #layout.addWidget(self.inputtabs)
+        layout.addWidget(self.serialwidget)
         #layout.addWidget(self.startbtn)
         #layout.addWidget(self.stopbtn)
-
+        
     def init_serialwidget(self):
         """Fills the serial widget with content
         """
         layout = QtWidgets.QGridLayout(self.serialwidget)
         # Serial baud rates
         baud = [300,600,1200,2400,4800,9600,19200,38400,57600,115200,576000,921600]
         self._combo_serial_devices = QtWidgets.QComboBox()
         #self._combo_serial_devices.currentIndexChanged.connect(self._serial_device_changed)
         self._combo_serial_baud = QtWidgets.QComboBox()
         for b in baud:
             self._combo_serial_baud.addItem(str(b))
 
         self._combo_serial_baud.setCurrentIndex(4)
+        # creating a line edit
+        edit = QtWidgets.QLineEdit(self)
+        onlyInt = QtGui.QIntValidator()
+        edit.setValidator(onlyInt)
+  
+        # setting line edit
+        self._combo_serial_baud.setLineEdit(edit)
+        
+        self._combo_parity = QtWidgets.QComboBox()
+        self._combo_parity.addItem('None')
+        self._combo_parity.addItem('Odd')
+        self._combo_parity.addItem('Even')
+        self._combo_parity.addItem('Mark')
+        self._combo_parity.addItem('Space')
+        
+        self._combo_stopbits = QtWidgets.QComboBox()
+        self._combo_stopbits.addItem('1')
+        self._combo_stopbits.addItem('1.5')
+        self._combo_stopbits.addItem('2')
+        
+        self._combo_databits = QtWidgets.QComboBox()
+        self._combo_databits.addItem('8')
+        self._combo_databits.addItem('7')
+        self._combo_databits.addItem('6')
+        self._combo_databits.addItem('5')
+        
         self._button_serial_openclose = QtWidgets.QPushButton('Open')
         self._button_serial_openclose.clicked.connect(self.start_clicked)
 
 
         # Check for serial devices and list them
         for comport in serial.tools.list_ports.comports():
             self._combo_serial_devices.addItem(str(comport.device))
 
-        layout.addWidget(self._combo_serial_devices,0,0)
-        layout.addWidget(self._combo_serial_baud,0,1)
-        layout.addWidget(self._button_serial_openclose,0,2)            
+        #How to differentiate packets
+        self._packet_ident_lab = QtWidgets.QLabel('Packet identification')
+        self._packet_ident     = QtWidgets.QComboBox()
+        self._packet_ident.addItem('newline \\n')
+        self._packet_ident.addItem('newline \\r\\n')
+        self._packet_ident.addItem('None')
+        # Max packetsize
+        self._packet_size_lab   = QtWidgets.QLabel("Maximum packet size")
+        self._packet_size_lab.setToolTip('The number of received bytes after which a packet is sent.\n Add 0 for no size check')
+        onlyInt = QtGui.QIntValidator()
+        self._packet_size       = QtWidgets.QLineEdit()
+        self._packet_size.setValidator(onlyInt)
+        self._packet_size.setText('0')
+        #self.packet_ident
+
+        layout.addWidget(self._packet_ident,0,1)
+        layout.addWidget(self._packet_ident_lab,0,0)
+        layout.addWidget(self._packet_size_lab,0,2)
+        layout.addWidget(self._packet_size,0,3)
+        layout.addWidget(QtWidgets.QLabel('Serial device'),1,0)
+        layout.addWidget(self._combo_serial_devices,2,0)
+        layout.addWidget(QtWidgets.QLabel('Baud'),1,1)
+        layout.addWidget(self._combo_serial_baud,2,1)
+        layout.addWidget(QtWidgets.QLabel('Parity'),1,2)  
+        layout.addWidget(self._combo_parity,2,2) 
+        layout.addWidget(QtWidgets.QLabel('Databits'),1,3)  
+        layout.addWidget(self._combo_databits,2,3) 
+        layout.addWidget(QtWidgets.QLabel('Stopbits'),1,4)  
+        layout.addWidget(self._combo_stopbits,2,4) 
+        layout.addWidget(self._button_serial_openclose,2,5)
+
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update_buttons)
+        self.statustimer.start(500)
+        
+    
+    def update_buttons(self):
+        """ Updating all buttons depending on the thread status (if its alive, graying out things)
+        """
+
+        status = self.device.get_thread_status()
+        thread_status = status['thread_status']
+
+        if(thread_status):
+            self._button_serial_openclose.setText('Close')
+            self._combo_serial_baud.setEnabled(False)
+            self._combo_serial_devices.setEnabled(False)
+        else:
+            self._button_serial_openclose.setText('Open')
+            self._combo_serial_baud.setEnabled(True)
+            self._combo_serial_devices.setEnabled(True)
+        
             
     def start_clicked(self):
-        button = self.sender()
+        #print('Start clicked')
+        button = self._button_serial_openclose
+        #print('Start clicked:' + button.text())
+        #config_template['comport'] = {'type': 'str'}
+        #config_template['baud'] = {'type': 'int', 'default': 4800}
+        #config_template['parity'] = {'type': 'int', 'default': serial.PARITY_NONE}
+        #config_template['stopbits'] = {'type': 'int', 'default': serial.STOPBITS_ONE}
+        #config_template['bytesize'] = {'type': 'int', 'default': serial.EIGHTBITS}
+        #config_template['dt_poll'] = {'type': 'float', 'default': 0.05}
+        #config_template['chunksize'] = {'type': 'int',
+        #                                'default': 1000}  # The maximum amount of bytes read with one chunk
+        #config_template['packetdelimiter'] = {'type': 'str',
+        #                                      'default': '\n'}  # The maximum amount of bytes read with one chunk
         if('Open' in button.text()):
             button.setText('Close')
             serial_name = str(self._combo_serial_devices.currentText())
             serial_baud = int(self._combo_serial_baud.currentText())
-            #self.device.open_serial_device(serial_name,serial_baud)
-            self.device.serial_name = serial_name
-            self.device.baud = serial_baud
-            self.device_start.emit(self.device)
+            self.device.config['comport'].data = serial_name
+            self.device.config['baud'].data = serial_baud
+            stopbits = self._combo_stopbits.currentText()
+            if(stopbits=='1'):
+                self.device.config['stopbits'].data =  serial.STOPBITS_ONE
+            elif(stopbits=='1.5'):
+                self.device.config['stopbits'].data =  serial.STOPBITS_ONE_POINT_FIVE
+            elif(stopbits=='2'):
+                self.device.config['stopbits'].data =  serial.STOPBITS_TWO
+                
+            databits = int(self._combo_databits.currentText())
+            self.device.config['bytesize'].data = databits
+
+            parity = self._combo_parity.currentText()
+            if(parity=='None'):
+                self.device.config['parity'] = serial.PARITY_NONE
+            elif(parity=='Even'):                
+                self.device.config['parity'] = serial.PARITY_EVEN
+            elif(parity=='Odd'):                
+                self.device.config['parity'] = serial.PARITY_ODD
+            elif(parity=='Mark'):                
+                self.device.config['parity'] = serial.PARITY_MARK
+            elif(parity=='Space'):                
+                self.device.config['parity'] = serial.PARITY_SPACE
+                
+
+            self.device.thread_start()
         else:
             self.stop_clicked()
 
     def stop_clicked(self):
-        button = self.sender()        
-        self.device_stop.emit(self.device)
-        button.setText('Open')        
+        button = self._button_serial_openclose
+        self.device.thread_stop()
+        button.setText('Closing') 
+        #self._combo_serial_baud.setEnabled(True)
+        #self._combo_serial_devices.setEnabled(True)      
 
 
 
 class displayDeviceWidget(QtWidgets.QWidget):
-    def __init__(self):
+    def __init__(self,device=None):
         super(QtWidgets.QWidget, self).__init__()
         layout        = QtWidgets.QVBoxLayout(self)
-        hlayout        = QtWidgets.QHBoxLayout(self)
+        hlayout        = QtWidgets.QHBoxLayout()
+        self.device = device
+        self.bytes_read = QtWidgets.QLabel('Bytes read: ')
+        self.lines_read = QtWidgets.QLabel('Lines read: ')
         self.text     = QtWidgets.QPlainTextEdit(self)
         self.text.setReadOnly(True)
         self.text.setMaximumBlockCount(10000)
-        self.scrollchk= QtWidgets.QCheckBox('Scroll to end')        
-        self.posstatus= QtWidgets.QPushButton('Position')
-        self.posstatus.setStyleSheet("background-color: red")
-        self.datestatus= QtWidgets.QPushButton('Date')
-        self.datestatus.setStyleSheet("background-color: red")
-        self.timestatus= QtWidgets.QPushButton('Time')
-        self.timestatus.setStyleSheet("background-color: red")
-        hlayout.addWidget(self.posstatus)
-        hlayout.addWidget(self.timestatus)
-        hlayout.addWidget(self.datestatus)
+        hlayout.addWidget(self.bytes_read)
+        hlayout.addWidget(self.lines_read)
         layout.addLayout(hlayout)
-        hlayout.addWidget(self.scrollchk)        
         layout.addWidget(self.text)
-        self.goodpos = -1
 
     def update(self,data):
         #print('data',data)
-        prev_cursor = self.text.textCursor()
-        pos = self.text.verticalScrollBar().value()
-        self.text.moveCursor(QtGui.QTextCursor.End)        
-        self.text.insertPlainText(str(data['nmea']))
-        if(self.scrollchk.isChecked()):
-            self.text.verticalScrollBar().setValue(self.text.verticalScrollBar().maximum())
-        else:
-            self.text.verticalScrollBar().setValue(pos)        
-        if('lon' in data.keys()):
-            self.goodpos = time.time()
-            if(data['lon'] == None):
-                self.posstatus.setStyleSheet("background-color: yellow")
-                posstr = "Position, Lat: NA Lon: NA"
-                self.posstatus.setText(posstr)
-            else:
-                posstr = "Position, Lat: {:.4f} Lon: {:.4f}".format(data['lat'],data['lon'])
-                #print(posstr) 
-                self.posstatus.setText(posstr)
-                self.posstatus.setStyleSheet("background-color: green")
-                
-        if('time' in data.keys()):
-            self.goodtime = time.time()
-            if(data['time'] == None):
-                self.timestatus.setStyleSheet("background-color: yellow")
-                posstr = "Time: NA"
-                self.timestatus.setText(posstr)
-            else:
-                posstr = "Time: {:s}:{:s}:{:s}".format(data['time'][0:2],data['time'][2:4],data['time'][4:])
-                #print(posstr) 
-                self.timestatus.setText(posstr)
-                self.timestatus.setStyleSheet("background-color: green")
-                
-        if('date' in data.keys()):
-            self.gooddate = time.time()
-            if(data['date'] == None):
-                self.datestatus.setStyleSheet("background-color: yellow")
-                posstr = "Date: NA"
-                self.datestatus.setText(posstr)
-            else:
-                posstr = "Date: {:s}.{:s}.{:s}".format(data['date'][0:2],data['date'][2:4],data['date'][4:])
-                #print(posstr) 
-                self.datestatus.setText(posstr)
-                self.datestatus.setStyleSheet("background-color: green")
-            
-        if((time.time() - self.goodpos)>10):
-            self.posstatus.setStyleSheet("background-color: red")
+        try:
+            bstr = "Bytes read: {:d}".format(data['bytes_read'])
+            lstr = "Sentences read: {:d}".format(data['sentences_read'])
+        except Exception as e:
+            logger.exception(e)
+        try:
+            self.bytes_read.setText(bstr)
+            self.lines_read.setText(lstr)
+            self.text.insertPlainText(str(data['data']))
+            self.text.insertPlainText('\n')
+        except Exception as e:
+            logger.exception(e)
```

### Comparing `redvypr-0.4.4/redvypr/devices/manufacturer/leitenberger/lrcal_Tfluid.py` & `redvypr-0.5.3/redvypr/gui.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,580 +1,730 @@
-"""
-
-Temperature calibration device from Leitenberger
-
-Configuration options for a heatflow device
-
-.. code-block::
-
-- deviceconfig:
-    name: lrTcal
-    loglevel: debug
-  devicemodulename: lrcal_Tfluid
-
-"""
-
-import datetime
-import logging
-import queue
-from PyQt5 import QtWidgets, QtCore, QtGui
+import copy
 import time
-import numpy as np
 import logging
 import sys
 import yaml
-import pyqtgraph
-import serial
+from PyQt5 import QtWidgets, QtCore, QtGui
+from redvypr.device import redvypr_device
+from redvypr.widgets.gui_config_widgets import redvypr_ip_widget, configQTreeWidget, configWidget
+from redvypr.widgets.standard_device_widgets import displayDeviceWidget_standard, redvypr_deviceInitWidget
+from redvypr.widgets.datastream_widget import datastreamWidget
+import redvypr.configdata
+import redvypr.files as files
+import redvypr.data_packets as data_packets
+import redvypr.device as device
 
-description = 'Interface for the Leitenberger temperature calibration device'
+_logo_file = files.logo_file
+_icon_file = files.icon_file
 
-pyqtgraph.setConfigOption('background', 'w')
-pyqtgraph.setConfigOption('foreground', 'k')
 
 logging.basicConfig(stream=sys.stderr)
-logger = logging.getLogger('lrcal_Tfluid')
+logger = logging.getLogger('redvypr')
 logger.setLevel(logging.DEBUG)
 
-class datadisplay(QtWidgets.QWidget):
-    """ A class that displays a number together with a title
+class LineEditFocus(QtWidgets.QLineEdit):
+    focusInSignal = QtCore.pyqtSignal()
+    focusOutSignal = QtCore.pyqtSignal()
+    def focusInEvent(self, event):
+        # do custom stuff
+        self.focusInSignal.emit()
+        super(LineEditFocus, self).focusInEvent(event)
+
+    def focusOutEvent(self, event):
+        # do custom stuff
+        self.focusOutSignal.emit()
+        super(LineEditFocus, self).focusOutEvent(event)
+
+def get_QColor(data):
+    funcname = __name__ + '.get_QColor():'
+    if(type(data.data) == str):
+        color = QtGui.QColor(data.data)
+    else:
+        colors = data.data
+        color = QtGui.QColor(colors['r'].data, colors['g'].data, colors['b'].data)
+
+    return color
+
+class redvyprDeviceWidget(QtWidgets.QWidget):
+    """ A widget that lists all devices found in modules and in the python files included in the path list.
     """
-    def __init__(self,title=''):
-        super(QtWidgets.QWidget, self).__init__()
-        layout        = QtWidgets.QVBoxLayout(self)
-        self.titlestr = title
-        self.title    = QtWidgets.QLabel(self.titlestr)
-        self.data     = QtWidgets.QLabel('no data')
-        fsize         = self.data.fontMetrics().size(0, self.data.text())
-        self.data.setFont(QtGui.QFont('Arial', fsize.height()+10))
-        layout.addWidget(self.title)
-        layout.addWidget(self.data)
-
-    def set_data(self,data):
-        newdatastr = "{:.2f}".format(data) # TODO, here a format string defined in the widget could be applied
-        self.data.setText(newdatastr)
-  
-        
+    def __init__(self, redvypr_device_scan=None,redvypr=None):
+        """
 
+        Args:
+            redvypr:
+            device:
+        """
+        super(redvyprDeviceWidget, self).__init__()
+        self.redvypr = redvypr
+        if redvypr is not None:
+            self.redvypr_device_scan = redvypr.redvypr_device_scan
+        elif (redvypr_device_scan is not None):
+            self.redvypr_device_scan = redvypr_device_scan
+        else:
+            self.redvypr_device_scan = device.redvypr_device_scan()
 
+        # Update the devicetree
+        self.create_tree_widget()
+        self.update_tree_widget()
+        self.create_deviceinfo_widget()
+        # Create widgets for adding/removing devices
+        self.addbtn = QtWidgets.QPushButton('Add')
+        self.addbtn.clicked.connect(self.add_device_click)
+        self.devnamelabel = QtWidgets.QLabel('Devicename')
+        self.devname = QtWidgets.QLineEdit()
+        self.mp_label = QtWidgets.QLabel('Multiprocessing options')
+        self.mp_thread = QtWidgets.QRadioButton('Thread')
+        self.mp_multi = QtWidgets.QRadioButton('Multiprocessing')
+        self.mp_multi.setChecked(True)
+        self.mp_group = QtWidgets.QButtonGroup()
+        self.mp_group.addButton(self.mp_thread)
+        self.mp_group.addButton(self.mp_multi)
+
+        self.layout = QtWidgets.QFormLayout(self)
+        self.layout.addRow(self.devicetree)
+        self.layout.addRow(self.deviceinfo)
+        self.layout.addRow(self.mp_label)
+        self.layout.addRow(self.mp_thread, self.mp_multi)
+        self.layout.addRow(self.devnamelabel, self.devname)
+        self.layout.addRow(self.addbtn)
 
+        self.setWindowIcon(QtGui.QIcon(_icon_file))
+        self.setWindowTitle("redvypr devices")
 
+    def create_deviceinfo_widget(self):
+        """
+        Creates a widget that shows the device information
+        Returns:
 
-def start(datainqueue,dataqueue,comqueue,devicename,config={}):
-    funcname = __name__ + '.start()'
-    chunksize = 1000 # The maximum amount of bytes read with one chunk
-    logger.debug(funcname + ':Starting reading serial data')        
-    nmea_sentence = ''
-    sentences = 0
-    bytes_read = 0
-    ttest = time.time()
-    serial_device = False
-    
-    try:
-        serial_name = config['serial_name']
-    except:
-        serial_name = 'NaN'
-    try:
-        baud = config['baud']
-    except:
-        baud = 9600
-    try:
-        parity=config['parity']
-    except:
-        parity=serial.PARITY_NONE
-    try:
-        stopbits=config['stopbits']
-    except:
-        stopbits=serial.STOPBITS_ONE
-    try:
-        bytesize= config['bytesize']
-    except: 
-        bytesize=serial.EIGHTBITS
-    
-    try:
-        max_size = config['max_size']
-    except:
-        max_size=10000
-        
-    try:
-        dt = config['dt']
-    except:
-        dt = 2.0
-        
-    if True:
-        try:
-            ser = serial.Serial(serial_name,baud,parity=parity,stopbits=stopbits,bytesize=bytesize,timeout=0.1)
-        except Exception as e:
-            logger.debug(funcname + ': Exception open_serial_device {:s} {:d}: '.format(serial_name,baud) + str(e))
-            return False
-        
-    try:
-        datakey = config['datakey']
-    except:
-        datakey = 'data'  
-        
-    while True:
-        t0 = time.time()
-        try:
-            com = comqueue.get(block=False)
-            logger.debug(funcname + ': received command {:s}'.format(str(com)))
-            logger.info(funcname + ': received command {:s}'.format(str(com)))
-            if(com == 'stop'):
-                break
-            elif(type(com) == dict):
-                logger.debug(funcname + ': Dictionary')
-                if('set' in com.keys()): # Set a new temperature
-                    logger.debug(funcname + ': Dictionary set')                    
-                    T = com['set']
-                    try:
-                        Tstr = "{:2.1f}".format(T).replace('.',',').encode('UTF-8')
-                        com = b'$1WVAR0 ' + Tstr + b'\r'
-                        logger.debug(funcname + ' Writing command: {:s}'.format(str(com)))
-                        ser.write(com) # write a string
-                        s = ser.read(100)
-                        print(s)
-                    except Exception as e:
-                        logger.debug(funcname + ': Could not write command because of: {:s}'.format(str(e)))
-        except:
-            pass
+        """
+        self.deviceinfo = QtWidgets.QWidget()  #
+        self.deviceinfo_layout = QtWidgets.QFormLayout(self.deviceinfo)
+        self.__devices_info_sourcelabel2 = QtWidgets.QLabel()
+        self.__devices_info_sourcelabel4 = QtWidgets.QLabel()
+        self.__devices_info_sourcelabel6 = QtWidgets.QLabel()
+        self.deviceinfo_layout.addRow(QtWidgets.QLabel('Name'),self.__devices_info_sourcelabel2)
+        self.deviceinfo_layout.addRow(QtWidgets.QLabel('Source'),self.__devices_info_sourcelabel4)
+        self.deviceinfo_layout.addRow(QtWidgets.QLabel('Description'),self.__devices_info_sourcelabel6)
 
+    def create_tree_widget(self):
+        """
+        Creates the QtreeWidget with the
+        Returns:
 
-        datadict = {}        
-        # Read T set
-        com = b'$1RVAR0 \r'
-        #print(com)
-        ser.write(com) # write a string
-        s = ser.read(100)
-        #print(s)
-        # Parse the result (should look like this: b'*1 +0015.00\r'
-        sstr = s.decode()
-        #print(sstr)
-        if('*1' in sstr):
+        """
+        self.devicetree = QtWidgets.QTreeWidget()  # All dataproviding devices
+        self.devicetree.setColumnCount(1)
+        #self.devicetree.setHeaderHidden(True)
+        self.devicetree.setHeaderLabels(['Device'])
+        self.devicetree.currentItemChanged.connect(self.__item_changed__)
+        self.devicetree.itemDoubleClicked.connect(self.__apply_item__)
+        self.devicetree.setSortingEnabled(True)
+
+    def update_tree_widget(self):
+        self.devicetree.clear()
+        root = self.devicetree.invisibleRootItem()
+        #moduleroot = QtWidgets.QTreeWidgetItem(['modules', ''])
+        #root.addChild(moduleroot)
+        def update_recursive(moddict,parentitem):
             try:
-                Tset = sstr.split(' ')[1][:-1]
-                Tset = float(Tset)
-            except Exception as e:
-                logger.debug(funcname + ':' + str(e))
-                Tset = np.NaN
+                keys = moddict.keys()
+            except:
+                keys = None
+
+            if(keys is None):
+                return
+            else:
+                for k in moddict.keys():
+                    if(k == '__devices__'): # List of devices in the module
+                        for devdict in moddict[k]:
+                            devicename = devdict['name']
+                            #print('devdict',devdict)
+                            # remove trailing modules separated by '.'
+                            devicename = devicename.split('.')[-1]
+                            itm = QtWidgets.QTreeWidgetItem([devicename, ''])
+                            itm.devdict = devdict # Add device information
+                            parentitem.addChild(itm)
+                    else:
+                        # remove trailing modules separated by '.'
+                        if '/' in k: # Check if its a path or a module file
+                            ktxt = k
+                        else:
+                            ktxt = k.split('.')[-1]
+
+                        itm = QtWidgets.QTreeWidgetItem([ktxt, ''])
+                        itm.devdict = None # Not a device
+                        parentitem.addChild(itm)
+                        update_recursive(moddict[k],itm)
+
+        #update_recursive(self.redvypr_device_scan.redvypr_devices['modules'],moduleroot)
+        update_recursive(self.redvypr_device_scan.redvypr_devices, root)
+
+
+        self.devicetree.expandAll()
+        self.devicetree.resizeColumnToContents(0)
+        self.devicetree.sortByColumn(0, QtCore.Qt.AscendingOrder)
+
+    def __item_changed__(self, new, old):
+        print('Item changed')
+        print('new',new,old)
+        if new.devdict is not None:
+            self.__update_device_info__(new.devdict)
+            self.addbtn.setEnabled(True)
+        else:
+            self.addbtn.setEnabled(False)
 
-            datadict['Tset'] = Tset
 
-            
-        com = b'$1RVAR100 \r'
-        #print('Reading bath temperature',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Parse the result (should look like this: b'*1 +0015.00\r'
-        sstr = s.decode()
-        #print(sstr)
-        if('*1' in sstr):
-            try:
-                Tbath = sstr.split(' ')[1][:-1]
-                Tbath = float(Tbath)
-            except Exception as e:
-                logger.debug(funcname + ':' + str(e))
-                Tbath = np.NaN
-
-            datadict['Tbath'] = Tbath
-
-        # Title
-        com = b'$1RVAR9 \r'
-        #print('Reading title',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Unit
-        com = b'$1RVAR10 \r'
-        #print('Reading unit',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Serial number
-        com = b'$1RVAR16 \r'
-        #print('Reading serial number',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Min set point
-        com = b'$1RVAR17 \r'
-        #print('Reading min set point',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Max set point
-        com = b'$1RVAR18 \r'
-        #print('Reading max set point',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        
-        # Stability range
-        com = b'$1RVAR28 \r'
-        #print('Stability range',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)
-        # Symbol of steadiness
-        com = b'$1RVAR29 \r'
-        #print('Steadiness',com)
-        ser.write(com)     # write a string
-        #time.sleep(0.1)
-        s = ser.read(100)
-        #print(s)                      
-
-        if(len(datadict.keys())>0):
-            dataqueue.put(datadict)
-
-        t1 = time.time()
-        dt_load = t1 - t0
-        dt_sleep = dt - dt_load
-        if(dt_sleep > 0):
-            time.sleep(dt_sleep)            
-
-class Device():
-    def __init__(self,dataqueue=None,comqueue=None,datainqueue=None,config = {}):
-        """
-        """
-        self.publish     = True # publishes data, a typical device is doing this
-        self.subscribe   = True  # subscribing data, a typical datalogger is doing this
-        self.datainqueue = datainqueue
-        self.dataqueue   = dataqueue        
-        self.comqueue    = comqueue
-        self.config      = config # Please note that this is typically a placeholder, the config structure will be written by redvypr and the yaml
-        self.name        = 'Tfluid' # This will be overwritten by the config!
-                
-    def start(self):
-        start(self.datainqueue,self.dataqueue,self.comqueue,devicename=self.name,config=self.config)
-        
-    def __str__(self):
-        sstr = 'Leitenberger temperature calibration device'
-        return sstr
-    
-    
-    
-class initDeviceWidget(QtWidgets.QWidget):
-    device_start = QtCore.pyqtSignal(Device)
-    device_stop = QtCore.pyqtSignal(Device)        
-    def __init__(self,device=None):
-        super(QtWidgets.QWidget, self).__init__()
-        layout        = QtWidgets.QVBoxLayout(self)
-        self.device   = device
-        self.serialwidget = QtWidgets.QWidget()
-        self.init_serialwidget()
-        self.label    = QtWidgets.QLabel("Leitenberger FLUID100 Calibration setup")
-        #self.startbtn = QtWidgets.QPushButton("Open device")
-        #self.startbtn.clicked.connect(self.start_clicked)
-        #self.stopbtn = QtWidgets.QPushButton("Close device")
-        #self.stopbtn.clicked.connect(self.stop_clicked)
-        layout.addWidget(self.label)        
-        layout.addWidget(self.serialwidget)
-        layout.addStretch()
-        #layout.addWidget(self.startbtn)
-        #layout.addWidget(self.stopbtn)
-        
-    def thread_status(self,status):
-        self.update_buttons(status['threadalive'])
+    def __apply_item__(self):
+        print('Apply')
 
-    def init_serialwidget(self):
-        """Fills the serial widget with content
+    def __update_device_info__(self,devdict):
+        """ Populates the self.__devices_info widget with the info of the module
         """
-        layout = QtWidgets.QGridLayout(self.serialwidget)
-        # Serial baud rates
-        baud = [300,600,1200,2400,4800,9600,19200,38400,57600,115200,576000,921600]
-        self._combo_serial_devices = QtWidgets.QComboBox()
-        #self._combo_serial_devices.currentIndexChanged.connect(self._serial_device_changed)
-        self._combo_serial_baud = QtWidgets.QComboBox()
-        for b in baud:
-            self._combo_serial_baud.addItem(str(b))
-
-        self._combo_serial_baud.setCurrentIndex(5)
-        # creating a line edit
-        edit = QtWidgets.QLineEdit(self)
-        onlyInt = QtGui.QIntValidator()
-        edit.setValidator(onlyInt)
-  
-        # setting line edit
-        self._combo_serial_baud.setLineEdit(edit)
-        
-        self._combo_parity = QtWidgets.QComboBox()
-        self._combo_parity.addItem('None')
-        self._combo_parity.addItem('Odd')
-        self._combo_parity.addItem('Even')
-        self._combo_parity.addItem('Mark')
-        self._combo_parity.addItem('Space')
-        
-        self._combo_stopbits = QtWidgets.QComboBox()
-        self._combo_stopbits.addItem('1')
-        self._combo_stopbits.addItem('1.5')
-        self._combo_stopbits.addItem('2')
-        
-        self._combo_databits = QtWidgets.QComboBox()
-        self._combo_databits.addItem('8')
-        self._combo_databits.addItem('7')
-        self._combo_databits.addItem('6')
-        self._combo_databits.addItem('5')
-        
-        self._button_serial_openclose = QtWidgets.QPushButton('Open')
-        self._button_serial_openclose.clicked.connect(self.start_clicked)
+        infotxt = devdict['name']
+        self.__devices_info_sourcelabel2.setText(infotxt)
+        infotxt2 = devdict['file']
+        self.__devices_info_sourcelabel4.setText(infotxt2)
+        try:
+            desctxt = devdict['module'].description
+        except Exception as e:
+            desctxt = ''
 
+        self.__devices_info_sourcelabel6.setText(desctxt)
 
-        # Check for serial devices and list them
-        for comport in serial.tools.list_ports.comports():
-            self._combo_serial_devices.addItem(str(comport.device))
-
-        layout.addWidget(QtWidgets.QLabel('Serial device'),1,0)
-        layout.addWidget(self._combo_serial_devices,2,0)
-        layout.addWidget(QtWidgets.QLabel('Baud'),1,1)
-        layout.addWidget(self._combo_serial_baud,2,1)
-        layout.addWidget(QtWidgets.QLabel('Parity'),1,2)  
-        layout.addWidget(self._combo_parity,2,2) 
-        layout.addWidget(QtWidgets.QLabel('Databits'),1,3)  
-        layout.addWidget(self._combo_databits,2,3) 
-        layout.addWidget(QtWidgets.QLabel('Stopbits'),1,4)  
-        layout.addWidget(self._combo_stopbits,2,4) 
-        layout.addWidget(self._button_serial_openclose,2,5)
+    def __device_name(self):
+        devicemodulename = self.__devices_list.currentItem().text()
+        devicename = devicemodulename + '_{:d}'.format(self.redvypr.numdevice + 1)
+        self.__devices_devname.setText(devicename)
+        self.__device_info()
 
-        
-    
-    def update_buttons(self,thread_status):
-        """ Updating all buttons depending on the thread status (if its alive, graying out things)
+    def add_device_click(self):
         """
-        if(thread_status):
-            self._button_serial_openclose.setText('Close')
-            self._combo_serial_baud.setEnabled(False)
-            self._combo_serial_devices.setEnabled(False)
-        else:
-            self._button_serial_openclose.setText('Open')
-            self._combo_serial_baud.setEnabled(True)
-            self._combo_serial_devices.setEnabled(True)
-        
-            
-    def start_clicked(self):
-        #print('Start clicked')
-        button = self._button_serial_openclose
-        #print('Start clicked:' + button.text())
-        if('Open' in button.text()):
-            button.setText('Close')
-            serial_name = str(self._combo_serial_devices.currentText())
-            serial_baud = int(self._combo_serial_baud.currentText())
-            stopbits = self._combo_stopbits.currentText()
-            if(stopbits=='1'):
-                self.device.stopbits =  serial.STOPBITS_ONE
-            elif(stopbits=='1.5'):
-                self.device.stopbits =  serial.STOPBITS_ONE_POINT_FIVE
-            elif(stopbits=='2'):
-                self.device.config['stopbits'] =  serial.STOPBITS_TWO
-                
-            databits = int(self._combo_databits.currentText())
-            self.device.config['bytesize'] = databits
-
-            parity = self._combo_parity.currentText()
-            if(parity=='None'):
-                self.device.config['parity'] = serial.PARITY_NONE
-            elif(parity=='Even'):                
-                self.device.config['parity'] = serial.PARITY_EVEN
-            elif(parity=='Odd'):                
-                self.device.config['parity'] = serial.PARITY_ODD
-            elif(parity=='Mark'):                
-                self.device.config['parity'] = serial.PARITY_MARK
-            elif(parity=='Space'):                
-                self.device.config['parity'] = serial.PARITY_SPACE
-                
-            self.device.config['serial_name'] = serial_name
-            self.device.config['baud'] = serial_baud
-            self.device_start.emit(self.device)
+        """
+        funcname = __name__ + 'add_device_click():'
+        logger.debug(funcname)
+        getSelected = self.devicetree.selectedItems()
+        if getSelected:
+            item = getSelected[0]
+
+        if item.devdict is not None:
+            devicemodulename = item.devdict['name']
+            thread = self.mp_thread.isChecked()
+            config = {'loglevel':logger.level}
+            devname = str(self.devname.text())
+            if len(devname) > 0:
+                config['name'] = devname
+            deviceconfig = {'config':config}
+            print('devicemodulename',devicemodulename)
+            print('Adding device, config',deviceconfig)
+            if self.redvypr is not None:
+                self.redvypr.add_device(devicemodulename=devicemodulename, thread=thread, deviceconfig=deviceconfig)
+            self.devname.clear()
+            # Update the name
+            #self.__device_name()
         else:
-            self.stop_clicked()
+            print('Not a device')
 
-    def stop_clicked(self):
-        #print('Stop clicked')
-        button = self._button_serial_openclose
-        self.device_stop.emit(self.device)
-        button.setText('Closing') 
-        #self._combo_serial_baud.setEnabled(True)
-        #self._combo_serial_devices.setEnabled(True)      
 
 
-class displayDeviceWidget(QtWidgets.QWidget):
-    """ Widget is showing temperature calibration data
+class redvyprSubscribeWidget(QtWidgets.QWidget):
+    """ A widget that lists all devices and datastreams as potential inputs and a second list of all the subscriptions
+     of the
+
     """
-    def __init__(self,dt_update = 0.5,device=None,buffersize=1000,tabwidget=None):
-        funcname = __name__ + '.init()'
-        super(QtWidgets.QWidget, self).__init__()
-        self.layout_plot  = QtWidgets.QGridLayout(self)
+
+    def __init__(self, redvypr=None, device=None):
+        """
+
+        Args:
+            redvypr:
+            device:
+        """
+        super(redvyprSubscribeWidget, self).__init__()
+        self.redvypr = redvypr
+        self.devices = self.redvypr.devices
+        self.redvypr.devices_connected.connect(self.__devices_connected__)
+        self.redvypr.devices_disconnected.connect(self.__devices_connected__)
+        self.redvypr.device_status_changed_signal.connect(self.__devices_connected__)
+        if (len(self.devices) > 0):
+            if (device == None):  # Take the first one
+                device = self.devices[0]['device']
+
+        # Set icon
+        self.setWindowIcon(QtGui.QIcon(_icon_file))
+        self.setWindowTitle("redvypr subscribe")
+        layout = QtWidgets.QGridLayout(self)
+
+        font = QtGui.QFont('Arial', 20)
+        font.setBold(True)
+
+        lab = QtWidgets.QLabel('Device subscriptions')
+        lab.setFont(font)
+        lab.setAlignment(QtCore.Qt.AlignCenter)
+
+        self.device_label = QtWidgets.QLabel('Device')
+        self.device_label.setAlignment(QtCore.Qt.AlignCenter)
+        self.dataprovider_label = QtWidgets.QLabel('Data providing devices')
+        self.dataprovider_label.setAlignment(QtCore.Qt.AlignCenter)
+        self.subscribe_label = QtWidgets.QLabel('Subscribed')
+        self.subscribe_label.setAlignment(QtCore.Qt.AlignCenter)
+
+        self.devices_listallout = QtWidgets.QTreeWidget()  # All dataproviding devices
+        self.devices_listallout.setColumnCount(2)
+        self.devices_listallout.setHeaderHidden(True)
+        self.devices_listallout.currentItemChanged.connect(self.__update_device_choice__)
+
+        self.devices_listcon = QtWidgets.QListWidget()  # The devices a connection is to be defined
+        self.devices_listcon.itemClicked.connect(self.itemcon_clicked)
+        self.devices_listcon.itemDoubleClicked.connect(self.itemcon_dclicked)
+
+        self.devices_listallsub = QtWidgets.QListWidget()  # The subscriptions of the device
+        self.devices_listallsub.itemClicked.connect(self.__itemsubscribed_clicked__)
+
+        self.subscribe_edit = LineEditFocus()
+        self.subscribe_edit.focusInSignal.connect(self.__focus_in__)
+        self.subscribe_edit.focusOutSignal.connect(self.__focus_out__)
+
+        self.__commitbtn = QtWidgets.QPushButton('Subscribe')
+        self.__commitbtn.clicked.connect(self.commit_clicked)
+        self.__commitbtn.setEnabled(False)
+
+        #layout.addWidget(lab, 0, 1,1,3)
+        layout.addWidget(lab, 0, 0,1,3)
+        layout.addWidget(self.device_label, 1, 0)
+        layout.addWidget(self.devices_listcon, 2, 0)
+        layout.addWidget(self.subscribe_label, 1, 1)
+        layout.addWidget(self.devices_listallsub, 2, 1)
+        layout.addWidget(self.dataprovider_label, 1, 2)
+        layout.addWidget(self.devices_listallout, 2, 2)
+        layout.addWidget(self.subscribe_edit, 3, 0, 1, 3)
+        layout.addWidget(self.__commitbtn,4,0,1,3)
+
+        if (len(self.devices) > 0):
+            self.update_list(device)
+
+    def __itemsubscribed_clicked__(self,item):
+        self.__commitbtn.setText('Remove')
+        self.__commitbtn.setEnabled(True)
+        self.__commitbtn.__status__ = 'remove'
+        self.__commitbtn.redvypr_addr_remove = item.redvypr_addr
+
+    def __focus_in__(self):
+        self.__commitbtn.setText('Subscribe')
+        self.__commitbtn.__status__ = 'add'
+        self.__commitbtn.setEnabled(True)
+
+    def __focus_out__(self):
+        pass
+
+    def __devices_connected__(self, dev1=None, dev2=None):
+        #print('Devices have been connected',dev1,dev2)
+        self.update_list(self.device)
+
+    def __update_device_choice__(self,newitem,olditem):
+        """
+        A device was clicked, update all buttons
+        Args:
+            item:
+
+        Returns:
+
+        """
+        if newitem is not None:
+            devstr = newitem.redvypr_address.get_str()
+
+            try:
+                subscribed = newitem.subscribed
+            except:
+                subscribed = False
+
+            if(subscribed):
+                self.__commitbtn.setText('Unsubscribe')
+                self.__commitbtn.__status__ = 'remove'
+                self.__commitbtn.setEnabled(True)
+                self.__commitbtn.redvypr_addr_remove = devstr
+            else:
+                self.subscribe_edit.setText(devstr)
+                print(devstr)
+                print('Item',newitem.text(0))
+                self.__commitbtn.setText('Subscribe')
+                self.__commitbtn.__status__ = 'add'
+                self.__commitbtn.setEnabled(True)
+        else:
+            self.__commitbtn.setEnabled(False)
+
+    def update_list(self, device):
+        """ Update the list
+        """
+
+        funcname = __name__ + '.update_list()'
+        try:
+            devname = device.name
+        except:
+            devname = 'NA'
+        logger.debug(funcname + ':update_list for device: {:s}, name {:s}'.format(str(device),devname))
+        self.devices_listallout.clear()
+        self.devices_listallsub.clear()
+        self.devices_listcon.clear()
         self.device = device
-        self.tabname = 'Data'        
-        self.dt_update = dt_update
-        self.buffersizestd = buffersize
-        
-        config = {'dt_update':self.dt_update,'last_update':time.time()}
-        self.config = config
-        # 
-        self.create_plotwidget()
-
-
-    def create_plotwidget(self):
-        funcname = __name__ + '.create_dataplotwidget()'
-        # Add axes to the widget
-        logger.debug(funcname )
-        # The axes
-        title = 'LR Cal'
-        location = [2,0]
-        whichwidget = 0
-        datetick = True
-        ylabel = 'T [°C]'
-        # The line to plot
-        buffersize = self.buffersizestd
-        xdata = np.zeros(buffersize) * np.NaN
-        ydata = np.zeros(buffersize) * np.NaN
-        xdata2 = np.zeros(buffersize) * np.NaN
-        ydata2 = np.zeros(buffersize) * np.NaN        
-        name = 'LR cal'
-        lineplot = pyqtgraph.PlotDataItem( name = 'T bath' )
-        lineplot2 = pyqtgraph.PlotDataItem( name = 'T set' )
-        linewidth = 1
-        color = QtGui.QColor(255,10,10)
-        x = 't'
-        y = 'hfV'
-        if True:
-            plot = pyqtgraph.PlotWidget(title=title)
-            axis = pyqtgraph.DateAxisItem(orientation='bottom')
-            plot.setAxisItems({"bottom": axis})
-            plot.setLabel('left', ylabel )
-            plot_dict = {'widget':plot,'lines':{}}
-            # Add a lines with the actual data to the graph
+
+        if (len(self.devices) > 0):
+            root = self.devices_listallout.invisibleRootItem()
+            # self.devices_listcon.addItem(str(device))
+            data_provider_all = self.redvypr.get_devices(publishes=True)
+            font1 = QtGui.QFont('Arial')
+            font1.setBold(True)
+            font0 = QtGui.QFont('Arial')
+
+
+            # Fill the qtreewidget
+            #print('data provider',data_provider_all)
+            if (data_provider_all is not None):
+                for dev in data_provider_all:
+                    if dev == self.device:
+                        continue
+
+                    # Check if the device is already subscribed
+                    subscribed = False
+                    #print('dev',dev.name,dev.redvypr.hostinfo)
+                    for a in self.device.subscribed_addresses:
+                        subscribed = a in dev.address
+                        if subscribed:
+                            break
+
+                    itm = QtWidgets.QTreeWidgetItem([dev.name, ''])
+                    itm.device = dev
+                    itm.redvypr_address = dev.address
+                    if subscribed:
+                        status = 'subscribed'
+                        itm.setFont(0,font1)
+                        itm.subscribed = True
+                    else:
+                        itm.setFont(0, font0)
+                        itm.subscribed = False
+
+                    root.addChild(itm)
+                    # Check for forwarded devices
+                    if True:
+                        devs_forwarded = dev.get_device_info()
+                        for devaddress in devs_forwarded.keys():
+                            devaddress_redvypr = data_packets.redvypr_address(devaddress)
+                            subscribed = False
+                            for a in self.device.subscribed_addresses:
+                                subscribed = a in devaddress_redvypr
+                                if subscribed:
+                                    break
+
+                            itmf = QtWidgets.QTreeWidgetItem([devaddress, ''])
+                            itmf.device = dev
+                            itmf.redvypr_address = devaddress_redvypr
+                            itmf.address_forwarded = devaddress
+                            if(subscribed):
+                                itmf.setFont(0, font1)
+                                itmf.subscribed = True
+                            else:
+                                itmf.setFont(0, font0)
+                                itmf.subscribed = False
+
+                            itm.addChild(itmf)
+
+            self.devices_listallout.expandAll()
+            self.devices_listallout.resizeColumnToContents(0)
+
+            # Fill list of devices subscribing
+            devitm = None
+            if True:
+                # connecting devices
+                for s in self.devices:
+                    sen = s['device']
+                    itm = QtWidgets.QListWidgetItem(sen.name)
+                    itm.device = sen
+                    self.devices_listcon.addItem(itm)
+                    if (sen == device):
+                        devitm = itm
+
+                if(devitm is not None):
+                    self.devices_listcon.setCurrentItem(devitm)
+
+            # Fill the subscribed list
             if True:
-                # Bath temperature
-                logger.debug(funcname + ':Adding a line to the plot')
-                # Configuration of the line plot
-                linewidth = 2
-                color = QtGui.QColor(255,50,50)
-                lineconfig = {'device':self.device,'x':x,'y':y,'linewidth':linewidth,'color':color}
-                # Add the line and the configuration to the lines list
-                line_dict = {'line':lineplot,'config':lineconfig,'x':xdata,'y':ydata}
-                # The lines are sorted according to the devicenames, each device has a list of lines attached to it
-                plot_dict['lines']['Tbath'] = line_dict
-                plot.addLegend()                
-                plot.addItem(lineplot)
-
-                # The set temperature
-                linewidth = 1
-                color = QtGui.QColor(10,10,10)
-                lineconfig = {'device':self.device,'x':x,'y':y,'linewidth':linewidth,'color':color}
-                # Add the line and the configuration to the lines list
-                line_dict = {'line':lineplot2,'config':lineconfig,'x':xdata2,'y':ydata2}
-                # The lines are sorted according to the devicenames, each device has a list of lines attached to it
-                plot_dict['lines']['Tset'] = line_dict
-                plot.addItem(lineplot2)
-                
-                # Add the line to all plots
-                self.plot = plot_dict
-
-        self.timelabel     = QtWidgets.QLabel('Time')
-        fsize         = self.timelabel.fontMetrics().size(0, self.timelabel.text())
-        self.timelabel.setFont(QtGui.QFont('Arial', fsize.height()+10))
-        self.timelabel.setAlignment(QtCore.Qt.AlignCenter)                        
-        # Add displays
-        self._datadisplays = {}
-        self._datadisplays['Tbath'] = datadisplay(title='T bath')
-        self._datadisplays['Tset'] = datadisplay(title='T set')
-        self._datadisplays['Tseted'] = QtWidgets.QLineEdit()
-        self._datadisplays['Tseted'].setText('18.00')
-        self._datadisplays['Tseted'].setValidator(QtGui.QDoubleValidator())
-        self._datadisplays['Tseted'].setMaxLength(6)
-        self._datadisplays['Tseted'].setAlignment(QtCore.Qt.AlignRight)
-        self._datadisplays['Tsetbut'] = QtWidgets.QPushButton('Set temperature')
-        self._datadisplays['Tsetbut'].clicked.connect(self._set_temp)
-        self.layout_plot.addWidget(self.timelabel,0,0) 
-        self.layout_plot.addWidget(self._datadisplays['Tbath'],1,0)
-        self.layout_plot.addWidget(self._datadisplays['Tset'],1,1)
-        self.layout_plot.addWidget(self._datadisplays['Tseted'],2,0)
-        self.layout_plot.addWidget(self._datadisplays['Tsetbut'],2,1)
-        # Pyqtgraph plot
-        self.layout_plot.addWidget(plot,3,0,1,2)        
+                # connecting devices
+                for s in self.device.subscribed_addresses:
+                    sstr = s.address_str
+                    litm = QtWidgets.QListWidgetItem(sstr)
+                    litm.redvypr_addr = s
+                    self.devices_listallsub.addItem(litm)
+
+    # End update_list()
+    def commit_clicked(self):
+        """ Apply changes to subscribe/unsubscribe
+        """
+        funcname = 'commit_clicked'
+        logger.debug(funcname)
+
+        if (self.device is not None):
+            if self.__commitbtn.__status__ == 'add':
+                address_add = str(self.subscribe_edit.text())
+                if (len(address_add) > 0):
+                    print('Adding', address_add)
+                    self.device.subscribe_address(address_add)
+                    self.update_list(self.device)
+                else:
+                    print('Nothing to add')
+            elif self.__commitbtn.__status__ == 'remove':
+                raddr = self.__commitbtn.redvypr_addr_remove
+                self.device.unsubscribe_address(raddr)
+                self.update_list(self.device)
+
+
+        getSelected = self.devices_listallout.selectedItems()
+        if getSelected:
+            itm = getSelected[0]
+            try:
+                device = itm.device
+                devicename = device.name
+            except:
+                device = None
+                devicename = ''
+
+            # Get subscriber
+            subscriber_item  = self.devices_listcon.currentItem()
+            subscriber = subscriber_item.device
+            try:
+                address_forwarded = itm.address_forwarded
+            except:
+                address_forwarded = None
+
+
+    def disconnect_clicked(self):
+        logger.debug('Disconnect')
+
+    def itemcon_clicked(self, item):
+        # Update the connection list
+        self.update_list(item.device)
+
+    def itemcon_dclicked(self, item):
+        if (item.isSelected()):
+            item.setSelected(False)
+
+class deviceinfoWidget(QtWidgets.QWidget):
+    """ A widget to display the general info of a device
+    """
+    device_start = QtCore.pyqtSignal(dict) # Signal requesting a start of the device (starting the thread)
+    device_stop  = QtCore.pyqtSignal(dict) # Signal requesting a stop of device
+    connect      = QtCore.pyqtSignal(dict) # Signal requesting a change of the connection
+
+    def __init__(self,devicedict,redvyprwidget):
+        super(deviceinfoWidget, self).__init__()
+        self.devicedict = devicedict
+        self.device = devicedict['device']
+        # Connect the status signal
+        self.device.status_signal.connect(self.thread_status)
+        self.redvyprwidget = redvyprwidget
+        self.devicetab = self.redvyprwidget.devicetabs # The parent tab with all devices listed
+        self.namelabel = QtWidgets.QLabel(devicedict['device'].name)
+        label = self.namelabel
+        fsize         = label.fontMetrics().size(0, label.text())
+        label.setFont(QtGui.QFont('Arial', fsize.height()+4))        
+        #self.numlabel = QtWidgets.QLabel(str(devicedict['device'].numdevice))
+        #label = self.numlabel
+        #fsize         = label.fontMetrics().size(0, label.text())
+        #label.setFont(QtGui.QFont('Arial', fsize.height()+4))                
+        self.layout = QtWidgets.QHBoxLayout(self)
+        self.layout2 = QtWidgets.QGridLayout()
+        self.logwidget = QtWidgets.QComboBox() # A Combobox to change the loglevel of the device
+        self.logwidget.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)
+        # Fill the logwidget
+        logger    = self.devicedict['logger']
+        if(logger is not None):
+            level     = logger.getEffectiveLevel()
+            levelname = logging.getLevelName(level)
+            loglevels = ['CRITICAL','ERROR','WARNING','INFO','DEBUG']
+            for i,l in enumerate(loglevels):
+                self.logwidget.addItem(l)
+                    
+            self.logwidget.setCurrentText(levelname)
+        else:
+            self.logwidget.addItem('NA')
+            
+        self.logwidget.currentIndexChanged.connect(self.loglevel_changed)
         
-    def _set_temp(self):
-        """ Temperature set command
+        self.viewbtn = QtWidgets.QPushButton("View")
+        self.viewbtn.clicked.connect(self.viewclicked)
+        self.viewbtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)        
+        self.conbtn = QtWidgets.QPushButton("Connections")
+        self.conbtn.clicked.connect(self.conclicked)
+        self.conbtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)
+        self.rembtn = QtWidgets.QPushButton("Remove")
+        self.rembtn.clicked.connect(self.remdevice)
+        self.rembtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)        
+        self.renbtn = QtWidgets.QPushButton("Rename")
+        self.renbtn.clicked.connect(self.rendevice)
+        self.renbtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)        
+        self.startbtn = QtWidgets.QPushButton("Start")
+        self.startbtn.setCheckable(True)
+        self.startbtn.clicked.connect(self.startstopclicked)
+        self.startbtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)
+        self.infobtn = QtWidgets.QPushButton("Info")
+        self.infobtn.clicked.connect(self.get_info)
+        self.infobtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)
+        #Configuration
+        configlayout = QtWidgets.QVBoxLayout()
+        # Autostart
+        self.autostart = QtWidgets.QPushButton('Autostart')
+        self.autostart.setCheckable(True)
+        self.autostart.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        try: # If the device has an autostart attribute
+            self.autostart.isChecked(self.device.autostart)
+        except:
+            pass
+        self.autostart.clicked.connect(self.autostart_clicked)
+        #self.layout2.addWidget(QtWidgets.QLabel('Name' + ' Device #' + str(devicedict['device'].numdevice)),0,0)
+        self.layout2.addWidget(self.namelabel,0,0)
+        self.layout.addLayout(self.layout2)
+        self.layout.addStretch()
+        self.layout.addWidget(self.autostart)
+        self.layout.addWidget(self.logwidget)
+        self.layout.addWidget(self.viewbtn)
+        self.layout.addWidget(self.infobtn)
+        self.layout.addWidget(self.renbtn)
+        self.layout.addWidget(self.conbtn)
+        self.layout.addWidget(self.rembtn)
+        self.layout.addWidget(self.startbtn)
+
+    def autostart_clicked(self):
+        #print('Autostart',self.autostart.isChecked())
+        self.device.autostart = self.autostart.isChecked()
+
+    def loglevel_changed(self):
+        loglevel = self.logwidget.currentText()
+        logger = self.devicedict['logger']
+        print('loglevel changed to',loglevel)
+        if(logger is not None):
+            logger.setLevel(loglevel)
+
+    def get_info(self):        
+        self.infowidget       = QtWidgets.QPlainTextEdit()
+        self.infowidget.setReadOnly(True)
+        sortstat ={}
+        for i in sorted(self.devicedict['statistics']):
+            sortstat[i]=self.devicedict['statistics'][i]
+
+        sortstat['datakeys'] = sorted(sortstat['datakeys'])
+        statstr = yaml.dump(sortstat)
+        self.infowidget.insertPlainText(statstr + '\n')
+        self.infowidget.show()
+        
+        
+    def viewclicked(self):
+        self.redvyprwidget.devicetabs.setCurrentWidget(self.devicedict['widget'])        
+
+    def conclicked(self):
+        self.connect.emit(self.devicedict)
+
+    def startstopclicked(self):
+        funcname = __name__ + '.startstopclicked()'
+        logger.debug(funcname)
+        if(self.startbtn.text() == 'Stop'):
+            self.device.thread_stop()
+        else:
+            self.device.thread_start()
+
+    def thread_status(self,statusdict):
+        """ Function regularly called by redvypr to update the thread status
         """
-        T = float(self._datadisplays['Tseted'].text())
-        logger.debug('Setting temperature to {:f}'.format(T))
-        comdict = {'set':T}
-        self.device.comqueue.put(comdict)
-    
-    def thread_status(self,status):
-        """ This function is regularly called by redvypr whenever the thread is started/stopped
+        status = statusdict['thread_status']
+        if(status):
+            self.startbtn.setText('Stop')
+            self.startbtn.setChecked(True)            
+        else:
+            self.startbtn.setText('Start')
+            self.startbtn.setChecked(False)                        
+
+    def remdevice(self):
+        """ Removing the device
         """
-        pass        
+        ret = QtWidgets.QMessageBox.question(self,'', "Are you sure to remove the device?", QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No)
+        if ret == QtWidgets.QMessageBox.Yes:
+            widget = self.devicedict['widget']
+            for i in range(self.devicetab.count()):
+                if(self.devicetab.widget(i) == widget):
+                    self.redvyprwidget.closeTab(i)
 
-    def update(self,data):
-        """ Updates the data display
+    def rendevice(self):
+        """ Renaming a device
         """
-        
-        funcname = __name__ + '.update():'
-        tnow = time.time()
-        #logger.debug(funcname + 'data {:s}'.format(str(data)))
-        try:
-            print(funcname + 'got data',data)
-            update = (tnow - self.config['last_update']) > self.config['dt_update']
+        oldname = self.devicedict['device'].name
+        name, okPressed = QtWidgets.QInputDialog.getText(self, "Enter new name","Device name:", QtWidgets.QLineEdit.Normal, oldname)
+        if okPressed and name != '':
+            renamed = self.redvyprwidget.renamedevice(oldname,name)
+
+#
+#
+#
+# A logging handler for qplaintext
+#
+#
+#
+class QPlainTextEditLogger(logging.Handler):
+    def __init__(self):
+        super(QPlainTextEditLogger, self).__init__()
+
+    def add_widget(self,widget):        
+        self.widget = widget
+
+    def emit(self, record):
+        msg = self.format(record)
+        self.widget.appendPlainText(msg)
+
+    def write(self, m):
+        pass   
+    
+
+
+
+#
+#
+# Widget shows the statistics of the device
+#
+#
+class redvypr_deviceInfoWidget(QtWidgets.QWidget):
+    def __init__(self, device=None):
+        funcname = __name__ + '.__init__():'
+        logger.debug(funcname)
+        super().__init__()
+        self.device = device
+        self.layout = QtWidgets.QGridLayout(self)
+        self.infowidget       = QtWidgets.QPlainTextEdit()
+        self.infowidget.setReadOnly(True)
+        self.layout.addWidget(self.infowidget,0,0)
+
+        self.updatetimer = QtCore.QTimer()
+        self.updatetimer.timeout.connect(self.__update_info)
+        self.updatetimer.start(500)
+
+    def __update_info(self):
+        funcname = __name__ + '.__update_info():'
+        prev_cursor = self.infowidget.textCursor()
+        pos  = self.infowidget.verticalScrollBar().value()
+        pos2 = self.infowidget.verticalScrollBar().value()
+        self.infowidget.clear()
+        sortstat = {}
+        for i in sorted(self.device.statistics):
+            sortstat[i]=self.device.statistics[i]
+
+        sortstat['datakeys'] = sorted(sortstat['datakeys'])
+        statstr = yaml.dump(sortstat)
+        self.infowidget.insertPlainText(statstr + '\n')
+        #self.infowidget.moveCursor(QtGui.QTextCursor.End)
+        # cursor.setPosition(0)
+        # self.text.setTextCursor(prev_cursor)
+        if True:
+            self.infowidget.verticalScrollBar().setValue(pos)
+
+
+
 
-            if(update):
-                self.config['last_update'] = tnow
 
-            # Update the time
-            t = data['t']
-            timestr = datetime.datetime.fromtimestamp(t).strftime('%d %b %Y %H:%M:%S')
-            self.timelabel.setText(timestr)
-            try:
-                self._datadisplays['Tset'].set_data(data['Tset'])
-                Tset = data['Tset']
-            except Exception as e:
-                logger.debug(funcname + ':Tset error: {:s}'.format(str(e)))
-                Tset = None
 
-            try:
-                self._datadisplays['Tbath'].set_data(data['Tbath'])
-                Tbath = data['Tbath']
-            except Exception as e:
-                logger.debug(funcname + ':Tbath error: {:s}'.format(str(e)))
-                Tbath = None
-
-            if(Tbath is not None):
-                # Update the plot
-                lbath = self.plot['lines']['Tbath']
-                x = lbath['x']
-                y = lbath['y']            
-                x        = np.roll(x,-1)
-                y        = np.roll(y,-1)
-                x[-1]    = float(t)
-                y[-1]    = float(Tbath)
-                lbath['x']  = x
-                lbath['y']  = y
-                color = lbath['config']['color']
-                linewidth = lbath['config']['linewidth']                                
-                lbath['line'].setData(x=x,y=y,pen = pyqtgraph.mkPen(color), width=linewidth)
-
-            if(Tset is not None):
-                # Update the plot
-                lset = self.plot['lines']['Tset']
-                x = lset['x']
-                y = lset['y']            
-                x        = np.roll(x,-1)
-                y        = np.roll(y,-1)
-                x[-1]    = float(t)
-                y[-1]    = float(Tset)
-                lset['x']  = x
-                lset['y']  = y
-                color = lset['config']['color']
-                linewidth = lset['config']['linewidth']                
-                lset['line'].setData(x=x,y=y,pen = pyqtgraph.mkPen(color), width=linewidth)                                
-                
-        except Exception as e:
-            logger.debug(funcname + ':' + str(e))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `redvypr-0.4.4/redvypr/devices/network_device.py` & `redvypr-0.5.3/redvypr/devices/network/network_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 import logging
 import sys
 import threading
 import socket
 #from apt_pkg import config
 import yaml
 import copy
+from redvypr.device import redvypr_device
+from redvypr.data_packets import check_for_command
 
 logging.basicConfig(stream=sys.stderr)
 logger = logging.getLogger('network_device')
 logger.setLevel(logging.DEBUG)
 
 #https://stackoverflow.com/questions/166506/finding-local-ip-addresses-using-pythons-stdlib
 def get_ip():
@@ -53,36 +55,73 @@
     return IP
 
 
 def yaml_dump(data):
     #return yaml.dump(data,default_flow_style=False)
     return yaml.dump(data,explicit_end=True,explicit_start=True)
 
+def raw_to_packet(datab,config):
+    """
+    Packs the received raw data into a packet that can be sent via the dataqueue
+
+    Args:
+        datab:
+        config:
+
+    Returns:
+        packets: A list of datapackets to be sent via the dataqueue
+
+    """
+    funcname = __name__ + '.raw_to_packet()'
+    t = time.time()
+    packets = []
+    if(config['serialize'] == 'yaml'):
+        for databs in datab.split(b'...\n'): # Split the text into single subpackets
+            try:
+                data = yaml.safe_load(databs)
+            except Exception as e:
+                logger.debug(funcname + ': Could not decode message {:s}'.format(str(data)))
+                logger.debug(funcname + ': Could not decode message  with supposed format {:s} into something useful.'.format(config['data']))
+            if(data is not None):
+                if(config['data'] == 'all'): # Forward the whole message
+                    packets.append(data)
+                else:
+                    datan = {'t':t}
+                    datan[config['data']] = data[k]
+                    packets.append(datan)
+
+    elif (config['serialize'] == 'utf-8'):  # Put the "str" data into the packet with the key in "data"
+        data = datab.decode('utf-8')
+        datan = {'t':t}
+        datan[config['data']] = data
+        packets.append(datan)
+    elif(config['serialize'] == 'raw'): # Put the "str" data into the packet with the key in "data"
+        datan = {'t':t}
+        datan[config['data']] = datab
+        packets.append(datan)
 
-def send_data(data_dict,config):
+    return packets
+
+def packet_to_raw(data_dict,config):
     """ Function that processes the data_dict to a serialized datastream sendable over network connections 
     """
     funcname = __name__ + 'send_data()'
-
-    # Choose the serialize function
-    if(config['serialize'] == 'str'):
-        serialize = str 
-    elif(config['serialize'] == 'yaml'):
-        serialize = yaml_dump # A dump with options
-        
-    # 
-    if(config['data'][0] == 'all'):
-        datab = serialize(data_dict).encode('utf-8')
-    else:
-        if(type(config['data']) == str):
-            config['data'] = [config['data']]
-            
-        datab = b''
-        for key in config['data']:
-            datab += serialize(data_dict[key]).encode('utf-8')
+    #
+    if (config['data'] == 'all') and (config['serialize'] == 'yaml'):
+        datab = yaml_dump(data_dict).encode('utf-8')
+    elif (config['serialize'] == 'utf-8'):
+        key = config['data']
+        datab = str(data_dict[key]).encode('utf-8')
+    elif (config['serialize'] == 'raw'):
+        key = config['data']
+        data = data_dict[key]
+        if(isinstance(data, (bytes, bytearray))):
+            datab = data
+        else:
+            datab = str(data).encode('utf-8')
 
     return datab
 
 
 def handle_tcp_client_send(client,threadqueue,statusqueue):
     funcname =  __name__ + 'handle_tcp_client_send()'
     address = client[1]
@@ -94,27 +133,26 @@
     except Exception as e:
         logger.warning(funcname + ':' + str(e))
     
     while True:
         data = threadqueue.get()
         #print('Read data from queue')
         try:
-            #logger.debug(funcname  + ':Sending data: {:s}'.format(str(data)))
+            logger.debug(funcname  + ':Sending data: {:s}'.format(str(data)))
             client.send(data)
         except Exception as e:
             statusstr = 'Connection to {:s} closed, stopping thread'.format(str(address))
             try:
                 statusqueue.put_nowait(statusstr)
             except: # If the queue is full
                 pass
             logger.info(funcname + ':' + statusstr)
             return
-        
 
-def start_tcp_send(dataqueue, datainqueue, comqueue, statusqueue, config=None):
+def start_tcp_send(dataqueue, datainqueue, statusqueue, config=None, device_info=None):
     """ TCP publishing, this thread waits for TCP connections connections. For each connection a new connection is created that is fed with a subthread (handle_tcp_send) is created that is receiving data with a new queue. 
     """
     funcname = __name__ + '.start_tcp_send()'
     logger.debug(funcname + ':Starting network thread')        
     npackets     = 0 # Number of packets
     bytes_read   = 0
     threadqueues = []
@@ -122,41 +160,50 @@
     server.bind((config['address'],config['port']))
     server.listen(8)
     server.settimeout(0.05) # timeout for listening
     # Some variables for status
     tstatus = time.time()
     dtstatus = 5 # Send a status message every dtstatus seconds
     npackets = 0 # Number packets received via the datainqueue
-            
-    while True:
-        try:
-            com = comqueue.get(block=False)
-            logger.info(funcname + 'received command:' + str(com) + ' stopping now')
-            server.close()            
-            break
-        except:
-            pass
+    clients = []
+    try:
+        queuesize = config['queuesize']
+    except:
+        queuesize = 1000
 
-        try:        
+    FLAG_RUN = True
+    while FLAG_RUN:
+        try:
             client, address = server.accept() # Here the timeout will let the loop run with 20 Hz
-            threadqueue = queue.Queue()
-            tcp_thread = threading.Thread(target=handle_tcp_client_send, args=([client,address],threadqueue,statusqueue))
+            threadqueue = queue.Queue(maxsize=queuesize)
+            tcp_thread = threading.Thread(target=handle_tcp_client_send, args=([client,address],threadqueue,statusqueue), daemon=True)
             tcp_thread.start()
+            clients.append(client)
             threadqueues.append({'thread':tcp_thread,'queue': threadqueue,'address':address,'bytes_sent':0,'packets_sent':0})
         except socket.timeout:
             pass
         except Exception as e:
             logger.info(funcname + ':thread start: ' + str(e))
         
         while(datainqueue.empty() == False):
             try:
                 data_dict = datainqueue.get(block=False)
+                command = check_for_command(data_dict, thread_uuid=device_info['thread_uuid'])
+                if (command is not None):
+                    logger.debug('Command is for me: {:s}'.format(str(command)))
+                    for client in clients:
+                        client.close()
+                    server.close()
+                    logger.info(funcname + 'received command:' + str(data_dict) + ' stopping now')
+                    FLAG_RUN = False
+                    break
+
                 npackets += 1
                 # Call the send_data function to create a binary sendable datastream
-                datab      = send_data(data_dict,config)
+                datab      = packet_to_raw(data_dict,config)
                 #print('sending data',datab)
                 for q in threadqueues:
                     q['queue'].put(datab)
                     q['bytes_sent'] += len(datab)
                     q['packets_sent'] += 1
 
             except Exception as e:
@@ -185,15 +232,15 @@
             except: # If the queue is full
                 pass                
 
             
         
         
             
-def start_tcp_recv(dataqueue, datainqueue, comqueue, statusqueue, config=None):
+def start_tcp_recv(dataqueue, datainqueue, statusqueue, config=None, device_info=None):
     """ TCP receiving
     """
     funcname = __name__ + '.start_tcp_recv()'
     logger.debug(funcname + ':Starting network thread')        
     sentences = 0
     bytes_read = 0
     reconnections = 0
@@ -228,18 +275,22 @@
     except:
         config['tcp_numreconnect'] = 10
         
     # 
     npackets = 0 # Number packets received via the datainqueue
     while True:
         try:
-            com = comqueue.get(block=False)
-            logger.debug('received command:' + str(com) + ' stopping now')
-            client.close()            
-            break
+            com = datainqueue.get(block=False)
+            command = check_for_command(com, thread_uuid=device_info['thread_uuid'])
+            print(funcname + ': Got command',com)
+            if (command is not None):
+                logger.debug('Command is for me: {:s}'.format(str(command)))
+                client.close()
+                logger.info(funcname + 'received command:' + str(com) + ' stopping now')
+                break
         except:
             pass
 
         try:
             datab = client.recv(1000000)
             if(datab == b''): # Connection closed
                 logger.warning(funcname + ': Connection closed by host')
@@ -252,52 +303,28 @@
                             client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                             client.settimeout(1.0) # timeout for listening
                             client.connect((config['address'],config['port']))
                             reconnections += 1
                         except:
                             logger.warning(funcname + ': Could not connect to host.')
                             
-                    return
-                    
                     logger.info(funcname + ': Connected to '+ str(config))
                     client.settimeout(0.05) # timeout for listening
                 else:
                     logger.warning(funcname + ': Stopping thread')
                     client.close()
                     break
-            
-            t = time.time()
+
             bytes_read += len(datab)
             # Check what data we are expecting and convert it accordingly
-            if(config['serialize'] == 'yaml'):
-                for databs in datab.split(b'...\n'): # Split the text into single subpackets
-                    try:
-                        data = yaml.safe_load(databs)
-                        #print(datab)
-                        #print(data)
-                    except Exception as e:
-                        logger.debug(funcname + ': Could not decode message {:s}'.format(str(datab)))
-                        logger.debug(funcname + ': Could not decode message  with supposed format {:s} into something useful.'.format(str(config['data'])))
-                        data = None
-
-                    if(data is not None):
-                        if(config['data'][0] == 'all'): # Forward the whole message
-                            dataqueue.put(data)
-                        else:
-                            datan = {'t':t}
-                            for k in config['data']: # List of keys
-                                datan[k] = data[k]
-
-                            dataqueue.put(datan)
-            else: # Put the "str" data into the packet with the key in "data"
-                data = datab.decode('utf-8')
-                datan = {'t':t}
-                datan['data'] = data
-                dataqueue.put(datan)
-            
+            packets = raw_to_packet(datab, config)
+            for p in packets:
+                dataqueue.put(p)
+                npackets += 1
+
         except socket.timeout as e:
             pass
         except Exception as e:
             logger.info(funcname + ':' + str(e))
             return
 
         # Sending a status message
@@ -310,19 +337,16 @@
             #statusdata['clients'] = []
             statusdata['config'] = copy.deepcopy(config)
                 
             try:
                 statusqueue.put_nowait(statusdata)
             except: # If the queue is full
                 pass
-        
-
-
 
-def start_udp_send(dataqueue, datainqueue, comqueue, statusqueue, config=None):
+def start_udp_send(dataqueue, datainqueue, statusqueue, config=None, device_info=None):
     """ UDP publishing
     """
     funcname = __name__ + '.start_udp_send()'
     logger.debug(funcname + ':Starting network thread')        
     sentences = 0
     bytes_sent = 0
 
@@ -331,34 +355,44 @@
     dtstatus = 5 # Send a status message every dtstatus seconds
     npackets = 0 # Number packets received via the datainqueue
     client = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP) # UDP
     if(config['address'] == '<broadcast>'):        
         client.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         # Enable broadcasting mode
         client.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-    client.settimeout(0.01) # timeout for listening
-
-    while True:
-        try:
-            com = comqueue.get(block=False)
-            logger.info(funcname + 'received command:' + str(com) + ' stopping now')
-            client.close()            
-            break
-        except:
-            pass
 
+    client.settimeout(0.01) # timeout for listening, do we need that here??
+    FLAG_RUN=True
+    while FLAG_RUN:
         time.sleep(0.05)
         while(datainqueue.empty() == False):
             try:
                 data_dict = datainqueue.get(block=False)
-                npackets += 1
-                # Call the send_data function to create a binary sendable datastream
-                datab      = send_data(data_dict,config)
-                bytes_sent += len(datab)
-                client.sendto(datab, (config['address'], config['port']))
+                command = check_for_command(data_dict, thread_uuid=device_info['thread_uuid'])
+                if (command is not None):
+                    logger.debug('Command is for me: {:s}'.format(str(command)))
+                    client.close()
+                    logger.info(funcname + 'received command:' + str(data_dict) + ' stopping now')
+                    statusdata = {}
+                    statusdata['status'] = 'Stopping UDP redcv thread'
+                    statusdata['time'] = str(datetime.datetime.now())
+                    try:
+                        statusqueue.put_nowait(statusdata)
+                    except:  # If the queue is full
+                        pass
+
+                    FLAG_RUN=False
+                    break
+                else:
+                    npackets   += 1
+                    # Call the send_data function to create a binary sendable datastream
+                    datab       = packet_to_raw(data_dict,config)
+                    bytes_sent += len(datab)
+                    #print('Sending data',datab)
+                    client.sendto(datab, (config['address'], config['port']))
 
             except Exception as e:
                 logger.debug(funcname + ':Exception:' + str(e))
 
 
 
         # Sending a status message
@@ -374,19 +408,19 @@
             except: # If the queue is full
                 pass
             
 
 
         
         
-def start_udp_recv(dataqueue, datainqueue, comqueue, statusqueue, config=None):
+def start_udp_recv(dataqueue, datainqueue, statusqueue, config=None, device_info = None):
     """ UDP receiving
     """
     funcname = __name__ + '.start_udp_recv():'
-    logger.debug(funcname + ':Starting network thread')        
+    logger.debug(funcname + ':Starting network thread (uuid: {:s})'.format(device_info['thread_uuid']))
     npackets     = 0
     bytes_read   = 0
     threadqueues = []
     tstatus      = 0
     dtstatus     = 2 # Send a status message every dtstatus seconds
     
     #client = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP) # UDP
@@ -395,58 +429,45 @@
         client.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         # Enable broadcasting mode
         client.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
     client.settimeout(0.05) # timeout for listening
     client.bind((config['address'],config['port']))
     while True:
         try:
-            com = comqueue.get(block=False)
-            client.close()            
-            logger.info(funcname + 'received command:' + str(com) + ' stopping now')
-            statusdata = {}
-            statusdata['status'] = 'Stopping UDP redcv thread'
-            statusdata['time'] = str(datetime.datetime.now())
-            try:
-                statusqueue.put_nowait(statusdata)
-            except: # If the queue is full
-                pass            
+            com = datainqueue.get(block=False)
+            command = check_for_command(com,thread_uuid=device_info['thread_uuid'])
+            logger.debug('Got a command: {:s}'.format(str(com)))
+            if (command is not None):
+                logger.debug('Command is for me: {:s}'.format(str(command)))
+                client.close()
+                logger.info(funcname + 'received command:' + str(com) + ' stopping now')
+                statusdata = {}
+                statusdata['status'] = 'Stopping UDP redcv thread'
+                statusdata['time'] = str(datetime.datetime.now())
+                try:
+                    statusqueue.put_nowait(statusdata)
+                except:  # If the queue is full
+                    pass
+
+                break
 
-            break
         except:
             pass
 
         try:
             datab, addr = client.recvfrom(1000000)
+            #print('Got data',datab,addr)
             bytes_read += len(datab)
             t = time.time()
             # Check what data we are expecting and convert it accordingly
-            if(config['serialize'] == 'yaml'):
-                for databs in datab.split(b'...\n'): # Split the text into single subpackets                
-                    try:
-                        data = yaml.safe_load(databs)
-                    except Exception as e:
-                        logger.debug(funcname + ': Could not decode message {:s}'.format(str(data)))
-                        logger.debug(funcname + ': Could not decode message  with supposed format {:s} into something useful.'.format(config['data']))
-                    if(data is not None):                    
-                        if(config['data'][0] == 'all'): # Forward the whole message
-                            dataqueue.put(data)
-                        else:
-                            datan = {'t':t}
-                            for k in config['data']: # List of keys
-                                datan[k] = data[k]
-
-                            dataqueue.put(datan)
-                            npackets += 1
-            else: # Put the "str" data into the packet with the key in "data"
-                data = datab.decode('utf-8')
-                datan = {'t':t}
-                datan['data'] = data
-                dataqueue.put(datan)
+            packets = raw_to_packet(datab, config)
+            for p in packets:
+                dataqueue.put(p)
                 npackets += 1
-            
+
             #print(config)
             #print('UDP Received',datab)
             #print('UDP sent as',datan)
         except socket.timeout as e:
             pass
         except Exception as e:
             logger.info(funcname + ': Error: ' + str(e))
@@ -468,50 +489,57 @@
                 statusqueue.put_nowait(statusdata)
             except: # If the queue is full
                 pass
 
 
     logger.info(funcname + ' stopped')
 
-class Device():
-    def __init__(self,dataqueue=None,comqueue=None,datainqueue=None,statusqueue=None):
+class Device(redvypr_device):
+    def __init__(self, **kwargs):
         """
         """
-        self.publish     = False # publishes data, a typical device is doing this
-        self.subscribe   = False  # subscribing data, a typical datalogger is doing this
-        self.datainqueue = datainqueue
-        self.dataqueue   = dataqueue        
-        self.comqueue    = comqueue
-        self.statusqueue = statusqueue
-        self.config = {}
+        super(Device, self).__init__(**kwargs)
+        self.publish = True
+        self.subscribe = True
+        self.description = 'network device'
+        self.thread_communication = self.datainqueue  # Change the commandqueue to the datainqueue
         self.check_and_fill_config() # Add standard stuff
         
-    def thread_status(self,status):
-        """ Function that is called by redvypr, allowing to update the status of the device according to the thread 
+    def start(self, device_info, config, dataqueue, datainqueue, statusqueue):
         """
-        self.threadalive = status['threadalive']
 
-    def start(self):
+        Args:
+            device_info:
+            config:
+            dataqueue:
+            datainqueue:
+            statusqueue:
+
+        Returns:
+
+        """
         funcname = __name__ + '.start():'
         self.check_and_fill_config()
         logger.debug(funcname + self.config['protocol'])
         if(self.config['direction'] == 'publish'):
             if(self.config['protocol'] == 'tcp'):
                 logger.info(__name__ + ':Start to serve data on address (TCP):' + str(self.config))
-                start_tcp_send(self.dataqueue,self.datainqueue,self.comqueue,self.statusqueue,config=self.config)
+                start_tcp_send(self.dataqueue,self.datainqueue,self.statusqueue,config=self.config,device_info=device_info)
             elif(self.config['protocol'] == 'udp'):
                 logger.info(__name__ + ':Start to serve data on address (UDP broadcast)')
-                start_udp_send(self.dataqueue,self.datainqueue,self.comqueue,self.statusqueue,config=self.config)                
+                #start_udp_send(self.dataqueue,self.datainqueue,self.statusqueue,config=self.config)
+                start_udp_send(self.dataqueue, self.datainqueue, self.statusqueue, config=self.config,
+                               device_info=device_info)
         elif(self.config['direction'] == 'receive'):
             if(self.config['protocol'] == 'tcp'):
                 logger.info('Start to receive data from address (TCP):' + str(self.config))
-                start_tcp_recv(self.dataqueue,self.datainqueue,self.comqueue,self.statusqueue,config=self.config)
+                start_tcp_recv(self.dataqueue,self.datainqueue,self.statusqueue,config=self.config,device_info=device_info)
             elif(self.config['protocol'] == 'udp'):
                 logger.info('Start to receive data from address (UDP):' + str(self.config))
-                start_udp_recv(self.dataqueue,self.datainqueue,self.comqueue,self.statusqueue,config=self.config)
+                start_udp_recv(self.dataqueue,self.datainqueue,self.statusqueue,config=self.config,device_info=device_info)
                 
     
     def check_and_fill_config(self):
         """ Fills a config, if essential entries are missing
         """
         try:
             self.config['address']
@@ -542,24 +570,20 @@
             self.config['direction']
         except:
             self.config['direction'] = 'publish' # publish/receive
             
         try:
             self.config['data']
         except: 
-            self.config['data'] = ['all'] # "all" for the whole dictionary, comma separated "keys" for parts of the dictionary
+            self.config['data'] = 'data' #
 
-        # Make a list out of a string
-        if(self.config['data'] == 'all'):
-            self.config['data'] = ['all']
-            
         try:
             self.config['serialize']
         except:
-            self.config['serialize'] = 'yaml' # yaml/str
+            self.config['serialize'] = 'raw' # yaml/str/raw
 
     def status(self):
         funcname = 'status()'
         #print('Status')
         status = self.statusqueue.get_nowait()
         #print(statusstr)
         statusstr = yaml.dump(status)
@@ -569,29 +593,31 @@
     def __str__(self):
         sstr = 'network device'
         return sstr
 
 
 
 class initDeviceWidget(QtWidgets.QWidget):
-    device_start = QtCore.pyqtSignal(Device)
-    device_stop = QtCore.pyqtSignal(Device)        
+    #device_start = QtCore.pyqtSignal(Device)
+    #device_stop = QtCore.pyqtSignal(Device)
+    connect      = QtCore.pyqtSignal(redvypr_device) # Signal requesting a connect of the datainqueue with available dataoutqueues of other devices
     def __init__(self,device=None):
         super(QtWidgets.QWidget, self).__init__()
         layout        = QtWidgets.QFormLayout(self)
         self.device   = device
         self.device.check_and_fill_config() # Add standard stuff
         self.inputtabs = QtWidgets.QTabWidget() # Create tabs for different connection types
         self.serialwidget = QtWidgets.QWidget()
         self.label    = QtWidgets.QLabel("Network device")
         self.label.setAlignment(QtCore.Qt.AlignCenter)
         self.label.setStyleSheet("font-weight: bold; font-size: 16")
         self.startbtn = QtWidgets.QPushButton("Open device")
         self.startbtn.clicked.connect(self.start_clicked)
         self.startbtn.setCheckable(True)
+
         self.config_widgets = [] # Collecting all config widgets here, makinf it easier to grey them out
         # Address and port
         self.addressline = QtWidgets.QLineEdit()
         self.addressline.setStatusTip('The IP Address, for UDP Broadcast use "<broadcast>", use <IP> for local network IP')
         myip = get_ip()
         addresses = ["<broadcast>", "<IP>", myip ]
         completer = QtWidgets.QCompleter(addresses)
@@ -599,40 +625,44 @@
         self.portline = QtWidgets.QLineEdit()
         
             
         # Data direction
         self._combo_inout = QtWidgets.QComboBox()
         self._combo_inout.addItem('Publish')        
         self._combo_inout.addItem('Receive')
-        self._combo_inout.currentIndexChanged.connect(self.process_options)
+
         
         # Data direction
         self._combo_proto = QtWidgets.QComboBox()
         self._combo_proto.addItem('TCP')        
         self._combo_proto.addItem('UDP')
-        self._combo_proto.currentIndexChanged.connect(self.process_options)
-        
-        
+
         # Publish options
         # Create an array of radio buttons
-        self._data_pub_all  = QtWidgets.QRadioButton("Whole dictionary")
-        self._data_pub_all.setStatusTip('Serializes the whole dictionary into a string using YAML')
+        self._data_pub_all  = QtWidgets.QRadioButton("Redvypr YAML datapacket")
+        self._data_pub_all.setStatusTip('Sends/Expects the whole datapacket as a YAML string')
         self._data_pub_all.setChecked(True)
+
         self._data_pub_dict = QtWidgets.QRadioButton("Dictionary entries")
-        self._data_pub_dict.setStatusTip('Choose entries of the dictionary and serialize them as utf-8 string or yaml')
-        
+        self._data_pub_dict.setStatusTip('Sends entries and serialize them as choosen by the serialization box')
+
         self._data_pub_group = QtWidgets.QButtonGroup()
         self._data_pub_group.addButton(self._data_pub_all)
         self._data_pub_group.addButton(self._data_pub_dict)
         
         # Serialize
         self._combo_ser = QtWidgets.QComboBox()
-        self._combo_ser.addItem('str')
-        self._combo_ser.addItem('YAML')
-        
+        self._combo_ser.addItem('utf-8')
+        self._combo_ser.addItem('raw')
+        self._combo_ser.addItem('yaml')
+
+
+
+
+
         
         
         # Data format to submit
         self.fdataentry  = QtWidgets.QLabel("Data keys publish")        
         self.dataentry   = QtWidgets.QLineEdit()
         self.dataentry.setText('data')
 
@@ -643,136 +673,154 @@
         layout.addRow(QtWidgets.QLabel("Port"),self.portline)
         layout.addRow(QtWidgets.QLabel("Data direction"),self._combo_inout)
         layout.addRow(QtWidgets.QLabel("Protocol"),self._combo_proto)
         self._serialize_label = QtWidgets.QLabel("Data publishing options")
         layout.addRow(self._serialize_label)
         layout.addRow(self._data_pub_all,self._data_pub_dict)
         layout.addRow(QtWidgets.QLabel("Serialize"),self._combo_ser)
-        layout.addRow(self.fdataentry,self.dataentry)  
+        layout.addRow(self.fdataentry,self.dataentry)
         layout.addRow(self.startbtn)
         
         self.config_widgets.append(self.addressline)
         self.config_widgets.append(self.portline)
         self.config_widgets.append(self._combo_inout)
         self.config_widgets.append(self._combo_proto)        
         self.config_widgets.append(self._data_pub_all)
         self.config_widgets.append(self._data_pub_dict)
         self.config_widgets.append(self._combo_ser)
         self.config_widgets.append(self.dataentry)
 
         self.config_to_buttons()
         self.process_options()
+        self.connect_signals_options(connect=True)
+
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update_buttons)
+        self.statustimer.start(500)
+
+    def connect_signals_options(self,connect=True):
+        if True:
+            if(connect):
+                self._combo_inout.currentIndexChanged.connect(self.process_options)
+                self._combo_proto.currentIndexChanged.connect(self.process_options)
+                self._data_pub_all.toggled.connect(self.process_options)
+                self._combo_ser.currentIndexChanged.connect(self.process_options)
+            else:
+                try:
+                    self._combo_inout.currentIndexChanged.disconnect()
+                    self._combo_proto.currentIndexChanged.disconnect()
+                    self._data_pub_all.toggled.disconnect()
+                    self._combo_ser.currentIndexChanged.disconnect()
+                except:
+                    pass
+
         
     def config_to_buttons(self):
         """ Update the configuration widgets according to the config dictionary in the device module 
         """
-        print('Config to buttons',self.device.config)
+        #print('Config to buttons',self.device.config)
+
+        # Disconnect all signals
+        self.connect_signals_options(connect=False)
+        if (self.device.config['protocol'] == 'tcp'):
+            self._combo_proto.setCurrentIndex(0)
+        else:
+            self._combo_proto.setCurrentIndex(1)
+
         if(self.device.config['address'] is not None):
             self.addressline.setText(self.device.config['address'])
         if(self.device.config['port'] is not None):
             self.portline.setText(str(self.device.config['port']))
             
         if(self.device.config['direction'] == 'publish'):
             self._combo_inout.setCurrentIndex(0)
         else:
             self._combo_inout.setCurrentIndex(1)
-            
-        if(self.device.config['protocol'] == 'tcp'):
-            self._combo_proto.setCurrentIndex(0)
-        else:
-            self._combo_proto.setCurrentIndex(1)
-            
-        if(self.device.config['serialize'] == 'yaml'):
-            self._combo_ser.setCurrentIndex(0)
-        else:
-            self._combo_ser.setCurrentIndex(1)
-            
-        if(self.device.config['data'][0] == ['all']):
-            self._data_pub_all.setChecked(True)   
+
+        for i in range(self._combo_ser.count()):
+            self._combo_ser.setCurrentIndex(i)
+            txt = self._combo_ser.currentText()
+            print('txt',i,txt)
+            if(txt.lower() == self.device.config['serialize'].lower()):
+                print('break')
+                break
+
+        if(self.device.config['serialize'].lower() == 'all'):
+            self._data_pub_all.setChecked(True)
         else:
             self._data_pub_dict.setChecked(True)
-            txt = ''
-            for d in self.device.config['data']:
-                txt += d + ','
 
-            txt = txt[:-1]
-            self.dataentry.setText(txt)
-            
+
+        self.dataentry.setText(self.device.config['data'])
+        self.connect_signals_options(connect=True)
             
     def process_options(self):
         """ Reads all options and creates a configuration dictionary
         """
         funcname = __name__ + '.process_options()'
         config   = {}
-        
+        print('Process options')
+
+        config['address']   = self.addressline.text()
+        config['direction'] = self._combo_inout.currentText().lower()
+        config['protocol']  = self._combo_proto.currentText().lower()
+        if(self._data_pub_all.isChecked()): # sending/receiving YAML dictionaries
+            self.dataentry.setEnabled(False)
+            self._combo_ser.setEnabled(False)
+            config['serialize'] = 'yaml'
+            config['data']      = 'all'
+        else:
+            self.dataentry.setEnabled(True)
+            self._combo_ser.setEnabled(True)
+            config['serialize'] = self._combo_ser.currentText().lower()
+            config['data']      = self.dataentry.text()
+
         # Change the GUI according to send/receive
         if(self._combo_inout.currentText() == 'Publish'):
             self._serialize_label.setText("Data publishing options")
-            self.dataentry.setEnabled(True)
-        else:  
-            self._serialize_label.setText("Data receiving options")
-            #self._combo_ser.setCurrentIndex(0)
-            self._data_pub_all.setChecked(True)
-            self.dataentry.setEnabled(False)
-         
-        if(self._combo_inout.currentText() == 'Publish'):
-            config['direction'] = 'publish'
-            self.device.publish   = False
-            self.device.subscribe = True
+            self.fdataentry.setText("Data key to publish")
         else:
-            config['direction'] = 'receive'
-            self.device.publish   = True
-            self.device.subscribe = False
+            self._serialize_label.setText("Data receiving options")
+            self.fdataentry.setText("Data key to receive")
+
 
-        if(self._combo_proto.currentText() == 'TCP'):
-            config['protocol'] = 'tcp'
-        else:
-            config['protocol'] = 'udp'
-    
-        config['address'] = self.addressline.text()
         # Check for invalid combinations
         if((config['address'].lower()) == '<broadcast>' and config['protocol'] == 'tcp'):
             logger.warning(funcname + ': Broadcast works only with UDP')
-            config = None
-            return config
-        
+
         try:
             config['port'] = int(self.portline.text())
         except:
             logger.warning(funcname + ': Port is not an int')
-            raise ValueError
-        
-        if(self._data_pub_all.isChecked()):
-            config['data'] = ['all']
-        else:
-            config['data'] = self.dataentry.text().split(',')
-        
-        config['serialize'] = self._combo_ser.currentText().lower()
-                    
-        
-        logger.debug(funcname + ': config: ' + str(config))    
+
+
+        self.device.config = config
+        logger.debug(funcname + ': config: ' + str(config))
         return config
-    
+
     def thread_status(self,status):
         self.update_buttons(status['threadalive'])
         
-    def update_buttons(self,thread_status):
+    def update_buttons(self):
             """ Updating all buttons depending on the thread status (if its alive, graying out things)
             """
+
+            status = self.device.get_thread_status()
+            thread_status = status['thread_status']
             # Running
             if(thread_status):
                 self.startbtn.setText('Stop')
                 self.startbtn.setChecked(True)
-                for w in self.config_widgets:
-                    w.setEnabled(False)
+                #for w in self.config_widgets:
+                #    w.setEnabled(False)
             # Not running
             else:
                 self.startbtn.setText('Start')
-                for w in self.config_widgets:
-                    w.setEnabled(True)
+                #for w in self.config_widgets:
+                #    w.setEnabled(True)
                     
                 # Check if an error occured and the startbutton 
                 if(self.startbtn.isChecked()):
                     self.startbtn.setChecked(False)
                 #self.conbtn.setEnabled(True)
 
     def start_clicked(self):
@@ -787,21 +835,21 @@
                 return
 
             if(config == None):
                 self.startbtn.setChecked(False)
                 return
             
             # Setting the configuration
-            print('Starting network with config',config)
+            #print('Starting network with config',config)
             self.device.config = config
-            self.device_start.emit(self.device)
-            print('Config',config)
+            self.device.thread_start()
             button.setText("Starting")
         else:
-            self.device_stop.emit(self.device)
+            logger.debug('Stopping thread now')
+            self.device.thread_stop()
             button.setText("Stopping")
 
 
 
 
 # class displayDeviceWidget(QtWidgets.QWidget):
 #     def __init__(self):
```

### Comparing `redvypr-0.4.4/redvypr/devices/rawdatareplay.py` & `redvypr-0.5.3/redvypr/devices/fileio/rawdatareplay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,63 @@
-# TODO, improve keys!
 import datetime
 import logging
 import queue
 from PyQt5 import QtWidgets, QtCore, QtGui
 import time
 import numpy as np
 import logging
 import sys
 import yaml
 import copy
 import os
-from redvypr.data_packets import do_data_statistics, create_data_statistic_dict
+from redvypr.device import redvypr_device
+from redvypr.data_packets import do_data_statistics, create_data_statistic_dict,check_for_command
 
 logging.basicConfig(stream=sys.stderr)
 logger = logging.getLogger('rawdatareplay')
 logger.setLevel(logging.DEBUG)
 
 description = "Replays a raw redvypr data file"
 
+description = "Saves the raw redvypr packets into a file"
+config_template = {}
+config_template['name']      = 'rawdatareplay'
+config_template['files']             = {'type':'list','description':'List of files ro replay'} # TODO, list
+config_template['loop']              = {'type':'bool','default':True,'description':'Loop over all files if set'}
+config_template['speedup']           = {'type':'float','description':'Speedup factor of the data'}
+config_template['redvypr_device']    = {}
+config_template['redvypr_device']['publish']   = False
+config_template['redvypr_device']['subscribe'] = True
+config_template['redvypr_device']['description'] = description
+
 def get_packets(filestream=None):
-    funcname = __name__ + '.get_packets()' 
+    funcname = __name__ + '.get_packets()'
     packets = []
     if(filestream is not None):
         data = filestream.read()
         for databs in data.split('...\n'): # Split the text into single subpackets
             try:
                 data = yaml.safe_load(databs)
                 if(data is not None):
                     packets.append(data)
                     
             except Exception as e:
-                logger.debug(funcname + ': Could not decode message {:s}'.format(str(datab)))
-                logger.debug(funcname + ': Could not decode message  with supposed format {:s} into something useful.'.format(str(config['data'])))
+                logger.debug(funcname + ': Could not decode message {:s}'.format(str(databs)))
                 data = None
     
         return packets
     else:
         return None
         
     
 
 
-def start(datainqueue,dataqueue,comqueue,config={'filename':''}):
+def start(device_info, config={'filename': ''}, dataqueue=None, datainqueue=None, statusqueue=None):
     funcname = __name__ + '.start()'
-    logger.debug(funcname + ':Opening writing:')
+    logger.debug(funcname + ':Opening reading:')
     files = config['files']
     t_sent = 0 # The time the last packets was sent
     t_packet_old = 1e12 # The time the last packet had (internally)
     #
     try:
         config['speedup']
     except:
@@ -59,151 +69,118 @@
         config['loop']
     except:
         config['loop'] = False
         
     loop = config['loop']
     
     
-    print(funcname,'Config',config)    
     statistics = create_data_statistic_dict()
     
     bytes_read         = 0
     packets_read       = 0
     bytes_read_total   = 0
     packets_read_total = 0
     
     tfile           = time.time() # Save the time the file was created
     tflush          = time.time() # Save the time the file was created
     f = None    
     nfile = 0
     while True:
         tcheck      = time.time()
         try:
-            com = comqueue.get(block=False)
-            logger.debug(funcname + ': received:' + str(com))
-            break
-        except Exception as e:
-            #logger.warning(funcname + ': Error stopping thread:' + str(e))
-            pass
+            data = datainqueue.get(block=False)
+        except:
+            data = None
+        if (data is not None):
+            command = check_for_command(data, thread_uuid=device_info['thread_uuid'])
+            # logger.debug('Got a command: {:s}'.format(str(data)))
+            if (command is not None):
+                sstr = funcname + ': Command is for me: {:s}'.format(str(command))
+                logger.debug(sstr)
+                try:
+                    statusqueue.put_nowait(sstr)
+                except:
+                    pass
+                break
 
         packets = get_packets(f)
         if(packets is None):
             FLAG_NEW_FILE = True
         else:
             FLAG_NEW_FILE = False
             
         if(packets is not None):
             for p in packets:
                 t_now = time.time()
                 dt = t_now - t_sent
-                dt_packet = (p['t'] - t_packet_old)/speedup
+                dt_packet = (p['_redvypr']['t'] - t_packet_old)/speedup
                 if(dt_packet < 0):
                     dt_packet = 0
-                print('Sending packet in {:f} s.'.format(dt_packet))
+
                 if True:
-                    time.sleep(dt_packet) 
+                    time.sleep(dt_packet)
                     t_sent = time.time()
-                    t_packet_old = p['t']
+                    t_packet_old = p['_redvypr']['t']
                     dataqueue.put(p)
-                
-                #print(p)
-                
-                
+
+                sstr = 'Sending packet in {:f} s.'.format(dt_packet)
+                logger.debug(sstr)
+                try:
+                    statusqueue.put_nowait(sstr)
+                except:
+                    pass
+
+
             FLAG_NEW_FILE = True
             f.close()
             
         if(FLAG_NEW_FILE):
             if(nfile >= len(files)):
                 if(loop == False):
-                    logger.info(funcname + ': All files read, stopping now.')
+                    sstr = funcname + ': All files read, stopping now.'
+                    try:
+                        statusqueue.put_nowait(sstr)
+                    except:
+                        pass
+                    logger.info(sstr)
                     break
                 else:
-                    logger.info(funcname + ': All files read, loop again.')
+                    sstr = funcname + ': All files read, loop again.'
+                    try:
+                        statusqueue.put_nowait(sstr)
+                    except:
+                        pass
+
+                    logger.info(sstr)
                     nfile = 0
             
             filename = files[nfile]
-            print('Opening new file',filename)
+            sstr = 'Opening file {:s}'.format(filename)
+            try:
+                statusqueue.put_nowait(sstr)
+            except:
+                pass
+            logger.info(sstr)
             f = open(filename)
             nfile += 1
         
         time.sleep(0.05)
 
-class Device():
-    def __init__(self,dataqueue=None,comqueue=None,datainqueue=None):
-        """
-        """
-        self.publish     = True  # publishes data, a typical device is doing this
-        self.subscribe   = False   # subscribing data, a typical datalogger is doing this
-        self.datainqueue = datainqueue
-        self.dataqueue   = dataqueue        
-        self.comqueue    = comqueue
-        self.config      = {}
-        self.config['files'] = []
-        self.file_statistics = {}
-                
-    def start(self):
-        """
-        """
-        funcname = self.__class__.__name__
-        logger.debug(funcname)
-        print('Starting',self.config)
-        config=copy.deepcopy(self.config)
-        start(self.datainqueue,self.dataqueue,self.comqueue,config=config)
-        
-    def inspect_data(self,filename,rescan=False):
-        """ Inspects the files for possible datastreams in the file with the filename located in config['files'][fileindex].
-        """
-        funcname = self.__class__.__name__ + '.inspect_data()'
-        logger.debug(funcname)
-        try:
-            stat = self.file_statistics[filename]
-            FLAG_HASSTAT=True
-        except:
-            FLAG_HASSTAT=False
-            
-        if(rescan or (FLAG_HASSTAT == False)):
-            logger.debug(funcname + ': Scanning file {:s}'.format(filename))  
-            stat = create_data_statistic_dict()
-            # Create tmin/tmax in statistics
-            stat['t_min'] = 1e12
-            stat['t_max'] = -1e12
-            f = open(filename)
-            packets = get_packets(f)
-            f.close()
-            for p in packets:
-                stat = do_data_statistics(p,stat)
-                tminlist = [stat['t_min'],p['t']]
-                tmaxlist = [stat['t_max'],p['t']]
-                stat['t_min'] = min(tminlist)
-                stat['t_max'] = max(tmaxlist)
-            
-            self.file_statistics[filename] = stat
-        else:
-            logger.debug(funcname + ': No rescan of {:s}'.format(filename))  
-            
-        return stat
-        
-    def __str__(self):
-        sstr = 'rawdatareplay'
-        return sstr
 
 #
 #
 # The init widget
 #
 #
-
-
 class initDeviceWidget(QtWidgets.QWidget):
-    device_start = QtCore.pyqtSignal(Device) # Signal requesting a start of the device (starting the thread)
-    device_stop  = QtCore.pyqtSignal(Device) # Signal requesting a stop of device
-    connect      = QtCore.pyqtSignal(Device) # Signal requesting a connect of the datainqueue with available dataoutqueues of other devices
+    connect      = QtCore.pyqtSignal(redvypr_device) # Signal requesting a connect of the datainqueue with available dataoutqueues of other devices
     def __init__(self,device=None):
         super(QtWidgets.QWidget, self).__init__()
         layout        = QtWidgets.QGridLayout(self)
+        self.file_statistics = {}
         self.device   = device
         self.label    = QtWidgets.QLabel("rawdatareplay setup")
         self.label.setAlignment(QtCore.Qt.AlignCenter)
         self.label.setStyleSheet(''' font-size: 24px; font: bold''')
         self.config_widgets= [] # A list of all widgets that can only be used of the device is not started yet
         # Input output widget
         self.inlabel  = QtWidgets.QLabel("Filenames") 
@@ -230,15 +207,15 @@
         onlyDouble = QtGui.QDoubleValidator()
         self.speedup_edit.setValidator(onlyDouble)
         self.speedup_edit.setToolTip('Speedup of the packet replay.')
         self.speedup_label = QtWidgets.QLabel("Speedup factor")
         self.speedup_edit.setText("1.0")
         
         
-        self.startbtn = QtWidgets.QPushButton("Start logging")
+        self.startbtn = QtWidgets.QPushButton("Start replay")
         self.startbtn.clicked.connect(self.start_clicked)
         self.startbtn.setCheckable(True)
         self.startbtn.setSizePolicy(QtWidgets.QSizePolicy.Preferred,QtWidgets.QSizePolicy.Expanding)
         
         layout.addWidget(self.label,0,0,1,-1)
         
         layout.addWidget(self.addfilesbtn,1,0,1,-1)               
@@ -246,14 +223,51 @@
         layout.addWidget(self.scanfilesbtn,3,0,1,-1)
         layout.addWidget(self.inlabel,4,0,1,-1,QtCore.Qt.AlignCenter)         
         layout.addWidget(self.inlist,5,0,1,-1)
         layout.addWidget(self.loop_checkbox,6,0)
         layout.addWidget(self.speedup_label,6,1,1,1,QtCore.Qt.AlignRight)
         layout.addWidget(self.speedup_edit,6,2,1,1,QtCore.Qt.AlignRight)
         layout.addWidget(self.startbtn,7,0,2,-1)
+
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update_buttons)
+        self.statustimer.start(500)
+
+    def inspect_data(self, filename, rescan=False):
+        """ Inspects the files for possible datastreams in the file with the filename located in config['files'][fileindex].
+        """
+        funcname = self.__class__.__name__ + '.inspect_data()'
+        logger.debug(funcname)
+        try:
+            stat = self.file_statistics[filename]
+            FLAG_HASSTAT = True
+        except:
+            FLAG_HASSTAT = False
+
+        if (rescan or (FLAG_HASSTAT == False)):
+            logger.debug(funcname + ': Scanning file {:s}'.format(filename))
+            stat = create_data_statistic_dict()
+            # Create tmin/tmax in statistics
+            stat['t_min'] = 1e12
+            stat['t_max'] = -1e12
+            f = open(filename)
+            packets = get_packets(f)
+            f.close()
+            for p in packets:
+                stat = do_data_statistics(p, stat)
+                tminlist = [stat['t_min'], p['_redvypr']['t']]
+                tmaxlist = [stat['t_max'], p['_redvypr']['t']]
+                stat['t_min'] = min(tminlist)
+                stat['t_max'] = max(tmaxlist)
+
+            self.file_statistics[filename] = stat
+        else:
+            logger.debug(funcname + ': No rescan of {:s}'.format(filename))
+
+        return stat
         
     def finalize_init(self):
         """ Util function that is called by redvypr after initializing all config (i.e. the configuration from a yaml file)
         """
         funcname = self.__class__.__name__ + '.finalize_init()'
         logger.debug(funcname)
         
@@ -273,17 +287,16 @@
         """ Scans the selected files from the files list for possible datastreams 
         """
         funcname = self.__class__.__name__ + '.scan_files()'
         logger.debug(funcname)
 
         for i in rows:
             filename = self.inlist.item(i,0).text()
-            stat = self.device.inspect_data(filename,rescan=False)
-            
-            packetitem = QtWidgets.QTableWidgetItem(str(stat['numpackets']))
+            stat = self.inspect_data(filename,rescan=False)
+            packetitem = QtWidgets.QTableWidgetItem(str(stat['packets_sent']))
             self.inlist.setItem(i,1,packetitem)
             tdmin = datetime.datetime.fromtimestamp(stat['t_min'])
             tminstr = str(tdmin)
             tdmax = datetime.datetime.fromtimestamp(stat['t_max'])
             tmaxstr = str(tdmax)
             t_min_item = QtWidgets.QTableWidgetItem(tminstr)
             t_max_item = QtWidgets.QTableWidgetItem(tmaxstr)
@@ -310,15 +323,15 @@
         self.update_filenamelist() 
 
     def add_files(self):
         """ Opens a dialog to choose file to add
         """
         funcname = self.__class__.__name__ + '.add_files()'
         logger.debug(funcname)
-        filenames, _ = QtWidgets.QFileDialog.getOpenFileNames(self,"Rawdatafiles","","redvypr raw (*.redvypr_raw);;All Files (*)")
+        filenames, _ = QtWidgets.QFileDialog.getOpenFileNames(self,"Rawdatafiles","","redvypr raw (*.redvypr_yaml);;All Files (*)")
         for f in filenames: 
             self.device.config['files'].append(f)
             
         
         self.update_filenamelist()
         self.inlist.sortItems(0, QtCore.Qt.AscendingOrder)
             
@@ -368,26 +381,27 @@
             logger.debug(funcname + "button pressed")
             self.resort_files()
             loop = self.loop_checkbox.isChecked()
             # Loop
             self.device.config['loop']    = loop
             # Speedup
             self.device.config['speedup'] = float(self.speedup_edit.text())
-            self.device_start.emit(self.device)
+            self.device.thread_start()
         else:
             logger.debug(funcname + 'button released')
-            self.device_stop.emit(self.device)
+            self.device.thread_stop()
 
             
-    def thread_status(self,status):
-        self.update_buttons(status['threadalive'])
-        
-    def update_buttons(self,thread_status):
+    def update_buttons(self):
             """ Updating all buttons depending on the thread status (if its alive, graying out things)
             """
+
+            status = self.device.get_thread_status()
+            thread_status = status['thread_status']
+
             # Running
             if(thread_status):
                 self.startbtn.setText('Stop')
                 self.startbtn.setChecked(True)
                 for w in self.config_widgets:
                     w.setEnabled(False)
             # Not running
@@ -399,31 +413,42 @@
                 # Check if an error occured and the startbutton 
                 if(self.startbtn.isChecked()):
                     self.startbtn.setChecked(False)
                 #self.conbtn.setEnabled(True)
 
 
 class displayDeviceWidget(QtWidgets.QWidget):
-    def __init__(self):
+    def __init__(self,device=None):
         super(QtWidgets.QWidget, self).__init__()
         layout          = QtWidgets.QVBoxLayout(self)
-        hlayout         = QtWidgets.QHBoxLayout()        
+        hlayout         = QtWidgets.QHBoxLayout()
+        self.device     = device
         self.text       = QtWidgets.QPlainTextEdit(self)
         self.text.setReadOnly(True)
         self.filelab= QtWidgets.QLabel("File: ")
         self.byteslab   = QtWidgets.QLabel("Bytes written: ")
         self.packetslab = QtWidgets.QLabel("Packets written: ")
         self.text.setMaximumBlockCount(10000)
         hlayout.addWidget(self.byteslab)
         hlayout.addWidget(self.packetslab)
         layout.addWidget(self.filelab)        
         layout.addLayout(hlayout)
         layout.addWidget(self.text)
-        #self.text.insertPlainText("hallo!")        
-
-    def update(self,data):
-        #print('data',data)
-        self.filelab.setText("File: {:s}".format(data['filename']))        
-        self.byteslab.setText("Bytes written: {:d}".format(data['bytes_written']))
-        self.packetslab.setText("Packets written: {:d}".format(data['packets_written']))
-        self.text.insertPlainText(str(data['data']))
+        #self.text.insertPlainText("hallo!")
+        self.statustimer = QtCore.QTimer()
+        self.statustimer.timeout.connect(self.update)
+        self.statustimer.start(500)
+
+    def update(self):
+        statusqueue = self.device.statusqueue
+        while (statusqueue.empty() == False):
+            try:
+                data = statusqueue.get(block=False)
+            except:
+                break
+
+            self.text.insertPlainText(str(data) + '\n')
+
+        #self.byteslab.setText("Bytes written: {:d}".format(data['bytes_written']))
+        #self.packetslab.setText("Packets written: {:d}".format(data['packets_written']))
+        #self.text.insertPlainText(str(data['data']))
```

### Comparing `redvypr-0.4.4/redvypr/files.py` & `redvypr-0.5.3/redvypr/files.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v02.ico` & `redvypr-0.5.3/redvypr/icon/icon_v02.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v02.png` & `redvypr-0.5.3/redvypr/icon/icon_v02.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.1.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.1.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.1.svg` & `redvypr-0.5.3/redvypr/icon/icon_v03.1.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.1_small.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.1_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2.ico` & `redvypr-0.5.3/redvypr/icon/icon_v03.2.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.2.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2.svg` & `redvypr-0.5.3/redvypr/icon/icon_v03.2.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2_favicon.ico` & `redvypr-0.5.3/redvypr/icon/icon_v03.2_favicon.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2_small.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.2_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.2_verysmall.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.2_verysmall.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.png` & `redvypr-0.5.3/redvypr/icon/icon_v03.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/icon_v03.svg` & `redvypr-0.5.3/redvypr/icon/icon_v03.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_merged.svg` & `redvypr-0.5.3/redvypr/icon/logo_merged.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v01.svg` & `redvypr-0.5.3/redvypr/icon/logo_v01.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v02.svg` & `redvypr-0.5.3/redvypr/icon/logo_v02.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v03.1.png` & `redvypr-0.5.3/redvypr/icon/logo_v03.1.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v03.1.svg` & `redvypr-0.5.3/redvypr/icon/logo_v03.1.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v03.2.svg` & `redvypr-0.5.3/redvypr/icon/logo_v03.2.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/logo_v03.2_small.png` & `redvypr-0.5.3/redvypr/icon/logo_v03.2_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/icon/redvypr_logo_v02.png` & `redvypr-0.5.3/redvypr/icon/redvypr_logo_v02.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr/redvypr.py` & `redvypr-0.5.3/redvypr/redvypr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,1697 +1,1697 @@
-import serial
-import serial.tools
+import copy
 import os
 import time
 import datetime
 import logging
 import queue
 import sys
 import yaml
 import pkg_resources
 from PyQt5 import QtWidgets, QtCore, QtGui
-import pyqtgraph as pg
-import numpy as np
 import inspect
 import threading
 import multiprocessing
-import redvypr.devices as redvyprdevices
-from redvypr.data_packets import device_in_data, get_devicename_from_data, get_datastreams_from_data, parse_devicestring, do_data_statistics, create_data_statistic_dict
-from redvypr.gui import redvyprConnectWidget,QPlainTextEditLogger,displayDeviceWidget_standard,deviceinfoWidget,redvypr_devicelist_widget
-from redvypr.utils import addrm_device_as_data_provider,get_data_receiving_devices,get_data_providing_devices
 import socket
 import argparse
 import importlib.util
 import glob
 import pathlib
 import signal
 import uuid
+import random
+from pyqtconsole.console import PythonConsole
+from pyqtconsole.highlighter import format
+import platform
+# Import redvypr specific stuff
+import redvypr.data_packets as data_packets
+from redvypr.gui import redvypr_ip_widget, QPlainTextEditLogger, displayDeviceWidget_standard, \
+    deviceinfoWidget, datastreamWidget, redvypr_deviceInitWidget, redvypr_deviceInfoWidget
+import redvypr.gui as gui
+from redvypr.config import configuration
+import redvypr.config as redvyprconfig
 from redvypr.version import version
 import redvypr.files as files
+from redvypr.device import redvypr_device, redvypr_device_scan
+import redvypr.devices as redvyprdevices
+import faulthandler
+faulthandler.enable()
 
-from pyqtconsole.console import PythonConsole
-from pyqtconsole.highlighter import format
+# Platform information str
+__platform__ = "redvypr (REaltime Data Vi(Y)ewer and PRocessor (in Python))\n"
+__platform__ += "\n\n"
+__platform__ += "Version: {:s}\n".format(str(version))
+__platform__ += "Python: {:s}\n".format(sys.version)
+__platform__ += "Platform system: {:s}\n".format(platform.system())
+__platform__ += "Platform release: {:s}\n".format(platform.release())
+__platform__ += "Platform version: {:s}\n".format(platform.version())
 
 # Windows icon fix
 # https://stackoverflow.com/questions/1551605/how-to-set-applications-taskbar-icon-in-windows-7/1552105#1552105
 import ctypes
-myappid = u'redvypr.redvypr.version' # arbitrary string
+
+myappid = u'redvypr.redvypr.version'  # arbitrary string
 try:
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 except:
     pass
 
-
 _logo_file = files.logo_file
 _icon_file = files.icon_file
-    
-    
+
 # The maximum size the dataqueues have, this should be more than
 # enough for a "normal" usage case
 queuesize = 10000
-#queuesize = 10
+# queuesize = 10
 
 logging.basicConfig(stream=sys.stderr)
 logger = logging.getLogger('redvypr')
-logger.setLevel(logging.DEBUG)
+logger.setLevel(logging.INFO)
+
 
-#https://stackoverflow.com/questions/166506/finding-local-ip-addresses-using-pythons-stdlib
+# https://stackoverflow.com/questions/166506/finding-local-ip-addresses-using-pythons-stdlib
 def get_ip():
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't even have to be reachable
         s.connect(('10.255.255.255', 1))
         IP = s.getsockname()[0]
     except Exception:
         IP = '127.0.0.1'
     finally:
         s.close()
     return IP
 
+
 # The hostinfo, to distinguish between different redvypr instances
-hostinfo = {'hostname':'redvypr','tstart':time.time(),'addr':get_ip(),'uuid':str(uuid.uuid1()),'local':True}
+# redvyprid = str(uuid.uuid1()) # Old
+
+def create_hostinfo(hostname='redvypr'):
+    funcname = __name__ + '.create_hostinfo()'
+    logger.debug(funcname)
+    randstr = '{:03d}'.format(random.randrange(2 ** 8))
+    #redvyprid = datetime.datetime.now().strftime('%Y%m%d%H%M%S.%f-') + str(uuid.getnode()) + '-' + randstr
+    redvyprid = str(uuid.getnode()) + '-' + randstr
+    hostinfo = {'hostname': hostname, 'tstart': time.time(), 'addr': get_ip(), 'uuid': redvyprid, 'local': True}
+    return hostinfo
+
+
+
 
-def distribute_data(devices,infoqueue,dt=0.01):
+def distribute_data(devices, hostinfo, deviceinfo_all, infoqueue, redvyprqueue, dt=0.01):
     """ The heart of redvypr, this functions distributes the queue data onto the subqueues.
     """
     funcname = __name__ + '.distribute_data()'
-    dt_info = 1.0 # The time interval information will be sent
-    dt_avg = 0 # Averaging of the distribution time needed
-    navg = 0    
+    datastreams_all = {}
+    datastreams_all_old = {}
+    dt_info = 5.0  # The time interval information will be sent
+    dt_avg = 0  # Averaging of the distribution time needed
+    navg = 0
+    packets_processed = 0 # For statistics, count packets
     tinfo = time.time()
     tstop = time.time()
     dt_sleep = dt
+
+
     while True:
         time.sleep(dt_sleep)
         tstart = time.time()
+        FLAG_device_status_changed = False
+        devices_changed = []
+        devices_removed = []
+        # Read data from the main thread
+        try:
+            redvyprdata = redvyprqueue.get(block=False) # Data from the main thread
+        except Exception as e:
+            redvyprdata = None
+        # Process data from the main thread
+        if(redvyprdata is not None):
+            if(redvyprdata['type'] == 'device_removed'):
+                print('Device removed',redvyprdata)
+                FLAG_device_status_changed = True
+                devices_removed.append(redvyprdata['device'])
+                devinfo_rem = deviceinfo_all.pop(redvyprdata['device'])
+                #print('Devices len distribute data', len(devices))
+                devinfo_send = {'type':'deviceinfo_all', 'deviceinfo_all': copy.deepcopy(deviceinfo_all), 'devices_changed': list(set(devices_changed)),
+                'devices_removed': devices_removed,'change':'devrem','device_changed':redvyprdata['device']}
+                infoqueue.put_nowait(devinfo_send)
+
+
         for devicedict in devices:
             device = devicedict['device']
+            data_all = []
+            tread = time.time()
+            # Read all packets in a bunch
             while True:
                 try:
                     data = device.dataqueue.get(block=False)
-                    devicedict['numpacket'] += 1
+                    if(type(data) is not dict): # If data is not a dictionary, convert it to one
+                        data = {'data':data}
+
+                    devicedict['packets_sent'] += 1
+                    packets_processed += 1
+                    data_all.append(data)
                 except Exception as e:
                     break
-
-                # Add deviceinformation to the data package
-                if('device' not in data.keys()):
-                    data['device']   = str(device.name)
-                    data['host']     = hostinfo
-                else: # Check if we have a local data packet, i.e. a packet that comes from another redvypr instance with another UUID
-                    data['host']['local']    = data['host']['uuid'] == hostinfo['uuid']
-                    
-                # Add the time to the datadict if its not already in
-                if('t' not in data.keys()):
-                    data['t'] = tstart
-
-                # Add the packetnumber to the datadict
-                if('numpacket' not in data.keys()):
-                    data['numpacket'] = devicedict['numpacket']
-
+            # Process read packets
+            for data in data_all:
+                #
+                # Add additional information, if not present yet
+                data_packets.treat_datadict(data, device.name, hostinfo, devicedict['packets_sent'], tread,devicedict['devicemodulename'])
+                # Get the devicename
+                devicename_stat = data_packets.get_devicename_from_data(data, uuid=True)
+                #
+                # Do statistics
                 try:
                     if devicedict['statistics']['inspect']:
-                        devicedict['statistics'] = do_data_statistics(data,devicedict['statistics'])
-                        if False:
-                            devicedict['statistics']['numpackets'] += 1
-                            # Create a unique list of datakeys
-                            devicedict['statistics']['datakeys'] = list(set(devicedict['statistics']['datakeys'] + list(data.keys())))
-                            # Create a unqiue list of devices, device can
-                            # be different from the transporting device,
-                            # i.e. network devices do not change the name
-                            # of the transporting dictionary
-                            devicename_stat  = get_devicename_from_data(data,uuid=True)
-                            try:
-                                devicedict['statistics']['devicekeys'][devicename_stat]
-                            except:
-                                devicedict['statistics']['devicekeys'][devicename_stat] = []
-                                
-                            devicedict['statistics']['devicekeys'][devicename_stat] = list(set(devicedict['statistics']['devicekeys'][devicename_stat] + list(data.keys())))
-                            devicedict['statistics']['devices'] = list(set(devicedict['statistics']['devices'] + [devicename_stat]))
-                            datastreams_stat = get_datastreams_from_data(data,uuid=True)
-                            devicedict['statistics']['datastreams'] = list(set(devicedict['statistics']['datastreams'] + datastreams_stat))
+                        devicedict['statistics'] = data_packets.do_data_statistics(data, devicedict['statistics'])
                 except Exception as e:
+                    logger.exception(e)
                     logger.debug(funcname + ':Statistics:' + str(e))
 
-                if True:
-                    # Feed the data into the modules/functions/objects and
-                    # let them treat the data
-                    for dataout in devicedict['dataout']:
-                        devicedict['numpacketout'] += 1
+                #
+                # Check for a command packet
+                #
+                numtag = data['_redvypr']['tag'][hostinfo['uuid']]
+                if numtag < 2:  # Check if data packet fits with addr and its not recirculated again
+                    [command, comdata] = data_packets.check_for_command(data, add_data=True)
+                    if (command == 'device_status'):  # status update
+                        #print('device status command',device.name)
+                        #print('comdata',comdata)
+                        #print('data', data)
                         try:
-                            dataout.put_nowait(data)
-                        except Exception as e:
-                            logger.debug(funcname + ':dataout of :' + devicedict['device'].name + ' full: ' + str(e))
-                    for guiqueue in devicedict['guiqueue']: # Put data into the guiqueue, this queue does always exist
-                        try:                        
-                            guiqueue.put_nowait(data)
-                        except Exception as e:
-                            pass
-                            #logger.debug(funcname + ':guiqueue of :' + devicedict['device'].name + ' full')
+                            devaddr   = comdata['data']['deviceaddr']
+                            devstatus = comdata['data']['devicestatus']
+                        except:
+                            devaddr = None
+                            devstatus = None
+
+                        devices_changed.append(device.name) # LEGACY ...
+                        if(devaddr is not None):
+                            try: # Update the device
+                                devicedict['statistics']['device_redvypr'][devaddr]['_redvypr'].update(devstatus)
+                            except Exception as e:
+                                logger.warning('Could not update status ' + str(e))
+                                logger.exception(e)
+
+                        # Send an information about the change, that will trigger an pyqt signal in the main thread
+                        devinfo_send = {'type': 'deviceinfo_all', 'deviceinfo_all': copy.deepcopy(deviceinfo_all),
+                                        'devices_changed': list(set(devices_changed)), 'device_changed':device.name,
+                                        'devices_removed': devices_removed, 'change': 'device_status command','comdata':comdata}
+                        infoqueue.put_nowait(devinfo_send)
+
+                #
+                # Create a dictionary of all datastreams
+                #
+                datastreams_all.update(devicedict['statistics']['datastream_redvypr'])
+                try:
+                    deviceinfo_all[device.name].update(devicedict['statistics']['device_redvypr'])
+                except:
+                    deviceinfo_all[device.name] = devicedict['statistics']['device_redvypr']
+
+                #
+                # Compare if datastreams changed
+                #
+                if (list(datastreams_all.keys()) != list(datastreams_all_old.keys())):
+                    #print('Datastreams changed', len(datastreams_all.keys()))
+                    datastreams_all_old.update(datastreams_all)
+                    devices_changed.append(device.name)
+                    # Send an information about the change, that will trigger an pyqt signal in the main thread
+                    devinfo_send = {'type': 'deviceinfo_all', 'deviceinfo_all': copy.deepcopy(deviceinfo_all),
+                                    'devices_changed': list(set(devices_changed)),
+                                    'devices_removed': devices_removed, 'change': 'datastreams changed','device_changed':device.name}
+                    infoqueue.put_nowait(devinfo_send)
+
+                #
+                # And finally: Distribute the data
+                #
+                for devicedict_sub in devices:
+                    devicesub = devicedict_sub['device']
+                    if(devicesub == device): # Not to itself
+                        continue
+
+                    for addr in devicesub.subscribed_addresses: # Loop over all subscribed redvypr_addresses
+                        # This is the main functionality for sitribution, comparing a datapacket with a
+                        # redvypr_address using "in"
+                        if (data in addr) and (numtag < 2): # Check if data packet fits with addr and if its not recirculated again
+                            try:
+                                devicesub.datainqueue.put_nowait(data) # These are the datainqueues of the subscribing devices
+                                devicedict['packets_received'] += 1
+                                devicedict['statistics']['device_redvypr'][devicename_stat]['packets_received'] += 1
+                                break
+                            except Exception as e:
+                                logger.debug(funcname + ':dataout of :' + devicedict['device'].name + ' full: ' + str(e))
+
+                # The gui of the device
+                for guiqueue in devicedict['guiqueue']:  # Put data into the guiqueue, this queue does always exist
+                    try:
+                        guiqueue.put_nowait(data)
+                    except Exception as e:
+                        pass
+                        # logger.debug(funcname + ':guiqueue of :' + devicedict['device'].name + ' full')
+
+        #if FLAG_device_status_changed:
+            #infoqueue.put_nowait(copy.copy(datastreams_all))
+            #devinfo_send = {'type':'deviceinfo_all', 'deviceinfo_all': copy.deepcopy(deviceinfo_all), 'devices_changed': list(set(devices_changed)),
+            # 'devices_removed': devices_removed,''}
+            #infoqueue.put_nowait(devinfo_send)
 
         # Calculate the sleeping time
-        tstop = time.time()        
-        dt_dist = tstop - tstart # The time for all the looping
+        tstop = time.time()
+        dt_dist = tstop - tstart  # The time for all the looping
         dt_avg += dt_dist
         navg += 1
-        dt_sleep = max([0,dt - dt_dist])
-        if((tstop - tinfo) > dt_info):
+        dt_sleep = max([0, dt - dt_dist])
+        if ((tstop - tinfo) > dt_info):
             tinfo = tstop
-            info_dict = {'dt_avg':dt_avg/navg}
-            #print(info_dict)
-            infoqueue.put_nowait(info_dict)
-            
-            
-
-
+            info_dict = {'type':'dt_avg','dt_avg': dt_avg / navg,'packets_processed': packets_processed}
+            packets_processed = 0
+            # print(info_dict)
+            try:
+                infoqueue.put_nowait(info_dict)
+            except:
+                pass
 
 
 class redvypr(QtCore.QObject):
     """This is the redvypr heart. Here devices are added/threads
     are started and data is interchanged
 
     """
-    device_path_changed = QtCore.pyqtSignal() # Signal notifying if the device path was changed
-    device_added        = QtCore.pyqtSignal(list) # Signal notifying if the device path was changed
-    devices_connected   = QtCore.pyqtSignal(str,str) # Signal notifying if two devices were connected
-    def __init__(self,parent=None,config=None,nogui=False):
-        #super(redvypr, self).__init__(parent)
+    device_path_changed          = QtCore.pyqtSignal()  # Signal notifying if the device path was changed
+    device_added                 = QtCore.pyqtSignal(list)  # Signal notifying that a device was added
+    device_removed               = QtCore.pyqtSignal()  # Signal notifying that a device was removed
+    devices_connected            = QtCore.pyqtSignal(str, str)  # Signal notifying if two devices were connected
+    devices_disconnected         = QtCore.pyqtSignal(str, str)  # Signal notifying if two devices were connected
+    status_update_signal         = QtCore.pyqtSignal()  # Signal notifying if the status of redvypr has been changed
+    device_status_changed_signal = QtCore.pyqtSignal()  # Signal notifying if datastreams have been added
+    hostconfig_changed_signal    = QtCore.pyqtSignal()  # Signal notifying if the configuration of the host changed (hostname, hostinfo_opt)
+
+    def __init__(self, parent=None, config=None, hostname='redvypr',hostinfo_opt = {}, nogui=False):
+        # super(redvypr, self).__init__(parent)
         super(redvypr, self).__init__()
-        funcname = __name__ + '.__init__()'                                
+        print(__platform__)
+        funcname = __name__ + '.__init__()'
         logger.debug(funcname)
-        self.config = {} # Might be overwritten by parse_configuration()
+        self.hostinfo = create_hostinfo(hostname=hostname)
+        print('Hostinfo opt',hostinfo_opt)
+        try:
+            hostinfo_opt['description']
+        except:
+            hostinfo_opt['description'] = ''
+
+        try:
+            hostinfo_opt['location']
+        except:
+            hostinfo_opt['location'] = ''
+
+        try:
+            hostinfo_opt['lon']
+        except:
+            hostinfo_opt['lon'] = -9999.0
+
+        try:
+            hostinfo_opt['lat']
+        except:
+            hostinfo_opt['lat'] = -9999.0
+
+        self.hostinfo_opt = configuration(template=hostinfo_opt)
+
+        self.config = {}  # Might be overwritten by parse_configuration()
+        self.properties = {}  # Properties that are distributed with the device
         self.numdevice = 0
-        self.devices        = [] # List containing dictionaries with information about all attached devices
-        self.device_paths   = [] # A list of pathes to be searched for devices
-        self.device_modules = []        
-        
+        self.devices = []  # List containing dictionaries with information about all attached devices
+        self.device_paths = []  # A list of pathes to be searched for devices
+        self.datastreams_dict = {} # Information about all datastreams, this is updated by distribute data
+        self.deviceinfo_all   = {} # Information about all devices, this is updated by distribute data
+
+
+
+        self.dt_datadist = 0.01  # The time interval of datadistribution
+        self.dt_avg_datadist = 0.00  # The time interval of datadistribution
+        self.datadistinfoqueue = queue.Queue(maxsize=1000)  # A queue to get informations from the datadistthread
+        self.redvyprqueue = queue.Queue()  # A queue to send informations to the datadistthread
+        # Lets start the distribution!
+        self.datadistthread = threading.Thread(target=distribute_data, args=(
+        self.devices, self.hostinfo, self.deviceinfo_all, self.datadistinfoqueue, self.redvyprqueue, self.dt_datadist), daemon=True)
+        self.datadistthread.start()
+        logger.info(funcname + ':Searching for devices')
+        self.redvypr_device_scan = redvypr_device_scan(device_path = self.device_paths,redvypr_devices=redvyprdevices)
+        logger.info(funcname + ':Done searching for devices')
+
+        # Parsing configuration
+        self.parse_configuration(config)
+
         ## A timer to check the status of all threads
         self.devicethreadtimer = QtCore.QTimer()
-        self.devicethreadtimer.timeout.connect(self.update_devices_thread_status)
-        self.devicethreadtimer.start(500)
+        self.devicethreadtimer.timeout.connect(self.update_status)  # Add to the timer another update
+        self.devicethreadtimer.start(250)
 
 
         ## A timer to print the status in the nogui environment
-        if(nogui):
+        if (nogui):
             self.statustimer = QtCore.QTimer()
             self.statustimer.timeout.connect(self.print_status)
-            self.statustimer.start(5000)        
-        
+            self.statustimer.start(5000)
 
-        self.dt_datadist = 0.01 # The time interval of datadistribution
-        self.dt_avg_datadist = 0.00 # The time interval of datadistribution        
-        self.datadistinfoqueue = queue.Queue(maxsize=1000) # A queue to get informations from the datadistribution
-        self.datadistthread = threading.Thread(target=distribute_data, args=(self.devices,self.datadistinfoqueue,self.dt_datadist), daemon=True)
-        self.datadistthread.start()
-        logger.info(funcname + ':Searching for devices')
-        self.populate_device_path()
-        logger.info(funcname + ':Done searching for devices')
+    def get_deviceinfo(self,publishes=None,subscribes=None):
+        """
+
+        Args:
+            publishes:
+            subscribes:
+
+        Returns:
+            A dictionary containing the deviceinfo of all devices seen by this redvypr instance
+        """
+        if (publishes == None) and (subscribes == None):
+            return copy.deepcopy(self.deviceinfo_all)
+        else:
+            dinfo = {}
+            for d in self.devices:
+                dev = d['device']
+                FLAG_publishes   =   (publishes == dev.publishes) or (publishes == None)
+                FLAG_subscribes  = (subscribes == dev.subscribes) or (subscribes == None)
+                if FLAG_publishes and FLAG_subscribes:
+                    dinfo[dev.name] = copy.deepcopy(dev.statistics['device_redvypr'])
+
+            return dinfo
+
+    def update_status(self):
+        funcname = __name__ + '.update_status():'
+        # Check if the distribution thread is running, if not warn the user
+        if self.datadistthread.is_alive() == False:
+            logger.warning('Datadistribution thread is not running! This is bad, consider restarting redvypr.')
+            self.status_update_signal.emit()
+            return
+
+        while True:
+            try: # Reading data coming from distribute_data thread
+                data = self.datadistinfoqueue.get(block=False)
+                #print('Got data',data)
+                if('dt_avg' in data['type']):
+                    self.dt_avg_datadist   = data['dt_avg']
+                    self.packets_processed = data['packets_processed']
+                    self.status_update_signal.emit()
+                elif ('deviceinfo_all' in data['type']):
+                    data.pop('type')  # Remove the type key
+                    # Store the data of the changed devices
+                    self.__device_status_changed_data__ = data
 
-        # Configurating redvypr
-        if(config is not None):
-            logger.debug(funcname + ':Configuration: ' + str(config))
-            if(type(config) == str):
-                config = [config]
-
-            for c in config:
-                logger.debug(funcname + ':Parsing configuration: ' + str(c))
-                self.parse_configuration(c)
+                    #print('datastreams changed', data)
+                    self.device_status_changed_signal.emit()
+
+            except Exception as e:
+                #logger.exception(e)
+                break
 
     def print_status(self):
         funcname = __name__ + '.print_status():'
-        print(funcname + self.status())
+        logger.debug(funcname + self.status())
 
     def status(self):
         """ Creates a statusstr of the devices
         """
         tstr = str(datetime.datetime.now())
-        statusstr = "{:s}, {:s}, num devices {:d}".format(tstr, hostinfo['hostname'], len(self.devices))
-        
+        statusstr = "{:s}, {:s}, num devices {:d}".format(tstr, self.hostinfo['hostname'], len(self.devices))
+
         for sendict in self.devices:
-            try:
-                running = sendict['thread'].is_alive()
+            status = sendict['device'].get_thread_status()
+            #info_dict['uuid'] = self.uuid
+            #info_dict['thread_uuid'] = self.thread_uuid
+            #info_dict['thread_status'] = running
+            if(status['thread_status']):
                 runstr = 'running'
-            except:
-                running = False
-                runstr = 'stopped'    
+            else:
+                runstr = 'stopped'
 
-            statusstr += '\n\t' + sendict['device'].name + ':' + runstr + ': data packets: {:d}'.format(sendict['numpacket'])
-            #statusstr += ': data packets received: {:d}'.format(sendict['numpacketout'])
+            statusstr += '\n\t' + sendict['device'].name + ':' + runstr + ': data packets sent: {:d}' + ': data packets received: {:d}'.format(
+                sendict['packets_sent'],sendict['packets_received'])
+            # statusstr += ': data packets received: {:d}'.format(sendict['numpacketout'])
 
         return statusstr
 
-
-    def update_devices_thread_status(self):
-        """ This function is called regularly to check the status of the threads
+    def get_config(self):
         """
-        # Check the datadistribution statistics
-        datainfo = []
-        while True:
-            try:
-                data = self.datadistinfoqueue.get(block=False)
-                datainfo.append(data)
-                self.dt_avg_datadist = data['dt_avg']
+        Creates a configuration dictionary out of the current state.
 
-            except Exception as e:
-                break
+        Returns:
+            config: configuration dictionary
 
-        # Check the devicethreadstatusses
-        for sendict in self.devices:
-            # Update the device and the devicewidgets about the thread status
-            if(sendict['thread'] is not None):
-                running2 = sendict['thread'].is_alive()
-                try: # If the device has a thread_status function
-                    device.thread_status({'threadalive':running2})
-                except:
-                    pass
+        """
+        config = {}
 
-                # Tell it deviceinfos
-                try: # GUI?
-                    sendict['infowidget'].thread_status({'threadalive':running2})
-                except Exception as e:
-                    pass                    
-                # Go tell it to the widgets
-                try: # If the device has a thread_status function
-                    sendict['initwidget'].thread_status({'threadalive':running2})
-                except Exception as e:
-                    pass
-                    #print('Start thread exception:' + str(e))
+        config['hostname']     = self.hostinfo['hostname']
+        config['hostinfo_opt'] = copy.deepcopy(self.hostinfo_opt)
+        config['devicepath']   = []
+        for p in self.device_paths:
+            config['devicepath'].append(p)
+        # Loglevel
+        config['loglevel'] = logger.level
+        # Devices
+        config['devices'] = []
+        for devicedict in self.devices:
+            device = devicedict['device']
+            devsave = {'deviceconfig':{}}
+            devsave['deviceconfig']['name']     = device.name
+            devsave['deviceconfig']['loglevel'] = device.loglevel
+            devsave['deviceconfig']['autostart'] = device.autostart
 
+            devsave['devicemodulename']         = devicedict['devicemodulename']
+            devconfig = device.config
+            devsave['deviceconfig']['config'] = copy.deepcopy(devconfig)
+            # Treat subscriptions
+            devsave['deviceconfig']['subscriptions'] = []
+            for raddr in device.subscribed_addresses:
+                devsave['deviceconfig']['subscriptions'].append(raddr.address_str)
 
-                for guiwidget in sendict['gui']:
-                        try: # If the device has a thread_status function
-                            guiwidget.thread_status({'threadalive':running2})
-                        except Exception as e:
-                            pass
-                            #print('Start thread exception:' + str(e))
+            config['devices'].append(devsave)
 
 
+        return config
 
-    def parse_configuration(self,configfile=None):
+    def parse_configuration(self, redvypr_config=None):
         """ Parses a dictionary with a configuration, if the file does not exists it will return with false, otherwise self.config will be updated
 
         Arguments:
-            configfile (str or dict):
+            redvypr_config (str, dict or list of strs and dicts):
         Returns:
             True or False
         """
         funcname = "parse_configuration()"
+        parsed_devices = []
         logger.debug(funcname)
-        if(type(configfile) == str):
-            logger.info(funcname + ':Opening yaml file: ' + str(configfile))
-            if(os.path.exists(configfile)):
-                fconfig = open(configfile)
-                config = yaml.load(fconfig, Loader=yaml.loader.SafeLoader)
-            else:
-                logger.warning(funcname + ':Yaml file: ' + str(configfile) +  ' does not exist!')
-                return False
-        elif(type(configfile) == dict):
-            logger.info(funcname + ':Opening dictionary')
-            config = configfile
+
+        if (redvypr_config is not None):
+            logger.debug(funcname + ':Configuration: ' + str(redvypr_config))
+            if (type(redvypr_config) == str):
+                redvypr_config = [redvypr_config]
         else:
-            logger.warning(funcname + ':This shouldnt happen')
+            return False
 
+        config = {} # This is a merged config of all configurations
+        for configraw in redvypr_config:
+            if (type(configraw) == str):
+                logger.info(funcname + ':Opening yaml file: ' + str(configraw))
+                if (os.path.exists(configraw)):
+                    fconfig = open(configraw)
+                    config_tmp = yaml.load(fconfig, Loader=yaml.loader.SafeLoader)
+                else:
+                    logger.warning(funcname + ':Yaml file: ' + str(configraw) + ' does not exist!')
+                    continue
+            elif(type(configraw) == dict):
+                logger.info(funcname + ':Opening dictionary')
+                config_tmp = configraw
+            else:
+                logger.warning(funcname + ': Unknown type of configuration {:s}'.format(type(configraw)))
+                continue
 
-        self.config = config
-        # Add device path if found
-        if('devicepath' in config.keys()):
-            devpath = config['devicepath']
+            # Merge the configuration into one big dictionary
+            config.update(config_tmp)
 
-            if(type(devpath) == str):
-                devpath = [devpath]
+        # Apply the merged configuration
+        if True:
+            #self.config = config
+            if ('loglevel' in config.keys()):
+                logger.setLevel(config['loglevel'])
+            # Add device path if found
+            if ('devicepath' in config.keys()):
+                devpath = config['devicepath']
+
+                if (type(devpath) == str):
+                    devpath = [devpath]
+
+                FLAG_NEW_DEVPATH=False
+                for p in devpath:
+                    if (p not in self.device_paths):
+                        self.device_paths.append(p)
+                        FLAG_NEW_DEVPATH = True
+
+                if FLAG_NEW_DEVPATH:
+                    self.redvypr_device_scan.scan_devicepath()
+                    self.device_path_changed.emit()  # Notify about the changes
 
-            for p in devpath:
-                if(p not in self.device_paths):
-                    self.device_paths.append(p)
+            # Check for hostinformation
+            # Add the hostname
+            try:
+                logger.info(funcname + ': Setting hostname to {:s}'.format(config['hostname']))
+                self.hostinfo['hostname'] = config['hostname']
+            except:
+                pass
 
-            self.populate_device_path()
-            self.device_path_changed.emit() # Notify about the changes
+            try:
+                logger.info(funcname + ': Setting optional hostinfomation: {:s}'.format(str(config['hostinfo_opt'])))
+                c = redvyprconfig.dict_to_configDict(config['hostinfo_opt'])
+                self.hostinfo_opt.update(c)
+            except Exception as e:
+                #logger.exception(e)
+                pass
 
 
-            
-        # Adding the devices found in the config ['devices']
-        # Check if we have a list or something
-        try:
-            iter(config['devices'])
-            hasdevices = True
-        except:
-            hasdevices = False        
-        if(hasdevices):
-            for device in config['devices']:
-                try:
-                    device['deviceconfig']
-                except:
-                    device['deviceconfig'] = {}
-                    
-                self.add_device(devicemodulename=device['devicemodulename'],deviceconfig=device['deviceconfig'])
+            # Adding the devices found in the config ['devices']
+            # Check if we have a list or something
+            try:
+                iter(config['devices'])
+                hasdevices = True
+            except:
+                hasdevices = False
+            if (hasdevices):
+                for device in config['devices']:
+                    try:
+                        device['deviceconfig']
+                    except:
+                        device['deviceconfig'] = {}
 
-        # Connecting devices ['connections']
-        try:
-            iter(config['connections'])
-            hascons = True
-        except:
-            hascons = False        
-        if(hascons):        
-            logger.debug('Connecting devices')
-            for con in config['connections']:
-                logger.debug('Connecting devices:' + str(con))
-                devicenameprovider = con['publish']    
-                devicenamereceiver = con['receive']
-                indprovider = -1
-                indreceiver = -1
-                for i,s in enumerate(self.devices):
-                    if s['device'].name == devicenameprovider:
-                       deviceprovider = s['device']
-                       indprovider = i 
-                    if s['device'].name == devicenamereceiver:
-                       devicereceiver = s['device']
-                       indreceiver = i 
-
-                if((indprovider > -1) and (indreceiver > -1)):
-                    self.addrm_device_as_data_provider(deviceprovider,devicereceiver,remove=False)
-                    sensprov = get_data_providing_devices(self.devices,devicereceiver)
-                    sensreicv = get_data_receiving_devices(self.devices,deviceprovider)
-                    #print('provider',devicereceiver,sensprov)            
-                    #print('receiver',deviceprovider,sensreicv)            
-                    #print('provider',self.devices[indprovider])#,deviceprovider)
-                    #print('receiver',self.devices[indreceiver])
-                    #print(devicereceiver)
-                else:
-                    logger.warning(funcname + ':Could not create connection for devices: {:s} and {:s}'.format(devicenameprovider,devicenamereceiver))
+                    # Check if the devicemodulename kind of fits
+                    FLAG_MOD_DEVICEMODULENAME = True
+                    for smod in self.redvypr_device_scan.redvypr_devices_flat:
+                        if (device['devicemodulename'] == smod['name']):
+                            FLAG_MOD_DEVICEMODULENAME = False
+
+                    if FLAG_MOD_DEVICEMODULENAME:
+                        for smod in self.redvypr_device_scan.redvypr_devices_flat:
+                            if (device['devicemodulename'] in smod['name']): # This is a weaker test, can be potentially replaced by regex
+                                device['devicemodulename_orig'] = device['devicemodulename']
+                                device['devicemodulename'] = smod['name']
+
+                    dev_added = self.add_device(devicemodulename=device['devicemodulename'], deviceconfig=device['deviceconfig'])
+
+                    # Subscriptions
+                    # Name
+                    #
+                    parsed_devices.append(dev_added)
+
+
+            # Autostart the device, if wanted
+            #for dev in parsed_devices:
+            #    device = dev[0]['device']
+            #    if(device.autostart):
+            #        device.thread_start()
 
-        # Add the hostname
-        try:
-            logger.info(funcname + ': Setting hostname to {:s}'.format(config['hostname']))
-            hostinfo['hostname'] = config['hostname']
-        except:
-            pass
-        
-        if('start' in config.keys()):
-            logger.debug('Starting devices')
-            if(config['start'] is not None):
-                for start_device in config['start']:
-                    for s in self.devices:
-                        if(s['device'].name == start_device):
-                            self.start_device_thread(s['device'])
+            # Emit a signal that the configuration has been changed
+        self.hostconfig_changed_signal.emit()
         return True
-    
-    def check_devicename(self,devicename_orig):
-        """
-        Args:
-            devicename_orig:
-            
-        Returns:
-            
-        """
-         
-        return devicename
-
-    def populate_device_path(self):
-        """Searches all device paths for modules and creates a list with the
-        found devices in self.device_modules
-
-        """
-        funcname = 'populate_device_path()'
-        logger.debug(funcname)
-        self.device_modules = [] # Clear the list
-        # Add all devices from additional folders
-        for dpath in self.device_paths:
-            python_files = glob.glob(dpath + "/*.py")
-            logger.debug(funcname + ' will search in path for files: {:s}'.format(dpath))
-            for pfile in python_files:
-                logger.debug(funcname + ' opening {:s}'.format(pfile))
-                module_name = pathlib.Path(pfile).stem
-                spec = importlib.util.spec_from_file_location(module_name, pfile)
-                module = importlib.util.module_from_spec(spec)
-                try:
-                    spec.loader.exec_module(module)
-                except Exception as e:
-                    logger.warning(funcname + ' could not import module: {:s} \nError: {:s}'.format(pfile,str(e)))
-                    
-                module_members = inspect.getmembers(module,inspect.isclass)
-                hasdevice = False
-                try:
-                    module.Device
-                    hasdevice = True      
-                except:
-                    logger.debug(funcname + ' did not find Device class, will skip.')
-                    pass
-
-                if(hasdevice):
-                    devdict = {'module':module,'name':module_name,'source':module.__file__}
-                    self.device_modules.append(devdict)
-
-        # Add all devices from the device module
-        max_tries      = 5000 # The maximum recursion of modules
-        n_tries        = 0
-        testmodules    = [redvyprdevices]
-        device_modules = []
-        while (len(testmodules) > 0) and (n_tries < max_tries):
-            testmodule = testmodules[0]
-            device_module_tmp = inspect.getmembers(testmodule,inspect.ismodule)
-            for smod in device_module_tmp:
-                devicemodule  = getattr(testmodule, smod[0])
-                # Check if the device is valid
-                valid_module  = self.valid_device(devicemodule)
-                if(valid_module['valid']): # If the module is valid add it to devices
-                    devdict   = {'module':devicemodule,'name':smod[0],'source':smod[1].__file__}
-                    self.device_modules.append(devdict)
-                else: # Check recursive if devices are found
-                    n_tries   += 1
-                    testmodules.append(devicemodule)
 
-            testmodules.pop(0)
-    
 
-    def valid_device(self,devicemodule): 
-        """ Checks if the module is a valid redvypr module
-        """
-        funcname = 'valid_device()'
-        logger.debug('Checking device {:s}'.format(str(devicemodule))) 
-        try:
-            devicemodule.Device
-            hasdevice = True
-        except:
-            hasdevice = False
-        
-        try:
-            devicemodule.start
-            hasstart = True
-        except:
-            hasstart = False
-            
-        if(hasstart == False):
-            try:
-                devicemodule.Device.start
-                hasstart = True
-            except:
-                hasstart = False
-            
-        try:
-            devicemodule.displayDeviceWidget
-            hasdisplaywidget = True
-        except:
-            hasdisplaywidget = False
-            
-        try:
-            devicemodule.initDeviceWidget
-            hasinitwidget = True
-        except:
-            hasinitwidget = False
-                          
-        devicecheck = {}
-        devicecheck['valid'] = hasdevice and hasstart                                                 
-        devicecheck['Device'] = hasdevice                                                 
-        devicecheck['start'] = hasstart
-        devicecheck['initgui'] = hasinitwidget
-        devicecheck['displaygui'] = hasdisplaywidget
-        
-        return devicecheck
-    
-    
-    def device_loglevel(self,device,loglevel=None):
+    def device_loglevel(self, device, loglevel=None):
         """ Returns the loglevel of the device
         """
         loglevel = 'NA'
         for d in self.devices:
             if d['devices'] == device:
-                if(d['logger'] is not None):
+                if (d['logger'] is not None):
                     loglevel = d['logger'].getEffectiveLevel()
                     break
-                
+
         return loglevel
-        
 
-    def add_device(self,devicemodulename=None, deviceconfig = None, thread=None):
-        """ Function adds a device
+    def add_device(self, devicemodulename=None, deviceconfig={}, thread=None):
         """
-        funcname = self.__class__.__name__ + '.add_device():' 
-        logger.debug(funcname + ':devicemodule: ' + str(devicemodulename) + ':deviceconfig: ' + str(deviceconfig))
-        devicelist = []
-        device_found = False
-        # Loop over all modules and check of we find the name
-        for smod in self.device_modules:
-           if(devicemodulename == smod['name']):
-              logger.debug('Trying to import device {:s}'.format(smod['name']))
-              devicemodule     = smod['module']
-              # Check for multiprocess options in configuration
-              if(thread == None):
-                  try:
-                      multiprocess = deviceconfig['config']['mp'].lower()
-                  except:
-                      multiprocess = 'thread'
-
-                  if(multiprocess == 'thread'):
-                      thread = True
-                  elif(multiprocess == 'process'):
-                      thread = False
-                  else:
-                      thread = True
-                  
-              devicedict = self.create_devicedict(devicemodule,thread=thread,deviceconfig=deviceconfig)
-              
-              device = devicedict['device']
-              # If the device does not have a name, add a standard but unique one
-              try:
-                  device.name
-              except:
-                  device.name = devicemodulename + '_' + str(self.numdevice)
-
-              # Add the redvypr object to the device itself
-              device.redvypr = self
-              # Link the statistics directly into the device as well    
-              device.statistics = devicedict['statistics']
-              # Add a priori datakeys to the statistics, of the device supports it
-              try:
-                  datakeys = device.get_datakeys()
-                  logger.debug(funcname + 'Adding datakeys received from .get_datakeys(): {:s}'.format(str(datakeys)))
-              except Exception as e:
-                  logger.debug(funcname + 'Device does not have .get_datakeys()')
-                  datakeys = []
-                  
-              device.statistics['datakeys'] = list(set(datakeys))
-              if(len(device.statistics['datakeys'])>0): 
-                  # Add also the datastreams
-                  for dkey in datakeys:
-                      dstream = self.construct_datastream_from_device_datakey(dkey, device)
-                      device.statistics['datastreams'].append(dstream)
-                  
-                  device.statistics['datastreams'] = list(set(device.statistics['datastreams']))
-                  
-              # TODO, change that to datastreams
-              # Check if the device wants a direct start after initialization
-              try:
-                  autostart = device.autostart
-              except:
-                  autostart = False
-
-
-              # Do the loglevel use "standard" to take the loglevel of the redvypr instance
-              try:
-                  loglevel_device = device.loglevel.upper()
-              except: # Use the standard loglevel of redvypr
-                  loglevel_device = "standard"
-
-              # If we have standard 
-              if(loglevel_device == "standard"):
-                  loglevel_device = logger.level
-
-              
-              # If the device has a logger
-              devicedict['logger'] = None 
-              try:
-                  device.logger.setLevel(loglevel_device)
-                  devicedict['logger'] = device.logger
-              except Exception as e:
-                  logger.debug(funcname + ': NA logger device loglevel {:s}'.format(str(e)))
-                  
-
-              # If the module has a logger            
-              try:
-                  devicemodule.logger.setLevel(loglevel_device)
-                  devicedict['logger'] = devicemodule.logger
-              except Exception as e:            
-                  logger.debug(funcname + ': NA logger module loglevel {:s}'.format(str(e)))
-
-
-              # Add the device to the device list
-              self.devices.append(devicedict) # Add the device to the devicelist
-              ind_device = len(self.devices)-1    
-              
-              if(autostart):
-                  logger.debug(funcname + ': Starting device')
-                  self.start_device_thread(device)
-                  
-              devicelist = [devicedict,ind_device,devicemodule]
-              # Finalize the initialization of the device (after the configuration was included)
-              try:
-                  device.finalize_init()
-              except Exception as e:
-                  logger.debug(funcname + ': No finalize_init() of device (Exception: {:s}'.format(str(e)))
-                  
-              self.device_added.emit(devicelist)
-              device_found = True
-              
-              break
+        Function adds a device to redvypr
 
-        if(device_found == False):
-            logger.warning(funcname + ': Could not add device (not found): {:s}'.format(str(devicemodulename)))
-           
-        return devicelist
+        Configuration of the device can have options:
+        template and config:
+        template:
+        config:
 
+        Args:
+            devicemodulename:
+            deviceconfig: A dictionary with the configuration, this is filled by i.e. a yaml file with the configuration or if clicked in the gui just the name of the device
+            thread:
 
-    def create_devicedict(self,devicemodule,devicename = None,thread=False,deviceconfig=None):
-        """Adds a device of type devicemodulename
+        Returns:
+            devicelist: a list containing all devices of this redvypr instance
 
         """
 
-        if thread: # Thread or multiprocess
-            dataqueue        = queue.Queue(maxsize=queuesize)
-            datainqueue      = queue.Queue(maxsize=queuesize)            
-            comqueue         = queue.Queue(maxsize=queuesize)
-            statusqueue      = queue.Queue(maxsize=queuesize)
-            #dataoutqueue     = queue.Queue(maxsize=queuesize)
-            guiqueue         = queue.Queue(maxsize=queuesize)                                
-        else:
-            dataqueue        = multiprocessing.Queue(maxsize=queuesize)
-            datainqueue      = multiprocessing.Queue(maxsize=queuesize)            
-            comqueue         = multiprocessing.Queue(maxsize=queuesize)
-            statusqueue      = multiprocessing.Queue(maxsize=queuesize)
-            #dataoutqueue     = multiprocessing.Queue(maxsize=queuesize)
-            guiqueue         = multiprocessing.Queue(maxsize=queuesize)                                            
-        
-        # Device do not necessarily have a statusqueue
-        try:
-            device               = devicemodule.Device(dataqueue= dataqueue,comqueue = comqueue,datainqueue = datainqueue,statusqueue = statusqueue)
-        except:
-            device               = devicemodule.Device(dataqueue,comqueue,datainqueue)
-        # Add an unique number
-        device.numdevice     = self.numdevice
-        self.numdevice      += 1        
-        if thread: # Thread or multiprocess        
-            device.mp = 'thread'
-        else:
-            device.mp = 'multiprocessing'
+        funcname = self.__class__.__name__ + '.add_device():'
+        logger.debug(funcname + ':devicemodule: ' + str(devicemodulename) + ':deviceconfig: ' + str(deviceconfig))
+        devicelist = []
+        device_found = False
+        # Loop over all modules and check of we find the name
+        for smod in self.redvypr_device_scan.redvypr_devices_flat:
+            if (devicemodulename == smod['name']):
+                logger.debug('Trying to import device {:s}'.format(smod['name']))
+                devicemodule = smod['module']
+                # Try to get a configuration template
+                try:
+                    config_template = devicemodule.config_template
+                    logger.debug(funcname + ':Found configuation template of device {:s}'.format(str(devicemodule)))
+                    #templatedict = configtemplate_to_dict(config_template)
+                    FLAG_HAS_TEMPLATE = True
+                except Exception as e:
+                    logger.debug(
+                        funcname + ':No configuration template of device {:s}: {:s}'.format(str(devicemodule), str(e)))
+                    FLAG_HAS_TEMPLATE = False
 
-        # Add lists of receiving and providing devicenames
-        device.data_receiver = []
-        device.data_provider = []        
-        
-        statistics = create_data_statistic_dict()
-        devicedict = {'device':device,'thread':None,'dataout':[],'gui':[],'guiqueue':[guiqueue],'statistics':statistics}
-        # Add some statistics
-        devicedict['numpacket'] = 0
-        devicedict['numpacketout'] = 0        
-        # The displaywidget, to be filled by redvyprWidget.add_device (optional)
-        devicedict['devicedisplaywidget'] = None
-        
-        
-        # Setting the configuration of the device. Each key entry in
-        # the dict is directly set as an attribute in the device class
-        if(deviceconfig is not None):
-            logger.info('Setting configuration of device: ' + str(device) + ' #' + str(device.numdevice))
-            for key in deviceconfig:
-                confvalue = deviceconfig[key]                
-                logger.info(key + ':'+ str(confvalue))
-                setattr(device,key,confvalue)
-            
-                
-        
-        #self.devices.append(devicedict) # Add the device to the devicelist
-        return devicedict
+                # Try to get information about the maximum number of devices
+                try:
+                    max_devices = config_template['redvypr_device']['max_devices']
+                except:
+                    max_devices = -1
 
-    def start_device_thread(self,device):
-        """Functions starts a thread, to process the data (i.e. reading from a device, writing to a file)
-        Args:
-           device: Device is either a Device class defined in the device module or a dictionary containing the device class (when called from infodevicewidget in redvypr.py)
+                if(max_devices > 0):
+                    ndevices = 0
+                    for d in self.devices:
+                        devname = d['device'].devicemodulename
+                        if(devname == devicemodulename):
+                            ndevices += 1
+
+                    if ndevices >= max_devices:
+                        logger.warning(funcname + ' Could not add {:s}, maximum number of {:d} devices reached'.format(devicemodulename,max_devices))
+                        return
 
-        """
-        funcname = __name__ + '.start_device_thread():'
-        if(type(device) == dict): # If called from devicewidget
-            device = device['device']
+                # Try to get information about publish/subscribe capabilities described in the config_template
+                try:
+                    publishes = config_template['redvypr_device']['publishes']
+                except:
+                    publishes = False
+                try:
+                    subscribes = config_template['redvypr_device']['subscribes']
+                except:
+                    subscribes = False
+
+                try:
+                    deviceconfig['config']
+                except:
+                    deviceconfig['config'] = {}
+                # If the device does not have a name, add a standard but unique one
+                try:
+                    deviceconfig['name']
+                except:
+                    deviceconfig['name'] = devicemodulename + '_' + str(self.numdevice)
 
-        #logger.debug(funcname + 'Starting device: ' + str(device.name))
-        print(funcname + 'Starting device: ' + str(device.name))
+                try:
+                    deviceconfig['loglevel']
+                except:
+                    deviceconfig['loglevel'] = 'INFO'
 
-        # Find the right thread to start
-        for sendict in self.devices:
-            if(sendict['device'] == device):
                 try:
-                    running = sendict['thread'].is_alive()
+                    autostart = deviceconfig['autostart']
                 except:
-                    running = False
+                    autostart = False
+
+                # Check for multiprocess options in configuration
+                if (thread == None):
+                    try:
+                        multiprocess = deviceconfig['mp'].lower()
+                    except:
+                        multiprocess = 'thread'
+                elif(thread):
+                    multiprocess = 'thread'
+                else:
+                    multiprocess = 'multiprocess'
 
-                if(running):
-                    logger.info(funcname + ':thread/process is already running, doing nothing')
+                if multiprocess == 'thread':  # Thread or multiprocess
+                    dataqueue = queue.Queue(maxsize=queuesize)
+                    datainqueue = queue.Queue(maxsize=queuesize)
+                    comqueue = queue.Queue(maxsize=queuesize)
+                    statusqueue = queue.Queue(maxsize=queuesize)
+                    guiqueue = queue.Queue(maxsize=queuesize)
                 else:
+                    dataqueue = multiprocessing.Queue(maxsize=queuesize)
+                    datainqueue = multiprocessing.Queue(maxsize=queuesize)
+                    comqueue = multiprocessing.Queue(maxsize=queuesize)
+                    statusqueue = multiprocessing.Queue(maxsize=queuesize)
+                    guiqueue = multiprocessing.Queue(maxsize=queuesize)
+
+                # Create a dictionary for the statistics and general information about the device
+                # This is used extensively in exchanging information about devices between redvypr instances and or other devices
+                statistics = data_packets.create_data_statistic_dict()
+                # Device do not necessarily have a statusqueue
+                try:
+                    name = deviceconfig['name']
+                    loglevel = deviceconfig['loglevel']
+
+                    numdevices = len(self.devices)
+                    # Could also create a UUID based on the hostinfo UUID str
+                    device_uuid = '{:03d}--'.format(numdevices) + str(uuid.uuid1()) + '::' + self.hostinfo['uuid']
                     try:
-                        if device.mp == 'thread':
-                            devicethread     = threading.Thread(target=device.start, args=(), daemon=True)
-                            sendict['thread']= devicethread
-                            sendict['thread'].start()
-                            logger.info(funcname + 'started {:s} as thread'.format(device.name))
-                        else:
-                            deviceprocess    = multiprocessing.Process(target=device.start, args=())
-                            sendict['thread']= deviceprocess
-                            sendict['thread'].start()
-                            logger.info(funcname + 'started {:s} as process with PID {:d}'.format(device.name, deviceprocess.pid))
-
-                        # Update the device and the devicewidgets about the thread status
-                        running2 = sendict['thread'].is_alive()
-                        try: # If the device has a thread_status function
-                            device.thread_status({'threadalive':running2})
+                        devicemodule.Device
+                        HASDEVICE = True
+                    except:
+                        HASDEVICE = False
+
+                    if (HASDEVICE):  # Module has its own device
+                        Device = devicemodule.Device
+                        # Check if a startfunction is implemented
+                        try:
+                            Device.start
+                            startfunction = None
+                            logger.debug(
+                                funcname + ' Device has a start function')
                         except:
-                            pass
+                            logger.debug(
+                                funcname + ' Device does not have a start function, will add the standard function')
+                            startfunction = devicemodule.start
+                    else:
+                        Device = redvypr_device
+                        startfunction = devicemodule.start
 
-                        try: # If the device has a thread_status function
-                            sendict['initwidget'].thread_status({'threadalive':running2})
-                        except Exception as e:
-                            pass
+                    # Config used at all?
+                    print('Getting config')
+                    config = deviceconfig['config']
+                    print('Done')
+                    # Merge the config with a potentially existing template to fill in default values
+                    if FLAG_HAS_TEMPLATE:
+                        print('With template', config_template)
+                        print('With configuration', config)
+                        #config = apply_config_to_dict(config,templatedict)
+                        #config = copy.deepcopy(config)
+                        #redvypr.config.dict_to_configDict(templatedict, process_template=True)
+                        configu = configuration(template=config_template,config=config)
+                    else: # Make a configuration without a template directly from the config dict
+                        print('Without template')
+                        configu = configuration(config)
+                        config_template = None
+
+                    print('Config', configu)
+                    print('Config type', type(configu))
+                    print('loglevel', loglevel)
+                    device = Device(name=name, uuid=device_uuid, config=configu, redvypr=self, dataqueue=dataqueue,
+                                    publishes=publishes,subscribes=subscribes,autostart=autostart,
+                                    template=config_template, comqueue=comqueue, datainqueue=datainqueue,
+                                    statusqueue=statusqueue, loglevel=loglevel, multiprocess=multiprocess,
+                                    numdevice=self.numdevice, statistics=statistics,startfunction=startfunction,devicemodulename=devicemodulename)
+
+                    device.subscription_changed_signal.connect(self.process_subscription_changed)
+                    self.numdevice += 1
+                    # If the device has a logger
+                    devicelogger = device.logger
+                except Exception as e:
+                    logger.warning(funcname + ' Could not add device because of:')
+                    logger.exception(e)
 
-                        for guiwidget in sendict['gui']:
-                            try: # If the device has a thread_status function
-                                guiwidget.thread_status({'threadalive':running2})
-                            except Exception as e:
-                                pass
-                                #print('Start thread exception:' + str(e))
-                    except Exception as e:
-                        logger.warning(funcname + 'Could not start device {:s}'.format(str(e)))
-                    
 
-    def stop_device_thread(self,device):
+                devicedict = {'device': device, 'dataout': [], 'gui': [], 'guiqueue': [guiqueue],
+                              'statistics': statistics, 'logger': devicelogger,'comqueue':comqueue}
+
+                # Add the modulename
+                devicedict['devicemodulename'] = devicemodulename
+                # Add some statistics (LEGACY)
+                devicedict['packets_received'] = 0
+                devicedict['packets_sent'] = 0
+                # The displaywcreate_idget, to be filled by redvyprWidget.add_device (optional)
+                devicedict['devicedisplaywidget'] = None
+                # device = devicedict['device']
+
+                # Check if the device wants a direct start after initialization
+                try:
+                    autostart = device.autostart
+                except:
+                    autostart = False
+
+                # Add the device to the device list
+                self.devices.append(devicedict)  # Add the device to the devicelist
+                ind_device = len(self.devices) - 1
+
+                # Update the statistics of the device itself
+                deviceinfo_packet = {'_redvypr':{},'_deviceinfo': {'subscribes': subscribes, 'publishes': publishes, 'devicemodulename': devicemodulename}}
+                device.dataqueue.put(deviceinfo_packet)
+                # Send a device_status packet to notify that a new device was added (deviceinfo_all) is updated
+                datapacket = data_packets.commandpacket(command='device_status')
+                device.dataqueue.put(datapacket)
+                if (autostart):
+                    logger.info(funcname + ': Starting device')
+                    self.start_device_thread(device)
+
+                devicelist = [devicedict, ind_device, devicemodule]
+
+                #
+                # Subscribe to devices
+                #
+                try:
+                    subscribe_addresses =  deviceconfig['subscriptions']
+                except:
+                    subscribe_addresses = []
+
+                print('Subscribing to ...')
+                for a in subscribe_addresses:
+                    print('subscribing',a)
+                    device.subscribe_address(a)
+
+                logger.debug(funcname + ': Emitting device signal')
+                self.device_added.emit(devicelist)
+                device_found = True
+                break
+
+        if (device_found == False):
+            logger.warning(funcname + ': Could not add device (not found): {:s}'.format(str(devicemodulename)))
+
+        return devicelist
+
+
+    def start_device_thread(self, device):
+        """ Functions starts the device thread that is the core of each device
+        Args:
+           device: Device is either a Device class defined in the device module or a dictionary containing the device class (when called from infodevicewidget in redvypr.py)
+
+        """
+        funcname = __name__ + '.start_device_thread():'
+        if (type(device) == dict):  # If called from devicewidget
+            device = device['device']
+
+        # logger.debug(funcname + 'Starting device: ' + str(device.name))
+        logger.debug(funcname + 'Starting device: ' + str(device.name))
+        thread = device.thread_start()
+
+    def stop_device_thread(self, device):
         """Functions stops a thread, to process the data (i.e. reading from a device, writing to a file)
         Args:
            device: Device is either a Device class defined in the device module or a dictionary containing the device class (when called from infodevicewidget in redvypr.py)
 
-        """        
+        """
         funcname = __name__ + '.stop_device_thread()'
-        if(type(device) == dict): # If called from devicewidget
-            device = device['device']                
+        command = data_packets.commandpacket(command='stop', uuid=device.uuid)
+        if (type(device) == dict):  # If called from devicewidget
+            device = device['device']
         logger.debug(funcname + ':Stopping device: ' + device.name)
+        thread_status = device.thread_stop()
+
         for sendict in self.devices:
-            if(sendict['device'] == device):
-                if(sendict['thread'] == None):
+            if (sendict['device'] == device):
+                if (sendict['device'].thread == None):
                     return
-                elif(sendict['thread'].is_alive()):
+                elif (sendict['device'].thread.is_alive()):
                     try:
-                        if(device.datainqueuestop):
+                        device.thread_stop()
+                        return
+                    except:
+                        pass
+                    try:
+                        if (device.datainqueuestop):
                             datainqueuestop = True
                     except:
                         datainqueuestop = False
-                    
-                    if(datainqueuestop):
-                        logger.debug(funcname + ':Stopping device with datainqueue: ' + device.name)
-                        device.datainqueue.put({'command':'stop'})
-                    else:
-                        logger.debug(funcname + ':Stopping device with comqueue: ' + device.name)
-                        device.comqueue.put('stop')
-                                
-                else:
-                    print('Stop exception')
-                    
-                # This is probably still an alive thread, since it is usually checked in time intervals within the thread
-                try:    
-                    device.thread_status({'threadalive': sendict['thread'].is_alive()})
-                except:
-                    pass
 
+                    device.thread_stop()
 
-    def send_command(self,device,command):
-        """ Sends a command to a device by putting it into the command queue
-        """
-        funcname = self.__class__.__name__ + '.send_command():'
-        dev = self.get_device_from_str(device)
-        print(funcname,device,command,dev)
-        logger.debug(funcname + 'Sending command')
-        dev.comqueue.put(command)
-                
+                else:
+                    logger.warning(funcname + ': Could not stop thread.')
 
-    def adddevicepath(self,folder):
+    def adddevicepath(self, folder):
         """Adds a path to the devicepathlist
         """
         if folder:
-            if(folder not in self.device_paths):
+            if (folder not in self.device_paths):
                 self.device_paths.append(folder)
-                self.device_path_changed.emit() # Notify about the changes                
-
+                self.device_path_changed.emit()  # Notify about the changes
 
-
-    def remdevicepath(self,folder):
-        if(folder not in self.device_paths):
+    def remdevicepath(self, folder):
+        if (folder not in self.device_paths):
             self.device_paths.remove(folder)
-            self.device_path_changed.emit() # Notify about the changes
-            
-            
-    def get_devicename_from_device(self,device):
+            self.device_path_changed.emit()  # Notify about the changes
+
+    def process_subscription_changed(self):
         """
-        Creates a redvypr devicename from device and the hostinfo.
-        Args:
-            device:
-        
-        Returns
-        -------
-        device : str
-            The devicestring
-            
+        Process the subscription changed signals of the devices
+        Returns:
+
         """
-        devicename = device.name + ':' + hostinfo['hostname'] + '@' + hostinfo['addr'] + '::' + hostinfo['uuid']
-        return devicename
-    
-    def construct_datastream_from_device_datakey(self,datakey,device):
+        devsender = self.sender()
+        print('Subscribtion changed',devsender.name)
+        for d in self.devices:
+            dev = d['device']
+            if dev == devsender:
+                continue
+            dev.subscription_changed_global(devsender)
+
+    def get_all_subscriptions(self):
         """
-        Returns a full datastream from a redvypr device and datakey. Note that the datastream must no exist. 
-        Args:
-            datakey: str
-                The datakey
-            device: redvypr device
-                The redvypr device 
-        
-        
-        Returns
-        -------
-        str
-            A str of the datastream
-            
+
+        Returns:
+            List containing two lists of equal length, the first with all subscriptions, the second the device address
+
         """
-        devicename = self.get_devicename_from_device(device)
-        datastream = datakey + '/' + devicename
-        return datastream
-    
-    def get_device_from_str(self,devicestr):
-        """ Returns the deviced based on an inputstr, if not found returns None
-        """
-        devicedict = self.get_devicedict_from_str(devicestr)
-        if(devicedict == None):
-            return None
-        else:
-            return devicedict['device']
-            
+        all_subscriptions = []
+        all_devices = []
+        for d in self.devices:
+            dev = d['device']
+            nsub = len(dev.subscribed_addresses)
+            all_subscriptions.extend(dev.subscribed_addresses)
+            all_devices.extend([dev.address_str]*nsub)
+
+        return [all_subscriptions,all_devices]
 
-    def get_devicedict_from_str(self,devicestr):
+
+    def get_devices(self, publishes = None, subscribes = None):
         """
-        Returns the devicedict based on an devicestr, if not found returns None
-        
+        Returns a list of all devices of this redvypr instance. Returns all devices if "publishes" or "subscribes" is None.
+        Otherwise according to the publishes/subscribes flags
         Args:
-            devicestr (str): 
-            
-            
-        Returns
-        -------
-        device : dict
-            The redvypr devicedict corresponding to the devicestr.
-            
-        
-        """
-        deviceparsed = parse_devicestring(devicestr, local_hostinfo = hostinfo)
-        for d in self.devices:
-            flag_name     = d['device'].name     == deviceparsed['devicename']
-            flag_name     = flag_name or deviceparsed['deviceexpand']
-            
-            flag_hostname = hostinfo['hostname'] == deviceparsed['hostname']
-            flag_hostname = flag_hostname or deviceparsed['hostexpand']
-            
-            flag_addr     = hostinfo['addr']     == deviceparsed['addr']
-            flag_addr     = flag_addr or deviceparsed['addrexpand']
-            
-            flag_UUID     = hostinfo['uuid']     == deviceparsed['uuid']
-            flag_UUID     = flag_UUID or deviceparsed['uuidexpand']
-            
-            flag_local    = deviceparsed['local']
-            if (flag_name and flag_local) or (flag_name and flag_UUID) or (flag_name and flag_addr and flag_hostname):
-                return d
-
-        return None    
-    
-    def get_devices(self):
-        """
-        Returns a list of the devices
-
-        Returns
-        -------
-        devicelist : TYPE
-            DESCRIPTION.
+            publishes: True/False or None.
+            subscribes: True/False or None
 
+        Returns: List with redvypr_devices
 
         """
+
         devicelist = []
         for d in self.devices:
-            devicelist.append(d['device'].name)
+            dev = d['device']
+            if publishes == True:
+                if(dev.publishes):
+                    devicelist.append(dev)
+                    continue
+            elif publishes is None:
+                devicelist.append(dev)
+                continue
+
+            if (subscribes):
+                if (dev.subscribes):
+                    devicelist.append(dev)
+                    continue
+            elif subscribes is None:
+                devicelist.append(dev)
+                continue
+
 
         return devicelist
-    
-    def get_forwarded_devicenames(self,device=None):
-        """
-        """
-        try:
-            devicenames = device.statistics['devices']
-        except:
-            devicenames = []
-            
-        return devicenames
 
-    def get_data_providing_devicenames(self,device=None,forwarded_devices=True):
+    def get_deviceaddresses(self, local = None, publishes = None, subscribes = None):
         """
-        Returns a list of the devices that provide data to device. This is either the subscribed devices itself or a device that forwards data packets (i.e. network device)
+        Returns a list of redvypr_addresses of all devices. If local == None all known devices are listed,
+        also of all remote devices that are forwarded by a local host device (i.e. iored device).
+
 
         Args:
-            device: bool
-                None: Returns all data providing devices. 
-                Device:  Returns all data providing devices of device 
-            forwarded_devices: bool
-                A device might forward data packets from other devices. These devices can be listed as well, note that the device needs to have data packets received already to have them in their statistic.
+            local [bool/None]: None: all known devices are listed, False: Remote devices are listed, True: local devices are listed
+
+        Returns: List of redvypr_addresses
 
-        Returns
-        -------
-        list
-            A list containing the names of the data providing devices
 
         """
-        funcname = self.__class__.__name__ + '.get_data_providing_devices():'                                
-        logger.debug(funcname)
-        flag_device_itself = False
-        for devdict in self.devices:
-            if(devdict['device'] == device):
-                flag_device_itself = True 
-                break
-        
-        if(device == None):
-            flag_device_itself = True
-            
-        if(flag_device_itself == False):
-            raise ValueError('Device not in redvypr')
-        else:
-            devicenamelist = []
-            if(device == None):
-                for dev in self.devices:
-                    devname = dev['device'].name
-                    if(dev['device'].publish):
-                        devicenamelist.append(devname)
-                        print('Devname test',devname)
-                        devicenamelist_forward = self.get_forwarded_devicenames(dev['device'])
-                        print('Devname forward',devicenamelist_forward)
-                        devicenamelist.extend(devicenamelist_forward)
-                        
-            else:   
-                devicelist = get_data_providing_devices(self.devices,device)
-                for dev in devicelist:
-                    devicenamelist.append(dev.name)
-                    
-                devicenamelist_forward = self.get_forwarded_devicenames(dev['device'])
-                devicenamelist.extend(devicenamelist_forward)
+        raddrs = []
+        for dev in self.devices:
+            raddrs_tmp = dev['device'].get_deviceaddresses(local)
+            raddrs.extend(raddrs_tmp)
 
-            print('Devicelist 1',devicenamelist)    
-            devicenamelist = list(set(devicenamelist))
-            
-            return devicenamelist
-        
+        return raddrs
 
-    def get_data_providing_devices(self,device=None):
-        """
-        Returns LOCAL devices that provide data, note that if forwarded devices are needed, use get_data_providing_devicenames!
-        Args:
-            device: redvypr_device or None, if none return all data providing devices
-            
-        Returns
-        -------
-        list
-            A list containing redvypr_devices
+    def get_datastreams(self,local=None):
         """
-        devicelist = []
-        devicedicts = self.get_data_providing_devicedicts(device)
-        for d in devicedicts:
-            devicelist.append(d['device'])
-        return devicelist
-        
-    
-    def get_data_providing_devicedicts(self,device=None):
-        """
-        Returns LOCAL devices that provide data, note that if forwarded devices are needed, use get_data_providing_devicenames!
-        Args:
-            device: redvypr_device or None, if none return all data providing devices
-            
-        Returns
-        -------
-        list
-            A list containing redvypr dictionary containing the device and additional infrastructure::
-                redvypr.get_data_providing_devices()[0].keys()
-                dict_keys(['device', 'thread', 'dataout', 'gui', 'guiqueue', 'statistics', 'numpacket', 'numpacketout', 'devicedisplaywidget', 'logger', 'displaywidget', 'initwidget', 'widget', 'infowidget'])
-        """
-        if(device == None):
-            devicedicts = []
-            for dev in self.devices:
-                if(dev['device'].publish):
-                    devicedicts.append(dev)
-        else:
-            devicedicts = get_data_providing_devices(self.devices,device)
-                   
-        return devicedicts
-    
-    def get_datastreams(self,device=None,format='uuid'):
-        """
-        Gets datastreams from a device (or all devices if device == None).
-        Args:
-            device: (redvypr device or str):
-            format:
-            
-        Returns
-        -------
-        list
-            A list containing the datastreams
-        """
-        funcname       = self.__class__.__name__ + '.get_datastreams():'                                
-        datastreamlist = []
-        
-        if(type(device) == str):
-            datastreams_all = []
-            for dev in self.devices:
-                datastreams_all.extend(dev['statistics']['datastreams'])
-            datastreams_all = list(set(datastreams_all))
-            # Parse the devicestring
-            deviceparsed = parse_devicestring(device,local_hostinfo=hostinfo)
-            ##print('datastreams',datastreams_all)
-            ##print('deviceparsed',deviceparsed)
-            for stream in datastreams_all:
-                datastream_parsed = parse_devicestring(stream,local_hostinfo=hostinfo)
-                ##print('datastream parsed',datastream_parsed)
-                flag_name     = datastream_parsed['devicename'] == deviceparsed['devicename']
-                flag_name     = flag_name or deviceparsed['deviceexpand']
-            
-                flag_hostname = datastream_parsed['hostname']   == deviceparsed['hostname']
-                flag_hostname = flag_hostname or deviceparsed['hostexpand']
-            
-                flag_addr     = datastream_parsed['addr']       == deviceparsed['addr']
-                flag_addr     = flag_addr or deviceparsed['addrexpand']
-            
-                flag_uuid     = datastream_parsed['uuid']       == deviceparsed['uuid']
-                flag_uuid     = flag_uuid or deviceparsed['uuidexpand']
-            
-                flag_local    = datastream_parsed['local']      == deviceparsed['local']
-                
-                ##print('name',flag_name,'hostname',flag_hostname,'addr',flag_addr,'uuid',flag_uuid)
-                if (flag_name and flag_local) or (flag_name and flag_uuid) or (flag_name and flag_addr and flag_hostname):
-                    datastreamlist.append(stream)
-            
-            datastreamlist = list(set(datastreamlist))
-            
-        elif(device == None):
-            for dev in self.devices:
-                datastreamlist.extend(dev['statistics']['datastreams'])
-            datastreamlist = list(set(datastreamlist))
-            
-        else:
-            datastreamlist = device.statistics['datastreams']
-            datastreamlist = list(set(datastreamlist))
-            
-        return datastreamlist
-    
-    
-    def get_datakeys(self,device):
-        """
-        Get the datakeys for the device. 
-        
-        
+
         Args:
-            device (redvypr device or str):
-            
+            local:
+
         Returns:
-        --------
-        list
-            A list of the device datakeys
-         
+
         """
-        funcname = self.__class__.__name__ + '.get_datakeys():'                                
-        logger.debug(funcname)
-        datakeys = []    
-        datastreams = self.get_datastreams(device) # Get datastreams of device
-        for stream in datastreams:
-            key = stream.split('/')[0]
-            datakeys.append(key)
-        
-        datakeys = list(set(datakeys))
-        
-        return datakeys
-        
-    def get_data_receiving_devices(self,device):
-        funcname = self.__class__.__name__ + '.get_data_receiving_devices():'                                
-        logger.debug(funcname)        
-        return get_data_receiving_devices(self.devices,device)
-    
+        datastreams = []
+        for dev in self.devices:
+            raddrs_tmp = dev['device'].get_datastreams()
+            datastreams.extend(raddrs_tmp)
+
+        return datastreams
+
+
+    def get_datastream_info(self, datastream):
+        """ Gets additional information to the datastream
+        """
+
+        datastreams = self.get_datastreams()
+        datastreaminfo = {}
+        for dev in self.devices:
+            datastreaminfo |= dev['statistics']['datastreams_info']
+
+        for dstream in datastreaminfo.keys():
+            if (data_packets.compare_datastreams(datastream, dstream)):
+                return datastreaminfo[dstream]
+
+        return None
+
+
     def get_known_devices(self):
         """ List all known devices that can be loaded by redvypr
         
         Returns:
         --------
         list
             A list of known devices
         """
         funcname = self.__class__.__name__ + '.get_known_devices():'
         logger.debug(funcname)
         devices = []
-        for d in self.device_modules:
+        for d in self.redvypr_device_scan.redvypr_devices_flat:
             devices.append(d['name'])
 
         return devices
-    
-    def rm_all_data_provider(self,device):
+
+    def rem_device(self,device):
         """
-        Remove all devices that provide data
+        Removes a device, after the removal a signal for device change is sent
         Args:
-            device: The redvypr device
+            device: redvypr_device
+
+        Returns:
+
         """
-        funcname = self.__class__.__name__ + '.rm_all_data_provider():'
+        funcname = self.__class__.__name__ + '.rem_device():'
         logger.debug(funcname)
-        dataprovider = self.get_data_providing_devices(device)
-        for provider in dataprovider:
-            self.addrm_device_as_data_provider(provider,device,remove=True)
-        
-    def addrm_device_as_data_provider(self,deviceprovider,devicereceiver,remove=False):
-        """ Adding/removing devices as dataprovider for the device devicereceiver
-        Arguments:
-        deviceprovider: The device (type Device) or devicename (type str Device.name)
-        devicerreceiver: The device (type Device) or devicename (type str Device.name)
-        remove: False for adding, True for removing
-        """
-        if(type(deviceprovider) == str):
-            deviceprovider = self.get_device_from_str(deviceprovider)
-
-        if(type(devicereceiver) == str):
-            devicereceiver = self.get_device_from_str(devicereceiver)
-
-        ret = addrm_device_as_data_provider(self.devices,deviceprovider,devicereceiver,remove=remove)
-        # Emit a connection signal
-        self.devices_connected.emit(deviceprovider.name,devicereceiver.name)
-        return ret
+        FLAG_REMOVED = False
+        for sendict in self.devices:
+            if(sendict['device'] == device):
+                print('Sendict',sendict)
+                if (sendict['device'].thread == None):
+                    logger.debug(funcname + 'Thread is not runnung, doing nothing')
+                    pass
+                elif (sendict['device'].thread.is_alive()):
+                    logger.debug(funcname + 'Sending stop command')
+                    device.thread_stop()
+
+                self.devices.remove(sendict)
+                FLAG_REMOVED = True
+                self.device_removed.emit()
+                device_changed_dict = {'type':'device_removed','device':device.name,'uuid':device.uuid}
+                self.redvyprqueue.put(device_changed_dict)
+                break
+
+        return FLAG_REMOVED
+
+
+
 
 
 #
 #
 # ########################
 # Here the gui part starts
 # ########################
 #
 #
 #
-    
+
 
 #
 #
 #
 # redvyprwidget
 #
 #
 #
 
 class redvyprWidget(QtWidgets.QWidget):
     """This is the main widget of redvypr. 
 
     """
-    def __init__(self,width=None,height=None,config=None):
+
+    def __init__(self, width=None, height=None, config=None,hostname='redvypr',hostinfo_opt={}):
         """ Args: 
+            width:
+            height:
             config: Either a string containing a path of a yaml file, or a list with strings of yaml files
         """
         super(redvyprWidget, self).__init__()
         self.setGeometry(50, 50, 500, 300)
-        
+
         # Lets create the heart of redvypr
-        self.redvypr = redvypr() # Configuration comes later after all widgets are initialized
-        
+        self.redvypr = redvypr(hostname=hostname,hostinfo_opt=hostinfo_opt)  # Configuration comes later after all widgets are initialized
+
         self.redvypr.device_path_changed.connect(self.__populate_devicepathlistWidget)
-        self.redvypr.device_added.connect(self._add_device)
+        self.redvypr.device_added.connect(self._add_device_gui)
         # Fill the layout
         self.devicetabs = QtWidgets.QTabWidget()
         self.devicetabs.setMovable(True)
         self.devicetabs.setTabsClosable(True)
         self.devicetabs.tabCloseRequested.connect(self.closeTab)
-        
-        ## Add a console
-        #self.console = redvypr_console()
-        
-        
-           
+
         # The configuration of the redvypr
         self.create_devicepathwidget()
         self.create_statuswidget()
-        #self.devicetabs.addTab(self.__devicepathwidget,'Status')
-        self.devicetabs.addTab(self.__statuswidget,'Status')
-
+        # self.devicetabs.addTab(self.__devicepathwidget,'Status')
+        self.devicetabs.addTab(self.__statuswidget, 'Status')
 
         # A widget containing all connections
-        self.create_devicewidgetsummary() # Creates self.devicesummarywidget
-        self.devicetabs.addTab(self.devicesummarywidget,'Devices') # Add device summary widget
-        # A logwidget
-        self.logwidget = QtWidgets.QPlainTextEdit()
-        self.logwidget.setReadOnly(True)
-        self.logwidget_handler = QPlainTextEditLogger()
-        self.logwidget_handler.add_widget(self.logwidget)
-        self.devicetabs.addTab(self.logwidget,'Log') # Add a logwidget
-        # Connect the logwidget to the logging
-        #logger.addHandler(self.logwidget_handler)
-        #self.logwidget.append("Hallo!")
+        self.create_devicewidgetsummary()  # Creates self.devicesummarywidget
+        self.devicetabs.addTab(self.devicesummarywidget, 'Devices')  # Add device summary widget
+        if False:
+            # A logwidget
+            self.logwidget = QtWidgets.QPlainTextEdit()
+            self.logwidget.setReadOnly(True)
+            self.logwidget_handler = QPlainTextEditLogger()
+            self.logwidget_handler.add_widget(self.logwidget)
+            self.devicetabs.addTab(self.logwidget, 'Log')  # Add a logwidget
+            # Connect the logwidget to the logging
+            # logger.addHandler(self.logwidget_handler)
+            # self.logwidget.append("Hallo!")
 
         # A timer to gather all the data from the devices
         self.devicereadtimer = QtCore.QTimer()
         self.devicereadtimer.timeout.connect(self.readguiqueue)
         self.devicereadtimer.start(100)
-        #self.devicereadtimer.start(500)
-        
+        # self.devicereadtimer.start(500)
 
         self.layout = QtWidgets.QVBoxLayout(self)
         self.layout.addWidget(self.devicetabs)
-        if((width is not None) and (height is not None)):
+        if ((width is not None) and (height is not None)):
             self.resize(int(width), int(height))
-            
-        if True:    
-            # Configurating redvypr
-            if(config is not None):
-                if(type(config) == str):
-                    config = [config]
-
-                for c in config:
-                    self.redvypr.parse_configuration(c)
 
-                if('hostname' in self.redvypr.config.keys()):
-                    self.hostname_changed(self.redvypr.config['hostname'])   
+        self.redvypr.parse_configuration(config)
+        # Update hostinformation widgets
+        self.__update_hostinfo_widget__()
         self.__populate_devicepathlistWidget()
-        
+
+    def open_ipwidget(self):
+        self.ipwidget = redvypr_ip_widget()
+
     def open_console(self):
         """ Opens a pyqtconsole console widget
             
         """
         if True:
             width = 800
             height = 500
             # Console
             self.console = PythonConsole(formats={
                 'keyword': format('darkBlue', 'bold')
-                })
+            })
             self.console.setWindowIcon(QtGui.QIcon(_icon_file))
-            self.console.setWindowTitle("redvypr console")        
+            self.console.setWindowTitle("redvypr console")
             self.console.push_local_ns('redvypr_widget', self)
             self.console.push_local_ns('redvypr', self.redvypr)
             self.console.resize(width, height)
             self.console.show()
-            
+
             self.console.eval_queued()
-        
-        #self.devicetabs.addTab(self.console,'Console') 
-    def renamedevice(self,oldname,name):
+
+        # self.devicetabs.addTab(self.console,'Console')
+
+    def renamedevice(self, oldname, name):
         """ Renames a devices
         """
         funcname = 'renamedevice()'
         for dev in self.redvypr.devices:
             devname = dev['device'].name
-            if(devname == name): # Found a device with that name already, lets do nothging
+            if (devname == name):  # Found a device with that name already, lets do nothging
                 logger.debug(funcname + ': Name already in use. Will not rename')
                 return False
-            
+
         for dev in self.redvypr.devices:
             devname = dev['device'].name
-            if(devname == oldname): # Found the device, lets rename it
-                dev['device'].name = name
+            if (devname == oldname):  # Found the device, lets rename it
+                dev['device'].change_name(name)
                 widget = dev['widget']
                 # Create a new infowidget
                 dev['infowidget'].close()
-                dev['infowidget'] = deviceinfoWidget(dev,self)
-                dev['infowidget'].device_start.connect(self.redvypr.start_device_thread)
-                dev['infowidget'].device_stop.connect(self.redvypr.stop_device_thread)
-                dev['infowidget'].connect.connect(self.connect_device)                
+                dev['infowidget'] = deviceinfoWidget(dev, self)
+                # Note: commented for the moment to be replaced by the signals of the device itself
+                # dev['infowidget'].device_start.connect(self.redvypr.start_device_thread)
+                # dev['infowidget'].device_stop.connect(self.redvypr.stop_device_thread)
+                dev['infowidget'].connect.connect(self.connect_device)
                 for i in range(self.devicetabs.count()):
-                    if(self.devicetabs.widget(i) == widget):
-                        self.devicetabs.setTabText(i,name)
+                    if (self.devicetabs.widget(i) == widget):
+                        self.devicetabs.setTabText(i, name)
                         break
 
                 break
-                
+
         self.update_devicewidgetsummary()
         return True
-    
+
     def create_devicewidgetsummary(self):
         """ Creates the device summary widget
         """
         self.devicesummarywidget = QtWidgets.QWidget()
         self.devicesummarywidget_layout = QtWidgets.QVBoxLayout(self.devicesummarywidget)
 
-    def update_devicewidgetsummary(self):            
+    def update_devicewidgetsummary(self):
         """ Updates the device summary widget
         """
         # Remove all
         for i in reversed(range(self.devicesummarywidget_layout.count())):
             item = self.devicesummarywidget_layout.itemAt(i)
             self.devicesummarywidget_layout.removeItem(item)
 
         # and refill it
-        for i,devicedict in enumerate(self.redvypr.devices):
+        for i, devicedict in enumerate(self.redvypr.devices):
             self.devicesummarywidget_layout.addWidget(devicedict['infowidget'])
 
         self.devicesummarywidget_layout.addStretch()
 
     def readguiqueue(self):
-        """This periodically called functions reads the guiqueue and calls
+        """This periodically called function reads the guiqueue and calls
         the widgets of the devices update function (if they exist)
 
         """
         # Update devices
         for devicedict in self.redvypr.devices:
             device = devicedict['device']
             if True:
                 # Feed the data into the modules/functions/objects and
                 # let them treat the data
-                for i,guiqueue in enumerate(devicedict['guiqueue']):
+                for i, guiqueue in enumerate(devicedict['guiqueue']):
                     while True:
-                        try:                    
+                        try:
                             data = guiqueue.get(block=False)
+                        except Exception as e:
+                            # print('Exception gui',e)
+                            break
+                        try:
                             devicedict['gui'][i].update(data)
                         except Exception as e:
                             break
+                            #logger.exception(e)
 
 
     def load_config(self):
         """ Loads a configuration file
         """
-        funcname = self.__class__.__name__ + '.load_config()'                        
+        funcname = self.__class__.__name__ + '.load_config()'
         logger.debug(funcname)
-        conffile, _ = QtWidgets.QFileDialog.getOpenFileName(self,"QFileDialog.getOpenFileName()", "","Yaml Files (*.yaml);;All Files (*)")
+        conffile, _ = QtWidgets.QFileDialog.getOpenFileName(self, "QFileDialog.getOpenFileName()", "",
+                                                            "Yaml Files (*.yaml);;All Files (*)")
         if conffile:
             self.redvypr.parse_configuration(conffile)
-            
+
     def save_config(self):
         """ Saves a configuration file
         """
-        funcname = self.__class__.__name__ + '.save_config():'                        
+        funcname = self.__class__.__name__ + '.save_config():'
         logger.debug(funcname)
-        print('Not implented yet!')
-        data_save = self.redvypr.config
-        fname_full, _ = QtWidgets.QFileDialog.getSaveFileName(self,"QFileDialog.getSaveFileName()", "","Yaml Files (*.yaml);;All Files (*)")
-        if fname_full:
-            print('Saving to file {:s}'.format(fname_full))            
-            with open(fname_full, 'w') as fyaml:
-                yaml.dump(data_save, fyaml)
+        data_save = self.redvypr.get_config()
+        print('data_save',data_save)
+        if True:
+            tstr = datetime.datetime.now().strftime('%Y-%m-%d_%H%M%S')
+            fname_suggestion = 'config_' + self.redvypr.hostinfo['hostname'] + '_' +tstr + '.yaml'
 
+            fname_full, _ = QtWidgets.QFileDialog.getSaveFileName(self, "QFileDialog.getSaveFileName()", fname_suggestion,
+                                                                  "Yaml Files (*.yaml);;All Files (*)")
+            if fname_full:
+                print('Saving to file {:s}'.format(fname_full))
+                with open(fname_full, 'w') as fyaml:
+                    yaml.dump(data_save, fyaml)
 
     def open_add_device_widget(self):
-        """Opens a widget for the user to choose to add a device
-        TODO: make an own widget out of this
-
-        """
-        self.add_device_widget = QtWidgets.QWidget()
-        # Set icon    
-        self.add_device_widget.setWindowIcon(QtGui.QIcon(_icon_file))        
-        layout = QtWidgets.QFormLayout(self.add_device_widget)
-        self.__devices_list    = QtWidgets.QListWidget()
-        self.__devices_list.itemClicked.connect(self.__device_name)
-        self.__devices_list.currentItemChanged.connect(self.__device_name)
-        self.__devices_list.itemDoubleClicked.connect(self.add_device_click)
-        self.__devices_info    = QtWidgets.QWidget()
-        self.__devices_addbtn  = QtWidgets.QPushButton('Add')
-        self.__devices_addbtn.clicked.connect(self.add_device_click)
-        self.__devices_devnamelabel = QtWidgets.QLabel('Devicename')
-        self.__devices_devname = QtWidgets.QLineEdit()
-        self.__mp_label  = QtWidgets.QLabel('Multiprocessing options')
-        self.__mp_thread = QtWidgets.QRadioButton('Thread')
-        self.__mp_multi  = QtWidgets.QRadioButton('Multiprocessing')
-        self.__mp_multi.setChecked(True)        
-        self.__mp_group  = QtWidgets.QButtonGroup()
-        self.__mp_group.addButton(self.__mp_thread)
-        self.__mp_group.addButton(self.__mp_multi)
-        
-        
-        layout.addRow(self.__devices_info)
-        layout.addRow(self.__devices_list)
-        layout.addRow(self.__mp_label)
-        layout.addRow(self.__mp_thread,self.__mp_multi)
-        layout.addRow(self.__devices_devnamelabel,self.__devices_devname)                                
-        layout.addRow(self.__devices_addbtn)
-        # Searches for devices 
-        self.redvypr.populate_device_path()
-        # Create the info widget
-        infolayout = QtWidgets.QFormLayout(self.__devices_info)        
-        self.__devices_info_sourcelabel1 = QtWidgets.QLabel('Source:')
-        self.__devices_info_sourcelabel2 = QtWidgets.QLabel('')
-        self.__devices_info_sourcelabel3 = QtWidgets.QLabel('Path:')
-        self.__devices_info_sourcelabel4 = QtWidgets.QLabel('')
-        self.__devices_info_sourcelabel5 = QtWidgets.QLabel('Description:')
-        self.__devices_info_sourcelabel6 = QtWidgets.QLabel('')                
-        infolayout.addRow(self.__devices_info_sourcelabel1,self.__devices_info_sourcelabel2)
-        infolayout.addRow(self.__devices_info_sourcelabel3,self.__devices_info_sourcelabel4)
-        infolayout.addRow(self.__devices_info_sourcelabel5)
-        infolayout.addRow(self.__devices_info_sourcelabel6)        
-
-        # Populate the device list
-        itms = []
-        known_devices = self.redvypr.get_known_devices()
-        for d in known_devices:
-            itm = QtWidgets.QListWidgetItem(d)
-            itms.append(itm)
-            self.__devices_list.addItem(itm)
-        
-        self.__devices_list.setMinimumWidth(self.__devices_list.sizeHintForColumn(0))    
-        # Set the first item as current and create a device name
-        self.__devices_list.setCurrentItem(itms[0])
-        self.__device_name()
+        self.add_device_widget = gui.redvyprDeviceWidget(redvypr=self.redvypr)
         self.add_device_widget.show()
-        
 
-    def __device_info(self):
-        """ Populates the self.__devices_info widget with the info of the module
-        """
-        ind = int(self.__devices_list.currentRow())
-        infotxt = self.redvypr.device_modules[ind]['name']
-        self.__devices_info_sourcelabel2.setText(infotxt)
-        infotxt2 = self.redvypr.device_modules[ind]['source']
-        self.__devices_info_sourcelabel4.setText(infotxt2)
-        try:
-            desctxt = self.redvypr.device_modules[ind]['module'].description
-        except Exception as e:
-            desctxt = ''
-
-        self.__devices_info_sourcelabel6.setText(desctxt)        
-        
-    def __device_name(self):
-        devicemodulename = self.__devices_list.currentItem().text()
-        devicename = devicemodulename + '_{:d}'.format(self.redvypr.numdevice + 1 )
-        self.__devices_devname.setText(devicename)
-        self.__device_info()
-        
-    def add_device_click(self):
-        """
-        """
-        devicemodulename = self.__devices_list.currentItem().text()
-        thread = self.__mp_thread.isChecked()
-        deviceconfig = {'name':str(self.__devices_devname.text())}
-        self.redvypr.add_device(devicemodulename=devicemodulename,thread=thread,deviceconfig=deviceconfig)
-        # Update the name
-        self.__device_name()
-
-    def _add_device(self,devicelist):
+    def _add_device_gui(self, devicelist):
         """ Function is called via the redvypr.add_device signal and is adding
         all the gui functionality to the device
 
         """
-        funcname = __name__ + '.add_device()' 
+        funcname = __name__ + '._add_device_gui()'
         logger.debug(funcname)
-        devicedict   = devicelist[0]
-        ind_devices  = devicelist[1]
+        devicedict = devicelist[0]
+        ind_devices = devicelist[1]
         devicemodule = devicelist[2]
 
         # First create the device and then do the widget stuff here
         device = devicedict['device']
         #
         # Now add all the widgets to the device
         #
         # Create the init widget
         try:
             deviceinitwidget_bare = devicemodule.initDeviceWidget
         except Exception as e:
-            logger.debug(funcname + ': Widget does not have a deviceinitwidget or start/stop signals:' + str(e))
-            deviceinitwidget_bare = QtWidgets.QWidget() # Use a standard widget
-            
+            logger.debug(funcname + ': Widget does not have a deviceinitwidget using standard one:' + str(e))
+            #logger.exception(e)
+            deviceinitwidget_bare = redvypr_deviceInitWidget  # Use a standard widget
+
         try:
             deviceinitwidget = deviceinitwidget_bare(device)
-            deviceinitwidget.device_start.connect(self.redvypr.start_device_thread)
-            deviceinitwidget.device_stop.connect(self.redvypr.stop_device_thread)
         except Exception as e:
-            logger.warning(funcname + ': Widget does not have a deviceinitwidget or start/stop signals:' + str(e))
-            deviceinitwidget = QtWidgets.QWidget() # Use a standard widget
-            
+            logger.warning(funcname + ': Could not add deviceinitwidget because of:')
+            logger.exception(e)
+            deviceinitwidget = QtWidgets.QWidget()  # Use a standard widget
+
+        # Connect the connect signal with connect_device()
         try:
             logger.debug(funcname + ': Connect signal connected')
             deviceinitwidget.connect.connect(self.connect_device)
         except Exception as e:
             logger.debug('Widget does not have connect signal:' + str(e))
 
+        device.deviceinitwidget = deviceinitwidget
+        # Add the info widget
+        deviceinfowidget = redvypr_deviceInfoWidget(device)
 
         #
         # Check if we have a widget to display the data
         # Create the displaywidget
         #
         try:
             devicedisplaywidget = devicemodule.displayDeviceWidget
         except Exception as e:
             logger.debug(funcname + ': No displaywidget found for {:s}'.format(str(devicemodule)))
-            # Using the standard display widget
-            devicedisplaywidget = displayDeviceWidget_standard
+            ## Using the standard display widget
+            # devicedisplaywidget = displayDeviceWidget_standard
+            devicedisplaywidget = None
 
+        # The widget shown in the tab
         devicewidget = QtWidgets.QWidget()
+        devicewidget.device = device # Add the device to the devicewidget
         devicelayout = QtWidgets.QVBoxLayout(devicewidget)
         devicetab = QtWidgets.QTabWidget()
         devicetab.setMovable(True)
         devicelayout.addWidget(devicetab)
-        
-        devicetab.addTab(deviceinitwidget,'Init') 
+
+        # Add init widget
+        devicetab.addTab(deviceinitwidget, 'Init')
+        devicetab.addTab(deviceinfowidget, 'Info')
         # Devices can have their specific display objects, if one is
         # found, initialize it, otherwise just the init Widget
-        if(devicedisplaywidget is not None):
+        if (devicedisplaywidget is not None):
             initargs = inspect.signature(devicedisplaywidget.__init__)
             initdict = {}
-            if('device' in initargs.parameters.keys()):
+            if ('device' in initargs.parameters.keys()):
                 initdict['device'] = device
 
-            if('tabwidget' in initargs.parameters.keys()):
+            if ('tabwidget' in initargs.parameters.keys()):
                 initdict['tabwidget'] = devicetab
-                
+
+            if ('deviceinitwidget' in initargs.parameters.keys()):
+                initdict['deviceinitwidget'] = deviceinitwidget
+
             # https://stackoverflow.com/questions/334655/passing-a-dictionary-to-a-function-as-keyword-parameters
             devicedisplaywidget_called = devicedisplaywidget(**initdict)
-                
+            # Add the widget to the device
+            device.devicedisplaywidget = devicedisplaywidget_called
             # Test if the widget has a tabname
             try:
                 tabname = devicedisplaywidget_called.tabname
             except:
                 tabname = 'Display data'
-            
+
             # Check if the widget has included itself, otherwise add the displaytab
-            if(devicetab.indexOf(devicedisplaywidget_called)) < 0:   
-                devicetab.addTab(devicedisplaywidget_called,tabname)            
-            # Append the widget to the processing queue
+            if (devicetab.indexOf(devicedisplaywidget_called)) < 0:
+                devicetab.addTab(devicedisplaywidget_called, tabname)
+                # Append the widget to the processing queue
             self.redvypr.devices[ind_devices]['gui'].append(devicedisplaywidget_called)
             self.redvypr.devices[ind_devices]['displaywidget'] = self.redvypr.devices[ind_devices]['gui'][0]
             self.redvypr.devices[ind_devices]['initwidget'] = deviceinitwidget
         else:
-            self.redvypr.devices[ind_devices]['initwidget']    = deviceinitwidget
+            self.redvypr.devices[ind_devices]['initwidget'] = deviceinitwidget
             self.redvypr.devices[ind_devices]['displaywidget'] = None
-                               
-        
-        self.redvypr.devices[ind_devices]['widget'] = devicewidget # This is the displaywidget
+
+        self.redvypr.devices[ind_devices]['widget'] = devicewidget  # This is the displaywidget
         # Create the infowidget (for the overview of all devices)
-        self.redvypr.devices[ind_devices]['infowidget'] = deviceinfoWidget(self.redvypr.devices[ind_devices],self)
-        self.redvypr.devices[ind_devices]['infowidget'].device_start.connect(self.redvypr.start_device_thread)
-        self.redvypr.devices[ind_devices]['infowidget'].device_stop.connect(self.redvypr.stop_device_thread)
+        self.redvypr.devices[ind_devices]['infowidget'] = deviceinfoWidget(self.redvypr.devices[ind_devices], self)
         self.redvypr.devices[ind_devices]['infowidget'].connect.connect(self.connect_device)
-        
+
         #
         # Add the devicelistentry to the widget, this gives the full information to the device
         #
+        # 22.11.2022 TODO, this needs to be replaced by functional arguments instead of properties
         self.redvypr.devices[ind_devices]['initwidget'].redvyprdevicelistentry = self.redvypr.devices[ind_devices]
-        self.redvypr.devices[ind_devices]['gui'][0].redvyprdevicelistentry     = self.redvypr.devices[ind_devices]
         self.redvypr.devices[ind_devices]['initwidget'].redvypr = self.redvypr
-        self.redvypr.devices[ind_devices]['gui'][0].redvypr     = self.redvypr
-            
-        self.devicetabs.addTab(devicewidget,device.name)
+        if(len(self.redvypr.devices[ind_devices]['gui']) > 0):
+            self.redvypr.devices[ind_devices]['gui'][0].redvyprdevicelistentry = self.redvypr.devices[ind_devices]
+            self.redvypr.devices[ind_devices]['gui'][0].redvypr = self.redvypr
+
+
+        self.devicetabs.addTab(devicewidget, device.name)
         self.devicetabs.setCurrentWidget(devicewidget)
 
         # All set, now call finalizing functions
         # Finalize the initialization by calling a helper function (if exist)
         try:
             deviceinitwidget.finalize_init()
         except Exception as e:
-            logger.debug(funcname + ':finalize_init():' + str(e))        
+            logger.debug(funcname + ':finalize_init():' + str(e))
 
-        # Update the summary
-        self.update_devicewidgetsummary()        
+            # Update the summary
+        self.update_devicewidgetsummary()
 
     def connect_device_gui(self):
         """ Wrapper for the gui
         """
-        self.open_connect_widget(device = None)
+        # Get the current tab
+        curtab = self.devicetabs.currentWidget()
+        try:
+            device = curtab.device
+        except:
+            device = None
+        self.open_connect_widget(device=device)
 
-    def connect_device(self,device):
+    def connect_device(self, device):
         """ Handles the connect signal from devices, called when the connection between the device shall be changed
         """
         logger.debug('Connect clicked')
-        if(type(device) == dict):
+        if (type(device) == dict):
             device = device['device']
-        self.open_connect_widget(device = device)
+        self.open_connect_widget(device=device)
 
-    def open_connect_widget(self,device=None):
-        funcname = __name__ + '.open_connect_widget()'                
+    def open_connect_widget(self, device=None):
+        funcname = __name__ + '.open_connect_widget()'
         logger.debug(funcname + ':' + str(device))
-        self.__con_widget = redvyprConnectWidget(devices=self.redvypr.devices,device=device)        
+        #self.__con_widget = redvyprConnectWidget(devices=self.redvypr.devices, device=device)
+        self.__con_widget = gui.redvyprSubscribeWidget(redvypr=self.redvypr, device=device)
         self.__con_widget.show()
-        
-        
+
     def __hostname_changed_click(self):
         hostname, ok = QtWidgets.QInputDialog.getText(self, 'redvypr hostname', 'Enter new hostname:')
         if ok:
-            self.hostname_changed(hostname)
-    def hostname_changed(self,hostname):
-        if True:
+            self.redvypr.hostinfo['hostname'] = hostname
             self.__hostname_line.setText(hostname)
-            self.redvypr.config['hostname'] = hostname
-            hostinfo['hostname'] = hostname
 
+    def __update_hostinfo_widget__(self):
+        """
+        Updates the hostinformation
+        Returns:
 
-    def update_status(self):
-        self.__status_dtneeded.setText(' (needed {:0.5f}s)'.format(self.redvypr.dt_avg_datadist))                
+        """
+        funcname = __name__ + '.__update_hostinfo_widget__()'
+        print(funcname)
+
+
+    def __update_status_widget__(self):
+        """
+        Updates the status information
+        Returns:
+
+        """
+        if self.redvypr.datadistthread.is_alive() == False:
+            self.__status_dt.setText(
+                'Datadistribution thread is not running! This is bad, consider restarting redvypr.')
+            self.__status_dt.setStyleSheet("QLabel { background-color : white; color : red; }")
+            self.__status_dtneeded.setText('')
+        else:
+            npackets = self.redvypr.packets_processed
+            if(npackets > 0):
+                packets_pstr = npackets / self.redvypr.dt_avg_datadist
+            else:
+                packets_pstr = 0.0
+            self.__status_dtneeded.setText(' (needed {:0.5f}s, {:6.1f} packets/s)'.format(self.redvypr.dt_avg_datadist,packets_pstr))
 
     def create_statuswidget(self):
         """Creates the statuswidget
 
         """
-        self.redvypr.devicethreadtimer.timeout.connect(self.update_status) # Add to the timer another update
+        self.redvypr.status_update_signal.connect(self.__update_status_widget__)
+        self.redvypr.hostconfig_changed_signal.connect(self.__update_hostinfo_widget__)
         self.__statuswidget = QtWidgets.QWidget()
         layout = QtWidgets.QFormLayout(self.__statuswidget)
         # dt
         self.__status_dt = QtWidgets.QLabel('Distribution time: {:0.5f}s'.format(self.redvypr.dt_datadist))
-        self.__status_dtneeded = QtWidgets.QLabel(' (needed {:0.5f}s)'.format(self.redvypr.dt_avg_datadist))        
+        self.__status_dtneeded = QtWidgets.QLabel(' (needed {:0.5f}s)'.format(self.redvypr.dt_avg_datadist))
 
-        layout.addRow(self.__status_dt,self.__status_dtneeded)
+        layout.addRow(self.__status_dt, self.__status_dtneeded)
 
         # Hostname
         self.__hostname_label = QtWidgets.QLabel('Hostname:')
-        self.__hostname_line  = QtWidgets.QLabel('')
+        self.__hostname_line = QtWidgets.QLabel('')
         self.__hostname_line.setAlignment(QtCore.Qt.AlignRight)
         self.__hostname_line.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
-        self.__hostname_line.setText(hostinfo['hostname'])
+        self.__hostname_line.setText(self.redvypr.hostinfo['hostname'])
         # UUID
         self.__uuid_label = QtWidgets.QLabel('UUID:')
-        self.__uuid_line  = QtWidgets.QLabel('')
+        self.__uuid_line = QtWidgets.QLabel('')
         self.__uuid_line.setAlignment(QtCore.Qt.AlignRight)
         self.__uuid_line.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
-        self.__uuid_line.setText(hostinfo['uuid'])
+        self.__uuid_line.setText(self.redvypr.hostinfo['uuid'])
         # IP
         self.__ip_label = QtWidgets.QLabel('IP:')
-        self.__ip_line  = QtWidgets.QLabel('')
+        self.__ip_line = QtWidgets.QLabel('')
         self.__ip_line.setAlignment(QtCore.Qt.AlignRight)
         self.__ip_line.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
-        self.__ip_line.setText(hostinfo['addr'])
+        self.__ip_line.setText(self.redvypr.hostinfo['addr'])
+
+        # Location
+        try:
+            location = self.redvypr.hostinfo_opt['location'].data
+        except:
+            location = ''
+
+        self.__loc_label = QtWidgets.QLabel('Location:')
+        self.__loc_text = QtWidgets.QLineEdit(location)
+        self.__loc_text.textold = self.__loc_text.text() # the old text to check again
+        self.__loc_text.editingFinished.connect(self.__hostinfo_opt_changed_text)
+
+        # Description
+        try:
+            description = self.redvypr.hostinfo_opt['description'].data
+        except:
+            description = ''
+
+        self.__desc_label = QtWidgets.QLabel('Description:')
+        self.__desc_text = QtWidgets.QLineEdit(description)
+        self.__desc_text.textold = self.__desc_text.text()  # the old text to check again
+        self.__desc_text.editingFinished.connect(self.__hostinfo_opt_changed_text)
+
+        # Lon
+        try:
+            lon = self.redvypr.hostinfo_opt['lon'].data
+        except:
+            lon = -9999.0
+
+        # Lon/Lat
+        try:
+            lat = self.redvypr.hostinfo_opt['lat'].data
+        except:
+            lat = -9999.0
+
+
+        self.__lon_label = QtWidgets.QLabel('Longitude:')
+        self.__lat_label = QtWidgets.QLabel('Latitude:')
+        self.__lon_text = QtWidgets.QDoubleSpinBox()
+        self.__lon_text.setMinimum(-9999)
+        self.__lon_text.setMaximum(360)
+        self.__lon_text.setSingleStep(0.00001)
+        self.__lon_text.setDecimals(5)
+        self.__lon_text.setValue(lon)
+        self.__lon_text.oldvalue = self.__lon_text.value()
+        self.__lon_text.editingFinished.connect(self.__hostinfo_opt_changed_text)
+
+        self.__lat_text = QtWidgets.QDoubleSpinBox()
+        self.__lat_text.setMinimum(-9999)
+        self.__lat_text.setMaximum(90)
+        self.__lat_text.setSingleStep(0.00001)
+        self.__lat_text.setDecimals(5)
+        self.__lat_text.setValue(lat)
+        self.__lat_text.oldvalue = self.__lat_text.value()
+        self.__lat_text.editingFinished.connect(self.__hostinfo_opt_changed_text)
+
         # Change the hostname
-        self.__hostname_btn = QtWidgets.QPushButton('Change hostname')
-        self.__hostname_btn.clicked.connect(self.__hostname_changed_click)
+        self.__hostinfo_opt_btn = QtWidgets.QPushButton('Edit optional information')
+        self.__hostinfo_opt_btn.clicked.connect(self.__hostinfo_opt_changed_click)
+
 
-        layout.addRow(self.__hostname_label,self.__hostname_line)
-        layout.addRow(self.__uuid_label,self.__uuid_line)
-        layout.addRow(self.__ip_label,self.__ip_line)
-        layout.addRow(self.__hostname_btn)
 
         self.__statuswidget_pathbtn = QtWidgets.QPushButton('Edit device path')
         self.__statuswidget_pathbtn.clicked.connect(self.show_devicepathwidget)
+
+        layout.addRow(self.__hostname_label, self.__hostname_line)
+        layout.addRow(self.__uuid_label, self.__uuid_line)
+        layout.addRow(self.__ip_label, self.__ip_line)
+        layout.addRow(self.__desc_label, self.__desc_text)
+        layout.addRow(self.__loc_label, self.__loc_text)
+        layout.addRow(self.__lon_label,self.__lon_text)
+        layout.addRow(self.__lat_label, self.__lat_text)
+        layout.addRow(self.__hostinfo_opt_btn)
         layout.addRow(self.__statuswidget_pathbtn)
-        
+
         logo = QtGui.QPixmap(_logo_file)
         logolabel = QtWidgets.QLabel()
         logolabel.setPixmap(logo)
-        #layout.addRow(logolabel)        
+        # layout.addRow(logolabel)
 
+    def __hostinfo_opt_changed_text(self):
+        """
+        Called when the textedit was done, updates the hostinformation,
+        Returns:
+
+        """
+        funcname = __name__ + '.__hostinfo_opt_changed_text()'
+        print(funcname)
+        FLAG_CHANGE = False
+        # Location text
+        if self.__loc_text.textold == self.__loc_text.text():
+            print('Not really a change of the text')
+        else:
+            self.__loc_text.textold = self.__loc_text.text()
+            self.redvypr.hostinfo_opt['location'].data = self.__loc_text.text()
+            FLAG_CHANGE = True
+
+        # Location text
+        if self.__desc_text.textold == self.__desc_text.text():
+            print('Not really a change of the description text')
+        else:
+            self.__desc_text.textold = self.__desc_text.text()
+            self.redvypr.hostinfo_opt['description'].data = self.__desc_text.text()
+            FLAG_CHANGE = True
+
+        # Longitude
+        if self.__lon_text.oldvalue == self.__lon_text.value():
+            print('Not really a change of the longitude')
+        else:
+            self.__lon_text.oldvalue = self.__lon_text.value()
+            self.redvypr.hostinfo_opt['lon'].data = self.__lon_text.value()
+            FLAG_CHANGE = True
+
+        # Latitude
+        if self.__lat_text.oldvalue == self.__lat_text.value():
+            print('Not really a change of the latitude')
+        else:
+            self.__lat_text.oldvalue = self.__lat_text.value()
+            self.redvypr.hostinfo_opt['lat'].data = self.__lat_text.value()
+            FLAG_CHANGE = True
+
+        if FLAG_CHANGE:
+            print('Things have changed, lets send a signal')
+            try:
+                self.__hostinfo_opt_edit.reload_config()
+            except:
+                pass
+            self.redvypr.hostconfig_changed_signal.emit()
+
+    def __hostinfo_opt_changed_click(self):
+        """
+        Opens a widget that allow to change the optional hostinformation
+        Returns:
+
+        """
+        # Optional hostinformation
+        self.__hostinfo_opt_edit = gui.configWidget(self.redvypr.hostinfo_opt, loadsavebutton=False,
+                                               redvypr_instance=self.redvypr)
+
+        self.__hostinfo_opt_edit.show()
 
     def show_devicepathwidget(self):
         """A widget to show the pathes to search for additional devices
 
         """
         self.__devicepathwidget.show()
+
     def create_devicepathwidget(self):
         """A widget to show the pathes to search for additional devices
 
         """
         self.__devicepathwidget = QtWidgets.QWidget()
-        self.__devicepathlab = QtWidgets.QLabel('Devicepathes') # Button to add a path        
-        self.__deviceaddpathbtn = QtWidgets.QPushButton('Add') # Button to add a path
+        self.__devicepathlab = QtWidgets.QLabel('Devicepathes')  # Button to add a path
+        self.__deviceaddpathbtn = QtWidgets.QPushButton('Add')  # Button to add a path
         self.__deviceaddpathbtn.clicked.connect(self.adddevicepath)
-        self.__devicerempathbtn = QtWidgets.QPushButton('Remove') # Button to remove a path
+        self.__devicerempathbtn = QtWidgets.QPushButton('Remove')  # Button to remove a path
         self.__devicerempathbtn.clicked.connect(self.remdevicepath)
         layout = QtWidgets.QFormLayout(self.__devicepathwidget)
         self.__devicepathlist = QtWidgets.QListWidget()
-        layout.addRow(self.__devicepathlab)        
+        layout.addRow(self.__devicepathlab)
         layout.addRow(self.__devicepathlist)
-        layout.addRow(self.__deviceaddpathbtn,self.__devicerempathbtn)
+        layout.addRow(self.__deviceaddpathbtn, self.__devicerempathbtn)
         self.__populate_devicepathlistWidget()
 
     def __populate_devicepathlistWidget(self):
         self.__devicepathlist.clear()
         for d in self.redvypr.device_paths:
             itm = QtWidgets.QListWidgetItem(d)
             self.__devicepathlist.addItem(itm)
 
+    def __property_widget(self, device=None):
+        """
+
+        Returns:
+
+        """
+        w = QtWidgets.QWidget()
+        if (device == None):
+            props = self.properties
+        else:
+            props = device.properties
+
     def adddevicepath(self):
         """Adds a path to the devicepathlist
         """
         folder = QtWidgets.QFileDialog.getExistingDirectory(self, 'Devicepath', '')
         if folder:
             self.redvypr.adddevicepath(folder)
 
@@ -1699,107 +1699,109 @@
         """Removes the selected device pathes
         """
         ind = self.__devicepathlist.currentRow()
         rempath = self.__devicepathlist.item(ind).text()
         # Remove from the main widget and redraw the whole list (is done by the signal emitted by redvypr)
         self.redvypr.remdevicepath(rempath)
 
-
-    def closeTab (self, currentIndex):
-        """ Closing a device tab and stopping the device
+    def closeTab(self, currentIndex):
+        """ Closing a device tab and removing the device
         """
+        funcname = __name__ + '.closeTab()'
         logger.debug('Closing the tab now')
         currentWidget = self.devicetabs.widget(currentIndex)
         # Search for the corresponding device
         for sendict in self.redvypr.devices:
-            if(sendict['widget'] == currentWidget):
+            if (sendict['widget'] == currentWidget):
                 device = sendict['device']
-                if(sendict['thread'] == None):
-                    pass
-                elif(sendict['thread'].is_alive()):
-                    device.comqueue.put('stop')                
-
+                self.redvypr.rem_device(device)
                 # Close the widgets (init/display)
                 currentWidget.close()
                 # Info
                 sendict['infowidget'].close()
-                self.redvypr.devices.remove(sendict)
+
                 self.devicetabs.removeTab(currentIndex)
                 break
-                
+
         self.update_devicewidgetsummary()
-        
+
     def close_application(self):
-        funcname = __name__ +'.close_application():'        
-        logger.debug(funcname + ' Closing ...')
+        funcname = __name__ + '.close_application():'
+        print(funcname + ' Closing ...')
         try:
             self.add_device_widget.close()
         except:
             pass
 
         for sendict in self.redvypr.devices:
-            self.redvypr.stop_device_thread(sendict['device'])
+            print(funcname + ' Stopping {:s}'.format(sendict['device'].name))
+            sendict['device'].thread_stop()
 
         time.sleep(1)
-        for sendict in self.redvypr.devices:        
+        for sendict in self.redvypr.devices:
             try:
-                sendict['thread'].kill()
+                sendict['device'].thread.kill()
             except:
                 pass
-            
-        #sys.exit()        
-        
-    def closeEvent(self,event):
+
+        print('All stopped, sys.exit()')
+        #sys.exit()
+        os._exit(1)
+
+    def closeEvent(self, event):
         self.close_application()
-        
+
+
 #        
 #
 # The main widget
 #
 #
 class redvyprMainWidget(QtWidgets.QMainWindow):
-    def __init__(self,width=None,height=None,config=None):
+    def __init__(self, width=None, height=None, config=None,hostname='redvypr',hostinfo_opt={}):
         super(redvyprMainWidget, self).__init__()
-        #self.setGeometry(0, 0, width, height)
-        
-        self.setWindowTitle("redvypr")
+        # self.setGeometry(0, 0, width, height)
+
+
+        #self.setWindowTitle("redvypr")
+        self.setWindowTitle(hostname)
         # Add the icon
-        self.setWindowIcon(QtGui.QIcon(_icon_file))           
-        
-        self.redvypr_widget = redvyprWidget(config=config)
+        self.setWindowIcon(QtGui.QIcon(_icon_file))
+
+        self.redvypr_widget = redvyprWidget(config=config,hostname=hostname,hostinfo_opt=hostinfo_opt)
         self.setCentralWidget(self.redvypr_widget)
         quitAction = QtWidgets.QAction("&Quit", self)
         quitAction.setShortcut("Ctrl+Q")
         quitAction.setStatusTip('Close the program')
         quitAction.triggered.connect(self.close_application)
 
         loadcfgAction = QtWidgets.QAction("&Load", self)
         loadcfgAction.setShortcut("Ctrl+O")
         loadcfgAction.setStatusTip('Load a configuration file')
         loadcfgAction.triggered.connect(self.load_config)
-        
+
         savecfgAction = QtWidgets.QAction("&Save", self)
         savecfgAction.setShortcut("Ctrl+S")
         savecfgAction.setStatusTip('Saves a configuration file')
         savecfgAction.triggered.connect(self.save_config)
 
         pathAction = QtWidgets.QAction("&Devicepath", self)
         pathAction.setShortcut("Ctrl+L")
         pathAction.setStatusTip('Edit the device path')
-        pathAction.triggered.connect(self.redvypr_widget.show_devicepathwidget)                
+        pathAction.triggered.connect(self.redvypr_widget.show_devicepathwidget)
 
         deviceAction = QtWidgets.QAction("&Add device", self)
         deviceAction.setShortcut("Ctrl+A")
         deviceAction.setStatusTip('Add a device')
         deviceAction.triggered.connect(self.open_add_device_widget)
 
         devcurAction = QtWidgets.QAction("&Go to device tab", self)
         devcurAction.setShortcut("Ctrl+D")
         devcurAction.setStatusTip('Go to the device tab')
-        devcurAction.triggered.connect(self.gotodevicetab)        
+        devcurAction.triggered.connect(self.gotodevicetab)
 
         conAction = QtWidgets.QAction("&Connect devices", self)
         conAction.setShortcut("Ctrl+C")
         conAction.setStatusTip('Connect the input/output datastreams of the devices')
         conAction.triggered.connect(self.connect_device_gui)
 
         self.statusBar()
@@ -1808,219 +1810,279 @@
         fileMenu = mainMenu.addMenu('&File')
         fileMenu.addAction(loadcfgAction)
         fileMenu.addAction(savecfgAction)
         fileMenu.addAction(pathAction)
         fileMenu.addAction(quitAction)
 
         deviceMenu = mainMenu.addMenu('&Devices')
-        deviceMenu.addAction(devcurAction)        
+        deviceMenu.addAction(devcurAction)
         deviceMenu.addAction(deviceAction)
-        deviceMenu.addAction(conAction) 
-        
-        
+        deviceMenu.addAction(conAction)
+
         # Help and About menu
         toolMenu = mainMenu.addMenu('&Tools')
         toolAction = QtWidgets.QAction("&Choose Device/Datakey ", self)
         toolAction.setStatusTip('Opens a window to choose an available device and/or datakeys')
         toolAction.triggered.connect(self.show_deviceselect)
         consoleAction = QtWidgets.QAction("&Open console", self)
         consoleAction.triggered.connect(self.open_console)
         consoleAction.setShortcut("Ctrl+N")
+        IPAction = QtWidgets.QAction("&Network interfaces", self)
+        IPAction.triggered.connect(self.open_ipwidget)
         toolMenu.addAction(toolAction)
+        toolMenu.addAction(IPAction)
         toolMenu.addAction(consoleAction)
-        
-        
+
         # Help and About menu
         helpAction = QtWidgets.QAction("&About", self)
         helpAction.setStatusTip('Information about the software version')
         helpAction.triggered.connect(self.about)
-        
+
         helpMenu = mainMenu.addMenu('&Help')
         helpMenu.addAction(helpAction)
 
         self.resize(width, height)
         self.show()
-        
+
     def open_console(self):
         self.redvypr_widget.open_console()
+
+    def open_ipwidget(self):
+        self.redvypr_widget.open_ipwidget()
+
     def gotodevicetab(self):
         self.redvypr_widget.devicetabs.setCurrentWidget(self.redvypr_widget.devicesummarywidget)
 
     def connect_device_gui(self):
         self.redvypr_widget.connect_device_gui()
 
     def about(self):
+        """
+Opens an "about" widget showing basic information.
+        """
         self._about_widget = QtWidgets.QWidget()
         layout = QtWidgets.QVBoxLayout(self._about_widget)
-        label = QtWidgets.QLabel("Python based Realtime Data Viewer and Processor (redvypr)")
-        label1 = QtWidgets.QLabel("Version: {:s}".format(str(version)))
-        layout.addWidget(label)
+        label1 = QtWidgets.QTextEdit()
+        label1.setReadOnly(True)
+        label1.setText(__platform__)
+        font = label1.document().defaultFont()
+        fontMetrics = QtGui.QFontMetrics(font)
+        textSize = fontMetrics.size(0, label1.toPlainText())
+        w = textSize.width() + 10
+        h = textSize.height() + 20
+        label1.setMinimumSize(w, h)
+        label1.setMaximumSize(w, h)
+        label1.resize(w, h)
+        label1.setReadOnly(True)
+
         layout.addWidget(label1)
         icon = QtGui.QPixmap(_logo_file)
         iconlabel = QtWidgets.QLabel()
         iconlabel.setPixmap(icon)
         layout.addWidget(iconlabel)
         self._about_widget.show()
-        
+
     def show_deviceselect(self):
-        self.__deviceselect__ = redvypr_devicelist_widget(redvypr=self.redvypr_widget.redvypr,deviceonly=True)
+        self.__deviceselect__ = gui.datastreamWidget(redvypr=self.redvypr_widget.redvypr, deviceonly=True)
         self.__deviceselect__.show()
+
     def open_add_device_widget(self):
         self.redvypr_widget.open_add_device_widget()
 
     def load_config(self):
         self.redvypr_widget.load_config()
-        
+
     def save_config(self):
         self.redvypr_widget.save_config()
 
     def close_application(self):
         self.redvypr_widget.close_application()
-            
-        sys.exit()
-        
-    def closeEvent(self,event):
-        self.close_application()
 
+        sys.exit()
 
+    def closeEvent(self, event):
+        self.close_application()
 
 
 #
 #
-# A splash screen
-#
-#
-
-class SplashScreen(QtWidgets.QWidget):
-    def __init__(self):
-        super().__init__()
-        self.setFixedSize(700, 350)
-        self.setWindowFlag(QtCore.Qt.FramelessWindowHint)
-        self.setAttribute(QtCore.Qt.WA_TranslucentBackground)
-        self.counter = 0
-        self.n = 50
-        #self.initUI()
-        self.timer = QtCore.QTimer()
-        self.timer.timeout.connect(self.count)
-        self.timer.start(100)
-        
-    def count(self):
-        # set progressbar value
-        #self.progressBar.setValue(self.counter)
-        # stop progress if counter
-        # is greater than n and
-        # display main window app
-        if self.counter >= self.n:
-            self.timer.stop()
-            self.close()
-            time.sleep(1)
-            ## Start the main application
-            #self.main_window()
-        self.counter += 1
-#
-#
 # Main function called from os
 #
 #
 #
-
 def redvypr_main():
-    print("Python based REaltime Data VYewer and PlotteR  (REDVYPR)")
-    
-    redvypr_help          = 'redvypr'
-    config_help           = 'Using a yaml config file'
-    config_help_nogui     = 'start redvypr without a gui'
-    config_help_path      = 'add path to search for redvypr modules'
-    config_help_hostname  = 'hostname of redvypr, overwrites the hostname in a possible configuration '            
-    config_help_add       = 'add device, can be called multiple times'
+    redvypr_help = 'redvypr'
+    config_help = 'Using a yaml config file'
+    config_help_nogui = 'start redvypr without a gui'
+    config_help_path = 'add path to search for redvypr modules'
+    config_help_hostname = 'hostname of redvypr, overwrites the hostname in a possible configuration '
+    config_help_add = 'add device, can be called multiple times, options/configuration by commas separated, -a test_device,[s],[mp/th],name:test_1,delay_s:0.4'
+    config_optional = 'optional information about the redvypr instance, multiple calls possible or separated by ",". Given as a key:data pair: --hostinfo location:lab --hostinfo lat:10.2,lon:30.4. The data is tried to be converted to an int, if that is not working as a float, if that is neither working at is passed as string'
     parser = argparse.ArgumentParser()
     parser.add_argument('--verbose', '-v', action='count')
-    parser.add_argument('--config', '-c',help=config_help)
-    parser.add_argument('--nogui', '-ng',help=config_help_nogui,action='store_true')
-    parser.add_argument('--add_path', '-p',help=config_help_path)
-    parser.add_argument('--hostname', '-hn',help=config_help_hostname)        
-    parser.add_argument('--add_device', '-a',help=config_help_add, action='append')        
+    parser.add_argument('--config', '-c', help=config_help)
+    parser.add_argument('--nogui', '-ng', help=config_help_nogui, action='store_true')
+    parser.add_argument('--add_path', '-p', help=config_help_path)
+    parser.add_argument('--hostname', '-hn', help=config_help_hostname)
+    parser.add_argument('--hostinfo', '-o', help=config_optional, action='append')
+    parser.add_argument('--add_device', '-a', help=config_help_add, action='append')
     parser.set_defaults(nogui=False)
     args = parser.parse_args()
 
     logging_level = logging.INFO
-    if(args.verbose == None):
-        logging_level = logging.INFO      
-    elif(args.verbose >= 1):
+    if (args.verbose == None):
+        logging_level = logging.INFO
+    elif (args.verbose >= 1):
         print('Debug logging level')
         logging_level = logging.DEBUG
-        
 
     logger.setLevel(logging_level)
-    
+
     # Check if we have a redvypr.yaml, TODO, add also default path
-    config_all = []
-    if(os.path.exists('redvypr.yaml')):
+    config_all = [] # Make a config all, the list can have several dictionaries that will be all processed by the redvypr initialization
+    if (os.path.exists('redvypr.yaml')):
         config_all.append('redvypr.yaml')
 
+    # Adding device module pathes
+    if (args.add_path is not None):
+        # print('devicepath',args.add_path)
+        modpath = os.path.abspath(args.add_path)
+        # print('devicepath',args.add_path,modpath)
+        configp = {'devicepath': modpath}
+        # print('Modpath',modpath)
+        config_all.append(configp)
+
     # Add the configuration
     config = args.config
-    if(config is not None):
-        config_all.append(config)   
-        
-     # Add device
-    if(args.add_device is not None):
-        
-        hostconfig = {'devices':[]}
-        print('devices',args.add_device)
+    if (config is not None):
+        config_all.append(config)
+
+    # Add device
+    if (args.add_device is not None):
+        hostconfig = {'devices': []}
+        print('devices!', args.add_device)
         for d in args.add_device:
-            logger.info('Adding device {:s}'.format(d))
-            dev = {'devicemodulename':d}
+            deviceconfig = {'autostart':False,'loglevel':logging_level,'mp':'thread','config':{},'subscriptions':[]}
+            if(',' in d):
+                devicemodulename = d.split(',')[0]
+                options = d.split(',')[1:]
+                for option in options:
+                    print('Option',option)
+                    if(option == 's'):
+                        deviceconfig['autostart'] = True
+                    elif (option == 'mp' or option == 'multiprocess') and (':' not in option):
+                        deviceconfig['mp'] = 'multiprocess'
+                    elif (option == 'th' or option == 'thread') and (':' not in option):
+                        deviceconfig['mp'] = 'thread'
+                    elif (':' in option):
+                        key = option.split(':')[0]
+                        data = option.split(':')[1]
+                        try:
+                            data = int(data)
+                        except:
+                            try:
+                                data = float(data)
+                            except:
+                                pass
+
+                        if(key == 'name'):
+                            deviceconfig[key] = data
+                        elif (key == 'loglevel') or (key == 'll'):
+                            try:
+                                loglevel_tmp = data
+                                loglevel_device = getattr(logging, loglevel_tmp.upper())
+                            except Exception as e:
+                                print(e)
+                                loglevel_tmp = 'INFO'
+                                loglevel_device = getattr(logging, loglevel_tmp.upper())
+
+                            print('Setting device {:s} to loglevel {:s}'.format(devicemodulename,loglevel_tmp))
+                            deviceconfig['loglevel'] = loglevel_device
+                        elif (key == 'subscribe'):
+                            print('Subscribe',data)
+                            deviceconfig['subscriptions'].append(data)
+                        else:
+                            deviceconfig['config'][key] = data
+            else:
+                devicemodulename = d
+            dev = {'devicemodulename': devicemodulename, 'deviceconfig':deviceconfig}
+            print('dev',dev)
             hostconfig['devices'].append(dev)
+            logger.info('Adding device {:s}, autostart: {:s},'.format(d,str(deviceconfig['autostart'])))
 
         config_all.append(hostconfig)
 
     # Add hostname
-    if(args.hostname is not None):
-        hostconfig = {'hostname':args.hostname}
-        config_all.append(hostconfig)
-        
-    
-    # Adding device module pathes
-    if(args.add_path is not None):
-        #print('devicepath',args.add_path)        
-        modpath = os.path.abspath(args.add_path)
-        #print('devicepath',args.add_path,modpath)
-        configp = {'devicepath':modpath}
-        #print('Modpath',modpath)
-        config_all.append(configp)
+    if (args.hostname is not None):
+        hostname = args.hostname
+    else:
+        hostname = 'redvypr'
+
+    # Add hostname
+    if (args.hostinfo is not None):
+        hostinfo = args.hostinfo
+    else:
+        hostinfo = []
+
+    # Add optional hostinformations
+    hostinfo_opt = {}
+    for i in hostinfo:
+        for info in i.split(','):
+            print('Info',info)
+            if(':' in info):
+                key = info.split(':')[0]
+                data = info.split(':')[1]
+                try:
+                    data = int(data)
+                except:
+                    try:
+                        data = float(data)
+                    except:
+                        pass
+
+                hostinfo_opt[key] = data
+            else:
+                logger.warning('Not a key:data pair in hostinfo, skipping {:sf}'.format(info))
+
+    #config_all.append({'hostinfo_opt':hostinfo_opt})
+    print('Hostinfo', hostinfo)
+    print('Hostinfo opt', hostinfo_opt)
 
     logger.debug('Configuration:\n {:s}\n'.format(str(config_all)))
+    QtCore.QLocale.setDefault(QtCore.QLocale(QtCore.QLocale.English, QtCore.QLocale.UnitedStates))
     # GUI oder command line?
-    if(args.nogui):
+    if (args.nogui):
         def handleIntSignal(signum, frame):
             '''Ask app to close if Ctrl+C is pressed.'''
             print('Received CTRL-C: Closing now')
             sys.exit()
-            
+
         signal.signal(signal.SIGINT, handleIntSignal)
         app = QtCore.QCoreApplication(sys.argv)
-        redvypr_obj = redvypr(config=config_all,nogui=True)
+        redvypr_obj = redvypr(config=config_all, hostinfo_opt=hostinfo_opt,hostname=hostname,nogui=True)
         sys.exit(app.exec_())
     else:
         app = QtWidgets.QApplication(sys.argv)
         screen = app.primaryScreen()
-        #print('Screen: %s' % screen.name())
+        # print('Screen: %s' % screen.name())
         size = screen.size()
-        #print('Size: %d x %d' % (size.width(), size.height()))
+        # print('Size: %d x %d' % (size.width(), size.height()))
         rect = screen.availableGeometry()
-        width = int(rect.width()*4/5)
-        height = int(rect.height()*2/3)
-        
+        width = int(rect.width() * 4 / 5)
+        height = int(rect.height() * 2 / 3)
+
+        logger.debug(
+            'Available screen size: {:d} x {:d} using {:d} x {:d}'.format(rect.width(), rect.height(), width, height))
+        ex = redvyprMainWidget(width=width, height=height, config=config_all,hostname=hostname,hostinfo_opt=hostinfo_opt)
 
-        logger.debug('Available screen size: {:d} x {:d} using {:d} x {:d}'.format(rect.width(), rect.height(),width,height))
-        ex = redvyprMainWidget(width=width,height=height,config=config_all)
-                  
         sys.exit(app.exec_())
 
 
 if __name__ == '__main__':
     redvypr_main()
-    
+
+
+
+
```

### Comparing `redvypr-0.4.4/redvypr/version.py` & `redvypr-0.5.3/redvypr/version.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.4.4/redvypr.egg-info/PKG-INFO` & `redvypr-0.5.3/redvypr.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: redvypr
-Version: 0.4.4
+Version: 0.5.3
 Summary: redvypr: REaltime Data Viewer and PRocessor (in PYthon)
 Home-page: https://github.com/redvypr/redvypr
 Author: Peter Holtermann
-Author-email: peter.holtermann@systemausfall.org
+Author-email: peter.holtermann@io-warnemuende.de
 License: GPLv03
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 redvypr: REaltime Data Viewer and PRocessor (in PYthon). Python based software to read, process, fuse, distribute, save and visualize data from various sensors.
-
```

### Comparing `redvypr-0.4.4/redvypr.egg-info/SOURCES.txt` & `redvypr-0.5.3/redvypr.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 LICENSE
 README.md
 setup.py
 redvypr/VERSION
 redvypr/__init__.py
+redvypr/config.py
+redvypr/configdata.py
 redvypr/data_packets.py
 redvypr/device.py
 redvypr/files.py
 redvypr/gui.py
 redvypr/redvypr.py
-redvypr/standard_device_widgets.py
-redvypr/utils.py
 redvypr/version.py
 redvypr.egg-info/PKG-INFO
 redvypr.egg-info/SOURCES.txt
 redvypr.egg-info/dependency_links.txt
 redvypr.egg-info/entry_points.txt
 redvypr.egg-info/not-zip-safe
 redvypr.egg-info/requires.txt
 redvypr.egg-info/top_level.txt
 redvypr/devices/__init__.py
-redvypr/devices/calibration.py
-redvypr/devices/csvlogger.py
-redvypr/devices/exampledevice.py
-redvypr/devices/exampledevice_bare.py
-redvypr/devices/gps_device.py
-redvypr/devices/mergedata.py
-redvypr/devices/netcdflogger.py
-redvypr/devices/network_device.py
-redvypr/devices/nmea_logbook.py
-redvypr/devices/nmea_sensor.py
-redvypr/devices/plot.py
-redvypr/devices/randdata.py
-redvypr/devices/rawdatadisp.py
-redvypr/devices/rawdatalogger.py
-redvypr/devices/rawdatareplay.py
-redvypr/devices/serial_device.py
-redvypr/devices/textlogger.py
-redvypr/devices/manufacturer/__init__.py
-redvypr/devices/manufacturer/ce_sensors/__init__.py
-redvypr/devices/manufacturer/ce_sensors/ads124s0x.py
-redvypr/devices/manufacturer/ce_sensors/datalogger.py
-redvypr/devices/manufacturer/ce_sensors/datalogger_rpi.py
-redvypr/devices/manufacturer/ce_sensors/heatflow_sensor.py
-redvypr/devices/manufacturer/leitenberger/__init__.py
-redvypr/devices/manufacturer/leitenberger/lrcal_Tfluid.py
+redvypr/devices/db/__init__.py
+redvypr/devices/db/influxdb_device.py
+redvypr/devices/develop/__init__.py
+redvypr/devices/develop/csvlogger.py
+redvypr/devices/fileio/__init__.py
+redvypr/devices/fileio/rawdatalogger.py
+redvypr/devices/fileio/rawdatareplay.py
+redvypr/devices/interface/__init__.py
+redvypr/devices/interface/serial_device.py
+redvypr/devices/network/__init__.py
+redvypr/devices/network/iored.py
+redvypr/devices/network/network_device.py
+redvypr/devices/network/zeromq_device.py
+redvypr/devices/plot/__init__.py
+redvypr/devices/plot/plot.py
+redvypr/devices/plot/plot_widgets.py
+redvypr/devices/plot/rawdatadisp.py
+redvypr/devices/processing/__init__.py
+redvypr/devices/processing/csvparser.py
+redvypr/devices/processing/nmeaparser.py
+redvypr/devices/processing/sensor_raw2unit.py
+redvypr/devices/test/__init__.py
+redvypr/devices/test/test_device.py
 redvypr/icon/icon_v02.ico
 redvypr/icon/icon_v02.png
 redvypr/icon/icon_v03.1.png
 redvypr/icon/icon_v03.1.svg
 redvypr/icon/icon_v03.1_small.png
 redvypr/icon/icon_v03.2.ico
 redvypr/icon/icon_v03.2.png
@@ -60,8 +58,23 @@
 redvypr/icon/logo_merged.svg
 redvypr/icon/logo_v01.svg
 redvypr/icon/logo_v02.svg
 redvypr/icon/logo_v03.1.png
 redvypr/icon/logo_v03.1.svg
 redvypr/icon/logo_v03.2.svg
 redvypr/icon/logo_v03.2_small.png
-redvypr/icon/redvypr_logo_v02.png
+redvypr/icon/redvypr_logo_v02.png
+redvypr/utils/__init__.py
+redvypr/utils/csv2dict/NMEA_functions.py
+redvypr/utils/csv2dict/VERSION
+redvypr/utils/csv2dict/__init__.py
+redvypr/utils/csv2dict/csv2dict.py
+redvypr/widgets/__init__.py
+redvypr/widgets/datastream_widget.py
+redvypr/widgets/gui_config_widgets.py
+redvypr/widgets/standard_device_widgets.py
+redvypr/widgets/tmp.py
+test/test_config.py
+test/test_configwidget.py
+test/test_devicescanwidget.py
+test/test_find_devices.py
+test/test_iored_1.py
```

### Comparing `redvypr-0.4.4/setup.py` & `redvypr-0.5.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 #with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 #    long_description = f.read()    
 
 setup(name='redvypr',
       version=version,
       description='redvypr: REaltime Data Viewer and PRocessor (in PYthon)',
       long_description='redvypr: REaltime Data Viewer and PRocessor (in PYthon). Python based software to read, process, fuse, distribute, save and visualize data from various sensors.',
+      long_description_content_type="text/x-rst",
       url='https://github.com/redvypr/redvypr',
       author='Peter Holtermann',
-      author_email='peter.holtermann@systemausfall.org',
+      author_email='peter.holtermann@io-warnemuende.de',
       license='GPLv03',
       #packages=['redvypr'],
       packages=find_packages(),
       scripts = [],
       entry_points={ 'console_scripts': ['redvypr=redvypr:redvypr_main']},
       package_data = {'':['VERSION','icon/*']},
-      install_requires=[ 'pyaml', 'pynmea2','netCDF4', 'tempsensor'],
+      install_requires=[ 'pyaml', 'pyqtgraph','netCDF4', 'pyqtconsole', 'pyserial','qtawesome'],
       classifiers=[
         'Development Status :: 4 - Beta',
         'Topic :: Scientific/Engineering',          
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',  
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
```

