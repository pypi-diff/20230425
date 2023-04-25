# Comparing `tmp/sharedmap-1.0.2.tar.gz` & `tmp/sharedmap-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedmap-1.0.2.tar", last modified: Fri Apr 21 08:03:56 2023, max compression
+gzip compressed data, was "sharedmap-1.0.4.tar", last modified: Tue Apr 25 09:22:56 2023, max compression
```

## Comparing `sharedmap-1.0.2.tar` & `sharedmap-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.2/LICENSE
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 08:03:56.920754 sharedmap-1.0.2/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3853 2023-04-21 07:04:13.000000 sharedmap-1.0.2/README.md
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/native/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.2/native/avltree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.2/native/avltree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1551 2023-04-21 03:58:52.000000 sharedmap-1.0.2/native/pynative.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      288 2023-04-20 09:22:52.000000 sharedmap-1.0.2/native/pynative.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7178 2023-04-21 04:09:15.000000 sharedmap-1.0.2/native/pyrbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4340 2023-04-21 03:37:21.000000 sharedmap-1.0.2/native/pyshareabledict.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3441 2023-04-20 13:10:17.000000 sharedmap-1.0.2/native/pytree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.2/native/rbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.2/native/rbtree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.2/native/stringbox.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.2/native/stringbox.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.2/native/tree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.2/native/tree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-04-21 08:03:56.920754 sharedmap-1.0.2/setup.cfg
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1888 2023-04-21 08:03:51.000000 sharedmap-1.0.2/setup.py
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/sharedmap.egg-info/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      399 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/SOURCES.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/dependency_links.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/top_level.txt
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.4/LICENSE
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-04-25 09:22:56.691034 sharedmap-1.0.4/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3934 2023-04-25 09:14:13.000000 sharedmap-1.0.4/README.md
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/native/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.4/native/avltree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.4/native/avltree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1551 2023-04-21 03:58:52.000000 sharedmap-1.0.4/native/pynative.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      354 2023-04-25 08:55:57.000000 sharedmap-1.0.4/native/pynative.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7178 2023-04-25 09:10:45.000000 sharedmap-1.0.4/native/pyrbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4336 2023-04-25 09:10:35.000000 sharedmap-1.0.4/native/pyshareabledict.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3441 2023-04-20 13:10:17.000000 sharedmap-1.0.4/native/pytree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.4/native/rbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.4/native/rbtree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.4/native/stringbox.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.4/native/stringbox.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.4/native/tree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.4/native/tree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-04-25 09:22:56.691034 sharedmap-1.0.4/setup.cfg
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1698 2023-04-25 09:22:42.000000 sharedmap-1.0.4/setup.py
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/sharedmap.egg-info/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      399 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/top_level.txt
```

### Comparing `sharedmap-1.0.2/LICENSE` & `sharedmap-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/PKG-INFO` & `sharedmap-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.2
+Version: 1.0.4
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
@@ -13,36 +13,44 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# 安装
+补充上传到pypi了，传的sdist，所以也支持python2。
+```
+pip3 install sharedmap
+```
+
+
+
 # 示例
 ```
 import sharedmap
 
 def t1():
 	wmap = sharedmap.rbtree();
 	wmap.set("aaa","323");
 	wmap.set("zb","1233");
 	wmap.set("tes","32z");
 	wmap.set("红","32是");
-	print(wmap.get("tes").decode("utf8"));
+	print(wmap.get("tes"));
 	wmap.share("test:3325",force=True);
 
 
 print("测试写入");
 t1();
 
 
 
 def t2():
 	rmap = sharedmap.sharedmap("test:3325");
-	print(rmap.get("红").decode("utf8"));
+	print(rmap.get("红"));
 
 print("测试读取");
 t2();
 ```
 
 # 工具类
 ## rbtree
@@ -59,15 +67,15 @@
 该方法失败的时候会抛出异常。
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 ### ```share```
 
 把字典当前状态制作成一个快照(基于索引的内存池和avl树)保存到共享内存中，这个快照可以通过```sharedmap```读取。
 
 | 参数 | 类型 | 说明 |
@@ -90,15 +98,15 @@
 ### ```remove```
 
 这是一个静态方法，用户删除由```share```方法构造的共享内存```sharedmap```，删除操作不要求和写入操作在同一个进程中。删除后，已经获取的```sharedmap```依然有效，无法通过该名字获得```sharedmap```对象。删除后可以通过```share```方法建立新的```sharedmap```。更多细节和清理内存的时机参考共享内存的原理。
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | name | str | 共享字典的名字，sharedmap在初始化的时候会用到 |
-| 返回值 | bytes | 成功True |
+| 返回值 | bool | 成功True |
 
 
 ## sharedmap
 
 
 ### ```__init__```
 通过给定的名字获得一个共享内存字典，该字典数据必须是由上面的```rbtree```对象通过```share```方法写入的。
@@ -110,15 +118,15 @@
 
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 # 实现原理
 avl树是完美平衡树，在内存中可以用连续的内存块表示，同时avl树的读取操作并不需要在其内存结构中写入任何辅助的信息。avl树的插入操作成本非常高（用给定的有序定长数组构造avl树很快），但读取速度非常快。红黑树插入方便。
 
 共享内存中的数据修改需要在多个不同的进程中用锁来控制，是比较困难的，所以本文的方案是禁用了共享字典的持续写入能力。用红黑树初始化一个字典，然后制作成avl树快照供后续读取。一个共享内存字典的生命周期内，只允许一次性的写入操作，因此具有极好的无锁并发读取特性。
```

### Comparing `sharedmap-1.0.2/README.md` & `sharedmap-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,37 @@
+# 安装
+补充上传到pypi了，传的sdist，所以也支持python2。
+```
+pip3 install sharedmap
+```
+
+
+
 # 示例
 ```
 import sharedmap
 
 def t1():
 	wmap = sharedmap.rbtree();
 	wmap.set("aaa","323");
 	wmap.set("zb","1233");
 	wmap.set("tes","32z");
 	wmap.set("红","32是");
-	print(wmap.get("tes").decode("utf8"));
+	print(wmap.get("tes"));
 	wmap.share("test:3325",force=True);
 
 
 print("测试写入");
 t1();
 
 
 
 def t2():
 	rmap = sharedmap.sharedmap("test:3325");
-	print(rmap.get("红").decode("utf8"));
+	print(rmap.get("红"));
 
 print("测试读取");
 t2();
 ```
 
 # 工具类
 ## rbtree
@@ -40,15 +48,15 @@
 该方法失败的时候会抛出异常。
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 ### ```share```
 
 把字典当前状态制作成一个快照(基于索引的内存池和avl树)保存到共享内存中，这个快照可以通过```sharedmap```读取。
 
 | 参数 | 类型 | 说明 |
@@ -71,15 +79,15 @@
 ### ```remove```
 
 这是一个静态方法，用户删除由```share```方法构造的共享内存```sharedmap```，删除操作不要求和写入操作在同一个进程中。删除后，已经获取的```sharedmap```依然有效，无法通过该名字获得```sharedmap```对象。删除后可以通过```share```方法建立新的```sharedmap```。更多细节和清理内存的时机参考共享内存的原理。
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | name | str | 共享字典的名字，sharedmap在初始化的时候会用到 |
-| 返回值 | bytes | 成功True |
+| 返回值 | bool | 成功True |
 
 
 ## sharedmap
 
 
 ### ```__init__```
 通过给定的名字获得一个共享内存字典，该字典数据必须是由上面的```rbtree```对象通过```share```方法写入的。
@@ -91,15 +99,15 @@
 
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 # 实现原理
 avl树是完美平衡树，在内存中可以用连续的内存块表示，同时avl树的读取操作并不需要在其内存结构中写入任何辅助的信息。avl树的插入操作成本非常高（用给定的有序定长数组构造avl树很快），但读取速度非常快。红黑树插入方便。
 
 共享内存中的数据修改需要在多个不同的进程中用锁来控制，是比较困难的，所以本文的方案是禁用了共享字典的持续写入能力。用红黑树初始化一个字典，然后制作成avl树快照供后续读取。一个共享内存字典的生命周期内，只允许一次性的写入操作，因此具有极好的无锁并发读取特性。
```

### Comparing `sharedmap-1.0.2/native/avltree.cpp` & `sharedmap-1.0.4/native/avltree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/avltree.h` & `sharedmap-1.0.4/native/avltree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/pynative.cpp` & `sharedmap-1.0.4/native/pynative.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/pyrbtree.cpp` & `sharedmap-1.0.4/native/pyrbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/pyshareabledict.cpp` & `sharedmap-1.0.4/native/pyshareabledict.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 	0, /* tp_hash */
 	0, /* tp_call */
 	0, /* tp_str */
 	0, /* tp_getattro */
 	0, /* tp_setattro */
 	0, /* tp_as_buffer */
 	Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE, /* tp_flags */
-	"shareabledict desc", /* tp_doc */
+	"sharedmap desc", /* tp_doc */
 	0, /* tp_traverse */
 	0, /* tp_clear */
 	0, /* tp_richcompare */
 	0, /* tp_weaklistoffset */
 	0, /* tp_iter */
 	0, /* tp_iternext */
 	pyshareabledictObjectClassMethods, /* tp_methods */
```

### Comparing `sharedmap-1.0.2/native/pytree.h` & `sharedmap-1.0.4/native/pytree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/rbtree.cpp` & `sharedmap-1.0.4/native/rbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/rbtree.h` & `sharedmap-1.0.4/native/rbtree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/stringbox.cpp` & `sharedmap-1.0.4/native/stringbox.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/stringbox.h` & `sharedmap-1.0.4/native/stringbox.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/tree.cpp` & `sharedmap-1.0.4/native/tree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/native/tree.h` & `sharedmap-1.0.4/native/tree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.2/setup.py` & `sharedmap-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	with open("README.md", "r") as fh:
 		long_description = fh.read()
 except Exception as e:
 	long_description = "";
 
 
 setup (name = projname,
-	version = '1.0.2',
+	version = '1.0.4',
 	description = projname,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "lyramilk",
 	packages=[],
 	ext_modules = [module1],
 	data_files=include_files,
@@ -61,19 +61,7 @@
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Topic :: Utilities'
 	],
 	keywords = 'sharedmap,sharememory,rbtree,avltree',
 )
 
-
-'''
-
-	"native/stringbox.cpp",
-	"native/tree.cpp",
-	"native/avltree.cpp",
-	"native/rbtree.cpp",
-	"native/pyshareabledict.cpp",
-	"native/pyrbtree.cpp",
-	"native/pynative.cpp",
-
-'''
```

### Comparing `sharedmap-1.0.2/sharedmap.egg-info/PKG-INFO` & `sharedmap-1.0.4/sharedmap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.2
+Version: 1.0.4
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
@@ -13,36 +13,44 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# 安装
+补充上传到pypi了，传的sdist，所以也支持python2。
+```
+pip3 install sharedmap
+```
+
+
+
 # 示例
 ```
 import sharedmap
 
 def t1():
 	wmap = sharedmap.rbtree();
 	wmap.set("aaa","323");
 	wmap.set("zb","1233");
 	wmap.set("tes","32z");
 	wmap.set("红","32是");
-	print(wmap.get("tes").decode("utf8"));
+	print(wmap.get("tes"));
 	wmap.share("test:3325",force=True);
 
 
 print("测试写入");
 t1();
 
 
 
 def t2():
 	rmap = sharedmap.sharedmap("test:3325");
-	print(rmap.get("红").decode("utf8"));
+	print(rmap.get("红"));
 
 print("测试读取");
 t2();
 ```
 
 # 工具类
 ## rbtree
@@ -59,15 +67,15 @@
 该方法失败的时候会抛出异常。
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 ### ```share```
 
 把字典当前状态制作成一个快照(基于索引的内存池和avl树)保存到共享内存中，这个快照可以通过```sharedmap```读取。
 
 | 参数 | 类型 | 说明 |
@@ -90,15 +98,15 @@
 ### ```remove```
 
 这是一个静态方法，用户删除由```share```方法构造的共享内存```sharedmap```，删除操作不要求和写入操作在同一个进程中。删除后，已经获取的```sharedmap```依然有效，无法通过该名字获得```sharedmap```对象。删除后可以通过```share```方法建立新的```sharedmap```。更多细节和清理内存的时机参考共享内存的原理。
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | name | str | 共享字典的名字，sharedmap在初始化的时候会用到 |
-| 返回值 | bytes | 成功True |
+| 返回值 | bool | 成功True |
 
 
 ## sharedmap
 
 
 ### ```__init__```
 通过给定的名字获得一个共享内存字典，该字典数据必须是由上面的```rbtree```对象通过```share```方法写入的。
@@ -110,15 +118,15 @@
 
 
 ### ```get```
 
 | 参数 | 类型 | 说明 |
 | - | - | - |
 | key | str |  |
-| 返回值 | bytes |  |
+| 返回值 | str |  |
 
 
 # 实现原理
 avl树是完美平衡树，在内存中可以用连续的内存块表示，同时avl树的读取操作并不需要在其内存结构中写入任何辅助的信息。avl树的插入操作成本非常高（用给定的有序定长数组构造avl树很快），但读取速度非常快。红黑树插入方便。
 
 共享内存中的数据修改需要在多个不同的进程中用锁来控制，是比较困难的，所以本文的方案是禁用了共享字典的持续写入能力。用红黑树初始化一个字典，然后制作成avl树快照供后续读取。一个共享内存字典的生命周期内，只允许一次性的写入操作，因此具有极好的无锁并发读取特性。
```

