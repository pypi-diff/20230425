# Comparing `tmp/coolmongo-1.3.tar.gz` & `tmp/coolmongo-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.tar", last modified: Mon Apr 10 14:25:12 2023, max compression
+gzip compressed data, was "coolmongo-1.3.1.tar", last modified: Tue Apr 25 12:40:53 2023, max compression
```

## Comparing `coolmongo-1.3.tar` & `coolmongo-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3/LICENSE
--rw-r--r--   0        0        0     5124 2023-04-09 11:28:09.647580 coolmongo-1.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3/coolmongo.py
--rw-r--r--   0        0        0      566 2023-04-10 09:20:09.279348 coolmongo-1.3/pyproject.toml
--rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 coolmongo-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5025 2023-04-24 17:37:54.832465 coolmongo-1.3.1/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.1/coolmongo.py
+-rw-r--r--   0        0        0      570 2023-04-25 12:38:48.061938 coolmongo-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 coolmongo-1.3.1/PKG-INFO
```

### Comparing `coolmongo-1.3/LICENSE` & `coolmongo-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3/README.md` & `coolmongo-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc.md)
 
-[English tutorial](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc_en.md)
-
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
@@ -35,15 +33,15 @@
 ```
 
 创建ORM：
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
-orm = mg.ORM(mkconn=mkconn)  # 账户ORM
+orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['city']  # 库ORM
 sheet = db['school']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -111,25 +109,25 @@
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
 过滤器的集合运算：
 
-| 代码                                                                  | 解释 |
-| --------------------------------------------------------------------- | ---- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                          | 交集 |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集 |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                       | 差集 |
-| [ ~(mc.年龄>100) ]                                                    | 补集 |
+| 代码                                                                   | 解释 |
+| ---------------------------------------------------------------------- | ---- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集 |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集 |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集 |
+| [ ~(mc.年龄>100) ]                                                     | 补集 |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 特殊操作：
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
```

### Comparing `coolmongo-1.3/pyproject.toml` & `coolmongo-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.3"
+version = "1.3.1"
 description = "史上最优雅的 MongoDB ORM"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.4.5"]
 keywords = ["coolmongo", "pymongo", "mongodb"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmongo-1.3/PKG-INFO` & `coolmongo-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3
+Version: 1.3.1
 Summary: 史上最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4.5
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmongo
 
 # 项目描述
 
 史上最优雅的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc.md)
 
-[English tutorial](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc_en.md)
-
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
@@ -47,15 +45,15 @@
 ```
 
 创建ORM：
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
-orm = mg.ORM(mkconn=mkconn)  # 账户ORM
+orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['city']  # 库ORM
 sheet = db['school']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -123,25 +121,25 @@
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
 过滤器的集合运算：
 
-| 代码                                                                  | 解释 |
-| --------------------------------------------------------------------- | ---- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                          | 交集 |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集 |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                       | 差集 |
-| [ ~(mc.年龄>100) ]                                                    | 补集 |
+| 代码                                                                   | 解释 |
+| ---------------------------------------------------------------------- | ---- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集 |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集 |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集 |
+| [ ~(mc.年龄>100) ]                                                     | 补集 |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 特殊操作：
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
```

