# Comparing `tmp/raga-cli-0.1.1.tar.gz` & `tmp/raga-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.1.tar", last modified: Tue Apr 25 11:10:39 2023, max compression
+gzip compressed data, was "raga-cli-0.1.2.tar", last modified: Tue Apr 25 11:58:15 2023, max compression
```

## Comparing `raga-cli-0.1.1.tar` & `raga-cli-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.442180 raga-cli-0.1.1/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.1/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.1/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:10:39.441867 raga-cli-0.1.1/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.1/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-25 11:10:25.000000 raga-cli-0.1.1/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.435337 raga-cli-0.1.1/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-25 11:10:39.000000 raga-cli-0.1.1/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.435948 raga-cli-0.1.1/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.437131 raga-cli-0.1.1/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3885 2023-04-25 10:56:12.000000 raga-cli-0.1.1/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.1/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.1/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9802 2023-04-25 07:39:29.000000 raga-cli-0.1.1/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.439324 raga-cli-0.1.1/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.1/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.1/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-25 09:40:57.000000 raga-cli-0.1.1/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.440265 raga-cli-0.1.1/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5180 2023-04-25 07:42:51.000000 raga-cli-0.1.1/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.440473 raga-cli-0.1.1/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:10:39.441505 raga-cli-0.1.1/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.1.1/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.1/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-25 11:10:39.442236 raga-cli-0.1.1/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.1/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.063135 raga-cli-0.1.2/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.2/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.2/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:58:15.062850 raga-cli-0.1.2/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.2/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-25 11:57:59.000000 raga-cli-0.1.2/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.057372 raga-cli-0.1.2/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.058019 raga-cli-0.1.2/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.059229 raga-cli-0.1.2/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.2/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.2/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.2/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9802 2023-04-25 07:39:29.000000 raga-cli-0.1.2/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.060395 raga-cli-0.1.2/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.2/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.2/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     7752 2023-04-25 11:55:43.000000 raga-cli-0.1.2/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.061226 raga-cli-0.1.2/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5180 2023-04-25 07:42:51.000000 raga-cli-0.1.2/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.061457 raga-cli-0.1.2/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.062495 raga-cli-0.1.2/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.1.2/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-25 11:58:15.063197 raga-cli-0.1.2/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.2/setup.py
```

### Comparing `raga-cli-0.1.1/.gitignore` & `raga-cli-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/LICENSE` & `raga-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/PKG-INFO` & `raga-cli-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.1/pyproject.toml` & `raga-cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.1.1/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.2/raga_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.1/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.2/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.2/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/cli/__init__.py` & `raga-cli-0.1.2/rc/cli/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import logging
 import os
 import subprocess
-from rc.cli.utils import get_repo, run_command_on_subprocess
-import tempfile
+from rc.cli.utils import get_repo
 from rc.utils.request import RctlValidRequestError, get_config_value_by_key, update_repo_lock
 from rc.utils import DEBUG
 logger = logging.getLogger(__name__)
 level = logging.INFO
 
 def log_setup(args = None):
     if DEBUG:
@@ -64,22 +63,15 @@
 
     # if not os.environ.get("MINIO_ACCESS_KEY_ID"):
     #     raise RctlValidReqError("Error: MINIO_ACCESS_KEY_ID not found. Please add MINIO_ACCESS_KEY_ID Environment Variable")
 
 def main(argv=None):
     repo = get_repo()
     try:
-         # Create a temporary directory and get the path to it
-        temp_dir = tempfile.gettempdir()
-        # Create the path for the token.txt file inside the temp directory
-        token_file = temp_dir + '/token.txt'
-        # Open the file for writing
-        with open(token_file, 'w') as f:
-            f.write(get_config_value_by_key('gh_token'))
-        run_command_on_subprocess(f"gh auth login --with-token < {token_file}")
+        os.environ['GH_TOKEN'] = get_config_value_by_key('gh_token')
         valid_requirement()
         args = parse_args(argv)
         cmd = args.func(args)
         cmd.do_run()
     except KeyboardInterrupt as exc:
         logger.exception(exc)
         # update_repo_lock(repo, json.dumps({"locked":False}))
```

### Comparing `raga-cli-0.1.1/rc/cli/parser.py` & `raga-cli-0.1.2/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/cli/utils.py` & `raga-cli-0.1.2/rc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/commands/get.py` & `raga-cli-0.1.2/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/commands/list.py` & `raga-cli-0.1.2/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/commands/put.py` & `raga-cli-0.1.2/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/commands/repo.py` & `raga-cli-0.1.2/rc/commands/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         print("Repository has been created. `cd {}`".format(repository_name))    
         logger.debug(f"END CREATE REPO COMMAND")
 
     def clone_repo(self, args):
         start = timer()
         repository_name = args.name     
         print('Cloning...')
-        run_command_on_subprocess("gh repo clone {0}/{1}".format(self.GIT_ORG, repository_name), None, True)    
+        run_command_on_subprocess("git clone git@github.com:{0}/{1}.git".format(self.GIT_ORG, repository_name), None, True)    
         tag = get_repository(repository_name)
         if tag == "dataset":
             run_command_on_subprocess("dvc pull", repository_name, True) 
         print("Repository cloned successfully")
         end = timer()
         logger.debug('CLONE TIME {0}'.format(timedelta(seconds=end-start)))
```

### Comparing `raga-cli-0.1.1/rc/exceptions.py` & `raga-cli-0.1.2/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/prompt.py` & `raga-cli-0.1.2/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/repo/get.py` & `raga-cli-0.1.2/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/repo/put.py` & `raga-cli-0.1.2/rc/repo/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/utils/__init__.py` & `raga-cli-0.1.2/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/utils/request.py` & `raga-cli-0.1.2/rc/utils/request.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.1/rc/utils/sshKeyGen.py` & `raga-cli-0.1.2/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

