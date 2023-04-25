# Comparing `tmp/certfrtracker-1.6.2.tar.gz` & `tmp/certfrtracker-1.6.3.tar.gz`

## Comparing `certfrtracker-1.6.2.tar` & `certfrtracker-1.6.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/requirements.txt
--rwxr-xr-x   0        0        0     2516 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/NVD.py
--rwxr-xr-x   0        0        0    11190 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/Router.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/__init__.py
--rwxr-xr-x   0        0        0     4970 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/html_parser.py
--rwxr-xr-x   0        0        0     5474 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/sqlite.py
--rwxr-xr-x   0        0        0     8948 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/src/certfrtracker/version_parser.py
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/.gitignore
--rwxr-xr-x   0        0        0    35148 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/LICENSE
--rwxr-xr-x   0        0        0     3376 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/README.md
--rwxr-xr-x   0        0        0      739 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/pyproject.toml
--rw-r--r--   0        0        0    44561 2020-02-02 00:00:00.000000 certfrtracker-1.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0      430 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/22.1.0
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/requirements.txt
+-rwxr-xr-x   0        0        0     2516 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/NVD.py
+-rwxr-xr-x   0        0        0    11190 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/Router.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/__init__.py
+-rwxr-xr-x   0        0        0     4970 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/html_parser.py
+-rwxr-xr-x   0        0        0     5474 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/sqlite.py
+-rwxr-xr-x   0        0        0     8948 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/src/certfrtracker/version_parser.py
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/.gitignore
+-rwxr-xr-x   0        0        0    35148 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/LICENSE
+-rwxr-xr-x   0        0        0     3386 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/README.md
+-rwxr-xr-x   0        0        0      739 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0    44571 2020-02-02 00:00:00.000000 certfrtracker-1.6.3/PKG-INFO
```

### Comparing `certfrtracker-1.6.2/src/certfrtracker/NVD.py` & `certfrtracker-1.6.3/src/certfrtracker/NVD.py`

 * *Files identical despite different names*

### Comparing `certfrtracker-1.6.2/src/certfrtracker/Router.py` & `certfrtracker-1.6.3/src/certfrtracker/Router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import feedparser
 import requests
 import sys
 
-import Certfrtracker.NVD as NVD
-import Certfrtracker.html_parser as html_parser
-from Certfrtracker.sqlite import Sqlite
-from Certfrtracker.version_parser import systems_filter
+import certfrtracker.NVD as NVD
+import certfrtracker.html_parser as html_parser
+from certfrtracker.sqlite import Sqlite
+from certfrtracker.version_parser import systems_filter
 
 logger = logging.getLogger(__name__)
 
 
 class Report:
     """
     Plain object returned by Router class as list of Report.
```

### Comparing `certfrtracker-1.6.2/src/certfrtracker/html_parser.py` & `certfrtracker-1.6.3/src/certfrtracker/html_parser.py`

 * *Files identical despite different names*

### Comparing `certfrtracker-1.6.2/src/certfrtracker/sqlite.py` & `certfrtracker-1.6.3/src/certfrtracker/sqlite.py`

 * *Files identical despite different names*

### Comparing `certfrtracker-1.6.2/src/certfrtracker/version_parser.py` & `certfrtracker-1.6.3/src/certfrtracker/version_parser.py`

 * *Files identical despite different names*

### Comparing `certfrtracker-1.6.2/LICENSE` & `certfrtracker-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `certfrtracker-1.6.2/README.md` & `certfrtracker-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,9 +92,9 @@
 git push
 git rm dist/*
 python3 -m build
 git add dist/*
 git commit -m "pushing last build"
 git push
 python3 -m twine upload dist/*
-pip3 install CertfrTracker
+pip3 install --upgrade CertfrTracker
 ```
```

### Comparing `certfrtracker-1.6.2/pyproject.toml` & `certfrtracker-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "CertfrTracker"
-version = "1.6.2"
+version = "1.6.3"
 authors = [
   { name="MURARO Arthur", email="arthur.muraro7@gmail.com" },
 ]
 description = "This is the 'light' version of CertfrTracker-CLI, it only handles the scrapping of CertFr and the comparison system. You will have to provide the inventory system."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.0"
```

### Comparing `certfrtracker-1.6.2/PKG-INFO` & `certfrtracker-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CertfrTracker
-Version: 1.6.2
+Version: 1.6.3
 Summary: This is the 'light' version of CertfrTracker-CLI, it only handles the scrapping of CertFr and the comparison system. You will have to provide the inventory system.
 Project-URL: Homepage, https://gitlab.com/arthur_muraro/python-certfr/-/tree/pypi-package
 Author-email: MURARO Arthur <arthur.muraro7@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -779,9 +779,9 @@
 git push
 git rm dist/*
 python3 -m build
 git add dist/*
 git commit -m "pushing last build"
 git push
 python3 -m twine upload dist/*
-pip3 install CertfrTracker
+pip3 install --upgrade CertfrTracker
 ```
```

