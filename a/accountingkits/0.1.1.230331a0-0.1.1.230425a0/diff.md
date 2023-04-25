# Comparing `tmp/accountingkits-0.1.1.230331a0.tar.gz` & `tmp/accountingkits-0.1.1.230425a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accountingkits-0.1.1.230331a0.tar", last modified: Fri Mar 31 15:24:19 2023, max compression
+gzip compressed data, was "accountingkits-0.1.1.230425a0.tar", last modified: Tue Apr 25 07:48:03 2023, max compression
```

## Comparing `accountingkits-0.1.1.230331a0.tar` & `accountingkits-0.1.1.230425a0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.795380 accountingkits-0.1.1.230331a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.787380 accountingkits-0.1.1.230331a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.github/workflows/publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/accountingkits.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/other.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-31 15:24:19.795380 accountingkits-0.1.1.230331a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits/CrawlerApi/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/CrawlerApi/ApiT.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/CrawlerApi/CrawlerT.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/CrawlerApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/FuzzyMatchT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/NaDupOutlierT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/ReaderT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/SliceSelectT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/StringT.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits/OSKit/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/OSKit/DirectoryT.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/OSKit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/Stats/SummarizeT.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/Stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.795380 accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/JsonConverterT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/WayBackT.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.795380 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/ArrayLikeT.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/DecoratorT.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/MultiprocessT.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/UniversalBasicT.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/accountingkits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-31 15:24:19.000000 accountingkits-0.1.1.230331a0/accountingkits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:24:19.791381 accountingkits-0.1.1.230331a0/accountingkits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-31 15:24:19.000000 accountingkits-0.1.1.230331a0/accountingkits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-31 15:24:19.000000 accountingkits-0.1.1.230331a0/accountingkits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:24:19.000000 accountingkits-0.1.1.230331a0/accountingkits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 15:24:19.000000 accountingkits-0.1.1.230331a0/accountingkits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-31 15:24:11.000000 accountingkits-0.1.1.230331a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-31 15:24:19.795380 accountingkits-0.1.1.230331a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.github/workflows/publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/accountingkits.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/other.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/accountingkits/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/accountingkits/CrawlerApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/CrawlerApi/ApiT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/CrawlerApi/CrawlerT.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/CrawlerApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/
+-rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/FuzzyMatchT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/NaDupOutlierT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/ReaderT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/SliceSelectT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/StringT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/accountingkits/OSKit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/OSKit/DirectoryT.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/OSKit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/accountingkits/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/Stats/SummarizeT.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/Stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/WayBackT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/ArrayLikeT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/DecoratorT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/MultiprocessT.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/UniversalBasicT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/accountingkits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 07:48:03.000000 accountingkits-0.1.1.230425a0/accountingkits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:48:03.373793 accountingkits-0.1.1.230425a0/accountingkits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-25 07:48:03.000000 accountingkits-0.1.1.230425a0/accountingkits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 07:48:03.000000 accountingkits-0.1.1.230425a0/accountingkits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:48:03.000000 accountingkits-0.1.1.230425a0/accountingkits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 07:48:03.000000 accountingkits-0.1.1.230425a0/accountingkits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 07:47:53.000000 accountingkits-0.1.1.230425a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-25 07:48:03.377793 accountingkits-0.1.1.230425a0/setup.cfg
```

### Comparing `accountingkits-0.1.1.230331a0/LICENSE` & `accountingkits-0.1.1.230425a0/LICENSE`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/PKG-INFO` & `accountingkits-0.1.1.230425a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accountingkits
-Version: 0.1.1.230331a0
+Version: 0.1.1.230425a0
 Summary: The kit-package which made for accounting science research
 Home-page: https://github.com/qihangZH/accountingkits
 Author: zhang qihang
 Author-email: 694499657@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `accountingkits-0.1.1.230331a0/README.md` & `accountingkits-0.1.1.230425a0/README.md`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/CrawlerApi/ApiT.py` & `accountingkits-0.1.1.230425a0/accountingkits/CrawlerApi/ApiT.py`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/FuzzyMatchT.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/FuzzyMatchT.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,75 +30,68 @@
             f"querying_listarr {sum(pd.Series(querying_listarr).isna())} NA," +
             f" choice_list {sum(pd.Series(choice_list).isna())} NA"
         )
     
     if np.any(pd.Series(choice_list).duplicated()):
         raise ValueError('Error:there are duplicated in choice list, may cause confusing result')
     """
+    # 230415-> New version would detect the querying array's duplications, for better use may need to merge
+    #          instead of to concat...
+    if np.any(pd.Series(querying_listarr).duplicated()) or np.any(pd.Series(querying_listarr).isna()):
+        print(
+            "\nDuplicates or Null/Na in querying are detected and automatically removed\n"
+        )
+        querying_listarr = pd.Series(querying_listarr).dropna().drop_duplicates().to_list()
 
-    if np.any(pd.Series(querying_listarr).isna()):
-        raise ValueError("\033[31mNull/Na in querying list may cause confounding\033[0m")
+    # if np.any(pd.Series(querying_listarr).isna()):
+    #     raise ValueError("\033[31mNull/Na in querying list may cause confounding\033[0m")
 
     if np.any(pd.Series(choice_list).duplicated()) or np.any(pd.Series(choice_list).isna()):
         print(
             "\nDuplicates or Null/Na in choices are detected and automatically removed\n"
         )
         choice_list = pd.Series(choice_list).dropna().drop_duplicates().to_list()
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
 
     # set constants
     """CONSTANTS CAN NOT BE CHANGED"""
-    CONST_querying_listarr = pd.Series(querying_listarr).astype(str).tolist()
+    CONST_querying_list = pd.Series(querying_listarr).astype(str).tolist()
     CONST_choice_list = pd.Series(choice_list).astype(str).tolist()
 
     def __LAMBDA_taskof_list_fuzzymatching_list_tuple(identifier):
         """
         :param identifier:identifier
         :return: results tuple
         """
         value = thefuzz.process.extractOne(
-            query=CONST_querying_listarr[identifier],
+            query=CONST_querying_list[identifier],
             choices=CONST_choice_list,
             scorer=scorer
         )
         return (value, identifier)
 
-    """Dropped, for even slower then npapply and totally unstable, WRONG OUTPUTS MOSTTIMES"""
-
-    # def __LAMBDA_taskof_list_rapidFM_list_tuple(identifier):
-    #     """
-    #     :param identifier:identifier
-    #     :return: results tuple
-    #     """
-    #     value = rapidfuzz.process.extractOne(query=CONST_querying_listarr[identifier],
-    #                                         #Only Choose first two rows
-    #                                          choices=CONST_choice_list,
-    #                                          scorer=scorer
-    #                                          )[:2]
-    #     return (value,identifier)
-
     def __LAMBDA_taskof_list_difflibmatching_list_tuple(identifier):
         """
         :param identifier:
         :return:
         """
-        temp_input = CONST_querying_listarr[identifier]
+        temp_input = CONST_querying_list[identifier]
         match_result = difflib.get_close_matches(word=temp_input, possibilities=CONST_choice_list, n=1)
         if match_result == []:
             match_result = ''
         else:
             match_result = match_result[0]
         match_scores = difflib.SequenceMatcher(None, match_result, temp_input).ratio()
         #  *100
         value = (match_result, match_scores)
 
         return (value, identifier)
 
     if method == 'npapply':
-        npapply_query_arr = np.array(CONST_querying_listarr)[:, np.newaxis]
+        npapply_query_arr = np.array(CONST_querying_list)[:, np.newaxis]
 
         time_start = time.time()
         npapply_match_result_mat = np.apply_along_axis(
             func1d=lambda x: thefuzz.process.extractOne(query=x[0], choices=CONST_choice_list, scorer=scorer),
             arr=npapply_query_arr, axis=1)
         time_end = time.time()
         print('list_fuzzymatching_list method {} time cost'.format(method), time_end - time_start, 's')
@@ -122,17 +115,17 @@
         with pathos.multiprocessing.Pool(
                 # for safer exception in multiprocess
                 initializer=_BasicTools.MultiprocessT.threads_interrupt_initiator
         ) as pool:
             for result in tqdm.tqdm(
                     pool.imap_unordered(
                         _temp_loop_function,
-                        range(len(CONST_querying_listarr))
+                        range(len(CONST_querying_list))
                     ),
-                    total=len(CONST_querying_listarr)
+                    total=len(CONST_querying_list)
             ):
                 temp_matching_list.append(result[0][0])
                 temp_score_list.append(result[0][1])
                 temp_identifier_list.append(result[1])
 
         #  In after place match mean result from choice list
         mp_match_result_df = pd.DataFrame(
@@ -146,37 +139,41 @@
         mp_match_result_df = mp_match_result_df.sort_values(by='identifier', ascending=True)
         match_result_df = mp_match_result_df[['match_list', 'match_score']].reset_index().copy()
         del match_result_df['index']
 
     elif method == 'rapidfuzz_cdist':
         """SuperFast Cpp Matrix method for matching result"""
         time_start = time.time()
-        matchscores_total_mat = rapidfuzz.process.cdist(queries=CONST_querying_listarr,
+        matchscores_total_mat = rapidfuzz.process.cdist(queries=CONST_querying_list,
                                                         scorer=scorer,
                                                         choices=CONST_choice_list,
                                                         workers=-1)
         matchscores_position_arr = np.nanargmax(matchscores_total_mat, axis=1)
         # In after place match mean result from choice list
         match_result_df = pd.DataFrame(
             {
                 'match_list': np.array(CONST_choice_list)[matchscores_position_arr],
-                'match_score': matchscores_total_mat[np.arange(len(CONST_querying_listarr)),
+                'match_score': matchscores_total_mat[np.arange(len(CONST_querying_list)),
                 matchscores_position_arr],
             }
         )
         time_end = time.time()
         print('list_fuzzymatching_list method {} time cost'.format(method), time_end - time_start, 's')
     else:
         raise ValueError('Wrong method of iteration')
 
     match_result_df = match_result_df.copy()
+
+    # New idea: put the origin data in a result df column
+    match_result_df['origin_query'] = np.array(CONST_querying_list)
+
     match_result_df['match_score'] = match_result_df['match_score'].astype(float)
     # make 0~100%
-    if np.all((match_result_df['match_score'].values >= 0) &
-              (match_result_df['match_score'].values <= 1)):
+    if np.all((match_result_df['match_score'].to_numpy() >= 0) &
+              (match_result_df['match_score'].to_numpy() <= 1)):
         match_result_df['match_score'] = np.multiply(match_result_df['match_score'], 100)
         print(f'method {method},scorer {scorer} has *100 their scores')
 
     return match_result_df
 
 
 # ----------------------------------------------------------------------------------------------------------------------
@@ -196,17 +193,25 @@
     :param scorer: the scorer of fuzzymatch, it could be changed to different result,
             classic normalized_levenshtein be fuzz.ratio,however be useless in difflib method
     :return: result dataframe
     """
 
     # 0.1.1.230205_alpha-> new version only check the n.a. of query list, automatically remove choices duplicates/na >>>
 
-    # add this only for not raise Value-error after running long-time script
-    if np.any(pd.Series(querying_listarr).isna()):
-        raise ValueError("\033[31mAuto Function->Null/Na in querying list may cause confounding\033[0m")
+    # # add this only for not raise Value-error after running long-time script
+    # if np.any(pd.Series(querying_listarr).isna()):
+    #     raise ValueError("\033[31mAuto Function->Null/Na in querying list may cause confounding\033[0m")
+
+    # 230415-> New version would detect the querying array's duplications, for better use may need to merge
+    #          instead of to concat...
+    if np.any(pd.Series(querying_listarr).duplicated()) or np.any(pd.Series(querying_listarr).isna()):
+        print(
+            "\nDuplicates or Null/Na in querying are detected and automatically removed\n"
+        )
+        querying_listarr = pd.Series(querying_listarr).dropna().drop_duplicates().to_list()
 
     # add this to avoid waste of performance and consistency
     if np.any(pd.Series(choice_list).duplicated()) or np.any(pd.Series(choice_list).isna()):
         print(
             "\nDuplicates or Null/Na in choices are detected and automatically removed\n"
         )
         choice_list = pd.Series(choice_list).dropna().drop_duplicates().to_list()
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/NaDupOutlierT.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/NaDupOutlierT.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,50 @@
     na_percentage = sum(pd.isna(temp_ser)) / temp_len
     return na_percentage
 
 
 def remove_duplicate_na_arr(listarrser):
     """remove the duplicate obs and NA obs"""
     temp_ser = pd.Series(listarrser).drop_duplicates().dropna()
-    return temp_ser.values
+    return temp_ser.to_numpy()
 
 
-def latent_na_detector_bool_arr(listarrser, na_regex, case, is_detect_explicit_na: bool):
+def latent_na_detector_bool_arr(listarrser,
+                                na_regex,
+                                case,
+                                is_detect_explicit_na: bool,
+                                is_specify_zerolen_na: bool
+                                ):
     """
-    detect latent na, like spaces or comma
-    :param is_detect_explicit_na: bool, True for detect explicit na, False for not detect
+    detect latent na, like spaces or comma, only works for data which type is str
     :param listarrser: input
     :param na_regex: regex
     :param case: If True, case sensitive.
+    :param is_detect_explicit_na: bool, True for detect explicit na, False for not detect
+    :param is_specify_zerolen_na: bool, True for set zero length str as NA
     :return: bool array
     """
-    if not isinstance(is_detect_explicit_na,bool):
-        raise ValueError('is_detect_explicit_na only input for True or False')
+    if (not isinstance(is_detect_explicit_na, bool)) | (not isinstance(is_specify_zerolen_na, bool)):
+        raise ValueError('is_detect_explicit_na/is_specify_zerolen_na only input for True or False')
 
-    na_detect_arr = pd.Series(listarrser).str.match(
-        pat='^((,)|(\.)|( ))*('+na_regex+'){1}((,)|(\.)|( ))*$',
+    # fullmatch contains match works same here, Actually we need fullmatch here, however do not change
+    na_detect_arr = pd.Series(listarrser).astype(str).str.match(
+        # old version:
+        # pat='^((,)|(\.)|( ))*('+na_regex+'){1}((,)|(\.)|( ))*$',
+        pat=fr'^((,)|(\.)|(\s)|(;)|(\|))*({na_regex})?((,)|(\.)|(\s)|(;)|(\|))*$',
         case=case,
         na=is_detect_explicit_na  # substitute explicit n.a. with True/False
-    ).values
+    ).to_numpy()
+
+    # besides, we add another way to detect: string length==0 means na
+    if is_specify_zerolen_na:
+        zero_len_detect_arr = (pd.Series(listarrser).astype(str).apply(len) == 0).to_numpy()
+
+        # both of them detect the need anwser.
+        na_detect_arr = na_detect_arr | zero_len_detect_arr
 
     return na_detect_arr
 
 
 def auto_substituite_duplicates_bychoices_arr(duplicates_listarrser, choice_listarrser,
                                               duplicate_keep: typing.Literal['first', 'last', False]):
     """
@@ -57,28 +73,28 @@
 
     if pd.Series(duplicates_arr).nunique() != len(duplicates_arr):
         print('duplicates_listarrser has no duplicates')  # check duplicates
         return duplicates_arr
 
     if not (duplicate_keep is None):  # loop
         # Initialize
-        temp_duplicates_boolean_arr = pd.Series(duplicates_arr).duplicated(keep=duplicate_keep).values
+        temp_duplicates_boolean_arr = pd.Series(duplicates_arr).duplicated(keep=duplicate_keep).to_numpy()
         temp_nodup_remove_suffix_arr = copy.deepcopy(duplicates_arr)
         temp_nodup_remove_suffix_arr[temp_duplicates_boolean_arr] = choice_arr[temp_duplicates_boolean_arr]
         # other arguments
         _temp_loop_count = 0
         _temp_keep = duplicate_keep
         _temp_duplicate_count = sum(temp_duplicates_boolean_arr)
         print(f'Initialize autorestore duplicates last for:{sum(temp_duplicates_boolean_arr)},\n')
         # deal with duplicates
         while pd.Series(temp_nodup_remove_suffix_arr).nunique() != len(temp_nodup_remove_suffix_arr):
 
             last_loop_arr = temp_nodup_remove_suffix_arr
             temp_duplicates_boolean_arr = pd.Series(last_loop_arr
-                                                    ).duplicated(keep=_temp_keep).values
+                                                    ).duplicated(keep=_temp_keep).to_numpy()
             temp_nodup_remove_suffix_arr = copy.deepcopy(last_loop_arr)
             temp_nodup_remove_suffix_arr[temp_duplicates_boolean_arr] = choice_arr[temp_duplicates_boolean_arr]
             _temp_loop_count += 1
             # check if in INFINITE LOOP: IF same, means last time dealing is meaningless
             if _temp_duplicate_count == sum(temp_duplicates_boolean_arr):
                 if _temp_keep != False:
                     print('To stop infinite loop, change to False')
@@ -95,25 +111,31 @@
         raise ValueError('duplicate_keep can not be None, please reset')
 
 
 # -----------------------------------------------------------------------------------------
 # """level1 Complex DataPrepare Functions"""#################################################
 # -----------------------------------------------------------------------------------------
 
-def l1_latent_na_substitute_arr(listarrser, na_regex, case, substitute_value, is_detect_explicit_na):
+def l1_latent_na_substitute_arr(listarrser, na_regex, case,
+                                substitute_value: bool,
+                                is_detect_explicit_na: bool,
+                                ):
     """
     detect latent na, like spaces or comma, and substitute the whole element
-    :param is_detect_explicit_na: bool, True for substitute explicit na, False for not substitute explicit na
-    :param substitute_value: the substitute value to replace the detected na
     :param listarrser: input
     :param na_regex: regex
     :param case: If True, case sensitive.
+    :param is_detect_explicit_na: bool, True for substitute explicit na, False for not substitute explicit na
+    :param substitute_value: the substitute value to replace the detected na
+    :param is_detect_explicit_na: bool, True for set zero length str as NA
     :return: bool array
     """
     detect_arr = latent_na_detector_bool_arr(listarrser=listarrser,
                                              na_regex=na_regex,
                                              case=case,
-                                             is_detect_explicit_na=is_detect_explicit_na)
+                                             is_detect_explicit_na=is_detect_explicit_na,
+                                             is_specify_zerolen_na=is_detect_explicit_na
+                                             )
     temp_arr = copy.deepcopy(np.array(listarrser))
     # before change, first copy
     temp_arr[detect_arr] = substitute_value
     return temp_arr
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/ReaderT.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/ReaderT.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 import pandas as pd
 import sas7bdat
+import chardet
+
+
+def find_file_encoding(path):
+    """
+    find the encoding of target file(data or other else)
+    more details could be seen: https://chardet.readthedocs.io/en/latest/usage.html;
+    https://stackoverflow.com/questions/12468179/unicodedecodeerror-utf8-codec-cant-decode-byte-0x9c
+    :param path: the path of file which encoding should be detected, the type will return as string.
+    """
+    with open(path, 'rb') as file:
+        result = chardet.detect(file.read())
+
+    return result['encoding']
 
 
 def harte_hanks_txt_reader_2019_2021_df(PATH, **kwargs):
     """encoding='ISO-8859-1
     :param kwargs: other arguments should be passed to pd.read_csv()
     '"""
-    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="ISO-8859-1", low_memory=False, **kwargs)
+    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="ISO-8859-1", **kwargs)
     return temp_df
 
 
 def harte_hanks_txt_reader_2017_2018_df(PATH, **kwargs):
     """encoding='UTF-16'
     :param kwargs: other arguments should be passed to pd.read_csv()
     """
-    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="UTF-16", low_memory=False, **kwargs)
+    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="UTF-16", **kwargs)
     return temp_df
 
 
 def harte_hanks_txt_reader_2016_df(PATH, **kwargs):
     """encoding='ISO-8859-1'
     :param kwargs: other arguments should be passed to pd.read_csv()
     """
-    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="ISO-8859-1", low_memory=False, **kwargs)
+    temp_df = pd.read_csv(filepath_or_buffer=PATH, encoding="ISO-8859-1", **kwargs)
     return temp_df
 
 
 def harte_hanks_txt_reader_1996_2015_df(PATH, **kwargs):
     """encoding='ISO-8859-1'
     :param kwargs: other arguments should be passed to pd.read_csv()
     """
     temp_df = pd.read_csv(
-        filepath_or_buffer=PATH, encoding="ISO-8859-1", sep='\t', low_memory=False, **kwargs
+        filepath_or_buffer=PATH, encoding="ISO-8859-1", sep='\t', **kwargs
     )
     return temp_df
 
 
 def sas7bdat_reader_df(path, **kwargs):
     """
     read .sas7bdat data by sas7bdat.SAS7BDAT
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/SliceSelectT.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/SliceSelectT.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import numpy as np
 import pandas as pd
 
 
 def sic4_fininst_select_bool_arr(listarrser):
     # 2022/12/15
-    # temp_arr = pd.Series(listarrser).astype('int32').values
+    # temp_arr = pd.Series(listarrser).astype('int32').to_numpy()
     # Set again:
     # pandas.errors.IntCastingNaNError: Cannot convert non-finite values (NA or inf) to integer
     temp_ser = pd.Series(listarrser).copy()
     bool_not_na_ser = ~(temp_ser.isna())
     temp_ser[bool_not_na_ser] = (temp_ser[bool_not_na_ser]).apply('int32')
 
-    bool_arr = (np.greater_equal(temp_ser.values, 6000) & np.less_equal(temp_ser.values, 6999))
+    bool_arr = (np.greater_equal(temp_ser.to_numpy(), 6000) & np.less_equal(temp_ser.to_numpy(), 6999))
     return bool_arr
 
 
 def naic6_fininst_select_bool_arr(listarrser):
     # Set again:
     # pandas.errors.IntCastingNaNError: Cannot convert non-finite values (NA or inf) to integer
     temp_ser = pd.Series(listarrser).copy()
     bool_not_na_ser = ~(temp_ser.isna())
     temp_ser[bool_not_na_ser] = (temp_ser[bool_not_na_ser]).apply('int32')
 
-    bool_arr = (np.greater_equal(temp_ser.values, 520000) & np.less_equal(temp_ser.values, 529999))
+    bool_arr = (np.greater_equal(temp_ser.to_numpy(), 520000) & np.less_equal(temp_ser.to_numpy(), 529999))
     return bool_arr
 
 
 def int_rangeselect_bool_arr(listarrser, floor: int, ceil: int,
                              include_floor_bool: bool,
                              include_ceil_bool: bool
                              ):
@@ -49,15 +49,15 @@
     temp_ceil_func = np.less_equal if include_ceil_bool else np.less
     # Set again:
     # pandas.errors.IntCastingNaNError: Cannot convert non-finite values (NA or inf) to integer
     temp_ser = pd.Series(listarrser).copy()
     bool_not_na_ser = ~(temp_ser.isna())
     temp_ser[bool_not_na_ser] = (temp_ser[bool_not_na_ser]).apply('int32')
 
-    bool_arr = (temp_floor_func(temp_ser.values, floor) & temp_ceil_func(temp_ser.values, ceil))
+    bool_arr = (temp_floor_func(temp_ser.to_numpy(), floor) & temp_ceil_func(temp_ser.to_numpy(), ceil))
     return bool_arr
 
 
 # -----------------------------------------------------------------------------------------
 # """L1 Complex DataPrepare Functions"""#######################################################
 # -----------------------------------------------------------------------------------------
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/StringT.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/StringT.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,42 @@
     """
 
     # examine
     if (suffix_regex == '') or (not isinstance(suffix_regex, str)):
         raise ValueError('suffix_regex must be string and should not be ""')
 
     # core part
+
+    # old version >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+
+    # temp_remove_suffix_arr = pd.Series(listarrser).astype(str).str.replace(
+    #     '(' + suffix_regex + '){1}$', repl='', regex=True, **kwargs).to_numpy()
+
+    # old version <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+
+    # new version 2023/04/01 >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+    """
+    New version could use better regex
+    For it could safely use...
+    """
     temp_remove_suffix_arr = pd.Series(listarrser).astype(str).str.replace(
-        '(' + suffix_regex + '){1}$', repl='', regex=True, **kwargs).values
+        fr"({suffix_regex})$",
+        repl='',
+        regex=True,
+        **kwargs).to_numpy()
+    # new version <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
 
     return temp_remove_suffix_arr
 
 
 def extract_prefix_arr(listarrser, prefix_regex):
     """extract prefix by regex"""
-    temp_extract_arr = listarrser.astype(str).str.extract(
-        f'(^{prefix_regex}).*$', expand=False
-    ).values  # choose
+    temp_extract_arr = pd.Series(listarrser).astype(str).str.extract(
+        fr'(^{prefix_regex}).*$', expand=False
+    ).to_numpy()  # choose
 
     return temp_extract_arr
 
 
 def restore_leading_zeros_str_arr(listarrser, target_len):
     """
     Restore the lost leading zeros of the int/zeros list/arr/ser
@@ -48,15 +65,15 @@
         raise ValueError('Input array like should be int elements, or int strings')
 
     if np.nanmax(temp_string_ser.apply(len)) > target_len:
         raise ValueError('The max length of elements bigger than target length')
 
     dealed_string_arr = temp_string_ser.apply(
         lambda x: '0' * (target_len - len(x)) + x
-    ).values
+    ).to_numpy()
     return dealed_string_arr
 
 
 # -----------------------------------------------------------------------------------------
 # """L1 Complex DataPrepare Functions"""#######################################################
 # -----------------------------------------------------------------------------------------
 def l1_suffix_and_around_remove_arr(listarrser, suffix_regex: str, around_regex: str = '', **kwargs):
@@ -74,22 +91,29 @@
     # examine
     if (suffix_regex == '') or (not isinstance(suffix_regex, str)):
         raise ValueError('suffix_regex must be string and should not be ""')
 
     # core part
     if around_regex == '':
         # temp_remove_suffix_arr = pd.Series(listarrser).astype(str).str.replace(
-        #     '(' + suffix_regex + '){1}$', repl='', case=case, regex=True).values
+        #     '(' + suffix_regex + '){1}$', repl='', case=case, regex=True).to_numpy()
         temp_remove_suffix_arr = suffix_remove_arr(
             listarrser=listarrser,
             suffix_regex=suffix_regex,
             **kwargs
         )
     else:
+        # temp_remove_suffix_arr = pd.Series(listarrser).astype(str).str.replace(
+        #     f'({around_regex})*' + '(' + suffix_regex + '){1}' + f'({around_regex})*$',
+        #     repl='',
+        #     regex=True,
+        #     **kwargs
+        # ).to_numpy()
+
         temp_remove_suffix_arr = pd.Series(listarrser).astype(str).str.replace(
-            f'({around_regex})*' + '(' + suffix_regex + '){1}' + f'({around_regex})*$',
+            fr'({around_regex})*({suffix_regex})({around_regex})*$',
             repl='',
             regex=True,
             **kwargs
-        ).values
+        ).to_numpy()
 
     return temp_remove_suffix_arr
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/DataPrepare/__init__.py` & `accountingkits-0.1.1.230425a0/accountingkits/DataPrepare/__init__.py`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/OSKit/DirectoryT.py` & `accountingkits-0.1.1.230425a0/accountingkits/OSKit/DirectoryT.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,59 +23,67 @@
         temp_folder_maker(check_make_dir)
 
         print('Make dir:{}'.format(check_make_dir))
     else:
         print('{} already exist.'.format(check_make_dir))
 
 
-def dir_colnames_df(read_df_func, read_dir, suffix_regex: str, **kwargs):
+def dir_colnames_df(read_df_func, read_dir, suffix_regex: str | None = None, **kwargs):
     """
     To show the colnames of Each DF in a dir, summary in to an DF
 
     :param read_df_func: the function to read the datas in the dir, function(dir+names),
         equally function(path), however,read_function must return pd.DataFrame...
     :param read_dir: the directory of the datas saved
     :param suffix_regex: suffix regex to search for files, however, should be type in "regex" to search.
         if you need to set Nothing, then simply use '', None, etc...
-    :param kwargs: other arguments for suffix regex detect file names which pandas.Series.str.contains() use, see:
-        https://pandas.pydata.org/docs/reference/api/pandas.Series.str.contains.html,
+    :param kwargs: other arguments for suffix regex detect file names which pandas.Series.str.fullmatch() use, see:
+        https://pandas.pydata.org/docs/reference/api/pandas.Series.str.fullmatch.html,
         however, regex=True,pat=patterns(special) can not be modified.
     :return: dataframe of output cols
     """
     colname_dict = {}
     colname_len_dict = {}
 
     file_arr = np.array(os.listdir(read_dir))
 
     # if we are sure that the suffix regex is string, then set it to suffix check.
-    try:
-        if (len(suffix_regex) != 0) and (isinstance(suffix_regex, str)):
-            pattern = '^.*(' + suffix_regex + '){1}$'
-            temp_choose_arr = pd.Series(file_arr).str.contains(
-                pat=pattern, regex=True, **kwargs
-            ).values
-            file_arr = file_arr[temp_choose_arr]
-        else:
-            print('\033[31mfail in suffix regex using, \nhowever pass file suffix detecting, use all files\033[0m')
-    except Exception as e:
-        print(f'\033[31m{e} occurs in suffix regex using, \nhowever pass file suffix detecting, use all files\033[0m')
+
+    if pd.Series([suffix_regex]).isna().to_numpy()[0]:  # check if the regex input is None
+
+        print('\033[31mfail in suffix regex using, use all files in dir\033[0m')
+
+    elif (len(suffix_regex) != 0) and (isinstance(suffix_regex, str)):
+
+        # pattern = '^.*(' + suffix_regex + '){1}$'
+
+        """new version pattern"""
+        pattern = fr'^.*({suffix_regex})$'
+
+        temp_choose_arr = pd.Series(file_arr).str.fullmatch(
+            pat=pattern, **kwargs
+        ).to_numpy()
+        file_arr = file_arr[temp_choose_arr]
+
+    else:
+        print('\033[31mfail in suffix regex using, use all files in dir\033[0m')
 
     # print the detect result of the function...
     print('FILENAMES:\n', file_arr)
 
     # get read_sample to ensure the readfunc return dataframe
     read_sample = read_df_func(read_dir + file_arr[0])
     if not isinstance(read_sample, pd.DataFrame):
         raise ValueError('read_function must return pandas.Dataframe, '
                          f'However, your read_function return {type(read_sample)}'
                          'reset read function!')
 
     for i in file_arr:
         # read each
-        colname_dict[i] = read_df_func(read_dir + i).columns.values
+        colname_dict[i] = read_df_func(read_dir + i).columns.to_numpy()
         colname_len_dict[i] = len(colname_dict[i])
     for i in file_arr:
         colname_dict[i] = _BasicTools.ArrayLikeT.repunit_append_arr(
             target_len=max(colname_len_dict.values()),
             listarrser=colname_dict[i],
             repunit=np.nan)
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/Stats/SummarizeT.py` & `accountingkits-0.1.1.230425a0/accountingkits/Stats/SummarizeT.py`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/LICENSE` & `accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/LICENSE`

 * *Files identical despite different names*

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/WaybackScraper/WayBackT.py` & `accountingkits-0.1.1.230425a0/accountingkits/WaybackScraper/WayBackT.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from urllib.parse import urljoin
 from collections import Counter
 from nltk.corpus import stopwords
 from nltk.stem.porter import PorterStemmer
 from io import BytesIO
 
 import fake_useragent
+
 """
 Author: Romain Boulland, Thomas Bourveau, Matthias Breuer
 Date: Jun 24, 2021
 Code: Generate bag of words for a time-series of company websites
 
 * Please customize the config file before launching the program *
 
@@ -29,14 +30,16 @@
 
 """
 modified from origin files
 
 Author: Qihang Zhang in 2023/02/03,National University of Singapore,
 NUS Business School, Department of Accounting
 """
+
+
 # %% Macros
 # STATUS_CODE = config.status_code
 # MIME_TYPE = config.mime_type
 # HEADERS = config.headers
 # MAX_URL = config.max_url
 # MAX_SUB = config.max_sub
 # PARSER = config.parser
@@ -45,15 +48,15 @@
 # PATH = config.path
 
 
 class WayBack:
 
     def __init__(self, PATH, contact='youremail@domain.com', **kwargs):
         """
-        Modified from origin Romain Boulland, Thomas Bourveau, Matthias Breuer's work
+        Modified from origin Authors Romain Boulland, Thomas Bourveau, Matthias Breuer's work
         Author: Qihang Zhang in 2023/02/03,National University of Singapore,
         NUS Business School, Department of Accounting
         :param kwargs: useragent/alpha_token/word_len/stop_words/stemmer/STATUS_CODE/MIME_TYPE/
                         HEADERS/MAX_URL/MAX_SUB/PARSER/RAW/BOW_OPTIONS/PATH
                         see:https://github.com/r-boulland/Corporate-Website-Disclosure
         """
         # old-version -> new version, use random fake useragent instead of manuall input>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
@@ -71,15 +74,15 @@
         ).random
         if not ('useragent' in kwargs):
             print('\n', f'Automatically generate fake useragent:{useragent}', '\n')
 
         # Some Settings
         alpha_token = kwargs['alpha_token'] if 'alpha_token' in kwargs else True
 
-        word_len = kwargs['word_len'] if 'word_len' in kwargs else(1, 20)
+        word_len = kwargs['word_len'] if 'word_len' in kwargs else (1, 20)
 
         stop_words = kwargs['stop_words'] if 'stop_words' in kwargs else stopwords.words('english')
 
         stemmer = kwargs['stemmer'] if 'stemmer' in kwargs else PorterStemmer()
 
         # Arguments
 
@@ -135,19 +138,19 @@
             df['datetime'] = pd.to_datetime(df['timestamp'], format='%Y%m%d%H%M%S', errors='coerce')
             if df['datetime'].isnull().any():
                 df = df[df['datetime'].notnull()]
                 print('{} matches left after dropping invalid timestamps.'.format(df.shape[0]))
             # Search results cleaning: urlkey
             # Ensure uniqueness of urlkey, keep the shortest if not
             if df['urlkey'].nunique() > 1:
-                df = df[df['urlkey'] == sorted(df['urlkey'].values, key=len)[0]]
+                df = df[df['urlkey'] == sorted(df['urlkey'].to_numpy(), key=len)[0]]
                 print('Urlkey not unique, keep the shortest, {} matches left.'.format(df.shape[0]))
             # Complete url for archived websites (as stored on archive.org)
             df['url'] = ['https://web.archive.org/web' + '/' + t + '/' + o for t, o in
-                         zip(df['timestamp'].values, df['original'].values)]
+                         zip(df['timestamp'].to_numpy(), df['original'].to_numpy())]
             df.sort_values(['urlkey', 'datetime'], inplace=True)
             # Output a txt if specified
             return df
 
     @staticmethod
     def query_filter(df, freq, date_range=None):
         """
@@ -400,36 +403,121 @@
         df = self.wayback_query(host)
 
         # Break if no result found
         if df is None:
             return
 
         # Store the API query results
-        df.to_csv(path+'cdx['+re.sub(r'[^\w\s\-]', '_', host)+'].csv', index=False)
+        df.to_csv(path + 'cdx[' + re.sub(r'[^\w\s\-]', '_', host) + '].csv', index=False)
 
         # Aggregate query results at desired frequency
         df = self.query_filter(df, freq, date_range)
 
         # Scrape all URLs and their subs
         url_res_all = {}
-        for url in df['url'].values:
+        for url in df['url'].to_numpy():
             tree_res = self.tree_scrape(url, max_url=max_url, max_sub=max_sub)
             url_res_all[url] = tree_res
 
         # Store the time-series of scraped results
-        with open(path+'res['+re.sub(r'[^\w\s\-]', '_', host)+'].json', 'w') as f:
+        with open(path + 'res[' + re.sub(r'[^\w\s\-]', '_', host) + '].json', 'w') as f:
             json.dump(url_res_all, f)
 
         # Process scraped html texts
         args = bow_options.values()
         url_bow_all = {
             url: Counter(
                 itertools.chain(
                     *[self.text_tokenize(url_res['text'], *args) for url_res in tree_res]
                 )
             )
             for url, tree_res in url_res_all.items()
         }
 
         # Store the time-series of formed BoWs
-        with open(path+'bow[' + re.sub(r'[^\w\s\-]', '_', host)+'].json', 'w') as f:
+        with open(path + 'bow[' + re.sub(r'[^\w\s\-]', '_', host) + '].json', 'w') as f:
             json.dump(url_bow_all, f)
+
+    def wayback_scraper_text_df(self, host, freq, date_range=None, **kwargs):
+        """
+        Author: Qihang Zhang in 2023/04/22,National University of Singapore,
+        NUS Business School, Department of Accounting,
+
+        A modified function to process with the text scraper from wayback machine scraper
+
+        Main function
+        The function WaybackScraper() serves as the main function of the program.
+        It generates bag of words for a time-series of company websites.
+        :param host: website name
+        :param freq: frequency of time, see more in timedelta of pandas
+            https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
+        :param date_range: (str,str),default None Date (yyyy/mm/dd) range of URL search.
+        :param kwargs: max_url/max_sub
+        :return: DataFrame, contains url, error, text, suburl_list which contains found suburls, qurl
+        """
+        max_url = kwargs['max_url'] if 'max_url' in kwargs else self.MAX_URL
+
+        max_sub = kwargs['max_sub'] if 'max_sub' in kwargs else self.MAX_SUB
+
+        # Search all archives for the entered URL
+        df = self.wayback_query(host)
+
+        # Break if no result found
+        if df is None:
+            return
+
+        # Aggregate query results at desired frequency
+        df = self.query_filter(df, freq, date_range)
+
+        # Scrape all URLs and their subs
+        url_res_all_dict = {}
+        for url in df['url'].to_numpy():
+            tree_res = self.tree_scrape(url, max_url=max_url, max_sub=max_sub)
+            url_res_all_dict[url] = tree_res
+
+        # set the containers
+        chronicle_url_list = []
+        url_list = []
+        error_list = []
+        text_list = []
+        sub_url_list = []
+
+        # one chronic should have one subset
+        for c in url_res_all_dict.keys():
+            # chronic data list, this url is used for save the archive data of url
+            chronic_data_list = url_res_all_dict[c]
+            # there should be obs dicts in chronic data list
+            for obsdict in chronic_data_list:
+                chronicle_url_list.append(c)
+                url_list.append(obsdict['URL'])
+                error_list.append(obsdict['error'])
+                text_list.append(obsdict['text'])
+                sub_url_list.append(obsdict['subURLs'])
+
+        result_df = pd.DataFrame(
+            {
+                'chronicle_url': chronicle_url_list,
+                'url': url_list,
+                'error': error_list,
+                'text': text_list,
+                'suburls_list': sub_url_list  # this is actually a matrix
+            }
+        ).copy()
+
+        # From origin URL of chronical archive, we can get the
+        result_df['archive_chronicle'] = pd.to_datetime(
+            result_df['chronicle_url'].str.extract(
+                r'^https://web\.archive\.org/web/(\d+)/.*$', expand=False
+            ),
+            format="%Y%m%d%H%M%S"
+        )
+
+        result_df['url_date'] = pd.to_datetime(
+            result_df['url'].str.extract(
+                r'^https://web\.archive\.org/web/(\d+)/.*$', expand=False
+            ),
+            format="%Y%m%d%H%M%S"
+        )
+
+        result_df = result_df.drop(columns=['chronicle_url'])
+
+        return result_df
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits/_BasicTools/ArrayLikeT.py` & `accountingkits-0.1.1.230425a0/accountingkits/_BasicTools/ArrayLikeT.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     test all be same
     :return: bool, is all same or not all same
     """
     temp_df = pd.DataFrame({'ser1': listarrser1, 'ser2': listarrser2})
     temp_df = temp_df.dropna(axis=0)
     temp_len = temp_df.shape[0]
 
-    return np.nansum(temp_df.apply(func=lambda x: x['ser1'] == x['ser2'], axis=1).values) == temp_len
+    return np.nansum(temp_df.apply(func=lambda x: x['ser1'] == x['ser2'], axis=1).to_numpy()) == temp_len
 
 
 def repunit_append_arr(target_len, listarrser, repunit):
     """
     Append the repeat units to the end if the listarr to the target length
     :param target_len: target length of the list/array
     :param listarrser: input should be list/arr/ser
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits.egg-info/PKG-INFO` & `accountingkits-0.1.1.230425a0/accountingkits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accountingkits
-Version: 0.1.1.230331a0
+Version: 0.1.1.230425a0
 Summary: The kit-package which made for accounting science research
 Home-page: https://github.com/qihangZH/accountingkits
 Author: zhang qihang
 Author-email: 694499657@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `accountingkits-0.1.1.230331a0/accountingkits.egg-info/SOURCES.txt` & `accountingkits-0.1.1.230425a0/accountingkits.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 accountingkits/DataPrepare/SliceSelectT.py
 accountingkits/DataPrepare/StringT.py
 accountingkits/DataPrepare/__init__.py
 accountingkits/OSKit/DirectoryT.py
 accountingkits/OSKit/__init__.py
 accountingkits/Stats/SummarizeT.py
 accountingkits/Stats/__init__.py
-accountingkits/WaybackScraper/JsonConverterT.py
 accountingkits/WaybackScraper/LICENSE
 accountingkits/WaybackScraper/WayBackT.py
 accountingkits/WaybackScraper/__init__.py
 accountingkits/_BasicTools/ArrayLikeT.py
 accountingkits/_BasicTools/DecoratorT.py
 accountingkits/_BasicTools/MultiprocessT.py
 accountingkits/_BasicTools/UniversalBasicT.py
```

### Comparing `accountingkits-0.1.1.230331a0/demo.ipynb` & `accountingkits-0.1.1.230425a0/demo.ipynb`

 * *Files identical despite different names*

