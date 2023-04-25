# Comparing `tmp/app01-0.1.5.tar.gz` & `tmp/app01-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app01-0.1.5.tar", last modified: Mon Apr 24 01:39:02 2023, max compression
+gzip compressed data, was "app01-0.1.6.tar", last modified: Tue Apr 25 02:36:40 2023, max compression
```

## Comparing `app01-0.1.5.tar` & `app01-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.419999 app01-0.1.5/
--rw-r--r--   0 lihaijian   (501) staff       (20)      150 2023-04-23 06:59:22.000000 app01-0.1.5/AUTHORS.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     3500 2023-04-23 06:59:22.000000 app01-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       89 2023-04-23 06:59:22.000000 app01-0.1.5/HISTORY.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     1068 2023-04-23 06:59:22.000000 app01-0.1.5/LICENSE
--rw-r--r--   0 lihaijian   (501) staff       (20)      262 2023-04-23 06:59:22.000000 app01-0.1.5/MANIFEST.in
--rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-24 01:39:02.420289 app01-0.1.5/PKG-INFO
--rw-r--r--   0 lihaijian   (501) staff       (20)      812 2023-04-23 06:59:22.000000 app01-0.1.5/README.rst
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.406324 app01-0.1.5/app01/
--rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 12:21:07.000000 app01-0.1.5/app01/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)       19 2023-04-23 06:59:22.000000 app01-0.1.5/app01/app01.py
--rw-r--r--   0 lihaijian   (501) staff       (20)      582 2023-04-23 12:23:26.000000 app01-0.1.5/app01/cli.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.412025 app01-0.1.5/app01/matt/
--rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 09:15:37.000000 app01-0.1.5/app01/matt/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)       96 2023-04-23 12:18:06.000000 app01-0.1.5/app01/matt/math_add.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.410813 app01-0.1.5/app01.egg-info/
--rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/PKG-INFO
--rw-r--r--   0 lihaijian   (501) staff       (20)      589 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/SOURCES.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/dependency_links.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)       41 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/entry_points.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/not-zip-safe
--rw-r--r--   0 lihaijian   (501) staff       (20)        4 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/requires.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)        6 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/top_level.txt
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.418352 app01-0.1.5/docs/
--rw-r--r--   0 lihaijian   (501) staff       (20)      606 2023-04-23 06:59:22.000000 app01-0.1.5/docs/Makefile
--rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.5/docs/authors.rst
--rwxr-xr-x   0 lihaijian   (501) staff       (20)     4743 2023-04-23 06:59:22.000000 app01-0.1.5/docs/conf.py
--rw-r--r--   0 lihaijian   (501) staff       (20)       33 2023-04-23 06:59:22.000000 app01-0.1.5/docs/contributing.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.5/docs/history.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      302 2023-04-23 06:59:22.000000 app01-0.1.5/docs/index.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     1098 2023-04-23 06:59:22.000000 app01-0.1.5/docs/installation.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      803 2023-04-23 06:59:22.000000 app01-0.1.5/docs/make.bat
--rw-r--r--   0 lihaijian   (501) staff       (20)       27 2023-04-23 06:59:22.000000 app01-0.1.5/docs/readme.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       65 2023-04-23 06:59:22.000000 app01-0.1.5/docs/usage.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-24 01:39:02.421746 app01-0.1.5/setup.cfg
--rw-r--r--   0 lihaijian   (501) staff       (20)     1336 2023-04-24 01:38:37.000000 app01-0.1.5/setup.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.419520 app01-0.1.5/tests/
--rw-r--r--   0 lihaijian   (501) staff       (20)       35 2023-04-23 06:59:22.000000 app01-0.1.5/tests/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-23 06:59:22.000000 app01-0.1.5/tests/test_app01.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.390087 app01-0.1.6/
+-rw-r--r--   0 lihaijian   (501) staff       (20)      150 2023-04-23 06:59:22.000000 app01-0.1.6/AUTHORS.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     3500 2023-04-23 06:59:22.000000 app01-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       89 2023-04-23 06:59:22.000000 app01-0.1.6/HISTORY.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1068 2023-04-23 06:59:22.000000 app01-0.1.6/LICENSE
+-rw-r--r--   0 lihaijian   (501) staff       (20)      262 2023-04-23 06:59:22.000000 app01-0.1.6/MANIFEST.in
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1600 2023-04-25 02:36:40.390272 app01-0.1.6/PKG-INFO
+-rw-r--r--   0 lihaijian   (501) staff       (20)      812 2023-04-23 06:59:22.000000 app01-0.1.6/README.rst
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.372929 app01-0.1.6/app01/
+-rw-r--r--   0 lihaijian   (501) staff       (20)      117 2023-04-24 01:54:42.000000 app01-0.1.6/app01/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      713 2023-04-25 01:52:48.000000 app01-0.1.6/app01/cli.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.379360 app01-0.1.6/app01/config/
+-rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-24 09:55:06.000000 app01-0.1.6/app01/config/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      221 2023-04-24 10:05:54.000000 app01-0.1.6/app01/config/oss_config.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      692 2023-04-25 01:52:10.000000 app01-0.1.6/app01/config/oss_helper.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.380383 app01-0.1.6/app01/matt/
+-rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 09:15:37.000000 app01-0.1.6/app01/matt/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)       96 2023-04-23 12:18:06.000000 app01-0.1.6/app01/matt/math_add.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.377293 app01-0.1.6/app01.egg-info/
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1600 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/PKG-INFO
+-rw-r--r--   0 lihaijian   (501) staff       (20)      653 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/SOURCES.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/dependency_links.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)       41 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/entry_points.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/not-zip-safe
+-rw-r--r--   0 lihaijian   (501) staff       (20)      210 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/requires.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        6 2023-04-25 02:36:40.000000 app01-0.1.6/app01.egg-info/top_level.txt
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.387194 app01-0.1.6/docs/
+-rw-r--r--   0 lihaijian   (501) staff       (20)      606 2023-04-23 06:59:22.000000 app01-0.1.6/docs/Makefile
+-rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.6/docs/authors.rst
+-rwxr-xr-x   0 lihaijian   (501) staff       (20)     4743 2023-04-23 06:59:22.000000 app01-0.1.6/docs/conf.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)       33 2023-04-23 06:59:22.000000 app01-0.1.6/docs/contributing.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.6/docs/history.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      302 2023-04-23 06:59:22.000000 app01-0.1.6/docs/index.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1098 2023-04-23 06:59:22.000000 app01-0.1.6/docs/installation.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      803 2023-04-23 06:59:22.000000 app01-0.1.6/docs/make.bat
+-rw-r--r--   0 lihaijian   (501) staff       (20)       27 2023-04-23 06:59:22.000000 app01-0.1.6/docs/readme.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       65 2023-04-23 06:59:22.000000 app01-0.1.6/docs/usage.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-25 02:36:40.391062 app01-0.1.6/setup.cfg
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1655 2023-04-25 02:35:42.000000 app01-0.1.6/setup.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-25 02:36:40.389104 app01-0.1.6/tests/
+-rw-r--r--   0 lihaijian   (501) staff       (20)       35 2023-04-23 06:59:22.000000 app01-0.1.6/tests/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-23 06:59:22.000000 app01-0.1.6/tests/test_app01.py
```

### Comparing `app01-0.1.5/CONTRIBUTING.rst` & `app01-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/LICENSE` & `app01-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/PKG-INFO` & `app01-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app01
-Version: 0.1.5
+Version: 0.1.6
 Summary: my first app01
 Home-page: https://github.com/near2sea/app01
 Author: lihaijian
 Author-email: sanan.li@qq.com
 License: MIT license
 Keywords: app01
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =====
 app01
 =====
```

### Comparing `app01-0.1.5/README.rst` & `app01-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/app01.egg-info/PKG-INFO` & `app01-0.1.6/app01.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app01
-Version: 0.1.5
+Version: 0.1.6
 Summary: my first app01
 Home-page: https://github.com/near2sea/app01
 Author: lihaijian
 Author-email: sanan.li@qq.com
 License: MIT license
 Keywords: app01
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =====
 app01
 =====
```

### Comparing `app01-0.1.5/app01.egg-info/SOURCES.txt` & `app01-0.1.6/app01.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 app01/__init__.py
-app01/app01.py
 app01/cli.py
 app01.egg-info/PKG-INFO
 app01.egg-info/SOURCES.txt
 app01.egg-info/dependency_links.txt
 app01.egg-info/entry_points.txt
 app01.egg-info/not-zip-safe
 app01.egg-info/requires.txt
 app01.egg-info/top_level.txt
+app01/config/__init__.py
+app01/config/oss_config.py
+app01/config/oss_helper.py
 app01/matt/__init__.py
 app01/matt/math_add.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

### Comparing `app01-0.1.5/docs/Makefile` & `app01-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/docs/conf.py` & `app01-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/docs/installation.rst` & `app01-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/docs/make.bat` & `app01-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `app01-0.1.5/setup.py` & `app01-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,42 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['pip']
+tests_require = [
+    'pytest',
+    'responses',
+    'pytest-mock',
+    'werkzeug<2.1.0'
+]
+dev_require = [
+    *tests_require,
+    'flake8',
+    'flake8-comprehensions',
+    'flake8-deprecated',
+    'flake8-mutable',
+    'flake8-tuple',
+    'twine',
+    'wheel',
+    'oss2'
+]
 
-test_requirements = [
-    'pyyaml',
-    'twine']
+install_requires = [
+    'pip',
+    'setuptools'
+]
+
+# bdist_wheel
+extras_require = {
+    'dev': dev_require,
+    'test': tests_require
+}
 
 setup(
     author="lihaijian",
     author_email='sanan.li@qq.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -32,20 +55,19 @@
     ],
     description="my first app01",
     entry_points={
         'console_scripts': [
             'app01=app01.cli:main',
         ],
     },
-    install_requires=requirements,
+    extras_require=extras_require,
+    install_requires=install_requires,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='app01',
     name='app01',
     packages=find_packages(include=['app01', 'app01.*']),
-    test_suite='tests',
-    tests_require=test_requirements,
     url='https://github.com/near2sea/app01',
-    version='0.1.5',
+    version='0.1.6',
     zip_safe=False,
 )
```

