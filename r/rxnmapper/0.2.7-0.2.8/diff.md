# Comparing `tmp/rxnmapper-0.2.7.tar.gz` & `tmp/rxnmapper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnmapper-0.2.7.tar", last modified: Fri Mar 24 11:32:57 2023, max compression
+gzip compressed data, was "rxnmapper-0.2.8.tar", last modified: Tue Apr 25 09:28:23 2023, max compression
```

## Comparing `rxnmapper-0.2.7.tar` & `rxnmapper-0.2.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.553762 rxnmapper-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-24 11:32:57.553762 rxnmapper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.545761 rxnmapper-0.2.7/rxnmapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/rxnmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/rxnmapper/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/rxnmapper/batched_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/rxnmapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.545761 rxnmapper-0.2.7/rxnmapper/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.545761 rxnmapper-0.2.7/rxnmapper/models/transformers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.549761 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-24 11:32:48.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json
--rw-r--r--   0 runner    (1001) docker     (123)  3212952 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/smiles_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/rxnmapper/tokenization_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.545761 rxnmapper-0.2.7/rxnmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 11:32:57.000000 rxnmapper-0.2.7/rxnmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-24 11:32:57.553762 rxnmapper-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:57.553762 rxnmapper-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/tests/test_batched_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/tests/test_smiles_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-24 11:32:49.000000 rxnmapper-0.2.7/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.943157 rxnmapper-0.2.8/rxnmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/batched_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.939157 rxnmapper-0.2.8/rxnmapper/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.939157 rxnmapper-0.2.8/rxnmapper/models/transformers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3212952 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/smiles_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/tokenization_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.943157 rxnmapper-0.2.8/rxnmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_batched_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_smiles_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/utils.py
```

### Comparing `rxnmapper-0.2.7/LICENSE` & `rxnmapper-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/PKG-INFO` & `rxnmapper-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnmapper
-Version: 0.2.7
+Version: 0.2.8
 Summary: Reaction atom-mapping from transfomers
 Home-page: https://github.com/rxn4chemistry/rxnmapper
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `rxnmapper-0.2.7/README.md` & `rxnmapper-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/attention.py` & `rxnmapper-0.2.8/rxnmapper/attention.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/batched_mapper.py` & `rxnmapper-0.2.8/rxnmapper/batched_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             yield from self._map_reaction_batch(rxns_chunk, detailed=detailed)
 
     def _map_reaction_batch(
         self, reaction_batch: List[str], detailed: bool
     ) -> Iterator[ResultWithInfo]:
         try:
             yield from self._try_map_reaction_batch(reaction_batch, detailed=detailed)
-        except Exception:
+        except Exception as e:
             logger.warning(
-                f"Error while mapping chunk of {len(reaction_batch)} reactions. "
+                f"Error while mapping chunk of {len(reaction_batch)} reactions: {e}. "
                 "Mapping them individually."
             )
             yield from self._map_reactions_one_by_one(reaction_batch, detailed=detailed)
 
     def _try_map_reaction_batch(
         self, reaction_batch: List[str], detailed: bool
     ) -> List[ResultWithInfo]:
```

### Comparing `rxnmapper-0.2.7/rxnmapper/core.py` & `rxnmapper-0.2.8/rxnmapper/core.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json` & `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin` & `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin` & `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt` & `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/smiles_utils.py` & `rxnmapper-0.2.8/rxnmapper/smiles_utils.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper/tokenization_smiles.py` & `rxnmapper-0.2.8/rxnmapper/tokenization_smiles.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/rxnmapper.egg-info/PKG-INFO` & `rxnmapper-0.2.8/rxnmapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnmapper
-Version: 0.2.7
+Version: 0.2.8
 Summary: Reaction atom-mapping from transfomers
 Home-page: https://github.com/rxn4chemistry/rxnmapper
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `rxnmapper-0.2.7/rxnmapper.egg-info/SOURCES.txt` & `rxnmapper-0.2.8/rxnmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/setup.cfg` & `rxnmapper-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/tests/test_batched_mapper.py` & `rxnmapper-0.2.8/tests/test_batched_mapper.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/tests/test_mapper.py` & `rxnmapper-0.2.8/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/tests/test_smiles_utils.py` & `rxnmapper-0.2.8/tests/test_smiles_utils.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.7/tests/utils.py` & `rxnmapper-0.2.8/tests/utils.py`

 * *Files identical despite different names*

