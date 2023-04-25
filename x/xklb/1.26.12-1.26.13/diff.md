# Comparing `tmp/xklb-1.26.12.tar.gz` & `tmp/xklb-1.26.13.tar.gz`

## Comparing `xklb-1.26.12.tar` & `xklb-1.26.13.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.12/.gitattributes
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.12/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.12/Windows.md
--rw-r--r--   0        0        0   418454 2020-02-02 00:00:00.000000 xklb-1.26.12/pdm.lock
--rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 xklb-1.26.12/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.12/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.12/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.12/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.12/.github/workflows/push.yaml
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 xklb-1.26.12/sql/restore_listen_count.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/__init__.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/av.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/books.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/consts.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/dl_config.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/dl_extract.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/fs_extract.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/gui.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/hn_extract.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/lb.py
--rw-r--r--   0        0        0    34810 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/play_actions.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/playback.py
--rw-r--r--   0        0        0    26604 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/player.py
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/praw_extract.py
--rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/stats.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/subtitle.py
--rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/tube_backend.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/tube_extract.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/utils.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/christen.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.12/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.12/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.12/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.12/LICENSE
--rw-r--r--   0        0        0    40027 2020-02-02 00:00:00.000000 xklb-1.26.12/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 xklb-1.26.12/pyproject.toml
--rw-r--r--   0        0        0    43564 2020-02-02 00:00:00.000000 xklb-1.26.12/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.13/.gitattributes
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.13/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.13/Windows.md
+-rw-r--r--   0        0        0   418454 2020-02-02 00:00:00.000000 xklb-1.26.13/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.13/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 xklb-1.26.13/sql/restore_listen_count.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/__init__.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/av.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/books.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/consts.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/dl_config.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/gui.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/lb.py
+-rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/play_actions.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/playback.py
+-rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/player.py
+-rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/stats.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/subtitle.py
+-rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/utils.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/reddit_self.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.13/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.13/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.13/LICENSE
+-rw-r--r--   0        0        0    40448 2020-02-02 00:00:00.000000 xklb-1.26.13/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 xklb-1.26.13/pyproject.toml
+-rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 xklb-1.26.13/PKG-INFO
```

### Comparing `xklb-1.26.12/TODO` & `xklb-1.26.13/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/Windows.md` & `xklb-1.26.13/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/pdm.lock` & `xklb-1.26.13/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/readme.py` & `xklb-1.26.13/readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ![termtosvg](./examples/extract.svg)
 
 ### 2. Watch / Listen from local files
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
-    library listen finalists.db --post-action=ask # ask whether to delete after playing
+    library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
 ## Getting started with online media
 
 ### 1. Download Metadata
```

### Comparing `xklb-1.26.12/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.13/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.13/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/.github/workflows/push.yaml` & `xklb-1.26.13/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/av.py` & `xklb-1.26.13/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/books.py` & `xklb-1.26.13/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/consts.py` & `xklb-1.26.13/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/db.py` & `xklb-1.26.13/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/dl_config.py` & `xklb-1.26.13/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/dl_extract.py` & `xklb-1.26.13/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/fs_extract.py` & `xklb-1.26.13/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/gui.py` & `xklb-1.26.13/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/hn_extract.py` & `xklb-1.26.13/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/lb.py` & `xklb-1.26.13/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/play_actions.py` & `xklb-1.26.13/xklb/play_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,21 +224,28 @@
     Specify media play order:
         library {action} --sort duration   # play shortest media first
         library {action} -u duration desc  # play longest media first
         You can use multiple SQL ORDER BY expressions
         library {action} -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
 
     Post-actions -- choose what to do after playing:
-        library {action} --post-action delete  # delete file after playing
-        library {action} -k ask  # ask after each whether to keep or delete
+        library {action} --post-action keep    # do nothing after playing (default)
+        library {action} -k delete             # delete file after playing
+        library {action} -k softdelete         # mark deleted after playing
 
-        library {action} -k askkeep  # ask after each whether to move to a keep folder or delete
+        library {action} -k ask_keep           # ask whether to keep after playing
+        library {action} -k ask_delete         # ask whether to delete after playing
+
+        library {action} -k move               # move to "keep" dir after playing
+        library {action} -k ask_move           # ask whether to move to "keep" folder
         The default location of the keep folder is ./keep/ (relative to the played media file)
         You can change this by explicitly setting an *absolute* `keep-dir` path:
-        library {action} -k askkeep --keep-dir /home/my/music/keep/
+        library {action} -k ask_move --keep-dir /home/my/music/keep/
+
+        library {action} -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library {action} --interdimensional-cable 40
         library {action} -4dtv 40
 
         Playback multiple files at once
@@ -479,14 +486,17 @@
         args.keep_dir = Path(args.keep_dir).expanduser().resolve()
 
     if args.solo:
         args.upper = 1
     if args.sibling:
         args.lower = 2
 
+    if args.post_action:
+        args.post_action = args.post_action.replace("-", "_")
+
     utils.timeout(args.timeout)
 
     args.sock = None
     return args
 
 
 def construct_search_bindings(args, columns) -> None:
@@ -751,23 +761,25 @@
         if r.returncode != 0:
             print("Player exited with code", r.returncode)
             if args.ignore_errors:
                 return
             else:
                 raise SystemExit(r.returncode)
 
-    playhead = utils.get_playhead(
-        args,
-        original_path,
-        start_time,
-        existing_playhead=m.get("playhead"),
-        media_duration=m.get("duration"),
-    )
-    if playhead:
-        player.set_playhead(args, original_path, playhead)
+    m_columns = args.db["media"].columns_dict
+    if "playhead" in m_columns:
+        playhead = utils.get_playhead(
+            args,
+            original_path,
+            start_time,
+            existing_playhead=m.get("playhead"),
+            media_duration=m.get("duration"),
+        )
+        if playhead:
+            player.set_playhead(args, original_path, playhead)
     player.post_act(args, original_path)
 
 
 def process_playqueue(args) -> None:
     query, bindings = construct_query(args)
 
     if args.print:
```

### Comparing `xklb-1.26.12/xklb/playback.py` & `xklb-1.26.13/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/player.py` & `xklb-1.26.13/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,25 +289,23 @@
     DELETE_IF_AUDIOBOOK = "delete_if_audiobook"
     SOFTDELETE = "softdelete"
     MOVE = "move"
 
 
 class AskAction:
     ASK_KEEP = (Action.KEEP, Action.DELETE)
-    ASK_MOVE_OR_DELETE = (Action.MOVE, Action.DELETE)
+    ASK_MOVE = (Action.MOVE, Action.KEEP)
     ASK_DELETE = (Action.DELETE, Action.KEEP)
     ASK_SOFTDELETE = (Action.SOFTDELETE, Action.KEEP)
+    ASK_MOVE_OR_DELETE = (Action.MOVE, Action.DELETE)
 
 
 def post_act(args, media_file: str, action: Optional[str] = None, geom_data=None, media=None) -> None:
     mark_media_watched(args, [media_file])
 
-    def handle_keep_action():
-        return
-
     def handle_delete_action():
         if media_file.startswith("http"):
             mark_media_deleted(args, media_file)
         else:
             delete_media(args, media_file)
 
     def handle_soft_delete_action():
@@ -330,19 +328,20 @@
         else:
             response = utils.confirm(true_action.title() + "?")
         post_act(args, media_file, action=true_action if response else false_action)
 
     action = action or args.post_action
 
     if action == Action.KEEP:
-        handle_keep_action()
+        pass
     elif action == Action.DELETE:
         handle_delete_action()
-    elif action == Action.DELETE_IF_AUDIOBOOK and "audiobook" in media_file.lower():
-        handle_delete_action()
+    elif action == Action.DELETE_IF_AUDIOBOOK:
+        if "audiobook" in media_file.lower():
+            handle_delete_action()
     elif action == Action.SOFTDELETE:
         handle_soft_delete_action()
     elif action == Action.MOVE:
         handle_move_action()
     elif action.startswith("ask_"):
         handle_ask_action(action)
     else:
```

### Comparing `xklb-1.26.12/xklb/praw_extract.py` & `xklb-1.26.13/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/stats.py` & `xklb-1.26.13/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/subtitle.py` & `xklb-1.26.13/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/tabs_actions.py` & `xklb-1.26.13/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/tabs_extract.py` & `xklb-1.26.13/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/tube_backend.py` & `xklb-1.26.13/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/tube_extract.py` & `xklb-1.26.13/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/utils.py` & `xklb-1.26.13/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/__init__.py` & `xklb-1.26.13/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/bigdirs.py` & `xklb-1.26.13/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/christen.py` & `xklb-1.26.13/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/dedupe.py` & `xklb-1.26.13/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/merge_dbs.py` & `xklb-1.26.13/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/merge_online_local.py` & `xklb-1.26.13/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/move_list.py` & `xklb-1.26.13/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/optimize_db.py` & `xklb-1.26.13/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/redownload.py` & `xklb-1.26.13/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/relmv.py` & `xklb-1.26.13/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/scatter.py` & `xklb-1.26.13/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.13/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.13/xklb/scripts/mining/nfb_ca.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/mining/nouns.py` & `xklb-1.26.13/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/mining/pushshift.py` & `xklb-1.26.13/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/mining/reddit_self.py` & `xklb-1.26.13/xklb/scripts/mining/reddit_self.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/xklb/scripts/mining/words.py` & `xklb-1.26.13/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/assets/kotobago.png` & `xklb-1.26.13/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/.gitignore` & `xklb-1.26.13/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/LICENSE` & `xklb-1.26.13/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/README.md` & `xklb-1.26.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.012)
+    xk media library subcommands (v1.26.013)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -107,15 +107,15 @@
 
 ![termtosvg](./examples/extract.svg)
 
 ### 2. Watch / Listen from local files
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
-    library listen finalists.db --post-action=ask # ask whether to delete after playing
+    library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
 ## Getting started with online media
 
 ### 1. Download Metadata
 
@@ -421,21 +421,28 @@
     Specify media play order:
         library watch --sort duration   # play shortest media first
         library watch -u duration desc  # play longest media first
         You can use multiple SQL ORDER BY expressions
         library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
 
     Post-actions -- choose what to do after playing:
-        library watch --post-action delete  # delete file after playing
-        library watch -k ask  # ask after each whether to keep or delete
+        library watch --post-action keep    # do nothing after playing (default)
+        library watch -k delete             # delete file after playing
+        library watch -k softdelete         # mark deleted after playing
 
-        library watch -k askkeep  # ask after each whether to move to a keep folder or delete
+        library watch -k ask_keep           # ask whether to keep after playing
+        library watch -k ask_delete         # ask whether to delete after playing
+
+        library watch -k move               # move to "keep" dir after playing
+        library watch -k ask_move           # ask whether to move to "keep" folder
         The default location of the keep folder is ./keep/ (relative to the played media file)
         You can change this by explicitly setting an *absolute* `keep-dir` path:
-        library watch -k askkeep --keep-dir /home/my/music/keep/
+        library watch -k ask_move --keep-dir /home/my/music/keep/
+
+        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library watch --interdimensional-cable 40
         library watch -4dtv 40
 
         Playback multiple files at once
```

### Comparing `xklb-1.26.12/pyproject.toml` & `xklb-1.26.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.12/PKG-INFO` & `xklb-1.26.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.12
+Version: 1.26.13
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -100,15 +100,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.012)
+    xk media library subcommands (v1.26.013)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -190,15 +190,15 @@
 
 ![termtosvg](./examples/extract.svg)
 
 ### 2. Watch / Listen from local files
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
-    library listen finalists.db --post-action=ask # ask whether to delete after playing
+    library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
 ## Getting started with online media
 
 ### 1. Download Metadata
 
@@ -504,21 +504,28 @@
     Specify media play order:
         library watch --sort duration   # play shortest media first
         library watch -u duration desc  # play longest media first
         You can use multiple SQL ORDER BY expressions
         library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
 
     Post-actions -- choose what to do after playing:
-        library watch --post-action delete  # delete file after playing
-        library watch -k ask  # ask after each whether to keep or delete
+        library watch --post-action keep    # do nothing after playing (default)
+        library watch -k delete             # delete file after playing
+        library watch -k softdelete         # mark deleted after playing
 
-        library watch -k askkeep  # ask after each whether to move to a keep folder or delete
+        library watch -k ask_keep           # ask whether to keep after playing
+        library watch -k ask_delete         # ask whether to delete after playing
+
+        library watch -k move               # move to "keep" dir after playing
+        library watch -k ask_move           # ask whether to move to "keep" folder
         The default location of the keep folder is ./keep/ (relative to the played media file)
         You can change this by explicitly setting an *absolute* `keep-dir` path:
-        library watch -k askkeep --keep-dir /home/my/music/keep/
+        library watch -k ask_move --keep-dir /home/my/music/keep/
+
+        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library watch --interdimensional-cable 40
         library watch -4dtv 40
 
         Playback multiple files at once
```

