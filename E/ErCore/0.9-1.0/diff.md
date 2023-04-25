# Comparing `tmp/ErCore-0.9.tar.gz` & `tmp/ErCore-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ErCore-0.9.tar", last modified: Fri Mar 31 06:06:06 2023, max compression
+gzip compressed data, was "ErCore-1.0.tar", last modified: Tue Apr 25 04:31:02 2023, max compression
```

## Comparing `ErCore-0.9.tar` & `ErCore-1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:06:06.415517 ErCore-0.9/
-drwxrwxrwx   0        0        0        0 2023-03-31 06:06:06.400527 ErCore-0.9/ErCore/
--rw-rw-rw-   0        0        0     1280 2023-03-31 06:05:55.000000 ErCore-0.9/ErCore/Core.py
--rw-rw-rw-   0        0        0       33 2023-03-30 02:42:05.000000 ErCore-0.9/ErCore/__init__.py
--rw-rw-rw-   0        0        0     3230 2023-03-30 02:36:09.000000 ErCore-0.9/ErCore/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:06:06.412527 ErCore-0.9/ErCore/std/
--rw-rw-rw-   0        0        0        0 2023-03-21 03:55:03.000000 ErCore-0.9/ErCore/std/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:06:06.412527 ErCore-0.9/ErCore.egg-info/
--rw-rw-rw-   0        0        0      492 2023-03-31 06:06:05.000000 ErCore-0.9/ErCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-03-31 06:06:06.000000 ErCore-0.9/ErCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:06:05.000000 ErCore-0.9/ErCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-03-31 06:06:05.000000 ErCore-0.9/ErCore.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-03-31 06:06:05.000000 ErCore-0.9/ErCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-03-21 04:53:11.000000 ErCore-0.9/LICENSE
--rw-rw-rw-   0        0        0      492 2023-03-31 06:06:06.414518 ErCore-0.9/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-03-31 05:09:41.000000 ErCore-0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 06:06:06.415517 ErCore-0.9/setup.cfg
--rw-rw-rw-   0        0        0      770 2023-03-31 06:06:03.000000 ErCore-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.593178 ErCore-1.0/
+drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.568179 ErCore-1.0/ErCore/
+-rw-rw-rw-   0        0        0     2101 2023-04-25 04:23:54.000000 ErCore-1.0/ErCore/Core.py
+-rw-rw-rw-   0        0        0       33 2023-03-30 02:42:05.000000 ErCore-1.0/ErCore/__init__.py
+-rw-rw-rw-   0        0        0     3188 2023-04-25 04:23:54.000000 ErCore-1.0/ErCore/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.590179 ErCore-1.0/ErCore/std/
+-rw-rw-rw-   0        0        0      375 2023-04-25 04:21:27.000000 ErCore-1.0/ErCore/std/Base.py
+-rw-rw-rw-   0        0        0       33 2023-04-25 04:21:27.000000 ErCore-1.0/ErCore/std/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.588191 ErCore-1.0/ErCore.egg-info/
+-rw-rw-rw-   0        0        0      475 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.0/LICENSE
+-rw-rw-rw-   0        0        0      475 2023-04-25 04:31:02.592178 ErCore-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-04-25 04:23:54.000000 ErCore-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 04:31:02.593178 ErCore-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-04-21 12:03:04.000000 ErCore-1.0/setup.py
```

### Comparing `ErCore-0.9/ErCore/cli.py` & `ErCore-1.0/ErCore/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-import sys
 import datetime
 import platform
 
+from std import colors
+
 
 def make_project():
     try:
         name = str(input('Enter project name: '))
         readme = str(input('Add readme file?[Y/N]: '))
         python = str(input('Add python file?[Y/N]: '))
         license = str(input('Add license file?[Y/N]: '))
@@ -38,25 +39,22 @@
                 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
                 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
                 FROM,OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
                 with open('LICENSE', 'w') as lt:
                     lt.write(mit_l)
             else:
-                print('Error! WORK ONLY MIT LICENSE (try again)')
+                print(f'{colors["Red"]}Error! WORK ONLY MIT LICENSE (try again){colors["Reset"]}')
         else:
             print('')
     except ValueError as error:
         print('!!!' * 20)
         print(error)
         print('!!!' * 20)
         print('Helper: pls restart command and enter string')
-    finally:
-        print('1000-7 = ')  # this is a prank
-        sys.exit(1000 - 7)
 
 
 def make_runner():
     IS_WINDOWS = (platform.system() == 'Windows')
     IS_LINUX = (platform.system() == 'Linux')
     IS_MAC = (platform.system() == 'Darwin')
     file = input('file name: ')
```

### Comparing `ErCore-0.9/LICENSE` & `ErCore-1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 MIT License
 
 Copyright © 2023 Eragod
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software
+and associated documentation files (the “Software”), to deal in the Software without
+restriction, including without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or
+substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING
+BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ErCore-0.9/setup.py` & `ErCore-1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r') as readme_file:
-    long_description = readme_file.read()
-
-
 setup(
     name='ErCore',
-    version='0.9',
+    version='1.0',
     packages=find_packages(),
     author='Eragod',
-    description='This is a core for my package',
+    description='Core for projects',
     url="https://github.com/Eragod/ErCore",
-    long_description=long_description,
+    long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': ['ErCore-project = ErCore.cli:make_project',
                                       'ErCore-runner = ErCore.cli:make_runner']},
     classifiers=['Programming Language :: Python :: 3',
                  'License :: OSI Approved :: MIT License',
                  'Operating System :: OS Independent'],
 )
```

