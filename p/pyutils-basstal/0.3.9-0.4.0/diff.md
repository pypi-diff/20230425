# Comparing `tmp/pyutils_basstal-0.3.9.tar.gz` & `tmp/pyutils_basstal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutils_basstal-0.3.9.tar", last modified: Thu Feb 16 04:46:26 2023, max compression
+gzip compressed data, was "pyutils_basstal-0.4.0.tar", last modified: Tue Apr 25 07:58:55 2023, max compression
```

## Comparing `pyutils_basstal-0.3.9.tar` & `pyutils_basstal-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 04:46:26.210682 pyutils_basstal-0.3.9/
--rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0     1473 2023-02-16 04:46:26.210682 pyutils_basstal-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 04:46:26.178788 pyutils_basstal-0.3.9/pyutils/
--rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.3.9/pyutils/__init__.py
--rw-rw-rw-   0        0        0     5598 2023-02-16 04:43:53.000000 pyutils_basstal-0.3.9/pyutils/autoupgrade.py
--rw-rw-rw-   0        0        0    24013 2023-02-16 04:42:13.000000 pyutils_basstal-0.3.9/pyutils/executor.py
--rw-rw-rw-   0        0        0    14734 2022-12-20 09:13:11.000000 pyutils_basstal-0.3.9/pyutils/fsext.py
--rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.3.9/pyutils/shorthand.py
--rw-rw-rw-   0        0        0     3712 2023-01-04 06:19:55.000000 pyutils_basstal-0.3.9/pyutils/simplelogger.py
--rw-rw-rw-   0        0        0     5375 2022-07-14 05:36:33.000000 pyutils_basstal-0.3.9/pyutils/templite.py
-drwxrwxrwx   0        0        0        0 2023-02-16 04:46:26.209684 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/
--rw-rw-rw-   0        0        0     1473 2023-02-16 04:46:26.000000 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-02-16 04:46:26.000000 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 04:46:26.000000 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-02-16 04:46:26.000000 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-16 04:46:26.000000 pyutils_basstal-0.3.9/pyutils_basstal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2023-02-16 04:46:26.211678 pyutils_basstal-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     8835 2023-02-16 04:45:48.000000 pyutils_basstal-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.824128 pyutils_basstal-0.4.0/
+-rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1473 2023-04-25 07:58:55.823107 pyutils_basstal-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.800166 pyutils_basstal-0.4.0/pyutils/
+-rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.0/pyutils/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.0/pyutils/autoupgrade.py
+-rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.0/pyutils/executor.py
+-rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.0/pyutils/fsext.py
+-rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.0/pyutils/shorthand.py
+-rw-rw-rw-   0        0        0     5071 2023-04-25 05:43:17.000000 pyutils_basstal-0.4.0/pyutils/simplelogger.py
+-rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.0/pyutils/templite.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.822109 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:58:55.824128 pyutils_basstal-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     8820 2023-04-25 06:09:37.000000 pyutils_basstal-0.4.0/setup.py
```

### Comparing `pyutils_basstal-0.3.9/LICENSE.txt` & `pyutils_basstal-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.3.9/PKG-INFO` & `pyutils_basstal-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils_basstal
-Version: 0.3.9
+Version: 0.4.0
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.3.9/README.md` & `pyutils_basstal-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.3.9/pyutils/autoupgrade.py` & `pyutils_basstal-0.4.0/pyutils/autoupgrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: E501
+
 import sys
 from urllib.request import urlopen, Request
 import ssl
 import re
 from os import execl, environ
 from sys import executable
 import semantic_version
@@ -120,26 +122,47 @@
         return current
 
     def _get_highest_version(self):
         # NOTE:Match for newest pypi server
         url = "{}/{}".format(self.index, self.pkg_formatted)
         return self.parse_from_html_page(url)
 
+    def search_tar_version(self, text):
+        search_result = re.search(rf'{self.pkg}-(.*)(\.tar\.gz)', text)
+        if search_result is not None:
+            version = search_result.group(1)
+            return semantic_version.Version(version)
+        return None
+
+    def search_wheel_version(self, text):
+        # wheel_name 示例: some_package-0.1.2-cp37-cp37m-manylinux1_x86_64.whl
+
+        # 正则表达式匹配 wheel 包的名称和版本
+        pattern = rf'({self.pkg})-(?P<version>[0-9]+\.[0-9]+\.[0-9]+)(-[\w\.]+)?(-.*\.whl)'
+        match = re.match(pattern, text)
+
+        if match:
+            package_version = match.group('version')
+            return semantic_version.Version(package_version)
+        return None
+
     def parse_from_html_page(self, url):
         # bypass CA problem on MacOS
         # https://stackoverflow.com/questions/2792650/import-error-no-module-name-urllib2
         req = Request(url, headers={'X-Mashape-Key': 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'})
         gcontext = ssl.SSLContext()  # Only for gangstars
         html = urlopen(req, context=gcontext)
         if html.getcode() != 200:
             raise PkgNotFoundError
         soup = BeautifulSoup(html.read(), features="html.parser")
         versions = []
         for link in soup.find_all('a'):
             text = link.get_text()
-            search_result = re.search(rf'{self.pkg}-(.*)\.tar\.gz', text)
-            if search_result is not None:
-                version = search_result.group(1)
-                versions.append(semantic_version.Version(version))
+            tar_version = self.search_tar_version(text)
+            if tar_version is not None:
+                versions.append(tar_version)
+            wheel_version = self.search_wheel_version(text)
+            if wheel_version is not None:
+                versions.append(wheel_version)
         if len(versions) == 0:
             raise NoVersionsError()
         return max(versions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyutils_basstal-0.3.9/pyutils/executor.py` & `pyutils_basstal-0.4.0/pyutils/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: E501
+
 import os
 import re
 import shlex
 import tempfile
 import time
 import subprocess
 import sys
```

### Comparing `pyutils_basstal-0.3.9/pyutils/fsext.py` & `pyutils_basstal-0.4.0/pyutils/fsext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# ruff: noqa: E501
+
 import codecs
 import ctypes
 import filecmp
 import fnmatch
 import glob
 import os
 import shutil
 import base64
 import charade
+from deprecated import deprecated
 
 import pyutils.shorthand as shd
 import pyutils.simplelogger as logger
 ########################
 ########################
 #    文件系统扩展方法    #
 ########################
@@ -180,18 +183,21 @@
         result.extend(list_dirs)
         if recursive:
             for dir in list_dirs:
                 result.extend(get_dirs(dir, recursive, ignore_patterns))
     return result
 
 
+@deprecated(version='0.3.9', reason="Please use 'get_files_glob' instead.")
 def get_files(work_dir, include_patterns=None, ignore_patterns=None, follow_links=False, recursive=True, apply_ignore_when_conflict=True):
     """
     NOTE:这里的 patterns 用的是 UNIX 通配符，而非语言正则表达式
     TODO: replace with glob.glob
+    TODO: consider remove apply_ignore_when_conflict parameter.
+    TODO: 这个函数的内部实现感觉有问题，考虑废弃掉重写。
     Args:
         ignore_patterns (list[str], optional): 文件忽略规则. Defaults to True.
 
     """
     if os.path.isfile(work_dir):
         result = [work_dir]
     else:
@@ -223,14 +229,44 @@
                             if valid:
                                 break
                     if valid:
                         result.append(full_path)
     return sorted(result)
 
 
+def get_files_glob(work_dir, include_patterns=None, ignore_patterns=None, recursive=True):
+    """
+    Args:
+        work_dir (str): 要检索的工作目录
+        include_patterns (list[str], optional): 包含的文件规则
+        ignore_patterns (list[str], optional): 忽略的文件规则
+        recursive (bool, optional): 是否递归搜索子目录，默认为True
+    """
+    if os.path.isfile(work_dir):
+        result = [work_dir]
+    else:
+        result = []
+        patterns = include_patterns or ['*']
+
+        for pattern in patterns:
+            if recursive:
+                glob_pattern = os.path.join(work_dir, '**', pattern)
+                matched_files = glob.glob(glob_pattern, recursive=True)
+            else:
+                glob_pattern = os.path.join(work_dir, pattern)
+                matched_files = glob.glob(glob_pattern)
+
+            if ignore_patterns is not None:
+                for ignore_pattern in ignore_patterns:
+                    matched_files = [file for file in matched_files if not fnmatch.fnmatch(file, ignore_pattern)]
+            result.extend(matched_files)
+
+    return sorted(set(result))
+
+
 def to_base64(src, tar=None):
     """将 src 路径指定文件转为 base64 并返回，如果提供了 tar 目标文件路径，则将返回值同时存储在 tar 目标文件
 
     Args:
         src (str): 源文件路径
         tar (str): 目标文件路径
     """
```

### Comparing `pyutils_basstal-0.3.9/pyutils/shorthand.py` & `pyutils_basstal-0.4.0/pyutils/shorthand.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.3.9/pyutils/simplelogger.py` & `pyutils_basstal-0.4.0/pyutils/simplelogger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,94 @@
+# ruff: noqa: E501
+
 import os
 import logging
 import pyutils.shorthand as shd
+import sys
 
 ######################
 ######################
 #       Log          #
 ######################
 ######################
 
 ErrorRaiseExcpetion = False
 
 logging.basicConfig(level=logging.INFO, datefmt='%y-%m-%d %H:%M:%S', format='%(message)s')
-logger = logging.getLogger()
 
 
 class SimpleLogger(object):
+    # 这是原来的 error/warning logger
+    _logger = logging.getLogger("error_logger")
+    _logger.setLevel(logging.ERROR)
+    _logger.handlers.clear()
+    _logger.addHandler(logging.StreamHandler(sys.stderr))
+    _logger.propagate = False
+    # 创建 info logger
+    _info_logger = logging.getLogger("info_logger")
+    _info_logger.setLevel(logging.INFO)
+    _info_logger.handlers.clear()
+    _info_logger.addHandler(logging.StreamHandler(sys.stdout))
+    _info_logger.propagate = False
+
+    __hanlder_cache = {}
+
     @staticmethod
     def _color_message(message, color_code, bold=False):
         if shd.is_win():
             os.system('')
         bold_code = '\033[1m' if bold else ''
         return f'{bold_code}\033[{color_code}m{message}\033[0m'
 
     @staticmethod
-    def _preprocess_message(message):
+    def _preprocess_message(message: str):
         if not shd.is_win():
             message = message.replace('=>', '➜').replace('<=', '✔')
 
         if message.endswith('\r\n') or message.endswith('\n'):
             message = message.rstrip()
         return message
 
     @staticmethod
     def info(message, _):
         message = SimpleLogger._preprocess_message(message)
-        logger.info(message)
+        SimpleLogger._info_logger.info(message)
 
     @staticmethod
     def warning(message, bold=False):
         message = SimpleLogger._preprocess_message(message)
         message = SimpleLogger._color_message(message, 33, bold)
-        logger.warning(message)
+        SimpleLogger._logger.warning(message)
 
     @staticmethod
     def error(message, bold=False):
         if ErrorRaiseExcpetion:
             raise Exception(message)
         message = SimpleLogger._preprocess_message(message)
         message = SimpleLogger._color_message(message, 31, bold)
-        logger.error(message)
+        SimpleLogger._logger.error(message)
+
+    @staticmethod
+    def addFileHandler(file_path):
+        if file_path in SimpleLogger.__hanlder_cache:
+            return
+        file_handler = logging.FileHandler(file_path)
+        SimpleLogger.__hanlder_cache[file_path] = file_handler
+        SimpleLogger._logger.addHandler(file_handler)
+        SimpleLogger._info_logger.addHandler(file_handler)
+
+    @staticmethod
+    def removeFileHander(file_path):
+        if file_path in SimpleLogger.__hanlder_cache:
+            return
+        file_handler = SimpleLogger.__hanlder_cache[file_path]
+        SimpleLogger._logger.removeHandler(file_handler)
+        SimpleLogger._info_logger.removeHandler(file_handler)
+        file_handler.close()
+        del SimpleLogger.__hanlder_cache[file_path]
 
 
 def info(message, bold=False):
     SimpleLogger.info(message, bold)
 
 
 def warning(message, bold=False):
```

### Comparing `pyutils_basstal-0.3.9/pyutils/templite.py` & `pyutils_basstal-0.4.0/pyutils/templite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: E501
+
 #!/usr/bin/env python
 #
 #  Templite+
 #  A light-weight, fully functional, general purpose templating engine
 #
 #  Copyright (c) 2009 joonis new media
 #  Author: Thimo Kraemer <thimo.kraemer@joonis.de>
```

### Comparing `pyutils_basstal-0.3.9/pyutils_basstal.egg-info/PKG-INFO` & `pyutils_basstal-0.4.0/pyutils_basstal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils-basstal
-Version: 0.3.9
+Version: 0.4.0
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.3.9/setup.py` & `pyutils_basstal-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 See:
 https://packaging.python.org/guides/distributing-packages-using-setuptools/
 https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
@@ -32,15 +32,15 @@
     name="pyutils_basstal",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.3.9",  # Required
+    version="0.4.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="self used py utils",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

