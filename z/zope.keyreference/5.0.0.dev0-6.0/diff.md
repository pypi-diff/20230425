# Comparing `tmp/zope.keyreference-5.0.0.dev0.tar.gz` & `tmp/zope.keyreference-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.keyreference-5.0.0.dev0.tar", last modified: Fri Mar 25 07:09:33 2022, max compression
+gzip compressed data, was "zope.keyreference-6.0.tar", last modified: Tue Apr 25 07:23:32 2023, max compression
```

## Comparing `zope.keyreference-5.0.0.dev0.tar` & `zope.keyreference-6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.196360 zope.keyreference-5.0.0.dev0/
--rw-r--r--   0 mac        (513) staff       (20)     2007 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      458 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4539 2022-03-25 07:09:33.196465 zope.keyreference-5.0.0.dev0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1091 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      180 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)       87 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.191275 zope.keyreference-5.0.0.dev0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    10610 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      600 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       53 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/persistent.rst
--rw-r--r--   0 mac        (513) staff       (20)      189 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/docs/reference.rst
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-03-25 07:09:33.196959 zope.keyreference-5.0.0.dev0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3361 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.185041 zope.keyreference-5.0.0.dev0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.191569 zope.keyreference-5.0.0.dev0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.196142 zope.keyreference-5.0.0.dev0/src/zope/keyreference/
--rw-r--r--   0 mac        (513) staff       (20)      664 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      841 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2005 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     5866 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/persistent.py
--rw-r--r--   0 mac        (513) staff       (20)     8992 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/persistent.txt
--rw-r--r--   0 mac        (513) staff       (20)     1967 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/testing.py
--rw-r--r--   0 mac        (513) staff       (20)     3657 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/src/zope/keyreference/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-25 07:09:33.193849 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4539 2022-03-25 07:09:32.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      836 2022-03-25 07:09:33.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-25 07:09:32.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-25 07:09:32.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-25 07:09:32.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-03-25 07:09:33.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-25 07:09:33.000000 zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1389 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/tox.ini
--rw-r--r--   0 mac        (513) staff       (20)       11 2022-03-25 07:09:31.000000 zope.keyreference-5.0.0.dev0/version.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.852697 zope.keyreference-6.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2174 2023-04-25 07:23:32.000000 zope.keyreference-6.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-04-25 07:23:32.000000 zope.keyreference-6.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-04-25 07:23:32.000000 zope.keyreference-6.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-04-25 07:23:32.000000 zope.keyreference-6.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      458 2023-04-25 07:23:32.000000 zope.keyreference-6.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4532 2023-04-25 07:23:32.852778 zope.keyreference-6.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1091 2023-04-25 07:23:32.000000 zope.keyreference-6.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      180 2023-04-25 07:23:32.000000 zope.keyreference-6.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)       87 2023-04-25 07:23:32.000000 zope.keyreference-6.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.849740 zope.keyreference-6.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10610 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      600 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/persistent.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      189 2023-04-25 07:23:32.000000 zope.keyreference-6.0/docs/reference.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      446 2023-04-25 07:23:32.853175 zope.keyreference-6.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3240 2023-04-25 07:23:32.000000 zope.keyreference-6.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.846567 zope.keyreference-6.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.849904 zope.keyreference-6.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.852531 zope.keyreference-6.0/src/zope/keyreference/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      841 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2006 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5858 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/persistent.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8992 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/persistent.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1960 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3484 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope/keyreference/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 07:23:32.851215 zope.keyreference-6.0/src/zope.keyreference.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4532 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      836 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      174 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-25 07:23:32.000000 zope.keyreference-6.0/src/zope.keyreference.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1579 2023-04-25 07:23:32.000000 zope.keyreference-6.0/tox.ini
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-04-25 07:23:32.000000 zope.keyreference-6.0/version.txt
```

### Comparing `zope.keyreference-5.0.0.dev0/CHANGES.rst` & `zope.keyreference-6.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 =========
  Changes
 =========
 
-5.0.0 (unreleased)
+6.0 (2023-04-25)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+- Make the tests compatible with ``zope.testing >= 5``.
+
+
+5.0.0 (2022-03-25)
 ==================
 
 - Remove ``__cmp__`` methods. Since the implementation of the rich
   comparison methods (``__eq__``, etc) in 4.0a1, the interpreter won't
   call ``__cmp__``, even on Python 2. See `issue 10
   <https://github.com/zopefoundation/zope.keyreference/issues/10>`_.
```

### Comparing `zope.keyreference-5.0.0.dev0/CONTRIBUTING.md` & `zope.keyreference-6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/LICENSE.txt` & `zope.keyreference-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/PKG-INFO` & `zope.keyreference-6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: zope.keyreference
-Version: 5.0.0.dev0
+Version: 6.0
 Summary: Key References
 Home-page: https://github.com/zopefoundation/zope.keyreference
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopekeyreference.readthedocs.io/
 Keywords: zope3 key reference persistent
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
 Provides-Extra: test
@@ -62,15 +58,25 @@
 Documentation can be found at https://zopekeyreference.readthedocs.io
 
 
 =========
  Changes
 =========
 
-5.0.0 (unreleased)
+6.0 (2023-04-25)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+- Make the tests compatible with ``zope.testing >= 5``.
+
+
+5.0.0 (2022-03-25)
 ==================
 
 - Remove ``__cmp__`` methods. Since the implementation of the rich
   comparison methods (``__eq__``, etc) in 4.0a1, the interpreter won't
   call ``__cmp__``, even on Python 2. See `issue 10
   <https://github.com/zopefoundation/zope.keyreference/issues/10>`_.
 
@@ -146,9 +152,7 @@
   if its not installed anymore (so don't break if one updates a
   project that don't directly depends on zope.app.keyreference).
 
 3.6.0 (2009-01-31)
 ==================
 
 - Rename ``zope.app.keyreference`` to ``zope.keyreference``.
-
-
```

### Comparing `zope.keyreference-5.0.0.dev0/README.rst` & `zope.keyreference-6.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/docs/Makefile` & `zope.keyreference-6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/docs/conf.py` & `zope.keyreference-6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/docs/index.rst` & `zope.keyreference-6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/setup.py` & `zope.keyreference-6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 # http://docs.zope.org/zopetoolkit
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.keyreference package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -46,23 +48,20 @@
     keywords="zope3 key reference persistent",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Zope Public License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP",
         "Framework :: Zope :: 3",
     ],
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/__init__.py` & `zope.keyreference-6.0/src/zope/keyreference/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/configure.zcml` & `zope.keyreference-6.0/src/zope/keyreference/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/interfaces.py` & `zope.keyreference-6.0/src/zope/keyreference/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Key-reference interfaces
 """
 import zope.interface
-from zope.schema import DottedName
 from zope.i18nmessageid import MessageFactory
+from zope.schema import DottedName
+
 
 _ = MessageFactory('zope')
 
 
 class NotYet(Exception):
     """Can't compute a key reference for an object
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/persistent.py` & `zope.keyreference-6.0/src/zope/keyreference/persistent.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """KeyReference for persistent objects.
 
 Provides an IKeyReference adapter for persistent objects.
 """
-from ZODB.interfaces import IConnection
-from ZODB.ConflictResolution import PersistentReference
 import zope.interface
+from ZODB.ConflictResolution import PersistentReference
+from ZODB.interfaces import IConnection
 
 import zope.keyreference.interfaces
 
 
 @zope.interface.implementer(zope.keyreference.interfaces.IKeyReference)
-class KeyReferenceToPersistent(object):
+class KeyReferenceToPersistent:
     """An IKeyReference for persistent objects which is comparable.
 
     These references compare by database name and _p_oids of the objects they
     reference.
     """
 
     key_type_id = 'zope.app.keyreference.persistent'
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/persistent.txt` & `zope.keyreference-6.0/src/zope/keyreference/persistent.txt`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/testing.py` & `zope.keyreference-6.0/src/zope/keyreference/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """
 Testing components.
 """
 
-import zope.interface
 import zope.component
+import zope.interface
+
 import zope.keyreference.interfaces
 
 
 @zope.component.adapter(zope.interface.Interface)
 @zope.interface.implementer(zope.keyreference.interfaces.IKeyReference)
-class SimpleKeyReference(object):
+class SimpleKeyReference:
     """An IReference for all objects. This implementation is *not*
     ZODB safe.
 
     """
 
     key_type_id = 'zope.app.keyreference.simple'
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope/keyreference/tests.py` & `zope.keyreference-6.0/src/zope/keyreference/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the unique id utility.
 """
 import doctest
 import unittest
-from zope.testing import renormalizing
 
 
-class MockDatabase(object):
+class MockDatabase:
     database_name = ''
 
 
-class MockJar(object):
+class MockJar:
 
     def __init__(self):
         self._db = MockDatabase()
 
     def db(self):
         return self._db
 
 
-class MockPersistent(object):
+class MockPersistent:
     _p_oid = 1
     _p_jar = MockJar()
 
     def __hash__(self):
         # SimpleKeyReference depends on hash
         return hash(self._p_oid)
 
@@ -84,17 +83,17 @@
 class TestKeyReferenceToPersistent(TestSimpleKeyReference):
 
     def makeOne(self, obj):
         from zope.keyreference.persistent import KeyReferenceToPersistent
         return KeyReferenceToPersistent(obj)
 
     def test_multi_databases(self):
-        from ZODB.MappingStorage import DB
         import transaction
         from BTrees.OOBTree import OOBucket
+        from ZODB.MappingStorage import DB
 
         databases = {}
 
         db1 = DB(databases=databases, database_name='1')
         db2 = DB(databases=databases, database_name='2')
 
         conn1 = db1.open()
@@ -117,17 +116,15 @@
         self.assertNotEqual(hash(key1), hash(key2))
 
 
 def test_suite():
     doctest_flags = (
         doctest.NORMALIZE_WHITESPACE
         | doctest.ELLIPSIS
-        | renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2
     )
     return unittest.TestSuite((
         doctest.DocFileSuite(
             'persistent.txt',
             optionflags=doctest_flags,
-            checker=renormalizing.RENormalizing(),
         ),
         unittest.defaultTestLoader.loadTestsFromName(__name__),
     ))
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/PKG-INFO` & `zope.keyreference-6.0/src/zope.keyreference.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: zope.keyreference
-Version: 5.0.0.dev0
+Version: 6.0
 Summary: Key References
 Home-page: https://github.com/zopefoundation/zope.keyreference
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopekeyreference.readthedocs.io/
 Keywords: zope3 key reference persistent
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
 Provides-Extra: test
@@ -62,15 +58,25 @@
 Documentation can be found at https://zopekeyreference.readthedocs.io
 
 
 =========
  Changes
 =========
 
-5.0.0 (unreleased)
+6.0 (2023-04-25)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+- Make the tests compatible with ``zope.testing >= 5``.
+
+
+5.0.0 (2022-03-25)
 ==================
 
 - Remove ``__cmp__`` methods. Since the implementation of the rich
   comparison methods (``__eq__``, etc) in 4.0a1, the interpreter won't
   call ``__cmp__``, even on Python 2. See `issue 10
   <https://github.com/zopefoundation/zope.keyreference/issues/10>`_.
 
@@ -146,9 +152,7 @@
   if its not installed anymore (so don't break if one updates a
   project that don't directly depends on zope.app.keyreference).
 
 3.6.0 (2009-01-31)
 ==================
 
 - Rename ``zope.app.keyreference`` to ``zope.keyreference``.
-
-
```

### Comparing `zope.keyreference-5.0.0.dev0/src/zope.keyreference.egg-info/SOURCES.txt` & `zope.keyreference-6.0/src/zope.keyreference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.keyreference-5.0.0.dev0/tox.ini` & `zope.keyreference-6.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
@@ -23,23 +20,34 @@
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 extras =
     docs
 commands_pre =
@@ -48,24 +56,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=100
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.keyreference
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

