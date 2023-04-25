# Comparing `tmp/discake-0.0.3.tar.gz` & `tmp/discake-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discake-0.0.3.tar", last modified: Tue Apr 25 08:22:29 2023, max compression
+gzip compressed data, was "discake-0.0.4.tar", last modified: Tue Apr 25 08:29:37 2023, max compression
```

## Comparing `discake-0.0.3.tar` & `discake-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:22:29.496448 discake-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 08:22:16.000000 discake-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 08:22:29.496448 discake-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 08:22:16.000000 discake-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:22:29.496448 discake-0.0.3/discake/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 08:22:16.000000 discake-0.0.3/discake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:22:29.496448 discake-0.0.3/discake/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-25 08:22:16.000000 discake-0.0.3/discake/paginator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:22:29.496448 discake-0.0.3/discake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:22:16.000000 discake-0.0.3/discake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-25 08:22:16.000000 discake-0.0.3/discake/utils/paginate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:22:29.496448 discake-0.0.3/discake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 08:22:29.000000 discake-0.0.3/discake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 08:22:29.000000 discake-0.0.3/discake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:22:29.000000 discake-0.0.3/discake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 08:22:29.000000 discake-0.0.3/discake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:22:29.000000 discake-0.0.3/discake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:22:29.496448 discake-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-25 08:22:16.000000 discake-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:29:37.752896 discake-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 08:29:22.000000 discake-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 08:29:37.752896 discake-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 08:29:22.000000 discake-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:29:37.752896 discake-0.0.4/discake/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 08:29:22.000000 discake-0.0.4/discake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:29:37.752896 discake-0.0.4/discake/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-25 08:29:22.000000 discake-0.0.4/discake/paginator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:29:37.752896 discake-0.0.4/discake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:29:22.000000 discake-0.0.4/discake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-25 08:29:22.000000 discake-0.0.4/discake/utils/paginate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:29:37.752896 discake-0.0.4/discake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 08:29:37.000000 discake-0.0.4/discake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 08:29:37.000000 discake-0.0.4/discake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:29:37.000000 discake-0.0.4/discake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 08:29:37.000000 discake-0.0.4/discake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:29:37.000000 discake-0.0.4/discake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:29:37.752896 discake-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-25 08:29:22.000000 discake-0.0.4/setup.py
```

### Comparing `discake-0.0.3/LICENSE` & `discake-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discake-0.0.3/PKG-INFO` & `discake-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.3
+Version: 0.0.4
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discake-0.0.3/README.rst` & `discake-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `discake-0.0.3/discake/paginator/__init__.py` & `discake-0.0.4/discake/paginator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union, List, Any, Optional
 
 from discord import Embed, Interaction
 from discord.ext.commands import Context
 
-from utils import ButtonsView
+from discake import ButtonsView
 
 if TYPE_CHECKING:
     from discord import Member, Message, InteractionMessage, WebhookMessage
     
 __all__ = (
   'Paginator'
 )
```

### Comparing `discake-0.0.3/discake/utils/paginate.py` & `discake-0.0.4/discake/utils/paginate.py`

 * *Files identical despite different names*

### Comparing `discake-0.0.3/discake.egg-info/PKG-INFO` & `discake-0.0.4/discake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.3
+Version: 0.0.4
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discake-0.0.3/setup.py` & `discake-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.rst', 'r') as file:
     readme = file.read()
     
 setup(
     name='discake',
     author='Carlos',
     url='https://github.com/lollipop-69/discake',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     description='A discord py support library containing utilities.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     install_requires=[
         'discord.py'
     ],
```

