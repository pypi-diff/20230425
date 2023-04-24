# Comparing `tmp/viddiffusion-0.1.1.tar.gz` & `tmp/viddiffusion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viddiffusion-0.1.1.tar", last modified: Wed Apr 19 06:13:22 2023, max compression
+gzip compressed data, was "viddiffusion-0.1.2.tar", last modified: Mon Apr 24 22:40:55 2023, max compression
```

## Comparing `viddiffusion-0.1.1.tar` & `viddiffusion-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.754214 viddiffusion-0.1.1/
--rw-r--r--   0 masaishi   (501) staff       (20)    11357 2023-04-18 02:31:33.000000 viddiffusion-0.1.1/LICENSE
--rw-r--r--   0 masaishi   (501) staff       (20)     7653 2023-04-19 06:13:22.754057 viddiffusion-0.1.1/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)     7161 2023-04-19 06:12:03.000000 viddiffusion-0.1.1/README.md
--rw-r--r--   0 masaishi   (501) staff       (20)       38 2023-04-19 06:13:22.754265 viddiffusion-0.1.1/setup.cfg
--rw-r--r--   0 masaishi   (501) staff       (20)      834 2023-04-18 18:52:48.000000 viddiffusion-0.1.1/setup.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.753104 viddiffusion-0.1.1/viddiffusion/
--rw-r--r--   0 masaishi   (501) staff       (20)       78 2023-04-19 06:13:05.000000 viddiffusion-0.1.1/viddiffusion/__init__.py
--rw-r--r--   0 masaishi   (501) staff       (20)      723 2023-04-18 18:31:45.000000 viddiffusion-0.1.1/viddiffusion/image_utils.py
--rw-r--r--   0 masaishi   (501) staff       (20)     8484 2023-04-19 03:58:47.000000 viddiffusion-0.1.1/viddiffusion/pipeline_viddiffusion.py
--rw-r--r--   0 masaishi   (501) staff       (20)     2824 2023-04-18 18:32:08.000000 viddiffusion-0.1.1/viddiffusion/video_utils.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.753825 viddiffusion-0.1.1/viddiffusion.egg-info/
--rw-r--r--   0 masaishi   (501) staff       (20)     7653 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)      324 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/SOURCES.txt
--rw-r--r--   0 masaishi   (501) staff       (20)        1 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/dependency_links.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       66 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/requires.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       13 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/top_level.txt
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-24 22:40:55.707000 viddiffusion-0.1.2/
+-rw-r--r--   0 masaishi   (501) staff       (20)    11357 2023-04-18 02:31:33.000000 viddiffusion-0.1.2/LICENSE
+-rw-r--r--   0 masaishi   (501) staff       (20)     7659 2023-04-24 22:40:55.706885 viddiffusion-0.1.2/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)     7167 2023-04-19 06:17:36.000000 viddiffusion-0.1.2/README.md
+-rw-r--r--   0 masaishi   (501) staff       (20)       38 2023-04-24 22:40:55.707039 viddiffusion-0.1.2/setup.cfg
+-rw-r--r--   0 masaishi   (501) staff       (20)      834 2023-04-18 18:52:48.000000 viddiffusion-0.1.2/setup.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-24 22:40:55.706041 viddiffusion-0.1.2/viddiffusion/
+-rw-r--r--   0 masaishi   (501) staff       (20)       78 2023-04-24 22:38:39.000000 viddiffusion-0.1.2/viddiffusion/__init__.py
+-rw-r--r--   0 masaishi   (501) staff       (20)      723 2023-04-18 18:31:45.000000 viddiffusion-0.1.2/viddiffusion/image_utils.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     8560 2023-04-24 22:38:12.000000 viddiffusion-0.1.2/viddiffusion/pipeline_viddiffusion.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     2824 2023-04-18 18:32:08.000000 viddiffusion-0.1.2/viddiffusion/video_utils.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-24 22:40:55.706701 viddiffusion-0.1.2/viddiffusion.egg-info/
+-rw-r--r--   0 masaishi   (501) staff       (20)     7659 2023-04-24 22:40:55.000000 viddiffusion-0.1.2/viddiffusion.egg-info/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)      324 2023-04-24 22:40:55.000000 viddiffusion-0.1.2/viddiffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)        1 2023-04-24 22:40:55.000000 viddiffusion-0.1.2/viddiffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       66 2023-04-24 22:40:55.000000 viddiffusion-0.1.2/viddiffusion.egg-info/requires.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       13 2023-04-24 22:40:55.000000 viddiffusion-0.1.2/viddiffusion.egg-info/top_level.txt
```

### Comparing `viddiffusion-0.1.1/LICENSE` & `viddiffusion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.1/PKG-INFO` & `viddiffusion-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viddiffusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: VidDiffusion is a Python library that provides vid2vid pipeline by using Hugging Face's `diffusers`.
 Home-page: https://github.com/masaishi/VidDiffusion
 Author: Masamune Ishihara
 Author-email: masaishi_masa@yahoo.co.jp
 Maintainer: Masamune Ishihara
 Maintainer-email: masaishi_masa@yahoo.co.jp
 License: Apache License 2.0
@@ -46,15 +46,15 @@
 To install the library, run the following commands:
 ```bash
 export HUGGING_FACE_HUB_TOKEN=your_hf_auth_token
 pip install --upgrade transformers diffusers
 pip install viddiffusion
 ```
 
-[![VidDiffusion (PyPI)](https://badge.fury.io/py/viddiffusion.svg)](https://badge.fury.io/py/viddiffusion)
+[![VidDiffusion on PyPI](https://img.shields.io/pypi/v/viddiffusion.svg)](https://pypi.org/project/viddiffusion)
 
 
 # Usage
 
 First, import the library:
 ```python	
 from viddiffusion import VidDiffusionPipeline
```

### Comparing `viddiffusion-0.1.1/README.md` & `viddiffusion-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 To install the library, run the following commands:
 ```bash
 export HUGGING_FACE_HUB_TOKEN=your_hf_auth_token
 pip install --upgrade transformers diffusers
 pip install viddiffusion
 ```
 
-[![VidDiffusion (PyPI)](https://badge.fury.io/py/viddiffusion.svg)](https://badge.fury.io/py/viddiffusion)
+[![VidDiffusion on PyPI](https://img.shields.io/pypi/v/viddiffusion.svg)](https://pypi.org/project/viddiffusion)
 
 
 # Usage
 
 First, import the library:
 ```python	
 from viddiffusion import VidDiffusionPipeline
```

### Comparing `viddiffusion-0.1.1/setup.py` & `viddiffusion-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.1/viddiffusion/image_utils.py` & `viddiffusion-0.1.2/viddiffusion/image_utils.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.1/viddiffusion/pipeline_viddiffusion.py` & `viddiffusion-0.1.2/viddiffusion/pipeline_viddiffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         _is_pipe_updated = False
         if any(k in config for k in ('pretrained_model_name_or_path', 'custom_pipeline', 'torch_dtype', 'hf_auth_token')):
             self.pipe = DiffusionPipeline.from_pretrained(
                 pretrained_model_name_or_path=self.config['pretrained_model_name_or_path'],
                 custom_pipeline=self.config['custom_pipeline'],
                 torch_dtype=self.config['torch_dtype'],
                 use_auth_token=self.config['hf_auth_token'],
+                force_download=True,
+                resume_download=False,
             ).to(self.config['device'])
             self.pipe.safety_checker = self.config['safety_checker']
 
             _is_pipe_updated = True
         
         if any(k in config for k in ('scheduler', 'beta_start', 'beta_end', 'num_train_timesteps')) or _is_pipe_updated:
             self.pipe.scheduler = self.config['scheduler'](beta_start=self.config['beta_start'], beta_end=self.config['beta_end'], num_train_timesteps=self.config['num_train_timesteps'])
```

### Comparing `viddiffusion-0.1.1/viddiffusion/video_utils.py` & `viddiffusion-0.1.2/viddiffusion/video_utils.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.1/viddiffusion.egg-info/PKG-INFO` & `viddiffusion-0.1.2/viddiffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viddiffusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: VidDiffusion is a Python library that provides vid2vid pipeline by using Hugging Face's `diffusers`.
 Home-page: https://github.com/masaishi/VidDiffusion
 Author: Masamune Ishihara
 Author-email: masaishi_masa@yahoo.co.jp
 Maintainer: Masamune Ishihara
 Maintainer-email: masaishi_masa@yahoo.co.jp
 License: Apache License 2.0
@@ -46,15 +46,15 @@
 To install the library, run the following commands:
 ```bash
 export HUGGING_FACE_HUB_TOKEN=your_hf_auth_token
 pip install --upgrade transformers diffusers
 pip install viddiffusion
 ```
 
-[![VidDiffusion (PyPI)](https://badge.fury.io/py/viddiffusion.svg)](https://badge.fury.io/py/viddiffusion)
+[![VidDiffusion on PyPI](https://img.shields.io/pypi/v/viddiffusion.svg)](https://pypi.org/project/viddiffusion)
 
 
 # Usage
 
 First, import the library:
 ```python	
 from viddiffusion import VidDiffusionPipeline
```

