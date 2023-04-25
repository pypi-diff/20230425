# Comparing `tmp/ds4n6_lib-0.7.1.tar.gz` & `tmp/ds4n6_lib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds4n6_lib-0.7.1.tar", last modified: Tue Jun  7 15:03:33 2022, max compression
+gzip compressed data, was "ds4n6_lib-0.8.1.tar", last modified: Tue Apr 25 08:37:46 2023, max compression
```

## Comparing `ds4n6_lib-0.7.1.tar` & `ds4n6_lib-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxrwxr-x   0 lcortes   (1001) lcortes   (1001)        0 2022-06-07 15:03:33.635565 ds4n6_lib-0.7.1/
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)    35131 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/LICENSE
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)      249 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/MANIFEST.in
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     5141 2022-06-07 15:03:33.635565 ds4n6_lib-0.7.1/PKG-INFO
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     3255 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/README.md
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)      104 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/pyproject.toml
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     1952 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/requirements.txt
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)       79 2022-06-07 15:03:33.635565 ds4n6_lib-0.7.1/setup.cfg
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     1826 2022-06-07 14:59:43.000000 ds4n6_lib-0.7.1/setup.py
-drwxrwxr-x   0 lcortes   (1001) lcortes   (1001)        0 2022-06-07 15:03:33.627565 ds4n6_lib-0.7.1/src/
-drwxrwxr-x   0 lcortes   (1001) lcortes   (1001)        0 2022-06-07 15:03:33.631565 ds4n6_lib-0.7.1/src/ds4n6_lib/
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)        2 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/__init__.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     5592 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/amcache.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     7679 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/autoruns.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    60502 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/common.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     1716 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/d4.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)   100625 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/evtx.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    16146 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/evtx_parser.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    12712 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/flist.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    10527 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/fstl.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    33699 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/gui.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     9192 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/kansa.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    15301 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/kape.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    47534 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/knowledge.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    11124 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/macrobber.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     9569 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/mactime.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    42977 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/ml.py
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     2748 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/pf.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    44138 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/plaso.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    10771 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/pslist.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    17092 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/sabonis.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     6544 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/svclist.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    11225 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/tshark.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     6642 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/unx.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)    14267 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/utils.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     9284 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/volatility.py
--rwxrwxr-x   0 lcortes   (1001) lcortes   (1001)     5619 2022-06-07 14:28:51.000000 ds4n6_lib-0.7.1/src/ds4n6_lib/winreg.py
-drwxrwxr-x   0 lcortes   (1001) lcortes   (1001)        0 2022-06-07 15:03:33.631565 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)     5141 2022-06-07 15:03:33.000000 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/PKG-INFO
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)      883 2022-06-07 15:03:33.000000 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)        1 2022-06-07 15:03:33.000000 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)      179 2022-06-07 15:03:33.000000 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/requires.txt
--rw-rw-r--   0 lcortes   (1001) lcortes   (1001)       10 2022-06-07 15:03:33.000000 ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/top_level.txt
+drwxrwxr-x   0 mperez    (1001) mperez    (1001)        0 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)    35131 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/LICENSE
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)    35149 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/LICENSE.md
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)      249 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/MANIFEST.in
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     4360 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/PKG-INFO
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     3283 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/README.md
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)      104 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/pyproject.toml
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     1979 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/requirements.txt
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)       79 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/setup.cfg
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     1868 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/setup.py
+drwxrwxr-x   0 mperez    (1001) mperez    (1001)        0 2023-04-25 08:37:46.161937 ds4n6_lib-0.8.1/src/
+drwxrwxr-x   0 mperez    (1001) mperez    (1001)        0 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/src/ds4n6_lib/
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)        2 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/__init__.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     5592 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/amcache.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     7679 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/autoruns.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    60502 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/common.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     1716 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/d4.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)   100625 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/evtx.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    16146 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/evtx_parser.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    12712 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/flist.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    10527 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/fstl.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    33699 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/gui.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     9192 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/kansa.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    15301 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/kape.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    47534 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/knowledge.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    11124 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/macrobber.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     9569 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/mactime.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    42977 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/ml.py
+drwxrwxr-x   0 mperez    (1001) mperez    (1001)        0 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/src/ds4n6_lib/ml_modules/
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)        0 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/ml_modules/__init__.py
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)    11164 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/ml_modules/seq2seq_lstm.py
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)    12325 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/ml_modules/transformer.py
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)    12911 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/mlgraph.py
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     2748 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/pf.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    44138 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/plaso.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    10771 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/pslist.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    17092 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/sabonis.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     6544 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/svclist.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    11225 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/tshark.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     6642 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/unx.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)    14267 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/utils.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     9284 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/volatility.py
+-rwxrwxr-x   0 mperez    (1001) mperez    (1001)     5619 2023-04-25 06:59:54.000000 ds4n6_lib-0.8.1/src/ds4n6_lib/winreg.py
+drwxrwxr-x   0 mperez    (1001) mperez    (1001)        0 2023-04-25 08:37:46.169937 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     4360 2023-04-25 08:37:46.000000 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)     1037 2023-04-25 08:37:46.000000 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)        1 2023-04-25 08:37:46.000000 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)      195 2023-04-25 08:37:46.000000 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/requires.txt
+-rw-rw-r--   0 mperez    (1001) mperez    (1001)       10 2023-04-25 08:37:46.000000 ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/top_level.txt
```

### Comparing `ds4n6_lib-0.7.1/LICENSE` & `ds4n6_lib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/PKG-INFO` & `ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,128 @@
 Metadata-Version: 2.1
-Name: ds4n6_lib
-Version: 0.7.1
+Name: ds4n6-lib
+Version: 0.8.1
 Summary: Bringing Data Science & Artificial Intelligence to the fingertips of the average Forensicator, and promote advances in the field
 Home-page: https://github.com/ds4n6/ds4n6_lib
 Author: Jess Garcia
 Author-email: ds4n6@one-esecurity.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/issues
 Project-URL: Website, http://www.ds4n6.io/
-Description: <!-- PROJECT LOGO -->
-        
-        <p align="center">
-          <a href="http://www.ds4n6.io">
-            <img src="http://www.ds4n6.io/images/DS4N6.jpg">
-          </a>
-        </p>
-        
-        <a href="http://www.ds4n6.io" title=""><img src="http://ds4n6.io/images/logo-s.png" alt="" /></a>
-        
-        DS4N6 stands for Data Science Forensics.
-        
-        We also refer to this project as DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial Intelligence (AI), and the project goes beyond the strictly Forensics, covering the whole Digital Forensics & Incident Response (DFIR) discipline (and sometimes even beyond). But hey, we had to give the project a catchy name!
-        
-        The Mission of the DS4N6 project is simple:
-        
-        ```
-        Bringing Data Science & Artificial Intelligence
-        to the fingertips of the average Forensicator,
-        and promote advances in the field
-        ```
-        
-        The first (modest) alpha version of our ds4n6 python library, together with some easy-to-use python scripts, was originally made public after the presentation at the SANS DFIR Summit US, July 16-17.
-        **For detailed information about the Project, the Library, its Functions, its Usage, etc., visit the project page: http://www.ds4n6.io/tools/ds4n6.py.html**
-        
-        ## Getting Started
-        
-        These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
-        
-        https://github.com/ds4n6/ds4n6_lib.git
-        
-        ### Prerequisites
-        
-        The DS4N6 library works on the 3.x versions of the Python programming language. The module has external dependencies related to datascience and extraction of forensic evidence.
-        
-        Install requirements:
-        
-            - python-evtx
-            - Evtx
-            - ipyaggrid
-            - IPython
-            - ipywidgets
-            - keras
-            - matplotlib
-            - nbformat
-            - numpy
-            - pandas
-            - pyparsing
-            - qgrid
-            - ruamel.yaml
-            - sklearn
-            - tensorflow
-            - tqdm
-            - traitlets
-            - xmltodict
-        
-        ### Installation
-        
-        The installation can be easily done through pip.
-        
-        #### pip installation
-        
-        ```sh
-            pip install python-evtx Evtx ipyaggrid IPython ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib
-        ```
-        
-        Finally, import in your python3 program or Jupyter Notebook as "ds".
-        
-        ```python
-            import ds4n6_lib as ds
-        ```
-        
-        ## Contributing
-        
-        If you think you can provide value to the Community, collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
-        
-        Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.
-        
-        ### download from github
-        
-        All you will need to do is to clone the library, install the test, create a virtual enviroment to use it and active it.
-        
-        ```sh
-            
-            git clone https://github.com/ds4n6/ds4n6_lib    
-        
-            virtualenv -p python3.7 .test
-            source .test/bin/activate
-            
-            pip install -r requirements.txt 
-        ```
-        
-        ## Authors
-        
-        * **Jess Garcia** - *Initial work* - http://ds4n6.io/community/jess_garcia.html
-        
-        See also the list of [contributors](http://ds4n6.io/community.html) who participated in this project.
-        
-        ## License
-        
-        This project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE) file for details
-        
 Keywords: dfir,datascience,forensics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.md
+
+<!-- PROJECT LOGO -->
+
+<p align="center">
+  <a href="http://www.ds4n6.io">
+    <img src="http://www.ds4n6.io/images/DS4N6.jpg">
+  </a>
+</p>
+
+<a href="http://www.ds4n6.io" title=""><img src="http://ds4n6.io/images/logo-s.png" alt="" /></a>
+
+DS4N6 stands for Data Science Forensics.
+
+We also refer to this project as DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial Intelligence (AI), and the project goes beyond the strictly Forensics, covering the whole Digital Forensics & Incident Response (DFIR) discipline (and sometimes even beyond). But hey, we had to give the project a catchy name!
+
+The Mission of the DS4N6 project is simple:
+
+```
+Bringing Data Science & Artificial Intelligence
+to the fingertips of the average Forensicator,
+and promote advances in the field
+```
+
+The first (modest) alpha version of our ds4n6 python library, together with some easy-to-use python scripts, was originally made public after the presentation at the SANS DFIR Summit US, July 16-17.
+**For detailed information about the Project, the Library, its Functions, its Usage, etc., visit the project page: http://www.ds4n6.io/tools/ds4n6.py.html**
+
+## Getting Started
+
+These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
+
+https://github.com/ds4n6/ds4n6_lib.git
+
+### Prerequisites
+
+The DS4N6 library works on the 3.x versions of the Python programming language. The module has external dependencies related to datascience and extraction of forensic evidence.
+
+Install requirements:
+
+    - python-evtx
+    - Evtx
+    - ipyaggrid
+    - IPython
+    - ipywidgets
+    - keras
+    - matplotlib
+    - nbformat
+    - numpy
+    - pandas
+    - pyparsing
+    - qgrid
+    - ruamel.yaml
+    - sklearn
+    - tensorflow
+    - tqdm
+    - traitlets
+    - xmltodict
+    - networkx
+    - gensim
+
+### Installation
+
+The installation can be easily done through pip.
+
+#### pip installation
+
+```sh
+    pip install python-evtx Evtx ipyaggrid IPython ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib
+```
+
+Finally, import in your python3 program or Jupyter Notebook as "ds".
+
+```python
+    import ds4n6_lib as ds
+```
+
+## Contributing
+
+If you think you can provide value to the Community, collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
+
+Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.
+
+### download from github
+
+All you will need to do is to clone the library, install the test, create a virtual enviroment to use it and active it.
+
+```sh
+    
+    git clone https://github.com/ds4n6/ds4n6_lib    
+
+    virtualenv -p python3.7 .test
+    source .test/bin/activate
+    
+    pip install -r requirements.txt 
+```
+
+## Authors
+
+* **Jess Garcia** - *Initial work* - http://ds4n6.io/community/jess_garcia.html
+
+See also the list of [contributors](http://ds4n6.io/community.html) who participated in this project.
+
+## License
+
+This project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE) file for details
```

#### html2text {}

```diff
@@ -1,13 +1,22 @@
-Metadata-Version: 2.1 Name: ds4n6_lib Version: 0.7.1 Summary: Bringing Data
+Metadata-Version: 2.1 Name: ds4n6-lib Version: 0.8.1 Summary: Bringing Data
 Science & Artificial Intelligence to the fingertips of the average
 Forensicator, and promote advances in the field Home-page: https://github.com/
 ds4n6/ds4n6_lib Author: Jess Garcia Author-email: ds4n6@one-esecurity.com
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/
-issues Project-URL: Website, http://www.ds4n6.io/ Description:
+Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/issues Project-
+URL: Website, http://www.ds4n6.io/ Keywords: dfir,datascience,forensics
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Framework :: Jupyter Classifier: Topic :: Security Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE License-
+File: LICENSE.md
                     [http://www.ds4n6.io/images/DS4N6.jpg]
  DS4N6 stands for Data Science Forensics. We also refer to this project as
 DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial
 Intelligence (AI), and the project goes beyond the strictly Forensics, covering
 the whole Digital Forensics & Incident Response (DFIR) discipline (and
 sometimes even beyond). But hey, we had to give the project a catchy name! The
 Mission of the DS4N6 project is simple: ``` Bringing Data Science & Artificial
@@ -21,34 +30,26 @@
 running on your local machine for development and testing purposes. See
 deployment for notes on how to deploy the project on a live system. https://
 github.com/ds4n6/ds4n6_lib.git ### Prerequisites The DS4N6 library works on the
 3.x versions of the Python programming language. The module has external
 dependencies related to datascience and extraction of forensic evidence.
 Install requirements: - python-evtx - Evtx - ipyaggrid - IPython - ipywidgets -
 keras - matplotlib - nbformat - numpy - pandas - pyparsing - qgrid -
-ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict ###
-Installation The installation can be easily done through pip. #### pip
-installation ```sh pip install python-evtx Evtx ipyaggrid IPython ipywidgets
-keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn
-tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in your
-python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as ds
-``` ## Contributing If you think you can provide value to the Community,
+ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict - networkx -
+gensim ### Installation The installation can be easily done through pip. ####
+pip installation ```sh pip install python-evtx Evtx ipyaggrid IPython
+ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml
+sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in
+your python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as
+ds ``` ## Contributing If you think you can provide value to the Community,
 collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
 Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/
 b24679402957c63ec426) for details on our code of conduct, and the process for
 submitting pull requests to us. ### download from github All you will need to
 do is to clone the library, install the test, create a virtual enviroment to
 use it and active it. ```sh git clone https://github.com/ds4n6/ds4n6_lib
 virtualenv -p python3.7 .test source .test/bin/activate pip install -
 r requirements.txt ``` ## Authors * **Jess Garcia** - *Initial work* - http://
 ds4n6.io/community/jess_garcia.html See also the list of [contributors](http://
 ds4n6.io/community.html) who participated in this project. ## License This
 project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE)
-file for details Keywords: dfir,datascience,forensics Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Framework :: Jupyter Classifier: Topic :: Security Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python:
->=3.6 Description-Content-Type: text/markdown
+file for details
```

### Comparing `ds4n6_lib-0.7.1/README.md` & `ds4n6_lib-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     - qgrid
     - ruamel.yaml
     - sklearn
     - tensorflow
     - tqdm
     - traitlets
     - xmltodict
+    - networkx
+    - gensim
 
 ### Installation
 
 The installation can be easily done through pip.
 
 #### pip installation
```

#### html2text {}

```diff
@@ -15,21 +15,21 @@
 running on your local machine for development and testing purposes. See
 deployment for notes on how to deploy the project on a live system. https://
 github.com/ds4n6/ds4n6_lib.git ### Prerequisites The DS4N6 library works on the
 3.x versions of the Python programming language. The module has external
 dependencies related to datascience and extraction of forensic evidence.
 Install requirements: - python-evtx - Evtx - ipyaggrid - IPython - ipywidgets -
 keras - matplotlib - nbformat - numpy - pandas - pyparsing - qgrid -
-ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict ###
-Installation The installation can be easily done through pip. #### pip
-installation ```sh pip install python-evtx Evtx ipyaggrid IPython ipywidgets
-keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn
-tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in your
-python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as ds
-``` ## Contributing If you think you can provide value to the Community,
+ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict - networkx -
+gensim ### Installation The installation can be easily done through pip. ####
+pip installation ```sh pip install python-evtx Evtx ipyaggrid IPython
+ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml
+sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in
+your python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as
+ds ``` ## Contributing If you think you can provide value to the Community,
 collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
 Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/
 b24679402957c63ec426) for details on our code of conduct, and the process for
 submitting pull requests to us. ### download from github All you will need to
 do is to clone the library, install the test, create a virtual enviroment to
 use it and active it. ```sh git clone https://github.com/ds4n6/ds4n6_lib
 virtualenv -p python3.7 .test source .test/bin/activate pip install -
```

### Comparing `ds4n6_lib-0.7.1/requirements.txt` & `ds4n6_lib-0.8.1/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 cycler==0.10.0
 decorator==5.0.5
 defusedxml==0.7.1
 entrypoints==0.3
 evtx==0.6.11
 flatbuffers==1.12
 gast==0.3.3
+gensim==4.2.0
 google-auth==1.28.0
 google-auth-oauthlib==0.4.4
 google-pasta==0.2.0
 grpcio==1.32.0
 h5py==2.10.0
 hexdump==3.3
 idna==2.10
@@ -46,14 +47,15 @@
 matplotlib==3.4.1
 mistune==0.8.4
 more-itertools==5.0.0
 nbclient==0.5.3
 nbconvert==6.0.7
 nbformat==5.1.3
 nest-asyncio==1.5.1
+networkx==2.5
 notebook==6.3.0
 numpy==1.19.5
 oauthlib==3.1.0
 opt-einsum==3.3.0
 packaging==20.9
 pandas==1.2.3
 pandocfilters==1.4.3
@@ -103,8 +105,8 @@
 urllib3==1.26.4
 wcwidth==0.2.5
 webencodings==0.5.1
 Werkzeug==1.0.1
 widgetsnbextension==3.5.1
 wrapt==1.12.1
 xmltodict==0.12.0
-zipp==1.0.0
+zipp==1.0.0
```

### Comparing `ds4n6_lib-0.7.1/setup.py` & `ds4n6_lib-0.8.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ds4n6_lib",
-    version="0.7.1",
+    version="0.8.1",
     author="Jess Garcia",
     author_email="ds4n6@one-esecurity.com",
     description="Bringing Data Science & Artificial Intelligence to the fingertips of the average Forensicator, and promote advances in the field",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds4n6/ds4n6_lib",
     project_urls={
@@ -35,14 +35,16 @@
           'qgrid',
           'ruamel.yaml',
           'sklearn',
           'tensorflow',
           'tqdm',
           'traitlets',
           'xmltodict',
+          'networkx',
+          'gensim',
       ],
     classifiers=[
       "Development Status :: 3 - Alpha",
       "Intended Audience :: Developers",
       "Intended Audience :: Information Technology",
       "Framework :: Jupyter",
       "Topic :: Security",
```

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/amcache.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/amcache.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/autoruns.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/autoruns.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/common.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/common.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/d4.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/d4.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/evtx.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/evtx.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/evtx_parser.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/evtx_parser.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/flist.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/flist.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/fstl.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/fstl.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/gui.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/gui.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/kansa.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/kansa.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/kape.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/kape.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/knowledge.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/knowledge.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/macrobber.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/macrobber.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/mactime.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/mactime.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/ml.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/ml.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/pf.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/pf.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/plaso.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/plaso.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/pslist.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/pslist.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/sabonis.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/sabonis.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/svclist.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/svclist.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/tshark.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/tshark.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/unx.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/unx.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/utils.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/utils.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/volatility.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/volatility.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib/winreg.py` & `ds4n6_lib-0.8.1/src/ds4n6_lib/winreg.py`

 * *Files identical despite different names*

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/PKG-INFO` & `ds4n6_lib-0.8.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,128 @@
 Metadata-Version: 2.1
-Name: ds4n6-lib
-Version: 0.7.1
+Name: ds4n6_lib
+Version: 0.8.1
 Summary: Bringing Data Science & Artificial Intelligence to the fingertips of the average Forensicator, and promote advances in the field
 Home-page: https://github.com/ds4n6/ds4n6_lib
 Author: Jess Garcia
 Author-email: ds4n6@one-esecurity.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/issues
 Project-URL: Website, http://www.ds4n6.io/
-Description: <!-- PROJECT LOGO -->
-        
-        <p align="center">
-          <a href="http://www.ds4n6.io">
-            <img src="http://www.ds4n6.io/images/DS4N6.jpg">
-          </a>
-        </p>
-        
-        <a href="http://www.ds4n6.io" title=""><img src="http://ds4n6.io/images/logo-s.png" alt="" /></a>
-        
-        DS4N6 stands for Data Science Forensics.
-        
-        We also refer to this project as DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial Intelligence (AI), and the project goes beyond the strictly Forensics, covering the whole Digital Forensics & Incident Response (DFIR) discipline (and sometimes even beyond). But hey, we had to give the project a catchy name!
-        
-        The Mission of the DS4N6 project is simple:
-        
-        ```
-        Bringing Data Science & Artificial Intelligence
-        to the fingertips of the average Forensicator,
-        and promote advances in the field
-        ```
-        
-        The first (modest) alpha version of our ds4n6 python library, together with some easy-to-use python scripts, was originally made public after the presentation at the SANS DFIR Summit US, July 16-17.
-        **For detailed information about the Project, the Library, its Functions, its Usage, etc., visit the project page: http://www.ds4n6.io/tools/ds4n6.py.html**
-        
-        ## Getting Started
-        
-        These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
-        
-        https://github.com/ds4n6/ds4n6_lib.git
-        
-        ### Prerequisites
-        
-        The DS4N6 library works on the 3.x versions of the Python programming language. The module has external dependencies related to datascience and extraction of forensic evidence.
-        
-        Install requirements:
-        
-            - python-evtx
-            - Evtx
-            - ipyaggrid
-            - IPython
-            - ipywidgets
-            - keras
-            - matplotlib
-            - nbformat
-            - numpy
-            - pandas
-            - pyparsing
-            - qgrid
-            - ruamel.yaml
-            - sklearn
-            - tensorflow
-            - tqdm
-            - traitlets
-            - xmltodict
-        
-        ### Installation
-        
-        The installation can be easily done through pip.
-        
-        #### pip installation
-        
-        ```sh
-            pip install python-evtx Evtx ipyaggrid IPython ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib
-        ```
-        
-        Finally, import in your python3 program or Jupyter Notebook as "ds".
-        
-        ```python
-            import ds4n6_lib as ds
-        ```
-        
-        ## Contributing
-        
-        If you think you can provide value to the Community, collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
-        
-        Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.
-        
-        ### download from github
-        
-        All you will need to do is to clone the library, install the test, create a virtual enviroment to use it and active it.
-        
-        ```sh
-            
-            git clone https://github.com/ds4n6/ds4n6_lib    
-        
-            virtualenv -p python3.7 .test
-            source .test/bin/activate
-            
-            pip install -r requirements.txt 
-        ```
-        
-        ## Authors
-        
-        * **Jess Garcia** - *Initial work* - http://ds4n6.io/community/jess_garcia.html
-        
-        See also the list of [contributors](http://ds4n6.io/community.html) who participated in this project.
-        
-        ## License
-        
-        This project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE) file for details
-        
 Keywords: dfir,datascience,forensics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.md
+
+<!-- PROJECT LOGO -->
+
+<p align="center">
+  <a href="http://www.ds4n6.io">
+    <img src="http://www.ds4n6.io/images/DS4N6.jpg">
+  </a>
+</p>
+
+<a href="http://www.ds4n6.io" title=""><img src="http://ds4n6.io/images/logo-s.png" alt="" /></a>
+
+DS4N6 stands for Data Science Forensics.
+
+We also refer to this project as DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial Intelligence (AI), and the project goes beyond the strictly Forensics, covering the whole Digital Forensics & Incident Response (DFIR) discipline (and sometimes even beyond). But hey, we had to give the project a catchy name!
+
+The Mission of the DS4N6 project is simple:
+
+```
+Bringing Data Science & Artificial Intelligence
+to the fingertips of the average Forensicator,
+and promote advances in the field
+```
+
+The first (modest) alpha version of our ds4n6 python library, together with some easy-to-use python scripts, was originally made public after the presentation at the SANS DFIR Summit US, July 16-17.
+**For detailed information about the Project, the Library, its Functions, its Usage, etc., visit the project page: http://www.ds4n6.io/tools/ds4n6.py.html**
+
+## Getting Started
+
+These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
+
+https://github.com/ds4n6/ds4n6_lib.git
+
+### Prerequisites
+
+The DS4N6 library works on the 3.x versions of the Python programming language. The module has external dependencies related to datascience and extraction of forensic evidence.
+
+Install requirements:
+
+    - python-evtx
+    - Evtx
+    - ipyaggrid
+    - IPython
+    - ipywidgets
+    - keras
+    - matplotlib
+    - nbformat
+    - numpy
+    - pandas
+    - pyparsing
+    - qgrid
+    - ruamel.yaml
+    - sklearn
+    - tensorflow
+    - tqdm
+    - traitlets
+    - xmltodict
+    - networkx
+    - gensim
+
+### Installation
+
+The installation can be easily done through pip.
+
+#### pip installation
+
+```sh
+    pip install python-evtx Evtx ipyaggrid IPython ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib
+```
+
+Finally, import in your python3 program or Jupyter Notebook as "ds".
+
+```python
+    import ds4n6_lib as ds
+```
+
+## Contributing
+
+If you think you can provide value to the Community, collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
+
+Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.
+
+### download from github
+
+All you will need to do is to clone the library, install the test, create a virtual enviroment to use it and active it.
+
+```sh
+    
+    git clone https://github.com/ds4n6/ds4n6_lib    
+
+    virtualenv -p python3.7 .test
+    source .test/bin/activate
+    
+    pip install -r requirements.txt 
+```
+
+## Authors
+
+* **Jess Garcia** - *Initial work* - http://ds4n6.io/community/jess_garcia.html
+
+See also the list of [contributors](http://ds4n6.io/community.html) who participated in this project.
+
+## License
+
+This project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE) file for details
```

#### html2text {}

```diff
@@ -1,13 +1,22 @@
-Metadata-Version: 2.1 Name: ds4n6-lib Version: 0.7.1 Summary: Bringing Data
+Metadata-Version: 2.1 Name: ds4n6_lib Version: 0.8.1 Summary: Bringing Data
 Science & Artificial Intelligence to the fingertips of the average
 Forensicator, and promote advances in the field Home-page: https://github.com/
 ds4n6/ds4n6_lib Author: Jess Garcia Author-email: ds4n6@one-esecurity.com
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/
-issues Project-URL: Website, http://www.ds4n6.io/ Description:
+Project-URL: Bug Tracker, https://github.com/ds4n6/ds4n6_lib/issues Project-
+URL: Website, http://www.ds4n6.io/ Keywords: dfir,datascience,forensics
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Framework :: Jupyter Classifier: Topic :: Security Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE License-
+File: LICENSE.md
                     [http://www.ds4n6.io/images/DS4N6.jpg]
  DS4N6 stands for Data Science Forensics. We also refer to this project as
 DSDFIR, AI4N6 or AIDFIR, since Data Science (DS) includes Artificial
 Intelligence (AI), and the project goes beyond the strictly Forensics, covering
 the whole Digital Forensics & Incident Response (DFIR) discipline (and
 sometimes even beyond). But hey, we had to give the project a catchy name! The
 Mission of the DS4N6 project is simple: ``` Bringing Data Science & Artificial
@@ -21,34 +30,26 @@
 running on your local machine for development and testing purposes. See
 deployment for notes on how to deploy the project on a live system. https://
 github.com/ds4n6/ds4n6_lib.git ### Prerequisites The DS4N6 library works on the
 3.x versions of the Python programming language. The module has external
 dependencies related to datascience and extraction of forensic evidence.
 Install requirements: - python-evtx - Evtx - ipyaggrid - IPython - ipywidgets -
 keras - matplotlib - nbformat - numpy - pandas - pyparsing - qgrid -
-ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict ###
-Installation The installation can be easily done through pip. #### pip
-installation ```sh pip install python-evtx Evtx ipyaggrid IPython ipywidgets
-keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml sklearn
-tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in your
-python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as ds
-``` ## Contributing If you think you can provide value to the Community,
+ruamel.yaml - sklearn - tensorflow - tqdm - traitlets - xmltodict - networkx -
+gensim ### Installation The installation can be easily done through pip. ####
+pip installation ```sh pip install python-evtx Evtx ipyaggrid IPython
+ipywidgets keras matplotlib nbformat numpy pandas pyparsing qgrid ruamel.yaml
+sklearn tensorflow tqdm traitlets xmltodict ds4n6-lib ``` Finally, import in
+your python3 program or Jupyter Notebook as "ds". ```python import ds4n6_lib as
+ds ``` ## Contributing If you think you can provide value to the Community,
 collaborating with Research, Blog Posts, Cheatsheets, Code, etc., contact us!
 Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/
 b24679402957c63ec426) for details on our code of conduct, and the process for
 submitting pull requests to us. ### download from github All you will need to
 do is to clone the library, install the test, create a virtual enviroment to
 use it and active it. ```sh git clone https://github.com/ds4n6/ds4n6_lib
 virtualenv -p python3.7 .test source .test/bin/activate pip install -
 r requirements.txt ``` ## Authors * **Jess Garcia** - *Initial work* - http://
 ds4n6.io/community/jess_garcia.html See also the list of [contributors](http://
 ds4n6.io/community.html) who participated in this project. ## License This
 project is licensed under the GNU GPL v3.0 License - see the [LICENSE](LICENSE)
-file for details Keywords: dfir,datascience,forensics Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Framework :: Jupyter Classifier: Topic :: Security Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python:
->=3.6 Description-Content-Type: text/markdown
+file for details
```

### Comparing `ds4n6_lib-0.7.1/src/ds4n6_lib.egg-info/SOURCES.txt` & `ds4n6_lib-0.8.1/src/ds4n6_lib.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/ds4n6_lib/__init__.py
@@ -17,22 +18,26 @@
 src/ds4n6_lib/gui.py
 src/ds4n6_lib/kansa.py
 src/ds4n6_lib/kape.py
 src/ds4n6_lib/knowledge.py
 src/ds4n6_lib/macrobber.py
 src/ds4n6_lib/mactime.py
 src/ds4n6_lib/ml.py
+src/ds4n6_lib/mlgraph.py
 src/ds4n6_lib/pf.py
 src/ds4n6_lib/plaso.py
 src/ds4n6_lib/pslist.py
 src/ds4n6_lib/sabonis.py
 src/ds4n6_lib/svclist.py
 src/ds4n6_lib/tshark.py
 src/ds4n6_lib/unx.py
 src/ds4n6_lib/utils.py
 src/ds4n6_lib/volatility.py
 src/ds4n6_lib/winreg.py
 src/ds4n6_lib.egg-info/PKG-INFO
 src/ds4n6_lib.egg-info/SOURCES.txt
 src/ds4n6_lib.egg-info/dependency_links.txt
 src/ds4n6_lib.egg-info/requires.txt
-src/ds4n6_lib.egg-info/top_level.txt
+src/ds4n6_lib.egg-info/top_level.txt
+src/ds4n6_lib/ml_modules/__init__.py
+src/ds4n6_lib/ml_modules/seq2seq_lstm.py
+src/ds4n6_lib/ml_modules/transformer.py
```

