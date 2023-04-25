# Comparing `tmp/abst-1.9.4.tar.gz` & `tmp/abst-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.4.tar", last modified: Fri Apr 21 10:23:37 2023, max compression
+gzip compressed data, was "abst-1.9.5.tar", last modified: Tue Apr 25 11:56:21 2023, max compression
```

## Comparing `abst-1.9.4.tar` & `abst-1.9.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 10:23:25.000000 abst-1.9.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-21 10:23:37.115653 abst-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-21 10:23:25.000000 abst-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-21 10:23:25.000000 abst-1.9.4/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-21 10:23:25.000000 abst-1.9.4/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-21 10:23:25.000000 abst-1.9.4/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-21 10:23:25.000000 abst-1.9.4/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-21 10:23:25.000000 abst-1.9.4/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 10:23:25.000000 abst-1.9.4/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 10:23:25.000000 abst-1.9.4/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 10:23:25.000000 abst-1.9.4/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:23:36.000000 abst-1.9.4/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:23:37.115653 abst-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-21 10:23:25.000000 abst-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 10:23:25.000000 abst-1.9.4/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 11:56:10.000000 abst-1.9.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-25 11:56:21.188225 abst-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 11:56:10.000000 abst-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 11:56:10.000000 abst-1.9.5/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-25 11:56:10.000000 abst-1.9.5/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 11:56:10.000000 abst-1.9.5/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 11:56:10.000000 abst-1.9.5/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-25 11:56:10.000000 abst-1.9.5/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 11:56:10.000000 abst-1.9.5/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-25 11:56:10.000000 abst-1.9.5/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 11:56:10.000000 abst-1.9.5/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:56:21.188225 abst-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 11:56:10.000000 abst-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 11:56:10.000000 abst-1.9.5/tests/test_sample_dict.py
```

### Comparing `abst-1.9.4/LICENSE.md` & `abst-1.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/PKG-INFO` & `abst-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.4
+Version: 1.9.5
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.4/README.md` & `abst-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.5/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/bastion_support/oci_bastion.py` & `abst-1.9.5/abst/bastion_support/oci_bastion.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/cfg_func.py` & `abst-1.9.5/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/config.py` & `abst-1.9.5/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/dialogs.py` & `abst-1.9.5/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/main.py` & `abst-1.9.5/abst/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -379,29 +379,27 @@
 
 
 @cli.command("ssh", help="Will SSH into pod with containing string name")
 @click.argument("pod_name")
 @click.option("--debug", is_flag=True, default=False)
 def ssh_pod(pod_name, debug):
     setup_calls(debug)
-    found = list()
+
     try:
         rich.print("Fetching pods")
         pod_lines = (
             subprocess.check_output(f"kubectl get pods -A".split(" "))
             .decode()
             .split("\n")
         )
     except FileNotFoundError:
         rich.print("[red]kubectl not found on this machine[/red]")
         return
 
-    for pod_line in pod_lines:
-        if pod_name in pod_line:
-            found.append(pod_line)
+    found = list(filter(lambda pod_line: pod_name in pod_line, pod_lines))
 
     if len(found) > 1:
         data = re.sub(
             " +",
             " ",
             inquirer.select("Found more pods, choose one:", list(found)).execute(),
         ).split(" ")
@@ -418,14 +416,56 @@
         f"[green]Connecting to {pod_name_precise} in namespace: {data[0]}[/green]"
     )
     os.system(
         f"kubectl exec -n {data[0]} --stdin --tty {pod_name_precise} -- /bin/bash"
     )
 
 
+@cli.command("logs", help="Will get logs from a pod with containing string name")
+@click.argument("pod_name")
+@click.option("--debug", is_flag=True, default=False)
+def log_pod(pod_name, debug):
+    setup_calls(debug)
+
+    try:
+        rich.print("Fetching pods")
+        pod_lines = (
+            subprocess.check_output(f"kubectl get pods -A".split(" "))
+            .decode()
+            .split("\n")
+        )
+    except FileNotFoundError:
+        rich.print("[red]kubectl not found on this machine[/red]")
+        return
+
+    found = list(filter(lambda pod_line: pod_name in pod_line, pod_lines))
+
+    if len(found) > 1:
+        data = re.sub(
+            " +",
+            " ",
+            inquirer.select("Found more pods, choose one:", found).execute(),
+        ).split(" ")
+        pod_name_precise = data[1]
+    elif len(found) == 1:
+        tmp = found.pop()
+        data = re.sub(" +", " ", tmp).split(" ")
+        pod_name_precise = data[1]
+    else:
+        rich.print(f"[red]No pods with name {pod_name} found[/red]")
+        return
+
+    rich.print(
+        f"[green]Getting logs from {pod_name_precise} in namespace: {data[0]}[/green]"
+    )
+    os.system(
+        f"kubectl -n {data[0]} logs {pod_name_precise}"
+    )
+
+
 @cli.group("cp")
 def cp():
     pass
 
 
 @cli.group("helm")
 def helm():
```

### Comparing `abst-1.9.4/abst/notifier/version_notifier.py` & `abst-1.9.5/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/tools.py` & `abst-1.9.5/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst/wrappers.py` & `abst-1.9.5/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/abst.egg-info/PKG-INFO` & `abst-1.9.5/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.4
+Version: 1.9.5
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.4/abst.egg-info/SOURCES.txt` & `abst-1.9.5/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.4/setup.py` & `abst-1.9.5/setup.py`

 * *Files identical despite different names*

