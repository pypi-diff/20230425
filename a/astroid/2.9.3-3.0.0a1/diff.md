# Comparing `tmp/astroid-2.9.3.tar.gz` & `tmp/astroid-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-2.9.3.tar", last modified: Sun Jan  9 16:18:57 2022, max compression
+gzip compressed data, was "astroid-3.0.0a1.tar", last modified: Tue Apr 25 12:17:50 2023, max compression
```

## Comparing `astroid-2.9.3.tar` & `astroid-3.0.0a1.tar`

### file list

```diff
@@ -1,108 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    26516 2022-01-09 16:18:47.000000 astroid-2.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-09 16:18:47.000000 astroid-2.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-09 16:18:57.837204 astroid-2.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.829204 astroid-2.9.3/astroid/
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    21392 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (121)    31376 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (121)    14886 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    10798 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    21078 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5084 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (121)     9142 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2618 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     9128 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9522 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)    10960 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    37072 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13084 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)    28089 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    23522 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24779 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (121)   166435 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    26964 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   109939 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11709 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    31076 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    18102 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (121)    88326 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4304 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.829204 astroid-2.9.3/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-01-09 16:18:57.837204 astroid-2.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-09 16:18:47.000000 astroid-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.646873 astroid-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-25 12:17:30.000000 astroid-3.0.0a1/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 12:17:30.000000 astroid-3.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 12:17:30.000000 astroid-3.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 12:17:50.646873 astroid-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 12:17:30.000000 astroid-3.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.622873 astroid-3.0.0a1/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.634873 astroid-3.0.0a1/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23321 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.634873 astroid-3.0.0a1/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136648 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103259 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.626873 astroid-3.0.0a1/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-25 12:17:30.000000 astroid-3.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 12:17:50.646873 astroid-3.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.646873 astroid-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   221738 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63153 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96027 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_utils.py
```

### Comparing `astroid-2.9.3/LICENSE` & `astroid-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-2.9.3/PKG-INFO` & `astroid-3.0.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 2.9.3
+Version: 3.0.0a1
 Summary: An abstract syntax tree for Python with inference support.
-Home-page: https://github.com/PyCQA/astroid
-Author: Python Code Quality Authority
-Author-email: code-quality@python.org
 License: LGPL-2.1-or-later
-Project-URL: Bug tracker, https://github.com/PyCQA/astroid/issues
+Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
+Project-URL: Source Code, https://github.com/pylint-dev/astroid
+Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6.2
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+License-File: CONTRIBUTORS.txt
 
 Astroid
 =======
 
-.. image:: https://coveralls.io/repos/github/PyCQA/astroid/badge.svg?branch=main
-    :target: https://coveralls.io/github/PyCQA/astroid?branch=main
-    :alt: Coverage badge from coveralls.io
+.. image:: https://codecov.io/gh/pylint-dev/astroid/branch/main/graph/badge.svg?token=Buxy4WptLb
+    :target: https://codecov.io/gh/pylint-dev/astroid
+    :alt: Coverage badge from codecov
 
 .. image:: https://readthedocs.org/projects/astroid/badge/?version=latest
     :target: http://astroid.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
 
-.. image:: https://results.pre-commit.ci/badge/github/PyCQA/astroid/main.svg
-   :target: https://results.pre-commit.ci/latest/github/PyCQA/astroid/main
+.. image:: https://results.pre-commit.ci/badge/github/pylint-dev/astroid/main.svg
+   :target: https://results.pre-commit.ci/latest/github/pylint-dev/astroid/main
    :alt: pre-commit.ci status
 
-.. |tidelift_logo| image:: https://raw.githubusercontent.com/PyCQA/astroid/main/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
-   :width: 75
-   :height: 60
+.. |tidelift_logo| image:: https://raw.githubusercontent.com/pylint-dev/astroid/main/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+   :width: 200
    :alt: Tidelift
 
 .. list-table::
    :widths: 10 100
 
    * - |tidelift_logo|
      - Professional support for astroid is available as part of the
@@ -117,10 +114,8 @@
 Test
 ----
 
 Tests are in the 'test' subdirectory. To launch the whole tests suite, you can use
 either `tox` or `pytest`::
 
     tox
-    pytest astroid
-
-
+    pytest
```

### Comparing `astroid-2.9.3/astroid/__init__.py` & `astroid-3.0.0a1/astroid/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,23 @@
-# Copyright (c) 2006-2013, 2015 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2014 Google, Inc.
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2016 Moises Lopez <moylop260@vauxoo.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2019 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""Python Abstract Syntax Tree New Generation
+"""Python Abstract Syntax Tree New Generation.
 
 The aim of this module is to provide a common base representation of
 python source code for projects such as pychecker, pyreverse,
 pylint... Well, actually the development of this library is essentially
 governed by pylint's needs.
 
-It extends class defined in the python's _ast module with some
-additional methods and attributes. Instance attributes are added by a
+It mimics the class defined in the python's _ast module with some
+additional methods and attributes. New nodes instances are not fully
+compatible with python's _ast.
+
+Instance attributes are added by a
 builder object, which can either generate extended ast (let's call
 them astroid ;) by visiting an existent ast tree or by inspecting living
 object. Methods are added by monkey patching ast classes.
 
 Main modules are:
 
 * nodes and scoped_nodes for more information about methods and
@@ -36,33 +26,61 @@
 * the manager contains a high level object to get astroid trees from
   source files and living objects. It maintains a cache of previously
   constructed tree for quick access
 
 * builder contains the class responsible to build astroid trees
 """
 
+import functools
+import tokenize
 from importlib import import_module
-from pathlib import Path
 
 # isort: off
-# We have an isort: off on '__version__' because the packaging need to access
-# the version before the dependencies are installed (in particular 'wrapt'
-# that is imported in astroid.inference)
-from astroid.__pkginfo__ import __version__, version
+# We have an isort: off on '__version__' because of a circular import in nodes.
 from astroid.nodes import node_classes, scoped_nodes
 
 # isort: on
 
 from astroid import inference, raw_building
+from astroid.__pkginfo__ import __version__, version
 from astroid.astroid_manager import MANAGER
 from astroid.bases import BaseInstance, BoundMethod, Instance, UnboundMethod
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import extract_node, parse
-from astroid.const import Context, Del, Load, Store
-from astroid.exceptions import *
+from astroid.const import BRAIN_MODULES_DIRECTORY, PY310_PLUS, Context
+from astroid.exceptions import (
+    AstroidBuildingError,
+    AstroidBuildingException,
+    AstroidError,
+    AstroidImportError,
+    AstroidIndexError,
+    AstroidSyntaxError,
+    AstroidTypeError,
+    AstroidValueError,
+    AttributeInferenceError,
+    BinaryOperationError,
+    DuplicateBasesError,
+    InconsistentMroError,
+    InferenceError,
+    InferenceOverwriteError,
+    MroError,
+    NameInferenceError,
+    NoDefault,
+    NotFoundError,
+    OperationError,
+    ParentMissingError,
+    ResolveError,
+    StatementMissing,
+    SuperArgumentTypeError,
+    SuperError,
+    TooManyLevelsError,
+    UnaryOperationError,
+    UnresolvableName,
+    UseInferenceDefault,
+)
 from astroid.inference_tip import _inference_tip_cached, inference_tip
 from astroid.objects import ExceptionInstance
 
 # isort: off
 # It's impossible to import from astroid.nodes with a wildcard, because
 # there is a cyclic import that prevent creating an __all__ in astroid/nodes
 # and we need astroid/scoped_nodes and astroid/node_classes to work. So
@@ -141,14 +159,15 @@
     Set,
     SetComp,
     Slice,
     Starred,
     Subscript,
     TryExcept,
     TryFinally,
+    TryStar,
     Tuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
@@ -158,13 +177,20 @@
     function_to_method,
 )
 
 # isort: on
 
 from astroid.util import Uninferable
 
+# Performance hack for tokenize. See https://bugs.python.org/issue43014
+# Adapted from https://github.com/PyCQA/pycodestyle/pull/993
+if (
+    not PY310_PLUS
+    and callable(getattr(tokenize, "_compile", None))
+    and getattr(tokenize._compile, "__wrapped__", None) is None  # type: ignore[attr-defined]
+):
+    tokenize._compile = functools.lru_cache(tokenize._compile)  # type: ignore[attr-defined]
+
 # load brain plugins
-ASTROID_INSTALL_DIRECTORY = Path(__file__).parent
-BRAIN_MODULES_DIRECTORY = ASTROID_INSTALL_DIRECTORY / "brain"
 for module in BRAIN_MODULES_DIRECTORY.iterdir():
     if module.suffix == ".py":
         import_module(f"astroid.brain.{module.stem}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/arguments.py` & `astroid-3.0.0a1/astroid/arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-# Copyright (c) 2015-2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018 Anthony Sottile <asottile@umich.edu>
-# Copyright (c) 2020 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-from typing import Optional
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
 
 from astroid import nodes
 from astroid.bases import Instance
-from astroid.const import Context
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import InferenceError, NoDefault
-from astroid.util import Uninferable
+from astroid.helpers import safe_infer
+from astroid.util import Uninferable, UninferableBase
 
 
 class CallSite:
-    """Class for understanding arguments passed into a call site
+    """Class for understanding arguments passed into a call site.
 
     It needs a call context, which contains the arguments and the
     keyword arguments that were passed into a given call site.
     In order to infer what an argument represents, call :meth:`infer_argument`
     with the corresponding function node and the argument name.
 
     :param callcontext:
@@ -35,94 +26,84 @@
     :param argument_context_map:
         Additional contexts per node, passed in from :attr:`astroid.context.Context.extra_context`
     :param context:
         An instance of :class:`astroid.context.Context`.
     """
 
     def __init__(
-        self, callcontext: CallContext, argument_context_map=None, context=None
+        self,
+        callcontext: CallContext,
+        argument_context_map=None,
+        context: InferenceContext | None = None,
     ):
         if argument_context_map is None:
             argument_context_map = {}
         self.argument_context_map = argument_context_map
         args = callcontext.args
         keywords = callcontext.keywords
-        self.duplicated_keywords = set()
+        self.duplicated_keywords: set[str] = set()
         self._unpacked_args = self._unpack_args(args, context=context)
         self._unpacked_kwargs = self._unpack_keywords(keywords, context=context)
 
         self.positional_arguments = [
-            arg for arg in self._unpacked_args if arg is not Uninferable
+            arg for arg in self._unpacked_args if not isinstance(arg, UninferableBase)
         ]
         self.keyword_arguments = {
             key: value
             for key, value in self._unpacked_kwargs.items()
-            if value is not Uninferable
+            if not isinstance(value, UninferableBase)
         }
 
     @classmethod
-    def from_call(cls, call_node, context: Optional[Context] = None):
+    def from_call(cls, call_node, context: InferenceContext | None = None):
         """Get a CallSite object from the given Call node.
 
         context will be used to force a single inference path.
         """
 
         # Determine the callcontext from the given `context` object if any.
         context = context or InferenceContext()
         callcontext = CallContext(call_node.args, call_node.keywords)
         return cls(callcontext, context=context)
 
     def has_invalid_arguments(self):
-        """Check if in the current CallSite were passed *invalid* arguments
+        """Check if in the current CallSite were passed *invalid* arguments.
 
         This can mean multiple things. For instance, if an unpacking
         of an invalid object was passed, then this method will return True.
         Other cases can be when the arguments can't be inferred by astroid,
         for example, by passing objects which aren't known statically.
         """
         return len(self.positional_arguments) != len(self._unpacked_args)
 
-    def has_invalid_keywords(self):
-        """Check if in the current CallSite were passed *invalid* keyword arguments
+    def has_invalid_keywords(self) -> bool:
+        """Check if in the current CallSite were passed *invalid* keyword arguments.
 
         For instance, unpacking a dictionary with integer keys is invalid
         (**{1:2}), because the keys must be strings, which will make this
         method to return True. Other cases where this might return True if
         objects which can't be inferred were passed.
         """
         return len(self.keyword_arguments) != len(self._unpacked_kwargs)
 
-    def _unpack_keywords(self, keywords, context=None):
+    def _unpack_keywords(self, keywords, context: InferenceContext | None = None):
         values = {}
         context = context or InferenceContext()
         context.extra_context = self.argument_context_map
         for name, value in keywords:
             if name is None:
                 # Then it's an unpacking operation (**)
-                try:
-                    inferred = next(value.infer(context=context))
-                except InferenceError:
-                    values[name] = Uninferable
-                    continue
-                except StopIteration:
-                    continue
-
+                inferred = safe_infer(value, context=context)
                 if not isinstance(inferred, nodes.Dict):
                     # Not something we can work with.
                     values[name] = Uninferable
                     continue
 
                 for dict_key, dict_value in inferred.items:
-                    try:
-                        dict_key = next(dict_key.infer(context=context))
-                    except InferenceError:
-                        values[name] = Uninferable
-                        continue
-                    except StopIteration:
-                        continue
+                    dict_key = safe_infer(dict_key, context=context)
                     if not isinstance(dict_key, nodes.Const):
                         values[name] = Uninferable
                         continue
                     if not isinstance(dict_key.value, str):
                         values[name] = Uninferable
                         continue
                     if dict_key.value in values:
@@ -131,50 +112,43 @@
                         self.duplicated_keywords.add(dict_key.value)
                         continue
                     values[dict_key.value] = dict_value
             else:
                 values[name] = value
         return values
 
-    def _unpack_args(self, args, context=None):
+    def _unpack_args(self, args, context: InferenceContext | None = None):
         values = []
         context = context or InferenceContext()
         context.extra_context = self.argument_context_map
         for arg in args:
             if isinstance(arg, nodes.Starred):
-                try:
-                    inferred = next(arg.value.infer(context=context))
-                except InferenceError:
-                    values.append(Uninferable)
-                    continue
-                except StopIteration:
-                    continue
-
-                if inferred is Uninferable:
+                inferred = safe_infer(arg.value, context=context)
+                if isinstance(inferred, UninferableBase):
                     values.append(Uninferable)
                     continue
                 if not hasattr(inferred, "elts"):
                     values.append(Uninferable)
                     continue
                 values.extend(inferred.elts)
             else:
                 values.append(arg)
         return values
 
-    def infer_argument(self, funcnode, name, context):
-        """infer a function argument value according to the call context
+    def infer_argument(self, funcnode, name, context):  # noqa: C901
+        """Infer a function argument value according to the call context.
 
         Arguments:
             funcnode: The function being called.
             name: The name of the argument whose value is being inferred.
             context: Inference context object
         """
         if name in self.duplicated_keywords:
             raise InferenceError(
-                "The arguments passed to {func!r} " " have duplicate keywords.",
+                "The arguments passed to {func!r} have duplicate keywords.",
                 call_site=self,
                 func=funcnode,
                 arg=name,
                 context=context,
             )
 
         # Look into the keywords first, maybe it's already there.
```

### Comparing `astroid-2.9.3/astroid/bases.py` & `astroid-3.0.0a1/astroid/bases.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,47 @@
-# Copyright (c) 2009-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2012 FELD Boris <lothiraldan@gmail.com>
-# Copyright (c) 2014-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 Google, Inc.
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Florian Bruhin <me@the-compiler.org>
-# Copyright (c) 2016-2017 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017 Calen Pennington <calen.pennington@gmail.com>
-# Copyright (c) 2018-2019 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018-2019 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Daniel Colascione <dancol@dancol.org>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 pre-commit-ci[bot] <bot@noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 doranid <ddandd@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """This module contains base classes and functions for the nodes and some
 inference utils.
 """
+from __future__ import annotations
 
 import collections
+import collections.abc
+from collections.abc import Iterator, Sequence
+from typing import TYPE_CHECKING, Any, ClassVar, Literal
 
-from astroid import decorators
+from astroid import nodes
 from astroid.const import PY310_PLUS
 from astroid.context import (
     CallContext,
     InferenceContext,
     bind_context_to_node,
     copy_context,
 )
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     NameInferenceError,
 )
-from astroid.util import Uninferable, lazy_descriptor, lazy_import
-
-objectmodel = lazy_import("interpreter.objectmodel")
-helpers = lazy_import("helpers")
-manager = lazy_import("manager")
+from astroid.interpreter import objectmodel
+from astroid.typing import (
+    InferBinaryOp,
+    InferenceErrorInfo,
+    InferenceResult,
+    SuccessfulInferenceResult,
+)
+from astroid.util import Uninferable, UninferableBase
 
+if TYPE_CHECKING:
+    from astroid.constraint import Constraint
 
-# TODO: check if needs special treatment
-BOOL_SPECIAL_METHOD = "__bool__"
-BUILTINS = "builtins"  # TODO Remove in 2.8
 
 PROPERTIES = {"builtins.property", "abc.abstractproperty"}
 if PY310_PLUS:
     PROPERTIES.add("enum.property")
 
 # List of possible property names. We use this list in order
 # to see if a method is a property or not. This should be
@@ -79,133 +62,179 @@
     "LazyProperty",
     "lazy",
     "cache_readonly",
     "DynamicClassAttribute",
 }
 
 
-def _is_property(meth, context=None):
+def _is_property(meth, context: InferenceContext | None = None) -> bool:
+    from astroid import helpers  # pylint: disable=import-outside-toplevel
+
     decoratornames = meth.decoratornames(context=context)
     if PROPERTIES.intersection(decoratornames):
         return True
     stripped = {
-        name.split(".")[-1] for name in decoratornames if name is not Uninferable
+        name.split(".")[-1]
+        for name in decoratornames
+        if not isinstance(name, UninferableBase)
     }
     if any(name in stripped for name in POSSIBLE_PROPERTIES):
         return True
 
     # Lookup for subclasses of *property*
     if not meth.decorators:
         return False
     for decorator in meth.decorators.nodes or ():
         inferred = helpers.safe_infer(decorator, context=context)
-        if inferred is None or inferred is Uninferable:
+        if inferred is None or isinstance(inferred, UninferableBase):
             continue
-        if inferred.__class__.__name__ == "ClassDef":
+        if isinstance(inferred, nodes.ClassDef):
             for base_class in inferred.bases:
-                if base_class.__class__.__name__ != "Name":
+                if not isinstance(base_class, nodes.Name):
                     continue
                 module, _ = base_class.lookup(base_class.name)
                 if module.name == "builtins" and base_class.name == "property":
                     return True
 
     return False
 
 
 class Proxy:
-    """a simple proxy object
+    """A simple proxy object.
 
     Note:
 
     Subclasses of this object will need a custom __getattr__
     if new instance attributes are created. See the Const class
     """
 
-    _proxied = None  # proxied object may be set by class or by instance
+    _proxied: nodes.ClassDef | nodes.FunctionDef
 
-    def __init__(self, proxied=None):
-        if proxied is not None:
+    def __init__(
+        self, proxied: nodes.ClassDef | nodes.FunctionDef | None = None
+    ) -> None:
+        if proxied is None:
+            # This is a hack to allow calling this __init__ during bootstrapping of
+            # builtin classes and their docstrings.
+            # For Const, Generator, and UnionType nodes the _proxied attribute
+            # is set during bootstrapping
+            # as we first need to build the ClassDef that they can proxy.
+            # Thus, if proxied is None self should be a Const or Generator
+            # as that is the only way _proxied will be correctly set as a ClassDef.
+            assert isinstance(self, (nodes.Const, Generator, UnionType))
+        else:
             self._proxied = proxied
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Any:
         if name == "_proxied":
             return self.__class__._proxied
         if name in self.__dict__:
             return self.__dict__[name]
         return getattr(self._proxied, name)
 
-    def infer(self, context=None):
+    def infer(  # type: ignore[return]
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> collections.abc.Generator[InferenceResult, None, InferenceErrorInfo | None]:
         yield self
 
 
-def _infer_stmts(stmts, context, frame=None):
+def _infer_stmts(
+    stmts: Sequence[InferenceResult],
+    context: InferenceContext | None,
+    frame: nodes.NodeNG | BaseInstance | None = None,
+) -> collections.abc.Generator[InferenceResult, None, None]:
     """Return an iterator on statements inferred by each statement in *stmts*."""
     inferred = False
+    constraint_failed = False
     if context is not None:
         name = context.lookupname
         context = context.clone()
+        constraints = context.constraints.get(name, {})
     else:
         name = None
+        constraints = {}
         context = InferenceContext()
 
     for stmt in stmts:
-        if stmt is Uninferable:
+        if isinstance(stmt, UninferableBase):
             yield stmt
             inferred = True
             continue
-        context.lookupname = stmt._infer_name(frame, name)
+        # 'context' is always InferenceContext and Instances get '_infer_name' from ClassDef
+        context.lookupname = stmt._infer_name(frame, name)  # type: ignore[union-attr]
         try:
+            stmt_constraints: set[Constraint] = set()
+            for constraint_stmt, potential_constraints in constraints.items():
+                if not constraint_stmt.parent_of(stmt):
+                    stmt_constraints.update(potential_constraints)
             for inf in stmt.infer(context=context):
-                yield inf
-                inferred = True
+                if all(constraint.satisfied_by(inf) for constraint in stmt_constraints):
+                    yield inf
+                    inferred = True
+                else:
+                    constraint_failed = True
         except NameInferenceError:
             continue
         except InferenceError:
             yield Uninferable
             inferred = True
-    if not inferred:
+
+    if not inferred and constraint_failed:
+        yield Uninferable
+    elif not inferred:
         raise InferenceError(
             "Inference failed for all members of {stmts!r}.",
             stmts=stmts,
             frame=frame,
             context=context,
         )
 
 
-def _infer_method_result_truth(instance, method_name, context):
+def _infer_method_result_truth(
+    instance: Instance, method_name: str, context: InferenceContext
+) -> bool | UninferableBase:
     # Get the method from the instance and try to infer
     # its return's truth value.
     meth = next(instance.igetattr(method_name, context=context), None)
     if meth and hasattr(meth, "infer_call_result"):
         if not meth.callable():
             return Uninferable
         try:
             context.callcontext = CallContext(args=[], callee=meth)
             for value in meth.infer_call_result(instance, context=context):
-                if value is Uninferable:
+                if isinstance(value, UninferableBase):
                     return value
                 try:
                     inferred = next(value.infer(context=context))
                 except StopIteration as e:
                     raise InferenceError(context=context) from e
                 return inferred.bool_value()
         except InferenceError:
             pass
     return Uninferable
 
 
 class BaseInstance(Proxy):
-    """An instance base class, which provides lookup methods for potential instances."""
+    """An instance base class, which provides lookup methods for potential
+    instances.
+    """
+
+    _proxied: nodes.ClassDef
 
-    special_attributes = None
+    special_attributes: objectmodel.ObjectModel
 
-    def display_type(self):
+    def display_type(self) -> str:
         return "Instance of"
 
-    def getattr(self, name, context=None, lookupclass=True):
+    def getattr(
+        self,
+        name: str,
+        context: InferenceContext | None = None,
+        lookupclass: bool = True,
+    ) -> list[SuccessfulInferenceResult]:
         try:
             values = self._proxied.instance_attr(name, context)
         except AttributeInferenceError as exc:
             if self.special_attributes and name in self.special_attributes:
                 return [self.special_attributes.lookup(name)]
 
             if lookupclass:
@@ -223,16 +252,18 @@
                 return values + self._proxied.getattr(
                     name, context, class_context=False
                 )
             except AttributeInferenceError:
                 pass
         return values
 
-    def igetattr(self, name, context=None):
-        """inferred getattr"""
+    def igetattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
+        """Inferred getattr."""
         if not context:
             context = InferenceContext()
         try:
             context.lookupname = name
             # avoid recursively inferring the same attr on the same class
             if context.push(self._proxied):
                 raise InferenceError(
@@ -254,73 +285,91 @@
                 if self._proxied.__class__.__name__ != "ClassDef":
                     raise
                 attrs = self._proxied.igetattr(name, context, class_context=False)
                 yield from self._wrap_attr(attrs, context)
             except AttributeInferenceError as error:
                 raise InferenceError(**vars(error)) from error
 
-    def _wrap_attr(self, attrs, context=None):
-        """wrap bound methods of attrs in a InstanceMethod proxies"""
+    def _wrap_attr(self, attrs, context: InferenceContext | None = None):
+        """Wrap bound methods of attrs in a InstanceMethod proxies."""
         for attr in attrs:
             if isinstance(attr, UnboundMethod):
                 if _is_property(attr):
                     yield from attr.infer_call_result(self, context)
                 else:
                     yield BoundMethod(attr, self)
             elif hasattr(attr, "name") and attr.name == "<lambda>":
                 if attr.args.arguments and attr.args.arguments[0].name == "self":
                     yield BoundMethod(attr, self)
                     continue
                 yield attr
             else:
                 yield attr
 
-    def infer_call_result(self, caller, context=None):
-        """infer what a class instance is returning when called"""
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
+        """Infer what a class instance is returning when called."""
         context = bind_context_to_node(context, self)
         inferred = False
+
+        # If the call is an attribute on the instance, we infer the attribute itself
+        if isinstance(caller, nodes.Call) and isinstance(caller.func, nodes.Attribute):
+            for res in self.igetattr(caller.func.attrname, context):
+                inferred = True
+                yield res
+
+        # Otherwise we infer the call to the __call__ dunder normally
         for node in self._proxied.igetattr("__call__", context):
-            if node is Uninferable or not node.callable():
+            if isinstance(node, UninferableBase) or not node.callable():
                 continue
             for res in node.infer_call_result(caller, context):
                 inferred = True
                 yield res
         if not inferred:
             raise InferenceError(node=self, caller=caller, context=context)
 
 
 class Instance(BaseInstance):
     """A special node representing a class instance."""
 
-    # pylint: disable=unnecessary-lambda
-    special_attributes = lazy_descriptor(lambda: objectmodel.InstanceModel())
+    special_attributes = objectmodel.InstanceModel()
+
+    def __init__(self, proxied: nodes.ClassDef | None) -> None:
+        super().__init__(proxied)
 
-    def __repr__(self):
+    infer_binary_op: ClassVar[InferBinaryOp[Instance]]
+
+    def __repr__(self) -> str:
         return "<Instance of {}.{} at 0x{}>".format(
             self._proxied.root().name, self._proxied.name, id(self)
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Instance of {self._proxied.root().name}.{self._proxied.name}"
 
-    def callable(self):
+    def callable(self) -> bool:
         try:
             self._proxied.getattr("__call__", class_context=False)
             return True
         except AttributeInferenceError:
             return False
 
-    def pytype(self):
+    def pytype(self) -> str:
         return self._proxied.qname()
 
-    def display_type(self):
+    def display_type(self) -> str:
         return "Instance of"
 
-    def bool_value(self, context=None):
-        """Infer the truth value for an Instance
+    def bool_value(
+        self, context: InferenceContext | None = None
+    ) -> bool | UninferableBase:
+        """Infer the truth value for an Instance.
 
         The truth value of an instance is determined by these conditions:
 
            * if it implements __bool__ on Python 3 or __nonzero__
              on Python 2, then its bool value will be determined by
              calling this special method and checking its result.
            * when this method is not defined, __len__() is called, if it
@@ -328,25 +377,24 @@
              nonzero. If a class defines neither __len__() nor __bool__(),
              all its instances are considered true.
         """
         context = context or InferenceContext()
         context.boundnode = self
 
         try:
-            result = _infer_method_result_truth(self, BOOL_SPECIAL_METHOD, context)
+            result = _infer_method_result_truth(self, "__bool__", context)
         except (InferenceError, AttributeInferenceError):
             # Fallback to __len__.
             try:
                 result = _infer_method_result_truth(self, "__len__", context)
             except (AttributeInferenceError, InferenceError):
                 return True
         return result
 
-    def getitem(self, index, context=None):
-        # TODO: Rewrap index to Const for this case
+    def getitem(self, index, context: InferenceContext | None = None):
         new_context = bind_context_to_node(context, self)
         if not context:
             context = new_context
         method = next(self.igetattr("__getitem__", context=context), None)
         # Create a new CallContext for providing index as an argument.
         new_context.callcontext = CallContext(args=[index], callee=method)
         if not isinstance(method, BoundMethod):
@@ -359,90 +407,125 @@
                 node=self,
                 context=context,
             )
         return next(method.infer_call_result(self, new_context), None)
 
 
 class UnboundMethod(Proxy):
-    """a special node representing a method not bound to an instance"""
+    """A special node representing a method not bound to an instance."""
+
+    _proxied: nodes.FunctionDef
 
-    # pylint: disable=unnecessary-lambda
-    special_attributes = lazy_descriptor(lambda: objectmodel.UnboundMethodModel())
+    special_attributes: objectmodel.BoundMethodModel | objectmodel.UnboundMethodModel = (
+        objectmodel.UnboundMethodModel()
+    )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         frame = self._proxied.parent.frame(future=True)
         return "<{} {} of {} at 0x{}".format(
             self.__class__.__name__, self._proxied.name, frame.qname(), id(self)
         )
 
-    def implicit_parameters(self):
+    def implicit_parameters(self) -> Literal[0, 1]:
         return 0
 
-    def is_bound(self):
+    def is_bound(self) -> bool:
         return False
 
-    def getattr(self, name, context=None):
+    def getattr(self, name, context: InferenceContext | None = None):
         if name in self.special_attributes:
             return [self.special_attributes.lookup(name)]
         return self._proxied.getattr(name, context)
 
-    def igetattr(self, name, context=None):
+    def igetattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
         if name in self.special_attributes:
             return iter((self.special_attributes.lookup(name),))
         return self._proxied.igetattr(name, context)
 
-    def infer_call_result(self, caller, context):
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
         """
         The boundnode of the regular context with a function called
         on ``object.__new__`` will be of type ``object``,
         which is incorrect for the argument in general.
         If no context is given the ``object.__new__`` call argument will
-        correctly inferred except when inside a call that requires
+        be correctly inferred except when inside a call that requires
         the additional context (such as a classmethod) of the boundnode
         to determine which class the method was called from
         """
 
-        # If we're unbound method __new__ of builtin object, the result is an
+        # If we're unbound method __new__ of a builtin, the result is an
         # instance of the class given as first argument.
-        if (
-            self._proxied.name == "__new__"
-            and self._proxied.parent.frame(future=True).qname() == "builtins.object"
-        ):
-            if caller.args:
-                node_context = context.extra_context.get(caller.args[0])
-                infer = caller.args[0].infer(context=node_context)
-            else:
-                infer = []
-            return (Instance(x) if x is not Uninferable else x for x in infer)
+        if self._proxied.name == "__new__":
+            qname = self._proxied.parent.frame(future=True).qname()
+            # Avoid checking builtins.type: _infer_type_new_call() does more validation
+            if qname.startswith("builtins.") and qname != "builtins.type":
+                return self._infer_builtin_new(caller, context)
         return self._proxied.infer_call_result(caller, context)
 
-    def bool_value(self, context=None):
+    def _infer_builtin_new(
+        self,
+        caller: nodes.Call,
+        context: InferenceContext,
+    ) -> collections.abc.Generator[
+        nodes.Const | Instance | UninferableBase, None, None
+    ]:
+        if not caller.args:
+            return
+        # Attempt to create a constant
+        if len(caller.args) > 1:
+            value = None
+            if isinstance(caller.args[1], nodes.Const):
+                value = caller.args[1].value
+            else:
+                inferred_arg = next(caller.args[1].infer(), None)
+                if isinstance(inferred_arg, nodes.Const):
+                    value = inferred_arg.value
+            if value is not None:
+                const = nodes.const_factory(value)
+                assert not isinstance(const, nodes.EmptyNode)
+                yield const
+                return
+
+        node_context = context.extra_context.get(caller.args[0])
+        for inferred in caller.args[0].infer(context=node_context):
+            if isinstance(inferred, UninferableBase):
+                yield inferred
+            if isinstance(inferred, nodes.ClassDef):
+                yield Instance(inferred)
+            raise InferenceError
+
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         return True
 
 
 class BoundMethod(UnboundMethod):
-    """a special node representing a method bound to an instance"""
+    """A special node representing a method bound to an instance."""
 
-    # pylint: disable=unnecessary-lambda
-    special_attributes = lazy_descriptor(lambda: objectmodel.BoundMethodModel())
+    special_attributes = objectmodel.BoundMethodModel()
 
     def __init__(self, proxy, bound):
         super().__init__(proxy)
         self.bound = bound
 
-    def implicit_parameters(self):
+    def implicit_parameters(self) -> Literal[0, 1]:
         if self.name == "__new__":
             # __new__ acts as a classmethod but the class argument is not implicit.
             return 0
         return 1
 
-    def is_bound(self):
+    def is_bound(self) -> Literal[True]:
         return True
 
-    def _infer_type_new_call(self, caller, context):
+    def _infer_type_new_call(self, caller, context):  # noqa: C901
         """Try to infer what type.__new__(mcs, name, bases, attrs) returns.
 
         In order for such call to be valid, the metaclass needs to be
         a subtype of ``type``, the name needs to be a string, the bases
         needs to be a tuple of classes
         """
         # pylint: disable=import-outside-toplevel; circular import
@@ -512,89 +595,144 @@
 
         # Build the class from now.
         cls = mcs.__class__(
             name=name.value,
             lineno=caller.lineno,
             col_offset=caller.col_offset,
             parent=caller,
+            end_lineno=caller.end_lineno,
+            end_col_offset=caller.end_col_offset,
+        )
+        empty = Pass(
+            parent=cls,
+            lineno=caller.lineno,
+            col_offset=caller.col_offset,
+            end_lineno=caller.end_lineno,
+            end_col_offset=caller.end_col_offset,
         )
-        empty = Pass()
         cls.postinit(
             bases=bases.elts,
             body=[empty],
             decorators=[],
             newstyle=True,
             metaclass=mcs,
             keywords=[],
         )
         cls.locals = cls_locals
         return cls
 
-    def infer_call_result(self, caller, context=None):
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
         context = bind_context_to_node(context, self.bound)
         if (
             self.bound.__class__.__name__ == "ClassDef"
             and self.bound.name == "type"
             and self.name == "__new__"
             and len(caller.args) == 4
         ):
             # Check if we have a ``type.__new__(mcs, name, bases, attrs)`` call.
             new_cls = self._infer_type_new_call(caller, context)
             if new_cls:
                 return iter((new_cls,))
 
         return super().infer_call_result(caller, context)
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         return True
 
 
 class Generator(BaseInstance):
-    """a special node representing a generator.
+    """A special node representing a generator.
 
     Proxied class is set once for all in raw_building.
     """
 
-    special_attributes = lazy_descriptor(objectmodel.GeneratorModel)
-
-    def __init__(self, parent=None, generator_initial_context=None):
+    # We defer initialization of special_attributes to the __init__ method since the constructor
+    # of GeneratorModel requires the raw_building to be complete
+    # TODO: This should probably be refactored.
+    special_attributes: objectmodel.GeneratorModel
+
+    def __init__(
+        self, parent=None, generator_initial_context: InferenceContext | None = None
+    ):
         super().__init__()
         self.parent = parent
         self._call_context = copy_context(generator_initial_context)
 
-    @decorators.cached
+        # See comment above: this is a deferred initialization.
+        Generator.special_attributes = objectmodel.GeneratorModel()
+
     def infer_yield_types(self):
         yield from self.parent.infer_yield_result(self._call_context)
 
-    def callable(self):
+    def callable(self) -> Literal[False]:
         return False
 
-    def pytype(self):
+    def pytype(self) -> str:
         return "builtins.generator"
 
-    def display_type(self):
+    def display_type(self) -> str:
         return "Generator"
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         return True
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<Generator({self._proxied.name}) l.{self.lineno} at 0x{id(self)}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Generator({self._proxied.name})"
 
 
 class AsyncGenerator(Generator):
-    """Special node representing an async generator"""
+    """Special node representing an async generator."""
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.async_generator"]:
         return "builtins.async_generator"
 
-    def display_type(self):
+    def display_type(self) -> str:
         return "AsyncGenerator"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<AsyncGenerator({self._proxied.name}) l.{self.lineno} at 0x{id(self)}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"AsyncGenerator({self._proxied.name})"
+
+
+class UnionType(BaseInstance):
+    """Special node representing new style typing unions.
+
+    Proxied class is set once for all in raw_building.
+    """
+
+    def __init__(
+        self,
+        left: UnionType | nodes.ClassDef | nodes.Const,
+        right: UnionType | nodes.ClassDef | nodes.Const,
+        parent: nodes.NodeNG | None = None,
+    ) -> None:
+        super().__init__()
+        self.parent = parent
+        self.left = left
+        self.right = right
+
+    def callable(self) -> Literal[False]:
+        return False
+
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
+        return True
+
+    def pytype(self) -> Literal["types.UnionType"]:
+        return "types.UnionType"
+
+    def display_type(self) -> str:
+        return "UnionType"
+
+    def __repr__(self) -> str:
+        return f"<UnionType({self._proxied.name}) l.{self.lineno} at 0x{id(self)}>"
+
+    def __str__(self) -> str:
+        return f"UnionType({self._proxied.name})"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_attrs.py` & `astroid-3.0.0a1/astroid/brain/brain_attrs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """
 Astroid hook for the attrs library
 
 Without this hook pylint reports unsupported-assignment-operation
 for attrs classes
 """
+from astroid.helpers import safe_infer
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import AnnAssign, Assign, AssignName, Call, Unknown
 from astroid.nodes.scoped_nodes import ClassDef
 
-ATTRIB_NAMES = frozenset(("attr.ib", "attrib", "attr.attrib", "attr.field", "field"))
+ATTRIB_NAMES = frozenset(
+    (
+        "attr.Factory",
+        "attr.ib",
+        "attrib",
+        "attr.attrib",
+        "attr.field",
+        "attrs.field",
+        "field",
+    )
+)
 ATTRS_NAMES = frozenset(
     (
         "attr.s",
         "attrs",
         "attr.attrs",
         "attr.attributes",
         "attr.define",
         "attr.mutable",
         "attr.frozen",
+        "attrs.define",
+        "attrs.mutable",
+        "attrs.frozen",
     )
 )
 
 
-def is_decorated_with_attrs(node, decorator_names=ATTRS_NAMES):
-    """Return True if a decorated node has
-    an attr decorator applied."""
+def is_decorated_with_attrs(node, decorator_names=ATTRS_NAMES) -> bool:
+    """Return whether a decorated node has an attr decorator applied."""
     if not node.decorators:
         return False
     for decorator_attribute in node.decorators.nodes:
         if isinstance(decorator_attribute, Call):  # decorator with arguments
             decorator_attribute = decorator_attribute.func
         if decorator_attribute.as_string() in decorator_names:
             return True
+
+        inferred = safe_infer(decorator_attribute)
+        if inferred and inferred.root().name == "attr._next_gen":
+            return True
     return False
 
 
 def attr_attributes_transform(node: ClassDef) -> None:
     """Given that the ClassNode has an attr decorator,
     rewrite class attributes as instance attributes
     """
     # Astroid can't infer this attribute properly
-    # Prevents https://github.com/PyCQA/pylint/issues/1884
+    # Prevents https://github.com/pylint-dev/pylint/issues/1884
     node.locals["__attrs_attrs__"] = [Unknown(parent=node)]
 
     for cdef_body_node in node.body:
         if not isinstance(cdef_body_node, (Assign, AnnAssign)):
             continue
         if isinstance(cdef_body_node.value, Call):
             if cdef_body_node.value.func.as_string() not in ATTRIB_NAMES:
@@ -63,15 +82,15 @@
                 lineno=cdef_body_node.lineno,
                 col_offset=cdef_body_node.col_offset,
                 parent=cdef_body_node,
             )
             if isinstance(target, AssignName):
                 # Could be a subscript if the code analysed is
                 # i = Optional[str] = ""
-                # See https://github.com/PyCQA/pylint/issues/4439
+                # See https://github.com/pylint-dev/pylint/issues/4439
                 node.locals[target.name] = [rhs_node]
                 node.instance_attrs[target.name] = [rhs_node]
 
 
 AstroidManager().register_transform(
     ClassDef, attr_attributes_transform, is_decorated_with_attrs
 )
```

### Comparing `astroid-2.9.3/astroid/brain/brain_boto3.py` & `astroid-3.0.0a1/astroid/brain/brain_boto3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+"""Astroid hooks for understanding ``boto3.ServiceRequest()``."""
 
-"""Astroid hooks for understanding boto3.ServiceRequest()"""
 from astroid import extract_node
 from astroid.manager import AstroidManager
 from astroid.nodes.scoped_nodes import ClassDef
 
 BOTO_SERVICE_FACTORY_QUALIFIED_NAME = "boto3.resources.base.ServiceResource"
 
 
 def service_request_transform(node):
-    """Transform ServiceResource to look like dynamic classes"""
+    """Transform ServiceResource to look like dynamic classes."""
     code = """
     def __getattr__(self, attr):
         return 0
     """
     func_getattr = extract_node(code)
     node.locals["__getattr__"] = [func_getattr]
     return node
 
 
-def _looks_like_boto3_service_request(node):
+def _looks_like_boto3_service_request(node) -> bool:
     return node.qname() == BOTO_SERVICE_FACTORY_QUALIFIED_NAME
 
 
 AstroidManager().register_transform(
     ClassDef, service_request_transform, _looks_like_boto3_service_request
 )
```

### Comparing `astroid-2.9.3/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a1/astroid/brain/brain_builtin_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-# Copyright (c) 2014-2021 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014-2015 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Rene Zhang <rz99@cornell.edu>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2019-2020 Bryce Guinta <bryce.guinta@protonmail.com>
-# Copyright (c) 2019 Stanislav Levin <slev@altlinux.org>
-# Copyright (c) 2019 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2019 Frédéric Chapoton <fchapoton2@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 David Gilman <davidgilman1@gmail.com>
-# Copyright (c) 2020 Ram Rachum <ram@rachum.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for various builtins."""
 
+from __future__ import annotations
+
+import itertools
+from collections.abc import Iterator
 from functools import partial
 
 from astroid import arguments, helpers, inference_tip, nodes, objects, util
 from astroid.builder import AstroidBuilder
+from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     UseInferenceDefault,
 )
@@ -116,15 +104,15 @@
         return {rvalue}
     def ljust(self, width, fillchar=None):
         return {rvalue}
 """
 
 
 def _extend_string_class(class_node, code, rvalue):
-    """function to extend builtin str/unicode class"""
+    """Function to extend builtin str/unicode class."""
     code = code.format(rvalue=rvalue)
     fake = AstroidBuilder(AstroidManager()).string_build(code)["whatever"]
     for method in fake.mymethods():
         method.parent = class_node
         method.lineno = None
         method.col_offset = None
         if "__class__" in method.locals:
@@ -143,15 +131,15 @@
     {
         "bytes": partial(_extend_string_class, code=BYTES_CLASS, rvalue="b''"),
         "str": partial(_extend_string_class, code=STR_CLASS, rvalue="''"),
     }
 )
 
 
-def _builtin_filter_predicate(node, builtin_name):
+def _builtin_filter_predicate(node, builtin_name) -> bool:
     if (
         builtin_name == "type"
         and node.root().name == "re"
         and isinstance(node.func, nodes.Name)
         and node.func.name == "type"
         and isinstance(node.parent, nodes.Assign)
         and len(node.parent.targets) == 1
@@ -172,33 +160,33 @@
             node.func.attrname == "fromkeys"
             and isinstance(node.func.expr, nodes.Name)
             and node.func.expr.name == "dict"
         )
     return False
 
 
-def register_builtin_transform(transform, builtin_name):
+def register_builtin_transform(transform, builtin_name) -> None:
     """Register a new transform function for the given *builtin_name*.
 
     The transform function must accept two parameters, a node and
     an optional context.
     """
 
-    def _transform_wrapper(node, context=None):
+    def _transform_wrapper(node, context: InferenceContext | None = None):
         result = transform(node, context=context)
         if result:
             if not result.parent:
                 # Let the transformation function determine
                 # the parent for its result. Otherwise,
                 # we set it to be the node we transformed from.
                 result.parent = node
 
             if result.lineno is None:
                 result.lineno = node.lineno
-            # Can be a 'Module' see https://github.com/PyCQA/pylint/issues/4671
+            # Can be a 'Module' see https://github.com/pylint-dev/pylint/issues/4671
             # We don't have a regression test on this one: tread carefully
             if hasattr(result, "col_offset") and result.col_offset is None:
                 result.col_offset = node.col_offset
         return iter([result])
 
     AstroidManager().register_transform(
         nodes.Call,
@@ -217,18 +205,18 @@
     (arg,) = args
     transformed = transform(arg)
     if not transformed:
         try:
             inferred = next(arg.infer(context=context))
         except (InferenceError, StopIteration) as exc:
             raise UseInferenceDefault from exc
-        if inferred is util.Uninferable:
+        if isinstance(inferred, util.UninferableBase):
             raise UseInferenceDefault
         transformed = transform(inferred)
-    if not transformed or transformed is util.Uninferable:
+    if not transformed or isinstance(transformed, util.UninferableBase):
         raise UseInferenceDefault
     return transformed
 
 
 def _container_generic_transform(  # pylint: disable=inconsistent-return-statements
     arg, context, klass, iterables, build_elts
 ):
@@ -344,15 +332,15 @@
                 raise UseInferenceDefault()
             items.append(tuple(elt.elts))
     else:
         raise UseInferenceDefault()
     return items
 
 
-def infer_dict(node, context=None):
+def infer_dict(node, context: InferenceContext | None = None):
     """Try to infer a dict call to a Dict node.
 
     The function treats the following cases:
 
         * dict()
         * dict(mapping)
         * dict(iterable)
@@ -387,15 +375,17 @@
     value = nodes.Dict(
         col_offset=node.col_offset, lineno=node.lineno, parent=node.parent
     )
     value.postinit(items)
     return value
 
 
-def infer_super(node, context=None):
+def infer_super(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> objects.Super:
     """Understand super calls.
 
     There are some restrictions for what can be understood:
 
         * unbounded super (one argument form) is not understood.
 
         * if the super call is not inside a function (classmethod or method),
@@ -413,14 +403,15 @@
         # Ignore non-method uses of super.
         raise UseInferenceDefault
     if scope.type not in ("classmethod", "method"):
         # Not interested in staticmethods.
         raise UseInferenceDefault
 
     cls = scoped_nodes.get_wrapping_class(scope)
+    assert cls is not None
     if not node.args:
         mro_pointer = cls
         # In we are in a classmethod, the interpreter will fill
         # automatically the class as the second argument, not an instance.
         if scope.type == "classmethod":
             mro_type = cls
         else:
@@ -431,20 +422,26 @@
         except (InferenceError, StopIteration) as exc:
             raise UseInferenceDefault from exc
         try:
             mro_type = next(node.args[1].infer(context=context))
         except (InferenceError, StopIteration) as exc:
             raise UseInferenceDefault from exc
 
-    if mro_pointer is util.Uninferable or mro_type is util.Uninferable:
+    if isinstance(mro_pointer, util.UninferableBase) or isinstance(
+        mro_type, util.UninferableBase
+    ):
         # No way we could understand this.
         raise UseInferenceDefault
 
     super_obj = objects.Super(
-        mro_pointer=mro_pointer, mro_type=mro_type, self_class=cls, scope=scope
+        mro_pointer=mro_pointer,
+        mro_type=mro_type,
+        self_class=cls,
+        scope=scope,
+        call=node,
     )
     super_obj.parent = node
     return super_obj
 
 
 def _infer_getattr_args(node, context):
     if len(node.args) not in (2, 3):
@@ -453,38 +450,38 @@
 
     try:
         obj = next(node.args[0].infer(context=context))
         attr = next(node.args[1].infer(context=context))
     except (InferenceError, StopIteration) as exc:
         raise UseInferenceDefault from exc
 
-    if obj is util.Uninferable or attr is util.Uninferable:
+    if isinstance(obj, util.UninferableBase) or isinstance(attr, util.UninferableBase):
         # If one of the arguments is something we can't infer,
         # then also make the result of the getattr call something
         # which is unknown.
         return util.Uninferable, util.Uninferable
 
     is_string = isinstance(attr, nodes.Const) and isinstance(attr.value, str)
     if not is_string:
         raise UseInferenceDefault
 
     return obj, attr.value
 
 
-def infer_getattr(node, context=None):
-    """Understand getattr calls
+def infer_getattr(node, context: InferenceContext | None = None):
+    """Understand getattr calls.
 
     If one of the arguments is an Uninferable object, then the
     result will be an Uninferable object. Otherwise, the normal attribute
     lookup will be done.
     """
     obj, attr = _infer_getattr_args(node, context)
     if (
-        obj is util.Uninferable
-        or attr is util.Uninferable
+        isinstance(obj, util.UninferableBase)
+        or isinstance(attr, util.UninferableBase)
         or not hasattr(obj, "igetattr")
     ):
         return util.Uninferable
 
     try:
         return next(obj.igetattr(attr, context=context))
     except (StopIteration, InferenceError, AttributeInferenceError):
@@ -494,43 +491,43 @@
                 return next(node.args[2].infer(context=context))
             except (StopIteration, InferenceError) as exc:
                 raise UseInferenceDefault from exc
 
     raise UseInferenceDefault
 
 
-def infer_hasattr(node, context=None):
-    """Understand hasattr calls
+def infer_hasattr(node, context: InferenceContext | None = None):
+    """Understand hasattr calls.
 
     This always guarantees three possible outcomes for calling
     hasattr: Const(False) when we are sure that the object
     doesn't have the intended attribute, Const(True) when
     we know that the object has the attribute and Uninferable
     when we are unsure of the outcome of the function call.
     """
     try:
         obj, attr = _infer_getattr_args(node, context)
         if (
-            obj is util.Uninferable
-            or attr is util.Uninferable
+            isinstance(obj, util.UninferableBase)
+            or isinstance(attr, util.UninferableBase)
             or not hasattr(obj, "getattr")
         ):
             return util.Uninferable
         obj.getattr(attr, context=context)
     except UseInferenceDefault:
         # Can't infer something from this function call.
         return util.Uninferable
     except AttributeInferenceError:
         # Doesn't have it.
         return nodes.Const(False)
     return nodes.Const(True)
 
 
-def infer_callable(node, context=None):
-    """Understand callable calls
+def infer_callable(node, context: InferenceContext | None = None):
+    """Understand callable calls.
 
     This follows Python's semantics, where an object
     is callable if it provides an attribute __call__,
     even though that attribute is something which can't be
     called.
     """
     if len(node.args) != 1:
@@ -538,21 +535,23 @@
         raise UseInferenceDefault
 
     argument = node.args[0]
     try:
         inferred = next(argument.infer(context=context))
     except (InferenceError, StopIteration):
         return util.Uninferable
-    if inferred is util.Uninferable:
+    if isinstance(inferred, util.UninferableBase):
         return util.Uninferable
     return nodes.Const(inferred.callable())
 
 
-def infer_property(node, context=None):
-    """Understand `property` class
+def infer_property(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> objects.Property:
+    """Understand `property` class.
 
     This only infers the output of `property`
     call, not the arguments themselves.
     """
     if len(node.args) < 1:
         # Invalid property call.
         raise UseInferenceDefault
@@ -562,105 +561,115 @@
         inferred = next(getter.infer(context=context))
     except (InferenceError, StopIteration) as exc:
         raise UseInferenceDefault from exc
 
     if not isinstance(inferred, (nodes.FunctionDef, nodes.Lambda)):
         raise UseInferenceDefault
 
-    return objects.Property(
+    prop_func = objects.Property(
         function=inferred,
         name=inferred.name,
-        doc=getattr(inferred, "doc", None),
         lineno=node.lineno,
-        parent=node,
         col_offset=node.col_offset,
     )
+    # Set parent outside __init__: https://github.com/pylint-dev/astroid/issues/1490
+    prop_func.parent = node
+    prop_func.postinit(
+        body=[],
+        args=inferred.args,
+        doc_node=getattr(inferred, "doc_node", None),
+    )
+    return prop_func
 
 
-def infer_bool(node, context=None):
+def infer_bool(node, context: InferenceContext | None = None):
     """Understand bool calls."""
     if len(node.args) > 1:
         # Invalid bool call.
         raise UseInferenceDefault
 
     if not node.args:
         return nodes.Const(False)
 
     argument = node.args[0]
     try:
         inferred = next(argument.infer(context=context))
     except (InferenceError, StopIteration):
         return util.Uninferable
-    if inferred is util.Uninferable:
+    if isinstance(inferred, util.UninferableBase):
         return util.Uninferable
 
     bool_value = inferred.bool_value(context=context)
-    if bool_value is util.Uninferable:
+    if isinstance(bool_value, util.UninferableBase):
         return util.Uninferable
     return nodes.Const(bool_value)
 
 
-def infer_type(node, context=None):
+def infer_type(node, context: InferenceContext | None = None):
     """Understand the one-argument form of *type*."""
     if len(node.args) != 1:
         raise UseInferenceDefault
 
     return helpers.object_type(node.args[0], context)
 
 
-def infer_slice(node, context=None):
+def infer_slice(node, context: InferenceContext | None = None):
     """Understand `slice` calls."""
     args = node.args
     if not 0 < len(args) <= 3:
         raise UseInferenceDefault
 
     infer_func = partial(helpers.safe_infer, context=context)
     args = [infer_func(arg) for arg in args]
     for arg in args:
-        if not arg or arg is util.Uninferable:
+        if not arg or isinstance(arg, util.UninferableBase):
             raise UseInferenceDefault
         if not isinstance(arg, nodes.Const):
             raise UseInferenceDefault
         if not isinstance(arg.value, (type(None), int)):
             raise UseInferenceDefault
 
     if len(args) < 3:
         # Make sure we have 3 arguments.
         args.extend([None] * (3 - len(args)))
 
     slice_node = nodes.Slice(
-        lineno=node.lineno, col_offset=node.col_offset, parent=node.parent
+        lineno=node.lineno,
+        col_offset=node.col_offset,
+        parent=node.parent,
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
     )
     slice_node.postinit(*args)
     return slice_node
 
 
-def _infer_object__new__decorator(node, context=None):
+def _infer_object__new__decorator(node, context: InferenceContext | None = None):
     # Instantiate class immediately
     # since that's what @object.__new__ does
     return iter((node.instantiate_class(),))
 
 
-def _infer_object__new__decorator_check(node):
-    """Predicate before inference_tip
+def _infer_object__new__decorator_check(node) -> bool:
+    """Predicate before inference_tip.
 
     Check if the given ClassDef has an @object.__new__ decorator
     """
     if not node.decorators:
         return False
 
     for decorator in node.decorators.nodes:
         if isinstance(decorator, nodes.Attribute):
             if decorator.as_string() == OBJECT_DUNDER_NEW:
                 return True
     return False
 
 
-def infer_issubclass(callnode, context=None):
-    """Infer issubclass() calls
+def infer_issubclass(callnode, context: InferenceContext | None = None):
+    """Infer issubclass() calls.
 
     :param nodes.Call callnode: an `issubclass` call
     :param InferenceContext context: the context for the inference
     :rtype nodes.Const: Boolean Const value of the `issubclass` call
     :raises UseInferenceDefault: If the node cannot be inferred
     """
     call = arguments.CallSite.from_call(callnode, context=context)
@@ -694,20 +703,18 @@
     except AstroidTypeError as exc:
         raise UseInferenceDefault("TypeError: " + str(exc)) from exc
     except MroError as exc:
         raise UseInferenceDefault from exc
     return nodes.Const(issubclass_bool)
 
 
-def infer_isinstance(callnode, context=None):
-    """Infer isinstance calls
+def infer_isinstance(callnode, context: InferenceContext | None = None):
+    """Infer isinstance calls.
 
     :param nodes.Call callnode: an isinstance call
-    :param InferenceContext context: context for call
-        (currently unused but is a common interface for inference)
     :rtype nodes.Const: Boolean Const value of isinstance call
 
     :raises UseInferenceDefault: If the node cannot be inferred
     """
     call = arguments.CallSite.from_call(callnode, context=context)
     if call.keyword_arguments:
         # isinstance doesn't support keyword arguments
@@ -728,20 +735,20 @@
         raise UseInferenceDefault from exc
     try:
         isinstance_bool = helpers.object_isinstance(obj_node, class_container, context)
     except AstroidTypeError as exc:
         raise UseInferenceDefault("TypeError: " + str(exc)) from exc
     except MroError as exc:
         raise UseInferenceDefault from exc
-    if isinstance_bool is util.Uninferable:
+    if isinstance(isinstance_bool, util.UninferableBase):
         raise UseInferenceDefault
     return nodes.Const(isinstance_bool)
 
 
-def _class_or_tuple_to_container(node, context=None):
+def _class_or_tuple_to_container(node, context: InferenceContext | None = None):
     # Move inferences results into container
     # to simplify later logic
     # raises InferenceError if any of the inferences fall through
     try:
         node_infer = next(node.infer(context=context))
     except StopIteration as e:
         raise InferenceError(node=node, context=context) from e
@@ -758,16 +765,16 @@
             klass_node for klass_node in class_container if klass_node is not None
         ]
     else:
         class_container = [node_infer]
     return class_container
 
 
-def infer_len(node, context=None):
-    """Infer length calls
+def infer_len(node, context: InferenceContext | None = None):
+    """Infer length calls.
 
     :param nodes.Call node: len call to infer
     :param context.InferenceContext: node context
     :rtype nodes.Const: a Const node with the inferred length, if possible
     """
     call = arguments.CallSite.from_call(node, context=context)
     if call.keyword_arguments:
@@ -781,32 +788,32 @@
 
     try:
         return nodes.Const(helpers.object_len(argument_node, context=context))
     except (AstroidTypeError, InferenceError) as exc:
         raise UseInferenceDefault(str(exc)) from exc
 
 
-def infer_str(node, context=None):
-    """Infer str() calls
+def infer_str(node, context: InferenceContext | None = None):
+    """Infer str() calls.
 
     :param nodes.Call node: str() call to infer
     :param context.InferenceContext: node context
     :rtype nodes.Const: a Const containing an empty string
     """
     call = arguments.CallSite.from_call(node, context=context)
     if call.keyword_arguments:
         raise UseInferenceDefault("TypeError: str() must take no keyword arguments")
     try:
         return nodes.Const("")
     except (AstroidTypeError, InferenceError) as exc:
         raise UseInferenceDefault(str(exc)) from exc
 
 
-def infer_int(node, context=None):
-    """Infer int() calls
+def infer_int(node, context: InferenceContext | None = None):
+    """Infer int() calls.
 
     :param nodes.Call node: int() call to infer
     :param context.InferenceContext: node context
     :rtype nodes.Const: a Const containing the integer value of the int() call
     """
     call = arguments.CallSite.from_call(node, context=context)
     if call.keyword_arguments:
@@ -814,31 +821,31 @@
 
     if call.positional_arguments:
         try:
             first_value = next(call.positional_arguments[0].infer(context=context))
         except (InferenceError, StopIteration) as exc:
             raise UseInferenceDefault(str(exc)) from exc
 
-        if first_value is util.Uninferable:
+        if isinstance(first_value, util.UninferableBase):
             raise UseInferenceDefault
 
         if isinstance(first_value, nodes.Const) and isinstance(
             first_value.value, (int, str)
         ):
             try:
                 actual_value = int(first_value.value)
             except ValueError:
                 return nodes.Const(0)
             return nodes.Const(actual_value)
 
     return nodes.Const(0)
 
 
-def infer_dict_fromkeys(node, context=None):
-    """Infer dict.fromkeys
+def infer_dict_fromkeys(node, context: InferenceContext | None = None):
+    """Infer dict.fromkeys.
 
     :param nodes.Call node: dict.fromkeys() call to infer
     :param context.InferenceContext context: node context
     :rtype nodes.Dict:
         a Dictionary containing the values that astroid was able to infer.
         In case the inference failed for any reason, an empty dictionary
         will be inferred instead.
@@ -896,14 +903,85 @@
         elements_with_value = [(element, default) for element in keys]
         return _build_dict_with_elements(elements_with_value)
 
     # Fallback to an empty dictionary
     return _build_dict_with_elements([])
 
 
+def _infer_copy_method(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[nodes.NodeNG]:
+    assert isinstance(node.func, nodes.Attribute)
+    inferred_orig, inferred_copy = itertools.tee(node.func.expr.infer(context=context))
+    if all(
+        isinstance(
+            inferred_node, (nodes.Dict, nodes.List, nodes.Set, objects.FrozenSet)
+        )
+        for inferred_node in inferred_orig
+    ):
+        return inferred_copy
+
+    raise UseInferenceDefault()
+
+
+def _is_str_format_call(node: nodes.Call) -> bool:
+    """Catch calls to str.format()."""
+    if not isinstance(node.func, nodes.Attribute) or not node.func.attrname == "format":
+        return False
+
+    if isinstance(node.func.expr, nodes.Name):
+        value = helpers.safe_infer(node.func.expr)
+    else:
+        value = node.func.expr
+
+    return isinstance(value, nodes.Const) and isinstance(value.value, str)
+
+
+def _infer_str_format_call(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[nodes.Const | util.UninferableBase]:
+    """Return a Const node based on the template and passed arguments."""
+    call = arguments.CallSite.from_call(node, context=context)
+    if isinstance(node.func.expr, nodes.Name):
+        value: nodes.Const | None = helpers.safe_infer(node.func.expr)
+        if value is None:
+            return iter([util.Uninferable])
+    else:
+        value = node.func.expr
+
+    format_template = value.value
+
+    # Get the positional arguments passed
+    inferred_positional = [
+        helpers.safe_infer(i, context) for i in call.positional_arguments
+    ]
+    if not all(isinstance(i, nodes.Const) for i in inferred_positional):
+        return iter([util.Uninferable])
+    pos_values: list[str] = [i.value for i in inferred_positional]
+
+    # Get the keyword arguments passed
+    inferred_keyword = {
+        k: helpers.safe_infer(v, context) for k, v in call.keyword_arguments.items()
+    }
+    if not all(isinstance(i, nodes.Const) for i in inferred_keyword.values()):
+        return iter([util.Uninferable])
+    keyword_values: dict[str, str] = {k: v.value for k, v in inferred_keyword.items()}
+
+    try:
+        formatted_string = format_template.format(*pos_values, **keyword_values)
+    except (AttributeError, IndexError, KeyError, TypeError, ValueError):
+        # AttributeError: named field in format string was not found in the arguments
+        # IndexError: there are too few arguments to interpolate
+        # TypeError: Unsupported format string
+        # ValueError: Unknown format code
+        return iter([util.Uninferable])
+
+    return iter([nodes.const_factory(formatted_string)])
+
+
 # Builtins inference
 register_builtin_transform(infer_bool, "bool")
 register_builtin_transform(infer_super, "super")
 register_builtin_transform(infer_callable, "callable")
 register_builtin_transform(infer_property, "property")
 register_builtin_transform(infer_getattr, "getattr")
 register_builtin_transform(infer_hasattr, "hasattr")
@@ -924,7 +1002,18 @@
 
 # Infer object.__new__ calls
 AstroidManager().register_transform(
     nodes.ClassDef,
     inference_tip(_infer_object__new__decorator),
     _infer_object__new__decorator_check,
 )
+
+AstroidManager().register_transform(
+    nodes.Call,
+    inference_tip(_infer_copy_method),
+    lambda node: isinstance(node.func, nodes.Attribute)
+    and node.func.attrname == "copy",
+)
+
+AstroidManager().register_transform(
+    nodes.Call, inference_tip(_infer_str_format_call), _is_str_format_call
+)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_collections.py` & `astroid-3.0.0a1/astroid/brain/brain_collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-# Copyright (c) 2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016-2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2018 Ioana Tagirta <ioana.tagirta@gmail.com>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 John Belmonte <john@neggie.net>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
 
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import extract_node, parse
 from astroid.const import PY39_PLUS
+from astroid.context import InferenceContext
 from astroid.exceptions import AttributeInferenceError
 from astroid.manager import AstroidManager
 from astroid.nodes.scoped_nodes import ClassDef
 
 
 def _collections_transform():
     return parse(
@@ -88,16 +82,16 @@
 
 
 register_module_extender(AstroidManager(), "collections", _collections_transform)
 
 
 def _looks_like_subscriptable(node: ClassDef) -> bool:
     """
-    Returns True if the node corresponds to a ClassDef of the Collections.abc module that
-    supports subscripting
+    Returns True if the node corresponds to a ClassDef of the Collections.abc module
+    that supports subscripting.
 
     :param node: ClassDef node
     """
     if node.qname().startswith("_collections") or node.qname().startswith(
         "collections"
     ):
         try:
@@ -111,15 +105,15 @@
 CLASS_GET_ITEM_TEMPLATE = """
 @classmethod
 def __class_getitem__(cls, item):
     return cls
 """
 
 
-def easy_class_getitem_inference(node, context=None):
+def easy_class_getitem_inference(node, context: InferenceContext | None = None):
     # Here __class_getitem__ exists but is quite a mess to infer thus
     # put an easy inference tip
     func_to_add = extract_node(CLASS_GET_ITEM_TEMPLATE)
     node.locals["__class_getitem__"] = [func_to_add]
 
 
 if PY39_PLUS:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_curses.py` & `astroid-3.0.0a1/astroid/brain/brain_curses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.manager import AstroidManager
 
 
 def _curses_transform():
     return parse(
```

### Comparing `astroid-2.9.3/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a1/astroid/brain/brain_typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,464 +1,441 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-"""
-Astroid hook for the dataclasses library
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-Support built-in dataclasses, pydantic.dataclasses, and marshmallow_dataclass-annotated
-dataclasses. References:
-- https://docs.python.org/3/library/dataclasses.html
-- https://pydantic-docs.helpmanual.io/usage/dataclasses/
-- https://lovasoa.github.io/marshmallow_dataclass/
+"""Astroid hooks for typing.py support."""
 
-"""
-import sys
-from typing import FrozenSet, Generator, List, Optional, Tuple, Union
+from __future__ import annotations
+
+import typing
+from collections.abc import Iterator
+from functools import partial
+from typing import Final
 
-from astroid import context, inference_tip
-from astroid.builder import parse
-from astroid.const import PY37_PLUS, PY39_PLUS
+from astroid import context, extract_node, inference_tip
+from astroid.builder import _extract_single_node
+from astroid.const import PY39_PLUS
 from astroid.exceptions import (
-    AstroidSyntaxError,
+    AttributeInferenceError,
     InferenceError,
-    MroError,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import (
-    AnnAssign,
     Assign,
     AssignName,
     Attribute,
     Call,
+    Const,
+    JoinedStr,
     Name,
     NodeNG,
     Subscript,
-    Unknown,
+    Tuple,
 )
 from astroid.nodes.scoped_nodes import ClassDef, FunctionDef
-from astroid.util import Uninferable
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+TYPING_TYPEVARS = {"TypeVar", "NewType"}
+TYPING_TYPEVARS_QUALIFIED: Final = {
+    "typing.TypeVar",
+    "typing.NewType",
+    "typing_extensions.TypeVar",
+}
+TYPING_TYPEDDICT_QUALIFIED: Final = {"typing.TypedDict", "typing_extensions.TypedDict"}
+TYPING_TYPE_TEMPLATE = """
+class Meta(type):
+    def __getitem__(self, item):
+        return self
+
+    @property
+    def __args__(self):
+        return ()
 
-_FieldDefaultReturn = Union[
-    None, Tuple[Literal["default"], NodeNG], Tuple[Literal["default_factory"], Call]
-]
-
-DATACLASSES_DECORATORS = frozenset(("dataclass",))
-FIELD_NAME = "field"
-DATACLASS_MODULES = frozenset(
-    ("dataclasses", "marshmallow_dataclass", "pydantic.dataclasses")
-)
-DEFAULT_FACTORY = "_HAS_DEFAULT_FACTORY"  # based on typing.py
-
-
-def is_decorated_with_dataclass(node, decorator_names=DATACLASSES_DECORATORS):
-    """Return True if a decorated node has a `dataclass` decorator applied."""
-    if not isinstance(node, ClassDef) or not node.decorators:
-        return False
+class {0}(metaclass=Meta):
+    pass
+"""
+TYPING_MEMBERS = set(getattr(typing, "__all__", []))
 
-    return any(
-        _looks_like_dataclass_decorator(decorator_attribute, decorator_names)
-        for decorator_attribute in node.decorators.nodes
+TYPING_ALIAS = frozenset(
+    (
+        "typing.Hashable",
+        "typing.Awaitable",
+        "typing.Coroutine",
+        "typing.AsyncIterable",
+        "typing.AsyncIterator",
+        "typing.Iterable",
+        "typing.Iterator",
+        "typing.Reversible",
+        "typing.Sized",
+        "typing.Container",
+        "typing.Collection",
+        "typing.Callable",
+        "typing.AbstractSet",
+        "typing.MutableSet",
+        "typing.Mapping",
+        "typing.MutableMapping",
+        "typing.Sequence",
+        "typing.MutableSequence",
+        "typing.ByteString",
+        "typing.Tuple",
+        "typing.List",
+        "typing.Deque",
+        "typing.Set",
+        "typing.FrozenSet",
+        "typing.MappingView",
+        "typing.KeysView",
+        "typing.ItemsView",
+        "typing.ValuesView",
+        "typing.ContextManager",
+        "typing.AsyncContextManager",
+        "typing.Dict",
+        "typing.DefaultDict",
+        "typing.OrderedDict",
+        "typing.Counter",
+        "typing.ChainMap",
+        "typing.Generator",
+        "typing.AsyncGenerator",
+        "typing.Type",
+        "typing.Pattern",
+        "typing.Match",
     )
+)
 
+CLASS_GETITEM_TEMPLATE = """
+@classmethod
+def __class_getitem__(cls, item):
+    return cls
+"""
 
-def dataclass_transform(node: ClassDef) -> None:
-    """Rewrite a dataclass to be easily understood by pylint"""
 
-    for assign_node in _get_dataclass_attributes(node):
-        name = assign_node.target.name
+def looks_like_typing_typevar_or_newtype(node) -> bool:
+    func = node.func
+    if isinstance(func, Attribute):
+        return func.attrname in TYPING_TYPEVARS
+    if isinstance(func, Name):
+        return func.name in TYPING_TYPEVARS
+    return False
 
-        rhs_node = Unknown(
-            lineno=assign_node.lineno,
-            col_offset=assign_node.col_offset,
-            parent=assign_node,
-        )
-        rhs_node = AstroidManager().visit_transforms(rhs_node)
-        node.instance_attrs[name] = [rhs_node]
-
-    if not _check_generate_dataclass_init(node):
-        return
 
+def infer_typing_typevar_or_newtype(node, context_itton=None):
+    """Infer a typing.TypeVar(...) or typing.NewType(...) call."""
     try:
-        reversed_mro = list(reversed(node.mro()))
-    except MroError:
-        reversed_mro = [node]
-
-    field_assigns = {}
-    field_order = []
-    for klass in (k for k in reversed_mro if is_decorated_with_dataclass(k)):
-        for assign_node in _get_dataclass_attributes(klass, init=True):
-            name = assign_node.target.name
-            if name not in field_assigns:
-                field_order.append(name)
-            field_assigns[name] = assign_node
+        func = next(node.func.infer(context=context_itton))
+    except (InferenceError, StopIteration) as exc:
+        raise UseInferenceDefault from exc
 
-    init_str = _generate_dataclass_init([field_assigns[name] for name in field_order])
-    try:
-        init_node = parse(init_str)["__init__"]
-    except AstroidSyntaxError:
-        pass
-    else:
-        init_node.parent = node
-        init_node.lineno, init_node.col_offset = None, None
-        node.locals["__init__"] = [init_node]
-
-        root = node.root()
-        if DEFAULT_FACTORY not in root.locals:
-            new_assign = parse(f"{DEFAULT_FACTORY} = object()").body[0]
-            new_assign.parent = root
-            root.locals[DEFAULT_FACTORY] = [new_assign.targets[0]]
+    if func.qname() not in TYPING_TYPEVARS_QUALIFIED:
+        raise UseInferenceDefault
+    if not node.args:
+        raise UseInferenceDefault
+    # Cannot infer from a dynamic class name (f-string)
+    if isinstance(node.args[0], JoinedStr):
+        raise UseInferenceDefault
 
+    typename = node.args[0].as_string().strip("'")
+    node = extract_node(TYPING_TYPE_TEMPLATE.format(typename))
+    return node.infer(context=context_itton)
+
+
+def _looks_like_typing_subscript(node) -> bool:
+    """Try to figure out if a Subscript node *might* be a typing-related subscript."""
+    if isinstance(node, Name):
+        return node.name in TYPING_MEMBERS
+    if isinstance(node, Attribute):
+        return node.attrname in TYPING_MEMBERS
+    if isinstance(node, Subscript):
+        return _looks_like_typing_subscript(node.value)
+    return False
+
+
+def infer_typing_attr(
+    node: Subscript, ctx: context.InferenceContext | None = None
+) -> Iterator[ClassDef]:
+    """Infer a typing.X[...] subscript."""
+    try:
+        value = next(node.value.infer())  # type: ignore[union-attr] # value shouldn't be None for Subscript.
+    except (InferenceError, StopIteration) as exc:
+        raise UseInferenceDefault from exc
 
-def _get_dataclass_attributes(node: ClassDef, init: bool = False) -> Generator:
-    """Yield the AnnAssign nodes of dataclass attributes for the node.
+    if not value.qname().startswith("typing.") or value.qname() in TYPING_ALIAS:
+        # If typing subscript belongs to an alias handle it separately.
+        raise UseInferenceDefault
 
-    If init is True, also include InitVars, but exclude attributes from calls to
-    field where init=False.
-    """
-    for assign_node in node.body:
-        if not isinstance(assign_node, AnnAssign) or not isinstance(
-            assign_node.target, AssignName
+    if isinstance(value, ClassDef) and value.qname() in {
+        "typing.Generic",
+        "typing.Annotated",
+        "typing_extensions.Annotated",
+    }:
+        # typing.Generic and typing.Annotated (PY39) are subscriptable
+        # through __class_getitem__. Since astroid can't easily
+        # infer the native methods, replace them for an easy inference tip
+        func_to_add = _extract_single_node(CLASS_GETITEM_TEMPLATE)
+        value.locals["__class_getitem__"] = [func_to_add]
+        if (
+            isinstance(node.parent, ClassDef)
+            and node in node.parent.bases
+            and getattr(node.parent, "__cache", None)
         ):
-            continue
+            # node.parent.slots is evaluated and cached before the inference tip
+            # is first applied. Remove the last result to allow a recalculation of slots
+            cache = node.parent.__cache  # type: ignore[attr-defined] # Unrecognized getattr
+            if cache.get(node.parent.slots) is not None:
+                del cache[node.parent.slots]
+        return iter([value])
 
-        if _is_class_var(assign_node.annotation):  # type: ignore[arg-type] # annotation is never None
-            continue
+    node = extract_node(TYPING_TYPE_TEMPLATE.format(value.qname().split(".")[-1]))
+    return node.infer(context=ctx)
 
-        if init:
-            value = assign_node.value
-            if (
-                isinstance(value, Call)
-                and _looks_like_dataclass_field_call(value, check_scope=False)
-                and any(
-                    keyword.arg == "init"
-                    and not keyword.value.bool_value()  # type: ignore[union-attr] # value is never None
-                    for keyword in value.keywords
-                )
-            ):
-                continue
-        elif _is_init_var(assign_node.annotation):  # type: ignore[arg-type] # annotation is never None
-            continue
-
-        yield assign_node
-
-
-def _check_generate_dataclass_init(node: ClassDef) -> bool:
-    """Return True if we should generate an __init__ method for node.
-
-    This is True when:
-        - node doesn't define its own __init__ method
-        - the dataclass decorator was called *without* the keyword argument init=False
-    """
-    if "__init__" in node.locals:
-        return False
 
-    found = None
+def _looks_like_typedDict(  # pylint: disable=invalid-name
+    node: FunctionDef | ClassDef,
+) -> bool:
+    """Check if node is TypedDict FunctionDef."""
+    return node.qname() in TYPING_TYPEDDICT_QUALIFIED
 
-    for decorator_attribute in node.decorators.nodes:
-        if not isinstance(decorator_attribute, Call):
-            continue
-
-        if _looks_like_dataclass_decorator(decorator_attribute):
-            found = decorator_attribute
-
-    if found is None:
-        return True
-
-    # Check for keyword arguments of the form init=False
-    return all(
-        keyword.arg != "init"
-        and keyword.value.bool_value()  # type: ignore[union-attr] # value is never None
-        for keyword in found.keywords
-    )
 
+def infer_old_typedDict(  # pylint: disable=invalid-name
+    node: ClassDef, ctx: context.InferenceContext | None = None
+) -> Iterator[ClassDef]:
+    func_to_add = _extract_single_node("dict")
+    node.locals["__call__"] = [func_to_add]
+    return iter([node])
+
+
+def infer_typedDict(  # pylint: disable=invalid-name
+    node: FunctionDef, ctx: context.InferenceContext | None = None
+) -> Iterator[ClassDef]:
+    """Replace TypedDict FunctionDef with ClassDef."""
+    class_def = ClassDef(
+        name="TypedDict",
+        lineno=node.lineno,
+        col_offset=node.col_offset,
+        parent=node.parent,
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
+    )
+    class_def.postinit(bases=[extract_node("dict")], body=[], decorators=None)
+    func_to_add = _extract_single_node("dict")
+    class_def.locals["__call__"] = [func_to_add]
+    return iter([class_def])
 
-def _generate_dataclass_init(assigns: List[AnnAssign]) -> str:
-    """Return an init method for a dataclass given the targets."""
-    target_names = []
-    params = []
-    assignments = []
-
-    for assign in assigns:
-        name, annotation, value = assign.target.name, assign.annotation, assign.value
-        target_names.append(name)
-
-        if _is_init_var(annotation):  # type: ignore[arg-type] # annotation is never None
-            init_var = True
-            if isinstance(annotation, Subscript):
-                annotation = annotation.slice
-            else:
-                # Cannot determine type annotation for parameter from InitVar
-                annotation = None
-            assignment_str = ""
-        else:
-            init_var = False
-            assignment_str = f"self.{name} = {name}"
-
-        if annotation:
-            param_str = f"{name}: {annotation.as_string()}"
-        else:
-            param_str = name
-
-        if value:
-            if isinstance(value, Call) and _looks_like_dataclass_field_call(
-                value, check_scope=False
-            ):
-                result = _get_field_default(value)
-                if result:
-                    default_type, default_node = result
-                    if default_type == "default":
-                        param_str += f" = {default_node.as_string()}"
-                    elif default_type == "default_factory":
-                        param_str += f" = {DEFAULT_FACTORY}"
-                        assignment_str = (
-                            f"self.{name} = {default_node.as_string()} "
-                            f"if {name} is {DEFAULT_FACTORY} else {name}"
-                        )
-            else:
-                param_str += f" = {value.as_string()}"
-
-        params.append(param_str)
-        if not init_var:
-            assignments.append(assignment_str)
-
-    params_string = ", ".join(["self"] + params)
-    assignments_string = "\n    ".join(assignments) if assignments else "pass"
-    return f"def __init__({params_string}) -> None:\n    {assignments_string}"
-
-
-def infer_dataclass_attribute(
-    node: Unknown, ctx: Optional[context.InferenceContext] = None
-) -> Generator:
-    """Inference tip for an Unknown node that was dynamically generated to
-    represent a dataclass attribute.
 
-    In the case that a default value is provided, that is inferred first.
-    Then, an Instance of the annotated class is yielded.
+def _looks_like_typing_alias(node: Call) -> bool:
     """
-    assign = node.parent
-    if not isinstance(assign, AnnAssign):
-        yield Uninferable
-        return
-
-    annotation, value = assign.annotation, assign.value
-    if value is not None:
-        yield from value.infer(context=ctx)
-    if annotation is not None:
-        yield from _infer_instance_from_annotation(annotation, ctx=ctx)
-    else:
-        yield Uninferable
+    Returns True if the node corresponds to a call to _alias function.
 
+    For example :
 
-def infer_dataclass_field_call(
-    node: Call, ctx: Optional[context.InferenceContext] = None
-) -> Generator:
-    """Inference tip for dataclass field calls."""
-    if not isinstance(node.parent, (AnnAssign, Assign)):
-        raise UseInferenceDefault
-    result = _get_field_default(node)
-    if not result:
-        yield Uninferable
-    else:
-        default_type, default = result
-        if default_type == "default":
-            yield from default.infer(context=ctx)
-        else:
-            new_call = parse(default.as_string()).body[0].value
-            new_call.parent = node.parent
-            yield from new_call.infer(context=ctx)
-
-
-def _looks_like_dataclass_decorator(
-    node: NodeNG, decorator_names: FrozenSet[str] = DATACLASSES_DECORATORS
-) -> bool:
-    """Return True if node looks like a dataclass decorator.
+    MutableSet = _alias(collections.abc.MutableSet, T)
 
-    Uses inference to lookup the value of the node, and if that fails,
-    matches against specific names.
+    :param node: call node
     """
-    if isinstance(node, Call):  # decorator with arguments
-        node = node.func
-    try:
-        inferred = next(node.infer())
-    except (InferenceError, StopIteration):
-        inferred = Uninferable
-
-    if inferred is Uninferable:
-        if isinstance(node, Name):
-            return node.name in decorator_names
-        if isinstance(node, Attribute):
-            return node.attrname in decorator_names
-
-        return False
-
     return (
-        isinstance(inferred, FunctionDef)
-        and inferred.name in decorator_names
-        and inferred.root().name in DATACLASS_MODULES
+        isinstance(node.func, Name)
+        and node.func.name == "_alias"
+        and (
+            # _alias function works also for builtins object such as list and dict
+            isinstance(node.args[0], (Attribute, Name))
+        )
     )
 
 
-def _looks_like_dataclass_attribute(node: Unknown) -> bool:
-    """Return True if node was dynamically generated as the child of an AnnAssign
-    statement.
-    """
-    parent = node.parent
-    if not parent:
-        return False
+def _forbid_class_getitem_access(node: ClassDef) -> None:
+    """Disable the access to __class_getitem__ method for the node in parameters."""
 
-    scope = parent.scope()
-    return (
-        isinstance(parent, AnnAssign)
-        and isinstance(scope, ClassDef)
-        and is_decorated_with_dataclass(scope)
-    )
+    def full_raiser(origin_func, attr, *args, **kwargs):
+        """
+        Raises an AttributeInferenceError in case of access to __class_getitem__ method.
+        Otherwise, just call origin_func.
+        """
+        if attr == "__class_getitem__":
+            raise AttributeInferenceError("__class_getitem__ access is not allowed")
+        return origin_func(attr, *args, **kwargs)
 
+    try:
+        node.getattr("__class_getitem__")
+        # If we are here, then we are sure to modify an object that does have
+        # __class_getitem__ method (which origin is the protocol defined in
+        # collections module) whereas the typing module considers it should not.
+        # We do not want __class_getitem__ to be found in the classdef
+        partial_raiser = partial(full_raiser, node.getattr)
+        node.getattr = partial_raiser
+    except AttributeInferenceError:
+        pass
 
-def _looks_like_dataclass_field_call(node: Call, check_scope: bool = True) -> bool:
-    """Return True if node is calling dataclasses field or Field
-    from an AnnAssign statement directly in the body of a ClassDef.
 
-    If check_scope is False, skips checking the statement and body.
+def infer_typing_alias(
+    node: Call, ctx: context.InferenceContext | None = None
+) -> Iterator[ClassDef]:
     """
-    if check_scope:
-        stmt = node.statement(future=True)
-        scope = stmt.scope()
-        if not (
-            isinstance(stmt, AnnAssign)
-            and stmt.value is not None
-            and isinstance(scope, ClassDef)
-            and is_decorated_with_dataclass(scope)
-        ):
-            return False
+    Infers the call to _alias function
+    Insert ClassDef, with same name as aliased class,
+    in mro to simulate _GenericAlias.
 
+    :param node: call node
+    :param context: inference context
+    """
+    if (
+        not isinstance(node.parent, Assign)
+        or not len(node.parent.targets) == 1
+        or not isinstance(node.parent.targets[0], AssignName)
+    ):
+        raise UseInferenceDefault
     try:
-        inferred = next(node.func.infer())
-    except (InferenceError, StopIteration):
-        return False
-
-    if not isinstance(inferred, FunctionDef):
-        return False
+        res = next(node.args[0].infer(context=ctx))
+    except StopIteration as e:
+        raise InferenceError(node=node.args[0], context=ctx) from e
+
+    assign_name = node.parent.targets[0]
+
+    class_def = ClassDef(
+        name=assign_name.name,
+        lineno=assign_name.lineno,
+        col_offset=assign_name.col_offset,
+        parent=node.parent,
+        end_lineno=assign_name.end_lineno,
+        end_col_offset=assign_name.end_col_offset,
+    )
+    if isinstance(res, ClassDef):
+        # Only add `res` as base if it's a `ClassDef`
+        # This isn't the case for `typing.Pattern` and `typing.Match`
+        class_def.postinit(bases=[res], body=[], decorators=None)
+
+    maybe_type_var = node.args[1]
+    if (
+        not PY39_PLUS
+        and not (isinstance(maybe_type_var, Tuple) and not maybe_type_var.elts)
+        or PY39_PLUS
+        and isinstance(maybe_type_var, Const)
+        and maybe_type_var.value > 0
+    ):
+        # If typing alias is subscriptable, add `__class_getitem__` to ClassDef
+        func_to_add = _extract_single_node(CLASS_GETITEM_TEMPLATE)
+        class_def.locals["__class_getitem__"] = [func_to_add]
+    else:
+        # If not, make sure that `__class_getitem__` access is forbidden.
+        # This is an issue in cases where the aliased class implements it,
+        # but the typing alias isn't subscriptable. E.g., `typing.ByteString` for PY39+
+        _forbid_class_getitem_access(class_def)
+    return iter([class_def])
 
-    return inferred.name == FIELD_NAME and inferred.root().name in DATACLASS_MODULES
 
+def _looks_like_special_alias(node: Call) -> bool:
+    """Return True if call is for Tuple or Callable alias.
 
-def _get_field_default(field_call: Call) -> _FieldDefaultReturn:
-    """Return a the default value of a field call, and the corresponding keyword argument name.
+    In PY37 and PY38 the call is to '_VariadicGenericAlias' with 'tuple' as
+    first argument. In PY39+ it is replaced by a call to '_TupleType'.
 
-    field(default=...) results in the ... node
-    field(default_factory=...) results in a Call node with func ... and no arguments
+    PY37: Tuple = _VariadicGenericAlias(tuple, (), inst=False, special=True)
+    PY39: Tuple = _TupleType(tuple, -1, inst=False, name='Tuple')
 
-    If neither or both arguments are present, return ("", None) instead,
-    indicating that there is not a valid default value.
+    PY37: Callable = _VariadicGenericAlias(collections.abc.Callable, (), special=True)
+    PY39: Callable = _CallableType(collections.abc.Callable, 2)
     """
-    default, default_factory = None, None
-    for keyword in field_call.keywords:
-        if keyword.arg == "default":
-            default = keyword.value
-        elif keyword.arg == "default_factory":
-            default_factory = keyword.value
-
-    if default is not None and default_factory is None:
-        return "default", default
-
-    if default is None and default_factory is not None:
-        new_call = Call(
-            lineno=field_call.lineno,
-            col_offset=field_call.col_offset,
-            parent=field_call.parent,
+    return isinstance(node.func, Name) and (
+        not PY39_PLUS
+        and node.func.name == "_VariadicGenericAlias"
+        and (
+            isinstance(node.args[0], Name)
+            and node.args[0].name == "tuple"
+            or isinstance(node.args[0], Attribute)
+            and node.args[0].as_string() == "collections.abc.Callable"
+        )
+        or PY39_PLUS
+        and (
+            node.func.name == "_TupleType"
+            and isinstance(node.args[0], Name)
+            and node.args[0].name == "tuple"
+            or node.func.name == "_CallableType"
+            and isinstance(node.args[0], Attribute)
+            and node.args[0].as_string() == "collections.abc.Callable"
         )
-        new_call.postinit(func=default_factory)
-        return "default_factory", new_call
-
-    return None
-
-
-def _is_class_var(node: NodeNG) -> bool:
-    """Return True if node is a ClassVar, with or without subscripting."""
-    if PY39_PLUS:
-        try:
-            inferred = next(node.infer())
-        except (InferenceError, StopIteration):
-            return False
-
-        return getattr(inferred, "name", "") == "ClassVar"
-
-    # Before Python 3.9, inference returns typing._SpecialForm instead of ClassVar.
-    # Our backup is to inspect the node's structure.
-    return isinstance(node, Subscript) and (
-        isinstance(node.value, Name)
-        and node.value.name == "ClassVar"
-        or isinstance(node.value, Attribute)
-        and node.value.attrname == "ClassVar"
     )
 
 
-def _is_init_var(node: NodeNG) -> bool:
-    """Return True if node is an InitVar, with or without subscripting."""
+def infer_special_alias(
+    node: Call, ctx: context.InferenceContext | None = None
+) -> Iterator[ClassDef]:
+    """Infer call to tuple alias as new subscriptable class typing.Tuple."""
+    if not (
+        isinstance(node.parent, Assign)
+        and len(node.parent.targets) == 1
+        and isinstance(node.parent.targets[0], AssignName)
+    ):
+        raise UseInferenceDefault
     try:
-        inferred = next(node.infer())
-    except (InferenceError, StopIteration):
-        return False
-
-    return getattr(inferred, "name", "") == "InitVar"
+        res = next(node.args[0].infer(context=ctx))
+    except StopIteration as e:
+        raise InferenceError(node=node.args[0], context=ctx) from e
+
+    assign_name = node.parent.targets[0]
+    class_def = ClassDef(
+        name=assign_name.name,
+        parent=node.parent,
+        lineno=assign_name.lineno,
+        col_offset=assign_name.col_offset,
+        end_lineno=assign_name.end_lineno,
+        end_col_offset=assign_name.end_col_offset,
+    )
+    class_def.postinit(bases=[res], body=[], decorators=None)
+    func_to_add = _extract_single_node(CLASS_GETITEM_TEMPLATE)
+    class_def.locals["__class_getitem__"] = [func_to_add]
+    return iter([class_def])
 
 
-# Allowed typing classes for which we support inferring instances
-_INFERABLE_TYPING_TYPES = frozenset(
-    (
-        "Dict",
-        "FrozenSet",
-        "List",
-        "Set",
-        "Tuple",
+def _looks_like_typing_cast(node: Call) -> bool:
+    return isinstance(node, Call) and (
+        isinstance(node.func, Name)
+        and node.func.name == "cast"
+        or isinstance(node.func, Attribute)
+        and node.func.attrname == "cast"
     )
-)
 
 
-def _infer_instance_from_annotation(
-    node: NodeNG, ctx: Optional[context.InferenceContext] = None
-) -> Generator:
-    """Infer an instance corresponding to the type annotation represented by node.
+def infer_typing_cast(
+    node: Call, ctx: context.InferenceContext | None = None
+) -> Iterator[NodeNG]:
+    """Infer call to cast() returning same type as casted-from var."""
+    if not isinstance(node.func, (Name, Attribute)):
+        raise UseInferenceDefault
 
-    Currently has limited support for the typing module.
-    """
-    klass = None
     try:
-        klass = next(node.infer(context=ctx))
-    except (InferenceError, StopIteration):
-        yield Uninferable
-    if not isinstance(klass, ClassDef):
-        yield Uninferable
-    elif klass.root().name in {
-        "typing",
-        "_collections_abc",
-        "",
-    }:  # "" because of synthetic nodes in brain_typing.py
-        if klass.name in _INFERABLE_TYPING_TYPES:
-            yield klass.instantiate_class()
-        else:
-            yield Uninferable
-    else:
-        yield klass.instantiate_class()
+        func = next(node.func.infer(context=ctx))
+    except (InferenceError, StopIteration) as exc:
+        raise UseInferenceDefault from exc
+    if (
+        not isinstance(func, FunctionDef)
+        or func.qname() != "typing.cast"
+        or len(node.args) != 2
+    ):
+        raise UseInferenceDefault
 
+    return node.args[1].infer(context=ctx)
 
-if PY37_PLUS:
-    AstroidManager().register_transform(
-        ClassDef, dataclass_transform, is_decorated_with_dataclass
-    )
 
+AstroidManager().register_transform(
+    Call,
+    inference_tip(infer_typing_typevar_or_newtype),
+    looks_like_typing_typevar_or_newtype,
+)
+AstroidManager().register_transform(
+    Subscript, inference_tip(infer_typing_attr), _looks_like_typing_subscript
+)
+AstroidManager().register_transform(
+    Call, inference_tip(infer_typing_cast), _looks_like_typing_cast
+)
+
+if PY39_PLUS:
     AstroidManager().register_transform(
-        Call,
-        inference_tip(infer_dataclass_field_call, raise_on_overwrite=True),
-        _looks_like_dataclass_field_call,
+        FunctionDef, inference_tip(infer_typedDict), _looks_like_typedDict
     )
-
+else:
     AstroidManager().register_transform(
-        Unknown,
-        inference_tip(infer_dataclass_attribute, raise_on_overwrite=True),
-        _looks_like_dataclass_attribute,
+        ClassDef, inference_tip(infer_old_typedDict), _looks_like_typedDict
     )
+
+AstroidManager().register_transform(
+    Call, inference_tip(infer_typing_alias), _looks_like_typing_alias
+)
+AstroidManager().register_transform(
+    Call, inference_tip(infer_special_alias), _looks_like_special_alias
+)
```

### Comparing `astroid-2.9.3/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a1/astroid/brain/brain_dateutil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-# Copyright (c) 2015-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015 raylu <lurayl@gmail.com>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""Astroid hooks for dateutil"""
+"""Astroid hooks for dateutil."""
 
 import textwrap
 
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import AstroidBuilder
 from astroid.manager import AstroidManager
```

### Comparing `astroid-2.9.3/astroid/brain/brain_functools.py` & `astroid-3.0.0a1/astroid/brain/brain_functools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# Copyright (c) 2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2018 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Alphadelta14 <alpha@alphaservcomputing.solutions>
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for understanding functools library module."""
+
+from __future__ import annotations
+
+from collections.abc import Iterator
 from functools import partial
 from itertools import chain
 
-from astroid import BoundMethod, arguments, extract_node, helpers, objects
+from astroid import BoundMethod, arguments, extract_node, helpers, nodes, objects
+from astroid.context import InferenceContext
 from astroid.exceptions import InferenceError, UseInferenceDefault
 from astroid.inference_tip import inference_tip
 from astroid.interpreter import objectmodel
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import AssignName, Attribute, Call, Name
 from astroid.nodes.scoped_nodes import FunctionDef
-from astroid.util import Uninferable
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
+from astroid.util import UninferableBase
 
 LRU_CACHE = "functools.lru_cache"
 
 
 class LruWrappedModel(objectmodel.FunctionModel):
     """Special attribute model for functions decorated with functools.lru_cache.
 
@@ -37,51 +41,59 @@
             """
         from functools import _CacheInfo
         _CacheInfo(0, 0, 0, 0)
         """
         )
 
         class CacheInfoBoundMethod(BoundMethod):
-            def infer_call_result(self, caller, context=None):
-                yield helpers.safe_infer(cache_info)
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[InferenceResult]:
+                res = helpers.safe_infer(cache_info)
+                assert res is not None
+                yield res
 
         return CacheInfoBoundMethod(proxy=self._instance, bound=self._instance)
 
     @property
     def attr_cache_clear(self):
         node = extract_node("""def cache_clear(self): pass""")
         return BoundMethod(proxy=node, bound=self._instance.parent.scope())
 
 
-def _transform_lru_cache(node, context=None) -> None:
+def _transform_lru_cache(node, context: InferenceContext | None = None) -> None:
     # TODO: this is not ideal, since the node should be immutable,
-    # but due to https://github.com/PyCQA/astroid/issues/354,
+    # but due to https://github.com/pylint-dev/astroid/issues/354,
     # there's not much we can do now.
     # Replacing the node would work partially, because,
     # in pylint, the old node would still be available, leading
     # to spurious false positives.
     node.special_attributes = LruWrappedModel()(node)
 
 
-def _functools_partial_inference(node, context=None):
+def _functools_partial_inference(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[objects.PartialFunction]:
     call = arguments.CallSite.from_call(node, context=context)
     number_of_positional = len(call.positional_arguments)
     if number_of_positional < 1:
         raise UseInferenceDefault("functools.partial takes at least one argument")
     if number_of_positional == 1 and not call.keyword_arguments:
         raise UseInferenceDefault(
             "functools.partial needs at least to have some filled arguments"
         )
 
     partial_function = call.positional_arguments[0]
     try:
         inferred_wrapped_function = next(partial_function.infer(context=context))
     except (InferenceError, StopIteration) as exc:
         raise UseInferenceDefault from exc
-    if inferred_wrapped_function is Uninferable:
+    if isinstance(inferred_wrapped_function, UninferableBase):
         raise UseInferenceDefault("Cannot infer the wrapped function")
     if not isinstance(inferred_wrapped_function, FunctionDef):
         raise UseInferenceDefault("The wrapped function is not a function")
 
     # Determine if the passed keywords into the callsite are supported
     # by the wrapped function.
     if not inferred_wrapped_function.args:
@@ -97,44 +109,44 @@
     }
     if set(call.keyword_arguments) - parameter_names:
         raise UseInferenceDefault("wrapped function received unknown parameters")
 
     partial_function = objects.PartialFunction(
         call,
         name=inferred_wrapped_function.name,
-        doc=inferred_wrapped_function.doc,
         lineno=inferred_wrapped_function.lineno,
         col_offset=inferred_wrapped_function.col_offset,
         parent=node.parent,
     )
     partial_function.postinit(
         args=inferred_wrapped_function.args,
         body=inferred_wrapped_function.body,
         decorators=inferred_wrapped_function.decorators,
         returns=inferred_wrapped_function.returns,
         type_comment_returns=inferred_wrapped_function.type_comment_returns,
         type_comment_args=inferred_wrapped_function.type_comment_args,
+        doc_node=inferred_wrapped_function.doc_node,
     )
     return iter((partial_function,))
 
 
-def _looks_like_lru_cache(node):
+def _looks_like_lru_cache(node) -> bool:
     """Check if the given function node is decorated with lru_cache."""
     if not node.decorators:
         return False
     for decorator in node.decorators.nodes:
         if not isinstance(decorator, Call):
             continue
         if _looks_like_functools_member(decorator, "lru_cache"):
             return True
     return False
 
 
 def _looks_like_functools_member(node, member) -> bool:
-    """Check if the given Call node is a functools.partial call"""
+    """Check if the given Call node is a functools.partial call."""
     if isinstance(node.func, Name):
         return node.func.name == member
     if isinstance(node.func, Attribute):
         return (
             node.func.attrname == member
             and isinstance(node.func.expr, Name)
             and node.func.expr.name == "functools"
```

### Comparing `astroid-2.9.3/astroid/brain/brain_gi.py` & `astroid-3.0.0a1/astroid/brain/brain_gi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-# Copyright (c) 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2014 Google, Inc.
-# Copyright (c) 2014 Cole Robinson <crobinso@redhat.com>
-# Copyright (c) 2015-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 David Shea <dshea@redhat.com>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2016 Giuseppe Scrivano <gscrivan@redhat.com>
-# Copyright (c) 2018 Christoph Reiter <reiter.christoph@gmail.com>
-# Copyright (c) 2019 Philipp Hörist <philipp@hoerist.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for the Python 2 GObject introspection bindings.
 
 Helps with understanding everything imported from 'gi.repository'
 """
 
 # pylint:disable=import-error,import-outside-toplevel
@@ -51,29 +37,28 @@
         "__setitem__",
         "__delitem__",
         "__len__",
         "__bool__",
         "__nonzero__",
         "__next__",
         "__str__",
-        "__len__",
         "__contains__",
         "__enter__",
         "__exit__",
         "__repr__",
         "__getattr__",
         "__setattr__",
         "__delattr__",
         "__del__",
         "__hash__",
     }
 )
 
 
-def _gi_build_stub(parent):
+def _gi_build_stub(parent):  # noqa: C901
     """
     Inspect the passed module recursively and build stubs for functions,
     classes, etc.
     """
     classes = {}
     functions = {}
     constants = {}
@@ -84,15 +69,17 @@
 
         # Check if this is a valid name in python
         if not re.match(_identifier_re, name):
             continue
 
         try:
             obj = getattr(parent, name)
-        except AttributeError:
+        except Exception:  # pylint: disable=broad-except
+            # gi.module.IntrospectionModule.__getattr__() can raise all kinds of things
+            # like ValueError, TypeError, NotImplementedError, RepositoryError, etc
             continue
 
         if inspect.isclass(obj):
             classes[name] = obj
         elif inspect.isfunction(obj) or inspect.isbuiltin(obj):
             functions[name] = obj
         elif inspect.ismethod(obj) or inspect.ismethoddescriptor(obj):
@@ -216,15 +203,15 @@
     else:
         astng = _inspected_modules[modname]
     if astng is None:
         raise AstroidBuildingError(modname=modname)
     return astng
 
 
-def _looks_like_require_version(node):
+def _looks_like_require_version(node) -> bool:
     # Return whether this looks like a call to gi.require_version(<name>, <version>)
     # Only accept function calls with two constant arguments
     if len(node.args) != 2:
         return False
 
     if not all(isinstance(arg, nodes.Const) for arg in node.args):
         return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a1/astroid/brain/brain_multiprocessing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,107 @@
-# Copyright (c) 2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2018 David Poirier <david-poirier-csn@users.noreply.github.com>
-# Copyright (c) 2018 wgehalo <wgehalo@gmail.com>
-# Copyright (c) 2018 Ioana Tagirta <ioana.tagirta@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 David Gilman <davidgilman1@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
+from astroid.bases import BoundMethod
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
+from astroid.exceptions import InferenceError
 from astroid.manager import AstroidManager
+from astroid.nodes.scoped_nodes import FunctionDef
 
 
-def _hashlib_transform():
-    signature = "value=''"
-    template = """
-    class %(name)s(object):
-      def __init__(self, %(signature)s): pass
-      def digest(self):
-        return %(digest)s
-      def copy(self):
-        return self
-      def update(self, value): pass
-      def hexdigest(self):
-        return ''
-      @property
-      def name(self):
-        return %(name)r
-      @property
-      def block_size(self):
-        return 1
-      @property
-      def digest_size(self):
-        return 1
+def _multiprocessing_transform():
+    module = parse(
+        """
+    from multiprocessing.managers import SyncManager
+    def Manager():
+        return SyncManager()
     """
-    algorithms_with_signature = dict.fromkeys(
-        ["md5", "sha1", "sha224", "sha256", "sha384", "sha512"], signature
-    )
-    blake2b_signature = "data=b'', *, digest_size=64, key=b'', salt=b'', \
-            person=b'', fanout=1, depth=1, leaf_size=0, node_offset=0, \
-            node_depth=0, inner_size=0, last_node=False"
-    blake2s_signature = "data=b'', *, digest_size=32, key=b'', salt=b'', \
-            person=b'', fanout=1, depth=1, leaf_size=0, node_offset=0, \
-            node_depth=0, inner_size=0, last_node=False"
-    new_algorithms = dict.fromkeys(
-        ["sha3_224", "sha3_256", "sha3_384", "sha3_512", "shake_128", "shake_256"],
-        signature,
     )
-    algorithms_with_signature.update(new_algorithms)
-    algorithms_with_signature.update(
-        {"blake2b": blake2b_signature, "blake2s": blake2s_signature}
+    # Multiprocessing uses a getattr lookup inside contexts,
+    # in order to get the attributes they need. Since it's extremely
+    # dynamic, we use this approach to fake it.
+    node = parse(
+        """
+    from multiprocessing.context import DefaultContext, BaseContext
+    default = DefaultContext()
+    base = BaseContext()
+    """
     )
-    classes = "".join(
-        template % {"name": hashfunc, "digest": 'b""', "signature": signature}
-        for hashfunc, signature in algorithms_with_signature.items()
+    try:
+        context = next(node["default"].infer())
+        base = next(node["base"].infer())
+    except (InferenceError, StopIteration):
+        return module
+
+    for node in (context, base):
+        for key, value in node.locals.items():
+            if key.startswith("_"):
+                continue
+
+            value = value[0]
+            if isinstance(value, FunctionDef):
+                # We need to rebound this, since otherwise
+                # it will have an extra argument (self).
+                value = BoundMethod(value, node)
+            module[key] = value
+    return module
+
+
+def _multiprocessing_managers_transform():
+    return parse(
+        """
+    import array
+    import threading
+    import multiprocessing.pool as pool
+    import queue
+
+    class Namespace(object):
+        pass
+
+    class Value(object):
+        def __init__(self, typecode, value, lock=True):
+            self._typecode = typecode
+            self._value = value
+        def get(self):
+            return self._value
+        def set(self, value):
+            self._value = value
+        def __repr__(self):
+            return '%s(%r, %r)'%(type(self).__name__, self._typecode, self._value)
+        value = property(get, set)
+
+    def Array(typecode, sequence, lock=True):
+        return array.array(typecode, sequence)
+
+    class SyncManager(object):
+        Queue = JoinableQueue = queue.Queue
+        Event = threading.Event
+        RLock = threading.RLock
+        Lock = threading.Lock
+        BoundedSemaphore = threading.BoundedSemaphore
+        Condition = threading.Condition
+        Barrier = threading.Barrier
+        Pool = pool.Pool
+        list = list
+        dict = dict
+        Value = Value
+        Array = Array
+        Namespace = Namespace
+        __enter__ = lambda self: self
+        __exit__ = lambda *args: args
+
+        def start(self, initializer=None, initargs=None):
+            pass
+        def shutdown(self):
+            pass
+    """
     )
-    return parse(classes)
 
 
-register_module_extender(AstroidManager(), "hashlib", _hashlib_transform)
+register_module_extender(
+    AstroidManager(), "multiprocessing.managers", _multiprocessing_managers_transform
+)
+register_module_extender(
+    AstroidManager(), "multiprocessing", _multiprocessing_transform
+)
```

### Comparing `astroid-2.9.3/astroid/brain/brain_http.py` & `astroid-3.0.0a1/astroid/brain/brain_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-# Copyright (c) 2019-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid brain hints for some of the `http` module."""
 import textwrap
 
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import AstroidBuilder
 from astroid.manager import AstroidManager
 
 
 def _http_transform():
     code = textwrap.dedent(
         """
+    from enum import IntEnum
     from collections import namedtuple
     _HTTPStatus = namedtuple('_HTTPStatus', 'value phrase description')
 
-    class HTTPStatus:
+    class HTTPStatus(IntEnum):
 
         @property
         def phrase(self):
             return ""
         @property
         def value(self):
             return 0
```

### Comparing `astroid-2.9.3/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a1/astroid/brain/brain_hypothesis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """
 Astroid hook for the Hypothesis library.
 
 Without this hook pylint reports no-value-for-parameter for use of strategies
 defined using the `@hypothesis.strategies.composite` decorator.  For example:
 
     from hypothesis import strategies as st
 
     @st.composite
     def a_strategy(draw):
         return draw(st.integers())
 
     a_strategy()
-
 """
 from astroid.manager import AstroidManager
 from astroid.nodes.scoped_nodes import FunctionDef
 
 COMPOSITE_NAMES = (
     "composite",
     "st.composite",
     "strategies.composite",
     "hypothesis.strategies.composite",
 )
 
 
-def is_decorated_with_st_composite(node):
-    """Return True if a decorated node has @st.composite applied."""
+def is_decorated_with_st_composite(node) -> bool:
+    """Return whether a decorated node has @st.composite applied."""
     if node.decorators and node.args.args and node.args.args[0].name == "draw":
         for decorator_attribute in node.decorators.nodes:
             if decorator_attribute.as_string() in COMPOSITE_NAMES:
                 return True
     return False
```

### Comparing `astroid-2.9.3/astroid/brain/brain_io.py` & `astroid-3.0.0a1/astroid/brain/brain_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Copyright (c) 2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid brain hints for some of the _io C objects."""
 from astroid.manager import AstroidManager
 from astroid.nodes import ClassDef
 
 BUFFERED = {"BufferedWriter", "BufferedReader"}
 TextIOWrapper = "TextIOWrapper"
 FileIO = "FileIO"
 BufferedWriter = "BufferedWriter"
 
 
 def _generic_io_transform(node, name, cls):
-    """Transform the given name, by adding the given *class* as a member of the node."""
+    """Transform the given name, by adding the given *class* as a member of the
+    node.
+    """
 
     io_module = AstroidManager().ast_from_module_name("_io")
     attribute_object = io_module[cls]
     instance = attribute_object.instantiate_class()
     node.locals[name] = [instance]
```

### Comparing `astroid-2.9.3/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a1/astroid/brain/brain_namedtuple_enum.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,62 @@
-# Copyright (c) 2012-2015 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2014-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Dmitry Pribysh <dmand@yandex.ru>
-# Copyright (c) 2015 David Shea <dshea@redhat.com>
-# Copyright (c) 2015 Philip Lorenz <philip@bithub.de>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2016 Mateusz Bysiek <mb@mbdev.pl>
-# Copyright (c) 2017 Hugo <hugovk@users.noreply.github.com>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2019 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2020 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Ram Rachum <ram@rachum.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Dimitri Prybysh <dmand@yandex.ru>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 pre-commit-ci[bot] <bot@noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for the Python standard library."""
 
+from __future__ import annotations
+
 import functools
 import keyword
+from collections.abc import Iterator
 from textwrap import dedent
+from typing import Final
 
 import astroid
-from astroid import arguments, inference_tip, nodes, util
-from astroid.builder import AstroidBuilder, extract_node
+from astroid import arguments, bases, inference_tip, nodes, util
+from astroid.builder import AstroidBuilder, _extract_single_node, extract_node
+from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AstroidValueError,
     InferenceError,
     MroError,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 
-TYPING_NAMEDTUPLE_BASENAMES = {"NamedTuple", "typing.NamedTuple"}
 ENUM_BASE_NAMES = {
     "Enum",
     "IntEnum",
     "enum.Enum",
     "enum.IntEnum",
     "IntFlag",
     "enum.IntFlag",
 }
+ENUM_QNAME: Final[str] = "enum.Enum"
+TYPING_NAMEDTUPLE_QUALIFIED: Final = {
+    "typing.NamedTuple",
+    "typing_extensions.NamedTuple",
+}
+TYPING_NAMEDTUPLE_BASENAMES: Final = {
+    "NamedTuple",
+    "typing.NamedTuple",
+    "typing_extensions.NamedTuple",
+}
 
 
 def _infer_first(node, context):
-    if node is util.Uninferable:
+    if isinstance(node, util.UninferableBase):
         raise UseInferenceDefault
     try:
         value = next(node.infer(context=context))
     except StopIteration as exc:
         raise InferenceError from exc
-    if value is util.Uninferable:
+    if isinstance(value, util.UninferableBase):
         raise UseInferenceDefault()
     return value
 
 
 def _find_func_form_arguments(node, context):
     def _extract_namedtuple_arg_or_keyword(  # pylint: disable=inconsistent-return-statements
         position, key_name=None
@@ -85,30 +76,42 @@
     names = _extract_namedtuple_arg_or_keyword(position=1, key_name="field_names")
     if name and names:
         return name.value, names
 
     raise UseInferenceDefault()
 
 
-def infer_func_form(node, base_type, context=None, enum=False):
+def infer_func_form(
+    node: nodes.Call,
+    base_type: list[nodes.NodeNG],
+    context: InferenceContext | None = None,
+    enum: bool = False,
+) -> tuple[nodes.ClassDef, str, list[str]]:
     """Specific inference function for namedtuple or Python 3 enum."""
     # node is a Call node, class name as first argument and generated class
     # attributes as second argument
 
     # namedtuple or enums list of attributes can be a list of strings or a
     # whitespace-separate string
     try:
         name, names = _find_func_form_arguments(node, context)
         try:
-            attributes = names.value.replace(",", " ").split()
+            attributes: list[str] = names.value.replace(",", " ").split()
         except AttributeError as exc:
+            # Handle attributes of NamedTuples
             if not enum:
-                attributes = [
-                    _infer_first(const, context).value for const in names.elts
-                ]
+                attributes = []
+                fields = _get_namedtuple_fields(node)
+                if fields:
+                    fields_node = extract_node(fields)
+                    attributes = [
+                        _infer_first(const, context).value for const in fields_node.elts
+                    ]
+
+            # Handle attributes of Enums
             else:
                 # Enums supports either iterator of (name, value) pairs
                 # or mappings.
                 if hasattr(names, "items") and isinstance(names.items, list):
                     attributes = [
                         _infer_first(const[0], context).value
                         for const in names.items
@@ -142,60 +145,84 @@
         # in which case we should not have inferred these values and raised earlier
     attributes = [attr for attr in attributes if " " not in attr]
 
     # If we can't infer the name of the class, don't crash, up to this point
     # we know it is a namedtuple anyway.
     name = name or "Uninferable"
     # we want to return a Class node instance with proper attributes set
-    class_node = nodes.ClassDef(name, "docstring")
+    class_node = nodes.ClassDef(
+        name,
+        lineno=node.lineno,
+        col_offset=node.col_offset,
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
+        parent=nodes.Unknown(),
+    )
+    # A typical ClassDef automatically adds its name to the parent scope,
+    # but doing so causes problems, so defer setting parent until after init
+    # see: https://github.com/pylint-dev/pylint/issues/5982
     class_node.parent = node.parent
-    # set base class=tuple
-    class_node.bases.append(base_type)
+    class_node.postinit(
+        # set base class=tuple
+        bases=base_type,
+        body=[],
+        decorators=None,
+    )
     # XXX add __init__(*attributes) method
     for attr in attributes:
         fake_node = nodes.EmptyNode()
         fake_node.parent = class_node
         fake_node.attrname = attr
         class_node.instance_attrs[attr] = [fake_node]
     return class_node, name, attributes
 
 
 def _has_namedtuple_base(node):
-    """Predicate for class inference tip
+    """Predicate for class inference tip.
 
     :type node: ClassDef
     :rtype: bool
     """
     return set(node.basenames) & TYPING_NAMEDTUPLE_BASENAMES
 
 
-def _looks_like(node, name):
+def _looks_like(node, name) -> bool:
     func = node.func
     if isinstance(func, nodes.Attribute):
         return func.attrname == name
     if isinstance(func, nodes.Name):
         return func.name == name
     return False
 
 
 _looks_like_namedtuple = functools.partial(_looks_like, name="namedtuple")
 _looks_like_enum = functools.partial(_looks_like, name="Enum")
 _looks_like_typing_namedtuple = functools.partial(_looks_like, name="NamedTuple")
 
 
-def infer_named_tuple(node, context=None):
-    """Specific inference function for namedtuple Call node"""
-    tuple_base_name = nodes.Name(name="tuple", parent=node.root())
+def infer_named_tuple(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[nodes.ClassDef]:
+    """Specific inference function for namedtuple Call node."""
+    tuple_base_name: list[nodes.NodeNG] = [
+        nodes.Name(
+            name="tuple",
+            parent=node.root(),
+            lineno=0,
+            col_offset=0,
+            end_lineno=None,
+            end_col_offset=None,
+        )
+    ]
     class_node, name, attributes = infer_func_form(
         node, tuple_base_name, context=context
     )
     call_site = arguments.CallSite.from_call(node, context=context)
     node = extract_node("import collections; collections.namedtuple")
     try:
-
         func = next(node.infer())
     except StopIteration as e:
         raise InferenceError(node=node) from e
     try:
         rename = next(call_site.infer_argument(func, "rename", context)).bool_value()
     except (InferenceError, StopIteration):
         rename = False
@@ -263,15 +290,15 @@
 def _check_namedtuple_attributes(typename, attributes, rename=False):
     attributes = tuple(attributes)
     if rename:
         attributes = _get_renamed_namedtuple_attributes(attributes)
 
     # The following snippet is derived from the CPython Lib/collections/__init__.py sources
     # <snippet>
-    for name in (typename,) + attributes:
+    for name in (typename, *attributes):
         if not isinstance(name, str):
             raise AstroidTypeError("Type names and field names must be strings")
         if not name.isidentifier():
             raise AstroidValueError(
                 "Type names and field names must be valid" + f"identifiers: {name!r}"
             )
         if keyword.iskeyword(name):
@@ -289,17 +316,31 @@
             raise AstroidValueError(f"Encountered duplicate field name: {name!r}")
         seen.add(name)
     # </snippet>
 
     return attributes
 
 
-def infer_enum(node, context=None):
+def infer_enum(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[bases.Instance]:
     """Specific inference function for enum Call node."""
-    enum_meta = extract_node(
+    # Raise `UseInferenceDefault` if `node` is a call to a a user-defined Enum.
+    try:
+        inferred = node.func.infer(context)
+    except (InferenceError, StopIteration) as exc:
+        raise UseInferenceDefault from exc
+
+    if not any(
+        isinstance(item, nodes.ClassDef) and item.qname() == ENUM_QNAME
+        for item in inferred
+    ):
+        raise UseInferenceDefault
+
+    enum_meta = _extract_single_node(
         """
     class EnumMeta(object):
         'docstring'
         def __call__(self, node):
             class EnumAttribute(object):
                 name = ''
                 value = 0
@@ -325,15 +366,15 @@
                 def value(self):
                     return attr
 
             return Value()
         __members__ = ['']
     """
     )
-    class_node = infer_func_form(node, enum_meta, context=context, enum=True)[0]
+    class_node = infer_func_form(node, [enum_meta], context=context, enum=True)[0]
     return iter([class_node.instantiate_class()])
 
 
 INT_FLAG_ADDITION_METHODS = """
     def __or__(self, other):
         return {name}(self.value | other.value)
     def __and__(self, other):
@@ -347,19 +388,17 @@
     def __invert__(self):
         return {name}(~self.value)
     def __mul__(self, other):
         return {name}(self.value * other.value)
 """
 
 
-def infer_enum_class(node):
+def infer_enum_class(node: nodes.ClassDef) -> nodes.ClassDef:
     """Specific inference for enums."""
     for basename in (b for cls in node.mro() for b in cls.basenames):
-        if basename not in ENUM_BASE_NAMES:
-            continue
         if node.root().name == "enum":
             # Skip if the class is directly from enum module.
             break
         dunder_members = {}
         target_names = set()
         for local, values in node.locals.items():
             if any(not isinstance(value, nodes.AssignName) for value in values):
@@ -373,15 +412,15 @@
                     targets = stmt.targets
             elif isinstance(stmt, nodes.AnnAssign):
                 targets = [stmt.target]
             else:
                 continue
 
             inferred_return_value = None
-            if isinstance(stmt, nodes.Assign):
+            if stmt.value is not None:
                 if isinstance(stmt.value, nodes.Const):
                     if isinstance(stmt.value.value, str):
                         inferred_return_value = repr(stmt.value.value)
                     else:
                         inferred_return_value = stmt.value.value
                 else:
                     inferred_return_value = stmt.value.as_string()
@@ -419,18 +458,32 @@
                 ).string_build(classdef)[target.name]
                 fake.parent = target.parent
                 for method in node.mymethods():
                     fake.locals[method.name] = [method]
                 new_targets.append(fake.instantiate_class())
                 dunder_members[local] = fake
             node.locals[local] = new_targets
+
+        # The undocumented `_value2member_map_` member:
+        node.locals["_value2member_map_"] = [nodes.Dict(parent=node)]
+
         members = nodes.Dict(parent=node)
         members.postinit(
             [
-                (nodes.Const(k, parent=members), nodes.Name(v.name, parent=members))
+                (
+                    nodes.Const(k, parent=members),
+                    nodes.Name(
+                        v.name,
+                        parent=members,
+                        lineno=v.lineno,
+                        col_offset=v.col_offset,
+                        end_lineno=v.end_lineno,
+                        end_col_offset=v.end_col_offset,
+                    ),
+                )
                 for k, v in dunder_members.items()
             ]
         )
         node.locals["__members__"] = [members]
         # The enum.Enum class itself defines two @DynamicClassAttribute data-descriptors
         # "name" and "value" (which we override in the mocked class for each enum member
         # above). When dealing with inference of an arbitrary instance of the enum
@@ -454,16 +507,16 @@
                 "name"
             ]
             node.locals["name"] = [name_dynamicclassattr]
         break
     return node
 
 
-def infer_typing_namedtuple_class(class_node, context=None):
-    """Infer a subclass of typing.NamedTuple"""
+def infer_typing_namedtuple_class(class_node, context: InferenceContext | None = None):
+    """Infer a subclass of typing.NamedTuple."""
     # Check if it has the corresponding bases
     annassigns_fields = [
         annassign.target.name
         for annassign in class_node.body
         if isinstance(annassign, nodes.AnnAssign)
     ]
     code = dedent(
@@ -487,62 +540,92 @@
                 generated_class_node.locals[attr] = class_node.locals[attr]
         elif isinstance(body_node, nodes.ClassDef):
             generated_class_node.locals[body_node.name] = [body_node]
 
     return iter((generated_class_node,))
 
 
-def infer_typing_namedtuple_function(node, context=None):
+def infer_typing_namedtuple_function(node, context: InferenceContext | None = None):
     """
     Starting with python3.9, NamedTuple is a function of the typing module.
     The class NamedTuple is build dynamically through a call to `type` during
     initialization of the `_NamedTuple` variable.
     """
     klass = extract_node(
         """
         from typing import _NamedTuple
         _NamedTuple
         """
     )
     return klass.infer(context)
 
 
-def infer_typing_namedtuple(node, context=None):
+def infer_typing_namedtuple(
+    node: nodes.Call, context: InferenceContext | None = None
+) -> Iterator[nodes.ClassDef]:
     """Infer a typing.NamedTuple(...) call."""
     # This is essentially a namedtuple with different arguments
     # so we extract the args and infer a named tuple.
     try:
         func = next(node.func.infer())
     except (InferenceError, StopIteration) as exc:
         raise UseInferenceDefault from exc
 
-    if func.qname() != "typing.NamedTuple":
+    if func.qname() not in TYPING_NAMEDTUPLE_QUALIFIED:
         raise UseInferenceDefault
 
     if len(node.args) != 2:
         raise UseInferenceDefault
 
     if not isinstance(node.args[1], (nodes.List, nodes.Tuple)):
         raise UseInferenceDefault
 
+    return infer_named_tuple(node, context)
+
+
+def _get_namedtuple_fields(node: nodes.Call) -> str:
+    """Get and return fields of a NamedTuple in code-as-a-string.
+
+    Because the fields are represented in their code form we can
+    extract a node from them later on.
+    """
     names = []
-    for elt in node.args[1].elts:
+    container = None
+    try:
+        container = next(node.args[1].infer())
+    except (InferenceError, StopIteration) as exc:
+        raise UseInferenceDefault from exc
+    # We pass on IndexError as we'll try to infer 'field_names' from the keywords
+    except IndexError:
+        pass
+    if not container:
+        for keyword_node in node.keywords:
+            if keyword_node.arg == "field_names":
+                try:
+                    container = next(keyword_node.value.infer())
+                except (InferenceError, StopIteration) as exc:
+                    raise UseInferenceDefault from exc
+                break
+    if not isinstance(container, nodes.BaseContainer):
+        raise UseInferenceDefault
+    for elt in container.elts:
+        if isinstance(elt, nodes.Const):
+            names.append(elt.as_string())
+            continue
         if not isinstance(elt, (nodes.List, nodes.Tuple)):
             raise UseInferenceDefault
         if len(elt.elts) != 2:
             raise UseInferenceDefault
         names.append(elt.elts[0].as_string())
 
-    typename = node.args[0].as_string()
     if names:
         field_names = f"({','.join(names)},)"
     else:
-        field_names = "''"
-    node = extract_node(f"namedtuple({typename}, {field_names})")
-    return infer_named_tuple(node, context)
+        field_names = ""
+    return field_names
 
 
 def _is_enum_subclass(cls: astroid.ClassDef) -> bool:
     """Return whether cls is a subclass of an Enum."""
     try:
         return any(
             klass.name in ENUM_BASE_NAMES
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_nose.py` & `astroid-3.0.0a1/astroid/brain/brain_nose.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-# Copyright (c) 2015-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Hooks for nose library."""
 
 import re
 import textwrap
 
 import astroid.builder
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.fromnumeric module."""
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.manager import AstroidManager
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_function_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.function_base module."""
 
 import functools
 
 from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
 from astroid.inference_tip import inference_tip
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2019-2020 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.multiarray module."""
 
 import functools
 
 from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
 from astroid.brain.helpers import register_module_extender
@@ -48,18 +43,23 @@
             return numpy.ndarray((0, 0))""",
     "where": """def where(condition, x=None, y=None):
             return numpy.ndarray([0, 0])""",
     "empty": """def empty(shape, dtype=float, order='C'):
             return numpy.ndarray([0, 0])""",
     "bincount": """def bincount(x, weights=None, minlength=0):
             return numpy.ndarray([0, 0])""",
-    "busday_count": """def busday_count(begindates, enddates, weekmask='1111100', holidays=[], busdaycal=None, out=None):
-            return numpy.ndarray([0, 0])""",
-    "busday_offset": """def busday_offset(dates, offsets, roll='raise', weekmask='1111100', holidays=None, busdaycal=None, out=None):
-            return numpy.ndarray([0, 0])""",
+    "busday_count": """def busday_count(
+        begindates, enddates, weekmask='1111100', holidays=[], busdaycal=None, out=None
+    ):
+        return numpy.ndarray([0, 0])""",
+    "busday_offset": """def busday_offset(
+        dates, offsets, roll='raise', weekmask='1111100', holidays=None,
+        busdaycal=None, out=None
+    ):
+        return numpy.ndarray([0, 0])""",
     "can_cast": """def can_cast(from_, to, casting='safe'):
             return True""",
     "copyto": """def copyto(dst, src, casting='same_kind', where=True):
             return None""",
     "datetime_as_string": """def datetime_as_string(arr, unit=None, timezone='naive', casting='same_kind'):
             return numpy.ndarray([0, 0])""",
     "is_busday": """def is_busday(dates, weekmask='1111100', holidays=None, busdaycal=None, out=None):
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_numeric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy.core.numeric module."""
 
 import functools
 
 from astroid.brain.brain_numpy_utils import infer_numpy_member, looks_like_numpy_member
 from astroid.brain.helpers import register_module_extender
@@ -20,17 +15,17 @@
 
 
 def numpy_core_numeric_transform():
     return parse(
         """
     # different functions defined in numeric.py
     import numpy
-    def zeros_like(a, dtype=None, order='K', subok=True): return numpy.ndarray((0, 0))
-    def ones_like(a, dtype=None, order='K', subok=True): return numpy.ndarray((0, 0))
-    def full_like(a, fill_value, dtype=None, order='K', subok=True): return numpy.ndarray((0, 0))
+    def zeros_like(a, dtype=None, order='K', subok=True, shape=None): return numpy.ndarray((0, 0))
+    def ones_like(a, dtype=None, order='K', subok=True, shape=None): return numpy.ndarray((0, 0))
+    def full_like(a, fill_value, dtype=None, order='K', subok=True, shape=None): return numpy.ndarray((0, 0))
         """
     )
 
 
 register_module_extender(
     AstroidManager(), "numpy.core.numeric", numpy_core_numeric_transform
 )
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 # TODO(hippo91) : correct the methods signature.
 
 """Astroid hooks for numpy.core.numerictypes module."""
 from astroid.brain.brain_numpy_utils import numpy_supports_type_hints
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_core_umath.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 # Note: starting with version 1.18 numpy module has `__getattr__` method which prevent
 # `pylint` to emit `no-member` message for all numpy's attributes. (see pylint's module
 # typecheck in `_emit_no_member` function)
 
 """Astroid hooks for numpy.core.umath module."""
 from astroid.brain.helpers import register_module_extender
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_ndarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# Copyright (c) 2015-2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2017-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for numpy ndarray class."""
+from __future__ import annotations
+
 from astroid.brain.brain_numpy_utils import numpy_supports_type_hints
 from astroid.builder import extract_node
+from astroid.context import InferenceContext
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import Attribute
 
 
-def infer_numpy_ndarray(node, context=None):
+def infer_numpy_ndarray(node, context: InferenceContext | None = None):
     ndarray = """
     class ndarray(object):
         def __init__(self, shape, dtype=float, buffer=None, offset=0,
                      strides=None, order=None):
             self.T = numpy.ndarray([0, 0])
             self.base = None
             self.ctypes = None
@@ -150,15 +147,15 @@
         def __class_getitem__(cls, value):
             return cls
         """
     node = extract_node(ndarray)
     return node.infer(context=context)
 
 
-def _looks_like_numpy_ndarray(node):
+def _looks_like_numpy_ndarray(node) -> bool:
     return isinstance(node, Attribute) and node.attrname == "ndarray"
 
 
 AstroidManager().register_transform(
     Attribute,
     inference_tip(infer_numpy_ndarray),
     _looks_like_numpy_ndarray,
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 # TODO(hippo91) : correct the functions return types
 """Astroid hooks for numpy.random.mtrand module."""
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.manager import AstroidManager
```

### Comparing `astroid-2.9.3/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a1/astroid/brain/brain_numpy_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,44 @@
-# Copyright (c) 2019-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2019-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
+"""Different utilities for the numpy brains."""
 
-"""Different utilities for the numpy brains"""
-from typing import Tuple
+from __future__ import annotations
 
 from astroid.builder import extract_node
+from astroid.context import InferenceContext
 from astroid.nodes.node_classes import Attribute, Import, Name, NodeNG
 
 # Class subscript is available in numpy starting with version 1.20.0
 NUMPY_VERSION_TYPE_HINTS_SUPPORT = ("1", "20", "0")
 
 
 def numpy_supports_type_hints() -> bool:
-    """
-    Returns True if numpy supports type hints
-    """
+    """Returns True if numpy supports type hints."""
     np_ver = _get_numpy_version()
     return np_ver and np_ver > NUMPY_VERSION_TYPE_HINTS_SUPPORT
 
 
-def _get_numpy_version() -> Tuple[str, str, str]:
+def _get_numpy_version() -> tuple[str, str, str]:
     """
-    Return the numpy version number if numpy can be imported. Otherwise returns
-    ('0', '0', '0')
+    Return the numpy version number if numpy can be imported.
+
+    Otherwise returns ('0', '0', '0')
     """
     try:
         import numpy  # pylint: disable=import-outside-toplevel
 
         return tuple(numpy.version.version.split("."))
-    except ImportError:
+    except (ImportError, AttributeError):
         return ("0", "0", "0")
 
 
-def infer_numpy_member(src, node, context=None):
+def infer_numpy_member(src, node, context: InferenceContext | None = None):
     node = extract_node(src)
     return node.infer(context=context)
 
 
 def _is_a_numpy_module(node: Name) -> bool:
     """
     Returns True if the node is a representation of a numpy module.
```

### Comparing `astroid-2.9.3/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a1/astroid/brain/brain_pkg_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2016, 2018 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 from astroid import parse
 from astroid.brain.helpers import register_module_extender
 from astroid.manager import AstroidManager
 
 
 def pkg_resources_transform():
```

### Comparing `astroid-2.9.3/astroid/brain/brain_qt.py` & `astroid-3.0.0a1/astroid/brain/brain_qt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# Copyright (c) 2015-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2017 Roy Wright <roy@wright.org>
-# Copyright (c) 2018 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2019 Antoine Boellinger <aboellinger@hotmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for the PyQT library."""
 
 from astroid import nodes, parse
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import AstroidBuilder
 from astroid.manager import AstroidManager
 
 
-def _looks_like_signal(node, signal_name="pyqtSignal"):
-    if "__class__" in node.instance_attrs:
+def _looks_like_signal(
+    node: nodes.FunctionDef, signal_name: str = "pyqtSignal"
+) -> bool:
+    """Detect a Signal node."""
+    klasses = node.instance_attrs.get("__class__", [])
+    # On PySide2 or PySide6 (since  Qt 5.15.2) the Signal class changed locations
+    if node.qname().partition(".")[0] in {"PySide2", "PySide6"}:
+        return any(cls.qname() == "Signal" for cls in klasses)  # pragma: no cover
+    if klasses:
         try:
-            cls = node.instance_attrs["__class__"][0]
-            return cls.name == signal_name
-        except AttributeError:
+            return klasses[0].name == signal_name
+        except AttributeError:  # pragma: no cover
             # return False if the cls does not have a name attribute
             pass
     return False
 
 
-def transform_pyqt_signal(node):
+def transform_pyqt_signal(node: nodes.FunctionDef) -> None:
     module = parse(
         """
+    _UNSET = object()
+
     class pyqtSignal(object):
         def connect(self, slot, type=None, no_receiver_check=False):
             pass
-        def disconnect(self, slot):
+        def disconnect(self, slot=_UNSET):
             pass
         def emit(self, *args):
             pass
     """
     )
-    signal_cls = module["pyqtSignal"]
-    node.instance_attrs["emit"] = signal_cls["emit"]
-    node.instance_attrs["disconnect"] = signal_cls["disconnect"]
-    node.instance_attrs["connect"] = signal_cls["connect"]
+    signal_cls: nodes.ClassDef = module["pyqtSignal"]
+    node.instance_attrs["emit"] = [signal_cls["emit"]]
+    node.instance_attrs["disconnect"] = [signal_cls["disconnect"]]
+    node.instance_attrs["connect"] = [signal_cls["connect"]]
 
 
-def transform_pyside_signal(node):
+def transform_pyside_signal(node: nodes.FunctionDef) -> None:
     module = parse(
         """
     class NotPySideSignal(object):
         def connect(self, receiver, type=None):
             pass
         def disconnect(self, receiver):
             pass
         def emit(self, *args):
             pass
     """
     )
-    signal_cls = module["NotPySideSignal"]
-    node.instance_attrs["connect"] = signal_cls["connect"]
-    node.instance_attrs["disconnect"] = signal_cls["disconnect"]
-    node.instance_attrs["emit"] = signal_cls["emit"]
+    signal_cls: nodes.ClassDef = module["NotPySideSignal"]
+    node.instance_attrs["connect"] = [signal_cls["connect"]]
+    node.instance_attrs["disconnect"] = [signal_cls["disconnect"]]
+    node.instance_attrs["emit"] = [signal_cls["emit"]]
 
 
 def pyqt4_qtcore_transform():
     return AstroidBuilder(AstroidManager()).string_build(
         """
 
 def SIGNAL(signal_name): pass
```

### Comparing `astroid-2.9.3/astroid/brain/brain_random.py` & `astroid-3.0.0a1/astroid/brain/brain_random.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
+
 import random
 
 from astroid import helpers
+from astroid.context import InferenceContext
 from astroid.exceptions import UseInferenceDefault
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import (
     Attribute,
     Call,
     Const,
@@ -22,60 +27,72 @@
 
 def _clone_node_with_lineno(node, parent, lineno):
     if isinstance(node, EvaluatedObject):
         node = node.original
     cls = node.__class__
     other_fields = node._other_fields
     _astroid_fields = node._astroid_fields
-    init_params = {"lineno": lineno, "col_offset": node.col_offset, "parent": parent}
+    init_params = {
+        "lineno": lineno,
+        "col_offset": node.col_offset,
+        "parent": parent,
+        "end_lineno": node.end_lineno,
+        "end_col_offset": node.end_col_offset,
+    }
     postinit_params = {param: getattr(node, param) for param in _astroid_fields}
     if other_fields:
         init_params.update({param: getattr(node, param) for param in other_fields})
     new_node = cls(**init_params)
     if hasattr(node, "postinit") and _astroid_fields:
         new_node.postinit(**postinit_params)
     return new_node
 
 
-def infer_random_sample(node, context=None):
+def infer_random_sample(node, context: InferenceContext | None = None):
     if len(node.args) != 2:
         raise UseInferenceDefault
 
-    length = node.args[1]
-    if not isinstance(length, Const):
+    inferred_length = helpers.safe_infer(node.args[1], context=context)
+    if not isinstance(inferred_length, Const):
         raise UseInferenceDefault
-    if not isinstance(length.value, int):
+    if not isinstance(inferred_length.value, int):
         raise UseInferenceDefault
 
     inferred_sequence = helpers.safe_infer(node.args[0], context=context)
     if not inferred_sequence:
         raise UseInferenceDefault
 
     if not isinstance(inferred_sequence, ACCEPTED_ITERABLES_FOR_SAMPLE):
         raise UseInferenceDefault
 
-    if length.value > len(inferred_sequence.elts):
+    if inferred_length.value > len(inferred_sequence.elts):
         # In this case, this will raise a ValueError
         raise UseInferenceDefault
 
     try:
-        elts = random.sample(inferred_sequence.elts, length.value)
+        elts = random.sample(inferred_sequence.elts, inferred_length.value)
     except ValueError as exc:
         raise UseInferenceDefault from exc
 
-    new_node = List(lineno=node.lineno, col_offset=node.col_offset, parent=node.scope())
+    new_node = List(
+        lineno=node.lineno,
+        col_offset=node.col_offset,
+        parent=node.scope(),
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
+    )
     new_elts = [
         _clone_node_with_lineno(elt, parent=new_node, lineno=new_node.lineno)
         for elt in elts
     ]
     new_node.postinit(new_elts)
     return iter((new_node,))
 
 
-def _looks_like_random_sample(node):
+def _looks_like_random_sample(node) -> bool:
     func = node.func
     if isinstance(func, Attribute):
         return func.attrname == "sample"
     if isinstance(func, Name):
         return func.name == "sample"
     return False
```

### Comparing `astroid-2.9.3/astroid/brain/brain_re.py` & `astroid-3.0.0a1/astroid/brain/brain_re.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-from typing import Optional
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
 
 from astroid import context, inference_tip, nodes
 from astroid.brain.helpers import register_module_extender
-from astroid.builder import extract_node, parse
-from astroid.const import PY37_PLUS, PY39_PLUS
+from astroid.builder import _extract_single_node, parse
+from astroid.const import PY39_PLUS, PY311_PLUS
 from astroid.manager import AstroidManager
 
 
-def _re_transform():
-    # Since Python 3.6 there is the RegexFlag enum
-    # where every entry will be exposed via updating globals()
+def _re_transform() -> nodes.Module:
+    # The RegexFlag enum exposes all its entries by updating globals()
+    # In 3.6-3.10 all flags come from sre_compile
+    # On 3.11+ all flags come from re._compiler
+    if PY311_PLUS:
+        import_compiler = "import re._compiler as _compiler"
+    else:
+        import_compiler = "import sre_compile as _compiler"
     return parse(
-        """
-    import sre_compile
-    ASCII = sre_compile.SRE_FLAG_ASCII
-    IGNORECASE = sre_compile.SRE_FLAG_IGNORECASE
-    LOCALE = sre_compile.SRE_FLAG_LOCALE
-    UNICODE = sre_compile.SRE_FLAG_UNICODE
-    MULTILINE = sre_compile.SRE_FLAG_MULTILINE
-    DOTALL = sre_compile.SRE_FLAG_DOTALL
-    VERBOSE = sre_compile.SRE_FLAG_VERBOSE
+        f"""
+    {import_compiler}
+    NOFLAG = 0
+    ASCII = _compiler.SRE_FLAG_ASCII
+    IGNORECASE = _compiler.SRE_FLAG_IGNORECASE
+    LOCALE = _compiler.SRE_FLAG_LOCALE
+    UNICODE = _compiler.SRE_FLAG_UNICODE
+    MULTILINE = _compiler.SRE_FLAG_MULTILINE
+    DOTALL = _compiler.SRE_FLAG_DOTALL
+    VERBOSE = _compiler.SRE_FLAG_VERBOSE
+    TEMPLATE = _compiler.SRE_FLAG_TEMPLATE
+    DEBUG = _compiler.SRE_FLAG_DEBUG
     A = ASCII
     I = IGNORECASE
     L = LOCALE
     U = UNICODE
     M = MULTILINE
     S = DOTALL
     X = VERBOSE
-    TEMPLATE = sre_compile.SRE_FLAG_TEMPLATE
     T = TEMPLATE
-    DEBUG = sre_compile.SRE_FLAG_DEBUG
     """
     )
 
 
 register_module_extender(AstroidManager(), "re", _re_transform)
 
 
@@ -62,27 +70,29 @@
         and isinstance(node.parent, nodes.Assign)
         and len(node.parent.targets) == 1
         and isinstance(node.parent.targets[0], nodes.AssignName)
         and node.parent.targets[0].name in {"Pattern", "Match"}
     )
 
 
-def infer_pattern_match(
-    node: nodes.Call, ctx: Optional[context.InferenceContext] = None
-):
-    """Infer re.Pattern and re.Match as classes. For PY39+ add `__class_getitem__`."""
+def infer_pattern_match(node: nodes.Call, ctx: context.InferenceContext | None = None):
+    """Infer re.Pattern and re.Match as classes.
+
+    For PY39+ add `__class_getitem__`.
+    """
     class_def = nodes.ClassDef(
         name=node.parent.targets[0].name,
         lineno=node.lineno,
         col_offset=node.col_offset,
         parent=node.parent,
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
     )
     if PY39_PLUS:
-        func_to_add = extract_node(CLASS_GETITEM_TEMPLATE)
+        func_to_add = _extract_single_node(CLASS_GETITEM_TEMPLATE)
         class_def.locals["__class_getitem__"] = [func_to_add]
     return iter([class_def])
 
 
-if PY37_PLUS:
-    AstroidManager().register_transform(
-        nodes.Call, inference_tip(infer_pattern_match), _looks_like_pattern_or_match
-    )
+AstroidManager().register_transform(
+    nodes.Call, inference_tip(infer_pattern_match), _looks_like_pattern_or_match
+)
```

### Comparing `astroid-2.9.3/astroid/brain/brain_responses.py` & `astroid-3.0.0a1/astroid/brain/brain_responses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """
 Astroid hooks for responses.
 
 It might need to be manually updated from the public methods of
 :class:`responses.RequestsMock`.
 
 See: https://github.com/getsentry/responses/blob/master/responses.py
-
 """
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.manager import AstroidManager
 
 
 def responses_funcs():
```

### Comparing `astroid-2.9.3/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a1/astroid/brain/brain_scipy_signal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,88 @@
-# Copyright (c) 2019 Valentin Valls <valentin.valls@esrf.fr>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
-# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
-
-"""Astroid hooks for scipy.signal module."""
-from astroid.brain.helpers import register_module_extender
-from astroid.builder import parse
-from astroid.manager import AstroidManager
-
-
-def scipy_signal():
-    return parse(
-        """
-    # different functions defined in scipy.signals
-
-    def barthann(M, sym=True):
-        return numpy.ndarray([0])
-
-    def bartlett(M, sym=True):
-        return numpy.ndarray([0])
-
-    def blackman(M, sym=True):
-        return numpy.ndarray([0])
-
-    def blackmanharris(M, sym=True):
-        return numpy.ndarray([0])
-
-    def bohman(M, sym=True):
-        return numpy.ndarray([0])
-
-    def boxcar(M, sym=True):
-        return numpy.ndarray([0])
-
-    def chebwin(M, at, sym=True):
-        return numpy.ndarray([0])
-
-    def cosine(M, sym=True):
-        return numpy.ndarray([0])
-
-    def exponential(M, center=None, tau=1.0, sym=True):
-        return numpy.ndarray([0])
-
-    def flattop(M, sym=True):
-        return numpy.ndarray([0])
-
-    def gaussian(M, std, sym=True):
-        return numpy.ndarray([0])
-
-    def general_gaussian(M, p, sig, sym=True):
-        return numpy.ndarray([0])
-
-    def hamming(M, sym=True):
-        return numpy.ndarray([0])
-
-    def hann(M, sym=True):
-        return numpy.ndarray([0])
-
-    def hanning(M, sym=True):
-        return numpy.ndarray([0])
-
-    def impulse2(system, X0=None, T=None, N=None, **kwargs):
-        return numpy.ndarray([0]), numpy.ndarray([0])
-
-    def kaiser(M, beta, sym=True):
-        return numpy.ndarray([0])
-
-    def nuttall(M, sym=True):
-        return numpy.ndarray([0])
-
-    def parzen(M, sym=True):
-        return numpy.ndarray([0])
-
-    def slepian(M, width, sym=True):
-        return numpy.ndarray([0])
-
-    def step2(system, X0=None, T=None, N=None, **kwargs):
-        return numpy.ndarray([0]), numpy.ndarray([0])
-
-    def triang(M, sym=True):
-        return numpy.ndarray([0])
-
-    def tukey(M, alpha=0.5, sym=True):
-        return numpy.ndarray([0])
-        """
-    )
-
-
-register_module_extender(AstroidManager(), "scipy.signal", scipy_signal)
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+"""Astroid hooks for scipy.signal module."""
+from astroid.brain.helpers import register_module_extender
+from astroid.builder import parse
+from astroid.manager import AstroidManager
+
+
+def scipy_signal():
+    return parse(
+        """
+    # different functions defined in scipy.signals
+
+    def barthann(M, sym=True):
+        return numpy.ndarray([0])
+
+    def bartlett(M, sym=True):
+        return numpy.ndarray([0])
+
+    def blackman(M, sym=True):
+        return numpy.ndarray([0])
+
+    def blackmanharris(M, sym=True):
+        return numpy.ndarray([0])
+
+    def bohman(M, sym=True):
+        return numpy.ndarray([0])
+
+    def boxcar(M, sym=True):
+        return numpy.ndarray([0])
+
+    def chebwin(M, at, sym=True):
+        return numpy.ndarray([0])
+
+    def cosine(M, sym=True):
+        return numpy.ndarray([0])
+
+    def exponential(M, center=None, tau=1.0, sym=True):
+        return numpy.ndarray([0])
+
+    def flattop(M, sym=True):
+        return numpy.ndarray([0])
+
+    def gaussian(M, std, sym=True):
+        return numpy.ndarray([0])
+
+    def general_gaussian(M, p, sig, sym=True):
+        return numpy.ndarray([0])
+
+    def hamming(M, sym=True):
+        return numpy.ndarray([0])
+
+    def hann(M, sym=True):
+        return numpy.ndarray([0])
+
+    def hanning(M, sym=True):
+        return numpy.ndarray([0])
+
+    def impulse2(system, X0=None, T=None, N=None, **kwargs):
+        return numpy.ndarray([0]), numpy.ndarray([0])
+
+    def kaiser(M, beta, sym=True):
+        return numpy.ndarray([0])
+
+    def nuttall(M, sym=True):
+        return numpy.ndarray([0])
+
+    def parzen(M, sym=True):
+        return numpy.ndarray([0])
+
+    def slepian(M, width, sym=True):
+        return numpy.ndarray([0])
+
+    def step2(system, X0=None, T=None, N=None, **kwargs):
+        return numpy.ndarray([0]), numpy.ndarray([0])
+
+    def triang(M, sym=True):
+        return numpy.ndarray([0])
+
+    def tukey(M, alpha=0.5, sym=True):
+        return numpy.ndarray([0])
+        """
+    )
+
+
+register_module_extender(AstroidManager(), "scipy.signal", scipy_signal)
```

### Comparing `astroid-2.9.3/astroid/brain/brain_signal.py` & `astroid-3.0.0a1/astroid/brain/brain_signal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """Astroid hooks for the signal library.
 
 The signal module generates the 'Signals', 'Handlers' and 'Sigmasks' IntEnums
 dynamically using the IntEnum._convert() classmethod, which modifies the module
 globals. Astroid is unable to handle this type of code.
 
 Without these hooks, the following are erroneously triggered by Pylint:
@@ -31,15 +33,15 @@
 
 
 def _signals_enums_transform():
     """Generates the AST for 'Signals', 'Handlers' and 'Sigmasks' IntEnums."""
     return parse(_signals_enum() + _handlers_enum() + _sigmasks_enum())
 
 
-def _signals_enum():
+def _signals_enum() -> str:
     """Generates the source code for the Signals int enum."""
     signals_enum = """
     import enum
     class Signals(enum.IntEnum):
         SIGABRT   = enum.auto()
         SIGEMT    = enum.auto()
         SIGFPE    = enum.auto()
@@ -87,25 +89,25 @@
         SIGPWR    = enum.auto()
         SIGRTMAX  = enum.auto()
         SIGRTMIN  = enum.auto()
         """
     return signals_enum
 
 
-def _handlers_enum():
+def _handlers_enum() -> str:
     """Generates the source code for the Handlers int enum."""
     return """
     import enum
     class Handlers(enum.IntEnum):
         SIG_DFL = enum.auto()
         SIG_IGN = eunm.auto()
     """
 
 
-def _sigmasks_enum():
+def _sigmasks_enum() -> str:
     """Generates the source code for the Sigmasks int enum."""
     if sys.platform != "win32":
         return """
     import enum
     class Sigmasks(enum.IntEnum):
         SIG_BLOCK   = enum.auto()
         SIG_UNBLOCK = enum.auto()
```

### Comparing `astroid-2.9.3/astroid/brain/brain_six.py` & `astroid-3.0.0a1/astroid/brain/brain_six.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,10 @@
-# Copyright (c) 2014-2016, 2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Ram Rachum <ram@rachum.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Artsiom Kaval <lezeroq@gmail.com>
-# Copyright (c) 2021 Francis Charette Migneault <francis.charette.migneault@gmail.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for six module."""
 
 from textwrap import dedent
 
 from astroid import nodes
 from astroid.brain.helpers import register_module_extender
@@ -30,15 +20,15 @@
 SIX_WITH_METACLASS = "six.with_metaclass"
 
 
 def default_predicate(line):
     return line.strip()
 
 
-def _indent(text, prefix, predicate=default_predicate):
+def _indent(text, prefix, predicate=default_predicate) -> str:
     """Adds 'prefix' to the beginning of selected lines in 'text'.
 
     If 'predicate' is provided, 'prefix' will only be added to the lines
     where 'predicate(line)' is True. If 'predicate' is not provided,
     it will default to adding 'prefix' to all non-empty lines that do not
     consist solely of whitespace characters.
     """
@@ -160,28 +150,28 @@
             submodule = AstroidManager().ast_from_module_name(import_attr.names[0][0])
             return submodule
     # Let dummy submodule imports pass through
     # This will cause an Uninferable result, which is okay
     return module
 
 
-def _looks_like_decorated_with_six_add_metaclass(node):
+def _looks_like_decorated_with_six_add_metaclass(node) -> bool:
     if not node.decorators:
         return False
 
     for decorator in node.decorators.nodes:
         if not isinstance(decorator, nodes.Call):
             continue
         if decorator.func.as_string() == SIX_ADD_METACLASS:
             return True
     return False
 
 
 def transform_six_add_metaclass(node):  # pylint: disable=inconsistent-return-statements
-    """Check if the given class node is decorated with *six.add_metaclass*
+    """Check if the given class node is decorated with *six.add_metaclass*.
 
     If so, inject its argument as the metaclass of the underlying class.
     """
     if not node.decorators:
         return
 
     for decorator in node.decorators.nodes:
@@ -195,15 +185,15 @@
         if func.qname() == SIX_ADD_METACLASS and decorator.args:
             metaclass = decorator.args[0]
             node._metaclass = metaclass
             return node
     return
 
 
-def _looks_like_nested_from_six_with_metaclass(node):
+def _looks_like_nested_from_six_with_metaclass(node) -> bool:
     if len(node.bases) != 1:
         return False
     base = node.bases[0]
     if not isinstance(base, nodes.Call):
         return False
     try:
         if hasattr(base.func, "expr"):
@@ -219,15 +209,15 @@
             func = f"{import_from.modname}.{base.func.name}"
     except (AttributeError, KeyError, IndexError):
         return False
     return func == SIX_WITH_METACLASS
 
 
 def transform_six_with_metaclass(node):
-    """Check if the given class node is defined with *six.with_metaclass*
+    """Check if the given class node is defined with *six.with_metaclass*.
 
     If so, inject its argument as the metaclass of the underlying class.
     """
     call = node.bases[0]
     node._metaclass = call.args[0]
     return node
```

### Comparing `astroid-2.9.3/astroid/brain/brain_threading.py` & `astroid-3.0.0a1/astroid/brain/brain_threading.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# Copyright (c) 2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import parse
 from astroid.manager import AstroidManager
 
 
 def _thread_transform():
@@ -23,14 +18,14 @@
         def __enter__(self):
             return True
         def __exit__(self, *args):
             pass
         def locked(self):
             return False
 
-    def Lock():
+    def Lock(*args, **kwargs):
         return lock()
     """
     )
 
 
 register_module_extender(AstroidManager(), "threading", _thread_transform)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/brain/brain_type.py` & `astroid-3.0.0a1/astroid/brain/brain_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """
 Astroid hooks for type support.
 
 Starting from python3.9, type object behaves as it had __class_getitem__ method.
 However it was not possible to simply add this method inside type's body, otherwise
 all types would also have this method. In this case it would have been possible
 to write str[int].
@@ -12,42 +16,42 @@
 to the type object. Instead we choose to add it only in the case of a subscript node
 which inside name node is type.
 Doing this type[int] is allowed whereas str[int] is not.
 
 Thanks to Lukasz Langa for fruitful discussion.
 """
 
+from __future__ import annotations
+
 from astroid import extract_node, inference_tip, nodes
 from astroid.const import PY39_PLUS
+from astroid.context import InferenceContext
 from astroid.exceptions import UseInferenceDefault
 from astroid.manager import AstroidManager
 
 
-def _looks_like_type_subscript(node):
+def _looks_like_type_subscript(node) -> bool:
     """
-    Try to figure out if a Name node is used inside a type related subscript
+    Try to figure out if a Name node is used inside a type related subscript.
 
     :param node: node to check
     :type node: astroid.nodes.node_classes.NodeNG
-    :return: true if the node is a Name node inside a type related subscript
-    :rtype: bool
+    :return: whether the node is a Name node inside a type related subscript
     """
     if isinstance(node, nodes.Name) and isinstance(node.parent, nodes.Subscript):
         return node.name == "type"
     return False
 
 
-def infer_type_sub(node, context=None):
+def infer_type_sub(node, context: InferenceContext | None = None):
     """
-    Infer a type[...] subscript
+    Infer a type[...] subscript.
 
     :param node: node to infer
     :type node: astroid.nodes.node_classes.NodeNG
-    :param context: inference context
-    :type context: astroid.context.InferenceContext
     :return: the inferred node
     :rtype: nodes.NodeNG
     """
     node_scope, _ = node.scope().lookup("type")
     if not isinstance(node_scope, nodes.Module) or node_scope.qname() != "builtins":
         raise UseInferenceDefault()
     class_src = """
```

### Comparing `astroid-2.9.3/astroid/brain/brain_typing.py` & `astroid-3.0.0a1/astroid/objects.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,438 +1,373 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-# Copyright (c) 2017-2018 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 David Euresti <github@euresti.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Redoubts <Redoubts@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Tim Martin <tim@asymptotic.co.uk>
-# Copyright (c) 2021 hippo91 <guillaume.peillex@gmail.com>
-
-"""Astroid hooks for typing.py support."""
-import typing
-from functools import partial
+"""
+Inference objects are a way to represent composite AST nodes,
+which are used only as inference results, so they can't be found in the
+original AST tree. For instance, inferring the following frozenset use,
+leads to an inferred FrozenSet:
+
+    Call(func=Name('frozenset'), args=Tuple(...))
+"""
+
+from __future__ import annotations
+
+from collections.abc import Generator, Iterator
+from functools import cached_property
+from typing import Any, Literal, NoReturn, TypeVar
 
-from astroid import context, extract_node, inference_tip
-from astroid.const import PY37_PLUS, PY38_PLUS, PY39_PLUS
+from astroid import bases, decorators, util
+from astroid.context import InferenceContext
 from astroid.exceptions import (
     AttributeInferenceError,
     InferenceError,
-    UseInferenceDefault,
+    MroError,
+    SuperError,
 )
+from astroid.interpreter import objectmodel
 from astroid.manager import AstroidManager
-from astroid.nodes.node_classes import (
-    Assign,
-    AssignName,
-    Attribute,
-    Call,
-    Const,
-    Name,
-    NodeNG,
-    Subscript,
-    Tuple,
-)
-from astroid.nodes.scoped_nodes import ClassDef, FunctionDef
-from astroid.util import Uninferable
+from astroid.nodes import node_classes, scoped_nodes
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
-TYPING_NAMEDTUPLE_BASENAMES = {"NamedTuple", "typing.NamedTuple"}
-TYPING_TYPEVARS = {"TypeVar", "NewType"}
-TYPING_TYPEVARS_QUALIFIED = {"typing.TypeVar", "typing.NewType"}
-TYPING_TYPE_TEMPLATE = """
-class Meta(type):
-    def __getitem__(self, item):
-        return self
+_T = TypeVar("_T")
 
-    @property
-    def __args__(self):
-        return ()
 
-class {0}(metaclass=Meta):
-    pass
-"""
-TYPING_MEMBERS = set(getattr(typing, "__all__", []))
+class FrozenSet(node_classes.BaseContainer):
+    """Class representing a FrozenSet composite node."""
 
-TYPING_ALIAS = frozenset(
-    (
-        "typing.Hashable",
-        "typing.Awaitable",
-        "typing.Coroutine",
-        "typing.AsyncIterable",
-        "typing.AsyncIterator",
-        "typing.Iterable",
-        "typing.Iterator",
-        "typing.Reversible",
-        "typing.Sized",
-        "typing.Container",
-        "typing.Collection",
-        "typing.Callable",
-        "typing.AbstractSet",
-        "typing.MutableSet",
-        "typing.Mapping",
-        "typing.MutableMapping",
-        "typing.Sequence",
-        "typing.MutableSequence",
-        "typing.ByteString",
-        "typing.Tuple",
-        "typing.List",
-        "typing.Deque",
-        "typing.Set",
-        "typing.FrozenSet",
-        "typing.MappingView",
-        "typing.KeysView",
-        "typing.ItemsView",
-        "typing.ValuesView",
-        "typing.ContextManager",
-        "typing.AsyncContextManager",
-        "typing.Dict",
-        "typing.DefaultDict",
-        "typing.OrderedDict",
-        "typing.Counter",
-        "typing.ChainMap",
-        "typing.Generator",
-        "typing.AsyncGenerator",
-        "typing.Type",
-        "typing.Pattern",
-        "typing.Match",
-    )
-)
+    def pytype(self) -> Literal["builtins.frozenset"]:
+        return "builtins.frozenset"
 
-CLASS_GETITEM_TEMPLATE = """
-@classmethod
-def __class_getitem__(cls, item):
-    return cls
-"""
+    def _infer(self, context: InferenceContext | None = None, **kwargs: Any):
+        yield self
 
+    @cached_property
+    def _proxied(self):  # pylint: disable=method-hidden
+        ast_builtins = AstroidManager().builtins_module
+        return ast_builtins.getattr("frozenset")[0]
 
-def looks_like_typing_typevar_or_newtype(node):
-    func = node.func
-    if isinstance(func, Attribute):
-        return func.attrname in TYPING_TYPEVARS
-    if isinstance(func, Name):
-        return func.name in TYPING_TYPEVARS
-    return False
-
-
-def infer_typing_typevar_or_newtype(node, context_itton=None):
-    """Infer a typing.TypeVar(...) or typing.NewType(...) call"""
-    try:
-        func = next(node.func.infer(context=context_itton))
-    except (InferenceError, StopIteration) as exc:
-        raise UseInferenceDefault from exc
-
-    if func.qname() not in TYPING_TYPEVARS_QUALIFIED:
-        raise UseInferenceDefault
-    if not node.args:
-        raise UseInferenceDefault
-
-    typename = node.args[0].as_string().strip("'")
-    node = extract_node(TYPING_TYPE_TEMPLATE.format(typename))
-    return node.infer(context=context_itton)
-
-
-def _looks_like_typing_subscript(node):
-    """Try to figure out if a Subscript node *might* be a typing-related subscript"""
-    if isinstance(node, Name):
-        return node.name in TYPING_MEMBERS
-    if isinstance(node, Attribute):
-        return node.attrname in TYPING_MEMBERS
-    if isinstance(node, Subscript):
-        return _looks_like_typing_subscript(node.value)
-    return False
-
-
-def infer_typing_attr(
-    node: Subscript, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[ClassDef]:
-    """Infer a typing.X[...] subscript"""
-    try:
-        value = next(node.value.infer())
-    except (InferenceError, StopIteration) as exc:
-        raise UseInferenceDefault from exc
-
-    if (
-        not value.qname().startswith("typing.")
-        or PY37_PLUS
-        and value.qname() in TYPING_ALIAS
-    ):
-        # If typing subscript belongs to an alias
-        # (PY37+) handle it separately.
-        raise UseInferenceDefault
-
-    if (
-        PY37_PLUS
-        and isinstance(value, ClassDef)
-        and value.qname()
-        in {"typing.Generic", "typing.Annotated", "typing_extensions.Annotated"}
-    ):
-        # With PY37+ typing.Generic and typing.Annotated (PY39) are subscriptable
-        # through __class_getitem__. Since astroid can't easily
-        # infer the native methods, replace them for an easy inference tip
-        func_to_add = extract_node(CLASS_GETITEM_TEMPLATE)
-        value.locals["__class_getitem__"] = [func_to_add]
-        if (
-            isinstance(node.parent, ClassDef)
-            and node in node.parent.bases
-            and getattr(node.parent, "__cache", None)
-        ):
-            # node.parent.slots is evaluated and cached before the inference tip
-            # is first applied. Remove the last result to allow a recalculation of slots
-            cache = node.parent.__cache  # type: ignore[attr-defined] # Unrecognized getattr
-            if cache.get(node.parent.slots) is not None:
-                del cache[node.parent.slots]
-        return iter([value])
-
-    node = extract_node(TYPING_TYPE_TEMPLATE.format(value.qname().split(".")[-1]))
-    return node.infer(context=ctx)
-
-
-def _looks_like_typedDict(  # pylint: disable=invalid-name
-    node: typing.Union[FunctionDef, ClassDef],
-) -> bool:
-    """Check if node is TypedDict FunctionDef."""
-    return node.qname() in {"typing.TypedDict", "typing_extensions.TypedDict"}
-
-
-def infer_old_typedDict(  # pylint: disable=invalid-name
-    node: ClassDef, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[ClassDef]:
-    func_to_add = extract_node("dict")
-    node.locals["__call__"] = [func_to_add]
-    return iter([node])
-
-
-def infer_typedDict(  # pylint: disable=invalid-name
-    node: FunctionDef, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[ClassDef]:
-    """Replace TypedDict FunctionDef with ClassDef."""
-    class_def = ClassDef(
-        name="TypedDict",
-        lineno=node.lineno,
-        col_offset=node.col_offset,
-        parent=node.parent,
-    )
-    class_def.postinit(bases=[extract_node("dict")], body=[], decorators=None)
-    func_to_add = extract_node("dict")
-    class_def.locals["__call__"] = [func_to_add]
-    return iter([class_def])
 
+class Super(node_classes.NodeNG):
+    """Proxy class over a super call.
 
-def _looks_like_typing_alias(node: Call) -> bool:
+    This class offers almost the same behaviour as Python's super,
+    which is MRO lookups for retrieving attributes from the parents.
+
+    The *mro_pointer* is the place in the MRO from where we should
+    start looking, not counting it. *mro_type* is the object which
+    provides the MRO, it can be both a type or an instance.
+    *self_class* is the class where the super call is, while
+    *scope* is the function where the super call is.
     """
-    Returns True if the node corresponds to a call to _alias function.
-    For example :
 
-    MutableSet = _alias(collections.abc.MutableSet, T)
+    special_attributes = objectmodel.SuperModel()
 
-    :param node: call node
-    """
-    return (
-        isinstance(node.func, Name)
-        and node.func.name == "_alias"
-        and (
-            # _alias function works also for builtins object such as list and dict
-            isinstance(node.args[0], (Attribute, Name))
+    def __init__(
+        self,
+        mro_pointer: SuccessfulInferenceResult,
+        mro_type: SuccessfulInferenceResult,
+        self_class: scoped_nodes.ClassDef,
+        scope: scoped_nodes.FunctionDef,
+        call: node_classes.Call,
+    ) -> None:
+        self.type = mro_type
+        self.mro_pointer = mro_pointer
+        self._class_based = False
+        self._self_class = self_class
+        self._scope = scope
+        super().__init__(
+            parent=scope,
+            lineno=scope.lineno,
+            col_offset=scope.col_offset,
+            end_lineno=scope.end_lineno,
+            end_col_offset=scope.end_col_offset,
         )
-    )
 
+    def _infer(self, context: InferenceContext | None = None, **kwargs: Any):
+        yield self
 
-def _forbid_class_getitem_access(node: ClassDef) -> None:
-    """
-    Disable the access to __class_getitem__ method for the node in parameters
-    """
+    def super_mro(self):
+        """Get the MRO which will be used to lookup attributes in this super."""
+        if not isinstance(self.mro_pointer, scoped_nodes.ClassDef):
+            raise SuperError(
+                "The first argument to super must be a subtype of "
+                "type, not {mro_pointer}.",
+                super_=self,
+            )
+
+        if isinstance(self.type, scoped_nodes.ClassDef):
+            # `super(type, type)`, most likely in a class method.
+            self._class_based = True
+            mro_type = self.type
+        else:
+            mro_type = getattr(self.type, "_proxied", None)
+            if not isinstance(mro_type, (bases.Instance, scoped_nodes.ClassDef)):
+                raise SuperError(
+                    "The second argument to super must be an "
+                    "instance or subtype of type, not {type}.",
+                    super_=self,
+                )
+
+        if not mro_type.newstyle:
+            raise SuperError("Unable to call super on old-style classes.", super_=self)
+
+        mro = mro_type.mro()
+        if self.mro_pointer not in mro:
+            raise SuperError(
+                "The second argument to super must be an "
+                "instance or subtype of type, not {type}.",
+                super_=self,
+            )
+
+        index = mro.index(self.mro_pointer)
+        return mro[index + 1 :]
+
+    @cached_property
+    def _proxied(self):
+        ast_builtins = AstroidManager().builtins_module
+        return ast_builtins.getattr("super")[0]
+
+    def pytype(self) -> Literal["builtins.super"]:
+        return "builtins.super"
+
+    def display_type(self) -> str:
+        return "Super of"
 
-    def full_raiser(origin_func, attr, *args, **kwargs):
-        """
-        Raises an AttributeInferenceError in case of access to __class_getitem__ method.
-        Otherwise just call origin_func.
-        """
-        if attr == "__class_getitem__":
-            raise AttributeInferenceError("__class_getitem__ access is not allowed")
-        return origin_func(attr, *args, **kwargs)
-
-    try:
-        node.getattr("__class_getitem__")
-        # If we are here, then we are sure to modify object that do have __class_getitem__ method (which origin is one the
-        # protocol defined in collections module) whereas the typing module consider it should not
-        # We do not want __class_getitem__ to be found in the classdef
-        partial_raiser = partial(full_raiser, node.getattr)
-        node.getattr = partial_raiser
-    except AttributeInferenceError:
-        pass
-
-
-def infer_typing_alias(
-    node: Call, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[ClassDef]:
+    @property
+    def name(self):
+        """Get the name of the MRO pointer."""
+        return self.mro_pointer.name
+
+    def qname(self) -> Literal["super"]:
+        return "super"
+
+    def igetattr(  # noqa: C901
+        self, name: str, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
+        """Retrieve the inferred values of the given attribute name."""
+        # '__class__' is a special attribute that should be taken directly
+        # from the special attributes dict
+        if name == "__class__":
+            yield self.special_attributes.lookup(name)
+            return
+
+        try:
+            mro = self.super_mro()
+        # Don't let invalid MROs or invalid super calls
+        # leak out as is from this function.
+        except SuperError as exc:
+            raise AttributeInferenceError(
+                (
+                    "Lookup for {name} on {target!r} because super call {super!r} "
+                    "is invalid."
+                ),
+                target=self,
+                attribute=name,
+                context=context,
+                super_=exc.super_,
+            ) from exc
+        except MroError as exc:
+            raise AttributeInferenceError(
+                (
+                    "Lookup for {name} on {target!r} failed because {cls!r} has an "
+                    "invalid MRO."
+                ),
+                target=self,
+                attribute=name,
+                context=context,
+                mros=exc.mros,
+                cls=exc.cls,
+            ) from exc
+        found = False
+        for cls in mro:
+            if name not in cls.locals:
+                continue
+
+            found = True
+            for inferred in bases._infer_stmts([cls[name]], context, frame=self):
+                if not isinstance(inferred, scoped_nodes.FunctionDef):
+                    yield inferred
+                    continue
+
+                # We can obtain different descriptors from a super depending
+                # on what we are accessing and where the super call is.
+                if inferred.type == "classmethod":
+                    yield bases.BoundMethod(inferred, cls)
+                elif self._scope.type == "classmethod" and inferred.type == "method":
+                    yield inferred
+                elif self._class_based or inferred.type == "staticmethod":
+                    yield inferred
+                elif isinstance(inferred, Property):
+                    function = inferred.function
+                    try:
+                        yield from function.infer_call_result(
+                            caller=self, context=context
+                        )
+                    except InferenceError:
+                        yield util.Uninferable
+                elif bases._is_property(inferred):
+                    # TODO: support other descriptors as well.
+                    try:
+                        yield from inferred.infer_call_result(self, context)
+                    except InferenceError:
+                        yield util.Uninferable
+                else:
+                    yield bases.BoundMethod(inferred, cls)
+
+        # Only if we haven't found any explicit overwrites for the
+        # attribute we look it up in the special attributes
+        if not found and name in self.special_attributes:
+            yield self.special_attributes.lookup(name)
+            return
+
+        if not found:
+            raise AttributeInferenceError(target=self, attribute=name, context=context)
+
+    def getattr(self, name, context: InferenceContext | None = None):
+        return list(self.igetattr(name, context=context))
+
+
+class ExceptionInstance(bases.Instance):
+    """Class for instances of exceptions.
+
+    It has special treatment for some of the exceptions's attributes,
+    which are transformed at runtime into certain concrete objects, such as
+    the case of .args.
     """
-    Infers the call to _alias function
-    Insert ClassDef, with same name as aliased class,
-    in mro to simulate _GenericAlias.
 
-    :param node: call node
-    :param context: inference context
+    @cached_property
+    def special_attributes(self):
+        qname = self.qname()
+        instance = objectmodel.BUILTIN_EXCEPTIONS.get(
+            qname, objectmodel.ExceptionInstanceModel
+        )
+        return instance()(self)
+
+
+class DictInstance(bases.Instance):
+    """Special kind of instances for dictionaries.
+
+    This instance knows the underlying object model of the dictionaries, which means
+    that methods such as .values or .items can be properly inferred.
     """
-    if (
-        not isinstance(node.parent, Assign)
-        or not len(node.parent.targets) == 1
-        or not isinstance(node.parent.targets[0], AssignName)
-    ):
-        raise UseInferenceDefault
-    try:
-        res = next(node.args[0].infer(context=ctx))
-    except StopIteration as e:
-        raise InferenceError(node=node.args[0], context=context) from e
-
-    assign_name = node.parent.targets[0]
-
-    class_def = ClassDef(
-        name=assign_name.name,
-        lineno=assign_name.lineno,
-        col_offset=assign_name.col_offset,
-        parent=node.parent,
-    )
-    if res != Uninferable and isinstance(res, ClassDef):
-        # Only add `res` as base if it's a `ClassDef`
-        # This isn't the case for `typing.Pattern` and `typing.Match`
-        class_def.postinit(bases=[res], body=[], decorators=None)
-
-    maybe_type_var = node.args[1]
-    if (
-        not PY39_PLUS
-        and not (isinstance(maybe_type_var, Tuple) and not maybe_type_var.elts)
-        or PY39_PLUS
-        and isinstance(maybe_type_var, Const)
-        and maybe_type_var.value > 0
-    ):
-        # If typing alias is subscriptable, add `__class_getitem__` to ClassDef
-        func_to_add = extract_node(CLASS_GETITEM_TEMPLATE)
-        class_def.locals["__class_getitem__"] = [func_to_add]
-    else:
-        # If not, make sure that `__class_getitem__` access is forbidden.
-        # This is an issue in cases where the aliased class implements it,
-        # but the typing alias isn't subscriptable. E.g., `typing.ByteString` for PY39+
-        _forbid_class_getitem_access(class_def)
-    return iter([class_def])
 
+    special_attributes = objectmodel.DictModel()
 
-def _looks_like_special_alias(node: Call) -> bool:
-    """Return True if call is for Tuple or Callable alias.
 
-    In PY37 and PY38 the call is to '_VariadicGenericAlias' with 'tuple' as
-    first argument. In PY39+ it is replaced by a call to '_TupleType'.
+# Custom objects tailored for dictionaries, which are used to
+# disambiguate between the types of Python 2 dict's method returns
+# and Python 3 (where they return set like objects).
+class DictItems(bases.Proxy):
+    __str__ = node_classes.NodeNG.__str__
+    __repr__ = node_classes.NodeNG.__repr__
 
-    PY37: Tuple = _VariadicGenericAlias(tuple, (), inst=False, special=True)
-    PY39: Tuple = _TupleType(tuple, -1, inst=False, name='Tuple')
 
+class DictKeys(bases.Proxy):
+    __str__ = node_classes.NodeNG.__str__
+    __repr__ = node_classes.NodeNG.__repr__
+
+
+class DictValues(bases.Proxy):
+    __str__ = node_classes.NodeNG.__str__
+    __repr__ = node_classes.NodeNG.__repr__
 
-    PY37: Callable = _VariadicGenericAlias(collections.abc.Callable, (), special=True)
-    PY39: Callable = _CallableType(collections.abc.Callable, 2)
-    """
-    return isinstance(node.func, Name) and (
-        not PY39_PLUS
-        and node.func.name == "_VariadicGenericAlias"
-        and (
-            isinstance(node.args[0], Name)
-            and node.args[0].name == "tuple"
-            or isinstance(node.args[0], Attribute)
-            and node.args[0].as_string() == "collections.abc.Callable"
-        )
-        or PY39_PLUS
-        and (
-            node.func.name == "_TupleType"
-            and isinstance(node.args[0], Name)
-            and node.args[0].name == "tuple"
-            or node.func.name == "_CallableType"
-            and isinstance(node.args[0], Attribute)
-            and node.args[0].as_string() == "collections.abc.Callable"
-        )
-    )
 
+class PartialFunction(scoped_nodes.FunctionDef):
+    """A class representing partial function obtained via functools.partial."""
 
-def infer_special_alias(
-    node: Call, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[ClassDef]:
-    """Infer call to tuple alias as new subscriptable class typing.Tuple."""
-    if not (
-        isinstance(node.parent, Assign)
-        and len(node.parent.targets) == 1
-        and isinstance(node.parent.targets[0], AssignName)
+    @decorators.deprecate_arguments(doc="Use the postinit arg 'doc_node' instead")
+    def __init__(
+        self, call, name=None, doc=None, lineno=None, col_offset=None, parent=None
     ):
-        raise UseInferenceDefault
-    try:
-        res = next(node.args[0].infer(context=ctx))
-    except StopIteration as e:
-        raise InferenceError(node=node.args[0], context=context) from e
-
-    assign_name = node.parent.targets[0]
-    class_def = ClassDef(
-        name=assign_name.name,
-        parent=node.parent,
-    )
-    class_def.postinit(bases=[res], body=[], decorators=None)
-    func_to_add = extract_node(CLASS_GETITEM_TEMPLATE)
-    class_def.locals["__class_getitem__"] = [func_to_add]
-    return iter([class_def])
-
-
-def _looks_like_typing_cast(node: Call) -> bool:
-    return isinstance(node, Call) and (
-        isinstance(node.func, Name)
-        and node.func.name == "cast"
-        or isinstance(node.func, Attribute)
-        and node.func.attrname == "cast"
-    )
-
-
-def infer_typing_cast(
-    node: Call, ctx: typing.Optional[context.InferenceContext] = None
-) -> typing.Iterator[NodeNG]:
-    """Infer call to cast() returning same type as casted-from var"""
-    if not isinstance(node.func, (Name, Attribute)):
-        raise UseInferenceDefault
-
-    try:
-        func = next(node.func.infer(context=ctx))
-    except (InferenceError, StopIteration) as exc:
-        raise UseInferenceDefault from exc
-    if (
-        not isinstance(func, FunctionDef)
-        or func.qname() != "typing.cast"
-        or len(node.args) != 2
+        # TODO: Pass end_lineno, end_col_offset and parent as well
+        super().__init__(
+            name,
+            lineno=lineno,
+            col_offset=col_offset,
+            parent=node_classes.Unknown(),
+            end_col_offset=0,
+            end_lineno=0,
+        )
+        # Assigned directly to prevent triggering the DeprecationWarning.
+        self._doc = doc
+        # A typical FunctionDef automatically adds its name to the parent scope,
+        # but a partial should not, so defer setting parent until after init
+        self.parent = parent
+        self.filled_args = call.positional_arguments[1:]
+        self.filled_keywords = call.keyword_arguments
+
+        wrapped_function = call.positional_arguments[0]
+        inferred_wrapped_function = next(wrapped_function.infer())
+        if isinstance(inferred_wrapped_function, PartialFunction):
+            self.filled_args = inferred_wrapped_function.filled_args + self.filled_args
+            self.filled_keywords = {
+                **inferred_wrapped_function.filled_keywords,
+                **self.filled_keywords,
+            }
+
+        self.filled_positionals = len(self.filled_args)
+
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
+        if context:
+            current_passed_keywords = {
+                keyword for (keyword, _) in context.callcontext.keywords
+            }
+            for keyword, value in self.filled_keywords.items():
+                if keyword not in current_passed_keywords:
+                    context.callcontext.keywords.append((keyword, value))
+
+            call_context_args = context.callcontext.args or []
+            context.callcontext.args = self.filled_args + call_context_args
+
+        return super().infer_call_result(caller=caller, context=context)
+
+    def qname(self) -> str:
+        return self.__class__.__name__
+
+
+# TODO: Hack to solve the circular import problem between node_classes and objects
+# This is not needed in 2.0, which has a cleaner design overall
+node_classes.Dict.__bases__ = (node_classes.NodeNG, DictInstance)
+
+
+class Property(scoped_nodes.FunctionDef):
+    """Class representing a Python property."""
+
+    @decorators.deprecate_arguments(doc="Use the postinit arg 'doc_node' instead")
+    def __init__(
+        self, function, name=None, doc=None, lineno=None, col_offset=None, parent=None
     ):
-        raise UseInferenceDefault
-
-    return node.args[1].infer(context=ctx)
+        self.function = function
+        super().__init__(
+            name,
+            lineno=lineno,
+            col_offset=col_offset,
+            parent=parent,
+            end_col_offset=function.end_col_offset,
+            end_lineno=function.end_lineno,
+        )
+        # Assigned directly to prevent triggering the DeprecationWarning.
+        self._doc = doc
 
+    special_attributes = objectmodel.PropertyModel()
+    type = "property"
 
-AstroidManager().register_transform(
-    Call,
-    inference_tip(infer_typing_typevar_or_newtype),
-    looks_like_typing_typevar_or_newtype,
-)
-AstroidManager().register_transform(
-    Subscript, inference_tip(infer_typing_attr), _looks_like_typing_subscript
-)
-AstroidManager().register_transform(
-    Call, inference_tip(infer_typing_cast), _looks_like_typing_cast
-)
+    def pytype(self) -> Literal["builtins.property"]:
+        return "builtins.property"
 
-if PY39_PLUS:
-    AstroidManager().register_transform(
-        FunctionDef, inference_tip(infer_typedDict), _looks_like_typedDict
-    )
-elif PY38_PLUS:
-    AstroidManager().register_transform(
-        ClassDef, inference_tip(infer_old_typedDict), _looks_like_typedDict
-    )
-
-if PY37_PLUS:
-    AstroidManager().register_transform(
-        Call, inference_tip(infer_typing_alias), _looks_like_typing_alias
-    )
-    AstroidManager().register_transform(
-        Call, inference_tip(infer_special_alias), _looks_like_special_alias
-    )
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> NoReturn:
+        raise InferenceError("Properties are not callable")
+
+    def _infer(
+        self: _T, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[_T, None, None]:
+        yield self
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/builder.py` & `astroid-3.0.0a1/astroid/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,53 @@
-# Copyright (c) 2006-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2013 Phil Schaf <flying-sheep@web.de>
-# Copyright (c) 2014-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014-2015 Google, Inc.
-# Copyright (c) 2014 Alexander Presnyakov <flagist0@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2018 Anthony Sottile <asottile@umich.edu>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Gregory P. Smith <greg@krypto.org>
-# Copyright (c) 2021 Kian Meng, Ang <kianmeng.ang@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""The AstroidBuilder makes astroid from living object and / or from _ast
+"""The AstroidBuilder makes astroid from living object and / or from _ast.
 
 The builder is not thread safe and can't be used to parse different sources
 at the same time.
 """
+
+from __future__ import annotations
+
+import ast
 import os
 import textwrap
 import types
+from collections.abc import Iterator, Sequence
+from io import TextIOWrapper
 from tokenize import detect_encoding
-from typing import List, Optional, Union
 
 from astroid import bases, modutils, nodes, raw_building, rebuilder, util
-from astroid._ast import get_parser_module
+from astroid._ast import ParserModule, get_parser_module
 from astroid.exceptions import AstroidBuildingError, AstroidSyntaxError, InferenceError
 from astroid.manager import AstroidManager
-from astroid.nodes.node_classes import NodeNG
-
-objects = util.lazy_import("objects")
 
 # The name of the transient function that is used to
 # wrap expressions to be extracted when calling
 # extract_node.
 _TRANSIENT_FUNCTION = "__"
 
 # The comment used to select a statement to be extracted
 # when calling extract_node.
 _STATEMENT_SELECTOR = "#@"
 MISPLACED_TYPE_ANNOTATION_ERROR = "misplaced type annotation"
 
 
-def open_source_file(filename):
+def open_source_file(filename: str) -> tuple[TextIOWrapper, str, str]:
     # pylint: disable=consider-using-with
     with open(filename, "rb") as byte_stream:
         encoding = detect_encoding(byte_stream.readline)[0]
     stream = open(filename, newline=None, encoding=encoding)
     data = stream.read()
     return stream, encoding, data
 
 
-def _can_assign_attr(node, attrname):
+def _can_assign_attr(node: nodes.ClassDef, attrname: str | None) -> bool:
     try:
         slots = node.slots()
     except NotImplementedError:
         pass
     else:
         if slots and attrname not in {slot.value for slot in slots}:
             return False
@@ -75,21 +60,22 @@
     The param *manager* specifies the manager class which should be used.
     If no manager is given, then the default one will be used. The
     param *apply_transforms* determines if the transforms should be
     applied after the tree was built from source or from a live object,
     by default being True.
     """
 
-    # pylint: disable=redefined-outer-name
-    def __init__(self, manager=None, apply_transforms=True):
+    def __init__(
+        self, manager: AstroidManager | None = None, apply_transforms: bool = True
+    ) -> None:
         super().__init__(manager)
         self._apply_transforms = apply_transforms
 
     def module_build(
-        self, module: types.ModuleType, modname: Optional[str] = None
+        self, module: types.ModuleType, modname: str | None = None
     ) -> nodes.Module:
         """Build an astroid from a living module instance."""
         node = None
         path = getattr(module, "__file__", None)
         loader = getattr(module, "__loader__", None)
         # Prefer the loader to get the source rather than assuming we have a
         # filesystem to read the source file from ourselves.
@@ -106,18 +92,19 @@
             # this is a built-in module
             # get a partial representation by introspection
             node = self.inspect_build(module, modname=modname, path=path)
             if self._apply_transforms:
                 # We have to handle transformation by ourselves since the
                 # rebuilder isn't called for builtin nodes
                 node = self._manager.visit_transforms(node)
+        assert isinstance(node, nodes.Module)
         return node
 
-    def file_build(self, path, modname=None):
-        """Build astroid from a source code file (i.e. from an ast)
+    def file_build(self, path: str, modname: str | None = None) -> nodes.Module:
+        """Build astroid from a source code file (i.e. from an ast).
 
         *path* is expected to be a python source file
         """
         try:
             stream, encoding, data = open_source_file(path)
         except OSError as exc:
             raise AstroidBuildingError(
@@ -143,44 +130,50 @@
             # get module name if necessary
             if modname is None:
                 try:
                     modname = ".".join(modutils.modpath_from_file(path))
                 except ImportError:
                     modname = os.path.splitext(os.path.basename(path))[0]
             # build astroid representation
-            module = self._data_build(data, modname, path)
-            return self._post_build(module, encoding)
+            module, builder = self._data_build(data, modname, path)
+            return self._post_build(module, builder, encoding)
 
-    def string_build(self, data, modname="", path=None):
+    def string_build(
+        self, data: str, modname: str = "", path: str | None = None
+    ) -> nodes.Module:
         """Build astroid from source code string."""
-        module = self._data_build(data, modname, path)
+        module, builder = self._data_build(data, modname, path)
         module.file_bytes = data.encode("utf-8")
-        return self._post_build(module, "utf-8")
+        return self._post_build(module, builder, "utf-8")
 
-    def _post_build(self, module, encoding):
-        """Handles encoding and delayed nodes after a module has been built"""
+    def _post_build(
+        self, module: nodes.Module, builder: rebuilder.TreeRebuilder, encoding: str
+    ) -> nodes.Module:
+        """Handles encoding and delayed nodes after a module has been built."""
         module.file_encoding = encoding
         self._manager.cache_module(module)
         # post tree building steps after we stored the module in the cache:
-        for from_node in module._import_from_nodes:
+        for from_node in builder._import_from_nodes:
             if from_node.modname == "__future__":
                 for symbol, _ in from_node.names:
                     module.future_imports.add(symbol)
             self.add_from_names_to_locals(from_node)
         # handle delayed assattr nodes
-        for delayed in module._delayed_assattr:
+        for delayed in builder._delayed_assattr:
             self.delayed_assattr(delayed)
 
         # Visit the transforms
         if self._apply_transforms:
             module = self._manager.visit_transforms(module)
         return module
 
-    def _data_build(self, data, modname, path):
-        """Build tree node from data and add some information"""
+    def _data_build(
+        self, data: str, modname: str, path: str | None
+    ) -> tuple[nodes.Module, rebuilder.TreeRebuilder]:
+        """Build tree node from data and add some informations."""
         try:
             node, parser_module = _parse_string(data, type_comments=True)
         except (TypeError, ValueError, SyntaxError) as exc:
             raise AstroidSyntaxError(
                 "Parsing Python code failed:\n{error}",
                 source=data,
                 modname=modname,
@@ -196,66 +189,73 @@
             modname = modname[:-9]
             package = True
         else:
             package = (
                 path is not None
                 and os.path.splitext(os.path.basename(path))[0] == "__init__"
             )
-        builder = rebuilder.TreeRebuilder(self._manager, parser_module)
+        builder = rebuilder.TreeRebuilder(self._manager, parser_module, data)
         module = builder.visit_module(node, modname, node_file, package)
-        module._import_from_nodes = builder._import_from_nodes
-        module._delayed_assattr = builder._delayed_assattr
-        return module
+        return module, builder
 
-    def add_from_names_to_locals(self, node):
-        """Store imported names to the locals
+    def add_from_names_to_locals(self, node: nodes.ImportFrom) -> None:
+        """Store imported names to the locals.
 
         Resort the locals if coming from a delayed node
         """
 
-        def _key_func(node):
-            return node.fromlineno
+        def _key_func(node: nodes.NodeNG) -> int:
+            return node.fromlineno or 0
 
-        def sort_locals(my_list):
+        def sort_locals(my_list: list[nodes.NodeNG]) -> None:
             my_list.sort(key=_key_func)
 
-        for (name, asname) in node.names:
+        assert node.parent  # It should always default to the module
+        for name, asname in node.names:
             if name == "*":
                 try:
                     imported = node.do_import_module()
                 except AstroidBuildingError:
                     continue
                 for name in imported.public_names():
                     node.parent.set_local(name, node)
-                    sort_locals(node.parent.scope().locals[name])
+                    sort_locals(node.parent.scope().locals[name])  # type: ignore[arg-type]
             else:
                 node.parent.set_local(asname or name, node)
-                sort_locals(node.parent.scope().locals[asname or name])
+                sort_locals(node.parent.scope().locals[asname or name])  # type: ignore[arg-type]
 
-    def delayed_assattr(self, node):
-        """Visit a AssAttr node
+    def delayed_assattr(self, node: nodes.AssignAttr) -> None:
+        """Visit a AssAttr node.
 
         This adds name to locals and handle members definition.
         """
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         try:
             frame = node.frame(future=True)
             for inferred in node.expr.infer():
-                if inferred is util.Uninferable:
+                if isinstance(inferred, util.UninferableBase):
                     continue
                 try:
-                    cls = inferred.__class__
-                    if cls is bases.Instance or cls is objects.ExceptionInstance:
+                    # pylint: disable=unidiomatic-typecheck # We want a narrow check on the
+                    # parent type, not all of its subclasses
+                    if (
+                        type(inferred) == bases.Instance
+                        or type(inferred) == objects.ExceptionInstance
+                    ):
                         inferred = inferred._proxied
                         iattrs = inferred.instance_attrs
                         if not _can_assign_attr(inferred, node.attrname):
                             continue
                     elif isinstance(inferred, bases.Instance):
                         # Const, Tuple or other containers that inherit from
                         # `Instance`
                         continue
+                    elif isinstance(inferred, (bases.Proxy, util.UninferableBase)):
+                        continue
                     elif inferred.is_function:
                         iattrs = inferred.instance_attrs
                     else:
                         iattrs = inferred.locals
                 except AttributeError:
                     # XXX log error
                     continue
@@ -271,20 +271,27 @@
                     values.insert(0, node)
                 else:
                     values.append(node)
         except InferenceError:
             pass
 
 
-def build_namespace_package_module(name: str, path: List[str]) -> nodes.Module:
-    return nodes.Module(name, doc="", path=path, package=True)
+def build_namespace_package_module(name: str, path: Sequence[str]) -> nodes.Module:
+    module = nodes.Module(name, path=path, package=True)
+    module.postinit(body=[], doc_node=None)
+    return module
 
 
-def parse(code, module_name="", path=None, apply_transforms=True):
-    """Parses a source string in order to obtain an astroid AST from it
+def parse(
+    code: str,
+    module_name: str = "",
+    path: str | None = None,
+    apply_transforms: bool = True,
+) -> nodes.Module:
+    """Parses a source string in order to obtain an astroid AST from it.
 
     :param str code: The code for the module.
     :param str module_name: The name for the module, if any
     :param str path: The path for the module
     :param bool apply_transforms:
         Apply the transforms for the give code. Use it if you
         don't want the default transforms to be applied.
@@ -292,15 +299,15 @@
     code = textwrap.dedent(code)
     builder = AstroidBuilder(
         manager=AstroidManager(), apply_transforms=apply_transforms
     )
     return builder.string_build(code, modname=module_name, path=path)
 
 
-def _extract_expressions(node):
+def _extract_expressions(node: nodes.NodeNG) -> Iterator[nodes.NodeNG]:
     """Find expressions in a call to _TRANSIENT_FUNCTION and extract them.
 
     The function walks the AST recursively to search for expressions that
     are wrapped into a call to _TRANSIENT_FUNCTION. If it finds such an
     expression, it completely removes the function call node from the tree,
     replacing it by the wrapped expression inside the parent.
 
@@ -311,35 +318,36 @@
     """
     if (
         isinstance(node, nodes.Call)
         and isinstance(node.func, nodes.Name)
         and node.func.name == _TRANSIENT_FUNCTION
     ):
         real_expr = node.args[0]
+        assert node.parent
         real_expr.parent = node.parent
         # Search for node in all _astng_fields (the fields checked when
         # get_children is called) of its parent. Some of those fields may
         # be lists or tuples, in which case the elements need to be checked.
         # When we find it, replace it by real_expr, so that the AST looks
         # like no call to _TRANSIENT_FUNCTION ever took place.
         for name in node.parent._astroid_fields:
             child = getattr(node.parent, name)
-            if isinstance(child, (list, tuple)):
+            if isinstance(child, list):
                 for idx, compound_child in enumerate(child):
                     if compound_child is node:
                         child[idx] = real_expr
             elif child is node:
                 setattr(node.parent, name, real_expr)
         yield real_expr
     else:
         for child in node.get_children():
             yield from _extract_expressions(child)
 
 
-def _find_statement_by_line(node, line):
+def _find_statement_by_line(node: nodes.NodeNG, line: int) -> nodes.NodeNG | None:
     """Extracts the statement on a specific line from an AST.
 
     If the line number of node matches line, it will be returned;
     otherwise its children are iterated and the function is called
     recursively.
 
     :param node: An astroid node.
@@ -366,15 +374,15 @@
         result = _find_statement_by_line(child, line)
         if result:
             return result
 
     return None
 
 
-def extract_node(code: str, module_name: str = "") -> Union[NodeNG, List[NodeNG]]:
+def extract_node(code: str, module_name: str = "") -> nodes.NodeNG | list[nodes.NodeNG]:
     """Parses some Python code as a module and extracts a designated AST node.
 
     Statements:
      To extract one or more statement nodes, append #@ to the end of the line
 
      Examples:
        >>> def x():
@@ -420,46 +428,57 @@
 
     :param str code: A piece of Python code that is parsed as
     a module. Will be passed through textwrap.dedent first.
     :param str module_name: The name of the module.
     :returns: The designated node from the parse tree, or a list of nodes.
     """
 
-    def _extract(node):
+    def _extract(node: nodes.NodeNG | None) -> nodes.NodeNG | None:
         if isinstance(node, nodes.Expr):
             return node.value
 
         return node
 
-    requested_lines = []
+    requested_lines: list[int] = []
     for idx, line in enumerate(code.splitlines()):
         if line.strip().endswith(_STATEMENT_SELECTOR):
             requested_lines.append(idx + 1)
 
     tree = parse(code, module_name=module_name)
     if not tree.body:
         raise ValueError("Empty tree, cannot extract from it")
 
-    extracted = []
+    extracted: list[nodes.NodeNG | None] = []
     if requested_lines:
         extracted = [_find_statement_by_line(tree, line) for line in requested_lines]
 
     # Modifies the tree.
     extracted.extend(_extract_expressions(tree))
 
     if not extracted:
         extracted.append(tree.body[-1])
 
     extracted = [_extract(node) for node in extracted]
-    if len(extracted) == 1:
-        return extracted[0]
-    return extracted
-
-
-def _parse_string(data, type_comments=True):
+    extracted_without_none = [node for node in extracted if node is not None]
+    if len(extracted_without_none) == 1:
+        return extracted_without_none[0]
+    return extracted_without_none
+
+
+def _extract_single_node(code: str, module_name: str = "") -> nodes.NodeNG:
+    """Call extract_node while making sure that only one value is returned."""
+    ret = extract_node(code, module_name)
+    if isinstance(ret, list):
+        return ret[0]
+    return ret
+
+
+def _parse_string(
+    data: str, type_comments: bool = True
+) -> tuple[ast.Module, ParserModule]:
     parser_module = get_parser_module(type_comments=type_comments)
     try:
         parsed = parser_module.parse(data + "\n", type_comments=type_comments)
     except SyntaxError as exc:
         # If the type annotations are misplaced for some reason, we do not want
         # to fail the entire parsing of the file, so we need to retry the parsing without
         # type comment support.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/filter_statements.py` & `astroid-3.0.0a1/astroid/filter_statements.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""_filter_stmts and helper functions. This method gets used in LocalsDictnodes.NodeNG._scope_lookup.
+"""_filter_stmts and helper functions.
+
+This method gets used in LocalsDictnodes.NodeNG._scope_lookup.
 It is not considered public.
 """
 
-from typing import List, Optional, Tuple
+from __future__ import annotations
 
 from astroid import nodes
+from astroid.nodes import node_classes
+from astroid.typing import SuccessfulInferenceResult
 
 
 def _get_filtered_node_statements(
-    base_node: nodes.NodeNG, stmt_nodes: List[nodes.NodeNG]
-) -> List[Tuple[nodes.NodeNG, nodes.Statement]]:
+    base_node: nodes.NodeNG, stmt_nodes: list[nodes.NodeNG]
+) -> list[tuple[nodes.NodeNG, nodes.Statement]]:
     statements = [(node, node.statement(future=True)) for node in stmt_nodes]
     # Next we check if we have ExceptHandlers that are parent
     # of the underlying variable, in which case the last one survives
     if len(statements) > 1 and all(
         isinstance(stmt, nodes.ExceptHandler) for _, stmt in statements
     ):
         statements = [
             (node, stmt) for node, stmt in statements if stmt.parent_of(base_node)
         ]
     return statements
 
 
-def _is_from_decorator(node):
-    """Return True if the given node is the child of a decorator"""
+def _is_from_decorator(node) -> bool:
+    """Return whether the given node is the child of a decorator."""
     return any(isinstance(parent, nodes.Decorators) for parent in node.node_ancestors())
 
 
-def _get_if_statement_ancestor(node: nodes.NodeNG) -> Optional[nodes.If]:
-    """Return the first parent node that is an If node (or None)"""
+def _get_if_statement_ancestor(node: nodes.NodeNG) -> nodes.If | None:
+    """Return the first parent node that is an If node (or None)."""
     for parent in node.node_ancestors():
         if isinstance(parent, nodes.If):
             return parent
     return None
 
 
-def _filter_stmts(base_node: nodes.NodeNG, stmts, frame, offset):
+def _filter_stmts(
+    base_node: node_classes.LookupMixIn,
+    stmts: list[SuccessfulInferenceResult],
+    frame: nodes.LocalsDictNodeNG,
+    offset: int,
+) -> list[nodes.NodeNG]:
     """Filter the given list of statements to remove ignorable statements.
 
     If base_node is not a frame itself and the name is found in the inner
     frame locals, statements will be filtered to remove ignorable
     statements according to base_node's location.
 
     :param stmts: The statements to filter.
-    :type stmts: list(nodes.NodeNG)
 
     :param frame: The frame that all of the given statements belong to.
-    :type frame: nodes.NodeNG
 
     :param offset: The line offset to filter statements up to.
-    :type offset: int
 
     :returns: The filtered statements.
-    :rtype: list(nodes.NodeNG)
     """
     # if offset == -1, my actual frame is not the inner frame but its parent
     #
     # class A(B): pass
     #
     # we need this to resolve B correctly
     if offset == -1:
@@ -80,50 +86,50 @@
         if (
             base_node.parent
             and base_node.statement(future=True) is myframe
             and myframe.parent
         ):
             myframe = myframe.parent.frame()
 
-    mystmt: Optional[nodes.Statement] = None
+    mystmt: nodes.Statement | None = None
     if base_node.parent:
         mystmt = base_node.statement(future=True)
 
     # line filtering if we are in the same frame
     #
     # take care node may be missing lineno information (this is the case for
     # nodes inserted for living objects)
     if myframe is frame and mystmt and mystmt.fromlineno is not None:
         assert mystmt.fromlineno is not None, mystmt
         mylineno = mystmt.fromlineno + offset
     else:
         # disabling lineno filtering
         mylineno = 0
 
-    _stmts = []
+    _stmts: list[nodes.NodeNG] = []
     _stmt_parents = []
     statements = _get_filtered_node_statements(base_node, stmts)
     for node, stmt in statements:
         # line filtering is on and we have reached our location, break
         if stmt.fromlineno and stmt.fromlineno > mylineno > 0:
             break
         # Ignore decorators with the same name as the
         # decorated function
         # Fixes issue #375
         if mystmt is stmt and _is_from_decorator(base_node):
             continue
-        assert hasattr(node, "assign_type"), (
-            node,
-            node.scope(),
-            node.scope().locals,
-        )
-        assign_type = node.assign_type()
         if node.has_base(base_node):
             break
 
+        if isinstance(node, nodes.EmptyNode):
+            # EmptyNode does not have assign_type(), so just add it and move on
+            _stmts.append(node)
+            continue
+
+        assign_type = node.assign_type()
         _stmts, done = assign_type._get_filtered_stmts(base_node, node, _stmts, mystmt)
         if done:
             break
 
         optional_assign = assign_type.optional_assign
         if optional_assign and assign_type.parent_of(base_node):
             # we are inside a loop, loop var assignment is hiding previous
@@ -138,24 +144,18 @@
             if if_parent:
                 # If the if statement is within another if statement we append the node
                 # to possible statements
                 if _get_if_statement_ancestor(if_parent):
                     optional_assign = False
                     _stmts.append(node)
                     _stmt_parents.append(stmt.parent)
-                # If the if statement is first-level and not within an orelse block
-                # we know that it will be evaluated
-                elif not if_parent.is_orelse:
+                # Else we assume that it will be evaluated
+                else:
                     _stmts = [node]
                     _stmt_parents = [stmt.parent]
-                # Else we do not known enough about the control flow to be 100% certain
-                # and we append to possible statements
-                else:
-                    _stmts.append(node)
-                    _stmt_parents.append(stmt.parent)
             else:
                 _stmts = [node]
                 _stmt_parents = [stmt.parent]
 
         # XXX comment various branches below!!!
         try:
             pindex = _stmt_parents.index(stmt.parent)
```

### Comparing `astroid-2.9.3/astroid/helpers.py` & `astroid-3.0.0a1/astroid/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,87 @@
-# Copyright (c) 2015-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Simon Hewitt <si@sjhewitt.co.uk>
-# Copyright (c) 2020 Bryce Guinta <bryce.guinta@protonmail.com>
-# Copyright (c) 2020 Ram Rachum <ram@rachum.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
+"""Various helper utilities."""
 
-"""
-Various helper utilities.
-"""
+from __future__ import annotations
 
+from collections.abc import Generator
 
 from astroid import bases, manager, nodes, raw_building, util
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     _NonDeducibleTypeHierarchy,
 )
 from astroid.nodes import scoped_nodes
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 
-def _build_proxy_class(cls_name, builtins):
+def _build_proxy_class(cls_name: str, builtins: nodes.Module) -> nodes.ClassDef:
     proxy = raw_building.build_class(cls_name)
     proxy.parent = builtins
     return proxy
 
 
-def _function_type(function, builtins):
-    if isinstance(function, scoped_nodes.Lambda):
+def _function_type(
+    function: nodes.Lambda | bases.UnboundMethod, builtins: nodes.Module
+) -> nodes.ClassDef:
+    if isinstance(function, (scoped_nodes.Lambda, scoped_nodes.FunctionDef)):
         if function.root().name == "builtins":
             cls_name = "builtin_function_or_method"
         else:
             cls_name = "function"
     elif isinstance(function, bases.BoundMethod):
         cls_name = "method"
-    elif isinstance(function, bases.UnboundMethod):
+    else:
         cls_name = "function"
     return _build_proxy_class(cls_name, builtins)
 
 
-def _object_type(node, context=None):
+def _object_type(
+    node: SuccessfulInferenceResult, context: InferenceContext | None = None
+) -> Generator[InferenceResult | None, None, None]:
     astroid_manager = manager.AstroidManager()
     builtins = astroid_manager.builtins_module
     context = context or InferenceContext()
 
     for inferred in node.infer(context=context):
         if isinstance(inferred, scoped_nodes.ClassDef):
             if inferred.newstyle:
                 metaclass = inferred.metaclass(context=context)
                 if metaclass:
                     yield metaclass
                     continue
             yield builtins.getattr("type")[0]
-        elif isinstance(inferred, (scoped_nodes.Lambda, bases.UnboundMethod)):
+        elif isinstance(
+            inferred,
+            (scoped_nodes.Lambda, bases.UnboundMethod, scoped_nodes.FunctionDef),
+        ):
             yield _function_type(inferred, builtins)
         elif isinstance(inferred, scoped_nodes.Module):
             yield _build_proxy_class("module", builtins)
-        else:
+        elif isinstance(inferred, nodes.Unknown):
+            raise InferenceError
+        elif isinstance(inferred, util.UninferableBase):
+            yield inferred
+        elif isinstance(inferred, (bases.Proxy, nodes.Slice)):
             yield inferred._proxied
+        else:  # pragma: no cover
+            raise AssertionError(f"We don't handle {type(inferred)} currently")
 
 
-def object_type(node, context=None):
-    """Obtain the type of the given node
+def object_type(
+    node: SuccessfulInferenceResult, context: InferenceContext | None = None
+) -> InferenceResult | None:
+    """Obtain the type of the given node.
 
     This is used to implement the ``type`` builtin, which means that it's
     used for inferring type calls, as well as used in a couple of other places
     in the inference.
     The node will be inferred first, so this function can support all
     sorts of objects, as long as they support inference.
     """
@@ -88,73 +91,77 @@
     except InferenceError:
         return util.Uninferable
     if len(types) > 1 or not types:
         return util.Uninferable
     return list(types)[0]
 
 
-def _object_type_is_subclass(obj_type, class_or_seq, context=None):
+def _object_type_is_subclass(
+    obj_type, class_or_seq, context: InferenceContext | None = None
+):
     if not isinstance(class_or_seq, (tuple, list)):
         class_seq = (class_or_seq,)
     else:
         class_seq = class_or_seq
 
-    if obj_type is util.Uninferable:
+    if isinstance(obj_type, util.UninferableBase):
         return util.Uninferable
 
     # Instances are not types
     class_seq = [
         item if not isinstance(item, bases.Instance) else util.Uninferable
         for item in class_seq
     ]
     # strict compatibility with issubclass
     # issubclass(type, (object, 1)) evaluates to true
     # issubclass(object, (1, type)) raises TypeError
     for klass in class_seq:
-        if klass is util.Uninferable:
+        if isinstance(klass, util.UninferableBase):
             raise AstroidTypeError("arg 2 must be a type or tuple of types")
 
         for obj_subclass in obj_type.mro():
             if obj_subclass == klass:
                 return True
     return False
 
 
-def object_isinstance(node, class_or_seq, context=None):
-    """Check if a node 'isinstance' any node in class_or_seq
+def object_isinstance(node, class_or_seq, context: InferenceContext | None = None):
+    """Check if a node 'isinstance' any node in class_or_seq.
 
     :param node: A given node
     :param class_or_seq: Union[nodes.NodeNG, Sequence[nodes.NodeNG]]
     :rtype: bool
 
     :raises AstroidTypeError: if the given ``classes_or_seq`` are not types
     """
     obj_type = object_type(node, context)
-    if obj_type is util.Uninferable:
+    if isinstance(obj_type, util.UninferableBase):
         return util.Uninferable
     return _object_type_is_subclass(obj_type, class_or_seq, context=context)
 
 
-def object_issubclass(node, class_or_seq, context=None):
-    """Check if a type is a subclass of any node in class_or_seq
+def object_issubclass(node, class_or_seq, context: InferenceContext | None = None):
+    """Check if a type is a subclass of any node in class_or_seq.
 
     :param node: A given node
     :param class_or_seq: Union[Nodes.NodeNG, Sequence[nodes.NodeNG]]
     :rtype: bool
 
     :raises AstroidTypeError: if the given ``classes_or_seq`` are not types
     :raises AstroidError: if the type of the given node cannot be inferred
         or its type's mro doesn't work
     """
     if not isinstance(node, nodes.ClassDef):
         raise TypeError(f"{node} needs to be a ClassDef node")
     return _object_type_is_subclass(node, class_or_seq, context=context)
 
 
-def safe_infer(node, context=None):
+def safe_infer(
+    node: nodes.NodeNG | bases.Proxy, context: InferenceContext | None = None
+) -> InferenceResult | None:
     """Return the inferred value for the given node.
 
     Return None if inference failed or if there is some ambiguity (more than
     one node has been inferred).
     """
     try:
         inferit = node.infer(context=context)
@@ -166,16 +173,16 @@
         return None  # None if there is ambiguity on the inferred node
     except InferenceError:
         return None  # there is some kind of ambiguity
     except StopIteration:
         return value
 
 
-def has_known_bases(klass, context=None):
-    """Return true if all base classes of a class could be inferred."""
+def has_known_bases(klass, context: InferenceContext | None = None) -> bool:
+    """Return whether all base classes of a class could be inferred."""
     try:
         return klass._all_bases_known
     except AttributeError:
         pass
     for base in klass.bases:
         result = safe_infer(base, context=context)
         # TODO: check for A->B->A->B pattern in class structure too?
@@ -186,38 +193,38 @@
         ):
             klass._all_bases_known = False
             return False
     klass._all_bases_known = True
     return True
 
 
-def _type_check(type1, type2):
+def _type_check(type1, type2) -> bool:
     if not all(map(has_known_bases, (type1, type2))):
         raise _NonDeducibleTypeHierarchy
 
     if not all([type1.newstyle, type2.newstyle]):
         return False
     try:
         return type1 in type2.mro()[:-1]
     except MroError as e:
         # The MRO is invalid.
         raise _NonDeducibleTypeHierarchy from e
 
 
-def is_subtype(type1, type2):
+def is_subtype(type1, type2) -> bool:
     """Check if *type1* is a subtype of *type2*."""
     return _type_check(type1=type2, type2=type1)
 
 
-def is_supertype(type1, type2):
+def is_supertype(type1, type2) -> bool:
     """Check if *type2* is a supertype of *type1*."""
     return _type_check(type1, type2)
 
 
-def class_instance_as_index(node):
+def class_instance_as_index(node: bases.Instance) -> nodes.Const | None:
     """Get the value as an index for the given instance.
 
     If an instance provides an __index__ method, then it can
     be used in some scenarios where an integer is expected,
     for instance when multiplying or subscripting a list.
     """
     context = InferenceContext()
@@ -232,16 +239,16 @@
                 if isinstance(result, nodes.Const) and isinstance(result.value, int):
                     return result
     except InferenceError:
         pass
     return None
 
 
-def object_len(node, context=None):
-    """Infer length of given node object
+def object_len(node, context: InferenceContext | None = None):
+    """Infer length of given node object.
 
     :param Union[nodes.ClassDef, nodes.Instance] node:
     :param node: Node to infer length of
 
     :raises AstroidTypeError: If an invalid node is returned
         from __len__ method or no __len__ method exists
     :raises InferenceError: If the given node cannot be inferred
@@ -251,15 +258,15 @@
     """
     # pylint: disable=import-outside-toplevel; circular import
     from astroid.objects import FrozenSet
 
     inferred_node = safe_infer(node, context=context)
 
     # prevent self referential length calls from causing a recursion error
-    # see https://github.com/PyCQA/astroid/issues/777
+    # see https://github.com/pylint-dev/astroid/issues/777
     node_frame = node.frame(future=True)
     if (
         isinstance(node_frame, scoped_nodes.FunctionDef)
         and node_frame.name == "__len__"
         and hasattr(inferred_node, "_proxied")
         and inferred_node._proxied == node_frame.parent
     ):
@@ -267,15 +274,15 @@
             "Self referential __len__ function will "
             "cause a RecursionError on line {} of {}".format(
                 node.lineno, node.root().file
             )
         )
         raise InferenceError(message)
 
-    if inferred_node is None or inferred_node is util.Uninferable:
+    if inferred_node is None or isinstance(inferred_node, util.UninferableBase):
         raise InferenceError(node=node)
     if isinstance(inferred_node, nodes.Const) and isinstance(
         inferred_node.value, (bytes, str)
     ):
         return len(inferred_node.value)
     if isinstance(inferred_node, (nodes.List, nodes.Set, nodes.Tuple, FrozenSet)):
         return len(inferred_node.elts)
@@ -292,15 +299,15 @@
         raise AstroidTypeError(str(e)) from e
     except AttributeInferenceError as e:
         raise AstroidTypeError(
             f"object of type '{node_type.pytype()}' has no len()"
         ) from e
 
     inferred = len_call.infer_call_result(node, context)
-    if inferred is util.Uninferable:
+    if isinstance(inferred, util.UninferableBase):
         raise InferenceError(node=node, context=context)
     result_of_len = next(inferred, None)
     if (
         isinstance(result_of_len, nodes.Const)
         and result_of_len.pytype() == "builtins.int"
     ):
         return result_of_len.value
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/inference.py` & `astroid-3.0.0a1/astroid/protocols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1080 +1,976 @@
-# Copyright (c) 2006-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2012 FELD Boris <lothiraldan@gmail.com>
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2014-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Dmitry Pribysh <dmand@yandex.ru>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2017 Michał Masłowski <m.maslowski@clearcode.cc>
-# Copyright (c) 2017 Calen Pennington <cale@edx.org>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2018-2019 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018 Daniel Martin <daniel.martin@crowdstrike.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2018 HoverHell <hoverhell@gmail.com>
-# Copyright (c) 2020 Leandro T. C. Melo <ltcmelo@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Kian Meng, Ang <kianmeng.ang@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""this module contains a set of functions to handle inference on astroid trees
+"""This module contains a set of functions to handle python protocols for nodes
+where it makes sense.
 """
 
-import ast
-import functools
-import itertools
-import operator
-from typing import Any, Callable, Dict, Iterable, Optional
-
-import wrapt
+from __future__ import annotations
 
-from astroid import bases, decorators, helpers, nodes, protocols, util
-from astroid.context import (
-    CallContext,
-    InferenceContext,
-    bind_context_to_node,
-    copy_context,
-)
+import collections
+import itertools
+import operator as operator_mod
+from collections.abc import Callable, Generator, Iterator, Sequence
+from typing import Any, TypeVar
+
+from astroid import arguments, bases, decorators, helpers, nodes, objects, util
+from astroid.const import Context
+from astroid.context import InferenceContext, copy_context
 from astroid.exceptions import (
-    AstroidBuildingError,
-    AstroidError,
     AstroidIndexError,
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
-    NameInferenceError,
-    _NonDeducibleTypeHierarchy,
+    NoDefault,
+)
+from astroid.nodes import node_classes
+from astroid.typing import (
+    ConstFactoryResult,
+    InferenceResult,
+    SuccessfulInferenceResult,
 )
-from astroid.interpreter import dunder_lookup
-from astroid.manager import AstroidManager
-
-# Prevents circular imports
-objects = util.lazy_import("objects")
 
+_TupleListNodeT = TypeVar("_TupleListNodeT", nodes.Tuple, nodes.List)
 
-# .infer method ###############################################################
 
+def _reflected_name(name) -> str:
+    return "__r" + name[2:]
 
-def infer_end(self, context=None):
-    """Inference's end for nodes that yield themselves on inference
 
-    These are objects for which inference does not have any semantic,
-    such as Module or Consts.
-    """
-    yield self
+def _augmented_name(name) -> str:
+    return "__i" + name[2:]
+
+
+_CONTEXTLIB_MGR = "contextlib.contextmanager"
+BIN_OP_METHOD = {
+    "+": "__add__",
+    "-": "__sub__",
+    "/": "__truediv__",
+    "//": "__floordiv__",
+    "*": "__mul__",
+    "**": "__pow__",
+    "%": "__mod__",
+    "&": "__and__",
+    "|": "__or__",
+    "^": "__xor__",
+    "<<": "__lshift__",
+    ">>": "__rshift__",
+    "@": "__matmul__",
+}
 
+REFLECTED_BIN_OP_METHOD = {
+    key: _reflected_name(value) for (key, value) in BIN_OP_METHOD.items()
+}
+AUGMENTED_OP_METHOD = {
+    key + "=": _augmented_name(value) for (key, value) in BIN_OP_METHOD.items()
+}
 
-# We add ignores to all these assignments in this file
-# See https://github.com/python/mypy/issues/2427
-nodes.Module._infer = infer_end  # type: ignore[assignment]
-nodes.ClassDef._infer = infer_end  # type: ignore[assignment]
-nodes.Lambda._infer = infer_end  # type: ignore[assignment]
-nodes.Const._infer = infer_end  # type: ignore[assignment]
-nodes.Slice._infer = infer_end  # type: ignore[assignment]
-
-
-def _infer_sequence_helper(node, context=None):
-    """Infer all values based on _BaseContainer.elts"""
-    values = []
-
-    for elt in node.elts:
-        if isinstance(elt, nodes.Starred):
-            starred = helpers.safe_infer(elt.value, context)
-            if not starred:
-                raise InferenceError(node=node, context=context)
-            if not hasattr(starred, "elts"):
-                raise InferenceError(node=node, context=context)
-            values.extend(_infer_sequence_helper(starred))
-        elif isinstance(elt, nodes.NamedExpr):
-            value = helpers.safe_infer(elt.value, context)
-            if not value:
-                raise InferenceError(node=node, context=context)
-            values.append(value)
-        else:
-            values.append(elt)
-    return values
+UNARY_OP_METHOD = {
+    "+": "__pos__",
+    "-": "__neg__",
+    "~": "__invert__",
+    "not": None,  # XXX not '__nonzero__'
+}
+_UNARY_OPERATORS: dict[str, Callable[[Any], Any]] = {
+    "+": operator_mod.pos,
+    "-": operator_mod.neg,
+    "~": operator_mod.invert,
+    "not": operator_mod.not_,
+}
 
 
-@decorators.raise_if_nothing_inferred
-def infer_sequence(self, context=None):
-    has_starred_named_expr = any(
-        isinstance(e, (nodes.Starred, nodes.NamedExpr)) for e in self.elts
-    )
-    if has_starred_named_expr:
-        values = _infer_sequence_helper(self, context)
-        new_seq = type(self)(
-            lineno=self.lineno, col_offset=self.col_offset, parent=self.parent
-        )
-        new_seq.postinit(values)
+def _infer_unary_op(obj: Any, op: str) -> ConstFactoryResult:
+    """Perform unary operation on `obj`, unless it is `NotImplemented`.
 
-        yield new_seq
+    Can raise TypeError if operation is unsupported.
+    """
+    if obj is NotImplemented:
+        value = obj
     else:
-        yield self
-
-
-nodes.List._infer = infer_sequence  # type: ignore[assignment]
-nodes.Tuple._infer = infer_sequence  # type: ignore[assignment]
-nodes.Set._infer = infer_sequence  # type: ignore[assignment]
+        func = _UNARY_OPERATORS[op]
+        value = func(obj)
+    return nodes.const_factory(value)
+
+
+nodes.Tuple.infer_unary_op = lambda self, op: _infer_unary_op(tuple(self.elts), op)
+nodes.List.infer_unary_op = lambda self, op: _infer_unary_op(self.elts, op)
+nodes.Set.infer_unary_op = lambda self, op: _infer_unary_op(set(self.elts), op)
+nodes.Const.infer_unary_op = lambda self, op: _infer_unary_op(self.value, op)
+nodes.Dict.infer_unary_op = lambda self, op: _infer_unary_op(dict(self.items), op)
+
+# Binary operations
+
+BIN_OP_IMPL = {
+    "+": lambda a, b: a + b,
+    "-": lambda a, b: a - b,
+    "/": lambda a, b: a / b,
+    "//": lambda a, b: a // b,
+    "*": lambda a, b: a * b,
+    "**": lambda a, b: a**b,
+    "%": lambda a, b: a % b,
+    "&": lambda a, b: a & b,
+    "|": lambda a, b: a | b,
+    "^": lambda a, b: a ^ b,
+    "<<": lambda a, b: a << b,
+    ">>": lambda a, b: a >> b,
+    "@": operator_mod.matmul,
+}
+for _KEY, _IMPL in list(BIN_OP_IMPL.items()):
+    BIN_OP_IMPL[_KEY + "="] = _IMPL
 
 
-def infer_map(self, context=None):
-    if not any(isinstance(k, nodes.DictUnpack) for k, _ in self.items):
-        yield self
+@decorators.yes_if_nothing_inferred
+def const_infer_binary_op(
+    self: nodes.Const,
+    opnode: nodes.AugAssign | nodes.BinOp,
+    operator: str,
+    other: InferenceResult,
+    context: InferenceContext,
+    _: SuccessfulInferenceResult,
+) -> Generator[ConstFactoryResult | util.UninferableBase, None, None]:
+    not_implemented = nodes.Const(NotImplemented)
+    if isinstance(other, nodes.Const):
+        if (
+            operator == "**"
+            and isinstance(self.value, (int, float))
+            and isinstance(other.value, (int, float))
+            and (self.value > 1e5 or other.value > 1e5)
+        ):
+            yield not_implemented
+            return
+        try:
+            impl = BIN_OP_IMPL[operator]
+            try:
+                yield nodes.const_factory(impl(self.value, other.value))
+            except TypeError:
+                # ArithmeticError is not enough: float >> float is a TypeError
+                yield not_implemented
+            except Exception:  # pylint: disable=broad-except
+                yield util.Uninferable
+        except TypeError:
+            yield not_implemented
+    elif isinstance(self.value, str) and operator == "%":
+        # TODO(cpopa): implement string interpolation later on.
+        yield util.Uninferable
     else:
-        items = _infer_map(self, context)
-        new_seq = type(self)(self.lineno, self.col_offset, self.parent)
-        new_seq.postinit(list(items.items()))
-        yield new_seq
+        yield not_implemented
 
 
-def _update_with_replacement(lhs_dict, rhs_dict):
-    """Delete nodes that equate to duplicate keys
+nodes.Const.infer_binary_op = const_infer_binary_op
 
-    Since an astroid node doesn't 'equal' another node with the same value,
-    this function uses the as_string method to make sure duplicate keys
-    don't get through
 
-    Note that both the key and the value are astroid nodes
+def _multiply_seq_by_int(
+    self: _TupleListNodeT,
+    opnode: nodes.AugAssign | nodes.BinOp,
+    other: nodes.Const,
+    context: InferenceContext,
+) -> _TupleListNodeT:
+    node = self.__class__(parent=opnode)
+    filtered_elts = (
+        helpers.safe_infer(elt, context) or util.Uninferable
+        for elt in self.elts
+        if not isinstance(elt, util.UninferableBase)
+    )
+    node.elts = list(filtered_elts) * other.value
+    return node
 
-    Fixes issue with DictUnpack causing duplicte keys
-    in inferred Dict items
 
-    :param dict(nodes.NodeNG, nodes.NodeNG) lhs_dict: Dictionary to 'merge' nodes into
-    :param dict(nodes.NodeNG, nodes.NodeNG) rhs_dict: Dictionary with nodes to pull from
-    :return dict(nodes.NodeNG, nodes.NodeNG): merged dictionary of nodes
-    """
-    combined_dict = itertools.chain(lhs_dict.items(), rhs_dict.items())
-    # Overwrite keys which have the same string values
-    string_map = {key.as_string(): (key, value) for key, value in combined_dict}
-    # Return to dictionary
-    return dict(string_map.values())
-
-
-def _infer_map(node, context):
-    """Infer all values based on Dict.items"""
-    values = {}
-    for name, value in node.items:
-        if isinstance(name, nodes.DictUnpack):
-            double_starred = helpers.safe_infer(value, context)
-            if not double_starred:
-                raise InferenceError
-            if not isinstance(double_starred, nodes.Dict):
-                raise InferenceError(node=node, context=context)
-            unpack_items = _infer_map(double_starred, context)
-            values = _update_with_replacement(values, unpack_items)
+def _filter_uninferable_nodes(
+    elts: Sequence[InferenceResult], context: InferenceContext
+) -> Iterator[SuccessfulInferenceResult]:
+    for elt in elts:
+        if isinstance(elt, util.UninferableBase):
+            yield nodes.Unknown()
         else:
-            key = helpers.safe_infer(name, context=context)
-            value = helpers.safe_infer(value, context=context)
-            if any(not elem for elem in (key, value)):
-                raise InferenceError(node=node, context=context)
-            values = _update_with_replacement(values, {key: value})
-    return values
-
-
-nodes.Dict._infer = infer_map  # type: ignore[assignment]
-
-
-def _higher_function_scope(node):
-    """Search for the first function which encloses the given
-    scope. This can be used for looking up in that function's
-    scope, in case looking up in a lower scope for a particular
-    name fails.
-
-    :param node: A scope node.
-    :returns:
-        ``None``, if no parent function scope was found,
-        otherwise an instance of :class:`astroid.nodes.scoped_nodes.Function`,
-        which encloses the given node.
-    """
-    current = node
-    while current.parent and not isinstance(current.parent, nodes.FunctionDef):
-        current = current.parent
-    if current and current.parent:
-        return current.parent
-    return None
-
-
-def infer_name(self, context=None):
-    """infer a Name: use name lookup rules"""
-    frame, stmts = self.lookup(self.name)
-    if not stmts:
-        # Try to see if the name is enclosed in a nested function
-        # and use the higher (first function) scope for searching.
-        parent_function = _higher_function_scope(self.scope())
-        if parent_function:
-            _, stmts = parent_function.lookup(self.name)
-
-        if not stmts:
-            raise NameInferenceError(
-                name=self.name, scope=self.scope(), context=context
-            )
-    context = copy_context(context)
-    context.lookupname = self.name
-    return bases._infer_stmts(stmts, context, frame)
-
-
-# pylint: disable=no-value-for-parameter
-nodes.Name._infer = decorators.raise_if_nothing_inferred(
-    decorators.path_wrapper(infer_name)
-)
-nodes.AssignName.infer_lhs = infer_name  # won't work with a path wrapper
+            for inferred in elt.infer(context):
+                if not isinstance(inferred, util.UninferableBase):
+                    yield inferred
+                else:
+                    yield nodes.Unknown()
 
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_call(self, context=None):
-    """infer a Call node by trying to guess what the function returns"""
-    callcontext = copy_context(context)
-    callcontext.boundnode = None
-    if context is not None:
-        callcontext.extra_context = _populate_context_lookup(self, context.clone())
-
-    for callee in self.func.infer(context):
-        if callee is util.Uninferable:
-            yield callee
-            continue
-        try:
-            if hasattr(callee, "infer_call_result"):
-                callcontext.callcontext = CallContext(
-                    args=self.args, keywords=self.keywords, callee=callee
-                )
-                yield from callee.infer_call_result(caller=self, context=callcontext)
-        except InferenceError:
-            continue
-    return dict(node=self, context=context)
-
+@decorators.yes_if_nothing_inferred
+def tl_infer_binary_op(
+    self: _TupleListNodeT,
+    opnode: nodes.AugAssign | nodes.BinOp,
+    operator: str,
+    other: InferenceResult,
+    context: InferenceContext,
+    method: SuccessfulInferenceResult,
+) -> Generator[_TupleListNodeT | nodes.Const | util.UninferableBase, None, None]:
+    """Infer a binary operation on a tuple or list.
+
+    The instance on which the binary operation is performed is a tuple
+    or list. This refers to the left-hand side of the operation, so:
+    'tuple() + 1' or '[] + A()'
+    """
+    # For tuples and list the boundnode is no longer the tuple or list instance
+    context.boundnode = None
+    not_implemented = nodes.Const(NotImplemented)
+    if isinstance(other, self.__class__) and operator == "+":
+        node = self.__class__(parent=opnode)
+        node.elts = list(
+            itertools.chain(
+                _filter_uninferable_nodes(self.elts, context),
+                _filter_uninferable_nodes(other.elts, context),
+            )
+        )
+        yield node
+    elif isinstance(other, nodes.Const) and operator == "*":
+        if not isinstance(other.value, int):
+            yield not_implemented
+            return
+        yield _multiply_seq_by_int(self, opnode, other, context)
+    elif isinstance(other, bases.Instance) and operator == "*":
+        # Verify if the instance supports __index__.
+        as_index = helpers.class_instance_as_index(other)
+        if not as_index:
+            yield util.Uninferable
+        else:
+            yield _multiply_seq_by_int(self, opnode, as_index, context)
+    else:
+        yield not_implemented
 
-nodes.Call._infer = infer_call  # type: ignore[assignment]
 
+nodes.Tuple.infer_binary_op = tl_infer_binary_op
+nodes.List.infer_binary_op = tl_infer_binary_op
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_import(self, context=None, asname=True):
-    """infer an Import node: return the imported module/object"""
-    name = context.lookupname
-    if name is None:
-        raise InferenceError(node=self, context=context)
 
-    try:
-        if asname:
-            yield self.do_import_module(self.real_name(name))
-        else:
-            yield self.do_import_module(name)
-    except AstroidBuildingError as exc:
-        raise InferenceError(node=self, context=context) from exc
+@decorators.yes_if_nothing_inferred
+def instance_class_infer_binary_op(
+    self: bases.Instance | nodes.ClassDef,
+    opnode: nodes.AugAssign | nodes.BinOp,
+    operator: str,
+    other: InferenceResult,
+    context: InferenceContext,
+    method: SuccessfulInferenceResult,
+) -> Generator[InferenceResult, None, None]:
+    return method.infer_call_result(self, context)
 
 
-nodes.Import._infer = infer_import
+bases.Instance.infer_binary_op = instance_class_infer_binary_op
+nodes.ClassDef.infer_binary_op = instance_class_infer_binary_op
 
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_import_from(self, context=None, asname=True):
-    """infer a ImportFrom node: return the imported module/object"""
-    name = context.lookupname
-    if name is None:
-        raise InferenceError(node=self, context=context)
-    if asname:
-        try:
-            name = self.real_name(name)
-        except AttributeInferenceError as exc:
-            # See https://github.com/PyCQA/pylint/issues/4692
-            raise InferenceError(node=self, context=context) from exc
-    try:
-        module = self.do_import_module()
-    except AstroidBuildingError as exc:
-        raise InferenceError(node=self, context=context) from exc
+# assignment ##################################################################
 
-    try:
-        context = copy_context(context)
-        context.lookupname = name
-        stmts = module.getattr(name, ignore_locals=module is self.root())
-        return bases._infer_stmts(stmts, context)
-    except AttributeInferenceError as error:
-        raise InferenceError(
-            str(error), target=self, attribute=name, context=context
-        ) from error
+"""The assigned_stmts method is responsible to return the assigned statement
+(e.g. not inferred) according to the assignment type.
 
+The `assign_path` argument is used to record the lhs path of the original node.
+For instance if we want assigned statements for 'c' in 'a, (b,c)', assign_path
+will be [1, 1] once arrived to the Assign node.
 
-nodes.ImportFrom._infer = infer_import_from  # type: ignore[assignment]
+The `context` argument is the current inference context which should be given
+to any intermediary inference necessary.
+"""
 
 
-def infer_attribute(self, context=None):
-    """infer an Attribute node by using getattr on the associated object"""
-    for owner in self.expr.infer(context):
-        if owner is util.Uninferable:
-            yield owner
+def _resolve_looppart(parts, assign_path, context):
+    """Recursive function to resolve multiple assignments on loops."""
+    assign_path = assign_path[:]
+    index = assign_path.pop(0)
+    for part in parts:
+        if isinstance(part, util.UninferableBase):
+            continue
+        if not hasattr(part, "itered"):
             continue
-
-        if not context:
-            context = InferenceContext()
-
-        old_boundnode = context.boundnode
         try:
-            context.boundnode = owner
-            yield from owner.igetattr(self.attrname, context)
-        except (
-            AttributeInferenceError,
-            InferenceError,
-            AttributeError,
-        ):
+            itered = part.itered()
+        except TypeError:
+            continue
+        try:
+            if isinstance(itered[index], (nodes.Const, nodes.Name)):
+                itered = [part]
+        except IndexError:
             pass
-        finally:
-            context.boundnode = old_boundnode
-    return dict(node=self, context=context)
-
-
-nodes.Attribute._infer = decorators.raise_if_nothing_inferred(
-    decorators.path_wrapper(infer_attribute)
-)
-# won't work with a path wrapper
-nodes.AssignAttr.infer_lhs = decorators.raise_if_nothing_inferred(infer_attribute)
+        for stmt in itered:
+            index_node = nodes.Const(index)
+            try:
+                assigned = stmt.getitem(index_node, context)
+            except (AttributeError, AstroidTypeError, AstroidIndexError):
+                continue
+            if not assign_path:
+                # we achieved to resolved the assignment path,
+                # don't infer the last part
+                yield assigned
+            elif isinstance(assigned, util.UninferableBase):
+                break
+            else:
+                # we are not yet on the last part of the path
+                # search on each possibly inferred value
+                try:
+                    yield from _resolve_looppart(
+                        assigned.infer(context), assign_path, context
+                    )
+                except InferenceError:
+                    break
 
 
 @decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_global(self, context=None):
-    if context.lookupname is None:
-        raise InferenceError(node=self, context=context)
+def for_assigned_stmts(
+    self: nodes.For | nodes.Comprehension,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    if isinstance(self, nodes.AsyncFor) or getattr(self, "is_async", False):
+        # Skip inferring of async code for now
+        return {
+            "node": self,
+            "unknown": node,
+            "assign_path": assign_path,
+            "context": context,
+        }
+    if assign_path is None:
+        for lst in self.iter.infer(context):
+            if isinstance(lst, (nodes.Tuple, nodes.List)):
+                yield from lst.elts
+    else:
+        yield from _resolve_looppart(self.iter.infer(context), assign_path, context)
+    return {
+        "node": self,
+        "unknown": node,
+        "assign_path": assign_path,
+        "context": context,
+    }
+
+
+nodes.For.assigned_stmts = for_assigned_stmts
+nodes.Comprehension.assigned_stmts = for_assigned_stmts
+
+
+def sequence_assigned_stmts(
+    self: nodes.Tuple | nodes.List,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    if assign_path is None:
+        assign_path = []
     try:
-        return bases._infer_stmts(self.root().getattr(context.lookupname), context)
-    except AttributeInferenceError as error:
+        index = self.elts.index(node)  # type: ignore[arg-type]
+    except ValueError as exc:
         raise InferenceError(
-            str(error), target=self, attribute=context.lookupname, context=context
-        ) from error
+            "Tried to retrieve a node {node!r} which does not exist",
+            node=self,
+            assign_path=assign_path,
+            context=context,
+        ) from exc
+
+    assign_path.insert(0, index)
+    return self.parent.assigned_stmts(
+        node=self, context=context, assign_path=assign_path
+    )
 
 
-nodes.Global._infer = infer_global  # type: ignore[assignment]
+nodes.Tuple.assigned_stmts = sequence_assigned_stmts
+nodes.List.assigned_stmts = sequence_assigned_stmts
 
 
-_SUBSCRIPT_SENTINEL = object()
+def assend_assigned_stmts(
+    self: nodes.AssignName | nodes.AssignAttr,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    return self.parent.assigned_stmts(node=self, context=context)
 
 
-def infer_subscript(self, context=None):
-    """Inference for subscripts
+nodes.AssignName.assigned_stmts = assend_assigned_stmts
+nodes.AssignAttr.assigned_stmts = assend_assigned_stmts
 
-    We're understanding if the index is a Const
-    or a slice, passing the result of inference
-    to the value's `getitem` method, which should
-    handle each supported index type accordingly.
-    """
 
-    found_one = False
-    for value in self.value.infer(context):
-        if value is util.Uninferable:
-            yield util.Uninferable
-            return None
-        for index in self.slice.infer(context):
-            if index is util.Uninferable:
-                yield util.Uninferable
-                return None
+def _arguments_infer_argname(
+    self, name: str | None, context: InferenceContext
+) -> Generator[InferenceResult, None, None]:
+    # arguments information may be missing, in which case we can't do anything
+    # more
+    if not (self.arguments or self.vararg or self.kwarg):
+        yield util.Uninferable
+        return
 
-            # Try to deduce the index value.
-            index_value = _SUBSCRIPT_SENTINEL
-            if value.__class__ == bases.Instance:
-                index_value = index
-            elif index.__class__ == bases.Instance:
-                instance_as_index = helpers.class_instance_as_index(index)
-                if instance_as_index:
-                    index_value = instance_as_index
-            else:
-                index_value = index
+    functype = self.parent.type
+    # first argument of instance/class method
+    if (
+        self.arguments
+        and getattr(self.arguments[0], "name", None) == name
+        and functype != "staticmethod"
+    ):
+        cls = self.parent.parent.scope()
+        is_metaclass = isinstance(cls, nodes.ClassDef) and cls.type == "metaclass"
+        # If this is a metaclass, then the first argument will always
+        # be the class, not an instance.
+        if context.boundnode and isinstance(context.boundnode, bases.Instance):
+            cls = context.boundnode._proxied
+        if is_metaclass or functype == "classmethod":
+            yield cls
+            return
+        if functype == "method":
+            yield cls.instantiate_class()
+            return
 
-            if index_value is _SUBSCRIPT_SENTINEL:
-                raise InferenceError(node=self, context=context)
+    if context and context.callcontext:
+        callee = context.callcontext.callee
+        while hasattr(callee, "_proxied"):
+            callee = callee._proxied
+        if getattr(callee, "name", None) == self.parent.name:
+            call_site = arguments.CallSite(context.callcontext, context.extra_context)
+            yield from call_site.infer_argument(self.parent, name, context)
+            return
 
-            try:
-                assigned = value.getitem(index_value, context)
-            except (
-                AstroidTypeError,
-                AstroidIndexError,
-                AttributeInferenceError,
-                AttributeError,
-            ) as exc:
-                raise InferenceError(node=self, context=context) from exc
-
-            # Prevent inferring if the inferred subscript
-            # is the same as the original subscripted object.
-            if self is assigned or assigned is util.Uninferable:
-                yield util.Uninferable
-                return None
-            yield from assigned.infer(context)
-            found_one = True
+    if name == self.vararg:
+        vararg = nodes.const_factory(())
+        vararg.parent = self
+        if not self.arguments and self.parent.name == "__init__":
+            cls = self.parent.parent.scope()
+            vararg.elts = [cls.instantiate_class()]
+        yield vararg
+        return
+    if name == self.kwarg:
+        kwarg = nodes.const_factory({})
+        kwarg.parent = self
+        yield kwarg
+        return
+    # if there is a default value, yield it. And then yield Uninferable to reflect
+    # we can't guess given argument value
+    try:
+        context = copy_context(context)
+        yield from self.default_value(name).infer(context)
+        yield util.Uninferable
+    except NoDefault:
+        yield util.Uninferable
 
-    if found_one:
-        return dict(node=self, context=context)
-    return None
 
+def arguments_assigned_stmts(
+    self: nodes.Arguments,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    try:
+        node_name = node.name  # type: ignore[union-attr]
+    except AttributeError:
+        # Added to handle edge cases where node.name is not defined.
+        # https://github.com/pylint-dev/astroid/pull/1644#discussion_r901545816
+        node_name = None  # pragma: no cover
+
+    if context and context.callcontext:
+        callee = context.callcontext.callee
+        while hasattr(callee, "_proxied"):
+            callee = callee._proxied
+    else:
+        return _arguments_infer_argname(self, node_name, context)
+    if node and getattr(callee, "name", None) == node.frame(future=True).name:
+        # reset call context/name
+        callcontext = context.callcontext
+        context = copy_context(context)
+        context.callcontext = None
+        args = arguments.CallSite(callcontext, context=context)
+        return args.infer_argument(self.parent, node_name, context)
+    return _arguments_infer_argname(self, node_name, context)
 
-nodes.Subscript._infer = decorators.raise_if_nothing_inferred(  # type: ignore[assignment]
-    decorators.path_wrapper(infer_subscript)
-)
-nodes.Subscript.infer_lhs = decorators.raise_if_nothing_inferred(infer_subscript)
 
+nodes.Arguments.assigned_stmts = arguments_assigned_stmts
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def _infer_boolop(self, context=None):
-    """Infer a boolean operation (and / or / not).
-
-    The function will calculate the boolean operation
-    for all pairs generated through inference for each component
-    node.
-    """
-    values = self.values
-    if self.op == "or":
-        predicate = operator.truth
-    else:
-        predicate = operator.not_
 
-    try:
-        values = [value.infer(context=context) for value in values]
-    except InferenceError:
-        yield util.Uninferable
+@decorators.raise_if_nothing_inferred
+def assign_assigned_stmts(
+    self: nodes.AugAssign | nodes.Assign | nodes.AnnAssign,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    if not assign_path:
+        yield self.value
         return None
+    yield from _resolve_assignment_parts(
+        self.value.infer(context), assign_path, context
+    )
 
-    for pair in itertools.product(*values):
-        if any(item is util.Uninferable for item in pair):
-            # Can't infer the final result, just yield Uninferable.
-            yield util.Uninferable
-            continue
+    return {
+        "node": self,
+        "unknown": node,
+        "assign_path": assign_path,
+        "context": context,
+    }
 
-        bool_values = [item.bool_value() for item in pair]
-        if any(item is util.Uninferable for item in bool_values):
-            # Can't infer the final result, just yield Uninferable.
-            yield util.Uninferable
-            continue
 
-        # Since the boolean operations are short circuited operations,
-        # this code yields the first value for which the predicate is True
-        # and if no value respected the predicate, then the last value will
-        # be returned (or Uninferable if there was no last value).
-        # This is conforming to the semantics of `and` and `or`:
-        #   1 and 0 -> 1
-        #   0 and 1 -> 0
-        #   1 or 0 -> 1
-        #   0 or 1 -> 1
-        value = util.Uninferable
-        for value, bool_value in zip(pair, bool_values):
-            if predicate(bool_value):
-                yield value
-                break
+def assign_annassigned_stmts(
+    self: nodes.AnnAssign,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    for inferred in assign_assigned_stmts(self, node, context, assign_path):
+        if inferred is None:
+            yield util.Uninferable
         else:
-            yield value
-
-    return dict(node=self, context=context)
+            yield inferred
 
 
-nodes.BoolOp._infer = _infer_boolop
-
+nodes.Assign.assigned_stmts = assign_assigned_stmts
+nodes.AnnAssign.assigned_stmts = assign_annassigned_stmts
+nodes.AugAssign.assigned_stmts = assign_assigned_stmts
+
+
+def _resolve_assignment_parts(parts, assign_path, context):
+    """Recursive function to resolve multiple assignments."""
+    assign_path = assign_path[:]
+    index = assign_path.pop(0)
+    for part in parts:
+        assigned = None
+        if isinstance(part, nodes.Dict):
+            # A dictionary in an iterating context
+            try:
+                assigned, _ = part.items[index]
+            except IndexError:
+                return
 
-# UnaryOp, BinOp and AugAssign inferences
+        elif hasattr(part, "getitem"):
+            index_node = nodes.Const(index)
+            try:
+                assigned = part.getitem(index_node, context)
+            except (AstroidTypeError, AstroidIndexError):
+                return
 
+        if not assigned:
+            return
 
-def _filter_operation_errors(self, infer_callable, context, error):
-    for result in infer_callable(self, context):
-        if isinstance(result, error):
-            # For the sake of .infer(), we don't care about operation
-            # errors, which is the job of pylint. So return something
-            # which shows that we can't infer the result.
-            yield util.Uninferable
+        if not assign_path:
+            # we achieved to resolved the assignment path, don't infer the
+            # last part
+            yield assigned
+        elif isinstance(assigned, util.UninferableBase):
+            return
         else:
-            yield result
-
-
-def _infer_unaryop(self, context=None):
-    """Infer what an UnaryOp should return when evaluated."""
-    for operand in self.operand.infer(context):
-        try:
-            yield operand.infer_unary_op(self.op)
-        except TypeError as exc:
-            # The operand doesn't support this operation.
-            yield util.BadUnaryOperationMessage(operand, self.op, exc)
-        except AttributeError as exc:
-            meth = protocols.UNARY_OP_METHOD[self.op]
-            if meth is None:
-                # `not node`. Determine node's boolean
-                # value and negate its result, unless it is
-                # Uninferable, which will be returned as is.
-                bool_value = operand.bool_value()
-                if bool_value is not util.Uninferable:
-                    yield nodes.const_factory(not bool_value)
-                else:
-                    yield util.Uninferable
-            else:
-                if not isinstance(operand, (bases.Instance, nodes.ClassDef)):
-                    # The operation was used on something which
-                    # doesn't support it.
-                    yield util.BadUnaryOperationMessage(operand, self.op, exc)
-                    continue
-
-                try:
-                    try:
-                        methods = dunder_lookup.lookup(operand, meth)
-                    except AttributeInferenceError:
-                        yield util.BadUnaryOperationMessage(operand, self.op, exc)
-                        continue
-
-                    meth = methods[0]
-                    inferred = next(meth.infer(context=context), None)
-                    if inferred is util.Uninferable or not inferred.callable():
-                        continue
-
-                    context = copy_context(context)
-                    context.boundnode = operand
-                    context.callcontext = CallContext(args=[], callee=inferred)
-
-                    call_results = inferred.infer_call_result(self, context=context)
-                    result = next(call_results, None)
-                    if result is None:
-                        # Failed to infer, return the same type.
-                        yield operand
-                    else:
-                        yield result
-                except AttributeInferenceError as exc:
-                    # The unary operation special method was not found.
-                    yield util.BadUnaryOperationMessage(operand, self.op, exc)
-                except InferenceError:
-                    yield util.Uninferable
+            # we are not yet on the last part of the path search on each
+            # possibly inferred value
+            try:
+                yield from _resolve_assignment_parts(
+                    assigned.infer(context), assign_path, context
+                )
+            except InferenceError:
+                return
 
 
 @decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_unaryop(self, context=None):
-    """Infer what an UnaryOp should return when evaluated."""
-    yield from _filter_operation_errors(
-        self, _infer_unaryop, context, util.BadUnaryOperationMessage
-    )
-    return dict(node=self, context=context)
-
+def excepthandler_assigned_stmts(
+    self: nodes.ExceptHandler,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    for assigned in node_classes.unpack_infer(self.type):
+        if isinstance(assigned, nodes.ClassDef):
+            assigned = objects.ExceptionInstance(assigned)
 
-nodes.UnaryOp._infer_unaryop = _infer_unaryop
-nodes.UnaryOp._infer = infer_unaryop
+        yield assigned
+    return {
+        "node": self,
+        "unknown": node,
+        "assign_path": assign_path,
+        "context": context,
+    }
 
 
-def _is_not_implemented(const):
-    """Check if the given const node is NotImplemented."""
-    return isinstance(const, nodes.Const) and const.value is NotImplemented
+nodes.ExceptHandler.assigned_stmts = excepthandler_assigned_stmts
 
 
-def _invoke_binop_inference(instance, opnode, op, other, context, method_name):
-    """Invoke binary operation inference on the given instance."""
-    methods = dunder_lookup.lookup(instance, method_name)
-    context = bind_context_to_node(context, instance)
-    method = methods[0]
-    context.callcontext.callee = method
+def _infer_context_manager(self, mgr, context):
     try:
-        inferred = next(method.infer(context=context))
+        inferred = next(mgr.infer(context=context))
     except StopIteration as e:
-        raise InferenceError(node=method, context=context) from e
-    if inferred is util.Uninferable:
-        raise InferenceError
-    return instance.infer_binary_op(opnode, op, other, context, inferred)
-
-
-def _aug_op(instance, opnode, op, other, context, reverse=False):
-    """Get an inference callable for an augmented binary operation."""
-    method_name = protocols.AUGMENTED_OP_METHOD[op]
-    return functools.partial(
-        _invoke_binop_inference,
-        instance=instance,
-        op=op,
-        opnode=opnode,
-        other=other,
-        context=context,
-        method_name=method_name,
-    )
+        raise InferenceError(node=mgr) from e
+    if isinstance(inferred, bases.Generator):
+        # Check if it is decorated with contextlib.contextmanager.
+        func = inferred.parent
+        if not func.decorators:
+            raise InferenceError(
+                "No decorators found on inferred generator %s", node=func
+            )
 
+        for decorator_node in func.decorators.nodes:
+            decorator = next(decorator_node.infer(context=context), None)
+            if isinstance(decorator, nodes.FunctionDef):
+                if decorator.qname() == _CONTEXTLIB_MGR:
+                    break
+        else:
+            # It doesn't interest us.
+            raise InferenceError(node=func)
+        try:
+            yield next(inferred.infer_yield_types())
+        except StopIteration as e:
+            raise InferenceError(node=func) from e
+
+    elif isinstance(inferred, bases.Instance):
+        try:
+            enter = next(inferred.igetattr("__enter__", context=context))
+        except (InferenceError, AttributeInferenceError, StopIteration) as exc:
+            raise InferenceError(node=inferred) from exc
+        if not isinstance(enter, bases.BoundMethod):
+            raise InferenceError(node=enter)
+        yield from enter.infer_call_result(self, context)
+    else:
+        raise InferenceError(node=mgr)
 
-def _bin_op(instance, opnode, op, other, context, reverse=False):
-    """Get an inference callable for a normal binary operation.
 
-    If *reverse* is True, then the reflected method will be used instead.
-    """
-    if reverse:
-        method_name = protocols.REFLECTED_BIN_OP_METHOD[op]
-    else:
-        method_name = protocols.BIN_OP_METHOD[op]
-    return functools.partial(
-        _invoke_binop_inference,
-        instance=instance,
-        op=op,
-        opnode=opnode,
-        other=other,
-        context=context,
-        method_name=method_name,
-    )
+@decorators.raise_if_nothing_inferred
+def with_assigned_stmts(
+    self: nodes.With,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    """Infer names and other nodes from a *with* statement.
 
+    This enables only inference for name binding in a *with* statement.
+    For instance, in the following code, inferring `func` will return
+    the `ContextManager` class, not whatever ``__enter__`` returns.
+    We are doing this intentionally, because we consider that the context
+    manager result is whatever __enter__ returns and what it is binded
+    using the ``as`` keyword.
+
+        class ContextManager(object):
+            def __enter__(self):
+                return 42
+        with ContextManager() as f:
+            pass
 
-def _get_binop_contexts(context, left, right):
-    """Get contexts for binary operations.
+        # ContextManager().infer() will return ContextManager
+        # f.infer() will return 42.
 
-    This will return two inference contexts, the first one
-    for x.__op__(y), the other one for y.__rop__(x), where
-    only the arguments are inversed.
-    """
-    # The order is important, since the first one should be
-    # left.__op__(right).
-    for arg in (right, left):
-        new_context = context.clone()
-        new_context.callcontext = CallContext(args=[arg])
-        new_context.boundnode = None
-        yield new_context
-
-
-def _same_type(type1, type2):
-    """Check if type1 is the same as type2."""
-    return type1.qname() == type2.qname()
-
-
-def _get_binop_flow(
-    left, left_type, binary_opnode, right, right_type, context, reverse_context
-):
-    """Get the flow for binary operations.
-
-    The rules are a bit messy:
-
-        * if left and right have the same type, then only one
-          method will be called, left.__op__(right)
-        * if left and right are unrelated typewise, then first
-          left.__op__(right) is tried and if this does not exist
-          or returns NotImplemented, then right.__rop__(left) is tried.
-        * if left is a subtype of right, then only left.__op__(right)
-          is tried.
-        * if left is a supertype of right, then right.__rop__(left)
-          is first tried and then left.__op__(right)
+    Arguments:
+        self: nodes.With
+        node: The target of the assignment, `as (a, b)` in `with foo as (a, b)`.
+        context: Inference context used for caching already inferred objects
+        assign_path:
+            A list of indices, where each index specifies what item to fetch from
+            the inference results.
     """
-    op = binary_opnode.op
-    if _same_type(left_type, right_type):
-        methods = [_bin_op(left, binary_opnode, op, right, context)]
-    elif helpers.is_subtype(left_type, right_type):
-        methods = [_bin_op(left, binary_opnode, op, right, context)]
-    elif helpers.is_supertype(left_type, right_type):
-        methods = [
-            _bin_op(right, binary_opnode, op, left, reverse_context, reverse=True),
-            _bin_op(left, binary_opnode, op, right, context),
-        ]
+    try:
+        mgr = next(mgr for (mgr, vars) in self.items if vars == node)
+    except StopIteration:
+        return None
+    if assign_path is None:
+        yield from _infer_context_manager(self, mgr, context)
     else:
-        methods = [
-            _bin_op(left, binary_opnode, op, right, context),
-            _bin_op(right, binary_opnode, op, left, reverse_context, reverse=True),
-        ]
-    return methods
-
-
-def _get_aug_flow(
-    left, left_type, aug_opnode, right, right_type, context, reverse_context
-):
-    """Get the flow for augmented binary operations.
-
-    The rules are a bit messy:
-
-        * if left and right have the same type, then left.__augop__(right)
-          is first tried and then left.__op__(right).
-        * if left and right are unrelated typewise, then
-          left.__augop__(right) is tried, then left.__op__(right)
-          is tried and then right.__rop__(left) is tried.
-        * if left is a subtype of right, then left.__augop__(right)
-          is tried and then left.__op__(right).
-        * if left is a supertype of right, then left.__augop__(right)
-          is tried, then right.__rop__(left) and then
-          left.__op__(right)
-    """
-    bin_op = aug_opnode.op.strip("=")
-    aug_op = aug_opnode.op
-    if _same_type(left_type, right_type):
-        methods = [
-            _aug_op(left, aug_opnode, aug_op, right, context),
-            _bin_op(left, aug_opnode, bin_op, right, context),
-        ]
-    elif helpers.is_subtype(left_type, right_type):
-        methods = [
-            _aug_op(left, aug_opnode, aug_op, right, context),
-            _bin_op(left, aug_opnode, bin_op, right, context),
-        ]
-    elif helpers.is_supertype(left_type, right_type):
-        methods = [
-            _aug_op(left, aug_opnode, aug_op, right, context),
-            _bin_op(right, aug_opnode, bin_op, left, reverse_context, reverse=True),
-            _bin_op(left, aug_opnode, bin_op, right, context),
-        ]
+        for result in _infer_context_manager(self, mgr, context):
+            # Walk the assign_path and get the item at the final index.
+            obj = result
+            for index in assign_path:
+                if not hasattr(obj, "elts"):
+                    raise InferenceError(
+                        "Wrong type ({targets!r}) for {node!r} assignment",
+                        node=self,
+                        targets=node,
+                        assign_path=assign_path,
+                        context=context,
+                    )
+                try:
+                    obj = obj.elts[index]
+                except IndexError as exc:
+                    raise InferenceError(
+                        "Tried to infer a nonexistent target with index {index} "
+                        "in {node!r}.",
+                        node=self,
+                        targets=node,
+                        assign_path=assign_path,
+                        context=context,
+                    ) from exc
+                except TypeError as exc:
+                    raise InferenceError(
+                        "Tried to unpack a non-iterable value in {node!r}.",
+                        node=self,
+                        targets=node,
+                        assign_path=assign_path,
+                        context=context,
+                    ) from exc
+            yield obj
+    return {
+        "node": self,
+        "unknown": node,
+        "assign_path": assign_path,
+        "context": context,
+    }
+
+
+nodes.With.assigned_stmts = with_assigned_stmts
+
+
+@decorators.raise_if_nothing_inferred
+def named_expr_assigned_stmts(
+    self: nodes.NamedExpr,
+    node: node_classes.AssignedStmtsPossibleNode,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
+    """Infer names and other nodes from an assignment expression."""
+    if self.target == node:
+        yield from self.value.infer(context=context)
     else:
-        methods = [
-            _aug_op(left, aug_opnode, aug_op, right, context),
-            _bin_op(left, aug_opnode, bin_op, right, context),
-            _bin_op(right, aug_opnode, bin_op, left, reverse_context, reverse=True),
-        ]
-    return methods
+        raise InferenceError(
+            "Cannot infer NamedExpr node {node!r}",
+            node=self,
+            assign_path=assign_path,
+            context=context,
+        )
+
 
+nodes.NamedExpr.assigned_stmts = named_expr_assigned_stmts
 
-def _infer_binary_operation(left, right, binary_opnode, context, flow_factory):
-    """Infer a binary operation between a left operand and a right operand
 
-    This is used by both normal binary operations and augmented binary
-    operations, the only difference is the flow factory used.
+@decorators.yes_if_nothing_inferred
+def starred_assigned_stmts(  # noqa: C901
+    self: nodes.Starred,
+    node: node_classes.AssignedStmtsPossibleNode = None,
+    context: InferenceContext | None = None,
+    assign_path: list[int] | None = None,
+) -> Any:
     """
+    Arguments:
+        self: nodes.Starred
+        node: a node related to the current underlying Node.
+        context: Inference context used for caching already inferred objects
+        assign_path:
+            A list of indices, where each index specifies what item to fetch from
+            the inference results.
+    """
+
+    # pylint: disable=too-many-locals,too-many-statements
+    def _determine_starred_iteration_lookups(
+        starred: nodes.Starred, target: nodes.Tuple, lookups: list[tuple[int, int]]
+    ) -> None:
+        # Determine the lookups for the rhs of the iteration
+        itered = target.itered()
+        for index, element in enumerate(itered):
+            if (
+                isinstance(element, nodes.Starred)
+                and element.value.name == starred.value.name
+            ):
+                lookups.append((index, len(itered)))
+                break
+            if isinstance(element, nodes.Tuple):
+                lookups.append((index, len(element.itered())))
+                _determine_starred_iteration_lookups(starred, element, lookups)
 
-    context, reverse_context = _get_binop_contexts(context, left, right)
-    left_type = helpers.object_type(left)
-    right_type = helpers.object_type(right)
-    methods = flow_factory(
-        left, left_type, binary_opnode, right, right_type, context, reverse_context
-    )
-    for method in methods:
-        try:
-            results = list(method())
-        except AttributeError:
-            continue
-        except AttributeInferenceError:
-            continue
-        except InferenceError:
+    stmt = self.statement(future=True)
+    if not isinstance(stmt, (nodes.Assign, nodes.For)):
+        raise InferenceError(
+            "Statement {stmt!r} enclosing {node!r} must be an Assign or For node.",
+            node=self,
+            stmt=stmt,
+            unknown=node,
+            context=context,
+        )
+
+    if context is None:
+        context = InferenceContext()
+
+    if isinstance(stmt, nodes.Assign):
+        value = stmt.value
+        lhs = stmt.targets[0]
+        if not isinstance(lhs, nodes.BaseContainer):
             yield util.Uninferable
             return
-        else:
-            if any(result is util.Uninferable for result in results):
-                yield util.Uninferable
-                return
 
-            if all(map(_is_not_implemented, results)):
-                continue
-            not_implemented = sum(
-                1 for result in results if _is_not_implemented(result)
+        if sum(1 for _ in lhs.nodes_of_class(nodes.Starred)) > 1:
+            raise InferenceError(
+                "Too many starred arguments in the assignment targets {lhs!r}.",
+                node=self,
+                targets=lhs,
+                unknown=node,
+                context=context,
             )
-            if not_implemented and not_implemented != len(results):
-                # Can't infer yet what this is.
-                yield util.Uninferable
-                return
 
-            yield from results
+        try:
+            rhs = next(value.infer(context))
+        except (InferenceError, StopIteration):
+            yield util.Uninferable
             return
-    # The operation doesn't seem to be supported so let the caller know about it
-    yield util.BadBinaryOperationMessage(left_type, binary_opnode.op, right_type)
-
-
-def _infer_binop(self, context):
-    """Binary operation inference logic."""
-    left = self.left
-    right = self.right
-
-    # we use two separate contexts for evaluating lhs and rhs because
-    # 1. evaluating lhs may leave some undesired entries in context.path
-    #    which may not let us infer right value of rhs
-    context = context or InferenceContext()
-    lhs_context = copy_context(context)
-    rhs_context = copy_context(context)
-    lhs_iter = left.infer(context=lhs_context)
-    rhs_iter = right.infer(context=rhs_context)
-    for lhs, rhs in itertools.product(lhs_iter, rhs_iter):
-        if any(value is util.Uninferable for value in (rhs, lhs)):
-            # Don't know how to process this.
+        if isinstance(rhs, util.UninferableBase) or not hasattr(rhs, "itered"):
             yield util.Uninferable
             return
 
         try:
-            yield from _infer_binary_operation(lhs, rhs, self, context, _get_binop_flow)
-        except _NonDeducibleTypeHierarchy:
+            elts = collections.deque(rhs.itered())  # type: ignore[union-attr]
+        except TypeError:
             yield util.Uninferable
+            return
 
+        # Unpack iteratively the values from the rhs of the assignment,
+        # until the find the starred node. What will remain will
+        # be the list of values which the Starred node will represent
+        # This is done in two steps, from left to right to remove
+        # anything before the starred node and from right to left
+        # to remove anything after the starred node.
+
+        for index, left_node in enumerate(lhs.elts):
+            if not isinstance(left_node, nodes.Starred):
+                if not elts:
+                    break
+                elts.popleft()
+                continue
+            lhs_elts = collections.deque(reversed(lhs.elts[index:]))
+            for right_node in lhs_elts:
+                if not isinstance(right_node, nodes.Starred):
+                    if not elts:
+                        break
+                    elts.pop()
+                    continue
 
-@decorators.yes_if_nothing_inferred
-@decorators.path_wrapper
-def infer_binop(self, context=None):
-    return _filter_operation_errors(
-        self, _infer_binop, context, util.BadBinaryOperationMessage
-    )
-
-
-nodes.BinOp._infer_binop = _infer_binop
-nodes.BinOp._infer = infer_binop
-
-COMPARE_OPS: Dict[str, Callable[[Any, Any], bool]] = {
-    "==": operator.eq,
-    "!=": operator.ne,
-    "<": operator.lt,
-    "<=": operator.le,
-    ">": operator.gt,
-    ">=": operator.ge,
-    "in": lambda a, b: a in b,
-    "not in": lambda a, b: a not in b,
-}
-UNINFERABLE_OPS = {
-    "is",
-    "is not",
-}
-
-
-def _to_literal(node: nodes.NodeNG) -> Any:
-    # Can raise SyntaxError or ValueError from ast.literal_eval
-    # Can raise AttributeError from node.as_string() as not all nodes have a visitor
-    # Is this the stupidest idea or the simplest idea?
-    return ast.literal_eval(node.as_string())
-
-
-def _do_compare(
-    left_iter: Iterable[nodes.NodeNG], op: str, right_iter: Iterable[nodes.NodeNG]
-) -> "bool | type[util.Uninferable]":
-    """
-    If all possible combinations are either True or False, return that:
-    >>> _do_compare([1, 2], '<=', [3, 4])
-    True
-    >>> _do_compare([1, 2], '==', [3, 4])
-    False
-
-    If any item is uninferable, or if some combinations are True and some
-    are False, return Uninferable:
-    >>> _do_compare([1, 3], '<=', [2, 4])
-    util.Uninferable
-    """
-    retval = None
-    if op in UNINFERABLE_OPS:
-        return util.Uninferable
-    op_func = COMPARE_OPS[op]
-
-    for left, right in itertools.product(left_iter, right_iter):
-        if left is util.Uninferable or right is util.Uninferable:
-            return util.Uninferable
-
-        try:
-            left, right = _to_literal(left), _to_literal(right)
-        except (SyntaxError, ValueError, AttributeError):
-            return util.Uninferable
-
-        try:
-            expr = op_func(left, right)
-        except TypeError as exc:
-            raise AstroidTypeError from exc
-
-        if retval is None:
-            retval = expr
-        elif retval != expr:
-            return util.Uninferable
-            # (or both, but "True | False" is basically the same)
-
-    return retval  # it was all the same value
-
-
-def _infer_compare(
-    self: nodes.Compare, context: Optional[InferenceContext] = None
-) -> Any:
-    """Chained comparison inference logic."""
-    retval = True
+                # We're done unpacking.
+                packed = nodes.List(
+                    ctx=Context.Store,
+                    parent=self,
+                    lineno=lhs.lineno,
+                    col_offset=lhs.col_offset,
+                )
+                packed.postinit(elts=list(elts))
+                yield packed
+                break
 
-    ops = self.ops
-    left_node = self.left
-    lhs = list(left_node.infer(context=context))
-    # should we break early if first element is uninferable?
-    for op, right_node in ops:
-        # eagerly evaluate rhs so that values can be re-used as lhs
-        rhs = list(right_node.infer(context=context))
+    if isinstance(stmt, nodes.For):
         try:
-            retval = _do_compare(lhs, op, rhs)
-        except AstroidTypeError:
-            retval = util.Uninferable
-            break
-        if retval is not True:
-            break  # short-circuit
-        lhs = rhs  # continue
-    if retval is util.Uninferable:
-        yield retval
-    else:
-        yield nodes.Const(retval)
-
-
-nodes.Compare._infer = _infer_compare  # type: ignore[assignment]
-
-
-def _infer_augassign(self, context=None):
-    """Inference logic for augmented binary operations."""
-    if context is None:
-        context = InferenceContext()
-
-    rhs_context = context.clone()
-
-    lhs_iter = self.target.infer_lhs(context=context)
-    rhs_iter = self.value.infer(context=rhs_context)
-    for lhs, rhs in itertools.product(lhs_iter, rhs_iter):
-        if any(value is util.Uninferable for value in (rhs, lhs)):
-            # Don't know how to process this.
+            inferred_iterable = next(stmt.iter.infer(context=context))
+        except (InferenceError, StopIteration):
+            yield util.Uninferable
+            return
+        if isinstance(inferred_iterable, util.UninferableBase) or not hasattr(
+            inferred_iterable, "itered"
+        ):
             yield util.Uninferable
             return
-
         try:
-            yield from _infer_binary_operation(
-                left=lhs,
-                right=rhs,
-                binary_opnode=self,
-                context=context,
-                flow_factory=_get_aug_flow,
-            )
-        except _NonDeducibleTypeHierarchy:
+            itered = inferred_iterable.itered()  # type: ignore[union-attr]
+        except TypeError:
             yield util.Uninferable
+            return
 
+        target = stmt.target
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_augassign(self, context=None):
-    return _filter_operation_errors(
-        self, _infer_augassign, context, util.BadBinaryOperationMessage
-    )
-
-
-nodes.AugAssign._infer_augassign = _infer_augassign
-nodes.AugAssign._infer = infer_augassign
-
-# End of binary operation inference.
-
-
-@decorators.raise_if_nothing_inferred
-def infer_arguments(self, context=None):
-    name = context.lookupname
-    if name is None:
-        raise InferenceError(node=self, context=context)
-    return protocols._arguments_infer_argname(self, name, context)
-
-
-nodes.Arguments._infer = infer_arguments  # type: ignore[assignment]
-
-
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_assign(self, context=None):
-    """infer a AssignName/AssignAttr: need to inspect the RHS part of the
-    assign node
-    """
-    if isinstance(self.parent, nodes.AugAssign):
-        return self.parent.infer(context)
-
-    stmts = list(self.assigned_stmts(context=context))
-    return bases._infer_stmts(stmts, context)
+        if not isinstance(target, nodes.Tuple):
+            raise InferenceError(
+                "Could not make sense of this, the target must be a tuple",
+                context=context,
+            )
 
+        lookups: list[tuple[int, int]] = []
+        _determine_starred_iteration_lookups(self, target, lookups)
+        if not lookups:
+            raise InferenceError(
+                "Could not make sense of this, needs at least a lookup", context=context
+            )
 
-nodes.AssignName._infer = infer_assign
-nodes.AssignAttr._infer = infer_assign
+        # Make the last lookup a slice, since that what we want for a Starred node
+        last_element_index, last_element_length = lookups[-1]
+        is_starred_last = last_element_index == (last_element_length - 1)
+
+        lookup_slice = slice(
+            last_element_index,
+            None if is_starred_last else (last_element_length - last_element_index),
+        )
+        last_lookup = lookup_slice
 
+        for element in itered:
+            # We probably want to infer the potential values *for each* element in an
+            # iterable, but we can't infer a list of all values, when only a list of
+            # step values are expected:
+            #
+            # for a, *b in [...]:
+            #   b
+            #
+            # *b* should now point to just the elements at that particular iteration step,
+            # which astroid can't know about.
+
+            found_element = None
+            for index, lookup in enumerate(lookups):
+                if not hasattr(element, "itered"):
+                    break
+                if index + 1 is len(lookups):
+                    cur_lookup: slice | int = last_lookup
+                else:
+                    # Grab just the index, not the whole length
+                    cur_lookup = lookup[0]
+                try:
+                    itered_inner_element = element.itered()
+                    element = itered_inner_element[cur_lookup]
+                except IndexError:
+                    break
+                except TypeError:
+                    # Most likely the itered() call failed, cannot make sense of this
+                    yield util.Uninferable
+                    return
+                else:
+                    found_element = element
 
-@decorators.raise_if_nothing_inferred
-@decorators.path_wrapper
-def infer_empty_node(self, context=None):
-    if not self.has_underlying_object():
-        yield util.Uninferable
-    else:
-        try:
-            yield from AstroidManager().infer_ast_from_something(
-                self.object, context=context
+            unpacked = nodes.List(
+                ctx=Context.Store,
+                parent=self,
+                lineno=self.lineno,
+                col_offset=self.col_offset,
             )
-        except AstroidError:
-            yield util.Uninferable
-
+            unpacked.postinit(elts=found_element or [])
+            yield unpacked
+            return
 
-nodes.EmptyNode._infer = infer_empty_node  # type: ignore[assignment]
+        yield util.Uninferable
 
 
-@decorators.raise_if_nothing_inferred
-def infer_index(self, context=None):
-    return self.value.infer(context)
+nodes.Starred.assigned_stmts = starred_assigned_stmts
 
 
-nodes.Index._infer = infer_index  # type: ignore[assignment]
-
+@decorators.yes_if_nothing_inferred
+def match_mapping_assigned_stmts(
+    self: nodes.MatchMapping,
+    node: nodes.AssignName,
+    context: InferenceContext | None = None,
+    assign_path: None = None,
+) -> Generator[nodes.NodeNG, None, None]:
+    """Return empty generator (return -> raises StopIteration) so inferred value
+    is Uninferable.
+    """
+    return
+    yield
 
-def _populate_context_lookup(call, context):
-    # Allows context to be saved for later
-    # for inference inside a function
-    context_lookup = {}
-    if context is None:
-        return context_lookup
-    for arg in call.args:
-        if isinstance(arg, nodes.Starred):
-            context_lookup[arg.value] = context
-        else:
-            context_lookup[arg] = context
-    keywords = call.keywords if call.keywords is not None else []
-    for keyword in keywords:
-        context_lookup[keyword.value] = context
-    return context_lookup
 
+nodes.MatchMapping.assigned_stmts = match_mapping_assigned_stmts
 
-@decorators.raise_if_nothing_inferred
-def infer_ifexp(self, context=None):
-    """Support IfExp inference
 
-    If we can't infer the truthiness of the condition, we default
-    to inferring both branches. Otherwise, we infer either branch
-    depending on the condition.
+@decorators.yes_if_nothing_inferred
+def match_star_assigned_stmts(
+    self: nodes.MatchStar,
+    node: nodes.AssignName,
+    context: InferenceContext | None = None,
+    assign_path: None = None,
+) -> Generator[nodes.NodeNG, None, None]:
+    """Return empty generator (return -> raises StopIteration) so inferred value
+    is Uninferable.
     """
-    both_branches = False
-    # We use two separate contexts for evaluating lhs and rhs because
-    # evaluating lhs may leave some undesired entries in context.path
-    # which may not let us infer right value of rhs.
-
-    context = context or InferenceContext()
-    lhs_context = copy_context(context)
-    rhs_context = copy_context(context)
-    try:
-        test = next(self.test.infer(context=context.clone()))
-    except (InferenceError, StopIteration):
-        both_branches = True
-    else:
-        if test is not util.Uninferable:
-            if test.bool_value():
-                yield from self.body.infer(context=lhs_context)
-            else:
-                yield from self.orelse.infer(context=rhs_context)
-        else:
-            both_branches = True
-    if both_branches:
-        yield from self.body.infer(context=lhs_context)
-        yield from self.orelse.infer(context=rhs_context)
+    return
+    yield
 
 
-nodes.IfExp._infer = infer_ifexp  # type: ignore[assignment]
+nodes.MatchStar.assigned_stmts = match_star_assigned_stmts
 
 
-# pylint: disable=dangerous-default-value
-@wrapt.decorator
-def _cached_generator(func, instance, args, kwargs, _cache={}):  # noqa: B006
-    node = args[0]
-    try:
-        return iter(_cache[func, id(node)])
-    except KeyError:
-        result = func(*args, **kwargs)
-        # Need to keep an iterator around
-        original, copy = itertools.tee(result)
-        _cache[func, id(node)] = list(copy)
-        return original
-
-
-# When inferring a property, we instantiate a new `objects.Property` object,
-# which in turn, because it inherits from `FunctionDef`, sets itself in the locals
-# of the wrapping frame. This means that every time we infer a property, the locals
-# are mutated with a new instance of the property. This is why we cache the result
-# of the function's inference.
-@_cached_generator
-def infer_functiondef(self, context=None):
-    if not self.decorators or not bases._is_property(self):
-        yield self
-        return dict(node=self, context=context)
-
-    prop_func = objects.Property(
-        function=self,
-        name=self.name,
-        doc=self.doc,
-        lineno=self.lineno,
-        parent=self.parent,
-        col_offset=self.col_offset,
-    )
-    prop_func.postinit(body=[], args=self.args)
-    yield prop_func
-    return dict(node=self, context=context)
+@decorators.yes_if_nothing_inferred
+def match_as_assigned_stmts(
+    self: nodes.MatchAs,
+    node: nodes.AssignName,
+    context: InferenceContext | None = None,
+    assign_path: None = None,
+) -> Generator[nodes.NodeNG, None, None]:
+    """Infer MatchAs as the Match subject if it's the only MatchCase pattern
+    else raise StopIteration to yield Uninferable.
+    """
+    if (
+        isinstance(self.parent, nodes.MatchCase)
+        and isinstance(self.parent.parent, nodes.Match)
+        and self.pattern is None
+    ):
+        yield self.parent.parent.subject
 
 
-nodes.FunctionDef._infer = infer_functiondef  # type: ignore[assignment]
+nodes.MatchAs.assigned_stmts = match_as_assigned_stmts
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a1/astroid/interpreter/_import/spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,338 +1,434 @@
-# Copyright (c) 2016-2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017 Chris Philip <chrisp533@gmail.com>
-# Copyright (c) 2017 Hugo <hugovk@users.noreply.github.com>
-# Copyright (c) 2017 ioanatia <ioanatia@users.noreply.github.com>
-# Copyright (c) 2017 Calen Pennington <cale@edx.org>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2019 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Peter Kolbus <peter.kolbus@gmail.com>
-# Copyright (c) 2020 Raphael Gaschignard <raphael@rtpg.co>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 DudeNr33 <3929834+DudeNr33@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
 
 import abc
-import collections
 import enum
+import importlib
 import importlib.machinery
+import importlib.util
 import os
+import pathlib
 import sys
+import types
+import warnings
 import zipimport
-from functools import lru_cache
+from collections.abc import Iterator, Sequence
+from pathlib import Path
+from typing import Any, Literal, NamedTuple, Protocol
 
-from . import util
+from astroid.const import PY310_PLUS
+from astroid.modutils import EXT_LIB_DIRS
 
-ModuleType = enum.Enum(
-    "ModuleType",
-    "C_BUILTIN C_EXTENSION PKG_DIRECTORY "
-    "PY_CODERESOURCE PY_COMPILED PY_FROZEN PY_RESOURCE "
-    "PY_SOURCE PY_ZIPMODULE PY_NAMESPACE",
-)
+from . import util
 
 
-_ModuleSpec = collections.namedtuple(
-    "_ModuleSpec", "name type location " "origin submodule_search_locations"
-)
+# The MetaPathFinder protocol comes from typeshed, which says:
+# Intentionally omits one deprecated and one optional method of `importlib.abc.MetaPathFinder`
+class _MetaPathFinder(Protocol):
+    def find_spec(
+        self,
+        fullname: str,
+        path: Sequence[str] | None,
+        target: types.ModuleType | None = ...,
+    ) -> importlib.machinery.ModuleSpec | None:
+        ...  # pragma: no cover
+
+
+class ModuleType(enum.Enum):
+    """Python module types used for ModuleSpec."""
+
+    C_BUILTIN = enum.auto()
+    C_EXTENSION = enum.auto()
+    PKG_DIRECTORY = enum.auto()
+    PY_CODERESOURCE = enum.auto()
+    PY_COMPILED = enum.auto()
+    PY_FROZEN = enum.auto()
+    PY_RESOURCE = enum.auto()
+    PY_SOURCE = enum.auto()
+    PY_ZIPMODULE = enum.auto()
+    PY_NAMESPACE = enum.auto()
+
+
+_MetaPathFinderModuleTypes: dict[str, ModuleType] = {
+    # Finders created by setuptools editable installs
+    "_EditableFinder": ModuleType.PY_SOURCE,
+    "_EditableNamespaceFinder": ModuleType.PY_NAMESPACE,
+    # Finders create by six
+    "_SixMetaPathImporter": ModuleType.PY_SOURCE,
+}
+
+_EditableFinderClasses: set[str] = {
+    "_EditableFinder",
+    "_EditableNamespaceFinder",
+}
 
 
-class ModuleSpec(_ModuleSpec):
-    """Defines a class similar to PEP 420's ModuleSpec
+class ModuleSpec(NamedTuple):
+    """Defines a class similar to PEP 420's ModuleSpec.
 
     A module spec defines a name of a module, its type, location
     and where submodules can be found, if the module is a package.
     """
 
-    def __new__(
-        cls,
-        name,
-        module_type,
-        location=None,
-        origin=None,
-        submodule_search_locations=None,
-    ):
-        return _ModuleSpec.__new__(
-            cls,
-            name=name,
-            type=module_type,
-            location=location,
-            origin=origin,
-            submodule_search_locations=submodule_search_locations,
-        )
+    name: str
+    type: ModuleType | None
+    location: str | None = None
+    origin: str | None = None
+    submodule_search_locations: Sequence[str] | None = None
 
 
 class Finder:
     """A finder is a class which knows how to find a particular module."""
 
-    def __init__(self, path=None):
+    def __init__(self, path: Sequence[str] | None = None) -> None:
         self._path = path or sys.path
 
     @abc.abstractmethod
-    def find_module(self, modname, module_parts, processed, submodule_path):
-        """Find the given module
+    def find_module(
+        self,
+        modname: str,
+        module_parts: Sequence[str],
+        processed: list[str],
+        submodule_path: Sequence[str] | None,
+    ) -> ModuleSpec | None:
+        """Find the given module.
 
         Each finder is responsible for each protocol of finding, as long as
         they all return a ModuleSpec.
 
-        :param str modname: The module which needs to be searched.
-        :param list module_parts: It should be a list of strings,
+        :param modname: The module which needs to be searched.
+        :param module_parts: It should be a list of strings,
                                   where each part contributes to the module's
                                   namespace.
-        :param list processed: What parts from the module parts were processed
+        :param processed: What parts from the module parts were processed
                                so far.
-        :param list submodule_path: A list of paths where the module
+        :param submodule_path: A list of paths where the module
                                     can be looked into.
         :returns: A ModuleSpec, describing how and where the module was found,
                   None, otherwise.
         """
 
-    def contribute_to_path(self, spec, processed):
+    def contribute_to_path(
+        self, spec: ModuleSpec, processed: list[str]
+    ) -> Sequence[str] | None:
         """Get a list of extra paths where this finder can search."""
 
 
 class ImportlibFinder(Finder):
     """A finder based on the importlib module."""
 
-    _SUFFIXES = (
+    _SUFFIXES: Sequence[tuple[str, ModuleType]] = (
         [(s, ModuleType.C_EXTENSION) for s in importlib.machinery.EXTENSION_SUFFIXES]
         + [(s, ModuleType.PY_SOURCE) for s in importlib.machinery.SOURCE_SUFFIXES]
         + [(s, ModuleType.PY_COMPILED) for s in importlib.machinery.BYTECODE_SUFFIXES]
     )
 
-    def find_module(self, modname, module_parts, processed, submodule_path):
-        if not isinstance(modname, str):
-            raise TypeError(f"'modname' must be a str, not {type(modname)}")
+    def find_module(
+        self,
+        modname: str,
+        module_parts: Sequence[str],
+        processed: list[str],
+        submodule_path: Sequence[str] | None,
+    ) -> ModuleSpec | None:
         if submodule_path is not None:
             submodule_path = list(submodule_path)
+        elif modname in sys.builtin_module_names:
+            return ModuleSpec(
+                name=modname,
+                location=None,
+                type=ModuleType.C_BUILTIN,
+            )
         else:
             try:
-                spec = importlib.util.find_spec(modname)
-                if spec:
-                    if spec.loader is importlib.machinery.BuiltinImporter:
-                        return ModuleSpec(
-                            name=modname,
-                            location=None,
-                            module_type=ModuleType.C_BUILTIN,
-                        )
-                    if spec.loader is importlib.machinery.FrozenImporter:
-                        return ModuleSpec(
-                            name=modname,
-                            location=None,
-                            module_type=ModuleType.PY_FROZEN,
-                        )
+                with warnings.catch_warnings():
+                    warnings.filterwarnings("ignore", category=UserWarning)
+                    spec = importlib.util.find_spec(modname)
+                if (
+                    spec
+                    and spec.loader  # type: ignore[comparison-overlap] # noqa: E501
+                    is importlib.machinery.FrozenImporter
+                ):
+                    # No need for BuiltinImporter; builtins handled above
+                    return ModuleSpec(
+                        name=modname,
+                        location=getattr(spec.loader_state, "filename", None),
+                        type=ModuleType.PY_FROZEN,
+                    )
             except ValueError:
                 pass
             submodule_path = sys.path
 
         for entry in submodule_path:
             package_directory = os.path.join(entry, modname)
             for suffix in (".py", importlib.machinery.BYTECODE_SUFFIXES[0]):
                 package_file_name = "__init__" + suffix
                 file_path = os.path.join(package_directory, package_file_name)
                 if os.path.isfile(file_path):
                     return ModuleSpec(
                         name=modname,
                         location=package_directory,
-                        module_type=ModuleType.PKG_DIRECTORY,
+                        type=ModuleType.PKG_DIRECTORY,
                     )
             for suffix, type_ in ImportlibFinder._SUFFIXES:
                 file_name = modname + suffix
                 file_path = os.path.join(entry, file_name)
                 if os.path.isfile(file_path):
-                    return ModuleSpec(
-                        name=modname, location=file_path, module_type=type_
-                    )
+                    return ModuleSpec(name=modname, location=file_path, type=type_)
         return None
 
-    def contribute_to_path(self, spec, processed):
+    def contribute_to_path(
+        self, spec: ModuleSpec, processed: list[str]
+    ) -> Sequence[str] | None:
         if spec.location is None:
             # Builtin.
             return None
 
-        if _is_setuptools_namespace(spec.location):
+        if _is_setuptools_namespace(Path(spec.location)):
             # extend_path is called, search sys.path for module/packages
             # of this name see pkgutil.extend_path documentation
             path = [
                 os.path.join(p, *processed)
                 for p in sys.path
                 if os.path.isdir(os.path.join(p, *processed))
             ]
+        elif spec.name == "distutils" and not any(
+            spec.location.lower().startswith(ext_lib_dir.lower())
+            for ext_lib_dir in EXT_LIB_DIRS
+        ):
+            # virtualenv below 20.0 patches distutils in an unexpected way
+            # so we just find the location of distutils that will be
+            # imported to avoid spurious import-error messages
+            # https://github.com/pylint-dev/pylint/issues/5645
+            # A regression test to create this scenario exists in release-tests.yml
+            # and can be triggered manually from GitHub Actions
+            distutils_spec = importlib.util.find_spec("distutils")
+            if distutils_spec and distutils_spec.origin:
+                origin_path = Path(
+                    distutils_spec.origin
+                )  # e.g. .../distutils/__init__.py
+                path = [str(origin_path.parent)]  # e.g. .../distutils
+            else:
+                path = [spec.location]
         else:
             path = [spec.location]
         return path
 
 
 class ExplicitNamespacePackageFinder(ImportlibFinder):
-    """A finder for the explicit namespace packages, generated through pkg_resources."""
+    """A finder for the explicit namespace packages."""
 
-    def find_module(self, modname, module_parts, processed, submodule_path):
+    def find_module(
+        self,
+        modname: str,
+        module_parts: Sequence[str],
+        processed: list[str],
+        submodule_path: Sequence[str] | None,
+    ) -> ModuleSpec | None:
         if processed:
-            modname = ".".join(processed + [modname])
+            modname = ".".join([*processed, modname])
         if util.is_namespace(modname) and modname in sys.modules:
             submodule_path = sys.modules[modname].__path__
             return ModuleSpec(
                 name=modname,
                 location="",
                 origin="namespace",
-                module_type=ModuleType.PY_NAMESPACE,
+                type=ModuleType.PY_NAMESPACE,
                 submodule_search_locations=submodule_path,
             )
         return None
 
-    def contribute_to_path(self, spec, processed):
+    def contribute_to_path(
+        self, spec: ModuleSpec, processed: list[str]
+    ) -> Sequence[str] | None:
         return spec.submodule_search_locations
 
 
 class ZipFinder(Finder):
     """Finder that knows how to find a module inside zip files."""
 
-    def __init__(self, path):
+    def __init__(self, path: Sequence[str]) -> None:
         super().__init__(path)
-        self._zipimporters = _precache_zipimporters(path)
+        for entry_path in path:
+            if entry_path not in sys.path_importer_cache:
+                try:
+                    sys.path_importer_cache[entry_path] = zipimport.zipimporter(  # type: ignore[assignment]
+                        entry_path
+                    )
+                except zipimport.ZipImportError:
+                    continue
 
-    def find_module(self, modname, module_parts, processed, submodule_path):
+    def find_module(
+        self,
+        modname: str,
+        module_parts: Sequence[str],
+        processed: list[str],
+        submodule_path: Sequence[str] | None,
+    ) -> ModuleSpec | None:
         try:
-            file_type, filename, path = _search_zip(module_parts, self._zipimporters)
+            file_type, filename, path = _search_zip(module_parts)
         except ImportError:
             return None
 
         return ModuleSpec(
             name=modname,
             location=filename,
             origin="egg",
-            module_type=file_type,
+            type=file_type,
             submodule_search_locations=path,
         )
 
 
 class PathSpecFinder(Finder):
     """Finder based on importlib.machinery.PathFinder."""
 
-    def find_module(self, modname, module_parts, processed, submodule_path):
+    def find_module(
+        self,
+        modname: str,
+        module_parts: Sequence[str],
+        processed: list[str],
+        submodule_path: Sequence[str] | None,
+    ) -> ModuleSpec | None:
         spec = importlib.machinery.PathFinder.find_spec(modname, path=submodule_path)
-        if spec:
-            # origin can be either a string on older Python versions
-            # or None in case it is a namespace package:
-            # https://github.com/python/cpython/pull/5481
-            is_namespace_pkg = spec.origin in {"namespace", None}
+        if spec is not None:
+            is_namespace_pkg = spec.origin is None
             location = spec.origin if not is_namespace_pkg else None
             module_type = ModuleType.PY_NAMESPACE if is_namespace_pkg else None
-            spec = ModuleSpec(
+            return ModuleSpec(
                 name=spec.name,
                 location=location,
                 origin=spec.origin,
-                module_type=module_type,
+                type=module_type,
                 submodule_search_locations=list(spec.submodule_search_locations or []),
             )
         return spec
 
-    def contribute_to_path(self, spec, processed):
+    def contribute_to_path(
+        self, spec: ModuleSpec, processed: list[str]
+    ) -> Sequence[str] | None:
         if spec.type == ModuleType.PY_NAMESPACE:
             return spec.submodule_search_locations
         return None
 
 
 _SPEC_FINDERS = (
     ImportlibFinder,
     ZipFinder,
     PathSpecFinder,
     ExplicitNamespacePackageFinder,
 )
 
 
-def _is_setuptools_namespace(location):
+def _is_setuptools_namespace(location: pathlib.Path) -> bool:
     try:
-        with open(os.path.join(location, "__init__.py"), "rb") as stream:
+        with open(location / "__init__.py", "rb") as stream:
             data = stream.read(4096)
     except OSError:
-        return None
-    else:
-        extend_path = b"pkgutil" in data and b"extend_path" in data
-        declare_namespace = (
-            b"pkg_resources" in data and b"declare_namespace(__name__)" in data
-        )
-        return extend_path or declare_namespace
-
-
-@lru_cache()
-def _cached_set_diff(left, right):
-    result = set(left)
-    result.difference_update(right)
-    return result
-
-
-def _precache_zipimporters(path=None):
-    """
-    For each path that has not been already cached
-    in the sys.path_importer_cache, create a new zipimporter
-    instance and add it into the cache.
-    Return a dict associating all paths, stored in the cache, to corresponding
-    zipimporter instances.
+        return False
+    extend_path = b"pkgutil" in data and b"extend_path" in data
+    declare_namespace = (
+        b"pkg_resources" in data and b"declare_namespace(__name__)" in data
+    )
+    return extend_path or declare_namespace
 
-    :param path: paths that has to be added into the cache
-    :return: association between paths stored in the cache and zipimporter instances
-    """
-    pic = sys.path_importer_cache
 
-    # When measured, despite having the same complexity (O(n)),
-    # converting to tuples and then caching the conversion to sets
-    # and the set difference is faster than converting to sets
-    # and then only caching the set difference.
-
-    req_paths = tuple(path or sys.path)
-    cached_paths = tuple(pic)
-    new_paths = _cached_set_diff(req_paths, cached_paths)
-    # pylint: disable=no-member
-    for entry_path in new_paths:
-        try:
-            pic[entry_path] = zipimport.zipimporter(entry_path)
-        except zipimport.ZipImportError:
-            continue
-    return {
-        key: value
-        for key, value in pic.items()
-        if isinstance(value, zipimport.zipimporter)
-    }
+def _get_zipimporters() -> Iterator[tuple[str, zipimport.zipimporter]]:
+    for filepath, importer in sys.path_importer_cache.items():
+        if isinstance(importer, zipimport.zipimporter):
+            yield filepath, importer
 
 
-def _search_zip(modpath, pic):
-    for filepath, importer in list(pic.items()):
-        if importer is not None:
+def _search_zip(
+    modpath: Sequence[str],
+) -> tuple[Literal[ModuleType.PY_ZIPMODULE], str, str]:
+    for filepath, importer in _get_zipimporters():
+        if PY310_PLUS:
+            found: Any = importer.find_spec(modpath[0])
+        else:
             found = importer.find_module(modpath[0])
-            if found:
-                if not importer.find_module(os.path.sep.join(modpath)):
+        if found:
+            if PY310_PLUS:
+                if not importer.find_spec(os.path.sep.join(modpath)):
                     raise ImportError(
                         "No module named %s in %s/%s"
                         % (".".join(modpath[1:]), filepath, modpath)
                     )
-                # import code; code.interact(local=locals())
-                return (
-                    ModuleType.PY_ZIPMODULE,
-                    os.path.abspath(filepath) + os.path.sep + os.path.sep.join(modpath),
-                    filepath,
+            elif not importer.find_module(os.path.sep.join(modpath)):
+                raise ImportError(
+                    "No module named %s in %s/%s"
+                    % (".".join(modpath[1:]), filepath, modpath)
                 )
+            return (
+                ModuleType.PY_ZIPMODULE,
+                os.path.abspath(filepath) + os.path.sep + os.path.sep.join(modpath),
+                filepath,
+            )
     raise ImportError(f"No module named {'.'.join(modpath)}")
 
 
-def _find_spec_with_path(search_path, modname, module_parts, processed, submodule_path):
-    finders = [finder(search_path) for finder in _SPEC_FINDERS]
-    for finder in finders:
-        spec = finder.find_module(modname, module_parts, processed, submodule_path)
+def _find_spec_with_path(
+    search_path: Sequence[str],
+    modname: str,
+    module_parts: list[str],
+    processed: list[str],
+    submodule_path: Sequence[str] | None,
+) -> tuple[Finder | _MetaPathFinder, ModuleSpec]:
+    for finder in _SPEC_FINDERS:
+        finder_instance = finder(search_path)
+        spec = finder_instance.find_module(
+            modname, module_parts, processed, submodule_path
+        )
         if spec is None:
             continue
-        return finder, spec
+        return finder_instance, spec
+
+    # Support for custom finders
+    for meta_finder in sys.meta_path:
+        # See if we support the customer import hook of the meta_finder
+        meta_finder_name = meta_finder.__class__.__name__
+        if meta_finder_name not in _MetaPathFinderModuleTypes:
+            # Setuptools>62 creates its EditableFinders dynamically and have
+            # "type" as their __class__.__name__. We check __name__ as well
+            # to see if we can support the finder.
+            try:
+                meta_finder_name = meta_finder.__name__
+            except AttributeError:
+                continue
+            if meta_finder_name not in _MetaPathFinderModuleTypes:
+                continue
+
+        module_type = _MetaPathFinderModuleTypes[meta_finder_name]
+
+        # Meta path finders are supposed to have a find_spec method since
+        # Python 3.4. However, some third-party finders do not implement it.
+        # PEP302 does not refer to find_spec as well.
+        # See: https://github.com/pylint-dev/astroid/pull/1752/
+        if not hasattr(meta_finder, "find_spec"):
+            continue
+
+        spec = meta_finder.find_spec(modname, submodule_path)
+        if spec:
+            return (
+                meta_finder,
+                ModuleSpec(
+                    spec.name,
+                    module_type,
+                    spec.origin,
+                    spec.origin,
+                    spec.submodule_search_locations,
+                ),
+            )
 
     raise ImportError(f"No module named {'.'.join(module_parts)}")
 
 
-def find_spec(modpath, path=None):
+def find_spec(modpath: list[str], path: Sequence[str] | None = None) -> ModuleSpec:
     """Find a spec for the given module.
 
     :type modpath: list or tuple
     :param modpath:
       split module's name (i.e name of a module or package split
       on '.'), with leading empty strings for explicit relative import
 
@@ -348,22 +444,27 @@
     _path = path or sys.path
 
     # Need a copy for not mutating the argument.
     modpath = modpath[:]
 
     submodule_path = None
     module_parts = modpath[:]
-    processed = []
+    processed: list[str] = []
 
     while modpath:
         modname = modpath.pop(0)
         finder, spec = _find_spec_with_path(
             _path, modname, module_parts, processed, submodule_path or path
         )
         processed.append(modname)
         if modpath:
-            submodule_path = finder.contribute_to_path(spec, processed)
+            if isinstance(finder, Finder):
+                submodule_path = finder.contribute_to_path(spec, processed)
+            # If modname is a package from an editable install, update submodule_path
+            # so that the next module in the path will be found inside of it using importlib.
+            elif finder.__name__ in _EditableFinderClasses:
+                submodule_path = spec.submodule_search_locations
 
         if spec.type == ModuleType.PKG_DIRECTORY:
             spec = spec._replace(submodule_search_locations=submodule_path)
 
     return spec
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a1/astroid/interpreter/dunder_lookup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# Copyright (c) 2016-2018 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Contains logic for retrieving special methods.
 
 This implementation does not rely on the dot attribute access
 logic, found in ``.getattr()``. The difference between these two
 is that the dunder methods are looked with the type slots
 (you can find more about these here
@@ -16,29 +14,29 @@
 """
 import itertools
 
 import astroid
 from astroid.exceptions import AttributeInferenceError
 
 
-def _lookup_in_mro(node, name):
+def _lookup_in_mro(node, name) -> list:
     attrs = node.locals.get(name, [])
 
     nodes = itertools.chain.from_iterable(
         ancestor.locals.get(name, []) for ancestor in node.ancestors(recurs=True)
     )
     values = list(itertools.chain(attrs, nodes))
     if not values:
         raise AttributeInferenceError(attribute=name, target=node)
 
     return values
 
 
-def lookup(node, name):
-    """Lookup the given special method name in the given *node*
+def lookup(node, name) -> list:
+    """Lookup the given special method name in the given *node*.
 
     If the special method was found, then a list of attributes
     will be returned. Otherwise, `astroid.AttributeInferenceError`
     is going to be raised.
     """
     if isinstance(
         node, (astroid.List, astroid.Tuple, astroid.Const, astroid.Dict, astroid.Set)
@@ -48,21 +46,21 @@
         return _lookup_in_mro(node, name)
     if isinstance(node, astroid.ClassDef):
         return _class_lookup(node, name)
 
     raise AttributeInferenceError(attribute=name, target=node)
 
 
-def _class_lookup(node, name):
+def _class_lookup(node, name) -> list:
     metaclass = node.metaclass()
     if metaclass is None:
         raise AttributeInferenceError(attribute=name, target=node)
 
     return _lookup_in_mro(metaclass, name)
 
 
-def _builtin_lookup(node, name):
+def _builtin_lookup(node, name) -> list:
     values = node.locals.get(name, [])
     if not values:
         raise AttributeInferenceError(attribute=name, target=node)
 
     return values
```

### Comparing `astroid-2.9.3/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a1/astroid/interpreter/objectmodel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-# Copyright (c) 2016-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017-2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2017 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2017 Calen Pennington <cale@edx.org>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 """
 Data object model, as per https://docs.python.org/3/reference/datamodel.html.
 
 This module describes, at least partially, a data object model for some
 of astroid's nodes. The model contains special attributes that nodes such
 as functions, classes, modules etc have, such as __doc__, __class__,
 __module__ etc, being used when doing attribute lookups over nodes.
@@ -26,34 +17,37 @@
 and the lookup mechanism will try to see if attributes such as
 `__class__` are defined by the model or not. If they are defined,
 the model will be requested to return the corresponding value of that
 attribute. Thus the model can be viewed as a special part of the lookup
 mechanism.
 """
 
+from __future__ import annotations
+
 import itertools
 import os
 import pprint
 import types
+from collections.abc import Iterator
 from functools import lru_cache
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Literal
 
 import astroid
-from astroid import util
+from astroid import bases, nodes, util
 from astroid.context import InferenceContext, copy_context
 from astroid.exceptions import AttributeInferenceError, InferenceError, NoDefault
 from astroid.manager import AstroidManager
 from astroid.nodes import node_classes
-
-objects = util.lazy_import("objects")
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid.objects import Property
 
 IMPL_PREFIX = "attr_"
+LEN_OF_IMPL_PREFIX = len(IMPL_PREFIX)
 
 
 def _dunder_dict(instance, attributes):
     obj = node_classes.Dict(parent=instance)
 
     # Convert the keys to node strings
     keys = [
@@ -65,14 +59,22 @@
     # In this case, we're picking the last value from each list.
     values = [elem[-1] for elem in attributes.values()]
 
     obj.postinit(list(zip(keys, values)))
     return obj
 
 
+def _get_bound_node(model: ObjectModel) -> Any:
+    # TODO: Use isinstance instead of try ... except after _instance has typing
+    try:
+        return model._instance._proxied
+    except AttributeError:
+        return model._instance
+
+
 class ObjectModel:
     def __init__(self):
         self._instance = None
 
     def __repr__(self):
         result = []
         cname = type(self).__name__
@@ -102,35 +104,63 @@
         # But at the same time, node.special_attributes should return an object
         # which can be used for manipulating the special attributes. That's the reason
         # we pass the instance through which it got accessed to ObjectModel.__call__,
         # returning itself afterwards, so we can still have access to the
         # underlying data model and to the instance for which it got accessed.
         return self(instance)
 
-    def __contains__(self, name):
+    def __contains__(self, name) -> bool:
         return name in self.attributes()
 
-    @lru_cache(maxsize=None)
-    def attributes(self):
+    @lru_cache  # noqa
+    def attributes(self) -> list[str]:
         """Get the attributes which are exported by this object model."""
-        return [
-            obj[len(IMPL_PREFIX) :] for obj in dir(self) if obj.startswith(IMPL_PREFIX)
-        ]
+        return [o[LEN_OF_IMPL_PREFIX:] for o in dir(self) if o.startswith(IMPL_PREFIX)]
 
     def lookup(self, name):
-        """Look up the given *name* in the current model
+        """Look up the given *name* in the current model.
 
         It should return an AST or an interpreter object,
         but if the name is not found, then an AttributeInferenceError will be raised.
         """
-
         if name in self.attributes():
             return getattr(self, IMPL_PREFIX + name)
         raise AttributeInferenceError(target=self._instance, attribute=name)
 
+    @property
+    def attr___new__(self) -> bases.BoundMethod:
+        """Calling cls.__new__(type) on an object returns an instance of 'type'."""
+        from astroid import builder  # pylint: disable=import-outside-toplevel
+
+        node: nodes.FunctionDef = builder.extract_node(
+            """def __new__(self, cls): return cls()"""
+        )
+        # We set the parent as being the ClassDef of 'object' as that
+        # triggers correct inference as a call to __new__ in bases.py
+        node.parent = AstroidManager().builtins_module["object"]
+
+        return bases.BoundMethod(proxy=node, bound=_get_bound_node(self))
+
+    @property
+    def attr___init__(self) -> bases.BoundMethod:
+        """Calling cls.__init__() normally returns None."""
+        from astroid import builder  # pylint: disable=import-outside-toplevel
+
+        # The *args and **kwargs are necessary not to trigger warnings about missing
+        # or extra parameters for '__init__' methods we don't infer correctly.
+        # This BoundMethod is the fallback value for those.
+        node: nodes.FunctionDef = builder.extract_node(
+            """def __init__(self, *args, **kwargs): return None"""
+        )
+        # We set the parent as being the ClassDef of 'object' as that
+        # is where this method originally comes from
+        node.parent = AstroidManager().builtins_module["object"]
+
+        return bases.BoundMethod(proxy=node, bound=_get_bound_node(self))
+
 
 class ModuleModel(ObjectModel):
     def _builtins(self):
         builtins_ast_module = AstroidManager().builtins_module
         return builtins_ast_module.special_attributes.lookup("__dict__")
 
     @property
@@ -159,15 +189,18 @@
 
     @property
     def attr___name__(self):
         return node_classes.Const(value=self._instance.name, parent=self._instance)
 
     @property
     def attr___doc__(self):
-        return node_classes.Const(value=self._instance.doc, parent=self._instance)
+        return node_classes.Const(
+            value=getattr(self._instance.doc_node, "value", None),
+            parent=self._instance,
+        )
 
     @property
     def attr___file__(self):
         return node_classes.Const(value=self._instance.file, parent=self._instance)
 
     @property
     def attr___dict__(self):
@@ -205,15 +238,18 @@
 class FunctionModel(ObjectModel):
     @property
     def attr___name__(self):
         return node_classes.Const(value=self._instance.name, parent=self._instance)
 
     @property
     def attr___doc__(self):
-        return node_classes.Const(value=self._instance.doc, parent=self._instance)
+        return node_classes.Const(
+            value=getattr(self._instance.doc_node, "value", None),
+            parent=self._instance,
+        )
 
     @property
     def attr___qualname__(self):
         return node_classes.Const(value=self._instance.qname(), parent=self._instance)
 
     @property
     def attr___defaults__(self):
@@ -286,94 +322,118 @@
 
     @property
     def attr___module__(self):
         return node_classes.Const(self._instance.root().qname())
 
     @property
     def attr___get__(self):
-        # pylint: disable=import-outside-toplevel; circular import
-        from astroid import bases
-
         func = self._instance
 
         class DescriptorBoundMethod(bases.BoundMethod):
-            """Bound method which knows how to understand calling descriptor binding."""
+            """Bound method which knows how to understand calling descriptor
+            binding.
+            """
 
-            def implicit_parameters(self):
+            def implicit_parameters(self) -> Literal[0]:
                 # Different than BoundMethod since the signature
                 # is different.
                 return 0
 
-            def infer_call_result(self, caller, context=None):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[bases.BoundMethod]:
                 if len(caller.args) > 2 or len(caller.args) < 1:
                     raise InferenceError(
                         "Invalid arguments for descriptor binding",
                         target=self,
                         context=context,
                     )
 
                 context = copy_context(context)
                 try:
                     cls = next(caller.args[0].infer(context=context))
                 except StopIteration as e:
                     raise InferenceError(context=context, node=caller.args[0]) from e
 
-                if cls is astroid.Uninferable:
+                if isinstance(cls, util.UninferableBase):
                     raise InferenceError(
                         "Invalid class inferred", target=self, context=context
                     )
 
                 # For some reason func is a Node that the below
                 # code is not expecting
                 if isinstance(func, bases.BoundMethod):
                     yield func
                     return
 
                 # Rebuild the original value, but with the parent set as the
                 # class where it will be bound.
                 new_func = func.__class__(
                     name=func.name,
-                    doc=func.doc,
                     lineno=func.lineno,
                     col_offset=func.col_offset,
                     parent=func.parent,
+                    end_lineno=func.end_lineno,
+                    end_col_offset=func.end_col_offset,
                 )
                 # pylint: disable=no-member
-                new_func.postinit(func.args, func.body, func.decorators, func.returns)
+                new_func.postinit(
+                    func.args,
+                    func.body,
+                    func.decorators,
+                    func.returns,
+                    doc_node=func.doc_node,
+                )
 
                 # Build a proper bound method that points to our newly built function.
                 proxy = bases.UnboundMethod(new_func)
                 yield bases.BoundMethod(proxy=proxy, bound=cls)
 
             @property
             def args(self):
-                """Overwrite the underlying args to match those of the underlying func
+                """Overwrite the underlying args to match those of the underlying func.
 
                 Usually the underlying *func* is a function/method, as in:
 
                     def test(self):
                         pass
 
                 This has only the *self* parameter but when we access test.__get__
                 we get a new object which has two parameters, *self* and *type*.
                 """
                 nonlocal func
+                arguments = astroid.Arguments(
+                    parent=func.args.parent, vararg=None, kwarg=None
+                )
+
                 positional_or_keyword_params = func.args.args.copy()
-                positional_or_keyword_params.append(astroid.AssignName(name="type"))
+                positional_or_keyword_params.append(
+                    astroid.AssignName(
+                        name="type",
+                        lineno=0,
+                        col_offset=0,
+                        parent=arguments,
+                        end_lineno=None,
+                        end_col_offset=None,
+                    )
+                )
 
                 positional_only_params = func.args.posonlyargs.copy()
 
-                arguments = astroid.Arguments(parent=func.args.parent)
                 arguments.postinit(
                     args=positional_or_keyword_params,
                     posonlyargs=positional_only_params,
                     defaults=[],
                     kwonlyargs=[],
                     kw_defaults=[],
                     annotations=[],
+                    kwonlyargs_annotations=[],
+                    posonlyargs_annotations=[],
                 )
                 return arguments
 
         return DescriptorBoundMethod(proxy=self._instance, bound=self._instance)
 
     # These are here just for completion.
     @property
@@ -383,23 +443,21 @@
     attr___subclasshook__ = attr___ne__
     attr___str__ = attr___ne__
     attr___sizeof__ = attr___ne__
     attr___setattr___ = attr___ne__
     attr___repr__ = attr___ne__
     attr___reduce__ = attr___ne__
     attr___reduce_ex__ = attr___ne__
-    attr___new__ = attr___ne__
     attr___lt__ = attr___ne__
     attr___eq__ = attr___ne__
     attr___gt__ = attr___ne__
     attr___format__ = attr___ne__
     attr___delattr___ = attr___ne__
     attr___getattribute__ = attr___ne__
     attr___hash__ = attr___ne__
-    attr___init__ = attr___ne__
     attr___dir__ = attr___ne__
     attr___call__ = attr___ne__
     attr___class__ = attr___ne__
     attr___closure__ = attr___ne__
     attr___code__ = attr___ne__
 
 
@@ -420,15 +478,15 @@
 
     @property
     def attr___qualname__(self):
         return node_classes.Const(self._instance.qname())
 
     @property
     def attr___doc__(self):
-        return node_classes.Const(self._instance.doc)
+        return node_classes.Const(getattr(self._instance.doc_node, "value", None))
 
     @property
     def attr___mro__(self):
         if not self._instance.newstyle:
             raise AttributeInferenceError(target=self._instance, attribute="__mro__")
 
         mro = self._instance.mro()
@@ -437,23 +495,24 @@
         return obj
 
     @property
     def attr_mro(self):
         if not self._instance.newstyle:
             raise AttributeInferenceError(target=self._instance, attribute="mro")
 
-        # pylint: disable=import-outside-toplevel; circular import
-        from astroid import bases
-
         other_self = self
 
         # Cls.mro is a method and we need to return one in order to have a proper inference.
         # The method we're returning is capable of inferring the underlying MRO though.
         class MroBoundMethod(bases.BoundMethod):
-            def infer_call_result(self, caller, context=None):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[node_classes.Tuple]:
                 yield other_self.attr___mro__
 
         implicit_metaclass = self._instance.implicit_metaclass()
         mro_method = implicit_metaclass.locals["mro"][0]
         return MroBoundMethod(proxy=mro_method, bound=implicit_metaclass)
 
     @property
@@ -469,51 +528,56 @@
         # pylint: disable=import-outside-toplevel; circular import
         from astroid import helpers
 
         return helpers.object_type(self._instance)
 
     @property
     def attr___subclasses__(self):
-        """Get the subclasses of the underlying class
+        """Get the subclasses of the underlying class.
 
         This looks only in the current module for retrieving the subclasses,
         thus it might miss a couple of them.
         """
-        # pylint: disable=import-outside-toplevel; circular import
-        from astroid import bases
-        from astroid.nodes import scoped_nodes
-
         if not self._instance.newstyle:
             raise AttributeInferenceError(
                 target=self._instance, attribute="__subclasses__"
             )
 
         qname = self._instance.qname()
         root = self._instance.root()
         classes = [
             cls
-            for cls in root.nodes_of_class(scoped_nodes.ClassDef)
+            for cls in root.nodes_of_class(nodes.ClassDef)
             if cls != self._instance and cls.is_subtype_of(qname, context=self.context)
         ]
 
         obj = node_classes.List(parent=self._instance)
         obj.postinit(classes)
 
         class SubclassesBoundMethod(bases.BoundMethod):
-            def infer_call_result(self, caller, context=None):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[node_classes.List]:
                 yield obj
 
         implicit_metaclass = self._instance.implicit_metaclass()
         subclasses_method = implicit_metaclass.locals["__subclasses__"][0]
         return SubclassesBoundMethod(proxy=subclasses_method, bound=implicit_metaclass)
 
     @property
     def attr___dict__(self):
         return node_classes.Dict(parent=self._instance)
 
+    @property
+    def attr___call__(self):
+        """Calling a class A() returns an instance of A."""
+        return self._instance.instantiate_class()
+
 
 class SuperModel(ObjectModel):
     @property
     def attr___thisclass__(self):
         return self._instance.mro_pointer
 
     @property
@@ -546,25 +610,71 @@
         return node_classes.Const(value=None, parent=self._instance)
 
     attr_im_func = attr___func__
     attr_im_class = attr___class__
     attr_im_self = attr___self__
 
 
+class ContextManagerModel(ObjectModel):
+    """Model for context managers.
+
+    Based on 3.3.9 of the Data Model documentation:
+    https://docs.python.org/3/reference/datamodel.html#with-statement-context-managers
+    """
+
+    @property
+    def attr___enter__(self) -> bases.BoundMethod:
+        """Representation of the base implementation of __enter__.
+
+        As per Python documentation:
+        Enter the runtime context related to this object. The with statement
+        will bind this method's return value to the target(s) specified in the
+        as clause of the statement, if any.
+        """
+        from astroid import builder  # pylint: disable=import-outside-toplevel
+
+        node: nodes.FunctionDef = builder.extract_node("""def __enter__(self): ...""")
+        # We set the parent as being the ClassDef of 'object' as that
+        # is where this method originally comes from
+        node.parent = AstroidManager().builtins_module["object"]
+
+        return bases.BoundMethod(proxy=node, bound=_get_bound_node(self))
+
+    @property
+    def attr___exit__(self) -> bases.BoundMethod:
+        """Representation of the base implementation of __exit__.
+
+        As per Python documentation:
+        Exit the runtime context related to this object. The parameters describe the
+        exception that caused the context to be exited. If the context was exited
+        without an exception, all three arguments will be None.
+        """
+        from astroid import builder  # pylint: disable=import-outside-toplevel
+
+        node: nodes.FunctionDef = builder.extract_node(
+            """def __exit__(self, exc_type, exc_value, traceback): ..."""
+        )
+        # We set the parent as being the ClassDef of 'object' as that
+        # is where this method originally comes from
+        node.parent = AstroidManager().builtins_module["object"]
+
+        return bases.BoundMethod(proxy=node, bound=_get_bound_node(self))
+
+
 class BoundMethodModel(FunctionModel):
     @property
     def attr___func__(self):
         return self._instance._proxied._proxied
 
     @property
     def attr___self__(self):
         return self._instance.bound
 
 
-class GeneratorModel(FunctionModel):
+class GeneratorModel(FunctionModel, ContextManagerModel):
     def __new__(cls, *args, **kwargs):
         # Append the values from the GeneratorType unto this object.
         ret = super().__new__(cls, *args, **kwargs)
         generator = AstroidManager().builtins_module["generator"]
         for name, values in generator.locals.items():
             method = values[0]
 
@@ -580,15 +690,16 @@
         return node_classes.Const(
             value=self._instance.parent.name, parent=self._instance
         )
 
     @property
     def attr___doc__(self):
         return node_classes.Const(
-            value=self._instance.parent.doc, parent=self._instance
+            value=getattr(self._instance.parent.doc_node, "value", None),
+            parent=self._instance,
         )
 
 
 class AsyncGeneratorModel(GeneratorModel):
     def __new__(cls, *args, **kwargs):
         # Append the values from the AGeneratorType unto this object.
         ret = super().__new__(cls, *args, **kwargs)
@@ -616,31 +727,28 @@
 
     @property
     def attr___module__(self):
         return node_classes.Const(self._instance.root().qname())
 
     @property
     def attr___doc__(self):
-        return node_classes.Const(self._instance.doc)
+        return node_classes.Const(getattr(self._instance.doc_node, "value", None))
 
     @property
     def attr___dict__(self):
         return _dunder_dict(self._instance, self._instance.instance_attrs)
 
 
 # Exception instances
 
 
 class ExceptionInstanceModel(InstanceModel):
     @property
-    def attr_args(self):
-        message = node_classes.Const("")
-        args = node_classes.Tuple(parent=self._instance)
-        args.postinit((message,))
-        return args
+    def attr_args(self) -> nodes.Tuple:
+        return nodes.Tuple(parent=self._instance)
 
     @property
     def attr___traceback__(self):
         builtins_ast_module = AstroidManager().builtins_module
         traceback_type = builtins_ast_module[types.TracebackType.__name__]
         return traceback_type.instantiate_class()
 
@@ -712,107 +820,126 @@
     def attr___class__(self):
         return self._instance._proxied
 
     def _generic_dict_attribute(self, obj, name):
         """Generate a bound method that can infer the given *obj*."""
 
         class DictMethodBoundMethod(astroid.BoundMethod):
-            def infer_call_result(self, caller, context=None):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[InferenceResult]:
                 yield obj
 
         meth = next(self._instance._proxied.igetattr(name), None)
         return DictMethodBoundMethod(proxy=meth, bound=self._instance)
 
     @property
     def attr_items(self):
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         elems = []
         obj = node_classes.List(parent=self._instance)
         for key, value in self._instance.items:
             elem = node_classes.Tuple(parent=obj)
             elem.postinit((key, value))
             elems.append(elem)
         obj.postinit(elts=elems)
 
-        obj = objects.DictItems(obj)
-        return self._generic_dict_attribute(obj, "items")
+        items_obj = objects.DictItems(obj)
+        return self._generic_dict_attribute(items_obj, "items")
 
     @property
     def attr_keys(self):
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         keys = [key for (key, _) in self._instance.items]
         obj = node_classes.List(parent=self._instance)
         obj.postinit(elts=keys)
 
-        obj = objects.DictKeys(obj)
-        return self._generic_dict_attribute(obj, "keys")
+        keys_obj = objects.DictKeys(obj)
+        return self._generic_dict_attribute(keys_obj, "keys")
 
     @property
     def attr_values(self):
+        from astroid import objects  # pylint: disable=import-outside-toplevel
 
         values = [value for (_, value) in self._instance.items]
         obj = node_classes.List(parent=self._instance)
         obj.postinit(values)
 
-        obj = objects.DictValues(obj)
-        return self._generic_dict_attribute(obj, "values")
+        values_obj = objects.DictValues(obj)
+        return self._generic_dict_attribute(values_obj, "values")
 
 
 class PropertyModel(ObjectModel):
-    """Model for a builtin property"""
+    """Model for a builtin property."""
 
-    # pylint: disable=import-outside-toplevel
     def _init_function(self, name):
-        from astroid.nodes.node_classes import Arguments
-        from astroid.nodes.scoped_nodes import FunctionDef
+        function = nodes.FunctionDef(
+            name=name,
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
 
-        args = Arguments()
+        args = nodes.Arguments(parent=function, vararg=None, kwarg=None)
         args.postinit(
             args=[],
             defaults=[],
             kwonlyargs=[],
             kw_defaults=[],
             annotations=[],
             posonlyargs=[],
             posonlyargs_annotations=[],
             kwonlyargs_annotations=[],
         )
 
-        function = FunctionDef(name=name, parent=self._instance)
-
         function.postinit(args=args, body=[])
         return function
 
     @property
     def attr_fget(self):
-        from astroid.nodes.scoped_nodes import FunctionDef
-
         func = self._instance
 
-        class PropertyFuncAccessor(FunctionDef):
-            def infer_call_result(self, caller=None, context=None):
+        class PropertyFuncAccessor(nodes.FunctionDef):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[InferenceResult]:
                 nonlocal func
                 if caller and len(caller.args) != 1:
                     raise InferenceError(
                         "fget() needs a single argument", target=self, context=context
                     )
 
                 yield from func.function.infer_call_result(
                     caller=caller, context=context
                 )
 
-        property_accessor = PropertyFuncAccessor(name="fget", parent=self._instance)
+        property_accessor = PropertyFuncAccessor(
+            name="fget",
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
         property_accessor.postinit(args=func.args, body=func.body)
         return property_accessor
 
     @property
     def attr_fset(self):
-        from astroid.nodes.scoped_nodes import FunctionDef
-
         func = self._instance
 
-        def find_setter(func: "Property") -> Optional[astroid.FunctionDef]:
+        def find_setter(func: Property) -> astroid.FunctionDef | None:
             """
             Given a property, find the corresponding setter function and returns it.
 
             :param func: property for which the setter has to be found
             :return: the setter function or None
             """
             for target in [
@@ -825,24 +952,35 @@
 
         func_setter = find_setter(func)
         if not func_setter:
             raise InferenceError(
                 f"Unable to find the setter of property {func.function.name}"
             )
 
-        class PropertyFuncAccessor(FunctionDef):
-            def infer_call_result(self, caller=None, context=None):
+        class PropertyFuncAccessor(nodes.FunctionDef):
+            def infer_call_result(
+                self,
+                caller: SuccessfulInferenceResult | None,
+                context: InferenceContext | None = None,
+            ) -> Iterator[InferenceResult]:
                 nonlocal func_setter
                 if caller and len(caller.args) != 2:
                     raise InferenceError(
                         "fset() needs two arguments", target=self, context=context
                     )
                 yield from func_setter.infer_call_result(caller=caller, context=context)
 
-        property_accessor = PropertyFuncAccessor(name="fset", parent=self._instance)
+        property_accessor = PropertyFuncAccessor(
+            name="fset",
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
         property_accessor.postinit(args=func_setter.args, body=func_setter.body)
         return property_accessor
 
     @property
     def attr_setter(self):
         return self._init_function("setter")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/manager.py` & `astroid-3.0.0a1/astroid/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,190 @@
-# Copyright (c) 2006-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2014-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 BioGeek <jeroen.vangoey@gmail.com>
-# Copyright (c) 2014 Google, Inc.
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017 Iva Miholic <ivamiho@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2019 Raphael Gaschignard <raphael@makeleaps.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Raphael Gaschignard <raphael@rtpg.co>
-# Copyright (c) 2020 Anubhav <35621759+anubh-v@users.noreply.github.com>
-# Copyright (c) 2020 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 grayjk <grayjk@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-# Copyright (c) 2021 DudeNr33 <3929834+DudeNr33@users.noreply.github.com>
-# Copyright (c) 2021 pre-commit-ci[bot] <bot@noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """astroid manager: avoid multiple astroid build of a same module when
 possible by providing a class responsible to get astroid representation
 from various source and using a cache of built modules)
 """
 
+from __future__ import annotations
+
+import collections
 import os
 import types
 import zipimport
-from typing import TYPE_CHECKING, ClassVar, List, Optional
-
+from collections.abc import Callable, Iterator, Sequence
+from importlib.util import find_spec, module_from_spec
+from typing import Any, ClassVar
+
+from astroid import nodes
+from astroid.const import BRAIN_MODULES_DIRECTORY
+from astroid.context import InferenceContext, _invalidate_cache
 from astroid.exceptions import AstroidBuildingError, AstroidImportError
-from astroid.interpreter._import import spec
+from astroid.interpreter._import import spec, util
 from astroid.modutils import (
     NoSourceFile,
+    _cache_normalize_path_,
     file_info_from_modpath,
     get_source_file,
     is_module_name_part_of_extension_package_whitelist,
     is_python_source,
-    is_standard_module,
+    is_stdlib_module,
     load_module_from_name,
     modpath_from_file,
 )
 from astroid.transforms import TransformVisitor
-
-if TYPE_CHECKING:
-    from astroid import nodes
+from astroid.typing import AstroidManagerBrain, InferenceResult
 
 ZIP_IMPORT_EXTS = (".zip", ".egg", ".whl", ".pyz", ".pyzw")
 
 
-def safe_repr(obj):
+def safe_repr(obj: Any) -> str:
     try:
         return repr(obj)
     except Exception:  # pylint: disable=broad-except
         return "???"
 
 
 class AstroidManager:
     """Responsible to build astroid from files or modules.
 
     Use the Borg (singleton) pattern.
     """
 
     name = "astroid loader"
-    brain = {}
+    brain: AstroidManagerBrain = {
+        "astroid_cache": {},
+        "_mod_file_cache": {},
+        "_failed_import_hooks": [],
+        "always_load_extensions": False,
+        "optimize_ast": False,
+        "extension_package_whitelist": set(),
+        "_transform": TransformVisitor(),
+    }
     max_inferable_values: ClassVar[int] = 100
 
-    def __init__(self):
-        self.__dict__ = AstroidManager.brain
-        if not self.__dict__:
-            # NOTE: cache entries are added by the [re]builder
-            self.astroid_cache = {}
-            self._mod_file_cache = {}
-            self._failed_import_hooks = []
-            self.always_load_extensions = False
-            self.optimize_ast = False
-            self.extension_package_whitelist = set()
-            self._transform = TransformVisitor()
+    def __init__(self) -> None:
+        # NOTE: cache entries are added by the [re]builder
+        self.astroid_cache = AstroidManager.brain["astroid_cache"]
+        self._mod_file_cache = AstroidManager.brain["_mod_file_cache"]
+        self._failed_import_hooks = AstroidManager.brain["_failed_import_hooks"]
+        self.always_load_extensions = AstroidManager.brain["always_load_extensions"]
+        self.optimize_ast = AstroidManager.brain["optimize_ast"]
+        self.extension_package_whitelist = AstroidManager.brain[
+            "extension_package_whitelist"
+        ]
+        self._transform = AstroidManager.brain["_transform"]
 
     @property
     def register_transform(self):
         # This and unregister_transform below are exported for convenience
         return self._transform.register_transform
 
     @property
     def unregister_transform(self):
         return self._transform.unregister_transform
 
     @property
-    def builtins_module(self):
+    def builtins_module(self) -> nodes.Module:
         return self.astroid_cache["builtins"]
 
-    def visit_transforms(self, node):
+    def visit_transforms(self, node: nodes.NodeNG) -> InferenceResult:
         """Visit the transforms and apply them to the given *node*."""
         return self._transform.visit(node)
 
-    def ast_from_file(self, filepath, modname=None, fallback=True, source=False):
-        """given a module name, return the astroid object"""
-        try:
-            filepath = get_source_file(filepath, include_no_ext=True)
-            source = True
-        except NoSourceFile:
-            pass
+    def ast_from_file(
+        self,
+        filepath: str,
+        modname: str | None = None,
+        fallback: bool = True,
+        source: bool = False,
+    ) -> nodes.Module:
+        """Given a module name, return the astroid object."""
         if modname is None:
             try:
                 modname = ".".join(modpath_from_file(filepath))
             except ImportError:
                 modname = filepath
         if (
             modname in self.astroid_cache
             and self.astroid_cache[modname].file == filepath
         ):
             return self.astroid_cache[modname]
+        # Call get_source_file() only after a cache miss,
+        # since it calls os.path.exists().
+        try:
+            filepath = get_source_file(filepath, include_no_ext=True)
+            source = True
+        except NoSourceFile:
+            pass
+        # Second attempt on the cache after get_source_file().
+        if (
+            modname in self.astroid_cache
+            and self.astroid_cache[modname].file == filepath
+        ):
+            return self.astroid_cache[modname]
         if source:
             # pylint: disable=import-outside-toplevel; circular import
             from astroid.builder import AstroidBuilder
 
             return AstroidBuilder(self).file_build(filepath, modname)
         if fallback and modname:
             return self.ast_from_module_name(modname)
         raise AstroidBuildingError("Unable to build an AST for {path}.", path=filepath)
 
-    def ast_from_string(self, data, modname="", filepath=None):
-        """Given some source code as a string, return its corresponding astroid object"""
+    def ast_from_string(
+        self, data: str, modname: str = "", filepath: str | None = None
+    ) -> nodes.Module:
+        """Given some source code as a string, return its corresponding astroid
+        object.
+        """
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.builder import AstroidBuilder
 
         return AstroidBuilder(self).string_build(data, modname, filepath)
 
-    def _build_stub_module(self, modname):
+    def _build_stub_module(self, modname: str) -> nodes.Module:
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.builder import AstroidBuilder
 
         return AstroidBuilder(self).string_build("", modname)
 
-    def _build_namespace_module(self, modname: str, path: List[str]) -> "nodes.Module":
+    def _build_namespace_module(
+        self, modname: str, path: Sequence[str]
+    ) -> nodes.Module:
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.builder import build_namespace_package_module
 
         return build_namespace_package_module(modname, path)
 
     def _can_load_extension(self, modname: str) -> bool:
         if self.always_load_extensions:
             return True
-        if is_standard_module(modname):
+        if is_stdlib_module(modname):
             return True
         return is_module_name_part_of_extension_package_whitelist(
             modname, self.extension_package_whitelist
         )
 
-    def ast_from_module_name(self, modname, context_file=None):
-        """given a module name, return the astroid object"""
-        if modname in self.astroid_cache:
+    def ast_from_module_name(  # noqa: C901
+        self,
+        modname: str | None,
+        context_file: str | None = None,
+        use_cache: bool = True,
+    ) -> nodes.Module:
+        """Given a module name, return the astroid object."""
+        if modname is None:
+            raise AstroidBuildingError("No module name given.")
+        # Sometimes we don't want to use the cache. For example, when we're
+        # importing a module with the same name as the file that is importing
+        # we want to fallback on the import system to make sure we get the correct
+        # module.
+        if modname in self.astroid_cache and use_cache:
             return self.astroid_cache[modname]
         if modname == "__main__":
             return self._build_stub_module(modname)
         if context_file:
             old_cwd = os.getcwd()
             os.chdir(os.path.dirname(context_file))
         try:
@@ -176,36 +200,40 @@
             ):
                 if (
                     found_spec.type == spec.ModuleType.C_EXTENSION
                     and not self._can_load_extension(modname)
                 ):
                     return self._build_stub_module(modname)
                 try:
-                    module = load_module_from_name(modname)
+                    named_module = load_module_from_name(modname)
                 except Exception as e:
                     raise AstroidImportError(
                         "Loading {modname} failed with:\n{error}",
                         modname=modname,
                         path=found_spec.location,
                     ) from e
-                return self.ast_from_module(module, modname)
+                return self.ast_from_module(named_module, modname)
 
             elif found_spec.type == spec.ModuleType.PY_COMPILED:
                 raise AstroidImportError(
                     "Unable to load compiled module {modname}.",
                     modname=modname,
                     path=found_spec.location,
                 )
 
             elif found_spec.type == spec.ModuleType.PY_NAMESPACE:
                 return self._build_namespace_module(
-                    modname, found_spec.submodule_search_locations
+                    modname, found_spec.submodule_search_locations or []
                 )
             elif found_spec.type == spec.ModuleType.PY_FROZEN:
-                return self._build_stub_module(modname)
+                if found_spec.location is None:
+                    return self._build_stub_module(modname)
+                # For stdlib frozen modules we can determine the location and
+                # can therefore create a module from the source file
+                return self.ast_from_file(found_spec.location, modname, fallback=False)
 
             if found_spec.location is None:
                 raise AstroidImportError(
                     "Can't find a file for module {modname}.", modname=modname
                 )
 
             return self.ast_from_file(found_spec.location, modname, fallback=False)
@@ -216,15 +244,15 @@
                 except AstroidBuildingError:
                     pass
             raise e
         finally:
             if context_file:
                 os.chdir(old_cwd)
 
-    def zip_import_data(self, filepath):
+    def zip_import_data(self, filepath: str) -> nodes.Module | None:
         if zipimport is None:
             return None
 
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.builder import AstroidBuilder
 
         builder = AstroidBuilder(self)
@@ -243,74 +271,90 @@
                     importer.get_source(resource), zmodname, filepath
                 )
                 return module
             except Exception:  # pylint: disable=broad-except
                 continue
         return None
 
-    def file_from_module_name(self, modname, contextfile):
+    def file_from_module_name(
+        self, modname: str, contextfile: str | None
+    ) -> spec.ModuleSpec:
         try:
             value = self._mod_file_cache[(modname, contextfile)]
         except KeyError:
             try:
                 value = file_info_from_modpath(
                     modname.split("."), context_file=contextfile
                 )
             except ImportError as e:
+                # pylint: disable-next=redefined-variable-type
                 value = AstroidImportError(
                     "Failed to import module {modname} with error:\n{error}.",
                     modname=modname,
                     # we remove the traceback here to save on memory usage (since these exceptions are cached)
                     error=e.with_traceback(None),
                 )
             self._mod_file_cache[(modname, contextfile)] = value
         if isinstance(value, AstroidBuildingError):
             # we remove the traceback here to save on memory usage (since these exceptions are cached)
-            raise value.with_traceback(None)
+            raise value.with_traceback(None)  # pylint: disable=no-member
         return value
 
-    def ast_from_module(self, module: types.ModuleType, modname: Optional[str] = None):
-        """given an imported module, return the astroid object"""
+    def ast_from_module(
+        self, module: types.ModuleType, modname: str | None = None
+    ) -> nodes.Module:
+        """Given an imported module, return the astroid object."""
         modname = modname or module.__name__
         if modname in self.astroid_cache:
             return self.astroid_cache[modname]
         try:
             # some builtin modules don't have __file__ attribute
             filepath = module.__file__
             if is_python_source(filepath):
-                return self.ast_from_file(filepath, modname)
+                # Type is checked in is_python_source
+                return self.ast_from_file(filepath, modname)  # type: ignore[arg-type]
         except AttributeError:
             pass
 
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.builder import AstroidBuilder
 
         return AstroidBuilder(self).module_build(module, modname)
 
-    def ast_from_class(self, klass, modname=None):
-        """get astroid for the given class"""
+    def ast_from_class(self, klass: type, modname: str | None = None) -> nodes.ClassDef:
+        """Get astroid for the given class."""
         if modname is None:
             try:
                 modname = klass.__module__
             except AttributeError as exc:
                 raise AstroidBuildingError(
                     "Unable to get module for class {class_name}.",
                     cls=klass,
                     class_repr=safe_repr(klass),
                     modname=modname,
                 ) from exc
         modastroid = self.ast_from_module_name(modname)
-        return modastroid.getattr(klass.__name__)[0]  # XXX
-
-    def infer_ast_from_something(self, obj, context=None):
-        """infer astroid for the given class"""
+        ret = modastroid.getattr(klass.__name__)[0]
+        assert isinstance(ret, nodes.ClassDef)
+        return ret
+
+    def infer_ast_from_something(
+        self, obj: object, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
+        """Infer astroid for the given class."""
         if hasattr(obj, "__class__") and not isinstance(obj, type):
             klass = obj.__class__
-        else:
+        elif isinstance(obj, type):
             klass = obj
+        else:
+            raise AstroidBuildingError(  # pragma: no cover
+                "Unable to get type for {class_repr}.",
+                cls=None,
+                class_repr=safe_repr(obj),
+            )
         try:
             modname = klass.__module__
         except AttributeError as exc:
             raise AstroidBuildingError(
                 "Unable to get module for {class_repr}.",
                 cls=klass,
                 class_repr=safe_repr(klass),
@@ -328,48 +372,81 @@
             raise AstroidBuildingError(
                 "Unable to get name for {class_repr}:\n",
                 cls=klass,
                 class_repr=safe_repr(klass),
             ) from exc
         except Exception as exc:
             raise AstroidImportError(
-                "Unexpected error while retrieving name for {class_repr}:\n" "{error}",
+                "Unexpected error while retrieving name for {class_repr}:\n{error}",
                 cls=klass,
                 class_repr=safe_repr(klass),
             ) from exc
         # take care, on living object __module__ is regularly wrong :(
         modastroid = self.ast_from_module_name(modname)
         if klass is obj:
             for inferred in modastroid.igetattr(name, context):
                 yield inferred
         else:
             for inferred in modastroid.igetattr(name, context):
                 yield inferred.instantiate_class()
 
-    def register_failed_import_hook(self, hook):
+    def register_failed_import_hook(self, hook: Callable[[str], nodes.Module]) -> None:
         """Registers a hook to resolve imports that cannot be found otherwise.
 
         `hook` must be a function that accepts a single argument `modname` which
         contains the name of the module or package that could not be imported.
         If `hook` can resolve the import, must return a node of type `astroid.Module`,
         otherwise, it must raise `AstroidBuildingError`.
         """
         self._failed_import_hooks.append(hook)
 
-    def cache_module(self, module):
+    def cache_module(self, module: nodes.Module) -> None:
         """Cache a module if no module with the same name is known yet."""
         self.astroid_cache.setdefault(module.name, module)
 
-    def bootstrap(self):
-        """Bootstrap the required AST modules needed for the manager to work
+    def bootstrap(self) -> None:
+        """Bootstrap the required AST modules needed for the manager to work.
 
         The bootstrap usually involves building the AST for the builtins
         module, which is required by the rest of astroid to work correctly.
         """
         from astroid import raw_building  # pylint: disable=import-outside-toplevel
 
         raw_building._astroid_bootstrapping()
 
-    def clear_cache(self):
-        """Clear the underlying cache. Also bootstraps the builtins module."""
+    def clear_cache(self) -> None:
+        """Clear the underlying caches, bootstrap the builtins module and
+        re-register transforms.
+        """
+        # import here because of cyclic imports
+        # pylint: disable=import-outside-toplevel
+        from astroid.inference_tip import clear_inference_tip_cache
+        from astroid.interpreter.objectmodel import ObjectModel
+        from astroid.nodes.node_classes import LookupMixIn
+        from astroid.nodes.scoped_nodes import ClassDef
+
+        clear_inference_tip_cache()
+        _invalidate_cache()  # inference context cache
+
         self.astroid_cache.clear()
+        # NB: not a new TransformVisitor()
+        AstroidManager.brain["_transform"].transforms = collections.defaultdict(list)
+
+        for lru_cache in (
+            LookupMixIn.lookup,
+            _cache_normalize_path_,
+            util.is_namespace,
+            ObjectModel.attributes,
+            ClassDef._metaclass_lookup_attribute,
+        ):
+            lru_cache.cache_clear()  # type: ignore[attr-defined]
+
         self.bootstrap()
+
+        # Reload brain plugins. During initialisation this is done in astroid.__init__.py
+        for module in BRAIN_MODULES_DIRECTORY.iterdir():
+            if module.suffix == ".py":
+                module_spec = find_spec(f"astroid.brain.{module.stem}")
+                assert module_spec
+                module_object = module_from_spec(module_spec)
+                assert module_spec.loader
+                module_spec.loader.exec_module(module_object)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/modutils.py` & `astroid-3.0.0a1/astroid/modutils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,63 @@
-# Copyright (c) 2014-2018, 2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 Google, Inc.
-# Copyright (c) 2014 Denis Laxalde <denis.laxalde@logilab.fr>
-# Copyright (c) 2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015 Florian Bruhin <me@the-compiler.org>
-# Copyright (c) 2015 Radosław Ganczarek <radoslaw@ganczarek.in>
-# Copyright (c) 2016 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Mario Corchero <mcorcherojim@bloomberg.net>
-# Copyright (c) 2018 Mario Corchero <mariocj89@gmail.com>
-# Copyright (c) 2018 Anthony Sottile <asottile@umich.edu>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2019 markmcclain <markmcclain@users.noreply.github.com>
-# Copyright (c) 2019 BasPH <BasPH@users.noreply.github.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Peter Kolbus <peter.kolbus@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Keichi Takahashi <hello@keichi.dev>
-# Copyright (c) 2021 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 DudeNr33 <3929834+DudeNr33@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Python modules manipulation utility functions.
 
 :type PY_SOURCE_EXTS: tuple(str)
 :var PY_SOURCE_EXTS: list of possible python source file extension
 
 :type STD_LIB_DIRS: set of str
 :var STD_LIB_DIRS: directories where standard modules are located
 
 :type BUILTIN_MODULES: dict
 :var BUILTIN_MODULES: dictionary with builtin module names has key
 """
 
-# We disable the import-error so pylint can work without distutils installed.
-# pylint: disable=no-name-in-module,useless-suppression
+from __future__ import annotations
 
 import importlib
 import importlib.machinery
 import importlib.util
+import io
 import itertools
+import logging
 import os
-import platform
 import sys
+import sysconfig
 import types
-from distutils.errors import DistutilsPlatformError  # pylint: disable=import-error
-from distutils.sysconfig import get_python_lib  # pylint: disable=import-error
-from typing import Dict, Set
+import warnings
+from collections.abc import Callable, Iterable, Sequence
+from contextlib import redirect_stderr, redirect_stdout
+from functools import lru_cache
+from pathlib import Path
 
+from astroid.const import IS_JYTHON, IS_PYPY, PY310_PLUS
 from astroid.interpreter._import import spec, util
 
-# distutils is replaced by virtualenv with a module that does
-# weird path manipulations in order to get to the
-# real distutils module.
+if PY310_PLUS:
+    from sys import stdlib_module_names
+else:
+    from astroid._backport_stdlib_names import stdlib_module_names
+
+logger = logging.getLogger(__name__)
 
 
 if sys.platform.startswith("win"):
     PY_SOURCE_EXTS = ("py", "pyw")
     PY_COMPILED_EXTS = ("dll", "pyd")
 else:
     PY_SOURCE_EXTS = ("py",)
     PY_COMPILED_EXTS = ("so",)
 
 
-try:
-    # The explicit sys.prefix is to work around a patch in virtualenv that
-    # replaces the 'real' sys.prefix (i.e. the location of the binary)
-    # with the prefix from which the virtualenv was created. This throws
-    # off the detection logic for standard library modules, thus the
-    # workaround.
-    STD_LIB_DIRS = {
-        get_python_lib(standard_lib=True, prefix=sys.prefix),
-        # Take care of installations where exec_prefix != prefix.
-        get_python_lib(standard_lib=True, prefix=sys.exec_prefix),
-        get_python_lib(standard_lib=True),
-    }
-# get_python_lib(standard_lib=1) is not available on pypy, set STD_LIB_DIR to
-# non-valid path, see https://bugs.pypy.org/issue1164
-except DistutilsPlatformError:
-    STD_LIB_DIRS = set()
+# TODO: Adding `platstdlib` is a fix for a workaround in virtualenv. At some point we should
+# revisit whether this is still necessary. See https://github.com/pylint-dev/astroid/pull/1323.
+STD_LIB_DIRS = {sysconfig.get_path("stdlib"), sysconfig.get_path("platstdlib")}
 
 if os.name == "nt":
     STD_LIB_DIRS.add(os.path.join(sys.prefix, "dlls"))
     try:
         # real_prefix is defined when running inside virtual environments,
         # created with the **virtualenv** library.
         # Deprecated in virtualenv==16.7.9
@@ -99,118 +68,110 @@
         # created with the stdlib **venv** module, it points to the original
         # installation, if the virtual env is activated.
         try:
             STD_LIB_DIRS.add(os.path.join(sys.base_exec_prefix, "dlls"))
         except AttributeError:
             pass
 
-if platform.python_implementation() == "PyPy":
-    # The get_python_lib(standard_lib=True) function does not give valid
-    # result with pypy in a virtualenv.
-    # In a virtual environment, with CPython implementation the call to this function returns a path toward
-    # the binary (its libraries) which has been used to create the virtual environment.
-    # Not with pypy implementation.
-    # The only way to retrieve such information is to use the sys.base_prefix hint.
-    # It's worth noticing that under CPython implementation the return values of
-    # get_python_lib(standard_lib=True) and get_python_lib(santdard_lib=True, prefix=sys.base_prefix)
-    # are the same.
-    # In the lines above, we could have replace the call to get_python_lib(standard=True)
-    # with the one using prefix=sys.base_prefix but we prefer modifying only what deals with pypy.
-    STD_LIB_DIRS.add(get_python_lib(standard_lib=True, prefix=sys.base_prefix))
-    _root = os.path.join(sys.prefix, "lib_pypy")
-    STD_LIB_DIRS.add(_root)
-    try:
-        # real_prefix is defined when running inside virtualenv.
-        STD_LIB_DIRS.add(os.path.join(sys.base_prefix, "lib_pypy"))
-    except AttributeError:
-        pass
-    del _root
+if IS_PYPY and sys.version_info < (3, 8):
+    # PyPy stores the stdlib in two places: sys.prefix/lib_pypy and sys.prefix/lib-python/3
+    # sysconfig.get_path on PyPy returns the first, but without an underscore so we patch this manually.
+    # Beginning with 3.8 the stdlib is only stored in: sys.prefix/pypy{py_version_short}
+    STD_LIB_DIRS.add(str(Path(sysconfig.get_path("stdlib")).parent / "lib_pypy"))
+    STD_LIB_DIRS.add(str(Path(sysconfig.get_path("stdlib")).parent / "lib-python/3"))
+
+    # TODO: This is a fix for a workaround in virtualenv. At some point we should revisit
+    # whether this is still necessary. See https://github.com/pylint-dev/astroid/pull/1324.
+    STD_LIB_DIRS.add(str(Path(sysconfig.get_path("platstdlib")).parent / "lib_pypy"))
+    STD_LIB_DIRS.add(
+        str(Path(sysconfig.get_path("platstdlib")).parent / "lib-python/3")
+    )
+
 if os.name == "posix":
     # Need the real prefix if we're in a virtualenv, otherwise
     # the usual one will do.
     # Deprecated in virtualenv==16.7.9
     # See: https://github.com/pypa/virtualenv/issues/1622
     try:
-        prefix = sys.real_prefix  # type: ignore[attr-defined]
+        prefix: str = sys.real_prefix  # type: ignore[attr-defined]
     except AttributeError:
         prefix = sys.prefix
 
-    def _posix_path(path):
+    def _posix_path(path: str) -> str:
         base_python = "python%d.%d" % sys.version_info[:2]
         return os.path.join(prefix, path, base_python)
 
     STD_LIB_DIRS.add(_posix_path("lib"))
-    if sys.maxsize > 2 ** 32:
+    if sys.maxsize > 2**32:
         # This tries to fix a problem with /usr/lib64 builds,
         # where systems are running both 32-bit and 64-bit code
         # on the same machine, which reflects into the places where
         # standard library could be found. More details can be found
         # here http://bugs.python.org/issue1294959.
         # An easy reproducing case would be
-        # https://github.com/PyCQA/pylint/issues/712#issuecomment-163178753
+        # https://github.com/pylint-dev/pylint/issues/712#issuecomment-163178753
         STD_LIB_DIRS.add(_posix_path("lib64"))
 
-EXT_LIB_DIRS = {get_python_lib(), get_python_lib(True)}
-IS_JYTHON = platform.python_implementation() == "Jython"
+EXT_LIB_DIRS = {sysconfig.get_path("purelib"), sysconfig.get_path("platlib")}
 BUILTIN_MODULES = dict.fromkeys(sys.builtin_module_names, True)
 
 
 class NoSourceFile(Exception):
-    """exception raised when we are not able to get a python
-    source file for a precompiled file
+    """Exception raised when we are not able to get a python
+    source file for a precompiled file.
     """
 
 
 def _normalize_path(path: str) -> str:
     """Resolve symlinks in path and convert to absolute path.
 
     Note that environment variables and ~ in the path need to be expanded in
     advance.
 
     This can be cached by using _cache_normalize_path.
     """
     return os.path.normcase(os.path.realpath(path))
 
 
-def _path_from_filename(filename, is_jython=IS_JYTHON):
+def _path_from_filename(filename: str, is_jython: bool = IS_JYTHON) -> str:
     if not is_jython:
         return filename
     head, has_pyclass, _ = filename.partition("$py.class")
     if has_pyclass:
         return head + ".py"
     return filename
 
 
-def _handle_blacklist(blacklist, dirnames, filenames):
-    """remove files/directories in the black list
+def _handle_blacklist(
+    blacklist: Sequence[str], dirnames: list[str], filenames: list[str]
+) -> None:
+    """Remove files/directories in the black list.
 
     dirnames/filenames are usually from os.walk
     """
     for norecurs in blacklist:
         if norecurs in dirnames:
             dirnames.remove(norecurs)
         elif norecurs in filenames:
             filenames.remove(norecurs)
 
 
-_NORM_PATH_CACHE: Dict[str, str] = {}
+@lru_cache
+def _cache_normalize_path_(path: str) -> str:
+    return _normalize_path(path)
 
 
 def _cache_normalize_path(path: str) -> str:
     """Normalize path with caching."""
     # _module_file calls abspath on every path in sys.path every time it's
     # called; on a larger codebase this easily adds up to half a second just
     # assembling path components. This cache alleviates that.
-    try:
-        return _NORM_PATH_CACHE[path]
-    except KeyError:
-        if not path:  # don't cache result for ''
-            return _normalize_path(path)
-        result = _NORM_PATH_CACHE[path] = _normalize_path(path)
-        return result
+    if not path:  # don't cache result for ''
+        return _normalize_path(path)
+    return _cache_normalize_path_(path)
 
 
 def load_module_from_name(dotted_name: str) -> types.ModuleType:
     """Load a Python module from its name.
 
     :type dotted_name: str
     :param dotted_name: python name of a module or package
@@ -221,62 +182,78 @@
     :return: the loaded module
     """
     try:
         return sys.modules[dotted_name]
     except KeyError:
         pass
 
-    return importlib.import_module(dotted_name)
+    # Capture and log anything emitted during import to avoid
+    # contaminating JSON reports in pylint
+    with redirect_stderr(io.StringIO()) as stderr, redirect_stdout(
+        io.StringIO()
+    ) as stdout:
+        module = importlib.import_module(dotted_name)
+
+    stderr_value = stderr.getvalue()
+    if stderr_value:
+        logger.error(
+            "Captured stderr while importing %s:\n%s", dotted_name, stderr_value
+        )
+    stdout_value = stdout.getvalue()
+    if stdout_value:
+        logger.info(
+            "Captured stdout while importing %s:\n%s", dotted_name, stdout_value
+        )
+
+    return module
 
 
-def load_module_from_modpath(parts):
+def load_module_from_modpath(parts: Sequence[str]) -> types.ModuleType:
     """Load a python module from its split name.
 
-    :type parts: list(str) or tuple(str)
     :param parts:
       python name of a module or package split on '.'
 
     :raise ImportError: if the module or package is not found
 
-    :rtype: module
     :return: the loaded module
     """
     return load_module_from_name(".".join(parts))
 
 
-def load_module_from_file(filepath: str):
+def load_module_from_file(filepath: str) -> types.ModuleType:
     """Load a Python module from it's path.
 
     :type filepath: str
     :param filepath: path to the python module or package
 
     :raise ImportError: if the module or package is not found
 
     :rtype: module
     :return: the loaded module
     """
     modpath = modpath_from_file(filepath)
     return load_module_from_modpath(modpath)
 
 
-def check_modpath_has_init(path, mod_path):
-    """check there are some __init__.py all along the way"""
-    modpath = []
+def check_modpath_has_init(path: str, mod_path: list[str]) -> bool:
+    """Check there are some __init__.py all along the way."""
+    modpath: list[str] = []
     for part in mod_path:
         modpath.append(part)
         path = os.path.join(path, part)
         if not _has_init(path):
             old_namespace = util.is_namespace(".".join(modpath))
             if not old_namespace:
                 return False
     return True
 
 
-def _get_relative_base_path(filename, path_to_check):
-    """Extracts the relative mod path of the file to import from
+def _get_relative_base_path(filename: str, path_to_check: str) -> list[str] | None:
+    """Extracts the relative mod path of the file to import from.
 
     Check if a file is within the passed in path and if so, returns the
     relative mod path from the one passed in.
 
     If the filename is no in path_to_check, returns None
 
     Note this function will look for both abs and realpath of the file,
@@ -304,37 +281,42 @@
         base_path = os.path.splitext(importable_path)[0]
         relative_base_path = base_path[len(path_to_check) :]
         return [pkg for pkg in relative_base_path.split(os.sep) if pkg]
 
     return None
 
 
-def modpath_from_file_with_callback(filename, path=None, is_package_cb=None):
+def modpath_from_file_with_callback(
+    filename: str,
+    path: Sequence[str] | None = None,
+    is_package_cb: Callable[[str, list[str]], bool] | None = None,
+) -> list[str]:
     filename = os.path.expanduser(_path_from_filename(filename))
     paths_to_check = sys.path.copy()
     if path:
         paths_to_check += path
     for pathname in itertools.chain(
         paths_to_check, map(_cache_normalize_path, paths_to_check)
     ):
         if not pathname:
             continue
         modpath = _get_relative_base_path(filename, pathname)
         if not modpath:
             continue
+        assert is_package_cb is not None
         if is_package_cb(pathname, modpath[:-1]):
             return modpath
 
     raise ImportError(
         "Unable to find module for {} in {}".format(filename, ", \n".join(sys.path))
     )
 
 
-def modpath_from_file(filename, path=None):
-    """Get the corresponding split module's name from a filename
+def modpath_from_file(filename: str, path: Sequence[str] | None = None) -> list[str]:
+    """Get the corresponding split module's name from a filename.
 
     This function will return the name of a module or package split on `.`.
 
     :type filename: str
     :param filename: file's path for which we want the module's name
 
     :type Optional[List[str]] path:
@@ -346,87 +328,88 @@
 
     :rtype: list(str)
     :return: the corresponding split module's name
     """
     return modpath_from_file_with_callback(filename, path, check_modpath_has_init)
 
 
-def file_from_modpath(modpath, path=None, context_file=None):
+def file_from_modpath(
+    modpath: list[str],
+    path: Sequence[str] | None = None,
+    context_file: str | None = None,
+) -> str | None:
     return file_info_from_modpath(modpath, path, context_file).location
 
 
-def file_info_from_modpath(modpath, path=None, context_file=None):
-    """given a mod path (i.e. split module / package name), return the
-    corresponding file, giving priority to source file over precompiled
-    file if it exists
+def file_info_from_modpath(
+    modpath: list[str],
+    path: Sequence[str] | None = None,
+    context_file: str | None = None,
+) -> spec.ModuleSpec:
+    """Given a mod path (i.e. split module / package name), return the
+    corresponding file.
+
+    Giving priority to source file over precompiled file if it exists.
 
-    :type modpath: list or tuple
     :param modpath:
       split module's name (i.e name of a module or package split
       on '.')
       (this means explicit relative imports that start with dots have
       empty strings in this list!)
 
-    :type path: list or None
     :param path:
       optional list of path where the module or package should be
       searched (use sys.path if nothing or None is given)
 
-    :type context_file: str or None
     :param context_file:
       context file to consider, necessary if the identifier has been
       introduced using a relative import unresolvable in the actual
       context (i.e. modutils)
 
     :raise ImportError: if there is no such module in the directory
 
-    :rtype: (str or None, import type)
     :return:
       the path to the module's file or None if it's an integrated
       builtin module such as 'sys'
     """
     if context_file is not None:
-        context = os.path.dirname(context_file)
+        context: str | None = os.path.dirname(context_file)
     else:
         context = context_file
     if modpath[0] == "xml":
         # handle _xmlplus
         try:
             return _spec_from_modpath(["_xmlplus"] + modpath[1:], path, context)
         except ImportError:
             return _spec_from_modpath(modpath, path, context)
     elif modpath == ["os", "path"]:
         # FIXME: currently ignoring search_path...
         return spec.ModuleSpec(
             name="os.path",
             location=os.path.__file__,
-            module_type=spec.ModuleType.PY_SOURCE,
+            type=spec.ModuleType.PY_SOURCE,
         )
     return _spec_from_modpath(modpath, path, context)
 
 
-def get_module_part(dotted_name, context_file=None):
-    """given a dotted name return the module part of the name :
+def get_module_part(dotted_name: str, context_file: str | None = None) -> str:
+    """Given a dotted name return the module part of the name :
 
     >>> get_module_part('astroid.as_string.dump')
     'astroid.as_string'
 
-    :type dotted_name: str
     :param dotted_name: full name of the identifier we are interested in
 
-    :type context_file: str or None
     :param context_file:
       context file to consider, necessary if the identifier has been
       introduced using a relative import unresolvable in the actual
       context (i.e. modutils)
 
-
     :raise ImportError: if there is no such module in the directory
 
-    :rtype: str or None
     :return:
       the module part of the name or None if we have not been able at
       all to import the given name
 
     XXX: deprecated, since it doesn't handle package precedence over module
     (see #10066)
     """
@@ -438,59 +421,60 @@
         # first check for builtin module which won't be considered latter
         # in that case (path != None)
         if parts[0] in BUILTIN_MODULES:
             if len(parts) > 2:
                 raise ImportError(dotted_name)
             return parts[0]
         # don't use += or insert, we want a new list to be created !
-    path = None
+    path: list[str] | None = None
     starti = 0
     if parts[0] == "":
         assert (
             context_file is not None
         ), "explicit relative import, but no context_file?"
         path = []  # prevent resolving the import non-relatively
         starti = 1
     while parts[starti] == "":  # for all further dots: change context
         starti += 1
+        assert (
+            context_file is not None
+        ), "explicit relative import, but no context_file?"
         context_file = os.path.dirname(context_file)
     for i in range(starti, len(parts)):
         try:
             file_from_modpath(
                 parts[starti : i + 1], path=path, context_file=context_file
             )
         except ImportError:
             if i < max(1, len(parts) - 2):
                 raise
             return ".".join(parts[:i])
     return dotted_name
 
 
-def get_module_files(src_directory, blacklist, list_all=False):
-    """given a package directory return a list of all available python
-    module's files in the package and its subpackages
+def get_module_files(
+    src_directory: str, blacklist: Sequence[str], list_all: bool = False
+) -> list[str]:
+    """Given a package directory return a list of all available python
+    module's files in the package and its subpackages.
 
-    :type src_directory: str
     :param src_directory:
       path of the directory corresponding to the package
 
-    :type blacklist: list or tuple
     :param blacklist: iterable
       list of files or directories to ignore.
 
-    :type list_all: bool
     :param list_all:
         get files from all paths, including ones without __init__.py
 
-    :rtype: list
     :return:
       the list of all available python module's files in the package and
       its subpackages
     """
-    files = []
+    files: list[str] = []
     for directory, dirnames, filenames in os.walk(src_directory):
         if directory in blacklist:
             continue
         _handle_blacklist(blacklist, dirnames, filenames)
         # check for __init__.py
         if not list_all and "__init__.py" not in filenames:
             dirnames[:] = ()
@@ -498,64 +482,97 @@
         for filename in filenames:
             if _is_python_file(filename):
                 src = os.path.join(directory, filename)
                 files.append(src)
     return files
 
 
-def get_source_file(filename, include_no_ext=False):
-    """given a python module's file name return the matching source file
+def get_source_file(filename: str, include_no_ext: bool = False) -> str:
+    """Given a python module's file name return the matching source file
     name (the filename will be returned identically if it's already an
-    absolute path to a python source file...)
+    absolute path to a python source file).
 
-    :type filename: str
     :param filename: python module's file name
 
-
     :raise NoSourceFile: if no source file exists on the file system
 
-    :rtype: str
     :return: the absolute path of the source file if it exists
     """
     filename = os.path.abspath(_path_from_filename(filename))
     base, orig_ext = os.path.splitext(filename)
     for ext in PY_SOURCE_EXTS:
         source_path = f"{base}.{ext}"
         if os.path.exists(source_path):
             return source_path
     if include_no_ext and not orig_ext and os.path.exists(base):
         return base
     raise NoSourceFile(filename)
 
 
-def is_python_source(filename):
-    """
-    rtype: bool
-    return: True if the filename is a python source file
-    """
+def is_python_source(filename: str | None) -> bool:
+    """Return: True if the filename is a python source file."""
+    if not filename:
+        return False
     return os.path.splitext(filename)[1][1:] in PY_SOURCE_EXTS
 
 
-def is_standard_module(modname, std_path=None):
-    """try to guess if a module is a standard python module (by default,
-    see `std_path` parameter's description)
+def is_stdlib_module(modname: str) -> bool:
+    """Return: True if the modname is in the standard library"""
+    return modname.split(".")[0] in stdlib_module_names
+
+
+def module_in_path(modname: str, path: str | Iterable[str]) -> bool:
+    """Try to determine if a module is imported from one of the specified paths
+
+    :param modname: name of the module
+
+    :param path: paths to consider
+
+    :return:
+      true if the module:
+      - is located on the path listed in one of the directory in `paths`
+    """
+
+    modname = modname.split(".")[0]
+    try:
+        filename = file_from_modpath([modname])
+    except ImportError:
+        # Import failed, we can't check path if we don't know it
+        return False
+
+    if filename is None:
+        # No filename likely means it's compiled in, or potentially a namespace
+        return False
+    filename = _normalize_path(filename)
+
+    if isinstance(path, str):
+        return filename.startswith(_cache_normalize_path(path))
+
+    return any(filename.startswith(_cache_normalize_path(entry)) for entry in path)
+
+
+def is_standard_module(modname: str, std_path: Iterable[str] | None = None) -> bool:
+    """Try to guess if a module is a standard python module (by default,
+    see `std_path` parameter's description).
 
-    :type modname: str
     :param modname: name of the module we are interested in
 
-    :type std_path: list(str) or tuple(str)
     :param std_path: list of path considered has standard
 
-
-    :rtype: bool
     :return:
       true if the module:
       - is located on the path listed in one of the directory in `std_path`
       - is a built-in module
     """
+    warnings.warn(
+        "is_standard_module() is deprecated. Use, is_stdlib_module() or module_in_path() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
     modname = modname.split(".")[0]
     try:
         filename = file_from_modpath([modname])
     except ImportError:
         # import failed, i'm probably not so wrong by supposing it's
         # not standard...
         return False
@@ -570,26 +587,23 @@
             return False
     if std_path is None:
         std_path = STD_LIB_DIRS
 
     return any(filename.startswith(_cache_normalize_path(path)) for path in std_path)
 
 
-def is_relative(modname, from_file):
-    """return true if the given module name is relative to the given
-    file name
+def is_relative(modname: str, from_file: str) -> bool:
+    """Return true if the given module name is relative to the given
+    file name.
 
-    :type modname: str
     :param modname: name of the module we are interested in
 
-    :type from_file: str
     :param from_file:
       path of the module from which modname has been imported
 
-    :rtype: bool
     :return:
       true if the module has been imported relatively to `from_file`
     """
     if not os.path.isdir(from_file):
         from_file = os.path.dirname(from_file)
     if from_file in sys.path:
         return False
@@ -599,17 +613,21 @@
         )
     )
 
 
 # internal only functions #####################################################
 
 
-def _spec_from_modpath(modpath, path=None, context=None):
-    """given a mod path (i.e. split module / package name), return the
-    corresponding spec
+def _spec_from_modpath(
+    modpath: list[str],
+    path: Sequence[str] | None = None,
+    context: str | None = None,
+) -> spec.ModuleSpec:
+    """Given a mod path (i.e. split module / package name), return the
+    corresponding spec.
 
     this function is used internally, see `file_from_modpath`'s
     documentation for more information
     """
     assert modpath
     location = None
     if context is not None:
@@ -619,61 +637,63 @@
         except ImportError:
             found_spec = spec.find_spec(modpath, path)
             location = found_spec.location
     else:
         found_spec = spec.find_spec(modpath, path)
     if found_spec.type == spec.ModuleType.PY_COMPILED:
         try:
+            assert found_spec.location is not None
             location = get_source_file(found_spec.location)
             return found_spec._replace(
                 location=location, type=spec.ModuleType.PY_SOURCE
             )
         except NoSourceFile:
             return found_spec._replace(location=location)
     elif found_spec.type == spec.ModuleType.C_BUILTIN:
         # integrated builtin module
         return found_spec._replace(location=None)
     elif found_spec.type == spec.ModuleType.PKG_DIRECTORY:
+        assert found_spec.location is not None
         location = _has_init(found_spec.location)
         return found_spec._replace(location=location, type=spec.ModuleType.PY_SOURCE)
     return found_spec
 
 
-def _is_python_file(filename):
-    """return true if the given filename should be considered as a python file
+def _is_python_file(filename: str) -> bool:
+    """Return true if the given filename should be considered as a python file.
 
     .pyc and .pyo are ignored
     """
     return filename.endswith((".py", ".so", ".pyd", ".pyw"))
 
 
-def _has_init(directory):
-    """if the given directory has a valid __init__ file, return its path,
-    else return None
+def _has_init(directory: str) -> str | None:
+    """If the given directory has a valid __init__ file, return its path,
+    else return None.
     """
     mod_or_pack = os.path.join(directory, "__init__")
-    for ext in PY_SOURCE_EXTS + ("pyc", "pyo"):
+    for ext in (*PY_SOURCE_EXTS, "pyc", "pyo"):
         if os.path.exists(mod_or_pack + "." + ext):
             return mod_or_pack + "." + ext
     return None
 
 
-def is_namespace(specobj):
+def is_namespace(specobj: spec.ModuleSpec) -> bool:
     return specobj.type == spec.ModuleType.PY_NAMESPACE
 
 
-def is_directory(specobj):
+def is_directory(specobj: spec.ModuleSpec) -> bool:
     return specobj.type == spec.ModuleType.PKG_DIRECTORY
 
 
 def is_module_name_part_of_extension_package_whitelist(
-    module_name: str, package_whitelist: Set[str]
+    module_name: str, package_whitelist: set[str]
 ) -> bool:
     """
-    Returns True if one part of the module name is in the package whitelist
+    Returns True if one part of the module name is in the package whitelist.
 
     >>> is_module_name_part_of_extension_package_whitelist('numpy.core.umath', {'numpy'})
     True
     """
     parts = module_name.split(".")
     return any(
         ".".join(parts[:x]) in package_whitelist for x in range(1, len(parts) + 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/node_classes.py` & `astroid-3.0.0a1/astroid/node_classes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 # pylint: disable=unused-import
 
 import warnings
 
 from astroid.nodes.node_classes import (  # pylint: disable=redefined-builtin (Ellipsis)
     CONST_CLS,
     AnnAssign,
@@ -68,14 +72,15 @@
     Return,
     Set,
     Slice,
     Starred,
     Subscript,
     TryExcept,
     TryFinally,
+    TryStar,
     Tuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
@@ -84,10 +89,12 @@
     unpack_infer,
 )
 
 # We cannot create a __all__ here because it would create a circular import
 # Please remove astroid/scoped_nodes.py|astroid/node_classes.py in autoflake
 # exclude when removing this file.
 warnings.warn(
-    "The 'astroid.node_classes' module is deprecated and will be replaced by 'astroid.nodes' in astroid 3.0.0",
+    "The 'astroid.node_classes' module is deprecated and will be replaced by "
+    "'astroid.nodes' in astroid 3.0.0",
     DeprecationWarning,
+    stacklevel=2,
 )
```

### Comparing `astroid-2.9.3/astroid/nodes/as_string.py` & `astroid-3.0.0a1/astroid/nodes/as_string.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-# Copyright (c) 2009-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2010 Daniel Harding <dharding@gmail.com>
-# Copyright (c) 2013-2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016 Jared Garst <jgarst@users.noreply.github.com>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2017, 2019 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 rr- <rr-@sakuya.pl>
-# Copyright (c) 2018 Serhiy Storchaka <storchaka@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 brendanator <brendan.maginnis@gmail.com>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2019 Alex Hall <alex.mojaki@gmail.com>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 pre-commit-ci[bot] <bot@noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """This module renders Astroid nodes as string"""
-from typing import TYPE_CHECKING, List
+
+from __future__ import annotations
+
+from collections.abc import Iterator
+from typing import TYPE_CHECKING
+
+from astroid import nodes
 
 if TYPE_CHECKING:
+    from astroid.nodes import Const
     from astroid.nodes.node_classes import (
         Match,
         MatchAs,
         MatchCase,
         MatchClass,
         MatchMapping,
         MatchOr,
@@ -45,41 +33,48 @@
 
 
 # Visitor pattern require argument all the time and is not better with staticmethod
 # noinspection PyUnusedLocal,PyMethodMayBeStatic
 class AsStringVisitor:
     """Visitor to render an Astroid node as a valid python code string"""
 
-    def __init__(self, indent="    "):
-        self.indent = indent
+    def __init__(self, indent: str = "    "):
+        self.indent: str = indent
 
-    def __call__(self, node):
+    def __call__(self, node) -> str:
         """Makes this visitor behave as a simple function"""
         return node.accept(self).replace(DOC_NEWLINE, "\n")
 
-    def _docs_dedent(self, doc):
+    def _docs_dedent(self, doc_node: Const | None) -> str:
         """Stop newlines in docs being indented by self._stmt_list"""
-        return '\n{}"""{}"""'.format(self.indent, doc.replace("\n", DOC_NEWLINE))
+        if not doc_node:
+            return ""
 
-    def _stmt_list(self, stmts, indent=True):
+        return '\n{}"""{}"""'.format(
+            self.indent, doc_node.value.replace("\n", DOC_NEWLINE)
+        )
+
+    def _stmt_list(self, stmts: list, indent: bool = True) -> str:
         """return a list of nodes to string"""
-        stmts = "\n".join(nstr for nstr in [n.accept(self) for n in stmts] if nstr)
-        if indent:
-            return self.indent + stmts.replace("\n", "\n" + self.indent)
+        stmts_str: str = "\n".join(
+            nstr for nstr in [n.accept(self) for n in stmts] if nstr
+        )
+        if not indent:
+            return stmts_str
 
-        return stmts
+        return self.indent + stmts_str.replace("\n", "\n" + self.indent)
 
-    def _precedence_parens(self, node, child, is_left=True):
+    def _precedence_parens(self, node, child, is_left: bool = True) -> str:
         """Wrap child in parens only if required to keep same semantics"""
         if self._should_wrap(node, child, is_left):
             return f"({child.accept(self)})"
 
         return child.accept(self)
 
-    def _should_wrap(self, node, child, is_left):
+    def _should_wrap(self, node, child, is_left: bool) -> bool:
         """Wrap child if:
         - it has lower precedence
         - same precedence with position opposite to associativity direction
         """
         node_precedence = node.op_precedence()
         child_precedence = child.op_precedence()
 
@@ -95,205 +90,208 @@
             # (2**3)**4
             return True
 
         return False
 
     # visit_<node> methods ###########################################
 
-    def visit_await(self, node):
+    def visit_await(self, node) -> str:
         return f"await {node.value.accept(self)}"
 
-    def visit_asyncwith(self, node):
+    def visit_asyncwith(self, node) -> str:
         return f"async {self.visit_with(node)}"
 
-    def visit_asyncfor(self, node):
+    def visit_asyncfor(self, node) -> str:
         return f"async {self.visit_for(node)}"
 
-    def visit_arguments(self, node):
+    def visit_arguments(self, node) -> str:
         """return an astroid.Function node as string"""
         return node.format_args()
 
-    def visit_assignattr(self, node):
+    def visit_assignattr(self, node) -> str:
         """return an astroid.AssAttr node as string"""
         return self.visit_attribute(node)
 
-    def visit_assert(self, node):
+    def visit_assert(self, node) -> str:
         """return an astroid.Assert node as string"""
         if node.fail:
             return f"assert {node.test.accept(self)}, {node.fail.accept(self)}"
         return f"assert {node.test.accept(self)}"
 
-    def visit_assignname(self, node):
+    def visit_assignname(self, node) -> str:
         """return an astroid.AssName node as string"""
         return node.name
 
-    def visit_assign(self, node):
+    def visit_assign(self, node) -> str:
         """return an astroid.Assign node as string"""
         lhs = " = ".join(n.accept(self) for n in node.targets)
         return f"{lhs} = {node.value.accept(self)}"
 
-    def visit_augassign(self, node):
+    def visit_augassign(self, node) -> str:
         """return an astroid.AugAssign node as string"""
         return f"{node.target.accept(self)} {node.op} {node.value.accept(self)}"
 
-    def visit_annassign(self, node):
+    def visit_annassign(self, node) -> str:
         """Return an astroid.AugAssign node as string"""
 
         target = node.target.accept(self)
         annotation = node.annotation.accept(self)
         if node.value is None:
             return f"{target}: {annotation}"
         return f"{target}: {annotation} = {node.value.accept(self)}"
 
-    def visit_binop(self, node):
+    def visit_binop(self, node) -> str:
         """return an astroid.BinOp node as string"""
         left = self._precedence_parens(node, node.left)
         right = self._precedence_parens(node, node.right, is_left=False)
         if node.op == "**":
             return f"{left}{node.op}{right}"
 
         return f"{left} {node.op} {right}"
 
-    def visit_boolop(self, node):
+    def visit_boolop(self, node) -> str:
         """return an astroid.BoolOp node as string"""
         values = [f"{self._precedence_parens(node, n)}" for n in node.values]
         return (f" {node.op} ").join(values)
 
-    def visit_break(self, node):
+    def visit_break(self, node) -> str:
         """return an astroid.Break node as string"""
         return "break"
 
-    def visit_call(self, node):
+    def visit_call(self, node) -> str:
         """return an astroid.Call node as string"""
         expr_str = self._precedence_parens(node, node.func)
         args = [arg.accept(self) for arg in node.args]
         if node.keywords:
             keywords = [kwarg.accept(self) for kwarg in node.keywords]
         else:
             keywords = []
 
         args.extend(keywords)
         return f"{expr_str}({', '.join(args)})"
 
-    def visit_classdef(self, node):
+    def visit_classdef(self, node) -> str:
         """return an astroid.ClassDef node as string"""
         decorate = node.decorators.accept(self) if node.decorators else ""
         args = [n.accept(self) for n in node.bases]
         if node._metaclass and not node.has_metaclass_hack():
             args.append("metaclass=" + node._metaclass.accept(self))
         args += [n.accept(self) for n in node.keywords]
-        args = f"({', '.join(args)})" if args else ""
-        docs = self._docs_dedent(node.doc) if node.doc else ""
+        args_str = f"({', '.join(args)})" if args else ""
+        docs = self._docs_dedent(node.doc_node)
         return "\n\n{}class {}{}:{}\n{}\n".format(
-            decorate, node.name, args, docs, self._stmt_list(node.body)
+            decorate, node.name, args_str, docs, self._stmt_list(node.body)
         )
 
-    def visit_compare(self, node):
+    def visit_compare(self, node) -> str:
         """return an astroid.Compare node as string"""
         rhs_str = " ".join(
             f"{op} {self._precedence_parens(node, expr, is_left=False)}"
             for op, expr in node.ops
         )
         return f"{self._precedence_parens(node, node.left)} {rhs_str}"
 
-    def visit_comprehension(self, node):
+    def visit_comprehension(self, node) -> str:
         """return an astroid.Comprehension node as string"""
         ifs = "".join(f" if {n.accept(self)}" for n in node.ifs)
         generated = f"for {node.target.accept(self)} in {node.iter.accept(self)}{ifs}"
         return f"{'async ' if node.is_async else ''}{generated}"
 
-    def visit_const(self, node):
+    def visit_const(self, node) -> str:
         """return an astroid.Const node as string"""
         if node.value is Ellipsis:
             return "..."
         return repr(node.value)
 
-    def visit_continue(self, node):
+    def visit_continue(self, node) -> str:
         """return an astroid.Continue node as string"""
         return "continue"
 
-    def visit_delete(self, node):  # XXX check if correct
+    def visit_delete(self, node) -> str:  # XXX check if correct
         """return an astroid.Delete node as string"""
         return f"del {', '.join(child.accept(self) for child in node.targets)}"
 
-    def visit_delattr(self, node):
+    def visit_delattr(self, node) -> str:
         """return an astroid.DelAttr node as string"""
         return self.visit_attribute(node)
 
-    def visit_delname(self, node):
+    def visit_delname(self, node) -> str:
         """return an astroid.DelName node as string"""
         return node.name
 
-    def visit_decorators(self, node):
+    def visit_decorators(self, node) -> str:
         """return an astroid.Decorators node as string"""
         return "@%s\n" % "\n@".join(item.accept(self) for item in node.nodes)
 
-    def visit_dict(self, node):
+    def visit_dict(self, node) -> str:
         """return an astroid.Dict node as string"""
         return "{%s}" % ", ".join(self._visit_dict(node))
 
-    def _visit_dict(self, node):
+    def _visit_dict(self, node) -> Iterator[str]:
         for key, value in node.items:
             key = key.accept(self)
             value = value.accept(self)
             if key == "**":
                 # It can only be a DictUnpack node.
                 yield key + value
             else:
                 yield f"{key}: {value}"
 
-    def visit_dictunpack(self, node):
+    def visit_dictunpack(self, node) -> str:
         return "**"
 
-    def visit_dictcomp(self, node):
+    def visit_dictcomp(self, node) -> str:
         """return an astroid.DictComp node as string"""
         return "{{{}: {} {}}}".format(
             node.key.accept(self),
             node.value.accept(self),
             " ".join(n.accept(self) for n in node.generators),
         )
 
-    def visit_expr(self, node):
+    def visit_expr(self, node) -> str:
         """return an astroid.Discard node as string"""
         return node.value.accept(self)
 
-    def visit_emptynode(self, node):
+    def visit_emptynode(self, node) -> str:
         """dummy method for visiting an Empty node"""
         return ""
 
-    def visit_excepthandler(self, node):
+    def visit_excepthandler(self, node) -> str:
+        n = "except"
+        if isinstance(getattr(node, "parent", None), nodes.TryStar):
+            n = "except*"
         if node.type:
             if node.name:
-                excs = f"except {node.type.accept(self)} as {node.name.accept(self)}"
+                excs = f"{n} {node.type.accept(self)} as {node.name.accept(self)}"
             else:
-                excs = f"except {node.type.accept(self)}"
+                excs = f"{n} {node.type.accept(self)}"
         else:
-            excs = "except"
+            excs = f"{n}"
         return f"{excs}:\n{self._stmt_list(node.body)}"
 
-    def visit_empty(self, node):
+    def visit_empty(self, node) -> str:
         """return an Empty node as string"""
         return ""
 
-    def visit_for(self, node):
+    def visit_for(self, node) -> str:
         """return an astroid.For node as string"""
         fors = "for {} in {}:\n{}".format(
             node.target.accept(self), node.iter.accept(self), self._stmt_list(node.body)
         )
         if node.orelse:
             fors = f"{fors}\nelse:\n{self._stmt_list(node.orelse)}"
         return fors
 
-    def visit_importfrom(self, node):
+    def visit_importfrom(self, node) -> str:
         """return an astroid.ImportFrom node as string"""
         return "from {} import {}".format(
             "." * (node.level or 0) + node.modname, _import_string(node.names)
         )
 
-    def visit_joinedstr(self, node):
+    def visit_joinedstr(self, node) -> str:
         string = "".join(
             # Use repr on the string literal parts
             # to get proper escapes, e.g. \n, \\, \"
             # But strip the quotes off the ends
             # (they will always be one character: ' or ")
             repr(value.value)[1:-1]
             # Literal braces must be doubled to escape them
@@ -309,29 +307,29 @@
         # using a triple quote is sometimes necessary
         for quote in ("'", '"', '"""', "'''"):
             if quote not in string:
                 break
 
         return "f" + quote + string + quote
 
-    def visit_formattedvalue(self, node):
+    def visit_formattedvalue(self, node) -> str:
         result = node.value.accept(self)
         if node.conversion and node.conversion >= 0:
             # e.g. if node.conversion == 114: result += "!r"
             result += "!" + chr(node.conversion)
         if node.format_spec:
             # The format spec is itself a JoinedString, i.e. an f-string
             # We strip the f and quotes of the ends
             result += ":" + node.format_spec.accept(self)[2:-1]
         return "{%s}" % result
 
-    def handle_functiondef(self, node, keyword):
+    def handle_functiondef(self, node, keyword) -> str:
         """return a (possibly async) function definition node as string"""
         decorate = node.decorators.accept(self) if node.decorators else ""
-        docs = self._docs_dedent(node.doc) if node.doc else ""
+        docs = self._docs_dedent(node.doc_node)
         trailer = ":"
         if node.returns:
             return_annotation = " -> " + node.returns.as_string()
             trailer = return_annotation + ":"
         def_format = "\n%s%s %s(%s)%s%s\n%s"
         return def_format % (
             decorate,
@@ -339,296 +337,307 @@
             node.name,
             node.args.accept(self),
             trailer,
             docs,
             self._stmt_list(node.body),
         )
 
-    def visit_functiondef(self, node):
+    def visit_functiondef(self, node) -> str:
         """return an astroid.FunctionDef node as string"""
         return self.handle_functiondef(node, "def")
 
-    def visit_asyncfunctiondef(self, node):
+    def visit_asyncfunctiondef(self, node) -> str:
         """return an astroid.AsyncFunction node as string"""
         return self.handle_functiondef(node, "async def")
 
-    def visit_generatorexp(self, node):
+    def visit_generatorexp(self, node) -> str:
         """return an astroid.GeneratorExp node as string"""
         return "({} {})".format(
             node.elt.accept(self), " ".join(n.accept(self) for n in node.generators)
         )
 
-    def visit_attribute(self, node):
+    def visit_attribute(self, node) -> str:
         """return an astroid.Getattr node as string"""
         left = self._precedence_parens(node, node.expr)
         if left.isdigit():
             left = f"({left})"
         return f"{left}.{node.attrname}"
 
-    def visit_global(self, node):
+    def visit_global(self, node) -> str:
         """return an astroid.Global node as string"""
         return f"global {', '.join(node.names)}"
 
-    def visit_if(self, node):
+    def visit_if(self, node) -> str:
         """return an astroid.If node as string"""
         ifs = [f"if {node.test.accept(self)}:\n{self._stmt_list(node.body)}"]
         if node.has_elif_block():
             ifs.append(f"el{self._stmt_list(node.orelse, indent=False)}")
         elif node.orelse:
             ifs.append(f"else:\n{self._stmt_list(node.orelse)}")
         return "\n".join(ifs)
 
-    def visit_ifexp(self, node):
+    def visit_ifexp(self, node) -> str:
         """return an astroid.IfExp node as string"""
         return "{} if {} else {}".format(
             self._precedence_parens(node, node.body, is_left=True),
             self._precedence_parens(node, node.test, is_left=True),
             self._precedence_parens(node, node.orelse, is_left=False),
         )
 
-    def visit_import(self, node):
+    def visit_import(self, node) -> str:
         """return an astroid.Import node as string"""
         return f"import {_import_string(node.names)}"
 
-    def visit_keyword(self, node):
+    def visit_keyword(self, node) -> str:
         """return an astroid.Keyword node as string"""
         if node.arg is None:
             return f"**{node.value.accept(self)}"
         return f"{node.arg}={node.value.accept(self)}"
 
-    def visit_lambda(self, node):
+    def visit_lambda(self, node) -> str:
         """return an astroid.Lambda node as string"""
         args = node.args.accept(self)
         body = node.body.accept(self)
         if args:
             return f"lambda {args}: {body}"
 
         return f"lambda: {body}"
 
-    def visit_list(self, node):
+    def visit_list(self, node) -> str:
         """return an astroid.List node as string"""
         return f"[{', '.join(child.accept(self) for child in node.elts)}]"
 
-    def visit_listcomp(self, node):
+    def visit_listcomp(self, node) -> str:
         """return an astroid.ListComp node as string"""
         return "[{} {}]".format(
             node.elt.accept(self), " ".join(n.accept(self) for n in node.generators)
         )
 
-    def visit_module(self, node):
+    def visit_module(self, node) -> str:
         """return an astroid.Module node as string"""
-        docs = f'"""{node.doc}"""\n\n' if node.doc else ""
+        docs = f'"""{node.doc_node.value}"""\n\n' if node.doc_node else ""
         return docs + "\n".join(n.accept(self) for n in node.body) + "\n\n"
 
-    def visit_name(self, node):
+    def visit_name(self, node) -> str:
         """return an astroid.Name node as string"""
         return node.name
 
-    def visit_namedexpr(self, node):
+    def visit_namedexpr(self, node) -> str:
         """Return an assignment expression node as string"""
         target = node.target.accept(self)
         value = node.value.accept(self)
         return f"{target} := {value}"
 
-    def visit_nonlocal(self, node):
+    def visit_nonlocal(self, node) -> str:
         """return an astroid.Nonlocal node as string"""
         return f"nonlocal {', '.join(node.names)}"
 
-    def visit_pass(self, node):
+    def visit_pass(self, node) -> str:
         """return an astroid.Pass node as string"""
         return "pass"
 
-    def visit_raise(self, node):
+    def visit_raise(self, node) -> str:
         """return an astroid.Raise node as string"""
         if node.exc:
             if node.cause:
                 return f"raise {node.exc.accept(self)} from {node.cause.accept(self)}"
             return f"raise {node.exc.accept(self)}"
         return "raise"
 
-    def visit_return(self, node):
+    def visit_return(self, node) -> str:
         """return an astroid.Return node as string"""
         if node.is_tuple_return() and len(node.value.elts) > 1:
             elts = [child.accept(self) for child in node.value.elts]
             return f"return {', '.join(elts)}"
 
         if node.value:
             return f"return {node.value.accept(self)}"
 
         return "return"
 
-    def visit_set(self, node):
+    def visit_set(self, node) -> str:
         """return an astroid.Set node as string"""
         return "{%s}" % ", ".join(child.accept(self) for child in node.elts)
 
-    def visit_setcomp(self, node):
+    def visit_setcomp(self, node) -> str:
         """return an astroid.SetComp node as string"""
         return "{{{} {}}}".format(
             node.elt.accept(self), " ".join(n.accept(self) for n in node.generators)
         )
 
-    def visit_slice(self, node):
+    def visit_slice(self, node) -> str:
         """return an astroid.Slice node as string"""
         lower = node.lower.accept(self) if node.lower else ""
         upper = node.upper.accept(self) if node.upper else ""
         step = node.step.accept(self) if node.step else ""
         if step:
             return f"{lower}:{upper}:{step}"
         return f"{lower}:{upper}"
 
-    def visit_subscript(self, node):
+    def visit_subscript(self, node) -> str:
         """return an astroid.Subscript node as string"""
         idx = node.slice
         if idx.__class__.__name__.lower() == "index":
             idx = idx.value
         idxstr = idx.accept(self)
         if idx.__class__.__name__.lower() == "tuple" and idx.elts:
             # Remove parenthesis in tuple and extended slice.
             # a[(::1, 1:)] is not valid syntax.
             idxstr = idxstr[1:-1]
         return f"{self._precedence_parens(node, node.value)}[{idxstr}]"
 
-    def visit_tryexcept(self, node):
+    def visit_tryexcept(self, node) -> str:
         """return an astroid.TryExcept node as string"""
         trys = [f"try:\n{self._stmt_list(node.body)}"]
         for handler in node.handlers:
             trys.append(handler.accept(self))
         if node.orelse:
             trys.append(f"else:\n{self._stmt_list(node.orelse)}")
         return "\n".join(trys)
 
-    def visit_tryfinally(self, node):
+    def visit_tryfinally(self, node) -> str:
         """return an astroid.TryFinally node as string"""
         return "try:\n{}\nfinally:\n{}".format(
             self._stmt_list(node.body), self._stmt_list(node.finalbody)
         )
 
-    def visit_tuple(self, node):
+    def visit_trystar(self, node) -> str:
+        """return an astroid.TryStar node as string"""
+        trys = [f"try:\n{self._stmt_list(node.body)}"]
+        for handler in node.handlers:
+            trys.append(handler.accept(self))
+        if node.orelse:
+            trys.append(f"else:\n{self._stmt_list(node.orelse)}")
+        if node.finalbody:
+            trys.append(f"finally:\n{self._stmt_list(node.finalbody)}")
+        return "\n".join(trys)
+
+    def visit_tuple(self, node) -> str:
         """return an astroid.Tuple node as string"""
         if len(node.elts) == 1:
             return f"({node.elts[0].accept(self)}, )"
         return f"({', '.join(child.accept(self) for child in node.elts)})"
 
-    def visit_unaryop(self, node):
+    def visit_unaryop(self, node) -> str:
         """return an astroid.UnaryOp node as string"""
         if node.op == "not":
             operator = "not "
         else:
             operator = node.op
         return f"{operator}{self._precedence_parens(node, node.operand)}"
 
-    def visit_while(self, node):
+    def visit_while(self, node) -> str:
         """return an astroid.While node as string"""
         whiles = f"while {node.test.accept(self)}:\n{self._stmt_list(node.body)}"
         if node.orelse:
             whiles = f"{whiles}\nelse:\n{self._stmt_list(node.orelse)}"
         return whiles
 
-    def visit_with(self, node):  # 'with' without 'as' is possible
+    def visit_with(self, node) -> str:  # 'with' without 'as' is possible
         """return an astroid.With node as string"""
         items = ", ".join(
             f"{expr.accept(self)}" + (v and f" as {v.accept(self)}" or "")
             for expr, v in node.items
         )
         return f"with {items}:\n{self._stmt_list(node.body)}"
 
-    def visit_yield(self, node):
+    def visit_yield(self, node) -> str:
         """yield an ast.Yield node as string"""
         yi_val = (" " + node.value.accept(self)) if node.value else ""
         expr = "yield" + yi_val
         if node.parent.is_statement:
             return expr
 
         return f"({expr})"
 
-    def visit_yieldfrom(self, node):
+    def visit_yieldfrom(self, node) -> str:
         """Return an astroid.YieldFrom node as string."""
         yi_val = (" " + node.value.accept(self)) if node.value else ""
         expr = "yield from" + yi_val
         if node.parent.is_statement:
             return expr
 
         return f"({expr})"
 
-    def visit_starred(self, node):
+    def visit_starred(self, node) -> str:
         """return Starred node as string"""
         return "*" + node.value.accept(self)
 
-    def visit_match(self, node: "Match") -> str:
+    def visit_match(self, node: Match) -> str:
         """Return an astroid.Match node as string."""
         return f"match {node.subject.accept(self)}:\n{self._stmt_list(node.cases)}"
 
-    def visit_matchcase(self, node: "MatchCase") -> str:
+    def visit_matchcase(self, node: MatchCase) -> str:
         """Return an astroid.MatchCase node as string."""
         guard_str = f" if {node.guard.accept(self)}" if node.guard else ""
         return (
             f"case {node.pattern.accept(self)}{guard_str}:\n"
             f"{self._stmt_list(node.body)}"
         )
 
-    def visit_matchvalue(self, node: "MatchValue") -> str:
+    def visit_matchvalue(self, node: MatchValue) -> str:
         """Return an astroid.MatchValue node as string."""
         return node.value.accept(self)
 
     @staticmethod
-    def visit_matchsingleton(node: "MatchSingleton") -> str:
+    def visit_matchsingleton(node: MatchSingleton) -> str:
         """Return an astroid.MatchSingleton node as string."""
         return str(node.value)
 
-    def visit_matchsequence(self, node: "MatchSequence") -> str:
+    def visit_matchsequence(self, node: MatchSequence) -> str:
         """Return an astroid.MatchSequence node as string."""
         if node.patterns is None:
             return "[]"
         return f"[{', '.join(p.accept(self) for p in node.patterns)}]"
 
-    def visit_matchmapping(self, node: "MatchMapping") -> str:
+    def visit_matchmapping(self, node: MatchMapping) -> str:
         """Return an astroid.MatchMapping node as string."""
-        mapping_strings: List[str] = []
+        mapping_strings: list[str] = []
         if node.keys and node.patterns:
             mapping_strings.extend(
                 f"{key.accept(self)}: {p.accept(self)}"
                 for key, p in zip(node.keys, node.patterns)
             )
         if node.rest:
             mapping_strings.append(f"**{node.rest.accept(self)}")
         return f"{'{'}{', '.join(mapping_strings)}{'}'}"
 
-    def visit_matchclass(self, node: "MatchClass") -> str:
+    def visit_matchclass(self, node: MatchClass) -> str:
         """Return an astroid.MatchClass node as string."""
         if node.cls is None:
-            raise Exception(f"{node} does not have a 'cls' node")
-        class_strings: List[str] = []
+            raise AssertionError(f"{node} does not have a 'cls' node")
+        class_strings: list[str] = []
         if node.patterns:
             class_strings.extend(p.accept(self) for p in node.patterns)
         if node.kwd_attrs and node.kwd_patterns:
             for attr, pattern in zip(node.kwd_attrs, node.kwd_patterns):
                 class_strings.append(f"{attr}={pattern.accept(self)}")
         return f"{node.cls.accept(self)}({', '.join(class_strings)})"
 
-    def visit_matchstar(self, node: "MatchStar") -> str:
+    def visit_matchstar(self, node: MatchStar) -> str:
         """Return an astroid.MatchStar node as string."""
         return f"*{node.name.accept(self) if node.name else '_'}"
 
-    def visit_matchas(self, node: "MatchAs") -> str:
+    def visit_matchas(self, node: MatchAs) -> str:
         """Return an astroid.MatchAs node as string."""
         # pylint: disable=import-outside-toplevel
         # Prevent circular dependency
         from astroid.nodes.node_classes import MatchClass, MatchMapping, MatchSequence
 
         if isinstance(node.parent, (MatchSequence, MatchMapping, MatchClass)):
             return node.name.accept(self) if node.name else "_"
         return (
             f"{node.pattern.accept(self) if node.pattern else '_'}"
             f"{f' as {node.name.accept(self)}' if node.name else ''}"
         )
 
-    def visit_matchor(self, node: "MatchOr") -> str:
+    def visit_matchor(self, node: MatchOr) -> str:
         """Return an astroid.MatchOr node as string."""
         if node.patterns is None:
-            raise Exception(f"{node} does not have pattern nodes")
+            raise AssertionError(f"{node} does not have pattern nodes")
         return " | ".join(p.accept(self) for p in node.patterns)
 
     # These aren't for real AST nodes, but for inference objects.
 
     def visit_frozenset(self, node):
         return node.parent.accept(self)
 
@@ -640,19 +649,19 @@
 
     def visit_property(self, node):
         return node.function.accept(self)
 
     def visit_evaluatedobject(self, node):
         return node.original.accept(self)
 
-    def visit_unknown(self, node: "Unknown") -> str:
+    def visit_unknown(self, node: Unknown) -> str:
         return str(node)
 
 
-def _import_string(names):
+def _import_string(names) -> str:
     """return a list of (name, asname) formatted as a string"""
     _names = []
     for name, asname in names:
         if asname is not None:
             _names.append(f"{name} as {asname}")
         else:
             _names.append(name)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/nodes/const.py` & `astroid-3.0.0a1/astroid/nodes/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/master/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 OP_PRECEDENCE = {
     op: precedence
     for precedence, ops in enumerate(
         [
             ["Lambda"],  # lambda x: x + 1
             ["IfExp"],  # 1 if True else 2
```

### Comparing `astroid-2.9.3/astroid/nodes/node_classes.py` & `astroid-3.0.0a1/astroid/nodes/node_classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,117 @@
-# Copyright (c) 2009-2011, 2013-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2010 Daniel Harding <dharding@gmail.com>
-# Copyright (c) 2012 FELD Boris <lothiraldan@gmail.com>
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2014-2021 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Florian Bruhin <me@the-compiler.org>
-# Copyright (c) 2016-2017 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2016 Jared Garst <jgarst@users.noreply.github.com>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2016 Dave Baum <dbaum@google.com>
-# Copyright (c) 2017-2020 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2017, 2019 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 rr- <rr-@sakuya.pl>
-# Copyright (c) 2018, 2021 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 brendanator <brendan.maginnis@gmail.com>
-# Copyright (c) 2018 HoverHell <hoverhell@gmail.com>
-# Copyright (c) 2019 kavins14 <kavin.singh@mail.utoronto.ca>
-# Copyright (c) 2019 kavins14 <kavinsingh@hotmail.com>
-# Copyright (c) 2020 Raphael Gaschignard <raphael@rtpg.co>
-# Copyright (c) 2020 Bryce Guinta <bryce.guinta@protonmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Kian Meng, Ang <kianmeng.ang@gmail.com>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 Alphadelta14 <alpha@alphaservcomputing.solutions>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-# Copyright (c) 2021 Federico Bond <federicobond@gmail.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Module for some node classes. More nodes in scoped_nodes.py"""
 
+from __future__ import annotations
+
 import abc
 import itertools
-import sys
 import typing
 import warnings
-from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Callable, Generator, Optional, TypeVar, Union
+from collections.abc import Generator, Iterable, Iterator, Mapping
+from functools import cached_property, lru_cache
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    ClassVar,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+)
 
-from astroid import decorators, mixins, util
+from astroid import decorators, util
 from astroid.bases import Instance, _infer_stmts
-from astroid.const import Context
+from astroid.const import _EMPTY_OBJECT_MARKER, Context
 from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidIndexError,
     AstroidTypeError,
+    AstroidValueError,
     InferenceError,
     NoDefault,
     ParentMissingError,
 )
 from astroid.manager import AstroidManager
+from astroid.nodes import _base_nodes
 from astroid.nodes.const import OP_PRECEDENCE
 from astroid.nodes.node_ng import NodeNG
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from astroid.typing import (
+    ConstFactoryResult,
+    InferBinaryOp,
+    InferenceErrorInfo,
+    InferenceResult,
+    SuccessfulInferenceResult,
+)
 
 if TYPE_CHECKING:
     from astroid import nodes
     from astroid.nodes import LocalsDictNodeNG
 
 
-def _is_const(value):
+def _is_const(value) -> bool:
     return isinstance(value, tuple(CONST_CLS))
 
 
-T_Nodes = TypeVar("T_Nodes", bound=NodeNG)
+_NodesT = TypeVar("_NodesT", bound=NodeNG)
+_BadOpMessageT = TypeVar("_BadOpMessageT", bound=util.BadOperationMessage)
 
 AssignedStmtsPossibleNode = Union["List", "Tuple", "AssignName", "AssignAttr", None]
 AssignedStmtsCall = Callable[
     [
-        T_Nodes,
+        _NodesT,
         AssignedStmtsPossibleNode,
         Optional[InferenceContext],
         Optional[typing.List[int]],
     ],
     Any,
 ]
+InferBinaryOperation = Callable[
+    [_NodesT, Optional[InferenceContext]],
+    typing.Generator[Union[InferenceResult, _BadOpMessageT], None, None],
+]
+InferLHS = Callable[
+    [_NodesT, Optional[InferenceContext]],
+    typing.Generator[InferenceResult, None, Optional[InferenceErrorInfo]],
+]
+InferUnaryOp = Callable[[_NodesT, str], ConstFactoryResult]
 
 
 @decorators.raise_if_nothing_inferred
-def unpack_infer(stmt, context=None):
+def unpack_infer(stmt, context: InferenceContext | None = None):
     """recursively generate nodes inferred by the given statement.
     If the inferred value is a list or a tuple, recurse on the elements
     """
     if isinstance(stmt, (List, Tuple)):
         for elt in stmt.elts:
             if elt is util.Uninferable:
                 yield elt
                 continue
             yield from unpack_infer(elt, context)
-        return dict(node=stmt, context=context)
+        return {"node": stmt, "context": context}
     # if inferred is a final node, return it and stop
     inferred = next(stmt.infer(context), util.Uninferable)
     if inferred is stmt:
         yield inferred
-        return dict(node=stmt, context=context)
+        return {"node": stmt, "context": context}
     # else, infer recursively, except Uninferable object that should be returned as is
     for inferred in stmt.infer(context):
-        if inferred is util.Uninferable:
+        if isinstance(inferred, util.UninferableBase):
             yield inferred
         else:
             yield from unpack_infer(inferred, context)
 
-    return dict(node=stmt, context=context)
+    return {"node": stmt, "context": context}
 
 
-def are_exclusive(stmt1, stmt2, exceptions: Optional[typing.List[str]] = None) -> bool:
+def are_exclusive(stmt1, stmt2, exceptions: list[str] | None = None) -> bool:
     """return true if the two given statements are mutually exclusive
 
     `exceptions` may be a list of exception names. If specified, discard If
     branches and check one of the statement is in an exception handler catching
     one of the given exceptions.
 
     algorithm :
@@ -140,18 +131,22 @@
     # climb among stmt2's parents until we find a common parent
     previous = stmt2
     for node in stmt2.node_ancestors():
         if node in stmt1_parents:
             # if the common parent is a If or TryExcept statement, look if
             # nodes are in exclusive branches
             if isinstance(node, If) and exceptions is None:
-                if (
-                    node.locate_child(previous)[1]
-                    is not node.locate_child(children[node])[1]
-                ):
+                c2attr, c2node = node.locate_child(previous)
+                c1attr, c1node = node.locate_child(children[node])
+                if "test" in (c1attr, c2attr):
+                    # If any node is `If.test`, then it must be inclusive with
+                    # the other node (`If.body` and `If.orelse`)
+                    return False
+                if c1attr != c2attr:
+                    # different `If` branches (`If.body` and `If.orelse`)
                     return True
             elif isinstance(node, TryExcept):
                 c2attr, c2node = node.locate_child(previous)
                 c1attr, c1node = node.locate_child(children[node])
                 if c1node is not c2node:
                     first_in_body_caught_by_handlers = (
                         c2attr == "handlers"
@@ -186,15 +181,15 @@
 
 
 # getitem() helpers.
 
 _SLICE_SENTINEL = object()
 
 
-def _slice_value(index, context=None):
+def _slice_value(index, context: InferenceContext | None = None):
     """Get the value of the given slice index."""
 
     if isinstance(index, Const):
         if isinstance(index.value, (int, type(None))):
             return index.value
     elif index is None:
         return None
@@ -213,40 +208,47 @@
 
     # Use a sentinel, because None can be a valid
     # value that this function can return,
     # as it is the case for unspecified bounds.
     return _SLICE_SENTINEL
 
 
-def _infer_slice(node, context=None):
+def _infer_slice(node, context: InferenceContext | None = None):
     lower = _slice_value(node.lower, context)
     upper = _slice_value(node.upper, context)
     step = _slice_value(node.step, context)
     if all(elem is not _SLICE_SENTINEL for elem in (lower, upper, step)):
         return slice(lower, upper, step)
 
     raise AstroidTypeError(
         message="Could not infer slice used in subscript",
         node=node,
         index=node.parent,
         context=context,
     )
 
 
-def _container_getitem(instance, elts, index, context=None):
+def _container_getitem(instance, elts, index, context: InferenceContext | None = None):
     """Get a slice or an item, using the given *index*, for the given sequence."""
     try:
         if isinstance(index, Slice):
             index_slice = _infer_slice(index, context=context)
             new_cls = instance.__class__()
             new_cls.elts = elts[index_slice]
             new_cls.parent = instance.parent
             return new_cls
         if isinstance(index, Const):
             return elts[index.value]
+    except ValueError as exc:
+        raise AstroidValueError(
+            message="Slice {index!r} cannot index container",
+            node=instance,
+            index=index,
+            context=context,
+        ) from exc
     except IndexError as exc:
         raise AstroidIndexError(
             message="Index {index!s} out of range",
             node=instance,
             index=index,
             context=context,
         ) from exc
@@ -254,87 +256,53 @@
         raise AstroidTypeError(
             message="Type error {error!r}", node=instance, index=index, context=context
         ) from exc
 
     raise AstroidTypeError(f"Could not use {index} as subscript index")
 
 
-class Statement(NodeNG):
-    """Statement node adding a few attributes"""
-
-    is_statement = True
-    """Whether this node indicates a statement."""
-
-    def next_sibling(self):
-        """The next sibling statement node.
-
-        :returns: The next sibling statement node.
-        :rtype: NodeNG or None
-        """
-        stmts = self.parent.child_sequence(self)
-        index = stmts.index(self)
-        try:
-            return stmts[index + 1]
-        except IndexError:
-            return None
-
-    def previous_sibling(self):
-        """The previous sibling statement.
-
-        :returns: The previous sibling statement node.
-        :rtype: NodeNG or None
-        """
-        stmts = self.parent.child_sequence(self)
-        index = stmts.index(self)
-        if index >= 1:
-            return stmts[index - 1]
-        return None
-
-
-class BaseContainer(
-    mixins.ParentAssignTypeMixin, NodeNG, Instance, metaclass=abc.ABCMeta
-):
+class BaseContainer(_base_nodes.ParentAssignNode, Instance, metaclass=abc.ABCMeta):
     """Base class for Set, FrozenSet, Tuple and List."""
 
     _astroid_fields = ("elts",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.elts: typing.List[NodeNG] = []
+        self.elts: list[NodeNG] = []
         """The elements in the node."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, elts: typing.List[NodeNG]) -> None:
+    def postinit(self, elts: list[NodeNG]) -> None:
         """Do some setup after initialisation.
 
         :param elts: The list of elements the that node contains.
         """
         self.elts = elts
 
     @classmethod
@@ -358,52 +326,49 @@
         """An iterator over the elements this node contains.
 
         :returns: The contents of this node.
         :rtype: iterable(NodeNG)
         """
         return self.elts
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> bool:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
-        :rtype: bool or Uninferable
         """
         return bool(self.elts)
 
     @abc.abstractmethod
-    def pytype(self):
+    def pytype(self) -> str:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
 
     def get_children(self):
         yield from self.elts
 
 
-class LookupMixIn:
+# TODO: Move into _base_nodes. Blocked by import of _infer_stmts from bases.
+class LookupMixIn(NodeNG):
     """Mixin to look up a name in the right scope."""
 
-    @lru_cache(maxsize=None)
-    def lookup(self, name):
+    @lru_cache  # noqa
+    def lookup(self, name: str) -> tuple[LocalsDictNodeNG, list[NodeNG]]:
         """Lookup where the given variable is assigned.
 
         The lookup starts from self's scope. If self is not a frame itself
         and the name is found in the inner frame locals, statements will be
         filtered to remove ignorable statements according to self's location.
 
         :param name: The name of the variable to find assignments for.
-        :type name: str
 
         :returns: The scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
-        :rtype: tuple(str, list(NodeNG))
         """
         return self.scope().scope_lookup(self, name)
 
     def ilookup(self, name):
         """Lookup the inferred values of the given variable.
 
         :param name: The variable name to find values for.
@@ -417,17 +382,15 @@
         context = InferenceContext()
         return _infer_stmts(stmts, context, frame)
 
 
 # Name classes
 
 
-class AssignName(
-    mixins.NoChildrenMixin, LookupMixIn, mixins.ParentAssignTypeMixin, NodeNG
-):
+class AssignName(_base_nodes.NoChildrenNode, LookupMixIn, _base_nodes.ParentAssignNode):
     """Variation of :class:`ast.Assign` representing assignment to a name.
 
     An :class:`AssignName` is the name of something that is assigned to.
     This includes variables defined in a function signature or in a loop.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable = range(10)')
@@ -437,113 +400,81 @@
     [<AssignName.variable l.1 at 0x7effe1db8748>, <Call l.1 at 0x7effe1db8630>]
     >>> list(node.get_children())[0].as_string()
     'variable'
     """
 
     _other_fields = ("name",)
 
-    @decorators.deprecate_default_argument_values(name="str")
+    infer_lhs: ClassVar[InferLHS[AssignName]]
+
     def __init__(
         self,
-        name: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        name: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param name: The name that is assigned to.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.name: Optional[str] = name
+        self.name = name
         """The name that is assigned to."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: AssignedStmtsCall["AssignName"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[AssignName]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
-class DelName(
-    mixins.NoChildrenMixin, LookupMixIn, mixins.ParentAssignTypeMixin, NodeNG
-):
+class DelName(_base_nodes.NoChildrenNode, LookupMixIn, _base_nodes.ParentAssignNode):
     """Variation of :class:`ast.Delete` representing deletion of a name.
 
     A :class:`DelName` is the name of something that is deleted.
 
     >>> import astroid
     >>> node = astroid.extract_node("del variable #@")
     >>> list(node.get_children())
     [<DelName.variable l.1 at 0x7effe1da4d30>]
     >>> list(node.get_children())[0].as_string()
     'variable'
     """
 
     _other_fields = ("name",)
 
-    @decorators.deprecate_default_argument_values(name="str")
     def __init__(
         self,
-        name: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        name: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param name: The name that is being deleted.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.name: Optional[str] = name
+        self.name = name
         """The name that is being deleted."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
 
-class Name(mixins.NoChildrenMixin, LookupMixIn, NodeNG):
+class Name(_base_nodes.NoChildrenNode, LookupMixIn):
     """Class representing an :class:`ast.Name` node.
 
     A :class:`Name` node is something that is named, but not covered by
     :class:`AssignName` or :class:`DelName`.
 
     >>> import astroid
     >>> node = astroid.extract_node('range(10)')
@@ -553,41 +484,25 @@
     [<Name.range l.1 at 0x7effe1db86a0>, <Const.int l.1 at 0x7effe1db8518>]
     >>> list(node.get_children())[0].as_string()
     'range'
     """
 
     _other_fields = ("name",)
 
-    @decorators.deprecate_default_argument_values(name="str")
     def __init__(
         self,
-        name: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        name: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param name: The name that this node refers to.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.name: Optional[str] = name
+        self.name = name
         """The name that this node refers to."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
@@ -597,15 +512,15 @@
     def _get_name_nodes(self):
         yield self
 
         for child_node in self.get_children():
             yield from child_node._get_name_nodes()
 
 
-class Arguments(mixins.AssignTypeMixin, NodeNG):
+class Arguments(_base_nodes.AssignTypeNode):
     """Class representing an :class:`ast.arguments` node.
 
     An :class:`Arguments` node represents that arguments in a
     function definition.
 
     >>> import astroid
     >>> node = astroid.extract_node('def foo(bar): pass')
@@ -639,200 +554,151 @@
         "type_comment_args",
         "type_comment_kwonlyargs",
         "type_comment_posonlyargs",
     )
 
     _other_fields = ("vararg", "kwarg")
 
-    lineno: None
-    col_offset: None
-    end_lineno: None
-    end_col_offset: None
+    args: list[AssignName] | None
+    """The names of the required arguments.
 
-    def __init__(
-        self,
-        vararg: Optional[str] = None,
-        kwarg: Optional[str] = None,
-        parent: Optional[NodeNG] = None,
-    ) -> None:
-        """
-        :param vararg: The name of the variable length arguments.
-
-        :param kwarg: The name of the variable length keyword arguments.
-
-        :param parent: The parent node in the syntax tree.
-        """
-        super().__init__(parent=parent)
-
-        self.vararg: Optional[str] = vararg  # can be None
-        """The name of the variable length arguments."""
+    Can be None if the associated function does not have a retrievable
+    signature and the arguments are therefore unknown.
+    This can happen with (builtin) functions implemented in C that have
+    incomplete signature information.
+    """
 
-        self.kwarg: Optional[str] = kwarg  # can be None
-        """The name of the variable length keyword arguments."""
+    defaults: list[NodeNG] | None
+    """The default values for arguments that can be passed positionally."""
 
-        self.args: typing.Optional[typing.List[AssignName]]
-        """The names of the required arguments.
+    kwonlyargs: list[AssignName]
+    """The keyword arguments that cannot be passed positionally."""
 
-        Can be None if the associated function does not have a retrievable
-        signature and the arguments are therefore unknown.
-        This happens with builtin functions implemented in C.
-        """
+    posonlyargs: list[AssignName]
+    """The arguments that can only be passed positionally."""
 
-        self.defaults: typing.List[NodeNG]
-        """The default values for arguments that can be passed positionally."""
+    kw_defaults: list[NodeNG | None] | None
+    """The default values for keyword arguments that cannot be passed positionally."""
 
-        self.kwonlyargs: typing.List[AssignName]
-        """The keyword arguments that cannot be passed positionally."""
+    annotations: list[NodeNG | None]
+    """The type annotations of arguments that can be passed positionally."""
 
-        self.posonlyargs: typing.List[AssignName] = []
-        """The arguments that can only be passed positionally."""
+    posonlyargs_annotations: list[NodeNG | None]
+    """The type annotations of arguments that can only be passed positionally."""
 
-        self.kw_defaults: typing.List[Optional[NodeNG]]
-        """The default values for keyword arguments that cannot be passed positionally."""
+    kwonlyargs_annotations: list[NodeNG | None]
+    """The type annotations of arguments that cannot be passed positionally."""
 
-        self.annotations: typing.List[Optional[NodeNG]]
-        """The type annotations of arguments that can be passed positionally."""
+    type_comment_args: list[NodeNG | None]
+    """The type annotation, passed by a type comment, of each argument.
 
-        self.posonlyargs_annotations: typing.List[Optional[NodeNG]] = []
-        """The type annotations of arguments that can only be passed positionally."""
+    If an argument does not have a type comment,
+    the value for that argument will be None.
+    """
 
-        self.kwonlyargs_annotations: typing.List[Optional[NodeNG]] = []
-        """The type annotations of arguments that cannot be passed positionally."""
+    type_comment_kwonlyargs: list[NodeNG | None]
+    """The type annotation, passed by a type comment, of each keyword only argument.
 
-        self.type_comment_args: typing.List[Optional[NodeNG]] = []
-        """The type annotation, passed by a type comment, of each argument.
+    If an argument does not have a type comment,
+    the value for that argument will be None.
+    """
 
-        If an argument does not have a type comment,
-        the value for that argument will be None.
-        """
+    type_comment_posonlyargs: list[NodeNG | None]
+    """The type annotation, passed by a type comment, of each positional argument.
 
-        self.type_comment_kwonlyargs: typing.List[Optional[NodeNG]] = []
-        """The type annotation, passed by a type comment, of each keyword only argument.
+    If an argument does not have a type comment,
+    the value for that argument will be None.
+    """
 
-        If an argument does not have a type comment,
-        the value for that argument will be None.
-        """
+    varargannotation: NodeNG | None
+    """The type annotation for the variable length arguments."""
 
-        self.type_comment_posonlyargs: typing.List[Optional[NodeNG]] = []
-        """The type annotation, passed by a type comment, of each positional argument.
+    kwargannotation: NodeNG | None
+    """The type annotation for the variable length keyword arguments."""
 
-        If an argument does not have a type comment,
-        the value for that argument will be None.
-        """
+    def __init__(self, vararg: str | None, kwarg: str | None, parent: NodeNG) -> None:
+        """Almost all attributes can be None for living objects where introspection failed."""
+        super().__init__(
+            parent=parent,
+            lineno=None,
+            col_offset=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
 
-        self.varargannotation: Optional[NodeNG] = None  # can be None
-        """The type annotation for the variable length arguments."""
+        self.vararg = vararg
+        """The name of the variable length arguments."""
 
-        self.kwargannotation: Optional[NodeNG] = None  # can be None
-        """The type annotation for the variable length keyword arguments."""
+        self.kwarg = kwarg
+        """The name of the variable length keyword arguments."""
 
     # pylint: disable=too-many-arguments
     def postinit(
         self,
-        args: typing.List[AssignName],
-        defaults: typing.List[NodeNG],
-        kwonlyargs: typing.List[AssignName],
-        kw_defaults: typing.List[Optional[NodeNG]],
-        annotations: typing.List[Optional[NodeNG]],
-        posonlyargs: Optional[typing.List[AssignName]] = None,
-        kwonlyargs_annotations: Optional[typing.List[Optional[NodeNG]]] = None,
-        posonlyargs_annotations: Optional[typing.List[Optional[NodeNG]]] = None,
-        varargannotation: Optional[NodeNG] = None,
-        kwargannotation: Optional[NodeNG] = None,
-        type_comment_args: Optional[typing.List[Optional[NodeNG]]] = None,
-        type_comment_kwonlyargs: Optional[typing.List[Optional[NodeNG]]] = None,
-        type_comment_posonlyargs: Optional[typing.List[Optional[NodeNG]]] = None,
+        args: list[AssignName] | None,
+        defaults: list[NodeNG] | None,
+        kwonlyargs: list[AssignName],
+        kw_defaults: list[NodeNG | None] | None,
+        annotations: list[NodeNG | None],
+        posonlyargs: list[AssignName],
+        kwonlyargs_annotations: list[NodeNG | None],
+        posonlyargs_annotations: list[NodeNG | None],
+        varargannotation: NodeNG | None = None,
+        kwargannotation: NodeNG | None = None,
+        type_comment_args: list[NodeNG | None] | None = None,
+        type_comment_kwonlyargs: list[NodeNG | None] | None = None,
+        type_comment_posonlyargs: list[NodeNG | None] | None = None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param args: The names of the required arguments.
-
-        :param defaults: The default values for arguments that can be passed
-            positionally.
-
-        :param kwonlyargs: The keyword arguments that cannot be passed
-            positionally.
-
-        :param posonlyargs: The arguments that can only be passed
-            positionally.
-
-        :param kw_defaults: The default values for keyword arguments that
-            cannot be passed positionally.
-
-        :param annotations: The type annotations of arguments that can be
-            passed positionally.
-
-        :param kwonlyargs_annotations: The type annotations of arguments that
-            cannot be passed positionally. This should always be passed in
-            Python 3.
-
-        :param posonlyargs_annotations: The type annotations of arguments that
-            can only be passed positionally. This should always be passed in
-            Python 3.
-
-        :param varargannotation: The type annotation for the variable length
-            arguments.
-
-        :param kwargannotation: The type annotation for the variable length
-            keyword arguments.
-
-        :param type_comment_args: The type annotation,
-            passed by a type comment, of each argument.
-
-        :param type_comment_args: The type annotation,
-            passed by a type comment, of each keyword only argument.
-
-        :param type_comment_args: The type annotation,
-            passed by a type comment, of each positional argument.
-        """
         self.args = args
         self.defaults = defaults
         self.kwonlyargs = kwonlyargs
-        if posonlyargs is not None:
-            self.posonlyargs = posonlyargs
+        self.posonlyargs = posonlyargs
         self.kw_defaults = kw_defaults
         self.annotations = annotations
-        if kwonlyargs_annotations is not None:
-            self.kwonlyargs_annotations = kwonlyargs_annotations
-        if posonlyargs_annotations is not None:
-            self.posonlyargs_annotations = posonlyargs_annotations
+        self.kwonlyargs_annotations = kwonlyargs_annotations
+        self.posonlyargs_annotations = posonlyargs_annotations
+
+        # Parameters that got added later and need a default
         self.varargannotation = varargannotation
         self.kwargannotation = kwargannotation
-        if type_comment_args is not None:
-            self.type_comment_args = type_comment_args
-        if type_comment_kwonlyargs is not None:
-            self.type_comment_kwonlyargs = type_comment_kwonlyargs
-        if type_comment_posonlyargs is not None:
-            self.type_comment_posonlyargs = type_comment_posonlyargs
+        if type_comment_args is None:
+            type_comment_args = []
+        self.type_comment_args = type_comment_args
+        if type_comment_kwonlyargs is None:
+            type_comment_kwonlyargs = []
+        self.type_comment_kwonlyargs = type_comment_kwonlyargs
+        if type_comment_posonlyargs is None:
+            type_comment_posonlyargs = []
+        self.type_comment_posonlyargs = type_comment_posonlyargs
 
-    assigned_stmts: AssignedStmtsCall["Arguments"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[Arguments]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def _infer_name(self, frame, name):
         if self.parent is frame:
             return name
         return None
 
-    @decorators.cachedproperty
-    def fromlineno(self):
+    @cached_property
+    def fromlineno(self) -> int:
         """The first line that this node appears on in the source code.
 
-        :type: int or None
+        Can also return 0 if the line can not be determined.
         """
         lineno = super().fromlineno
         return max(lineno, self.parent.fromlineno or 0)
 
-    @decorators.cachedproperty
+    @cached_property
     def arguments(self):
         """Get all the arguments for this node, including positional only and positional and keyword"""
         return list(itertools.chain((self.posonlyargs or ()), self.args or ()))
 
-    def format_args(self):
+    def format_args(self, *, skippable_names: set[str] | None = None) -> str:
         """Get the arguments formatted as string.
 
         :returns: The formatted arguments.
         :rtype: str
         """
         result = []
         positional_only_defaults = []
@@ -844,39 +710,113 @@
 
         if self.posonlyargs:
             result.append(
                 _format_args(
                     self.posonlyargs,
                     positional_only_defaults,
                     self.posonlyargs_annotations,
+                    skippable_names=skippable_names,
                 )
             )
             result.append("/")
         if self.args:
             result.append(
                 _format_args(
                     self.args,
                     positional_or_keyword_defaults,
                     getattr(self, "annotations", None),
+                    skippable_names=skippable_names,
                 )
             )
         if self.vararg:
             result.append(f"*{self.vararg}")
         if self.kwonlyargs:
             if not self.vararg:
                 result.append("*")
             result.append(
                 _format_args(
-                    self.kwonlyargs, self.kw_defaults, self.kwonlyargs_annotations
+                    self.kwonlyargs,
+                    self.kw_defaults,
+                    self.kwonlyargs_annotations,
+                    skippable_names=skippable_names,
                 )
             )
         if self.kwarg:
             result.append(f"**{self.kwarg}")
         return ", ".join(result)
 
+    def _get_arguments_data(
+        self,
+    ) -> tuple[
+        dict[str, tuple[str | None, str | None]],
+        dict[str, tuple[str | None, str | None]],
+    ]:
+        """Get the arguments as dictionary with information about typing and defaults.
+
+        The return tuple contains a dictionary for positional and keyword arguments with their typing
+        and their default value, if any.
+        The method follows a similar order as format_args but instead of formatting into a string it
+        returns the data that is used to do so.
+        """
+        pos_only: dict[str, tuple[str | None, str | None]] = {}
+        kw_only: dict[str, tuple[str | None, str | None]] = {}
+
+        # Setup and match defaults with arguments
+        positional_only_defaults = []
+        positional_or_keyword_defaults = self.defaults
+        if self.defaults:
+            args = self.args or []
+            positional_or_keyword_defaults = self.defaults[-len(args) :]
+            positional_only_defaults = self.defaults[: len(self.defaults) - len(args)]
+
+        for index, posonly in enumerate(self.posonlyargs):
+            annotation, default = self.posonlyargs_annotations[index], None
+            if annotation is not None:
+                annotation = annotation.as_string()
+            if positional_only_defaults:
+                default = positional_only_defaults[index].as_string()
+            pos_only[posonly.name] = (annotation, default)
+
+        for index, arg in enumerate(self.args):
+            annotation, default = self.annotations[index], None
+            if annotation is not None:
+                annotation = annotation.as_string()
+            if positional_or_keyword_defaults:
+                defaults_offset = len(self.args) - len(positional_or_keyword_defaults)
+                default_index = index - defaults_offset
+                if (
+                    default_index > -1
+                    and positional_or_keyword_defaults[default_index] is not None
+                ):
+                    default = positional_or_keyword_defaults[default_index].as_string()
+            pos_only[arg.name] = (annotation, default)
+
+        if self.vararg:
+            annotation = self.varargannotation
+            if annotation is not None:
+                annotation = annotation.as_string()
+            pos_only[self.vararg] = (annotation, None)
+
+        for index, kwarg in enumerate(self.kwonlyargs):
+            annotation = self.kwonlyargs_annotations[index]
+            if annotation is not None:
+                annotation = annotation.as_string()
+            default = self.kw_defaults[index]
+            if default is not None:
+                default = default.as_string()
+            kw_only[kwarg.name] = (annotation, default)
+
+        if self.kwarg:
+            annotation = self.kwargannotation
+            if annotation is not None:
+                annotation = annotation.as_string()
+            kw_only[self.kwarg] = (annotation, None)
+
+        return pos_only, kw_only
+
     def default_value(self, argname):
         """Get the default value for an argument.
 
         :param argname: The name of the argument to get the default value for.
         :type argname: str
 
         :raises NoDefault: If there is no default value defined for the
@@ -889,23 +829,21 @@
             if idx >= 0:
                 return self.defaults[idx]
         index = _find_arg(argname, self.kwonlyargs)[0]
         if index is not None and self.kw_defaults[index] is not None:
             return self.kw_defaults[index]
         raise NoDefault(func=self.parent, name=argname)
 
-    def is_argument(self, name):
+    def is_argument(self, name) -> bool:
         """Check if the given name is defined in the arguments.
 
         :param name: The name to check for.
         :type name: str
 
-        :returns: True if the given name is defined in the arguments,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether the given name is defined in the arguments,
         """
         if name == self.vararg:
             return True
         if name == self.kwarg:
             return True
         return (
             self.find_argname(name, rec=True)[1] is not None
@@ -935,18 +873,19 @@
 
         for elt in self.posonlyargs_annotations:
             if elt is not None:
                 yield elt
 
         yield from self.args or ()
 
-        yield from self.defaults
+        if self.defaults is not None:
+            yield from self.defaults
         yield from self.kwonlyargs
 
-        for elt in self.kw_defaults:
+        for elt in self.kw_defaults or ():
             if elt is not None:
                 yield elt
 
         for elt in self.annotations:
             if elt is not None:
                 yield elt
 
@@ -969,24 +908,30 @@
                 if found[0] is not None:
                     return found
         elif arg.name == argname:
             return i, arg
     return None, None
 
 
-def _format_args(args, defaults=None, annotations=None):
+def _format_args(
+    args, defaults=None, annotations=None, skippable_names: set[str] | None = None
+) -> str:
+    if skippable_names is None:
+        skippable_names = set()
     values = []
     if args is None:
         return ""
     if annotations is None:
         annotations = []
     if defaults is not None:
         default_offset = len(args) - len(defaults)
     packed = itertools.zip_longest(args, annotations)
     for i, (arg, annotation) in enumerate(packed):
+        if arg.name in skippable_names:
+            continue
         if isinstance(arg, Tuple):
             values.append(f"({_format_args(arg.elts)})")
         else:
             argname = arg.name
             default_sep = "="
             if annotation is not None:
                 argname += ": " + annotation.as_string()
@@ -995,15 +940,15 @@
 
             if defaults is not None and i >= default_offset:
                 if defaults[i - default_offset] is not None:
                     values[-1] += default_sep + defaults[i - default_offset].as_string()
     return ", ".join(values)
 
 
-class AssignAttr(mixins.ParentAssignTypeMixin, NodeNG):
+class AssignAttr(_base_nodes.ParentAssignNode):
     """Variation of :class:`ast.Assign` representing assignment to an attribute.
 
     >>> import astroid
     >>> node = astroid.extract_node('self.attribute = range(10)')
     >>> node
     <Assign l.1 at 0x7effe1d521d0>
     >>> list(node.get_children())
@@ -1011,402 +956,244 @@
     >>> list(node.get_children())[0].as_string()
     'self.attribute'
     """
 
     _astroid_fields = ("expr",)
     _other_fields = ("attrname",)
 
-    @decorators.deprecate_default_argument_values(attrname="str")
+    infer_lhs: ClassVar[InferLHS[AssignAttr]]
+
+    expr: NodeNG
+    """What has the attribute that is being assigned to."""
+
     def __init__(
         self,
-        attrname: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        attrname: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param attrname: The name of the attribute being assigned to.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.expr: Optional[NodeNG] = None
-        """What has the attribute that is being assigned to."""
-
-        self.attrname: Optional[str] = attrname
+        self.attrname = attrname
         """The name of the attribute being assigned to."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, expr: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param expr: What has the attribute that is being assigned to.
-        """
+    def postinit(self, expr: NodeNG) -> None:
         self.expr = expr
 
-    assigned_stmts: AssignedStmtsCall["AssignAttr"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[AssignAttr]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.expr
 
 
-class Assert(Statement):
+class Assert(_base_nodes.Statement):
     """Class representing an :class:`ast.Assert` node.
 
     An :class:`Assert` node represents an assert statement.
 
     >>> import astroid
     >>> node = astroid.extract_node('assert len(things) == 10, "Not enough things"')
     >>> node
     <Assert l.1 at 0x7effe1d527b8>
     """
 
     _astroid_fields = ("test", "fail")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.test: Optional[NodeNG] = None
-        """The test that passes or fails the assertion."""
+    test: NodeNG
+    """The test that passes or fails the assertion."""
 
-        self.fail: Optional[NodeNG] = None  # can be None
-        """The message shown when the assertion fails."""
+    fail: NodeNG | None
+    """The message shown when the assertion fails."""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(
-        self, test: Optional[NodeNG] = None, fail: Optional[NodeNG] = None
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param test: The test that passes or fails the assertion.
-
-        :param fail: The message shown when the assertion fails.
-        """
+    def postinit(self, test: NodeNG, fail: NodeNG | None) -> None:
         self.fail = fail
         self.test = test
 
     def get_children(self):
         yield self.test
 
         if self.fail is not None:
             yield self.fail
 
 
-class Assign(mixins.AssignTypeMixin, Statement):
+class Assign(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Assign` node.
 
     An :class:`Assign` is a statement where something is explicitly
     asssigned to.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable = range(10)')
     >>> node
     <Assign l.1 at 0x7effe1db8550>
     """
 
-    _astroid_fields = ("targets", "value")
-    _other_other_fields = ("type_annotation",)
-
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.targets: typing.List[NodeNG] = []
-        """What is being assigned to."""
+    targets: list[NodeNG]
+    """What is being assigned to."""
 
-        self.value: Optional[NodeNG] = None
-        """The value being assigned to the variables."""
+    value: NodeNG
+    """The value being assigned to the variables."""
 
-        self.type_annotation: Optional[NodeNG] = None  # can be None
-        """If present, this will contain the type annotation passed by a type comment"""
+    type_annotation: NodeNG | None
+    """If present, this will contain the type annotation passed by a type comment"""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    _astroid_fields = ("targets", "value")
+    _other_other_fields = ("type_annotation",)
 
     def postinit(
         self,
-        targets: Optional[typing.List[NodeNG]] = None,
-        value: Optional[NodeNG] = None,
-        type_annotation: Optional[NodeNG] = None,
+        targets: list[NodeNG],
+        value: NodeNG,
+        type_annotation: NodeNG | None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param targets: What is being assigned to.
-        :param value: The value being assigned to the variables.
-        :param type_annotation:
-        """
-        if targets is not None:
-            self.targets = targets
+        self.targets = targets
         self.value = value
         self.type_annotation = type_annotation
 
-    assigned_stmts: AssignedStmtsCall["Assign"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[Assign]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield from self.targets
 
         yield self.value
 
-    @decorators.cached
-    def _get_assign_nodes(self):
-        return [self] + list(self.value._get_assign_nodes())
+    @cached_property
+    def _assign_nodes_in_scope(self) -> list[nodes.Assign]:
+        return [self, *self.value._assign_nodes_in_scope]
 
     def _get_yield_nodes_skip_lambdas(self):
         yield from self.value._get_yield_nodes_skip_lambdas()
 
 
-class AnnAssign(mixins.AssignTypeMixin, Statement):
+class AnnAssign(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing an :class:`ast.AnnAssign` node.
 
     An :class:`AnnAssign` is an assignment with a type annotation.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable: List[int] = range(10)')
     >>> node
     <AnnAssign l.1 at 0x7effe1d4c630>
     """
 
     _astroid_fields = ("target", "annotation", "value")
     _other_fields = ("simple",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
+    target: Name | Attribute | Subscript
+    """What is being assigned to."""
 
-        :param end_lineno: The last line this node appears on in the source code.
+    annotation: NodeNG
+    """The type annotation of what is being assigned to."""
 
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.target: Optional[NodeNG] = None
-        """What is being assigned to."""
+    value: NodeNG | None
+    """The value being assigned to the variables."""
 
-        self.annotation: Optional[NodeNG] = None
-        """The type annotation of what is being assigned to."""
-
-        self.value: Optional[NodeNG] = None  # can be None
-        """The value being assigned to the variables."""
-
-        self.simple: Optional[int] = None
-        """Whether :attr:`target` is a pure name or a complex statement."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    simple: int
+    """Whether :attr:`target` is a pure name or a complex statement."""
 
     def postinit(
         self,
-        target: NodeNG,
+        target: Name | Attribute | Subscript,
         annotation: NodeNG,
         simple: int,
-        value: Optional[NodeNG] = None,
+        value: NodeNG | None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param target: What is being assigned to.
-
-        :param annotation: The type annotation of what is being assigned to.
-
-        :param simple: Whether :attr:`target` is a pure name
-            or a complex statement.
-
-        :param value: The value being assigned to the variables.
-        """
         self.target = target
         self.annotation = annotation
         self.value = value
         self.simple = simple
 
-    assigned_stmts: AssignedStmtsCall["AnnAssign"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[AnnAssign]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.target
         yield self.annotation
 
         if self.value is not None:
             yield self.value
 
 
-class AugAssign(mixins.AssignTypeMixin, Statement):
+class AugAssign(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing an :class:`ast.AugAssign` node.
 
     An :class:`AugAssign` is an assignment paired with an operator.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable += 1')
     >>> node
     <AugAssign l.1 at 0x7effe1db4d68>
     """
 
     _astroid_fields = ("target", "value")
     _other_fields = ("op",)
 
-    @decorators.deprecate_default_argument_values(op="str")
+    target: Name | Attribute | Subscript
+    """What is being assigned to."""
+
+    value: NodeNG
+    """The value being assigned to the variable."""
+
     def __init__(
         self,
-        op: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        op: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param op: The operator that is being combined with the assignment.
-            This includes the equals sign.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.target: Optional[NodeNG] = None
-        """What is being assigned to."""
-
-        self.op: Optional[str] = op
+        self.op = op
         """The operator that is being combined with the assignment.
 
         This includes the equals sign.
         """
 
-        self.value: Optional[NodeNG] = None
-        """The value being assigned to the variable."""
-
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(
-        self, target: Optional[NodeNG] = None, value: Optional[NodeNG] = None
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param target: What is being assigned to.
-
-        :param value: The value being assigned to the variable.
-        """
+    def postinit(self, target: Name | Attribute | Subscript, value: NodeNG) -> None:
         self.target = target
         self.value = value
 
-    assigned_stmts: AssignedStmtsCall["AugAssign"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[AugAssign]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     # This is set by inference.py
-    def _infer_augassign(self, context=None):
-        raise NotImplementedError
+    _infer_augassign: ClassVar[
+        InferBinaryOperation[AugAssign, util.BadBinaryOperationMessage]
+    ]
 
-    def type_errors(self, context=None):
+    def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
         Each TypeError is represented by a :class:`BadBinaryOperationMessage` ,
         which holds the original exception.
 
         :returns: The list of possible type errors.
         :rtype: list(BadBinaryOperationMessage)
@@ -1441,74 +1228,49 @@
     >>> node
     <BinOp l.1 at 0x7f23b2e8cfd0>
     """
 
     _astroid_fields = ("left", "right")
     _other_fields = ("op",)
 
-    @decorators.deprecate_default_argument_values(op="str")
+    left: NodeNG
+    """What is being applied to the operator on the left side."""
+
+    right: NodeNG
+    """What is being applied to the operator on the right side."""
+
     def __init__(
         self,
-        op: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        op: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param op: The operator.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.left: Optional[NodeNG] = None
-        """What is being applied to the operator on the left side."""
-
-        self.op: Optional[str] = op
+        self.op = op
         """The operator."""
 
-        self.right: Optional[NodeNG] = None
-        """What is being applied to the operator on the right side."""
-
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(
-        self, left: Optional[NodeNG] = None, right: Optional[NodeNG] = None
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param left: What is being applied to the operator on the left side.
-
-        :param right: What is being applied to the operator on the right side.
-        """
+    def postinit(self, left: NodeNG, right: NodeNG) -> None:
         self.left = left
         self.right = right
 
     # This is set by inference.py
-    def _infer_binop(self, context=None):
-        raise NotImplementedError
+    _infer_binop: ClassVar[InferBinaryOperation[BinOp, util.BadBinaryOperationMessage]]
 
-    def type_errors(self, context=None):
+    def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
         Each TypeError is represented by a :class:`BadBinaryOperationMessage`,
         which holds the original exception.
 
         :returns: The list of possible type errors.
         :rtype: list(BadBinaryOperationMessage)
@@ -1526,15 +1288,15 @@
     def get_children(self):
         yield self.left
         yield self.right
 
     def op_precedence(self):
         return OP_PRECEDENCE[self.op]
 
-    def op_left_associative(self):
+    def op_left_associative(self) -> bool:
         # 2**3**4 == 2**(3**4)
         return self.op != "**"
 
 
 class BoolOp(NodeNG):
     """Class representing an :class:`ast.BoolOp` node.
 
@@ -1548,21 +1310,21 @@
 
     _astroid_fields = ("values",)
     _other_fields = ("op",)
 
     @decorators.deprecate_default_argument_values(op="str")
     def __init__(
         self,
-        op: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        op: str | None = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param op: The operator.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -1571,44 +1333,44 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.op: Optional[str] = op
+        self.op: str | None = op
         """The operator."""
 
-        self.values: typing.List[NodeNG] = []
+        self.values: list[NodeNG] = []
         """The values being applied to the operator."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, values: Optional[typing.List[NodeNG]] = None) -> None:
+    def postinit(self, values: list[NodeNG] | None = None) -> None:
         """Do some setup after initialisation.
 
         :param values: The values being applied to the operator.
         """
         if values is not None:
             self.values = values
 
     def get_children(self):
         yield from self.values
 
     def op_precedence(self):
         return OP_PRECEDENCE[self.op]
 
 
-class Break(mixins.NoChildrenMixin, Statement):
+class Break(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Break` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('break')
     >>> node
     <Break l.1 at 0x7f23b2e9e5c0>
     """
@@ -1623,80 +1385,37 @@
     >>> node = astroid.extract_node('function()')
     >>> node
     <Call l.1 at 0x7f23b2e71eb8>
     """
 
     _astroid_fields = ("func", "args", "keywords")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
+    func: NodeNG
+    """What is being called."""
 
-        :param parent: The parent node in the syntax tree.
+    args: list[NodeNG]
+    """The positional arguments being given to the call."""
 
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.func: Optional[NodeNG] = None
-        """What is being called."""
-
-        self.args: typing.List[NodeNG] = []
-        """The positional arguments being given to the call."""
-
-        self.keywords: typing.List["Keyword"] = []
-        """The keyword arguments being given to the call."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    keywords: list[Keyword]
+    """The keyword arguments being given to the call."""
 
     def postinit(
-        self,
-        func: Optional[NodeNG] = None,
-        args: Optional[typing.List[NodeNG]] = None,
-        keywords: Optional[typing.List["Keyword"]] = None,
+        self, func: NodeNG, args: list[NodeNG], keywords: list[Keyword]
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param func: What is being called.
-
-        :param args: The positional arguments being given to the call.
-
-        :param keywords: The keyword arguments being given to the call.
-        """
         self.func = func
-        if args is not None:
-            self.args = args
-        if keywords is not None:
-            self.keywords = keywords
+        self.args = args
+        self.keywords = keywords
 
     @property
-    def starargs(self) -> typing.List["Starred"]:
+    def starargs(self) -> list[Starred]:
         """The positional arguments that unpack something."""
         return [arg for arg in self.args if isinstance(arg, Starred)]
 
     @property
-    def kwargs(self) -> typing.List["Keyword"]:
+    def kwargs(self) -> list[Keyword]:
         """The keyword arguments that unpack something."""
         return [keyword for keyword in self.keywords if keyword.arg is None]
 
     def get_children(self):
         yield self.func
 
         yield from self.args
@@ -1715,66 +1434,23 @@
     <Compare l.1 at 0x7f23b2e9e6d8>
     >>> node.ops
     [('<=', <Name.b l.1 at 0x7f23b2e9e2b0>), ('<=', <Name.c l.1 at 0x7f23b2e9e390>)]
     """
 
     _astroid_fields = ("left", "ops")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.left: Optional[NodeNG] = None
-        """The value at the left being applied to a comparison operator."""
+    left: NodeNG
+    """The value at the left being applied to a comparison operator."""
 
-        self.ops: typing.List[typing.Tuple[str, NodeNG]] = []
-        """The remainder of the operators and their relevant right hand value."""
+    ops: list[tuple[str, NodeNG]]
+    """The remainder of the operators and their relevant right hand value."""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(
-        self,
-        left: Optional[NodeNG] = None,
-        ops: Optional[typing.List[typing.Tuple[str, NodeNG]]] = None,
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param left: The value at the left being applied to a comparison
-            operator.
-
-        :param ops: The remainder of the operators
-            and their relevant right hand value.
-        """
+    def postinit(self, left: NodeNG, ops: list[tuple[str, NodeNG]]) -> None:
         self.left = left
-        if ops is not None:
-            self.ops = ops
+        self.ops = ops
 
     def get_children(self):
         """Get the child nodes below this node.
 
         Overridden to handle the tuple fields and skip returning the operator
         strings.
 
@@ -1812,77 +1488,53 @@
 
     _astroid_fields = ("target", "iter", "ifs")
     _other_fields = ("is_async",)
 
     optional_assign = True
     """Whether this node optionally assigns a variable."""
 
-    lineno: None
-    col_offset: None
-    end_lineno: None
-    end_col_offset: None
-
-    def __init__(self, parent: Optional[NodeNG] = None) -> None:
-        """
-        :param parent: The parent node in the syntax tree.
-        """
-        self.target: Optional[NodeNG] = None
-        """What is assigned to by the comprehension."""
-
-        self.iter: Optional[NodeNG] = None
-        """What is iterated over by the comprehension."""
+    target: NodeNG
+    """What is assigned to by the comprehension."""
 
-        self.ifs: typing.List[NodeNG] = []
-        """The contents of any if statements that filter the comprehension."""
+    iter: NodeNG
+    """What is iterated over by the comprehension."""
 
-        self.is_async: Optional[bool] = None
-        """Whether this is an asynchronous comprehension or not."""
+    ifs: list[NodeNG]
+    """The contents of any if statements that filter the comprehension."""
 
-        super().__init__(parent=parent)
+    is_async: bool
+    """Whether this is an asynchronous comprehension or not."""
 
-    # pylint: disable=redefined-builtin; same name as builtin ast module.
     def postinit(
         self,
-        target: Optional[NodeNG] = None,
-        iter: Optional[NodeNG] = None,
-        ifs: Optional[typing.List[NodeNG]] = None,
-        is_async: Optional[bool] = None,
+        target: NodeNG,
+        iter: NodeNG,  # pylint: disable = redefined-builtin
+        ifs: list[NodeNG],
+        is_async: bool,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param target: What is assigned to by the comprehension.
-
-        :param iter: What is iterated over by the comprehension.
-
-        :param ifs: The contents of any if statements that filter
-            the comprehension.
-
-        :param is_async: Whether this is an asynchronous comprehension or not.
-        """
         self.target = target
         self.iter = iter
-        if ifs is not None:
-            self.ifs = ifs
+        self.ifs = ifs
         self.is_async = is_async
 
-    assigned_stmts: AssignedStmtsCall["Comprehension"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[Comprehension]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def assign_type(self):
         """The type of assignment that this node performs.
 
         :returns: The assignment type.
         :rtype: NodeNG
         """
         return self
 
     def _get_filtered_stmts(
-        self, lookup_node, node, stmts, mystmt: Optional[Statement]
+        self, lookup_node, node, stmts, mystmt: _base_nodes.Statement | None
     ):
         """method used in filter_stmts"""
         if self is mystmt:
             if isinstance(lookup_node, (Const, Name)):
                 return [lookup_node], True
 
         elif self.statement(future=True) is mystmt:
@@ -1896,15 +1548,15 @@
     def get_children(self):
         yield self.target
         yield self.iter
 
         yield from self.ifs
 
 
-class Const(mixins.NoChildrenMixin, NodeNG, Instance):
+class Const(_base_nodes.NoChildrenNode, Instance):
     """Class representing any constant including num, str, bool, None, bytes.
 
     >>> import astroid
     >>> node = astroid.extract_node('(5, "This is a string.", True, None, b"bytes")')
     >>> node
     <Tuple.tuple l.1 at 0x7f23b2e358d0>
     >>> list(node.get_children())
@@ -1915,22 +1567,22 @@
     <Const.bytes l.1 at 0x7f23b2e35a20>]
     """
 
     _other_fields = ("value", "kind")
 
     def __init__(
         self,
-        value: typing.Any,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        kind: Optional[str] = None,
+        value: Any,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
+        kind: str | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param value: The value that the constant represents.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -1941,40 +1593,45 @@
         :param kind: The string prefix. "u" for u-prefixed strings and ``None`` otherwise. Python 3.8+ only.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.value: typing.Any = value
+        self.value: Any = value
         """The value that the constant represents."""
 
-        self.kind: Optional[str] = kind  # can be None
+        self.kind: str | None = kind  # can be None
         """"The string prefix. "u" for u-prefixed strings and ``None`` otherwise. Python 3.8+ only."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
+        Instance.__init__(self, None)
+
+    infer_unary_op: ClassVar[InferUnaryOp[Const]]
+    infer_binary_op: ClassVar[InferBinaryOp[Const]]
+
     def __getattr__(self, name):
         # This is needed because of Proxy's __getattr__ method.
         # Calling object.__new__ on this class without calling
         # __init__ would result in an infinite loop otherwise
         # since __getattr__ is called when an attribute doesn't
         # exist and self._proxied indirectly calls self.value
         # and Proxy __getattr__ calls self.value
         if name == "value":
             raise AttributeError
         return super().__getattr__(name)
 
-    def getitem(self, index, context=None):
+    def getitem(self, index, context: InferenceContext | None = None):
         """Get an item from this node if subscriptable.
 
         :param index: The node to use as a subscript index.
         :type index: Const or Slice
 
         :raises AstroidTypeError: When the given index cannot be used as a
             subscript index, or if this node is not subscriptable.
@@ -1988,35 +1645,37 @@
             raise AstroidTypeError(
                 f"Could not use type {type(index)} as subscript index"
             )
 
         try:
             if isinstance(self.value, (str, bytes)):
                 return Const(self.value[index_value])
+        except ValueError as exc:
+            raise AstroidValueError(
+                f"Could not index {self.value!r} with {index_value!r}"
+            ) from exc
         except IndexError as exc:
             raise AstroidIndexError(
                 message="Index {index!r} out of range",
                 node=self,
                 index=index,
                 context=context,
             ) from exc
         except TypeError as exc:
             raise AstroidTypeError(
                 message="Type error {error!r}", node=self, index=index, context=context
             ) from exc
 
         raise AstroidTypeError(f"{self!r} (value={self.value})")
 
-    def has_dynamic_getattr(self):
+    def has_dynamic_getattr(self) -> bool:
         """Check if the node has a custom __getattr__ or __getattribute__.
 
-        :returns: True if the class has a custom
-            __getattr__ or __getattribute__, False otherwise.
+        :returns: Whether the class has a custom __getattr__ or __getattribute__.
             For a :class:`Const` this is always ``False``.
-        :rtype: bool
         """
         return False
 
     def itered(self):
         """An iterator over the elements this node contains.
 
         :returns: The contents of this node.
@@ -2024,32 +1683,31 @@
 
         :raises TypeError: If this node does not represent something that is iterable.
         """
         if isinstance(self.value, str):
             return [const_factory(elem) for elem in self.value]
         raise TypeError(f"Cannot iterate over type {type(self.value)!r}")
 
-    def pytype(self):
+    def pytype(self) -> str:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return self._proxied.qname()
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
         :rtype: bool
         """
         return bool(self.value)
 
 
-class Continue(mixins.NoChildrenMixin, Statement):
+class Continue(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Continue` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('continue')
     >>> node
     <Continue l.1 at 0x7f23b2e35588>
     """
@@ -2071,59 +1729,21 @@
     <FunctionDef.my_property l.2 at 0x7f23b2e35d30>
     >>> list(node.get_children())[0]
     <Decorators l.1 at 0x7f23b2e35d68>
     """
 
     _astroid_fields = ("nodes",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.nodes: typing.List[NodeNG]
-        """The decorators that this node contains.
-
-        :type: list(Name or Call) or None
-        """
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(self, nodes: typing.List[NodeNG]) -> None:
-        """Do some setup after initialisation.
+    nodes: list[NodeNG]
+    """The decorators that this node contains."""
 
-        :param nodes: The decorators that this node contains.
-        :type nodes: list(Name or Call)
-        """
+    def postinit(self, nodes: list[NodeNG]) -> None:
         self.nodes = nodes
 
-    def scope(self) -> "LocalsDictNodeNG":
+    def scope(self) -> LocalsDictNodeNG:
         """The first parent node defining a new scope.
         These can be Module, FunctionDef, ClassDef, Lambda, or GeneratorExp nodes.
 
         :returns: The first parent scope node.
         """
         # skip the function node to go directly to the upper level scope
         if not self.parent:
@@ -2132,136 +1752,94 @@
             raise ParentMissingError(target=self.parent)
         return self.parent.parent.scope()
 
     def get_children(self):
         yield from self.nodes
 
 
-class DelAttr(mixins.ParentAssignTypeMixin, NodeNG):
+class DelAttr(_base_nodes.ParentAssignNode):
     """Variation of :class:`ast.Delete` representing deletion of an attribute.
 
     >>> import astroid
     >>> node = astroid.extract_node('del self.attr')
     >>> node
     <Delete l.1 at 0x7f23b2e35f60>
     >>> list(node.get_children())[0]
     <DelAttr.attr l.1 at 0x7f23b2e411d0>
     """
 
     _astroid_fields = ("expr",)
     _other_fields = ("attrname",)
 
-    @decorators.deprecate_default_argument_values(attrname="str")
+    expr: NodeNG
+    """The name that this node represents."""
+
     def __init__(
         self,
-        attrname: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        attrname: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param attrname: The name of the attribute that is being deleted.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.expr: Optional[NodeNG] = None
-        """The name that this node represents.
-
-        :type: Name or None
-        """
-
-        self.attrname: Optional[str] = attrname
+        self.attrname = attrname
         """The name of the attribute that is being deleted."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, expr: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param expr: The name that this node represents.
-        :type expr: Name or None
-        """
+    def postinit(self, expr: NodeNG) -> None:
         self.expr = expr
 
     def get_children(self):
         yield self.expr
 
 
-class Delete(mixins.AssignTypeMixin, Statement):
+class Delete(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Delete` node.
 
     A :class:`Delete` is a ``del`` statement this is deleting something.
 
     >>> import astroid
     >>> node = astroid.extract_node('del self.attr')
     >>> node
     <Delete l.1 at 0x7f23b2e35f60>
     """
 
     _astroid_fields = ("targets",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.targets: typing.List[NodeNG] = []
+        self.targets: list[NodeNG] = []
         """What is being deleted."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, targets: Optional[typing.List[NodeNG]] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param targets: What is being deleted.
-        """
-        if targets is not None:
-            self.targets = targets
+    def postinit(self, targets: list[NodeNG]) -> None:
+        self.targets = targets
 
     def get_children(self):
         yield from self.targets
 
 
 class Dict(NodeNG, Instance):
     """Class representing an :class:`ast.Dict` node.
@@ -2274,52 +1852,58 @@
     <Dict.dict l.1 at 0x7f23b2e35cc0>
     """
 
     _astroid_fields = ("items",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.items: typing.List[typing.Tuple[NodeNG, NodeNG]] = []
+        self.items: list[
+            tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]
+        ] = []
         """The key-value pairs contained in the dictionary."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, items: typing.List[typing.Tuple[NodeNG, NodeNG]]) -> None:
+    def postinit(
+        self, items: list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]]
+    ) -> None:
         """Do some setup after initialisation.
 
         :param items: The key-value pairs contained in the dictionary.
         """
         self.items = items
 
+    infer_unary_op: ClassVar[InferUnaryOp[Dict]]
+
     @classmethod
     def from_elements(cls, items=None):
         """Create a :class:`Dict` of constants from a live dictionary.
 
         :param items: The items to store in the node.
         :type items: dict
 
@@ -2334,19 +1918,18 @@
                 (const_factory(k), const_factory(v) if _is_const(v) else v)
                 for k, v in items.items()
                 # The keys need to be constants
                 if _is_const(k)
             ]
         return node
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.dict"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.dict"
 
     def get_children(self):
         """Get the key and value nodes below this node.
 
         Children are returned in the order that they are defined in the source
@@ -2373,51 +1956,60 @@
         """An iterator over the keys this node contains.
 
         :returns: The keys of this node.
         :rtype: iterable(NodeNG)
         """
         return [key for (key, _) in self.items]
 
-    def getitem(self, index, context=None):
+    def getitem(
+        self, index: Const | Slice, context: InferenceContext | None = None
+    ) -> NodeNG:
         """Get an item from this node.
 
         :param index: The node to use as a subscript index.
-        :type index: Const or Slice
 
         :raises AstroidTypeError: When the given index cannot be used as a
             subscript index, or if this node is not subscriptable.
         :raises AstroidIndexError: If the given index does not exist in the
             dictionary.
         """
+        # pylint: disable-next=import-outside-toplevel; circular import
+        from astroid.helpers import safe_infer
+
         for key, value in self.items:
             # TODO(cpopa): no support for overriding yet, {1:2, **{1: 3}}.
             if isinstance(key, DictUnpack):
+                inferred_value = safe_infer(value, context)
+                if not isinstance(inferred_value, Dict):
+                    continue
+
                 try:
-                    return value.getitem(index, context)
+                    return inferred_value.getitem(index, context)
                 except (AstroidTypeError, AstroidIndexError):
                     continue
+
             for inferredkey in key.infer(context):
-                if inferredkey is util.Uninferable:
+                if isinstance(inferredkey, util.UninferableBase):
                     continue
                 if isinstance(inferredkey, Const) and isinstance(index, Const):
                     if inferredkey.value == index.value:
                         return value
 
         raise AstroidIndexError(index)
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
         :rtype: bool
         """
         return bool(self.items)
 
 
-class Expr(Statement):
+class Expr(_base_nodes.Statement):
     """Class representing an :class:`ast.Expr` node.
 
     An :class:`Expr` is any expression that does not have its value used or
     stored.
 
     >>> import astroid
     >>> node = astroid.extract_node('method()')
@@ -2425,79 +2017,67 @@
     <Call l.1 at 0x7f23b2e352b0>
     >>> node.parent
     <Expr l.1 at 0x7f23b2e35278>
     """
 
     _astroid_fields = ("value",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None
-        """What the expression does."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
+    value: NodeNG
+    """What the expression does."""
 
-        :param value: What the expression does.
-        """
+    def postinit(self, value: NodeNG) -> None:
         self.value = value
 
     def get_children(self):
         yield self.value
 
     def _get_yield_nodes_skip_lambdas(self):
         if not self.value.is_lambda:
             yield from self.value._get_yield_nodes_skip_lambdas()
 
 
-class Ellipsis(mixins.NoChildrenMixin, NodeNG):  # pylint: disable=redefined-builtin
+class Ellipsis(_base_nodes.NoChildrenNode):  # pylint: disable=redefined-builtin
     """Class representing an :class:`ast.Ellipsis` node.
 
     An :class:`Ellipsis` is the ``...`` syntax.
 
     Deprecated since v2.6.0 - Use :class:`Const` instead.
     Will be removed with the release v2.7.0
     """
 
 
-class EmptyNode(mixins.NoChildrenMixin, NodeNG):
+class EmptyNode(_base_nodes.NoChildrenNode):
     """Holds an arbitrary object in the :attr:`LocalsDictNodeNG.locals`."""
 
     object = None
 
+    def __init__(
+        self,
+        lineno: None = None,
+        col_offset: None = None,
+        parent: None = None,
+        *,
+        end_lineno: None = None,
+        end_col_offset: None = None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def has_underlying_object(self) -> bool:
+        return self.object is not None and self.object is not _EMPTY_OBJECT_MARKER
+
 
-class ExceptHandler(mixins.MultiLineBlockMixin, mixins.AssignTypeMixin, Statement):
+class ExceptHandler(
+    _base_nodes.MultiLineBlockNode, _base_nodes.AssignTypeNode, _base_nodes.Statement
+):
     """Class representing an :class:`ast.ExceptHandler`. node.
 
     An :class:`ExceptHandler` is an ``except`` block on a try-except.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
         try:
@@ -2510,104 +2090,60 @@
     >>> node.handlers
     [<ExceptHandler l.4 at 0x7f23b2e9e860>]
     """
 
     _astroid_fields = ("type", "name", "body")
     _multi_line_block_fields = ("body",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
+    type: NodeNG | None
+    """The types that the block handles."""
 
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.type: Optional[NodeNG] = None  # can be None
-        """The types that the block handles.
+    name: AssignName | None
+    """The name that the caught exception is assigned to."""
 
-        :type: Tuple or NodeNG or None
-        """
+    body: list[NodeNG]
+    """The contents of the block."""
 
-        self.name: Optional[AssignName] = None  # can be None
-        """The name that the caught exception is assigned to."""
-
-        self.body: typing.List[NodeNG] = []
-        """The contents of the block."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    assigned_stmts: AssignedStmtsCall["ExceptHandler"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[ExceptHandler]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
+    def postinit(
+        self,
+        type: NodeNG | None,  # pylint: disable = redefined-builtin
+        name: AssignName | None,
+        body: list[NodeNG],
+    ) -> None:
+        self.type = type
+        self.name = name
+        self.body = body
+
     def get_children(self):
         if self.type is not None:
             yield self.type
 
         if self.name is not None:
             yield self.name
 
         yield from self.body
 
-    # pylint: disable=redefined-builtin; had to use the same name as builtin ast module.
-    def postinit(
-        self,
-        type: Optional[NodeNG] = None,
-        name: Optional[AssignName] = None,
-        body: Optional[typing.List[NodeNG]] = None,
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param type: The types that the block handles.
-        :type type: Tuple or NodeNG or None
-
-        :param name: The name that the caught exception is assigned to.
-
-        :param body:The contents of the block.
-        """
-        self.type = type
-        self.name = name
-        if body is not None:
-            self.body = body
-
-    @decorators.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         if self.name:
             return self.name.tolineno
         if self.type:
             return self.type.tolineno
         return self.lineno
 
-    def catch(self, exceptions: Optional[typing.List[str]]) -> bool:
+    def catch(self, exceptions: list[str] | None) -> bool:
         """Check if this node handles any of the given
 
         :param exceptions: The names of the exceptions to check for.
         """
         if self.type is None or exceptions is None:
             return True
         return any(node.name in exceptions for node in self.type._get_name_nodes())
@@ -2620,18 +2156,17 @@
 
     Deprecated since v2.6.0 - Now part of the :class:`Subscript` node.
     Will be removed with the release of v2.7.0
     """
 
 
 class For(
-    mixins.MultiLineBlockMixin,
-    mixins.BlockRangeMixIn,
-    mixins.AssignTypeMixin,
-    Statement,
+    _base_nodes.MultiLineWithElseBlockNode,
+    _base_nodes.AssignTypeNode,
+    _base_nodes.Statement,
 ):
     """Class representing an :class:`ast.For` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('for thing in things: print(thing)')
     >>> node
     <For l.1 at 0x7f23b2e8cf28>
@@ -2643,92 +2178,49 @@
 
     optional_assign = True
     """Whether this node optionally assigns a variable.
 
     This is always ``True`` for :class:`For` nodes.
     """
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
+    target: NodeNG
+    """What the loop assigns to."""
 
-        :param col_offset: The column that this node appears on in the
-            source code.
+    iter: NodeNG
+    """What the loop iterates over."""
 
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.target: Optional[NodeNG] = None
-        """What the loop assigns to."""
-
-        self.iter: Optional[NodeNG] = None
-        """What the loop iterates over."""
-
-        self.body: typing.List[NodeNG] = []
-        """The contents of the body of the loop."""
+    body: list[NodeNG]
+    """The contents of the body of the loop."""
 
-        self.orelse: typing.List[NodeNG] = []
-        """The contents of the ``else`` block of the loop."""
+    orelse: list[NodeNG]
+    """The contents of the ``else`` block of the loop."""
 
-        self.type_annotation: Optional[NodeNG] = None  # can be None
-        """If present, this will contain the type annotation passed by a type comment"""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    type_annotation: NodeNG | None
+    """If present, this will contain the type annotation passed by a type comment"""
 
-    # pylint: disable=redefined-builtin; had to use the same name as builtin ast module.
     def postinit(
         self,
-        target: Optional[NodeNG] = None,
-        iter: Optional[NodeNG] = None,
-        body: Optional[typing.List[NodeNG]] = None,
-        orelse: Optional[typing.List[NodeNG]] = None,
-        type_annotation: Optional[NodeNG] = None,
+        target: NodeNG,
+        iter: NodeNG,  # pylint: disable = redefined-builtin
+        body: list[NodeNG],
+        orelse: list[NodeNG],
+        type_annotation: NodeNG | None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param target: What the loop assigns to.
-
-        :param iter: What the loop iterates over.
-
-        :param body: The contents of the body of the loop.
-
-        :param orelse: The contents of the ``else`` block of the loop.
-        """
         self.target = target
         self.iter = iter
-        if body is not None:
-            self.body = body
-        if orelse is not None:
-            self.orelse = orelse
+        self.body = body
+        self.orelse = orelse
         self.type_annotation = type_annotation
 
-    assigned_stmts: AssignedStmtsCall["For"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[For]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    @decorators.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         return self.iter.tolineno
 
@@ -2775,80 +2267,46 @@
     <Expr l.3 at 0x7f23b2e419e8>
     >>> list(node.body[0].get_children())[0]
     <Await l.3 at 0x7f23b2e41a20>
     """
 
     _astroid_fields = ("value",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None
-        """What to wait for."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
+    value: NodeNG
+    """What to wait for."""
 
-        :param value: What to wait for.
-        """
+    def postinit(self, value: NodeNG) -> None:
         self.value = value
 
     def get_children(self):
         yield self.value
 
 
-class ImportFrom(mixins.NoChildrenMixin, mixins.ImportFromMixin, Statement):
+class ImportFrom(_base_nodes.ImportNode):
     """Class representing an :class:`ast.ImportFrom` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('from my_package import my_module')
     >>> node
     <ImportFrom l.1 at 0x7f23b2e415c0>
     """
 
     _other_fields = ("modname", "names", "level")
 
     def __init__(
         self,
-        fromname: Optional[str],
-        names: typing.List[typing.Tuple[str, Optional[str]]],
-        level: Optional[int] = 0,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        fromname: str | None,
+        names: list[tuple[str, str | None]],
+        level: int | None = 0,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param fromname: The module that is being imported from.
 
         :param names: What is being imported from the module.
 
         :param level: The level of relative import.
@@ -2861,29 +2319,29 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.modname: Optional[str] = fromname  # can be None
+        self.modname: str | None = fromname  # can be None
         """The module that is being imported from.
 
         This is ``None`` for relative imports.
         """
 
-        self.names: typing.List[typing.Tuple[str, Optional[str]]] = names
+        self.names: list[tuple[str, str | None]] = names
         """What is being imported from the module.
 
         Each entry is a :class:`tuple` of the name being imported,
         and the alias that the name is assigned to (if any).
         """
 
         # TODO When is 'level' None?
-        self.level: Optional[int] = level  # can be None
+        self.level: int | None = level  # can be None
         """The level of relative import.
 
         Essentially this is the number of dots in the import.
         This is always 0 for absolute imports.
         """
 
         super().__init__(
@@ -2897,89 +2355,65 @@
 
 class Attribute(NodeNG):
     """Class representing an :class:`ast.Attribute` node."""
 
     _astroid_fields = ("expr",)
     _other_fields = ("attrname",)
 
-    @decorators.deprecate_default_argument_values(attrname="str")
+    expr: NodeNG
+    """The name that this node represents."""
+
     def __init__(
         self,
-        attrname: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        attrname: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param attrname: The name of the attribute.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.expr: Optional[NodeNG] = None
-        """The name that this node represents.
-
-        :type: Name or None
-        """
-
-        self.attrname: Optional[str] = attrname
+        self.attrname = attrname
         """The name of the attribute."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, expr: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param expr: The name that this node represents.
-        :type expr: Name or None
-        """
+    def postinit(self, expr: NodeNG) -> None:
         self.expr = expr
 
     def get_children(self):
         yield self.expr
 
 
-class Global(mixins.NoChildrenMixin, Statement):
+class Global(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Global` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('global a_global')
     >>> node
     <Global l.1 at 0x7f23b2e9de10>
     """
 
     _other_fields = ("names",)
 
     def __init__(
         self,
-        names: typing.List[str],
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        names: list[str],
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param names: The names being declared as global.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -2988,122 +2422,70 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.names: typing.List[str] = names
+        self.names: list[str] = names
         """The names being declared as global."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def _infer_name(self, frame, name):
         return name
 
 
-class If(mixins.MultiLineBlockMixin, mixins.BlockRangeMixIn, Statement):
+class If(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.If` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('if condition: print(True)')
     >>> node
     <If l.1 at 0x7f23b2e9dd30>
     """
 
     _astroid_fields = ("test", "body", "orelse")
     _multi_line_block_fields = ("body", "orelse")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.test: Optional[NodeNG] = None
-        """The condition that the statement tests."""
-
-        self.body: typing.List[NodeNG] = []
-        """The contents of the block."""
+    test: NodeNG
+    """The condition that the statement tests."""
 
-        self.orelse: typing.List[NodeNG] = []
-        """The contents of the ``else`` block."""
+    body: list[NodeNG]
+    """The contents of the block."""
 
-        self.is_orelse: bool = False
-        """Whether the if-statement is the orelse-block of another if statement."""
+    orelse: list[NodeNG]
+    """The contents of the ``else`` block."""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(
-        self,
-        test: Optional[NodeNG] = None,
-        body: Optional[typing.List[NodeNG]] = None,
-        orelse: Optional[typing.List[NodeNG]] = None,
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param test: The condition that the statement tests.
-
-        :param body: The contents of the block.
-
-        :param orelse: The contents of the ``else`` block.
-        """
+    def postinit(self, test: NodeNG, body: list[NodeNG], orelse: list[NodeNG]) -> None:
         self.test = test
-        if body is not None:
-            self.body = body
-        if orelse is not None:
-            self.orelse = orelse
-        if isinstance(self.parent, If) and self in self.parent.orelse:
-            self.is_orelse = True
+        self.body = body
+        self.orelse = orelse
 
-    @decorators.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         return self.test.tolineno
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: The line number to start the range at.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
             starting at the given line number.
-        :rtype: tuple(int, int)
         """
         if lineno == self.body[0].fromlineno:
             return lineno, lineno
         if lineno <= self.body[-1].tolineno:
             return lineno, self.body[-1].tolineno
         return self._elsed_block_range(lineno, self.orelse, self.body[0].fromlineno - 1)
 
@@ -3136,14 +2518,15 @@
         True
         """
         warnings.warn(
             "The 'is_sys_guard' function is deprecated and will be removed in astroid 3.0.0 "
             "It has been moved to pylint and can be imported from 'pylint.checkers.utils' "
             "starting with pylint 2.12",
             DeprecationWarning,
+            stacklevel=2,
         )
         if isinstance(self.test, Compare):
             value = self.test.left
             if isinstance(value, Subscript):
                 value = value.value
             if isinstance(value, Attribute) and value.as_string() == "sys.version_info":
                 return True
@@ -3163,14 +2546,15 @@
         True
         """
         warnings.warn(
             "The 'is_typing_guard' function is deprecated and will be removed in astroid 3.0.0 "
             "It has been moved to pylint and can be imported from 'pylint.checkers.utils' "
             "starting with pylint 2.12",
             DeprecationWarning,
+            stacklevel=2,
         )
         return isinstance(
             self.test, (Name, Attribute)
         ) and self.test.as_string().endswith("TYPE_CHECKING")
 
 
 class IfExp(NodeNG):
@@ -3179,102 +2563,59 @@
     >>> node = astroid.extract_node('value if condition else other')
     >>> node
     <IfExp l.1 at 0x7f23b2e9dbe0>
     """
 
     _astroid_fields = ("test", "body", "orelse")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
+    test: NodeNG
+    """The condition that the statement tests."""
 
-        :param end_lineno: The last line this node appears on in the source code.
+    body: NodeNG
+    """The contents of the block."""
 
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.test: Optional[NodeNG] = None
-        """The condition that the statement tests."""
+    orelse: NodeNG
+    """The contents of the ``else`` block."""
 
-        self.body: Optional[NodeNG] = None
-        """The contents of the block."""
-
-        self.orelse: Optional[NodeNG] = None
-        """The contents of the ``else`` block."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(
-        self,
-        test: Optional[NodeNG] = None,
-        body: Optional[NodeNG] = None,
-        orelse: Optional[NodeNG] = None,
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param test: The condition that the statement tests.
-
-        :param body: The contents of the block.
-
-        :param orelse: The contents of the ``else`` block.
-        """
+    def postinit(self, test: NodeNG, body: NodeNG, orelse: NodeNG) -> None:
         self.test = test
         self.body = body
         self.orelse = orelse
 
     def get_children(self):
         yield self.test
         yield self.body
         yield self.orelse
 
-    def op_left_associative(self):
+    def op_left_associative(self) -> Literal[False]:
         # `1 if True else 2 if False else 3` is parsed as
         # `1 if True else (2 if False else 3)`
         return False
 
 
-class Import(mixins.NoChildrenMixin, mixins.ImportFromMixin, Statement):
+class Import(_base_nodes.ImportNode):
     """Class representing an :class:`ast.Import` node.
     >>> import astroid
     >>> node = astroid.extract_node('import astroid')
     >>> node
     <Import l.1 at 0x7f23b2e4e5c0>
     """
 
     _other_fields = ("names",)
 
     @decorators.deprecate_default_argument_values(names="list[tuple[str, str | None]]")
     def __init__(
         self,
-        names: Optional[typing.List[typing.Tuple[str, Optional[str]]]] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        names: list[tuple[str, str | None]] | None = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param names: The names being imported.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -3283,15 +2624,15 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.names: typing.List[typing.Tuple[str, Optional[str]]] = names or []
+        self.names: list[tuple[str, str | None]] = names or []
         """The names being imported.
 
         Each entry is a :class:`tuple` of the name being imported,
         and the alias that the name is assigned to (if any).
         """
 
         super().__init__(
@@ -3323,58 +2664,39 @@
     >>> node.keywords
     [<Keyword l.1 at 0x7f23b2e9e9b0>]
     """
 
     _astroid_fields = ("value",)
     _other_fields = ("arg",)
 
+    value: NodeNG
+    """The value being assigned to the keyword argument."""
+
     def __init__(
         self,
-        arg: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        arg: str | None,
+        lineno: int | None,
+        col_offset: int | None,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param arg: The argument being assigned to.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.arg: Optional[str] = arg  # can be None
+        self.arg = arg
         """The argument being assigned to."""
 
-        self.value: Optional[NodeNG] = None
-        """The value being assigned to the keyword argument."""
-
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param value: The value being assigned to the keyword argument.
-        """
+    def postinit(self, value: NodeNG) -> None:
         self.value = value
 
     def get_children(self):
         yield self.value
 
 
 class List(BaseContainer):
@@ -3386,21 +2708,21 @@
     <List.list l.1 at 0x7f23b2e9e128>
     """
 
     _other_fields = ("ctx",)
 
     def __init__(
         self,
-        ctx: Optional[Context] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        ctx: Context | None = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param ctx: Whether the list is assigned to or loaded from.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -3409,48 +2731,50 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.ctx: Optional[Context] = ctx
+        self.ctx: Context | None = ctx
         """Whether the list is assigned to or loaded from."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: AssignedStmtsCall["List"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[List]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    def pytype(self):
+    infer_unary_op: ClassVar[InferUnaryOp[List]]
+    infer_binary_op: ClassVar[InferBinaryOp[List]]
+
+    def pytype(self) -> Literal["builtins.list"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.list"
 
-    def getitem(self, index, context=None):
+    def getitem(self, index, context: InferenceContext | None = None):
         """Get an item from this node.
 
         :param index: The node to use as a subscript index.
         :type index: Const or Slice
         """
         return _container_getitem(self, self.elts, index, context=context)
 
 
-class Nonlocal(mixins.NoChildrenMixin, Statement):
+class Nonlocal(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Nonlocal` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     def function():
         nonlocal var
     ''')
@@ -3460,21 +2784,21 @@
     <Nonlocal l.3 at 0x7f23b2e9e908>
     """
 
     _other_fields = ("names",)
 
     def __init__(
         self,
-        names: typing.List[str],
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        names: list[str],
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param names: The names being declared as not local.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -3483,106 +2807,68 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.names: typing.List[str] = names
+        self.names: list[str] = names
         """The names being declared as not local."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def _infer_name(self, frame, name):
         return name
 
 
-class Pass(mixins.NoChildrenMixin, Statement):
+class Pass(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Pass` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('pass')
     >>> node
     <Pass l.1 at 0x7f23b2e9e748>
     """
 
 
-class Raise(Statement):
+class Raise(_base_nodes.Statement):
     """Class representing an :class:`ast.Raise` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('raise RuntimeError("Something bad happened!")')
     >>> node
     <Raise l.1 at 0x7f23b2e9e828>
     """
 
     _astroid_fields = ("exc", "cause")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.exc: Optional[NodeNG] = None  # can be None
-        """What is being raised."""
-
-        self.cause: Optional[NodeNG] = None  # can be None
-        """The exception being used to raise this one."""
+    exc: NodeNG | None
+    """What is being raised."""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    cause: NodeNG | None
+    """The exception being used to raise this one."""
 
     def postinit(
         self,
-        exc: Optional[NodeNG] = None,
-        cause: Optional[NodeNG] = None,
+        exc: NodeNG | None,
+        cause: NodeNG | None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param exc: What is being raised.
-
-        :param cause: The exception being used to raise this one.
-        """
         self.exc = exc
         self.cause = cause
 
-    def raises_not_implemented(self):
+    def raises_not_implemented(self) -> bool:
         """Check if this node raises a :class:`NotImplementedError`.
 
-        :returns: True if this node raises a :class:`NotImplementedError`,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether this node raises a :class:`NotImplementedError`.
         """
         if not self.exc:
             return False
         return any(
             name.name == "NotImplementedError" for name in self.exc._get_name_nodes()
         )
 
@@ -3590,63 +2876,29 @@
         if self.exc is not None:
             yield self.exc
 
         if self.cause is not None:
             yield self.cause
 
 
-class Return(Statement):
+class Return(_base_nodes.Statement):
     """Class representing an :class:`ast.Return` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('return True')
     >>> node
     <Return l.1 at 0x7f23b8211908>
     """
 
     _astroid_fields = ("value",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None  # can be None
-        """The value being returned."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
+    value: NodeNG | None
+    """The value being returned."""
 
-        :param value: The value being returned.
-        """
+    def postinit(self, value: NodeNG | None) -> None:
         self.value = value
 
     def get_children(self):
         if self.value is not None:
             yield self.value
 
     def is_tuple_return(self):
@@ -3661,19 +2913,20 @@
 
     >>> import astroid
     >>> node = astroid.extract_node('{1, 2, 3}')
     >>> node
     <Set.set l.1 at 0x7f23b2e71d68>
     """
 
-    def pytype(self):
+    infer_unary_op: ClassVar[InferUnaryOp[Set]]
+
+    def pytype(self) -> Literal["builtins.set"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.set"
 
 
 class Slice(NodeNG):
     """Class representing an :class:`ast.Slice` node.
 
@@ -3683,183 +2936,125 @@
     <Subscript l.1 at 0x7f23b2e71f60>
     >>> node.slice
     <Slice l.1 at 0x7f23b2e71e80>
     """
 
     _astroid_fields = ("lower", "upper", "step")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
+    lower: NodeNG | None
+    """The lower index in the slice."""
 
-        :param col_offset: The column that this node appears on in the
-            source code.
+    upper: NodeNG | None
+    """The upper index in the slice."""
 
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.lower: Optional[NodeNG] = None  # can be None
-        """The lower index in the slice."""
-
-        self.upper: Optional[NodeNG] = None  # can be None
-        """The upper index in the slice."""
-
-        self.step: Optional[NodeNG] = None  # can be None
-        """The step to take between indexes."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    step: NodeNG | None
+    """The step to take between indexes."""
 
     def postinit(
         self,
-        lower: Optional[NodeNG] = None,
-        upper: Optional[NodeNG] = None,
-        step: Optional[NodeNG] = None,
+        lower: NodeNG | None,
+        upper: NodeNG | None,
+        step: NodeNG | None,
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param lower: The lower index in the slice.
-
-        :param upper: The upper index in the slice.
-
-        :param step: The step to take between index.
-        """
         self.lower = lower
         self.upper = upper
         self.step = step
 
     def _wrap_attribute(self, attr):
         """Wrap the empty attributes of the Slice in a Const node."""
         if not attr:
             const = const_factory(attr)
             const.parent = self
             return const
         return attr
 
-    @decorators.cachedproperty
-    def _proxied(self):
+    @cached_property
+    def _proxied(self) -> nodes.ClassDef:
         builtins = AstroidManager().builtins_module
         return builtins.getattr("slice")[0]
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.slice"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.slice"
 
-    def igetattr(self, attrname, context=None):
+    def igetattr(
+        self, attrname: str, context: InferenceContext | None = None
+    ) -> Iterator[SuccessfulInferenceResult]:
         """Infer the possible values of the given attribute on the slice.
 
         :param attrname: The name of the attribute to infer.
-        :type attrname: str
 
         :returns: The inferred possible values.
-        :rtype: iterable(NodeNG)
         """
         if attrname == "start":
             yield self._wrap_attribute(self.lower)
         elif attrname == "stop":
             yield self._wrap_attribute(self.upper)
         elif attrname == "step":
             yield self._wrap_attribute(self.step)
         else:
             yield from self.getattr(attrname, context=context)
 
-    def getattr(self, attrname, context=None):
+    def getattr(self, attrname, context: InferenceContext | None = None):
         return self._proxied.getattr(attrname, context)
 
     def get_children(self):
         if self.lower is not None:
             yield self.lower
 
         if self.upper is not None:
             yield self.upper
 
         if self.step is not None:
             yield self.step
 
 
-class Starred(mixins.ParentAssignTypeMixin, NodeNG):
+class Starred(_base_nodes.ParentAssignNode):
     """Class representing an :class:`ast.Starred` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('*args')
     >>> node
     <Starred l.1 at 0x7f23b2e41978>
     """
 
     _astroid_fields = ("value",)
     _other_fields = ("ctx",)
 
+    value: NodeNG
+    """What is being unpacked."""
+
     def __init__(
         self,
-        ctx: Optional[Context] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        ctx: Context,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param ctx: Whether the list is assigned to or loaded from.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None
-        """What is being unpacked."""
-
-        self.ctx: Optional[Context] = ctx
+        self.ctx = ctx
         """Whether the starred item is assigned to or loaded from."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param value: What is being unpacked.
-        """
+    def postinit(self, value: NodeNG) -> None:
         self.value = value
 
-    assigned_stmts: AssignedStmtsCall["Starred"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[Starred]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.value
 
@@ -3872,75 +3067,54 @@
     >>> node
     <Subscript l.1 at 0x7f23b2e71f60>
     """
 
     _astroid_fields = ("value", "slice")
     _other_fields = ("ctx",)
 
+    infer_lhs: ClassVar[InferLHS[Subscript]]
+
+    value: NodeNG
+    """What is being indexed."""
+
+    slice: NodeNG
+    """The slice being used to lookup."""
+
     def __init__(
         self,
-        ctx: Optional[Context] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        ctx: Context,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param ctx: Whether the subscripted item is assigned to or loaded from.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None
-        """What is being indexed."""
-
-        self.slice: Optional[NodeNG] = None
-        """The slice being used to lookup."""
-
-        self.ctx: Optional[Context] = ctx
+        self.ctx = ctx
         """Whether the subscripted item is assigned to or loaded from."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     # pylint: disable=redefined-builtin; had to use the same name as builtin ast module.
-    def postinit(
-        self, value: Optional[NodeNG] = None, slice: Optional[NodeNG] = None
-    ) -> None:
-        """Do some setup after initialisation.
-
-        :param value: What is being indexed.
-
-        :param slice: The slice being used to lookup.
-        """
+    def postinit(self, value: NodeNG, slice: NodeNG) -> None:
         self.value = value
         self.slice = slice
 
     def get_children(self):
         yield self.value
         yield self.slice
 
 
-class TryExcept(mixins.MultiLineBlockMixin, mixins.BlockRangeMixIn, Statement):
+class TryExcept(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.TryExcept` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
         try:
             do_something()
         except Exception as error:
@@ -3949,86 +3123,43 @@
     >>> node
     <TryExcept l.2 at 0x7f23b2e9d908>
     """
 
     _astroid_fields = ("body", "handlers", "orelse")
     _multi_line_block_fields = ("body", "handlers", "orelse")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.body: typing.List[NodeNG] = []
-        """The contents of the block to catch exceptions from."""
-
-        self.handlers: typing.List[ExceptHandler] = []
-        """The exception handlers."""
+    body: list[NodeNG]
+    """The contents of the block to catch exceptions from."""
 
-        self.orelse: typing.List[NodeNG] = []
-        """The contents of the ``else`` block."""
+    handlers: list[ExceptHandler]
+    """The exception handlers."""
 
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    orelse: list[NodeNG]
+    """The contents of the ``else`` block."""
 
     def postinit(
         self,
-        body: Optional[typing.List[NodeNG]] = None,
-        handlers: Optional[typing.List[ExceptHandler]] = None,
-        orelse: Optional[typing.List[NodeNG]] = None,
+        body: list[NodeNG],
+        handlers: list[ExceptHandler],
+        orelse: list[NodeNG],
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param body: The contents of the block to catch exceptions from.
-
-        :param handlers: The exception handlers.
-
-        :param orelse: The contents of the ``else`` block.
-        """
-        if body is not None:
-            self.body = body
-        if handlers is not None:
-            self.handlers = handlers
-        if orelse is not None:
-            self.orelse = orelse
+        self.body = body
+        self.handlers = handlers
+        self.orelse = orelse
 
     def _infer_name(self, frame, name):
         return name
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: The line number to start the range at.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
             starting at the given line number.
-        :rtype: tuple(int, int)
         """
         last = None
         for exhandler in self.handlers:
             if exhandler.type and lineno == exhandler.type.fromlineno:
                 return lineno, lineno
             if exhandler.body[0].fromlineno <= lineno <= exhandler.body[-1].tolineno:
                 return lineno, exhandler.body[-1].tolineno
@@ -4039,15 +3170,15 @@
     def get_children(self):
         yield from self.body
 
         yield from self.handlers or ()
         yield from self.orelse or ()
 
 
-class TryFinally(mixins.MultiLineBlockMixin, mixins.BlockRangeMixIn, Statement):
+class TryFinally(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.TryFinally` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     try:
         do_something()
     except Exception as error:
@@ -4060,73 +3191,71 @@
     """
 
     _astroid_fields = ("body", "finalbody")
     _multi_line_block_fields = ("body", "finalbody")
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.body: typing.Union[typing.List[TryExcept], typing.List[NodeNG]] = []
+        self.body: list[NodeNG | TryExcept] = []
         """The try-except that the finally is attached to."""
 
-        self.finalbody: typing.List[NodeNG] = []
+        self.finalbody: list[NodeNG] = []
         """The contents of the ``finally`` block."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
-        body: typing.Union[typing.List[TryExcept], typing.List[NodeNG], None] = None,
-        finalbody: Optional[typing.List[NodeNG]] = None,
+        body: list[NodeNG | TryExcept] | None = None,
+        finalbody: list[NodeNG] | None = None,
     ) -> None:
         """Do some setup after initialisation.
 
         :param body: The try-except that the finally is attached to.
 
         :param finalbody: The contents of the ``finally`` block.
         """
         if body is not None:
             self.body = body
         if finalbody is not None:
             self.finalbody = finalbody
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: The line number to start the range at.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
             starting at the given line number.
-        :rtype: tuple(int, int)
         """
         child = self.body[0]
         # py2.5 try: except: finally:
         if (
             isinstance(child, TryExcept)
             and child.fromlineno == self.fromlineno
             and child.tolineno >= lineno > self.fromlineno
@@ -4135,34 +3264,135 @@
         return self._elsed_block_range(lineno, self.finalbody)
 
     def get_children(self):
         yield from self.body
         yield from self.finalbody
 
 
+class TryStar(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
+    """Class representing an :class:`ast.TryStar` node."""
+
+    _astroid_fields = ("body", "handlers", "orelse", "finalbody")
+    _multi_line_block_fields = ("body", "handlers", "orelse", "finalbody")
+
+    def __init__(
+        self,
+        *,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
+        parent: NodeNG | None = None,
+    ) -> None:
+        """
+        :param lineno: The line that this node appears on in the source code.
+        :param col_offset: The column that this node appears on in the
+            source code.
+        :param parent: The parent node in the syntax tree.
+        :param end_lineno: The last line this node appears on in the source code.
+        :param end_col_offset: The end column this node appears on in the
+            source code. Note: This is after the last symbol.
+        """
+        self.body: list[NodeNG] = []
+        """The contents of the block to catch exceptions from."""
+
+        self.handlers: list[ExceptHandler] = []
+        """The exception handlers."""
+
+        self.orelse: list[NodeNG] = []
+        """The contents of the ``else`` block."""
+
+        self.finalbody: list[NodeNG] = []
+        """The contents of the ``finally`` block."""
+
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def postinit(
+        self,
+        *,
+        body: list[NodeNG] | None = None,
+        handlers: list[ExceptHandler] | None = None,
+        orelse: list[NodeNG] | None = None,
+        finalbody: list[NodeNG] | None = None,
+    ) -> None:
+        """Do some setup after initialisation.
+        :param body: The contents of the block to catch exceptions from.
+        :param handlers: The exception handlers.
+        :param orelse: The contents of the ``else`` block.
+        :param finalbody: The contents of the ``finally`` block.
+        """
+        if body:
+            self.body = body
+        if handlers:
+            self.handlers = handlers
+        if orelse:
+            self.orelse = orelse
+        if finalbody:
+            self.finalbody = finalbody
+
+    def _infer_name(self, frame, name):
+        return name
+
+    def block_range(self, lineno: int) -> tuple[int, int]:
+        """Get a range from a given line number to where this node ends."""
+        if lineno == self.fromlineno:
+            return lineno, lineno
+        if self.body and self.body[0].fromlineno <= lineno <= self.body[-1].tolineno:
+            # Inside try body - return from lineno till end of try body
+            return lineno, self.body[-1].tolineno
+        for exhandler in self.handlers:
+            if exhandler.type and lineno == exhandler.type.fromlineno:
+                return lineno, lineno
+            if exhandler.body[0].fromlineno <= lineno <= exhandler.body[-1].tolineno:
+                return lineno, exhandler.body[-1].tolineno
+        if self.orelse:
+            if self.orelse[0].fromlineno - 1 == lineno:
+                return lineno, lineno
+            if self.orelse[0].fromlineno <= lineno <= self.orelse[-1].tolineno:
+                return lineno, self.orelse[-1].tolineno
+        if self.finalbody:
+            if self.finalbody[0].fromlineno - 1 == lineno:
+                return lineno, lineno
+            if self.finalbody[0].fromlineno <= lineno <= self.finalbody[-1].tolineno:
+                return lineno, self.finalbody[-1].tolineno
+        return lineno, self.tolineno
+
+    def get_children(self):
+        yield from self.body
+        yield from self.handlers
+        yield from self.orelse
+        yield from self.finalbody
+
+
 class Tuple(BaseContainer):
     """Class representing an :class:`ast.Tuple` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('(1, 2, 3)')
     >>> node
     <Tuple.tuple l.1 at 0x7f23b2e41780>
     """
 
     _other_fields = ("ctx",)
 
     def __init__(
         self,
-        ctx: Optional[Context] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        ctx: Context | None = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param ctx: Whether the tuple is assigned to or loaded from.
 
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
@@ -4171,39 +3401,41 @@
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.ctx: Optional[Context] = ctx
+        self.ctx: Context | None = ctx
         """Whether the tuple is assigned to or loaded from."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: AssignedStmtsCall["Tuple"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[Tuple]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    def pytype(self):
+    infer_unary_op: ClassVar[InferUnaryOp[Tuple]]
+    infer_binary_op: ClassVar[InferBinaryOp[Tuple]]
+
+    def pytype(self) -> Literal["builtins.tuple"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.tuple"
 
-    def getitem(self, index, context=None):
+    def getitem(self, index, context: InferenceContext | None = None):
         """Get an item from this node.
 
         :param index: The node to use as a subscript index.
         :type index: Const or Slice
         """
         return _container_getitem(self, self.elts, index, context=context)
 
@@ -4216,66 +3448,47 @@
     >>> node
     <UnaryOp l.1 at 0x7f23b2e4e198>
     """
 
     _astroid_fields = ("operand",)
     _other_fields = ("op",)
 
-    @decorators.deprecate_default_argument_values(op="str")
+    operand: NodeNG
+    """What the unary operator is applied to."""
+
     def __init__(
         self,
-        op: Optional[str] = None,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        op: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param op: The operator.
-
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.op: Optional[str] = op
+        self.op = op
         """The operator."""
 
-        self.operand: Optional[NodeNG] = None
-        """What the unary operator is applied to."""
-
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, operand: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
-
-        :param operand: What the unary operator is applied to.
-        """
+    def postinit(self, operand: NodeNG) -> None:
         self.operand = operand
 
     # This is set by inference.py
-    def _infer_unaryop(self, context=None):
-        raise NotImplementedError
+    _infer_unaryop: ClassVar[
+        InferBinaryOperation[UnaryOp, util.BadUnaryOperationMessage]
+    ]
 
-    def type_errors(self, context=None):
+    def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
         Each TypeError is represented by a :class:`BadBinaryOperationMessage`,
         which holds the original exception.
 
         :returns: The list of possible type errors.
         :rtype: list(BadBinaryOperationMessage)
@@ -4296,105 +3509,63 @@
     def op_precedence(self):
         if self.op == "not":
             return OP_PRECEDENCE[self.op]
 
         return super().op_precedence()
 
 
-class While(mixins.MultiLineBlockMixin, mixins.BlockRangeMixIn, Statement):
+class While(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.While` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     while condition():
         print("True")
     ''')
     >>> node
     <While l.2 at 0x7f23b2e4e390>
     """
 
     _astroid_fields = ("test", "body", "orelse")
     _multi_line_block_fields = ("body", "orelse")
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
+    test: NodeNG
+    """The condition that the loop tests."""
 
-        :param col_offset: The column that this node appears on in the
-            source code.
+    body: list[NodeNG]
+    """The contents of the loop."""
 
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.test: Optional[NodeNG] = None
-        """The condition that the loop tests."""
-
-        self.body: typing.List[NodeNG] = []
-        """The contents of the loop."""
-
-        self.orelse: typing.List[NodeNG] = []
-        """The contents of the ``else`` block."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
+    orelse: list[NodeNG]
+    """The contents of the ``else`` block."""
 
     def postinit(
         self,
-        test: Optional[NodeNG] = None,
-        body: Optional[typing.List[NodeNG]] = None,
-        orelse: Optional[typing.List[NodeNG]] = None,
+        test: NodeNG,
+        body: list[NodeNG],
+        orelse: list[NodeNG],
     ) -> None:
-        """Do some setup after initialisation.
-
-        :param test: The condition that the loop tests.
-
-        :param body: The contents of the loop.
-
-        :param orelse: The contents of the ``else`` block.
-        """
         self.test = test
-        if body is not None:
-            self.body = body
-        if orelse is not None:
-            self.orelse = orelse
+        self.body = body
+        self.orelse = orelse
 
-    @decorators.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         return self.test.tolineno
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: The line number to start the range at.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
             starting at the given line number.
-        :rtype: tuple(int, int)
         """
         return self._elsed_block_range(lineno, self.orelse)
 
     def get_children(self):
         yield self.test
 
         yield from self.body
@@ -4403,18 +3574,17 @@
     def _get_yield_nodes_skip_lambdas(self):
         """A While node can contain a Yield node in the test"""
         yield from self.test._get_yield_nodes_skip_lambdas()
         yield from super()._get_yield_nodes_skip_lambdas()
 
 
 class With(
-    mixins.MultiLineBlockMixin,
-    mixins.BlockRangeMixIn,
-    mixins.AssignTypeMixin,
-    Statement,
+    _base_nodes.MultiLineWithElseBlockNode,
+    _base_nodes.AssignTypeNode,
+    _base_nodes.Statement,
 ):
     """Class representing an :class:`ast.With` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     with open(file_path) as file_:
         print(file_.read())
@@ -4425,76 +3595,76 @@
 
     _astroid_fields = ("items", "body")
     _other_other_fields = ("type_annotation",)
     _multi_line_block_fields = ("body",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.items: typing.List[typing.Tuple[NodeNG, Optional[NodeNG]]] = []
+        self.items: list[tuple[NodeNG, NodeNG | None]] = []
         """The pairs of context managers and the names they are assigned to."""
 
-        self.body: typing.List[NodeNG] = []
+        self.body: list[NodeNG] = []
         """The contents of the ``with`` block."""
 
-        self.type_annotation: Optional[NodeNG] = None  # can be None
+        self.type_annotation: NodeNG | None = None  # can be None
         """If present, this will contain the type annotation passed by a type comment"""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
-        items: Optional[typing.List[typing.Tuple[NodeNG, Optional[NodeNG]]]] = None,
-        body: Optional[typing.List[NodeNG]] = None,
-        type_annotation: Optional[NodeNG] = None,
+        items: list[tuple[NodeNG, NodeNG | None]] | None = None,
+        body: list[NodeNG] | None = None,
+        type_annotation: NodeNG | None = None,
     ) -> None:
         """Do some setup after initialisation.
 
         :param items: The pairs of context managers and the names
             they are assigned to.
 
         :param body: The contents of the ``with`` block.
         """
         if items is not None:
             self.items = items
         if body is not None:
             self.body = body
         self.type_annotation = type_annotation
 
-    assigned_stmts: AssignedStmtsCall["With"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[With]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    @decorators.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         return self.items[-1][0].tolineno
 
@@ -4522,67 +3692,33 @@
     >>> node = astroid.extract_node('yield True')
     >>> node
     <Yield l.1 at 0x7f23b2e4e5f8>
     """
 
     _astroid_fields = ("value",)
 
-    def __init__(
-        self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.value: Optional[NodeNG] = None  # can be None
-        """The value to yield."""
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-    def postinit(self, value: Optional[NodeNG] = None) -> None:
-        """Do some setup after initialisation.
+    value: NodeNG | None
+    """The value to yield."""
 
-        :param value: The value to yield.
-        """
+    def postinit(self, value: NodeNG | None) -> None:
         self.value = value
 
     def get_children(self):
         if self.value is not None:
             yield self.value
 
     def _get_yield_nodes_skip_lambdas(self):
         yield self
 
 
 class YieldFrom(Yield):  # TODO value is required, not optional
     """Class representing an :class:`ast.YieldFrom` node."""
 
 
-class DictUnpack(mixins.NoChildrenMixin, NodeNG):
+class DictUnpack(_base_nodes.NoChildrenNode):
     """Represents the unpacking of dicts into dicts using :pep:`448`."""
 
 
 class FormattedValue(NodeNG):
     """Class representing an :class:`ast.FormattedValue` node.
 
     Represents a :pep:`498` format string.
@@ -4596,20 +3732,20 @@
     """
 
     _astroid_fields = ("value", "format_spec")
     _other_fields = ("conversion",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
@@ -4619,43 +3755,42 @@
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
         self.value: NodeNG
         """The value to be formatted into the string."""
 
-        self.conversion: Optional[int] = None  # can be None
+        self.conversion: int
         """The type of formatting to be applied to the value.
 
         .. seealso::
             :class:`ast.FormattedValue`
         """
 
-        self.format_spec: Optional[NodeNG] = None  # can be None
+        self.format_spec: JoinedStr | None = None
         """The formatting to be applied to the value.
 
         .. seealso::
             :class:`ast.FormattedValue`
-
-        :type: JoinedStr or None
         """
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
+        *,
         value: NodeNG,
-        conversion: Optional[int] = None,
-        format_spec: Optional[NodeNG] = None,
+        conversion: int,
+        format_spec: JoinedStr | None = None,
     ) -> None:
         """Do some setup after initialisation.
 
         :param value: The value to be formatted into the string.
 
         :param conversion: The type of formatting to be applied to the value.
 
@@ -4682,63 +3817,63 @@
     <JoinedStr l.1 at 0x7f23b2e4ed30>
     """
 
     _astroid_fields = ("values",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.values: typing.List[NodeNG] = []
+        self.values: list[NodeNG] = []
         """The string expressions to be joined.
 
         :type: list(FormattedValue or Const)
         """
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, values: Optional[typing.List[NodeNG]] = None) -> None:
+    def postinit(self, values: list[NodeNG] | None = None) -> None:
         """Do some setup after initialisation.
 
         :param value: The string expressions to be joined.
 
         :type: list(FormattedValue or Const)
         """
         if values is not None:
             self.values = values
 
     def get_children(self):
         yield from self.values
 
 
-class NamedExpr(mixins.AssignTypeMixin, NodeNG):
+class NamedExpr(_base_nodes.AssignTypeNode):
     """Represents the assignment from the assignment expression
 
     >>> import astroid
     >>> module = astroid.parse('if a := 1: pass')
     >>> module.body[0].test
     <NamedExpr l.1 at 0x7f23b2e4ed30>
     """
@@ -4748,20 +3883,20 @@
     optional_assign = True
     """Whether this node optionally assigns a variable.
 
     Since NamedExpr are not always called they do not always assign."""
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
@@ -4789,22 +3924,22 @@
             parent=parent,
         )
 
     def postinit(self, target: NodeNG, value: NodeNG) -> None:
         self.target = target
         self.value = value
 
-    assigned_stmts: AssignedStmtsCall["NamedExpr"]
+    assigned_stmts: ClassVar[AssignedStmtsCall[NamedExpr]]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def frame(
         self, *, future: Literal[None, True] = None
-    ) -> Union["nodes.FunctionDef", "nodes.Module", "nodes.ClassDef", "nodes.Lambda"]:
+    ) -> nodes.FunctionDef | nodes.Module | nodes.ClassDef | nodes.Lambda:
         """The first parent frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         or :class:`ClassDef`.
 
         :returns: The first parent frame node.
         """
@@ -4817,15 +3952,15 @@
                 raise ParentMissingError(target=self.parent)
             if not self.parent.parent.parent:
                 raise ParentMissingError(target=self.parent.parent)
             return self.parent.parent.parent.frame(future=True)
 
         return self.parent.frame(future=True)
 
-    def scope(self) -> "LocalsDictNodeNG":
+    def scope(self) -> LocalsDictNodeNG:
         """The first parent node defining a new scope.
         These can be Module, FunctionDef, ClassDef, Lambda, or GeneratorExp nodes.
 
         :returns: The first parent scope node.
         """
         if not self.parent:
             raise ParentMissingError(target=self)
@@ -4836,41 +3971,58 @@
                 raise ParentMissingError(target=self.parent)
             if not self.parent.parent.parent:
                 raise ParentMissingError(target=self.parent.parent)
             return self.parent.parent.parent.scope()
 
         return self.parent.scope()
 
-    def set_local(self, name: str, stmt: AssignName) -> None:
+    def set_local(self, name: str, stmt: NodeNG) -> None:
         """Define that the given name is declared in the given statement node.
         NamedExpr's in Arguments, Keyword or Comprehension are evaluated in their
         parent's parent scope. So we add to their frame's locals.
 
         .. seealso:: :meth:`scope`
 
         :param name: The name that is being defined.
 
         :param stmt: The statement that defines the given name.
         """
         self.frame(future=True).set_local(name, stmt)
 
 
-class Unknown(mixins.AssignTypeMixin, NodeNG):
+class Unknown(_base_nodes.AssignTypeNode):
     """This node represents a node in a constructed AST where
     introspection is not possible.  At the moment, it's only used in
     the args attribute of FunctionDef nodes where function signature
     introspection failed.
     """
 
     name = "Unknown"
 
-    def qname(self):
+    def __init__(
+        self,
+        lineno: None = None,
+        col_offset: None = None,
+        parent: None = None,
+        *,
+        end_lineno: None = None,
+        end_col_offset: None = None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def qname(self) -> Literal["Unknown"]:
         return "Unknown"
 
-    def _infer(self, context=None, **kwargs):
+    def _infer(self, context: InferenceContext | None = None, **kwargs):
         """Inference on an Unknown node immediately terminates."""
         yield util.Uninferable
 
 
 class EvaluatedObject(NodeNG):
     """Contains an object that has already been inferred
 
@@ -4878,37 +4030,39 @@
     with the resulting class acting as the non-evaluated node.
     """
 
     name = "EvaluatedObject"
     _astroid_fields = ("original",)
     _other_fields = ("value",)
 
-    def __init__(
-        self, original: NodeNG, value: typing.Union[NodeNG, util.Uninferable]
-    ) -> None:
+    def __init__(self, original: NodeNG, value: NodeNG | util.UninferableBase) -> None:
         self.original: NodeNG = original
         """The original node that has already been evaluated"""
 
-        self.value: typing.Union[NodeNG, util.Uninferable] = value
+        self.value: NodeNG | util.UninferableBase = value
         """The inferred value"""
 
         super().__init__(
             lineno=self.original.lineno,
             col_offset=self.original.col_offset,
             parent=self.original.parent,
+            end_lineno=self.original.end_lineno,
+            end_col_offset=self.original.end_col_offset,
         )
 
-    def infer(self, context=None, **kwargs):
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[NodeNG | util.UninferableBase, None, None]:
         yield self.value
 
 
 # Pattern matching #######################################################
 
 
-class Match(Statement):
+class Match(_base_nodes.Statement, _base_nodes.MultiLineBlockNode):
     """Class representing a :class:`ast.Match` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     match x:
         case 200:
             ...
@@ -4916,49 +4070,50 @@
             ...
     ''')
     >>> node
     <Match l.2 at 0x10c24e170>
     """
 
     _astroid_fields = ("subject", "cases")
+    _multi_line_block_fields = ("cases",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         self.subject: NodeNG
-        self.cases: typing.List["MatchCase"]
+        self.cases: list[MatchCase]
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
         *,
         subject: NodeNG,
-        cases: typing.List["MatchCase"],
+        cases: list[MatchCase],
     ) -> None:
         self.subject = subject
         self.cases = cases
 
 
 class Pattern(NodeNG):
     """Base class for all Pattern nodes."""
 
 
-class MatchCase(mixins.MultiLineBlockMixin, NodeNG):
+class MatchCase(_base_nodes.MultiLineBlockNode):
     """Class representing a :class:`ast.match_case` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     match x:
         case 200:
             ...
@@ -4971,26 +4126,32 @@
     _multi_line_block_fields = ("body",)
 
     lineno: None
     col_offset: None
     end_lineno: None
     end_col_offset: None
 
-    def __init__(self, *, parent: Optional[NodeNG] = None) -> None:
+    def __init__(self, *, parent: NodeNG | None = None) -> None:
         self.pattern: Pattern
-        self.guard: Optional[NodeNG]
-        self.body: typing.List[NodeNG]
-        super().__init__(parent=parent)
+        self.guard: NodeNG | None
+        self.body: list[NodeNG]
+        super().__init__(
+            parent=parent,
+            lineno=None,
+            col_offset=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
 
     def postinit(
         self,
         *,
         pattern: Pattern,
-        guard: Optional[NodeNG],
-        body: typing.List[NodeNG],
+        guard: NodeNG | None,
+        body: list[NodeNG],
     ) -> None:
         self.pattern = pattern
         self.guard = guard
         self.body = body
 
 
 class MatchValue(Pattern):
@@ -5006,20 +4167,20 @@
     <MatchValue l.3 at 0x10c24e200>
     """
 
     _astroid_fields = ("value",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         self.value: NodeNG
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
@@ -5053,19 +4214,19 @@
 
     _other_fields = ("value",)
 
     def __init__(
         self,
         *,
         value: Literal[True, False, None],
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
+        parent: NodeNG | None = None,
     ) -> None:
         self.value = value
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
@@ -5090,35 +4251,35 @@
     <MatchSequence l.5 at 0x10ca80b20>
     """
 
     _astroid_fields = ("patterns",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
-        self.patterns: typing.List[Pattern]
+        self.patterns: list[Pattern]
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, *, patterns: typing.List[Pattern]) -> None:
+    def postinit(self, *, patterns: list[Pattern]) -> None:
         self.patterns = patterns
 
 
-class MatchMapping(mixins.AssignTypeMixin, Pattern):
+class MatchMapping(_base_nodes.AssignTypeNode, Pattern):
     """Class representing a :class:`ast.MatchMapping` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     match x:
         case {1: "Hello", 2: "World", 3: _, **rest}:
             ...
@@ -5127,51 +4288,53 @@
     <MatchMapping l.3 at 0x10c8a8850>
     """
 
     _astroid_fields = ("keys", "patterns", "rest")
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
-        *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
-    ) -> None:
-        self.keys: typing.List[NodeNG]
-        self.patterns: typing.List[Pattern]
-        self.rest: Optional[AssignName]
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
+        *,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
+    ) -> None:
+        self.keys: list[NodeNG]
+        self.patterns: list[Pattern]
+        self.rest: AssignName | None
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
         *,
-        keys: typing.List[NodeNG],
-        patterns: typing.List[Pattern],
-        rest: Optional[AssignName],
+        keys: list[NodeNG],
+        patterns: list[Pattern],
+        rest: AssignName | None,
     ) -> None:
         self.keys = keys
         self.patterns = patterns
         self.rest = rest
 
-    assigned_stmts: Callable[
-        [
-            "MatchMapping",
-            AssignName,
-            Optional[InferenceContext],
-            Literal[None],
-        ],
-        Generator[NodeNG, None, None],
+    assigned_stmts: ClassVar[
+        Callable[
+            [
+                MatchMapping,
+                AssignName,
+                InferenceContext | None,
+                None,
+            ],
+            Generator[NodeNG, None, None],
+        ]
     ]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
 class MatchClass(Pattern):
@@ -5192,48 +4355,48 @@
     """
 
     _astroid_fields = ("cls", "patterns", "kwd_patterns")
     _other_fields = ("kwd_attrs",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
         self.cls: NodeNG
-        self.patterns: typing.List[Pattern]
-        self.kwd_attrs: typing.List[str]
-        self.kwd_patterns: typing.List[Pattern]
+        self.patterns: list[Pattern]
+        self.kwd_attrs: list[str]
+        self.kwd_patterns: list[Pattern]
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
         *,
         cls: NodeNG,
-        patterns: typing.List[Pattern],
-        kwd_attrs: typing.List[str],
-        kwd_patterns: typing.List[Pattern],
+        patterns: list[Pattern],
+        kwd_attrs: list[str],
+        kwd_patterns: list[Pattern],
     ) -> None:
         self.cls = cls
         self.patterns = patterns
         self.kwd_attrs = kwd_attrs
         self.kwd_patterns = kwd_patterns
 
 
-class MatchStar(mixins.AssignTypeMixin, Pattern):
+class MatchStar(_base_nodes.AssignTypeNode, Pattern):
     """Class representing a :class:`ast.MatchStar` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     match x:
         case [1, *_]:
             ...
@@ -5242,48 +4405,50 @@
     <MatchStar l.3 at 0x10ca809a0>
     """
 
     _astroid_fields = ("name",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
-        self.name: Optional[AssignName]
+        self.name: AssignName | None
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, *, name: Optional[AssignName]) -> None:
+    def postinit(self, *, name: AssignName | None) -> None:
         self.name = name
 
-    assigned_stmts: Callable[
-        [
-            "MatchStar",
-            AssignName,
-            Optional[InferenceContext],
-            Literal[None],
-        ],
-        Generator[NodeNG, None, None],
+    assigned_stmts: ClassVar[
+        Callable[
+            [
+                MatchStar,
+                AssignName,
+                InferenceContext | None,
+                None,
+            ],
+            Generator[NodeNG, None, None],
+        ]
     ]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
-class MatchAs(mixins.AssignTypeMixin, Pattern):
+class MatchAs(_base_nodes.AssignTypeNode, Pattern):
     """Class representing a :class:`ast.MatchAs` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     match x:
         case [1, a]:
             ...
@@ -5304,48 +4469,50 @@
     <MatchAs l.9 at 0x10d09b880>
     """
 
     _astroid_fields = ("pattern", "name")
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
-        self.pattern: Optional[Pattern]
-        self.name: Optional[AssignName]
+        self.pattern: Pattern | None
+        self.name: AssignName | None
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
         *,
-        pattern: Optional[Pattern],
-        name: Optional[AssignName],
+        pattern: Pattern | None,
+        name: AssignName | None,
     ) -> None:
         self.pattern = pattern
         self.name = name
 
-    assigned_stmts: Callable[
-        [
-            "MatchAs",
-            AssignName,
-            Optional[InferenceContext],
-            Literal[None],
-        ],
-        Generator[NodeNG, None, None],
+    assigned_stmts: ClassVar[
+        Callable[
+            [
+                MatchAs,
+                AssignName,
+                InferenceContext | None,
+                None,
+            ],
+            Generator[NodeNG, None, None],
+        ]
     ]
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
 class MatchOr(Pattern):
@@ -5361,97 +4528,97 @@
     <MatchOr l.3 at 0x10d0b0b50>
     """
 
     _astroid_fields = ("patterns",)
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional[NodeNG] = None,
+        lineno: int | None = None,
+        col_offset: int | None = None,
+        parent: NodeNG | None = None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None = None,
+        end_col_offset: int | None = None,
     ) -> None:
-        self.patterns: typing.List[Pattern]
+        self.patterns: list[Pattern]
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, *, patterns: typing.List[Pattern]) -> None:
+    def postinit(self, *, patterns: list[Pattern]) -> None:
         self.patterns = patterns
 
 
 # constants ##############################################################
 
-CONST_CLS = {
+# The _proxied attribute of all container types (List, Tuple, etc.)
+# are set during bootstrapping by _astroid_bootstrapping().
+CONST_CLS: dict[type, type[NodeNG]] = {
     list: List,
     tuple: Tuple,
     dict: Dict,
     set: Set,
     type(None): Const,
     type(NotImplemented): Const,
     type(...): Const,
+    bool: Const,
+    int: Const,
+    float: Const,
+    complex: Const,
+    str: Const,
+    bytes: Const,
 }
 
 
-def _update_const_classes():
-    """update constant classes, so the keys of CONST_CLS can be reused"""
-    klasses = (bool, int, float, complex, str, bytes)
-    for kls in klasses:
-        CONST_CLS[kls] = Const
-
-
-_update_const_classes()
-
-
-def _two_step_initialization(cls, value):
-    instance = cls()
-    instance.postinit(value)
-    return instance
-
+def _create_basic_elements(
+    value: Iterable[Any], node: List | Set | Tuple
+) -> list[NodeNG]:
+    """Create a list of nodes to function as the elements of a new node."""
+    elements: list[NodeNG] = []
+    for element in value:
+        element_node = const_factory(element)
+        element_node.parent = node
+        elements.append(element_node)
+    return elements
+
+
+def _create_dict_items(
+    values: Mapping[Any, Any], node: Dict
+) -> list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]]:
+    """Create a list of node pairs to function as the items of a new dict node."""
+    elements: list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]] = []
+    for key, value in values.items():
+        key_node = const_factory(key)
+        key_node.parent = node
+        value_node = const_factory(value)
+        value_node.parent = node
+        elements.append((key_node, value_node))
+    return elements
 
-def _dict_initialization(cls, value):
-    if isinstance(value, dict):
-        value = tuple(value.items())
-    return _two_step_initialization(cls, value)
 
-
-_CONST_CLS_CONSTRUCTORS = {
-    List: _two_step_initialization,
-    Tuple: _two_step_initialization,
-    Dict: _dict_initialization,
-    Set: _two_step_initialization,
-    Const: lambda cls, value: cls(value),
-}
-
-
-def const_factory(value):
-    """return an astroid node for a python value"""
-    # XXX we should probably be stricter here and only consider stuff in
-    # CONST_CLS or do better treatment: in case where value is not in CONST_CLS,
-    # we should rather recall the builder on this value than returning an empty
-    # node (another option being that const_factory shouldn't be called with something
-    # not in CONST_CLS)
+def const_factory(value: Any) -> ConstFactoryResult:
+    """Return an astroid node for a python value."""
     assert not isinstance(value, NodeNG)
 
-    # Hack for ignoring elements of a sequence
-    # or a mapping, in order to avoid transforming
-    # each element to an AST. This is fixed in 2.0
-    # and this approach is a temporary hack.
-    if isinstance(value, (list, set, tuple, dict)):
-        elts = []
-    else:
-        elts = value
-
-    try:
-        initializer_cls = CONST_CLS[value.__class__]
-        initializer = _CONST_CLS_CONSTRUCTORS[initializer_cls]
-        return initializer(initializer_cls, elts)
-    except (KeyError, AttributeError):
+    # This only handles instances of the CONST types. Any
+    # subclasses get inferred as EmptyNode.
+    # TODO: See if we should revisit these with the normal builder.
+    if value.__class__ not in CONST_CLS:
         node = EmptyNode()
         node.object = value
         return node
+
+    instance: List | Set | Tuple | Dict
+    initializer_cls = CONST_CLS[value.__class__]
+    if issubclass(initializer_cls, (List, Set, Tuple)):
+        instance = initializer_cls()
+        instance.postinit(_create_basic_elements(value, instance))
+        return instance
+    if issubclass(initializer_cls, Dict):
+        instance = initializer_cls()
+        instance.postinit(_create_dict_items(value, instance))
+        return instance
+    return Const(value)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/nodes/node_ng.py` & `astroid-3.0.0a1/astroid/nodes/node_ng.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,54 @@
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
+from __future__ import annotations
+
 import pprint
-import sys
-import typing
 import warnings
+from collections.abc import Generator, Iterator
+from functools import cached_property
 from functools import singledispatch as _singledispatch
 from typing import (
     TYPE_CHECKING,
+    Any,
     ClassVar,
-    Iterator,
-    List,
-    Optional,
+    Literal,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-from astroid import decorators, util
+from astroid import util
+from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidError,
     InferenceError,
     ParentMissingError,
     StatementMissing,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 from astroid.nodes.as_string import AsStringVisitor
 from astroid.nodes.const import OP_PRECEDENCE
+from astroid.nodes.utils import Position
+from astroid.typing import InferenceErrorInfo, InferenceResult, InferFn
 
 if TYPE_CHECKING:
     from astroid import nodes
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 
 # Types for 'NodeNG.nodes_of_class()'
-T_Nodes = TypeVar("T_Nodes", bound="NodeNG")
-T_Nodes2 = TypeVar("T_Nodes2", bound="NodeNG")
-T_Nodes3 = TypeVar("T_Nodes3", bound="NodeNG")
+_NodesT = TypeVar("_NodesT", bound="NodeNG")
+_NodesT2 = TypeVar("_NodesT2", bound="NodeNG")
+_NodesT3 = TypeVar("_NodesT3", bound="NodeNG")
 SkipKlassT = Union[None, Type["NodeNG"], Tuple[Type["NodeNG"], ...]]
 
 
 class NodeNG:
     """A node of the new Abstract Syntax Tree (AST).
 
     This is the base class for all Astroid node classes.
@@ -63,66 +66,63 @@
     This is also the case from comprehensions in Python 2.
     """
     is_function: ClassVar[bool] = False  # True for FunctionDef nodes
     """Whether this node indicates a function."""
     is_lambda: ClassVar[bool] = False
 
     # Attributes below are set by the builder module or by raw factories
-    _astroid_fields: ClassVar[typing.Tuple[str, ...]] = ()
+    _astroid_fields: ClassVar[tuple[str, ...]] = ()
     """Node attributes that contain child nodes.
 
     This is redefined in most concrete classes.
     """
-    _other_fields: ClassVar[typing.Tuple[str, ...]] = ()
+    _other_fields: ClassVar[tuple[str, ...]] = ()
     """Node attributes that do not contain child nodes."""
-    _other_other_fields: ClassVar[typing.Tuple[str, ...]] = ()
+    _other_other_fields: ClassVar[tuple[str, ...]] = ()
     """Attributes that contain AST-dependent fields."""
     # instance specific inference function infer(node, context)
-    _explicit_inference = None
+    _explicit_inference: InferFn | None = None
 
     def __init__(
         self,
-        lineno: Optional[int] = None,
-        col_offset: Optional[int] = None,
-        parent: Optional["NodeNG"] = None,
+        lineno: int | None,
+        col_offset: int | None,
+        parent: NodeNG | None,
         *,
-        end_lineno: Optional[int] = None,
-        end_col_offset: Optional[int] = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.lineno: Optional[int] = lineno
+        self.lineno = lineno
         """The line that this node appears on in the source code."""
 
-        self.col_offset: Optional[int] = col_offset
+        self.col_offset = col_offset
         """The column that this node appears on in the source code."""
 
-        self.parent: Optional["NodeNG"] = parent
+        self.parent = parent
         """The parent node in the syntax tree."""
 
-        self.end_lineno: Optional[int] = end_lineno
+        self.end_lineno = end_lineno
         """The last line this node appears on in the source code."""
 
-        self.end_col_offset: Optional[int] = end_col_offset
+        self.end_col_offset = end_col_offset
         """The end column this node appears on in the source code.
+
         Note: This is after the last symbol.
         """
 
-    def infer(self, context=None, **kwargs):
+        self.position: Position | None = None
+        """Position of keyword(s) and name.
+
+        Used as fallback for block nodes which might not provide good
+        enough positional information. E.g. ClassDef, FunctionDef.
+        """
+
+    def infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
         """Get a generator of the inferred values.
 
         This is the main entry point to the inference system.
 
         .. seealso:: :ref:`inference`
 
         If the instance has some explicit inference function set, it will be
@@ -143,54 +143,54 @@
                 yield from results
                 return
             except UseInferenceDefault:
                 pass
 
         if not context:
             # nodes_inferred?
-            yield from self._infer(context, **kwargs)
+            yield from self._infer(context=context, **kwargs)
             return
 
         key = (self, context.lookupname, context.callcontext, context.boundnode)
         if key in context.inferred:
             yield from context.inferred[key]
             return
 
-        generator = self._infer(context, **kwargs)
         results = []
 
         # Limit inference amount to help with performance issues with
         # exponentially exploding possible results.
-        limit = AstroidManager().max_inferable_values
-        for i, result in enumerate(generator):
+        limit = AstroidManager.max_inferable_values
+        for i, result in enumerate(self._infer(context=context, **kwargs)):
             if i >= limit or (context.nodes_inferred > context.max_inferred):
+                results.append(util.Uninferable)
                 yield util.Uninferable
                 break
             results.append(result)
             yield result
             context.nodes_inferred += 1
 
         # Cache generated results for subsequent inferences of the
         # same node using the same context
         context.inferred[key] = tuple(results)
         return
 
-    def _repr_name(self):
+    def _repr_name(self) -> str:
         """Get a name for nice representation.
 
         This is either :attr:`name`, :attr:`attrname`, or the empty string.
 
         :returns: The nice name.
         :rtype: str
         """
         if all(name not in self._astroid_fields for name in ("name", "attrname")):
             return getattr(self, "name", "") or getattr(self, "attrname", "")
         return ""
 
-    def __str__(self):
+    def __str__(self) -> str:
         rname = self._repr_name()
         cname = type(self).__name__
         if rname:
             string = "%(cname)s.%(rname)s(%(fields)s)"
             alignment = len(cname) + len(rname) + 2
         else:
             string = "%(cname)s(%(fields)s)"
@@ -208,15 +208,15 @@
 
         return string % {
             "cname": cname,
             "rname": rname,
             "fields": (",\n" + " " * alignment).join(result),
         }
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         rname = self._repr_name()
         if rname:
             string = "<%(cname)s.%(rname)s l.%(lineno)s at 0x%(id)x>"
         else:
             string = "<%(cname)s l.%(lineno)s at 0x%(id)x>"
         return string % {
             "cname": type(self).__name__,
@@ -226,69 +226,65 @@
         }
 
     def accept(self, visitor):
         """Visit this node using the given visitor."""
         func = getattr(visitor, "visit_" + self.__class__.__name__.lower())
         return func(self)
 
-    def get_children(self) -> Iterator["NodeNG"]:
+    def get_children(self) -> Iterator[NodeNG]:
         """Get the child nodes below this node."""
         for field in self._astroid_fields:
             attr = getattr(self, field)
             if attr is None:
                 continue
             if isinstance(attr, (list, tuple)):
                 yield from attr
             else:
                 yield attr
         yield from ()
 
-    def last_child(self) -> Optional["NodeNG"]:
-        """An optimized version of list(get_children())[-1]"""
+    def last_child(self) -> NodeNG | None:
+        """An optimized version of list(get_children())[-1]."""
         for field in self._astroid_fields[::-1]:
             attr = getattr(self, field)
-            if not attr:  # None or empty listy / tuple
+            if not attr:  # None or empty list / tuple
                 continue
             if isinstance(attr, (list, tuple)):
                 return attr[-1]
             return attr
         return None
 
-    def node_ancestors(self) -> Iterator["NodeNG"]:
+    def node_ancestors(self) -> Iterator[NodeNG]:
         """Yield parent, grandparent, etc until there are no more."""
         parent = self.parent
         while parent is not None:
             yield parent
             parent = parent.parent
 
-    def parent_of(self, node):
+    def parent_of(self, node) -> bool:
         """Check if this node is the parent of the given node.
 
         :param node: The node to check if it is the child.
         :type node: NodeNG
 
-        :returns: True if this node is the parent of the given node,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether this node is the parent of the given node.
         """
         return any(self is parent for parent in node.node_ancestors())
 
     @overload
-    def statement(
-        self, *, future: Literal[None] = ...
-    ) -> Union["nodes.Statement", "nodes.Module"]:
+    def statement(self, *, future: None = ...) -> nodes.Statement | nodes.Module:
         ...
 
     @overload
-    def statement(self, *, future: Literal[True]) -> "nodes.Statement":
+    def statement(self, *, future: Literal[True]) -> nodes.Statement:
         ...
 
     def statement(
         self, *, future: Literal[None, True] = None
-    ) -> Union["nodes.Statement", "nodes.Module"]:
+    ) -> nodes.Statement | nodes.Module:
         """The first parent node, including self, marked as statement node.
 
         TODO: Deprecate the future parameter and only raise StatementMissing and return
         nodes.Statement
 
         :raises AttributeError: If self has no parent attribute
         :raises StatementMissing: If self has no parent attribute and future is True
@@ -300,21 +296,22 @@
                 raise StatementMissing(target=self)
             warnings.warn(
                 "In astroid 3.0.0 NodeNG.statement() will return either a nodes.Statement "
                 "or raise a StatementMissing exception. AttributeError will no longer be raised. "
                 "This behaviour can already be triggered "
                 "by passing 'future=True' to a statement() call.",
                 DeprecationWarning,
+                stacklevel=2,
             )
             raise AttributeError(f"{self} object has no attribute 'parent'")
         return self.parent.statement(future=future)
 
     def frame(
         self, *, future: Literal[None, True] = None
-    ) -> Union["nodes.FunctionDef", "nodes.Module", "nodes.ClassDef", "nodes.Lambda"]:
+    ) -> nodes.FunctionDef | nodes.Module | nodes.ClassDef | nodes.Lambda:
         """The first parent frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The first parent frame node.
         """
@@ -323,38 +320,39 @@
                 raise ParentMissingError(target=self)
             warnings.warn(
                 "In astroid 3.0.0 NodeNG.frame() will return either a Frame node, "
                 "or raise ParentMissingError. AttributeError will no longer be raised. "
                 "This behaviour can already be triggered "
                 "by passing 'future=True' to a frame() call.",
                 DeprecationWarning,
+                stacklevel=2,
             )
             raise AttributeError(f"{self} object has no attribute 'parent'")
 
         return self.parent.frame(future=future)
 
-    def scope(self) -> "nodes.LocalsDictNodeNG":
+    def scope(self) -> nodes.LocalsDictNodeNG:
         """The first parent node defining a new scope.
+
         These can be Module, FunctionDef, ClassDef, Lambda, or GeneratorExp nodes.
 
         :returns: The first parent scope node.
         """
         if not self.parent:
             raise ParentMissingError(target=self)
         return self.parent.scope()
 
-    def root(self):
+    def root(self) -> nodes.Module:
         """Return the root node of the syntax tree.
 
         :returns: The root node.
-        :rtype: Module
         """
         if self.parent:
             return self.parent.root()
-        return self
+        return self  # type: ignore[return-value] # Only 'Module' does not have a parent node.
 
     def child_sequence(self, child):
         """Search for the sequence that contains this child.
 
         :param child: The child node to search sequences for.
         :type child: NodeNG
 
@@ -422,120 +420,126 @@
         :rtype: NodeNG or None
         """
         return self.parent.previous_sibling()
 
     # these are lazy because they're relatively expensive to compute for every
     # single node, and they rarely get looked at
 
-    @decorators.cachedproperty
-    def fromlineno(self) -> Optional[int]:
-        """The first line that this node appears on in the source code."""
+    @cached_property
+    def fromlineno(self) -> int:
+        """The first line that this node appears on in the source code.
+
+        Can also return 0 if the line can not be determined.
+        """
         if self.lineno is None:
             return self._fixed_source_line()
         return self.lineno
 
-    @decorators.cachedproperty
-    def tolineno(self) -> Optional[int]:
-        """The last line that this node appears on in the source code."""
+    @cached_property
+    def tolineno(self) -> int:
+        """The last line that this node appears on in the source code.
+
+        Can also return 0 if the line can not be determined.
+        """
+        if self.end_lineno is not None:
+            return self.end_lineno
         if not self._astroid_fields:
             # can't have children
             last_child = None
         else:
             last_child = self.last_child()
         if last_child is None:
             return self.fromlineno
         return last_child.tolineno
 
-    def _fixed_source_line(self) -> Optional[int]:
+    def _fixed_source_line(self) -> int:
         """Attempt to find the line that this node appears on.
 
         We need this method since not all nodes have :attr:`lineno` set.
+        Will return 0 if the line number can not be determined.
         """
         line = self.lineno
-        _node: Optional[NodeNG] = self
+        _node = self
         try:
             while line is None:
                 _node = next(_node.get_children())
                 line = _node.lineno
         except StopIteration:
-            _node = self.parent
-            while _node and line is None:
-                line = _node.lineno
-                _node = _node.parent
-        return line
+            parent = self.parent
+            while parent and line is None:
+                line = parent.lineno
+                parent = parent.parent
+        return line or 0
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: The line number to start the range at.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
             starting at the given line number.
-        :rtype: tuple(int, int or None)
         """
         return lineno, self.tolineno
 
-    def set_local(self, name, stmt):
+    def set_local(self, name: str, stmt: NodeNG) -> None:
         """Define that the given name is declared in the given statement node.
 
         This definition is stored on the parent scope node.
 
         .. seealso:: :meth:`scope`
 
         :param name: The name that is being defined.
-        :type name: str
 
         :param stmt: The statement that defines the given name.
-        :type stmt: NodeNG
         """
+        assert self.parent
         self.parent.set_local(name, stmt)
 
     @overload
     def nodes_of_class(
         self,
-        klass: Type[T_Nodes],
-        skip_klass: SkipKlassT = None,
-    ) -> Iterator[T_Nodes]:
+        klass: type[_NodesT],
+        skip_klass: SkipKlassT = ...,
+    ) -> Iterator[_NodesT]:
         ...
 
     @overload
     def nodes_of_class(
         self,
-        klass: Tuple[Type[T_Nodes], Type[T_Nodes2]],
-        skip_klass: SkipKlassT = None,
-    ) -> Union[Iterator[T_Nodes], Iterator[T_Nodes2]]:
+        klass: tuple[type[_NodesT], type[_NodesT2]],
+        skip_klass: SkipKlassT = ...,
+    ) -> Iterator[_NodesT] | Iterator[_NodesT2]:
         ...
 
     @overload
     def nodes_of_class(
         self,
-        klass: Tuple[Type[T_Nodes], Type[T_Nodes2], Type[T_Nodes3]],
-        skip_klass: SkipKlassT = None,
-    ) -> Union[Iterator[T_Nodes], Iterator[T_Nodes2], Iterator[T_Nodes3]]:
+        klass: tuple[type[_NodesT], type[_NodesT2], type[_NodesT3]],
+        skip_klass: SkipKlassT = ...,
+    ) -> Iterator[_NodesT] | Iterator[_NodesT2] | Iterator[_NodesT3]:
         ...
 
     @overload
     def nodes_of_class(
         self,
-        klass: Tuple[Type[T_Nodes], ...],
-        skip_klass: SkipKlassT = None,
-    ) -> Iterator[T_Nodes]:
+        klass: tuple[type[_NodesT], ...],
+        skip_klass: SkipKlassT = ...,
+    ) -> Iterator[_NodesT]:
         ...
 
     def nodes_of_class(  # type: ignore[misc] # mypy doesn't correctly recognize the overloads
         self,
-        klass: Union[
-            Type[T_Nodes],
-            Tuple[Type[T_Nodes], Type[T_Nodes2]],
-            Tuple[Type[T_Nodes], Type[T_Nodes2], Type[T_Nodes3]],
-            Tuple[Type[T_Nodes], ...],
-        ],
+        klass: (
+            type[_NodesT]
+            | tuple[type[_NodesT], type[_NodesT2]]
+            | tuple[type[_NodesT], type[_NodesT2], type[_NodesT3]]
+            | tuple[type[_NodesT], ...]
+        ),
         skip_klass: SkipKlassT = None,
-    ) -> Union[Iterator[T_Nodes], Iterator[T_Nodes2], Iterator[T_Nodes3]]:
+    ) -> Iterator[_NodesT] | Iterator[_NodesT2] | Iterator[_NodesT3]:
         """Get the nodes (including this one or below) of the given types.
 
         :param klass: The types of node to search for.
 
         :param skip_klass: The types of node to ignore. This is useful to ignore
             subclasses of :attr:`klass`.
 
@@ -551,34 +555,36 @@
             return
 
         for child_node in self.get_children():
             if isinstance(child_node, skip_klass):
                 continue
             yield from child_node.nodes_of_class(klass, skip_klass)
 
-    @decorators.cached
-    def _get_assign_nodes(self):
+    @cached_property
+    def _assign_nodes_in_scope(self) -> list[nodes.Assign]:
         return []
 
     def _get_name_nodes(self):
         for child_node in self.get_children():
             yield from child_node._get_name_nodes()
 
     def _get_return_nodes_skip_functions(self):
         yield from ()
 
     def _get_yield_nodes_skip_lambdas(self):
         yield from ()
 
     def _infer_name(self, frame, name):
-        # overridden for ImportFrom, Import, Global, TryExcept and Arguments
+        # overridden for ImportFrom, Import, Global, TryExcept, TryStar and Arguments
         pass
 
-    def _infer(self, context=None):
-        """we don't know how to resolve a statement by default"""
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """We don't know how to resolve a statement by default."""
         # this method is overridden by most concrete classes
         raise InferenceError(
             "No inference function for {node!r}.", node=self, context=context
         )
 
     def inferred(self):
         """Get a list of the inferred values.
@@ -598,33 +604,31 @@
             On anything other than a :class:`ClassDef` this will return self.
 
         :returns: An instance of the defined class.
         :rtype: object
         """
         return self
 
-    def has_base(self, node):
+    def has_base(self, node) -> bool:
         """Check if this node inherits from the given type.
 
         :param node: The node defining the base to look for.
             Usually this is a :class:`Name` node.
         :type node: NodeNG
         """
         return False
 
-    def callable(self):
+    def callable(self) -> bool:
         """Whether this node defines something that is callable.
 
-        :returns: True if this defines something that is callable,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether this defines something that is callable.
         """
         return False
 
-    def eq(self, value):
+    def eq(self, value) -> bool:
         return False
 
     def as_string(self) -> str:
         """Get the source code that this node represents."""
         return AsStringVisitor()(self)
 
     def repr_tree(
@@ -677,15 +681,17 @@
             result.extend([cur_indent + line for line in lines[1:]])
             return len(lines) != 1
 
         # pylint: disable=unused-variable,useless-suppression; doesn't understand singledispatch
         @_repr_tree.register(tuple)
         @_repr_tree.register(list)
         def _repr_seq(node, result, done, cur_indent="", depth=1):
-            """Outputs a representation of a sequence that's contained within an AST."""
+            """Outputs a representation of a sequence that's contained within an
+            AST.
+            """
             cur_indent += indent
             result.append("[")
             if not node:
                 broken = False
             elif len(node) == 1:
                 broken = _repr_tree(node[0], result, done, cur_indent, depth)
             elif len(node) == 2:
@@ -742,29 +748,32 @@
                 broken = _repr_tree(
                     getattr(node, fields[0]), result, done, cur_indent, depth
                 )
             else:
                 result.append("\n")
                 result.append(cur_indent)
                 for field in fields[:-1]:
+                    # TODO: Remove this after removal of the 'doc' attribute
+                    if field == "doc":
+                        continue
                     result.append(f"{field}=")
                     _repr_tree(getattr(node, field), result, done, cur_indent, depth)
                     result.append(",\n")
                     result.append(cur_indent)
                 result.append(f"{fields[-1]}=")
                 _repr_tree(getattr(node, fields[-1]), result, done, cur_indent, depth)
                 broken = True
             result.append(")")
             return broken
 
-        result: List[str] = []
+        result: list[str] = []
         _repr_tree(self, result, set())
         return "".join(result)
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         The boolean value of a node can have three
         possible values:
 
             * False: For instance, empty data structures,
               False, empty strings, instances which return
@@ -780,10 +789,10 @@
         """
         return util.Uninferable
 
     def op_precedence(self):
         # Look up by class name or default to highest precedence
         return OP_PRECEDENCE.get(self.__class__.__name__, len(OP_PRECEDENCE))
 
-    def op_left_associative(self):
+    def op_left_associative(self) -> bool:
         # Everything is left associative except `**` and IfExp
         return True
```

### Comparing `astroid-2.9.3/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a1/astroid/nodes/scoped_nodes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
+"""This module contains all classes that are considered a "scoped" node and anything
+related.
 
-"""This module contains all classes that are considered a "scoped" node and anything related.
 A scope node is a node that opens a new local scope in the language definition:
 Module, ClassDef, FunctionDef (and Lambda, GeneratorExp, DictComp and SetComp to some extent).
 """
+
+from astroid.nodes.scoped_nodes.mixin import ComprehensionScope, LocalsDictNodeNG
 from astroid.nodes.scoped_nodes.scoped_nodes import (
     AsyncFunctionDef,
     ClassDef,
-    ComprehensionScope,
     DictComp,
     FunctionDef,
     GeneratorExp,
     Lambda,
     ListComp,
-    LocalsDictNodeNG,
     Module,
     SetComp,
     _is_metaclass,
-    builtin_lookup,
     function_to_method,
     get_wrapping_class,
 )
+from astroid.nodes.scoped_nodes.utils import builtin_lookup
 
 __all__ = (
     "AsyncFunctionDef",
     "ClassDef",
     "ComprehensionScope",
     "DictComp",
     "FunctionDef",
```

### Comparing `astroid-2.9.3/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a1/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,29 @@
-# Copyright (c) 2006-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2010 Daniel Harding <dharding@gmail.com>
-# Copyright (c) 2011, 2013-2015 Google, Inc.
-# Copyright (c) 2013-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2013 Phil Schaf <flying-sheep@web.de>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Florian Bruhin <me@the-compiler.org>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2015 Rene Zhang <rz99@cornell.edu>
-# Copyright (c) 2015 Philip Lorenz <philip@bithub.de>
-# Copyright (c) 2016-2017 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2017-2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2017-2018 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 David Euresti <david@dropbox.com>
-# Copyright (c) 2018-2019, 2021 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Anthony Sottile <asottile@umich.edu>
-# Copyright (c) 2018 HoverHell <hoverhell@gmail.com>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2019 Peter de Blanc <peter@standard.ai>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Peter Kolbus <peter.kolbus@gmail.com>
-# Copyright (c) 2020 Tim Martin <tim@asymptotic.co.uk>
-# Copyright (c) 2020 Ram Rachum <ram@rachum.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Tushar Sadhwani <86737547+tushar-deepsource@users.noreply.github.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Kian Meng, Ang <kianmeng.ang@gmail.com>
-# Copyright (c) 2021 Dmitry Shachnev <mitya57@users.noreply.github.com>
-# Copyright (c) 2021 David Liu <david@cs.toronto.edu>
-# Copyright (c) 2021 pre-commit-ci[bot] <bot@noreply.github.com>
-# Copyright (c) 2021 doranid <ddandd@gmail.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """
 This module contains the classes for "scoped" node, i.e. which are opening a
 new local scope in the language definition : Module, ClassDef, FunctionDef (and
 Lambda, GeneratorExp, DictComp and SetComp to some extent).
 """
-import builtins
+
+from __future__ import annotations
+
 import io
 import itertools
 import os
-import sys
-import typing
 import warnings
-from typing import List, Optional, TypeVar, Union, overload
+from collections.abc import Generator, Iterable, Iterator, Sequence
+from functools import cached_property, lru_cache
+from typing import TYPE_CHECKING, ClassVar, Literal, NoReturn, TypeVar, overload
 
-from astroid import bases
-from astroid import decorators as decorators_mod
-from astroid import mixins, util
-from astroid.const import PY39_PLUS
+from astroid import bases, util
+from astroid.const import IS_PYPY, PY38, PY39_PLUS, PYPY_7_3_11_PLUS
 from astroid.context import (
     CallContext,
     InferenceContext,
     bind_context_to_node,
     copy_context,
 )
 from astroid.exceptions import (
@@ -69,40 +33,34 @@
     DuplicateBasesError,
     InconsistentMroError,
     InferenceError,
     MroError,
     StatementMissing,
     TooManyLevelsError,
 )
-from astroid.filter_statements import _filter_stmts
 from astroid.interpreter.dunder_lookup import lookup
 from astroid.interpreter.objectmodel import ClassModel, FunctionModel, ModuleModel
 from astroid.manager import AstroidManager
-from astroid.nodes import Arguments, Const, node_classes
+from astroid.nodes import Arguments, Const, NodeNG, Unknown, _base_nodes, node_classes
+from astroid.nodes.scoped_nodes.mixin import ComprehensionScope, LocalsDictNodeNG
+from astroid.nodes.scoped_nodes.utils import builtin_lookup
+from astroid.nodes.utils import Position
+from astroid.typing import InferBinaryOp, InferenceResult, SuccessfulInferenceResult
 
-if sys.version_info >= (3, 6, 2):
-    from typing import NoReturn
-else:
-    from typing_extensions import NoReturn
-
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if TYPE_CHECKING:
+    from astroid import nodes
 
 
 ITER_METHODS = ("__iter__", "__getitem__")
 EXCEPTION_BASE_CLASSES = frozenset({"Exception", "BaseException"})
-objects = util.lazy_import("objects")
 BUILTIN_DESCRIPTORS = frozenset(
     {"classmethod", "staticmethod", "builtins.classmethod", "builtins.staticmethod"}
 )
 
-T = TypeVar("T")
+_T = TypeVar("_T")
 
 
 def _c3_merge(sequences, cls, context):
     """Merges MROs in *sequences* to a single MRO using the C3 algorithm.
 
     Adapted from http://www.python.org/download/releases/2.3/mro/.
 
@@ -135,15 +93,15 @@
         # remove the chosen candidate
         for seq in sequences:
             if seq[0] == candidate:
                 del seq[0]
     return None
 
 
-def clean_typing_generic_mro(sequences: List[List["ClassDef"]]) -> None:
+def clean_typing_generic_mro(sequences: list[list[ClassDef]]) -> None:
     """A class can inherit from typing.Generic directly, as base,
     and as base of bases. The merged MRO must however only contain the last entry.
     To prepare for _c3_merge, remove some typing.Generic entries from
     sequences if multiple are present.
 
     This method will check if Generic is in inferred_bases and also
     part of bases_mro. If true, remove it from inferred_bases
@@ -202,345 +160,135 @@
         if n.type == "property":
             return n
         if n.type != "staticmethod":
             return bases.UnboundMethod(n)
     return n
 
 
-def builtin_lookup(name):
-    """lookup a name into the builtin module
-    return the list of matching statements and the astroid for the builtin
-    module
-    """
-    builtin_astroid = AstroidManager().ast_from_module(builtins)
-    if name == "__dict__":
-        return builtin_astroid, ()
-    try:
-        stmts = builtin_astroid.locals[name]
-    except KeyError:
-        stmts = ()
-    return builtin_astroid, stmts
-
-
-# TODO move this Mixin to mixins.py; problem: 'FunctionDef' in _scope_lookup
-class LocalsDictNodeNG(node_classes.LookupMixIn, node_classes.NodeNG):
-    """this class provides locals handling common to Module, FunctionDef
-    and ClassDef nodes, including a dict like interface for direct access
-    to locals information
-    """
-
-    # attributes below are set by the builder module or by raw factories
-
-    locals = {}
-    """A map of the name of a local variable to the node defining the local.
-
-    :type: dict(str, NodeNG)
-    """
-
-    def qname(self):
-        """Get the 'qualified' name of the node.
-
-        For example: module.name, module.class.name ...
-
-        :returns: The qualified name.
-        :rtype: str
-        """
-        # pylint: disable=no-member; github.com/pycqa/astroid/issues/278
-        if self.parent is None:
-            return self.name
-        return f"{self.parent.frame(future=True).qname()}.{self.name}"
-
-    def scope(self: T) -> T:
-        """The first parent node defining a new scope.
-
-        :returns: The first parent scope node.
-        :rtype: Module or FunctionDef or ClassDef or Lambda or GenExpr
-        """
-        return self
-
-    def _scope_lookup(self, node, name, offset=0):
-        """XXX method for interfacing the scope lookup"""
-        try:
-            stmts = _filter_stmts(node, self.locals[name], self, offset)
-        except KeyError:
-            stmts = ()
-        if stmts:
-            return self, stmts
-
-        # Handle nested scopes: since class names do not extend to nested
-        # scopes (e.g., methods), we find the next enclosing non-class scope
-        pscope = self.parent and self.parent.scope()
-        while pscope is not None:
-            if not isinstance(pscope, ClassDef):
-                return pscope.scope_lookup(node, name)
-            pscope = pscope.parent and pscope.parent.scope()
-
-        # self is at the top level of a module, or is enclosed only by ClassDefs
-        return builtin_lookup(name)
-
-    def set_local(self, name, stmt):
-        """Define that the given name is declared in the given statement node.
-
-        .. seealso:: :meth:`scope`
-
-        :param name: The name that is being defined.
-        :type name: str
-
-        :param stmt: The statement that defines the given name.
-        :type stmt: NodeNG
-        """
-        # assert not stmt in self.locals.get(name, ()), (self, stmt)
-        self.locals.setdefault(name, []).append(stmt)
-
-    __setitem__ = set_local
-
-    def _append_node(self, child):
-        """append a child, linking it in the tree"""
-        # pylint: disable=no-member; depending by the class
-        # which uses the current class as a mixin or base class.
-        # It's rewritten in 2.0, so it makes no sense for now
-        # to spend development time on it.
-        self.body.append(child)
-        child.parent = self
-
-    def add_local_node(self, child_node, name=None):
-        """Append a child that should alter the locals of this scope node.
-
-        :param child_node: The child node that will alter locals.
-        :type child_node: NodeNG
-
-        :param name: The name of the local that will be altered by
-            the given child node.
-        :type name: str or None
-        """
-        if name != "__class__":
-            # add __class__ node as a child will cause infinite recursion later!
-            self._append_node(child_node)
-        self.set_local(name or child_node.name, child_node)
-
-    def __getitem__(self, item):
-        """The first node the defines the given local.
-
-        :param item: The name of the locally defined object.
-        :type item: str
-
-        :raises KeyError: If the name is not defined.
-        """
-        return self.locals[item][0]
-
-    def __iter__(self):
-        """Iterate over the names of locals defined in this scoped node.
-
-        :returns: The names of the defined locals.
-        :rtype: iterable(str)
-        """
-        return iter(self.keys())
-
-    def keys(self):
-        """The names of locals defined in this scoped node.
-
-        :returns: The names of the defined locals.
-        :rtype: list(str)
-        """
-        return list(self.locals.keys())
-
-    def values(self):
-        """The nodes that define the locals in this scoped node.
-
-        :returns: The nodes that define locals.
-        :rtype: list(NodeNG)
-        """
-        # pylint: disable=consider-using-dict-items
-        # It look like this class override items/keys/values,
-        # probably not worth the headache
-        return [self[key] for key in self.keys()]
-
-    def items(self):
-        """Get the names of the locals and the node that defines the local.
-
-        :returns: The names of locals and their associated node.
-        :rtype: list(tuple(str, NodeNG))
-        """
-        return list(zip(self.keys(), self.values()))
-
-    def __contains__(self, name):
-        """Check if a local is defined in this scope.
-
-        :param name: The name of the local to check for.
-        :type name: str
-
-        :returns: True if this node has a local of the given name,
-            False otherwise.
-        :rtype: bool
-        """
-        return name in self.locals
-
-
 class Module(LocalsDictNodeNG):
     """Class representing an :class:`ast.Module` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('import astroid')
     >>> node
     <Import l.1 at 0x7f23b2e4e5c0>
     >>> node.parent
     <Module l.0 at 0x7f23b2e4eda0>
     """
 
-    _astroid_fields = ("body",)
-
-    fromlineno = 0
-    """The first line that this node appears on in the source code.
+    _astroid_fields = ("doc_node", "body")
 
-    :type: int or None
-    """
-    lineno: Literal[0] = 0
-    """The line that this node appears on in the source code.
-    """
+    doc_node: Const | None
+    """The doc node associated with this node."""
 
     # attributes below are set by the builder module or by raw factories
 
-    file = None
-    """The path to the file that this ast has been extracted from.
+    file_bytes: str | bytes | None = None
+    """The string/bytes that this ast was built from."""
 
-    This will be ``None`` when the representation has been built from a
-    built-in module.
-
-    :type: str or None
-    """
-    file_bytes = None
-    """The string/bytes that this ast was built from.
-
-    :type: str or bytes or None
-    """
-    file_encoding = None
+    file_encoding: str | None = None
     """The encoding of the source file.
 
     This is used to get unicode out of a source file.
     Python 2 only.
-
-    :type: str or None
-    """
-    name = None
-    """The name of the module.
-
-    :type: str or None
     """
-    pure_python = None
-    """Whether the ast was built from source.
 
-    :type: bool or None
-    """
-    package = None
-    """Whether the node represents a package or a module.
-
-    :type: bool or None
-    """
-    globals = None
-    """A map of the name of a global variable to the node defining the global.
-
-    :type: dict(str, NodeNG)
-    """
-
-    # Future imports
-    future_imports = None
-    """The imports from ``__future__``.
-
-    :type: set(str) or None
-    """
     special_attributes = ModuleModel()
-    """The names of special attributes that this module has.
-
-    :type: objectmodel.ModuleModel
-    """
+    """The names of special attributes that this module has."""
 
     # names of module attributes available through the global scope
     scope_attrs = {"__name__", "__doc__", "__file__", "__path__", "__package__"}
-    """The names of module attributes available through the global scope.
-
-    :type: str(str)
-    """
+    """The names of module attributes available through the global scope."""
 
     _other_fields = (
         "name",
         "doc",
         "file",
         "path",
         "package",
         "pure_python",
         "future_imports",
     )
     _other_other_fields = ("locals", "globals")
 
-    col_offset: None
-    end_lineno: None
-    end_col_offset: None
-    parent: None
-
     def __init__(
         self,
-        name,
-        doc,
-        file=None,
-        path: Optional[List[str]] = None,
-        package=None,
-        parent=None,
-        pure_python=True,
-    ):
-        """
-        :param name: The name of the module.
-        :type name: str
-
-        :param doc: The module docstring.
-        :type doc: str
-
-        :param file: The path to the file that this ast has been extracted from.
-        :type file: str or None
-
-        :param path:
-        :type path: Optional[List[str]]
+        name: str,
+        file: str | None = None,
+        path: Sequence[str] | None = None,
+        package: bool = False,
+        pure_python: bool = True,
+    ) -> None:
+        self.name = name
+        """The name of the module."""
 
-        :param package: Whether the node represents a package or a module.
-        :type package: bool or None
+        self._doc: str | None = None
+        """The module docstring."""
 
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
+        self.file = file
+        """The path to the file that this ast has been extracted from.
 
-        :param pure_python: Whether the ast was built from source.
-        :type pure_python: bool or None
+        This will be ``None`` when the representation has been built from a
+        built-in module.
         """
-        self.name = name
-        self.doc = doc
-        self.file = file
+
         self.path = path
+
         self.package = package
+        """Whether the node represents a package or a module."""
+
         self.pure_python = pure_python
+        """Whether the ast was built from source."""
+
+        self.globals: dict[str, list[SuccessfulInferenceResult]]
+        """A map of the name of a global variable to the node defining the global."""
+
         self.locals = self.globals = {}
-        """A map of the name of a local variable to the node defining the local.
+        """A map of the name of a local variable to the node defining the local."""
 
-        :type: dict(str, NodeNG)
-        """
-        self.body = []
-        """The contents of the module.
+        self.body: list[node_classes.NodeNG] = []
+        """The contents of the module."""
 
-        :type: list(NodeNG) or None
-        """
-        self.future_imports = set()
+        self.future_imports: set[str] = set()
+        """The imports from ``__future__``."""
 
-        super().__init__(lineno=0, parent=parent)
+        super().__init__(
+            lineno=0, parent=None, col_offset=0, end_lineno=None, end_col_offset=None
+        )
 
     # pylint: enable=redefined-builtin
 
-    def postinit(self, body=None):
-        """Do some setup after initialisation.
-
-        :param body: The contents of the module.
-        :type body: list(NodeNG) or None
-        """
+    def postinit(
+        self, body: list[node_classes.NodeNG], *, doc_node: Const | None = None
+    ):
         self.body = body
+        self.doc_node = doc_node
+        if doc_node:
+            self._doc = doc_node.value
+
+    @property
+    def doc(self) -> str | None:
+        """The module docstring."""
+        warnings.warn(
+            "The 'Module.doc' attribute is deprecated, "
+            "use 'Module.doc_node' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._doc
+
+    @doc.setter
+    def doc(self, value: str | None) -> None:
+        warnings.warn(
+            "Setting the 'Module.doc' attribute is deprecated, "
+            "use 'Module.doc_node' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self._doc = value
 
     def _get_stream(self):
         if self.file_bytes is not None:
             return io.BytesIO(self.file_bytes)
         if self.file is not None:
             # pylint: disable=consider-using-with
             stream = open(self.file, "rb")
@@ -550,67 +298,64 @@
     def stream(self):
         """Get a stream to the underlying file or bytes.
 
         :type: file or io.BytesIO or None
         """
         return self._get_stream()
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from where this node starts to where this node ends.
 
         :param lineno: Unused.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to.
-        :rtype: tuple(int, int)
         """
         return self.fromlineno, self.tolineno
 
-    def scope_lookup(self, node, name, offset=0):
+    def scope_lookup(
+        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+    ) -> tuple[LocalsDictNodeNG, list[node_classes.NodeNG]]:
         """Lookup where the given variable is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
-        :type node: NodeNG
 
         :param name: The name of the variable to find assignments for.
-        :type name: str
 
         :param offset: The line offset to filter statements up to.
-        :type offset: int
 
         :returns: This scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
-        :rtype: tuple(str, list(NodeNG))
         """
         if name in self.scope_attrs and name not in self.locals:
             try:
                 return self, self.getattr(name)
             except AttributeInferenceError:
-                return self, ()
+                return self, []
         return self._scope_lookup(node, name, offset)
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.module"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         return "builtins.module"
 
-    def display_type(self):
+    def display_type(self) -> str:
         """A human readable type of this node.
 
         :returns: The type of this node.
         :rtype: str
         """
         return "Module"
 
-    def getattr(self, name, context=None, ignore_locals=False):
+    def getattr(
+        self, name, context: InferenceContext | None = None, ignore_locals=False
+    ):
         if not name:
             raise AttributeInferenceError(target=self, attribute=name, context=context)
 
         result = []
         name_in_locals = name in self.locals
 
         if name in self.special_attributes and not ignore_locals and not name_in_locals:
@@ -625,58 +370,53 @@
                     target=self, attribute=name, context=context
                 ) from exc
         result = [n for n in result if not isinstance(n, node_classes.DelName)]
         if result:
             return result
         raise AttributeInferenceError(target=self, attribute=name, context=context)
 
-    def igetattr(self, name, context=None):
+    def igetattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
         """Infer the possible values of the given variable.
 
         :param name: The name of the variable to infer.
-        :type name: str
 
         :returns: The inferred possible values.
-        :rtype: iterable(NodeNG) or None
         """
         # set lookup name since this is necessary to infer on import nodes for
         # instance
         context = copy_context(context)
         context.lookupname = name
         try:
             return bases._infer_stmts(self.getattr(name, context), context, frame=self)
         except AttributeInferenceError as error:
             raise InferenceError(
                 str(error), target=self, attribute=name, context=context
             ) from error
 
-    def fully_defined(self):
+    def fully_defined(self) -> bool:
         """Check if this module has been build from a .py file.
 
         If so, the module contains a complete representation,
         including the code.
 
-        :returns: True if the module has been built from a .py file.
-        :rtype: bool
+        :returns: Whether the module has been built from a .py file.
         """
         return self.file is not None and self.file.endswith(".py")
 
     @overload
-    def statement(self, *, future: Literal[None] = ...) -> "Module":
+    def statement(self, *, future: None = ...) -> Module:
         ...
 
-    # pylint: disable-next=arguments-differ
-    # https://github.com/PyCQA/pylint/issues/5264
     @overload
     def statement(self, *, future: Literal[True]) -> NoReturn:
         ...
 
-    def statement(
-        self, *, future: Literal[None, True] = None
-    ) -> Union["NoReturn", "Module"]:
+    def statement(self, *, future: Literal[None, True] = None) -> Module | NoReturn:
         """The first parent node, including self, marked as statement node.
 
         When called on a :class:`Module` with the future parameter this raises an error.
 
         TODO: Deprecate the future parameter and only raise StatementMissing
 
         :raises StatementMissing: If no self has no parent attribute and future is True
@@ -685,14 +425,15 @@
             raise StatementMissing(target=self)
         warnings.warn(
             "In astroid 3.0.0 NodeNG.statement() will return either a nodes.Statement "
             "or raise a StatementMissing exception. nodes.Module will no longer be "
             "considered a statement. This behaviour can already be triggered "
             "by passing 'future=True' to a statement() call.",
             DeprecationWarning,
+            stacklevel=2,
         )
         return self
 
     def previous_sibling(self):
         """The previous sibling statement.
 
         :returns: The previous sibling statement node.
@@ -704,51 +445,56 @@
 
         :returns: The next sibling statement node.
         :rtype: NodeNG or None
         """
 
     _absolute_import_activated = True
 
-    def absolute_import_activated(self):
+    def absolute_import_activated(self) -> bool:
         """Whether :pep:`328` absolute import behaviour has been enabled.
 
-        :returns: True if :pep:`328` has been enabled, False otherwise.
-        :rtype: bool
+        :returns: Whether :pep:`328` has been enabled.
         """
         return self._absolute_import_activated
 
-    def import_module(self, modname, relative_only=False, level=None):
+    def import_module(
+        self,
+        modname: str,
+        relative_only: bool = False,
+        level: int | None = None,
+        use_cache: bool = True,
+    ) -> Module:
         """Get the ast for a given module as if imported from this module.
 
         :param modname: The name of the module to "import".
-        :type modname: str
 
         :param relative_only: Whether to only consider relative imports.
-        :type relative_only: bool
 
         :param level: The level of relative import.
-        :type level: int or None
+
+        :param use_cache: Whether to use the astroid_cache of modules.
 
         :returns: The imported module ast.
-        :rtype: NodeNG
         """
         if relative_only and level is None:
             level = 0
         absmodname = self.relative_to_absolute_name(modname, level)
 
         try:
-            return AstroidManager().ast_from_module_name(absmodname)
+            return AstroidManager().ast_from_module_name(
+                absmodname, use_cache=use_cache
+            )
         except AstroidBuildingError:
             # we only want to import a sub module or package of this module,
             # skip here
             if relative_only:
                 raise
         return AstroidManager().ast_from_module_name(modname)
 
-    def relative_to_absolute_name(self, modname: str, level: int) -> str:
+    def relative_to_absolute_name(self, modname: str, level: int | None) -> str:
         """Get the absolute module name for a relative import.
 
         The relative import can be implicit or explicit.
 
         :param modname: The module name to convert.
 
         :param level: The level of relative import.
@@ -823,15 +569,15 @@
         try:
             explicit = next(explicit.infer())
         except (InferenceError, StopIteration):
             return default
         if not isinstance(explicit, (node_classes.Tuple, node_classes.List)):
             return default
 
-        def str_const(node):
+        def str_const(node) -> bool:
             return isinstance(node, node_classes.Const) and isinstance(node.value, str)
 
         for node in explicit.elts:
             if str_const(node):
                 inferred.append(node.value)
             else:
                 try:
@@ -846,127 +592,82 @@
         """The list of the names that are publicly available in this module.
 
         :returns: The list of public names.
         :rtype: list(str)
         """
         return [name for name in self.keys() if not name.startswith("_")]
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> bool:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`Module` this is always ``True``.
-        :rtype: bool
         """
         return True
 
     def get_children(self):
         yield from self.body
 
-    def frame(self: T, *, future: Literal[None, True] = None) -> T:
+    def frame(self: _T, *, future: Literal[None, True] = None) -> _T:
         """The node's frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
         return self
 
 
-class ComprehensionScope(LocalsDictNodeNG):
-    """Scoping for different types of comprehensions."""
-
-    scope_lookup = LocalsDictNodeNG._scope_lookup
-
-
 class GeneratorExp(ComprehensionScope):
     """Class representing an :class:`ast.GeneratorExp` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('(thing for thing in things if thing)')
     >>> node
     <GeneratorExp l.1 at 0x7f23b2e4e400>
     """
 
     _astroid_fields = ("elt", "generators")
     _other_other_fields = ("locals",)
-    elt = None
-    """The element that forms the output of the expression.
-
-    :type: NodeNG or None
-    """
-    generators = None
-    """The generators that are looped through.
-
-    :type: list(Comprehension) or None
-    """
+    elt: NodeNG
+    """The element that forms the output of the expression."""
 
     def __init__(
         self,
-        lineno=None,
-        col_offset=None,
-        parent=None,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        """
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
-
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
         self.locals = {}
-        """A map of the name of a local variable to the node defining the local.
+        """A map of the name of a local variable to the node defining the local."""
 
-        :type: dict(str, NodeNG)
-        """
+        self.generators: list[nodes.Comprehension] = []
+        """The generators that are looped through."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, elt=None, generators=None):
-        """Do some setup after initialisation.
-
-        :param elt: The element that forms the output of the expression.
-        :type elt: NodeNG or None
-
-        :param generators: The generators that are looped through.
-        :type generators: list(Comprehension) or None
-        """
+    def postinit(self, elt: NodeNG, generators: list[nodes.Comprehension]) -> None:
         self.elt = elt
-        if generators is None:
-            self.generators = []
-        else:
-            self.generators = generators
+        self.generators = generators
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`GeneratorExp` this is always ``True``.
-        :rtype: bool
         """
         return True
 
     def get_children(self):
         yield self.elt
 
         yield from self.generators
@@ -979,91 +680,48 @@
     >>> node = astroid.extract_node('{k:v for k, v in things if k > v}')
     >>> node
     <DictComp l.1 at 0x7f23b2e41d68>
     """
 
     _astroid_fields = ("key", "value", "generators")
     _other_other_fields = ("locals",)
-    key = None
-    """What produces the keys.
+    key: NodeNG
+    """What produces the keys."""
 
-    :type: NodeNG or None
-    """
-    value = None
-    """What produces the values.
-
-    :type: NodeNG or None
-    """
-    generators = None
-    """The generators that are looped through.
-
-    :type: list(Comprehension) or None
-    """
+    value: NodeNG
+    """What produces the values."""
 
     def __init__(
         self,
-        lineno=None,
-        col_offset=None,
-        parent=None,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        """
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
-
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
         self.locals = {}
-        """A map of the name of a local variable to the node defining the local.
-
-        :type: dict(str, NodeNG)
-        """
+        """A map of the name of a local variable to the node defining the local."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, key=None, value=None, generators=None):
-        """Do some setup after initialisation.
-
-        :param key: What produces the keys.
-        :type key: NodeNG or None
-
-        :param value: What produces the values.
-        :type value: NodeNG or None
-
-        :param generators: The generators that are looped through.
-        :type generators: list(Comprehension) or None
-        """
+    def postinit(
+        self, key: NodeNG, value: NodeNG, generators: list[nodes.Comprehension]
+    ) -> None:
         self.key = key
         self.value = value
-        if generators is None:
-            self.generators = []
-        else:
-            self.generators = generators
+        self.generators = generators
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`DictComp` this is always :class:`Uninferable`.
         :rtype: Uninferable
         """
         return util.Uninferable
@@ -1082,179 +740,116 @@
     >>> node = astroid.extract_node('{thing for thing in things if thing}')
     >>> node
     <SetComp l.1 at 0x7f23b2e41898>
     """
 
     _astroid_fields = ("elt", "generators")
     _other_other_fields = ("locals",)
-    elt = None
-    """The element that forms the output of the expression.
-
-    :type: NodeNG or None
-    """
-    generators = None
-    """The generators that are looped through.
-
-    :type: list(Comprehension) or None
-    """
+    elt: NodeNG
+    """The element that forms the output of the expression."""
 
     def __init__(
         self,
-        lineno=None,
-        col_offset=None,
-        parent=None,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        """
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
-
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
         self.locals = {}
-        """A map of the name of a local variable to the node defining the local.
+        """A map of the name of a local variable to the node defining the local."""
 
-        :type: dict(str, NodeNG)
-        """
+        self.generators: list[nodes.Comprehension] = []
+        """The generators that are looped through."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, elt=None, generators=None):
-        """Do some setup after initialisation.
-
-        :param elt: The element that forms the output of the expression.
-        :type elt: NodeNG or None
-
-        :param generators: The generators that are looped through.
-        :type generators: list(Comprehension) or None
-        """
+    def postinit(self, elt: NodeNG, generators: list[nodes.Comprehension]) -> None:
         self.elt = elt
-        if generators is None:
-            self.generators = []
-        else:
-            self.generators = generators
+        self.generators = generators
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`SetComp` this is always :class:`Uninferable`.
         :rtype: Uninferable
         """
         return util.Uninferable
 
     def get_children(self):
         yield self.elt
 
         yield from self.generators
 
 
-class _ListComp(node_classes.NodeNG):
+class ListComp(ComprehensionScope):
     """Class representing an :class:`ast.ListComp` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('[thing for thing in things if thing]')
     >>> node
     <ListComp l.1 at 0x7f23b2e418d0>
     """
 
     _astroid_fields = ("elt", "generators")
-    elt = None
-    """The element that forms the output of the expression.
+    _other_other_fields = ("locals",)
 
-    :type: NodeNG or None
-    """
-    generators = None
-    """The generators that are looped through.
+    elt: NodeNG
+    """The element that forms the output of the expression."""
 
-    :type: list(Comprehension) or None
-    """
+    def __init__(
+        self,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        self.locals = {}
+        """A map of the name of a local variable to the node defining it."""
 
-    def postinit(self, elt=None, generators=None):
-        """Do some setup after initialisation.
+        self.generators: list[nodes.Comprehension] = []
+        """The generators that are looped through."""
 
-        :param elt: The element that forms the output of the expression.
-        :type elt: NodeNG or None
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
 
-        :param generators: The generators that are looped through.
-        :type generators: list(Comprehension) or None
-        """
+    def postinit(self, elt: NodeNG, generators: list[nodes.Comprehension]):
         self.elt = elt
         self.generators = generators
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None):
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`ListComp` this is always :class:`Uninferable`.
         :rtype: Uninferable
         """
         return util.Uninferable
 
     def get_children(self):
         yield self.elt
 
         yield from self.generators
 
 
-class ListComp(_ListComp, ComprehensionScope):
-    """Class representing an :class:`ast.ListComp` node.
-
-    >>> import astroid
-    >>> node = astroid.extract_node('[thing for thing in things if thing]')
-    >>> node
-    <ListComp l.1 at 0x7f23b2e418d0>
-    """
-
-    _other_other_fields = ("locals",)
-
-    def __init__(
-        self,
-        lineno=None,
-        col_offset=None,
-        parent=None,
-        *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        self.locals = {}
-        """A map of the name of a local variable to the node defining it.
-
-        :type: dict(str, NodeNG)
-        """
-
-        super().__init__(
-            lineno=lineno,
-            col_offset=col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
-            parent=parent,
-        )
-
-
 def _infer_decorator_callchain(node):
     """Detect decorator call chaining and see if the end result is a
     static or a classmethod.
     """
     if not isinstance(node, FunctionDef):
         return None
     if not node.parent:
@@ -1284,239 +879,226 @@
                 and decorator.expr.name == "builtins"
                 and decorator.attrname in BUILTIN_DESCRIPTORS
             ):
                 return decorator.attrname
     return None
 
 
-class Lambda(mixins.FilterStmtsMixin, LocalsDictNodeNG):
+class Lambda(_base_nodes.FilterStmtsBaseNode, LocalsDictNodeNG):
     """Class representing an :class:`ast.Lambda` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('lambda arg: arg + 1')
     >>> node
     <Lambda.<lambda> l.1 at 0x7f23b2e41518>
     """
 
-    _astroid_fields = ("args", "body")
-    _other_other_fields = ("locals",)
+    _astroid_fields: ClassVar[tuple[str, ...]] = ("args", "body")
+    _other_other_fields: ClassVar[tuple[str, ...]] = ("locals",)
     name = "<lambda>"
     is_lambda = True
+    special_attributes = FunctionModel()
+    """The names of special attributes that this function has."""
+
+    args: Arguments
+    """The arguments that the function takes."""
 
-    def implicit_parameters(self):
+    body: NodeNG
+    """The contents of the function body."""
+
+    def implicit_parameters(self) -> Literal[0]:
         return 0
 
-    # function's type, 'function' | 'method' | 'staticmethod' | 'classmethod'
     @property
-    def type(self):
+    def type(self) -> Literal["method", "function"]:
         """Whether this is a method or function.
 
         :returns: 'method' if this is a method, 'function' otherwise.
-        :rtype: str
         """
         if self.args.arguments and self.args.arguments[0].name == "self":
             if isinstance(self.parent.scope(), ClassDef):
                 return "method"
         return "function"
 
     def __init__(
         self,
-        lineno=None,
-        col_offset=None,
-        parent=None,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno=None,
-        end_col_offset=None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ):
-        """
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
-
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
         self.locals = {}
-        """A map of the name of a local variable to the node defining it.
-
-        :type: dict(str, NodeNG)
-        """
+        """A map of the name of a local variable to the node defining it."""
 
-        self.args: Arguments
-        """The arguments that the function takes."""
-
-        self.body = []
-        """The contents of the function body.
-
-        :type: list(NodeNG)
-        """
+        self.instance_attrs: dict[str, list[NodeNG]] = {}
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, args: Arguments, body):
-        """Do some setup after initialisation.
-
-        :param args: The arguments that the function takes.
-
-        :param body: The contents of the function body.
-        :type body: list(NodeNG)
-        """
+    def postinit(self, args: Arguments, body: NodeNG) -> None:
         self.args = args
         self.body = body
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.instancemethod", "builtins.function"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         if "method" in self.type:
             return "builtins.instancemethod"
         return "builtins.function"
 
-    def display_type(self):
+    def display_type(self) -> str:
         """A human readable type of this node.
 
         :returns: The type of this node.
         :rtype: str
         """
         if "method" in self.type:
             return "Method"
         return "Function"
 
-    def callable(self):
+    def callable(self) -> Literal[True]:
         """Whether this node defines something that is callable.
 
-        :returns: True if this defines something that is callable,
-            False otherwise.
+        :returns: Whether this defines something that is callable
             For a :class:`Lambda` this is always ``True``.
-        :rtype: bool
         """
         return True
 
-    def argnames(self):
-        """Get the names of each of the arguments.
+    def argnames(self) -> list[str]:
+        """Get the names of each of the arguments, including that
+        of the collections of variable-length arguments ("args", "kwargs",
+        etc.), as well as positional-only and keyword-only arguments.
 
         :returns: The names of the arguments.
         :rtype: list(str)
         """
         if self.args.arguments:  # maybe None with builtin functions
             names = _rec_get_names(self.args.arguments)
         else:
             names = []
         if self.args.vararg:
             names.append(self.args.vararg)
+        names += [elt.name for elt in self.args.kwonlyargs]
         if self.args.kwarg:
             names.append(self.args.kwarg)
         return names
 
-    def infer_call_result(self, caller, context=None):
-        """Infer what the function returns when called.
-
-        :param caller: Unused
-        :type caller: object
-        """
-        # pylint: disable=no-member; github.com/pycqa/astroid/issues/291
-        # args is in fact redefined later on by postinit. Can't be changed
-        # to None due to a strong interaction between Lambda and FunctionDef.
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
+        """Infer what the function returns when called."""
         return self.body.infer(context)
 
-    def scope_lookup(self, node, name, offset=0):
+    def scope_lookup(
+        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+    ) -> tuple[LocalsDictNodeNG, list[NodeNG]]:
         """Lookup where the given names is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
-        :type node: NodeNG
 
         :param name: The name to find assignments for.
-        :type name: str
 
         :param offset: The line offset to filter statements up to.
-        :type offset: int
 
         :returns: This scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
-        :rtype: tuple(str, list(NodeNG))
         """
-        if node in self.args.defaults or node in self.args.kw_defaults:
+        if (self.args.defaults and node in self.args.defaults) or (
+            self.args.kw_defaults and node in self.args.kw_defaults
+        ):
             frame = self.parent.frame(future=True)
             # line offset to avoid that def func(f=func) resolve the default
             # value to the defined function
             offset = -1
         else:
             # check this is not used in function decorators
             frame = self
         return frame._scope_lookup(node, name, offset)
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`Lambda` this is always ``True``.
-        :rtype: bool
         """
         return True
 
     def get_children(self):
         yield self.args
         yield self.body
 
-    def frame(self: T, *, future: Literal[None, True] = None) -> T:
+    def frame(self: _T, *, future: Literal[None, True] = None) -> _T:
         """The node's frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
         return self
 
+    def getattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> list[NodeNG]:
+        if not name:
+            raise AttributeInferenceError(target=self, attribute=name, context=context)
 
-class FunctionDef(mixins.MultiLineBlockMixin, node_classes.Statement, Lambda):
+        found_attrs = []
+        if name in self.instance_attrs:
+            found_attrs = self.instance_attrs[name]
+        if name in self.special_attributes:
+            found_attrs.append(self.special_attributes.lookup(name))
+        if found_attrs:
+            return found_attrs
+        raise AttributeInferenceError(target=self, attribute=name)
+
+
+class FunctionDef(
+    _base_nodes.MultiLineBlockNode,
+    _base_nodes.FilterStmtsBaseNode,
+    _base_nodes.Statement,
+    LocalsDictNodeNG,
+):
     """Class representing an :class:`ast.FunctionDef`.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     ... def my_func(arg):
     ...     return arg + 1
     ... ''')
     >>> node
     <FunctionDef.my_func l.2 at 0x7f23b2e71e10>
     """
 
-    _astroid_fields = ("decorators", "args", "returns", "body")
+    _astroid_fields = ("decorators", "args", "returns", "doc_node", "body")
     _multi_line_block_fields = ("body",)
     returns = None
-    decorators = None
-    """The decorators that are applied to this method or function.
 
-    :type: Decorators or None
-    """
-    special_attributes = FunctionModel()
-    """The names of special attributes that this function has.
+    decorators: node_classes.Decorators | None
+    """The decorators that are applied to this method or function."""
+
+    doc_node: Const | None
+    """The doc node associated with this node."""
+
+    args: Arguments
+    """The arguments that the function takes."""
 
-    :type: objectmodel.FunctionModel
-    """
     is_function = True
     """Whether this node indicates a function.
 
     For a :class:`FunctionDef` this is always ``True``.
 
     :type: bool
     """
@@ -1529,131 +1111,141 @@
     """
     If present, this will contain the type annotation for arguments
     passed by a type comment
     """
     type_comment_returns = None
     """If present, this will contain the return type annotation, passed by a type comment"""
     # attributes below are set by the builder module or by raw factories
-    _other_fields = ("name", "doc")
+    _other_fields = ("name", "doc", "position")
     _other_other_fields = (
         "locals",
         "_type",
         "type_comment_returns",
         "type_comment_args",
     )
     _type = None
 
-    def __init__(
-        self,
-        name=None,
-        doc=None,
-        lineno=None,
-        col_offset=None,
-        parent=None,
-        *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        """
-        :param name: The name of the function.
-        :type name: str or None
-
-        :param doc: The function's docstring.
-        :type doc: str or None
+    name = "<functiondef>"
 
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
+    is_lambda = True
 
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
+    special_attributes = FunctionModel()
+    """The names of special attributes that this function has."""
 
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
+    def __init__(
+        self,
+        name: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
         self.name = name
-        """The name of the function.
+        """The name of the function."""
 
-        :type name: str or None
-        """
+        self._doc: str | None = None
+        """DEPRECATED: The function docstring."""
 
-        self.doc = doc
-        """The function's docstring.
+        self.locals = {}
+        """A map of the name of a local variable to the node defining it."""
 
-        :type doc: str or None
-        """
+        self.body: list[NodeNG] = []
+        """The contents of the function body."""
+
+        self.instance_attrs: dict[str, list[NodeNG]] = {}
 
-        self.instance_attrs = {}
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
-        if parent:
+        if parent and not isinstance(parent, Unknown):
             frame = parent.frame(future=True)
             frame.set_local(name, self)
 
-    # pylint: disable=arguments-differ; different than Lambdas
     def postinit(
         self,
         args: Arguments,
-        body,
-        decorators=None,
+        body: list[NodeNG],
+        decorators: node_classes.Decorators | None = None,
         returns=None,
         type_comment_returns=None,
         type_comment_args=None,
+        *,
+        position: Position | None = None,
+        doc_node: Const | None = None,
     ):
         """Do some setup after initialisation.
 
         :param args: The arguments that the function takes.
 
         :param body: The contents of the function body.
-        :type body: list(NodeNG)
 
         :param decorators: The decorators that are applied to this
             method or function.
-        :type decorators: Decorators or None
         :params type_comment_returns:
             The return type annotation passed via a type comment.
         :params type_comment_args:
             The args type annotation passed via a type comment.
+        :params position:
+            Position of function keyword(s) and name.
+        :param doc_node:
+            The doc node associated with this node.
         """
         self.args = args
         self.body = body
         self.decorators = decorators
         self.returns = returns
         self.type_comment_returns = type_comment_returns
         self.type_comment_args = type_comment_args
+        self.position = position
+        self.doc_node = doc_node
+        if doc_node:
+            self._doc = doc_node.value
+
+    @property
+    def doc(self) -> str | None:
+        """The function docstring."""
+        warnings.warn(
+            "The 'FunctionDef.doc' attribute is deprecated, "
+            "use 'FunctionDef.doc_node' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._doc
+
+    @doc.setter
+    def doc(self, value: str | None) -> None:
+        warnings.warn(
+            "Setting the 'FunctionDef.doc' attribute is deprecated, "
+            "use 'FunctionDef.doc_node' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self._doc = value
 
-    @decorators_mod.cachedproperty
-    def extra_decorators(self):
+    @cached_property
+    def extra_decorators(self) -> list[node_classes.Call]:
         """The extra decorators that this function can have.
 
         Additional decorators are considered when they are used as
         assignments, as in ``method = staticmethod(method)``.
         The property will return all the callables that are used for
         decoration.
-
-        :type: list(NodeNG)
         """
         frame = self.parent.frame(future=True)
         if not isinstance(frame, ClassDef):
             return []
 
-        decorators = []
-        for assign in frame._get_assign_nodes():
+        decorators: list[node_classes.Call] = []
+        for assign in frame._assign_nodes_in_scope:
             if isinstance(assign.value, node_classes.Call) and isinstance(
                 assign.value.func, node_classes.Name
             ):
                 for assign_node in assign.targets:
                     if not isinstance(assign_node, node_classes.AssignName):
                         # Support only `name = callable(name)`
                         continue
@@ -1672,23 +1264,75 @@
                         if (
                             isinstance(meth, FunctionDef)
                             and assign_node.frame(future=True) == frame
                         ):
                             decorators.append(assign.value)
         return decorators
 
-    @decorators_mod.cachedproperty
-    def type(
-        self,
-    ):  # pylint: disable=invalid-overridden-method,too-many-return-statements
+    def pytype(self) -> Literal["builtins.instancemethod", "builtins.function"]:
+        """Get the name of the type that this node represents.
+
+        :returns: The name of the type.
+        """
+        if "method" in self.type:
+            return "builtins.instancemethod"
+        return "builtins.function"
+
+    def display_type(self) -> str:
+        """A human readable type of this node.
+
+        :returns: The type of this node.
+        :rtype: str
+        """
+        if "method" in self.type:
+            return "Method"
+        return "Function"
+
+    def callable(self) -> Literal[True]:
+        return True
+
+    def argnames(self) -> list[str]:
+        """Get the names of each of the arguments, including that
+        of the collections of variable-length arguments ("args", "kwargs",
+        etc.), as well as positional-only and keyword-only arguments.
+
+        :returns: The names of the arguments.
+        :rtype: list(str)
+        """
+        if self.args.arguments:  # maybe None with builtin functions
+            names = _rec_get_names(self.args.arguments)
+        else:
+            names = []
+        if self.args.vararg:
+            names.append(self.args.vararg)
+        names += [elt.name for elt in self.args.kwonlyargs]
+        if self.args.kwarg:
+            names.append(self.args.kwarg)
+        return names
+
+    def getattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> list[NodeNG]:
+        if not name:
+            raise AttributeInferenceError(target=self, attribute=name, context=context)
+
+        found_attrs = []
+        if name in self.instance_attrs:
+            found_attrs = self.instance_attrs[name]
+        if name in self.special_attributes:
+            found_attrs.append(self.special_attributes.lookup(name))
+        if found_attrs:
+            return found_attrs
+        raise AttributeInferenceError(target=self, attribute=name)
+
+    @cached_property
+    def type(self) -> str:  # pylint: disable=too-many-return-statements # noqa: C901
         """The function type for this node.
 
         Possible values are: method, function, staticmethod, classmethod.
-
-        :type: str
         """
         for decorator in self.extra_decorators:
             if decorator.func.name in BUILTIN_DESCRIPTORS:
                 return decorator.func.name
 
         frame = self.parent.frame(future=True)
         type_name = "function"
@@ -1746,88 +1390,73 @@
                             return "classmethod"
                         if ancestor.is_subtype_of("builtins.staticmethod"):
                             return "staticmethod"
             except InferenceError:
                 pass
         return type_name
 
-    @decorators_mod.cachedproperty
-    def fromlineno(self):
+    @cached_property
+    def fromlineno(self) -> int:
         """The first line that this node appears on in the source code.
 
-        :type: int or None
+        Can also return 0 if the line can not be determined.
         """
         # lineno is the line number of the first decorator, we want the def
-        # statement lineno
-        lineno = self.lineno
+        # statement lineno. Similar to 'ClassDef.fromlineno'
+        lineno = self.lineno or 0
         if self.decorators is not None:
             lineno += sum(
-                node.tolineno - node.lineno + 1 for node in self.decorators.nodes
+                node.tolineno - (node.lineno or 0) + 1 for node in self.decorators.nodes
             )
 
-        return lineno
+        return lineno or 0
 
-    @decorators_mod.cachedproperty
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         return self.args.tolineno
 
-    def block_range(self, lineno):
+    def implicit_parameters(self) -> Literal[0, 1]:
+        return 1 if self.is_bound() else 0
+
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: Unused.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
-        :rtype: tuple(int, int)
         """
         return self.fromlineno, self.tolineno
 
-    def getattr(self, name, context=None):
-        """this method doesn't look in the instance_attrs dictionary since it's
-        done by an Instance proxy at inference time.
-        """
-        if not name:
-            raise AttributeInferenceError(target=self, attribute=name, context=context)
-
-        found_attrs = []
-        if name in self.instance_attrs:
-            found_attrs = self.instance_attrs[name]
-        if name in self.special_attributes:
-            found_attrs.append(self.special_attributes.lookup(name))
-        if found_attrs:
-            return found_attrs
-        raise AttributeInferenceError(target=self, attribute=name)
-
-    def igetattr(self, name, context=None):
+    def igetattr(
+        self, name: str, context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
         """Inferred getattr, which returns an iterator of inferred statements."""
         try:
             return bases._infer_stmts(self.getattr(name, context), context, frame=self)
         except AttributeInferenceError as error:
             raise InferenceError(
                 str(error), target=self, attribute=name, context=context
             ) from error
 
-    def is_method(self):
+    def is_method(self) -> bool:
         """Check if this function node represents a method.
 
-        :returns: True if this is a method, False otherwise.
-        :rtype: bool
+        :returns: Whether this is a method.
         """
         # check we are defined in a ClassDef, because this is usually expected
         # (e.g. pylint...) when is_method() return True
         return self.type != "function" and isinstance(
             self.parent.frame(future=True), ClassDef
         )
 
-    @decorators_mod.cached
-    def decoratornames(self, context=None):
+    def decoratornames(self, context: InferenceContext | None = None):
         """Get the qualified names of each of the decorators on this function.
 
         :param context:
             An inference context that can be passed to inference functions
         :returns: The names of the decorators.
         :rtype: set(str)
         """
@@ -1840,34 +1469,31 @@
             try:
                 for infnode in decnode.infer(context=context):
                     result.add(infnode.qname())
             except InferenceError:
                 continue
         return result
 
-    def is_bound(self):
+    def is_bound(self) -> bool:
         """Check if the function is bound to an instance or class.
 
-        :returns: True if the function is bound to an instance or class,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether the function is bound to an instance or class.
         """
-        return self.type == "classmethod"
+        return self.type in {"method", "classmethod"}
 
-    def is_abstract(self, pass_is_abstract=True, any_raise_is_abstract=False):
+    def is_abstract(self, pass_is_abstract=True, any_raise_is_abstract=False) -> bool:
         """Check if the method is abstract.
 
         A method is considered abstract if any of the following is true:
         * The only statement is 'raise NotImplementedError'
         * The only statement is 'raise <SomeException>' and any_raise_is_abstract is True
         * The only statement is 'pass' and pass_is_abstract is True
         * The method is annotated with abc.astractproperty/abc.abstractmethod
 
-        :returns: True if the method is abstract, False otherwise.
-        :rtype: bool
+        :returns: Whether the method is abstract.
         """
         if self.decorators:
             for node in self.decorators.nodes:
                 try:
                     inferred = next(node.infer())
                 except (InferenceError, StopIteration):
                     continue
@@ -1884,77 +1510,108 @@
                 if child_node.raises_not_implemented():
                     return True
             return pass_is_abstract and isinstance(child_node, node_classes.Pass)
         # empty function is the same as function with a single "pass" statement
         if pass_is_abstract:
             return True
 
-    def is_generator(self):
+        return False
+
+    def is_generator(self) -> bool:
         """Check if this is a generator function.
 
-        :returns: True is this is a generator function, False otherwise.
-        :rtype: bool
+        :returns: Whether this is a generator function.
         """
         return bool(next(self._get_yield_nodes_skip_lambdas(), False))
 
-    def infer_yield_result(self, context=None):
+    def infer_yield_result(self, context: InferenceContext | None = None):
         """Infer what the function yields when called
 
         :returns: What the function yields
         :rtype: iterable(NodeNG or Uninferable) or None
         """
         # pylint: disable=not-an-iterable
-        # https://github.com/PyCQA/astroid/issues/1015
+        # https://github.com/pylint-dev/astroid/issues/1015
         for yield_ in self.nodes_of_class(node_classes.Yield):
             if yield_.value is None:
                 const = node_classes.Const(None)
                 const.parent = yield_
                 const.lineno = yield_.lineno
                 yield const
             elif yield_.scope() == self:
                 yield from yield_.value.infer(context=context)
 
-    def infer_call_result(self, caller=None, context=None):
-        """Infer what the function returns when called.
-
-        :returns: What the function returns.
-        :rtype: iterable(NodeNG or Uninferable) or None
-        """
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
+        """Infer what the function returns when called."""
         if self.is_generator():
             if isinstance(self, AsyncFunctionDef):
-                generator_cls = bases.AsyncGenerator
+                generator_cls: type[bases.Generator] = bases.AsyncGenerator
             else:
                 generator_cls = bases.Generator
             result = generator_cls(self, generator_initial_context=context)
             yield result
             return
         # This is really a gigantic hack to work around metaclass generators
         # that return transient class-generating functions. Pylint's AST structure
         # cannot handle a base class object that is only used for calling __new__,
         # but does not contribute to the inheritance structure itself. We inject
         # a fake class into the hierarchy here for several well-known metaclass
         # generators, and filter it out later.
         if (
             self.name == "with_metaclass"
+            and caller is not None
+            and self.args.args
             and len(self.args.args) == 1
             and self.args.vararg is not None
         ):
-            metaclass = next(caller.args[0].infer(context), None)
+            if isinstance(caller.args, Arguments):
+                assert caller.args.args is not None
+                metaclass = next(caller.args.args[0].infer(context), None)
+            elif isinstance(caller.args, list):
+                metaclass = next(caller.args[0].infer(context), None)
+            else:
+                raise TypeError(  # pragma: no cover
+                    f"caller.args was neither Arguments nor list; got {type(caller.args)}"
+                )
             if isinstance(metaclass, ClassDef):
                 try:
-                    class_bases = [next(arg.infer(context)) for arg in caller.args[1:]]
+                    class_bases = [
+                        # Find the first non-None inferred base value
+                        next(
+                            b
+                            for b in arg.infer(
+                                context=context.clone() if context else context
+                            )
+                            if not (isinstance(b, Const) and b.value is None)
+                        )
+                        for arg in caller.args[1:]
+                    ]
                 except StopIteration as e:
                     raise InferenceError(node=caller.args[1:], context=context) from e
-                new_class = ClassDef(name="temporary_class")
+                new_class = ClassDef(
+                    name="temporary_class",
+                    lineno=0,
+                    col_offset=0,
+                    end_lineno=0,
+                    end_col_offset=0,
+                    parent=self,
+                )
                 new_class.hide = True
-                new_class.parent = self
                 new_class.postinit(
-                    bases=[base for base in class_bases if base != util.Uninferable],
+                    bases=[
+                        base
+                        for base in class_bases
+                        if not isinstance(base, util.UninferableBase)
+                    ],
                     body=[],
-                    decorators=[],
+                    decorators=None,
                     metaclass=metaclass,
                 )
                 yield new_class
                 return
         returns = self._get_return_nodes_skip_functions()
 
         first_return = next(returns, None)
@@ -1973,47 +1630,59 @@
                 yield node_classes.Const(None)
             else:
                 try:
                     yield from returnnode.value.infer(context)
                 except InferenceError:
                     yield util.Uninferable
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> bool:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`FunctionDef` this is always ``True``.
-        :rtype: bool
         """
         return True
 
     def get_children(self):
         if self.decorators is not None:
             yield self.decorators
 
         yield self.args
 
         if self.returns is not None:
             yield self.returns
 
         yield from self.body
 
-    def scope_lookup(self, node, name, offset=0):
+    def scope_lookup(
+        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+    ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """Lookup where the given name is assigned."""
         if name == "__class__":
             # __class__ is an implicit closure reference created by the compiler
             # if any methods in a class body refer to either __class__ or super.
             # In our case, we want to be able to look it up in the current scope
             # when `__class__` is being used.
             frame = self.parent.frame(future=True)
             if isinstance(frame, ClassDef):
                 return self, [frame]
-        return super().scope_lookup(node, name, offset)
 
-    def frame(self: T, *, future: Literal[None, True] = None) -> T:
+        if (self.args.defaults and node in self.args.defaults) or (
+            self.args.kw_defaults and node in self.args.kw_defaults
+        ):
+            frame = self.parent.frame(future=True)
+            # line offset to avoid that def func(f=func) resolve the default
+            # value to the defined function
+            offset = -1
+        else:
+            # check this is not used in function decorators
+            frame = self
+        return frame._scope_lookup(node, name, offset)
+
+    def frame(self: _T, *, future: Literal[None, True] = None) -> _T:
         """The node's frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
@@ -2035,27 +1704,27 @@
     >>> node
     <AsyncFunctionDef.func l.2 at 0x7f23b2e416d8>
     >>> node.body[0]
     <AsyncFor l.3 at 0x7f23b2e417b8>
     """
 
 
-def _rec_get_names(args, names=None):
+def _rec_get_names(args, names: list[str] | None = None) -> list[str]:
     """return a list of all argument names"""
     if names is None:
         names = []
     for arg in args:
         if isinstance(arg, node_classes.Tuple):
             _rec_get_names(arg.elts, names)
         else:
             names.append(arg.name)
     return names
 
 
-def _is_metaclass(klass, seen=None):
+def _is_metaclass(klass, seen=None) -> bool:
     """Return if the given class can be
     used as a metaclass.
     """
     if klass.name == "type":
         return True
     if seen is None:
         seen = set()
@@ -2066,16 +1735,14 @@
                 if baseobj_name in seen:
                     continue
 
                 seen.add(baseobj_name)
                 if isinstance(baseobj, bases.Instance):
                     # not abstract
                     return False
-                if baseobj is util.Uninferable:
-                    continue
                 if baseobj is klass:
                     continue
                 if not isinstance(baseobj, ClassDef):
                     continue
                 if baseobj._type == "metaclass":
                     return True
                 if _is_metaclass(baseobj, seen):
@@ -2134,15 +1801,18 @@
         if klass.parent is None:
             klass = None
         else:
             klass = klass.parent.frame(future=True)
     return klass
 
 
-class ClassDef(mixins.FilterStmtsMixin, LocalsDictNodeNG, node_classes.Statement):
+# pylint: disable=too-many-instance-attributes
+class ClassDef(
+    _base_nodes.FilterStmtsBaseNode, LocalsDictNodeNG, _base_nodes.Statement
+):
     """Class representing an :class:`ast.ClassDef` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     class Thing:
         def my_meth(self, arg):
             return arg + self.offset
@@ -2151,130 +1821,121 @@
     <ClassDef.Thing l.2 at 0x7f23b2e9e748>
     """
 
     # some of the attributes below are set by the builder module or
     # by a raw factories
 
     # a dictionary of class instances attributes
-    _astroid_fields = ("decorators", "bases", "keywords", "body")  # name
+    _astroid_fields = ("decorators", "bases", "keywords", "doc_node", "body")  # name
 
     decorators = None
     """The decorators that are applied to this class.
 
     :type: Decorators or None
     """
     special_attributes = ClassModel()
     """The names of special attributes that this class has.
 
     :type: objectmodel.ClassModel
     """
 
     _type = None
+    _metaclass: NodeNG | None = None
     _metaclass_hack = False
     hide = False
     type = property(
         _class_type,
         doc=(
             "The class type for this node.\n\n"
             "Possible values are: class, metaclass, exception.\n\n"
             ":type: str"
         ),
     )
-    _other_fields = ("name", "doc")
+    _other_fields = ("name", "doc", "is_dataclass", "position")
     _other_other_fields = ("locals", "_newstyle")
-    _newstyle = None
+    _newstyle: bool | None = None
 
     def __init__(
         self,
-        name=None,
-        doc=None,
-        lineno=None,
-        col_offset=None,
-        parent=None,
+        name: str,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
         *,
-        end_lineno=None,
-        end_col_offset=None,
-    ):
-        """
-        :param name: The name of the class.
-        :type name: str or None
-
-        :param doc: The function's docstring.
-        :type doc: str or None
-
-        :param lineno: The line that this node appears on in the source code.
-        :type lineno: int or None
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-        :type col_offset: int or None
-
-        :param parent: The parent node in the syntax tree.
-        :type parent: NodeNG or None
-
-        :param end_lineno: The last line this node appears on in the source code.
-        :type end_lineno: Optional[int]
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        :type end_col_offset: Optional[int]
-        """
-        self.instance_attrs = {}
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        self.instance_attrs: dict[str, NodeNG] = {}
         self.locals = {}
-        """A map of the name of a local variable to the node defining it.
+        """A map of the name of a local variable to the node defining it."""
 
-        :type: dict(str, NodeNG)
-        """
-
-        self.keywords = []
+        self.keywords: list[node_classes.Keyword] = []
         """The keywords given to the class definition.
 
         This is usually for :pep:`3115` style metaclass declaration.
-
-        :type: list(Keyword) or None
         """
 
-        self.bases = []
-        """What the class inherits from.
+        self.bases: list[NodeNG] = []
+        """What the class inherits from."""
 
-        :type: list(NodeNG)
-        """
-
-        self.body = []
-        """The contents of the class body.
-
-        :type: list(NodeNG)
-        """
+        self.body: list[NodeNG] = []
+        """The contents of the class body."""
 
         self.name = name
-        """The name of the class.
+        """The name of the class."""
 
-        :type name: str or None
-        """
+        self.decorators = None
+        """The decorators that are applied to this class."""
 
-        self.doc = doc
-        """The class' docstring.
+        self._doc: str | None = None
+        """DEPRECATED: The class docstring."""
 
-        :type doc: str or None
-        """
+        self.doc_node: Const | None = None
+        """The doc node associated with this node."""
+
+        self.is_dataclass: bool = False
+        """Whether this class is a dataclass."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
-        if parent is not None:
+        if parent and not isinstance(parent, Unknown):
             parent.frame(future=True).set_local(name, self)
 
         for local_name, node in self.implicit_locals():
             self.add_local_node(node, local_name)
 
-    def implicit_parameters(self):
+    infer_binary_op: ClassVar[InferBinaryOp[ClassDef]]
+
+    @property
+    def doc(self) -> str | None:
+        """The class docstring."""
+        warnings.warn(
+            "The 'ClassDef.doc' attribute is deprecated, "
+            "use 'ClassDef.doc_node' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._doc
+
+    @doc.setter
+    def doc(self, value: str | None) -> None:
+        warnings.warn(
+            "Setting the 'ClassDef.doc' attribute is deprecated, "
+            "use 'ClassDef.doc_node.value' instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self._doc = value
+
+    def implicit_parameters(self) -> Literal[1]:
         return 1
 
     def implicit_locals(self):
         """Get implicitly defined class definition locals.
 
         :returns: the the name and Const pair for each local
         :rtype: tuple(tuple(str, node_classes.Const), ...)
@@ -2282,47 +1943,38 @@
         locals_ = (("__module__", self.special_attributes.attr___module__),)
         # __qualname__ is defined in PEP3155
         locals_ += (("__qualname__", self.special_attributes.attr___qualname__),)
         return locals_
 
     # pylint: disable=redefined-outer-name
     def postinit(
-        self, bases, body, decorators, newstyle=None, metaclass=None, keywords=None
-    ):
-        """Do some setup after initialisation.
-
-        :param bases: What the class inherits from.
-        :type bases: list(NodeNG)
-
-        :param body: The contents of the class body.
-        :type body: list(NodeNG)
-
-        :param decorators: The decorators that are applied to this class.
-        :type decorators: Decorators or None
-
-        :param newstyle: Whether this is a new style class or not.
-        :type newstyle: bool or None
-
-        :param metaclass: The metaclass of this class.
-        :type metaclass: NodeNG or None
-
-        :param keywords: The keywords given to the class definition.
-        :type keywords: list(Keyword) or None
-        """
+        self,
+        bases: list[NodeNG],
+        body: list[NodeNG],
+        decorators: node_classes.Decorators | None,
+        newstyle: bool | None = None,
+        metaclass: NodeNG | None = None,
+        keywords: list[node_classes.Keyword] | None = None,
+        *,
+        position: Position | None = None,
+        doc_node: Const | None = None,
+    ) -> None:
         if keywords is not None:
             self.keywords = keywords
         self.bases = bases
         self.body = body
         self.decorators = decorators
-        if newstyle is not None:
-            self._newstyle = newstyle
-        if metaclass is not None:
-            self._metaclass = metaclass
+        self._newstyle = newstyle
+        self._metaclass = metaclass
+        self.position = position
+        self.doc_node = doc_node
+        if doc_node:
+            self._doc = doc_node.value
 
-    def _newstyle_impl(self, context=None):
+    def _newstyle_impl(self, context: InferenceContext | None = None):
         if context is None:
             context = InferenceContext()
         if self._newstyle is not None:
             return self._newstyle
         for base in self.ancestors(recurs=False, context=context):
             if base._newstyle_impl(context):
                 self._newstyle = True
@@ -2338,73 +1990,86 @@
 
     _newstyle = None
     newstyle = property(
         _newstyle_impl,
         doc=("Whether this is a new style class or not\n\n" ":type: bool or None"),
     )
 
-    @decorators_mod.cachedproperty
+    @cached_property
+    def fromlineno(self) -> int:
+        """The first line that this node appears on in the source code.
+
+        Can also return 0 if the line can not be determined.
+        """
+        if IS_PYPY and PY38 and not PYPY_7_3_11_PLUS:
+            # For Python < 3.8 the lineno is the line number of the first decorator.
+            # We want the class statement lineno. Similar to 'FunctionDef.fromlineno'
+            # PyPy (3.8): Fixed with version v7.3.11
+            lineno = self.lineno or 0
+            if self.decorators is not None:
+                lineno += sum(
+                    node.tolineno - (node.lineno or 0) + 1
+                    for node in self.decorators.nodes
+                )
+
+            return lineno or 0
+        return super().fromlineno
+
+    @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
 
         :type: int
         """
         if self.bases:
             return self.bases[-1].tolineno
 
         return self.fromlineno
 
-    def block_range(self, lineno):
+    def block_range(self, lineno: int) -> tuple[int, int]:
         """Get a range from the given line number to where this node ends.
 
         :param lineno: Unused.
-        :type lineno: int
 
         :returns: The range of line numbers that this node belongs to,
-        :rtype: tuple(int, int)
         """
         return self.fromlineno, self.tolineno
 
-    def pytype(self):
+    def pytype(self) -> Literal["builtins.type", "builtins.classobj"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
-        :rtype: str
         """
         if self.newstyle:
             return "builtins.type"
         return "builtins.classobj"
 
-    def display_type(self):
+    def display_type(self) -> str:
         """A human readable type of this node.
 
         :returns: The type of this node.
         :rtype: str
         """
         return "Class"
 
-    def callable(self):
+    def callable(self) -> bool:
         """Whether this node defines something that is callable.
 
-        :returns: True if this defines something that is callable,
-            False otherwise.
+        :returns: Whether this defines something that is callable.
             For a :class:`ClassDef` this is always ``True``.
-        :rtype: bool
         """
         return True
 
-    def is_subtype_of(self, type_name, context=None):
+    def is_subtype_of(self, type_name, context: InferenceContext | None = None) -> bool:
         """Whether this class is a subtype of the given type.
 
         :param type_name: The name of the type of check against.
         :type type_name: str
 
-        :returns: True if this class is a subtype of the given type,
-            False otherwise.
-        :rtype: bool
+        :returns: Whether this class is a subtype of the given type.
         """
         if self.qname() == type_name:
             return True
 
         return any(anc.qname() == type_name for anc in self.ancestors(context=context))
 
     def _infer_type_call(self, caller, context):
@@ -2415,15 +2080,22 @@
         if isinstance(name_node, node_classes.Const) and isinstance(
             name_node.value, str
         ):
             name = name_node.value
         else:
             return util.Uninferable
 
-        result = ClassDef(name, None)
+        result = ClassDef(
+            name,
+            lineno=0,
+            col_offset=0,
+            end_lineno=0,
+            end_col_offset=0,
+            parent=Unknown(),
+        )
 
         # Get the bases of the class.
         try:
             class_bases = next(caller.args[1].infer(context))
         except StopIteration as e:
             raise InferenceError(node=caller.args[1], context=context) from e
         if isinstance(class_bases, (node_classes.Tuple, node_classes.List)):
@@ -2451,55 +2123,62 @@
             for attr, value in members.items:
                 if isinstance(attr, node_classes.Const) and isinstance(attr.value, str):
                     result.locals[attr.value] = [value]
 
         result.parent = caller.parent
         return result
 
-    def infer_call_result(self, caller, context=None):
+    def infer_call_result(
+        self,
+        caller: SuccessfulInferenceResult | None,
+        context: InferenceContext | None = None,
+    ) -> Iterator[InferenceResult]:
         """infer what a class is returning when called"""
         if self.is_subtype_of("builtins.type", context) and len(caller.args) == 3:
             result = self._infer_type_call(caller, context)
             yield result
             return
 
         dunder_call = None
         try:
             metaclass = self.metaclass(context=context)
             if metaclass is not None:
-                dunder_call = next(metaclass.igetattr("__call__", context))
+                # Only get __call__ if it's defined locally for the metaclass.
+                # Otherwise we will find ObjectModel.__call__ which will
+                # return an instance of the metaclass. Instantiating the class is
+                # handled later.
+                if "__call__" in metaclass.locals:
+                    dunder_call = next(metaclass.igetattr("__call__", context))
         except (AttributeInferenceError, StopIteration):
             pass
 
         if dunder_call and dunder_call.qname() != "builtins.type.__call__":
             # Call type.__call__ if not set metaclass
             # (since type is the default metaclass)
             context = bind_context_to_node(context, self)
             context.callcontext.callee = dunder_call
             yield from dunder_call.infer_call_result(caller, context)
         else:
             yield self.instantiate_class()
 
-    def scope_lookup(self, node, name, offset=0):
+    def scope_lookup(
+        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+    ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """Lookup where the given name is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
-        :type node: NodeNG
 
         :param name: The name to find assignments for.
-        :type name: str
 
         :param offset: The line offset to filter statements up to.
-        :type offset: int
 
         :returns: This scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
-        :rtype: tuple(str, list(NodeNG))
         """
         # If the name looks like a builtin name, just try to look
         # into the upper scope of this class. We might have a
         # decorator that it's poorly named after a builtin object
         # inside this class.
         lookup_upper_frame = (
             isinstance(node.parent, node_classes.Decorators)
@@ -2536,22 +2215,22 @@
 
         Names are given in the order they appear in the class definition.
 
         :type: list(str)
         """
         return [bnode.as_string() for bnode in self.bases]
 
-    def ancestors(self, recurs=True, context=None):
+    def ancestors(
+        self, recurs: bool = True, context: InferenceContext | None = None
+    ) -> Generator[ClassDef, None, None]:
         """Iterate over the base classes in prefixed depth first order.
 
         :param recurs: Whether to recurse or return direct ancestors only.
-        :type recurs: bool
 
         :returns: The base classes
-        :rtype: iterable(NodeNG)
         """
         # FIXME: should be possible to choose the resolution order
         # FIXME: inference make infinite loops possible here
         yielded = {self}
         if context is None:
             context = InferenceContext()
         if not self.bases and self.qname() != "builtins.object":
@@ -2581,61 +2260,60 @@
                             if grandpa in yielded:
                                 continue
                             yielded.add(grandpa)
                             yield grandpa
                 except InferenceError:
                     continue
 
-    def local_attr_ancestors(self, name, context=None):
+    def local_attr_ancestors(self, name, context: InferenceContext | None = None):
         """Iterate over the parents that define the given name.
 
         :param name: The name to find definitions for.
         :type name: str
 
         :returns: The parents that define the given name.
         :rtype: iterable(NodeNG)
         """
         # Look up in the mro if we can. This will result in the
         # attribute being looked up just as Python does it.
         try:
-            ancestors = self.mro(context)[1:]
+            ancestors: Iterable[ClassDef] = self.mro(context)[1:]
         except MroError:
             # Fallback to use ancestors, we can't determine
             # a sane MRO.
             ancestors = self.ancestors(context=context)
         for astroid in ancestors:
             if name in astroid:
                 yield astroid
 
-    def instance_attr_ancestors(self, name, context=None):
+    def instance_attr_ancestors(self, name, context: InferenceContext | None = None):
         """Iterate over the parents that define the given name as an attribute.
 
         :param name: The name to find definitions for.
         :type name: str
 
         :returns: The parents that define the given name as
             an instance attribute.
         :rtype: iterable(NodeNG)
         """
         for astroid in self.ancestors(context=context):
             if name in astroid.instance_attrs:
                 yield astroid
 
-    def has_base(self, node):
+    def has_base(self, node) -> bool:
         """Whether this class directly inherits from the given node.
 
         :param node: The node to check for.
         :type node: NodeNG
 
-        :returns: True if this class directly inherits from the given node.
-        :rtype: bool
+        :returns: Whether this class directly inherits from the given node.
         """
         return node in self.bases
 
-    def local_attr(self, name, context=None):
+    def local_attr(self, name, context: InferenceContext | None = None):
         """Get the list of assign nodes associated to the given name.
 
         Assignments are looked for in both this class and in parents.
 
         :returns: The list of assignments to the given name.
         :rtype: list(NodeNG)
 
@@ -2650,15 +2328,15 @@
             if class_node:
                 result = class_node.locals[name]
         result = [n for n in result if not isinstance(n, node_classes.DelAttr)]
         if result:
             return result
         raise AttributeInferenceError(target=self, attribute=name, context=context)
 
-    def instance_attr(self, name, context=None):
+    def instance_attr(self, name, context: InferenceContext | None = None):
         """Get the list of nodes associated to the given attribute name.
 
         Assignments are looked for in both this class and in parents.
 
         :returns: The list of assignments to the given name.
         :rtype: list(NodeNG)
 
@@ -2672,30 +2350,35 @@
         for class_node in self.instance_attr_ancestors(name, context):
             values += class_node.instance_attrs[name]
         values = [n for n in values if not isinstance(n, node_classes.DelAttr)]
         if values:
             return values
         raise AttributeInferenceError(target=self, attribute=name, context=context)
 
-    def instantiate_class(self):
+    def instantiate_class(self) -> bases.Instance:
         """Get an :class:`Instance` of the :class:`ClassDef` node.
 
-        :returns: An :class:`Instance` of the :class:`ClassDef` node,
-            or self if this is not possible.
-        :rtype: Instance or ClassDef
+        :returns: An :class:`Instance` of the :class:`ClassDef` node
         """
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         try:
             if any(cls.name in EXCEPTION_BASE_CLASSES for cls in self.mro()):
                 # Subclasses of exceptions can be exception instances
                 return objects.ExceptionInstance(self)
         except MroError:
             pass
         return bases.Instance(self)
 
-    def getattr(self, name, context=None, class_context=True):
+    def getattr(
+        self,
+        name: str,
+        context: InferenceContext | None = None,
+        class_context: bool = True,
+    ) -> list[SuccessfulInferenceResult]:
         """Get an attribute from this class, using Python's attribute semantic.
 
         This method doesn't look in the :attr:`instance_attrs` dictionary
         since it is done by an :class:`Instance` proxy at inference time.
         It may return an :class:`Uninferable` object if
         the attribute has not been
         found, but a ``__getattr__`` or ``__getattribute__`` method is defined.
@@ -2703,70 +2386,68 @@
         attribute is accessed from a class context,
         e.g. ClassDef.attribute, otherwise it might have been accessed
         from an instance as well. If ``class_context`` is used in that
         case, then a lookup in the implicit metaclass and the explicit
         metaclass will be done.
 
         :param name: The attribute to look for.
-        :type name: str
 
         :param class_context: Whether the attribute can be accessed statically.
-        :type class_context: bool
 
         :returns: The attribute.
-        :rtype: list(NodeNG)
 
         :raises AttributeInferenceError: If the attribute cannot be inferred.
         """
         if not name:
             raise AttributeInferenceError(target=self, attribute=name, context=context)
 
-        values = self.locals.get(name, [])
+        # don't modify the list in self.locals!
+        values: list[SuccessfulInferenceResult] = list(self.locals.get(name, []))
+        for classnode in self.ancestors(recurs=True, context=context):
+            values += classnode.locals.get(name, [])
+
         if name in self.special_attributes and class_context and not values:
             result = [self.special_attributes.lookup(name)]
             if name == "__bases__":
                 # Need special treatment, since they are mutable
                 # and we need to return all the values.
                 result += values
             return result
 
-        # don't modify the list in self.locals!
-        values = list(values)
-        for classnode in self.ancestors(recurs=True, context=context):
-            values += classnode.locals.get(name, [])
-
         if class_context:
             values += self._metaclass_lookup_attribute(name, context)
 
-        if not values:
-            raise AttributeInferenceError(target=self, attribute=name, context=context)
-
-        # Look for AnnAssigns, which are not attributes in the purest sense.
-        for value in values:
+        # Remove AnnAssigns without value, which are not attributes in the purest sense.
+        for value in values.copy():
             if isinstance(value, node_classes.AssignName):
                 stmt = value.statement(future=True)
                 if isinstance(stmt, node_classes.AnnAssign) and stmt.value is None:
-                    raise AttributeInferenceError(
-                        target=self, attribute=name, context=context
-                    )
+                    values.pop(values.index(value))
+
+        if not values:
+            raise AttributeInferenceError(target=self, attribute=name, context=context)
+
         return values
 
+    @lru_cache(maxsize=1024)  # noqa
     def _metaclass_lookup_attribute(self, name, context):
         """Search the given name in the implicit and the explicit metaclass."""
         attrs = set()
         implicit_meta = self.implicit_metaclass()
         context = copy_context(context)
         metaclass = self.metaclass(context=context)
         for cls in (implicit_meta, metaclass):
             if cls and cls != self and isinstance(cls, ClassDef):
                 cls_attributes = self._get_attribute_from_metaclass(cls, name, context)
                 attrs.update(set(cls_attributes))
         return attrs
 
     def _get_attribute_from_metaclass(self, cls, name, context):
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         try:
             attrs = cls.getattr(name, context=context, class_context=True)
         except AttributeInferenceError:
             return
 
         for attr in bases._infer_stmts(attrs, context, frame=cls):
             if not isinstance(attr, FunctionDef):
@@ -2785,23 +2466,28 @@
                 frame = get_wrapping_class(attr) or self
                 yield bases.BoundMethod(attr, frame)
             elif attr.type == "staticmethod":
                 yield attr
             else:
                 yield bases.BoundMethod(attr, self)
 
-    def igetattr(self, name, context=None, class_context=True):
+    def igetattr(
+        self,
+        name: str,
+        context: InferenceContext | None = None,
+        class_context: bool = True,
+    ) -> Iterator[InferenceResult]:
         """Infer the possible values of the given variable.
 
         :param name: The name of the variable to infer.
-        :type name: str
 
         :returns: The inferred possible values.
-        :rtype: iterable(NodeNG or Uninferable)
         """
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
         # set lookup name since this is necessary to infer on import nodes for
         # instance
         context = copy_context(context)
         context.lookupname = name
 
         metaclass = self.metaclass(context=context)
         try:
@@ -2856,24 +2542,22 @@
                 # class handle some dynamic attributes, return a Uninferable object
                 yield util.Uninferable
             else:
                 raise InferenceError(
                     str(error), target=self, attribute=name, context=context
                 ) from error
 
-    def has_dynamic_getattr(self, context=None):
+    def has_dynamic_getattr(self, context: InferenceContext | None = None) -> bool:
         """Check if the class has a custom __getattr__ or __getattribute__.
 
         If any such method is found and it is not from
         builtins, nor from an extension module, then the function
         will return True.
 
-        :returns: True if the class has a custom
-            __getattr__ or __getattribute__, False otherwise.
-        :rtype: bool
+        :returns: Whether the class has a custom __getattr__ or __getattribute__.
         """
 
         def _valid_getattr(node):
             root = node.root()
             return root.name != "builtins" and getattr(root, "pure_python", None)
 
         try:
@@ -2883,15 +2567,15 @@
             try:
                 getattribute = self.getattr("__getattribute__", context)[0]
                 return _valid_getattr(getattribute)
             except AttributeInferenceError:
                 pass
         return False
 
-    def getitem(self, index, context=None):
+    def getitem(self, index, context: InferenceContext | None = None):
         """Return the inference of a subscript.
 
         This is basically looking up the method in the metaclass and calling it.
 
         :returns: The inferred value of a subscript to this class.
         :rtype: NodeNG
 
@@ -2928,15 +2612,15 @@
             # Starting with python3.9, builtin types list, dict etc...
             # are subscriptable thanks to __class_getitem___ classmethod.
             # However in such case the method is bound to an EmptyNode and
             # EmptyNode doesn't have infer_call_result method yielding to
             # AttributeError
             if (
                 isinstance(method, node_classes.EmptyNode)
-                and self.name in {"list", "dict", "set", "tuple", "frozenset"}
+                and self.pytype() == "builtins.type"
                 and PY39_PLUS
             ):
                 return self
             raise
         except InferenceError:
             return util.Uninferable
 
@@ -2974,28 +2658,27 @@
         :returns: The metaclass.
         :rtype: builtins.type or None
         """
         if self.newstyle:
             return builtin_lookup("type")[1][0]
         return None
 
-    _metaclass = None
-
-    def declared_metaclass(self, context=None):
+    def declared_metaclass(
+        self, context: InferenceContext | None = None
+    ) -> SuccessfulInferenceResult | None:
         """Return the explicit declared metaclass for the current class.
 
         An explicit declared metaclass is defined
         either by passing the ``metaclass`` keyword argument
         in the class definition line (Python 3) or (Python 2) by
         having a ``__metaclass__`` class attribute, or if there are
         no explicit bases but there is a global ``__metaclass__`` variable.
 
         :returns: The metaclass of this class,
             or None if one could not be found.
-        :rtype: NodeNG or None
         """
         for base in self.bases:
             try:
                 for baseobj in base.infer(context=context):
                     if isinstance(baseobj, ClassDef) and baseobj.hide:
                         self._metaclass = baseobj._metaclass
                         self._metaclass_hack = True
@@ -3005,44 +2688,47 @@
 
         if self._metaclass:
             # Expects this from Py3k TreeRebuilder
             try:
                 return next(
                     node
                     for node in self._metaclass.infer(context=context)
-                    if node is not util.Uninferable
+                    if not isinstance(node, util.UninferableBase)
                 )
             except (InferenceError, StopIteration):
                 return None
 
         return None
 
-    def _find_metaclass(self, seen=None, context=None):
+    def _find_metaclass(
+        self, seen: set[ClassDef] | None = None, context: InferenceContext | None = None
+    ) -> SuccessfulInferenceResult | None:
         if seen is None:
             seen = set()
         seen.add(self)
 
         klass = self.declared_metaclass(context=context)
         if klass is None:
             for parent in self.ancestors(context=context):
                 if parent not in seen:
                     klass = parent._find_metaclass(seen)
                     if klass is not None:
                         break
         return klass
 
-    def metaclass(self, context=None):
+    def metaclass(
+        self, context: InferenceContext | None = None
+    ) -> SuccessfulInferenceResult | None:
         """Get the metaclass of this class.
 
         If this class does not define explicitly a metaclass,
         then the first defined metaclass in ancestors will be used
         instead.
 
         :returns: The metaclass of this class.
-        :rtype: NodeNG or None
         """
         return self._find_metaclass(context=context)
 
     def has_metaclass_hack(self):
         return self._metaclass_hack
 
     def _islots(self):
@@ -3070,26 +2756,24 @@
                 # we can't obtain the values, maybe a .deque?
                 continue
 
             if isinstance(slots, node_classes.Dict):
                 values = [item[0] for item in slots.items]
             else:
                 values = slots.itered()
-            if values is util.Uninferable:
+            if isinstance(values, util.UninferableBase):
                 continue
             if not values:
                 # Stop the iteration, because the class
                 # has an empty list of slots.
                 return values
 
             for elt in values:
                 try:
                     for inferred in elt.infer():
-                        if inferred is util.Uninferable:
-                            continue
                         if not isinstance(
                             inferred, node_classes.Const
                         ) or not isinstance(inferred.value, str):
                             continue
                         if not inferred.value:
                             continue
                         yield inferred
@@ -3108,33 +2792,35 @@
         try:
             first = next(slots)
         except StopIteration as exc:
             # The class doesn't have a __slots__ definition or empty slots.
             if exc.args and exc.args[0] not in ("", None):
                 return exc.args[0]
             return None
-        return [first] + list(slots)
+        return [first, *slots]
 
     # Cached, because inferring them all the time is expensive
-    @decorators_mod.cached
-    def slots(self):
+    @cached_property
+    def _all_slots(self):
         """Get all the slots for this node.
 
         :returns: The names of slots for this class.
             If the class doesn't define any slot, through the ``__slots__``
             variable, then this function will return a None.
             Also, it will return None in the case the slots were not inferred.
         :rtype: list(str) or None
         """
 
         def grouped_slots(
-            mro: List["ClassDef"],
-        ) -> typing.Iterator[Optional[node_classes.NodeNG]]:
-            # Not interested in object, since it can't have slots.
-            for cls in mro[:-1]:
+            mro: list[ClassDef],
+        ) -> Iterator[node_classes.NodeNG | None]:
+            for cls in mro:
+                # Not interested in object, since it can't have slots.
+                if cls.qname() == "builtins.object":
+                    continue
                 try:
                     cls_slots = cls._slots()
                 except NotImplementedError:
                     continue
                 if cls_slots is not None:
                     yield from cls_slots
                 else:
@@ -3154,15 +2840,18 @@
 
         slots = list(grouped_slots(mro))
         if not all(slot is not None for slot in slots):
             return None
 
         return sorted(set(slots), key=lambda item: item.value)
 
-    def _inferred_bases(self, context=None):
+    def slots(self):
+        return self._all_slots
+
+    def _inferred_bases(self, context: InferenceContext | None = None):
         # Similar with .ancestors, but the difference is when one base is inferred,
         # only the first object is wanted. That's because
         # we aren't interested in superclasses, as in the following
         # example:
         #
         # class SomeSuperClass(object): pass
         # class SomeClass(SomeSuperClass): pass
@@ -3193,15 +2882,15 @@
             if not isinstance(baseobj, ClassDef):
                 continue
             if not baseobj.hide:
                 yield baseobj
             else:
                 yield from baseobj.bases
 
-    def _compute_mro(self, context=None):
+    def _compute_mro(self, context: InferenceContext | None = None):
         inferred_bases = list(self._inferred_bases(context=context))
         bases_mro = []
         for base in inferred_bases:
             if base is self:
                 continue
 
             try:
@@ -3212,55 +2901,54 @@
                 # old style classes. For these we can't retrieve the .mro,
                 # although in Python it's possible, since the class we are
                 # currently working is in fact new style.
                 # So, we fallback to ancestors here.
                 ancestors = list(base.ancestors(context=context))
                 bases_mro.append(ancestors)
 
-        unmerged_mro = [[self]] + bases_mro + [inferred_bases]
+        unmerged_mro = [[self], *bases_mro, inferred_bases]
         unmerged_mro = list(clean_duplicates_mro(unmerged_mro, self, context))
         clean_typing_generic_mro(unmerged_mro)
         return _c3_merge(unmerged_mro, self, context)
 
-    def mro(self, context=None) -> List["ClassDef"]:
+    def mro(self, context: InferenceContext | None = None) -> list[ClassDef]:
         """Get the method resolution order, using C3 linearization.
 
         :returns: The list of ancestors, sorted by the mro.
         :rtype: list(NodeNG)
         :raises DuplicateBasesError: Duplicate bases in the same class base
         :raises InconsistentMroError: A class' MRO is inconsistent
         """
         return self._compute_mro(context=context)
 
-    def bool_value(self, context=None):
+    def bool_value(self, context: InferenceContext | None = None) -> Literal[True]:
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
             For a :class:`ClassDef` this is always ``True``.
-        :rtype: bool
         """
         return True
 
     def get_children(self):
         if self.decorators is not None:
             yield self.decorators
 
         yield from self.bases
         if self.keywords is not None:
             yield from self.keywords
         yield from self.body
 
-    @decorators_mod.cached
-    def _get_assign_nodes(self):
+    @cached_property
+    def _assign_nodes_in_scope(self):
         children_assign_nodes = (
-            child_node._get_assign_nodes() for child_node in self.body
+            child_node._assign_nodes_in_scope for child_node in self.body
         )
         return list(itertools.chain.from_iterable(children_assign_nodes))
 
-    def frame(self: T, *, future: Literal[None, True] = None) -> T:
+    def frame(self: _T, *, future: Literal[None, True] = None) -> _T:
         """The node's frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/rebuilder.py` & `astroid-3.0.0a1/astroid/rebuilder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,34 @@
-# Copyright (c) 2009-2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2013-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2014 Alexander Presnyakov <flagist0@gmail.com>
-# Copyright (c) 2014 Eevee (Alex Munroe) <amunroe@yelp.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016-2017 Derek Gustafson <degustaf@gmail.com>
-# Copyright (c) 2016 Jared Garst <jgarst@users.noreply.github.com>
-# Copyright (c) 2017 Hugo <hugovk@users.noreply.github.com>
-# Copyright (c) 2017 Łukasz Rogalski <rogalski.91@gmail.com>
-# Copyright (c) 2017 rr- <rr-@sakuya.pl>
-# Copyright (c) 2018-2019 Ville Skyttä <ville.skytta@iki.fi>
-# Copyright (c) 2018 Tomas Gavenciak <gavento@ucw.cz>
-# Copyright (c) 2018 Serhiy Storchaka <storchaka@gmail.com>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2019-2021 Ashley Whetter <ashley@awhetter.co.uk>
-# Copyright (c) 2019 Hugo van Kemenade <hugovk@users.noreply.github.com>
-# Copyright (c) 2019 Zbigniew Jędrzejewski-Szmek <zbyszek@in.waw.pl>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Daniël van Noord <13665637+DanielNoord@users.noreply.github.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Federico Bond <federicobond@gmail.com>
-# Copyright (c) 2021 hippo91 <guillaume.peillex@gmail.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
-"""this module contains utilities for rebuilding an _ast tree in
-order to get a single Astroid representation
+"""This module contains utilities for rebuilding an _ast tree in
+order to get a single Astroid representation.
 """
 
+from __future__ import annotations
+
+import ast
 import sys
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Generator,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+import token
+from collections.abc import Callable, Generator
+from io import StringIO
+from tokenize import TokenInfo, generate_tokens
+from typing import TYPE_CHECKING, Final, TypeVar, Union, cast, overload
 
 from astroid import nodes
 from astroid._ast import ParserModule, get_parser_module, parse_function_type_comment
-from astroid.const import PY38, PY38_PLUS, Context
+from astroid.const import IS_PYPY, PY38, PY39_PLUS, Context
 from astroid.manager import AstroidManager
 from astroid.nodes import NodeNG
+from astroid.nodes.utils import Position
+from astroid.typing import SuccessfulInferenceResult
 
-if sys.version_info >= (3, 8):
-    from typing import Final
-else:
-    from typing_extensions import Final
-
-if TYPE_CHECKING:
-    import ast
-
-
-REDIRECT: Final[Dict[str, str]] = {
+REDIRECT: Final[dict[str, str]] = {
     "arguments": "Arguments",
     "comprehension": "Comprehension",
     "ListCompFor": "Comprehension",
     "GenExprFor": "Comprehension",
     "excepthandler": "ExceptHandler",
     "keyword": "Keyword",
     "match_case": "MatchCase",
@@ -74,758 +37,524 @@
 
 T_Doc = TypeVar(
     "T_Doc",
     "ast.Module",
     "ast.ClassDef",
     Union["ast.FunctionDef", "ast.AsyncFunctionDef"],
 )
-T_Function = TypeVar("T_Function", nodes.FunctionDef, nodes.AsyncFunctionDef)
-T_For = TypeVar("T_For", nodes.For, nodes.AsyncFor)
-T_With = TypeVar("T_With", nodes.With, nodes.AsyncWith)
+_FunctionT = TypeVar("_FunctionT", nodes.FunctionDef, nodes.AsyncFunctionDef)
+_ForT = TypeVar("_ForT", nodes.For, nodes.AsyncFor)
+_WithT = TypeVar("_WithT", nodes.With, nodes.AsyncWith)
+NodesWithDocsType = Union[nodes.Module, nodes.ClassDef, nodes.FunctionDef]
 
 
 # noinspection PyMethodMayBeStatic
 class TreeRebuilder:
-    """Rebuilds the _ast tree to become an Astroid tree"""
+    """Rebuilds the _ast tree to become an Astroid tree."""
 
     def __init__(
-        self, manager: AstroidManager, parser_module: Optional[ParserModule] = None
-    ):
+        self,
+        manager: AstroidManager,
+        parser_module: ParserModule | None = None,
+        data: str | None = None,
+    ) -> None:
         self._manager = manager
-        self._global_names: List[Dict[str, List[nodes.Global]]] = []
-        self._import_from_nodes: List[nodes.ImportFrom] = []
-        self._delayed_assattr: List[nodes.AssignAttr] = []
-        self._visit_meths: Dict[
-            Type["ast.AST"], Callable[["ast.AST", NodeNG], NodeNG]
-        ] = {}
+        self._data = data.split("\n") if data else None
+        self._global_names: list[dict[str, list[nodes.Global]]] = []
+        self._import_from_nodes: list[nodes.ImportFrom] = []
+        self._delayed_assattr: list[nodes.AssignAttr] = []
+        self._visit_meths: dict[type[ast.AST], Callable[[ast.AST, NodeNG], NodeNG]] = {}
 
         if parser_module is None:
             self._parser_module = get_parser_module()
         else:
             self._parser_module = parser_module
-        self._module = self._parser_module.module
 
-    def _get_doc(self, node: T_Doc) -> Tuple[T_Doc, Optional[str]]:
+    def _get_doc(self, node: T_Doc) -> tuple[T_Doc, ast.Constant | ast.Str | None]:
+        """Return the doc ast node."""
         try:
-            if node.body and isinstance(node.body[0], self._module.Expr):
+            if node.body and isinstance(node.body[0], ast.Expr):
                 first_value = node.body[0].value
-                if isinstance(first_value, self._module.Str) or (
-                    PY38_PLUS
-                    and isinstance(first_value, self._module.Constant)
-                    and isinstance(first_value.value, str)
+                if isinstance(first_value, ast.Constant) and isinstance(
+                    first_value.value, str
                 ):
-                    doc = first_value.value if PY38_PLUS else first_value.s
+                    doc_ast_node = first_value
                     node.body = node.body[1:]
-                    return node, doc
+                    # The ast parser of python < 3.8 sets col_offset of multi-line strings to -1
+                    # as it is unable to determine the value correctly. We reset this to None.
+                    if doc_ast_node.col_offset == -1:
+                        doc_ast_node.col_offset = None
+                    return node, doc_ast_node
         except IndexError:
             pass  # ast built from scratch
         return node, None
 
     def _get_context(
         self,
-        node: Union[
-            "ast.Attribute",
-            "ast.List",
-            "ast.Name",
-            "ast.Subscript",
-            "ast.Starred",
-            "ast.Tuple",
-        ],
+        node: (
+            ast.Attribute
+            | ast.List
+            | ast.Name
+            | ast.Subscript
+            | ast.Starred
+            | ast.Tuple
+        ),
     ) -> Context:
         return self._parser_module.context_classes.get(type(node.ctx), Context.Load)
 
+    def _get_position_info(
+        self,
+        node: ast.ClassDef | ast.FunctionDef | ast.AsyncFunctionDef,
+        parent: nodes.ClassDef | nodes.FunctionDef | nodes.AsyncFunctionDef,
+    ) -> Position | None:
+        """Return position information for ClassDef and FunctionDef nodes.
+
+        In contrast to AST positions, these only include the actual keyword(s)
+        and the class / function name.
+
+        >>> @decorator
+        >>> async def some_func(var: int) -> None:
+        >>> ^^^^^^^^^^^^^^^^^^^
+        """
+        if not self._data:
+            return None
+        end_lineno = node.end_lineno
+        if node.body:
+            end_lineno = node.body[0].lineno
+        # pylint: disable-next=unsubscriptable-object
+        data = "\n".join(self._data[node.lineno - 1 : end_lineno])
+
+        start_token: TokenInfo | None = None
+        keyword_tokens: tuple[int, ...] = (token.NAME,)
+        if isinstance(parent, nodes.AsyncFunctionDef):
+            search_token = "async"
+        elif isinstance(parent, nodes.FunctionDef):
+            search_token = "def"
+        else:
+            search_token = "class"
+
+        for t in generate_tokens(StringIO(data).readline):
+            if (
+                start_token is not None
+                and t.type == token.NAME
+                and t.string == node.name
+            ):
+                break
+            if t.type in keyword_tokens:
+                if t.string == search_token:
+                    start_token = t
+                    continue
+                if t.string in {"def"}:
+                    continue
+            start_token = None
+        else:
+            return None
+
+        return Position(
+            lineno=node.lineno + start_token.start[0] - 1,
+            col_offset=start_token.start[1],
+            end_lineno=node.lineno + t.end[0] - 1,
+            end_col_offset=t.end[1],
+        )
+
+    def _reset_end_lineno(self, newnode: nodes.NodeNG) -> None:
+        """Reset end_lineno and end_col_offset attributes for PyPy 3.8.
+
+        For some nodes, these are either set to -1 or only partially assigned.
+        To keep consistency across astroid and pylint, reset all.
+
+        This has been fixed in PyPy 3.9.
+        For reference, an (incomplete) list of nodes with issues:
+            - ClassDef          - For
+            - FunctionDef       - While
+            - Call              - If
+            - Decorators        - TryExcept
+            - With              - TryFinally
+            - Assign
+        """
+        newnode.end_lineno = None
+        newnode.end_col_offset = None
+        for child_node in newnode.get_children():
+            self._reset_end_lineno(child_node)
+
     def visit_module(
-        self, node: "ast.Module", modname: str, modpath: str, package: bool
+        self, node: ast.Module, modname: str, modpath: str, package: bool
     ) -> nodes.Module:
-        """visit a Module node by returning a fresh instance of it
+        """Visit a Module node by returning a fresh instance of it.
 
         Note: Method not called by 'visit'
         """
-        node, doc = self._get_doc(node)
+        node, doc_ast_node = self._get_doc(node)
         newnode = nodes.Module(
             name=modname,
-            doc=doc,
             file=modpath,
             path=[modpath],
             package=package,
-            parent=None,
         )
-        newnode.postinit([self.visit(child, newnode) for child in node.body])
+        newnode.postinit(
+            [self.visit(child, newnode) for child in node.body],
+            doc_node=self.visit(doc_ast_node, newnode),
+        )
+        if IS_PYPY and PY38:
+            self._reset_end_lineno(newnode)
         return newnode
 
-    if sys.version_info >= (3, 10):
+    if TYPE_CHECKING:  # noqa: C901
 
         @overload
-        def visit(self, node: "ast.arg", parent: NodeNG) -> nodes.AssignName:
+        def visit(self, node: ast.arg, parent: NodeNG) -> nodes.AssignName:
             ...
 
         @overload
-        def visit(self, node: "ast.arguments", parent: NodeNG) -> nodes.Arguments:
+        def visit(self, node: ast.arguments, parent: NodeNG) -> nodes.Arguments:
             ...
 
         @overload
-        def visit(self, node: "ast.Assert", parent: NodeNG) -> nodes.Assert:
+        def visit(self, node: ast.Assert, parent: NodeNG) -> nodes.Assert:
             ...
 
         @overload
         def visit(
-            self, node: "ast.AsyncFunctionDef", parent: NodeNG
+            self, node: ast.AsyncFunctionDef, parent: NodeNG
         ) -> nodes.AsyncFunctionDef:
             ...
 
         @overload
-        def visit(self, node: "ast.AsyncFor", parent: NodeNG) -> nodes.AsyncFor:
+        def visit(self, node: ast.AsyncFor, parent: NodeNG) -> nodes.AsyncFor:
             ...
 
         @overload
-        def visit(self, node: "ast.Await", parent: NodeNG) -> nodes.Await:
+        def visit(self, node: ast.Await, parent: NodeNG) -> nodes.Await:
             ...
 
         @overload
-        def visit(self, node: "ast.AsyncWith", parent: NodeNG) -> nodes.AsyncWith:
+        def visit(self, node: ast.AsyncWith, parent: NodeNG) -> nodes.AsyncWith:
             ...
 
         @overload
-        def visit(self, node: "ast.Assign", parent: NodeNG) -> nodes.Assign:
+        def visit(self, node: ast.Assign, parent: NodeNG) -> nodes.Assign:
             ...
 
         @overload
-        def visit(self, node: "ast.AnnAssign", parent: NodeNG) -> nodes.AnnAssign:
+        def visit(self, node: ast.AnnAssign, parent: NodeNG) -> nodes.AnnAssign:
             ...
 
         @overload
-        def visit(self, node: "ast.AugAssign", parent: NodeNG) -> nodes.AugAssign:
+        def visit(self, node: ast.AugAssign, parent: NodeNG) -> nodes.AugAssign:
             ...
 
         @overload
-        def visit(self, node: "ast.BinOp", parent: NodeNG) -> nodes.BinOp:
+        def visit(self, node: ast.BinOp, parent: NodeNG) -> nodes.BinOp:
             ...
 
         @overload
-        def visit(self, node: "ast.BoolOp", parent: NodeNG) -> nodes.BoolOp:
+        def visit(self, node: ast.BoolOp, parent: NodeNG) -> nodes.BoolOp:
             ...
 
         @overload
-        def visit(self, node: "ast.Break", parent: NodeNG) -> nodes.Break:
+        def visit(self, node: ast.Break, parent: NodeNG) -> nodes.Break:
             ...
 
         @overload
-        def visit(self, node: "ast.Call", parent: NodeNG) -> nodes.Call:
+        def visit(self, node: ast.Call, parent: NodeNG) -> nodes.Call:
             ...
 
         @overload
-        def visit(self, node: "ast.ClassDef", parent: NodeNG) -> nodes.ClassDef:
+        def visit(self, node: ast.ClassDef, parent: NodeNG) -> nodes.ClassDef:
             ...
 
         @overload
-        def visit(self, node: "ast.Continue", parent: NodeNG) -> nodes.Continue:
+        def visit(self, node: ast.Continue, parent: NodeNG) -> nodes.Continue:
             ...
 
         @overload
-        def visit(self, node: "ast.Compare", parent: NodeNG) -> nodes.Compare:
+        def visit(self, node: ast.Compare, parent: NodeNG) -> nodes.Compare:
             ...
 
         @overload
-        def visit(
-            self, node: "ast.comprehension", parent: NodeNG
-        ) -> nodes.Comprehension:
+        def visit(self, node: ast.comprehension, parent: NodeNG) -> nodes.Comprehension:
             ...
 
         @overload
-        def visit(self, node: "ast.Delete", parent: NodeNG) -> nodes.Delete:
+        def visit(self, node: ast.Delete, parent: NodeNG) -> nodes.Delete:
             ...
 
         @overload
-        def visit(self, node: "ast.Dict", parent: NodeNG) -> nodes.Dict:
+        def visit(self, node: ast.Dict, parent: NodeNG) -> nodes.Dict:
             ...
 
         @overload
-        def visit(self, node: "ast.DictComp", parent: NodeNG) -> nodes.DictComp:
+        def visit(self, node: ast.DictComp, parent: NodeNG) -> nodes.DictComp:
             ...
 
         @overload
-        def visit(self, node: "ast.Expr", parent: NodeNG) -> nodes.Expr:
+        def visit(self, node: ast.Expr, parent: NodeNG) -> nodes.Expr:
             ...
 
-        # Not used in Python 3.8+
         @overload
-        def visit(self, node: "ast.Ellipsis", parent: NodeNG) -> nodes.Const:
+        def visit(self, node: ast.ExceptHandler, parent: NodeNG) -> nodes.ExceptHandler:
             ...
 
         @overload
-        def visit(
-            self, node: "ast.ExceptHandler", parent: NodeNG
-        ) -> nodes.ExceptHandler:
+        def visit(self, node: ast.For, parent: NodeNG) -> nodes.For:
             ...
 
-        # Not used in Python 3.9+
         @overload
-        def visit(self, node: "ast.ExtSlice", parent: nodes.Subscript) -> nodes.Tuple:
+        def visit(self, node: ast.ImportFrom, parent: NodeNG) -> nodes.ImportFrom:
             ...
 
         @overload
-        def visit(self, node: "ast.For", parent: NodeNG) -> nodes.For:
+        def visit(self, node: ast.FunctionDef, parent: NodeNG) -> nodes.FunctionDef:
             ...
 
         @overload
-        def visit(self, node: "ast.ImportFrom", parent: NodeNG) -> nodes.ImportFrom:
+        def visit(self, node: ast.GeneratorExp, parent: NodeNG) -> nodes.GeneratorExp:
             ...
 
         @overload
-        def visit(self, node: "ast.FunctionDef", parent: NodeNG) -> nodes.FunctionDef:
+        def visit(self, node: ast.Attribute, parent: NodeNG) -> nodes.Attribute:
             ...
 
         @overload
-        def visit(self, node: "ast.GeneratorExp", parent: NodeNG) -> nodes.GeneratorExp:
+        def visit(self, node: ast.Global, parent: NodeNG) -> nodes.Global:
             ...
 
         @overload
-        def visit(self, node: "ast.Attribute", parent: NodeNG) -> nodes.Attribute:
+        def visit(self, node: ast.If, parent: NodeNG) -> nodes.If:
             ...
 
         @overload
-        def visit(self, node: "ast.Global", parent: NodeNG) -> nodes.Global:
+        def visit(self, node: ast.IfExp, parent: NodeNG) -> nodes.IfExp:
             ...
 
         @overload
-        def visit(self, node: "ast.If", parent: NodeNG) -> nodes.If:
+        def visit(self, node: ast.Import, parent: NodeNG) -> nodes.Import:
             ...
 
         @overload
-        def visit(self, node: "ast.IfExp", parent: NodeNG) -> nodes.IfExp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Import", parent: NodeNG) -> nodes.Import:
-            ...
-
-        @overload
-        def visit(self, node: "ast.JoinedStr", parent: NodeNG) -> nodes.JoinedStr:
+        def visit(self, node: ast.JoinedStr, parent: NodeNG) -> nodes.JoinedStr:
             ...
 
         @overload
         def visit(
-            self, node: "ast.FormattedValue", parent: NodeNG
+            self, node: ast.FormattedValue, parent: NodeNG
         ) -> nodes.FormattedValue:
             ...
 
         @overload
-        def visit(self, node: "ast.NamedExpr", parent: NodeNG) -> nodes.NamedExpr:
-            ...
-
-        # Not used in Python 3.9+
-        @overload
-        def visit(self, node: "ast.Index", parent: nodes.Subscript) -> NodeNG:
-            ...
-
-        @overload
-        def visit(self, node: "ast.keyword", parent: NodeNG) -> nodes.Keyword:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Lambda", parent: NodeNG) -> nodes.Lambda:
-            ...
-
-        @overload
-        def visit(self, node: "ast.List", parent: NodeNG) -> nodes.List:
-            ...
-
-        @overload
-        def visit(self, node: "ast.ListComp", parent: NodeNG) -> nodes.ListComp:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.Name", parent: NodeNG
-        ) -> Union[nodes.Name, nodes.Const, nodes.AssignName, nodes.DelName]:
-            ...
-
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.NameConstant", parent: NodeNG) -> nodes.Const:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Nonlocal", parent: NodeNG) -> nodes.Nonlocal:
-            ...
-
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.Str", parent: NodeNG) -> nodes.Const:
-            ...
-
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.Bytes", parent: NodeNG) -> nodes.Const:
-            ...
-
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.Num", parent: NodeNG) -> nodes.Const:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Constant", parent: NodeNG) -> nodes.Const:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Pass", parent: NodeNG) -> nodes.Pass:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Raise", parent: NodeNG) -> nodes.Raise:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Return", parent: NodeNG) -> nodes.Return:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Set", parent: NodeNG) -> nodes.Set:
-            ...
-
-        @overload
-        def visit(self, node: "ast.SetComp", parent: NodeNG) -> nodes.SetComp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Slice", parent: nodes.Subscript) -> nodes.Slice:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Subscript", parent: NodeNG) -> nodes.Subscript:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Starred", parent: NodeNG) -> nodes.Starred:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.Try", parent: NodeNG
-        ) -> Union[nodes.TryExcept, nodes.TryFinally]:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Tuple", parent: NodeNG) -> nodes.Tuple:
-            ...
-
-        @overload
-        def visit(self, node: "ast.UnaryOp", parent: NodeNG) -> nodes.UnaryOp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.While", parent: NodeNG) -> nodes.While:
-            ...
-
-        @overload
-        def visit(self, node: "ast.With", parent: NodeNG) -> nodes.With:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Yield", parent: NodeNG) -> nodes.Yield:
-            ...
-
-        @overload
-        def visit(self, node: "ast.YieldFrom", parent: NodeNG) -> nodes.YieldFrom:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Match", parent: NodeNG) -> nodes.Match:
-            ...
-
-        @overload
-        def visit(self, node: "ast.match_case", parent: NodeNG) -> nodes.MatchCase:
-            ...
-
-        @overload
-        def visit(self, node: "ast.MatchValue", parent: NodeNG) -> nodes.MatchValue:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.MatchSingleton", parent: NodeNG
-        ) -> nodes.MatchSingleton:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.MatchSequence", parent: NodeNG
-        ) -> nodes.MatchSequence:
-            ...
-
-        @overload
-        def visit(self, node: "ast.MatchMapping", parent: NodeNG) -> nodes.MatchMapping:
+        def visit(self, node: ast.NamedExpr, parent: NodeNG) -> nodes.NamedExpr:
             ...
 
-        @overload
-        def visit(self, node: "ast.MatchClass", parent: NodeNG) -> nodes.MatchClass:
-            ...
-
-        @overload
-        def visit(self, node: "ast.MatchStar", parent: NodeNG) -> nodes.MatchStar:
-            ...
-
-        @overload
-        def visit(self, node: "ast.MatchAs", parent: NodeNG) -> nodes.MatchAs:
-            ...
+        if sys.version_info < (3, 9):
+            # Not used in Python 3.9+
+            @overload
+            def visit(self, node: ast.ExtSlice, parent: nodes.Subscript) -> nodes.Tuple:
+                ...
 
-        @overload
-        def visit(self, node: "ast.MatchOr", parent: NodeNG) -> nodes.MatchOr:
-            ...
-
-        @overload
-        def visit(self, node: "ast.pattern", parent: NodeNG) -> nodes.Pattern:
-            ...
-
-        @overload
-        def visit(self, node: "ast.AST", parent: NodeNG) -> NodeNG:
-            ...
+            @overload
+            def visit(self, node: ast.Index, parent: nodes.Subscript) -> NodeNG:
+                ...
 
         @overload
-        def visit(self, node: None, parent: NodeNG) -> None:
+        def visit(self, node: ast.keyword, parent: NodeNG) -> nodes.Keyword:
             ...
 
-        def visit(self, node: Optional["ast.AST"], parent: NodeNG) -> Optional[NodeNG]:
-            if node is None:
-                return None
-            cls = node.__class__
-            if cls in self._visit_meths:
-                visit_method = self._visit_meths[cls]
-            else:
-                cls_name = cls.__name__
-                visit_name = "visit_" + REDIRECT.get(cls_name, cls_name).lower()
-                visit_method = getattr(self, visit_name)
-                self._visit_meths[cls] = visit_method
-            return visit_method(node, parent)
-
-    else:
-
         @overload
-        def visit(self, node: "ast.arg", parent: NodeNG) -> nodes.AssignName:
+        def visit(self, node: ast.Lambda, parent: NodeNG) -> nodes.Lambda:
             ...
 
         @overload
-        def visit(self, node: "ast.arguments", parent: NodeNG) -> nodes.Arguments:
+        def visit(self, node: ast.List, parent: NodeNG) -> nodes.List:
             ...
 
         @overload
-        def visit(self, node: "ast.Assert", parent: NodeNG) -> nodes.Assert:
+        def visit(self, node: ast.ListComp, parent: NodeNG) -> nodes.ListComp:
             ...
 
         @overload
         def visit(
-            self, node: "ast.AsyncFunctionDef", parent: NodeNG
-        ) -> nodes.AsyncFunctionDef:
-            ...
-
-        @overload
-        def visit(self, node: "ast.AsyncFor", parent: NodeNG) -> nodes.AsyncFor:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Await", parent: NodeNG) -> nodes.Await:
-            ...
-
-        @overload
-        def visit(self, node: "ast.AsyncWith", parent: NodeNG) -> nodes.AsyncWith:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Assign", parent: NodeNG) -> nodes.Assign:
-            ...
-
-        @overload
-        def visit(self, node: "ast.AnnAssign", parent: NodeNG) -> nodes.AnnAssign:
-            ...
-
-        @overload
-        def visit(self, node: "ast.AugAssign", parent: NodeNG) -> nodes.AugAssign:
-            ...
-
-        @overload
-        def visit(self, node: "ast.BinOp", parent: NodeNG) -> nodes.BinOp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.BoolOp", parent: NodeNG) -> nodes.BoolOp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Break", parent: NodeNG) -> nodes.Break:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Call", parent: NodeNG) -> nodes.Call:
-            ...
-
-        @overload
-        def visit(self, node: "ast.ClassDef", parent: NodeNG) -> nodes.ClassDef:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Continue", parent: NodeNG) -> nodes.Continue:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Compare", parent: NodeNG) -> nodes.Compare:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.comprehension", parent: NodeNG
-        ) -> nodes.Comprehension:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Delete", parent: NodeNG) -> nodes.Delete:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Dict", parent: NodeNG) -> nodes.Dict:
-            ...
-
-        @overload
-        def visit(self, node: "ast.DictComp", parent: NodeNG) -> nodes.DictComp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Expr", parent: NodeNG) -> nodes.Expr:
-            ...
-
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.Ellipsis", parent: NodeNG) -> nodes.Const:
-            ...
-
-        @overload
-        def visit(
-            self, node: "ast.ExceptHandler", parent: NodeNG
-        ) -> nodes.ExceptHandler:
-            ...
-
-        # Not used in Python 3.9+
-        @overload
-        def visit(self, node: "ast.ExtSlice", parent: nodes.Subscript) -> nodes.Tuple:
-            ...
-
-        @overload
-        def visit(self, node: "ast.For", parent: NodeNG) -> nodes.For:
-            ...
-
-        @overload
-        def visit(self, node: "ast.ImportFrom", parent: NodeNG) -> nodes.ImportFrom:
-            ...
-
-        @overload
-        def visit(self, node: "ast.FunctionDef", parent: NodeNG) -> nodes.FunctionDef:
-            ...
-
-        @overload
-        def visit(self, node: "ast.GeneratorExp", parent: NodeNG) -> nodes.GeneratorExp:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Attribute", parent: NodeNG) -> nodes.Attribute:
-            ...
-
-        @overload
-        def visit(self, node: "ast.Global", parent: NodeNG) -> nodes.Global:
+            self, node: ast.Name, parent: NodeNG
+        ) -> nodes.Name | nodes.Const | nodes.AssignName | nodes.DelName:
             ...
 
         @overload
-        def visit(self, node: "ast.If", parent: NodeNG) -> nodes.If:
+        def visit(self, node: ast.Nonlocal, parent: NodeNG) -> nodes.Nonlocal:
             ...
 
         @overload
-        def visit(self, node: "ast.IfExp", parent: NodeNG) -> nodes.IfExp:
+        def visit(self, node: ast.Constant, parent: NodeNG) -> nodes.Const:
             ...
 
         @overload
-        def visit(self, node: "ast.Import", parent: NodeNG) -> nodes.Import:
+        def visit(self, node: ast.Pass, parent: NodeNG) -> nodes.Pass:
             ...
 
         @overload
-        def visit(self, node: "ast.JoinedStr", parent: NodeNG) -> nodes.JoinedStr:
+        def visit(self, node: ast.Raise, parent: NodeNG) -> nodes.Raise:
             ...
 
         @overload
-        def visit(
-            self, node: "ast.FormattedValue", parent: NodeNG
-        ) -> nodes.FormattedValue:
-            ...
-
-        @overload
-        def visit(self, node: "ast.NamedExpr", parent: NodeNG) -> nodes.NamedExpr:
+        def visit(self, node: ast.Return, parent: NodeNG) -> nodes.Return:
             ...
 
-        # Not used in Python 3.9+
         @overload
-        def visit(self, node: "ast.Index", parent: nodes.Subscript) -> NodeNG:
+        def visit(self, node: ast.Set, parent: NodeNG) -> nodes.Set:
             ...
 
         @overload
-        def visit(self, node: "ast.keyword", parent: NodeNG) -> nodes.Keyword:
+        def visit(self, node: ast.SetComp, parent: NodeNG) -> nodes.SetComp:
             ...
 
         @overload
-        def visit(self, node: "ast.Lambda", parent: NodeNG) -> nodes.Lambda:
+        def visit(self, node: ast.Slice, parent: nodes.Subscript) -> nodes.Slice:
             ...
 
         @overload
-        def visit(self, node: "ast.List", parent: NodeNG) -> nodes.List:
+        def visit(self, node: ast.Subscript, parent: NodeNG) -> nodes.Subscript:
             ...
 
         @overload
-        def visit(self, node: "ast.ListComp", parent: NodeNG) -> nodes.ListComp:
+        def visit(self, node: ast.Starred, parent: NodeNG) -> nodes.Starred:
             ...
 
         @overload
         def visit(
-            self, node: "ast.Name", parent: NodeNG
-        ) -> Union[nodes.Name, nodes.Const, nodes.AssignName, nodes.DelName]:
+            self, node: ast.Try, parent: NodeNG
+        ) -> nodes.TryExcept | nodes.TryFinally:
             ...
 
-        # Not used in Python 3.8+
-        @overload
-        def visit(self, node: "ast.NameConstant", parent: NodeNG) -> nodes.Const:
-            ...
+        if sys.version_info >= (3, 11):
 
-        @overload
-        def visit(self, node: "ast.Nonlocal", parent: NodeNG) -> nodes.Nonlocal:
-            ...
+            @overload
+            def visit(self, node: ast.TryStar, parent: NodeNG) -> nodes.TryStar:
+                ...
 
-        # Not used in Python 3.8+
         @overload
-        def visit(self, node: "ast.Str", parent: NodeNG) -> nodes.Const:
+        def visit(self, node: ast.Tuple, parent: NodeNG) -> nodes.Tuple:
             ...
 
-        # Not used in Python 3.8+
         @overload
-        def visit(self, node: "ast.Bytes", parent: NodeNG) -> nodes.Const:
+        def visit(self, node: ast.UnaryOp, parent: NodeNG) -> nodes.UnaryOp:
             ...
 
-        # Not used in Python 3.8+
         @overload
-        def visit(self, node: "ast.Num", parent: NodeNG) -> nodes.Const:
+        def visit(self, node: ast.While, parent: NodeNG) -> nodes.While:
             ...
 
         @overload
-        def visit(self, node: "ast.Constant", parent: NodeNG) -> nodes.Const:
+        def visit(self, node: ast.With, parent: NodeNG) -> nodes.With:
             ...
 
         @overload
-        def visit(self, node: "ast.Pass", parent: NodeNG) -> nodes.Pass:
+        def visit(self, node: ast.Yield, parent: NodeNG) -> nodes.Yield:
             ...
 
         @overload
-        def visit(self, node: "ast.Raise", parent: NodeNG) -> nodes.Raise:
+        def visit(self, node: ast.YieldFrom, parent: NodeNG) -> nodes.YieldFrom:
             ...
 
-        @overload
-        def visit(self, node: "ast.Return", parent: NodeNG) -> nodes.Return:
-            ...
+        if sys.version_info >= (3, 10):
 
-        @overload
-        def visit(self, node: "ast.Set", parent: NodeNG) -> nodes.Set:
-            ...
-
-        @overload
-        def visit(self, node: "ast.SetComp", parent: NodeNG) -> nodes.SetComp:
-            ...
+            @overload
+            def visit(self, node: ast.Match, parent: NodeNG) -> nodes.Match:
+                ...
 
-        @overload
-        def visit(self, node: "ast.Slice", parent: nodes.Subscript) -> nodes.Slice:
-            ...
+            @overload
+            def visit(self, node: ast.match_case, parent: NodeNG) -> nodes.MatchCase:
+                ...
 
-        @overload
-        def visit(self, node: "ast.Subscript", parent: NodeNG) -> nodes.Subscript:
-            ...
+            @overload
+            def visit(self, node: ast.MatchValue, parent: NodeNG) -> nodes.MatchValue:
+                ...
 
-        @overload
-        def visit(self, node: "ast.Starred", parent: NodeNG) -> nodes.Starred:
-            ...
+            @overload
+            def visit(
+                self, node: ast.MatchSingleton, parent: NodeNG
+            ) -> nodes.MatchSingleton:
+                ...
 
-        @overload
-        def visit(
-            self, node: "ast.Try", parent: NodeNG
-        ) -> Union[nodes.TryExcept, nodes.TryFinally]:
-            ...
+            @overload
+            def visit(
+                self, node: ast.MatchSequence, parent: NodeNG
+            ) -> nodes.MatchSequence:
+                ...
 
-        @overload
-        def visit(self, node: "ast.Tuple", parent: NodeNG) -> nodes.Tuple:
-            ...
+            @overload
+            def visit(
+                self, node: ast.MatchMapping, parent: NodeNG
+            ) -> nodes.MatchMapping:
+                ...
 
-        @overload
-        def visit(self, node: "ast.UnaryOp", parent: NodeNG) -> nodes.UnaryOp:
-            ...
+            @overload
+            def visit(self, node: ast.MatchClass, parent: NodeNG) -> nodes.MatchClass:
+                ...
 
-        @overload
-        def visit(self, node: "ast.While", parent: NodeNG) -> nodes.While:
-            ...
+            @overload
+            def visit(self, node: ast.MatchStar, parent: NodeNG) -> nodes.MatchStar:
+                ...
 
-        @overload
-        def visit(self, node: "ast.With", parent: NodeNG) -> nodes.With:
-            ...
+            @overload
+            def visit(self, node: ast.MatchAs, parent: NodeNG) -> nodes.MatchAs:
+                ...
 
-        @overload
-        def visit(self, node: "ast.Yield", parent: NodeNG) -> nodes.Yield:
-            ...
+            @overload
+            def visit(self, node: ast.MatchOr, parent: NodeNG) -> nodes.MatchOr:
+                ...
 
-        @overload
-        def visit(self, node: "ast.YieldFrom", parent: NodeNG) -> nodes.YieldFrom:
-            ...
+            @overload
+            def visit(self, node: ast.pattern, parent: NodeNG) -> nodes.Pattern:
+                ...
 
         @overload
-        def visit(self, node: "ast.AST", parent: NodeNG) -> NodeNG:
+        def visit(self, node: ast.AST, parent: NodeNG) -> NodeNG:
             ...
 
         @overload
         def visit(self, node: None, parent: NodeNG) -> None:
             ...
 
-        def visit(self, node: Optional["ast.AST"], parent: NodeNG) -> Optional[NodeNG]:
-            if node is None:
-                return None
-            cls = node.__class__
-            if cls in self._visit_meths:
-                visit_method = self._visit_meths[cls]
-            else:
-                cls_name = cls.__name__
-                visit_name = "visit_" + REDIRECT.get(cls_name, cls_name).lower()
-                visit_method = getattr(self, visit_name)
-                self._visit_meths[cls] = visit_method
-            return visit_method(node, parent)
+    def visit(self, node: ast.AST | None, parent: NodeNG) -> NodeNG | None:
+        if node is None:
+            return None
+        cls = node.__class__
+        if cls in self._visit_meths:
+            visit_method = self._visit_meths[cls]
+        else:
+            cls_name = cls.__name__
+            visit_name = "visit_" + REDIRECT.get(cls_name, cls_name).lower()
+            visit_method = getattr(self, visit_name)
+            self._visit_meths[cls] = visit_method
+        return visit_method(node, parent)
 
-    def _save_assignment(self, node: Union[nodes.AssignName, nodes.DelName]) -> None:
-        """save assignment situation since node.parent is not available yet"""
+    def _save_assignment(self, node: nodes.AssignName | nodes.DelName) -> None:
+        """Save assignment situation since node.parent is not available yet."""
         if self._global_names and node.name in self._global_names[-1]:
             node.root().set_local(node.name, node)
         else:
             assert node.parent
+            assert node.name
             node.parent.set_local(node.name, node)
 
-    def visit_arg(self, node: "ast.arg", parent: NodeNG) -> nodes.AssignName:
-        """visit an arg node by returning a fresh AssName instance"""
+    def visit_arg(self, node: ast.arg, parent: NodeNG) -> nodes.AssignName:
+        """Visit an arg node by returning a fresh AssName instance."""
         return self.visit_assignname(node, parent, node.arg)
 
-    def visit_arguments(self, node: "ast.arguments", parent: NodeNG) -> nodes.Arguments:
-        """visit an Arguments node by returning a fresh instance of it"""
-        vararg: Optional[str] = None
-        kwarg: Optional[str] = None
+    def visit_arguments(self, node: ast.arguments, parent: NodeNG) -> nodes.Arguments:
+        """Visit an Arguments node by returning a fresh instance of it."""
+        vararg: str | None = None
+        kwarg: str | None = None
         newnode = nodes.Arguments(
             node.vararg.arg if node.vararg else None,
             node.kwarg.arg if node.kwarg else None,
             parent,
         )
         args = [self.visit(child, newnode) for child in node.args]
         defaults = [self.visit(child, newnode) for child in node.defaults]
-        varargannotation: Optional[NodeNG] = None
-        kwargannotation: Optional[NodeNG] = None
-        posonlyargs: List[nodes.AssignName] = []
+        varargannotation: NodeNG | None = None
+        kwargannotation: NodeNG | None = None
         if node.vararg:
             vararg = node.vararg.arg
             varargannotation = self.visit(node.vararg.annotation, newnode)
         if node.kwarg:
             kwarg = node.kwarg.arg
             kwargannotation = self.visit(node.kwarg.annotation, newnode)
 
@@ -840,32 +569,27 @@
         kwonlyargs = [self.visit(child, newnode) for child in node.kwonlyargs]
         kw_defaults = [self.visit(child, newnode) for child in node.kw_defaults]
         annotations = [self.visit(arg.annotation, newnode) for arg in node.args]
         kwonlyargs_annotations = [
             self.visit(arg.annotation, newnode) for arg in node.kwonlyargs
         ]
 
-        posonlyargs_annotations: List[Optional[NodeNG]] = []
-        if PY38_PLUS:
-            posonlyargs = [self.visit(child, newnode) for child in node.posonlyargs]
-            posonlyargs_annotations = [
-                self.visit(arg.annotation, newnode) for arg in node.posonlyargs
-            ]
+        posonlyargs = [self.visit(child, newnode) for child in node.posonlyargs]
+        posonlyargs_annotations = [
+            self.visit(arg.annotation, newnode) for arg in node.posonlyargs
+        ]
         type_comment_args = [
             self.check_type_comment(child, parent=newnode) for child in node.args
         ]
         type_comment_kwonlyargs = [
             self.check_type_comment(child, parent=newnode) for child in node.kwonlyargs
         ]
-        type_comment_posonlyargs: List[Optional[NodeNG]] = []
-        if PY38_PLUS:
-            type_comment_posonlyargs = [
-                self.check_type_comment(child, parent=newnode)
-                for child in node.posonlyargs
-            ]
+        type_comment_posonlyargs = [
+            self.check_type_comment(child, parent=newnode) for child in node.posonlyargs
+        ]
 
         newnode.postinit(
             args=args,
             defaults=defaults,
             kwonlyargs=kwonlyargs,
             posonlyargs=posonlyargs,
             kw_defaults=kw_defaults,
@@ -882,314 +606,255 @@
         assert newnode.parent
         if vararg:
             newnode.parent.set_local(vararg, newnode)
         if kwarg:
             newnode.parent.set_local(kwarg, newnode)
         return newnode
 
-    def visit_assert(self, node: "ast.Assert", parent: NodeNG) -> nodes.Assert:
-        """visit a Assert node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Assert(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Assert(node.lineno, node.col_offset, parent)
-        msg: Optional[NodeNG] = None
+    def visit_assert(self, node: ast.Assert, parent: NodeNG) -> nodes.Assert:
+        """Visit a Assert node by returning a fresh instance of it."""
+        newnode = nodes.Assert(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        msg: NodeNG | None = None
         if node.msg:
             msg = self.visit(node.msg, newnode)
         newnode.postinit(self.visit(node.test, newnode), msg)
         return newnode
 
     def check_type_comment(
         self,
-        node: Union[
-            "ast.Assign",
-            "ast.arg",
-            "ast.For",
-            "ast.AsyncFor",
-            "ast.With",
-            "ast.AsyncWith",
-        ],
-        parent: Union[
-            nodes.Assign,
-            nodes.Arguments,
-            nodes.For,
-            nodes.AsyncFor,
-            nodes.With,
-            nodes.AsyncWith,
-        ],
-    ) -> Optional[NodeNG]:
-        type_comment = getattr(node, "type_comment", None)  # Added in Python 3.8
-        if not type_comment:
+        node: (
+            ast.Assign | ast.arg | ast.For | ast.AsyncFor | ast.With | ast.AsyncWith
+        ),
+        parent: (
+            nodes.Assign
+            | nodes.Arguments
+            | nodes.For
+            | nodes.AsyncFor
+            | nodes.With
+            | nodes.AsyncWith
+        ),
+    ) -> NodeNG | None:
+        if not node.type_comment:
             return None
 
         try:
-            type_comment_ast = self._parser_module.parse(type_comment)
+            type_comment_ast = self._parser_module.parse(node.type_comment)
         except SyntaxError:
             # Invalid type comment, just skip it.
             return None
 
+        # For '# type: # any comment' ast.parse returns a Module node,
+        # without any nodes in the body.
+        if not type_comment_ast.body:
+            return None
+
         type_object = self.visit(type_comment_ast.body[0], parent=parent)
         if not isinstance(type_object, nodes.Expr):
             return None
 
         return type_object.value
 
     def check_function_type_comment(
-        self, node: Union["ast.FunctionDef", "ast.AsyncFunctionDef"], parent: NodeNG
-    ) -> Optional[Tuple[Optional[NodeNG], List[NodeNG]]]:
-        type_comment = getattr(node, "type_comment", None)  # Added in Python 3.8
-        if not type_comment:
+        self, node: ast.FunctionDef | ast.AsyncFunctionDef, parent: NodeNG
+    ) -> tuple[NodeNG | None, list[NodeNG]] | None:
+        if not node.type_comment:
             return None
 
         try:
-            type_comment_ast = parse_function_type_comment(type_comment)
+            type_comment_ast = parse_function_type_comment(node.type_comment)
         except SyntaxError:
             # Invalid type comment, just skip it.
             return None
 
         if not type_comment_ast:
             return None
 
-        returns: Optional[NodeNG] = None
-        argtypes: List[NodeNG] = [
+        returns: NodeNG | None = None
+        argtypes: list[NodeNG] = [
             self.visit(elem, parent) for elem in (type_comment_ast.argtypes or [])
         ]
         if type_comment_ast.returns:
             returns = self.visit(type_comment_ast.returns, parent)
 
         return returns, argtypes
 
     def visit_asyncfunctiondef(
-        self, node: "ast.AsyncFunctionDef", parent: NodeNG
+        self, node: ast.AsyncFunctionDef, parent: NodeNG
     ) -> nodes.AsyncFunctionDef:
         return self._visit_functiondef(nodes.AsyncFunctionDef, node, parent)
 
-    def visit_asyncfor(self, node: "ast.AsyncFor", parent: NodeNG) -> nodes.AsyncFor:
+    def visit_asyncfor(self, node: ast.AsyncFor, parent: NodeNG) -> nodes.AsyncFor:
         return self._visit_for(nodes.AsyncFor, node, parent)
 
-    def visit_await(self, node: "ast.Await", parent: NodeNG) -> nodes.Await:
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Await(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Await(node.lineno, node.col_offset, parent)
+    def visit_await(self, node: ast.Await, parent: NodeNG) -> nodes.Await:
+        newnode = nodes.Await(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(value=self.visit(node.value, newnode))
         return newnode
 
-    def visit_asyncwith(self, node: "ast.AsyncWith", parent: NodeNG) -> nodes.AsyncWith:
+    def visit_asyncwith(self, node: ast.AsyncWith, parent: NodeNG) -> nodes.AsyncWith:
         return self._visit_with(nodes.AsyncWith, node, parent)
 
-    def visit_assign(self, node: "ast.Assign", parent: NodeNG) -> nodes.Assign:
-        """visit a Assign node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Assign(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Assign(node.lineno, node.col_offset, parent)
+    def visit_assign(self, node: ast.Assign, parent: NodeNG) -> nodes.Assign:
+        """Visit a Assign node by returning a fresh instance of it."""
+        newnode = nodes.Assign(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         type_annotation = self.check_type_comment(node, parent=newnode)
         newnode.postinit(
             targets=[self.visit(child, newnode) for child in node.targets],
             value=self.visit(node.value, newnode),
             type_annotation=type_annotation,
         )
         return newnode
 
-    def visit_annassign(self, node: "ast.AnnAssign", parent: NodeNG) -> nodes.AnnAssign:
-        """visit an AnnAssign node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.AnnAssign(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.AnnAssign(node.lineno, node.col_offset, parent)
+    def visit_annassign(self, node: ast.AnnAssign, parent: NodeNG) -> nodes.AnnAssign:
+        """Visit an AnnAssign node by returning a fresh instance of it."""
+        newnode = nodes.AnnAssign(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             target=self.visit(node.target, newnode),
             annotation=self.visit(node.annotation, newnode),
             simple=node.simple,
             value=self.visit(node.value, newnode),
         )
         return newnode
 
     @overload
     def visit_assignname(
-        self, node: "ast.AST", parent: NodeNG, node_name: str
+        self, node: ast.AST, parent: NodeNG, node_name: str
     ) -> nodes.AssignName:
         ...
 
     @overload
-    def visit_assignname(
-        self, node: "ast.AST", parent: NodeNG, node_name: None
-    ) -> None:
+    def visit_assignname(self, node: ast.AST, parent: NodeNG, node_name: None) -> None:
         ...
 
     def visit_assignname(
-        self, node: "ast.AST", parent: NodeNG, node_name: Optional[str]
-    ) -> Optional[nodes.AssignName]:
-        """visit a node and return a AssignName node
+        self, node: ast.AST, parent: NodeNG, node_name: str | None
+    ) -> nodes.AssignName | None:
+        """Visit a node and return a AssignName node.
 
         Note: Method not called by 'visit'
         """
         if node_name is None:
             return None
-        if sys.version_info >= (3, 8):
-            newnode = nodes.AssignName(
-                name=node_name,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.AssignName(
-                node_name,
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+        newnode = nodes.AssignName(
+            name=node_name,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         self._save_assignment(newnode)
         return newnode
 
-    def visit_augassign(self, node: "ast.AugAssign", parent: NodeNG) -> nodes.AugAssign:
-        """visit a AugAssign node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.AugAssign(
-                op=self._parser_module.bin_op_classes[type(node.op)] + "=",
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.AugAssign(
-                self._parser_module.bin_op_classes[type(node.op)] + "=",
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+    def visit_augassign(self, node: ast.AugAssign, parent: NodeNG) -> nodes.AugAssign:
+        """Visit a AugAssign node by returning a fresh instance of it."""
+        newnode = nodes.AugAssign(
+            op=self._parser_module.bin_op_classes[type(node.op)] + "=",
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.target, newnode), self.visit(node.value, newnode)
         )
         return newnode
 
-    def visit_binop(self, node: "ast.BinOp", parent: NodeNG) -> nodes.BinOp:
-        """visit a BinOp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.BinOp(
-                op=self._parser_module.bin_op_classes[type(node.op)],
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.BinOp(
-                self._parser_module.bin_op_classes[type(node.op)],
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+    def visit_binop(self, node: ast.BinOp, parent: NodeNG) -> nodes.BinOp:
+        """Visit a BinOp node by returning a fresh instance of it."""
+        newnode = nodes.BinOp(
+            op=self._parser_module.bin_op_classes[type(node.op)],
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.left, newnode), self.visit(node.right, newnode)
         )
         return newnode
 
-    def visit_boolop(self, node: "ast.BoolOp", parent: NodeNG) -> nodes.BoolOp:
-        """visit a BoolOp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.BoolOp(
-                op=self._parser_module.bool_op_classes[type(node.op)],
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.BoolOp(
-                self._parser_module.bool_op_classes[type(node.op)],
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+    def visit_boolop(self, node: ast.BoolOp, parent: NodeNG) -> nodes.BoolOp:
+        """Visit a BoolOp node by returning a fresh instance of it."""
+        newnode = nodes.BoolOp(
+            op=self._parser_module.bool_op_classes[type(node.op)],
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.values])
         return newnode
 
-    def visit_break(self, node: "ast.Break", parent: NodeNG) -> nodes.Break:
-        """visit a Break node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            return nodes.Break(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        return nodes.Break(node.lineno, node.col_offset, parent)
+    def visit_break(self, node: ast.Break, parent: NodeNG) -> nodes.Break:
+        """Visit a Break node by returning a fresh instance of it."""
+        return nodes.Break(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
 
-    def visit_call(self, node: "ast.Call", parent: NodeNG) -> nodes.Call:
-        """visit a CallFunc node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Call(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Call(node.lineno, node.col_offset, parent)
+    def visit_call(self, node: ast.Call, parent: NodeNG) -> nodes.Call:
+        """Visit a CallFunc node by returning a fresh instance of it."""
+        newnode = nodes.Call(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             func=self.visit(node.func, newnode),
             args=[self.visit(child, newnode) for child in node.args],
             keywords=[self.visit(child, newnode) for child in node.keywords],
         )
         return newnode
 
     def visit_classdef(
-        self, node: "ast.ClassDef", parent: NodeNG, newstyle: bool = True
+        self, node: ast.ClassDef, parent: NodeNG, newstyle: bool = True
     ) -> nodes.ClassDef:
-        """visit a ClassDef node to become astroid"""
-        node, doc = self._get_doc(node)
-        if sys.version_info >= (3, 8):
-            newnode = nodes.ClassDef(
-                name=node.name,
-                doc=doc,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.ClassDef(
-                node.name, doc, node.lineno, node.col_offset, parent
-            )
+        """Visit a ClassDef node to become astroid."""
+        node, doc_ast_node = self._get_doc(node)
+        newnode = nodes.ClassDef(
+            name=node.name,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         metaclass = None
         for keyword in node.keywords:
             if keyword.arg == "metaclass":
                 metaclass = self.visit(keyword, newnode).value
                 break
         decorators = self.visit_decorators(node, newnode)
         newnode.postinit(
@@ -1199,346 +864,298 @@
             newstyle,
             metaclass,
             [
                 self.visit(kwd, newnode)
                 for kwd in node.keywords
                 if kwd.arg != "metaclass"
             ],
+            position=self._get_position_info(node, newnode),
+            doc_node=self.visit(doc_ast_node, newnode),
         )
         return newnode
 
-    def visit_continue(self, node: "ast.Continue", parent: NodeNG) -> nodes.Continue:
-        """visit a Continue node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            return nodes.Continue(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        return nodes.Continue(node.lineno, node.col_offset, parent)
+    def visit_continue(self, node: ast.Continue, parent: NodeNG) -> nodes.Continue:
+        """Visit a Continue node by returning a fresh instance of it."""
+        return nodes.Continue(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
 
-    def visit_compare(self, node: "ast.Compare", parent: NodeNG) -> nodes.Compare:
-        """visit a Compare node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Compare(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Compare(node.lineno, node.col_offset, parent)
+    def visit_compare(self, node: ast.Compare, parent: NodeNG) -> nodes.Compare:
+        """Visit a Compare node by returning a fresh instance of it."""
+        newnode = nodes.Compare(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.left, newnode),
             [
                 (
                     self._parser_module.cmp_op_classes[op.__class__],
                     self.visit(expr, newnode),
                 )
                 for (op, expr) in zip(node.ops, node.comparators)
             ],
         )
         return newnode
 
     def visit_comprehension(
-        self, node: "ast.comprehension", parent: NodeNG
+        self, node: ast.comprehension, parent: NodeNG
     ) -> nodes.Comprehension:
-        """visit a Comprehension node by returning a fresh instance of it"""
-        newnode = nodes.Comprehension(parent)
+        """Visit a Comprehension node by returning a fresh instance of it."""
+        newnode = nodes.Comprehension(
+            parent=parent,
+            # Comprehension nodes don't have these attributes
+            # see https://docs.python.org/3/library/ast.html#abstract-grammar
+            lineno=None,
+            col_offset=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
         newnode.postinit(
             self.visit(node.target, newnode),
             self.visit(node.iter, newnode),
             [self.visit(child, newnode) for child in node.ifs],
             bool(node.is_async),
         )
         return newnode
 
     def visit_decorators(
         self,
-        node: Union["ast.ClassDef", "ast.FunctionDef", "ast.AsyncFunctionDef"],
+        node: ast.ClassDef | ast.FunctionDef | ast.AsyncFunctionDef,
         parent: NodeNG,
-    ) -> Optional[nodes.Decorators]:
-        """visit a Decorators node by returning a fresh instance of it
+    ) -> nodes.Decorators | None:
+        """Visit a Decorators node by returning a fresh instance of it.
 
         Note: Method not called by 'visit'
         """
         if not node.decorator_list:
             return None
         # /!\ node is actually an _ast.FunctionDef node while
         # parent is an astroid.nodes.FunctionDef node
-        if sys.version_info >= (3, 8):
-            # Set the line number of the first decorator for Python 3.8+.
-            lineno = node.decorator_list[0].lineno
-            end_lineno = node.decorator_list[-1].end_lineno
-            end_col_offset = node.decorator_list[-1].end_col_offset
-        else:
-            lineno = node.lineno
-            end_lineno = None
-            end_col_offset = None
+
+        # Set the line number of the first decorator for Python 3.8+.
+        lineno = node.decorator_list[0].lineno
+        end_lineno = node.decorator_list[-1].end_lineno
+        end_col_offset = node.decorator_list[-1].end_col_offset
+
         newnode = nodes.Decorators(
             lineno=lineno,
             col_offset=node.col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
         newnode.postinit([self.visit(child, newnode) for child in node.decorator_list])
         return newnode
 
-    def visit_delete(self, node: "ast.Delete", parent: NodeNG) -> nodes.Delete:
-        """visit a Delete node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Delete(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Delete(node.lineno, node.col_offset, parent)
+    def visit_delete(self, node: ast.Delete, parent: NodeNG) -> nodes.Delete:
+        """Visit a Delete node by returning a fresh instance of it."""
+        newnode = nodes.Delete(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.targets])
         return newnode
 
     def _visit_dict_items(
-        self, node: "ast.Dict", parent: NodeNG, newnode: nodes.Dict
-    ) -> Generator[Tuple[NodeNG, NodeNG], None, None]:
+        self, node: ast.Dict, parent: NodeNG, newnode: nodes.Dict
+    ) -> Generator[tuple[NodeNG, NodeNG], None, None]:
         for key, value in zip(node.keys, node.values):
             rebuilt_key: NodeNG
             rebuilt_value = self.visit(value, newnode)
             if not key:
                 # Extended unpacking
-                if sys.version_info >= (3, 8):
-                    rebuilt_key = nodes.DictUnpack(
-                        lineno=rebuilt_value.lineno,
-                        col_offset=rebuilt_value.col_offset,
-                        end_lineno=rebuilt_value.end_lineno,
-                        end_col_offset=rebuilt_value.end_col_offset,
-                        parent=parent,
-                    )
-                else:
-                    rebuilt_key = nodes.DictUnpack(
-                        rebuilt_value.lineno, rebuilt_value.col_offset, parent
-                    )
+                rebuilt_key = nodes.DictUnpack(
+                    lineno=rebuilt_value.lineno,
+                    col_offset=rebuilt_value.col_offset,
+                    end_lineno=rebuilt_value.end_lineno,
+                    end_col_offset=rebuilt_value.end_col_offset,
+                    parent=parent,
+                )
             else:
                 rebuilt_key = self.visit(key, newnode)
             yield rebuilt_key, rebuilt_value
 
-    def visit_dict(self, node: "ast.Dict", parent: NodeNG) -> nodes.Dict:
-        """visit a Dict node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Dict(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Dict(node.lineno, node.col_offset, parent)
-        items = list(self._visit_dict_items(node, parent, newnode))
+    def visit_dict(self, node: ast.Dict, parent: NodeNG) -> nodes.Dict:
+        """Visit a Dict node by returning a fresh instance of it."""
+        newnode = nodes.Dict(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        items: list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]] = list(
+            self._visit_dict_items(node, parent, newnode)
+        )
         newnode.postinit(items)
         return newnode
 
-    def visit_dictcomp(self, node: "ast.DictComp", parent: NodeNG) -> nodes.DictComp:
-        """visit a DictComp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.DictComp(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.DictComp(node.lineno, node.col_offset, parent)
+    def visit_dictcomp(self, node: ast.DictComp, parent: NodeNG) -> nodes.DictComp:
+        """Visit a DictComp node by returning a fresh instance of it."""
+        newnode = nodes.DictComp(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.key, newnode),
             self.visit(node.value, newnode),
             [self.visit(child, newnode) for child in node.generators],
         )
         return newnode
 
-    def visit_expr(self, node: "ast.Expr", parent: NodeNG) -> nodes.Expr:
-        """visit a Expr node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Expr(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Expr(node.lineno, node.col_offset, parent)
-        newnode.postinit(self.visit(node.value, newnode))
-        return newnode
-
-    # Not used in Python 3.8+.
-    def visit_ellipsis(self, node: "ast.Ellipsis", parent: NodeNG) -> nodes.Const:
-        """visit an Ellipsis node by returning a fresh instance of Const"""
-        return nodes.Const(
-            value=Ellipsis,
+    def visit_expr(self, node: ast.Expr, parent: NodeNG) -> nodes.Expr:
+        """Visit a Expr node by returning a fresh instance of it."""
+        newnode = nodes.Expr(
             lineno=node.lineno,
             col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
             parent=parent,
         )
+        newnode.postinit(self.visit(node.value, newnode))
+        return newnode
 
     def visit_excepthandler(
-        self, node: "ast.ExceptHandler", parent: NodeNG
+        self, node: ast.ExceptHandler, parent: NodeNG
     ) -> nodes.ExceptHandler:
-        """visit an ExceptHandler node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.ExceptHandler(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.ExceptHandler(node.lineno, node.col_offset, parent)
+        """Visit an ExceptHandler node by returning a fresh instance of it."""
+        newnode = nodes.ExceptHandler(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.type, newnode),
             self.visit_assignname(node, newnode, node.name),
             [self.visit(child, newnode) for child in node.body],
         )
         return newnode
 
-    # Not used in Python 3.9+.
-    def visit_extslice(
-        self, node: "ast.ExtSlice", parent: nodes.Subscript
-    ) -> nodes.Tuple:
-        """visit an ExtSlice node by returning a fresh instance of Tuple"""
-        # ExtSlice doesn't have lineno or col_offset information
-        newnode = nodes.Tuple(ctx=Context.Load, parent=parent)
-        newnode.postinit([self.visit(dim, newnode) for dim in node.dims])  # type: ignore[attr-defined]
-        return newnode
-
     @overload
     def _visit_for(
-        self, cls: Type[nodes.For], node: "ast.For", parent: NodeNG
+        self, cls: type[nodes.For], node: ast.For, parent: NodeNG
     ) -> nodes.For:
         ...
 
     @overload
     def _visit_for(
-        self, cls: Type[nodes.AsyncFor], node: "ast.AsyncFor", parent: NodeNG
+        self, cls: type[nodes.AsyncFor], node: ast.AsyncFor, parent: NodeNG
     ) -> nodes.AsyncFor:
         ...
 
     def _visit_for(
-        self, cls: Type[T_For], node: Union["ast.For", "ast.AsyncFor"], parent: NodeNG
-    ) -> T_For:
-        """visit a For node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = cls(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = cls(node.lineno, node.col_offset, parent)
+        self, cls: type[_ForT], node: ast.For | ast.AsyncFor, parent: NodeNG
+    ) -> _ForT:
+        """Visit a For node by returning a fresh instance of it."""
+        col_offset = node.col_offset
+        if IS_PYPY and not PY39_PLUS and isinstance(node, ast.AsyncFor) and self._data:
+            # pylint: disable-next=unsubscriptable-object
+            col_offset = self._data[node.lineno - 1].index("async")
+
+        newnode = cls(
+            lineno=node.lineno,
+            col_offset=col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         type_annotation = self.check_type_comment(node, parent=newnode)
         newnode.postinit(
             target=self.visit(node.target, newnode),
             iter=self.visit(node.iter, newnode),
             body=[self.visit(child, newnode) for child in node.body],
             orelse=[self.visit(child, newnode) for child in node.orelse],
             type_annotation=type_annotation,
         )
         return newnode
 
-    def visit_for(self, node: "ast.For", parent: NodeNG) -> nodes.For:
+    def visit_for(self, node: ast.For, parent: NodeNG) -> nodes.For:
         return self._visit_for(nodes.For, node, parent)
 
     def visit_importfrom(
-        self, node: "ast.ImportFrom", parent: NodeNG
+        self, node: ast.ImportFrom, parent: NodeNG
     ) -> nodes.ImportFrom:
-        """visit an ImportFrom node by returning a fresh instance of it"""
+        """Visit an ImportFrom node by returning a fresh instance of it."""
         names = [(alias.name, alias.asname) for alias in node.names]
-        if sys.version_info >= (3, 8):
-            newnode = nodes.ImportFrom(
-                fromname=node.module or "",
-                names=names,
-                level=node.level or None,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.ImportFrom(
-                node.module or "",
-                names,
-                node.level or None,
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+        newnode = nodes.ImportFrom(
+            fromname=node.module or "",
+            names=names,
+            level=node.level or None,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         # store From names to add them to locals after building
         self._import_from_nodes.append(newnode)
         return newnode
 
     @overload
     def _visit_functiondef(
-        self, cls: Type[nodes.FunctionDef], node: "ast.FunctionDef", parent: NodeNG
+        self, cls: type[nodes.FunctionDef], node: ast.FunctionDef, parent: NodeNG
     ) -> nodes.FunctionDef:
         ...
 
     @overload
     def _visit_functiondef(
         self,
-        cls: Type[nodes.AsyncFunctionDef],
-        node: "ast.AsyncFunctionDef",
+        cls: type[nodes.AsyncFunctionDef],
+        node: ast.AsyncFunctionDef,
         parent: NodeNG,
     ) -> nodes.AsyncFunctionDef:
         ...
 
     def _visit_functiondef(
         self,
-        cls: Type[T_Function],
-        node: Union["ast.FunctionDef", "ast.AsyncFunctionDef"],
+        cls: type[_FunctionT],
+        node: ast.FunctionDef | ast.AsyncFunctionDef,
         parent: NodeNG,
-    ) -> T_Function:
-        """visit an FunctionDef node to become astroid"""
+    ) -> _FunctionT:
+        """Visit an FunctionDef node to become astroid."""
         self._global_names.append({})
-        node, doc = self._get_doc(node)
+        node, doc_ast_node = self._get_doc(node)
 
         lineno = node.lineno
-        if PY38_PLUS and node.decorator_list:
+        if node.decorator_list:
             # Python 3.8 sets the line number of a decorated function
             # to be the actual line number of the function, but the
             # previous versions expected the decorator's line number instead.
             # We reset the function's line number to that of the
             # first decorator to maintain backward compatibility.
             # It's not ideal but this discrepancy was baked into
             # the framework for *years*.
             lineno = node.decorator_list[0].lineno
 
-        if sys.version_info >= (3, 8):
-            newnode = cls(
-                name=node.name,
-                doc=doc,
-                lineno=lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = cls(node.name, doc, lineno, node.col_offset, parent)
+        newnode = cls(
+            name=node.name,
+            lineno=lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         decorators = self.visit_decorators(node, newnode)
-        returns: Optional[NodeNG]
+        returns: NodeNG | None
         if node.returns:
             returns = self.visit(node.returns, newnode)
         else:
             returns = None
 
         type_comment_args = type_comment_returns = None
         type_comment_annotation = self.check_function_type_comment(node, newnode)
@@ -1547,856 +1164,683 @@
         newnode.postinit(
             args=self.visit(node.args, newnode),
             body=[self.visit(child, newnode) for child in node.body],
             decorators=decorators,
             returns=returns,
             type_comment_returns=type_comment_returns,
             type_comment_args=type_comment_args,
+            position=self._get_position_info(node, newnode),
+            doc_node=self.visit(doc_ast_node, newnode),
         )
         self._global_names.pop()
         return newnode
 
     def visit_functiondef(
-        self, node: "ast.FunctionDef", parent: NodeNG
+        self, node: ast.FunctionDef, parent: NodeNG
     ) -> nodes.FunctionDef:
         return self._visit_functiondef(nodes.FunctionDef, node, parent)
 
     def visit_generatorexp(
-        self, node: "ast.GeneratorExp", parent: NodeNG
+        self, node: ast.GeneratorExp, parent: NodeNG
     ) -> nodes.GeneratorExp:
-        """visit a GeneratorExp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.GeneratorExp(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.GeneratorExp(node.lineno, node.col_offset, parent)
+        """Visit a GeneratorExp node by returning a fresh instance of it."""
+        newnode = nodes.GeneratorExp(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.elt, newnode),
             [self.visit(child, newnode) for child in node.generators],
         )
         return newnode
 
     def visit_attribute(
-        self, node: "ast.Attribute", parent: NodeNG
-    ) -> Union[nodes.Attribute, nodes.AssignAttr, nodes.DelAttr]:
-        """visit an Attribute node by returning a fresh instance of it"""
+        self, node: ast.Attribute, parent: NodeNG
+    ) -> nodes.Attribute | nodes.AssignAttr | nodes.DelAttr:
+        """Visit an Attribute node by returning a fresh instance of it."""
         context = self._get_context(node)
-        newnode: Union[nodes.Attribute, nodes.AssignAttr, nodes.DelAttr]
+        newnode: nodes.Attribute | nodes.AssignAttr | nodes.DelAttr
         if context == Context.Del:
             # FIXME : maybe we should reintroduce and visit_delattr ?
             # for instance, deactivating assign_ctx
-            if sys.version_info >= (3, 8):
-                newnode = nodes.DelAttr(
-                    attrname=node.attr,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.DelAttr(node.attr, node.lineno, node.col_offset, parent)
+            newnode = nodes.DelAttr(
+                attrname=node.attr,
+                lineno=node.lineno,
+                col_offset=node.col_offset,
+                end_lineno=node.end_lineno,
+                end_col_offset=node.end_col_offset,
+                parent=parent,
+            )
         elif context == Context.Store:
-            if sys.version_info >= (3, 8):
-                newnode = nodes.AssignAttr(
-                    attrname=node.attr,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.AssignAttr(
-                    node.attr, node.lineno, node.col_offset, parent
-                )
+            newnode = nodes.AssignAttr(
+                attrname=node.attr,
+                lineno=node.lineno,
+                col_offset=node.col_offset,
+                end_lineno=node.end_lineno,
+                end_col_offset=node.end_col_offset,
+                parent=parent,
+            )
             # Prohibit a local save if we are in an ExceptHandler.
             if not isinstance(parent, nodes.ExceptHandler):
-                # mypy doesn't recognize that newnode has to be AssignAttr because it doesn't support ParamSpec
+                # mypy doesn't recognize that newnode has to be AssignAttr because it
+                # doesn't support ParamSpec
                 # See https://github.com/python/mypy/issues/8645
                 self._delayed_assattr.append(newnode)  # type: ignore[arg-type]
         else:
-            # pylint: disable-next=else-if-used
-            # Preserve symmetry with other cases
-            if sys.version_info >= (3, 8):
-                newnode = nodes.Attribute(
-                    attrname=node.attr,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.Attribute(
-                    node.attr, node.lineno, node.col_offset, parent
-                )
-        newnode.postinit(self.visit(node.value, newnode))
-        return newnode
-
-    def visit_global(self, node: "ast.Global", parent: NodeNG) -> nodes.Global:
-        """visit a Global node to become astroid"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Global(
-                names=node.names,
+            newnode = nodes.Attribute(
+                attrname=node.attr,
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
-        else:
-            newnode = nodes.Global(
-                node.names,
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+        newnode.postinit(self.visit(node.value, newnode))
+        return newnode
+
+    def visit_global(self, node: ast.Global, parent: NodeNG) -> nodes.Global:
+        """Visit a Global node to become astroid."""
+        newnode = nodes.Global(
+            names=node.names,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         if self._global_names:  # global at the module level, no effect
             for name in node.names:
                 self._global_names[-1].setdefault(name, []).append(newnode)
         return newnode
 
-    def visit_if(self, node: "ast.If", parent: NodeNG) -> nodes.If:
-        """visit an If node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.If(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.If(node.lineno, node.col_offset, parent)
+    def visit_if(self, node: ast.If, parent: NodeNG) -> nodes.If:
+        """Visit an If node by returning a fresh instance of it."""
+        newnode = nodes.If(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.test, newnode),
             [self.visit(child, newnode) for child in node.body],
             [self.visit(child, newnode) for child in node.orelse],
         )
         return newnode
 
-    def visit_ifexp(self, node: "ast.IfExp", parent: NodeNG) -> nodes.IfExp:
-        """visit a IfExp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.IfExp(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.IfExp(node.lineno, node.col_offset, parent)
+    def visit_ifexp(self, node: ast.IfExp, parent: NodeNG) -> nodes.IfExp:
+        """Visit a IfExp node by returning a fresh instance of it."""
+        newnode = nodes.IfExp(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.test, newnode),
             self.visit(node.body, newnode),
             self.visit(node.orelse, newnode),
         )
         return newnode
 
-    def visit_import(self, node: "ast.Import", parent: NodeNG) -> nodes.Import:
-        """visit a Import node by returning a fresh instance of it"""
+    def visit_import(self, node: ast.Import, parent: NodeNG) -> nodes.Import:
+        """Visit a Import node by returning a fresh instance of it."""
         names = [(alias.name, alias.asname) for alias in node.names]
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Import(
-                names=names,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Import(
-                names,
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+        newnode = nodes.Import(
+            names=names,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         # save import names in parent's locals:
-        for (name, asname) in newnode.names:
+        for name, asname in newnode.names:
             name = asname or name
             parent.set_local(name.split(".")[0], newnode)
         return newnode
 
-    def visit_joinedstr(self, node: "ast.JoinedStr", parent: NodeNG) -> nodes.JoinedStr:
-        if sys.version_info >= (3, 8):
-            newnode = nodes.JoinedStr(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.JoinedStr(node.lineno, node.col_offset, parent)
+    def visit_joinedstr(self, node: ast.JoinedStr, parent: NodeNG) -> nodes.JoinedStr:
+        newnode = nodes.JoinedStr(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.values])
         return newnode
 
     def visit_formattedvalue(
-        self, node: "ast.FormattedValue", parent: NodeNG
+        self, node: ast.FormattedValue, parent: NodeNG
     ) -> nodes.FormattedValue:
-        if sys.version_info >= (3, 8):
-            newnode = nodes.FormattedValue(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.FormattedValue(node.lineno, node.col_offset, parent)
+        newnode = nodes.FormattedValue(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
-            self.visit(node.value, newnode),
-            node.conversion,
-            self.visit(node.format_spec, newnode),
+            value=self.visit(node.value, newnode),
+            conversion=node.conversion,
+            format_spec=self.visit(node.format_spec, newnode),
         )
         return newnode
 
-    def visit_namedexpr(self, node: "ast.NamedExpr", parent: NodeNG) -> nodes.NamedExpr:
-        if sys.version_info >= (3, 8):
-            newnode = nodes.NamedExpr(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.NamedExpr(node.lineno, node.col_offset, parent)
+    def visit_namedexpr(self, node: ast.NamedExpr, parent: NodeNG) -> nodes.NamedExpr:
+        newnode = nodes.NamedExpr(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.target, newnode), self.visit(node.value, newnode)
         )
         return newnode
 
-    # Not used in Python 3.9+.
-    def visit_index(self, node: "ast.Index", parent: nodes.Subscript) -> NodeNG:
-        """visit a Index node by returning a fresh instance of NodeNG"""
-        return self.visit(node.value, parent)  # type: ignore[attr-defined]
-
-    def visit_keyword(self, node: "ast.keyword", parent: NodeNG) -> nodes.Keyword:
-        """visit a Keyword node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 9):
-            newnode = nodes.Keyword(
-                arg=node.arg,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Keyword(node.arg, parent=parent)
+    if sys.version_info < (3, 9):
+        # Not used in Python 3.9+.
+        def visit_extslice(
+            self, node: ast.ExtSlice, parent: nodes.Subscript
+        ) -> nodes.Tuple:
+            """Visit an ExtSlice node by returning a fresh instance of Tuple."""
+            # ExtSlice doesn't have lineno or col_offset information
+            newnode = nodes.Tuple(ctx=Context.Load, parent=parent)
+            newnode.postinit([self.visit(dim, newnode) for dim in node.dims])
+            return newnode
+
+        def visit_index(self, node: ast.Index, parent: nodes.Subscript) -> NodeNG:
+            """Visit a Index node by returning a fresh instance of NodeNG."""
+            return self.visit(node.value, parent)
+
+    def visit_keyword(self, node: ast.keyword, parent: NodeNG) -> nodes.Keyword:
+        """Visit a Keyword node by returning a fresh instance of it."""
+        newnode = nodes.Keyword(
+            arg=node.arg,
+            # position attributes added in 3.9
+            lineno=getattr(node, "lineno", None),
+            col_offset=getattr(node, "col_offset", None),
+            end_lineno=getattr(node, "end_lineno", None),
+            end_col_offset=getattr(node, "end_col_offset", None),
+            parent=parent,
+        )
         newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
-    def visit_lambda(self, node: "ast.Lambda", parent: NodeNG) -> nodes.Lambda:
-        """visit a Lambda node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Lambda(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Lambda(node.lineno, node.col_offset, parent)
+    def visit_lambda(self, node: ast.Lambda, parent: NodeNG) -> nodes.Lambda:
+        """Visit a Lambda node by returning a fresh instance of it."""
+        newnode = nodes.Lambda(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(self.visit(node.args, newnode), self.visit(node.body, newnode))
         return newnode
 
-    def visit_list(self, node: "ast.List", parent: NodeNG) -> nodes.List:
-        """visit a List node by returning a fresh instance of it"""
+    def visit_list(self, node: ast.List, parent: NodeNG) -> nodes.List:
+        """Visit a List node by returning a fresh instance of it."""
         context = self._get_context(node)
-        if sys.version_info >= (3, 8):
-            newnode = nodes.List(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.List(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                parent=parent,
-            )
+        newnode = nodes.List(
+            ctx=context,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.elts])
         return newnode
 
-    def visit_listcomp(self, node: "ast.ListComp", parent: NodeNG) -> nodes.ListComp:
-        """visit a ListComp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.ListComp(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.ListComp(node.lineno, node.col_offset, parent)
+    def visit_listcomp(self, node: ast.ListComp, parent: NodeNG) -> nodes.ListComp:
+        """Visit a ListComp node by returning a fresh instance of it."""
+        newnode = nodes.ListComp(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.elt, newnode),
             [self.visit(child, newnode) for child in node.generators],
         )
         return newnode
 
     def visit_name(
-        self, node: "ast.Name", parent: NodeNG
-    ) -> Union[nodes.Name, nodes.AssignName, nodes.DelName]:
-        """visit a Name node by returning a fresh instance of it"""
+        self, node: ast.Name, parent: NodeNG
+    ) -> nodes.Name | nodes.AssignName | nodes.DelName:
+        """Visit a Name node by returning a fresh instance of it."""
         context = self._get_context(node)
-        newnode: Union[nodes.Name, nodes.AssignName, nodes.DelName]
+        newnode: nodes.Name | nodes.AssignName | nodes.DelName
         if context == Context.Del:
-            if sys.version_info >= (3, 8):
-                newnode = nodes.DelName(
-                    name=node.id,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.DelName(node.id, node.lineno, node.col_offset, parent)
+            newnode = nodes.DelName(
+                name=node.id,
+                lineno=node.lineno,
+                col_offset=node.col_offset,
+                end_lineno=node.end_lineno,
+                end_col_offset=node.end_col_offset,
+                parent=parent,
+            )
         elif context == Context.Store:
-            if sys.version_info >= (3, 8):
-                newnode = nodes.AssignName(
-                    name=node.id,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.AssignName(
-                    node.id, node.lineno, node.col_offset, parent
-                )
-        else:
-            # pylint: disable-next=else-if-used
-            # Preserve symmetry with other cases
-            if sys.version_info >= (3, 8):
-                newnode = nodes.Name(
-                    name=node.id,
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.Name(node.id, node.lineno, node.col_offset, parent)
-        # XXX REMOVE me :
-        if context in (Context.Del, Context.Store):  # 'Aug' ??
-            newnode = cast(Union[nodes.AssignName, nodes.DelName], newnode)
-            self._save_assignment(newnode)
-        return newnode
-
-    # Not used in Python 3.8+.
-    def visit_nameconstant(
-        self, node: "ast.NameConstant", parent: NodeNG
-    ) -> nodes.Const:
-        # For singleton values True / False / None
-        return nodes.Const(
-            node.value,
-            node.lineno,
-            node.col_offset,
-            parent,
-        )
-
-    def visit_nonlocal(self, node: "ast.Nonlocal", parent: NodeNG) -> nodes.Nonlocal:
-        """visit a Nonlocal node and return a new instance of it"""
-        if sys.version_info >= (3, 8):
-            return nodes.Nonlocal(
-                names=node.names,
+            newnode = nodes.AssignName(
+                name=node.id,
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
-        return nodes.Nonlocal(
-            node.names,
-            node.lineno,
-            node.col_offset,
-            parent,
-        )
-
-    def visit_constant(self, node: "ast.Constant", parent: NodeNG) -> nodes.Const:
-        """visit a Constant node by returning a fresh instance of Const"""
-        if sys.version_info >= (3, 8):
-            return nodes.Const(
-                value=node.value,
-                kind=node.kind,
+        else:
+            newnode = nodes.Name(
+                name=node.id,
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
-        return nodes.Const(
-            node.value,
-            node.lineno,
-            node.col_offset,
-            parent,
-            node.kind,
-        )
+        # XXX REMOVE me :
+        if context in (Context.Del, Context.Store):  # 'Aug' ??
+            newnode = cast(Union[nodes.AssignName, nodes.DelName], newnode)
+            self._save_assignment(newnode)
+        return newnode
 
-    # Not used in Python 3.8+.
-    def visit_str(
-        self, node: Union["ast.Str", "ast.Bytes"], parent: NodeNG
-    ) -> nodes.Const:
-        """visit a String/Bytes node by returning a fresh instance of Const"""
-        return nodes.Const(
-            node.s,
-            node.lineno,
-            node.col_offset,
-            parent,
+    def visit_nonlocal(self, node: ast.Nonlocal, parent: NodeNG) -> nodes.Nonlocal:
+        """Visit a Nonlocal node and return a new instance of it."""
+        return nodes.Nonlocal(
+            names=node.names,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
         )
 
-    # Not used in Python 3.8+
-    visit_bytes = visit_str
-
-    # Not used in Python 3.8+.
-    def visit_num(self, node: "ast.Num", parent: NodeNG) -> nodes.Const:
-        """visit a Num node by returning a fresh instance of Const"""
+    def visit_constant(self, node: ast.Constant, parent: NodeNG) -> nodes.Const:
+        """Visit a Constant node by returning a fresh instance of Const."""
         return nodes.Const(
-            node.n,
-            node.lineno,
-            node.col_offset,
-            parent,
+            value=node.value,
+            kind=node.kind,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
         )
 
-    def visit_pass(self, node: "ast.Pass", parent: NodeNG) -> nodes.Pass:
-        """visit a Pass node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            return nodes.Pass(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        return nodes.Pass(node.lineno, node.col_offset, parent)
+    def visit_pass(self, node: ast.Pass, parent: NodeNG) -> nodes.Pass:
+        """Visit a Pass node by returning a fresh instance of it."""
+        return nodes.Pass(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
 
-    def visit_raise(self, node: "ast.Raise", parent: NodeNG) -> nodes.Raise:
-        """visit a Raise node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Raise(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Raise(node.lineno, node.col_offset, parent)
+    def visit_raise(self, node: ast.Raise, parent: NodeNG) -> nodes.Raise:
+        """Visit a Raise node by returning a fresh instance of it."""
+        newnode = nodes.Raise(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         # no traceback; anyway it is not used in Pylint
         newnode.postinit(
             exc=self.visit(node.exc, newnode),
             cause=self.visit(node.cause, newnode),
         )
         return newnode
 
-    def visit_return(self, node: "ast.Return", parent: NodeNG) -> nodes.Return:
-        """visit a Return node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Return(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Return(node.lineno, node.col_offset, parent)
-        if node.value is not None:
-            newnode.postinit(self.visit(node.value, newnode))
+    def visit_return(self, node: ast.Return, parent: NodeNG) -> nodes.Return:
+        """Visit a Return node by returning a fresh instance of it."""
+        newnode = nodes.Return(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
-    def visit_set(self, node: "ast.Set", parent: NodeNG) -> nodes.Set:
-        """visit a Set node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Set(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Set(node.lineno, node.col_offset, parent)
+    def visit_set(self, node: ast.Set, parent: NodeNG) -> nodes.Set:
+        """Visit a Set node by returning a fresh instance of it."""
+        newnode = nodes.Set(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.elts])
         return newnode
 
-    def visit_setcomp(self, node: "ast.SetComp", parent: NodeNG) -> nodes.SetComp:
-        """visit a SetComp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.SetComp(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.SetComp(node.lineno, node.col_offset, parent)
+    def visit_setcomp(self, node: ast.SetComp, parent: NodeNG) -> nodes.SetComp:
+        """Visit a SetComp node by returning a fresh instance of it."""
+        newnode = nodes.SetComp(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.elt, newnode),
             [self.visit(child, newnode) for child in node.generators],
         )
         return newnode
 
-    def visit_slice(self, node: "ast.Slice", parent: nodes.Subscript) -> nodes.Slice:
-        """visit a Slice node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 9):
-            newnode = nodes.Slice(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Slice(parent=parent)
+    def visit_slice(self, node: ast.Slice, parent: nodes.Subscript) -> nodes.Slice:
+        """Visit a Slice node by returning a fresh instance of it."""
+        newnode = nodes.Slice(
+            # position attributes added in 3.9
+            lineno=getattr(node, "lineno", None),
+            col_offset=getattr(node, "col_offset", None),
+            end_lineno=getattr(node, "end_lineno", None),
+            end_col_offset=getattr(node, "end_col_offset", None),
+            parent=parent,
+        )
         newnode.postinit(
             lower=self.visit(node.lower, newnode),
             upper=self.visit(node.upper, newnode),
             step=self.visit(node.step, newnode),
         )
         return newnode
 
-    def visit_subscript(self, node: "ast.Subscript", parent: NodeNG) -> nodes.Subscript:
-        """visit a Subscript node by returning a fresh instance of it"""
+    def visit_subscript(self, node: ast.Subscript, parent: NodeNG) -> nodes.Subscript:
+        """Visit a Subscript node by returning a fresh instance of it."""
         context = self._get_context(node)
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Subscript(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Subscript(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                parent=parent,
-            )
+        newnode = nodes.Subscript(
+            ctx=context,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.value, newnode), self.visit(node.slice, newnode)
         )
         return newnode
 
-    def visit_starred(self, node: "ast.Starred", parent: NodeNG) -> nodes.Starred:
-        """visit a Starred node and return a new instance of it"""
+    def visit_starred(self, node: ast.Starred, parent: NodeNG) -> nodes.Starred:
+        """Visit a Starred node and return a new instance of it."""
         context = self._get_context(node)
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Starred(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Starred(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                parent=parent,
-            )
+        newnode = nodes.Starred(
+            ctx=context,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
-    def visit_tryexcept(self, node: "ast.Try", parent: NodeNG) -> nodes.TryExcept:
-        """visit a TryExcept node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.TryExcept(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.TryExcept(node.lineno, node.col_offset, parent)
+    def visit_tryexcept(self, node: ast.Try, parent: NodeNG) -> nodes.TryExcept:
+        """Visit a TryExcept node by returning a fresh instance of it."""
+        # TryExcept excludes the 'finally' but that will be included in the
+        # end_lineno from 'node'. Therefore, we check all non 'finally'
+        # children to find the correct end_lineno and column.
+        end_lineno = node.end_lineno
+        end_col_offset = node.end_col_offset
+        all_children: list[ast.AST] = [*node.body, *node.handlers, *node.orelse]
+        for child in reversed(all_children):
+            end_lineno = child.end_lineno
+            end_col_offset = child.end_col_offset
+            break
+        newnode = nodes.TryExcept(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             [self.visit(child, newnode) for child in node.body],
             [self.visit(child, newnode) for child in node.handlers],
             [self.visit(child, newnode) for child in node.orelse],
         )
         return newnode
 
     def visit_try(
-        self, node: "ast.Try", parent: NodeNG
-    ) -> Union[nodes.TryExcept, nodes.TryFinally, None]:
+        self, node: ast.Try, parent: NodeNG
+    ) -> nodes.TryExcept | nodes.TryFinally | None:
         # python 3.3 introduce a new Try node replacing
         # TryFinally/TryExcept nodes
         if node.finalbody:
-            if sys.version_info >= (3, 8):
-                newnode = nodes.TryFinally(
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
-                    end_lineno=node.end_lineno,
-                    end_col_offset=node.end_col_offset,
-                    parent=parent,
-                )
-            else:
-                newnode = nodes.TryFinally(node.lineno, node.col_offset, parent)
-            body: Union[List[nodes.TryExcept], List[NodeNG]]
+            newnode = nodes.TryFinally(
+                lineno=node.lineno,
+                col_offset=node.col_offset,
+                end_lineno=node.end_lineno,
+                end_col_offset=node.end_col_offset,
+                parent=parent,
+            )
+            body: list[NodeNG | nodes.TryExcept]
             if node.handlers:
                 body = [self.visit_tryexcept(node, newnode)]
             else:
                 body = [self.visit(child, newnode) for child in node.body]
             newnode.postinit(body, [self.visit(n, newnode) for n in node.finalbody])
             return newnode
         if node.handlers:
             return self.visit_tryexcept(node, parent)
         return None
 
-    def visit_tryfinally(self, node: "ast.Try", parent: NodeNG) -> nodes.TryFinally:
-        """visit a TryFinally node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.TryFinally(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.TryFinally(node.lineno, node.col_offset, parent)
+    def visit_trystar(self, node: ast.TryStar, parent: NodeNG) -> nodes.TryStar:
+        newnode = nodes.TryStar(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
-            [self.visit(child, newnode) for child in node.body],
-            [self.visit(n, newnode) for n in node.finalbody],
+            body=[self.visit(n, newnode) for n in node.body],
+            handlers=[self.visit(n, newnode) for n in node.handlers],
+            orelse=[self.visit(n, newnode) for n in node.orelse],
+            finalbody=[self.visit(n, newnode) for n in node.finalbody],
         )
         return newnode
 
-    def visit_tuple(self, node: "ast.Tuple", parent: NodeNG) -> nodes.Tuple:
-        """visit a Tuple node by returning a fresh instance of it"""
+    def visit_tuple(self, node: ast.Tuple, parent: NodeNG) -> nodes.Tuple:
+        """Visit a Tuple node by returning a fresh instance of it."""
         context = self._get_context(node)
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Tuple(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Tuple(
-                ctx=context,
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                parent=parent,
-            )
+        newnode = nodes.Tuple(
+            ctx=context,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit([self.visit(child, newnode) for child in node.elts])
         return newnode
 
-    def visit_unaryop(self, node: "ast.UnaryOp", parent: NodeNG) -> nodes.UnaryOp:
-        """visit a UnaryOp node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.UnaryOp(
-                op=self._parser_module.unary_op_classes[node.op.__class__],
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.UnaryOp(
-                self._parser_module.unary_op_classes[node.op.__class__],
-                node.lineno,
-                node.col_offset,
-                parent,
-            )
+    def visit_unaryop(self, node: ast.UnaryOp, parent: NodeNG) -> nodes.UnaryOp:
+        """Visit a UnaryOp node by returning a fresh instance of it."""
+        newnode = nodes.UnaryOp(
+            op=self._parser_module.unary_op_classes[node.op.__class__],
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(self.visit(node.operand, newnode))
         return newnode
 
-    def visit_while(self, node: "ast.While", parent: NodeNG) -> nodes.While:
-        """visit a While node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.While(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.While(node.lineno, node.col_offset, parent)
+    def visit_while(self, node: ast.While, parent: NodeNG) -> nodes.While:
+        """Visit a While node by returning a fresh instance of it."""
+        newnode = nodes.While(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
         newnode.postinit(
             self.visit(node.test, newnode),
             [self.visit(child, newnode) for child in node.body],
             [self.visit(child, newnode) for child in node.orelse],
         )
         return newnode
 
     @overload
     def _visit_with(
-        self, cls: Type[nodes.With], node: "ast.With", parent: NodeNG
+        self, cls: type[nodes.With], node: ast.With, parent: NodeNG
     ) -> nodes.With:
         ...
 
     @overload
     def _visit_with(
-        self, cls: Type[nodes.AsyncWith], node: "ast.AsyncWith", parent: NodeNG
+        self, cls: type[nodes.AsyncWith], node: ast.AsyncWith, parent: NodeNG
     ) -> nodes.AsyncWith:
         ...
 
     def _visit_with(
         self,
-        cls: Type[T_With],
-        node: Union["ast.With", "ast.AsyncWith"],
+        cls: type[_WithT],
+        node: ast.With | ast.AsyncWith,
         parent: NodeNG,
-    ) -> T_With:
-        if sys.version_info >= (3, 8):
-            newnode = cls(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = cls(node.lineno, node.col_offset, parent)
+    ) -> _WithT:
+        col_offset = node.col_offset
+        if IS_PYPY and not PY39_PLUS and isinstance(node, ast.AsyncWith) and self._data:
+            # pylint: disable-next=unsubscriptable-object
+            col_offset = self._data[node.lineno - 1].index("async")
 
-        def visit_child(child: "ast.withitem") -> Tuple[NodeNG, Optional[NodeNG]]:
+        newnode = cls(
+            lineno=node.lineno,
+            col_offset=col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+
+        def visit_child(child: ast.withitem) -> tuple[NodeNG, NodeNG | None]:
             expr = self.visit(child.context_expr, newnode)
             var = self.visit(child.optional_vars, newnode)
             return expr, var
 
         type_annotation = self.check_type_comment(node, parent=newnode)
         newnode.postinit(
             items=[visit_child(child) for child in node.items],
             body=[self.visit(child, newnode) for child in node.body],
             type_annotation=type_annotation,
         )
         return newnode
 
-    def visit_with(self, node: "ast.With", parent: NodeNG) -> NodeNG:
+    def visit_with(self, node: ast.With, parent: NodeNG) -> NodeNG:
         return self._visit_with(nodes.With, node, parent)
 
-    def visit_yield(self, node: "ast.Yield", parent: NodeNG) -> NodeNG:
-        """visit a Yield node by returning a fresh instance of it"""
-        if sys.version_info >= (3, 8):
-            newnode = nodes.Yield(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.Yield(node.lineno, node.col_offset, parent)
-        if node.value is not None:
-            newnode.postinit(self.visit(node.value, newnode))
+    def visit_yield(self, node: ast.Yield, parent: NodeNG) -> NodeNG:
+        """Visit a Yield node by returning a fresh instance of it."""
+        newnode = nodes.Yield(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
-    def visit_yieldfrom(self, node: "ast.YieldFrom", parent: NodeNG) -> NodeNG:
-        if sys.version_info >= (3, 8):
-            newnode = nodes.YieldFrom(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-        else:
-            newnode = nodes.YieldFrom(node.lineno, node.col_offset, parent)
-        if node.value is not None:
-            newnode.postinit(self.visit(node.value, newnode))
+    def visit_yieldfrom(self, node: ast.YieldFrom, parent: NodeNG) -> NodeNG:
+        newnode = nodes.YieldFrom(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
     if sys.version_info >= (3, 10):
 
-        def visit_match(self, node: "ast.Match", parent: NodeNG) -> nodes.Match:
+        def visit_match(self, node: ast.Match, parent: NodeNG) -> nodes.Match:
             newnode = nodes.Match(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
             newnode.postinit(
                 subject=self.visit(node.subject, newnode),
                 cases=[self.visit(case, newnode) for case in node.cases],
             )
             return newnode
 
         def visit_matchcase(
-            self, node: "ast.match_case", parent: NodeNG
+            self, node: ast.match_case, parent: NodeNG
         ) -> nodes.MatchCase:
             newnode = nodes.MatchCase(parent=parent)
             newnode.postinit(
                 pattern=self.visit(node.pattern, newnode),
                 guard=self.visit(node.guard, newnode),
                 body=[self.visit(child, newnode) for child in node.body],
             )
             return newnode
 
         def visit_matchvalue(
-            self, node: "ast.MatchValue", parent: NodeNG
+            self, node: ast.MatchValue, parent: NodeNG
         ) -> nodes.MatchValue:
             newnode = nodes.MatchValue(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
             newnode.postinit(value=self.visit(node.value, newnode))
             return newnode
 
         def visit_matchsingleton(
-            self, node: "ast.MatchSingleton", parent: NodeNG
+            self, node: ast.MatchSingleton, parent: NodeNG
         ) -> nodes.MatchSingleton:
             return nodes.MatchSingleton(
-                value=node.value,  # type: ignore[arg-type] # See https://github.com/python/mypy/pull/10389
+                value=node.value,
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
 
         def visit_matchsequence(
-            self, node: "ast.MatchSequence", parent: NodeNG
+            self, node: ast.MatchSequence, parent: NodeNG
         ) -> nodes.MatchSequence:
             newnode = nodes.MatchSequence(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
             newnode.postinit(
                 patterns=[self.visit(pattern, newnode) for pattern in node.patterns]
             )
             return newnode
 
         def visit_matchmapping(
-            self, node: "ast.MatchMapping", parent: NodeNG
+            self, node: ast.MatchMapping, parent: NodeNG
         ) -> nodes.MatchMapping:
             newnode = nodes.MatchMapping(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
@@ -2407,15 +1851,15 @@
                 keys=[self.visit(child, newnode) for child in node.keys],
                 patterns=[self.visit(pattern, newnode) for pattern in node.patterns],
                 rest=self.visit_assignname(node, newnode, node.rest),
             )
             return newnode
 
         def visit_matchclass(
-            self, node: "ast.MatchClass", parent: NodeNG
+            self, node: ast.MatchClass, parent: NodeNG
         ) -> nodes.MatchClass:
             newnode = nodes.MatchClass(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
@@ -2427,29 +1871,29 @@
                 kwd_patterns=[
                     self.visit(pattern, newnode) for pattern in node.kwd_patterns
                 ],
             )
             return newnode
 
         def visit_matchstar(
-            self, node: "ast.MatchStar", parent: NodeNG
+            self, node: ast.MatchStar, parent: NodeNG
         ) -> nodes.MatchStar:
             newnode = nodes.MatchStar(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
             # Add AssignName node for 'node.name'
             # https://bugs.python.org/issue43994
             newnode.postinit(name=self.visit_assignname(node, newnode, node.name))
             return newnode
 
-        def visit_matchas(self, node: "ast.MatchAs", parent: NodeNG) -> nodes.MatchAs:
+        def visit_matchas(self, node: ast.MatchAs, parent: NodeNG) -> nodes.MatchAs:
             newnode = nodes.MatchAs(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
@@ -2457,15 +1901,15 @@
             # https://bugs.python.org/issue43994
             newnode.postinit(
                 pattern=self.visit(node.pattern, newnode),
                 name=self.visit_assignname(node, newnode, node.name),
             )
             return newnode
 
-        def visit_matchor(self, node: "ast.MatchOr", parent: NodeNG) -> nodes.MatchOr:
+        def visit_matchor(self, node: ast.MatchOr, parent: NodeNG) -> nodes.MatchOr:
             newnode = nodes.MatchOr(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 end_lineno=node.end_lineno,
                 end_col_offset=node.end_col_offset,
                 parent=parent,
             )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astroid-2.9.3/astroid/scoped_nodes.py` & `astroid-3.0.0a1/astroid/scoped_nodes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
+
 # pylint: disable=unused-import
 
 import warnings
 
 from astroid.nodes.scoped_nodes import (
     AsyncFunctionDef,
     ClassDef,
@@ -20,10 +24,12 @@
     get_wrapping_class,
 )
 
 # We cannot create a __all__ here because it would create a circular import
 # Please remove astroid/scoped_nodes.py|astroid/node_classes.py in autoflake
 # exclude when removing this file.
 warnings.warn(
-    "The 'astroid.scoped_nodes' module is deprecated and will be replaced by 'astroid.nodes' in astroid 3.0.0",
+    "The 'astroid.scoped_nodes' module is deprecated and will be replaced by "
+    "'astroid.nodes' in astroid 3.0.0",
     DeprecationWarning,
+    stacklevel=2,
 )
```

### Comparing `astroid-2.9.3/astroid/test_utils.py` & `astroid-3.0.0a1/astroid/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,51 @@
-# Copyright (c) 2013-2014 Google, Inc.
-# Copyright (c) 2014 LOGILAB S.A. (Paris, FRANCE) <contact@logilab.fr>
-# Copyright (c) 2015-2016, 2018-2020 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2016 Jakub Wilk <jwilk@jwilk.net>
-# Copyright (c) 2018 Anthony Sottile <asottile@umich.edu>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-# Copyright (c) 2021 Andrew Haigh <hello@nelf.in>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Utility functions for test code that uses astroid ASTs as input."""
+
+from __future__ import annotations
+
 import contextlib
 import functools
 import sys
 import warnings
-from typing import Callable, Tuple
+from collections.abc import Callable
 
 import pytest
 
 from astroid import manager, nodes, transforms
 
 
 def require_version(minver: str = "0.0.0", maxver: str = "4.0.0") -> Callable:
-    """Compare version of python interpreter to the given one.
-    Skip the test if older.
-    """
+    """Compare version of python interpreter to the given one and skips the test if older."""
 
-    def parse(python_version: str) -> Tuple[int, ...]:
+    def parse(python_version: str) -> tuple[int, ...]:
         try:
             return tuple(int(v) for v in python_version.split("."))
         except ValueError as e:
             msg = f"{python_version} is not a correct version : should be X.Y[.Z]."
             raise ValueError(msg) from e
 
     min_version = parse(minver)
     max_version = parse(maxver)
 
     def check_require_version(f):
-        current: Tuple[int, int, int] = sys.version_info[:3]
+        current: tuple[int, int, int] = sys.version_info[:3]
         if min_version < current <= max_version:
             return f
 
         version: str = ".".join(str(v) for v in sys.version_info)
 
         @functools.wraps(f)
         def new_f(*args, **kwargs):
-            if minver != "0.0.0":
+            if current <= min_version:
                 pytest.skip(f"Needs Python > {minver}. Current version is {version}.")
-            elif maxver != "4.0.0":
+            elif current > max_version:
                 pytest.skip(f"Needs Python <= {maxver}. Current version is {version}.")
 
         return new_f
 
     return check_require_version
 
 
@@ -78,9 +69,9 @@
     # avoid caching into the AstroidManager borg since we get problems
     # with other tests :
     m.__dict__ = {}
     m._failed_import_hooks = []
     m.astroid_cache = {}
     m._mod_file_cache = {}
     m._transform = transforms.TransformVisitor()
-    m.extension_package_whitelist = {}
+    m.extension_package_whitelist = set()
     return m
```

### Comparing `astroid-2.9.3/astroid/util.py` & `astroid-3.0.0a1/astroid/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,55 @@
-# Copyright (c) 2015-2018 Claudiu Popa <pcmanticore@gmail.com>
-# Copyright (c) 2015-2016 Ceridwen <ceridwenv@gmail.com>
-# Copyright (c) 2018 Bryce Guinta <bryce.paul.guinta@gmail.com>
-# Copyright (c) 2018 Nick Drozd <nicholasdrozd@gmail.com>
-# Copyright (c) 2020-2021 hippo91 <guillaume.peillex@gmail.com>
-# Copyright (c) 2020 Bryce Guinta <bryce.guinta@protonmail.com>
-# Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
-# Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
-
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
-# For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
-
-import importlib
-import warnings
-
-import lazy_object_proxy
+# For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
+# Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 
-def lazy_descriptor(obj):
-    class DescriptorProxy(lazy_object_proxy.Proxy):
-        def __get__(self, instance, owner=None):
-            return self.__class__.__get__(self, instance)
-
-    return DescriptorProxy(obj)
+from __future__ import annotations
 
+import warnings
+from typing import Any, Final, Literal
 
-def lazy_import(module_name):
-    return lazy_object_proxy.Proxy(
-        lambda: importlib.import_module("." + module_name, "astroid")
-    )
 
+class UninferableBase:
+    """Special inference object, which is returned when inference fails.
 
-@object.__new__
-class Uninferable:
-    """Special inference object, which is returned when inference fails."""
+    This is meant to be used as a singleton. Use astroid.util.Uninferable to access it.
+    """
 
-    def __repr__(self):
+    def __repr__(self) -> Literal["Uninferable"]:
         return "Uninferable"
 
     __str__ = __repr__
 
-    def __getattribute__(self, name):
+    def __getattribute__(self, name: str) -> Any:
         if name == "next":
             raise AttributeError("next method should not be called")
         if name.startswith("__") and name.endswith("__"):
             return object.__getattribute__(self, name)
         if name == "accept":
             return object.__getattribute__(self, name)
         return self
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> UninferableBase:
         return self
 
-    def __bool__(self):
+    def __bool__(self) -> Literal[False]:
         return False
 
     __nonzero__ = __bool__
 
     def accept(self, visitor):
         return visitor.visit_uninferable(self)
 
 
+Uninferable: Final = UninferableBase()
+
+
 class BadOperationMessage:
-    """Object which describes a TypeError occurred somewhere in the inference chain
+    """Object which describes a TypeError occurred somewhere in the inference chain.
 
     This is not an exception, but a container object which holds the types and
     the error which occurred.
     """
 
 
 class BadUnaryOperationMessage(BadOperationMessage):
@@ -74,25 +58,26 @@
     def __init__(self, operand, op, error):
         self.operand = operand
         self.op = op
         self.error = error
 
     @property
     def _object_type_helper(self):
-        helpers = lazy_import("helpers")
+        from astroid import helpers  # pylint: disable=import-outside-toplevel
+
         return helpers.object_type
 
     def _object_type(self, obj):
         objtype = self._object_type_helper(obj)
-        if objtype is Uninferable:
+        if isinstance(objtype, UninferableBase):
             return None
 
         return objtype
 
-    def __str__(self):
+    def __str__(self) -> str:
         if hasattr(self.operand, "name"):
             operand_type = self.operand.name
         else:
             object_type = self._object_type(self.operand)
             if hasattr(object_type, "name"):
                 operand_type = object_type.name
             else:
@@ -107,36 +92,36 @@
     """Object which describes type errors for BinOps."""
 
     def __init__(self, left_type, op, right_type):
         self.left_type = left_type
         self.right_type = right_type
         self.op = op
 
-    def __str__(self):
+    def __str__(self) -> str:
         msg = "unsupported operand type(s) for {}: {!r} and {!r}"
         return msg.format(self.op, self.left_type.name, self.right_type.name)
 
 
-def _instancecheck(cls, other):
+def _instancecheck(cls, other) -> bool:
     wrapped = cls.__wrapped__
     other_cls = other.__class__
     is_instance_of = wrapped is other_cls or issubclass(other_cls, wrapped)
     warnings.warn(
         "%r is deprecated and slated for removal in astroid "
         "2.0, use %r instead" % (cls.__class__.__name__, wrapped.__name__),
         PendingDeprecationWarning,
         stacklevel=2,
     )
     return is_instance_of
 
 
-def proxy_alias(alias_name, node_type):
-    """Get a Proxy from the given name to the given node type."""
-    proxy = type(
-        alias_name,
-        (lazy_object_proxy.Proxy,),
-        {
-            "__class__": object.__dict__["__class__"],
-            "__instancecheck__": _instancecheck,
-        },
+def check_warnings_filter() -> bool:
+    """Return True if any other than the default DeprecationWarning filter is enabled.
+
+    https://docs.python.org/3/library/warnings.html#default-warning-filter
+    """
+    return any(
+        issubclass(DeprecationWarning, filter[2])
+        and filter[0] != "ignore"
+        and filter[3] != "__main__"
+        for filter in warnings.filters
     )
-    return proxy(lambda: node_type)
```

### Comparing `astroid-2.9.3/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a1/astroid.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 2.9.3
+Version: 3.0.0a1
 Summary: An abstract syntax tree for Python with inference support.
-Home-page: https://github.com/PyCQA/astroid
-Author: Python Code Quality Authority
-Author-email: code-quality@python.org
 License: LGPL-2.1-or-later
-Project-URL: Bug tracker, https://github.com/PyCQA/astroid/issues
+Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
+Project-URL: Source Code, https://github.com/pylint-dev/astroid
+Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6.2
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+License-File: CONTRIBUTORS.txt
 
 Astroid
 =======
 
-.. image:: https://coveralls.io/repos/github/PyCQA/astroid/badge.svg?branch=main
-    :target: https://coveralls.io/github/PyCQA/astroid?branch=main
-    :alt: Coverage badge from coveralls.io
+.. image:: https://codecov.io/gh/pylint-dev/astroid/branch/main/graph/badge.svg?token=Buxy4WptLb
+    :target: https://codecov.io/gh/pylint-dev/astroid
+    :alt: Coverage badge from codecov
 
 .. image:: https://readthedocs.org/projects/astroid/badge/?version=latest
     :target: http://astroid.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
 
-.. image:: https://results.pre-commit.ci/badge/github/PyCQA/astroid/main.svg
-   :target: https://results.pre-commit.ci/latest/github/PyCQA/astroid/main
+.. image:: https://results.pre-commit.ci/badge/github/pylint-dev/astroid/main.svg
+   :target: https://results.pre-commit.ci/latest/github/pylint-dev/astroid/main
    :alt: pre-commit.ci status
 
-.. |tidelift_logo| image:: https://raw.githubusercontent.com/PyCQA/astroid/main/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
-   :width: 75
-   :height: 60
+.. |tidelift_logo| image:: https://raw.githubusercontent.com/pylint-dev/astroid/main/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+   :width: 200
    :alt: Tidelift
 
 .. list-table::
    :widths: 10 100
 
    * - |tidelift_logo|
      - Professional support for astroid is available as part of the
@@ -117,10 +114,8 @@
 Test
 ----
 
 Tests are in the 'test' subdirectory. To launch the whole tests suite, you can use
 either `tox` or `pytest`::
 
     tox
-    pytest astroid
-
-
+    pytest
```

