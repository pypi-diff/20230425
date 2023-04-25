# Comparing `tmp/ccdt-2.0.1.tar.gz` & `tmp/ccdt-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.1.tar", last modified: Tue Apr 25 09:58:05 2023, max compression
+gzip compressed data, was "ccdt-2.0.2.tar", last modified: Tue Apr 25 10:50:03 2023, max compression
```

## Comparing `ccdt-2.0.1.tar` & `ccdt-2.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.035232 ccdt-2.0.1/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-04-25 09:58:05.033238 ccdt-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:04.988384 ccdt-2.0.1/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.1/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.005312 ccdt-2.0.1/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.1/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.009302 ccdt-2.0.1/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.1/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.1/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.016283 ccdt-2.0.1/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.1/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7928 2023-04-20 07:09:49.000000 ccdt-2.0.1/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    59802 2023-04-25 06:24:11.000000 ccdt-2.0.1/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.018304 ccdt-2.0.1/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.1/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    10717 2023-04-25 08:57:24.000000 ccdt-2.0.1/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.026257 ccdt-2.0.1/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.1/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.1/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    10114 2023-04-25 08:58:44.000000 ccdt-2.0.1/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.1/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.031243 ccdt-2.0.1/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.1/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.1/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.1/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:58:05.001323 ccdt-2.0.1/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 09:58:04.000000 ccdt-2.0.1/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 09:58:05.035232 ccdt-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-04-25 09:57:41.000000 ccdt-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.253633 ccdt-2.0.2/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-04-25 10:50:03.252635 ccdt-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.200773 ccdt-2.0.2/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.2/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.219722 ccdt-2.0.2/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.2/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.223740 ccdt-2.0.2/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.2/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.2/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.230692 ccdt-2.0.2/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    59802 2023-04-25 06:24:11.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.233688 ccdt-2.0.2/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.2/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    10717 2023-04-25 08:57:24.000000 ccdt-2.0.2/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.242660 ccdt-2.0.2/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.2/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.2/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.2/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.2/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.249668 ccdt-2.0.2/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.2/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.2/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.2/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.214737 ccdt-2.0.2/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:50:03.254628 ccdt-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-04-25 10:49:25.000000 ccdt-2.0.2/setup.py
```

### Comparing `ccdt-2.0.1/LICENSE` & `ccdt-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/PKG-INFO` & `ccdt-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.1
+Version: 2.0.2
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.1/README.md` & `ccdt-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.2/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.2/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
                                                      data_info['labelme_file']).replace("\\", "/")
                             save_json(json_path, save_labelme_dir, index)  # 剪切
                         else:
                             json_path = os.path.join(save_labelme_dir, data_info['labelme_file']).replace("\\", "/")
                             save_json(json_path, data_info['labelme_info'], index)  # 拷贝即重写
                 else:  # 人工定义输出目录后，程序自动根据序号、按label标签名称重组目录，逻辑实现
                     if isinstance(index, int) and isinstance(custom_label, str):
-                        print(image_path)
                         custom_dir = '{:0>4d}'.format(index) + '_' + custom_label
                         rebuild_dir = os.path.join(data_info['output_dir'], custom_dir)
                         # 重构压缩包名称路径
                         # rebuild_zip = os.path.join(data_info['output_dir'], custom_dir + '.zip')
                         # 重构压缩文件绝对路径
                         # rebuild_zip_relative_filename = os.path.relpath(image_path, data_info['input_dir'])
                         # 重构压缩文件相对路径
```

### Comparing `ccdt-2.0.1/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.2/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/dataset/main.py` & `ccdt-2.0.2/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.2/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.0.2/ccdt/dataset/utils/labelme_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         针对封装好的压缩目录进行迭代写入压缩对象包中
         该算法可以跨平台解压
         :param zip_package:
         """
         print(f'开始压缩')
         for zip_key, zip_value in tqdm(zip_package.items()):
             # zip_value：压缩包名称路径
+            os.makedirs(os.path.dirname(zip_value), exist_ok=True)
             with zipfile.ZipFile(zip_value, 'w', zipfile.ZIP_DEFLATED, allowZip64=True) as zip:  # 创建一个压缩文件对象
                 for root, dirs, files in os.walk(zip_key):  # 递归遍历写入压缩文件到指定压缩文件对象中
                     for file in files:
                         file_path = os.path.join(root, file)
                         relative_path = os.path.join(os.path.basename(zip_key), os.path.relpath(file_path, zip_key))
                         # file_path：压缩文件绝对路径，relative_path：压缩文件相对路径，相对于压缩目录
                         zip.write(file_path, relative_path)
```

### Comparing `ccdt-2.0.1/ccdt/video_tool/split.py` & `ccdt-2.0.2/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt/video_tool/video_main.py` & `ccdt-2.0.2/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.2/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.1
+Version: 2.0.2
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.1/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.2/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.1/setup.py` & `ccdt-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.1',
+    version='2.0.2',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

