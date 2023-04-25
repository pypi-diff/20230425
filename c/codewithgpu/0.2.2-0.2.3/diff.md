# Comparing `tmp/codewithgpu-0.2.2-py3-none-any.whl.zip` & `tmp/codewithgpu-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 35550 bytes, number of entries: 29
--rw-r--r--  2.0 unx     1549 b- defN 23-Apr-25 08:58 codewithgpu/__init__.py
+Zip file size: 35495 bytes, number of entries: 29
+-rw-r--r--  2.0 unx     1448 b- defN 23-Apr-25 09:01 codewithgpu/__init__.py
 -rw-r--r--  2.0 unx     1924 b- defN 23-Apr-23 11:05 codewithgpu/cli.py
--rw-r--r--  2.0 unx      185 b- defN 23-Apr-25 08:58 codewithgpu/version.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Apr-25 09:01 codewithgpu/version.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/data/__init__.py
 -rw-r--r--  2.0 unx     6547 b- defN 23-Apr-23 11:05 codewithgpu/data/dataset.py
 -rw-r--r--  2.0 unx     7177 b- defN 23-Apr-23 11:05 codewithgpu/data/reader.py
 -rw-r--r--  2.0 unx      608 b- defN 23-Apr-23 11:05 codewithgpu/data/record.proto
 -rw-r--r--  2.0 unx     8941 b- defN 23-Apr-23 11:05 codewithgpu/data/record.py
 -rw-r--r--  2.0 unx    10202 b- defN 23-Apr-23 11:05 codewithgpu/data/record_pb2.py
 -rw-r--r--  2.0 unx      780 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record.proto
@@ -18,14 +18,14 @@
 -rw-r--r--  2.0 unx     1418 b- defN 23-Apr-23 11:05 codewithgpu/model/download.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/utils/__init__.py
 -rw-r--r--  2.0 unx     4076 b- defN 23-Apr-23 11:05 codewithgpu/utils/cg_cli.py
 -rw-r--r--  2.0 unx     3805 b- defN 23-Apr-23 11:05 codewithgpu/utils/decorator.py
 -rw-r--r--  2.0 unx     3629 b- defN 23-Apr-23 11:05 codewithgpu/utils/deprecation.py
 -rw-r--r--  2.0 unx     3741 b- defN 23-Apr-21 09:27 codewithgpu/utils/logging.py
 -rw-r--r--  2.0 unx     1226 b- defN 23-Apr-21 09:27 codewithgpu/utils/unittest_util.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3033 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2469 b- defN 23-Apr-25 08:58 codewithgpu-0.2.2.dist-info/RECORD
-29 files, 102695 bytes uncompressed, 31564 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3033 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2469 b- defN 23-Apr-25 09:01 codewithgpu-0.2.3.dist-info/RECORD
+29 files, 102594 bytes uncompressed, 31509 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -63,26 +63,26 @@
 
 Filename: codewithgpu/utils/logging.py
 Comment: 
 
 Filename: codewithgpu/utils/unittest_util.py
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/LICENSE
+Filename: codewithgpu-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/METADATA
+Filename: codewithgpu-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/WHEEL
+Filename: codewithgpu-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/entry_points.txt
+Filename: codewithgpu-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/top_level.txt
+Filename: codewithgpu-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: codewithgpu-0.2.2.dist-info/RECORD
+Filename: codewithgpu-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## codewithgpu/__init__.py

```diff
@@ -24,14 +24,10 @@
 from codewithgpu.data.dataset import TFRecordDataset
 from codewithgpu.data.reader import DatasetReader
 from codewithgpu.data.record import RecordWriter
 from codewithgpu.data.tf_record import TFRecordWriter
 from codewithgpu.inference.command import InferenceCommand
 from codewithgpu.inference.command import ServingCommand
 from codewithgpu.inference.module import InferenceModule
-from codewithgpu import model
 
 # Version
 from codewithgpu.version import version as __version__
-
-# Attributes
-__all__ = [_s for _s in dir() if not _s.startswith('_')]
```

## codewithgpu/version.py

```diff
@@ -1,6 +1,6 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-version = '0.2.2'
+version = '0.2.3'
 git_version = '9ec37e2480a68e67e04cba90c5d6f7e0921f14ba'
```

## Comparing `codewithgpu-0.2.2.dist-info/LICENSE` & `codewithgpu-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `codewithgpu-0.2.2.dist-info/METADATA` & `codewithgpu-0.2.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codewithgpu
-Version: 0.2.2
+Version: 0.2.3
 Summary: CodeWithGPU Python Client
 Home-page: https://github.com/seetacloud/codewithgpu
 Author: SeetaCloud
 License: Apache License
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codewithgpu Version: 0.2.2 Summary: CodeWithGPU
+Metadata-Version: 2.1 Name: codewithgpu Version: 0.2.3 Summary: CodeWithGPU
 Python Client Home-page: https://github.com/seetacloud/codewithgpu Author:
 SeetaCloud License: Apache License Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

## Comparing `codewithgpu-0.2.2.dist-info/RECORD` & `codewithgpu-0.2.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-codewithgpu/__init__.py,sha256=iCN3FvJ9iI98FWnUr-TRBMSMI8AqIk-2St7FKxTSDsM,1549
+codewithgpu/__init__.py,sha256=5G0tOZ6tnOhy4-GNBRPtpzabyubzMDj9m8M53oV_uow,1448
 codewithgpu/cli.py,sha256=OGi5C1KheYHv_4vL-_kzsep87W5WnbgesqZT96UMFw4,1924
-codewithgpu/version.py,sha256=8O3INcbvrfN0nFT3xYgbDmQ9Uc1oQsrAgvWOrThFbNs,185
+codewithgpu/version.py,sha256=gdLNQMLmBJYtAyLqH74UBSf6q4Krc6Se71nGZTl87xs,185
 codewithgpu/data/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
 codewithgpu/data/dataset.py,sha256=lhm1KAR12xb3-AUtHWvYjhPEytL3ozpIY6RDVdsr_Wc,6547
 codewithgpu/data/reader.py,sha256=obDLYyFvZf0WxXdeDMYwqsS14vgXPKvvIxRv7vfA-HE,7177
 codewithgpu/data/record.proto,sha256=mToQiLJ9idcmEoaKwEbCNffe1Cv4ZcNoUhyW2oTvw-Y,608
 codewithgpu/data/record.py,sha256=xD53qMX1UWAXrOemlhXuiYZfHxbw0lXGUDof9IsRbfM,8941
 codewithgpu/data/record_pb2.py,sha256=0eygLJUOK3KKsQXBOBbwB-wh-kMQW5Z35ZMAVs0vlsA,10202
 codewithgpu/data/tf_record.proto,sha256=iA-8rb9uDY6g-FFcpAsHW3He1Djc_pRzKXjtk2V3UlI,780
@@ -17,13 +17,13 @@
 codewithgpu/model/download.py,sha256=-SJ7EPqkKYEQTmIQCezDfLgx6YKtPoWuoxbfyTCu89A,1418
 codewithgpu/utils/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
 codewithgpu/utils/cg_cli.py,sha256=3Urv0uigHTPjfRF4EdSrk1hQbloCIUlgahe3ymL0pdo,4076
 codewithgpu/utils/decorator.py,sha256=eavLk-cu8K9kiTNquJjAwVIziQ2-dG23aFTe3i_1Vkk,3805
 codewithgpu/utils/deprecation.py,sha256=JNzJijpwuXdu9nf4pOzlLqmFvrCM__JZRy5zVU_Xkk8,3629
 codewithgpu/utils/logging.py,sha256=psQyhYN4RRfhcohMvOMIRb2SEsfsRzk3rQzhelhGjgI,3741
 codewithgpu/utils/unittest_util.py,sha256=jz2HVLIHe_TlrQ9QJ-HOg0Erf-QEVmfuQDo0Q4BkfDw,1226
-codewithgpu-0.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-codewithgpu-0.2.2.dist-info/METADATA,sha256=RIJp2NeEZY5sfJ9oM4yWv-cNpoVgTxKVkurkThpCXYU,3033
-codewithgpu-0.2.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-codewithgpu-0.2.2.dist-info/entry_points.txt,sha256=uIKsOHrbYlsA2As8st4u2hBbCA5pGUjKwJuRJUpK0MQ,49
-codewithgpu-0.2.2.dist-info/top_level.txt,sha256=orLQMHWZMLDPkZO_r-8233w9F1YzYk6xqY7Oti5-P4s,87
-codewithgpu-0.2.2.dist-info/RECORD,,
+codewithgpu-0.2.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+codewithgpu-0.2.3.dist-info/METADATA,sha256=9AXaTn4SJKjJ37ICh7-0hvOMwd4WhQfFDLnsD4hwxoE,3033
+codewithgpu-0.2.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+codewithgpu-0.2.3.dist-info/entry_points.txt,sha256=uIKsOHrbYlsA2As8st4u2hBbCA5pGUjKwJuRJUpK0MQ,49
+codewithgpu-0.2.3.dist-info/top_level.txt,sha256=orLQMHWZMLDPkZO_r-8233w9F1YzYk6xqY7Oti5-P4s,87
+codewithgpu-0.2.3.dist-info/RECORD,,
```

