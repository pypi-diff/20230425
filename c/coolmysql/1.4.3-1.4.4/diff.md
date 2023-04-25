# Comparing `tmp/coolmysql-1.4.3.tar.gz` & `tmp/coolmysql-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.3.tar", last modified: Sat Apr 22 15:48:41 2023, max compression
+gzip compressed data, was "coolmysql-1.4.4.tar", last modified: Tue Apr 25 12:41:11 2023, max compression
```

## Comparing `coolmysql-1.4.3.tar` & `coolmysql-1.4.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.3/LICENSE
--rw-r--r--   0        0        0     4343 2023-04-16 20:01:06.306928 coolmysql-1.4.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.3/coolmysql.py
--rw-r--r--   0        0        0      566 2023-04-22 15:48:30.912926 coolmysql-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 coolmysql-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.4/LICENSE
+-rw-r--r--   0        0        0     4252 2023-04-24 17:37:44.639289 coolmysql-1.4.4/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.4/coolmysql.py
+-rw-r--r--   0        0        0      566 2023-04-25 12:38:10.810919 coolmysql-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 coolmysql-1.4.4/PKG-INFO
```

### Comparing `coolmysql-1.4.3/LICENSE` & `coolmysql-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.3/README.md` & `coolmysql-1.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc.md)
 
-[English tutorial](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc_en.md)
-
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
```

### Comparing `coolmysql-1.4.3/pyproject.toml` & `coolmysql-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.3"
+version = "1.4.4"
 description = "史上最优雅的 mysql ORM"
 dependencies = ["lccpy >=1.4.5"]
 keywords = ["coolmysql", "pymysql", "mysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `coolmysql-1.4.3/PKG-INFO` & `coolmysql-1.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.3
+Version: 1.4.4
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.5
@@ -16,16 +16,14 @@
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc.md)
 
-[English tutorial](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc_en.md)
-
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
```

