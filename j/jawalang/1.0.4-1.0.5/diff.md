# Comparing `tmp/jawalang-1.0.4.tar.gz` & `tmp/jawalang-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jawalang-1.0.4.tar", last modified: Tue Apr 25 00:34:02 2023, max compression
+gzip compressed data, was "jawalang-1.0.5.tar", last modified: Tue Apr 25 00:35:50 2023, max compression
```

## Comparing `jawalang-1.0.4.tar` & `jawalang-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:34:02.850282 jawalang-1.0.4/
--rw-rw-rw-   0        0        0     1085 2023-04-23 23:08:13.000000 jawalang-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1151 2023-04-25 00:34:02.847952 jawalang-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-04-25 00:07:04.000000 jawalang-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:34:02.828504 jawalang-1.0.4/jawalang/
--rw-rw-rw-   0        0        0        4 2023-04-25 00:26:59.000000 jawalang-1.0.4/jawalang/__init__.py
--rw-rw-rw-   0        0        0     2980 2023-04-25 00:33:37.000000 jawalang-1.0.4/jawalang/__main__.py
--rw-rw-rw-   0        0        0     1423 2023-04-24 03:48:24.000000 jawalang-1.0.4/jawalang/errorHandle.py
--rw-rw-rw-   0        0        0      353 2023-04-24 21:34:07.000000 jawalang-1.0.4/jawalang/print.py
--rw-rw-rw-   0        0        0     1431 2023-04-24 22:04:50.000000 jawalang-1.0.4/jawalang/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:34:02.847952 jawalang-1.0.4/jawalang.egg-info/
--rw-rw-rw-   0        0        0     1151 2023-04-25 00:34:02.000000 jawalang-1.0.4/jawalang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-04-25 00:34:02.000000 jawalang-1.0.4/jawalang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:34:02.000000 jawalang-1.0.4/jawalang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-25 00:34:02.000000 jawalang-1.0.4/jawalang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 00:34:02.000000 jawalang-1.0.4/jawalang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 00:34:02.850282 jawalang-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-04-25 00:33:45.000000 jawalang-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:50.579334 jawalang-1.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 23:08:13.000000 jawalang-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1151 2023-04-25 00:35:50.577325 jawalang-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-04-25 00:07:04.000000 jawalang-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:50.559774 jawalang-1.0.5/jawalang/
+-rw-rw-rw-   0        0        0        4 2023-04-25 00:26:59.000000 jawalang-1.0.5/jawalang/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-04-25 00:35:31.000000 jawalang-1.0.5/jawalang/__main__.py
+-rw-rw-rw-   0        0        0     1423 2023-04-24 03:48:24.000000 jawalang-1.0.5/jawalang/errorHandle.py
+-rw-rw-rw-   0        0        0      353 2023-04-24 21:34:07.000000 jawalang-1.0.5/jawalang/print.py
+-rw-rw-rw-   0        0        0     1431 2023-04-24 22:04:50.000000 jawalang-1.0.5/jawalang/transform.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:50.576322 jawalang-1.0.5/jawalang.egg-info/
+-rw-rw-rw-   0        0        0     1151 2023-04-25 00:35:50.000000 jawalang-1.0.5/jawalang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-04-25 00:35:50.000000 jawalang-1.0.5/jawalang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:35:50.000000 jawalang-1.0.5/jawalang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-25 00:35:50.000000 jawalang-1.0.5/jawalang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 00:35:50.000000 jawalang-1.0.5/jawalang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:35:50.579334 jawalang-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-04-25 00:35:36.000000 jawalang-1.0.5/setup.py
```

### Comparing `jawalang-1.0.4/LICENSE` & `jawalang-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.4/PKG-INFO` & `jawalang-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jawalang
-Version: 1.0.4
+Version: 1.0.5
 Summary: Javanese programming language base on python
 Home-page: https://github.com/Arsybai/jawa-language
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: programming languages,languages
 Description-Content-Type: text/markdown
```

### Comparing `jawalang-1.0.4/README.md` & `jawalang-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.4/jawalang/__main__.py` & `jawalang-1.0.5/jawalang/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,9 +69,9 @@
                 else:
                     raise Exception("file ora ditemokake cuk!")
             except Exception as e:
                 e = traceback.format_exc()
                 #print(e)
                 raiseError(e)
     except Exception as e:
-        print(e)
-        # print("Use `jawalang run <path>` to execute file")
+        #print(e)
+        print("Use `jawalang run <path>` to execute file")
```

### Comparing `jawalang-1.0.4/jawalang/errorHandle.py` & `jawalang-1.0.5/jawalang/errorHandle.py`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.4/jawalang/transform.py` & `jawalang-1.0.5/jawalang/transform.py`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.4/jawalang.egg-info/PKG-INFO` & `jawalang-1.0.5/jawalang.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jawalang
-Version: 1.0.4
+Version: 1.0.5
 Summary: Javanese programming language base on python
 Home-page: https://github.com/Arsybai/jawa-language
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: programming languages,languages
 Description-Content-Type: text/markdown
```

### Comparing `jawalang-1.0.4/setup.py` & `jawalang-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jawalang",
-    version="1.0.4",
+    version="1.0.5",
     author="Arsybai",
     description="Javanese programming language base on python",
     packages=["jawalang"],
     license="MIT",
     author_email="me@arsybai.com",
     url="https://github.com/Arsybai/jawa-language",
     keywords=[
```

