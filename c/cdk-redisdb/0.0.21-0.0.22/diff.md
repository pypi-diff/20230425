# Comparing `tmp/cdk-redisdb-0.0.21.tar.gz` & `tmp/cdk-redisdb-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.21.tar", last modified: Sun Apr 23 12:33:59 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.22.tar", last modified: Tue Apr 25 04:42:41 2023, max compression
```

## Comparing `cdk-redisdb-0.0.21.tar` & `cdk-redisdb-0.0.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:33:59.228050 cdk-redisdb-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48022 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.21.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:33:40.000000 cdk-redisdb-0.0.21/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:33:59.232050 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-23 12:33:59.000000 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-23 12:33:59.000000 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:33:59.000000 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 12:33:59.000000 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 12:33:59.000000 cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.349387 cdk-redisdb-0.0.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25933 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.22.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.21/LICENSE` & `cdk-redisdb-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.21/PKG-INFO` & `cdk-redisdb-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.21
+Version: 0.0.22
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.21/README.md` & `cdk-redisdb-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.21/setup.py` & `cdk-redisdb-0.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.21",
+    "version": "0.0.22",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.21.jsii.tgz"
+            "cdk-redisdb@0.0.22.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-redisdb-0.0.21/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.22/src/cdk_redisdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,19 @@
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> _aws_cdk_aws_memorydb_ceddda9d.CfnCluster:
         return typing.cast(_aws_cdk_aws_memorydb_ceddda9d.CfnCluster, jsii.get(self, "cluster"))
 
+    @builtins.property
+    @jsii.member(jsii_name="vpc")
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
+
 
 class RedisDB(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-redisdb.RedisDB",
 ):
     def __init__(
@@ -338,14 +343,19 @@
     @builtins.property
     @jsii.member(jsii_name="replicationGroup")
     def replication_group(
         self,
     ) -> _aws_cdk_aws_elasticache_ceddda9d.CfnReplicationGroup:
         return typing.cast(_aws_cdk_aws_elasticache_ceddda9d.CfnReplicationGroup, jsii.get(self, "replicationGroup"))
 
+    @builtins.property
+    @jsii.member(jsii_name="vpc")
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
+
 
 @jsii.data_type(
     jsii_type="cdk-redisdb.RedisDBProps",
     jsii_struct_bases=[_aws_cdk_ceddda9d.StackProps],
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
```

### Comparing `cdk-redisdb-0.0.21/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.21
+Version: 0.0.22
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

