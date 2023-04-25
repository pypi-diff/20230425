# Comparing `tmp/ats_case-0.6.4.tar.gz` & `tmp/ats_case-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.6.4.tar", last modified: Mon Apr 24 06:03:46 2023, max compression
+gzip compressed data, was "ats_case-0.6.5.tar", last modified: Mon Apr 24 09:44:21 2023, max compression
```

## Comparing `ats_case-0.6.4.tar` & `ats_case-0.6.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.484498 ats_case-0.6.4/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-24 06:03:46.479508 ats_case-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:45.985761 ats_case-0.6.4/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.4/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.226234 ats_case-0.6.4/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.4/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17451 2023-04-24 06:03:25.000000 ats_case-0.6.4/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.4/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.6.4/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5549 2023-04-24 01:14:40.000000 ats_case-0.6.4/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.308938 ats_case-0.6.4/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.4/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.4/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.6.4/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.395733 ats_case-0.6.4/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.4/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.6.4/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3489 2023-04-24 03:07:03.000000 ats_case-0.6.4/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.469534 ats_case-0.6.4/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.4/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.4/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-24 06:03:46.086781 ats_case-0.6.4/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-24 06:03:45.000000 ats_case-0.6.4/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-24 06:03:45.000000 ats_case-0.6.4/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:03:45.000000 ats_case-0.6.4/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-24 06:03:45.000000 ats_case-0.6.4/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 06:03:45.000000 ats_case-0.6.4/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 06:03:46.484498 ats_case-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-24 06:03:39.000000 ats_case-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.563728 ats_case-0.6.5/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-24 09:44:21.561733 ats_case-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.138538 ats_case-0.6.5/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.5/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.364639 ats_case-0.6.5/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.5/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17451 2023-04-24 06:03:25.000000 ats_case-0.6.5/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.5/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.6.5/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5549 2023-04-24 01:14:40.000000 ats_case-0.6.5/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.430084 ats_case-0.6.5/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.5/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.5/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.6.5/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.506879 ats_case-0.6.5/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.5/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-04-24 09:43:48.000000 ats_case-0.6.5/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3489 2023-04-24 03:07:03.000000 ats_case-0.6.5/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.551760 ats_case-0.6.5/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.5/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.5/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-24 09:44:21.244303 ats_case-0.6.5/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-24 09:44:20.000000 ats_case-0.6.5/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-24 09:44:20.000000 ats_case-0.6.5/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:44:20.000000 ats_case-0.6.5/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-24 09:44:20.000000 ats_case-0.6.5/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 09:44:20.000000 ats_case-0.6.5/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:44:21.564724 ats_case-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-24 09:44:15.000000 ats_case-0.6.5/setup.py
```

### Comparing `ats_case-0.6.4/PKG-INFO` & `ats_case-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.6.4
+Version: 0.6.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.4/README.md` & `ats_case-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/case/command.py` & `ats_case-0.6.5/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/case/context.py` & `ats_case-0.6.5/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/case/executor.py` & `ats_case-0.6.5/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/case/translator.py` & `ats_case-0.6.5/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/common/error.py` & `ats_case-0.6.5/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/manage/core.py` & `ats_case-0.6.5/ats_case/manage/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def start(data):
     """
     启动测试进程
     :param data:
     :return:
     """
     # 判断测试终端是否可以连接
-    p = Process(target=run, kwargs=data)
+    p = Process(target=run, kwargs=data, daemon=True)
     p.start()
 
     logger.info('TEST PROCESS[{}] START - DATA: {}...'.format(p.pid, data))
     return p.pid
 
 
 def suspend(data):
```

### Comparing `ats_case-0.6.4/ats_case/manage/start.py` & `ats_case-0.6.5/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case/template/testcase_v1.tmp` & `ats_case-0.6.5/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/ats_case.egg-info/PKG-INFO` & `ats_case-0.6.5/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.6.4
+Version: 0.6.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.4/ats_case.egg-info/SOURCES.txt` & `ats_case-0.6.5/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.4/setup.py` & `ats_case-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.6.4",
+    version="0.6.5",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

