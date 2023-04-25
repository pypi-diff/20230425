# Comparing `tmp/aipha_geo_solutions-0.1.7.tar.gz` & `tmp/aipha_geo_solutions-0.1.8.tar.gz`

## Comparing `aipha_geo_solutions-0.1.7.tar` & `aipha_geo_solutions-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.1.7/example.py` & `aipha_geo_solutions-0.1.8/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/operators.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/webservice_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,18 @@
         username,
         password,
         server_address,
         verifySSL
     )
     services_dict = json.loads(running_services['running_processes'])
     for service_id in services:
-      this_complete = False
+      this_complete = True #ignore services that have been deleted
       for running_service in services_dict:
         if service_id.startswith(running_service['ID']):
+          this_complete = False
           if '1/1 completed' in running_service['Replicas']:
               this_complete = True
               break
       if this_complete == False:
           return False
     return True
   except:
```

### Comparing `aipha_geo_solutions-0.1.7/LICENSE` & `aipha_geo_solutions-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.7/pyproject.toml` & `aipha_geo_solutions-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.1.7/PKG-INFO` & `aipha_geo_solutions-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

