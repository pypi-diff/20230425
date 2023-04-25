# Comparing `tmp/py-Ayra-8.6.3.tar.gz` & `tmp/py-Ayra-8.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-8.6.3.tar", last modified: Mon Apr 24 18:38:47 2023, max compression
+gzip compressed data, was "py-Ayra-8.6.4.tar", last modified: Tue Apr 25 08:19:52 2023, max compression
```

## Comparing `py-Ayra-8.6.3.tar` & `py-Ayra-8.6.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.650686 py-Ayra-8.6.3/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-23 15:12:06.000000 py-Ayra-8.6.3/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.650686 py-Ayra-8.6.3/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-04-23 15:12:06.000000 py-Ayra-8.6.3/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.654686 py-Ayra-8.6.3/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-23 18:23:04.000000 py-Ayra-8.6.3/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-24 18:24:04.000000 py-Ayra-8.6.3/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19939 2023-04-23 01:47:25.000000 py-Ayra-8.6.3/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28729 2023-04-24 18:38:29.000000 py-Ayra-8.6.3/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.6.3/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-24 18:38:29.000000 py-Ayra-8.6.3/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-24 18:38:47.000000 py-Ayra-8.6.3/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-24 18:38:47.000000 py-Ayra-8.6.3/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:38:47.000000 py-Ayra-8.6.3/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:38:47.000000 py-Ayra-8.6.3/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 18:38:47.000000 py-Ayra-8.6.3/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:38:47.658686 py-Ayra-8.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.671318 py-Ayra-8.6.4/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-04-25 08:19:23.000000 py-Ayra-8.6.4/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.675318 py-Ayra-8.6.4/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-25 08:19:23.000000 py-Ayra-8.6.4/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.675318 py-Ayra-8.6.4/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-23 18:23:04.000000 py-Ayra-8.6.4/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-24 18:24:04.000000 py-Ayra-8.6.4/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19939 2023-04-23 01:47:25.000000 py-Ayra-8.6.4/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28729 2023-04-24 18:38:29.000000 py-Ayra-8.6.4/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.6.4/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-25 08:19:23.000000 py-Ayra-8.6.4/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-25 08:19:52.000000 py-Ayra-8.6.4/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-25 08:19:52.000000 py-Ayra-8.6.4/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:19:52.000000 py-Ayra-8.6.4/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 08:19:52.000000 py-Ayra-8.6.4/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-25 08:19:52.000000 py-Ayra-8.6.4/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 08:19:52.679318 py-Ayra-8.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.6.4/setup.py
```

### Comparing `py-Ayra-8.6.3/Ayra/__init__.py` & `py-Ayra-8.6.4/Ayra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     HNDLR = udB.get_key("HNDLR") or "."
     SUDOS = udB.get_key("SUDOS") or "1054295664"
     VC_SUDOS = udB.get_key("VC_SUDOS") or "1054295664"
     DUAL_HNDLR = udB.get_key("DUAL_HNDLR") or "/"
     SUDO_HNDLR = udB.get_key("SUDO_HNDLR") or "$"
     INLINE_PM = udB.set_key("INLINE_PM", "True")
     PMLOG = udB.set_key("PMLOG", "True")
-    PMSETTING = udB.set_key("PMSETTING", "True")
 else:
     print("Ayra 2022 © senpai80")
 
     from logging import getLogger
 
     LOGS = getLogger("Ayra")
```

### Comparing `py-Ayra-8.6.3/Ayra/__main__.py` & `py-Ayra-8.6.4/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/_misc/__init__.py` & `py-Ayra-8.6.4/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/_misc/_assistant.py` & `py-Ayra-8.6.4/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/_misc/_decorators.py` & `py-Ayra-8.6.4/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/_misc/_supporter.py` & `py-Ayra-8.6.4/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/_misc/_wrappers.py` & `py-Ayra-8.6.4/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/configs.py` & `py-Ayra-8.6.4/Ayra/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     HEROKU_APP_NAME = config("HEROKU_APP_NAME", default=None)
     HEROKU_API = config("HEROKU_API", default=None)
     SUDO = config("SUDO", default=True, cast=bool)
     VC_SESSION = config("VC_SESSION", default=SESSION)
     ADDONS = config("ADDONS", default=False, cast=bool)
     INLINE_PIC = config("INLINE_PIC", default=False, cast=bool)
     VCBOT = config("VCBOT", default=True, cast=bool)
-    PMSETTING = config("PMSETTING", default=True, cast=bool)
     DISABLE_PMDEL = config("DISABLE_PMDEL", default=True, cast=bool)
     # for railway
     REDISPASSWORD = config("REDISPASSWORD", default=None)
     REDISHOST = config("REDISHOST", default=None)
     REDISPORT = config("REDISPORT", default=None)
     REDISUSER = config("REDISUSER", default=None)
     # for sql
```

### Comparing `py-Ayra-8.6.3/Ayra/dB/__init__.py` & `py-Ayra-8.6.4/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/afk_db.py` & `py-Ayra-8.6.4/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/antiflood_db.py` & `py-Ayra-8.6.4/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/asst_fns.py` & `py-Ayra-8.6.4/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/asstcmd_db.py` & `py-Ayra-8.6.4/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/autoban_db.py` & `py-Ayra-8.6.4/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/blacklist_db.py` & `py-Ayra-8.6.4/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/botchat_db.py` & `py-Ayra-8.6.4/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/broadcast_db.py` & `py-Ayra-8.6.4/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/ch_db.py` & `py-Ayra-8.6.4/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/dnd_db.py` & `py-Ayra-8.6.4/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/echo_db.py` & `py-Ayra-8.6.4/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/filestore_db.py` & `py-Ayra-8.6.4/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/filter_db.py` & `py-Ayra-8.6.4/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/forcesub_db.py` & `py-Ayra-8.6.4/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/gban_mute_db.py` & `py-Ayra-8.6.4/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-8.6.4/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/greetings_db.py` & `py-Ayra-8.6.4/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/logusers_db.py` & `py-Ayra-8.6.4/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/mute_db.py` & `py-Ayra-8.6.4/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/night_db.py` & `py-Ayra-8.6.4/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/notes_db.py` & `py-Ayra-8.6.4/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/nsfw_db.py` & `py-Ayra-8.6.4/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/pmpermit_db.py` & `py-Ayra-8.6.4/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/snips_db.py` & `py-Ayra-8.6.4/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/vc_sudos.py` & `py-Ayra-8.6.4/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/dB/warn_db.py` & `py-Ayra-8.6.4/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/FastTelethon.py` & `py-Ayra-8.6.4/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/__init__.py` & `py-Ayra-8.6.4/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/admins.py` & `py-Ayra-8.6.4/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/executor.py` & `py-Ayra-8.6.4/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/gDrive.py` & `py-Ayra-8.6.4/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/google_image.py` & `py-Ayra-8.6.4/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/helper.py` & `py-Ayra-8.6.4/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/info.py` & `py-Ayra-8.6.4/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/misc.py` & `py-Ayra-8.6.4/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/tools.py` & `py-Ayra-8.6.4/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/fns/ytdl.py` & `py-Ayra-8.6.4/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/kynan.py` & `py-Ayra-8.6.4/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/loader.py` & `py-Ayra-8.6.4/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/BaseClient.py` & `py-Ayra-8.6.4/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/__init__.py` & `py-Ayra-8.6.4/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/_database.py` & `py-Ayra-8.6.4/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/_extra.py` & `py-Ayra-8.6.4/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/connections.py` & `py-Ayra-8.6.4/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/funcs.py` & `py-Ayra-8.6.4/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/loader.py` & `py-Ayra-8.6.4/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/Ayra/startup/utils.py` & `py-Ayra-8.6.4/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/LICENSE` & `py-Ayra-8.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/PKG-INFO` & `py-Ayra-8.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.6.3
+Version: 8.6.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.6.3/README.md` & `py-Ayra-8.6.4/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-8.6.4/py_Ayra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.6.3
+Version: 8.6.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.6.3/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-8.6.4/py_Ayra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.3/setup.py` & `py-Ayra-8.6.4/setup.py`

 * *Files identical despite different names*

