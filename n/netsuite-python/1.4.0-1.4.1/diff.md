# Comparing `tmp/netsuite_python-1.4.0.tar.gz` & `tmp/netsuite_python-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.4.0.tar", last modified: Mon Apr 17 18:32:26 2023, max compression
+gzip compressed data, was "netsuite_python-1.4.1.tar", last modified: Mon Apr 24 23:55:43 2023, max compression
```

## Comparing `netsuite_python-1.4.0.tar` & `netsuite_python-1.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/
--rw-rw-rw-   0        0        0    12699 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.278992 netsuite_python-1.4.0/netsuite/
--rw-rw-rw-   0        0        0    13726 2023-04-17 18:30:10.000000 netsuite_python-1.4.0/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.286775 netsuite_python-1.4.0/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.4.0/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.291774 netsuite_python-1.4.0/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.4.0/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.4.0/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.4.0/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.4.0/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.4.0/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.4.0/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.293778 netsuite_python-1.4.0/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     8422 2023-04-12 21:53:28.000000 netsuite_python-1.4.0/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.4.0/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.300775 netsuite_python-1.4.0/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.305775 netsuite_python-1.4.0/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    12699 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-04-17 18:32:00.000000 netsuite_python-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.734810 netsuite_python-1.4.1/
+-rw-rw-rw-   0        0        0    12699 2023-04-24 23:55:43.734810 netsuite_python-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.705811 netsuite_python-1.4.1/netsuite/
+-rw-rw-rw-   0        0        0    14525 2023-04-24 23:53:55.000000 netsuite_python-1.4.1/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.713810 netsuite_python-1.4.1/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.4.1/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.718809 netsuite_python-1.4.1/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.4.1/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.4.1/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.4.1/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.4.1/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.4.1/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.4.1/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.721809 netsuite_python-1.4.1/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     9979 2023-04-24 23:54:13.000000 netsuite_python-1.4.1/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.4.1/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.727811 netsuite_python-1.4.1/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.4.1/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:55:43.732811 netsuite_python-1.4.1/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    12699 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 23:55:43.000000 netsuite_python-1.4.1/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 23:55:43.734810 netsuite_python-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-04-24 23:54:41.000000 netsuite_python-1.4.1/setup.py
```

### Comparing `netsuite_python-1.4.0/PKG-INFO` & `netsuite_python-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.4.0/README.md` & `netsuite_python-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/Netsuite.py` & `netsuite_python-1.4.1/netsuite/Netsuite.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,24 +167,37 @@
         token = NetsuiteToken(**response.json())
         self.save_token(token)
         # if token.access_token is not None:
         #     self.get_customer_categories()
         #     self.get_status_dict()
         return self.token
 
-    def generate_rest_client(self):
+    def get_netsuite_recordtypes(self):
+        url = f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1/metadata-catalog"
+        token = self.storage.get_token(self.app_name)
+        headers = {
+            'Authorization': f'Bearer {token.access_token}'
+        }
+        response = requests.get(url, headers=headers)
+        records = []
+        for item in response.json().get('items'):
+            records.append(item.get("name"))
+        return records
+
+    def generate_rest_client(self, record_types=None):
+
         # from urllib.request import urlopen
         # from tempfile import NamedTemporaryFile
         # from shutil import unpack_archive
         import zipfile, shutil
         from io import BytesIO
         token = self.storage.get_token(self.app_name)
         url = f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1/metadata-catalog"
         params = {
-            'select': 'customer'
+            'select': record_types
         }
         headers = {
             'Accept': 'application/swagger+json',
             'Authorization': f'Bearer {token.access_token}'
         }
         response = requests.get(url, headers=headers, params=params)
         # print(token.access_token)
@@ -223,15 +236,15 @@
 
         shutil.copytree(client_src, dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
                         dirs_exist_ok=True)
 
         shutil.copy(class_src, dst)
 
         print('Netsuite Rest Client Created')
-        shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
+        # shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
         print('temp folder removed.')
 
         print('\n Netsuite is Ready To Go!')
         print('Usage Example')
         print('\n ----------------------')
         print('\nfrom netsuite import Netsuite'
               '\nfrom netsuite_rest_client import apis, rest_api_client'
@@ -292,14 +305,17 @@
             self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
             self.configuration.token_refresh_hook = self.refresh_token
             self.configuration.app_name = netsuite.netsuite_app_name
             self.configuration.host = f"https://{self.configuration.app_name}.restlets.api.netsuite.com/app/site/hosting/restlet.nl"
             self.api_client = api_clients.ApiClient(configuration=self.configuration)
             self.restlet_api = api_clients.RestletApi(api_client=self.api_client)
 
+            # self.contact_api = swagger_client.ContactApi(api_client=self.api_client)
+            # self.customer_api = swagger_client.CustomerApi(api_client=self.api_client)
+            # self.message_api = swagger_client.MessageApi(api_client=self.api_client)
 
         def refresh_token(self):
             self.configuration.token = self.netsuite.get_token()
             return self.configuration.token
 
     # def get_status_dict(self):
     #     if self.token.access_token is None:
```

### Comparing `netsuite_python-1.4.0/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.4.1/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.4.1/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/api_clients/api_client.py` & `netsuite_python-1.4.1/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/api_clients/configuration.py` & `netsuite_python-1.4.1/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/api_clients/rest.py` & `netsuite_python-1.4.1/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/module_loading.py` & `netsuite_python-1.4.1/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/scripts/cli.py` & `netsuite_python-1.4.1/netsuite/scripts/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,15 +174,53 @@
         click.echo(creds)
 
     return creds
 
 @cli.command()
 def generate_rest_client():
     netsuite = Netsuite()
-    netsuite.generate_rest_client()
+    display_ns_classes = prompt("Do you need to know which records are available?", type=click.BOOL, default=True)
+    records = netsuite.get_netsuite_recordtypes()
+    if display_ns_classes:
+        display_custom = prompt("Display Custom records (probably not)?", type=click.BOOL, default=False)
+        print("RECORDS")
+        print("-----------------")
+
+        for record in records:
+            if display_custom:
+                print(record)
+            else:
+                if "customrecord" not in record and "customlist" not in record:
+                    print(record)
+    records_added = True
+    ns_records_to_include = ["customer"]
+    while records_added:
+        next_record = prompt("Which records do you need?")
+        if next_record not in records:
+            print("That record is not available.")
+        elif next_record in ns_records_to_include:
+            print("record already included.")
+        else:
+            ns_records_to_include.append(next_record)
+        records_added = prompt("Add another?", type=click.BOOL, default=True)
+
+    record_str = ''
+    index = 0
+    for record in ns_records_to_include:
+        if index > 0:
+            record_str += f',{record}'
+        else:
+            record_str += f'{record}'
+        index += 1
+
+
+    # ns_records_to_include = prompt("Which records will you be using (comma separated list, no spaces)", type=click.STRING, default="customer")
+        # print(netsuite.get_netsuite_recordtypes())
+    print(record_str)
+    netsuite.generate_rest_client(record_types=record_str)
 
 @cli.command()
 @click.option('--credentials-file', '--f', type=click.File('r'), default=api_settings.CREDENTIALS_PATH,
               prompt="Path to Credentials File")
 @click.pass_context
 def get_access_token(ctx, credentials_file):
     """OAuth flow for Netsuite to obtain an access and refresh token"""
```

### Comparing `netsuite_python-1.4.0/netsuite/settings.py` & `netsuite_python-1.4.1/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.4.1/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite/storages/JSONStorage.py` & `netsuite_python-1.4.1/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.4.1/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.4.0/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.4.1/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.4.0/setup.py` & `netsuite_python-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.4.0',
+    version='1.4.1',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

