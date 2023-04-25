# Comparing `tmp/mipac-0.4.2.tar.gz` & `tmp/mipac-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipac-0.4.2.tar", last modified: Tue Mar 21 19:20:04 2023, max compression
+gzip compressed data, was "mipac-0.4.3.tar", last modified: Tue Apr 25 08:41:27 2023, max compression
```

## Comparing `mipac-0.4.2.tar` & `mipac-0.4.3.tar`

### file list

```diff
@@ -1,134 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.927587 mipac-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-21 19:19:52.000000 mipac-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-21 19:19:52.000000 mipac-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-03-21 19:20:04.927587 mipac-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-21 19:19:52.000000 mipac-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.927587 mipac-0.4.2/mipac/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 19:20:04.927587 mipac-0.4.2/mipac/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.915587 mipac-0.4.2/mipac/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/abstract/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/abstract/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/abstract/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.915587 mipac-0.4.2/mipac/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.915587 mipac-0.4.2/mipac/actions/admins/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/my.py
--rw-r--r--   0 runner    (1001) docker     (123)    18490 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/actions/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.919587 mipac-0.4.2/mipac/errors/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/errors/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.919587 mipac-0.4.2/mipac/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.919587 mipac-0.4.2/mipac/manager/admins/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/my.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/manager/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.923587 mipac-0.4.2/mipac/models/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.923587 mipac-0.4.2/mipac/models/lite/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/lite/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.927587 mipac-0.4.2/mipac/types/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-03-21 19:19:52.000000 mipac-0.4.2/mipac/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:20:04.915587 mipac-0.4.2/mipac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-03-21 19:20:04.000000 mipac-0.4.2/mipac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-03-21 19:20:04.000000 mipac-0.4.2/mipac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:20:04.000000 mipac-0.4.2/mipac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-21 19:20:04.000000 mipac-0.4.2/mipac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-21 19:20:04.000000 mipac-0.4.2/mipac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-21 19:19:52.000000 mipac-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-21 19:19:52.000000 mipac-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-21 19:20:04.927587 mipac-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-21 19:19:52.000000 mipac-0.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-21 19:19:52.000000 mipac-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 08:41:11.000000 mipac-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 08:41:11.000000 mipac-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-25 08:41:27.529852 mipac-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-25 08:41:11.000000 mipac-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.513851 mipac-0.4.3/mipac/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/actions/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.521851 mipac-0.4.3/mipac/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.521851 mipac-0.4.3/mipac/manager/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.525851 mipac-0.4.3/mipac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.525851 mipac-0.4.3/mipac/models/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.513851 mipac-0.4.3/mipac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-25 08:41:11.000000 mipac-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 08:41:11.000000 mipac-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 08:41:27.529852 mipac-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:41:11.000000 mipac-0.4.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:41:11.000000 mipac-0.4.3/versioneer.py
```

### Comparing `mipac-0.4.2/LICENSE` & `mipac-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/PKG-INFO` & `mipac-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipac
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/mipac
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
@@ -83,14 +83,24 @@
 Client.config.is_ayuskey = True
 Client.config.use_version = 13
 Client.config.from_dict(is_ayuskey=True, use_version=13)
 ```
 
 上記のように複数の値を同時に更新する場合特に`from_dict`は有効な方法になります。
 
+### 注意事項
+
+### 一部サーバー(インスタンス)のバージョンによっては正常に動作しない可能性があります
+
+MiPACの特徴として、v11,v12,v13のバージョンごとに生じる変更点をなるべく気にしなくてよいように作成していますが、現状の最新版であるv13でもv13の中で削除されたり、増えたりした物があります。結果的に追従しきれていない箇所があることがあります。そのため、そのような物を見つけた場合は、使用しているサーバーのバージョンと使用できないエンドポイント名をIssueに送信してください。
+
+### モデルを基本的に自分でインスタンス化することは推奨しません
+
+MiPACのモデルでは多くの場合、キーワード引数に `client`を受け取り、それを用いて`api` プロパティを生成します。しかし、サポート途中の機能なのではそこが省かれ、リリース後にモデルのインスタンス化に必要な引数として `client` が追加されることがあります。また、他にもモデルの更新のために引数が変更される可能性があります。そのため、引数の変更に関することをCHANGELOG等で通知することはありません。
+
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
 
 ## LICENSE
 
 準備中
```

### Comparing `mipac-0.4.2/README.md` & `mipac-0.4.3/mipac.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: mipac
+Version: 0.4.3
+Summary: A Python wrapper for the Misskey API
+Home-page: https://github.com/yupix/mipac
+Author: yupix
+Author-email: yupi0982@outlook.jp
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Natural Language :: Japanese
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.11, <4.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: ci
+Provides-Extra: speed
+Provides-Extra: doc
+License-File: LICENSE
+
 # MiPAC
 
 <a href="https://discord.gg/CcT997U"><img src="https://img.shields.io/discord/530299114387406860?style=flat-square&color=5865f2&logo=discord&logoColor=ffffff&label=discord" alt="Discord server invite" /></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-axblack-8bd124.svg"></a>
 <a href="https://www.codacy.com/gh/yupix/MiPAC/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yupix/MiPAC&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c9bf85f195f94ab58bc72ad018a2be9f"/></a>
 <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fyupix%2FMiPAC?
 ref=badge_shield" alt="FOSSA Status">
@@ -63,14 +83,24 @@
 Client.config.is_ayuskey = True
 Client.config.use_version = 13
 Client.config.from_dict(is_ayuskey=True, use_version=13)
 ```
 
 上記のように複数の値を同時に更新する場合特に`from_dict`は有効な方法になります。
 
+### 注意事項
+
+### 一部サーバー(インスタンス)のバージョンによっては正常に動作しない可能性があります
+
+MiPACの特徴として、v11,v12,v13のバージョンごとに生じる変更点をなるべく気にしなくてよいように作成していますが、現状の最新版であるv13でもv13の中で削除されたり、増えたりした物があります。結果的に追従しきれていない箇所があることがあります。そのため、そのような物を見つけた場合は、使用しているサーバーのバージョンと使用できないエンドポイント名をIssueに送信してください。
+
+### モデルを基本的に自分でインスタンス化することは推奨しません
+
+MiPACのモデルでは多くの場合、キーワード引数に `client`を受け取り、それを用いて`api` プロパティを生成します。しかし、サポート途中の機能なのではそこが省かれ、リリース後にモデルのインスタンス化に必要な引数として `client` が追加されることがあります。また、他にもモデルの更新のために引数が変更される可能性があります。そのため、引数の変更に関することをCHANGELOG等で通知することはありません。
+
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
 
 ## LICENSE
 
 準備中
```

### Comparing `mipac-0.4.2/mipac/__init__.py` & `mipac-0.4.3/mipac/__init__.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/admins/ad.py` & `mipac-0.4.3/mipac/actions/admins/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/admins/admin.py` & `mipac-0.4.3/mipac/actions/admins/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from mipac.http import HTTPClient, Route
 from mipac.models.admin import IndexStat, ModerationLog, ServerInfo, UserIP
 from mipac.models.meta import AdminMeta
 from mipac.models.user import UserDetailed
 from mipac.types.admin import IIndexStat, IModerationLog, IServerInfo, ITableStats, IUserIP
 from mipac.types.meta import IAdminMeta, IUpdateMetaBody
 from mipac.types.user import IUserDetailed
-from mipac.util import cache, convert_dict_keys_to_camel
+from mipac.utils.cache import cache
+from mipac.utils.format import convert_dict_keys_to_camel
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class AdminActions(AbstractAction):
     def __init__(self, *, session: HTTPClient, client: ClientManager):
```

### Comparing `mipac-0.4.2/mipac/actions/admins/announcement.py` & `mipac-0.4.3/mipac/actions/admins/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/admins/emoji.py` & `mipac-0.4.3/mipac/actions/admins/emoji.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import NotExistRequiredData, ParameterError
 from mipac.http import Route
 from mipac.models.emoji import CustomEmoji
 from mipac.types.emoji import ICustomEmoji
-from mipac.util import check_multi_arg
+from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.http import HTTPClient
     from mipac.manager.client import ClientManager
 
 
 class AdminEmojiActions(AbstractAction):
```

### Comparing `mipac-0.4.2/mipac/actions/admins/moderator.py` & `mipac-0.4.3/mipac/actions/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/admins/roles.py` & `mipac-0.4.3/mipac/actions/admins/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/admins/user.py` & `mipac-0.4.3/mipac/actions/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/blocking.py` & `mipac-0.4.3/mipac/actions/blocking.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/chart.py` & `mipac-0.4.3/mipac/actions/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/chat.py` & `mipac-0.4.3/mipac/actions/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import NotSupportVersion, NotSupportVersionText, ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.chat import ChatMessage
 from mipac.types.chat import IChatMessage
-from mipac.util import check_multi_arg
+from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class BaseChatAction(AbstractAction):
     def __init__(
```

### Comparing `mipac-0.4.2/mipac/actions/client.py` & `mipac-0.4.3/mipac/actions/client.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/drive.py` & `mipac-0.4.3/mipac/actions/drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,53 +3,60 @@
 from typing import TYPE_CHECKING
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.drive import File, Folder
 from mipac.types.drive import IDriveFile
-from mipac.util import bool_to_string, remove_dict_empty
+from mipac.utils.format import bool_to_string, remove_dict_empty
+from mipac.utils.util import deprecated
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 __all__ = ('DriveActions', 'FileActions', 'FolderActions')
 
 
-class FileActions(AbstractAction):
+class ClientFileActions(AbstractAction):
     def __init__(
-        self, file_id: str | None = None, *, session: HTTPClient, client: ClientManager
+        self,
+        file_id: str | None = None,
+        folder_id: str | None = None,
+        *,
+        session: HTTPClient,
+        client: ClientManager
     ) -> None:
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
-        self.__file_id = file_id
+        self._session: HTTPClient = session
+        self._client: ClientManager = client
+        self._file_id = file_id
+        self._folder_id = folder_id
 
-    async def show_file(self, file_id: str | None, url: str | None) -> File:
+    async def remove(self, file_id: str | None = None) -> bool:
         """
-        ファイルの情報を取得します。
+        指定したIDのファイルを削除します
 
         Parameters
         ----------
         file_id : str | None, default=None
-            ファイルのID
-        url : str | None, default=None
-            ファイルのURL
+            削除するファイルのID
 
         Returns
         -------
-        File
-            ファイルの情報
+        bool
+            削除に成功したかどうか
         """
 
-        data = remove_dict_empty({'fileId': file_id, 'url': url})
-        res: IDriveFile = await self.__session.request(
-            Route('POST', '/api/admin/drive/show-file'), json=data, auth=True, lower=True,
+        file_id = file_id or self._file_id
+        return bool(
+            await self._session.request(
+                Route('POST', '/api/drive/files/delete'), json={'fileId': file_id}, auth=True,
+            )
         )
-        return File(res, client=self.__client)
 
+    @deprecated
     async def remove_file(self, file_id: str | None = None) -> bool:
         """
         指定したIDのファイルを削除します
 
         Parameters
         ----------
         file_id : str | None, default=None
@@ -57,21 +64,56 @@
 
         Returns
         -------
         bool
             削除に成功したかどうか
         """
 
-        file_id = file_id or self.__file_id
+        file_id = file_id or self._file_id
         return bool(
-            await self.__session.request(
+            await self._session.request(
                 Route('POST', '/api/drive/files/delete'), json={'fileId': file_id}, auth=True,
             )
         )
 
+
+class FileActions(ClientFileActions):
+    def __init__(
+        self,
+        file_id: str | None = None,
+        folder_id: str | None = None,
+        *,
+        session: HTTPClient,
+        client: ClientManager
+    ) -> None:
+        super().__init__(file_id=file_id, folder_id=folder_id, session=session, client=client)
+
+    async def show_file(self, file_id: str | None = None, url: str | None = None) -> File:
+        """
+        ファイルの情報を取得します。
+
+        Parameters
+        ----------
+        file_id : str | None, default=None
+            ファイルのID
+        url : str | None, default=None
+            ファイルのURL
+
+        Returns
+        -------
+        File
+            ファイルの情報
+        """
+
+        data = remove_dict_empty({'fileId': file_id, 'url': url})
+        res: IDriveFile = await self._session.request(
+            Route('POST', '/api/admin/drive/show-file'), json=data, auth=True, lower=True,
+        )
+        return File(res, client=self._client)
+
     async def get_files(
         self,
         limit: int = 10,
         since_id: str | None = None,
         until_id: str | None = None,
         folder_id: str | None = None,
         file_type: str | None = None,
@@ -91,25 +133,27 @@
             指定すると、そのフォルダーを起点としてファイルを取得します
         file_type : str | None, default=None
             取得したいファイルの拡張子
         """
         if limit > 100:
             raise ParameterError('limit must be less than 100')
 
+        folder_id = self._folder_id or folder_id
+
         data = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
             'Type': file_type,
         }
-        res: list[IDriveFile] = await self.__session.request(
+        res: list[IDriveFile] = await self._session.request(
             Route('POST', '/api/drive/files'), json=data, auth=True, lower=True
         )
-        return [File(i, client=self.__client) for i in res]
+        return [File(i, client=self._client) for i in res]
 
     async def upload_file(
         self,
         file: str,
         file_name: str | None = None,
         folder_id: str | None = None,
         comment: str | None = None,
@@ -136,35 +180,37 @@
 
         Returns
         -------
         File
             アップロードしたファイルの情報
         """
         file_byte = open(file, 'rb') if file else None
+        folder_id = self._folder_id or folder_id
+
         data = {
             'file': file_byte,
             'name': file_name,
             'folderId': folder_id,
             'comment': comment,
             'isSensitive': bool_to_string(is_sensitive),
             'force': bool_to_string(force),
         }
-        res: IDriveFile = await self.__session.request(
+        res: IDriveFile = await self._session.request(
             Route('POST', '/api/drive/files/create'), data=data, auth=True, lower=True,
         )
-        return File(res, client=self.__client)
+        return File(res, client=self._client)
 
 
-class FolderActions(AbstractAction):
+class ClientFolderActions(AbstractAction):
     def __init__(
         self, folder_id: str | None = None, *, session: HTTPClient, client: ClientManager
     ):
-        self.__folder_id = folder_id
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
+        self._folder_id = folder_id
+        self._session: HTTPClient = session
+        self._client: ClientManager = client
 
     async def create(self, name: str, parent_id: str | None = None) -> bool:
         """
         フォルダーを作成します
 
         Parameters
         ----------
@@ -174,18 +220,18 @@
             親フォルダーのID
 
         Returns
         -------
         bool
             作成に成功したか否か
         """
-        parent_id = parent_id or self.__folder_id
+        parent_id = parent_id or self._folder_id
 
         data = {'name': name, 'parent_id': parent_id}
-        res: bool = await self.__session.request(
+        res: bool = await self._session.request(
             Route('POST', '/api/drive/folders/create'), json=data, lower=True, auth=True,
         )
         return bool(res)
 
     async def delete(self, folder_id: str | None = None) -> bool:
         """
         Parameters
@@ -194,17 +240,17 @@
             削除するノートのID
 
         Returns
         -------
         bool
             削除に成功したか否か
         """
-        folder_id = folder_id or self.__folder_id
+        folder_id = folder_id or self._folder_id
         data = {'folderId': folder_id}
-        res: bool = await self.__session.request(
+        res: bool = await self._session.request(
             Route('POST', '/api/drive/folders/delete'), json=data, lower=True, auth=True,
         )
         return bool(res)
 
     async def get_files(
         self,
         limit: int = 10,
@@ -228,32 +274,39 @@
             指定すると、そのフォルダーを起点としてファイルを取得します
         file_type : str | None, default=None
             取得したいファイルの拡張子
         """
         if limit > 100:
             raise ParameterError('limit must be less than 100')
 
-        folder_id = folder_id or self.__folder_id
+        folder_id = folder_id or self._folder_id
         data = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
             'Type': file_type,
         }
-        res: list[IDriveFile] = await self.__session.request(
+        res: list[IDriveFile] = await self._session.request(
             Route('POST', '/api/drive/files'), json=data, auth=True, lower=True
         )
-        return [File(i, client=self.__client) for i in res]
+        return [File(i, client=self._client) for i in res]
+
+
+class FolderActions(ClientFolderActions):
+    def __init__(
+        self, folder_id: str | None = None, *, session: HTTPClient, client: ClientManager
+    ):
+        super().__init__(folder_id=folder_id, session=session, client=client)
 
 
 class DriveActions(AbstractAction):
     def __init__(self, session: HTTPClient, client: ClientManager):
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
+        self._session: HTTPClient = session
+        self._client: ClientManager = client
 
     async def get_folders(
         self,
         limit: int = 100,
         since_id: str | None = None,
         until_id: str | None = None,
         folder_id: str | None = None,
@@ -275,11 +328,11 @@
 
         data = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
         }
-        data = await self.__session.request(
+        data = await self._session.request(
             Route('POST', '/api/drive/folders'), json=data, lower=True, auth=True,
         )
-        return [Folder(i, client=self.__client) for i in data]
+        return [Folder(i, client=self._client) for i in data]
```

### Comparing `mipac-0.4.2/mipac/actions/favorite.py` & `mipac-0.4.3/mipac/actions/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/federation.py` & `mipac-0.4.3/mipac/actions/federation.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/follow.py` & `mipac-0.4.3/mipac/actions/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/mute.py` & `mipac-0.4.3/mipac/actions/mute.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.mute import MuteUser
 from mipac.types.mute import IMuteUser
-from mipac.util import remove_dict_empty
+from mipac.utils.format import remove_dict_empty
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class MuteActions(AbstractAction):
     def __init__(self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager):
```

### Comparing `mipac-0.4.2/mipac/actions/my.py` & `mipac-0.4.3/mipac/actions/my.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/note.py` & `mipac-0.4.3/mipac/actions/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from mipac.errors.base import APIError, ParameterError
 from mipac.file import MiFile
 from mipac.http import HTTPClient, Route
 from mipac.models.drive import File
 from mipac.models.note import Note, NoteReaction, NoteState, NoteTranslateResult
 from mipac.models.poll import MiPoll, Poll
 from mipac.types.note import ICreatedNote, INote, INoteState, INoteTranslateResult
-from mipac.util import cache, check_multi_arg, remove_dict_empty
+from mipac.utils.cache import cache
+from mipac.utils.format import remove_dict_empty
+from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.client import ClientManager
 
 __all__ = ['NoteActions']
```

### Comparing `mipac-0.4.2/mipac/actions/poll.py` & `mipac-0.4.3/mipac/actions/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/actions/reaction.py` & `mipac-0.4.3/mipac/actions/reaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from mipac.config import config
 from mipac.errors.base import NotSupportVersion
 from mipac.http import Route
 from mipac.models.emoji import CustomEmoji
 from mipac.models.note import NoteReaction
 from mipac.types.meta import ILiteMeta
 from mipac.types.note import INoteReaction
-from mipac.util import remove_dict_empty
+from mipac.utils.format import remove_dict_empty
 
 if TYPE_CHECKING:
     from mipac.http import HTTPClient
     from mipac.manager.client import ClientManager
 
 
 class ReactionActions(AbstractAction):
```

### Comparing `mipac-0.4.2/mipac/actions/user.py` & `mipac-0.4.3/mipac/actions/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from typing import TYPE_CHECKING, AsyncGenerator, Literal, Optional
 
 from mipac.config import config
 from mipac.errors.base import NotExistRequiredData, NotSupportVersion, ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.user import Achievement, LiteUser, UserDetailed
-from mipac.util import cache, check_multi_arg, remove_dict_empty
+from mipac.utils.cache import cache
+from mipac.utils.format import remove_dict_empty
+from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
     from mipac.models.note import Note
 
 __all__ = ['UserActions']
```

### Comparing `mipac-0.4.2/mipac/client.py` & `mipac-0.4.3/mipac/manager/blocking.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from mipac.config import Config, config
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from mipac.abstract.manager import AbstractManager
+from mipac.actions.blocking import BlockingActions
 from mipac.http import HTTPClient
-from mipac.manager.client import ClientManager
 
+if TYPE_CHECKING:
+    from mipac.manager.client import ClientManager
 
-class Client:
-    def __init__(self, url: str, token: str | None = None) -> None:
-        self.__url: str = url
-        self.__token: str | None = token
-        self.config: Config = config
-        self.http: HTTPClient = HTTPClient(url, token)
 
-    @property
-    def api(self) -> ClientManager:
-        return ClientManager(self.http, self.config)
+class BlockingManager(AbstractManager):
+    def __init__(self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager):
+        self.__user_id: str | None = user_id
+        self.__session: HTTPClient = session
+        self.__client: ClientManager = client
 
-    async def close_session(self) -> None:
-        await self.http.close_session()
+    @property
+    def action(self) -> BlockingActions:
+        return BlockingActions(
+            user_id=self.__user_id, session=self.__session, client=self.__client
+        )
```

### Comparing `mipac-0.4.2/mipac/config.py` & `mipac-0.4.3/mipac/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class CacheConfig:
     def __init__(self, options: CacheConfigData) -> None:
         self.maxsize: int = options.maxsize
         self.ttl: int = options.ttl
 
 
 IMisskeyDistribution = Literal['ayuskey', 'm544', 'areionskey', 'official']
+IMisskeyVersions = Literal[13, 12, 11]
 
 
 class ILimits(TypedDict, total=False):
     channel_name: int
     channel_description: int
 
 
@@ -52,37 +53,37 @@
     def __init__(
         self,
         *,
         host: str = '',
         is_ssl: bool = True,
         distro: IMisskeyDistribution = 'official',
         is_ayuskey: bool = False,
-        use_version: Literal[13, 12, 11] = 12,
+        use_version: IMisskeyVersions = 12,
         cache: CacheConfigData | None = None,
         use_version_autodetect: bool = True,
         features: IFeatures | None = None,
         limits: ILimits | None = None,
     ) -> None:
         self.distro: IMisskeyDistribution = distro
         self.is_ssl: bool = is_ssl
         self.host: str = host
         self.is_ayuskey: bool = is_ayuskey
-        self.use_version: Literal[13, 12, 11] = use_version
+        self.use_version: IMisskeyVersions = use_version
         self.cache: CacheConfig = CacheConfig(cache or CacheConfigData())
         self.use_version_autodetect: bool = use_version_autodetect
         self.features: Features = Features(features) if features else Features()
         self.limits: Limits = Limits(limits) if limits else Limits()
 
     def from_dict(
         self,
         *,
         host: str | None = None,
         is_ssl: bool | None = None,
         is_ayuskey: bool | None = None,
-        use_version: Literal[13, 12, 11] | None = None,
+        use_version: IMisskeyVersions | None = None,
         cache: CacheConfigData | None = None,
         use_version_autodetect: bool | None = None,
         features: IFeatures | None = None,
         limits: ILimits | None = None,
     ) -> Self:
         self.host = host or self.host
         self.is_ssl = is_ssl if is_ssl is not None else self.is_ssl
```

### Comparing `mipac-0.4.2/mipac/errors/base.py` & `mipac-0.4.3/mipac/errors/base.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/errors/errors.py` & `mipac-0.4.3/mipac/errors/errors.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/file.py` & `mipac-0.4.3/mipac/file.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/http.py` & `mipac-0.4.3/mipac/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
 
+import json
+import logging
 import re
 import sys
 from typing import Any, Literal, TypeVar
 
 import aiohttp
 
 from mipac import __version__
 from mipac.config import config
 from mipac.errors.base import APIError
 from mipac.types.endpoints import ENDPOINTS
 from mipac.types.meta import IMeta
 from mipac.types.user import IUserDetailed
-from mipac.util import _from_json, remove_dict_empty, upper_to_lower
+from mipac.utils.format import remove_dict_empty, upper_to_lower
+from mipac.utils.util import COLORS, _from_json
+
+_log = logging.getLogger(__name__)
 
 
 class _MissingSentinel:
     def __eq__(self, other):
         return False
 
     def __bool__(self):
@@ -61,22 +66,25 @@
         self._token: str | None = token
 
     @property
     def session(self) -> aiohttp.ClientSession:
         return self._session
 
     async def request(
-        self, route: Route, auth: bool = False, remove_none: bool = True, **kwargs
+        self,
+        route: Route,
+        auth: bool = False,
+        remove_none: bool = True,
+        lower: bool = True,
+        **kwargs,
     ) -> R:
         headers: dict[str, str] = {
             'User-Agent': self.user_agent,
         }
 
-        is_lower = kwargs.pop('lower') if kwargs.get('lower') else False
-
         if 'json' in kwargs:
             headers['Content-Type'] = 'application/json'
             kwargs['json'] = kwargs.pop('json')
 
         if auth:
             key = 'json' if 'json' in kwargs or 'data' not in kwargs else 'data'
             if not kwargs.get(key):
@@ -87,19 +95,27 @@
         replace_list = kwargs.pop('replace_list', {})
 
         for i in ('json', 'data'):
             if kwargs.get(i) and remove_none:
                 kwargs[i] = remove_dict_empty(kwargs[i])
         async with self._session.request(route.method, self._url + route.path, **kwargs) as res:
             data = await json_or_text(res)
-            if is_lower:
+            if lower:
                 if isinstance(data, list):
                     data = [upper_to_lower(i, replace_list=replace_list) for i in data]
                 if isinstance(data, dict):
                     data = upper_to_lower(data)
+            _log.debug(
+                f'''{COLORS.green}
+REQUEST:{COLORS.reset}
+    {kwargs}
+{COLORS.green}RESPONSE:{COLORS.reset}
+    {json.dumps(data, ensure_ascii=False, indent=4) if data else data}
+                '''
+            )
             if res.status == 204 and data is None:
                 return True  # type: ignore
             if 300 > res.status >= 200:
                 return data  # type: ignore
             if 511 > res.status >= 300:
                 if isinstance(data, dict):
                     APIError(data, res.status).raise_error()
```

### Comparing `mipac-0.4.2/mipac/manager/admins/ad.py` & `mipac-0.4.3/mipac/manager/admins/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/admin.py` & `mipac-0.4.3/mipac/manager/admins/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/announcement.py` & `mipac-0.4.3/mipac/manager/admins/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/emoji.py` & `mipac-0.4.3/mipac/manager/admins/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/moderator.py` & `mipac-0.4.3/mipac/manager/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/roles.py` & `mipac-0.4.3/mipac/manager/admins/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/admins/user.py` & `mipac-0.4.3/mipac/manager/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/blocking.py` & `mipac-0.4.3/mipac/manager/chart.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
-from mipac.actions.blocking import BlockingActions
-from mipac.http import HTTPClient
+from mipac.actions.chart import ChartActions
 
 if TYPE_CHECKING:
-    from mipac.manager.client import ClientManager
+    from mipac.client import ClientManager
+    from mipac.http import HTTPClient
 
+__all__ = ('ChartManager',)
 
-class BlockingManager(AbstractManager):
-    def __init__(self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager):
-        self.__user_id: str | None = user_id
+
+class ChartManager(AbstractManager):
+    def __init__(self, *, session: HTTPClient, client: ClientManager):
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
 
     @property
-    def action(self) -> BlockingActions:
-        return BlockingActions(
-            user_id=self.__user_id, session=self.__session, client=self.__client
-        )
+    def action(self) -> ChartActions:
+        return ChartActions(session=self.__session, client=self.__client)
```

### Comparing `mipac-0.4.2/mipac/manager/chart.py` & `mipac-0.4.3/mipac/manager/mute.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
-from mipac.actions.chart import ChartActions
+from mipac.actions.mute import MuteActions
+from mipac.http import HTTPClient
 
 if TYPE_CHECKING:
-    from mipac.client import ClientManager
-    from mipac.http import HTTPClient
+    from mipac.manager.client import ClientManager
 
-__all__ = ('ChartManager',)
 
-
-class ChartManager(AbstractManager):
-    def __init__(self, *, session: HTTPClient, client: ClientManager):
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
+class MuteManager(AbstractManager):
+    def __init__(
+        self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager
+    ) -> None:
+        self._user_id: str | None = user_id
+        self._session: HTTPClient = session
+        self._client: ClientManager = client
 
     @property
-    def action(self) -> ChartActions:
-        return ChartActions(session=self.__session, client=self.__client)
+    def action(self) -> MuteActions:
+        return MuteActions(user_id=self._user_id, session=self._session, client=self._client)
```

### Comparing `mipac-0.4.2/mipac/manager/chat.py` & `mipac-0.4.3/mipac/manager/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/client.py` & `mipac-0.4.3/mipac/manager/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.actions.client import ClientActions
 from mipac.http import HTTPClient
 from mipac.manager.admins.admin import AdminManager
+from mipac.manager.channel import ChannelManager
 from mipac.manager.chart import ChartManager
 from mipac.manager.chat import ChatManager
 from mipac.manager.drive import DriveManager
+from mipac.manager.emoji import EmojiManager
 from mipac.manager.follow import FollowManager, FollowRequestManager
 from mipac.manager.my import MyManager
 from mipac.manager.note import NoteManager
 from mipac.manager.user import UserManager
 
 if TYPE_CHECKING:
     from mipac.config import Config
@@ -28,27 +30,32 @@
         self.i = MyManager(session=session, client=self)
         self.note: NoteManager = NoteManager(session=session, client=self)
         self.chat: ChatManager = ChatManager(session=session, client=self)
         self.user: UserManager = UserManager(session=session, client=self)
         self.admin: AdminManager = AdminManager(session=session, client=self)
         self.drive: DriveManager = DriveManager(session=session, client=self)
         self.chart: ChartManager = ChartManager(session=session, client=self)
+        self.channel: ChannelManager = ChannelManager(session=session, client=self)
         self.follow: FollowManager = FollowManager(
             session=session, client=self,
         )
         self.follow_request: FollowRequestManager = FollowRequestManager(
             session=session, client=self,
         )
+        self.emoji: EmojiManager = EmojiManager(session=session, client=self)
         self._config: Config = config
 
     @property
     def action(self) -> ClientActions:
         return ClientActions(session=self.__session, client=self)
 
     def _create_user_instance(self, user: LiteUser) -> UserManager:
         return UserManager(session=self.__session, client=self, user=user)
 
     def _create_note_instance(self, note_id: str) -> NoteManager:
         return NoteManager(note_id, session=self.__session, client=self)
 
+    def _create_channel_instance(self, channel_id: str) -> ChannelManager:
+        return ChannelManager(channel_id=channel_id, session=self.__session, client=self)
+
     async def get_me(self) -> UserDetailed:
         return await self.user.action.get_me()
```

### Comparing `mipac-0.4.2/mipac/manager/drive.py` & `mipac-0.4.3/mipac/manager/note.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
-from mipac.actions.drive import DriveActions, FileActions, FolderActions
-from mipac.http import HTTPClient
+from mipac.actions.note import ClientNoteActions, NoteActions
+from mipac.http import HTTPClient, Route
+from mipac.manager.favorite import FavoriteManager
+from mipac.manager.poll import PollManager
+from mipac.manager.reaction import ReactionManager
 
 if TYPE_CHECKING:
-    from mipac.client import ClientManager
+    from mipac.manager.client import ClientManager
 
-__all__ = ['FolderManager', 'FileManager', 'DriveManager']
 
-
-class FileManager(AbstractManager):
-    def __init__(self, file_id: str | None = None, *, session: HTTPClient, client: ClientManager):
+class ClientNoteManager(AbstractManager):
+    def __init__(self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager):
+        self.__note_id = note_id
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
-        self.__file_id = file_id
-
-    @property
-    def action(self) -> FileActions:
-        """
-        ファイルの操作を行うインスタンスを返します
-
-        Return
-        ------
-        FileActions
-            ファイルに対するアクション
-        """
-        return FileActions(file_id=self.__file_id, client=self.__client, session=self.__session,)
-
-
-class FolderManager(AbstractManager):
-    def __init__(
-        self, folder_id: str | None = None, *, session: HTTPClient, client: ClientManager
-    ):
-        self.__folder_id = folder_id
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
-        self.file: FileManager = FileManager(session=session, client=client)
+        self.reaction: ReactionManager = ReactionManager(
+            note_id=note_id, session=session, client=client
+        )
+        self.favorite = FavoriteManager(note_id=note_id, session=session, client=client)
+        self.poll: PollManager = PollManager(note_id=note_id, session=session, client=client)
 
     @property
-    def action(self) -> FolderActions:
-        """
-        フォルダーの操作を行うインスタンスを返します
-
-        Returns
-        -------
-        FolderActions
-            フォルダーに対するアクション
-        """
-        return FolderActions(
-            folder_id=self.__folder_id, session=self.__session, client=self.__client,
+    def action(self) -> ClientNoteActions:
+        return ClientNoteActions(
+            note_id=self.__note_id, session=self.__session, client=self.__client,
         )
 
-    def _get_file_instance(self, file_id: str) -> FileManager:
-        return FileManager(file_id=file_id, session=self.__session, client=self.__client)
 
+class NoteManager(AbstractManager):
+    """User behavior for notes"""
 
-class DriveManager(AbstractManager):
-    def __init__(self, *, session: HTTPClient, client: ClientManager):
+    def __init__(self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager):
+        self.__note_id: str | None = note_id
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
-        self.folder: FolderManager = FolderManager(session=session, client=client)
-        self.file: FileManager = FileManager(session=session, client=client)
+        self.reaction: ReactionManager = ReactionManager(
+            note_id=note_id, session=session, client=client
+        )
+        self.favorite = FavoriteManager(note_id=note_id, session=session, client=client)
+        self._client: ClientNoteManager = ClientNoteManager(
+            note_id=note_id, session=session, client=client
+        )
+        self.poll: PollManager = PollManager(note_id=note_id, session=session, client=client)
+
+    def create_client_note_manager(self, note_id: str) -> ClientNoteManager:
+        return ClientNoteManager(note_id=note_id, session=self.__session, client=self.__client)
 
     @property
-    def action(self) -> DriveActions:
-        """
-        ドライブの操作を行うインスタンスを返します
-
-        Returns
-        -------
-        DriveActions
-            ドライブに対するアクション
-        """
-        return DriveActions(client=self.__client, session=self.__session)
+    def action(self) -> NoteActions:
+        return NoteActions(note_id=self.__note_id, session=self.__session, client=self.__client,)
 
-    def _get_folder_instance(self, folder_id: str) -> FolderManager:
-        return FolderManager(session=self.__session, client=self.__client, folder_id=folder_id)
+    async def get(
+        self,
+        local: bool = True,
+        reply: bool = False,
+        renote: bool = True,
+        with_files: bool = False,
+        poll: bool = True,
+        limit: int = 10,
+        since_id: str | None = None,
+        until_id: str | None = None,
+    ):
+        data = {
+            'local': local,
+            'reply': reply,
+            'renote': renote,
+            'withFiles': with_files,
+            'poll': poll,
+            'limit': limit,
+            'sinceId': since_id,
+            'untilId': until_id,
+        }
+        await self.__session.request(Route('POST', '/api/notes'), json=data, auth=True, lower=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mipac-0.4.2/mipac/manager/favorite.py` & `mipac-0.4.3/mipac/manager/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/federation.py` & `mipac-0.4.3/mipac/manager/federation.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/follow.py` & `mipac-0.4.3/mipac/manager/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/mute.py` & `mipac-0.4.3/mipac/manager/channel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
-from mipac.actions.mute import MuteActions
+from mipac.actions.channel import ChannelActions
 from mipac.http import HTTPClient
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
-class MuteManager(AbstractManager):
+class ChannelManager(AbstractManager):
     def __init__(
-        self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager
-    ) -> None:
-        self._user_id: str | None = user_id
-        self._session: HTTPClient = session
-        self._client: ClientManager = client
+        self, channel_id: str | None = None, *, session: HTTPClient, client: ClientManager
+    ):
+        self.__channel_id: str | None = channel_id
+        self.__session: HTTPClient = session
+        self.__client: ClientManager = client
 
     @property
-    def action(self) -> MuteActions:
-        return MuteActions(user_id=self._user_id, session=self._session, client=self._client)
+    def action(self) -> ChannelActions:
+        return ChannelActions(
+            channel_id=self.__channel_id, session=self.__session, client=self.__client
+        )
```

### Comparing `mipac-0.4.2/mipac/manager/my.py` & `mipac-0.4.3/mipac/manager/my.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/note.py` & `mipac-0.4.3/mipac/actions/channel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,73 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal, overload
 
-from mipac.abstract.manager import AbstractManager
-from mipac.actions.note import ClientNoteActions, NoteActions
+from mipac.abstract.action import AbstractAction
 from mipac.http import HTTPClient, Route
-from mipac.manager.favorite import FavoriteManager
-from mipac.manager.poll import PollManager
-from mipac.manager.reaction import ReactionManager
+from mipac.models.channel import Channel
+from mipac.models.lite.channel import ChannelLite
+from mipac.types.channel import IChannel, IChannelLite
 
 if TYPE_CHECKING:
-    from mipac.manager.client import ClientManager
+    from mipac.client import ClientManager
 
 
-class ClientNoteManager(AbstractManager):
-    def __init__(self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager):
-        self.__note_id = note_id
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
-        self.reaction: ReactionManager = ReactionManager(
-            note_id=note_id, session=session, client=client
-        )
-        self.favorite = FavoriteManager(note_id=note_id, session=session, client=client)
-        self.poll: PollManager = PollManager(note_id=note_id, session=session, client=client)
+class ClientChannelActions(AbstractAction):
+    def __init__(
+        self, channel_id: str | None = None, *, session: HTTPClient, client: ClientManager
+    ):
+        self._channel_id: str | None = channel_id
+        self._session: HTTPClient = session
+        self._client: ClientManager = client
+
+    async def favorite(self, channel_id: str | None = None):
+        if self._client._config.use_version < 13:
+            raise Exception()
+
+        channel_id = self._channel_id or channel_id
+        if channel_id is None:
+            raise Exception()
 
-    @property
-    def action(self) -> ClientNoteActions:
-        return ClientNoteActions(
-            note_id=self.__note_id, session=self.__session, client=self.__client,
+        res: bool = await self._session.request(
+            Route('POST', '/api/channels/favorite'), auth=True, json={'channelId': channel_id}
         )
 
+        return res
 
-class NoteManager(AbstractManager):
-    """User behavior for notes"""
+    async def unfavorite(self, channel_id: str | None = None):
 
-    def __init__(self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager):
-        self.__note_id: str | None = note_id
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
-        self.reaction: ReactionManager = ReactionManager(
-            note_id=note_id, session=session, client=client
-        )
-        self.favorite = FavoriteManager(note_id=note_id, session=session, client=client)
-        self._client: ClientNoteManager = ClientNoteManager(
-            note_id=note_id, session=session, client=client
+        if self._client._config.use_version < 13:
+            raise Exception()
+
+        channel_id = self._channel_id or channel_id
+        if channel_id is None:
+            raise Exception()
+
+        res: bool = await self._session.request(
+            Route('POST', '/api/channels/unfavorite'), auth=True, json={'channelId': channel_id}
         )
-        self.poll: PollManager = PollManager(note_id=note_id, session=session, client=client)
 
-    def create_client_note_manager(self, note_id: str) -> ClientNoteManager:
-        return ClientNoteManager(note_id=note_id, session=self.__session, client=self.__client)
+        return res
 
-    @property
-    def action(self) -> NoteActions:
-        return NoteActions(note_id=self.__note_id, session=self.__session, client=self.__client,)
-
-    async def get(
-        self,
-        local: bool = True,
-        reply: bool = False,
-        renote: bool = True,
-        with_files: bool = False,
-        poll: bool = True,
-        limit: int = 10,
-        since_id: str | None = None,
-        until_id: str | None = None,
+
+class ChannelActions(ClientChannelActions):
+    def __init__(
+        self, channel_id: str | None = None, *, session: HTTPClient, client: ClientManager
     ):
-        data = {
-            'local': local,
-            'reply': reply,
-            'renote': renote,
-            'withFiles': with_files,
-            'poll': poll,
-            'limit': limit,
-            'sinceId': since_id,
-            'untilId': until_id,
-        }
-        await self.__session.request(Route('POST', '/api/notes'), json=data, auth=True, lower=True)
+        super().__init__(channel_id=channel_id, session=session, client=client)
+
+    async def get_my_favorite(self) -> list[Channel]:
+        """お気に入りに登録したチャンネルの一覧を取得します。
+
+        Returns
+        -------
+        Channel
+            チャンネル
+        """
+        if self._client._config.use_version < 13:
+            raise Exception()
+
+        res: list[IChannel] = await self._session.request(
+            Route('POST', '/api/channels/my-favorites'), auth=True
+        )
+        return [Channel(i, client=self._client) for i in res]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mipac-0.4.2/mipac/manager/page.py` & `mipac-0.4.3/mipac/manager/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/poll.py` & `mipac-0.4.3/mipac/manager/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/reaction.py` & `mipac-0.4.3/mipac/manager/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/manager/user.py` & `mipac-0.4.3/mipac/manager/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/ad.py` & `mipac-0.4.3/mipac/models/ad.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
 from mipac.types.ads import IAd
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.admins.ad import AdminAdvertisingModelManager
     from mipac.manager.client import ClientManager
 
 
 class Ad:
```

### Comparing `mipac-0.4.2/mipac/models/admin.py` & `mipac-0.4.3/mipac/models/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     IServerInfo,
     IServerInfoCpu,
     IServerInfoFs,
     IServerInfoMem,
     IServerInfoNet,
     IUserIP,
 )
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class UserIP:
     def __init__(self, user_ip: IUserIP) -> None:
```

### Comparing `mipac-0.4.2/mipac/models/announcement.py` & `mipac-0.4.3/mipac/models/announcement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from mipac.types.announcement import IAnnouncement, IAnnouncementCommon, IAnnouncementSystem
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.actions.admins.announcement import AdminAnnouncementClientActions
     from mipac.manager.client import ClientManager
 
 T = TypeVar('T', bound=IAnnouncementCommon)
```

### Comparing `mipac-0.4.2/mipac/models/chart.py` & `mipac-0.4.3/mipac/models/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/chat.py` & `mipac-0.4.3/mipac/models/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/drive.py` & `mipac-0.4.3/mipac/models/drive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
+    from mipac.manager.drive import ClientFileManager, ClientFolderManager
     from mipac.types import FolderPayload, IDriveFile, IFileProperties
 
 __all__ = ['FileProperties', 'File', 'Folder']
 
 
 class FileProperties:
     def __init__(self, properties: IFileProperties) -> None:
@@ -60,14 +61,18 @@
     def parent_id(self) -> str:
         return self.__folder['parent_id']
 
     @property
     def parent(self) -> dict[str, Any]:
         return self.__folder['parent']
 
+    @property
+    def api(self) -> ClientFolderManager:
+        return self.__client.drive._get_client_folder_instance(folder_id=self.id)
+
 
 class File:
     def __init__(self, file: IDriveFile, *, client: ClientManager):
         self.__file: IDriveFile = file
         self.__client: ClientManager = client
 
     @property
@@ -109,7 +114,11 @@
     @property
     def blurhash(self) -> str:
         return self.__file['blurhash']
 
     @property
     def properties(self) -> FileProperties:
         return FileProperties(self.__file['properties'])
+
+    @property
+    def api(self) -> ClientFileManager:
+        return self.__client.drive._get_client_file_instance(file_id=self.id)
```

### Comparing `mipac-0.4.2/mipac/models/emoji.py` & `mipac-0.4.3/mipac/models/emoji.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,11 @@
     @property
     def category(self) -> str:
         return self.__emoji['category']
 
     @property
     def license(self) -> str | None:
         return self.__emoji['license']
+
+    @property
+    def host(self) -> str | None:
+        return self.__emoji['host']
```

### Comparing `mipac-0.4.2/mipac/models/follow.py` & `mipac-0.4.3/mipac/models/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/instance.py` & `mipac-0.4.3/mipac/models/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/lite/channel.py` & `mipac-0.4.3/mipac/models/lite/channel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from mipac.types.channel import IChannelLite
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager import ClientManager
+    from mipac.manager.channel import ChannelManager
+
 
 T = TypeVar('T', bound=IChannelLite)
 
 
 class ChannelLite(Generic[T]):
     def __init__(self, channel: T, *, client: ClientManager) -> None:
         self._channel: T = channel
@@ -35,25 +37,29 @@
         return self._channel['name']
 
     @property
     def description(self) -> str | None:
         return self._channel['description']
 
     @property
-    def banner_url(self) -> str | None:
-        return self._channel['banner_url']
+    def user_id(self) -> str:
+        return self._channel['user_id']
 
     @property
-    def notes_count(self) -> int:
-        return self._channel['notes_count']
+    def banner_url(self) -> str | None:
+        return self._channel['banner_url']
 
     @property
     def users_count(self) -> int:
         return self._channel['users_count']
 
     @property
-    def is_following(self) -> bool:
-        return bool(self._channel['is_following'])
+    def notes_count(self) -> int:
+        return self._channel['notes_count']
 
     @property
-    def user_id(self) -> str:
-        return self._channel['user_id']
+    def pinned_note_ids(self) -> list:
+        return self._channel.get('pinned_note_ids', [])
+
+    @property
+    def api(self) -> ChannelManager:
+        return self.__client._create_channel_instance(channel_id=self.id)
```

### Comparing `mipac-0.4.2/mipac/models/lite/emoji.py` & `mipac-0.4.3/mipac/models/lite/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/lite/instance.py` & `mipac-0.4.3/mipac/models/lite/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/lite/meta.py` & `mipac-0.4.3/mipac/models/lite/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/lite/user.py` & `mipac-0.4.3/mipac/models/lite/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal
 
 from mipac.models.lite.instance import LiteInstance
 from mipac.types.emoji import ICustomEmojiLite
 from mipac.types.user import ILiteUser
-from mipac.util import deprecated
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
     from mipac.manager.user import UserManager
 
 
 class LiteUser:
@@ -28,19 +27,14 @@
         return self.__user['username']
 
     @property
     def host(self) -> str | None:
         return self.__user['host'] if 'host' in self.__user else None
 
     @property
-    @deprecated
-    def name(self) -> str:
-        return self.__user['name']
-
-    @property
     def nickname(self) -> str:
         return self.__user['name']
 
     @property
     def online_status(self,) -> Literal['online', 'active', 'offline', 'unknown']:
         return self.__user['online_status']
```

### Comparing `mipac-0.4.2/mipac/models/meta.py` & `mipac-0.4.3/mipac/models/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/mute.py` & `mipac-0.4.3/mipac/models/mute.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/note.py` & `mipac-0.4.3/mipac/models/note.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import TYPE_CHECKING, Literal, Optional
+from typing import TYPE_CHECKING, Optional, Self
 
 from mipac.errors.base import NotExistRequiredData
+from mipac.models.lite.note import PartialNote
 from mipac.models.lite.user import LiteUser
 from mipac.models.poll import Poll
-from mipac.types.note import INoteState, INoteTranslateResult, INoteUpdated, INoteUpdatedDelete
-from mipac.util import str_to_datetime
+from mipac.types.note import (
+    INote,
+    INoteReaction,
+    INoteState,
+    INoteTranslateResult,
+    INoteUpdated,
+    INoteUpdatedDelete,
+)
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
-    from mipac.manager.note import ClientNoteManager
     from mipac.models.user import UserDetailed
-    from mipac.types.drive import IDriveFile
     from mipac.types.emoji import ICustomEmojiLite
-    from mipac.types.note import INote, INoteReaction
 
 __all__ = (
     'NoteState',
     'Note',
     'Follow',
     'Header',
     'NoteReaction',
@@ -132,182 +137,83 @@
         return self.__reaction['type']
 
     @property
     def user(self) -> LiteUser:
         return LiteUser(self.__reaction['user'], client=self.__client)
 
 
-class Note:
+class Note(PartialNote[INote]):
     """
     Noteモデル
 
     Parameters
     ----------
     note: INote
         アクションを持たないNoteクラス
     client: ClientManager
     """
 
     def __init__(self, note: INote, client: ClientManager):
-        self.__note = note
-        self._client: ClientManager = client
-
-    @property
-    def id(self) -> str:
-        """
-        ユーザーのID
-
-        Returns
-        -------
-        str
-            ユーザーのID
-        """
-        return self.__note['id']
-
-    @property
-    def created_at(self) -> datetime:
-        return str_to_datetime(self.__note['created_at'])
-
-    @property
-    def content(self) -> str | None:
-        return self.__note.get('text')
-
-    @property
-    def cw(self) -> str | None:
-        return self.__note.get('cw')
-
-    @property
-    def user_id(self) -> str:
-        return self.__note['user_id']
-
-    @property
-    def author(self) -> LiteUser:
-        return LiteUser(self.__note['user'], client=self._client)
-
-    @property
-    def reply_id(self) -> str:
-        return self.__note['reply_id']
-
-    @property
-    def renote_id(self) -> str:
-        return self.__note['renote_id']
-
-    @property
-    def files(self) -> list[IDriveFile]:  # TODO: モデルに
-        return self.__note['files']
-
-    @property
-    def file_ids(self) -> list[str]:
-        return self.__note['file_ids']
-
-    @property
-    def visibility(self,) -> Literal['public', 'home', 'followers', 'specified']:
-        return self.__note['visibility']
-
-    @property
-    def reaction_acceptance(self) -> Literal['likeOnly', 'likeOnlyForRemote'] | None:
-        """リアクションを受け入れ
-
-        Returns
-        -------
-        Literal['likeOnly', 'likeOnlyForRemote'] | None
-        """
-        return self.__note.get('reaction_acceptance')
-
-    @property
-    def reaction_emojis(self) -> dict[str, str] | None:
-        """リアクション一覧です
-
-        Returns
-        -------
-        dict[str, str] | None
-            リアクション名がキー、値はリアクション画像のリンクです
-        """
-        return self.__note.get('reaction_emojis')
-
-    @property
-    def reactions(self) -> dict[str, int]:
-        return self.__note['reactions']
-
-    @property
-    def renote_count(self) -> int:
-        return self.__note['renote_count']
-
-    @property
-    def replies_count(self) -> int:
-        return self.__note['replies_count']
+        super().__init__(note_data=note, client=client)
 
     @property
     def emojis(self) -> list[ICustomEmojiLite]:  # TODO: モデルに
         """
         Note text contains a list of emojis
         Note: emojis have been abolished since misskey v13
 
         Returns
         -------
         list[ICustomEmojiLite]
             List of emojis contained in note text
         """
 
-        return self.__note.get('emojis', [])
+        return self._note.get('emojis', [])
 
     @property
-    def renote(self) -> 'Note' | None:
+    def renote(self) -> Self | None:
         return (
-            Note(note=self.__note['renote'], client=self._client)
-            if 'renote' in self.__note
+            Note(note=self._note['renote'], client=self._client)
+            if 'renote' in self._note
             else None
         )
 
     @property
-    def reply(self) -> 'Note' | None:
+    def reply(self) -> Self | None:
         return (
-            Note(note=self.__note['reply'], client=self._client)
-            if 'reply' in self.__note
-            else None
+            Note(note=self._note['reply'], client=self._client) if 'reply' in self._note else None
         )
 
     @property
     def visible_user_ids(self) -> list[str]:
-        return self.__note['visible_user_ids'] if 'visible_user_ids' in self.__note else []
+        return self._note['visible_user_ids'] if 'visible_user_ids' in self._note else []
 
     @property
     def local_only(self) -> bool:
-        return self.__note['local_only'] if 'local_only' in self.__note else False
+        return self._note['local_only'] if 'local_only' in self._note else False
 
     @property
     def my_reaction(self) -> str | None:
-        return self.__note['my_reaction'] if 'my_reaction' in self.__note else None
+        return self._note['my_reaction'] if 'my_reaction' in self._note else None
 
     @property
     def uri(self) -> str | None:
-        return self.__note['uri'] if 'uri' in self.__note else None
+        return self._note['uri'] if 'uri' in self._note else None
 
     @property
     def url(self) -> str | None:
-        return self.__note['url'] if 'url' in self.__note else None
+        return self._note['url'] if 'url' in self._note else None
 
     @property
     def is_hidden(self) -> bool:
-        return self.__note['is_hidden'] if 'is_hidden' in self.__note else False
+        return self._note['is_hidden'] if 'is_hidden' in self._note else False
 
     @property
     def poll(self) -> Poll | None:
-        return Poll(self.__note['poll'], client=self._client) if 'poll' in self.__note else None
-
-    @property
-    def api(self) -> ClientNoteManager:
-        """
-        ノートに対するアクション
-
-        Returns
-        -------
-        NoteActions
-        """
-        return self._client.note.create_client_note_manager(self.id)
+        return Poll(self._note['poll'], client=self._client) if 'poll' in self._note else None
 
 
 class NoteTranslateResult:
     """
     NoteTranslateResult
 
     Parameters
```

### Comparing `mipac-0.4.2/mipac/models/notification.py` & `mipac-0.4.3/mipac/models/notification.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/poll.py` & `mipac-0.4.3/mipac/models/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/models/roles.py` & `mipac-0.4.3/mipac/models/roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from mipac.models.lite.user import LiteUser
 from mipac.types.roles import IRole, IRolePolicies, IRolePolicieValue, IRoleUser
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.admins.roles import AdminRolesModelManager
     from mipac.manager.client import ClientManager
     from mipac.manager.user import UserManager
```

### Comparing `mipac-0.4.2/mipac/models/user.py` & `mipac-0.4.3/mipac/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mipac.types.user import (
     IAchievement,
     IBlockingUser,
     IFollowRequest,
     IUserDetailed,
     IUserDetailedField,
 )
-from mipac.util import str_to_datetime
+from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 __all__ = ('UserDetailed', 'FollowRequest', 'LiteUser', 'Achievement', 'BlockingUser')
```

### Comparing `mipac-0.4.2/mipac/types/achievement.py` & `mipac-0.4.3/mipac/types/achievement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/admin.py` & `mipac-0.4.3/mipac/types/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/chart.py` & `mipac-0.4.3/mipac/types/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/chat.py` & `mipac-0.4.3/mipac/types/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/drive.py` & `mipac-0.4.3/mipac/types/drive.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/emoji.py` & `mipac-0.4.3/mipac/types/emoji.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     url: str
 
 
 class ICustomEmoji(ICustomEmojiLite):
     id: str
     category: str
     aliases: list[str]
+    host: str | None
     license: str | None  # v13 only
 
 
 class EmojiPayload(TypedDict):
     id: str | None
     aliases: Optional[list[str]]
     name: str | None
```

### Comparing `mipac-0.4.2/mipac/types/endpoints.py` & `mipac-0.4.3/mipac/types/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     '/api/admin/get-table-stats',
     '/api/admin/get-user-ips',
     '/api/invite',
     '/api/admin/promo/create',
     '/api/admin/queue/clear',
     '/api/admin/queue/deliver-delayed',
     '/api/admin/queue/inbox-delayed',
+    '/api/admin/queue/promote',
     '/api/admin/queue/stats',
     '/api/admin/relays/add',
     '/api/admin/relays/list',
     '/api/admin/relays/remove',
     '/api/admin/reset-password',
     '/api/admin/resolve-abuse-user-report',
     '/api/admin/send-email',
@@ -190,14 +191,15 @@
     '/api/i/webhooks/create',
     '/api/i/webhooks/list',
     '/api/i/webhooks/show',
     '/api/i/webhooks/update',
     '/api/i/webhooks/delete',
     '/api/meta',
     '/api/emojis',
+    '/api/emoji',
     '/api/mute/create',
     '/api/mute/delete',
     '/api/mute/list',
     '/api/renote-mute/create',
     '/api/renote-mute/delete',
     '/api/renote-mute/list',
     '/api/my/apps',
@@ -345,9 +347,17 @@
     '/api/users/groups/invite',
     '/api/users/groups/joined',
     '/api/users/groups/owned',
     '/api/users/groups/pull',
     '/api/users/groups/show',
     '/api/users/groups/transfer',
     '/api/users/groups/update',
-    '/api/version'
+    '/api/version',
+    '/api/admin/queue/promote',
+    '/api/channels/favorite',
+    '/api/channels/unfavorite',
+    '/api/channels/my-favorites',
+    '/api/channels/search',
+    '/api/emoji',
+    '/api/roles/notes',
+    '/api/users/update-memo',
 ]
```

### Comparing `mipac-0.4.2/mipac/types/instance.py` & `mipac-0.4.3/mipac/types/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/meta.py` & `mipac-0.4.3/mipac/types/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/note.py` & `mipac-0.4.3/mipac/types/note.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,48 +50,49 @@
     altitude: int | None
     accuracy: int | None
     altitude_accuracy: int | None
     heading: int | None
     speed: int | None
 
 
-class INoteRequired(TypedDict):
-    id: str
+class IPartialNote(TypedDict):
     created_at: str
-    text: str | None
     cw: str | None
-    user: ILiteUser
-    user_id: str
-    reply_id: str
-    renote_id: str
-    files: list[IDriveFile]
     file_ids: list[str]
-    visibility: Literal['public', 'home', 'followers', 'specified']
-    reactions: dict[str, int]
+    files: list[IDriveFile]
+    id: str
+    reaction_acceptance: NotRequired[Literal['likeOnly', 'likeOnlyForRemote']]  # v13 only
+    reaction_emojis: NotRequired[dict[str, str]]  # v13 only
+    renote_id: str | None
     renote_count: int
+    reactions: dict[str, int]
     replies_count: int
+    reply_id: str | None
+    text: str | None
+    user: ILiteUser
+    user_id: str
+    visibility: Literal['public', 'home', 'followers', 'specified']
+    tags: NotRequired[list[str]]  # タグがついてないとbodyに存在しない
 
 
-class INote(INoteRequired, total=False):
+class INote(IPartialNote, total=False):
     """
     note object
     """
 
     renote: 'INote'
     reply: 'INote'
     visible_user_ids: list[str]
     local_only: bool
     my_reaction: str
     uri: str
     url: str
     is_hidden: bool
     poll: IPoll
     emojis: list[ICustomEmojiLite]
-    reaction_emojis: dict[str, str]
-    reaction_acceptance: Literal['likeOnly', 'likeOnlyForRemote'] | None
 
 
 class ICreatedNote(TypedDict):
     """
     created note
     """
```

### Comparing `mipac-0.4.2/mipac/types/notification.py` & `mipac-0.4.3/mipac/types/notification.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/page.py` & `mipac-0.4.3/mipac/types/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/roles.py` & `mipac-0.4.3/mipac/types/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/types/user.py` & `mipac-0.4.3/mipac/types/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.2/mipac/util.py` & `mipac-0.4.3/mipac/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import warnings
 from datetime import datetime, timedelta
 from typing import Any, Mapping, Optional
 from urllib.parse import urlencode
 
 import aiohttp
 
+from mipac.utils.util import deprecated as new_deprecated
+
 try:
     import orjson  # type: ignore
 except ModuleNotFoundError:
     HAS_ORJSON = False
 else:
     HAS_ORJSON = True
 
@@ -45,34 +47,59 @@
 else:
     _from_json = json.loads
 
 DEFAULT_CACHE: dict[str, list[str]] = {}
 DEFAULT_CACHE_VALUE: dict[str, Any] = {}
 
 
+@new_deprecated
+def deprecated(func):
+    """
+    This is a decorator which can be used to mark functions
+    as deprecated. It will result in a warning being emitted
+    when the function is used.
+    """
+
+    @functools.wraps(func)
+    def new_func(*args, **kwargs):
+        warnings.simplefilter('always', DeprecationWarning)  # turn off filter
+        warnings.warn(
+            'Call to deprecated function {}.'.format(func.__name__),
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        warnings.simplefilter('default', DeprecationWarning)  # reset filter
+        return func(*args, **kwargs)
+
+    return new_func
+
+
+@new_deprecated
 def snake_to_camel(snake_str: str, replace_list: dict[str, str]) -> str:
     components: list[str] = snake_str.split('_')
     for i in range(len(components)):
         if components[i] in replace_list:
             components[i] = replace_list[components[i]]
     return components[0] + ''.join(x.title() for x in components[1:])
 
 
+@new_deprecated
 def convert_dict_keys_to_camel(
     data: Mapping[Any, Any], replace_list: dict[str, str] | None = None
 ) -> Mapping[Any, Any]:
     if replace_list is None:
         replace_list = {}
     new_dict = {}
     for key, value in data.items():
         new_key = snake_to_camel(key, replace_list)
         new_dict[new_key] = value
     return new_dict
 
 
+@new_deprecated
 def str_to_datetime(data: str, format: str = '%Y-%m-%dT%H:%M:%S.%fZ') -> datetime:
     """
     Parameters
     ----------
     data : str
         datetimeに変更したい文字列
     format : str
@@ -82,41 +109,22 @@
     -------
     datetime
         変換後のデータ
     """
     return datetime.strptime(data, format)
 
 
-def deprecated(func):
-    """
-    This is a decorator which can be used to mark functions
-    as deprecated. It will result in a warning being emitted
-    when the function is used.
-    """
-
-    @functools.wraps(func)
-    def new_func(*args, **kwargs):
-        warnings.simplefilter('always', DeprecationWarning)  # turn off filter
-        warnings.warn(
-            'Call to deprecated function {}.'.format(func.__name__),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-        warnings.simplefilter('default', DeprecationWarning)  # reset filter
-        return func(*args, **kwargs)
-
-    return new_func
-
-
+@new_deprecated
 class MiTime:
     def __init__(self, start: timedelta, end: datetime):
         self.start = start
         self.end = end
 
 
+@new_deprecated
 class AuthClient:
     """
     Tokenの取得を手助けするクラス
     """
 
     def __init__(
         self,
@@ -221,25 +229,27 @@
             data = await self.wait_miauth()
         else:
             data = await self.wait_oldauth()
         await self.__client_session.close()
         return data['token'] if self.__use_miauth else data['accessToken']
 
 
+@new_deprecated
 def set_cache(group: str, key: str, value: Any):
     if len(DEFAULT_CACHE.get(group, [])) > 50:
         del DEFAULT_CACHE[group][-1]
         del DEFAULT_CACHE_VALUE[key]
 
     if DEFAULT_CACHE.get(group) is None:
         DEFAULT_CACHE[group] = []
     DEFAULT_CACHE[group].append(key)
     DEFAULT_CACHE_VALUE[key] = value
 
 
+@new_deprecated
 def cache(group: str = 'default', override: bool = False):
     def decorator(func):
         async def wrapper(self, *args, **kwargs):
             ordered_kwargs = sorted(kwargs.items())
             key = '.{0}' + str(args) + str(ordered_kwargs)
             hit_item = DEFAULT_CACHE_VALUE.get(key)
             if hit_item and override is False and kwargs.get('cache_override') is None:
@@ -249,31 +259,34 @@
             return res
 
         return wrapper
 
     return decorator
 
 
+@new_deprecated
 def get_cache_key(func):
     async def decorator(self, *args, **kwargs):
         ordered_kwargs = sorted(kwargs.items())
         key = (func.__module__ or '') + '.{0}' + f'{self}' + str(args) + str(ordered_kwargs)
         return await func(self, *args, **kwargs, cache_key=key)
 
     return decorator
 
 
+@new_deprecated
 def key_builder(func, cls, *args, **kwargs):
     ordered_kwargs = sorted(kwargs.items())
     key = (
         (func.__module__ or '') + f'.{func.__name__}' + f'{cls}' + str(args) + str(ordered_kwargs)
     )
     return key
 
 
+@new_deprecated
 def check_multi_arg(*args: Any) -> bool:
     """
     複数の値を受け取り値が存在するかをboolで返します
 
     Parameters
     ----------
     args : list
@@ -283,14 +296,15 @@
     -------
     bool
         存在する場合はTrue, 存在しない場合はFalse
     """
     return bool([i for i in args if i])
 
 
+@new_deprecated
 def remove_list_empty(data: list[Any]) -> list[Any]:
     """
     Parameters
     ----------
     data: dict
         空のkeyを削除したいdict
 
@@ -298,14 +312,15 @@
     -------
     dict[str, Any]
         空のkeyがなくなったdict
     """
     return [k for k in data if k]
 
 
+@new_deprecated
 def remove_dict_empty(data: dict[str, Any]) -> dict[str, Any]:
     """
     Parameters
     ----------
     data: dict
         空のkeyを削除したいdict
 
@@ -315,14 +330,15 @@
         空のkeyがなくなったdict
     """
     _data = {}
     _data = {k: v for k, v in data.items() if v is not None}
     return _data
 
 
+@new_deprecated
 def upper_to_lower(
     data: dict[str, Any],
     field: Optional[dict[str, Any]] = None,
     nest: bool = True,
     replace_list: Optional[dict[str, Any]] = None,
 ) -> dict[str, Any]:
     """
@@ -364,23 +380,25 @@
         elif isinstance(field[default_key], list) and nest:
             field[default_key] = [
                 upper_to_lower(i) if isinstance(i, dict) else i for i in field[default_key]
             ]
     return field
 
 
+@new_deprecated
 def str_lower(text: str):
     pattern = re.compile('[A-Z]')
     large = [i.group().lower() for i in pattern.finditer(text)]
     result = [None] * (len(large + pattern.split(text)))
     result[::2] = pattern.split(text)
     result[1::2] = ['_' + i.lower() for i in large]
     return ''.join(result)
 
 
+@new_deprecated
 def bool_to_string(boolean: bool) -> str:
     """
     boolを小文字にして文字列として返します
 
     Parameters
     ----------
     boolean : bool
```

### Comparing `mipac-0.4.2/mipac.egg-info/SOURCES.txt` & `mipac-0.4.3/mipac.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 mipac.egg-info/top_level.txt
 mipac/abstract/__init__.py
 mipac/abstract/action.py
 mipac/abstract/manager.py
 mipac/abstract/model.py
 mipac/actions/__init__.py
 mipac/actions/blocking.py
+mipac/actions/channel.py
 mipac/actions/chart.py
 mipac/actions/chat.py
 mipac/actions/client.py
 mipac/actions/drive.py
+mipac/actions/emoji.py
 mipac/actions/favorite.py
 mipac/actions/federation.py
 mipac/actions/follow.py
 mipac/actions/mute.py
 mipac/actions/my.py
 mipac/actions/note.py
 mipac/actions/poll.py
@@ -46,18 +48,20 @@
 mipac/actions/admins/roles.py
 mipac/actions/admins/user.py
 mipac/errors/__init__.py
 mipac/errors/base.py
 mipac/errors/errors.py
 mipac/manager/__init__.py
 mipac/manager/blocking.py
+mipac/manager/channel.py
 mipac/manager/chart.py
 mipac/manager/chat.py
 mipac/manager/client.py
 mipac/manager/drive.py
+mipac/manager/emoji.py
 mipac/manager/favorite.py
 mipac/manager/federation.py
 mipac/manager/follow.py
 mipac/manager/mute.py
 mipac/manager/my.py
 mipac/manager/note.py
 mipac/manager/page.py
@@ -92,14 +96,15 @@
 mipac/models/roles.py
 mipac/models/user.py
 mipac/models/lite/__init__.py
 mipac/models/lite/channel.py
 mipac/models/lite/emoji.py
 mipac/models/lite/instance.py
 mipac/models/lite/meta.py
+mipac/models/lite/note.py
 mipac/models/lite/user.py
 mipac/types/__init__.py
 mipac/types/achievement.py
 mipac/types/admin.py
 mipac/types/ads.py
 mipac/types/announcement.py
 mipac/types/channel.py
@@ -114,8 +119,14 @@
 mipac/types/mute.py
 mipac/types/note.py
 mipac/types/notification.py
 mipac/types/page.py
 mipac/types/poll.py
 mipac/types/reaction.py
 mipac/types/roles.py
-mipac/types/user.py
+mipac/types/user.py
+mipac/utils/__init__.py
+mipac/utils/auth.py
+mipac/utils/cache.py
+mipac/utils/format.py
+mipac/utils/log.py
+mipac/utils/util.py
```

### Comparing `mipac-0.4.2/setup.py` & `mipac-0.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     'mipac.actions.admins',
     'mipac.errors',
     'mipac.manager',
     'mipac.manager.admins',
     'mipac.models',
     'mipac.types',
     'mipac.models.lite',
+    'mipac.utils'
 ]
 
 setup(
     name='mipac',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     install_requires=requirements,
```

### Comparing `mipac-0.4.2/versioneer.py` & `mipac-0.4.3/versioneer.py`

 * *Files identical despite different names*

