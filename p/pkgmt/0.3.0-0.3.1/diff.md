# Comparing `tmp/pkgmt-0.3.0.tar.gz` & `tmp/pkgmt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.3.0.tar", last modified: Fri Mar 31 18:03:12 2023, max compression
+gzip compressed data, was "pkgmt-0.3.1.tar", last modified: Tue Apr 25 01:36:57 2023, max compression
```

## Comparing `pkgmt-0.3.0.tar` & `pkgmt-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-31 18:02:51.000000 pkgmt-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-31 18:02:51.000000 pkgmt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-31 18:02:51.000000 pkgmt-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-31 18:03:12.457030 pkgmt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-31 18:02:51.000000 pkgmt-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-31 18:02:51.000000 pkgmt-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 18:03:12.457030 pkgmt-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-31 18:02:51.000000 pkgmt-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.449030 pkgmt-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.453030 pkgmt-0.3.0/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.453030 pkgmt-0.3.0/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.449030 pkgmt-0.3.0/src/pkgmt/assets/template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.449030 pkgmt-0.3.0/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/src/pkgmt/assets/template/src/name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/src/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.457030 pkgmt-0.3.0/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-31 18:02:51.000000 pkgmt-0.3.0/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:03:12.453030 pkgmt-0.3.0/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 18:03:12.000000 pkgmt-0.3.0/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-25 01:36:42.000000 pkgmt-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 01:36:42.000000 pkgmt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 01:36:42.000000 pkgmt-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 01:36:57.986418 pkgmt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 01:36:42.000000 pkgmt-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 01:36:42.000000 pkgmt-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 01:36:57.986418 pkgmt-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-25 01:36:42.000000 pkgmt-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/pkgmt/assets/template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/src/pkgmt/assets/template/src/name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/src/name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.986418 pkgmt-0.3.1/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioner/abstractversioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioner/versionernonsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-25 01:36:42.000000 pkgmt-0.3.1/src/pkgmt/versioner/versionersetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:57.982418 pkgmt-0.3.1/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 01:36:57.000000 pkgmt-0.3.1/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.3.0/CHANGELOG.md` & `pkgmt-0.3.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.3.1 (2023-04-24)
+
+* [Fix] `pkgmt check-links` no longer reports `403` codes from `twitter.com` as errors
+
 ## 0.3.0 (2023-03-31)
 
 * [Feature] Running `black --check .` when running `pkgmt lint`
 * [Feature] Expanding GitHub handles when processing `CHANGELOG.md` files
 * [Fix] Updates inaccurate confirmation message when running `pkgmt format`
 
 ## 0.2.11 (2023-03-30)
```

### Comparing `pkgmt-0.3.0/LICENSE` & `pkgmt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/README.md` & `pkgmt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/setup.py` & `pkgmt-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.3.1/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.3.1/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/assets/template/setup.py` & `pkgmt-0.3.1/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.3.1/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/changelog.py` & `pkgmt-0.3.1/src/pkgmt/changelog.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/cli.py` & `pkgmt-0.3.1/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/config.py` & `pkgmt-0.3.1/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/dependencies.py` & `pkgmt-0.3.1/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/deprecation.py` & `pkgmt-0.3.1/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/dev.py` & `pkgmt-0.3.1/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/formatting.py` & `pkgmt-0.3.1/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/github.py` & `pkgmt-0.3.1/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/hook.py` & `pkgmt-0.3.1/src/pkgmt/hook.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/links.py` & `pkgmt-0.3.1/src/pkgmt/links.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,14 +201,27 @@
             invalid.append(candidate)
         else:
             valid.append(candidate)
 
     return valid, invalid
 
 
+# domains that we know return 403 (forbidden) if they're accessed from requests
+# instead of a browser
+KNOWN_403_DOMAINS = {"https://twitter.com"}
+
+
+def known_403(url):
+    for domain in KNOWN_403_DOMAINS:
+        if domain in url:
+            return True
+
+    return False
+
+
 class LinkChecker:
     def __init__(self) -> None:
         self.last_timestamp = defaultdict(lambda: datetime.min)
 
     def check_if_broken(self, url, broken_http_codes=None):
         """Check if a link is broken"""
         netloc = urlparse(url).netloc
@@ -233,14 +246,16 @@
 
         if broken_http_codes:
             broken = code in broken_http_codes
         else:
             # https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/405
             if code == 405:
                 broken = False
+            elif code == 403 and known_403(url):
+                broken = False
 
         response = Response(url, code, broken)
 
         return response
 
 
 # copied from soopervisor
```

### Comparing `pkgmt-0.3.0/src/pkgmt/new.py` & `pkgmt-0.3.1/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/test.py` & `pkgmt-0.3.1/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/versioneer.py` & `pkgmt-0.3.1/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.3.1/src/pkgmt/versioner/abstractversioner.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/versioner/util.py` & `pkgmt-0.3.1/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/versioner/versionernonsetup.py` & `pkgmt-0.3.1/src/pkgmt/versioner/versionernonsetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt/versioner/versionersetup.py` & `pkgmt-0.3.1/src/pkgmt/versioner/versionersetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.3.0/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.3.1/src/pkgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

