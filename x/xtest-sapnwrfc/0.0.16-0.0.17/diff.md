# Comparing `tmp/xtest_sapnwrfc-0.0.16.tar.gz` & `tmp/xtest_sapnwrfc-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtest_sapnwrfc-0.0.16.tar", last modified: Mon Apr 24 17:32:27 2023, max compression
+gzip compressed data, was "xtest_sapnwrfc-0.0.17.tar", last modified: Tue Apr 25 10:46:48 2023, max compression
```

## Comparing `xtest_sapnwrfc-0.0.16.tar` & `xtest_sapnwrfc-0.0.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:32:27.649243 xtest_sapnwrfc-0.0.16/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:32:27.633486 xtest_sapnwrfc-0.0.16/LICENSES/
--rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.16/LICENSES/Apache-2.0.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       78 2023-04-24 14:29:18.000000 xtest_sapnwrfc-0.0.16/MANIFEST.in
--rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 17:32:27.648955 xtest_sapnwrfc-0.0.16/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)    10368 2023-04-24 13:13:41.000000 xtest_sapnwrfc-0.0.16/README.md
--rw-r--r--   0 d037732    (501) wheel        (0)     1847 2023-04-24 17:32:25.000000 xtest_sapnwrfc-0.0.16/pyproject.toml
--rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 17:32:27.649285 xtest_sapnwrfc-0.0.16/setup.cfg
--rw-r--r--   0 d037732    (501) wheel        (0)     5751 2023-04-24 17:29:54.000000 xtest_sapnwrfc-0.0.16/setup.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:32:27.631396 xtest_sapnwrfc-0.0.16/src/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:32:27.643813 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/
--rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/__init__.py
--rw-r--r--   0 d037732    (501) wheel        (0)  2315334 2023-04-24 13:40:35.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_cyrfc.cpp
--rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_cyrfc.pyx
--rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_exception.py
--rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_utils.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)    23820 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/csapnwrfc.pxd
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:32:27.647536 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/
--rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 17:32:27.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)      423 2023-04-24 17:32:27.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/SOURCES.txt
--rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 17:32:27.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/dependency_links.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 17:32:27.000000 xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/top_level.txt
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-25 10:46:48.925305 xtest_sapnwrfc-0.0.17/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-25 10:46:48.911785 xtest_sapnwrfc-0.0.17/LICENSES/
+-rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.17/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       67 2023-04-25 10:44:01.000000 xtest_sapnwrfc-0.0.17/MANIFEST.in
+-rw-r--r--   0 d037732    (501) wheel        (0)    23397 2023-04-25 10:46:48.923819 xtest_sapnwrfc-0.0.17/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)    10174 2023-04-24 17:43:16.000000 xtest_sapnwrfc-0.0.17/README.md
+-rw-r--r--   0 d037732    (501) wheel        (0)     1833 2023-04-25 10:46:08.000000 xtest_sapnwrfc-0.0.17/pyproject.toml
+-rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-25 10:46:48.925399 xtest_sapnwrfc-0.0.17/setup.cfg
+-rw-r--r--   0 d037732    (501) wheel        (0)     5751 2023-04-25 10:37:45.000000 xtest_sapnwrfc-0.0.17/setup.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-25 10:46:48.908660 xtest_sapnwrfc-0.0.17/src/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-25 10:46:48.919221 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/__init__.py
+-rw-r--r--   0 d037732    (501) wheel        (0)  2315334 2023-04-24 13:40:35.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_cyrfc.cpp
+-rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_cyrfc.pyx
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_exception.py
+-rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_utils.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)    23820 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/csapnwrfc.pxd
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-25 10:46:48.922819 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/
+-rw-r--r--   0 d037732    (501) wheel        (0)    23397 2023-04-25 10:46:48.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)      423 2023-04-25 10:46:48.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-25 10:46:48.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-25 10:46:48.000000 xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/top_level.txt
```

### Comparing `xtest_sapnwrfc-0.0.16/LICENSES/Apache-2.0.txt` & `xtest_sapnwrfc-0.0.17/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/PKG-INFO` & `xtest_sapnwrfc-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest_sapnwrfc
-Version: 0.0.16
+Version: 0.0.17
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
@@ -252,16 +252,14 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
-  - [Linux](#linux)
-  - [Windows and macOS](#windows-and-macos)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -316,43 +314,35 @@
 
 - Remote paths must be set in SAP NWRFC SDK for macOS: [documentation](http://sap.github.io/PyRFC/install.html#macos)
 
 - When the PyRFC is started for the first time, the popups may come-up for each NWRFC SDK library, to confirm the usage. If SAP NW RFC SDK is installed in admin folder, the app shall be first time started with admin privileges, eg. `sudo -E`
 
 ## Download and installation
 
-### Linux
-
-Cython must be installed upfront because the build from source is standard installation method on Linux.
-
-Also the `pip` option `--no-build-isolation` is mandatory:
-
-```shell
-pip install --no-build-isolation pyrfc
-```
-
-### Windows and macOS
-
 ```shell
 pip install pyrfc
 ```
 
-Build from source can be requested also on Windows and macOS platforms:
+Cython must be installed upfront because the build from source is standard installation method on Linux.
+
+Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
 PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
+python -m pip install .
+# or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
```

### Comparing `xtest_sapnwrfc-0.0.16/README.md` & `xtest_sapnwrfc-0.0.17/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
-  - [Linux](#linux)
-  - [Windows and macOS](#windows-and-macos)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -78,43 +76,35 @@
 
 - Remote paths must be set in SAP NWRFC SDK for macOS: [documentation](http://sap.github.io/PyRFC/install.html#macos)
 
 - When the PyRFC is started for the first time, the popups may come-up for each NWRFC SDK library, to confirm the usage. If SAP NW RFC SDK is installed in admin folder, the app shall be first time started with admin privileges, eg. `sudo -E`
 
 ## Download and installation
 
-### Linux
-
-Cython must be installed upfront because the build from source is standard installation method on Linux.
-
-Also the `pip` option `--no-build-isolation` is mandatory:
-
-```shell
-pip install --no-build-isolation pyrfc
-```
-
-### Windows and macOS
-
 ```shell
 pip install pyrfc
 ```
 
-Build from source can be requested also on Windows and macOS platforms:
+Cython must be installed upfront because the build from source is standard installation method on Linux.
+
+Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
 PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
+python -m pip install .
+# or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
```

### Comparing `xtest_sapnwrfc-0.0.16/pyproject.toml` & `xtest_sapnwrfc-0.0.17/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["Cython ~= 0.29.0", "setuptools ~= 67.7.0", "wheel ~= 0.40.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "xtest_sapnwrfc"
-version = "0.0.16"
+version = "0.0.17"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"} ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.7"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
@@ -38,16 +38,17 @@
 repository = "https://github.com/SAP/PyRFC.git"
 
 [tool.cython-lint]
 max-line-length = 148
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [tool.setuptools]
-#include-package-data = false
-exclude-package-data = {"*" = ["*.cpp", "*.html", "*.pyx", "*.pxd"]}
+package-dir = {"" = "src"}
+include-package-data = false
 license-files=["LICENSES/*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
+include = ["xtest_sapnwrfc"]
 
 [tool.setuptools.dynamic]
 readme = {file = "README.md"}
```

### Comparing `xtest_sapnwrfc-0.0.16/setup.py` & `xtest_sapnwrfc-0.0.17/setup.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/__init__.py` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/__init__.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_cyrfc.cpp` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_cyrfc.cpp`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_cyrfc.pyx` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/_exception.py` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc/csapnwrfc.pxd` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.16/src/xtest_sapnwrfc.egg-info/PKG-INFO` & `xtest_sapnwrfc-0.0.17/src/xtest_sapnwrfc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest-sapnwrfc
-Version: 0.0.16
+Version: 0.0.17
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
@@ -252,16 +252,14 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
-  - [Linux](#linux)
-  - [Windows and macOS](#windows-and-macos)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -316,43 +314,35 @@
 
 - Remote paths must be set in SAP NWRFC SDK for macOS: [documentation](http://sap.github.io/PyRFC/install.html#macos)
 
 - When the PyRFC is started for the first time, the popups may come-up for each NWRFC SDK library, to confirm the usage. If SAP NW RFC SDK is installed in admin folder, the app shall be first time started with admin privileges, eg. `sudo -E`
 
 ## Download and installation
 
-### Linux
-
-Cython must be installed upfront because the build from source is standard installation method on Linux.
-
-Also the `pip` option `--no-build-isolation` is mandatory:
-
-```shell
-pip install --no-build-isolation pyrfc
-```
-
-### Windows and macOS
-
 ```shell
 pip install pyrfc
 ```
 
-Build from source can be requested also on Windows and macOS platforms:
+Cython must be installed upfront because the build from source is standard installation method on Linux.
+
+Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
 PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
+python -m pip install .
+# or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
```

