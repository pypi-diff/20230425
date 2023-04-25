# Comparing `tmp/pygptj-1.0.5.tar.gz` & `tmp/pygptj-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygptj-1.0.5.tar", last modified: Sun Apr 23 02:24:36 2023, max compression
+gzip compressed data, was "pygptj-1.0.6.tar", last modified: Tue Apr 25 03:21:37 2023, max compression
```

## Comparing `pygptj-1.0.5.tar` & `pygptj-1.0.6.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.534120 pygptj-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-23 02:24:25.000000 pygptj-1.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 02:24:25.000000 pygptj-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 02:24:25.000000 pygptj-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-23 02:24:36.534120 pygptj-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-23 02:24:25.000000 pygptj-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/examples/gpt-2/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/examples/gpt-2/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/examples/gpt-j/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/examples/gpt-j/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/ggml/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/examples/mnist/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.526120 pygptj-1.0.5/ggml/examples/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/examples/whisper/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.526120 pygptj-1.0.5/ggml/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.526120 pygptj-1.0.5/ggml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-23 02:24:27.000000 pygptj-1.0.5/ggml/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.526120 pygptj-1.0.5/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.526120 pygptj-1.0.5/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.530120 pygptj-1.0.5/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-23 02:24:25.000000 pygptj-1.0.5/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.522120 pygptj-1.0.5/pygptj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:25.000000 pygptj-1.0.5/pygptj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-23 02:24:25.000000 pygptj-1.0.5/pygptj/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 02:24:25.000000 pygptj-1.0.5/pygptj/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-23 02:24:25.000000 pygptj-1.0.5/pygptj/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.534120 pygptj-1.0.5/pygptj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-23 02:24:36.000000 pygptj-1.0.5/pygptj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-23 02:24:36.000000 pygptj-1.0.5/pygptj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:36.000000 pygptj-1.0.5/pygptj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:36.000000 pygptj-1.0.5/pygptj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 02:24:36.000000 pygptj-1.0.5/pygptj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 02:24:25.000000 pygptj-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 02:24:36.534120 pygptj-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-23 02:24:25.000000 pygptj-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:36.534120 pygptj-1.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/GGML_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27298 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/gptj.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-23 02:24:25.000000 pygptj-1.0.5/src/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.078075 pygptj-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-25 03:21:25.000000 pygptj-1.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 03:21:25.000000 pygptj-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 03:21:25.000000 pygptj-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 03:21:37.078075 pygptj-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 03:21:25.000000 pygptj-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.066075 pygptj-1.0.6/ggml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.066075 pygptj-1.0.6/ggml/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.066075 pygptj-1.0.6/ggml/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/examples/gpt-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/examples/gpt-2/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/examples/gpt-j/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/examples/gpt-j/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/examples/mnist/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/examples/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/examples/whisper/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/ggml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-25 03:21:26.000000 pygptj-1.0.6/ggml/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.066075 pygptj-1.0.6/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.070075 pygptj-1.0.6/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 03:21:25.000000 pygptj-1.0.6/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.066075 pygptj-1.0.6/pygptj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:25.000000 pygptj-1.0.6/pygptj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 03:21:25.000000 pygptj-1.0.6/pygptj/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 03:21:25.000000 pygptj-1.0.6/pygptj/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-25 03:21:25.000000 pygptj-1.0.6/pygptj/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.074075 pygptj-1.0.6/pygptj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 03:21:37.000000 pygptj-1.0.6/pygptj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 03:21:37.000000 pygptj-1.0.6/pygptj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:37.000000 pygptj-1.0.6/pygptj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:36.000000 pygptj-1.0.6/pygptj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 03:21:37.000000 pygptj-1.0.6/pygptj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 03:21:25.000000 pygptj-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:21:37.078075 pygptj-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-25 03:21:25.000000 pygptj-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:37.078075 pygptj-1.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/GGML_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/gptj.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/gptj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-25 03:21:25.000000 pygptj-1.0.6/src/utils.h
```

### Comparing `pygptj-1.0.5/CMakeLists.txt` & `pygptj-1.0.6/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
 
 add_subdirectory(pybind11)
 add_subdirectory(ggml)
 
 include_directories(ggml/include/ggml)
 
-# file (GLOB CPP_FILES "src/*.cpp")
+file (GLOB CPP_FILES "src/*.cpp")
 file (GLOB C_FILES "ggml/src/*.c")
 file (GLOB H_FILES "ggml/include/ggml/*.h")
 
 # ---------------------------------------------------------------------------------------------
 
 set(CMAKE_EXPORT_COMPILE_COMMANDS "on")
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
```

### Comparing `pygptj-1.0.5/LICENSE` & `pygptj-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/PKG-INFO` & `pygptj-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygptj
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python bindings for the GGML GPT-J Laguage model
 Author: Abdeladim Sadiki
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pygptj-1.0.5/README.md` & `pygptj-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/ggml/CMakeLists.txt` & `pygptj-1.0.6/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/ggml/cmake/BuildTypes.cmake` & `pygptj-1.0.6/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/ggml/cmake/GitVars.cmake` & `pygptj-1.0.6/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/ggml/src/CMakeLists.txt` & `pygptj-1.0.6/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/ggml/tests/CMakeLists.txt` & `pygptj-1.0.6/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/CMakeLists.txt` & `pygptj-1.0.6/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/LICENSE` & `pygptj-1.0.6/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/attr.h` & `pygptj-1.0.6/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/buffer_info.h` & `pygptj-1.0.6/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/cast.h` & `pygptj-1.0.6/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/chrono.h` & `pygptj-1.0.6/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/complex.h` & `pygptj-1.0.6/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/class.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/common.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/descr.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/init.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/internals.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/type_caster_base.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/detail/typeid.h` & `pygptj-1.0.6/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/eigen.h` & `pygptj-1.0.6/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/embed.h` & `pygptj-1.0.6/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/eval.h` & `pygptj-1.0.6/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/functional.h` & `pygptj-1.0.6/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/gil.h` & `pygptj-1.0.6/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/iostream.h` & `pygptj-1.0.6/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/numpy.h` & `pygptj-1.0.6/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/operators.h` & `pygptj-1.0.6/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/options.h` & `pygptj-1.0.6/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/pybind11.h` & `pygptj-1.0.6/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/pytypes.h` & `pygptj-1.0.6/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/stl/filesystem.h` & `pygptj-1.0.6/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/stl.h` & `pygptj-1.0.6/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/include/pybind11/stl_bind.h` & `pygptj-1.0.6/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tests/test_embed/CMakeLists.txt` & `pygptj-1.0.6/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/FindCatch.cmake` & `pygptj-1.0.6/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/FindEigen3.cmake` & `pygptj-1.0.6/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/FindPythonLibsNew.cmake` & `pygptj-1.0.6/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/check-style.sh` & `pygptj-1.0.6/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/cmake_uninstall.cmake.in` & `pygptj-1.0.6/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/libsize.py` & `pygptj-1.0.6/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/make_changelog.py` & `pygptj-1.0.6/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/pybind11Common.cmake` & `pygptj-1.0.6/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/pybind11Config.cmake.in` & `pygptj-1.0.6/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/pybind11NewTools.cmake` & `pygptj-1.0.6/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/pybind11Tools.cmake` & `pygptj-1.0.6/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/setup_global.py.in` & `pygptj-1.0.6/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pybind11/tools/setup_main.py.in` & `pygptj-1.0.6/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pygptj/_logger.py` & `pygptj-1.0.6/pygptj/_logger.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pygptj/model.py` & `pygptj-1.0.6/pygptj/model.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/pygptj.egg-info/PKG-INFO` & `pygptj-1.0.6/pygptj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygptj
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python bindings for the GGML GPT-J Laguage model
 Author: Abdeladim Sadiki
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pygptj-1.0.5/pygptj.egg-info/SOURCES.txt` & `pygptj-1.0.6/pygptj.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -73,11 +73,12 @@
 pygptj.egg-info/PKG-INFO
 pygptj.egg-info/SOURCES.txt
 pygptj.egg-info/dependency_links.txt
 pygptj.egg-info/not-zip-safe
 pygptj.egg-info/top_level.txt
 src/GGML_LICENSE
 src/gptj.cpp
+src/gptj.h
 src/main.cpp
 src/main.h
 src/utils.cpp
 src/utils.h
```

### Comparing `pygptj-1.0.5/pyproject.toml` & `pygptj-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/setup.py` & `pygptj-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pygptj",
-    version="1.0.5",
+    version="1.0.6",
     author="Abdeladim Sadiki",
     description="Python bindings for the GGML GPT-J Laguage model",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pygptj")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pygptj-1.0.5/src/GGML_LICENSE` & `pygptj-1.0.6/src/GGML_LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/src/gptj.cpp` & `pygptj-1.0.6/src/gptj.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -3,83 +3,30 @@
  * @file    gptj.cpp
  * @brief   GPT-J model taken from [ggml/examples/gpt-j/main.cpp](https://github.com/ggerganov/ggml/tree/master/examples/gpt-j/main.cpp)
  * @par     ggml is licensed under MIT Copyright (c) 2022 Georgi Gerganov,
             please see [ggml License](./GGML_LICENSE)
  ********************************************************************************
  */
 
-#include "ggml.h"
 #include "utils.h"
+#include "gptj.h"
 
 #include <cassert>
 #include <cmath>
 #include <cstdio>
 #include <cstring>
 #include <fstream>
 #include <map>
 #include <string>
 #include <vector>
 #include <iostream>
 
 #include <pybind11/pybind11.h>
 namespace py = pybind11;
 
-// default hparams (GPT-J 6B)
-struct gptj_hparams {
-    int32_t n_vocab = 50400;
-    int32_t n_ctx   = 2048;
-    int32_t n_embd  = 4096;
-    int32_t n_head  = 16;
-    int32_t n_layer = 28;
-    int32_t n_rot   = 64;
-    int32_t f16     = 1;
-};
-
-struct gptj_layer {
-    // normalization
-    struct ggml_tensor * ln_1_g;
-    struct ggml_tensor * ln_1_b;
-
-    // attention
-    struct ggml_tensor * c_attn_q_proj_w;
-    struct ggml_tensor * c_attn_k_proj_w;
-    struct ggml_tensor * c_attn_v_proj_w;
-
-    struct ggml_tensor * c_attn_proj_w;
-
-    // ff
-    struct ggml_tensor * c_mlp_fc_w;
-    struct ggml_tensor * c_mlp_fc_b;
-
-    struct ggml_tensor * c_mlp_proj_w;
-    struct ggml_tensor * c_mlp_proj_b;
-};
-
-struct gptj_model {
-    gptj_hparams hparams;
-
-    // normalization
-    struct ggml_tensor * ln_f_g;
-    struct ggml_tensor * ln_f_b;
-
-    struct ggml_tensor * wte; // position embedding
-
-    struct ggml_tensor * lmh_g; // language model head
-    struct ggml_tensor * lmh_b; // language model bias
-
-    std::vector<gptj_layer> layers;
-
-    // key + value memory
-    struct ggml_tensor * memory_k;
-    struct ggml_tensor * memory_v;
-
-    //
-    struct ggml_context * ctx;
-    std::map<std::string, struct ggml_tensor *> tensors;
-};
 
 // load the model's weights from a file
 bool gptj_model_load(const std::string & fname, gptj_model & model, gpt_vocab & vocab) {
     printf("%s: loading model from '%s' - please wait ...\n", __func__, fname.c_str());
 
     auto fin = std::ifstream(fname, std::ios::binary);
     if (!fin) {
@@ -658,17 +605,14 @@
 //        } else {
 //            params.prompt = gpt_random_prompt(rng);
 //        }
 //    }
 
     int64_t t_load_us = 0;
 
-
-
-
     // load the model
 //    {
 //        const int64_t t_start_us = ggml_time_us();
 //
 //        if (!gptj_model_load(params.model, model, vocab)) {
 //            fprintf(stderr, "%s: failed to load model from '%s'\n", __func__, params.model.c_str());
 //            return 1;
@@ -681,15 +625,15 @@
 
     int64_t t_sample_us  = 0;
     int64_t t_predict_us = 0;
 
     std::vector<float> logits;
 
     // tokenize the prompt
-    std::vector<gpt_vocab::id> embd_inp = ::gpt_tokenize(vocab, params.prompt);
+    std::vector<gpt_vocab::id> embd_inp = gpt_tokenize(vocab, params.prompt);
 
     params.n_predict = std::min(params.n_predict, model.hparams.n_ctx - (int) embd_inp.size());
 
     printf("%s: number of tokens in prompt = %zu\n", __func__, embd_inp.size());
     printf("\n");
 
     std::vector<gpt_vocab::id> embd;
@@ -743,16 +687,15 @@
                 }
             }
             i += embd.size() - 1;
         }
 
         // display text
         for (auto id : embd) {
-            new_text_callback(vocab.id_to_token[id].c_str());
-//            printf("%s", vocab.id_to_token[id].c_str());
+            new_text_callback(py::str(vocab.id_to_token[id].c_str()));
         }
         fflush(stdout);
 
         // end of text token
         if (embd.back() == 50256) {
             break;
         }
```

### Comparing `pygptj-1.0.5/src/main.cpp` & `pygptj-1.0.6/src/main.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,16 @@
  */
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/functional.h>
 #include <pybind11/numpy.h>
 
-#include "utils.cpp"
-#include "gptj.cpp"
+#include "utils.h"
+#include "gptj.h"
 #include "main.h"
 
 
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
@@ -46,15 +46,17 @@
         .def_readwrite("n_threads", &gpt_params::n_threads)
         .def_readwrite("n_predict", &gpt_params::n_predict)
         .def_readwrite("top_k", &gpt_params::top_k)
         .def_readwrite("top_p", &gpt_params::top_p)
         .def_readwrite("temp", &gpt_params::temp)
         .def_readwrite("n_batch", &gpt_params::n_batch)
         .def_readwrite("model", &gpt_params::model)
-        .def_readwrite("prompt", &gpt_params::prompt)
+//        .def_readwrite("prompt", &gpt_params::prompt)
+        .def_property("prompt", [](gpt_params &self) {return py::str(self.prompt);},
+                                 [](gpt_params &self, py::str &prompt) {self.prompt = prompt.cast<std::string>();})
         ;
 
     py::class_<gptj_hparams>(m,"gptj_hparams" /*,py::dynamic_attr()*/)
         .def(py::init<>())
         ;
     py::class_<gptj_model>(m,"gptj_model" /*,py::dynamic_attr()*/)
         .def(py::init<>())
```

### Comparing `pygptj-1.0.5/src/utils.cpp` & `pygptj-1.0.6/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.5/src/utils.h` & `pygptj-1.0.6/src/utils.h`

 * *Files identical despite different names*

