# Comparing `tmp/varc-1.0.6.tar.gz` & `tmp/varc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varc-1.0.6.tar", last modified: Sun Oct  2 20:01:46 2022, max compression
+gzip compressed data, was "varc-1.0.7.tar", last modified: Tue Apr 25 09:24:07 2023, max compression
```

## Comparing `varc-1.0.6.tar` & `varc-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.489961 varc-1.0.6/
--rw-rw-rw-   0        0        0    35149 2022-09-16 14:02:49.000000 varc-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     5401 2022-10-02 20:01:46.489961 varc-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4909 2022-09-28 09:58:46.000000 varc-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2022-10-02 20:01:46.489961 varc-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      737 2022-10-02 20:00:31.000000 varc-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.449823 varc-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2022-09-16 14:02:49.000000 varc-1.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      874 2022-09-16 14:02:49.000000 varc-1.0.6/tests/test_import.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.449823 varc-1.0.6/tests/test_linux/
--rw-rw-rw-   0        0        0        0 2022-09-16 14:02:49.000000 varc-1.0.6/tests/test_linux/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-09-16 14:02:49.000000 varc-1.0.6/tests/test_linux/test_base.py
--rw-rw-rw-   0        0        0      831 2022-09-16 14:02:49.000000 varc-1.0.6/tests/test_shared.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.466851 varc-1.0.6/varc.egg-info/
--rw-rw-rw-   0        0        0     5401 2022-10-02 20:01:46.000000 varc-1.0.6/varc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2022-10-02 20:01:46.000000 varc-1.0.6/varc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 20:01:46.000000 varc-1.0.6/varc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-10-02 20:01:46.000000 varc-1.0.6/varc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-10-02 20:01:46.000000 varc-1.0.6/varc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1240 2022-09-16 14:02:49.000000 varc-1.0.6/varc.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.466851 varc-1.0.6/varc_core/
--rw-rw-rw-   0        0        0        0 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/__init__.py
--rw-rw-rw-   0        0        0      411 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.482568 varc-1.0.6/varc_core/systems/
--rw-rw-rw-   0        0        0     1071 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/systems/__init__.py
--rw-rw-rw-   0        0        0    10582 2022-09-30 12:48:34.000000 varc-1.0.6/varc_core/systems/base_system.py
--rw-rw-rw-   0        0        0     5470 2022-10-02 19:58:28.000000 varc-1.0.6/varc_core/systems/linux.py
--rw-rw-rw-   0        0        0      409 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/systems/osx.py
--rw-rw-rw-   0        0        0     3938 2022-09-28 09:58:25.000000 varc-1.0.6/varc_core/systems/windows.py
-drwxrwxrwx   0        0        0        0 2022-10-02 20:01:46.489961 varc-1.0.6/varc_core/utils/
--rw-rw-rw-   0        0        0        0 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/utils/__init__.py
--rw-rw-rw-   0        0        0     9924 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/utils/dumpfile_extraction.py
--rw-rw-rw-   0        0        0      564 2022-09-16 14:02:49.000000 varc-1.0.6/varc_core/utils/string_manips.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.748706 varc-1.0.7/
+-rw-r--r--   0 chris      (503) staff       (20)    35149 2023-04-25 09:17:21.000000 varc-1.0.7/LICENSE
+-rw-r--r--   0 chris      (503) staff       (20)     5249 2023-04-25 09:24:07.748596 varc-1.0.7/PKG-INFO
+-rw-r--r--   0 chris      (503) staff       (20)     4909 2023-04-25 09:17:21.000000 varc-1.0.7/README.md
+-rw-r--r--   0 chris      (503) staff       (20)       38 2023-04-25 09:24:07.748736 varc-1.0.7/setup.cfg
+-rw-r--r--   0 chris      (503) staff       (20)      737 2023-04-25 09:23:51.000000 varc-1.0.7/setup.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.746265 varc-1.0.7/tests/
+-rw-r--r--   0 chris      (503) staff       (20)        0 2023-04-25 09:17:21.000000 varc-1.0.7/tests/__init__.py
+-rw-r--r--   0 chris      (503) staff       (20)      874 2023-04-25 09:17:21.000000 varc-1.0.7/tests/test_import.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.746493 varc-1.0.7/tests/test_linux/
+-rw-r--r--   0 chris      (503) staff       (20)        0 2023-04-25 09:17:21.000000 varc-1.0.7/tests/test_linux/__init__.py
+-rw-r--r--   0 chris      (503) staff       (20)     1078 2023-04-25 09:17:21.000000 varc-1.0.7/tests/test_linux/test_base.py
+-rw-r--r--   0 chris      (503) staff       (20)      831 2023-04-25 09:17:21.000000 varc-1.0.7/tests/test_shared.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.747131 varc-1.0.7/varc.egg-info/
+-rw-r--r--   0 chris      (503) staff       (20)     5249 2023-04-25 09:24:07.000000 varc-1.0.7/varc.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (503) staff       (20)      582 2023-04-25 09:24:07.000000 varc-1.0.7/varc.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (503) staff       (20)        1 2023-04-25 09:24:07.000000 varc-1.0.7/varc.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (503) staff       (20)       22 2023-04-25 09:24:07.000000 varc-1.0.7/varc.egg-info/requires.txt
+-rw-r--r--   0 chris      (503) staff       (20)       21 2023-04-25 09:24:07.000000 varc-1.0.7/varc.egg-info/top_level.txt
+-rw-r--r--   0 chris      (503) staff       (20)     1240 2023-04-25 09:17:21.000000 varc-1.0.7/varc.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.747327 varc-1.0.7/varc_core/
+-rw-r--r--   0 chris      (503) staff       (20)        0 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/__init__.py
+-rw-r--r--   0 chris      (503) staff       (20)      411 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/exceptions.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.748063 varc-1.0.7/varc_core/systems/
+-rw-r--r--   0 chris      (503) staff       (20)     1071 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/systems/__init__.py
+-rw-r--r--   0 chris      (503) staff       (20)    10660 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/systems/base_system.py
+-rw-r--r--   0 chris      (503) staff       (20)     6551 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/systems/linux.py
+-rw-r--r--   0 chris      (503) staff       (20)      409 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/systems/osx.py
+-rw-r--r--   0 chris      (503) staff       (20)     3938 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/systems/windows.py
+drwxr-xr-x   0 chris      (503) staff       (20)        0 2023-04-25 09:24:07.748440 varc-1.0.7/varc_core/utils/
+-rw-r--r--   0 chris      (503) staff       (20)        0 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/utils/__init__.py
+-rw-r--r--   0 chris      (503) staff       (20)     9924 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/utils/dumpfile_extraction.py
+-rw-r--r--   0 chris      (503) staff       (20)      564 2023-04-25 09:17:21.000000 varc-1.0.7/varc_core/utils/string_manips.py
```

### Comparing `varc-1.0.6/LICENSE` & `varc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/PKG-INFO` & `varc-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,111 @@
-Metadata-Version: 2.1
-Name: varc
-Version: 1.0.6
-Summary: varc Volatile Artifact Collector
-Home-page: https://github.com/cado-security/varc
-Author: Cado Security
-Author-email: varc@cadosecurity.com
-License: UNKNOWN
-Download-URL: https://github.com/cado-security/varc/archive/refs/heads/main.zip
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# varc (Volatile Artifact Collector) #
-![ci](https://github.com/cado-security/varc/actions/workflows/app-ci.yml/badge.svg?branch=main)
-[![PyPI version](https://badge.fury.io/py/varc.svg)](https://badge.fury.io/py/varc)
-
-varc collects a snapshot of volatile data from a system.
-It tells you what is happening on a system, and is of particular use when investigating a security incident.
-
-It creates a zip, which contains a number of different pieces of data to understand what is happening on a system:
-- JSON files e.g. running processes and what network connections they are making
-- Memory of running proccesses, on a per-process basis. This is also carved to extract log and text data from memory
-- Netstat data of active connections
-- The contents of open files, for example running binaries
-
-We have successfully executed it across:
-- Windows
-- Linux
-- OSX
-- Cloud environments such as AWS EC2
-- Containerised Docker/Kubernetes environments such as AWS ECS/EKS/Fargate and Azure AKS
-- Even serverless environments such as AWS Lambda
-
-Check out the example captures under the "Releases" tab to see some crazy data!
-The screen recording below shows a collection from a Docker container (left) and the output from running inside and AWS Lambda function which deployed Xmrig (right):
-
-![](docs/varc_demo.gif)
-
-In line with the order of volatility, we collect process memory before anything else. Note that varc, and any other tool that runs inside a system, will impact the memory of a system.
-
-### Using as a compiled binary ###
-You can find compiled binaries for Windows, Linux and OSX under the Releases tab.
-Simply execute and a zip is created with the output.
-To access some data, you will need to run with elevated privileges (i.e. sudo or root on Linux).
-```
-usage: varc [-h] [--skip-memory] [--skip-open] [--dump-extract] ...
-
-optional arguments:
-  -h, --help      show this help message and exit
-  --skip-memory   Skip collecting process memory, which can be slow
-  --skip-open     Skip collecting open files, which can be slow
-  --dump-extract  Extract process memory dumps, which can be slow
-```
-
-### Using as a Python library ###
-
-Install from pip with:
-```
-pip3 install varc
-```
-
-Or alternatively, clone this repository then install with:
-```
-python3 setup.py install
-```
-
-Then call with: 
-```
-from varc import acquire_system
-output_file_path = acquire_system().zip_path
-```
-
-### Automated Investigations and Response ###
-varc significantly simplifies the acquisition and analysis of volatile data.
-Whilst it can be used manually on an ad-hoc basis, it is a great match for automatic deployment in response to security detections.
-The output of varc is designed to be easily consumed by other tools, in standard JSON format as much as possible.
-
-A typical pipeline might be:
-* A detection is fired from a detection tool
-* varc is deployed to collect and identify further activity
-* Further remediation actions are taken based on the analysis of varc output
-
- ### Why are the collected memory files empty? ###
-Process memory collection is not currently supported on OSX.
-
-If you run varc on a Linux system without the Ptrace Kernel capability enabled, you will get empty memory files.
-You will still get detailed system output.
-
-For example, in our testing:
-* AWS Lambda successfully dumped process memory by default.
-* EKS on EC2 successfully dumped process memory by default.
-* ECS on Fargate required us to enable [CAP_SYS_PTRACE](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-kernelcapabilities.html) in our task definition.
-
-
-### Using the collected data ###
-All data is saved in an open, non-propietary format in the hope it can easily be processed by other community tools.
-
-Our free tool [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/) will happily parse this zip, and display the JSON data tables as intended.
-
-Our commercial tool [Cado Response](https://www.cadosecurity.com/platform/) additionally enables you to automatically capture both static and volatile data from systems through Cado Host. By using the API, you can automatically investigate and respond to to detections from third party tools such as an EDR like SentinelOne or a cloud detection tool like GuardDuty.
-
-Here is an example of varc output for a Lambda function running xmrig, viewed in [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/):
-![](docs/varc.png)
-
-### License ###
-This is licensed under the GPL. Please contact us if this does not work for your use case - we may be able to alternatively license under a non-copyleft license such as the Apache License. We're friendly!
-As this software is licensed under the GPL and used in our commercial product, we ask any contributors to sign a simple Contributor License Agreement (CLA). 
-
-### License ###
-We would love any Pull Requests or Bug Reports!
-
-
-
-
+Metadata-Version: 2.1
+Name: varc
+Version: 1.0.7
+Summary: varc Volatile Artifact Collector
+Home-page: https://github.com/cado-security/varc
+Download-URL: https://github.com/cado-security/varc/archive/refs/heads/main.zip
+Author: Cado Security
+Author-email: varc@cadosecurity.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# varc (Volatile Artifact Collector) #
+![ci](https://github.com/cado-security/varc/actions/workflows/app-ci.yml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/varc.svg)](https://badge.fury.io/py/varc)
+
+varc collects a snapshot of volatile data from a system.
+It tells you what is happening on a system, and is of particular use when investigating a security incident.
+
+It creates a zip, which contains a number of different pieces of data to understand what is happening on a system:
+- JSON files e.g. running processes and what network connections they are making
+- Memory of running proccesses, on a per-process basis. This is also carved to extract log and text data from memory
+- Netstat data of active connections
+- The contents of open files, for example running binaries
+
+We have successfully executed it across:
+- Windows
+- Linux
+- OSX
+- Cloud environments such as AWS EC2
+- Containerised Docker/Kubernetes environments such as AWS ECS/EKS/Fargate and Azure AKS
+- Even serverless environments such as AWS Lambda
+
+Check out the example captures under the "Releases" tab to see some crazy data!
+The screen recording below shows a collection from a Docker container (left) and the output from running inside and AWS Lambda function which deployed Xmrig (right):
+
+![](docs/varc_demo.gif)
+
+In line with the order of volatility, we collect process memory before anything else. Note that varc, and any other tool that runs inside a system, will impact the memory of a system.
+
+### Using as a compiled binary ###
+You can find compiled binaries for Windows, Linux and OSX under the Releases tab.
+Simply execute and a zip is created with the output.
+To access some data, you will need to run with elevated privileges (i.e. sudo or root on Linux).
+```
+usage: varc [-h] [--skip-memory] [--skip-open] [--dump-extract] ...
+
+optional arguments:
+  -h, --help      show this help message and exit
+  --skip-memory   Skip collecting process memory, which can be slow
+  --skip-open     Skip collecting open files, which can be slow
+  --dump-extract  Extract process memory dumps, which can be slow
+```
+
+### Using as a Python library ###
+
+Install from pip with:
+```
+pip3 install varc
+```
+
+Or alternatively, clone this repository then install with:
+```
+python3 setup.py install
+```
+
+Then call with: 
+```
+from varc import acquire_system
+output_file_path = acquire_system().zip_path
+```
+
+### Automated Investigations and Response ###
+varc significantly simplifies the acquisition and analysis of volatile data.
+Whilst it can be used manually on an ad-hoc basis, it is a great match for automatic deployment in response to security detections.
+The output of varc is designed to be easily consumed by other tools, in standard JSON format as much as possible.
+
+A typical pipeline might be:
+* A detection is fired from a detection tool
+* varc is deployed to collect and identify further activity
+* Further remediation actions are taken based on the analysis of varc output
+
+ ### Why are the collected memory files empty? ###
+Process memory collection is not currently supported on OSX.
+
+If you run varc on a Linux system without the Ptrace Kernel capability enabled, you will get empty memory files.
+You will still get detailed system output.
+
+For example, in our testing:
+* AWS Lambda successfully dumped process memory by default.
+* EKS on EC2 successfully dumped process memory by default.
+* ECS on Fargate required us to enable [CAP_SYS_PTRACE](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-kernelcapabilities.html) in our task definition.
+
+
+### Using the collected data ###
+All data is saved in an open, non-propietary format in the hope it can easily be processed by other community tools.
+
+Our free tool [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/) will happily parse this zip, and display the JSON data tables as intended.
+
+Our commercial tool [Cado Response](https://www.cadosecurity.com/platform/) additionally enables you to automatically capture both static and volatile data from systems through Cado Host. By using the API, you can automatically investigate and respond to to detections from third party tools such as an EDR like SentinelOne or a cloud detection tool like GuardDuty.
+
+Here is an example of varc output for a Lambda function running xmrig, viewed in [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/):
+![](docs/varc.png)
+
+### License ###
+This is licensed under the GPL. Please contact us if this does not work for your use case - we may be able to alternatively license under a non-copyleft license such as the Apache License. We're friendly!
+As this software is licensed under the GPL and used in our commercial product, we ask any contributors to sign a simple Contributor License Agreement (CLA). 
+
+### License ###
+We would love any Pull Requests or Bug Reports!
+
+
```

### Comparing `varc-1.0.6/README.md` & `varc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/setup.py` & `varc-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 setup(
     name='varc',
     version=VERSION,
     description='varc Volatile Artifact Collector',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `varc-1.0.6/tests/test_import.py` & `varc-1.0.7/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/tests/test_linux/test_base.py` & `varc-1.0.7/tests/test_linux/test_base.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/tests/test_shared.py` & `varc-1.0.7/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc.egg-info/PKG-INFO` & `varc-1.0.7/varc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,111 @@
-Metadata-Version: 2.1
-Name: varc
-Version: 1.0.6
-Summary: varc Volatile Artifact Collector
-Home-page: https://github.com/cado-security/varc
-Author: Cado Security
-Author-email: varc@cadosecurity.com
-License: UNKNOWN
-Download-URL: https://github.com/cado-security/varc/archive/refs/heads/main.zip
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# varc (Volatile Artifact Collector) #
-![ci](https://github.com/cado-security/varc/actions/workflows/app-ci.yml/badge.svg?branch=main)
-[![PyPI version](https://badge.fury.io/py/varc.svg)](https://badge.fury.io/py/varc)
-
-varc collects a snapshot of volatile data from a system.
-It tells you what is happening on a system, and is of particular use when investigating a security incident.
-
-It creates a zip, which contains a number of different pieces of data to understand what is happening on a system:
-- JSON files e.g. running processes and what network connections they are making
-- Memory of running proccesses, on a per-process basis. This is also carved to extract log and text data from memory
-- Netstat data of active connections
-- The contents of open files, for example running binaries
-
-We have successfully executed it across:
-- Windows
-- Linux
-- OSX
-- Cloud environments such as AWS EC2
-- Containerised Docker/Kubernetes environments such as AWS ECS/EKS/Fargate and Azure AKS
-- Even serverless environments such as AWS Lambda
-
-Check out the example captures under the "Releases" tab to see some crazy data!
-The screen recording below shows a collection from a Docker container (left) and the output from running inside and AWS Lambda function which deployed Xmrig (right):
-
-![](docs/varc_demo.gif)
-
-In line with the order of volatility, we collect process memory before anything else. Note that varc, and any other tool that runs inside a system, will impact the memory of a system.
-
-### Using as a compiled binary ###
-You can find compiled binaries for Windows, Linux and OSX under the Releases tab.
-Simply execute and a zip is created with the output.
-To access some data, you will need to run with elevated privileges (i.e. sudo or root on Linux).
-```
-usage: varc [-h] [--skip-memory] [--skip-open] [--dump-extract] ...
-
-optional arguments:
-  -h, --help      show this help message and exit
-  --skip-memory   Skip collecting process memory, which can be slow
-  --skip-open     Skip collecting open files, which can be slow
-  --dump-extract  Extract process memory dumps, which can be slow
-```
-
-### Using as a Python library ###
-
-Install from pip with:
-```
-pip3 install varc
-```
-
-Or alternatively, clone this repository then install with:
-```
-python3 setup.py install
-```
-
-Then call with: 
-```
-from varc import acquire_system
-output_file_path = acquire_system().zip_path
-```
-
-### Automated Investigations and Response ###
-varc significantly simplifies the acquisition and analysis of volatile data.
-Whilst it can be used manually on an ad-hoc basis, it is a great match for automatic deployment in response to security detections.
-The output of varc is designed to be easily consumed by other tools, in standard JSON format as much as possible.
-
-A typical pipeline might be:
-* A detection is fired from a detection tool
-* varc is deployed to collect and identify further activity
-* Further remediation actions are taken based on the analysis of varc output
-
- ### Why are the collected memory files empty? ###
-Process memory collection is not currently supported on OSX.
-
-If you run varc on a Linux system without the Ptrace Kernel capability enabled, you will get empty memory files.
-You will still get detailed system output.
-
-For example, in our testing:
-* AWS Lambda successfully dumped process memory by default.
-* EKS on EC2 successfully dumped process memory by default.
-* ECS on Fargate required us to enable [CAP_SYS_PTRACE](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-kernelcapabilities.html) in our task definition.
-
-
-### Using the collected data ###
-All data is saved in an open, non-propietary format in the hope it can easily be processed by other community tools.
-
-Our free tool [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/) will happily parse this zip, and display the JSON data tables as intended.
-
-Our commercial tool [Cado Response](https://www.cadosecurity.com/platform/) additionally enables you to automatically capture both static and volatile data from systems through Cado Host. By using the API, you can automatically investigate and respond to to detections from third party tools such as an EDR like SentinelOne or a cloud detection tool like GuardDuty.
-
-Here is an example of varc output for a Lambda function running xmrig, viewed in [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/):
-![](docs/varc.png)
-
-### License ###
-This is licensed under the GPL. Please contact us if this does not work for your use case - we may be able to alternatively license under a non-copyleft license such as the Apache License. We're friendly!
-As this software is licensed under the GPL and used in our commercial product, we ask any contributors to sign a simple Contributor License Agreement (CLA). 
-
-### License ###
-We would love any Pull Requests or Bug Reports!
-
-
-
-
+Metadata-Version: 2.1
+Name: varc
+Version: 1.0.7
+Summary: varc Volatile Artifact Collector
+Home-page: https://github.com/cado-security/varc
+Download-URL: https://github.com/cado-security/varc/archive/refs/heads/main.zip
+Author: Cado Security
+Author-email: varc@cadosecurity.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# varc (Volatile Artifact Collector) #
+![ci](https://github.com/cado-security/varc/actions/workflows/app-ci.yml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/varc.svg)](https://badge.fury.io/py/varc)
+
+varc collects a snapshot of volatile data from a system.
+It tells you what is happening on a system, and is of particular use when investigating a security incident.
+
+It creates a zip, which contains a number of different pieces of data to understand what is happening on a system:
+- JSON files e.g. running processes and what network connections they are making
+- Memory of running proccesses, on a per-process basis. This is also carved to extract log and text data from memory
+- Netstat data of active connections
+- The contents of open files, for example running binaries
+
+We have successfully executed it across:
+- Windows
+- Linux
+- OSX
+- Cloud environments such as AWS EC2
+- Containerised Docker/Kubernetes environments such as AWS ECS/EKS/Fargate and Azure AKS
+- Even serverless environments such as AWS Lambda
+
+Check out the example captures under the "Releases" tab to see some crazy data!
+The screen recording below shows a collection from a Docker container (left) and the output from running inside and AWS Lambda function which deployed Xmrig (right):
+
+![](docs/varc_demo.gif)
+
+In line with the order of volatility, we collect process memory before anything else. Note that varc, and any other tool that runs inside a system, will impact the memory of a system.
+
+### Using as a compiled binary ###
+You can find compiled binaries for Windows, Linux and OSX under the Releases tab.
+Simply execute and a zip is created with the output.
+To access some data, you will need to run with elevated privileges (i.e. sudo or root on Linux).
+```
+usage: varc [-h] [--skip-memory] [--skip-open] [--dump-extract] ...
+
+optional arguments:
+  -h, --help      show this help message and exit
+  --skip-memory   Skip collecting process memory, which can be slow
+  --skip-open     Skip collecting open files, which can be slow
+  --dump-extract  Extract process memory dumps, which can be slow
+```
+
+### Using as a Python library ###
+
+Install from pip with:
+```
+pip3 install varc
+```
+
+Or alternatively, clone this repository then install with:
+```
+python3 setup.py install
+```
+
+Then call with: 
+```
+from varc import acquire_system
+output_file_path = acquire_system().zip_path
+```
+
+### Automated Investigations and Response ###
+varc significantly simplifies the acquisition and analysis of volatile data.
+Whilst it can be used manually on an ad-hoc basis, it is a great match for automatic deployment in response to security detections.
+The output of varc is designed to be easily consumed by other tools, in standard JSON format as much as possible.
+
+A typical pipeline might be:
+* A detection is fired from a detection tool
+* varc is deployed to collect and identify further activity
+* Further remediation actions are taken based on the analysis of varc output
+
+ ### Why are the collected memory files empty? ###
+Process memory collection is not currently supported on OSX.
+
+If you run varc on a Linux system without the Ptrace Kernel capability enabled, you will get empty memory files.
+You will still get detailed system output.
+
+For example, in our testing:
+* AWS Lambda successfully dumped process memory by default.
+* EKS on EC2 successfully dumped process memory by default.
+* ECS on Fargate required us to enable [CAP_SYS_PTRACE](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-kernelcapabilities.html) in our task definition.
+
+
+### Using the collected data ###
+All data is saved in an open, non-propietary format in the hope it can easily be processed by other community tools.
+
+Our free tool [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/) will happily parse this zip, and display the JSON data tables as intended.
+
+Our commercial tool [Cado Response](https://www.cadosecurity.com/platform/) additionally enables you to automatically capture both static and volatile data from systems through Cado Host. By using the API, you can automatically investigate and respond to to detections from third party tools such as an EDR like SentinelOne or a cloud detection tool like GuardDuty.
+
+Here is an example of varc output for a Lambda function running xmrig, viewed in [Cado Community Edition](https://www.cadosecurity.com/cado-community-edition/):
+![](docs/varc.png)
+
+### License ###
+This is licensed under the GPL. Please contact us if this does not work for your use case - we may be able to alternatively license under a non-copyleft license such as the Apache License. We're friendly!
+As this software is licensed under the GPL and used in our commercial product, we ask any contributors to sign a simple Contributor License Agreement (CLA). 
+
+### License ###
+We would love any Pull Requests or Bug Reports!
+
+
```

### Comparing `varc-1.0.6/varc.egg-info/SOURCES.txt` & `varc-1.0.7/varc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc.py` & `varc-1.0.7/varc.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc_core/systems/__init__.py` & `varc-1.0.7/varc_core/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc_core/systems/base_system.py` & `varc-1.0.7/varc_core/systems/base_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         logging.info(f'Acquiring system: {self.get_machine_name()}, at {self.todays_date}')
         self.timestamp = datetime.timestamp(datetime.now())
         self.process_name = process_name
         self.process_id = process_id
         self.extract_dumps = extract_dumps
         self.include_memory = include_memory
         self.include_open = include_open
+        self.screenshot = take_screenshot
 
         if self.process_name and self.process_id:
             raise ValueError(
                 "Only one of Process name or Process ID (PID) can be used. Please re-run using one or the other.")
         self.zip_path = self.acquire_volatile()
 
     def get_network(self) -> List[str]:
@@ -219,34 +220,34 @@
         self.process_info = self.get_processes()
         self.network_log = self.get_network()
         self.dumped_files = self.dump_loaded_files() if self.include_open else []
         table_data = {}
         table_data["processes"] = self.dict_to_json(self.process_info)
         open_files_dict = [{"Open File": open_file} for open_file in self.dumped_files]
         table_data["open_files"] = self.dict_to_json(open_files_dict)
-        if self.take_screenshot:
-            screenshot = self.take_screenshot()
+        if self.screenshot:
+            screenshot_image = self.take_screenshot()
         else:
-            screenshot = None
+            screenshot_image = None
         if not output_path:
             output_path = os.path.join("", f"{self.get_machine_name()}-{self.timestamp}.zip")
         # strip .zip if in filename as shutil appends to end
         archive_out = output_path + ".zip" if not output_path.endswith(".zip") else output_path
         self.output_path = output_path
         with zipfile.ZipFile(archive_out, 'a', compression=zipfile.ZIP_DEFLATED) as zip_file:
-            if screenshot:
-                zip_file.writestr(f"{self.get_machine_name()}-{self.timestamp}.png", screenshot)
+            if screenshot_image:
+                zip_file.writestr(f"{self.get_machine_name()}-{self.timestamp}.png", screenshot_image)
             for key, value in table_data.items():
                 with zip_file.open(f"{key}.json", 'w') as json_file:
                     json_file.write(value.encode())
             if self.network_log:
                 logging.info("Adding Netstat Data")
                 with zip_file.open("netstat.log", 'w') as network_file:
                     network_file.write("\r\n".join(self.network_log).encode())
-            if self.dump_loaded_files:
+            if self.include_open and self.dumped_files:
                 for file_path in self.dumped_files:
                     logging.info(f"Adding open file {file_path}")
                     try:
                         if os.path.getsize(file_path) > _MAX_OPEN_FILE_SIZE:
                             logging.warning(f"Skipping file as too large {file_path}")
                         else:
                             try:
```

### Comparing `varc-1.0.6/varc_core/systems/linux.py` & `varc-1.0.7/varc_core/systems/linux.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             ctypes.c_ulong, 
             ctypes.POINTER(IOVec), 
             ctypes.c_ulong, 
             ctypes.c_ulong
         ]
         self.process_vm_readv.restype = ctypes.c_ssize_t
         if self.include_memory:
+            self._MAX_VIRTUAL_PAGE_CHUNK = 256 * 1000**2 # set max number of megabytes that will be read at a time
             self.dump_processes()
             if self.extract_dumps:
                 from varc_core.utils import dumpfile_extraction
                 dumpfile_extraction.extract_dumps(Path(self.output_path))
 
     def parse_mem_map(self, pid: int, p_name: str) -> List[Tuple[int, int]]:
         """Returns a list of (start address, end address) tuples of the regions of process memory that are mapped
@@ -103,17 +104,29 @@
                     if not maps:
                         continue
                     with NamedTemporaryFile(mode="w+b", buffering=0, delete=True) as tmpfile:
                         try:
                             for map in maps:
                                 page_start = map[0]
                                 page_len = map[1] - map[0]
-                                mem_page_content = self.read_bytes(pid, page_start, page_len)
-                                if mem_page_content:
-                                    tmpfile.write(mem_page_content)
+                                if page_len > self._MAX_VIRTUAL_PAGE_CHUNK:
+                                    sub_chunk_count, final_chunk_size = divmod(page_len, self._MAX_VIRTUAL_PAGE_CHUNK)
+                                    page_len = int(page_len / sub_chunk_count)
+                                    for sc in range(0, sub_chunk_count):
+                                        mem_page_content = self.read_bytes(pid, page_start, page_len)
+                                        if mem_page_content:
+                                            tmpfile.write(mem_page_content)
+                                        page_start = page_start + self._MAX_VIRTUAL_PAGE_CHUNK
+                                    mem_page_content = self.read_bytes(pid, page_start, final_chunk_size)
+                                    if mem_page_content:
+                                        tmpfile.write(mem_page_content)
+                                else:
+                                    mem_page_content = self.read_bytes(pid, page_start, page_len)
+                                    if mem_page_content:
+                                        tmpfile.write(mem_page_content)
                             zip_file.write(tmpfile.name, f"process_dumps{sep}{p_name}_{pid}.mem")
                         except PermissionError:
                             logging.warning(f"Permission denied opening process memory for {p_name} (pid {pid}). Cannot dump this process.")
                             continue
                         except OSError as oserror:
                             logging.warning(f"Error opening process memory page for {p_name} (pid {pid}). Error was {oserror}. Dump may be incomplete.")
                             pass
```

### Comparing `varc-1.0.6/varc_core/systems/windows.py` & `varc-1.0.7/varc_core/systems/windows.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc_core/utils/dumpfile_extraction.py` & `varc-1.0.7/varc_core/utils/dumpfile_extraction.py`

 * *Files identical despite different names*

### Comparing `varc-1.0.6/varc_core/utils/string_manips.py` & `varc-1.0.7/varc_core/utils/string_manips.py`

 * *Files identical despite different names*

