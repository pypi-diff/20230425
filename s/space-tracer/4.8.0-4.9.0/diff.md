# Comparing `tmp/space_tracer-4.8.0.tar.gz` & `tmp/space_tracer-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_tracer-4.8.0.tar", last modified: Tue Feb  8 01:45:10 2022, max compression
+gzip compressed data, was "space_tracer-4.9.0.tar", last modified: Tue Nov 29 06:51:21 2022, max compression
```

## Comparing `space_tracer-4.8.0.tar` & `space_tracer-4.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:10.126984 space_tracer-4.8.0/
--rw-rw-r--   0 don       (1000) don       (1000)      159 2021-04-04 21:59:33.000000 space_tracer-4.8.0/MANIFEST.in
--rw-rw-r--   0 don       (1000) don       (1000)     3378 2022-02-08 01:45:10.122983 space_tracer-4.8.0/PKG-INFO
--rw-rw-r--   0 don       (1000) don       (1000)     9861 2022-02-08 01:35:45.000000 space_tracer-4.8.0/README.md
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.558981 space_tracer-4.8.0/docs/
--rw-rw-r--   0 don       (1000) don       (1000)    29430 2021-11-12 15:48:38.000000 space_tracer-4.8.0/docs/starting_space_tracer.md
--rw-rw-r--   0 don       (1000) don       (1000)     1066 2021-04-04 21:59:34.000000 space_tracer-4.8.0/license.txt
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.554981 space_tracer-4.8.0/plugin/
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.554981 space_tracer-4.8.0/plugin/PySrc/
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.586981 space_tracer-4.8.0/plugin/PySrc/space_tracer/
--rw-rw-r--   0 don       (1000) don       (1000)      385 2021-11-06 15:52:37.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)       93 2021-04-04 21:59:34.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/__main__.py
--rw-rw-r--   0 don       (1000) don       (1000)      392 2022-02-08 01:39:46.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/about.py
--rw-rw-r--   0 don       (1000) don       (1000)     5344 2022-01-30 19:42:33.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/canvas.py
--rw-rw-r--   0 don       (1000) don       (1000)    33084 2021-10-22 23:17:28.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/code_tracer.py
--rw-rw-r--   0 don       (1000) don       (1000)    15700 2022-01-06 03:35:15.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/live_image.py
--rw-rw-r--   0 don       (1000) don       (1000)    28478 2021-12-28 06:23:34.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/main.py
--rw-rw-r--   0 don       (1000) don       (1000)    30605 2022-01-30 19:42:33.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/mock_turtle.py
--rw-rw-r--   0 don       (1000) don       (1000)    18360 2021-11-02 01:52:15.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/module_importers.py
--rw-rw-r--   0 don       (1000) don       (1000)    19264 2021-04-10 21:48:51.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/report_builder.py
--rw-rw-r--   0 don       (1000) don       (1000)     1490 2021-04-04 21:59:34.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer/traced_finder.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.586981 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/
--rw-rw-rw-   0 don       (1000) don       (1000)     3378 2022-02-08 01:45:08.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/PKG-INFO
--rw-rw-rw-   0 don       (1000) don       (1000)     2048 2022-02-08 01:45:08.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/SOURCES.txt
--rw-rw-rw-   0 don       (1000) don       (1000)        1 2022-02-08 01:45:08.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/dependency_links.txt
--rw-rw-rw-   0 don       (1000) don       (1000)       52 2022-02-08 01:45:08.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/entry_points.txt
--rw-rw-rw-   0 don       (1000) don       (1000)       13 2022-02-08 01:45:08.000000 space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/top_level.txt
--rw-rw-r--   0 don       (1000) don       (1000)      170 2021-04-04 21:59:34.000000 space_tracer-4.8.0/pytest.ini
--rw-rw-r--   0 don       (1000) don       (1000)       38 2022-02-08 01:45:10.126984 space_tracer-4.8.0/setup.cfg
--rw-rw-r--   0 don       (1000) don       (1000)     1514 2022-01-31 22:25:21.000000 space_tracer-4.8.0/setup.py
--rw-rw-r--   0 don       (1000) don       (1000)     2349 2021-04-04 21:59:34.000000 space_tracer-4.8.0/space_tracer.md
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.558981 space_tracer-4.8.0/test/
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:09.558981 space_tracer-4.8.0/test/PySrc/
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:10.058983 space_tracer-4.8.0/test/PySrc/tests/
--rw-rw-r--   0 don       (1000) don       (1000)      237 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_driver.py
--rw-rw-r--   0 don       (1000) don       (1000)       66 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_driver_syntax_error.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-02-08 01:45:10.122983 space_tracer-4.8.0/test/PySrc/tests/example_package/
--rw-rw-rw-   0 don       (1000) don       (1000)        0 2017-10-11 05:11:08.000000 space_tracer-4.8.0/test/PySrc/tests/example_package/__init__.py
--rw-rw-rw-   0 don       (1000) don       (1000)       95 2017-10-11 05:11:08.000000 space_tracer-4.8.0/test/PySrc/tests/example_package/__main__.py
--rw-rw-rw-   0 don       (1000) don       (1000)      118 2019-06-29 22:59:52.000000 space_tracer-4.8.0/test/PySrc/tests/example_package/driver_in_package.py
--rw-rw-rw-   0 don       (1000) don       (1000)       47 2017-10-11 05:11:08.000000 space_tracer-4.8.0/test/PySrc/tests/example_package/lib_in_package.py
--rw-rw-r--   0 don       (1000) don       (1000)      179 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_patching_driver.py
--rw-rw-r--   0 don       (1000) don       (1000)      166 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_printing.py
--rw-rw-r--   0 don       (1000) don       (1000)       86 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_pycharm_failures.py
--rw-rw-r--   0 don       (1000) don       (1000)      348 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_silent_driver.py
--rw-rw-r--   0 don       (1000) don       (1000)      121 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/example_source.py
--rw-rw-r--   0 don       (1000) don       (1000)      193 2021-04-11 01:40:13.000000 space_tracer-4.8.0/test/PySrc/tests/example_traced.py
--rw-rw-r--   0 don       (1000) don       (1000)     2511 2021-12-27 19:23:29.000000 space_tracer-4.8.0/test/PySrc/tests/test_canvas.py
--rw-rw-r--   0 don       (1000) don       (1000)    19719 2021-11-06 16:01:23.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer.py
--rw-rw-r--   0 don       (1000) don       (1000)     4178 2021-10-22 22:59:06.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_assignment.py
--rw-rw-r--   0 don       (1000) don       (1000)     3654 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_function.py
--rw-rw-r--   0 don       (1000) don       (1000)     4499 2021-04-10 21:55:14.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_loops.py
--rw-rw-r--   0 don       (1000) don       (1000)    29491 2021-12-25 01:01:07.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_main.py
--rw-rw-r--   0 don       (1000) don       (1000)     1611 2021-11-01 05:57:24.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_matplotlib.py
--rw-rw-r--   0 don       (1000) don       (1000)     8894 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_print.py
--rw-rw-r--   0 don       (1000) don       (1000)     6005 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_pytest.py
--rw-rw-r--   0 don       (1000) don       (1000)     4572 2021-04-10 21:54:10.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_repr.py
--rw-rw-r--   0 don       (1000) don       (1000)     1619 2021-07-01 19:40:09.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_structural_match.py
--rw-rw-r--   0 don       (1000) don       (1000)     3696 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_width.py
--rw-rw-r--   0 don       (1000) don       (1000)    11745 2021-12-28 06:52:58.000000 space_tracer-4.8.0/test/PySrc/tests/test_live_image.py
--rw-rw-r--   0 don       (1000) don       (1000)    20210 2022-01-30 19:42:33.000000 space_tracer-4.8.0/test/PySrc/tests/test_mock_turtle.py
--rw-rw-r--   0 don       (1000) don       (1000)    18068 2021-10-29 04:10:58.000000 space_tracer-4.8.0/test/PySrc/tests/test_report_builder.py
--rw-rw-r--   0 don       (1000) don       (1000)    20758 2021-04-11 02:42:23.000000 space_tracer-4.8.0/test/PySrc/tests/test_traced.py
--rw-rw-r--   0 don       (1000) don       (1000)     1736 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/test_traced_finder.py
--rw-rw-r--   0 don       (1000) don       (1000)      621 2021-04-04 21:59:34.000000 space_tracer-4.8.0/test/PySrc/tests/validate_legacy_python.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.780652 space_tracer-4.9.0/
+-rw-rw-r--   0 don       (1000) don       (1000)      159 2022-03-26 15:42:28.000000 space_tracer-4.9.0/MANIFEST.in
+-rw-rw-r--   0 don       (1000) don       (1000)     3342 2022-11-29 06:51:21.780652 space_tracer-4.9.0/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)     9974 2022-05-06 15:31:34.000000 space_tracer-4.9.0/README.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.772652 space_tracer-4.9.0/docs/
+-rw-rw-r--   0 don       (1000) don       (1000)    29430 2022-03-26 15:42:28.000000 space_tracer-4.9.0/docs/starting_space_tracer.md
+-rw-rw-r--   0 don       (1000) don       (1000)     1066 2022-03-26 15:42:28.000000 space_tracer-4.9.0/license.txt
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.768652 space_tracer-4.9.0/plugin/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.768652 space_tracer-4.9.0/plugin/PySrc/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.772652 space_tracer-4.9.0/plugin/PySrc/space_tracer/
+-rw-rw-r--   0 don       (1000) don       (1000)      385 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)       93 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/__main__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      392 2022-11-29 06:24:29.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/about.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5344 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/canvas.py
+-rw-rw-r--   0 don       (1000) don       (1000)    33196 2022-11-25 18:53:43.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/code_tracer.py
+-rw-rw-r--   0 don       (1000) don       (1000)    15755 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/live_image.py
+-rw-rw-r--   0 don       (1000) don       (1000)    28808 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/main.py
+-rw-rw-r--   0 don       (1000) don       (1000)    30733 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/mock_turtle.py
+-rw-rw-r--   0 don       (1000) don       (1000)    18430 2022-09-24 17:44:44.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/module_importers.py
+-rw-rw-r--   0 don       (1000) don       (1000)    19264 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/report_builder.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1490 2022-09-24 15:03:38.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer/traced_finder.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.772652 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/
+-rw-rw-r--   0 don       (1000) don       (1000)     3342 2022-11-29 06:51:21.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)     2048 2022-11-29 06:51:21.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/SOURCES.txt
+-rw-rw-r--   0 don       (1000) don       (1000)        1 2022-11-29 06:51:21.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/dependency_links.txt
+-rw-rw-r--   0 don       (1000) don       (1000)       51 2022-11-29 06:51:21.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/entry_points.txt
+-rw-rw-r--   0 don       (1000) don       (1000)       13 2022-11-29 06:51:21.000000 space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/top_level.txt
+-rw-rw-r--   0 don       (1000) don       (1000)      170 2022-03-26 15:42:28.000000 space_tracer-4.9.0/pytest.ini
+-rw-rw-r--   0 don       (1000) don       (1000)       38 2022-11-29 06:51:21.780652 space_tracer-4.9.0/setup.cfg
+-rw-rw-r--   0 don       (1000) don       (1000)     1593 2022-11-25 18:53:43.000000 space_tracer-4.9.0/setup.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2349 2022-03-26 15:42:28.000000 space_tracer-4.9.0/space_tracer.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.768652 space_tracer-4.9.0/test/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.768652 space_tracer-4.9.0/test/PySrc/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.776652 space_tracer-4.9.0/test/PySrc/tests/
+-rw-rw-r--   0 don       (1000) don       (1000)      237 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_driver.py
+-rw-rw-r--   0 don       (1000) don       (1000)       66 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_driver_syntax_error.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2022-11-29 06:51:21.780652 space_tracer-4.9.0/test/PySrc/tests/example_package/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_package/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)       95 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_package/__main__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      118 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_package/driver_in_package.py
+-rw-rw-r--   0 don       (1000) don       (1000)       47 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_package/lib_in_package.py
+-rw-rw-r--   0 don       (1000) don       (1000)      179 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_patching_driver.py
+-rw-rw-r--   0 don       (1000) don       (1000)      166 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_printing.py
+-rw-rw-r--   0 don       (1000) don       (1000)       86 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_pycharm_failures.py
+-rw-rw-r--   0 don       (1000) don       (1000)      348 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_silent_driver.py
+-rw-rw-r--   0 don       (1000) don       (1000)      121 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_source.py
+-rw-rw-r--   0 don       (1000) don       (1000)      193 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/example_traced.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2511 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_canvas.py
+-rw-rw-r--   0 don       (1000) don       (1000)    19719 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4178 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_assignment.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3654 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_function.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4499 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_loops.py
+-rw-rw-r--   0 don       (1000) don       (1000)    29491 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_main.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3270 2022-05-11 23:25:58.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_matplotlib.py
+-rw-rw-r--   0 don       (1000) don       (1000)     8894 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_print.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6005 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_pytest.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4572 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_repr.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1619 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_structural_match.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3696 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_width.py
+-rw-rw-r--   0 don       (1000) don       (1000)    13785 2022-04-04 00:00:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_live_image.py
+-rw-rw-r--   0 don       (1000) don       (1000)    20215 2022-05-18 02:04:36.000000 space_tracer-4.9.0/test/PySrc/tests/test_mock_turtle.py
+-rw-rw-r--   0 don       (1000) don       (1000)    18068 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_report_builder.py
+-rw-rw-r--   0 don       (1000) don       (1000)    20758 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_traced.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1736 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/test_traced_finder.py
+-rw-rw-r--   0 don       (1000) don       (1000)      621 2022-03-26 15:42:28.000000 space_tracer-4.9.0/test/PySrc/tests/validate_legacy_python.py
```

### Comparing `space_tracer-4.8.0/PKG-INFO` & `space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
-Name: space_tracer
-Version: 4.8.0
+Name: space-tracer
+Version: 4.9.0
 Summary: Trade time for space when debugging your code.
 Home-page: https://donkirkby.github.io/live-py-plugin/
 Author: Don Kirkby
 Author-email: donkirkby@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/live-py-plugin/issues
 Project-URL: Source, https://github.com/donkirkby/live-py-plugin
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Debuggers
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 
 Space Tracer
@@ -67,9 +65,7 @@
         message += '!'       | message = 'Hello, World!' | message = 'Hello, World!!' | message = 'Hello, World!!!' 
     print(message)           | print('Hello, World!!!') 
     $
 
 [Live Coding in Python]: https://donkirkby.github.io/live-py-plugin/
 [Getting Started]: https://donkirkby.github.io/live-py-plugin/starting_space_tracer.html
 [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-
-
```

### Comparing `space_tracer-4.8.0/README.md` & `space_tracer-4.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [![Python Build Status]][actions]
 [![HTML Build Status]][actions]
 [![Code Coverage]][codecov]
 [![PyCharm downloads]][pycharm plugin]
 [![Sublime downloads]][sublime plugin]
 [![space-tracer downloads]][space-tracer]
+[![DOI]][zenodo]
 
 Visualize your Python code while you type it in PyCharm, Emacs, Sublime Text, or
 even your browser.
 
 [Python Build Status]: https://github.com/donkirkby/live-py-plugin/actions/workflows/py-build.yml/badge.svg?branch=master
 [HTML Build Status]: https://github.com/donkirkby/live-py-plugin/actions/workflows/html-build.yml/badge.svg?branch=master
 [actions]: https://github.com/donkirkby/live-py-plugin/actions
@@ -18,15 +19,16 @@
 [codecov]: https://codecov.io/github/donkirkby/live-py-plugin?branch=master
 [PyCharm downloads]: https://img.shields.io/jetbrains/plugin/d/9742?label=PyCharm%20%E2%86%93
 [pycharm plugin]: https://plugins.jetbrains.com/plugin/9742
 [Sublime downloads]: https://img.shields.io/packagecontrol/dt/Live%20Coding%20in%20Python?label=Sublime%20%E2%86%93
 [sublime plugin]: https://packagecontrol.io/packages/Live%20Coding%20in%20Python
 [space-tracer downloads]: https://static.pepy.tech/personalized-badge/space-tracer?left_color=grey&right_color=brightgreen&left_text=space-tracer%20%E2%86%93
 [space-tracer]: https://pypi.org/project/space-tracer/
-
+[DOI]: https://zenodo.org/badge/4332096.svg
+[zenodo]: https://zenodo.org/badge/latestdoi/4332096
 To see how to use one of the Live Coding in Python plugins, watch the
 [demo video][video] or read the getting started pages for [PyCharm], [Emacs],
 or [Sublime Text]. Want to try it without installing anything? Try the
 [browser version]. You can also try [Space Tracer], the command-line tool that
 trades time for space when you debug. You might also find some useful examples
 in the [tools folder][tools]. To learn more, read about [how it works][how].
```

### Comparing `space_tracer-4.8.0/docs/starting_space_tracer.md` & `space_tracer-4.9.0/docs/starting_space_tracer.md`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/license.txt` & `space_tracer-4.9.0/license.txt`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/canvas.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/canvas.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/code_tracer.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/code_tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,14 +783,16 @@
     def visit(self, node):
         lineno = getattr(node, 'lineno', None)
         if lineno is not None:
             if lineno < self.max_line:
                 node.lineno = self.max_line
             else:
                 self.max_line = lineno
+            if getattr(node, 'end_lineno', lineno) < node.lineno:
+                node.end_lineno = node.lineno
         return self.generic_visit(node)
 
 
 def trace_source_tree(source_tree):
     source_tree = Tracer().visit(source_tree)
     fix_missing_locations(source_tree)
     LineNumberCleaner().visit(source_tree)
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/live_image.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/live_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     @abstractmethod
     def convert_to_png(self) -> bytes:
         """ Convert this image to bytes in PNG format.
 
         Override this method for any subclass to handle an image format.
         """
-        pass
 
     def convert_to_painter(self) -> 'LivePainter':
         """ Convert this image to one that can be edited.
 
         Override this method if you don't want to depend on Pillow.
         """
         png_file = io.BytesIO(self.convert_to_png())
@@ -143,21 +142,22 @@
 class LiveFigure(LiveImage):
     def __init__(self, figure):
         super().__init__()
         self.figure = figure
 
     def convert_to_png(self) -> bytes:
         data = io.BytesIO()
-        self.figure.savefig(data, format='PNG')
+        self.figure.savefig(data, format='PNG', dpi=self.figure.dpi)
 
         return data.getvalue()
 
 
 class LiveImageDiffer:
     def __init__(self, diffs_path: Path = None, request=None, is_displayed=True):
+        # noinspection PySingleQuotedDocstring
         ''' Initialize the object and clean out the diffs path.
 
         This class requires Pillow to be installed, but you can remove that
         dependency with a subclass that overrides the start_diff() and
         end_diff() methods.
 
         A good way to use this class is to create a session fixture and regular
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/main.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,15 @@
                        '--stdout', '!',
                        '--stderr', '!']
         if canvas_size is not None:
             canvas_width, canvas_height = canvas_size
             tracer_args.append('--canvas')
             tracer_args.append('-x{}'.format(canvas_width))
             tracer_args.append('-y{}'.format(canvas_height))
+            tracer_args.append('--zoomed')
         tracer_args.append(PSEUDO_FILENAME)
         code_report = tracer.trace_command(tracer_args)
     stdout = tracer.standard_files.old_files['stderr'].getvalue()
     return code_report, stdout
 
 
 def web_main():
@@ -416,14 +417,22 @@
             self.canvas = Canvas(args.width, args.height)
         was_patched = False
         if MockTurtle is not None:
             if MockTurtle.is_patched():
                 was_patched = True
             else:
                 MockTurtle.monkey_patch(self.canvas)
+        plt = sys.modules.get('matplotlib.pyplot')
+        if plt is not None:
+            # Clear any plot state from previous runs.
+            plt.close()
+            plt.live_coding_size = (args.width, args.height)
+            if args.zoomed:
+                plt.live_coding_zoom()
+
         self.standard_files['stdin'] = args.stdin
         self.standard_files['stdout'] = args.stdout
         self.standard_files['stderr'] = args.stderr
         self.standard_files['report'] = args.report
 
         ReportBuilder.hide = args.hide
         ReportBuilder.is_using_traced_blocks = False
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/mock_turtle.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/mock_turtle.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 try:
     import tkinter as tk
 except ImportError:
     tkinter_name = 'tkinter'
     tk = sys.modules[tkinter_name] = types.ModuleType(tkinter_name)
 
     tk.Frame = tk.Canvas = tk.Tk = tk.ROUND = object
-    tk.mainloop = lambda *args, **kwargs: None
+    class TkMisc: pass
+    tk.Misc = TkMisc()
+    class TclError(Exception): pass
+    tk.TclError = TclError
+    tk.mainloop = tk.Misc.mainloop = lambda *args, **kwargs: None
 
     dialog_name = tkinter_name + '.simpledialog'
     tk.simpledialog = sys.modules[dialog_name] = types.ModuleType(dialog_name)
 
 from turtle import RawTurtle, TurtleScreen, TurtleGraphicsError
 
 DEFAULT_FONT = ("Arial", 8, "normal")
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/module_importers.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/module_importers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ast import parse
 import builtins
+from functools import partial
 from importlib.abc import MetaPathFinder, Loader
 from importlib.machinery import ModuleSpec
 from importlib.util import find_spec
 import inspect
 import os
 import sys
 import types
@@ -403,15 +404,15 @@
             module.use('Agg')
         elif self.fullname == 'matplotlib.pyplot':
             self.plt = module
             # noinspection PyProtectedMember
             turtle_screen = MockTurtle._screen
             screen_width = turtle_screen.cv.cget('width')
             screen_height = turtle_screen.cv.cget('height')
-            module.show = self.mock_show
+            module.show = partial(self.mock_show)  # Lets it accept a signature.
             module.live_coding_size = (screen_width, screen_height)
             module.live_coding_zoom = self.live_coding_zoom
             if self.is_zoomed:
                 self.live_coding_zoom()
         elif self.fullname == 'pyglet':
             # noinspection PyProtectedMember
             monkey_patch_pyglet(MockTurtle._screen.cv)
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/report_builder.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/report_builder.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer/traced_finder.py` & `space_tracer-4.9.0/plugin/PySrc/space_tracer/traced_finder.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/PKG-INFO` & `space_tracer-4.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
-Name: space-tracer
-Version: 4.8.0
+Name: space_tracer
+Version: 4.9.0
 Summary: Trade time for space when debugging your code.
 Home-page: https://donkirkby.github.io/live-py-plugin/
 Author: Don Kirkby
 Author-email: donkirkby@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/live-py-plugin/issues
 Project-URL: Source, https://github.com/donkirkby/live-py-plugin
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Debuggers
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 
 Space Tracer
@@ -67,9 +65,7 @@
         message += '!'       | message = 'Hello, World!' | message = 'Hello, World!!' | message = 'Hello, World!!!' 
     print(message)           | print('Hello, World!!!') 
     $
 
 [Live Coding in Python]: https://donkirkby.github.io/live-py-plugin/
 [Getting Started]: https://donkirkby.github.io/live-py-plugin/starting_space_tracer.html
 [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-
-
```

### Comparing `space_tracer-4.8.0/plugin/PySrc/space_tracer.egg-info/SOURCES.txt` & `space_tracer-4.9.0/plugin/PySrc/space_tracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/setup.py` & `space_tracer-4.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     packages=setuptools.find_packages('plugin/PySrc/'),
     package_dir={'': 'plugin/PySrc/'},
     entry_points=dict(console_scripts=[
         'space_tracer = space_tracer:main']),
     classifiers=[  # from https://pypi.org/classifiers/
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Debuggers",
-        "Programming Language :: Python :: 3.5",
+        # Synchronize Python versions with py-build.yml workflow and tox.ini.
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console"
     ],
     project_urls={
         'Bug Reports': 'https://github.com/donkirkby/live-py-plugin/issues',
```

### Comparing `space_tracer-4.8.0/space_tracer.md` & `space_tracer-4.9.0/space_tracer.md`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_canvas.py` & `space_tracer-4.9.0/test/PySrc/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_assignment.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_assignment.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_function.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_function.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_loops.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_loops.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_main.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_main.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_print.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_print.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_pytest.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_pytest.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_repr.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_repr.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_structural_match.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_structural_match.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_code_tracer_width.py` & `space_tracer-4.9.0/test/PySrc/tests/test_code_tracer_width.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_live_image.py` & `space_tracer-4.9.0/test/PySrc/tests/test_live_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -184,14 +184,37 @@
     p1 = image.get_pixel((5, 10))
     p2 = image.get_pixel((6, 10))
 
     assert p1 == blue
     assert p2 == default
 
 
+# noinspection DuplicatedCode
+@pytest.mark.skipif(Image is None, reason='Pillow not installed.')
+def test_live_png_as_painter(tmp_path):
+    blue = (0, 0, 255, 255)
+    white = (255, 255, 255, 255)
+
+    image1 = LivePillowImage(Image.new('RGBA', (10, 20)))
+    image1.set_pixel((5, 10), blue)
+    image1.set_pixel((6, 10), white)
+
+    image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
+    image2.set_pixel((5, 10), blue)
+    bytes2 = image2.convert_to_png()
+    image3 = LivePng(bytes2)
+    painter3 = image3.convert_to_painter()
+    painter3.set_pixel((6, 10), white)
+
+    differ = LiveImageDiffer(tmp_path)
+
+    differ.assert_equal(image1, painter3, 'live_png_as_painter')
+
+
+# noinspection DuplicatedCode
 @pytest.mark.skipif(Image is None, reason='Pillow not installed.')
 def test_differ_compare():
     blue = (0, 0, 255, 255)
     white = (255, 255, 255, 255)
     expected_match = (0, 0, 255, 255//3)
     expected_diff = (255, 255//5, 255*2//5, 255)
 
@@ -263,14 +286,32 @@
 
     report = t.report
 
     assert replace_image(report) == expected_report
 
 
 @pytest.mark.skipif(Image is None, reason='Pillow not installed.')
+def test_differ_compare_display_disabled(patched_turtle):
+    expected_report = '\n'
+
+    t = MockTurtle()
+
+    image1 = LivePillowImage(Image.new('RGBA', (10, 20)))
+    image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
+
+    differ = LiveImageDiffer(is_displayed=False)
+
+    differ.compare(image1, image2)
+
+    report = t.report
+
+    assert replace_image(report) == expected_report
+
+
+@pytest.mark.skipif(Image is None, reason='Pillow not installed.')
 def test_differ_compare_writes_file(tmp_path):
     image1 = LivePillowImage(Image.new('RGBA', (10, 20)))
     image1.set_pixel((5, 10), (0, 0, 255, 255))
     image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
 
     diffs_path = tmp_path / 'image_diffs'
     actual_path = diffs_path / 'test_name-actual.png'
@@ -362,14 +403,15 @@
     diff_pixel2 = diff.get_pixel((2, 0))
 
     assert diff_pixel1 == missing_blue
     assert diff_pixel2 == missing_green
     assert differ.diff_count == 5
 
 
+# noinspection DuplicatedCode
 @pytest.mark.skipif(Image is None, reason='Pillow not installed.')
 def test_differ_remove_common_prefix(tmp_path):
     image1 = LivePillowImage(Image.new('RGBA', (10, 20)))
     image1.set_pixel((5, 10), (0, 0, 101, 255))
     image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
 
     diffs_path = tmp_path / 'image_diffs'
@@ -381,14 +423,34 @@
     differ.compare(image1, image2, 'test_banana')
     differ.remove_common_prefix()
 
     assert actual_path1.exists()
     assert actual_path2.exists()
 
 
+# noinspection DuplicatedCode
+@pytest.mark.skipif(Image is None, reason='Pillow not installed.')
+def test_differ_remove_no_prefix(tmp_path):
+    image1 = LivePillowImage(Image.new('RGBA', (10, 20)))
+    image1.set_pixel((5, 10), (0, 0, 101, 255))
+    image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
+
+    diffs_path = tmp_path / 'image_diffs'
+    actual_path1 = diffs_path / 'apple-actual.png'
+    actual_path2 = diffs_path / 'banana-actual.png'
+    differ = LiveImageDiffer(diffs_path)
+
+    differ.compare(image1, image2, 'apple')
+    differ.compare(image1, image2, 'banana')
+    differ.remove_common_prefix()
+
+    assert actual_path1.exists()
+    assert actual_path2.exists()
+
+
 @pytest.mark.skipif(Image is None, reason='Pillow not installed.')
 def test_differ_cleans_diffs_path(tmp_path):
     diffs_path = tmp_path / 'image_diffs'
     diffs_path.mkdir()
     leftover_path = diffs_path / 'leftover-actual.png'
     leftover_path.write_text('garbage')
     unrelated_path = diffs_path / 'leftover-unrelated.png'
@@ -430,7 +492,12 @@
     image1.set_pixel((5, 10), blue)
     image2 = LivePillowImage(Image.new('RGBA', (10, 20)))
 
     differ = LiveImageDiffer()
 
     with pytest.raises(AssertionError, match=r'Images differ by 1 pixel.'):
         differ.assert_equal(image1, image2)
+
+    image1.set_pixel((5, 11), blue)
+
+    with pytest.raises(AssertionError, match=r'Images differ by 2 pixels.'):
+        differ.assert_equal(image1, image2)
```

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_mock_turtle.py` & `space_tracer-4.9.0/test/PySrc/tests/test_mock_turtle.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,15 +587,15 @@
     fill='black'
     pensize=1"""
 
     t = MockTurtle()
     t.fd(100)
     with pytest.raises(TurtleGraphicsError,
                        match=re.escape(expected_error)):
-        t.color(colour_in)
+        turtle.color(colour_in)
     report = t.report
 
     assert report == expected_report.splitlines()
 
 
 def test_pen_dict(patched_turtle):
     expected_report = """\
```

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_report_builder.py` & `space_tracer-4.9.0/test/PySrc/tests/test_report_builder.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_traced.py` & `space_tracer-4.9.0/test/PySrc/tests/test_traced.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/test_traced_finder.py` & `space_tracer-4.9.0/test/PySrc/tests/test_traced_finder.py`

 * *Files identical despite different names*

### Comparing `space_tracer-4.8.0/test/PySrc/tests/validate_legacy_python.py` & `space_tracer-4.9.0/test/PySrc/tests/validate_legacy_python.py`

 * *Files identical despite different names*

