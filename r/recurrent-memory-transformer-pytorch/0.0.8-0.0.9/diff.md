# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.8.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.8.tar", last modified: Mon Apr 24 20:57:14 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.9.tar", last modified: Mon Apr 24 21:25:39 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.8.tar` & `recurrent-memory-transformer-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.455706 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:25:39.639459 recurrent-memory-transformer-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 21:25:39.639459 recurrent-memory-transformer-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:25:39.639459 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:25:39.639459 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 21:25:39.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 21:25:39.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:25:39.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 21:25:39.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 21:25:39.000000 recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:25:39.639459 recurrent-memory-transformer-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 21:25:28.000000 recurrent-memory-transformer-pytorch-0.0.9/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/README.md` & `recurrent-memory-transformer-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -268,32 +268,51 @@
         length,
         memories = None,
         temperature = 1.,
         filter_thres = 0.9,
     ):
         assert self.transformer.causal, 'only autoregressive transformers can generate'
 
-        start_len = prime.shape[-1]
+        start_len, seq_len = prime.shape[-1], self.seq_len
 
-        output = prime
+        assert length >= start_len
+
+        *past_segments, curr_segment = prime.split(seq_len, dim = -1)
+
+        # catch memories up to the current segment
+
+        for past_segment in past_segments:
+            _, memories = self.forward(past_segment, memories)
+
+        # sample for the remaining length
 
         for ind in range(length - start_len):
 
-            logits, next_memories = self.forward(output, memories)
+            logits, next_memories = self.forward(curr_segment, memories)
 
             logits = logits[:, -1]
 
             filtered_logits = top_k(logits, thres = filter_thres)
             sampled = gumbel_sample(filtered_logits, temperature = temperature)
             sampled = rearrange(sampled, 'b -> b 1')
 
-            output = torch.cat((output, sampled), dim = -1)
+            curr_segment = torch.cat((curr_segment, sampled), dim = -1)
 
-            if divisible_by(output.shape[-1] - 1, self.seq_len):
+            if divisible_by(curr_segment.shape[-1] - 1, seq_len):
                 memories = next_memories
+                past_segment, curr_segment = curr_segment[..., :seq_len], curr_segment[..., -1:]
+                past_segments.append(past_segment)
+
+        # add current segment to all segments
+
+        past_segments.append(curr_segment)
+
+        # reconcat all segments
+
+        output = torch.cat(past_segments, dim = -1)
 
         output = output[:, start_len:]
         return output
 
     def forward(
         self,
         x,
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.8/setup.py` & `recurrent-memory-transformer-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

