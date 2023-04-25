# Comparing `tmp/peitho_data-2.1.3.tar.gz` & `tmp/peitho_data-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.1.3.tar", last modified: Tue Apr 25 08:49:09 2023, max compression
+gzip compressed data, was "peitho_data-2.1.4.tar", last modified: Tue Apr 25 10:27:08 2023, max compression
```

## Comparing `peitho_data-2.1.3.tar` & `peitho_data-2.1.4.tar`

### file list

```diff
@@ -1,19 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 08:49:08.000000 peitho_data-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 08:49:08.000000 peitho_data-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 08:49:09.555800 peitho_data-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 08:49:08.000000 peitho_data-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:49:09.555800 peitho_data-2.1.3/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:49:09.000000 peitho_data-2.1.3/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 08:49:09.555800 peitho_data-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 08:49:09.000000 peitho_data-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 10:27:08.000000 peitho_data-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 10:27:08.000000 peitho_data-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 10:27:08.933914 peitho_data-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 10:27:08.000000 peitho_data-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/visualization/file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/visualization/test_file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 10:27:08.933914 peitho_data-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 10:27:08.000000 peitho_data-2.1.4/setup.py
```

### Comparing `peitho_data-2.1.3/LICENSE` & `peitho_data-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.3/README.md` & `peitho_data-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.3/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.1.4/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.3/peitho_data/trello_api.py` & `peitho_data-2.1.4/peitho_data/trello_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,19 +68,19 @@
                 token
             )
         )
 
 
 def upload_attachment(card_id: str, attachment_name: str, attachment_relative_path: str) -> requests.models.Response:
     """
-    Uploads file to a Trello card as attachment.
-
     :param card_id:  The ID of the Trello card against whihc the attachment is to be uploaded
     :param attachment_name:  Attachment display name, e.g. book.pdf
     :param attachment_relative_path:  Attachment file path relative to the location of this scrip invocation
+
+    :return: a response object whose trello API response fields can be retrieved via "response.json()"
     """
     # Define the credential info
     params = (
         ('key', key),
         ('token', token),
     )
```

### Comparing `peitho_data-2.1.3/peitho_data/word_cloud.py` & `peitho_data-2.1.4/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.3/setup.py` & `peitho_data-2.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.1.3",
+    version="2.1.4",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
-    packages=["peitho_data"],
+    packages=find_packages(),
     python_requires='>=3.10',
     install_requires=[
         "bs4",
         "wordcloud",
         "pycodestyle",
         "requests",
         "sphinx-rtd-theme",
```

