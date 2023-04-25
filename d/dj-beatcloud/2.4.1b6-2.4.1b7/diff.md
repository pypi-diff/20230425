# Comparing `tmp/dj_beatcloud-2.4.1b6.tar.gz` & `tmp/dj_beatcloud-2.4.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b6.tar", last modified: Mon Apr 24 19:51:17 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b7.tar", last modified: Tue Apr 25 02:44:14 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b6.tar` & `dj_beatcloud-2.4.1b7.tar`

### file list

```diff
@@ -1,79 +1,68 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.293552 dj_beatcloud-2.4.1b6/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-24 19:51:17.293658 dj_beatcloud-2.4.1b6/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-24 19:51:17.294093 dj_beatcloud-2.4.1b6/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/setup.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.278750 dj_beatcloud-2.4.1b6/src/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.281256 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.281916 dj_beatcloud-2.4.1b6/src/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/__init__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.285277 dj_beatcloud-2.4.1b6/src/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/.DS_Store
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4641 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/dj_tools.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.285451 dj_beatcloud-2.4.1b6/src/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/src/djtools/logs/empty.txt
--rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b6/src/djtools/main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.287374 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3013 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.288826 dj_beatcloud-2.4.1b6/src/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.290748 dj_beatcloud-2.4.1b6/src/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8185 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4713 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.292988 dj_beatcloud-2.4.1b6/src/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7970 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/url_download.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.293394 dj_beatcloud-2.4.1b6/src/test_data/
--rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/test_data/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/test_data/conftest.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.431740 dj_beatcloud-2.4.1b7/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b7/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 02:22:26.000000 dj_beatcloud-2.4.1b7/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:44:14.431918 dj_beatcloud-2.4.1b7/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28208 2023-04-25 02:22:18.000000 dj_beatcloud-2.4.1b7/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.415862 dj_beatcloud-2.4.1b7/djtools/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.420364 dj_beatcloud-2.4.1b7/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      466 2023-04-25 02:08:56.000000 dj_beatcloud-2.4.1b7/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-25 02:17:53.000000 dj_beatcloud-2.4.1b7/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4653 2023-04-25 02:00:36.000000 dj_beatcloud-2.4.1b7/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.421325 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1827 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       42 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       37 2023-04-25 02:44:14.000000 dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.424773 dj_beatcloud-2.4.1b7/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1292 2023-04-25 02:09:11.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-25 02:18:09.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-25 02:18:14.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-25 02:18:19.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-25 02:18:24.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-25 02:18:32.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1173 2023-04-25 02:34:57.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1353 2023-04-25 01:39:07.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2974 2023-04-25 01:39:31.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5102 2023-04-25 01:39:22.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1437 2023-04-25 01:41:25.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3905 2023-04-25 02:19:02.000000 dj_beatcloud-2.4.1b7/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.426979 dj_beatcloud-2.4.1b7/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      680 2023-04-25 02:09:26.000000 dj_beatcloud-2.4.1b7/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-04-25 02:19:12.000000 dj_beatcloud-2.4.1b7/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-25 02:19:17.000000 dj_beatcloud-2.4.1b7/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-25 02:19:22.000000 dj_beatcloud-2.4.1b7/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17439 2023-04-25 01:59:43.000000 dj_beatcloud-2.4.1b7/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6108 2023-04-25 02:00:00.000000 dj_beatcloud-2.4.1b7/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.428951 dj_beatcloud-2.4.1b7/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      736 2023-04-25 02:09:42.000000 dj_beatcloud-2.4.1b7/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-25 02:19:34.000000 dj_beatcloud-2.4.1b7/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8218 2023-04-25 02:19:45.000000 dj_beatcloud-2.4.1b7/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-25 02:19:55.000000 dj_beatcloud-2.4.1b7/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4010 2023-04-25 02:35:23.000000 dj_beatcloud-2.4.1b7/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8157 2023-04-25 01:59:07.000000 dj_beatcloud-2.4.1b7/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4686 2023-04-25 02:00:54.000000 dj_beatcloud-2.4.1b7/djtools/sync/test_sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:44:14.431507 dj_beatcloud-2.4.1b7/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      795 2023-04-25 02:09:52.000000 dj_beatcloud-2.4.1b7/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-25 02:20:08.000000 dj_beatcloud-2.4.1b7/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-25 02:20:13.000000 dj_beatcloud-2.4.1b7/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9423 2023-04-25 02:33:38.000000 dj_beatcloud-2.4.1b7/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3187 2023-04-25 01:42:11.000000 dj_beatcloud-2.4.1b7/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-04-25 01:37:07.000000 dj_beatcloud-2.4.1b7/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8505 2023-04-25 02:00:22.000000 dj_beatcloud-2.4.1b7/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1540 2023-04-25 02:17:17.000000 dj_beatcloud-2.4.1b7/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 02:20:37.000000 dj_beatcloud-2.4.1b7/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 01:26:32.000000 dj_beatcloud-2.4.1b7/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      148 2023-04-25 02:44:14.432257 dj_beatcloud-2.4.1b7/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-25 02:37:51.000000 dj_beatcloud-2.4.1b7/setup.py
```

### Comparing `dj_beatcloud-2.4.1b6/LICENSE` & `dj_beatcloud-2.4.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/PKG-INFO` & `dj_beatcloud-2.4.1b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b6
+Version: 2.4.1b7
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
@@ -90,15 +90,15 @@
     * automatically generate playlists based on the tags of your Collection
     * emulating a playlist randomization feature which is strangely absent from Rekordbox
 4. `utils`: contains a variety of utilities for things such as:
     * downloading mp3 files from a URL (e.g. Soundcloud)
     * compare the tracks of Spotify playlists and / or local directories against the `beatcloud` (to identify redundancies)
     * copy audio files from a given playlist to a new location and generate a new XML for those files (for backups and ensuring you can play a preparation on non-Pioneer setups)
 
-For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools).
+For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/djtools/).
 
 # Setup
 
 ## Python
 1. The `DJ Tools` library uses f-strings so a minimum version of Python 3.6 is required. As always, when working with a Python project, you're going to want to create a virtual environment; [Pyenv](https://github.com/pyenv/pyenv) is really nice, but if you insist on doing a system-wide python installation then proceed with the following instructions:
     - Mac installation: `brew install python@3.6`
     - Linux installation: `sudo apt install python3.6`
@@ -142,19 +142,19 @@
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --link_configs /path/to/djtools_configs/`
 
 After running this command, base templates for all config files used by `djtools` will be symlinked allowing you to navigate to that directory and open `config.yaml` (and all other config files) with your favorite text editor and configure the library for your needs.
 
 Please be sure to checkout the package-level README files regarding the usage of the other config files which must also be stored in the same location as `config.yaml`:
 * `spotify`
-    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/spotify)
+    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/spotify)
 * `sync`
-    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/sync)
+    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/sync)
 * `rekordbox`
-    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/rekordbox)
+    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/rekordbox)
 
 ## Populating `config.yaml`
 `DJ Tools` contains quite a bit of functionality, but all of it is configurable via `config.yaml`. You may decide to not use `config.yaml` at all and, instead, opt to use the corollary command-line arguments; all configuration options may be overridden via command-line arguments of the same name but in lowercase. Example:
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --download_xml --import_user bob --aws_profile DJ`
```

### Comparing `dj_beatcloud-2.4.1b6/README.md` & `dj_beatcloud-2.4.1b7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     * automatically generate playlists based on the tags of your Collection
     * emulating a playlist randomization feature which is strangely absent from Rekordbox
 4. `utils`: contains a variety of utilities for things such as:
     * downloading mp3 files from a URL (e.g. Soundcloud)
     * compare the tracks of Spotify playlists and / or local directories against the `beatcloud` (to identify redundancies)
     * copy audio files from a given playlist to a new location and generate a new XML for those files (for backups and ensuring you can play a preparation on non-Pioneer setups)
 
-For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools).
+For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/djtools/).
 
 # Setup
 
 ## Python
 1. The `DJ Tools` library uses f-strings so a minimum version of Python 3.6 is required. As always, when working with a Python project, you're going to want to create a virtual environment; [Pyenv](https://github.com/pyenv/pyenv) is really nice, but if you insist on doing a system-wide python installation then proceed with the following instructions:
     - Mac installation: `brew install python@3.6`
     - Linux installation: `sudo apt install python3.6`
@@ -111,19 +111,19 @@
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --link_configs /path/to/djtools_configs/`
 
 After running this command, base templates for all config files used by `djtools` will be symlinked allowing you to navigate to that directory and open `config.yaml` (and all other config files) with your favorite text editor and configure the library for your needs.
 
 Please be sure to checkout the package-level README files regarding the usage of the other config files which must also be stored in the same location as `config.yaml`:
 * `spotify`
-    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/spotify)
+    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/spotify)
 * `sync`
-    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/sync)
+    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/sync)
 * `rekordbox`
-    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/rekordbox)
+    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/rekordbox)
 
 ## Populating `config.yaml`
 `DJ Tools` contains quite a bit of functionality, but all of it is configurable via `config.yaml`. You may decide to not use `config.yaml` at all and, instead, opt to use the corollary command-line arguments; all configuration options may be overridden via command-line arguments of the same name but in lowercase. Example:
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --download_xml --import_user bob --aws_profile DJ`
```

### Comparing `dj_beatcloud-2.4.1b6/setup.py` & `dj_beatcloud-2.4.1b7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,30 +48,30 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b6',
+    version='2.4.1-b7',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
     author='Alex Richards',
     author_email='alex.richards006@gmail.com',
     license='GNU GPLv3',
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    package_dir={"": "djtools"},
+    packages=find_packages(where="djtools"),
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
     extras_require=EXTRAS,
     python_requires=">=3.6",
     include_package_data=True,
     keywords='MP3 Rekordbox XML spotify reddit aws s3',
     entry_points={
-        'console_scripts': ['djtools=djtools:dj_tools.main']
+        'console_scripts': ['djtools=dj_tools.main']
     }
 )
```

### Comparing `dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b7/djtools/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b6
+Version: 2.4.1b7
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
@@ -90,15 +90,15 @@
     * automatically generate playlists based on the tags of your Collection
     * emulating a playlist randomization feature which is strangely absent from Rekordbox
 4. `utils`: contains a variety of utilities for things such as:
     * downloading mp3 files from a URL (e.g. Soundcloud)
     * compare the tracks of Spotify playlists and / or local directories against the `beatcloud` (to identify redundancies)
     * copy audio files from a given playlist to a new location and generate a new XML for those files (for backups and ensuring you can play a preparation on non-Pioneer setups)
 
-For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools).
+For usage details relating to the individual packages of `DJ Tools`, checkout the README files that are [collocated with those packages](https://github.com/a-rich/DJ-Tools/tree/main/djtools/).
 
 # Setup
 
 ## Python
 1. The `DJ Tools` library uses f-strings so a minimum version of Python 3.6 is required. As always, when working with a Python project, you're going to want to create a virtual environment; [Pyenv](https://github.com/pyenv/pyenv) is really nice, but if you insist on doing a system-wide python installation then proceed with the following instructions:
     - Mac installation: `brew install python@3.6`
     - Linux installation: `sudo apt install python3.6`
@@ -142,19 +142,19 @@
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --link_configs /path/to/djtools_configs/`
 
 After running this command, base templates for all config files used by `djtools` will be symlinked allowing you to navigate to that directory and open `config.yaml` (and all other config files) with your favorite text editor and configure the library for your needs.
 
 Please be sure to checkout the package-level README files regarding the usage of the other config files which must also be stored in the same location as `config.yaml`:
 * `spotify`
-    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/spotify)
+    - [spotify_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/spotify)
 * `sync`
-    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/sync)
+    - [registered_users.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/sync)
 * `rekordbox`
-    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/src/djtools/rekordbox)
+    - [rekordbox_playlists.yaml](https://github.com/a-rich/DJ-Tools/tree/main/djtools/rekordbox)
 
 ## Populating `config.yaml`
 `DJ Tools` contains quite a bit of functionality, but all of it is configurable via `config.yaml`. You may decide to not use `config.yaml` at all and, instead, opt to use the corollary command-line arguments; all configuration options may be overridden via command-line arguments of the same name but in lowercase. Example:
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`djtools --download_xml --import_user bob --aws_profile DJ`
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/README.md` & `dj_beatcloud-2.4.1b7/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/config.py` & `dj_beatcloud-2.4.1b7/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b7/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b7/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.4.1b7/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b7/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b7/djtools/configs/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 
 from djtools.configs.config import BaseConfig
 from djtools.configs.helpers import (
     arg_parse, build_config, convert_to_paths, filter_dict, parse_yaml, pkg_cfg
 )
-from test_data import MockOpen
+from djtools.utils.helpers import MockOpen
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs(mock_parse_args, tmpdir):
     config_path = Path(tmpdir) / "test_dir"
     mock_parse_args.return_value = Namespace(
         link_configs=config_path, log_level="INFO"
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         `rekordbox_playlists.yaml`
     * `randomize_playlists`: writes sequential numbers to Rekordbox tags of
         shuffled tracks in playlists to emulate playlist shuffling
     * `tag_parsers`: the `TagParser` abstract base class and its
         implementations used by the `playlist_builder`
 """
 
-from djtools.rekordbox.config import RekordboxConfig
-from djtools.rekordbox.copy_playlists import copy_playlists
-from djtools.rekordbox.playlist_builder import rekordbox_playlists
-from djtools.rekordbox.randomize_playlists import randomize_playlists
+from .config import RekordboxConfig
+from .copy_playlists import copy_playlists
+from .playlist_builder import rekordbox_playlists
+from .randomize_playlists import randomize_playlists
 
 
 REKORDBOX_OPERATIONS = {
     "COPY_PLAYLISTS": copy_playlists,
     "RANDOMIZE_PLAYLISTS": randomize_playlists,
     "REKORDBOX_PLAYLISTS": rekordbox_playlists
 }
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.rekordbox.config import RekordboxConfig
-from test_data import mock_exists
-
-
-pytest_plugins = [
-   "test_data",
-]
+from djtools.utils.helpers import mock_exists
 
 
 def test_rekordboxconfig():
     cfg = {
         "COPY_PLAYLISTS": [],
         "RANDOMIZE_PLAYLISTS": [],
         "REKORDBOX_PLAYLISTS": False,
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_copy_playlists.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.copy_playlists import copy_playlists
 
 
-pytest_plugins = [
- "test_data",
-]
-
-
 def test_copy_playlists(tmpdir, test_config, test_xml):
     target_playlists = ["Hip Hop"]
     test_xml = Path(test_xml)
     new_xml = test_xml.parent / "relocated_rekordbox.xml"
     test_output_dir = Path(tmpdir) / "output"
     test_config.XML_PATH = test_xml
     test_config.COPY_PLAYLISTS = target_playlists
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from djtools.rekordbox.helpers import (
     BooleanNode,
     copy_file,
     get_playlist_track_locations,
     set_tag,
 )
 
-pytest_plugins = [
-    "test_data",
-]
-
 
 @pytest.mark.parametrize(
     "node_attributes",
     [
         (
             [set.intersection, set.union, set.difference],
             ["Jungle", "Breaks", "Techno", "Tech House"],
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 import yaml
 
 from djtools.rekordbox.playlist_builder import (
     PlaylistBuilder, rekordbox_playlists    
 )
 
 
-pytest_plugins = [
-    "test_data",
-]
-
-
 @pytest.mark.parametrize(
     "remainder_type", ["", "folder", "playlist", "invalid"]
 )
 def test_playlistbuilder(remainder_type, test_xml, test_playlist_config):
     playlist_builder = PlaylistBuilder(
         rekordbox_database=Path(test_xml),
         playlist_config=Path(test_playlist_config),
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_randomize_playlists.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.randomize_playlists import randomize_playlists
 
 
-pytest_plugins = [
-    "test_data",
-]
-
-
 def test_randomize_playlists(test_config, test_xml, caplog):
     caplog.set_level("INFO")
     playlists = ["Hip Hop"]
     test_xml = Path(test_xml)
     test_config.XML_PATH = test_xml
     test_config.RANDOMIZE_PLAYLISTS = playlists
     randomize_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b7/djtools/rekordbox/test_tag_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-from bs4 import BeautifulSoup
 import pytest
 import yaml
 
 from djtools.rekordbox.tag_parsers import (
     Combiner, GenreTagParser, MyTagParser, TagParser
 )
 
 
-pytest_plugins = [
-    "test_data",
-]
-
-
 def test_combiner(test_playlist_config, xml, caplog):
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     bad_playlist = "Dark & [-1, 5-7, a-5]"
     selector_playlists = [
         x for x in playlist_config["Combiner"]["playlists"]
         if "[" in x or "{" in x
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """The `spotify` package contains modules:
     * `config`: the configuration object for the `spotify` package
     * `helpers`: helper functions for `playlist_builder`
     * `playlist_builder`: constructs or updates Spotify playlists using either
         Subreddit posts or the Discord webhook output from `UPLOAD_MUSIC`
 """
-from djtools.spotify.config import SpotifyConfig
-from djtools.spotify.playlist_builder import (
-    playlist_from_upload, update_auto_playlists
-)
+from .config import SpotifyConfig
+from .playlist_builder import playlist_from_upload, update_auto_playlists
 
 
 SPOTIFY_OPERATIONS = {
     "PLAYLIST_FROM_UPLOAD": playlist_from_upload,
     "AUTO_PLAYLIST_UPDATE": update_auto_playlists,
 }
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import asyncio
 from unittest import mock
 
-import asyncpraw
 import pytest
-import spotipy
 
 from djtools.spotify.config import SubredditConfig
 from djtools.spotify.helpers import (
     build_new_playlist,
     filter_results,
     filter_tracks,
     fuzzy_match,
@@ -18,20 +16,15 @@
     parse_title,
     populate_playlist,
     process,
     track_name_too_similar,
     update_existing_playlist,
     write_playlist_ids
 )
-from test_data import MockOpen
-
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import MockOpen
 
 
 async def aiter(obj, num_subs):
     for i in range(num_subs):
         yield obj
         await asyncio.sleep(0.1)
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b7/djtools/spotify/test_playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from pathlib import Path
 from unittest import mock
 
-import pyperclip
 import pytest
 
 from djtools.spotify.config import SubredditConfig
 from djtools.spotify.playlist_builder import (
     async_update_auto_playlists,
     playlist_from_upload,
     update_auto_playlists,
 )
-from test_data import MockOpen
-
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "playlist_subreddits", [[], [SubredditConfig(name="jungle").dict()]],
 )
 @pytest.mark.parametrize("got_playlist_ids", [True, False])
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b7/djtools/sync/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """The `sync` package contains modules:
     * `config`: the configuration object for the `sync` package
     * `helpers`: helper functions for the `sync_operations` module
     * `sync_operations`: for syncing audio and Rekordbox XML files to the
         Beatcloud
 """
-from djtools.sync.config import SyncConfig
-from djtools.sync.helpers import upload_log
-from djtools.sync.sync_operations import (
+from .config import SyncConfig
+from .helpers import upload_log
+from .sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
 
 
 SYNC_OPERATIONS = {
     'DOWNLOAD_MUSIC': download_music,
     'DOWNLOAD_XML': download_xml,
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/config.py` & `dj_beatcloud-2.4.1b7/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b7/djtools/sync/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modifying IMPORT_USER's XML to point to tracks located at "USB_PATH".
 """
 from datetime import datetime, timedelta
 from itertools import groupby
 import logging
 from pathlib import Path
 from subprocess import Popen, PIPE, CalledProcessError
-from typing import Dict, List, Optional, Union
+from typing import Optional
 
 from bs4 import BeautifulSoup
 import requests
 import yaml
 
 from djtools.configs.config import BaseConfig
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b7/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b7/djtools/sync/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 from unittest import mock
 
 import getpass
 import pytest
 
 
 from djtools.sync.config import SyncConfig
-from test_data import mock_exists, MockOpen
-
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import mock_exists, MockOpen
 
 
 @mock.patch(
     "builtins.open",
     MockOpen(
         files=["registered_users.yaml"],
         content="bad:\tfile",
@@ -89,22 +84,22 @@
         RuntimeError,
         match="Config must include AWS_PROFILE for sync operations"
     ):
         SyncConfig(**cfg)
 
 
 @mock.patch(
+    "djtools.sync.config.Path.exists",
+    lambda path: mock_exists([("registered_users.yaml", False)], path)
+)
+@mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"],
     write_only=True).open,
 )
-@mock.patch(
-    "djtools.sync.config.Path.exists",
-    lambda path: mock_exists([("registered_users.yaml", False)], path)
-)
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 def test_syncconfig_no_registered_users(
     mock_get_spotify_client, test_xml, caplog
 ):
     cfg = {
         "XML_PATH": test_xml,
         "SPOTIFY_CLIENT_ID": "id",
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b7/djtools/sync/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.sync.helpers import (
     parse_sync_command, rewrite_xml, run_sync, upload_log, webhook
 )
-from test_data import MockOpen
-
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.parametrize("upload", [True, False])
 @pytest.mark.parametrize(
     "include_dirs", [[], ["path/to/stuff", "path/to/things.mp3"]]
 )
 @pytest.mark.parametrize(
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b7/djtools/sync/test_sync_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from unittest import mock
 
 import pytest
 
 from djtools.sync.sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
-from test_data import MockOpen
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.parametrize("playlist_name", ["", "playlist Uploads"])
 @mock.patch(
     "djtools.sync.sync_operations.compare_tracks",
     return_value=(
         ["file.mp3"],
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b7/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/config.py` & `dj_beatcloud-2.4.1b7/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b7/djtools/utils/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,69 @@
 from datetime import datetime
 from itertools import product
 import logging
 import logging.config
 import os
 from pathlib import Path
 from subprocess import check_output
+import tempfile
 from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple
+from unittest import mock
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
 from djtools.spotify.helpers import get_playlist_ids, get_spotify_client
 
 
 logger = logging.getLogger(__name__)
 
 
+class MockOpen:
+    builtin_open = open
+
+    def __init__(
+        self,
+        files: List[str],
+        user_a: Optional[Tuple[str]] = None,
+        user_b: Optional[Tuple[str]] = None,
+        content: Optional[str] = "",
+        write_only: Optional[bool] = False,
+    ):
+        self._user_a = user_a 
+        self._user_b = user_b 
+        self._files = files
+        self._content = content
+        self._write_only = write_only
+
+    def open(self, *args, **kwargs):
+        file_name = os.path.basename(args[0])
+        if file_name in self._files:
+            if "w" in kwargs.get("mode"):
+                return tempfile.TemporaryFile(mode=kwargs["mode"])
+            elif not self._write_only:
+                return self._file_strategy(file_name, *args, **kwargs)
+        return self.builtin_open(*args, **kwargs)
+    
+    def _file_strategy(self, file_name, *args, **kwargs):
+        if self._content:
+            data = self._content
+        elif file_name == "registered_users.yaml":
+            data = (
+                f'{{"{self._user_a[0]}": "{self._user_a[1]}", '
+                f'"{self._user_b[0]}": "{self._user_b[1]}"}}'
+            )
+        else:
+            data = "{}"
+
+        return mock.mock_open(read_data=data)(*args, **kwargs)
+
+
 def add_tracks(result: Dict[str, Any]) -> List[str]:
     """Parses a page of Spotify API result tracks and returns a list of the
         track titles and artist names.
 
     Args:
         result: Paged result of Spotify tracks.
 
@@ -251,7 +293,15 @@
         fname=log_conf,
         # NOTE(a-rich): the `logfilename` needs a unix-style path.
         defaults={"logfilename": log_file.as_posix()},
         disable_existing_loggers=False,
     )
 
     return logging.getLogger(__name__), log_file
+
+
+def mock_exists(files, path):
+    for file_name, exists in files:
+        if file_name == path.name:
+            return exists
+
+    return True
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b7/djtools/utils/test_check_tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 from unittest import mock
 
 import pytest
 
 from djtools.utils.check_tracks import compare_tracks
 
 
-pytest_plugins = [
-    "test_data",
-]
-
-
 @pytest.mark.parametrize("get_spotify_tracks_flag", [True, False])
 @pytest.mark.parametrize("get_local_tracks_flag", [True, False])
 @pytest.mark.parametrize("beatcloud_tracks", [[], [Path("track - artist")]])
 @pytest.mark.parametrize("download_spotify", ["", "playlist Uploads"])
 @mock.patch("djtools.utils.check_tracks.get_local_tracks", return_value={})
 @mock.patch(
     "djtools.utils.check_tracks.get_beatcloud_tracks",
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b7/djtools/utils/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,15 @@
     find_matches,
     initialize_logger,
     get_beatcloud_tracks,
     get_local_tracks,
     get_playlist_tracks,
     get_spotify_tracks,
 )
-from test_data import MockOpen
-
-
-pytest_plugins = [
-    "test_data",
-]
+from djtools.utils.helpers import MockOpen
 
 
 def test_add_tracks():
     test_input = {
         "items": [
             {
                 "track": {
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b7/djtools/utils/test_url_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 
 import pytest
 from youtube_dl.utils import DownloadError
 
 from djtools.utils.url_download import fix_up, url_download
 
 
-pytest_plugins = [
-    "test_data",
-]
-
-
 @pytest.mark.parametrize(
     "test_assets",
     [
         (
             "Some Artist - Some Track-1224569284.mp3",
             "Some Track - Some Artist.mp3",
         ),
```

### Comparing `dj_beatcloud-2.4.1b6/src/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b7/djtools/utils/url_download.py`

 * *Files identical despite different names*

