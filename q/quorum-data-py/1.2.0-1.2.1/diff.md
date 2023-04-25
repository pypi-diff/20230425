# Comparing `tmp/quorum_data_py-1.2.0.tar.gz` & `tmp/quorum_data_py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.2.0.tar", last modified: Mon Apr 24 03:45:50 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.1.tar", last modified: Tue Apr 25 03:00:51 2023, max compression
```

## Comparing `quorum_data_py-1.2.0.tar` & `quorum_data_py-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.802922 quorum_data_py-1.2.0/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-24 03:45:50.781978 quorum_data_py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.0/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.763028 quorum_data_py-1.2.0/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-24 03:44:48.000000 quorum_data_py-1.2.0/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.0/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.0/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5897 2023-04-24 03:44:25.000000 quorum_data_py-1.2.0/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.0/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.778986 quorum_data_py-1.2.0/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 03:45:50.803919 quorum_data_py-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-24 03:44:48.000000 quorum_data_py-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.363324 quorum_data_py-1.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-25 03:00:51.362331 quorum_data_py-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.1/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.351359 quorum_data_py-1.2.1/quorum_data_py/
+-rw-rw-rw-   0        0        0      355 2023-04-25 02:58:21.000000 quorum_data_py-1.2.1/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.1/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.1/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5897 2023-04-24 03:44:25.000000 quorum_data_py-1.2.1/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.1/quorum_data_py/trx_type.py
+-rw-rw-rw-   0        0        0      328 2023-04-25 02:57:45.000000 quorum_data_py-1.2.1/quorum_data_py/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:00:51.360334 quorum_data_py-1.2.1/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 03:00:51.000000 quorum_data_py-1.2.1/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:00:51.364323 quorum_data_py-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-25 03:00:39.000000 quorum_data_py-1.2.1/setup.py
```

### Comparing `quorum_data_py-1.2.0/LICENSE` & `quorum_data_py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/PKG-INFO` & `quorum_data_py-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.0/README.md` & `quorum_data_py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/quorum_data_py/_utils.py` & `quorum_data_py-1.2.1/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/quorum_data_py/converter.py` & `quorum_data_py-1.2.1/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/quorum_data_py/feed.py` & `quorum_data_py-1.2.1/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.1/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.0/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.1/quorum_data_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.0/setup.py` & `quorum_data_py-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.2.0",
+    version="1.2.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

