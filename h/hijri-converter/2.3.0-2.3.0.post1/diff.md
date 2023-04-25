# Comparing `tmp/hijri-converter-2.3.0.tar.gz` & `tmp/hijri-converter-2.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijri-converter-2.3.0.tar", last modified: Mon Apr 24 18:45:27 2023, max compression
+gzip compressed data, was "hijri-converter-2.3.0.post1.tar", last modified: Mon Apr 24 19:47:58 2023, max compression
```

## Comparing `hijri-converter-2.3.0.tar` & `hijri-converter-2.3.0.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.870163 hijri-converter-2.3.0/
--rw-r--r--   0 mohd       (501) staff       (20)     6243 2023-04-24 18:21:26.000000 hijri-converter-2.3.0/CHANGELOG.md
--rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/LICENSE
--rw-r--r--   0 mohd       (501) staff       (20)       56 2023-04-24 04:34:05.000000 hijri-converter-2.3.0/MANIFEST.in
--rw-r--r--   0 mohd       (501) staff       (20)     3884 2023-04-24 18:45:27.870228 hijri-converter-2.3.0/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)     3822 2023-04-24 18:21:27.000000 hijri-converter-2.3.0/README.md
--rw-r--r--   0 mohd       (501) staff       (20)     1320 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/pyproject.toml
--rw-r--r--   0 mohd       (501) staff       (20)     1512 2023-04-24 18:45:27.870490 hijri-converter-2.3.0/setup.cfg
--rw-r--r--   0 mohd       (501) staff       (20)      858 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/setup.py
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.864941 hijri-converter-2.3.0/src/
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.867640 hijri-converter-2.3.0/src/hijri_converter/
--rw-r--r--   0 mohd       (501) staff       (20)      207 2023-04-24 18:21:27.000000 hijri-converter-2.3.0/src/hijri_converter/__init__.py
--rw-r--r--   0 mohd       (501) staff       (20)    10938 2023-04-20 18:10:31.000000 hijri-converter-2.3.0/src/hijri_converter/convert.py
--rw-r--r--   0 mohd       (501) staff       (20)      805 2023-04-20 18:10:34.000000 hijri-converter-2.3.0/src/hijri_converter/helpers.py
--rw-r--r--   0 mohd       (501) staff       (20)     5108 2023-04-20 18:10:37.000000 hijri-converter-2.3.0/src/hijri_converter/locales.py
--rw-r--r--   0 mohd       (501) staff       (20)       26 2022-05-23 16:57:16.000000 hijri-converter-2.3.0/src/hijri_converter/py.typed
--rw-r--r--   0 mohd       (501) staff       (20)    14615 2023-04-20 18:10:42.000000 hijri-converter-2.3.0/src/hijri_converter/ummalqura.py
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.868423 hijri-converter-2.3.0/src/hijri_converter.egg-info/
--rw-r--r--   0 mohd       (501) staff       (20)     3884 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)      773 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/SOURCES.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/dependency_links.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 04:35:10.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/not-zip-safe
--rw-r--r--   0 mohd       (501) staff       (20)       16 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/top_level.txt
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.865188 hijri-converter-2.3.0/tests/
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.868530 hijri-converter-2.3.0/tests/integration/
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.869558 hijri-converter-2.3.0/tests/integration/fixtures/
--rw-r--r--   0 mohd       (501) staff       (20)    20308 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/kfupm_comparison_calendar.json
--rw-r--r--   0 mohd       (501) staff       (20)    25374 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_calendar_website.json
--rw-r--r--   0 mohd       (501) staff       (20)    13869 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_newspaper_issues.json
--rwxr-xr-x   0 mohd       (501) staff       (20)     1280 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/test_month_starts.py
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.870039 hijri-converter-2.3.0/tests/unit/
--rwxr-xr-x   0 mohd       (501) staff       (20)     6753 2022-02-09 22:52:24.000000 hijri-converter-2.3.0/tests/unit/test_convert.py
--rwxr-xr-x   0 mohd       (501) staff       (20)      380 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/unit/test_helpers.py
--rwxr-xr-x   0 mohd       (501) staff       (20)     1787 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/unit/test_locales.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.612537 hijri-converter-2.3.0.post1/
+-rw-r--r--   0 mohd       (501) staff       (20)     6243 2023-04-24 18:21:26.000000 hijri-converter-2.3.0.post1/CHANGELOG.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-24 04:43:29.000000 hijri-converter-2.3.0.post1/LICENSE
+-rw-r--r--   0 mohd       (501) staff       (20)       56 2023-04-24 04:34:05.000000 hijri-converter-2.3.0.post1/MANIFEST.in
+-rw-r--r--   0 mohd       (501) staff       (20)     2753 2023-04-24 19:47:58.612613 hijri-converter-2.3.0.post1/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)     3822 2023-04-24 18:21:27.000000 hijri-converter-2.3.0.post1/README.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1320 2023-04-24 04:43:29.000000 hijri-converter-2.3.0.post1/pyproject.toml
+-rw-r--r--   0 mohd       (501) staff       (20)      612 2023-04-24 19:47:58.612887 hijri-converter-2.3.0.post1/setup.cfg
+-rw-r--r--   0 mohd       (501) staff       (20)      858 2023-04-24 04:43:29.000000 hijri-converter-2.3.0.post1/setup.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.605599 hijri-converter-2.3.0.post1/src/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.608285 hijri-converter-2.3.0.post1/src/hijri_converter/
+-rw-r--r--   0 mohd       (501) staff       (20)      213 2023-04-24 19:47:39.000000 hijri-converter-2.3.0.post1/src/hijri_converter/__init__.py
+-rw-r--r--   0 mohd       (501) staff       (20)    10938 2023-04-20 18:10:31.000000 hijri-converter-2.3.0.post1/src/hijri_converter/convert.py
+-rw-r--r--   0 mohd       (501) staff       (20)      805 2023-04-20 18:10:34.000000 hijri-converter-2.3.0.post1/src/hijri_converter/helpers.py
+-rw-r--r--   0 mohd       (501) staff       (20)     5108 2023-04-20 18:10:37.000000 hijri-converter-2.3.0.post1/src/hijri_converter/locales.py
+-rw-r--r--   0 mohd       (501) staff       (20)       26 2022-05-23 16:57:16.000000 hijri-converter-2.3.0.post1/src/hijri_converter/py.typed
+-rw-r--r--   0 mohd       (501) staff       (20)    14615 2023-04-20 18:10:42.000000 hijri-converter-2.3.0.post1/src/hijri_converter/ummalqura.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.610470 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/
+-rw-r--r--   0 mohd       (501) staff       (20)     2753 2023-04-24 19:47:58.000000 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      773 2023-04-24 19:47:58.000000 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 19:47:58.000000 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 04:35:10.000000 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/not-zip-safe
+-rw-r--r--   0 mohd       (501) staff       (20)       16 2023-04-24 19:47:58.000000 hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/top_level.txt
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.605838 hijri-converter-2.3.0.post1/tests/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.610645 hijri-converter-2.3.0.post1/tests/integration/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.611752 hijri-converter-2.3.0.post1/tests/integration/fixtures/
+-rw-r--r--   0 mohd       (501) staff       (20)    20308 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/integration/fixtures/kfupm_comparison_calendar.json
+-rw-r--r--   0 mohd       (501) staff       (20)    25374 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/integration/fixtures/ummalqura_calendar_website.json
+-rw-r--r--   0 mohd       (501) staff       (20)    13869 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/integration/fixtures/ummalqura_newspaper_issues.json
+-rwxr-xr-x   0 mohd       (501) staff       (20)     1280 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/integration/test_month_starts.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 19:47:58.612300 hijri-converter-2.3.0.post1/tests/unit/
+-rwxr-xr-x   0 mohd       (501) staff       (20)     6753 2022-02-09 22:52:24.000000 hijri-converter-2.3.0.post1/tests/unit/test_convert.py
+-rwxr-xr-x   0 mohd       (501) staff       (20)      380 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/unit/test_helpers.py
+-rwxr-xr-x   0 mohd       (501) staff       (20)     1787 2022-02-09 22:30:41.000000 hijri-converter-2.3.0.post1/tests/unit/test_locales.py
```

### Comparing `hijri-converter-2.3.0/CHANGELOG.md` & `hijri-converter-2.3.0.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/LICENSE` & `hijri-converter-2.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/README.md` & `hijri-converter-2.3.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/pyproject.toml` & `hijri-converter-2.3.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/setup.py` & `hijri-converter-2.3.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/src/hijri_converter/convert.py` & `hijri-converter-2.3.0.post1/src/hijri_converter/convert.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/src/hijri_converter/helpers.py` & `hijri-converter-2.3.0.post1/src/hijri_converter/helpers.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/src/hijri_converter/locales.py` & `hijri-converter-2.3.0.post1/src/hijri_converter/locales.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/src/hijri_converter/ummalqura.py` & `hijri-converter-2.3.0.post1/src/hijri_converter/ummalqura.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/src/hijri_converter.egg-info/SOURCES.txt` & `hijri-converter-2.3.0.post1/src/hijri_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/integration/fixtures/kfupm_comparison_calendar.json` & `hijri-converter-2.3.0.post1/tests/integration/fixtures/kfupm_comparison_calendar.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_calendar_website.json` & `hijri-converter-2.3.0.post1/tests/integration/fixtures/ummalqura_calendar_website.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_newspaper_issues.json` & `hijri-converter-2.3.0.post1/tests/integration/fixtures/ummalqura_newspaper_issues.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/integration/test_month_starts.py` & `hijri-converter-2.3.0.post1/tests/integration/test_month_starts.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/unit/test_convert.py` & `hijri-converter-2.3.0.post1/tests/unit/test_convert.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.3.0/tests/unit/test_locales.py` & `hijri-converter-2.3.0.post1/tests/unit/test_locales.py`

 * *Files identical despite different names*

