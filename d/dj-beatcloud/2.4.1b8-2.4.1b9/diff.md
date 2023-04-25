# Comparing `tmp/dj_beatcloud-2.4.1b8.tar.gz` & `tmp/dj_beatcloud-2.4.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b8.tar", last modified: Tue Apr 25 02:50:51 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b9.tar", last modified: Tue Apr 25 02:58:27 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b8.tar` & `dj_beatcloud-2.4.1b9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.663833 dj_beatcloud-2.4.1b8/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b8/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 02:22:26.000000 dj_beatcloud-2.4.1b8/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:50:51.663945 dj_beatcloud-2.4.1b8/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28208 2023-04-25 02:22:18.000000 dj_beatcloud-2.4.1b8/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.653243 dj_beatcloud-2.4.1b8/djtools/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.656257 dj_beatcloud-2.4.1b8/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      466 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4653 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.657080 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1827 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       42 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       37 2023-04-25 02:50:51.000000 dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.658909 dj_beatcloud-2.4.1b8/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1292 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1173 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1353 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2974 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5102 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1437 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3905 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.660638 dj_beatcloud-2.4.1b8/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      680 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17439 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6108 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.662113 dj_beatcloud-2.4.1b8/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      736 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8218 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4010 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8157 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4686 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/sync/test_sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:50:51.663694 dj_beatcloud-2.4.1b8/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      795 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9423 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3187 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8505 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1540 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b8/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 01:26:32.000000 dj_beatcloud-2.4.1b8/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      148 2023-04-25 02:50:51.664260 dj_beatcloud-2.4.1b8/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-25 02:50:41.000000 dj_beatcloud-2.4.1b8/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.594237 dj_beatcloud-2.4.1b9/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b9/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 02:22:26.000000 dj_beatcloud-2.4.1b9/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:58:27.594350 dj_beatcloud-2.4.1b9/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28208 2023-04-25 02:22:18.000000 dj_beatcloud-2.4.1b9/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.582440 dj_beatcloud-2.4.1b9/djtools/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.586050 dj_beatcloud-2.4.1b9/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      466 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4653 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.587016 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1827 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       37 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.589712 dj_beatcloud-2.4.1b9/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1292 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1173 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1353 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2974 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5102 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1437 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3905 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.591318 dj_beatcloud-2.4.1b9/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      680 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17439 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6108 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.592623 dj_beatcloud-2.4.1b9/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      736 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8218 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4010 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8157 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4686 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.594105 dj_beatcloud-2.4.1b9/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      795 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9423 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3187 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8505 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1540 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 01:26:32.000000 dj_beatcloud-2.4.1b9/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      148 2023-04-25 02:58:27.594744 dj_beatcloud-2.4.1b9/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2233 2023-04-25 02:58:11.000000 dj_beatcloud-2.4.1b9/setup.py
```

### Comparing `dj_beatcloud-2.4.1b8/LICENSE` & `dj_beatcloud-2.4.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/PKG-INFO` & `dj_beatcloud-2.4.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b8
+Version: 2.4.1b9
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b8/README.md` & `dj_beatcloud-2.4.1b9/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/README.md` & `dj_beatcloud-2.4.1b9/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/config.py` & `dj_beatcloud-2.4.1b9/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b9/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b9/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.4.1b9/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b9/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b9/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b8
+Version: 2.4.1b9
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b8/djtools/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b9/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b9/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/config.py` & `dj_beatcloud-2.4.1b9/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b9/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b9/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b9/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b9/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b9/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/__init__.py` & `dj_beatcloud-2.4.1b9/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b9/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/config.py` & `dj_beatcloud-2.4.1b9/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b9/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b9/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b9/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b9/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b9/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b8/setup.py` & `dj_beatcloud-2.4.1b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b8',
+    version='2.4.1-b9',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
@@ -68,10 +68,10 @@
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
     extras_require=EXTRAS,
     python_requires=">=3.6",
     include_package_data=True,
     keywords='MP3 Rekordbox XML spotify reddit aws s3',
     entry_points={
-        'console_scripts': ['djtools=dj_tools:main']
+        'console_scripts': ['djtools=djtools:dj_tools.main']
     }
 )
```

