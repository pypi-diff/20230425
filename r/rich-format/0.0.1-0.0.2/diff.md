# Comparing `tmp/rich_format-0.0.1.tar.gz` & `tmp/rich_format-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/desac/Documents/my-python-packages/rich_format/dist/.tmp-ncy4ata1/rich_format-0.0.1.tar", last modified: Tue Apr 25 09:54:54 2023, max compression
+gzip compressed data, was "/Users/desac/Documents/my-python-packages/rich_format/dist/.tmp-llo_yiyl/rich_format-0.0.2.tar", last modified: Tue Apr 25 10:24:16 2023, max compression
```

## Comparing `rich_format-0.0.1.tar` & `rich_format-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 09:54:54.000000 rich_format-0.0.1/
--rw-r--r--   0 desac      (501) staff       (20)     1062 2023-04-25 08:45:30.000000 rich_format-0.0.1/LICENSE
--rw-r--r--   0 desac      (501) staff       (20)       33 2023-04-25 08:53:37.000000 rich_format-0.0.1/MANIFEST.in
--rw-r--r--   0 desac      (501) staff       (20)      805 2023-04-25 09:54:54.000000 rich_format-0.0.1/PKG-INFO
--rw-r--r--   0 desac      (501) staff       (20)       13 2023-04-25 08:45:30.000000 rich_format-0.0.1/README.md
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format/
--rw-r--r--   0 desac      (501) staff       (20)     6791 2023-04-25 09:35:15.000000 rich_format-0.0.1/rich_format/__init__.py
--rw-r--r--   0 desac      (501) staff       (20)     2394 2023-04-25 09:36:17.000000 rich_format-0.0.1/rich_format/test.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/
--rw-r--r--   0 desac      (501) staff       (20)      805 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/PKG-INFO
--rw-r--r--   0 desac      (501) staff       (20)      324 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/SOURCES.txt
--rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/dependency_links.txt
--rw-r--r--   0 desac      (501) staff       (20)       67 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/entry_points.txt
--rw-r--r--   0 desac      (501) staff       (20)        5 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/requires.txt
--rw-r--r--   0 desac      (501) staff       (20)       12 2023-04-25 09:54:54.000000 rich_format-0.0.1/rich_format.egg-info/top_level.txt
--rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-25 09:07:40.000000 rich_format-0.0.1/rich_format.egg-info/zip-safe
--rw-r--r--   0 desac      (501) staff       (20)       38 2023-04-25 09:54:54.000000 rich_format-0.0.1/setup.cfg
--rw-r--r--   0 desac      (501) staff       (20)     1446 2023-04-25 09:36:10.000000 rich_format-0.0.1/setup.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 10:24:16.000000 rich_format-0.0.2/
+-rw-r--r--   0 desac      (501) staff       (20)     1062 2023-04-25 08:45:30.000000 rich_format-0.0.2/LICENSE
+-rw-r--r--   0 desac      (501) staff       (20)       33 2023-04-25 08:53:37.000000 rich_format-0.0.2/MANIFEST.in
+-rw-r--r--   0 desac      (501) staff       (20)     2527 2023-04-25 10:24:16.000000 rich_format-0.0.2/PKG-INFO
+-rw-r--r--   0 desac      (501) staff       (20)     1736 2023-04-25 10:23:32.000000 rich_format-0.0.2/README.md
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format/
+-rw-r--r--   0 desac      (501) staff       (20)     6791 2023-04-25 09:35:15.000000 rich_format-0.0.2/rich_format/__init__.py
+-rw-r--r--   0 desac      (501) staff       (20)     2394 2023-04-25 09:36:17.000000 rich_format-0.0.2/rich_format/test.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/
+-rw-r--r--   0 desac      (501) staff       (20)     2527 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/PKG-INFO
+-rw-r--r--   0 desac      (501) staff       (20)      324 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/SOURCES.txt
+-rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/dependency_links.txt
+-rw-r--r--   0 desac      (501) staff       (20)       67 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/entry_points.txt
+-rw-r--r--   0 desac      (501) staff       (20)        5 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/requires.txt
+-rw-r--r--   0 desac      (501) staff       (20)       12 2023-04-25 10:24:16.000000 rich_format-0.0.2/rich_format.egg-info/top_level.txt
+-rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-25 09:07:40.000000 rich_format-0.0.2/rich_format.egg-info/zip-safe
+-rw-r--r--   0 desac      (501) staff       (20)       38 2023-04-25 10:24:16.000000 rich_format-0.0.2/setup.cfg
+-rw-r--r--   0 desac      (501) staff       (20)     1446 2023-04-25 10:24:04.000000 rich_format-0.0.2/setup.py
```

### Comparing `rich_format-0.0.1/LICENSE` & `rich_format-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_format-0.0.1/rich_format/__init__.py` & `rich_format-0.0.2/rich_format/__init__.py`

 * *Files identical despite different names*

### Comparing `rich_format-0.0.1/rich_format/test.py` & `rich_format-0.0.2/rich_format/test.py`

 * *Files identical despite different names*

### Comparing `rich_format-0.0.1/setup.py` & `rich_format-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
@@ -47,10 +47,10 @@
 	long_description_content_type="text/markdown",
 	include_package_data=True,
 	keywords='rich',
 	name='rich_format',
 	packages=find_packages(include=['rich_format', 'rich_format.*']),
 	setup_requires=setup_requirements,
 	url='https://github.com/pom11/rich_format',
-	version='0.0.1',
+	version='0.0.2',
 	zip_safe=True,
 )
```

