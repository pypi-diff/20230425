# Comparing `tmp/aireplication-0.0.3.tar.gz` & `tmp/aireplication-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aireplication-0.0.3.tar", last modified: Tue Apr 25 08:07:12 2023, max compression
+gzip compressed data, was "aireplication-0.0.4.tar", last modified: Tue Apr 25 08:30:07 2023, max compression
```

## Comparing `aireplication-0.0.3.tar` & `aireplication-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.423297 aireplication-0.0.3/
--rw-rw-rw-   0        0        0    11558 2023-04-25 07:54:43.000000 aireplication-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2728 2023-04-25 08:07:12.423390 aireplication-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2120 2023-04-25 08:03:15.000000 aireplication-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.393796 aireplication-0.0.3/aireplication/
--rw-rw-rw-   0        0        0       21 2023-04-25 08:06:39.000000 aireplication-0.0.3/aireplication/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.421793 aireplication-0.0.3/aireplication/ultils/
--rw-rw-rw-   0        0        0      236 2023-04-25 07:54:43.000000 aireplication-0.0.3/aireplication/ultils/__init__.py
--rw-rw-rw-   0        0        0    13046 2023-04-25 07:59:53.000000 aireplication-0.0.3/aireplication/ultils/data.py
--rw-rw-rw-   0        0        0     6724 2023-04-25 07:57:19.000000 aireplication-0.0.3/aireplication/ultils/datasets.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.416303 aireplication-0.0.3/aireplication.egg-info/
--rw-rw-rw-   0        0        0     2728 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-25 08:07:12.424795 aireplication-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-04-25 07:54:43.000000 aireplication-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:30:07.248316 aireplication-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-25 07:54:43.000000 aireplication-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2728 2023-04-25 08:30:07.248316 aireplication-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2120 2023-04-25 08:03:15.000000 aireplication-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:30:07.221818 aireplication-0.0.4/aireplication/
+-rw-rw-rw-   0        0        0       21 2023-04-25 08:28:59.000000 aireplication-0.0.4/aireplication/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:30:07.246816 aireplication-0.0.4/aireplication/ultils/
+-rw-rw-rw-   0        0        0      236 2023-04-25 07:54:43.000000 aireplication-0.0.4/aireplication/ultils/__init__.py
+-rw-rw-rw-   0        0        0    13061 2023-04-25 08:28:10.000000 aireplication-0.0.4/aireplication/ultils/data.py
+-rw-rw-rw-   0        0        0     6724 2023-04-25 07:57:19.000000 aireplication-0.0.4/aireplication/ultils/datasets.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:30:07.241817 aireplication-0.0.4/aireplication.egg-info/
+-rw-rw-rw-   0        0        0     2728 2023-04-25 08:30:07.000000 aireplication-0.0.4/aireplication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-04-25 08:30:07.000000 aireplication-0.0.4/aireplication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:30:07.000000 aireplication-0.0.4/aireplication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-25 08:30:07.000000 aireplication-0.0.4/aireplication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 08:30:07.000000 aireplication-0.0.4/aireplication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-25 08:30:07.250316 aireplication-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-04-25 07:54:43.000000 aireplication-0.0.4/setup.py
```

### Comparing `aireplication-0.0.3/LICENSE` & `aireplication-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aireplication-0.0.3/PKG-INFO` & `aireplication-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aireplication
-Version: 0.0.3
+Version: 0.0.4
 Summary: Private API for Andrew
 Home-page: https://github.com/andrewlee1807/ai-replicate
 Author: Andrew
 Author-email: andrewlee1807@gmail.com
 License: Apache-2.0 license
 Keywords: python,blackhole,aireplication
 Platform: UNKNOWN
```

### Comparing `aireplication-0.0.3/README.md` & `aireplication-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aireplication-0.0.3/aireplication/ultils/data.py` & `aireplication-0.0.4/aireplication/ultils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             y_label.append(data[i: i + self.output_length][::, feature_order])
 
         X_data, y_label = np.array(X_data), np.array(y_label)
 
         return X_data, y_label
 
 
-from utils.datasets import *
+from aireplication.ultils.datasets import *
 
 
 def get_all_data_supported():
     return list(CONFIG_PATH.keys())
 
 
 class Dataset:
```

### Comparing `aireplication-0.0.3/aireplication/ultils/datasets.py` & `aireplication-0.0.4/aireplication/ultils/datasets.py`

 * *Files identical despite different names*

### Comparing `aireplication-0.0.3/aireplication.egg-info/PKG-INFO` & `aireplication-0.0.4/aireplication.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aireplication
-Version: 0.0.3
+Version: 0.0.4
 Summary: Private API for Andrew
 Home-page: https://github.com/andrewlee1807/ai-replicate
 Author: Andrew
 Author-email: andrewlee1807@gmail.com
 License: Apache-2.0 license
 Keywords: python,blackhole,aireplication
 Platform: UNKNOWN
```

### Comparing `aireplication-0.0.3/setup.py` & `aireplication-0.0.4/setup.py`

 * *Files identical despite different names*

