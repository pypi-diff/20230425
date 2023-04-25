# Comparing `tmp/tritondse-0.1.1.tar.gz` & `tmp/tritondse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.1.tar", last modified: Fri Apr  7 07:09:24 2023, max compression
+gzip compressed data, was "tritondse-0.1.2.tar", last modified: Tue Apr 25 05:15:22 2023, max compression
```

## Comparing `tritondse-0.1.1.tar` & `tritondse-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:09:24.462888 tritondse-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11357 2023-04-07 07:09:21.000000 tritondse-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-07 07:09:24.462888 tritondse-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-07 07:09:21.000000 tritondse-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 07:09:24.466888 tritondse-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-07 07:09:21.000000 tritondse-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:09:24.462888 tritondse-0.1.1/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36095 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:09:24.462888 tritondse-0.1.1/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    50567 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    73739 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    35783 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-07 07:09:21.000000 tritondse-0.1.1/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:09:24.462888 tritondse-0.1.1/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-07 07:09:24.000000 tritondse-0.1.1/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-07 07:09:24.000000 tritondse-0.1.1/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 07:09:24.000000 tritondse-0.1.1/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-07 07:09:24.000000 tritondse-0.1.1/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 07:09:24.000000 tritondse-0.1.1/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11357 2023-04-25 05:15:20.000000 tritondse-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-25 05:15:22.614865 tritondse-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-25 05:15:20.000000 tritondse-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 05:15:22.614865 tritondse-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 05:15:20.000000 tritondse-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36095 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50567 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73739 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35783 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.1/LICENSE` & `tritondse-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/README.md` & `tritondse-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 The pip package will install all dependencies.
 
 
 ## Documentation
 
 A complete documentation on how to use TritonDSE is available on
-[Github pages](https://quarkslab.github.io/qsynthesis).
+[Github pages](https://quarkslab.github.io/tritondse).
 
 
 ---
 
 
 ## External Contributors
```

#### html2text {}

```diff
@@ -22,10 +22,10 @@
 ones) * Memory segmentation * Coverage strategies (block, edge, path) * Pointer
 coverage * Automatic input injection on stdin, argv * Input replay with QBDI *
 input scheduling *(customizable)* * sanitizer mechanism * basic heap allocator
 * some libc symbolic stubs --- # Quick start * [Installation](#installation) *
 [Documentation](#documentation) ## Installation ```bash pip install tritondse
 ``` The pip package will install all dependencies. ## Documentation A complete
 documentation on how to use TritonDSE is available on [Github pages](https://
-quarkslab.github.io/qsynthesis). --- ## External Contributors * Jonathan Salwan
+quarkslab.github.io/tritondse). --- ## External Contributors * Jonathan Salwan
 * Richard Abou Chaaya [*All contributions**](https://github.com/quarkslab/
 tritondse/graphs/contributors)
```

### Comparing `tritondse-0.1.1/tritondse/__init__.py` & `tritondse-0.1.2/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/arch.py` & `tritondse-0.1.2/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/callbacks.py` & `tritondse-0.1.2/tritondse/callbacks.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/config.py` & `tritondse-0.1.2/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/coverage.py` & `tritondse-0.1.2/tritondse/coverage.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/exception.py` & `tritondse-0.1.2/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/heap_allocator.py` & `tritondse-0.1.2/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/loaders/cle_loader.py` & `tritondse-0.1.2/tritondse/loaders/cle_loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/loaders/loader.py` & `tritondse-0.1.2/tritondse/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/loaders/program.py` & `tritondse-0.1.2/tritondse/loaders/program.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.2/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/memory.py` & `tritondse-0.1.2/tritondse/memory.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/process_state.py` & `tritondse-0.1.2/tritondse/process_state.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/qbdi_trace.py` & `tritondse-0.1.2/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/routines.py` & `tritondse-0.1.2/tritondse/routines.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/sanitizers.py` & `tritondse-0.1.2/tritondse/sanitizers.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/seed.py` & `tritondse-0.1.2/tritondse/seed.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/seeds_manager.py` & `tritondse-0.1.2/tritondse/seeds_manager.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/symbolic_executor.py` & `tritondse-0.1.2/tritondse/symbolic_executor.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/symbolic_explorator.py` & `tritondse-0.1.2/tritondse/symbolic_explorator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/thread_context.py` & `tritondse-0.1.2/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/trace.py` & `tritondse-0.1.2/tritondse/trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/types.py` & `tritondse-0.1.2/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/worklist.py` & `tritondse-0.1.2/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse/workspace.py` & `tritondse-0.1.2/tritondse/workspace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.1/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.2/tritondse.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -27,8 +27,10 @@
 tritondse.egg-info/dependency_links.txt
 tritondse.egg-info/requires.txt
 tritondse.egg-info/top_level.txt
 tritondse/loaders/__init__.py
 tritondse/loaders/cle_loader.py
 tritondse/loaders/loader.py
 tritondse/loaders/program.py
-tritondse/loaders/quokkaprogram.py
+tritondse/loaders/quokkaprogram.py
+tritondse/probes/__init__.py
+tritondse/probes/basic_trace.py
```

