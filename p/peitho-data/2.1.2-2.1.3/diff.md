# Comparing `tmp/peitho_data-2.1.2.tar.gz` & `tmp/peitho_data-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.1.2.tar", last modified: Wed Nov  9 03:31:53 2022, max compression
+gzip compressed data, was "peitho_data-2.1.3.tar", last modified: Tue Apr 25 08:49:09 2023, max compression
```

## Comparing `peitho_data-2.1.2.tar` & `peitho_data-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 03:31:53.320085 peitho_data-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-09 03:31:52.000000 peitho_data-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-11-09 03:31:53.320085 peitho_data-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4684 2022-11-09 03:31:52.000000 peitho_data-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 03:31:53.320085 peitho_data-2.1.2/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (121)   333612 2022-11-09 03:31:52.000000 peitho_data-2.1.2/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 03:31:52.000000 peitho_data-2.1.2/peitho_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-11-09 03:31:52.000000 peitho_data-2.1.2/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-11-09 03:31:52.000000 peitho_data-2.1.2/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 03:31:53.320085 peitho_data-2.1.2/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-09 03:31:53.000000 peitho_data-2.1.2/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-09 03:31:53.320085 peitho_data-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-11-09 03:31:52.000000 peitho_data-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 08:49:08.000000 peitho_data-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 08:49:08.000000 peitho_data-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 08:49:09.555800 peitho_data-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 08:49:08.000000 peitho_data-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 08:49:09.555800 peitho_data-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 08:49:09.000000 peitho_data-2.1.3/setup.py
```

### Comparing `peitho_data-2.1.2/README.md` & `peitho_data-2.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 <div align="right">
 
 [![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-orange.svg)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 
 </div>
 
 
-What is Peitho Data
+What is Peitho Data <sup>![Python Version Badge is Missing](https://img.shields.io/badge/Python-3.10-brightgreen?style=flat-square&logo=python&logoColor=white)</sup>
 -------------------
 
 <a href="https://www.bilibili.com/video/BV1kb4y1m7e7?p=3">
     <img align="right" width="50%" alt="永恒" src="./theme/永恒.gif">
 </a>
 
 [Peitho Data](https://qubitpi.github.io/peitho-data/) is an opinionated **data analytics** package that team can
```

#### html2text {}

```diff
@@ -43,16 +43,18 @@
        sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-
            data&metric=sqale_rating)](https://sonarcloud.io/summary/
 new_code?id=QubitPi_peitho-data) [![Security Rating](https://sonarcloud.io/api/
   project_badges/measure?project=QubitPi_peitho-data&metric=security_rating)]
         (https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
          [![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-
     orange.svg)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
-What is Peitho Data ------------------- [æ°¸æ] [Peitho Data](https://
-qubitpi.github.io/peitho-data/) is an opinionated **data analytics** package
-that team can leverage to quickly incorporate capabilities of * Data Analytics/
-Visualization * Machine Learning * AI Documentation -------------
-[é·çµå°å.png] [Start exploring Peitho Data](https://qubitpi.github.io/
-peitho-data/) License ------- The use and distribution terms for [Peitho Data]
-(https://qubitpi.github.io/peitho-data/) are covered by the [Apache License,
-Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
+What is Peitho Data ![Python Version Badge is Missing](https://img.shields.io/
+badge/Python-3.10-brightgreen?style=flat-square&logo=python&logoColor=white) --
+----------------- [æ°¸æ] [Peitho Data](https://qubitpi.github.io/peitho-data/
+) is an opinionated **data analytics** package that team can leverage to
+quickly incorporate capabilities of * Data Analytics/Visualization * Machine
+Learning * AI Documentation ------------- [é·çµå°å.png] [Start exploring
+Peitho Data](https://qubitpi.github.io/peitho-data/) License ------- The use
+and distribution terms for [Peitho Data](https://qubitpi.github.io/peitho-data/
+) are covered by the [Apache License, Version 2.0](http://www.apache.org/
+licenses/LICENSE-2.0.html).
                             [License_Illustration]
```

### Comparing `peitho_data-2.1.2/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.1.3/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.2/peitho_data/trello_api.py` & `peitho_data-2.1.3/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.2/peitho_data/word_cloud.py` & `peitho_data-2.1.3/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.2/setup.py` & `peitho_data-2.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="peitho_data",
-    version="2.1.2",
+    version="2.1.3",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=["peitho_data"],
     python_requires='>=3.10',
@@ -14,12 +14,13 @@
         "bs4",
         "wordcloud",
         "pycodestyle",
         "requests",
         "sphinx-rtd-theme",
         "matplotlib",
         "ebooklib",
-        "networkx"
+        "networkx",
+        "requests_mock"
     ],
     zip_safe=False,
     include_package_data=True
 )
```

