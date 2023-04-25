# Comparing `tmp/nacos-client-py-0.0.8.tar.gz` & `tmp/nacos-client-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacos-client-py-0.0.8.tar", last modified: Tue Aug  9 06:27:00 2022, max compression
+gzip compressed data, was "nacos-client-py-0.0.9.tar", last modified: Mon Aug 29 08:32:07 2022, max compression
```

## Comparing `nacos-client-py-0.0.8.tar` & `nacos-client-py-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-09 06:27:00.555185 nacos-client-py-0.0.8/
--rw-r--r--   0 rencanwei   (501) staff       (20)    11356 2022-05-24 12:45:53.000000 nacos-client-py-0.0.8/LICENSE
--rw-r--r--   0 rencanwei   (501) staff       (20)     1962 2022-08-09 06:27:00.555039 nacos-client-py-0.0.8/PKG-INFO
--rw-r--r--   0 rencanwei   (501) staff       (20)     1321 2022-08-08 12:13:51.000000 nacos-client-py-0.0.8/README.md
-drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-09 06:27:00.554164 nacos-client-py-0.0.8/nacos_client/
--rw-r--r--   0 rencanwei   (501) staff       (20)       46 2022-05-25 04:22:53.000000 nacos-client-py-0.0.8/nacos_client/__init__.py
--rw-r--r--   0 rencanwei   (501) staff       (20)     4302 2022-08-09 06:26:11.000000 nacos-client-py-0.0.8/nacos_client/client.py
-drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-09 06:27:00.554832 nacos-client-py-0.0.8/nacos_client_py.egg-info/
--rw-r--r--   0 rencanwei   (501) staff       (20)     1962 2022-08-09 06:27:00.000000 nacos-client-py-0.0.8/nacos_client_py.egg-info/PKG-INFO
--rw-r--r--   0 rencanwei   (501) staff       (20)      268 2022-08-09 06:27:00.000000 nacos-client-py-0.0.8/nacos_client_py.egg-info/SOURCES.txt
--rw-r--r--   0 rencanwei   (501) staff       (20)        1 2022-08-09 06:27:00.000000 nacos-client-py-0.0.8/nacos_client_py.egg-info/dependency_links.txt
--rw-r--r--   0 rencanwei   (501) staff       (20)       41 2022-08-09 06:27:00.000000 nacos-client-py-0.0.8/nacos_client_py.egg-info/requires.txt
--rw-r--r--   0 rencanwei   (501) staff       (20)       13 2022-08-09 06:27:00.000000 nacos-client-py-0.0.8/nacos_client_py.egg-info/top_level.txt
--rw-r--r--   0 rencanwei   (501) staff       (20)       38 2022-08-09 06:27:00.555231 nacos-client-py-0.0.8/setup.cfg
--rw-r--r--   0 rencanwei   (501) staff       (20)     2129 2022-08-09 06:26:23.000000 nacos-client-py-0.0.8/setup.py
+drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-29 08:32:07.472646 nacos-client-py-0.0.9/
+-rw-r--r--   0 rencanwei   (501) staff       (20)    11356 2022-05-24 12:45:53.000000 nacos-client-py-0.0.9/LICENSE
+-rw-r--r--   0 rencanwei   (501) staff       (20)     1962 2022-08-29 08:32:07.472516 nacos-client-py-0.0.9/PKG-INFO
+-rw-r--r--   0 rencanwei   (501) staff       (20)     1321 2022-08-08 12:13:51.000000 nacos-client-py-0.0.9/README.md
+drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-29 08:32:07.471445 nacos-client-py-0.0.9/nacos_client/
+-rw-r--r--   0 rencanwei   (501) staff       (20)       46 2022-05-25 04:22:53.000000 nacos-client-py-0.0.9/nacos_client/__init__.py
+-rw-r--r--   0 rencanwei   (501) staff       (20)     4640 2022-08-29 08:30:05.000000 nacos-client-py-0.0.9/nacos_client/client.py
+drwxr-xr-x   0 rencanwei   (501) staff       (20)        0 2022-08-29 08:32:07.472353 nacos-client-py-0.0.9/nacos_client_py.egg-info/
+-rw-r--r--   0 rencanwei   (501) staff       (20)     1962 2022-08-29 08:32:07.000000 nacos-client-py-0.0.9/nacos_client_py.egg-info/PKG-INFO
+-rw-r--r--   0 rencanwei   (501) staff       (20)      268 2022-08-29 08:32:07.000000 nacos-client-py-0.0.9/nacos_client_py.egg-info/SOURCES.txt
+-rw-r--r--   0 rencanwei   (501) staff       (20)        1 2022-08-29 08:32:07.000000 nacos-client-py-0.0.9/nacos_client_py.egg-info/dependency_links.txt
+-rw-r--r--   0 rencanwei   (501) staff       (20)       41 2022-08-29 08:32:07.000000 nacos-client-py-0.0.9/nacos_client_py.egg-info/requires.txt
+-rw-r--r--   0 rencanwei   (501) staff       (20)       13 2022-08-29 08:32:07.000000 nacos-client-py-0.0.9/nacos_client_py.egg-info/top_level.txt
+-rw-r--r--   0 rencanwei   (501) staff       (20)       38 2022-08-29 08:32:07.472685 nacos-client-py-0.0.9/setup.cfg
+-rw-r--r--   0 rencanwei   (501) staff       (20)     2129 2022-08-29 08:30:51.000000 nacos-client-py-0.0.9/setup.py
```

### Comparing `nacos-client-py-0.0.8/LICENSE` & `nacos-client-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nacos-client-py-0.0.8/PKG-INFO` & `nacos-client-py-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacos-client-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for Nacos
 Home-page: UNKNOWN
 Author: rencanwei
 Author-email: rencanwei@58.com
 License: Apache License 2.0
 Keywords: nacos-client-py
 Platform: UNKNOWN
```

### Comparing `nacos-client-py-0.0.8/README.md` & `nacos-client-py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nacos-client-py-0.0.8/nacos_client/client.py` & `nacos-client-py-0.0.9/nacos_client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,46 +43,51 @@
 
     def __init__(self, server_addresses, namespace=None, username=None, password=None):
         self.server_address = server_addresses
         self.namespace = namespace
         self.client = nacos.NacosClient(server_addresses, namespace=namespace, username=username, password=password)
         self.service_dict = {}
 
-    def register(self, service_name, ip, port, cluster_name='DEFAULT', weight=1, metadata=None):
+    def register(self, service_name, ip, port, cluster_name='DEFAULT', group_name='public', weight=1, metadata=None):
         cluster, group = os.environ.get('WCloud_Cluster'), os.environ.get('WCloud_Cluster_Group')
         if cluster and group:
             cluster_name = f'{cluster}__{group}'
         if metadata is None:
             metadata = {}
-        logger.info("[register] service_name:%s, ip:%s, port:%s, cluster_name:%s, weight:%s" % (
-            service_name, ip, port, cluster_name, weight))
+        logger.info("[register] service_name:%s, ip:%s, port:%s, cluster_name:%s, group_name:%s, weight:%s" % (
+            service_name, ip, port, cluster_name, group_name, weight))
         try:
-            re = self.client.add_naming_instance(service_name, ip, port, cluster_name=cluster_name, weight=weight, metadata=metadata)
+            re = self.client.add_naming_instance(
+                service_name, ip, port, cluster_name=cluster_name, group_name=group_name, weight=weight, metadata=metadata)
             logger.info(f"[register] success! {re}")
-            thread = threading.Thread(target=self.health_check, args=(service_name, ip, port, cluster_name, weight, metadata))
+            thread = threading.Thread(target=self.health_check, args=(
+                service_name, ip, port, cluster_name, group_name, weight, metadata, ))
             thread.start()
         except:
             logging.error("[regiser] failed!", exc_info=True)
 
-    def health_check(self, service_name, ip, port, cluster_name, weight, metadata):
-        logger.info("[health_check] service_name:%s, ip:%s, port:%s, cluster_name:%s, weight:%s" % (
-            service_name, ip, port, cluster_name, weight))
+    def health_check(self, service_name, ip, port, cluster_name, group_name, weight, metadata):
+        logger.info("[health_check] service_name:%s, ip:%s, port:%s, cluster_name:%s, group_name:%s, weight:%s" % (
+            service_name, ip, port, cluster_name, group_name, weight))
         while True:
             time.sleep(3)
             try:
-                result = self.client.send_heartbeat(service_name, ip, port, cluster_name, weight, metadata=metadata)
+                result = self.client.send_heartbeat(
+                    f'{group_name}@@{service_name}', ip, port, cluster_name=cluster_name, weight=weight, group_name=group_name, metadata=metadata)
                 if result.get('code') != 10200:
                     logger.info(f'[send_heartbeat] failed! register again')
-                    self.register(service_name, ip, port, cluster_name, weight)
+                    self.register(service_name, ip, port, cluster_name=cluster_name,
+                                  group_name=group_name, weight=weight)
                     break
             except:
                 logging.error("[send_heartbeat] error!", exc_info=True)
 
     def get_service_host(self, service_name, clusters=None, group_name=None):
-        logger.info("[get_service_host] service_name:%s, clusters:%s, group_name:%s" % (service_name, clusters, group_name))
+        logger.info("[get_service_host] service_name:%s, clusters:%s, group_name:%s" %
+                    (service_name, clusters, group_name))
         if not self.service_dict.get(service_name):
             config_dic = self.client.list_naming_instance(
                 service_name, clusters, namespace_id=self.namespace, group_name=group_name, healthy_only=True)
             hosts = config_dic.get("hosts")
             if not hosts:
                 logger.error(f'[get_service_host] no service avaliable! service: {service_name}')
                 return None
```

### Comparing `nacos-client-py-0.0.8/nacos_client_py.egg-info/PKG-INFO` & `nacos-client-py-0.0.9/nacos_client_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacos-client-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for Nacos
 Home-page: UNKNOWN
 Author: rencanwei
 Author-email: rencanwei@58.com
 License: Apache License 2.0
 Keywords: nacos-client-py
 Platform: UNKNOWN
```

### Comparing `nacos-client-py-0.0.8/setup.py` & `nacos-client-py-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         os.system('twine upload dist/*')
 
         sys.exit()
 
 
 setup(
     name="nacos-client-py",
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(
         exclude=["test", "*.tests", "*.tests.*", "tests.*", "tests"]),
     license="Apache License 2.0",
     python_requires='>=3.6',
     classifiers=[
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Operating System :: OS Independent",
```

