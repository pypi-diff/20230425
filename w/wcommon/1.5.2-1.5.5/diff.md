# Comparing `tmp/wcommon-1.5.2.tar.gz` & `tmp/wcommon-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.5.2.tar", last modified: Thu Apr 20 05:56:04 2023, max compression
+gzip compressed data, was "wcommon-1.5.5.tar", last modified: Tue Apr 25 09:31:20 2023, max compression
```

## Comparing `wcommon-1.5.2.tar` & `wcommon-1.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:56:04.516014 wcommon-1.5.2/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-20 05:56:04.515727 wcommon-1.5.2/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.2/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-04-20 05:56:04.516144 wcommon-1.5.2/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-04-20 05:55:53.000000 wcommon-1.5.2/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:56:04.512653 wcommon-1.5.2/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    24001 2023-04-20 05:55:20.000000 wcommon-1.5.2/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:56:04.515242 wcommon-1.5.2/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-20 05:56:04.000000 wcommon-1.5.2/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-04-20 05:56:04.000000 wcommon-1.5.2/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-04-20 05:56:04.000000 wcommon-1.5.2/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-04-20 05:56:04.000000 wcommon-1.5.2/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-04-20 05:56:04.000000 wcommon-1.5.2/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.076849 wcommon-1.5.5/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-25 09:31:20.076590 wcommon-1.5.5/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.5/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-04-25 09:31:20.076955 wcommon-1.5.5/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-04-25 09:31:05.000000 wcommon-1.5.5/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.073238 wcommon-1.5.5/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    24477 2023-04-25 09:22:06.000000 wcommon-1.5.5/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.076191 wcommon-1.5.5/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.5.2/PKG-INFO` & `wcommon-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.2
+Version: 1.5.5
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wcommon-1.5.2/README.md` & `wcommon-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `wcommon-1.5.2/setup.py` & `wcommon-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.5.2",
+    version="1.5.5",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.5.2/wcommon/__init__.py` & `wcommon-1.5.5/wcommon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,16 @@
 def query(database, sql, argumentTuple=(), timestamp2str=True):
     import pymysql
     cursor = database.cursor()
     logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
+        if type(argumentTuple) == list:
+            argumentTuple = tuple(argumentTuple)
         cursor.execute(sql, argumentTuple)
     rows = []
 
     if timestamp2str:
         timestamp_field_array = []
         date_field_array = []
         for tp in cursor.description:
@@ -288,14 +290,16 @@
 
 def execute(database, sql, argumentTuple=()):
     cursor = database.cursor()
     logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
+        if type(argumentTuple) == list:
+            argumentTuple = tuple(argumentTuple)
         cursor.execute(sql, argumentTuple)
 
 
 def delete(database, sql, commit=True):
     cursor = database.cursor()
     logger.debug("delete sql:\t" + sql)
     if commit:
@@ -304,15 +308,17 @@
 
 
 def mysql_execute(database, sql, argumentTuple, commit=True):
     cursor = database.cursor()
     if argumentTuple:
         cursor.execute(sql, argumentTuple)
     else:
-        cursor.execute(sql)
+        if type(argumentTuple) == list:
+            argumentTuple = tuple(argumentTuple)
+        cursor.execute(sql, argumentTuple)
     if commit:
         database.commit()
 
 
 # 获取文件的创建时间
 def getFileCreateTime(filePath):
     # filePath = unicode(filePath,'utf8')
@@ -581,14 +587,16 @@
     @pingmysql
     def query(self, sql, argumentTuple=(), timestamp2str=True):
         cursor = self.database.cursor()
         logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
         if len(argumentTuple) == 0:
             cursor.execute(sql)
         else:
+            if type(argumentTuple) == list:
+                argumentTuple = tuple(argumentTuple)
             cursor.execute(sql, argumentTuple)
         rows = []
 
         if timestamp2str:
             timestamp_field_array = []
             date_field_array = []
             for tp in cursor.description:
@@ -676,14 +684,16 @@
     @pingmysql
     def execute(self, sql, argumentTuple=(), commit=True):
         cursor = self.database.cursor()
         logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
         if len(argumentTuple) == 0:
             cursor.execute(sql)
         else:
+            if type(argumentTuple) == list:
+                argumentTuple = tuple(argumentTuple)
             cursor.execute(sql, argumentTuple)
         if commit:
             self.database.commit()
 
     @pingmysql
     def delete(self, sql, commit=True):
         cursor = self.database.cursor()
```

### Comparing `wcommon-1.5.2/wcommon.egg-info/PKG-INFO` & `wcommon-1.5.5/wcommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.2
+Version: 1.5.5
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

