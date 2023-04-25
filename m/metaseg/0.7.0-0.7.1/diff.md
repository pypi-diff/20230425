# Comparing `tmp/metaseg-0.7.0.tar.gz` & `tmp/metaseg-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.7.0.tar", last modified: Sun Apr 23 14:53:37 2023, max compression
+gzip compressed data, was "metaseg-0.7.1.tar", last modified: Tue Apr 25 08:31:39 2023, max compression
```

## Comparing `metaseg-0.7.0.tar` & `metaseg-0.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-20 11:50:36.000000 metaseg-0.7.0/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-20 11:50:36.000000 metaseg-0.7.0/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-23 14:53:37.570629 metaseg-0.7.0/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4145 2023-04-23 14:51:06.000000 metaseg-0.7.0/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.560629 metaseg-0.7.0/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      707 2023-04-23 14:53:31.000000 metaseg-0.7.0/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2832 2023-04-23 14:53:31.000000 metaseg-0.7.0/metaseg/falai_demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.567296 metaseg-0.7.0/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8048 2023-04-23 14:51:06.000000 metaseg-0.7.0/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.567296 metaseg-0.7.0/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-04-23 14:10:49.000000 metaseg-0.7.0/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.563963 metaseg-0.7.0/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-20 11:50:36.000000 metaseg-0.7.0/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-04-23 14:51:06.000000 metaseg-0.7.0/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-23 14:53:37.573963 metaseg-0.7.0/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-21 13:07:40.000000 metaseg-0.7.0/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.745072 metaseg-0.7.1/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-20 11:50:36.000000 metaseg-0.7.1/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-20 11:50:36.000000 metaseg-0.7.1/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-25 08:31:39.745072 metaseg-0.7.1/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4145 2023-04-23 14:51:06.000000 metaseg-0.7.1/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.741738 metaseg-0.7.1/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      707 2023-04-25 08:31:34.000000 metaseg-0.7.1/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2847 2023-04-25 08:31:27.000000 metaseg-0.7.1/metaseg/falai_demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.741738 metaseg-0.7.1/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8048 2023-04-23 14:51:06.000000 metaseg-0.7.1/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.745072 metaseg-0.7.1/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.745072 metaseg-0.7.1/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-04-23 14:10:49.000000 metaseg-0.7.1/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.745072 metaseg-0.7.1/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-20 11:50:36.000000 metaseg-0.7.1/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:31:39.741738 metaseg-0.7.1/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-25 08:31:39.000000 metaseg-0.7.1/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-04-25 08:31:39.000000 metaseg-0.7.1/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-25 08:31:39.000000 metaseg-0.7.1/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-04-25 08:31:39.000000 metaseg-0.7.1/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-25 08:31:39.000000 metaseg-0.7.1/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-20 11:50:36.000000 metaseg-0.7.1/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-04-23 14:51:06.000000 metaseg-0.7.1/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-25 08:31:39.748405 metaseg-0.7.1/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-21 13:07:40.000000 metaseg-0.7.1/setup.py
```

### Comparing `metaseg-0.7.0/LICENSE` & `metaseg-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/PKG-INFO` & `metaseg-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.7.0
+Version: 0.7.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.7.0/README.md` & `metaseg-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/__init__.py` & `metaseg-0.7.1/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `metaseg-0.7.0/metaseg/falai_demo.py` & `metaseg-0.7.1/metaseg/falai_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import BytesIO
 
 from PIL import Image
 
-from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
+from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.utils.data_utils import load_server_image
 
 try:
     from fal_serverless import isolated
 except ImportError:
     raise ImportError("Please install FalAI library using 'pip install fal_serverless'.")
```

### Comparing `metaseg-0.7.0/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.1/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/generator/build_sam.py` & `metaseg-0.7.1/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/generator/predictor.py` & `metaseg-0.7.1/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/mask_predictor.py` & `metaseg-0.7.1/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/common.py` & `metaseg-0.7.1/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/image_encoder.py` & `metaseg-0.7.1/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.1/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.1/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/sam.py` & `metaseg-0.7.1/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/modeling/transformer.py` & `metaseg-0.7.1/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/sahi_predict.py` & `metaseg-0.7.1/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/utils/amg.py` & `metaseg-0.7.1/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/utils/data_utils.py` & `metaseg-0.7.1/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/utils/file_utils.py` & `metaseg-0.7.1/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/utils/onnx.py` & `metaseg-0.7.1/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/utils/transforms.py` & `metaseg-0.7.1/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/webapp/app.py` & `metaseg-0.7.1/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg/webapp/demo.py` & `metaseg-0.7.1/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/metaseg.egg-info/PKG-INFO` & `metaseg-0.7.1/metaseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.7.0
+Version: 0.7.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.7.0/metaseg.egg-info/SOURCES.txt` & `metaseg-0.7.1/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.0/setup.py` & `metaseg-0.7.1/setup.py`

 * *Files identical despite different names*

