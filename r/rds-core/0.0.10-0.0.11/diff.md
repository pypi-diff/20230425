# Comparing `tmp/rds-core-0.0.10.tar.gz` & `tmp/rds-core-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.0.10.tar", last modified: Tue Apr 25 00:27:51 2023, max compression
+gzip compressed data, was "rds-core-0.0.11.tar", last modified: Tue Apr 25 00:29:33 2023, max compression
```

## Comparing `rds-core-0.0.10.tar` & `rds-core-0.0.11.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/
--rw-r--r--   0 kelso     (1000) kelso     (1000)       37 2023-04-20 17:24:59.000000 rds-core-0.0.10/LICENSE.md
--rw-r--r--   0 kelso     (1000) kelso     (1000)      927 2023-04-25 00:27:50.996713 rds-core-0.0.10/PKG-INFO
--rw-r--r--   0 kelso     (1000) kelso     (1000)      952 2023-04-24 23:04:40.000000 rds-core-0.0.10/README.md
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core/
--rw-r--r--   0 kelso     (1000) kelso     (1000)      295 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/__init__.py
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core/cache/
--rw-r--r--   0 kelso     (1000) kelso     (1000)      568 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/cache/__init__.py
--rw-r--r--   0 kelso     (1000) kelso     (1000)     5618 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/cache/base.py
--rw-r--r--   0 kelso     (1000) kelso     (1000)      621 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/cache/nocache.py
--rw-r--r--   0 kelso     (1000) kelso     (1000)     3780 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/cache/search_engine.py
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core/config/
--rw-r--r--   0 kelso     (1000) kelso     (1000)      100 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/config/__init__.py
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core/helpers/
--rw-r--r--   0 kelso     (1000) kelso     (1000)      606 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/helpers/__init__.py
--rw-r--r--   0 kelso     (1000) kelso     (1000)      244 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/helpers/cnes.py
--rw-r--r--   0 kelso     (1000) kelso     (1000)     1798 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/helpers/http_client.py
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core/searchengine/
--rw-r--r--   0 kelso     (1000) kelso     (1000)     5349 2023-04-24 23:04:40.000000 rds-core-0.0.10/rds_core/searchengine/__init__.py
-drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:27:50.996713 rds-core-0.0.10/rds_core.egg-info/
--rw-r--r--   0 kelso     (1000) kelso     (1000)      927 2023-04-25 00:27:50.000000 rds-core-0.0.10/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 kelso     (1000) kelso     (1000)      475 2023-04-25 00:27:50.000000 rds-core-0.0.10/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 kelso     (1000) kelso     (1000)        1 2023-04-25 00:27:50.000000 rds-core-0.0.10/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 kelso     (1000) kelso     (1000)      142 2023-04-25 00:27:50.000000 rds-core-0.0.10/rds_core.egg-info/requires.txt
--rw-r--r--   0 kelso     (1000) kelso     (1000)        9 2023-04-25 00:27:50.000000 rds-core-0.0.10/rds_core.egg-info/top_level.txt
--rw-r--r--   0 kelso     (1000) kelso     (1000)      105 2023-04-25 00:27:50.996713 rds-core-0.0.10/setup.cfg
--rw-r--r--   0 kelso     (1000) kelso     (1000)     2155 2023-04-24 23:04:40.000000 rds-core-0.0.10/setup.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)       37 2023-04-20 17:24:59.000000 rds-core-0.0.11/LICENSE.md
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     1028 2023-04-25 00:29:32.993390 rds-core-0.0.11/PKG-INFO
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      952 2023-04-24 23:04:40.000000 rds-core-0.0.11/README.md
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      295 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/__init__.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core/cache/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      568 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/cache/__init__.py
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     5618 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/cache/base.py
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      621 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/cache/nocache.py
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     3780 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/cache/search_engine.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core/config/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      100 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/config/__init__.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core/helpers/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      606 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/helpers/__init__.py
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      244 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/helpers/cnes.py
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     1798 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/helpers/http_client.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core/searchengine/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     5349 2023-04-24 23:04:40.000000 rds-core-0.0.11/rds_core/searchengine/__init__.py
+drwxr-xr-x   0 kelso     (1000) kelso     (1000)        0 2023-04-25 00:29:32.993390 rds-core-0.0.11/rds_core.egg-info/
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     1028 2023-04-25 00:29:32.000000 rds-core-0.0.11/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      475 2023-04-25 00:29:32.000000 rds-core-0.0.11/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 kelso     (1000) kelso     (1000)        1 2023-04-25 00:29:32.000000 rds-core-0.0.11/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      142 2023-04-25 00:29:32.000000 rds-core-0.0.11/rds_core.egg-info/requires.txt
+-rw-r--r--   0 kelso     (1000) kelso     (1000)        9 2023-04-25 00:29:32.000000 rds-core-0.0.11/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 kelso     (1000) kelso     (1000)      105 2023-04-25 00:29:32.993390 rds-core-0.0.11/setup.cfg
+-rw-r--r--   0 kelso     (1000) kelso     (1000)     2254 2023-04-25 00:28:49.000000 rds-core-0.0.11/setup.py
```

### Comparing `rds-core-0.0.10/PKG-INFO` & `rds-core-0.0.11/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.0.10
+Version: 0.0.11
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: UNKNOWN
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: rds,framework,cache,config,helper,searchengine
@@ -12,12 +12,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `rds-core-0.0.10/README.md` & `rds-core-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/cache/__init__.py` & `rds-core-0.0.11/rds_core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/cache/base.py` & `rds-core-0.0.11/rds_core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/cache/nocache.py` & `rds-core-0.0.11/rds_core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/cache/search_engine.py` & `rds-core-0.0.11/rds_core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/helpers/__init__.py` & `rds-core-0.0.11/rds_core/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/helpers/http_client.py` & `rds-core-0.0.11/rds_core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core/searchengine/__init__.py` & `rds-core-0.0.11/rds_core/searchengine/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.10/rds_core.egg-info/PKG-INFO` & `rds-core-0.0.11/rds_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.0.10
+Version: 0.0.11
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: UNKNOWN
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: rds,framework,cache,config,helper,searchengine
@@ -12,12 +12,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `rds-core-0.0.10/setup.py` & `rds-core-0.0.11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,30 +35,32 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.0.10",
+    version="0.0.11",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
     keywords=["rds", "framework", "cache", "config", "helper", "searchengine"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.7",
     install_requires=requirements,
     packages=[
         "rds_core",
         "rds_core.cache",
```

