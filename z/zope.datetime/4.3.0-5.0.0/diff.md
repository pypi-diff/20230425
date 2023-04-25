# Comparing `tmp/zope.datetime-4.3.0.tar.gz` & `tmp/zope.datetime-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zope.datetime-4.3.0.tar", last modified: Fri Feb 26 15:38:40 2021, max compression
+gzip compressed data, was "zope.datetime-5.0.0.tar", last modified: Tue Apr 25 06:14:08 2023, max compression
```

## Comparing `zope.datetime-4.3.0.tar` & `zope.datetime-5.0.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/
--rw-r--r--   0 mac        (513) staff       (20)     1794 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      443 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4903 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1103 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       95 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)     1063 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    10646 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      450 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      232 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2973 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope/datetime/
--rw-r--r--   0 mac        (513) staff       (20)    36838 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope/datetime/tests/
--rw-r--r--   0 mac        (513) staff       (20)       32 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     9521 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_datetime.py
--rw-r--r--   0 mac        (513) staff       (20)     4717 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_datetimeparse.py
--rw-r--r--   0 mac        (513) staff       (20)     2552 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_lp_139360.py
--rw-r--r--   0 mac        (513) staff       (20)     3207 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_standard_dates.py
--rw-r--r--   0 mac        (513) staff       (20)     1093 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_timezones.py
--rw-r--r--   0 mac        (513) staff       (20)     1607 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/tests/test_tzinfo.py
--rw-r--r--   0 mac        (513) staff       (20)    98885 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/src/zope/datetime/timezones.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4903 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      843 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       71 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2021-02-26 15:38:40.000000 zope.datetime-4.3.0/src/zope.datetime.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1391 2021-02-26 15:38:39.000000 zope.datetime-4.3.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.142327 zope.datetime-5.0.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1914 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      315 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4157 2023-04-25 06:14:08.142395 zope.datetime-5.0.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1107 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       95 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.139564 zope.datetime-5.0.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1063 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10646 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      450 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      505 2023-04-25 06:14:08.142726 zope.datetime-5.0.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2911 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.137122 zope.datetime-5.0.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.139699 zope.datetime-5.0.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.141095 zope.datetime-5.0.0/src/zope/datetime/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    36804 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.142192 zope.datetime-5.0.0/src/zope/datetime/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9495 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_datetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4792 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_datetimeparse.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2583 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_lp_139360.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3207 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_standard_dates.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1093 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_timezones.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1607 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/tests/test_tzinfo.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    98856 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/src/zope/datetime/timezones.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:14:08.140786 zope.datetime-5.0.0/src/zope.datetime.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4157 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      859 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-25 06:14:08.000000 zope.datetime-5.0.0/src/zope.datetime.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1574 2023-04-25 06:14:06.000000 zope.datetime-5.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zope.datetime-4.3.0/CHANGES.rst` & `zope.datetime-5.0.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  CHANGES
 =========
 
+5.0.0 (2023-04-25)
+==================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.10, 3.11.
+
+
 4.3.0 (2021-02-26)
 ==================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.7, 3.8 and 3.9.
```

### Comparing `zope.datetime-4.3.0/LICENSE.txt` & `zope.datetime-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.datetime-4.3.0/PKG-INFO` & `zope.datetime-5.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,136 @@
 Metadata-Version: 2.1
 Name: zope.datetime
-Version: 4.3.0
+Version: 5.0.0
 Summary: Zope datetime
 Home-page: http://github.com/zopefoundation/zope.datetime
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Description: ===================
-         ``zope.datetime``
-        ===================
-        
-        .. image:: https://img.shields.io/pypi/v/zope.datetime.svg
-                :target: https://pypi.python.org/pypi/zope.datetime/
-                :alt: Latest release
-        
-        .. image:: https://img.shields.io/pypi/pyversions/zope.datetime.svg
-                :target: https://pypi.org/project/zope.datetime/
-                :alt: Supported Python versions
-        
-        .. image:: https://github.com/zopefoundation/zope.datetime/workflows/tests/badge.svg
-                :target: https://github.com/zopefoundation/zope.datetime/actions?query=workflow%3Atests
-                :alt: CI status
-        
-        .. image:: https://coveralls.io/repos/github/zopefoundation/zope.datetime/badge.svg?branch=master
-                :target: https://coveralls.io/github/zopefoundation/zope.datetime?branch=master
-                :alt: Coverage
-        
-        .. image:: https://readthedocs.org/projects/zopedatetime/badge/?version=latest
-                :target: https://zopedatetime.readthedocs.io/en/latest/
-                :alt: Documentation Status
-        
-        Functions to parse and format date/time strings in common formats.
-        
-        Documentation is hosted at https://zopedatetime.readthedocs.io/
-        
-        
-        =========
-         CHANGES
-        =========
-        
-        4.3.0 (2021-02-26)
-        ==================
-        
-        - Drop support for Python 3.4.
-        
-        - Add support for Python 3.7, 3.8 and 3.9.
-        
-        - Prevent a ``DeprecationWarning`` in Python 3.8+ when using a parameter for
-          ``iso8601_date``, ``rfc850_date``, or ``rfc1123_date`` which has to be
-          converted via its ``__int__`` method.
-        
-        
-        4.2.0 (2017-08-14)
-        ==================
-        
-        - Remove support for guessing the timezone name when a timestamp
-          exceeds the value supported by Python's ``localtime`` function. On
-          platforms with a 32-bit ``time_t``, this would involve parsed values
-          that do not specify a timezone and are past the year 2038. Now the
-          underlying exception will be propagated. Previously an undocumented
-          heuristic was used. This is not expected to be a common issue;
-          Windows, as one example, always uses a 64-bit ``time_t``, even on
-          32-bit platforms. See
-          https://github.com/zopefoundation/zope.datetime/issues/4
-        
-        - Use true division on Python 2 to match Python 3, in case certain
-          parameters turn out to be integers instead of floating point values.
-          This is not expected to be user-visible, but it can arise in
-          artificial tests of internal functions.
-        
-        - Add support for Python 3.5 and 3.6.
-        
-        - Drop support for Python 2.6, 3.2 and 3.3.
-        
-        
-        4.1.0 (2014-12-26)
-        ==================
-        
-        - Add support for PyPy and PyPy3.
-        
-        - Add support for Python 3.4.
-        
-        - Add support for testing on Travis.
-        
-        
-        4.0.0 (2013-02-19)
-        ==================
-        
-        - Add support for Python 3.2 and 3.3.
-        
-        - Drop support for Python 2.4 and 2.5.
-        
-        
-        3.4.1 (2011-11-29)
-        ==================
-        
-        - Add test cases from LP #139360 (all passed without modification to
-          the ``parse`` function).
-        
-        - Remove unneeded ``zope.testing`` dependency.
-        
-        
-        3.4.0 (2007-07-20)
-        ==================
-        
-        - Initial release as a separate project.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE.txt
+
+===================
+ ``zope.datetime``
+===================
+
+.. image:: https://img.shields.io/pypi/v/zope.datetime.svg
+        :target: https://pypi.python.org/pypi/zope.datetime/
+        :alt: Latest release
+
+.. image:: https://img.shields.io/pypi/pyversions/zope.datetime.svg
+        :target: https://pypi.org/project/zope.datetime/
+        :alt: Supported Python versions
+
+.. image:: https://github.com/zopefoundation/zope.datetime/workflows/tests/badge.svg
+        :target: https://github.com/zopefoundation/zope.datetime/actions?query=workflow%3Atests
+        :alt: CI status
+
+.. image:: https://coveralls.io/repos/github/zopefoundation/zope.datetime/badge.svg?branch=master
+        :target: https://coveralls.io/github/zopefoundation/zope.datetime?branch=master
+        :alt: Coverage
+
+.. image:: https://readthedocs.org/projects/zopedatetime/badge/?version=latest
+        :target: https://zopedatetime.readthedocs.io/en/latest/
+        :alt: Documentation Status
+
+Functions to parse and format date/time strings in common formats.
+
+The documentation is hosted at https://zopedatetime.readthedocs.io/
+
+
+=========
+ CHANGES
+=========
+
+5.0.0 (2023-04-25)
+==================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.10, 3.11.
+
+
+4.3.0 (2021-02-26)
+==================
+
+- Drop support for Python 3.4.
+
+- Add support for Python 3.7, 3.8 and 3.9.
+
+- Prevent a ``DeprecationWarning`` in Python 3.8+ when using a parameter for
+  ``iso8601_date``, ``rfc850_date``, or ``rfc1123_date`` which has to be
+  converted via its ``__int__`` method.
+
+
+4.2.0 (2017-08-14)
+==================
+
+- Remove support for guessing the timezone name when a timestamp
+  exceeds the value supported by Python's ``localtime`` function. On
+  platforms with a 32-bit ``time_t``, this would involve parsed values
+  that do not specify a timezone and are past the year 2038. Now the
+  underlying exception will be propagated. Previously an undocumented
+  heuristic was used. This is not expected to be a common issue;
+  Windows, as one example, always uses a 64-bit ``time_t``, even on
+  32-bit platforms. See
+  https://github.com/zopefoundation/zope.datetime/issues/4
+
+- Use true division on Python 2 to match Python 3, in case certain
+  parameters turn out to be integers instead of floating point values.
+  This is not expected to be user-visible, but it can arise in
+  artificial tests of internal functions.
+
+- Add support for Python 3.5 and 3.6.
+
+- Drop support for Python 2.6, 3.2 and 3.3.
+
+
+4.1.0 (2014-12-26)
+==================
+
+- Add support for PyPy and PyPy3.
+
+- Add support for Python 3.4.
+
+- Add support for testing on Travis.
+
+
+4.0.0 (2013-02-19)
+==================
+
+- Add support for Python 3.2 and 3.3.
+
+- Drop support for Python 2.4 and 2.5.
+
+
+3.4.1 (2011-11-29)
+==================
+
+- Add test cases from LP #139360 (all passed without modification to
+  the ``parse`` function).
+
+- Remove unneeded ``zope.testing`` dependency.
+
+
+3.4.0 (2007-07-20)
+==================
+
+- Initial release as a separate project.
```

### Comparing `zope.datetime-4.3.0/README.rst` & `zope.datetime-5.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 .. image:: https://readthedocs.org/projects/zopedatetime/badge/?version=latest
         :target: https://zopedatetime.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 Functions to parse and format date/time strings in common formats.
 
-Documentation is hosted at https://zopedatetime.readthedocs.io/
+The documentation is hosted at https://zopedatetime.readthedocs.io/
```

### Comparing `zope.datetime-4.3.0/docs/Makefile` & `zope.datetime-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.datetime-4.3.0/docs/api.rst` & `zope.datetime-5.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.datetime-4.3.0/docs/conf.py` & `zope.datetime-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.datetime-4.3.0/setup.py` & `zope.datetime-5.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,62 +16,61 @@
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.datetime package
 """
 import os
 
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
 TESTS_REQUIRE = [
     'zope.testrunner',
 ]
 
 setup(name='zope.datetime',
-      version='4.3.0',
+      version='5.0.0',
       url='http://github.com/zopefoundation/zope.datetime',
       license='ZPL 2.1',
       description='Zope datetime',
       author='Zope Foundation and Contributors',
-      author_email='zope-dev@zope.org',
+      author_email='zope-dev@zope.dev',
       long_description=read('README.rst') + '\n\n' + read('CHANGES.rst'),
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
           'Topic :: Software Development',
       ],
       packages=find_packages('src'),
       package_dir={'': 'src'},
       test_suite='zope.datetime',
       namespace_packages=['zope', ],
       install_requires=[
           'setuptools',
-          'six',
       ],
+      python_requires='>=3.7',
       tests_require=TESTS_REQUIRE,
       extras_require={
           'test': TESTS_REQUIRE,
           'docs': [
               'Sphinx',
               'sphinx_rtd_theme',
           ],
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/__init__.py` & `zope.datetime-5.0.0/src/zope/datetime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Commonly used utility functions.
 
 Encapsulation of date/time values
 """
-from __future__ import division
 
 import math
 import re
 # there is a method definition that makes just "time"
 # problematic while executing a class definition
 import time as _time
-from time import tzname
-
 from datetime import datetime as _datetime
-from datetime import tzinfo as _std_tzinfo, timedelta as _timedelta
-
+from datetime import timedelta as _timedelta
+from datetime import tzinfo as _std_tzinfo
+from time import tzname
 
 from zope.datetime.timezones import historical_zone_info as _data
 
 
 if str is bytes:  # PY2
     StringTypes = (basestring,)  # noqa: F821 undefined name pragma: PY2
 else:
@@ -164,15 +162,15 @@
 
 EPOCH = _calc_epoch()
 jd1901 = 2415385
 
 numericTimeZoneMatch = re.compile(r'[+-][0-9][0-9][0-9][0-9]').match  # TS
 
 
-class _timezone(object):
+class _timezone:
 
     def __init__(self, data):
         self.name, self.timect, self.typect, \
             ttrans, self.tindex, self.tinfo, self.az = data
         self.ttrans = [int(tt) for tt in ttrans]
 
     def default_index(self):
@@ -209,15 +207,15 @@
 
     def info(self, t=None):
         idx = self.index(t)[0]
         zs = self.az[self.tinfo[idx][2]:]
         return self.tinfo[idx][0], self.tinfo[idx][1], zs[: zs.find('\000')]
 
 
-class _cache(object):
+class _cache:
 
     _zlst = [
         'Brazil/Acre', 'Brazil/DeNoronha', 'Brazil/East',
         'Brazil/West', 'Canada/Atlantic', 'Canada/Central',
         'Canada/Eastern', 'Canada/East-Saskatchewan',
         'Canada/Mountain', 'Canada/Newfoundland',
         'Canada/Pacific', 'Canada/Yukon',
@@ -516,15 +514,15 @@
     try:
         return _time.localtime(t)
     except (ValueError, OverflowError):  # Py2/Py3 respectively
         raise TimeError('The time %r is beyond the range '
                         'of this Python implementation.' % t)
 
 
-class DateTimeParser(object):
+class DateTimeParser:
 
     def parse(self, arg, local=True):
         """
         Parse a string containing some sort of date-time data into a tuple.
 
         As a general rule, any date-time representation that is
         recognized and unambigous to a resident of North America is
@@ -782,15 +780,15 @@
             if ts_results:
                 s = ts_results.group(0)
 
                 ls = len(s)
                 i = i + ls
                 if (ls == 4 and d and d in '+-' and
                         (len(ints) + (not not month) >= 3)):
-                    tz = '%s%s' % (d, s)
+                    tz = '{}{}'.format(d, s)
                 else:
                     v = int(s)
                     ints.append(v)
                 continue
 
             ts_results = wordpat.match(string, i)
             if ts_results:
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_datetime.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # pylint:disable=protected-access
+import time
 import unittest
 
-import time
-import six
 from zope import datetime
 
 
 class TestCache(unittest.TestCase):
 
     def test_error(self):
-        with six.assertRaisesRegex(
-                self, datetime.DateTimeError, "Unrecognized timezone"):
+        with self.assertRaisesRegex(
+                datetime.DateTimeError, "Unrecognized timezone"):
             datetime._cache().__getitem__('foo')
 
 
 class TestFuncs(unittest.TestCase):
 
     def test_correctYear(self):
         self.assertEqual(2069, datetime._correctYear(69))
@@ -144,16 +143,16 @@
         # Have to mock the time() method here to get
         # the desired return value for TZ, I couldn't find
         # input that would get is there naturally
         def t(*args):
             return (2000, 1, 1, 0, 0, 0, '+FOO')
         dtp = self._makeOne()
         dtp.parse = t
-        with six.assertRaisesRegex(
-                self, datetime.DateTimeError, "Unknown time zone"):
+        with self.assertRaisesRegex(
+                datetime.DateTimeError, "Unknown time zone"):
             dtp.time("foo")
 
     def test_time_no_tz(self):
         # See test_time_bad_tz
         def t(*args):
             return (2000, 1, 1, 0, 0, 0, '')
         dtp = self._makeOne()
@@ -260,16 +259,16 @@
             self._call_parse("10 30 30 19:61")
 
         with self.assertRaises(datetime.SyntaxError):
             self._call_parse("10 30 30 20 20 20 20")
 
     def test_parse_iso_index_error(self):
         dtp = self._makeOne()
-        with six.assertRaisesRegex(
-                self, datetime.DateError, "Not an ISO 8601 compliant"):
+        with self.assertRaisesRegex(
+                datetime.DateError, "Not an ISO 8601 compliant"):
             dtp._parse_iso8601('')
 
     def test_parse_with_dot(self):
         result = self._call_parse("Jan.1.2000")
         self.assertEqual(result[:-1],
                          (2000, 1, 1, 0, 0, 0))
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_datetimeparse.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_datetimeparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test datetime parser
 """
 import unittest
-from time import gmtime
 from datetime import datetime
+from time import gmtime
 
-from zope.datetime import parse, time, DateTimeError
-from zope.datetime import parseDatetimetz, tzinfo
+from zope.datetime import DateTimeError
 from zope.datetime import _tzoffset
+from zope.datetime import parse
+from zope.datetime import parseDatetimetz
+from zope.datetime import time
+from zope.datetime import tzinfo
 
 
 class Test(unittest.TestCase):
 
     def testParse(self):
         self.assertEqual(parse('1999 12 31')[:6],
                          (1999, 12, 31, 0, 0, 0))
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_lp_139360.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_lp_139360.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 
+
 # The separator character:
 s = '-'
 
 # The sets of single digit days and months:
 D = [(d, repr(d)) for d in range(1, 10)]
 M = [(m, repr(m)) for m in range(1, 10)]
 
@@ -69,9 +70,9 @@
 
 # Hide the temporary from nose
 del _test
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(LP_139360),
+        unittest.defaultTestLoader.loadTestsFromTestCase(LP_139360),
     ))
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_standard_dates.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_standard_dates.py`

 * *Files identical despite different names*

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_timezones.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_timezones.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 import unittest
 
 
 class TestTimezones(unittest.TestCase):
 
     def test_dumpTimezoneInfo(self):
+        import io
+
         from zope.datetime.timezones import dumpTimezoneInfo
         from zope.datetime.timezones import historical_zone_info
 
-        import io
-
         output = io.StringIO() if bytes is not str else io.BytesIO()
 
         dumpTimezoneInfo(historical_zone_info, out=output)
 
         value = output.getvalue()
 
         self.assertTrue(value.endswith('\n}\n'))
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/tests/test_tzinfo.py` & `zope.datetime-5.0.0/src/zope/datetime/tests/test_tzinfo.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test for the 'tzinfo() function
 """
 
-import unittest
-import pickle
 import datetime
+import pickle
+import unittest
 
 from zope.datetime import tzinfo
 
 
 class Test(unittest.TestCase):
 
     def test(self):
```

### Comparing `zope.datetime-4.3.0/src/zope/datetime/timezones.py` & `zope.datetime-5.0.0/src/zope/datetime/timezones.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Historical timezone data, ported from Zope2's DateTime.DateTimeZone.
 """
-from __future__ import print_function
+
 
 historical_zone_info = {
     'Brazil/Acre': ('Brazil/Acre', 101, 2,
                     ['561970800', '571644000', '593420400', '603093600', '625561200',
                      '634543200', '656924400', '665992800', '688374000', '697442400',
                      '719823600', '729496800', '751273200', '760946400', '782722800',
                      '792396000', '814863600', '823845600', '846226800', '855295200',
@@ -1185,22 +1185,22 @@
         out = sys.stdout
 
     print("historical_zone_info = {", file=out)
 
     items = sorted(_data.items())
     for key, value in items:
         v1, v2, v3, ilist, bitmap, two_by_three, two_nullterm = value
-        print("'%s': ('%s', %s, %s," % (key, v1, v2, v3), file=out)
+        print("'{}': ('{}', {}, {},".format(key, v1, v2, v3), file=out)
         print("[", end='', file=out)
         while ilist:
             next_5, ilist = ilist[:5], ilist[5:]
             line = ", ".join(["'%s'" % x for x in next_5])
             print("%s," % line, file=out)
         print("], ", file=out)
         print("%s," % repr(bitmap), file=out)
-        print("%s, %s)," % (repr(two_by_three), repr(two_nullterm)), file=out)
+        print("{}, {}),".format(repr(two_by_three), repr(two_nullterm)), file=out)
 
     print("}", file=out)
 
 
 if __name__ == '__main__':
     dumpTimezoneInfo(historical_zone_info)
```

### Comparing `zope.datetime-4.3.0/src/zope.datetime.egg-info/PKG-INFO` & `zope.datetime-5.0.0/src/zope.datetime.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,136 @@
 Metadata-Version: 2.1
 Name: zope.datetime
-Version: 4.3.0
+Version: 5.0.0
 Summary: Zope datetime
 Home-page: http://github.com/zopefoundation/zope.datetime
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Description: ===================
-         ``zope.datetime``
-        ===================
-        
-        .. image:: https://img.shields.io/pypi/v/zope.datetime.svg
-                :target: https://pypi.python.org/pypi/zope.datetime/
-                :alt: Latest release
-        
-        .. image:: https://img.shields.io/pypi/pyversions/zope.datetime.svg
-                :target: https://pypi.org/project/zope.datetime/
-                :alt: Supported Python versions
-        
-        .. image:: https://github.com/zopefoundation/zope.datetime/workflows/tests/badge.svg
-                :target: https://github.com/zopefoundation/zope.datetime/actions?query=workflow%3Atests
-                :alt: CI status
-        
-        .. image:: https://coveralls.io/repos/github/zopefoundation/zope.datetime/badge.svg?branch=master
-                :target: https://coveralls.io/github/zopefoundation/zope.datetime?branch=master
-                :alt: Coverage
-        
-        .. image:: https://readthedocs.org/projects/zopedatetime/badge/?version=latest
-                :target: https://zopedatetime.readthedocs.io/en/latest/
-                :alt: Documentation Status
-        
-        Functions to parse and format date/time strings in common formats.
-        
-        Documentation is hosted at https://zopedatetime.readthedocs.io/
-        
-        
-        =========
-         CHANGES
-        =========
-        
-        4.3.0 (2021-02-26)
-        ==================
-        
-        - Drop support for Python 3.4.
-        
-        - Add support for Python 3.7, 3.8 and 3.9.
-        
-        - Prevent a ``DeprecationWarning`` in Python 3.8+ when using a parameter for
-          ``iso8601_date``, ``rfc850_date``, or ``rfc1123_date`` which has to be
-          converted via its ``__int__`` method.
-        
-        
-        4.2.0 (2017-08-14)
-        ==================
-        
-        - Remove support for guessing the timezone name when a timestamp
-          exceeds the value supported by Python's ``localtime`` function. On
-          platforms with a 32-bit ``time_t``, this would involve parsed values
-          that do not specify a timezone and are past the year 2038. Now the
-          underlying exception will be propagated. Previously an undocumented
-          heuristic was used. This is not expected to be a common issue;
-          Windows, as one example, always uses a 64-bit ``time_t``, even on
-          32-bit platforms. See
-          https://github.com/zopefoundation/zope.datetime/issues/4
-        
-        - Use true division on Python 2 to match Python 3, in case certain
-          parameters turn out to be integers instead of floating point values.
-          This is not expected to be user-visible, but it can arise in
-          artificial tests of internal functions.
-        
-        - Add support for Python 3.5 and 3.6.
-        
-        - Drop support for Python 2.6, 3.2 and 3.3.
-        
-        
-        4.1.0 (2014-12-26)
-        ==================
-        
-        - Add support for PyPy and PyPy3.
-        
-        - Add support for Python 3.4.
-        
-        - Add support for testing on Travis.
-        
-        
-        4.0.0 (2013-02-19)
-        ==================
-        
-        - Add support for Python 3.2 and 3.3.
-        
-        - Drop support for Python 2.4 and 2.5.
-        
-        
-        3.4.1 (2011-11-29)
-        ==================
-        
-        - Add test cases from LP #139360 (all passed without modification to
-          the ``parse`` function).
-        
-        - Remove unneeded ``zope.testing`` dependency.
-        
-        
-        3.4.0 (2007-07-20)
-        ==================
-        
-        - Initial release as a separate project.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE.txt
+
+===================
+ ``zope.datetime``
+===================
+
+.. image:: https://img.shields.io/pypi/v/zope.datetime.svg
+        :target: https://pypi.python.org/pypi/zope.datetime/
+        :alt: Latest release
+
+.. image:: https://img.shields.io/pypi/pyversions/zope.datetime.svg
+        :target: https://pypi.org/project/zope.datetime/
+        :alt: Supported Python versions
+
+.. image:: https://github.com/zopefoundation/zope.datetime/workflows/tests/badge.svg
+        :target: https://github.com/zopefoundation/zope.datetime/actions?query=workflow%3Atests
+        :alt: CI status
+
+.. image:: https://coveralls.io/repos/github/zopefoundation/zope.datetime/badge.svg?branch=master
+        :target: https://coveralls.io/github/zopefoundation/zope.datetime?branch=master
+        :alt: Coverage
+
+.. image:: https://readthedocs.org/projects/zopedatetime/badge/?version=latest
+        :target: https://zopedatetime.readthedocs.io/en/latest/
+        :alt: Documentation Status
+
+Functions to parse and format date/time strings in common formats.
+
+The documentation is hosted at https://zopedatetime.readthedocs.io/
+
+
+=========
+ CHANGES
+=========
+
+5.0.0 (2023-04-25)
+==================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.10, 3.11.
+
+
+4.3.0 (2021-02-26)
+==================
+
+- Drop support for Python 3.4.
+
+- Add support for Python 3.7, 3.8 and 3.9.
+
+- Prevent a ``DeprecationWarning`` in Python 3.8+ when using a parameter for
+  ``iso8601_date``, ``rfc850_date``, or ``rfc1123_date`` which has to be
+  converted via its ``__int__`` method.
+
+
+4.2.0 (2017-08-14)
+==================
+
+- Remove support for guessing the timezone name when a timestamp
+  exceeds the value supported by Python's ``localtime`` function. On
+  platforms with a 32-bit ``time_t``, this would involve parsed values
+  that do not specify a timezone and are past the year 2038. Now the
+  underlying exception will be propagated. Previously an undocumented
+  heuristic was used. This is not expected to be a common issue;
+  Windows, as one example, always uses a 64-bit ``time_t``, even on
+  32-bit platforms. See
+  https://github.com/zopefoundation/zope.datetime/issues/4
+
+- Use true division on Python 2 to match Python 3, in case certain
+  parameters turn out to be integers instead of floating point values.
+  This is not expected to be user-visible, but it can arise in
+  artificial tests of internal functions.
+
+- Add support for Python 3.5 and 3.6.
+
+- Drop support for Python 2.6, 3.2 and 3.3.
+
+
+4.1.0 (2014-12-26)
+==================
+
+- Add support for PyPy and PyPy3.
+
+- Add support for Python 3.4.
+
+- Add support for testing on Travis.
+
+
+4.0.0 (2013-02-19)
+==================
+
+- Add support for Python 3.2 and 3.3.
+
+- Drop support for Python 2.4 and 2.5.
+
+
+3.4.1 (2011-11-29)
+==================
+
+- Add test cases from LP #139360 (all passed without modification to
+  the ``parse`` function).
+
+- Remove unneeded ``zope.testing`` dependency.
+
+
+3.4.0 (2007-07-20)
+==================
+
+- Initial release as a separate project.
```

### Comparing `zope.datetime-4.3.0/src/zope.datetime.egg-info/SOURCES.txt` & `zope.datetime-5.0.0/src/zope.datetime.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 setup.cfg
 setup.py
```

