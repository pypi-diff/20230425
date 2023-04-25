# Comparing `tmp/quorum_data_py-1.2.1.tar.gz` & `tmp/quorum_data_py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.2.1.tar", last modified: Tue Apr 25 03:00:51 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.2.tar", last modified: Tue Apr 25 06:34:55 2023, max compression
```

## Comparing `quorum_data_py-1.2.1.tar` & `quorum_data_py-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.363324 quorum_data_py-1.2.1/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-25 03:00:51.362331 quorum_data_py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.1/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.351359 quorum_data_py-1.2.1/quorum_data_py/
--rw-rw-rw-   0        0        0      355 2023-04-25 02:58:21.000000 quorum_data_py-1.2.1/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.1/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.1/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5897 2023-04-24 03:44:25.000000 quorum_data_py-1.2.1/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.1/quorum_data_py/trx_type.py
--rw-rw-rw-   0        0        0      328 2023-04-25 02:57:45.000000 quorum_data_py-1.2.1/quorum_data_py/util.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.360334 quorum_data_py-1.2.1/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 03:00:51.364323 quorum_data_py-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-25 03:00:39.000000 quorum_data_py-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.946364 quorum_data_py-1.2.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:34:55.945370 quorum_data_py-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.2/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.935392 quorum_data_py-1.2.2/quorum_data_py/
+-rw-rw-rw-   0        0        0      355 2023-04-25 06:33:47.000000 quorum_data_py-1.2.2/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.2/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.2/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.2/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.2/quorum_data_py/trx_type.py
+-rw-rw-rw-   0        0        0      944 2023-04-25 06:32:44.000000 quorum_data_py-1.2.2/quorum_data_py/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.944377 quorum_data_py-1.2.2/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:34:55.947342 quorum_data_py-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-25 06:34:38.000000 quorum_data_py-1.2.2/setup.py
```

### Comparing `quorum_data_py-1.2.1/LICENSE` & `quorum_data_py-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.1/PKG-INFO` & `quorum_data_py-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.1/README.md` & `quorum_data_py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.1/quorum_data_py/_utils.py` & `quorum_data_py-1.2.2/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.1/quorum_data_py/converter.py` & `quorum_data_py-1.2.2/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.1/quorum_data_py/feed.py` & `quorum_data_py-1.2.2/quorum_data_py/feed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 """Data structure recommendations in Quorum. For webapp Feed, Port and RumApp"""
 
-import datetime
 import logging
 
+from quorum_data_py import util
 from quorum_data_py._utils import pack_icon, pack_imgs, pack_obj
 
 logger = logging.getLogger(__name__)
 
 
-def check_publiched(published):
-    if isinstance(published, (float, int)):
-        published = int(str(published)[:10])
-        dt = datetime.datetime.fromtimestamp(published, datetime.timezone.utc)
-        published = dt.isoformat(timespec="seconds")
-    else:
-        try:
-            dt = datetime.datetime.fromisoformat(
-                published.replace("Z", "+00:00")
-            )
-            published = dt.isoformat(timespec="seconds")
-        except Exception as e:
-            raise ValueError(f"published format error: {published}") from e
-    return published
-
-
 def add_published(data: dict, published):
     """
     published: timestamp int or ISO format string
     e.g. 2020-01-01T00:00:00Z, 2023-04-04T10:31:45+08:00
     """
-    data["published"] = check_publiched(published)
+    data["published"] = util.check_publiched(published)
     return data
 
 
 def add_origin(data: dict, origin_name, origin_type=None):
     origin_type = origin_type or "Application"
     if origin_type not in ["Application", "Service"]:
         logger.warning("origin_type should be 'Application' or 'Service'")
```

### Comparing `quorum_data_py-1.2.1/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.2/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.1/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.2/quorum_data_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.1/setup.py` & `quorum_data_py-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.2.1",
+    version="1.2.2",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

