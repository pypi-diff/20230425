# Comparing `tmp/eotdl_cli-0.0.6.tar.gz` & `tmp/eotdl_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl_cli-0.0.6.tar", max compression
+gzip compressed data, was "eotdl_cli-0.0.7.tar", max compression
```

## Comparing `eotdl_cli-0.0.6.tar` & `eotdl_cli-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.6/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.6/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      940 2023-04-18 13:03:59.183525 eotdl_cli-0.0.6/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1175 2023-04-18 13:04:05.455544 eotdl_cli-0.0.6/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      312 2023-04-18 13:03:47.587490 eotdl_cli-0.0.6/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.6/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.6/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.6/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     2132 2023-04-18 14:38:06.636513 eotdl_cli-0.0.6/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.6/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.6/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.6/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      573 2023-04-18 14:43:48.589541 eotdl_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 eotdl_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.7/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-25 09:43:24.394687 eotdl_cli-0.0.7/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1184 2023-04-25 09:43:34.326720 eotdl_cli-0.0.7/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      480 2023-04-25 09:41:49.358365 eotdl_cli-0.0.7/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2527 2023-04-25 09:32:20.840458 eotdl_cli-0.0.7/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      573 2023-04-25 09:44:06.534826 eotdl_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 eotdl_cli-0.0.7/PKG-INFO
```

### Comparing `eotdl_cli-0.0.6/eotdl_cli/commands/auth.py` & `eotdl_cli-0.0.7/eotdl_cli/commands/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-from eotdl_cli.src.usecases.auth import is_logged, auth, generate_logout_url
-from eotdl_cli.src.errors.auth import LoginError
+from src.usecases.auth import is_logged, auth, generate_logout_url
+from src.errors.auth import LoginError
 
 app = typer.Typer()
 
 @app.command()
 def login():
     """
     Login to your account
```

### Comparing `eotdl_cli-0.0.6/eotdl_cli/commands/datasets.py` & `eotdl_cli-0.0.7/eotdl_cli/commands/datasets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-from eotdl_cli.src.usecases.datasets import retrieve_datasets, download_dataset, ingest_dataset
-from eotdl_cli.src.usecases.auth import auth
+from src.usecases.datasets import retrieve_datasets, download_dataset, ingest_dataset
+from src.usecases.auth import auth
 
 app = typer.Typer()
 
 @app.command()
 def list():
     """
     List all datasets
@@ -12,38 +12,38 @@
     datasets = retrieve_datasets()
     typer.echo(datasets)
 
 @app.command()
 def get(name: str, path: str = None):
     """
     Download a dataset
-    
+
     name: Name of the dataset
     path: Path to download the dataset to
     """
     try:
         user = auth()
         dst_path = download_dataset(name, path, user)
         typer.echo(f"Dataset {name} downloaded to {dst_path}")
     except Exception as e:
         typer.echo(e)
 
 @app.command()
 def ingest(path: str):
     """
     Ingest a dataset
-    
+
     path: Path to dataset to ingest
     """
     try:
         user = auth()
-        name = typer.prompt("Dataset name")
-        description = typer.prompt("Description")
-        # confirm 
-        typer.confirm(f"Is the data correct?", abort=True)
+        name = 'asasdasdas' #typer.prompt("Dataset name")
+        description = 'asdjklhfgalskdjghf' #typer.prompt("Description")
+        # confirm
+        # typer.confirm(f"Is the data correct?", abort=True)
         ingest_dataset(name, description, path, user)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/repos/APIRepo.py` & `eotdl_cli-0.0.7/eotdl_cli/src/repos/APIRepo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import requests
 from tqdm import tqdm
 from pathlib import Path
 import os 
+import httpx
+import time
 
 class APIRepo():
-    # def __init__(self, url='http://localhost:8000/'):
-    def __init__(self, url='https://api.eotdl.com/'):
+    def __init__(self, url='http://localhost:8000/'):
+    # def __init__(self, url='https://api.eotdl.com/'):
         self.url = url
 
     def login(self):
         return requests.get(self.url + 'auth/login')
     
     def token(self, code):
         return requests.get(self.url + 'auth/token?code=' + code)
@@ -43,12 +45,20 @@
                     f.write(chunk)
             progress_bar.close()
             return path
         
     def ingest_dataset(self, name, description, path, id_token):
         # Not sure this will work with large datasets, need to test
         url = self.url + 'datasets'
-        headers={'Authorization': 'Bearer ' + id_token}
+        # headers={'Authorization': 'Bearer ' + id_token}
+        headers={'Filename': 'bigFile.zip'}
         files = {'file': open(path, 'rb')}
-        data = {'name': name, 'description': description}
-        response = requests.post(url, headers=headers, files=files, data=data)
-        return response
+        # data = {'name': name, 'description': description}
+        data = {'data': 'Hello World!'}
+        # response = requests.post(url, headers=headers, files=files, data=data)
+        with httpx.Client() as client:
+            start = time.time()
+            r = client.post(url, data=data, files=files, headers=headers)
+            end = time.time()
+            print(f'Time elapsed: {end - start}s')
+            print(r.status_code, r.json(), sep=' ')
+        # return response
```

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/repos/AuthRepo.py` & `eotdl_cli-0.0.7/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/usecases/auth/main.py` & `eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.6/eotdl_cli/src/usecases/datasets/main.py` & `eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.6/pyproject.toml` & `eotdl_cli-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl_cli-0.0.6/PKG-INFO` & `eotdl_cli-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

