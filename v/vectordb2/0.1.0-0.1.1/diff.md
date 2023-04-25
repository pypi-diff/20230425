# Comparing `tmp/vectordb2-0.1.0.tar.gz` & `tmp/vectordb2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb2-0.1.0.tar", last modified: Tue Apr 25 04:04:48 2023, max compression
+gzip compressed data, was "vectordb2-0.1.1.tar", last modified: Tue Apr 25 04:31:47 2023, max compression
```

## Comparing `vectordb2-0.1.0.tar` & `vectordb2-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:04:48.641844 vectordb2-0.1.0/
--rw-r--r--   0 prelovac   (502) staff       (20)      698 2023-04-25 04:04:48.641595 vectordb2-0.1.0/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)     6469 2023-04-25 03:59:49.000000 vectordb2-0.1.0/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:04:48.640042 vectordb2-0.1.0/pymemory/
--rw-r--r--   0 prelovac   (502) staff       (20)       31 2023-04-25 01:36:30.000000 vectordb2-0.1.0/pymemory/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2546 2023-04-25 04:00:36.000000 vectordb2-0.1.0/pymemory/chunking.py
--rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:00:36.000000 vectordb2-0.1.0/pymemory/embedding.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3707 2023-04-25 04:00:36.000000 vectordb2-0.1.0/pymemory/pymemory.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1047 2023-04-25 04:00:36.000000 vectordb2-0.1.0/pymemory/storage.py
--rw-r--r--   0 prelovac   (502) staff       (20)      873 2023-04-25 04:00:36.000000 vectordb2-0.1.0/pymemory/vector_search.py
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 04:04:48.641911 vectordb2-0.1.0/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1017 2023-04-25 04:04:32.000000 vectordb2-0.1.0/setup.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:04:48.641282 vectordb2-0.1.0/vectordb2.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)      698 2023-04-25 04:04:48.000000 vectordb2-0.1.0/vectordb2.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      313 2023-04-25 04:04:48.000000 vectordb2-0.1.0/vectordb2.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 04:04:48.000000 vectordb2-0.1.0/vectordb2.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      104 2023-04-25 04:04:48.000000 vectordb2-0.1.0/vectordb2.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-04-25 04:04:48.000000 vectordb2-0.1.0/vectordb2.egg-info/top_level.txt
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.382151 vectordb2-0.1.1/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-25 04:13:48.000000 vectordb2-0.1.1/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:31:47.381923 vectordb2-0.1.1/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)     9011 2023-04-25 04:29:42.000000 vectordb2-0.1.1/README.md
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 04:31:47.382221 vectordb2-0.1.1/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1117 2023-04-25 04:31:30.000000 vectordb2-0.1.1/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.380452 vectordb2-0.1.1/vectordb/
+-rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-04-25 04:10:57.000000 vectordb2-0.1.1/vectordb/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2546 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/chunking.py
+-rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/embedding.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3703 2023-04-25 04:10:33.000000 vectordb2-0.1.1/vectordb/memory.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1047 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/storage.py
+-rw-r--r--   0 prelovac   (502) staff       (20)      873 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/vector_search.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.381635 vectordb2-0.1.1/vectordb2.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      319 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      104 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/top_level.txt
```

### Comparing `vectordb2-0.1.0/PKG-INFO` & `vectordb2-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: vectordb2
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for storing and retrieving text using chunking, embedding, and vector search
 Home-page: https://github.com/yourusername/pymemory
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: text chunking embedding vector search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
```

### Comparing `vectordb2-0.1.0/README.md` & `vectordb2-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-# PyMemory
+# VectorDB
 
-PyMemory is a Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata.
+VectorDB is a minimal Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata.
 
 ## Installation
 
-To install PyMemory, use pip:
+To install VectorDB, use pip:
 
 ```
-pip install pymemory
+pip install vectordb2
 ```
 
 ## Usage
 
 Here's a quick example of how to use PyMemory:
 
 ```
-from pymemory import PyMemory
+from vectordb import Memory
 
-memory = PyMemory(chunking_strategy={'mode':"sliding_window"})
+memory = Memory()
+
+# text = "..."
+# metadata = {...}
 
 # Save text with metadata
 memory.save(text, metadata)
 
 # Search for relevant chunks
 results = memory.search(query, top_n=3)
 ```
 
 ## Methods
-PyMemory provides the following methods:
+Memory provides the following methods:
 
 
 **__init__(self, memory_file=None, chunking_strategy={"mode":"sliding_window"},
 embedding_model="sentence-transformers/all-MiniLM-L6-v2")**
 
 
-- Initializes the PyMemory class.
-- **memory_file** (str): Path to the memory file (default: None). If provided, memory will persist to disk
+- Initializes the Memory class.
+- **memory_file** (str): Path to the memory file (default: None). If provided, memory will persist to disk.
 - **chunking_strategy** (dict): Dictionary containing the chunking mode (default: {"mode": "sliding_window"})
    Options::
 	{'mode':'sliding_window', 'window_size': 256, 'overlap': 32}
 	{'mode':'paragraph'}
 - **embedding_model** (str): Name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2").
 
 **save(self, texts, metadata_list, memory_file=None)**
@@ -65,24 +68,17 @@
 
 - Prints the contents of the memory.
 
 
 ## Example
 
 ```
-from pymemory import PyMemory
-
-memory = PyMemory(chunking_strategy={'mode':"sliding_window"})
-
-text = """
-Machine learning is a method of data analysis that automates analytical model building.
-...
-from pymemory import PyMemory
+from vectordb import Memory
 
-memory = PyMemory(chunking_strategy={'mode':"sliding_window"})
+memory = Memory(chunking_strategy={'mode':'sliding_window', 'window_size': 128, 'overlap': 16})
 
 text = """
 Machine learning is a method of data analysis that automates analytical model building.
 
 It is a branch of artificial intelligence based on the idea that systems can learn from data,
 identify patterns and make decisions with minimal human intervention.
 
@@ -136,18 +132,48 @@
 It is important to weigh the potential benefits and risks of AI carefully as we continue to develop this technology. With careful planning and oversight, AI has the potential to make the world a better place. However, if we are not careful, it could also lead to serious problems.
 """
 
 metadata2 = {"title": "Introduction to Artificial Intelligence", "url": "https://example.com/introduction-to-artificial-intelligence"}
 
 memory.save(text2, metadata2)
 
-
 query = "What is the relationship between AI and machine learning?"
 
 results = memory.search(query, top_n=3)
 
 print(results)
 ```
 
+Output:
+```
+[
+  {
+    'chunk': 'Machine learning is a method of data analysis that automates analytical model building . It is a branch of artificial intelligence based on the idea that systems can learn from data , identify patterns and make decisions with minimal human intervention . Machine learning algorithms are trained on data sets that contain examples of the desired output . For example , a machine learning algorithm that is used to classify images might be trained on a data set that contains images of cats and dogs . Once an algorithm is trained , it can be used to make predictions on new data . For example , the machine learning algorithm that is used to classify images could be used to predict whether a new image contains a cat', 
+    'metadata': 
+    {
+      'title': 'Introduction to Machine Learning', 
+      'url': 'https://example.com/introduction-to-machine-learning'
+    }
+  }, 
+  {
+    'chunk': 'Artificial intelligence ( AI ) is the simulation of human intelligence in machines that are programmed to think like humans and mimic their actions . The term may also be applied to any machine that exhibits traits associated with a human mind such as learning and problem - solving . AI research has been highly successful in developing effective techniques for solving a wide range of problems , from game playing to medical diagnosis . However , there is still a long way to go before AI can truly match the intelligence of humans . One of the main challenges is that human intelligence is incredibly complex and poorly understood . Despite the challenges , AI is a rapidly growing field with the potential to revolutionize many aspects', 
+    'metadata': 
+    {
+      'title': 'Introduction to Artificial Intelligence', 
+      'url': 'https://example.com/introduction-to-artificial-intelligence'
+    }
+  }, 
+  {
+    'chunk': 'are also potential risks associated with AI , such as : Job displacement : As AI becomes more capable , it is possible that it will displace some human workers . Weaponization : AI could be used to develop new weapons that are more powerful and destructive than anything we have today . Loss of control : If AI becomes too powerful , we may lose control over it , with potentially disastrous consequences . It is important to weigh the potential benefits and risks of AI carefully as we continue to develop this technology . With careful planning and oversight , AI has the potential to make the world a better place . However , if we are not careful , it could also lead to serious', 
+    'metadata': 
+    {
+      'title': 'Introduction to Artificial Intelligence', 
+      'url': 'https://example.com/introduction-to-artificial-intelligence'
+    }
+  }
+]
+```
+
+
 ## License
 
 MIT License.
```

### Comparing `vectordb2-0.1.0/pymemory/chunking.py` & `vectordb2-0.1.1/vectordb/chunking.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.0/pymemory/embedding.py` & `vectordb2-0.1.1/vectordb/embedding.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.0/pymemory/pymemory.py` & `vectordb2-0.1.1/vectordb/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import List, Dict, Any
 from .chunking import Chunker
 from .embedding import Embedder
 from .vector_search import VectorSearch
 from .storage import Storage
 
 
-class PyMemory:
+class Memory:
     def __init__(
         self,
         memory_file: str = None,
         chunking_strategy: dict = {"mode": "sliding_window"},
         embedding_model: str = "sentence-transformers/all-MiniLM-L6-v2",
     ):
         """
-        Initializes the PyMemory class.
+        Initializes the Memory class.
 
         :param memory_file: a string containing the path to the memory file. (default: None)
         :param chunking_strategy: a dictionary containing the chunking mode (default: {"mode": "sliding_window"}).
         :param embedding_model: a string containing the name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2").
         """
         self.memory_file = memory_file
         self.memory = (
```

### Comparing `vectordb2-0.1.0/pymemory/storage.py` & `vectordb2-0.1.1/vectordb/storage.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.0/pymemory/vector_search.py` & `vectordb2-0.1.1/vectordb/vector_search.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.0/setup.py` & `vectordb2-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vectordb2",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "torch>=1.9.0",
         "transformers>=4.10.0",
         "numpy>=1.21.0",
         "scikit-learn>=0.24.0",
         "scipy>=1.7.0",
@@ -22,9 +22,11 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `vectordb2-0.1.0/vectordb2.egg-info/PKG-INFO` & `vectordb2-0.1.1/vectordb2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: vectordb2
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for storing and retrieving text using chunking, embedding, and vector search
 Home-page: https://github.com/yourusername/pymemory
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: text chunking embedding vector search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
```

