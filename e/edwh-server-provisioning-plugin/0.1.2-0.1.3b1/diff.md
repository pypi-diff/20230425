# Comparing `tmp/edwh_server_provisioning_plugin-0.1.2.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.1.3b1.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.1.2.tar` & `edwh_server_provisioning_plugin-0.1.3b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/.dcignore
--rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    45349 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/readme.md
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/.dcignore
+-rw-r--r--   0        0        0    14236 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    45350 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/LICENSE.txt
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/readme.md
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.1.2/.dcignore` & `edwh_server_provisioning_plugin-0.1.3b1/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.2/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.1.3b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.3-beta.1 (2023-04-25)
+### Fix
+* `ssh -tt` instead of `ssh -t` to avoid `pseudo-terminal  will not be allocated because stdin is not a terminal` ([`fa18bd9`](https://github.com/educationwarehouse/server_provisioning/commit/fa18bd980763790df7ef3a34c4193d1b171189a2))
+
 ## v0.1.2 (2023-04-17)
 ### Documentation
 * **versions:** Remove unsupported python versions + fix md badges ([`d696150`](https://github.com/educationwarehouse/server_provisioning/commit/d696150b974bb8e37faf08ebcbc9d524d3d29586))
 
 ## v0.1.1 (2023-04-17)
 ### Documentation
 * **readme:** New plugin docs, keep old (Dutch) readme for reference ([`fe2e8da`](https://github.com/educationwarehouse/server_provisioning/commit/fe2e8daec6ca758cc3997fc5ce95de9f3735ad52))
```

### Comparing `edwh_server_provisioning_plugin-0.1.2/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.1.3b1/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.2/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,15 +633,15 @@
             print("Adding github.com signatures to .ssh/known_hosts")
             c.put(io.StringIO(known_hosts), ".ssh/known_hosts")
         # respond_to_security=Responder(r'Are you sure you want to continue connecting \(yes/no/\[fingerprint\]\)\?.*','yes\n')
         # failsafe(lambda:c.run(f'ssh -tN git@github.com', watchers=[respond_to_security]))
 
         # check als machine correcte git ssh verbinding kan maken
         # fingerprint
-        if failsafe("Permission denied" in c.run("ssh -t git@github.com", hide=True)).stderr:
+        if failsafe("Permission denied" in c.run("ssh -tt git@github.com", hide=True)).stderr:
             raise Exception("github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py")
 
         # test if the repo exists:
         if (
                 "fatal:"
                 in c.run(
             f"cd {target_directory or git_repo}; git status", warn=True, hide=True
```

### Comparing `edwh_server_provisioning_plugin-0.1.2/LICENSE.txt` & `edwh_server_provisioning_plugin-0.1.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.2/pyproject.toml` & `edwh_server_provisioning_plugin-0.1.3b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.2/readme.md` & `edwh_server_provisioning_plugin-0.1.3b1/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.2/PKG-INFO` & `edwh_server_provisioning_plugin-0.1.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.1.2
+Version: 0.1.3b1
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

