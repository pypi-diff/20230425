# Comparing `tmp/quorum_data_py-1.2.2.tar.gz` & `tmp/quorum_data_py-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.2.2.tar", last modified: Tue Apr 25 06:34:55 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.3.tar", last modified: Tue Apr 25 06:41:29 2023, max compression
```

## Comparing `quorum_data_py-1.2.2.tar` & `quorum_data_py-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.946364 quorum_data_py-1.2.2/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-25 06:34:55.945370 quorum_data_py-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.2/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.935392 quorum_data_py-1.2.2/quorum_data_py/
--rw-rw-rw-   0        0        0      355 2023-04-25 06:33:47.000000 quorum_data_py-1.2.2/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.2/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.2/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.2/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.2/quorum_data_py/trx_type.py
--rw-rw-rw-   0        0        0      944 2023-04-25 06:32:44.000000 quorum_data_py-1.2.2/quorum_data_py/util.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:34:55.944377 quorum_data_py-1.2.2/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 06:34:55.000000 quorum_data_py-1.2.2/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:34:55.947342 quorum_data_py-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-25 06:34:38.000000 quorum_data_py-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.493574 quorum_data_py-1.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:41:29.246169 quorum_data_py-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.3/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.233204 quorum_data_py-1.2.3/quorum_data_py/
+-rw-rw-rw-   0        0        0      355 2023-04-25 06:40:43.000000 quorum_data_py-1.2.3/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.3/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.3/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.3/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.3/quorum_data_py/trx_type.py
+-rw-rw-rw-   0        0        0      946 2023-04-25 06:40:27.000000 quorum_data_py-1.2.3/quorum_data_py/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.244176 quorum_data_py-1.2.3/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:41:29.493574 quorum_data_py-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-25 06:40:43.000000 quorum_data_py-1.2.3/setup.py
```

### Comparing `quorum_data_py-1.2.2/LICENSE` & `quorum_data_py-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/PKG-INFO` & `quorum_data_py-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.2/README.md` & `quorum_data_py-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/quorum_data_py/_utils.py` & `quorum_data_py-1.2.3/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/quorum_data_py/converter.py` & `quorum_data_py-1.2.3/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/quorum_data_py/feed.py` & `quorum_data_py-1.2.3/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.3/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.2/quorum_data_py/util.py` & `quorum_data_py-1.2.3/quorum_data_py/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
             raise ValueError(f"published format error: {published}") from e
     return published
 
 
 def get_published_datetime(trx: dict):
     published = trx["Data"].get("published")
     if published:
-        dt = datetime.datetime.strptime(published, "%Y-%m-%dT%H:%M:%S%z")
+        dt = datetime.datetime.strptime(published, "%Y-%m-%dT%H:%M:%S.%fZ")
         utc_dt = dt - dt.utcoffset()
     else:
         trx_ts = int(str(trx["TimeStamp"])[:10])
         utc_dt = datetime.datetime.utcfromtimestamp(trx_ts)
     return utc_dt
```

### Comparing `quorum_data_py-1.2.2/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.3/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.2/setup.py` & `quorum_data_py-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.2.2",
+    version="1.2.3",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

