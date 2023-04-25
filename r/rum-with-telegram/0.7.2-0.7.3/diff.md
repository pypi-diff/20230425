# Comparing `tmp/rum_with_telegram-0.7.2.tar.gz` & `tmp/rum_with_telegram-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.7.2.tar", last modified: Tue Apr 25 07:48:26 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.7.3.tar", last modified: Tue Apr 25 07:54:12 2023, max compression
```

## Comparing `rum_with_telegram-0.7.2.tar` & `rum_with_telegram-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:48:26.914260 rum_with_telegram-0.7.2/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-25 07:48:26.913262 rum_with_telegram-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.7.2/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.7.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 07:48:26.899299 rum_with_telegram-0.7.2/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-25 07:48:07.000000 rum_with_telegram-0.7.2/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0    22603 2023-04-25 07:47:55.000000 rum_with_telegram-0.7.2/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.7.2/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.7.2/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-25 07:48:26.911269 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-25 07:48:26.000000 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-25 07:48:26.000000 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:48:26.000000 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-25 07:48:26.000000 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 07:48:26.000000 rum_with_telegram-0.7.2/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 07:48:26.914260 rum_with_telegram-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-25 07:48:07.000000 rum_with_telegram-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:54:12.078753 rum_with_telegram-0.7.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-25 07:54:12.077787 rum_with_telegram-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.7.3/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.7.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 07:54:12.038731 rum_with_telegram-0.7.3/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-25 07:53:56.000000 rum_with_telegram-0.7.3/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0    22638 2023-04-25 07:53:34.000000 rum_with_telegram-0.7.3/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.7.3/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.7.3/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:54:12.075762 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-25 07:54:11.000000 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-25 07:54:12.000000 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:54:11.000000 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-25 07:54:11.000000 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 07:54:11.000000 rum_with_telegram-0.7.3/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:54:12.079751 rum_with_telegram-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-25 07:53:56.000000 rum_with_telegram-0.7.3/setup.py
```

### Comparing `rum_with_telegram-0.7.2/LICENSE` & `rum_with_telegram-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.7.2/PKG-INFO` & `rum_with_telegram-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.7.2
+Version: 0.7.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.7.2/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.7.3/rum_with_telegram/data_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
         # send reply to user in group chat
         rum_post_url = self.db.get_trx_sent(channel_message_id).rum_post_url
         if not rum_post_url:
             logger.warning("not found channel_message_id %s", channel_message_id)
             return
 
-        if entities := update.message.entities:
+        if entities := update.message.entities or update.message.caption_entities:
             for entity in entities:
                 if entity.url == rum_post_url:
                     return
         await self._comment_with_feedurl(
             context, "", update.message.chat.id, chat_message_id, rum_post_url
         )
         payload = {
```

### Comparing `rum_with_telegram-0.7.2/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.7.3/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.7.2/rum_with_telegram/module.py` & `rum_with_telegram-0.7.3/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.7.2/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.7.3/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.7.2
+Version: 0.7.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.7.2/setup.py` & `rum_with_telegram-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.7.2",
+    version="0.7.3",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

