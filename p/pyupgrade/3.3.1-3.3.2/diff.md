# Comparing `tmp/pyupgrade-3.3.1.tar.gz` & `tmp/pyupgrade-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrade-3.3.1.tar", last modified: Tue Dec  6 22:19:56 2022, max compression
+gzip compressed data, was "pyupgrade-3.3.2.tar", last modified: Tue Apr 25 01:35:06 2023, max compression
```

## Comparing `pyupgrade-3.3.1.tar` & `pyupgrade-3.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-06 22:19:56.431605 pyupgrade-3.3.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13751 2022-12-06 22:19:56.431605 pyupgrade-3.3.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13129 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-06 22:19:56.419605 pyupgrade-3.3.1/pyupgrade/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2022-11-10 15:38:09.000000 pyupgrade-3.3.1/pyupgrade/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11784 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-06 22:19:56.431605 pyupgrade-3.3.1/pyupgrade/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/collections_abc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2022-12-02 18:20:28.000000 pyupgrade-3.3.1/pyupgrade/_plugins/datetime_utc_alias.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1231 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/default_encoding.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/dict_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1709 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/format_locals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4334 2022-11-29 16:14:49.000000 pyupgrade-3.3.1/pyupgrade/_plugins/fstrings.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1483 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/identity_equality.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    20301 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/io_open.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/lru_cache.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/metaclass_type.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/mock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2224 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/native_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/new_style_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3851 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/open_mode.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/oserror_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9357 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/percent_format.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/set_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/six_base_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6558 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/six_calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/six_metaclasses.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/six_remove_decorators.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/six_simple.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/subprocess_run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1747 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/type_of_primitive.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8084 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4836 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep563.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep585.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5610 2022-11-10 15:10:00.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep604.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2022-11-10 15:10:00.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep646_unpack.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/typing_text.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/unittest_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1189 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/unpack_list_comprehension.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6416 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_plugins/versioned_branches.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/pyupgrade/_string_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    15888 2022-10-29 19:34:22.000000 pyupgrade-3.3.1/pyupgrade/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-06 22:19:56.419605 pyupgrade-3.3.1/pyupgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13751 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2022-12-06 22:19:56.000000 pyupgrade-3.3.1/pyupgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1199 2022-12-06 22:19:56.431605 pyupgrade-3.3.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:39.000000 pyupgrade-3.3.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.876028 pyupgrade-3.3.2/pyupgrade/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2022-11-10 15:38:09.000000 pyupgrade-3.3.2/pyupgrade/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11784 2023-02-20 22:41:07.000000 pyupgrade-3.3.2/pyupgrade/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/pyupgrade/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/collections_abc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2022-12-02 18:20:28.000000 pyupgrade-3.3.2/pyupgrade/_plugins/datetime_utc_alias.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1231 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/default_encoding.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/dict_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1709 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/format_locals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4334 2022-11-29 16:14:49.000000 pyupgrade-3.3.2/pyupgrade/_plugins/fstrings.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1483 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/identity_equality.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-04-25 01:35:03.000000 pyupgrade-3.3.2/pyupgrade/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/io_open.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/lru_cache.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/metaclass_type.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/mock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2224 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/native_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/new_style_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3851 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/open_mode.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/oserror_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9357 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/percent_format.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/set_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_base_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6558 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_metaclasses.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_remove_decorators.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_simple.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/subprocess_run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1747 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/type_of_primitive.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8084 2022-12-06 22:19:56.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4836 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep563.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep585.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5610 2022-11-10 15:10:00.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep604.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2022-11-10 15:10:00.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep646_unpack.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_text.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/unittest_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1189 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/unpack_list_comprehension.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6416 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/versioned_branches.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_string_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    15888 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.876028 pyupgrade-3.3.2/pyupgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1199 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/setup.py
```

### Comparing `pyupgrade-3.3.1/LICENSE` & `pyupgrade-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/PKG-INFO` & `pyupgrade-3.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.3.1
+Version: 3.3.2
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.pyupgrade?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/2/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
+[![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
 =========
 
 A tool (and pre-commit hook) to automatically upgrade syntax for newer
 versions of the language.
@@ -35,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.1/README.md` & `pyupgrade-3.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.pyupgrade?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/2/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
+[![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
 =========
 
 A tool (and pre-commit hook) to automatically upgrade syntax for newer
 versions of the language.
@@ -18,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.1/pyupgrade/_ast_helpers.py` & `pyupgrade-3.3.2/pyupgrade/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_data.py` & `pyupgrade-3.3.2/pyupgrade/_data.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_main.py` & `pyupgrade-3.3.2/pyupgrade/_main.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/collections_abc.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/collections_abc.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/datetime_utc_alias.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/datetime_utc_alias.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/default_encoding.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/default_encoding.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/dict_literals.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/dict_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/format_locals.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/format_locals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/fstrings.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/fstrings.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/identity_equality.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/identity_equality.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/imports.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 
 
 class FromImport(NamedTuple):
     start: int
     mod_start: int
     mod_end: int
     names: tuple[int, ...]
+    ends: tuple[int, ...]
     end: int
 
     @classmethod
     def parse(cls, i: int, tokens: list[Token]) -> FromImport:
         if has_space_before(i, tokens):
             start = i - 1
         else:
@@ -306,35 +307,38 @@
 
         # XXX: does not handle `*` imports
         names = [
             j
             for j in range(import_token + 1, end)
             if tokens[j].name == 'NAME'
         ]
+        ends_by_offset = {}
         for i in reversed(range(len(names))):
             if tokens[names[i]].src == 'as':
+                ends_by_offset[names[i - 1]] = names[i + 1]
                 del names[i:i + 2]
+        ends = tuple(ends_by_offset.get(pos, pos) for pos in names)
 
-        return cls(start, mod_start, mod_end + 1, tuple(names), end)
+        return cls(start, mod_start, mod_end + 1, tuple(names), ends, end)
 
     def remove_self(self, tokens: list[Token]) -> None:
         del tokens[self.start:self.end]
 
     def replace_modname(self, tokens: list[Token], modname: str) -> None:
         tokens[self.mod_start:self.mod_end] = [Token('CODE', modname)]
 
     def remove_parts(self, tokens: list[Token], idxs: list[int]) -> None:
         for idx in reversed(idxs):
             if idx == 0:  # look forward until next name and del
                 del tokens[self.names[idx]:self.names[idx + 1]]
             else:  # look backward for comma and del
-                j = end = self.names[idx]
+                j = self.names[idx]
                 while tokens[j].src != ',':
                     j -= 1
-                del tokens[j:end + 1]
+                del tokens[j:self.ends[idx] + 1]
 
 
 def _alias_to_s(alias: ast.alias) -> str:
     if alias.asname:
         return f'{alias.name} as {alias.asname}'
     else:
         return alias.name
```

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/io_open.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/io_open.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/legacy.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/lru_cache.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/lru_cache.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/metaclass_type.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/metaclass_type.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/mock.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/mock.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/native_literals.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/native_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/new_style_classes.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/new_style_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/open_mode.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/open_mode.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/oserror_aliases.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/oserror_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/percent_format.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/percent_format.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/set_literals.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/set_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/six_base_classes.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/six_base_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/six_calls.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/six_calls.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/six_metaclasses.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/six_metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/six_remove_decorators.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/six_remove_decorators.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/six_simple.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/six_simple.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/subprocess_run.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/type_of_primitive.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/type_of_primitive.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_classes.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep563.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep563.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep585.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep585.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep604.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep604.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_pep646_unpack.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep646_unpack.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/typing_text.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/typing_text.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/unittest_aliases.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/unittest_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/unpack_list_comprehension.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/unpack_list_comprehension.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_plugins/versioned_branches.py` & `pyupgrade-3.3.2/pyupgrade/_plugins/versioned_branches.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_string_helpers.py` & `pyupgrade-3.3.2/pyupgrade/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade/_token_helpers.py` & `pyupgrade-3.3.2/pyupgrade/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/pyupgrade.egg-info/PKG-INFO` & `pyupgrade-3.3.2/pyupgrade.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.3.1
+Version: 3.3.2
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.pyupgrade?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/2/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=2&branchName=main)
+[![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
 =========
 
 A tool (and pre-commit hook) to automatically upgrade syntax for newer
 versions of the language.
@@ -35,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.1/pyupgrade.egg-info/SOURCES.txt` & `pyupgrade-3.3.2/pyupgrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.1/setup.cfg` & `pyupgrade-3.3.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyupgrade
-version = 3.3.1
+version = 3.3.2
 description = A tool to automatically upgrade syntax for newer versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/pyupgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

