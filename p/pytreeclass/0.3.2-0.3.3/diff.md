# Comparing `tmp/pytreeclass-0.3.2.tar.gz` & `tmp/pytreeclass-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.2.tar", last modified: Mon Apr 24 01:04:21 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.3.tar", last modified: Tue Apr 25 07:45:16 2023, max compression
```

## Comparing `pytreeclass-0.3.2.tar` & `pytreeclass-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.141938 pytreeclass-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.141938 pytreeclass-0.3.2/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30880 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.437437 pytreeclass-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.437437 pytreeclass-0.3.3/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.441437 pytreeclass-0.3.3/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30880 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.441437 pytreeclass-0.3.3/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.2/LICENSE` & `pytreeclass-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/PKG-INFO` & `pytreeclass-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.2
+Version: 0.3.3
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.2/README.md` & `pytreeclass-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/docs/conf.py` & `pytreeclass-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/pytreeclass/__init__.py` & `pytreeclass-0.3.3/pytreeclass/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     "tree_indexer",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `pytreeclass-0.3.2/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.3.3/pytreeclass/_src/tree_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -329,16 +329,16 @@
         # unflatten rule for `treeclass` to use with `jax.tree_unflatten`
         tree = getattr(object, "__new__")(klass)
         vars(tree).update(zip(keys, leaves))
         return tree
 
     def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
         # flatten rule for `treeclass` to use with `jax.tree_flatten`
-        keys, leaves = zip(*vars(tree).items())
-        return leaves, keys
+        dynamic = vars(tree)
+        return tuple(dynamic.values()), tuple(dynamic.keys())
 
     def tree_flatten_with_keys(tree: T):
         # flatten rule for `treeclass` to use with `jax.tree_util.tree_flatten_with_path`
         dynamic = dict(vars(tree))
         for idx, key in enumerate(vars(tree)):
             entry = NamedSequenceKey(idx, key)
             dynamic[key] = (entry, dynamic[key])
@@ -409,40 +409,40 @@
 
     Note:
         ``leafwise=True`` adds the following methods to the class
 
         ==================      ============
         Method                  Operator
         ==================      ============
-        ``__add__``              `+`
-        ``__and__``              `&`
-        ``__ceil__``             `math.ceil`
-        ``__divmod__``           `divmod`
-        ``__eq__``               `==`
-        ``__floor__``            math.floor
-        ``__floordiv__``         `//`
-        ``__ge__``               `>=`
-        ``__gt__``               `>`
-        ``__invert__``           `~`
-        ``__le__``               `<=`
-        ``__lshift__``           `<<`
-        ``__lt__``               `<`
-        ``__matmul__``           `@`
-        ``__mod__``              `%`
-        ``__mul__``              `*`
-        ``__ne__``               `!=`
-        ``__neg__``              `-`
-        ``__or__``               `|`
-        ``__pos__``              `+`
-        ``__pow__``              `**`
-        ``__round__``            `round`
-        ``__sub__``              `-`
-        ``__truediv__``          `/`
-        ``__trunc__``            `math.trunc`
-        ``__xor__``              `^`
+        ``__add__``              ``+``
+        ``__and__``              ``&``
+        ``__ceil__``             ``math.ceil``
+        ``__divmod__``           ``divmod``
+        ``__eq__``               ``==``
+        ``__floor__``            ``math.floor``
+        ``__floordiv__``         ``//``
+        ``__ge__``               ``>=``
+        ``__gt__``               ``>``
+        ``__invert__``           ``~``
+        ``__le__``               ``<=``
+        ``__lshift__``           ``<<``
+        ``__lt__``               ``<``
+        ``__matmul__``           ``@``
+        ``__mod__``              ``%``
+        ``__mul__``              ``*``
+        ``__ne__``               ``!=``
+        ``__neg__``              ``-``
+        ``__or__``               ``|``
+        ``__pos__``              ``+``
+        ``__pow__``              ``**``
+        ``__round__``            ``round``
+        ``__sub__``              ``-``
+        ``__truediv__``          ``/``
+        ``__trunc__``            ``math.trunc``
+        ``__xor__``              ``^``
         ==================      ============
 
     """
 
     def __init_subclass__(klass: type[T], *a, leafwise: bool = False, **k) -> None:
         super().__init_subclass__(*a, **k)
         klass = _register_treeclass(klass)
```

### Comparing `pytreeclass-0.3.2/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.3.3/pytreeclass/_src/tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.3.3/pytreeclass/_src/tree_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,16 +145,18 @@
         nonlocal match
 
         return (match := True)
 
     mask = tree_map_with_trace(map_func, tree, is_leaf=is_leaf)
 
     if not match:
-        msg = f"No match is found for path={where} for tree with trace:\n"
-        msg += f"{tree_repr_with_trace(tree)}"
+        fmt = "/".join(map(str, where))
+        msg = f"No leaf match is found for path={fmt} for tree with trace:\n"
+        msg += f"{tree_repr_with_trace(tree)}\n"
+        msg += f"with mask={mask}"
         raise LookupError(msg)
 
     return mask
 
 
 def _combine_maybe_bool_masks(*masks: PyTree) -> PyTree:
     def is_bool_leaf(leaf: Any) -> bool:
```

### Comparing `pytreeclass-0.3.2/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.3/pytreeclass/_src/tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.3.3/pytreeclass/_src/tree_trace.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.3/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.2
+Version: 0.3.3
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.2/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.3/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/setup.py` & `pytreeclass-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_indexing.py` & `pytreeclass-0.3.3/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_nn.py` & `pytreeclass-0.3.3/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_tree_freeze.py` & `pytreeclass-0.3.3/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_tree_operator.py` & `pytreeclass-0.3.3/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_tree_pprint.py` & `pytreeclass-0.3.3/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_tree_viz_util.py` & `pytreeclass-0.3.3/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_treeclass.py` & `pytreeclass-0.3.3/tests/test_treeclass.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.2/tests/test_under_jit.py` & `pytreeclass-0.3.3/tests/test_under_jit.py`

 * *Files identical despite different names*

