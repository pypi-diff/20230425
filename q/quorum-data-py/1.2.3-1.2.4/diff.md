# Comparing `tmp/quorum_data_py-1.2.3.tar.gz` & `tmp/quorum_data_py-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.2.3.tar", last modified: Tue Apr 25 06:41:29 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.4.tar", last modified: Tue Apr 25 06:48:36 2023, max compression
```

## Comparing `quorum_data_py-1.2.3.tar` & `quorum_data_py-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.493574 quorum_data_py-1.2.3/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-25 06:41:29.246169 quorum_data_py-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.3/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.233204 quorum_data_py-1.2.3/quorum_data_py/
--rw-rw-rw-   0        0        0      355 2023-04-25 06:40:43.000000 quorum_data_py-1.2.3/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.3/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.3/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.3/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.3/quorum_data_py/trx_type.py
--rw-rw-rw-   0        0        0      946 2023-04-25 06:40:27.000000 quorum_data_py-1.2.3/quorum_data_py/util.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:41:29.244176 quorum_data_py-1.2.3/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 06:41:29.000000 quorum_data_py-1.2.3/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:41:29.493574 quorum_data_py-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-25 06:40:43.000000 quorum_data_py-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.206225 quorum_data_py-1.2.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:48:36.205241 quorum_data_py-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.4/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:35.938626 quorum_data_py-1.2.4/quorum_data_py/
+-rw-rw-rw-   0        0        0      355 2023-04-25 06:47:05.000000 quorum_data_py-1.2.4/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.4/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.4/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.4/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.4/quorum_data_py/trx_type.py
+-rw-rw-rw-   0        0        0     1093 2023-04-25 06:46:18.000000 quorum_data_py-1.2.4/quorum_data_py/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:48:36.203220 quorum_data_py-1.2.4/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-25 06:48:35.000000 quorum_data_py-1.2.4/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-25 06:48:35.000000 quorum_data_py-1.2.4/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:48:35.000000 quorum_data_py-1.2.4/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 06:48:35.000000 quorum_data_py-1.2.4/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 06:48:35.000000 quorum_data_py-1.2.4/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:48:36.207212 quorum_data_py-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-25 06:47:05.000000 quorum_data_py-1.2.4/setup.py
```

### Comparing `quorum_data_py-1.2.3/LICENSE` & `quorum_data_py-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/PKG-INFO` & `quorum_data_py-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.3/README.md` & `quorum_data_py-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/quorum_data_py/_utils.py` & `quorum_data_py-1.2.4/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/quorum_data_py/converter.py` & `quorum_data_py-1.2.4/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/quorum_data_py/feed.py` & `quorum_data_py-1.2.4/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.4/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.3/quorum_data_py/util.py` & `quorum_data_py-1.2.4/quorum_data_py/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,12 +17,16 @@
     return published
 
 
 def get_published_datetime(trx: dict):
     published = trx["Data"].get("published")
     if published:
         dt = datetime.datetime.strptime(published, "%Y-%m-%dT%H:%M:%S.%fZ")
-        utc_dt = dt - dt.utcoffset()
+        utc_offset = dt.utcoffset()
+        if utc_offset is not None:
+            utc_dt = dt - utc_offset
+        else:
+            utc_dt = dt.replace(tzinfo=datetime.timezone.utc)
     else:
         trx_ts = int(str(trx["TimeStamp"])[:10])
         utc_dt = datetime.datetime.utcfromtimestamp(trx_ts)
     return utc_dt
```

### Comparing `quorum_data_py-1.2.3/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.4/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.3/setup.py` & `quorum_data_py-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.2.3",
+    version="1.2.4",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

