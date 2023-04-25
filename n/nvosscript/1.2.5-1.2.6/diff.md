# Comparing `tmp/nvosscript-1.2.5.tar.gz` & `tmp/nvosscript-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.5.tar", last modified: Wed Apr 12 10:01:23 2023, max compression
+gzip compressed data, was "nvosscript-1.2.6.tar", last modified: Tue Apr 25 07:46:16 2023, max compression
```

## Comparing `nvosscript-1.2.5.tar` & `nvosscript-1.2.6.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 10:01:23.205567 nvosscript-1.2.5/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.5/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 10:01:23.205426 nvosscript-1.2.5/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.5/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 10:01:23.203494 nvosscript-1.2.5/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.5/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.5/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.5/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8071 2023-04-12 09:32:00.000000 nvosscript-1.2.5/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4612 2023-04-12 02:02:57.000000 nvosscript-1.2.5/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      903 2023-04-12 01:53:07.000000 nvosscript-1.2.5/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 10:01:23.204546 nvosscript-1.2.5/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 10:01:23.000000 nvosscript-1.2.5/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 10:01:23.205613 nvosscript-1.2.5/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-12 09:59:27.000000 nvosscript-1.2.5/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 10:01:23.204792 nvosscript-1.2.5/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.5/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 09:59:37.000000 nvosscript-1.2.5/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 10:01:23.205104 nvosscript-1.2.5/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.5/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.980406 nvosscript-1.2.6/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.6/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-25 07:46:16.980255 nvosscript-1.2.6/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.6/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.977045 nvosscript-1.2.6/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.6/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    13019 2023-04-25 03:18:40.000000 nvosscript-1.2.6/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-24 10:46:35.000000 nvosscript-1.2.6/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8571 2023-04-25 06:40:19.000000 nvosscript-1.2.6/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4796 2023-04-24 10:50:50.000000 nvosscript-1.2.6/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      985 2023-04-25 03:15:56.000000 nvosscript-1.2.6/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.978072 nvosscript-1.2.6/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      474 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-04-25 07:46:16.000000 nvosscript-1.2.6/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-25 07:46:16.980650 nvosscript-1.2.6/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-25 07:45:26.000000 nvosscript-1.2.6/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.978826 nvosscript-1.2.6/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.2.6/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      712 2023-04-25 06:34:28.000000 nvosscript-1.2.6/skyeye/datahandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1797 2023-04-25 03:19:08.000000 nvosscript-1.2.6/skyeye/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      240 2023-04-24 10:14:48.000000 nvosscript-1.2.6/skyeye/skyeyecommand.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.979564 nvosscript-1.2.6/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.6/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      185 2023-04-25 03:16:06.000000 nvosscript-1.2.6/start/commonUtil.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4529 2023-04-25 07:45:36.000000 nvosscript-1.2.6/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-25 07:46:16.979828 nvosscript-1.2.6/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1273 2023-04-24 10:15:28.000000 nvosscript-1.2.6/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.5/LICENSE` & `nvosscript-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.5/nvos/file.py` & `nvosscript-1.2.6/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import subprocess
 import logging
 import json
-from nvos import remote
+from nvos import remote, utils
+from start import commonUtil
 
 logger = logging.getLogger(__name__)
 
 
 # 初始化工作环境
 def init_work_space(workspace_path):
     if len(workspace_path) == 0:
@@ -24,22 +25,22 @@
     with open(os.path.join(nvos_dir, "config"), 'w') as file:
         for item in file_list:
             file.write(json.dumps(item) + "\n")
 
     remote.upload_file(file_list, project_space_list)
 
     workspace_env = []
-    if os.path.exists(os.path.expanduser(os.path.join("~", "workspace_env"))):
-        with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
+    if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
+        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
             for line in f:
                 workspace_env.append(line.strip())
     workspace_env.append(workspace_path)
     workspace_env = list(set(workspace_env))
-
-    with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'w') as f:
+    commonUtil.check_local_workspace()
+    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'w') as f:
         for item in workspace_env:
             f.write(item + "\n")
 
     return True
 
 
 def pull_data_from_cloud(workspace_path):
```

### Comparing `nvosscript-1.2.5/nvos/login.py` & `nvosscript-1.2.6/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.5/nvos/remote.py` & `nvosscript-1.2.6/nvos/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,40 @@
 daemon_network_front_mapping = {
     "prod": "https://ndtc.nioint.com/#/nvosTool/spaceList",
     "stg": "https://ndtc-stg.nioint.com/#/nvosTool/spaceList",
     "dev": " https://soa-tools-dev.nioint.com/#/nvosTool/spaceList"
 }
 global_var = 0
 
+
+def upload_logger_file(file_path):
+    get_current_env()
+    s3_secret = get_s3_secret()
+    bucket_name = s3_secret["bucket"]
+    aws_ak = s3_secret["ak"]
+    aws_sk = s3_secret["sk"]
+    aws_region = s3_secret["regionId"]
+    s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
+                        aws_secret_access_key=aws_sk)
+    bucket = s3.Bucket(bucket_name)
+    file_name = "/log/" + login.get_user_id() + "/ndtc.log"
+    bucket.upload_file(file_path, file_name)
+
 def upload_linux_client_script():
     file_name = "/nvos-script/linux/nvosscript.zip"
-    file_path = "/home/andre.zhao/software/nvos-script/dist/nvosscript.zip"
+    file_path = os.path.join(os.getcwd(), 'nvosscript.zip');
     upload_client_script(file_name, file_path)
 
+
 def upload_win_client_script():
     file_name = "/nvos-script/nvosscript.zip"
-    file_path = "C:\\Users\\moshang\\Desktop\\nvos-script\\dis\\nvosscript.zip"
+    file_path = os.path.join(os.getcwd(), 'nvosscript.zip')
     upload_client_script(file_name, file_path)
 
+
 def upload_client_script(file_name, file_path):
     get_current_env()
     s3_secret = get_s3_secret()
     bucket_name = s3_secret["bucket"]
     aws_ak = s3_secret["ak"]
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
@@ -191,24 +207,24 @@
 
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
     tip = daemon_network_front_mapping.get(env)
     result = {"cloud":val,"tip":tip,"env":env}
-    with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'w') as f:
+    with open(os.path.expanduser(os.path.join('~','.ndtcrc' ,'nvos_env')), 'w') as f:
         f.writelines(json.dumps(result))
     print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
     result = {}
-    if os.path.exists(os.path.expanduser(os.path.join('~', 'nvos_env'))):
-        with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'r')as f:
+    if os.path.exists(os.path.expanduser(os.path.join('~', '.ndtcrc', 'nvos_env'))):
+        with open(os.path.expanduser(os.path.join('~', '.ndtcrc', 'nvos_env')), 'r')as f:
             result = json.loads(f.readline().strip())
             daemon_network = result["cloud"]
             tip = result["tip"]
             env = result["env"]
             logger.info(f"current env:{env} this cloud linked:{tip} daemon_network:{daemon_network}")
     if result == {}:
         result["cloud"] = daemon_network_mapping.get('prod')
```

### Comparing `nvosscript-1.2.5/nvos/run.py` & `nvosscript-1.2.6/nvos/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,37 +18,38 @@
     if not status:
         print("Please login first. you could use login command to login this script")
         return
     workspace_path, success = utils.check_workspace_exist(os.getcwd())
 
     sub_workspace_path, flag = utils.check_subdirectory_workspace_exist(os.getcwd())
     if flag:
-        print(f"The subdirectory has already bean initialized, don't repeat execute init command, this subdirectory:{sub_workspace_path}")
+        print(
+            f"The subdirectory has already bean initialized, don't repeat execute init command, this subdirectory:{sub_workspace_path}")
         try:
             shutil.rmtree(os.path.join(os.getcwd(), ".ndtc"))
         except OSError as e:
             print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
         return
 
     print("please wait one minute.........")
     try:
         file.init_work_space(workspace_path)
     except Exception as e:
         logger.exception("command_init")
         print(f"Error: {e}")
 
 
-def command_async():
+def command_async(type=None):
     global all_workspace_path
     workspace_path, success = common_verify()
     if not success:
         return
     all_workspace_path.update({workspace_path: workspace_path})
     if platform.system() == 'Windows':
-        with open(os.path.expanduser(os.path.join("~", "workspace")), "w") as f:
+        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace")), "w") as f:
             f.write(json.dumps(all_workspace_path))
         return
     # 在运行时执行
     import daemon
     proc1 = subprocess.Popen(['ps', 'aux'], stdout=subprocess.PIPE)
     proc2 = subprocess.Popen(['grep', 'ndtc'], stdin=proc1.stdout,
                              stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -116,19 +117,23 @@
     if env is None:
         result = remote.get_current_env()
         print(f"current env:{result['env']} this cloud linked:{result['tip']}")
         return
 
     remote.switch_env(env)
     workspace_env = []
-    if os.path.exists(os.path.expanduser(os.path.join("~", "workspace_env"))):
-        with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
+    if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
+        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
             for line in f:
                 workspace_env.append(line.strip())
         for item in workspace_env:
             try:
                 os.remove(os.path.join(item, ".ndtc", 'offset'))
                 os.remove(os.path.join(item, ".ndtc", 'project_space'))
                 os.remove(os.path.join(item, ".ndtc", 'config'))
             except OSError:
                 logger.exception("command_env")
 
+
+def command_upload():
+    file_path = os.path.expanduser(os.path.join('~', 'ndtc.log'))
+    remote.upload_logger_file(file_path)
```

### Comparing `nvosscript-1.2.5/nvos/utils.py` & `nvosscript-1.2.6/nvos/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 def check_subdirectory_workspace_exist(current_path, index=0):
     for file_name in os.listdir(current_path):
         if ".ndtc" == file_name and index >= 1:
             return os.path.join(current_path, file_name), True
     for file_name in os.listdir(current_path):
         if os.path.isdir(os.path.join(current_path, file_name)):
             index = index + 1
-            subdirectory_workspace, result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name), index)
+            subdirectory_workspace, result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name),
+                                                                                index)
             if result:
                 return subdirectory_workspace, result
     return "", False
+
+
```

### Comparing `nvosscript-1.2.5/setup.py` & `nvosscript-1.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.5',
+    version='1.2.6',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.2.5/start/main.py` & `nvosscript-1.2.6/start/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,70 +3,97 @@
 # Press ⌃R to execute it or replace it with your code.
 # Press Double ⇧ to search everywhere for classes, files, tool windows, actions, and settings.
 import sys
 import logging
 import getpass
 import argparse
 import multiprocessing
-from nvos import login, run,remote
+from nvos import login, run
+from skyeye import skyeyecommand, datahandler
 
 # 创建全局记录器
 # 配置日志格式化信息
-logging.basicConfig(filename=os.path.expanduser(os.path.join("~", "logger.log")), level=logging.INFO,
+logging.basicConfig(filename=os.path.expanduser(os.path.join('~', 'ndtc.log')), level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logger = logging.getLogger()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Script Description")
-    subparsers = parser.add_subparsers(title="NVOS Script Command", dest='subcommand')
-    subparsers.add_parser('login', help='The login command is the first command that must be executed.')
+    subparsers = parser.add_subparsers(title="NDTC Script Command", dest='subcommand')
+    subparsers.add_parser('login', help='[NVOS]The login command is the first command that must be executed.')
+
+    subparsers.add_parser('init', help='[NVOS]The Init command is used to initialize the workspace. Please execute the '
+                                       'command in your workspace directory')
+    asyncparse = subparsers.add_parser('async',
+                                       help='[NVOS]The async command automatically synchronizes the data you modify from the cloud and to push addtion file to cloud')
+    asyncparse.add_argument('-t', '--type', choices=['pull', 'push', 'all'],
+                            help='switch you want async model,The currently owned modes are pull and push.')
+    subparsers.add_parser('pull', help='[NVOS]The pull command pulls the data you modify from the cloud')
+    subparsers.add_parser('push', help='[NVOS]The push command is used upload local new files or folders to the cloud')
+    subparsers.add_parser('version', help='[NVOS]The version command will tell you this script really version')
+    subparsers.add_parser('path',
+                          help='[NVOS]The path command will return windows service register script path, so you can '
+                               'install this script for windows like async command.You need execute "pythonw '
+                               'win_auto_script.py" and script is this command return path content')
+    upload = subparsers.add_parser('upload', help="[NVOS,SkyEye] upload your something to cloud")
+    upload.add_argument("-m", "--module", choices=['nvos', 'skyeye'] , help="choose you want to upload module,if you don't choose, it will default to all")
+    upload.add_argument("-l", '--log', help="input your SkeyEye log path,then we will analysis this log")
+    env = subparsers.add_parser('env')
+    env.add_argument('module', choices=['nvos', 'skyeye'])
+    env.add_argument('-s', '--switch', choices=['dev', 'stg', 'prod'])
 
-    init_command = subparsers.add_parser('init', help='The Init command is used to initialize the workspace. Please execute the '
-                                      'command in your workspace directory')
-    subparsers.add_parser('async', help='The async command automatically synchronizes the data you modify from the cloud and to push addtion file to cloud')
-    subparsers.add_parser('pull', help='The pull command pulls the data you modify from the cloud')
-    subparsers.add_parser('push', help='The push command is used upload local new files or folders to the cloud')
-    subparsers.add_parser('version', help='The version command will tell you this script really version')
-    subparsers.add_parser('path', help='The path command will return windows service register script path, so you can '
-                                       'install this script for windows like async command.You need execute "pythonw '
-                                       'win_auto_script.py" and script is this command return path content')
-    env = subparsers.add_parser('env', help='The env command will switch you need to network cloud, this args have dev,'
-                                      'stg and prod.')
-    env.add_argument('-s', '--switch', help='switch you want linked cloud environment')
     args = parser.parse_args()
 
     if args.subcommand == "login":
         username = input("email：")
         password = getpass.getpass("password：")
         status = login.login_user_check(username, password)
         print(status)
     elif args.subcommand == "init":
         run.command_init()
     elif args.subcommand == "async":
-        run.command_async()
+        run.command_async(args.type)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.5")
+        print("1.2.6")
     elif args.subcommand == 'env':
-        run.command_env(args.switch)
+        switch_command_env(args.module, args.switch)
+    elif args.subcommand == "upload":
+        switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
         print(win_path)
     else:
         parser.print_help()
         print(
             "\n\t if you still have many things you don't understand,you can take a look as https://nio.feishu.cn/wiki/wikcn9L7Di4ILQKaNmDDTrmpLqg ")
 
 
+def switch_command_env(module, switch=None):
+    if module == "nvos":
+        run.command_env(switch)
+    elif module == "skyeye":
+        skyeyecommand.command_env(switch)
+
+def switch_command_upload(module,log=None):
+    if module == "nvos":
+        run.command_upload()
+    elif module == "skyeye":
+        datahandler.filter_effective_log(log)
+    else:
+        run.command_upload()
+
+
+
+
 if __name__ == '__main__':
     multiprocessing.freeze_support()
     main()
-    # remote.upload_client_script("/Users/andre.zhao/Documents/test/nvosscript.zip")
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `nvosscript-1.2.5/win/win_auto_script.py` & `nvosscript-1.2.6/win/win_auto_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nvos import file
 import logging
 import json
 import os
 import concurrent.futures
 import time
 
-logging.basicConfig(filename=os.path.expanduser(os.path.join("~", "auto_service_logger.log")), level=logging.INFO,
+logging.basicConfig(filename=os.path.expanduser(os.path.join("~", "ndtc_auto.log")), level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logger = logging.getLogger()
 
 
 def execute_async(workspace_path):
     file.push_data_to_cloud(workspace_path)
     file.pull_data_from_cloud(workspace_path)
```

