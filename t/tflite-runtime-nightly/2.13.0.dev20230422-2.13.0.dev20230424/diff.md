# Comparing `tmp/tflite_runtime_nightly-2.13.0.dev20230422-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.13.0.dev20230424-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2385879 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Apr-23 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-23 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-23 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-23 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-23 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-23 04:53 tflite_runtime_nightly-2.13.0.dev20230422.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Apr-23 04:53 tflite_runtime_nightly-2.13.0.dev20230422.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-23 04:53 tflite_runtime_nightly-2.13.0.dev20230422.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Apr-23 04:53 tflite_runtime_nightly-2.13.0.dev20230422.dist-info/RECORD
-9 files, 6826017 bytes uncompressed, 2384333 bytes compressed:  65.1%
+Zip file size: 2385881 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Apr-25 04:51 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-25 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-25 04:51 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-25 04:51 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-25 04:51 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-25 04:53 tflite_runtime_nightly-2.13.0.dev20230424.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Apr-25 04:53 tflite_runtime_nightly-2.13.0.dev20230424.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-25 04:53 tflite_runtime_nightly-2.13.0.dev20230424.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Apr-25 04:53 tflite_runtime_nightly-2.13.0.dev20230424.dist-info/RECORD
+9 files, 6826017 bytes uncompressed, 2384335 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230422.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.13.0.dev20230424.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230422.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.13.0.dev20230424.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230422.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.13.0.dev20230424.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230422.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.13.0.dev20230424.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.13.0dev20230422'
-__git_version__ = '0.6.0-146890-gd3d6ef081e5'
+__version__ = '2.13.0dev20230424'
+__git_version__ = '0.6.0-146949-ge56048795b2'
```

## Comparing `tflite_runtime_nightly-2.13.0.dev20230422.dist-info/METADATA` & `tflite_runtime_nightly-2.13.0.dev20230424.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.13.0.dev20230422
+Version: 2.13.0.dev20230424
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

