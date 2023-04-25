# Comparing `tmp/neophaser-0.1.1.tar.gz` & `tmp/neophaser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophaser-0.1.1.tar", last modified: Thu Apr 20 06:13:20 2023, max compression
+gzip compressed data, was "neophaser-0.1.2.tar", last modified: Tue Apr 25 02:19:17 2023, max compression
```

## Comparing `neophaser-0.1.1.tar` & `neophaser-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 maxtretikov   (501) staff       (20)        0 2023-04-20 06:13:20.202879 neophaser-0.1.1/
--rw-r--r--   0 maxtretikov   (501) staff       (20)       26 2023-04-20 06:06:50.000000 neophaser-0.1.1/MANIFEST.in
--rw-r--r--   0 maxtretikov   (501) staff       (20)      892 2023-04-20 06:13:20.202744 neophaser-0.1.1/PKG-INFO
--rw-r--r--   0 maxtretikov   (501) staff       (20)      335 2023-04-19 14:35:27.000000 neophaser-0.1.1/README.md
-drwxr-xr-x   0 maxtretikov   (501) staff       (20)        0 2023-04-20 06:13:20.200678 neophaser-0.1.1/neophaser/
--rw-r--r--   0 maxtretikov   (501) staff       (20)        0 2023-04-19 04:58:07.000000 neophaser-0.1.1/neophaser/__init__.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)      365 2023-04-20 06:08:21.000000 neophaser-0.1.1/neophaser/__main__.py
-drwxr-xr-x   0 maxtretikov   (501) staff       (20)        0 2023-04-20 06:13:20.201679 neophaser-0.1.1/neophaser/assets/
--rw-r--r--   0 maxtretikov   (501) staff       (20)   208914 2023-04-19 13:55:33.000000 neophaser-0.1.1/neophaser/assets/icon.png
--rw-r--r--   0 maxtretikov   (501) staff       (20)     2140 2023-04-19 13:38:21.000000 neophaser-0.1.1/neophaser/board.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)     3673 2023-04-19 12:20:35.000000 neophaser-0.1.1/neophaser/controllers.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)    10107 2023-04-19 14:04:14.000000 neophaser-0.1.1/neophaser/gui.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)      717 2023-04-19 12:12:10.000000 neophaser-0.1.1/neophaser/options.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)     1187 2023-04-19 11:02:23.000000 neophaser-0.1.1/neophaser/utils.py
--rw-r--r--   0 maxtretikov   (501) staff       (20)     1304 2023-04-19 13:25:19.000000 neophaser-0.1.1/neophaser/visual.py
-drwxr-xr-x   0 maxtretikov   (501) staff       (20)        0 2023-04-20 06:13:20.201551 neophaser-0.1.1/neophaser.egg-info/
--rw-r--r--   0 maxtretikov   (501) staff       (20)      892 2023-04-20 06:13:20.000000 neophaser-0.1.1/neophaser.egg-info/PKG-INFO
--rw-r--r--   0 maxtretikov   (501) staff       (20)      391 2023-04-20 06:13:20.000000 neophaser-0.1.1/neophaser.egg-info/SOURCES.txt
--rw-r--r--   0 maxtretikov   (501) staff       (20)        1 2023-04-20 06:13:20.000000 neophaser-0.1.1/neophaser.egg-info/dependency_links.txt
--rw-r--r--   0 maxtretikov   (501) staff       (20)       45 2023-04-20 06:13:20.000000 neophaser-0.1.1/neophaser.egg-info/requires.txt
--rw-r--r--   0 maxtretikov   (501) staff       (20)       10 2023-04-20 06:13:20.000000 neophaser-0.1.1/neophaser.egg-info/top_level.txt
--rw-r--r--   0 maxtretikov   (501) staff       (20)      725 2023-04-20 06:12:36.000000 neophaser-0.1.1/pyproject.toml
--rw-r--r--   0 maxtretikov   (501) staff       (20)       38 2023-04-20 06:13:20.202918 neophaser-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.539664 neophaser-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-25 02:19:07.000000 neophaser-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-25 02:19:17.538664 neophaser-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 02:19:07.000000 neophaser-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.535664 neophaser-0.1.2/neophaser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.538664 neophaser-0.1.2/neophaser/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/assets/icon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   208914 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/assets/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/board.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10107 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.537664 neophaser-0.1.2/neophaser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-04-25 02:19:07.000000 neophaser-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 02:19:17.539664 neophaser-0.1.2/setup.cfg
```

### Comparing `neophaser-0.1.1/PKG-INFO` & `neophaser-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.1
+Version: 0.1.2
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # NEOPHASER; or, audio effects as applied to the retina
 
-neophaser is a project designed to apply audio effect chains to image and video data. There is no better explanation than to use it yourself. Check out cool examples and download at https://neophaser.library.8oc.org
+neophaser is a project designed to apply audio effect chains to image and video data. There is no better explanation than to use it yourself. Check out cool examples at https://neophaser.library.8oc.org.
 
-To run the project in python, just run ``pipenv run start``.
+Install with `pip install neophaser`, run with `python -m neophaser`.
```

### Comparing `neophaser-0.1.1/neophaser/assets/icon.png` & `neophaser-0.1.2/neophaser/assets/icon.png`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/board.py` & `neophaser-0.1.2/neophaser/board.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/controllers.py` & `neophaser-0.1.2/neophaser/controllers.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/gui.py` & `neophaser-0.1.2/neophaser/gui.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/options.py` & `neophaser-0.1.2/neophaser/options.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/utils.py` & `neophaser-0.1.2/neophaser/utils.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser/visual.py` & `neophaser-0.1.2/neophaser/visual.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.1/neophaser.egg-info/PKG-INFO` & `neophaser-0.1.2/neophaser.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.1
+Version: 0.1.2
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # NEOPHASER; or, audio effects as applied to the retina
 
-neophaser is a project designed to apply audio effect chains to image and video data. There is no better explanation than to use it yourself. Check out cool examples and download at https://neophaser.library.8oc.org
+neophaser is a project designed to apply audio effect chains to image and video data. There is no better explanation than to use it yourself. Check out cool examples at https://neophaser.library.8oc.org.
 
-To run the project in python, just run ``pipenv run start``.
+Install with `pip install neophaser`, run with `python -m neophaser`.
```

### Comparing `neophaser-0.1.1/pyproject.toml` & `neophaser-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neophaser"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="8o-COLLECTIVE", email="ops@8oc.org" },
 ]
 description = "NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

