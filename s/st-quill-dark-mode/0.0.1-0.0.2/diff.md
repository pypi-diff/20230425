# Comparing `tmp/st-quill-dark-mode-0.0.1.tar.gz` & `tmp/st-quill-dark-mode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-quill-dark-mode-0.0.1.tar", last modified: Mon Apr 24 07:19:26 2023, max compression
+gzip compressed data, was "st-quill-dark-mode-0.0.2.tar", last modified: Mon Apr 24 07:46:02 2023, max compression
```

## Comparing `st-quill-dark-mode-0.0.1.tar` & `st-quill-dark-mode-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:19:26.393899 st-quill-dark-mode-0.0.1/
--rw-r--r--   0 bryan.saggese   (503) staff       (20)     1063 2023-04-23 23:43:13.000000 st-quill-dark-mode-0.0.1/LICENSE
--rw-r--r--   0 bryan.saggese   (503) staff       (20)       54 2023-04-24 07:12:08.000000 st-quill-dark-mode-0.0.1/MANIFEST.in
--rw-r--r--   0 bryan.saggese   (503) staff       (20)      180 2023-04-24 07:19:26.393571 st-quill-dark-mode-0.0.1/PKG-INFO
--rw-r--r--   0 bryan.saggese   (503) staff       (20)       38 2023-04-24 07:19:26.394091 st-quill-dark-mode-0.0.1/setup.cfg
--rw-r--r--   0 bryan.saggese   (503) staff       (20)      563 2023-04-24 07:11:48.000000 st-quill-dark-mode-0.0.1/setup.py
-drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:19:26.390567 st-quill-dark-mode-0.0.1/st_quill_dark_mode/
--rw-r--r--   0 bryan.saggese   (503) staff       (20)     3730 2023-04-24 07:09:30.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode/__init__.py
-drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:19:26.392913 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/
--rw-r--r--   0 bryan.saggese   (503) staff       (20)      180 2023-04-24 07:19:26.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/PKG-INFO
--rw-r--r--   0 bryan.saggese   (503) staff       (20)      268 2023-04-24 07:19:26.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/SOURCES.txt
--rw-r--r--   0 bryan.saggese   (503) staff       (20)        1 2023-04-24 07:19:26.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/dependency_links.txt
--rw-r--r--   0 bryan.saggese   (503) staff       (20)       16 2023-04-24 07:19:26.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/requires.txt
--rw-r--r--   0 bryan.saggese   (503) staff       (20)       19 2023-04-24 07:19:26.000000 st-quill-dark-mode-0.0.1/st_quill_dark_mode.egg-info/top_level.txt
+drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:46:02.914022 st-quill-dark-mode-0.0.2/
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)     1063 2023-04-23 23:43:13.000000 st-quill-dark-mode-0.0.2/LICENSE
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)       54 2023-04-24 07:12:08.000000 st-quill-dark-mode-0.0.2/MANIFEST.in
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)      218 2023-04-24 07:46:02.913497 st-quill-dark-mode-0.0.2/PKG-INFO
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)       38 2023-04-24 07:46:02.914241 st-quill-dark-mode-0.0.2/setup.cfg
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)      591 2023-04-24 07:45:40.000000 st-quill-dark-mode-0.0.2/setup.py
+drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:46:02.909529 st-quill-dark-mode-0.0.2/st_quill_dark_mode/
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)     3730 2023-04-24 07:09:30.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode/__init__.py
+drwxr-xr-x   0 bryan.saggese   (503) staff       (20)        0 2023-04-24 07:46:02.912634 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)      218 2023-04-24 07:46:02.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/PKG-INFO
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)      268 2023-04-24 07:46:02.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/SOURCES.txt
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)        1 2023-04-24 07:46:02.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/dependency_links.txt
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)       16 2023-04-24 07:46:02.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/requires.txt
+-rw-r--r--   0 bryan.saggese   (503) staff       (20)       19 2023-04-24 07:46:02.000000 st-quill-dark-mode-0.0.2/st_quill_dark_mode.egg-info/top_level.txt
```

### Comparing `st-quill-dark-mode-0.0.1/LICENSE` & `st-quill-dark-mode-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st-quill-dark-mode-0.0.1/setup.py` & `st-quill-dark-mode-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name="st-quill-dark-mode",
-    version="0.0.1",
+    version="0.0.2",
     author="",
     author_email="",
-    description="",
+    description="Dark Streamlit Quill Editor.",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.6",
```

### Comparing `st-quill-dark-mode-0.0.1/st_quill_dark_mode/__init__.py` & `st-quill-dark-mode-0.0.2/st_quill_dark_mode/__init__.py`

 * *Files identical despite different names*

