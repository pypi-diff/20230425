# Comparing `tmp/mvt-2.2.5.tar.gz` & `tmp/mvt-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.2.5.tar", last modified: Thu Apr 13 16:02:19 2023, max compression
+gzip compressed data, was "mvt-2.2.6.tar", last modified: Tue Apr 25 10:26:51 2023, max compression
```

## Comparing `mvt-2.2.5.tar` & `mvt-2.2.6.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.253983 mvt-2.2.5/
--rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2021-07-26 21:43:37.000000 mvt-2.2.5/LICENSE
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-13 16:02:19.253983 mvt-2.2.5/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2509 2022-06-17 08:45:47.000000 mvt-2.2.5/README.md
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.177982 mvt-2.2.5/mvt/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.181982 mvt-2.2.5/mvt/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10608 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      973 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/cmd_check_adb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1083 2023-02-21 19:16:49.000000 mvt-2.2.5/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3798 2023-04-07 13:03:23.000000 mvt-2.2.5/mvt/android/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2589 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6078 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.181982 mvt-2.2.5/mvt/android/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.189983 mvt-2.2.5/mvt/android/modules/adb/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1271 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12263 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3211 2023-03-24 17:45:57.000000 mvt-2.2.5/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1772 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-03-24 17:25:12.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1975 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1633 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1329 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3080 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5130 2023-03-24 17:36:10.000000 mvt-2.2.5/mvt/android/modules/adb/files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2173 2023-03-29 12:05:03.000000 mvt-2.2.5/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1905 2023-03-01 21:33:36.000000 mvt-2.2.5/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12138 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/adb/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2685 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1367 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3543 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5656 2023-04-12 10:39:42.000000 mvt-2.2.5/mvt/android/modules/adb/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3474 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.193982 mvt-2.2.5/mvt/android/modules/androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      739 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1291 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2330 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2285 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3045 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3865 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3567 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-03-29 12:05:03.000000 mvt-2.2.5/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2918 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2115 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2935 2023-03-01 21:41:19.000000 mvt-2.2.5/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.193982 mvt-2.2.5/mvt/android/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2031 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/backup/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2175 2023-04-12 10:39:42.000000 mvt-2.2.5/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.197982 mvt-2.2.5/mvt/android/modules/bugreport/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      646 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2396 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3202 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2911 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2146 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2315 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2341 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4205 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3772 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.201983 mvt-2.2.5/mvt/android/parsers/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      549 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/android/parsers/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7503 2023-04-12 10:39:42.000000 mvt-2.2.5/mvt/android/parsers/backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    15778 2023-03-01 21:38:01.000000 mvt-2.2.5/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      723 2023-03-29 12:05:03.000000 mvt-2.2.5/mvt/android/parsers/getprop.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.205983 mvt-2.2.5/mvt/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-03-24 17:47:13.000000 mvt-2.2.5/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6435 2023-03-15 09:02:05.000000 mvt-2.2.5/mvt/common/command.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      765 2023-02-21 19:16:49.000000 mvt-2.2.5/mvt/common/help.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    20857 2023-04-07 13:06:52.000000 mvt-2.2.5/mvt/common/indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2132 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/common/logo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8227 2023-04-13 07:25:51.000000 mvt-2.2.5/mvt/common/module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1242 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/common/options.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7797 2023-03-24 17:57:36.000000 mvt-2.2.5/mvt/common/updates.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5787 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/common/url.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5919 2023-04-07 12:48:42.000000 mvt-2.2.5/mvt/common/utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-04-13 15:58:54.000000 mvt-2.2.5/mvt/common/version.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1365 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/common/virustotal.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.209982 mvt-2.2.5/mvt/ios/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10530 2023-03-01 21:38:00.000000 mvt-2.2.5/mvt/ios/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1189 2023-02-21 19:16:49.000000 mvt-2.2.5/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1170 2023-02-21 19:16:49.000000 mvt-2.2.5/mvt/ios/cmd_check_fs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8970 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/decrypt.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.209982 mvt-2.2.5/mvt/ios/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.209982 mvt-2.2.5/mvt/ios/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2450 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6222 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6614 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3829 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7223 2023-04-07 10:26:00.000000 mvt-2.2.5/mvt/ios/modules/base.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.213982 mvt-2.2.5/mvt/ios/modules/fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      894 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4691 2023-04-12 08:16:00.000000 mvt-2.2.5/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2669 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2887 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3014 2023-04-11 19:15:22.000000 mvt-2.2.5/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1651 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3734 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3735 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2140 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1369 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1692 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1702 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1425 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.233983 mvt-2.2.5/mvt/ios/modules/mixed/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1506 2023-04-11 18:44:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4947 2023-04-12 08:16:00.000000 mvt-2.2.5/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5072 2023-04-13 10:56:06.000000 mvt-2.2.5/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2349 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3354 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3185 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2148 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3215 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2906 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4377 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    14449 2023-04-07 10:26:00.000000 mvt-2.2.5/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5163 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1442 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2869 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6075 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5912 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5364 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5094 2023-04-12 10:39:42.000000 mvt-2.2.5/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4227 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6842 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4525 2023-04-07 12:42:40.000000 mvt-2.2.5/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6438 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4597 2023-04-12 16:50:38.000000 mvt-2.2.5/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10455 2023-02-21 19:11:24.000000 mvt-2.2.5/mvt/ios/modules/net_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    14195 2023-04-07 20:22:15.000000 mvt-2.2.5/mvt/ios/versions.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.181982 mvt-2.2.5/mvt.egg-info/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6096 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/entry_points.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)      189 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/requires.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-04-13 16:02:19.000000 mvt-2.2.5/mvt.egg-info/top_level.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-04-13 16:02:19.257983 mvt-2.2.5/setup.cfg
--rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-02-21 19:11:24.000000 mvt-2.2.5/setup.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.237983 mvt-2.2.5/tests/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.241983 mvt-2.2.5/tests/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2720 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android/test_backup_module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2061 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android/test_backup_parser.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1585 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android/test_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2372 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android/test_dumpsys_parser.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.245983 mvt-2.2.5/tests/android_androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.5/tests/android_androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      629 2023-03-01 21:41:05.000000 mvt-2.2.5/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      633 2023-03-01 21:39:38.000000 mvt-2.2.5/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1353 2023-03-29 10:50:24.000000 mvt-2.2.5/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      607 2023-03-01 21:41:53.000000 mvt-2.2.5/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-29 12:05:03.000000 mvt-2.2.5/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      670 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/android_androidqf/test_processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      618 2023-03-01 21:40:12.000000 mvt-2.2.5/tests/android_androidqf/test_settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      639 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.245983 mvt-2.2.5/tests/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1744 2023-04-07 12:35:45.000000 mvt-2.2.5/tests/common/test_indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2290 2023-03-01 21:38:00.000000 mvt-2.2.5/tests/common/test_utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/conftest.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.253983 mvt-2.2.5/tests/ios_backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      571 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1133 2023-04-11 19:12:42.000000 mvt-2.2.5/tests/ios_backup/test_calendar.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1125 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1008 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1010 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1266 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_backup/test_tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      688 2023-03-01 21:42:08.000000 mvt-2.2.5/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-13 16:02:19.253983 mvt-2.2.5/tests/ios_fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/ios_fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1139 2023-04-11 19:15:26.000000 mvt-2.2.5/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      573 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/test_check_android_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      587 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/test_check_android_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      526 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/test_check_ios_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      484 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/test_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      928 2023-02-21 19:11:25.000000 mvt-2.2.5/tests/utils.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2021-07-26 21:43:37.000000 mvt-2.2.6/LICENSE
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-25 10:26:51.083432 mvt-2.2.6/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2509 2022-06-17 08:45:47.000000 mvt-2.2.6/README.md
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    11066 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/android/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      973 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1083 2023-04-21 21:07:25.000000 mvt-2.2.6/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3798 2023-04-21 21:12:02.000000 mvt-2.2.6/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2589 2023-04-21 21:12:14.000000 mvt-2.2.6/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6077 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/android/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/adb/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1271 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12263 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3211 2023-03-24 17:45:57.000000 mvt-2.2.6/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1772 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-03-24 17:25:12.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1975 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1633 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1329 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3080 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5130 2023-03-24 17:36:10.000000 mvt-2.2.6/mvt/android/modules/adb/files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2173 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1905 2023-03-01 21:33:36.000000 mvt-2.2.6/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12138 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2685 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1367 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3543 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5656 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3474 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      739 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1291 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2330 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2285 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3045 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3865 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3567 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2918 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2115 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2935 2023-03-01 21:41:19.000000 mvt-2.2.6/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2031 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/backup/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2175 2023-04-19 15:56:21.000000 mvt-2.2.6/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/bugreport/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      646 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2396 2023-04-19 15:50:11.000000 mvt-2.2.6/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3202 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2911 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2146 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2315 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2341 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4205 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3772 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/parsers/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      549 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/parsers/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7503 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/android/parsers/backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    15778 2023-03-01 21:38:01.000000 mvt-2.2.6/mvt/android/parsers/dumpsys.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      723 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/parsers/getprop.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-03-24 17:47:13.000000 mvt-2.2.6/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6436 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/command.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      799 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/help.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    20857 2023-04-07 13:06:52.000000 mvt-2.2.6/mvt/common/indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2132 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/logo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     8227 2023-04-13 07:25:51.000000 mvt-2.2.6/mvt/common/module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1242 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/options.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7797 2023-03-24 17:57:36.000000 mvt-2.2.6/mvt/common/updates.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5787 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/url.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6695 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-04-25 10:18:47.000000 mvt-2.2.6/mvt/common/version.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1365 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/virustotal.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10628 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/ios/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1189 2023-04-21 21:13:24.000000 mvt-2.2.6/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1170 2023-04-21 21:13:33.000000 mvt-2.2.6/mvt/ios/cmd_check_fs.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     8970 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/decrypt.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2450 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6222 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6614 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3829 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7223 2023-04-07 10:26:00.000000 mvt-2.2.6/mvt/ios/modules/base.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      894 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4691 2023-04-12 08:16:00.000000 mvt-2.2.6/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2669 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2887 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3014 2023-04-11 19:15:22.000000 mvt-2.2.6/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1651 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3734 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3735 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2140 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1369 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1692 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1702 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1425 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/mvt/ios/modules/mixed/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1506 2023-04-11 18:44:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4984 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5072 2023-04-20 17:08:05.000000 mvt-2.2.6/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2349 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3354 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3185 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2148 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3215 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2906 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4377 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    14449 2023-04-07 10:26:00.000000 mvt-2.2.6/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5163 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1442 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2869 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6075 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5912 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5364 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5094 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4227 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6842 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4525 2023-04-07 12:42:40.000000 mvt-2.2.6/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6438 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4597 2023-04-12 16:50:38.000000 mvt-2.2.6/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10455 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/net_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    14195 2023-04-07 20:22:15.000000 mvt-2.2.6/mvt/ios/versions.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt.egg-info/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6096 2023-04-25 10:26:51.000000 mvt-2.2.6/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      189 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/requires.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/top_level.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-04-25 10:26:51.083432 mvt-2.2.6/setup.cfg
+-rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-02-21 19:11:24.000000 mvt-2.2.6/setup.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2720 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_backup_module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2061 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_backup_parser.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1585 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2372 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_dumpsys_parser.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/android_androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android_androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      629 2023-03-01 21:41:05.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      633 2023-03-01 21:39:38.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1353 2023-03-29 10:50:24.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      607 2023-03-01 21:41:53.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-29 12:05:03.000000 mvt-2.2.6/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      670 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      618 2023-03-01 21:40:12.000000 mvt-2.2.6/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      639 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1744 2023-04-07 12:35:45.000000 mvt-2.2.6/tests/common/test_indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2290 2023-03-01 21:38:00.000000 mvt-2.2.6/tests/common/test_utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/conftest.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/tests/ios_backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      571 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1133 2023-04-11 19:12:42.000000 mvt-2.2.6/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1125 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1008 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1010 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1266 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      688 2023-03-01 21:42:08.000000 mvt-2.2.6/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/tests/ios_fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1139 2023-04-11 19:15:26.000000 mvt-2.2.6/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      573 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_android_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      587 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_android_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      526 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_ios_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      484 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      928 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/utils.py
```

### Comparing `mvt-2.2.5/LICENSE` & `mvt-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/PKG-INFO` & `mvt-2.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.2.5
+Version: 2.2.6
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.2.5/README.md` & `mvt-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/cli.py` & `mvt-2.2.6/mvt/android/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 
 import click
-from rich.logging import RichHandler
 
 from mvt.common.cmd_check_iocs import CmdCheckIOCS
 from mvt.common.help import (HELP_MSG_FAST, HELP_MSG_HASHES, HELP_MSG_IOC,
                              HELP_MSG_LIST_MODULES, HELP_MSG_MODULE,
-                             HELP_MSG_OUTPUT, HELP_MSG_SERIAL)
+                             HELP_MSG_OUTPUT, HELP_MSG_SERIAL,
+                             HELP_MSG_VERBOSE)
 from mvt.common.logo import logo
 from mvt.common.updates import IndicatorsUpdates
+from mvt.common.utils import init_logging, set_verbose_logging
 
 from .cmd_check_adb import CmdAndroidCheckADB
 from .cmd_check_androidqf import CmdAndroidCheckAndroidQF
 from .cmd_check_backup import CmdAndroidCheckBackup
 from .cmd_check_bugreport import CmdAndroidCheckBugreport
 from .cmd_download_apks import DownloadAPKs
 from .modules.adb import ADB_MODULES
 from .modules.adb.packages import Packages
 from .modules.backup import BACKUP_MODULES
 from .modules.bugreport import BUGREPORT_MODULES
 
-# Setup logging using Rich.
-LOG_FORMAT = "[%(name)s] %(message)s"
-logging.basicConfig(level="INFO", format=LOG_FORMAT, handlers=[
-    RichHandler(show_path=False, log_time_format="%X")])
-log = logging.getLogger(__name__)
+init_logging()
+log = logging.getLogger("mvt")
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 #==============================================================================
 # Main
 #==============================================================================
 @click.group(invoke_without_command=False)
@@ -59,16 +57,18 @@
               help="Extract all packages installed on the phone, including system packages")
 @click.option("--virustotal", "-v", is_flag=True, help="Check packages on VirusTotal")
 @click.option("--output", "-o", type=click.Path(exists=False),
               help="Specify a path to a folder where you want to store the APKs")
 @click.option("--from-file", "-f", type=click.Path(exists=True),
               help="Instead of acquiring from phone, load an existing packages.json file for "
                    "lookups (mainly for debug purposes)")
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
-def download_apks(ctx, all_apks, virustotal, output, from_file, serial):
+def download_apks(ctx, all_apks, virustotal, output, from_file, serial, verbose):
+    set_verbose_logging(verbose)
     try:
         if from_file:
             download = DownloadAPKs.from_json(from_file)
         else:
             # TODO: Do we actually want to be able to run without storing any
             #       file?
             if not output:
@@ -108,16 +108,18 @@
 @click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
-def check_adb(ctx, serial, iocs, output, fast, list_modules, module):
+def check_adb(ctx, serial, iocs, output, fast, list_modules, module, verbose):
+    set_verbose_logging(verbose)
     cmd = CmdAndroidCheckADB(results_path=output, ioc_files=iocs,
                              module_name=module, serial=serial, fast_mode=fast)
 
     if list_modules:
         cmd.list_modules()
         return
 
@@ -137,17 +139,19 @@
              context_settings=CONTEXT_SETTINGS)
 @click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BUGREPORT_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_bugreport(ctx, iocs, output, list_modules, module, bugreport_path):
+def check_bugreport(ctx, iocs, output, list_modules, module, verbose, bugreport_path):
+    set_verbose_logging(verbose)
     # Always generate hashes as bug reports are small.
     cmd = CmdAndroidCheckBugreport(target_path=bugreport_path,
                                    results_path=output, ioc_files=iocs,
                                    module_name=module, hashes=True)
 
     if list_modules:
         cmd.list_modules()
@@ -168,17 +172,19 @@
 @cli.command("check-backup", help="Check an Android Backup",
              context_settings=CONTEXT_SETTINGS)
 @click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_backup(ctx, iocs, output, list_modules, backup_path):
+def check_backup(ctx, iocs, output, list_modules, verbose, backup_path):
+    set_verbose_logging(verbose)
     # Always generate hashes as backups are generally small.
     cmd = CmdAndroidCheckBackup(target_path=backup_path, results_path=output,
                                 ioc_files=iocs, hashes=True)
 
     if list_modules:
         cmd.list_modules()
         return
@@ -200,17 +206,19 @@
 @click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("ANDROIDQF_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_androidqf(ctx, iocs, output, list_modules, module, hashes, androidqf_path):
+def check_androidqf(ctx, iocs, output, list_modules, module, hashes, verbose, androidqf_path):
+    set_verbose_logging(verbose)
     cmd = CmdAndroidCheckAndroidQF(target_path=androidqf_path,
                                    results_path=output, ioc_files=iocs,
                                    module_name=module, hashes=hashes)
 
     if list_modules:
         cmd.list_modules()
         return
```

### Comparing `mvt-2.2.5/mvt/android/cmd_check_adb.py` & `mvt-2.2.6/mvt/android/cmd_check_adb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/cmd_check_androidqf.py` & `mvt-2.2.6/mvt/android/cmd_check_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/cmd_check_backup.py` & `mvt-2.2.6/mvt/android/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/cmd_check_bugreport.py` & `mvt-2.2.6/mvt/android/cmd_check_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/cmd_download_apks.py` & `mvt-2.2.6/mvt/android/cmd_download_apks.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,21 @@
 
 log = logging.getLogger(__name__)
 
 
 class DownloadAPKs(AndroidExtraction):
     """DownloadAPKs is the main class operating the download of APKs
     from the device.
-
-
     """
 
     def __init__(
         self,
         results_path: Optional[str] = None,
         all_apks: Optional[bool] = False,
-        packages: Optional[list] = None
+        packages: Optional[list] = None,
     ) -> None:
         """Initialize module.
         :param results_path: Path to the folder where data should be stored
         :param all_apks: Boolean indicating whether to download all packages
                          or filter known-goods
         :param packages: Provided list of packages, typically for JSON checks
         """
```

### Comparing `mvt-2.2.5/mvt/android/modules/adb/__init__.py` & `mvt-2.2.6/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/base.py` & `mvt-2.2.6/mvt/android/modules/adb/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/chrome_history.py` & `mvt-2.2.6/mvt/android/modules/adb/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_full.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.2.6/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/files.py` & `mvt-2.2.6/mvt/android/modules/adb/files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/getprop.py` & `mvt-2.2.6/mvt/android/modules/adb/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/logcat.py` & `mvt-2.2.6/mvt/android/modules/adb/logcat.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/packages.py` & `mvt-2.2.6/mvt/android/modules/adb/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/processes.py` & `mvt-2.2.6/mvt/android/modules/adb/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/root_binaries.py` & `mvt-2.2.6/mvt/android/modules/adb/root_binaries.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/selinux_status.py` & `mvt-2.2.6/mvt/android/modules/adb/selinux_status.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/settings.py` & `mvt-2.2.6/mvt/android/modules/adb/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/sms.py` & `mvt-2.2.6/mvt/android/modules/adb/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/adb/whatsapp.py` & `mvt-2.2.6/mvt/android/modules/adb/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/__init__.py` & `mvt-2.2.6/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/base.py` & `mvt-2.2.6/mvt/android/modules/androidqf/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/getprop.py` & `mvt-2.2.6/mvt/android/modules/androidqf/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/processes.py` & `mvt-2.2.6/mvt/android/modules/androidqf/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/settings.py` & `mvt-2.2.6/mvt/android/modules/androidqf/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/androidqf/sms.py` & `mvt-2.2.6/mvt/android/modules/androidqf/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/backup/base.py` & `mvt-2.2.6/mvt/android/modules/backup/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/backup/sms.py` & `mvt-2.2.6/mvt/android/modules/backup/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/__init__.py` & `mvt-2.2.6/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.2.6/mvt/android/modules/bugreport/accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/activities.py` & `mvt-2.2.6/mvt/android/modules/bugreport/activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/appops.py` & `mvt-2.2.6/mvt/android/modules/bugreport/appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/base.py` & `mvt-2.2.6/mvt/android/modules/bugreport/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.2.6/mvt/android/modules/bugreport/battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.2.6/mvt/android/modules/bugreport/battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.2.6/mvt/android/modules/bugreport/dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/getprop.py` & `mvt-2.2.6/mvt/android/modules/bugreport/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/packages.py` & `mvt-2.2.6/mvt/android/modules/bugreport/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/modules/bugreport/receivers.py` & `mvt-2.2.6/mvt/android/modules/bugreport/receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/parsers/__init__.py` & `mvt-2.2.6/mvt/android/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/parsers/backup.py` & `mvt-2.2.6/mvt/android/parsers/backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/parsers/dumpsys.py` & `mvt-2.2.6/mvt/android/parsers/dumpsys.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/android/parsers/getprop.py` & `mvt-2.2.6/mvt/android/parsers/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/cmd_check_iocs.py` & `mvt-2.2.6/mvt/common/cmd_check_iocs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/command.py` & `mvt-2.2.6/mvt/common/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,41 +38,43 @@
         self.results_path = results_path
         self.ioc_files = ioc_files if ioc_files else []
         self.module_name = module_name
         self.serial = serial
         self.fast_mode = fast_mode
         self.log = log
 
-        self.iocs = Indicators(log=log)
-        self.iocs.load_indicators_files(self.ioc_files)
-
         # This list will contain all executed modules.
         # We can use this to reference e.g. self.executed[0].results.
         self.executed = []
-
         self.detected_count = 0
-
         self.hashes = hashes
         self.hash_values = []
         self.timeline = []
         self.timeline_detected = []
 
+        # Load IOCs
+        self._create_storage()
+        self._setup_logging()
+        self.iocs = Indicators(log=log)
+        self.iocs.load_indicators_files(self.ioc_files)
+
     def _create_storage(self) -> None:
         if self.results_path and not os.path.exists(self.results_path):
             try:
                 os.makedirs(self.results_path)
             except Exception as exc:
                 self.log.critical("Unable to create output folder %s: %s",
                                   self.results_path, exc)
                 sys.exit(1)
 
-    def _add_log_file_handler(self, logger: logging.Logger) -> None:
+    def _setup_logging(self):
         if not self.results_path:
             return
 
+        logger = logging.getLogger("mvt")
         file_handler = logging.FileHandler(os.path.join(self.results_path,
                                                         "command.log"))
         formatter = logging.Formatter("%(asctime)s - %(name)s - "
                                       "%(levelname)s - %(message)s")
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
@@ -146,28 +148,26 @@
     def module_init(self, module: MVTModule) -> None:
         raise NotImplementedError
 
     def finish(self) -> None:
         raise NotImplementedError
 
     def run(self) -> None:
-        self._create_storage()
-        self._add_log_file_handler(self.log)
 
         try:
             self.init()
         except NotImplementedError:
             pass
 
         for module in self.modules:
             if self.module_name and module.__name__ != self.module_name:
                 continue
 
+            # FIXME: do we need the logger here
             module_logger = logging.getLogger(module.__module__)
-            self._add_log_file_handler(module_logger)
 
             m = module(target_path=self.target_path,
                        results_path=self.results_path,
                        fast_mode=self.fast_mode,
                        log=module_logger)
 
             if self.iocs.total_ioc_count:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mvt-2.2.5/mvt/common/help.py` & `mvt-2.2.6/mvt/common/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 # Help messages of repeating options.
 HELP_MSG_OUTPUT = "Specify a path to a folder where you want to store JSON results"
 HELP_MSG_IOC = "Path to indicators file (can be invoked multiple time)"
 HELP_MSG_FAST = "Avoid running time/resource consuming features"
 HELP_MSG_LIST_MODULES = "Print list of available modules and exit"
 HELP_MSG_MODULE = "Name of a single module you would like to run instead of all"
 HELP_MSG_HASHES = "Generate hashes of all the files analyzed"
+HELP_MSG_VERBOSE = "Verbose mode"
 
 # Android-specific.
 HELP_MSG_SERIAL = "Specify a device serial number or HOST:PORT connection string"
```

### Comparing `mvt-2.2.5/mvt/common/indicators.py` & `mvt-2.2.6/mvt/common/indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/logo.py` & `mvt-2.2.6/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/module.py` & `mvt-2.2.6/mvt/common/module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/options.py` & `mvt-2.2.6/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/updates.py` & `mvt-2.2.6/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/url.py` & `mvt-2.2.6/mvt/common/url.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/common/utils.py` & `mvt-2.2.6/mvt/common/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import datetime
 import hashlib
+import logging
 import os
 import re
 from typing import Any, Iterator, Union
 
+from rich.logging import RichHandler
+
 
 def convert_chrometime_to_datetime(timestamp: int) -> datetime.datetime:
     """Converts Chrome timestamp to a datetime.
 
     :param timestamp: Chrome timestamp as int.
     :type timestamp: int
     :returns: datetime.
@@ -193,7 +196,32 @@
                     continue
                 except PermissionError:
                     log.error("Failed to hash the file %s: permission denied",
                               file_path)
                     continue
 
                 yield {"file_path": file_path, "sha256": sha256}
+
+
+def init_logging(verbose: bool = False):
+    """
+    Initialise logging for the MVT module
+    """
+    # Setup logging using Rich.
+    log = logging.getLogger("mvt")
+    log.setLevel(logging.DEBUG)
+    consoleHandler = RichHandler(show_path=False, log_time_format="%X")
+    consoleHandler.setFormatter(logging.Formatter("[%(name)s] %(message)s"))
+    if verbose:
+        consoleHandler.setLevel(logging.DEBUG)
+    else:
+        consoleHandler.setLevel(logging.INFO)
+    log.addHandler(consoleHandler)
+
+
+def set_verbose_logging(verbose: bool = False):
+    log = logging.getLogger("mvt")
+    handler = log.handlers[0]
+    if verbose:
+        handler.setLevel(logging.DEBUG)
+    else:
+        handler.setLevel(logging.INFO)
```

### Comparing `mvt-2.2.5/mvt/common/virustotal.py` & `mvt-2.2.6/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/cli.py` & `mvt-2.2.6/mvt/ios/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,35 @@
 #   https://license.mvt.re/1.1/
 
 import json
 import logging
 import os
 
 import click
-from rich.logging import RichHandler
 from rich.prompt import Prompt
 
 from mvt.common.cmd_check_iocs import CmdCheckIOCS
 from mvt.common.help import (HELP_MSG_FAST, HELP_MSG_HASHES, HELP_MSG_IOC,
                              HELP_MSG_LIST_MODULES, HELP_MSG_MODULE,
-                             HELP_MSG_OUTPUT)
+                             HELP_MSG_OUTPUT, HELP_MSG_VERBOSE)
 from mvt.common.logo import logo
 from mvt.common.options import MutuallyExclusiveOption
 from mvt.common.updates import IndicatorsUpdates
-from mvt.common.utils import generate_hashes_from_path
+from mvt.common.utils import (generate_hashes_from_path, init_logging,
+                              set_verbose_logging)
 
 from .cmd_check_backup import CmdIOSCheckBackup
 from .cmd_check_fs import CmdIOSCheckFS
 from .decrypt import DecryptBackup
 from .modules.backup import BACKUP_MODULES
 from .modules.fs import FS_MODULES
 from .modules.mixed import MIXED_MODULES
 
-# Setup logging using Rich.
-LOG_FORMAT = "[%(name)s] %(message)s"
-logging.basicConfig(level="INFO", format=LOG_FORMAT, handlers=[
-    RichHandler(show_path=False, log_time_format="%X")])
-log = logging.getLogger(__name__)
+init_logging()
+log = logging.getLogger("mvt")
 
 # Set this environment variable to a password if needed.
 MVT_IOS_BACKUP_PASSWORD = "MVT_IOS_BACKUP_PASSWORD"
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 #==============================================================================
@@ -162,17 +159,20 @@
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_backup(ctx, iocs, output, fast, list_modules, module, hashes, backup_path):
+def check_backup(ctx, iocs, output, fast, list_modules, module, hashes, verbose, backup_path):
+    set_verbose_logging(verbose)
+
     cmd = CmdIOSCheckBackup(target_path=backup_path, results_path=output,
                             ioc_files=iocs, module_name=module, fast_mode=fast,
                             hashes=hashes)
 
     if list_modules:
         cmd.list_modules()
         return
@@ -195,17 +195,19 @@
               default=[], help=HELP_MSG_IOC)
 @click.option("--output", "-o", type=click.Path(exists=False),
               help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
+@click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("DUMP_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_fs(ctx, iocs, output, fast, list_modules, module, hashes, dump_path):
+def check_fs(ctx, iocs, output, fast, list_modules, module, hashes, verbose, dump_path):
+    set_verbose_logging(verbose)
     cmd = CmdIOSCheckFS(target_path=dump_path, results_path=output,
                         ioc_files=iocs, module_name=module, fast_mode=fast,
                         hashes=hashes)
 
     if list_modules:
         cmd.list_modules()
         return
```

### Comparing `mvt-2.2.5/mvt/ios/cmd_check_backup.py` & `mvt-2.2.6/mvt/ios/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/cmd_check_fs.py` & `mvt-2.2.6/mvt/ios/cmd_check_fs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/decrypt.py` & `mvt-2.2.6/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/backup/backup_info.py` & `mvt-2.2.6/mvt/ios/modules/backup/backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.2.6/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/backup/manifest.py` & `mvt-2.2.6/mvt/ios/modules/backup/manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/backup/profile_events.py` & `mvt-2.2.6/mvt/ios/modules/backup/profile_events.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/base.py` & `mvt-2.2.6/mvt/ios/modules/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/__init__.py` & `mvt-2.2.6/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/analytics.py` & `mvt-2.2.6/mvt/ios/modules/fs/analytics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.2.6/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/cache_files.py` & `mvt-2.2.6/mvt/ios/modules/fs/cache_files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/filesystem.py` & `mvt-2.2.6/mvt/ios/modules/fs/filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.2.6/mvt/ios/modules/fs/net_netusage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.2.6/mvt/ios/modules/fs/safari_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.2.6/mvt/ios/modules/fs/shutdownlog.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/version_history.py` & `mvt-2.2.6/mvt/ios/modules/fs/version_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.2.6/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.2.6/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.2.6/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.2.6/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/__init__.py` & `mvt-2.2.6/mvt/ios/modules/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/applications.py` & `mvt-2.2.6/mvt/ios/modules/mixed/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
                 ioc = self.indicators.check_app_id(result["softwareVersionBundleId"])
                 if ioc:
                     self.log.warning("Malicious application %s identified", result["softwareVersionBundleId"])
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
-            if result.get("sourceApp", "com.apple.AppStore") != "com.apple.AppStore":
-                self.log.warning("Suspicious app not installed from the App Store: %s", result["softwareVersionBundleId"])
+            if result.get("sourceApp", "com.apple.AppStore") not in ["com.apple.AppStore", "com.apple.dmd", "dmd"]:
+                self.log.warning("Suspicious app not installed from the App Store or MDM: %s", result["softwareVersionBundleId"])
                 self.detected.append(result)
 
     def _parse_itunes_timestamp(self, entry: Dict[str, Any]) -> None:
         """
         Parse the iTunes metadata info
         """
         if entry.get("com.apple.iTunesStore.downloadInfo", {}).get("purchaseDate", None):
```

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/calendar.py` & `mvt-2.2.6/mvt/ios/modules/mixed/calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/calls.py` & `mvt-2.2.6/mvt/ios/modules/mixed/calls.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.2.6/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.2.6/mvt/ios/modules/mixed/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/contacts.py` & `mvt-2.2.6/mvt/ios/modules/mixed/contacts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.2.6/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.2.6/mvt/ios/modules/mixed/firefox_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.2.6/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.2.6/mvt/ios/modules/mixed/interactionc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/locationd.py` & `mvt-2.2.6/mvt/ios/modules/mixed/locationd.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.2.6/mvt/ios/modules/mixed/net_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.2.6/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.2.6/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.2.6/mvt/ios/modules/mixed/safari_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.2.6/mvt/ios/modules/mixed/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/sms.py` & `mvt-2.2.6/mvt/ios/modules/mixed/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.2.6/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/tcc.py` & `mvt-2.2.6/mvt/ios/modules/mixed/tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.2.6/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.2.6/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.2.6/mvt/ios/modules/mixed/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/modules/net_base.py` & `mvt-2.2.6/mvt/ios/modules/net_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt/ios/versions.py` & `mvt-2.2.6/mvt/ios/versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/mvt.egg-info/PKG-INFO` & `mvt-2.2.6/mvt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.2.5
+Version: 2.2.6
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.2.5/mvt.egg-info/SOURCES.txt` & `mvt-2.2.6/mvt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/setup.cfg` & `mvt-2.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android/test_backup_module.py` & `mvt-2.2.6/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android/test_backup_parser.py` & `mvt-2.2.6/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android/test_bugreport.py` & `mvt-2.2.6/tests/android/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android/test_dumpsys_parser.py` & `mvt-2.2.6/tests/android/test_dumpsys_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.2.6/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.2.6/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.2.6/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.2.6/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_getprop.py` & `mvt-2.2.6/tests/android_androidqf/test_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_processes.py` & `mvt-2.2.6/tests/android_androidqf/test_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_settings.py` & `mvt-2.2.6/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/android_androidqf/test_sms.py` & `mvt-2.2.6/tests/android_androidqf/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/common/test_indicators.py` & `mvt-2.2.6/tests/common/test_indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/common/test_utils.py` & `mvt-2.2.6/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/conftest.py` & `mvt-2.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_backup_info.py` & `mvt-2.2.6/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_calendar.py` & `mvt-2.2.6/tests/ios_backup/test_calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_datausage.py` & `mvt-2.2.6/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_manifest.py` & `mvt-2.2.6/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.2.6/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_sms.py` & `mvt-2.2.6/tests/ios_backup/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_tcc.py` & `mvt-2.2.6/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.2.6/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/ios_fs/test_filesystem.py` & `mvt-2.2.6/tests/ios_fs/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/test_check_android_androidqf.py` & `mvt-2.2.6/tests/test_check_android_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/test_check_android_bugreport.py` & `mvt-2.2.6/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/test_check_ios_backup.py` & `mvt-2.2.6/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.5/tests/utils.py` & `mvt-2.2.6/tests/utils.py`

 * *Files identical despite different names*

