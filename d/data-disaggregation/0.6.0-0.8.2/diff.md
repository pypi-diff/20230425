# Comparing `tmp/data-disaggregation-0.6.0.tar.gz` & `tmp/data-disaggregation-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-disaggregation-0.6.0.tar", last modified: Wed Sep  7 07:32:15 2022, max compression
+gzip compressed data, was "data-disaggregation-0.8.2.tar", last modified: Tue Apr 25 06:18:03 2023, max compression
```

## Comparing `data-disaggregation-0.6.0.tar` & `data-disaggregation-0.8.2.tar`

### file list

```diff
@@ -1,36 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:15.002468 data-disaggregation-0.6.0/
--rw-rw-rw-   0        0        0      156 2022-09-07 07:13:21.000000 data-disaggregation-0.6.0/.bumpversion.cfg
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.861834 data-disaggregation-0.6.0/.github/
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.931538 data-disaggregation-0.6.0/.github/workflows/
--rw-rw-rw-   0        0        0      556 2022-09-07 07:22:49.000000 data-disaggregation-0.6.0/.github/workflows/unittest.yml
--rw-rw-rw-   0        0        0     1948 2022-02-18 13:48:04.000000 data-disaggregation-0.6.0/.gitignore
--rw-rw-rw-   0        0        0      752 2022-09-07 07:13:21.000000 data-disaggregation-0.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      554 2022-09-07 07:27:43.000000 data-disaggregation-0.6.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1028 2022-02-21 16:58:47.000000 data-disaggregation-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      458 2022-09-07 07:32:15.001466 data-disaggregation-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2022-09-07 07:29:10.000000 data-disaggregation-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.943927 data-disaggregation-0.6.0/data_disaggregation/
--rw-rw-rw-   0        0        0       82 2022-09-07 07:14:44.000000 data-disaggregation-0.6.0/data_disaggregation/__init__.py
--rw-rw-rw-   0        0        0     7639 2022-09-07 07:14:44.000000 data-disaggregation-0.6.0/data_disaggregation/test.py
--rw-rw-rw-   0        0        0     8539 2022-09-07 07:14:44.000000 data-disaggregation-0.6.0/data_disaggregation/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.962922 data-disaggregation-0.6.0/data_disaggregation.egg-info/
--rw-rw-rw-   0        0        0      458 2022-09-07 07:32:14.000000 data-disaggregation-0.6.0/data_disaggregation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2022-09-07 07:32:14.000000 data-disaggregation-0.6.0/data_disaggregation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-07 07:32:14.000000 data-disaggregation-0.6.0/data_disaggregation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-09-07 07:32:14.000000 data-disaggregation-0.6.0/data_disaggregation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-09-07 07:32:14.000000 data-disaggregation-0.6.0/data_disaggregation.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.986376 data-disaggregation-0.6.0/docs/
-drwxrwxrwx   0        0        0        0 2022-09-07 07:32:14.992465 data-disaggregation-0.6.0/docs/_static/
--rw-rw-rw-   0        0        0     9421 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/_static/favicon.ico
--rw-rw-rw-   0        0        0     6230 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/_static/logo.svg
--rw-rw-rw-   0        0        0        0 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/_static/main.css
--rw-rw-rw-   0        0        0        0 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/_static/main.js
--rw-rw-rw-   0        0        0      106 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/api.rst
--rw-rw-rw-   0        0        0     5672 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/concept.rst
--rw-rw-rw-   0        0        0     1488 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/conf.py
--rw-rw-rw-   0        0        0     2312 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/example.ipynb
--rw-rw-rw-   0        0        0      114 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/index.rst
--rw-rw-rw-   0        0        0       31 2022-09-07 07:15:03.000000 data-disaggregation-0.6.0/docs/readme.md
--rw-rw-rw-   0        0        0      152 2022-09-07 07:14:38.000000 data-disaggregation-0.6.0/docs/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-09-07 07:32:15.002468 data-disaggregation-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2022-09-07 07:23:43.000000 data-disaggregation-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/data_disaggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/data_disaggregation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/test/test.py
```

### Comparing `data-disaggregation-0.6.0/LICENSE` & `data-disaggregation-0.8.2/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `data-disaggregation-0.6.0/setup.py` & `data-disaggregation-0.8.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from setuptools import find_packages, setup
-
-if __name__ == "__main__":
-
-    setup(
-        packages=find_packages(),
-        name="data-disaggregation",
-        install_requires=["pandas"],
-        keywords=[],
-        description="",
-        long_description="",
-        long_description_content_type="text/markdown",
-        version="0.6.0",
-        author="Christian Winger",
-        platforms=["any"],
-        license="MIT",
-        project_urls={
-            "Documentation": "https://data-disaggregation.readthedocs.io",
-        },
-        classifiers=[
-            "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.10",
-            "License :: OSI Approved :: MIT License",
-            "Operating System :: OS Independent",
-        ],
-    )
+from setuptools import setup
+
+if __name__ == "__main__":
+    setup(
+        packages=["data_disaggregation"],
+        name="data-disaggregation",
+        install_requires=["pandas"],
+        keywords=[],
+        description="",
+        long_description="",
+        long_description_content_type="text/markdown",
+        version="0.8.2",
+        author="Christian Winger",
+        platforms=["any"],
+        license="MIT",
+        project_urls={
+            "Documentation": "https://data-disaggregation.readthedocs.io",
+        },
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+        ],
+    )
```

