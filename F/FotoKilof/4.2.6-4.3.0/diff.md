# Comparing `tmp/FotoKilof-4.2.6.tar.gz` & `tmp/FotoKilof-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FotoKilof-4.2.6.tar", last modified: Thu Feb  2 19:30:49 2023, max compression
+gzip compressed data, was "FotoKilof-4.3.0.tar", last modified: Tue Apr 25 00:01:00 2023, max compression
```

## Comparing `FotoKilof-4.2.6.tar` & `FotoKilof-4.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5544 2023-02-02 19:10:40.000000 FotoKilof-4.2.6/CHANGES.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.2.6/CONTRIBUTING.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.598976 FotoKilof-4.2.6/FotoKilof.egg-info/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5394 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1188 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/SOURCES.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/dependency_links.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       46 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/entry_points.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       26 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/requires.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-02-02 19:30:49.000000 FotoKilof-4.2.6/FotoKilof.egg-info/top_level.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.2.6/LICENSE
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      208 2022-12-11 22:24:11.000000 FotoKilof-4.2.6/MANIFEST.in
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5394 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.2.6/PROGRAM_GUIDE.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4850 2023-01-28 21:05:43.000000 FotoKilof-4.2.6/README.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.590976 FotoKilof-4.2.6/doc/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.598976 FotoKilof-4.2.6/doc/en/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.2.6/doc/en/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.602976 FotoKilof-4.2.6/doc/pl/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.2.6/doc/pl/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.602976 FotoKilof-4.2.6/fotokilof/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-02-02 19:30:48.000000 FotoKilof-4.2.6/fotokilof/__init__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)   110840 2023-02-02 19:22:51.000000 FotoKilof-4.2.6/fotokilof/__main__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     8030 2023-01-14 21:01:25.000000 FotoKilof-4.2.6/fotokilof/common.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.2.6/fotokilof/convert.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10842 2023-01-14 21:14:45.000000 FotoKilof-4.2.6/fotokilof/convert_wand.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.2.6/fotokilof/entries.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.2.6/fotokilof/gui.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-02-02 19:03:46.000000 FotoKilof-4.2.6/fotokilof/ini_read.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.2.6/fotokilof/ini_save.py
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.602976 FotoKilof-4.2.6/fotokilof/locale/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.594976 FotoKilof-4.2.6/fotokilof/locale/bg/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.2.6/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.594976 FotoKilof-4.2.6/fotokilof/locale/de/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/de/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.2.6/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.594976 FotoKilof-4.2.6/fotokilof/locale/en/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/en/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.2.6/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.2.6/fotokilof/locale/fotokilof.pot
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.594976 FotoKilof-4.2.6/fotokilof/locale/id/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/id/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.2.6/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.594976 FotoKilof-4.2.6/fotokilof/locale/pl/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.2.6/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.598976 FotoKilof-4.2.6/fotokilof/locale/tr/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/fotokilof/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-02-02 19:22:54.000000 FotoKilof-4.2.6/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.2.6/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.2.6/fotokilof/log.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.2.6/fotokilof/magick.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.2.6/fotokilof/mswindows.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4257 2023-01-14 20:51:23.000000 FotoKilof-4.2.6/fotokilof/preview.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-02-02 19:10:50.000000 FotoKilof-4.2.6/fotokilof/version.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       38 2023-02-02 19:30:49.606976 FotoKilof-4.2.6/setup.cfg
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1051 2022-12-11 22:22:38.000000 FotoKilof-4.2.6/setup.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5622 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/CHANGES.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.3.0/CONTRIBUTING.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/FotoKilof.egg-info/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1188 2023-04-25 00:01:00.000000 FotoKilof-4.3.0/FotoKilof.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       45 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/entry_points.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       25 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/requires.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/top_level.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.3.0/LICENSE
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      208 2022-12-11 22:24:11.000000 FotoKilof-4.3.0/MANIFEST.in
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.3.0/PROGRAM_GUIDE.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4845 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/README.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/doc/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/doc/en/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.3.0/doc/en/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/doc/pl/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.3.0/doc/pl/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/fotokilof/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/fotokilof/__init__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)   109944 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/fotokilof/__main__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7911 2023-02-25 15:39:02.000000 FotoKilof-4.3.0/fotokilof/common.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.3.0/fotokilof/convert.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10946 2023-02-25 23:07:28.000000 FotoKilof-4.3.0/fotokilof/convert_wand.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.3.0/fotokilof/entries.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.3.0/fotokilof/gui.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-02-25 15:43:09.000000 FotoKilof-4.3.0/fotokilof/ini_read.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.3.0/fotokilof/ini_save.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/fotokilof/locale/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/bg/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/de/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/en/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.3.0/fotokilof/locale/fotokilof.pot
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/id/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/pl/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/tr/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.3.0/fotokilof/log.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.3.0/fotokilof/magick.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.3.0/fotokilof/mswindows.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4284 2023-03-09 22:49:13.000000 FotoKilof-4.3.0/fotokilof/preview.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/fotokilof/version.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       38 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/setup.cfg
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1050 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/setup.py
```

### Comparing `FotoKilof-4.2.6/CHANGES.md` & `FotoKilof-4.3.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 ## 2023
 
+4.3.0 ttkbootstrap - solve many small annoying things, less duplicated code,
+
 4.2.6 removed theme selector, better paned window
 
 4.2.5 very small polishing tkinter, F1 fixed, progressbar works
 
 4.2.4 fix gui, better handle open file, fix crop
 
 ## 2022
```

### Comparing `FotoKilof-4.2.6/CONTRIBUTING.md` & `FotoKilof-4.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/FotoKilof.egg-info/PKG-INFO` & `FotoKilof-4.3.0/FotoKilof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.2.6
+Version: 4.3.0
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -122,15 +121,15 @@
 
 ### Install
 
 #### Linux
 
 Install requirements:
 ```bash
-apt-get install python3-pip python3-tk python3-wand idle imagemagick
+apt-get install python3-pip python3-tk python3-wand imagemagick
 ```
 
 Install as PyPi package by PIP:
 ```bash
 python3 -m pip install fotokilof
 ```
 
@@ -183,9 +182,7 @@
  - Olm - testing on Windows,
  - Carbene Hu - idea to fix issue
  - Mert Cobanov - Turkish translation
 
 ---
 
 ![Python powered](python-powered.png)
-
-
```

### Comparing `FotoKilof-4.2.6/FotoKilof.egg-info/SOURCES.txt` & `FotoKilof-4.3.0/FotoKilof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/LICENSE` & `FotoKilof-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/PKG-INFO` & `FotoKilof-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.2.6
+Version: 4.3.0
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -122,15 +121,15 @@
 
 ### Install
 
 #### Linux
 
 Install requirements:
 ```bash
-apt-get install python3-pip python3-tk python3-wand idle imagemagick
+apt-get install python3-pip python3-tk python3-wand imagemagick
 ```
 
 Install as PyPi package by PIP:
 ```bash
 python3 -m pip install fotokilof
 ```
 
@@ -183,9 +182,7 @@
  - Olm - testing on Windows,
  - Carbene Hu - idea to fix issue
  - Mert Cobanov - Turkish translation
 
 ---
 
 ![Python powered](python-powered.png)
-
-
```

### Comparing `FotoKilof-4.2.6/PROGRAM_GUIDE.md` & `FotoKilof-4.3.0/PROGRAM_GUIDE.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/README.md` & `FotoKilof-4.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 ### Install
 
 #### Linux
 
 Install requirements:
 ```bash
-apt-get install python3-pip python3-tk python3-wand idle imagemagick
+apt-get install python3-pip python3-tk python3-wand imagemagick
 ```
 
 Install as PyPi package by PIP:
 ```bash
 python3 -m pip install fotokilof
 ```
```

### Comparing `FotoKilof-4.2.6/doc/en/fotokilof.md` & `FotoKilof-4.3.0/doc/en/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/doc/pl/fotokilof.md` & `FotoKilof-4.3.0/doc/pl/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/__init__.py` & `FotoKilof-4.3.0/fotokilof/__init__.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/__main__.py` & `FotoKilof-4.3.0/fotokilof/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,24 +25,17 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
 nice GUI for ImageMagick command common used (by me)
 """
 
-from tkinter import Tk, ttk, Label, PhotoImage, PanedWindow, Canvas
-from tkinter.scrolledtext import ScrolledText
+from tkinter import PhotoImage, Canvas, Label
 from tkinter import filedialog, messagebox
 from tkinter import StringVar, IntVar, TclError, TkVersion
-from tkinter import N, S, W, E, X, BOTH, LEFT, RIGHT, TOP, BOTTOM, END, DISABLED, NORMAL, HORIZONTAL
-
-try:
-    from tkcolorpicker import askcolor
-except:
-    from tkinter.colorchooser import askcolor
 
 try:
     from wand.version import MAGICK_VERSION, VERSION
     IMAGEMAGICK_WAND_VERSION = "IM " + MAGICK_VERSION.split(' ')[1] + " : Wand " + VERSION
     IMAGEMAGICK_WAND = "OK"
 except:
     print(" ImageMagick or Wand-py not found")
@@ -52,15 +45,20 @@
 # standard modules
 import datetime
 import gettext
 import os
 import platform
 import sys
 import tempfile
-from idlelib.tooltip import Hovertip
+
+import ttkbootstrap as ttk
+from ttkbootstrap.scrolled import ScrolledText, ScrolledFrame
+from ttkbootstrap.tooltip import ToolTip
+from ttkbootstrap.dialogs.colorchooser import ColorChooserDialog
+from ttkbootstrap.constants import N, S, W, E, X, BOTH, LEFT, RIGHT, TOP, BOTTOM, END, DISABLED, NORMAL, HORIZONTAL
 
 # my modules
 import convert
 import convert_wand
 import common
 import gui
 import ini_read
@@ -118,15 +116,15 @@
 
 
 def preview_orig_clear():
     """ clear every preview if doesn't choose file """
     log.write_log("clear preview", "M")
     c_preview_orig_pi.delete('all')
     c_histogram_orig.delete('all')
-    # if no original, new previe should be clear too
+    # if no original, new preview should be clear too
     preview_new_clear()
 
 
 def preview_new_clear():
     """ clear every preview if doesn't choose file """
     log.write_log("clear preview", "M")
     c_preview_new_pi.delete('all')
@@ -541,40 +539,34 @@
         convert_wand.save_close_clone(clone, path_to_file_out(0), img_exif_on.get())
         preview_new(path_to_file_out(0))
     progress_files.set(_("done"))
 
 
 def open_file_logo():
     """ open logo file for inserting """
-    directory = os.path.dirname(file_logo_path.get())
-    if mswindows.windows() == 1:
-        filetypes = ((_("All graphics files"), ".JPG .JPEG .PNG .TIF .TIFF"),
-                     (_("JPG files"), ".JPG .JPEG"),
-                     (_("PNG files"), ".PNG"),
-                     (_("TIFF files"), ".TIF .TIFF"),
-                     (_("SVG files"), ".SVG"),
-                     (_("ALL types"), "*"))
-    else:
-        filetypes = ((_("All graphics files"),
-                    ".JPG .jpg .JPEG .jpeg .PNG .png .TIF .tif .TIFF .tiff"),
-                     (_("JPG files"), ".JPG .jpg .JPEG .jpeg"),
-                     (_("PNG files"), ".PNG .png"),
-                     (_("TIFF files"), ".TIF .tif .TIFF .tiff"),
-                     (_("SVG files"), ".SVG .svg"),
-                     (_("ALL types"), "*"))
+    filename = open_file_dialog(os.path.dirname(file_logo_path.get()),
+                                _("Select logo picture for inserting"))
+
+    file_logo_path.set(filename)
 
-    file_logo_path.set(filedialog.askopenfilename(initialdir=directory,
-                                                  filetypes=filetypes,
-                                                  title=_("Select logo picture for inserting")))
     if os.path.isfile(file_logo_path.get()):
         preview_logo()
     else:
         preview_logo_clear()
 
 
+def open_file():
+    """ open image for processing """
+
+    dirname = os.path.dirname(file_in_path.get())
+    filename = open_file_dialog(dirname,
+                                _("Select picture for processing"))
+    open_file_common(dirname, filename)
+
+
 def open_file_common(cwd, filename):
     """ common function for: open, first, last, next, prev """
     if filename is not None:
         try:
             file_in_path.set(os.path.normpath(os.path.join(cwd, filename)))
             root.title(window_title + file_in_path.get())
             image_size =  convert_wand.get_image_size(file_in_path.get())
@@ -586,38 +578,36 @@
                 preview_new_refresh("none")
             else:
                 preview_orig_clear()
         except:
             log.write_log("Error in open_file_common", "E")
 
 
-def open_file():
-    """ open image for processing """
-    filename = None
-    dir_name = os.path.dirname(file_in_path.get())
+def open_file_dialog(dir_initial, title):
+    """ open file dialog function for image and logo """
     if mswindows.windows() == 1:
-        filetypes = ((_("All graphics files"), ".JPG .JPEG .PNG .TIF .TIFF"),
+        filetypes = ((_("All graphics files"),
+                    ".JPG .JPEG .PNG .TIF .TIFF"),
                      (_("JPG files"), ".JPG .JPEG"),
                      (_("PNG files"), ".PNG"),
                      (_("TIFF files"), ".TIF .TIFF"),
-                     (_("SVG files"), ".SVG"),
                      (_("ALL types"), "*"))
     else:
         filetypes = ((_("All graphics files"),
                     ".JPG .jpg .JPEG .jpeg .PNG .png .TIF .tif .TIFF .tiff"),
                      (_("JPG files"), ".JPG .jpg .JPEG .jpeg"),
                      (_("PNG files"), ".PNG .png"),
                      (_("TIFF files"), ".TIF .tif .TIFF .tiff"),
-                     (_("SVG files"), ".SVG .svg"),
                      (_("ALL types"), "*"))
-
-    filename = filedialog.askopenfilename(initialdir=dir_name,
+    # Wand doesn't like SVG: (_("SVG files"), ".SVG .svg"),
+    filename = None
+    filename = filedialog.askopenfilename(initialdir=dir_initial,
                                         filetypes=filetypes,
-                                        title=_("Select picture for processing"))
-    open_file_common(dir_name, filename)
+                                        title=title)
+    return filename
 
 
 def open_file_last_key(event):
     """ call open_file_last from bind"""
     open_file_last()
 
 
@@ -715,51 +705,60 @@
         except:
             log.write_log('open_screenshot(), error in make screeshot ', 'E')
             do_it = 1
     if do_it:
         open_file_common(today_dir, filename)
 
 
+def askcolor(initial):
+    """ Use color widget ColorChooserDialog from ttkbootstrap"""
+    cd = ColorChooserDialog()
+    cd.show()
+    colors = cd.result
+    result = colors.hex
+    return result
+
+
 def color_choose_rotate():
     """ color selection for rotate"""
     color = askcolor(img_rotate_color.get())
-    if color[1] is not None:
-        img_rotate_color.set(color[1])
-        l_rotate_color.configure(bg=color[1])
+    if color is not None:
+        img_rotate_color.set(color)
+        l_rotate_color.configure(bg=color)
 
 
 def color_choose_border():
     """ Border color selection """
     color = askcolor(img_border_color.get())
-    if color[1] is not None:
-        img_border_color.set(color[1])
-        l_border_color.configure(bg=color[1])
+    if color is not None:
+        img_border_color.set(color)
+        l_border_color.configure(bg=color)
 
 
 def color_choose_vignette():
     """ color selection for rotate"""
     color = askcolor(img_vignette_color.get())
-    if color[1] is not None:
-        img_vignette_color.set(color[1])
-        l_vignette_color.configure(bg=color[1])
+    if color is not None:
+        img_vignette_color.set(color)
+        l_vignette_color.configure(bg=color)
 
 
 def color_choose_box():
     """ Background color selection """
     color = askcolor(img_text_color.get())
-    if color[1] is not None:
-        img_text_box_color.set(color[1])
+    if color is not None:
+        img_text_box_color.set(color)
         l_text_color.configure(bg=img_text_box_color.get())
 
 
 def color_choose():
     """ Color selection """
     color = askcolor(img_text_color.get())
-    if color[1] is not None:
-        img_text_color.set(color[1])
+    if color is not None:
+        img_text_color.set(color)
         l_text_color.configure(fg=img_text_color.get())
 
 
 def ini_read_wraper():
     """ Read config INI file """
     # main
     ini_entries = ini_read.main(FILE_INI, preview_size_list)
@@ -1367,16 +1366,17 @@
         frame_text_rotate.grid()
 
 
 ###############################################################################
 # GUI main window
 ###############################################################################
 
-root = Tk()
-
+#root = Tk()
+root = ttk.Window(resizable=(1,1), title=version.__author__ + " : " + version.__appname__ + " " + version.__version__)
+ttk.Sizegrip()
 # hidden file
 # https://code.activestate.com/lists/python-tkinter-discuss/3723/
 try:
     # call a dummy dialog with an impossible option to initialize the file
     # dialog without really getting a dialog window; this will throw a
     # TclError, so we need a try...except :
     try:
@@ -1385,21 +1385,14 @@
         pass
     # now set the magic variables accordingly
     root.tk.call('set', '::tk::dialog::file::showHiddenBtn', '1')
     root.tk.call('set', '::tk::dialog::file::showHiddenVar', '0')
 except:
     pass
 
-style = ttk.Style()
-style.configure("Blue.TButton", foreground="blue")
-style.configure("Brown.TButton", foreground="#8B0000")
-style.configure("Blue.TLabelframe.Label", foreground="blue")
-style.configure("Fiolet.TLabelframe.Label", foreground="#800080")
-style.configure("Rotate.TEntry", fieldbackground="#FFFFFF")
-
 ##########################
 # global variables
 FILE_INI = os.path.join(os.path.expanduser("~"), ".fotokilof.ini")
 PWD = os.getcwd()
 log_level = StringVar() # E(rror), W(arning), M(essage)
 work_dir = StringVar()  # default: "FotoKilof"
 work_sub_dir = StringVar()  # subdir for resized pictures
@@ -1458,208 +1451,215 @@
 file_extension = (".jpeg", ".jpg", ".png", ".tif")
 
 ######################################################################
 # Tabs
 ######################################################################
 main_menu = ttk.Frame()
 main_tools = ttk.Frame()
-main_paned = ttk.PanedWindow(orient=HORIZONTAL, width=5)
+main_paned = ttk.PanedWindow(orient=HORIZONTAL, bootstyle="default")
 main_progress = ttk.Frame()
 
 main_menu.pack(side=TOP, expand=0, fill=BOTH)
 main_tools.pack(side=TOP, expand=0, fill=BOTH)
 main_progress.pack(side=BOTTOM, expand=0, fill=X, anchor=S)
 main_paned.pack(side=BOTTOM, expand=1, fill=BOTH)
 
 
 validation = main_paned.register(gui.only_numbers)  # Entry validation
 validationint = main_paned.register(gui.only_integer)  # Entry validation integer value
 ####################################################################
-progressbar = ttk.Progressbar(main_progress, orient=HORIZONTAL, mode='determinate',
+progressbar = ttk.Progressbar(main_progress, orient=HORIZONTAL, bootstyle="info", mode='determinate',
                                 variable=progressbar_var, maximum=100)
 progressbar.pack(side=BOTTOM, padx=0, pady=0, fill=X, expand=0, anchor=S)
 ####################################################################
 # main_menu row
 ####################################################################
 ###########################
 # Picture selection
 ###########################
-frame_file_select = ttk.Labelframe(main_menu, text=_("Image"),
-                                   style="Fiolet.TLabelframe")
+frame_file_select = ttk.Labelframe(main_menu, text=_("Image"))
+
 frame_file_select.grid(row=1, column=1, sticky=(N, W, E, S), padx=5, pady=5)
 
 b_file_select = ttk.Button(frame_file_select, text=_("File selection"),
-                           command=open_file, style="Blue.TButton")
+                           command=open_file, bootstyle="info")
 
 b_file_select_screenshot = ttk.Button(frame_file_select, text=_("Screenshot"),
-                                 command=open_screenshot)
+                                      command=open_screenshot, bootstyle="info")
 if mswindows.windows() or mswindows.macos():
     b_file_select_screenshot.configure(text=_("Clipboard"))
 
-b_file_select_first = ttk.Button(frame_file_select, text=_("First"),
+b_file_select_first = ttk.Button(frame_file_select, text=_("First"), bootstyle="info-outline",
                                  command=open_file_first)
-b_file_select_prev = ttk.Button(frame_file_select, text=_("Previous"),
+b_file_select_prev = ttk.Button(frame_file_select, text=_("Previous"), bootstyle="info-outline",
                                 command=open_file_prev)
-b_file_select_next = ttk.Button(frame_file_select, text=_("Next"),
+b_file_select_next = ttk.Button(frame_file_select, text=_("Next"), bootstyle="info-outline",
                                 command=open_file_next)
-b_file_select_last = ttk.Button(frame_file_select, text=_("Last"),
+b_file_select_last = ttk.Button(frame_file_select, text=_("Last"), bootstyle="info-outline",
                                 command=open_file_last)
 
 b_file_select.grid(column=1, row=1, padx=5, pady=5, sticky=W)
 #
 b_file_select_screenshot.grid(column=2, row=1, padx=10, pady=5, sticky=W)
 #
 b_file_select_first.grid(column=5, row=1, padx=5, pady=5, sticky=W)
 b_file_select_prev.grid(column=6, row=1, padx=5, pady=5, sticky=W)
 b_file_select_next.grid(column=7, row=1, padx=5, pady=5, sticky=W)
 b_file_select_last.grid(column=8, row=1, padx=5, pady=5, sticky=W)
 
 ##########################
 # Execute all
 ##########################
-frame_apply = ttk.LabelFrame(main_menu, text=_("Execute all"),
-                             style="Fiolet.TLabelframe")
+frame_apply = ttk.LabelFrame(main_menu, text=_("Execute all"))
 frame_apply.grid(row=1, column=2, sticky=(N, W, E, S), padx=5, pady=5)
 
-rb_apply_dir = ttk.Radiobutton(frame_apply, text=_("Folder"),
+rb_apply_dir = ttk.Radiobutton(frame_apply, text=_("Folder"), bootstyle="info",
                                variable=file_dir_selector, value="1")
-rb_apply_file = ttk.Radiobutton(frame_apply, text=_("File"),
+rb_apply_file = ttk.Radiobutton(frame_apply, text=_("File"), bootstyle="info",
                                 variable=file_dir_selector, value="0")
 co_apply_type = ttk.Combobox(frame_apply, width=4, values=file_extension)
 co_apply_type.configure(state='readonly')
 co_apply_type.current(file_extension.index(".jpg"))
-b_apply_run = ttk.Button(frame_apply, text=_("Execute all"),
-                         command=apply_all_button,
-                         style="Blue.TButton")
+b_apply_run = ttk.Button(frame_apply, text=_("Execute all"), bootstyle="info",
+                         command=apply_all_button)
 
 b_apply_run.pack(side=LEFT, padx=5, pady=5, anchor=W)
 rb_apply_dir.pack(side=LEFT, pady=5, anchor=W)
 rb_apply_file.pack(side=LEFT, padx=5, pady=5, anchor=W)
 
 co_apply_type.pack(side=LEFT, padx=5, pady=1, anchor=W)
 
 l_pb = ttk.Label(frame_apply, textvariable=progress_files, width=15)
 l_pb.pack(side=LEFT, padx=5, pady=2, anchor=W)
 
 ###########################
 # Buttons
 ###########################
-frame_save = ttk.LabelFrame(main_menu, text=_("Settings"),
-                       style="Fiolet.TLabelframe")
+frame_save = ttk.LabelFrame(main_menu, text=_("Settings"))
 frame_save.grid(row=1, column=3, sticky=(N, W, E, S), padx=5, pady=5)
 
-b_last_save = ttk.Button(frame_save, text=_("Save"), command=ini_save_wraper)
-b_last_read = ttk.Button(frame_save, text=_("Load"), command=ini_read_wraper)
+b_last_save = ttk.Button(frame_save, text=_("Save"), command=ini_save_wraper, bootstyle="info-outline")
+b_last_read = ttk.Button(frame_save, text=_("Load"), command=ini_read_wraper, bootstyle="info-outline")
 
 b_last_save.pack(padx=5, pady=1, anchor=W, side=LEFT)
 b_last_read.pack(padx=5, pady=1, anchor=W, side=LEFT)
 
 ####################################################################
 # main_tools row
 ####################################################################
 frame_tools_selection = ttk.Frame(main_paned)
-#frame_tools_selection = ttk.Frame()
 
 ############################
 # Tools selection
 ############################
-frame_tools_set = ttk.Labelframe(main_tools, text=_("Tools"),
-                                style="Fiolet.TLabelframe")
+frame_tools_set = ttk.Labelframe(main_tools, text=_("Tools"))
 frame_tools_set.grid(row=1, column=1, padx=5, pady=2, sticky=(W, E))
 
 cb_resize = ttk.Checkbutton(frame_tools_set, text=_("Scaling/Resize"),
+                            bootstyle="info",
                             variable=img_resize_on,
                             offvalue="0", onvalue="1",
                             command=tools_set_off)
 cb_crop = ttk.Checkbutton(frame_tools_set, text=_("Crop"),
+                          bootstyle="info",
                           variable=img_crop_on,
                           offvalue="0", onvalue="1",
                           command=tools_set_on)
 cb_text = ttk.Checkbutton(frame_tools_set, text=_("Text"),
+                          bootstyle="info",
                           variable=img_text_on,
                           onvalue="1", offvalue="0",
                           command=tools_set_off)
 cb_rotate = ttk.Checkbutton(frame_tools_set, text=_("Rotate"),
+                            bootstyle="info",
                             variable=img_rotate_on,
                             offvalue="0", onvalue="1",
                             command=tools_set_off)
 cb_border = ttk.Checkbutton(frame_tools_set, text=_("Border"),
+                            bootstyle="info",
                             variable=img_border_on,
                             offvalue="0", onvalue="1",
                             command=tools_set_off)
 cb_bw = ttk.Checkbutton(frame_tools_set, text=_("Black&white"),
+                        bootstyle="info",
                         variable=img_bw_on, offvalue="0",
                         command=tools_set_off)
 cb_normalize = ttk.Checkbutton(frame_tools_set, text=_("Colors normalize"),
+                               bootstyle="info",
                                variable=img_normalize_on,
                                offvalue="0", onvalue="1",
                                command=tools_set_off)
 cb_contrast = ttk.Checkbutton(frame_tools_set, text=_("Contrast"),
+                              bootstyle="info",
                               variable=img_contrast_on,
                               offvalue="0", onvalue="1",
                               command=tools_set_off)
 cb_mirror = ttk.Checkbutton(frame_tools_set, text=_("Mirror"),
+                              bootstyle="info",
                               variable=img_mirror_on,
                               offvalue="0", onvalue="1",
                               command=tools_set_off)
 cb_logo = ttk.Checkbutton(frame_tools_set, text=_("Logo"),
+                          bootstyle="info",
                           variable=img_logo_on,
                           offvalue="0", onvalue="1",
                           command=tools_set_off)
 cb_custom = ttk.Checkbutton(frame_tools_set, text=_("Custom"),
+                            bootstyle="info",
                             variable=img_custom_on,
                             offvalue="0", onvalue="1",
                             command=tools_set_off)
 cb_vignette = ttk.Checkbutton(frame_tools_set, text=_("Vignette"),
+                            bootstyle="info",
                             variable=img_vignette_on,
                             offvalue="0", onvalue="1",
                             command=tools_set_off)
 cb_exif = ttk.Checkbutton(frame_tools_set, text=_("EXIF"),
+                                bootstyle="info",
                                 variable=img_exif_on,
                                 offvalue="0", onvalue="1",
                                 command=tools_set_off)
 cb_histograms = ttk.Checkbutton(frame_tools_set, text=_("Histograms"),
+                                bootstyle="info",
                                 variable=img_histograms_on,
                                 offvalue="0", onvalue="1",
                                 command=tools_set_off)
 
-cb_crop.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_mirror.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_bw.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_contrast.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_normalize.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_vignette.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_border.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_rotate.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_resize.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_text.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_logo.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_custom.pack(padx=5, pady=1, anchor=W, side=LEFT)
-cb_exif.pack(padx=5, pady=1, anchor=W, side=LEFT)
+cb_crop.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_mirror.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_bw.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_contrast.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_normalize.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_vignette.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_border.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_rotate.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_resize.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_text.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_logo.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_custom.pack(padx=5, pady=5, anchor=W, side=LEFT)
+cb_exif.pack(padx=5, pady=5, anchor=W, side=LEFT)
 #cb_histograms.pack(padx=5, pady=1, anchor=W, side=LEFT)
 
 ####################################################################
 # main row
 ####################################################################
 #####################################################
 # First column
 #####################################################
-#frame_first_col = ttk.Frame(main_paned)
-frame_first_col = ttk.Frame()
+frame_first_col = ScrolledFrame(autohide=True)
 
 ###########################
 # Label if no any tool selected
 l_info_when_no_tool = ttk.Label(frame_first_col,
                         text=_("Open file for processing\nSelect tools for conversion\nExecute conversion or perform all conversion in one run"))
 
 ###########################
 # Resize
 ###########################
-frame_resize = ttk.Labelframe(frame_first_col, text=_("Scale/Resize"),
-                              style="Fiolet.TLabelframe")
+frame_resize = ttk.Labelframe(frame_first_col, text=_("Scale/Resize"))
 ###
 frame_resize_row1 = ttk.Frame(frame_resize)
 rb_resize_3 = ttk.Radiobutton(frame_resize_row1, text="FullHD (1920x1080)",
                               variable=img_resize, value="3")
 rb_resize_4 = ttk.Radiobutton(frame_resize_row1, text="2K (2048×1556)",
                               variable=img_resize, value="4")
 rb_resize_5 = ttk.Radiobutton(frame_resize_row1, text="4K (4096×3112)",
@@ -1674,37 +1674,35 @@
 e1_resize_y = ttk.Entry(frame_resize_row2, width=4,
                       validate="key", validatecommand=(validation, '%S'))
 rb_resize_2 = ttk.Radiobutton(frame_resize_row2, text=_("Percent"),
                               variable=img_resize, value="2")
 e2_resize = ttk.Entry(frame_resize_row2, width=3,
                       validate="key", validatecommand=(validation, '%S'))
 b_resize_run = ttk.Button(frame_resize_row2, text=_("Execute"),
-                          style="Brown.TButton",
                           command=convert_resize_button)
 
 rb_resize_3.pack(side=LEFT, padx=5)
 rb_resize_4.pack(side=LEFT, padx=5)
 rb_resize_5.pack(side=LEFT, padx=5)
 rb_resize_1.pack(side=LEFT, padx=5)
 l_resize_x.pack(side=LEFT, padx=5)
 e1_resize_x.pack(side=LEFT, padx=0)
 l_resize_y.pack(side=LEFT, padx=5)
 e1_resize_y.pack(side=LEFT, padx=0)
 rb_resize_2.pack(side=LEFT, padx=5)
 e2_resize.pack(side=LEFT, padx=0)
-b_resize_run.pack(side=LEFT, padx=25)
+b_resize_run.pack(side=LEFT, padx=25, pady=5)
 
 frame_resize_row1.pack(side=TOP, fill=X, expand=1)
 frame_resize_row2.pack(side=TOP, fill=X, expand=1)
 
 ############################
 # crop
 ############################
-frame_crop = ttk.Labelframe(frame_first_col, text=_("Crop"),
-                            style="Fiolet.TLabelframe")
+frame_crop = ttk.Labelframe(frame_first_col, text=_("Crop"))
 frame_crop.grid(row=3, column=1, columnspan=2,
                 sticky=(N, W, E, S), padx=5, pady=1)
 ###
 rb1_crop = ttk.Radiobutton(frame_crop, variable=img_crop, value="1",
                            text=_("Coordinates (x1, y1) and (x2, y2)"),
                            command=crop_tool_hide_show)
 f_clickL_crop = ttk.Frame(frame_crop)
@@ -1771,19 +1769,18 @@
                              command=preview_orig)
 rb_crop_SE = ttk.Radiobutton(frame_crop_gravity, text="SE",
                              variable=img_crop_gravity, value="SE",
                              command=preview_orig)
 frame_crop_buttons = ttk.Frame(frame_crop)
 
 b_crop_show = ttk.Button(frame_crop_buttons, text=_("Preview"),
-                         command=preview_orig)
+                         command=preview_orig, bootstyle="outline")
 b_crop_read = ttk.Button(frame_crop_buttons, text=_("From image"),
-                         command=crop_read)
+                         command=crop_read, bootstyle="outline")
 b_crop_run = ttk.Button(frame_crop, text=_("Execute"),
-                        style="Brown.TButton",
                         command=convert_crop_button)
 
 rb1_crop.grid(row=2, column=1, sticky=W, padx=5, pady=5)
 f_clickL_crop.grid(row=1, column=2, rowspan=4, columnspan=2, padx=5, sticky=N)
 f_clickR_crop.grid(row=1, column=4, rowspan=4, columnspan=2, padx=5, sticky=N)
 e1_crop_1.grid(row=1, column=1, sticky=W, padx=5, pady=5)
 e2_crop_1.grid(row=1, column=2, sticky=W, padx=5, pady=5)
@@ -1815,18 +1812,17 @@
 b_crop_read.grid(row=1, column=1, sticky=W, padx=15, pady=5)
 b_crop_show.grid(row=1, column=2, sticky=W, padx=5, pady=5)
 b_crop_run.grid(row=5, column=4, columnspan=2, sticky=W, padx=5, pady=5)
 
 ###########################
 # Tekst
 ###########################
-frame_text = ttk.Labelframe(frame_first_col, text=_("Add text"),
-                            style="Fiolet.TLabelframe")
+frame_text = ttk.Labelframe(frame_first_col, text=_("Add text"))
 ###
-e_text = ttk.Entry(frame_text, width=55, style='Color.TEntry')
+e_text = ttk.Entry(frame_text, width=55)
 #frame_text_text.grid(row=1, column=1, columnspan=5, sticky=(W, E))
 e_text.grid(row=1, column=1, columnspan=5, sticky=W, padx=5)
 
 ###
 rb_text_in = ttk.Radiobutton(frame_text, text=_("Inside"),
                              variable=img_text_inout, value="0",
                              command=text_tool_hide_show)
@@ -1893,20 +1889,19 @@
 co_text_font = ttk.Combobox(frame_text, width=30,
                             textvariable=img_text_font)
 co_text_font.configure(state='readonly')
 e_text_size = ttk.Entry(frame_text, width=3,
                         validate="key", validatecommand=(validation, '%S'))
 l_text_color = Label(frame_text, text=_("Color test"))
 b_text_color = ttk.Button(frame_text, text=_("Font"),
-                          command=color_choose)
+                          command=color_choose, bootstyle="outline")
 l_text_heght = ttk.Label(frame_text, text=_("Height"))
 b_text_box_color = ttk.Button(frame_text, text=_("Background"),
-                              command=color_choose_box)
-b_text_run = ttk.Button(frame_text, text=_("Execute"),
-                        style="Brown.TButton", command=convert_text_button)
+                              command=color_choose_box, bootstyle="outline")
+b_text_run = ttk.Button(frame_text, text=_("Execute"), command=convert_text_button)
 
 l_text_color.grid(row=2, column=5, sticky=(W, E), padx=5, pady=1)
 b_text_color.grid(row=3, column=5, sticky=(W, E), padx=5, pady=1)
 b_text_box_color.grid(row=4, column=5, sticky=(W, E), padx=5, pady=1)
 co_text_font.grid(row=5, column=1, columnspan=2, sticky=(W, E), padx=5)
 l_text_heght.grid(row=5, column=3, sticky=W, padx=5)
 e_text_size.grid(row=5, column=4, sticky=W, padx=5)
@@ -1932,33 +1927,30 @@
 rb_text_rotate_own.grid(row=1, column=5, sticky=(N, W, E, S), padx=5, pady=5)
 e_text_angle.grid(row=1, column=6, sticky=(N, W, E, S), padx=5, pady=5)
 frame_text_rotate.grid(row=6, column=1, columnspan=6, sticky=W, padx=5)
 
 ###########################
 # Rotate
 ###########################
-frame_rotate = ttk.LabelFrame(frame_first_col, text=_("Rotate"),
-                              style="Fiolet.TLabelframe")
+frame_rotate = ttk.LabelFrame(frame_first_col, text=_("Rotate"))
 ###
 rb_rotate_90 = ttk.Radiobutton(frame_rotate, text="90",
                                variable=img_rotate, value="90")
 rb_rotate_180 = ttk.Radiobutton(frame_rotate, text="180",
                                 variable=img_rotate, value="180")
 rb_rotate_270 = ttk.Radiobutton(frame_rotate, text="270",
                                 variable=img_rotate, value="270")
 rb_rotate_own = ttk.Radiobutton(frame_rotate, text=_("Custom"),
                                 variable=img_rotate, value="0")
-e_rotate_own = ttk.Entry(frame_rotate, width=3, style='Rotate.TEntry',
+e_rotate_own = ttk.Entry(frame_rotate, width=3,
                      validate="key", validatecommand=(validation, '%S'))
 l_rotate_color = Label(frame_rotate, text=_("  "))
 b_rotate_color = ttk.Button(frame_rotate, text=_("Color"),
-                          command=color_choose_rotate)
-b_rotate_run = ttk.Button(frame_rotate, text=_("Execute"),
-                          style="Brown.TButton",
-                          command=convert_rotate_button)
+                          command=color_choose_rotate, bootstyle="outline")
+b_rotate_run = ttk.Button(frame_rotate, text=_("Execute"), command=convert_rotate_button)
 
 rb_rotate_90.pack(side=LEFT, padx=5, pady=5)
 rb_rotate_180.pack(side=LEFT, padx=5, pady=5)
 rb_rotate_270.pack(side=LEFT, padx=5, pady=5)
 rb_rotate_own.pack(side=LEFT, padx=5, pady=5)
 e_rotate_own.pack(side=LEFT, padx=5, pady=5)
 l_rotate_color.pack(side=LEFT, pady=5)
@@ -1971,143 +1963,129 @@
 frame_mirror_vignette = ttk.Frame(frame_first_col)
 frame_bw_contrast = ttk.Frame(frame_first_col)
 frame_border_normalize = ttk.Frame(frame_first_col)
 
 ###########################
 # Border
 ###########################
-frame_border = ttk.Labelframe(frame_border_normalize, text=_("Border"),
-                              style="Fiolet.TLabelframe")
+frame_border = ttk.Labelframe(frame_border_normalize, text=_("Border"))
 ###
 l_border_color = Label(frame_border, text=_("  "))
 l_border_we = ttk.Label(frame_border, text="WE")
 e_border_we = ttk.Entry(frame_border, width=3,
                      validate="key", validatecommand=(validation, '%S'))
 l_border_ns = ttk.Label(frame_border, text="NS")
 e_border_ns = ttk.Entry(frame_border, width=3,
                      validate="key", validatecommand=(validation, '%S'))
 b_border_color = ttk.Button(frame_border, text=_("Color"),
-                            command=color_choose_border)
-b_border_run = ttk.Button(frame_border, text=_("Execute"),
-                          style="Brown.TButton",
-                          command=convert_border_button)
+                            command=color_choose_border, bootstyle="outline")
+b_border_run = ttk.Button(frame_border, text=_("Execute"), command=convert_border_button)
 
 l_border_we.grid(row=1, column=1, padx=5, pady=0)
 e_border_we.grid(row=1, column=2, padx=5, pady=0)
 l_border_ns.grid(row=2, column=1, padx=5, pady=5)
 e_border_ns.grid(row=2, column=2, padx=5, pady=5)
 l_border_color.grid(row=1, column=3)
 b_border_color.grid(row=1, column=5, padx=5, pady=0)
 b_border_run.grid(row=2, column=5, padx=5, pady=5, sticky=E)
 
 ############################
 # Black-white
 ############################
-frame_bw = ttk.LabelFrame(frame_bw_contrast, text=_("Black-white"),
-                          style="Fiolet.TLabelframe")
+frame_bw = ttk.LabelFrame(frame_bw_contrast, text=_("Black-white"))
 ###
 rb1_bw = ttk.Radiobutton(frame_bw, text=_("Black-white"),
                          variable=img_bw, value="1")
 rb2_bw = ttk.Radiobutton(frame_bw, text=_("Sepia"),
                          variable=img_bw, value="2")
 e_bw_sepia = ttk.Entry(frame_bw, width=3,
                        validate="key", validatecommand=(validation, '%S'))
 l_bw_sepia = ttk.Label(frame_bw, text="%")
-b_bw_run = ttk.Button(frame_bw, text=_("Execute"),
-                      style="Brown.TButton",
-                      command=convert_bw_button)
+b_bw_run = ttk.Button(frame_bw, text=_("Execute"), command=convert_bw_button)
 
 rb2_bw.grid(row=1, column=1, padx=5, pady=5, sticky=W)
 e_bw_sepia.grid(row=1, column=2, padx=5, pady=5, sticky=E)
 l_bw_sepia.grid(row=1, column=3, padx=5, pady=5, sticky=W)
 rb1_bw.grid(row=2, column=1, padx=5, pady=0, sticky=W)
 b_bw_run.grid(row=2, column=2, columnspan=2, padx=5, pady=5, sticky=E)
 
 ########################
 # Contrast
 #########################
-frame_contrast = ttk.Labelframe(frame_bw_contrast, text=_("Contrast"),
-                                style="Fiolet.TLabelframe")
+frame_contrast = ttk.Labelframe(frame_bw_contrast, text=_("Contrast"))
 ###
 rb1_contrast = ttk.Radiobutton(frame_contrast, text=_("Stretch"),
                                variable=img_contrast, value="1")
 rb2_contrast = ttk.Radiobutton(frame_contrast, text=_("Contrast"),
                                variable=img_contrast, value="2")
 co_contrast_selection = ttk.Combobox(frame_contrast, width=3,
                                      values=contrast_selection)
 co_contrast_selection.configure(state='readonly')
 
 e1_contrast = ttk.Entry(frame_contrast, width=4)
 e2_contrast = ttk.Entry(frame_contrast, width=4)
 l1_contrast = ttk.Label(frame_contrast, text=_("Black"))
 l2_contrast = ttk.Label(frame_contrast, text=_("White"))
-b_contrast_run = ttk.Button(frame_contrast, text=_("Execute"),
-                            style="Brown.TButton",
-                            command=convert_contrast_button)
+b_contrast_run = ttk.Button(frame_contrast, text=_("Execute"), command=convert_contrast_button)
 
 rb1_contrast.grid(row=1, column=1, padx=5, pady=5, sticky=W)
 l1_contrast.grid(row=1, column=2, padx=5, pady=5, sticky=E)
 e1_contrast.grid(row=1, column=3, padx=5, pady=5, sticky=E)
 l2_contrast.grid(row=1, column=4, padx=5, pady=5, sticky=W)
 e2_contrast.grid(row=1, column=5, padx=5, pady=5, sticky=W)
 rb2_contrast.grid(row=2, column=1, padx=5, pady=5, sticky=W)
 co_contrast_selection.grid(row=2, column=2, padx=5, pady=5, sticky=W)
 b_contrast_run.grid(row=2, column=3, padx=5, pady=5, columnspan=3, sticky=E)
 
 ############################
 # Color normalize
 ############################
-frame_normalize = ttk.LabelFrame(frame_border_normalize, text=_("Color normalize"),
-                                 style="Fiolet.TLabelframe")
+frame_normalize = ttk.LabelFrame(frame_border_normalize, text=_("Color normalize"))
 ###
 rb1_normalize = ttk.Radiobutton(frame_normalize, text=_("Normalize"),
                                 variable=img_normalize,
                                 value="1")
 rb2_normalize = ttk.Radiobutton(frame_normalize, text=_("AutoLevel"),
                                 variable=img_normalize,
                                 value="2")
 l_normalize_channel = ttk.Label(frame_normalize, text=_("Channel:"))
 co_normalize_channel = ttk.Combobox(frame_normalize, width=7,
                                     values=normalize_channels)
 co_normalize_channel.configure(state='readonly')
 b_normalize_run = ttk.Button(frame_normalize, text=_("Execute"),
-                             style="Brown.TButton",
                              command=convert_normalize_button)
 
 rb1_normalize.grid(row=1, column=1, padx=5, pady=0, sticky=W)
 l_normalize_channel.grid(row=1, column=2, padx=5, pady=4, sticky=E)
 co_normalize_channel.grid(row=1, column=3, padx=5, pady=4, sticky=E)
 rb2_normalize.grid(row=2, column=1, padx=5, pady=4, sticky=W)
 b_normalize_run.grid(row=2, column=2, columnspan=2, padx=5, pady=4, sticky=E)
 
 ###########################
 # Mirror
 ###########################
-frame_mirror = ttk.LabelFrame(frame_mirror_vignette, text=_("Mirror"),
-                              style="Fiolet.TLabelframe")
+frame_mirror = ttk.LabelFrame(frame_mirror_vignette, text=_("Mirror"))
 
 cb_mirror_flip = ttk.Checkbutton(frame_mirror, text="NS",
                                  variable=img_mirror_flip,
                                  offvalue="0", onvalue="1")
 cb_mirror_flop = ttk.Checkbutton(frame_mirror, text="WE",
                                  variable=img_mirror_flop,
                                  offvalue="0", onvalue="1")
 b_mirror_run = ttk.Button(frame_mirror, text=_("Execute"),
-                          style="Brown.TButton",
                           command=convert_mirror_button)
 
 cb_mirror_flip.grid(row=1, column=1, sticky=(N, W, E, S), padx=5, pady=5)
 cb_mirror_flop.grid(row=1, column=2, sticky=(N, W, E, S), padx=5, pady=5)
 b_mirror_run.grid(row=1, column=5, sticky=E, padx=5, pady=5)
 
 ###########################
 # vignette
 ###########################
-frame_vignette = ttk.Labelframe(frame_mirror_vignette, text=_("Vignette"),
-                              style="Fiolet.TLabelframe")
+frame_vignette = ttk.Labelframe(frame_mirror_vignette, text=_("Vignette"))
 ###
 l_vignette_radius = ttk.Label(frame_vignette, text=_("Radius"))
 e_vignette_radius = ttk.Entry(frame_vignette, width=3,
                      validate="key", validatecommand=(validation, '%S'))
 l_vignette_sigma = ttk.Label(frame_vignette, text=_("Sigma"))
 e_vignette_sigma = ttk.Entry(frame_vignette, width=3,
                      validate="key", validatecommand=(validation, '%S'))
@@ -2115,17 +2093,16 @@
 e_vignette_dx = ttk.Entry(frame_vignette, width=3,
                      validate="key", validatecommand=(validationint, '%S'))
 l_vignette_dy = ttk.Label(frame_vignette, text=_("dy"))
 e_vignette_dy = ttk.Entry(frame_vignette, width=3,
                      validate="key", validatecommand=(validationint, '%S'))
 l_vignette_color = Label(frame_vignette, text=_("  "))
 b_vignette_color = ttk.Button(frame_vignette, text=_("Color"),
-                            command=color_choose_vignette)
+                            command=color_choose_vignette, bootstyle="outline")
 b_vignette_run = ttk.Button(frame_vignette, text=_("Execute"),
-                          style="Brown.TButton",
                           command=convert_vignette_button)
 l_vignette_radius.grid(row=1, column=1, padx=5, pady=0)
 e_vignette_radius.grid(row=1, column=2, padx=5, pady=0)
 l_vignette_sigma.grid(row=2, column=1, padx=5, pady=5)
 e_vignette_sigma.grid(row=2, column=2, padx=5, pady=5)
 l_vignette_dx.grid(row=1, column=3, padx=5, pady=0)
 e_vignette_dx.grid(row=1, column=4, padx=5, pady=0)
@@ -2134,28 +2111,26 @@
 l_vignette_color.grid(row=1, column=5)
 b_vignette_color.grid(row=1, column=6, padx=5, pady=0)
 b_vignette_run.grid(row=2, column=6, padx=5, pady=5)
 
 ###########################
 # Logo
 ###########################
-frame_logo = ttk.LabelFrame(frame_first_col, text=_("Logo"),
-                            style="Fiolet.TLabelframe")
+frame_logo = ttk.LabelFrame(frame_first_col, text=_("Logo"))
 
 b_logo_select = ttk.Button(frame_logo, text=_("File selection"),
-                           command=open_file_logo)
+                           command=open_file_logo, bootstyle="outline")
 
 b_logo_run = ttk.Button(frame_logo, text=_("Execute"),
-                        command=convert_logo_button,
-                        style="Brown.TButton")
+                        command=convert_logo_button)
 l_logo_filename = ttk.Label(frame_logo, width=25)
 
 b_logo_select.grid(row=1, column=1, padx=5, pady=5)
 l_logo_filename.grid(row=1, column=2, padx=5, pady=5, sticky=W)
-b_logo_run.grid(row=1, column=3, pady=5, sticky=E)
+b_logo_run.grid(row=1, column=3, padx=5, pady=5, sticky=E)
 
 ###
 frame_logo_xy = ttk.Frame(frame_logo)
 l_logo_XxY = ttk.Label(frame_logo_xy, text=_("Width\nHeight"))
 l_logo_dxdy = ttk.Label(frame_logo_xy, text=_("Offset\n(dx,dy)"))
 e_logo_width = ttk.Entry(frame_logo_xy, width=4,
                          validate="key", validatecommand=(validation, '%S'))
@@ -2190,15 +2165,15 @@
                             variable=img_logo_gravity, value="E")
 rb_logo_SW = ttk.Radiobutton(frame_logo_gravity, text="SW",
                              variable=img_logo_gravity, value="SW")
 rb_logo_S = ttk.Radiobutton(frame_logo_gravity, text="S",
                             variable=img_logo_gravity, value="S")
 rb_logo_SE = ttk.Radiobutton(frame_logo_gravity, text="SE",
                              variable=img_logo_gravity, value="SE")
-frame_logo_gravity.grid(row=2, column=3, sticky=E)
+frame_logo_gravity.grid(row=2, column=3, padx=5, sticky=E)
 rb_logo_NW.grid(row=1, column=1, sticky=W, pady=1)
 rb_logo_N.grid(row=1, column=2, pady=1)
 rb_logo_NE.grid(row=1, column=3, sticky=W, pady=1)
 rb_logo_W.grid(row=2, column=1, sticky=W, pady=1)
 rb_logo_C.grid(row=2, column=2, pady=1)
 rb_logo_E.grid(row=2, column=3, sticky=W, pady=1)
 rb_logo_SW.grid(row=3, column=1, sticky=W, pady=1)
@@ -2213,62 +2188,62 @@
 l_logo_preview = ttk.Label(frame_logo_preview)
 l_logo_preview_pi.grid(row=2, column=1, padx=5, pady=1)
 l_logo_preview.grid(row=1, column=1, padx=5, pady=1)
 
 ############################
 # Custom command
 ############################
-frame_custom = ttk.LabelFrame(frame_first_col, text=_("Custom command"),
-                              style="Fiolet.TLabelframe")
+frame_custom = ttk.LabelFrame(frame_first_col, text=_("Custom command"))
 
 b_custom_clear = ttk.Button(frame_custom, text=_("Clear"),
+                            bootstyle="warning",
                             command=convert_custom_clear)
 b_custom_run = ttk.Button(frame_custom, text=_("Execute"),
-                          style="Brown.TButton",
                           command=convert_custom_button)
 
 t_custom = ScrolledText(frame_custom, state=NORMAL,
                         height=5, width=45,
                         wrap='word', undo=True)
 
 t_custom.pack(expand=1, fill=BOTH, padx=5, pady=5)
 b_custom_run.pack(side=RIGHT, padx=5, pady=5)
 b_custom_clear.pack(side=RIGHT, padx=5, pady=5)
 
 ############################
 # Pack frames
 ############################
+frame_first_col.pack(fill=BOTH, expand=1)
+
 l_info_when_no_tool.grid(row=1, column=1, padx=5, pady=5)
 frame_crop.grid(row=2, column=1,             sticky=(N, W, S), padx=5, pady=1)
 frame_mirror_vignette.grid(row=3, column=1,  sticky=(N, W, S), padx=0, pady=1)
 frame_bw_contrast.grid(row=4, column=1,      sticky=(N, W, S), padx=0, pady=1)
 frame_border_normalize.grid(row=5, column=1, sticky=(N, W, S), padx=0, pady=1)
 frame_rotate.grid(row=7, column=1,           sticky=(N, W, S), padx=5, pady=1)
 frame_resize.grid(row=8, column=1,           sticky=(N, W, S), padx=5, pady=5)
 frame_text.grid(row=9, column=1,             sticky=(N, W, S), padx=5, pady=1)
 frame_logo.grid(row=10, column=1,            sticky=(N, W, S), padx=5, pady=1)
 frame_custom.grid(row=11, column=1,          sticky=(N, W, S), padx=5, pady=1)
 
 #####################################################
 # Second column
 #####################################################
-#frame_second_col = ttk.Frame(main_paned)
 frame_second_col = ttk.Frame()
 
 ############################
 # Original preview
 ############################
-frame_preview_orig = ttk.Labelframe(frame_second_col, text=_("Original"),
-                                    style="Fiolet.TLabelframe")
+frame_preview_orig = ttk.Labelframe(frame_second_col, text=_("Original"))
 frame_preview_orig.grid(row=1, column=1, sticky=(N, W, E, S), padx=5, pady=5)
 ###
 b_preview_orig_run = ttk.Button(frame_preview_orig, text=_("Preview"),
+                                bootstyle="secondary",
                                 command=preview_orig_button)
 l_preview_orig = ttk.Label(frame_preview_orig)
-co_preview_selector_orig = ttk.Combobox(frame_preview_orig, width=4,
+co_preview_selector_orig = ttk.Combobox(frame_preview_orig, width=4, bootstyle="secondary",
                                         values=preview_size_list)
 co_preview_selector_orig.configure(state='readonly')
 pi_preview_orig = PhotoImage()
 c_preview_orig_pi = Canvas(frame_preview_orig)
 c_preview_orig_pi.create_image(0, 0, image=pi_preview_orig, anchor='ne')
 
 c_preview_orig_pi.pack(side=BOTTOM, anchor=W)
@@ -2286,28 +2261,28 @@
 c_histogram_orig = Canvas(frame_histogram_orig)
 c_preview_orig_pi.create_image(0, 0, image=pi_histogram_orig, anchor='ne')
 c_histogram_orig.grid(row=2, column=1, padx=10, pady=5)
 
 #####################################################
 # Third column
 #####################################################
-#frame_third_col = ttk.Frame(main_paned)
 frame_third_col = ttk.Frame()
 
 ##########################
 # Result preview
 ###########################
-frame_preview_new = ttk.Labelframe(frame_third_col, text=_("Result"),
-                                   style="Fiolet.TLabelframe")
+frame_preview_new = ttk.Labelframe(frame_third_col, text=_("Result"))
+
 frame_preview_new.grid(row=1, column=1, sticky=(N, W, E, S), padx=5, pady=5)
 ###
 b_preview_new_run = ttk.Button(frame_preview_new, text=_("Preview"),
+                               bootstyle="secondary",
                                command=preview_new_button)
 l_preview_new = ttk.Label(frame_preview_new)
-co_preview_selector_new = ttk.Combobox(frame_preview_new, width=4,
+co_preview_selector_new = ttk.Combobox(frame_preview_new, width=4, bootstyle="secondary",
                                        values=preview_size_list)
 co_preview_selector_new.configure(state='readonly')
 pi_preview_new = PhotoImage()
 c_preview_new_pi = Canvas(frame_preview_new)
 c_preview_orig_pi.create_image(0, 0, image=pi_preview_orig, anchor='ne')
 
 c_preview_new_pi.pack(side=BOTTOM, anchor=W)
@@ -2325,15 +2300,15 @@
 c_histogram_new = Canvas(frame_histogram_new)
 c_histogram_new.create_image(0, 0, image=pi_histogram_new, anchor='ne')
 c_histogram_new.grid(row=2, column=1, padx=10, pady=5)
 
 ###############################################################################
 # Add Frames into PanedWindow
 ###############################################################################
-main_paned.add(frame_first_col)
+main_paned.add(frame_first_col.container)
 main_paned.add(frame_second_col)
 main_paned.add(frame_third_col)
 
 ###############################################################################
 # bind
 ###############################################################################
 # binding commands to widgets
@@ -2353,135 +2328,135 @@
 root.bind("<Home>", open_file_first_key)
 root.bind("<End>", open_file_last_key)
 
 ###############################################################################
 # toolTips
 ###############################################################################
 # main first
-Hovertip(b_file_select, _("Select image file for processing"))
-Hovertip(b_file_select_screenshot, _("MacOS and Windows: take image from clipboard.\nLinux: make screenshot, click window or select area.\nGrabbed image is saved into %TEMP%/today directory ad load for processing."))
-Hovertip(b_file_select_first, _("Load first image from current directory.\nUse Home key instead"))
-Hovertip(b_file_select_prev, _("Load previous image from current directory.\nUse PgUp key instead"))
-Hovertip(b_file_select_next, _("Load next image from current directory.\nUse PgDn key instead"))
-Hovertip(b_file_select_last, _("Load last image from current directory.\nUse End key instead"))
-Hovertip(rb_apply_dir, _("Processing all files in current directory"))
-Hovertip(rb_apply_file, _("Processing only current file"))
-Hovertip(co_apply_type, _("Selection of format output file; JPG, PNG or TIF"))
-Hovertip(b_apply_run, _("Perform all selected conversion for current file or all files in current directory"))
-Hovertip(b_last_save, _("Save all values into configuration file (~/.fotokilof.ini).\nFotoKilof will load it during starting"))
-Hovertip(b_last_read, _("Load saved values of conversion"))
+ToolTip(b_file_select, text=_("Select image file for processing"))
+ToolTip(b_file_select_screenshot, text=_("MacOS and Windows: take image from clipboard.\nLinux: make screenshot, click window or select area.\nGrabbed image is saved into %TEMP%/today directory ad load for processing."))
+ToolTip(b_file_select_first, text=_("Load first image from current directory.\nUse Home key instead"))
+ToolTip(b_file_select_prev, text=_("Load previous image from current directory.\nUse PgUp key instead"))
+ToolTip(b_file_select_next, text=_("Load next image from current directory.\nUse PgDn key instead"))
+ToolTip(b_file_select_last, text=_("Load last image from current directory.\nUse End key instead"))
+ToolTip(rb_apply_dir, text=_("Processing all files in current directory"))
+ToolTip(rb_apply_file, text=_("Processing only current file"))
+ToolTip(co_apply_type, text=_("Selection of format output file; JPG, PNG or TIF"))
+ToolTip(b_apply_run, text=_("Perform all selected conversion for current file or all files in current directory"))
+ToolTip(b_last_save, text=_("Save all values into configuration file (~/.fotokilof.ini).\nFotoKilof will load it during starting"))
+ToolTip(b_last_read, text=_("Load saved values of conversion"))
 # main second
-Hovertip(cb_resize, _("Scale image, proportions are saved.\nSpecify maximum dimensions of image or percent"))
-Hovertip(cb_crop, _("Take part of image. Select crop by:\n- absolute coordinate\n- absolute coorinate left-top corner plus width and height\n- gravity plus width and height plus offset.\nRemember point (0,0) is located in left-top corner of image."))
-Hovertip(cb_text, _("Insert text on picture or add text at bottom.\nText can be rotated, colored and with background.\nAll font from OS are available"))
-Hovertip(cb_rotate, _("Rotate picture by 90, 180, 270 degree or specify own angle of rotation"))
-Hovertip(cb_border, _("Add border around picture.\nSpecify width of horizontal and vertical border separately"))
-Hovertip(cb_bw, _("Convert into black-white or sepia"))
-Hovertip(cb_contrast, _("Change contrast or change range of contrast"))
-Hovertip(cb_normalize, _("Normalize of color level"))
-Hovertip(cb_mirror, _("Make mirror of picture in vertical or horizotal or both direction"))
-Hovertip(cb_vignette, _("Add vignette as on old photography or not the best lens"))
-Hovertip(cb_logo, _("Insert picture, eg. own logo, into picture"))
-Hovertip(cb_custom, _("Processing ImageMagick command.\nWorks only on Linux OS"))
-Hovertip(cb_exif, _("If ON keep EXIF data\nif OFF EXIF data will be removed"))
+ToolTip(cb_resize, text=_("Scale image, proportions are saved.\nSpecify maximum dimensions of image or percent"))
+ToolTip(cb_crop, text=_("Take part of image. Select crop by:\n- absolute coordinate\n- absolute coorinate left-top corner plus width and height\n- gravity plus width and height plus offset.\nRemember point (0,0) is located in left-top corner of image."))
+ToolTip(cb_text, text=_("Insert text on picture or add text at bottom.\nText can be rotated, colored and with background.\nAll font from OS are available"))
+ToolTip(cb_rotate, text=_("Rotate picture by 90, 180, 270 degree or specify own angle of rotation"))
+ToolTip(cb_border, text=_("Add border around picture.\nSpecify width of horizontal and vertical border separately"))
+ToolTip(cb_bw, text=_("Convert into black-white or sepia"))
+ToolTip(cb_contrast, text=_("Change contrast or change range of contrast"))
+ToolTip(cb_normalize, text=_("Normalize of color level"))
+ToolTip(cb_mirror, text=_("Make mirror of picture in vertical or horizotal or both direction"))
+ToolTip(cb_vignette, text=_("Add vignette as on old photography or not the best lens"))
+ToolTip(cb_logo, text=_("Insert picture, eg. own logo, into picture"))
+ToolTip(cb_custom, text=_("Processing ImageMagick command.\nWorks only on Linux OS"))
+ToolTip(cb_exif, text=_("If ON keep EXIF data\nif OFF EXIF data will be removed"))
 # preview
-Hovertip(b_preview_orig_run, _("Display original image by IMdisplay or default image viewer of OS"))
-Hovertip(co_preview_selector_orig, _("Select size of preview"))
-Hovertip(b_preview_new_run, _("Display result image by IMdisplay or default image viewer of OS"))
-Hovertip(co_preview_selector_new, _("Select size of preview"))
+ToolTip(b_preview_orig_run, text=_("Display original image by IMdisplay or default image viewer of OS"))
+ToolTip(co_preview_selector_orig, text=_("Select size of preview"))
+ToolTip(b_preview_new_run, text=_("Display result image by IMdisplay or default image viewer of OS"))
+ToolTip(co_preview_selector_new, text=_("Select size of preview"))
 # Scaling
-Hovertip(b_resize_run, _("Execute only resize conversion on current picture"))
+ToolTip(b_resize_run, text=_("Execute only resize conversion on current picture"))
 # Crop
-Hovertip(rb1_crop, _("Select crop by absolute coordinate.\nRemember point (0,0) is located in left-top corner of image."))
-Hovertip(rb2_crop, _("Select crop by absolute coorinate left-top corner plus width and height.\nRemember point (0,0) is located in left-top corner of image."))
-Hovertip(rb3_crop, _("Select crop by gravity plus width and height plus offset.\nRemember point (0,0) is located in left-top corner of image."))
-Hovertip(e1_crop_1, _("x1 - horizontal position of left-top corner of crop\nClick left mouse button on preview in place of left-top corner"))
-Hovertip(e2_crop_1, _("y1 - vertical position of left-top corner of crop\nClick left mouse button on preview in place of left-top corner"))
-Hovertip(e3_crop_1, _("x2 - horizontal position of right-bottom corner of crop\nClick right mouse button on preview in place of left-top corner"))
-Hovertip(e4_crop_1, _("y2 - vertical position of right-bottom corner of crop\nClick right mouse button on preview in place of left-top corner"))
-Hovertip(e1_crop_2, _("x1 - horizontal position of left-top corner of crop"))
-Hovertip(e2_crop_2, _("y1 - vertical position of left-top corner of crop"))
-Hovertip(e3_crop_2, _("X - width of crop"))
-Hovertip(e4_crop_2, _("Y - height of crop"))
-Hovertip(e1_crop_3, _("dx - horizontal offset from gravity point"))
-Hovertip(e2_crop_3, _("dy - vertical offsef from gravity point"))
-Hovertip(e3_crop_3, _("X - width of crop"))
-Hovertip(e4_crop_3, _("Y - height of crop"))
-Hovertip(b_crop_read, _("Take size of crop from current picture.\nCrop will be 100% of original picture"))
-Hovertip(b_crop_show, _("Refresh preview to see crop on picture"))
-Hovertip(frame_crop_gravity, _("Use gravity direction for select crop"))
-Hovertip(b_crop_run, _("Execute only crop conversion on current picture"))
+ToolTip(rb1_crop, text=_("Select crop by absolute coordinate.\nRemember point (0,0) is located in left-top corner of image."))
+ToolTip(rb2_crop, text=_("Select crop by absolute coorinate left-top corner plus width and height.\nRemember point (0,0) is located in left-top corner of image."))
+ToolTip(rb3_crop, text=_("Select crop by gravity plus width and height plus offset.\nRemember point (0,0) is located in left-top corner of image."))
+ToolTip(e1_crop_1, text=_("x1 - horizontal position of left-top corner of crop\nClick left mouse button on preview in place of left-top corner"))
+ToolTip(e2_crop_1, text=_("y1 - vertical position of left-top corner of crop\nClick left mouse button on preview in place of left-top corner"))
+ToolTip(e3_crop_1, text=_("x2 - horizontal position of right-bottom corner of crop\nClick right mouse button on preview in place of left-top corner"))
+ToolTip(e4_crop_1, text=_("y2 - vertical position of right-bottom corner of crop\nClick right mouse button on preview in place of left-top corner"))
+ToolTip(e1_crop_2, text=_("x1 - horizontal position of left-top corner of crop"))
+ToolTip(e2_crop_2, text=_("y1 - vertical position of left-top corner of crop"))
+ToolTip(e3_crop_2, text=_("X - width of crop"))
+ToolTip(e4_crop_2, text=_("Y - height of crop"))
+ToolTip(e1_crop_3, text=_("dx - horizontal offset from gravity point"))
+ToolTip(e2_crop_3, text=_("dy - vertical offsef from gravity point"))
+ToolTip(e3_crop_3, text=_("X - width of crop"))
+ToolTip(e4_crop_3, text=_("Y - height of crop"))
+ToolTip(b_crop_read, text=_("Take size of crop from current picture.\nCrop will be 100% of original picture"))
+ToolTip(b_crop_show, text=_("Refresh preview to see crop on picture"))
+ToolTip(frame_crop_gravity, text=_("Use gravity direction for select crop"))
+ToolTip(b_crop_run, text=_("Execute only crop conversion on current picture"))
 # Text
-Hovertip(e_text, _("Click here and type text"))
-Hovertip(e_text_size, _("Text size"))
-Hovertip(e_text_angle, _("Angle of text"))
-Hovertip(co_text_font, _("Font"))
-Hovertip(rb_text_in, _("Put text on picture"))
-Hovertip(rb_text_out, _("Put text below picture"))
-Hovertip(cb_text_gravity, _("Use gravity for putting text or Absolute position"))
-Hovertip(frame_text_gravity, _("Use gravity direction for text placement"))
-Hovertip(cb_text_box, _("Use background for text"))
-Hovertip(e_text_x, _("Offset from gravity or absolute position"))
-Hovertip(e_text_y, _("Offset from gravity or absolute position"))
-Hovertip(l_text_color, _("Selected color of text and background"))
-Hovertip(b_text_color,_("Select color of text"))
-Hovertip(b_text_box_color, _("Select color of background"))
-Hovertip(b_text_run, _("Execute only adding text on current picture"))
+ToolTip(e_text, text=_("Click here and type text"))
+ToolTip(e_text_size, text=_("Text size"))
+ToolTip(e_text_angle, text=_("Angle of text"))
+ToolTip(co_text_font, text=_("Font"))
+ToolTip(rb_text_in, text=_("Put text on picture"))
+ToolTip(rb_text_out, text=_("Put text below picture"))
+ToolTip(cb_text_gravity, text=_("Use gravity for putting text or Absolute position"))
+ToolTip(frame_text_gravity, text=_("Use gravity direction for text placement"))
+ToolTip(cb_text_box, text=_("Use background for text"))
+ToolTip(e_text_x, text=_("Offset from gravity or absolute position"))
+ToolTip(e_text_y, text=_("Offset from gravity or absolute position"))
+ToolTip(l_text_color, text=_("Selected color of text and background"))
+ToolTip(b_text_color, text=_("Select color of text"))
+ToolTip(b_text_box_color, text=_("Select color of background"))
+ToolTip(b_text_run, text=_("Execute only adding text on current picture"))
 # Rotate
-Hovertip(rb_rotate_own, _("Select if want to use own angle of rotation"))
-Hovertip(e_rotate_own, _("Put angle of rotation. Rotation is in right direction.\nBackground color is as choosed by Color button"))
-Hovertip(l_rotate_color, _("Selected color to fill a gap"))
-Hovertip(b_rotate_color, _("If OWN is choosed, select color to fill a gap."))
-Hovertip(b_rotate_run, _("Execute only rotate conversion on current picture"))
+ToolTip(rb_rotate_own, text=_("Select if want to use own angle of rotation"))
+ToolTip(e_rotate_own, text=_("Put angle of rotation. Rotation is in right direction.\nBackground color is as choosed by Color button"))
+ToolTip(l_rotate_color, text=_("Selected color to fill a gap"))
+ToolTip(b_rotate_color, text=_("If OWN is choosed, select color to fill a gap."))
+ToolTip(b_rotate_run, text=_("Execute only rotate conversion on current picture"))
 # Scaling
-Hovertip(e2_resize, _("Put percent for rescale of picture"))
-Hovertip(b_resize_run, _("Execute only resize conversion on current picture"))
+ToolTip(e2_resize, text=_("Put percent for rescale of picture"))
+ToolTip(b_resize_run, text=_("Execute only resize conversion on current picture"))
 # Border
-Hovertip(e_border_ns, _("Put width of vertical part of border"))
-Hovertip(e_border_we, _("Put width of horizontal part of border"))
-Hovertip(l_border_color, _("Selected color of border"))
-Hovertip(b_border_color, _("Select color of border"))
-Hovertip(b_border_run, _("Execute only add border conversion on current picture"))
+ToolTip(e_border_ns, text=_("Put width of vertical part of border"))
+ToolTip(e_border_we, text=_("Put width of horizontal part of border"))
+ToolTip(l_border_color, text=_("Selected color of border"))
+ToolTip(b_border_color, text=_("Select color of border"))
+ToolTip(b_border_run, text=_("Execute only add border conversion on current picture"))
 # Black-white
-Hovertip(rb1_bw, _("Convert picture into gray scale - black-white"))
-Hovertip(rb2_bw, _("Convert picture into sepia - old style silver based photography"))
-Hovertip(e_bw_sepia, _("Put threshold of sepia, try values in range 80-95"))
-Hovertip(b_bw_run, _("Execute only black-white/sepia conversion on current picture"))
+ToolTip(rb1_bw, text=_("Convert picture into gray scale - black-white"))
+ToolTip(rb2_bw, text=_("Convert picture into sepia - old style silver based photography"))
+ToolTip(e_bw_sepia, text=_("Put threshold of sepia, try values in range 80-95"))
+ToolTip(b_bw_run, text=_("Execute only black-white/sepia conversion on current picture"))
 # Contrast
-Hovertip(e1_contrast, _("Black point.\nTry values in range 0-0.2"))
-Hovertip(e2_contrast, _("White point.\nTry values in range 0-0.2"))
-Hovertip(rb1_contrast, _("Enhance contrast of image by adjusting the span of the available colors"))
-Hovertip(rb2_contrast, _("Enhances the difference between lighter & darker values of the image"))
-Hovertip(co_contrast_selection, _("Select power of reduce (negative values) or increase (positive values) contrast"))
-Hovertip(b_contrast_run, _("Execute only change contrast conversion on current picture"))
+ToolTip(e1_contrast, text=_("Black point.\nTry values in range 0-0.2"))
+ToolTip(e2_contrast, text=_("White point.\nTry values in range 0-0.2"))
+ToolTip(rb1_contrast, text=_("Enhance contrast of image by adjusting the span of the available colors"))
+ToolTip(rb2_contrast, text=_("Enhances the difference between lighter & darker values of the image"))
+ToolTip(co_contrast_selection, text=_("Select power of reduce (negative values) or increase (positive values) contrast"))
+ToolTip(b_contrast_run, text=_("Execute only change contrast conversion on current picture"))
 # Normalize
-Hovertip(rb1_normalize, _("Normalize color channels"))
-Hovertip(co_normalize_channel, _("Select channel for normalize"))
-Hovertip(rb2_normalize, _("Scale the minimum and maximum values to a full quantum range"))
-Hovertip(b_normalize_run, _("Execute only color normalize conversion on current picture"))
+ToolTip(rb1_normalize, text=_("Normalize color channels"))
+ToolTip(co_normalize_channel, text=_("Select channel for normalize"))
+ToolTip(rb2_normalize, text=_("Scale the minimum and maximum values to a full quantum range"))
+ToolTip(b_normalize_run, text=_("Execute only color normalize conversion on current picture"))
 # Mirror
-Hovertip(cb_mirror_flip, _("Mirror top-bottom"))
-Hovertip(cb_mirror_flop, _("Mirror left-right"))
-Hovertip(b_mirror_run, _("Execute only mirror conversion on current picture"))
+ToolTip(cb_mirror_flip, text=_("Mirror top-bottom"))
+ToolTip(cb_mirror_flop, text=_("Mirror left-right"))
+ToolTip(b_mirror_run, text=_("Execute only mirror conversion on current picture"))
 # Vignette
-Hovertip(e_vignette_radius, _("Radius of the Gaussian blur effect"))
-Hovertip(e_vignette_sigma, _("Standard deviation of the Gaussian effect"))
-Hovertip(e_vignette_dx, _("Horizontal offset of vignette"))
-Hovertip(e_vignette_dy, _("Vertical offset of vignette"))
-Hovertip(l_vignette_color, _("Selected color of corners"))
-Hovertip(b_vignette_color, _("Select color of corners"))
-Hovertip(b_vignette_run, _("Execute only vignette conversion on current picture"))
+ToolTip(e_vignette_radius, text=_("Radius of the Gaussian blur effect"))
+ToolTip(e_vignette_sigma, text=_("Standard deviation of the Gaussian effect"))
+ToolTip(e_vignette_dx, text=_("Horizontal offset of vignette"))
+ToolTip(e_vignette_dy, text=_("Vertical offset of vignette"))
+ToolTip(l_vignette_color, text=_("Selected color of corners"))
+ToolTip(b_vignette_color, text=_("Select color of corners"))
+ToolTip(b_vignette_run, text=_("Execute only vignette conversion on current picture"))
 # Logo
-Hovertip(b_logo_select, _("Select picture to put on picture"))
-Hovertip(e_logo_width, _("Width picture"))
-Hovertip(e_logo_height, _("Height picture"))
-Hovertip(e_logo_dx, _("Horizontal offset from gravity point"))
-Hovertip(e_logo_dy, _("Vertical offset from gravity point"))
-Hovertip(frame_logo_gravity, _("Use gravity for putting picture"))
-Hovertip(b_logo_run, _("Execute only add logo on current picture"))
+ToolTip(b_logo_select, text=_("Select picture to put on picture"))
+ToolTip(e_logo_width, text=_("Width picture"))
+ToolTip(e_logo_height, text=_("Height picture"))
+ToolTip(e_logo_dx, text=_("Horizontal offset from gravity point"))
+ToolTip(e_logo_dy, text=_("Vertical offset from gravity point"))
+ToolTip(frame_logo_gravity, text=_("Use gravity for putting picture"))
+ToolTip(b_logo_run, text=_("Execute only add logo on current picture"))
 
 ##########################################
 # Run functions
 #
 
 Python_version = "Py " + platform.python_version() + " Tk " + str(TkVersion)
 window_title = ( version.__author__ + " : "
```

### Comparing `FotoKilof-4.2.6/fotokilof/common.py` & `FotoKilof-4.3.0/fotokilof/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,18 +85,16 @@
     while nbytes >= 1024 and i < len(suffixes)-1:
         nbytes /= 1024.
         i += 1
     value = ('%.2f' % nbytes).rstrip('0').rstrip('.')
     return '%s %s' % (value, suffixes[i])
 
 
-def mouse_crop_calculation(width, height, size):
+def mouse_crop_calculation(x_orig, y_orig, size):
     """ recalculation pixels from previev original image """
-    x_orig = width
-    y_orig = height
 
     # x_max, y_max - size of preview, we know max: PREVIEW
     if x_orig > y_orig:
         # preview pixels, calculation of y_max preview
         x_max = size
         y_max = x_max*y_orig/x_orig
     elif y_orig > x_orig:
@@ -140,19 +138,17 @@
     """
     convert corrdinates from crop3:
     offset_x, offset_y, width, height, gravitation
     original image size:
     x_max, y_max
     return coordinates for drawing crop: x0, y0, x1, y1
     """
-    offset_x = coordinates[0]
-    offset_y = coordinates[1]
-    width = coordinates[2]
-    height = coordinates[3]
-    gravitation = coordinates[4]
+
+    offset_x, offset_y, width, height, gravitation = coordinates
+
     if gravitation == "NW":
         x0 = offset_x
         y0 = offset_y
         x1 = x0 + width
         y1 = y0 + height
     elif gravitation == "N":
         x0 = x_max/2 - width/2
```

### Comparing `FotoKilof-4.2.6/fotokilof/convert.py` & `FotoKilof-4.3.0/fotokilof/convert.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/convert_wand.py` & `FotoKilof-4.3.0/fotokilof/convert_wand.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
     return clone
 
 
 def save_close_clone(clone, file_out, exif = 0):
     """ save and close clone after processing """
     if not exif:
         clone.strip()
+    log.write_log(" Save file: " + file_out)
     clone.save(filename=file_out)
     clone.close()
-    log.write_log(" Save file: " + file_out)
 
 
 def gravitation(gravity):
     """ translate gravitation name from Tk to Wand-py specification"""
 
     if gravity == "N":
         result = "north"
@@ -157,16 +157,18 @@
     original image size: image_height, image_width
     """
     if len(logo):
         with Image(filename=logo) as logo_img:
             with Drawing() as draw:
                 position = common.preview_crop_gravity(logo_data, image_height, image_width)
                 draw.composite(operator='over',
-                                left=common.empty(position[0]), top=common.empty(position[1]),
-                                width=common.empty(logo_data[2]), height=common.empty(logo_data[3]),
+                                left=common.empty(position[0]),
+                                top=common.empty(position[1]),
+                                width=common.empty(logo_data[2]),
+                                height=common.empty(logo_data[3]),
                                 image=logo_img)
                 draw(clone)
     log.write_log(" Conversion: logo")
 
 
 def rotate(clone, angle, color, own):
     """ rotate """
@@ -334,12 +336,14 @@
     """ add vignette into picture
     clone - clone of image for processing
     dx, dy - offset from border
     radius - radius of Gaussian blur
     sigma - standard deviation for Gaussian blur
     color - color of corners
     """
-    clone.vignette(radius=common.empty(radius), sigma=common.empty(sigma),
-                    x=common.empty(dx), y=common.empty(dy))
+    clone.vignette(radius=common.empty(radius),
+                    sigma=common.empty(sigma),
+                    x=common.empty(dx),
+                    y=common.empty(dy))
     log.write_log(" Conversion: vigette")
 
 # EOF
```

### Comparing `FotoKilof-4.2.6/fotokilof/entries.py` & `FotoKilof-4.3.0/fotokilof/entries.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/gui.py` & `FotoKilof-4.3.0/fotokilof/gui.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/ini_read.py` & `FotoKilof-4.3.0/fotokilof/ini_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=bare-except
 # pylint: disable=too-many-branches
 
 """
-Copyright (c) 2019-2022 Tomasz Łuczak, TeaM-TL
+Copyright (c) 2019-2023 Tomasz Łuczak, TeaM-TL
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `FotoKilof-4.2.6/fotokilof/ini_save.py` & `FotoKilof-4.3.0/fotokilof/ini_save.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/de/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/en/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/fotokilof.pot` & `FotoKilof-4.3.0/fotokilof/locale/fotokilof.pot`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/id/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/log.py` & `FotoKilof-4.3.0/fotokilof/log.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/magick.py` & `FotoKilof-4.3.0/fotokilof/magick.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/mswindows.py` & `FotoKilof-4.3.0/fotokilof/mswindows.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.2.6/fotokilof/preview.py` & `FotoKilof-4.3.0/fotokilof/preview.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,31 +77,25 @@
     coord - coordinates for crop
     --
     return:
     - filename - path to PPM file
     - file size
     - width and height
     """
-    result = {'filename': None,
-            'size': '0',
-            'width': '0',
-            'height': '0',
-            'preview_width': '0',
-            'preview_height': '0'}
 
     if file_in is not None:
         if os.path.isfile(file_in):
             filesize = common.humansize(os.path.getsize(file_in))
 
             clone = convert_wand.make_clone(file_in)
             width = str(clone.width)
             height = str(clone.height)
-
-            convert_wand.resize(clone, str(size) + "x" + str(size))
             clone.convert('ppm')
+            convert_wand.resize(clone, str(size) + "x" + str(size))
+            
 
             # write crop if coordinates are given
             if len(coord) == 4 :
                 with Drawing() as draw:
                     left_top = (coord[0], coord[1])
                     left_bottom = (coord[0], coord[3])
                     right_top = (coord[2], coord[1])
@@ -119,10 +113,18 @@
             result = {'filename': common.spacja(file_preview),
                           'size': filesize,
                           'width': width,
                           'height': height,
                           'preview_width': preview_width,
                           'preview_height': preview_height
                     }
+    else:
+        result = {'filename': None,
+            'size': '0',
+            'width': '0',
+            'height': '0',
+            'preview_width': '0',
+            'preview_height': '0'}
+
     return result
 
 # EOF
```

### Comparing `FotoKilof-4.2.6/fotokilof/version.py` & `FotoKilof-4.3.0/fotokilof/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.2.6"
+__version__ = "4.3.0"
 __author__ = "Tomasz Łuczak"
 __email__ = "tlu@team-tl.pl"
 __appname__ = "FotoKilof"
 __description__ = "Nice gui for ImageMagick"
 __keywords__ = "GUI ImageMagick FotoKilof"
 __url__ = "https://github.com/TeaM-TL/FotoKilof"
 __copyright__ = "2019-2023"
```

### Comparing `FotoKilof-4.2.6/setup.py` & `FotoKilof-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['pillow','tkcolorpicker','wand'],
+    install_requires=['pillow','wand','ttkbootstrap'],
     entry_points = {
         "gui_scripts": [
             "fotokilof = fotokilof:__main__",
         ]
     },
     include_package_data=True,
 )
```

