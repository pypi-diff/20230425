# Comparing `tmp/raga-cli-0.0.9.tar.gz` & `tmp/raga-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.0.9.tar", last modified: Sat Apr 22 07:21:52 2023, max compression
+gzip compressed data, was "raga-cli-0.1.0.tar", last modified: Tue Apr 25 07:45:06 2023, max compression
```

## Comparing `raga-cli-0.0.9.tar` & `raga-cli-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.972719 raga-cli-0.0.9/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.9/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.9/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-22 07:21:52.972425 raga-cli-0.0.9/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.9/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-22 07:21:43.000000 raga-cli-0.0.9/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.967714 raga-cli-0.0.9/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-22 07:21:52.000000 raga-cli-0.0.9/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.968472 raga-cli-0.0.9/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.969313 raga-cli-0.0.9/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.9/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.9/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9621 2023-04-22 06:59:03.000000 raga-cli-0.0.9/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.970245 raga-cli-0.0.9/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.9/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.9/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.9/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.970942 raga-cli-0.0.9/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-22 07:01:22.000000 raga-cli-0.0.9/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.971106 raga-cli-0.0.9/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:21:52.972056 raga-cli-0.0.9/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.9/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.9/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-22 07:21:52.972781 raga-cli-0.0.9/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.9/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.682913 raga-cli-0.1.0/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.0/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.0/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 07:45:06.682553 raga-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.0/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-25 07:44:00.000000 raga-cli-0.1.0/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.676712 raga-cli-0.1.0/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-25 07:45:06.000000 raga-cli-0.1.0/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.677361 raga-cli-0.1.0/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.678530 raga-cli-0.1.0/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.0/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.0/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9802 2023-04-25 07:39:29.000000 raga-cli-0.1.0/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.679654 raga-cli-0.1.0/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.0/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.0/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.1.0/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.680908 raga-cli-0.1.0/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5180 2023-04-25 07:42:51.000000 raga-cli-0.1.0/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.681098 raga-cli-0.1.0/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 07:45:06.682173 raga-cli-0.1.0/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.1.0/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.0/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-25 07:45:06.682987 raga-cli-0.1.0/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.0/setup.py
```

### Comparing `raga-cli-0.0.9/.gitignore` & `raga-cli-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/LICENSE` & `raga-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/PKG-INFO` & `raga-cli-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.9/pyproject.toml` & `raga-cli-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.0.9"
+version = "0.1.0"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.0.9/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.0/raga_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.9/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.0/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.0/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/cli/__init__.py` & `raga-cli-0.1.0/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/cli/parser.py` & `raga-cli-0.1.0/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/cli/utils.py` & `raga-cli-0.1.0/rc/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,19 @@
     for path in paths:
         if not compare_dot_dvc_file(path):
             return current_version+1
         if get_dvc_data_status(path):
             return current_version+1
     return 1 if not current_version else current_version
 
+
+def model_current_version(repo):
+    current_version = 0 if not get_repo_version(repo) else int(get_repo_version(repo))
+    return 1 if not current_version else current_version+1
+
 def server_repo_commit_status(ids):
     elastic_processes = []
     for id in ids:
         elastic_processes.append(get_commit_repo(id)['check_elastic_process'])
     logger.debug("ELASTIC PROCESS {}".format(elastic_processes))
     return all(elastic_processes)
```

### Comparing `raga-cli-0.0.9/rc/commands/get.py` & `raga-cli-0.1.0/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/commands/list.py` & `raga-cli-0.1.0/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/commands/put.py` & `raga-cli-0.1.0/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/commands/repo.py` & `raga-cli-0.1.0/rc/commands/repo.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/exceptions.py` & `raga-cli-0.1.0/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/prompt.py` & `raga-cli-0.1.0/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/repo/get.py` & `raga-cli-0.1.0/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/repo/put.py` & `raga-cli-0.1.0/rc/repo/put.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,25 @@
     stop_checking_elastic_process = False
     while not stop_checking_elastic_process:
         stop_checking_elastic_process = server_repo_commit_status(repo_commit_ids)
         if not stop_checking_elastic_process:
             time.sleep(pool_time)
     return True
 
-def model_upload(message, repo):
+def model_upload(message, repo, model_version):
     update_repo_lock(repo, json.dumps({"locked":True}))
     print("Model files uploading...")
     branchName = current_branch()
     commit_hash = current_commit_hash()
     branchName = current_branch()
     request_payload = {
                 "commit_message" : message,
                 "repo" : repo,
                 "commit_id":commit_hash,
+                "version":model_version,
                 "branch":branchName
             }  
     upload_model_file_list_json(commit_hash)
     insert_repo_commit(json.dumps(request_payload))
     logger.debug("Data upload for branch {0} and {1} ".format(branchName,commit_hash ))
     print("Model files uploaded successfully")
 
@@ -99,24 +100,25 @@
         sys.exit()
     print("Files uploaded successfully")
 
 def put(args):
     start = timer()
     message = args.message      
     paths = args.path   
-    repo = get_repo()       
-    current_version = dataset_current_version(paths, repo)
+    repo = get_repo()     
+    
     # print("VERSION", current_version)
     # print("CHECK ELASTIC PROCESS", server_repo_commit_status(repo_commit_ids))
     # return
 
     tag = get_repository(repo)
     is_repo_lock(repo)
     
     if tag == "dataset":
+        current_version = dataset_current_version(paths, repo)
         # Create an Event object
         stop_event = threading.Event()
         # Create a thread for making an HTTP request
         http_thread = threading.Thread(target=make_repo_lock, args=(stop_event,))
         http_thread.start() 
         try:
             if dataset_upload(paths,message,repo, current_version):
@@ -133,11 +135,12 @@
         # Start both threads
         
         # Wait for both threads to finish
         http_thread.join()
         make_repo_commit(message)
         
     elif tag == "model":
-        model_upload(message, repo)
+        model_version = model_current_version(repo)
+        model_upload(message, repo, model_version)
         
     update_repo_lock(repo, json.dumps({"locked":False}))
     logger.debug('TOTAL UPLOAD TIME {0}'.format(timedelta(seconds=timer()-start)))
```

### Comparing `raga-cli-0.0.9/rc/utils/__init__.py` & `raga-cli-0.1.0/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/utils/request.py` & `raga-cli-0.1.0/rc/utils/request.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.9/rc/utils/sshKeyGen.py` & `raga-cli-0.1.0/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

