# Comparing `tmp/tortik-0.2.8.tar.gz` & `tmp/tortik-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tortik-0.2.8.tar", last modified: Wed Jan 20 12:29:07 2021, max compression
+gzip compressed data, was "dist/tortik-0.2.9.tar", last modified: Mon Oct  4 08:51:11 2021, max compression
```

## Comparing `tortik-0.2.8.tar` & `tortik-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/
--rw-r--r--   0 glibin     (503) staff       (20)     1778 2021-01-20 12:29:07.000000 tortik-0.2.8/PKG-INFO
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/tortik/
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/tortik/page/
--rw-r--r--   0 glibin     (503) staff       (20)    11901 2021-01-20 12:25:50.000000 tortik-0.2.8/tortik/page/__init__.py
--rw-r--r--   0 glibin     (503) staff       (20)      493 2021-01-20 12:26:27.000000 tortik-0.2.8/tortik/version.py
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/tortik/util/
--rw-r--r--   0 glibin     (503) staff       (20)     2234 2020-02-11 09:45:20.000000 tortik-0.2.8/tortik/util/async_group.py
--rw-r--r--   0 glibin     (503) staff       (20)     3287 2020-12-11 10:58:16.000000 tortik-0.2.8/tortik/util/__init__.py
--rw-r--r--   0 glibin     (503) staff       (20)     2406 2015-09-30 08:49:43.000000 tortik-0.2.8/tortik/util/dumper.py
--rw-r--r--   0 glibin     (503) staff       (20)     2696 2020-12-11 10:58:16.000000 tortik-0.2.8/tortik/util/url.py
--rw-r--r--   0 glibin     (503) staff       (20)      808 2016-11-18 09:53:35.000000 tortik-0.2.8/tortik/util/xml_etree.py
--rw-r--r--   0 glibin     (503) staff       (20)      900 2016-01-15 05:45:37.000000 tortik-0.2.8/tortik/util/parse.py
--rw-r--r--   0 glibin     (503) staff       (20)      114 2015-02-08 18:29:56.000000 tortik-0.2.8/tortik/__init__.py
--rw-r--r--   0 glibin     (503) staff       (20)     6803 2016-01-14 09:27:10.000000 tortik-0.2.8/tortik/logger.py
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/tortik/templates/
--rw-r--r--   0 glibin     (503) staff       (20)     1520 2015-09-22 06:52:57.000000 tortik-0.2.8/tortik/templates/dumper.html
--rw-r--r--   0 glibin     (503) staff       (20)    37472 2016-11-18 09:35:38.000000 tortik-0.2.8/tortik/templates/debug.html
--rw-r--r--   0 glibin     (503) staff       (20)     2231 2020-11-26 07:51:16.000000 tortik-0.2.8/setup.py
-drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-01-20 12:29:07.000000 tortik-0.2.8/tortik.egg-info/
--rw-r--r--   0 glibin     (503) staff       (20)     1778 2021-01-20 12:29:06.000000 tortik-0.2.8/tortik.egg-info/PKG-INFO
--rw-r--r--   0 glibin     (503) staff       (20)      451 2021-01-20 12:29:06.000000 tortik-0.2.8/tortik.egg-info/SOURCES.txt
--rw-r--r--   0 glibin     (503) staff       (20)       50 2021-01-20 12:29:06.000000 tortik-0.2.8/tortik.egg-info/requires.txt
--rw-r--r--   0 glibin     (503) staff       (20)        7 2021-01-20 12:29:06.000000 tortik-0.2.8/tortik.egg-info/top_level.txt
--rw-r--r--   0 glibin     (503) staff       (20)        1 2021-01-20 12:29:06.000000 tortik-0.2.8/tortik.egg-info/dependency_links.txt
--rw-r--r--   0 glibin     (503) staff       (20)       80 2021-01-20 12:29:07.000000 tortik-0.2.8/setup.cfg
--rw-r--r--   0 glibin     (503) staff       (20)      903 2016-01-15 05:56:09.000000 tortik-0.2.8/README.rst
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/
+-rw-r--r--   0 glibin     (503) staff       (20)     1778 2021-10-04 08:51:11.000000 tortik-0.2.9/PKG-INFO
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik/
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik/page/
+-rw-r--r--   0 glibin     (503) staff       (20)    11902 2021-10-04 08:35:11.000000 tortik-0.2.9/tortik/page/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)      493 2021-10-04 08:35:11.000000 tortik-0.2.9/tortik/version.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik/util/
+-rw-r--r--   0 glibin     (503) staff       (20)     2234 2020-02-11 09:45:20.000000 tortik-0.2.9/tortik/util/async_group.py
+-rw-r--r--   0 glibin     (503) staff       (20)     3287 2020-12-11 10:58:16.000000 tortik-0.2.9/tortik/util/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)     2406 2015-09-30 08:49:43.000000 tortik-0.2.9/tortik/util/dumper.py
+-rw-r--r--   0 glibin     (503) staff       (20)     2696 2020-12-11 10:58:16.000000 tortik-0.2.9/tortik/util/url.py
+-rw-r--r--   0 glibin     (503) staff       (20)      808 2016-11-18 09:53:35.000000 tortik-0.2.9/tortik/util/xml_etree.py
+-rw-r--r--   0 glibin     (503) staff       (20)      900 2016-01-15 05:45:37.000000 tortik-0.2.9/tortik/util/parse.py
+-rw-r--r--   0 glibin     (503) staff       (20)      114 2015-02-08 18:29:56.000000 tortik-0.2.9/tortik/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)     6801 2021-10-04 08:35:11.000000 tortik-0.2.9/tortik/logger.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik/templates/
+-rw-r--r--   0 glibin     (503) staff       (20)     1520 2015-09-22 06:52:57.000000 tortik-0.2.9/tortik/templates/dumper.html
+-rw-r--r--   0 glibin     (503) staff       (20)    37472 2016-11-18 09:35:38.000000 tortik-0.2.9/tortik/templates/debug.html
+-rw-r--r--   0 glibin     (503) staff       (20)     2231 2020-11-26 07:51:16.000000 tortik-0.2.9/setup.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/
+-rw-r--r--   0 glibin     (503) staff       (20)     1778 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/PKG-INFO
+-rw-r--r--   0 glibin     (503) staff       (20)      451 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/SOURCES.txt
+-rw-r--r--   0 glibin     (503) staff       (20)       50 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/requires.txt
+-rw-r--r--   0 glibin     (503) staff       (20)        7 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/top_level.txt
+-rw-r--r--   0 glibin     (503) staff       (20)        1 2021-10-04 08:51:11.000000 tortik-0.2.9/tortik.egg-info/dependency_links.txt
+-rw-r--r--   0 glibin     (503) staff       (20)       80 2021-10-04 08:51:11.000000 tortik-0.2.9/setup.cfg
+-rw-r--r--   0 glibin     (503) staff       (20)      903 2016-01-15 05:56:09.000000 tortik-0.2.9/README.rst
```

### Comparing `tortik-0.2.8/PKG-INFO` & `tortik-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: tortik
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tortik - python tornado framework
 Home-page: https://github.com/glibin/tortik
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
-Download-URL: https://github.com/glibin/tortik/tarball/0.2.8
+Download-URL: https://github.com/glibin/tortik/tarball/0.2.9
 Description: Tortik
         ==================
         
         Tortik is a frontend micro framework atop of Python Tornado making easier to develop SOA-based applications.
         
         .. image:: https://travis-ci.org/glibin/tortik.svg
             :target: https://travis-ci.org/glibin/tortik
```

### Comparing `tortik-0.2.8/tortik/page/__init__.py` & `tortik-0.2.9/tortik/page/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         self.responses = {}
         self.http_client = self.initialize_http_client()
 
         self.preprocessors = copy(self.preprocessors) if hasattr(self, 'preprocessors') else []
         self.postprocessors = copy(self.postprocessors) if hasattr(self, 'postprocessors') else []
 
-        self.log.info('Using http client: %s' % repr(self.http_client))
+        self.log.debug('Using http client: %s' % repr(self.http_client))
 
         self._extra_data = {}
 
     @tornado.gen.coroutine
     def prepare(self):
         if self.preprocessors:
             start_time = time.time()
```

### Comparing `tortik-0.2.8/tortik/util/async_group.py` & `tortik-0.2.9/tortik/util/async_group.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/util/__init__.py` & `tortik-0.2.9/tortik/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/util/dumper.py` & `tortik-0.2.9/tortik/util/dumper.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/util/url.py` & `tortik-0.2.9/tortik/util/url.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/util/xml_etree.py` & `tortik-0.2.9/tortik/util/xml_etree.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/util/parse.py` & `tortik-0.2.9/tortik/util/parse.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/logger.py` & `tortik-0.2.9/tortik/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     def add_metric(self, name, value):
         self.metrics[name] = value
 
     def stage_started(self, stage_name):
         if stage_name not in self.stages:
             self.stages[stage_name] = PageLogger.StageInfo(time.time())
         else:
-            self.warning('Stage {} already started'.format(stage_name))
+            self.debug('Stage {} already started'.format(stage_name))
             self.stages[stage_name].counter += 1
 
     def stage_complete(self, stage_name):
         if stage_name in self.stages:
             stage = self.stages[stage_name]
             stage.counter -= 1
             if stage.counter < 0:
```

### Comparing `tortik-0.2.8/tortik/templates/dumper.html` & `tortik-0.2.9/tortik/templates/dumper.html`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik/templates/debug.html` & `tortik-0.2.9/tortik/templates/debug.html`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/setup.py` & `tortik-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tortik-0.2.8/tortik.egg-info/PKG-INFO` & `tortik-0.2.9/tortik.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: tortik
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tortik - python tornado framework
 Home-page: https://github.com/glibin/tortik
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
-Download-URL: https://github.com/glibin/tortik/tarball/0.2.8
+Download-URL: https://github.com/glibin/tortik/tarball/0.2.9
 Description: Tortik
         ==================
         
         Tortik is a frontend micro framework atop of Python Tornado making easier to develop SOA-based applications.
         
         .. image:: https://travis-ci.org/glibin/tortik.svg
             :target: https://travis-ci.org/glibin/tortik
```

### Comparing `tortik-0.2.8/README.rst` & `tortik-0.2.9/README.rst`

 * *Files identical despite different names*

