# Comparing `tmp/xklb-1.25.3.tar.gz` & `tmp/xklb-1.26.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xklb-1.25.3.tar", max compression
+gzip compressed data, was "xklb-1.26.11.tar", last modified: Tue Apr 25 06:53:28 2023, max compression
```

## Comparing `xklb-1.25.3.tar` & `xklb-1.26.11.tar`

### file list

```diff
@@ -1,45 +1,7 @@
--rw-r--r--   0        0        0     1676 2023-04-21 07:18:15.452260 xklb-1.25.3/LICENSE
--rw-r--r--   0        0        0    40027 2023-04-21 07:18:15.452260 xklb-1.25.3/README.md
--rw-r--r--   0        0        0     8385 2023-04-21 07:18:15.452260 xklb-1.25.3/assets/kotobago.png
--rw-r--r--   0        0        0    13982 2023-04-21 07:18:16.436261 xklb-1.25.3/pyproject.toml
--rw-r--r--   0        0        0      693 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/__init__.py
--rw-r--r--   0        0        0     4199 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/bigdirs.py
--rw-r--r--   0        0        0     2376 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/christen.py
--rw-r--r--   0        0        0     7864 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/dedupe.py
--rw-r--r--   0        0        0     1370 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4020 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/merge_online_local.py
--rw-r--r--   0        0        0     1009 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1569 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2085 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/mining/words.py
--rw-r--r--   0        0        0     6864 2023-04-21 07:18:16.436261 xklb-1.25.3/scripts/move_list.py
--rw-r--r--   0        0        0      547 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/optimize_db.py
--rw-r--r--   0        0        0     9412 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/redownload.py
--rw-r--r--   0        0        0     2294 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/relmv.py
--rw-r--r--   0        0        0      483 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/restore_listen_count.sql
--rw-r--r--   0        0        0    17018 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/scatter.py
--rw-r--r--   0        0        0     2610 2023-04-21 07:18:16.440261 xklb-1.25.3/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0       25 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/__init__.py
--rw-r--r--   0        0        0     6637 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/av.py
--rw-r--r--   0        0        0     6870 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/books.py
--rw-r--r--   0        0        0     7676 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/consts.py
--rw-r--r--   0        0        0     7809 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/db.py
--rw-r--r--   0        0        0     7051 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/dl_config.py
--rw-r--r--   0        0        0    14677 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    13251 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     5444 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/gui.py
--rw-r--r--   0        0        0     5904 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/hn_extract.py
--rw-r--r--   0        0        0     9274 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/lb.py
--rw-r--r--   0        0        0    34308 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/play_actions.py
--rw-r--r--   0        0        0     4677 2023-04-21 07:18:16.440261 xklb-1.25.3/xklb/playback.py
--rw-r--r--   0        0        0    25538 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/player.py
--rw-r--r--   0        0        0    14553 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/praw_extract.py
--rw-r--r--   0        0        0    16048 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/stats.py
--rw-r--r--   0        0        0     4064 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/subtitle.py
--rw-r--r--   0        0        0    12060 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3607 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21475 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     6258 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/tube_extract.py
--rw-r--r--   0        0        0    26511 2023-04-21 07:18:16.444261 xklb-1.25.3/xklb/utils.py
--rw-r--r--   0        0        0    41215 1970-01-01 00:00:00.000000 xklb-1.25.3/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-04-25 06:53:14.311987 xklb-1.26.11/LICENSE
+-rw-r--r--   0        0        0     1676 2023-04-25 06:53:14.311987 xklb-1.26.11/LICENSE
+-rw-r--r--   0        0        0    40027 2023-04-25 06:53:14.315987 xklb-1.26.11/README.md
+-rw-r--r--   0        0        0    40027 2023-04-25 06:53:14.315987 xklb-1.26.11/README.md
+-rw-r--r--   0        0        0     8385 2023-04-25 06:53:14.315987 xklb-1.26.11/assets/kotobago.png
+-rw-r--r--   0        0        0     2409 2023-04-25 06:53:28.891852 xklb-1.26.11/pyproject.toml
+-rw-r--r--   0        0        0    43707 1970-01-01 00:00:00.000000 xklb-1.26.11/PKG-INFO
```

### Comparing `xklb-1.25.3/LICENSE` & `xklb-1.26.11/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.25.3/README.md` & `xklb-1.26.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.25.003)
+    xk media library subcommands (v1.26.011)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.25.3/assets/kotobago.png` & `xklb-1.26.11/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.25.3/PKG-INFO` & `xklb-1.26.11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.25.3
+Version: 1.26.11
 Summary: xk library
 Home-page: https://github.com/chapmanjacobd/library/
-License: BSD-3-Clause
-Author: Jacob Chapman
-Author-email: 7908073+chapmanjacobd@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Author-Email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
+License: BSD 3-Clause No Nuclear License
+        
+        Copyright (c) 2021, Jacob Chapman
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+        You acknowledge that this software is not designed nor intended for use in the
+        design, construction, operation or maintenance of any nuclear facility.
+Project-URL: Documentation, https://github.com/chapmanjacobd/library/wiki/Usage
+Project-URL: Homepage, https://github.com/chapmanjacobd/library/
+Project-URL: Repository, https://github.com/chapmanjacobd/library/
+Requires-Python: >=3.8
+Requires-Dist: sqlite-utils>=3.30
 Requires-Dist: Markdown
 Requires-Dist: catt
 Requires-Dist: ffmpeg-python
 Requires-Dist: ftfy
 Requires-Dist: gallery-dl
 Requires-Dist: humanize
 Requires-Dist: ipython
@@ -25,20 +53,39 @@
 Requires-Dist: natsort
 Requires-Dist: praw
 Requires-Dist: pysubs2
 Requires-Dist: python-mpv-jsonipc
 Requires-Dist: regex
 Requires-Dist: rich
 Requires-Dist: screeninfo
-Requires-Dist: sqlite-utils (>=3.30)
 Requires-Dist: subliminal
 Requires-Dist: tabulate
 Requires-Dist: tinytag
 Requires-Dist: yt-dlp
-Project-URL: Documentation, https://github.com/chapmanjacobd/library/wiki/Usage
+Requires-Dist: xklb[deluxe,dev,test]; extra == "all"
+Requires-Dist: xklb; extra == "deluxe"
+Requires-Dist: textract; extra == "deluxe"
+Requires-Dist: PyExifTool; extra == "deluxe"
+Requires-Dist: aiohttp; extra == "deluxe"
+Requires-Dist: brotab; extra == "deluxe"
+Requires-Dist: orjson; extra == "deluxe"
+Requires-Dist: pandas; extra == "deluxe"
+Requires-Dist: xklb; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: ipdb; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: scalene; extra == "dev"
+Requires-Dist: ssort; extra == "dev"
+Requires-Dist: xklb; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: all
+Provides-Extra: deluxe
+Provides-Extra: dev
+Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # xk media library
 
 A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage large media libraries. An index for your archive.
@@ -56,15 +103,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.25.003)
+    xk media library subcommands (v1.26.011)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -765,8 +812,7 @@
 
 Explore `library` databases in your browser
 
     pip install datasette
     datasette tv.db
 
 
-
```

