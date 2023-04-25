# Comparing `tmp/edwh_server_provisioning_plugin-0.1.3.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.1.3b1.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.1.3.tar` & `edwh_server_provisioning_plugin-0.1.3b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/.dcignore
--rw-r--r--   0        0        0    14611 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    44894 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/readme.md
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3/PKG-INFO
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

### Comparing `edwh_server_provisioning_plugin-0.1.3/.dcignore` & `edwh_server_provisioning_plugin-0.1.3b1/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.1.3b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
-## v0.1.3 (2023-04-25)
-### Fix
-* Now removes github keys before reassigning using `ssh -o StricHostKeyChecking=accept-new` to flush the old one and insert a new one. Also adds a better warning when installing a repo inside a git-repo (which you can't). ([`5402e03`](https://github.com/educationwarehouse/server_provisioning/commit/5402e0322301380dbd9e9abcdfe99457c7b4d288))
-
 ## v0.1.3-beta.1 (2023-04-25)
 ### Fix
 * `ssh -tt` instead of `ssh -t` to avoid `pseudo-terminal  will not be allocated because stdin is not a terminal` ([`fa18bd9`](https://github.com/educationwarehouse/server_provisioning/commit/fa18bd980763790df7ef3a34c4193d1b171189a2))
 
 ## v0.1.2 (2023-04-17)
 ### Documentation
 * **versions:** Remove unsupported python versions + fix md badges ([`d696150`](https://github.com/educationwarehouse/server_provisioning/commit/d696150b974bb8e37faf08ebcbc9d524d3d29586))
```

### Comparing `edwh_server_provisioning_plugin-0.1.3/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.1.3b1/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 $PATH.extend(':~/.local/bin/')
 #$FLIT_USERNAME='...'
 #$FLIT_PASSWORD='...'
 $PROMPT_FIELDS['prompt_end'] = $PROMPT_FIELDS['prompt_end'].replace('$', '{WHITE}@')
 $PROMPT = '{env_name}{BOLD_GREEN}{user}@{hostname}{BOLD_BLUE} {short_cwd}{branch_color}{curr_branch: {}}{NO_COLOR} {BOLD_BLUE}{prompt_end}{NO_COLOR} '
 """
 
+GITHUB_KNOWN_HOSTS = """
+|1|GNDleqLr6aOVYd889BVVy2ErPA4=|XdPSQ2p/b47kjCr8gt/vKTi+KT0= ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIOMqqnkVzrm0SdG6UOoqKLsabgH5C9okWi0dh2l9GKJl
+"""
+
 JOPLIN_DOCKER_COMPOSE = """
 version: '3.3'
 services:
     proxy:
         image: "traefik:v2.5"
         container_name: "traefik"
         restart: unless-stopped
@@ -377,15 +381,15 @@
 
 
 def failsafe(callable):
     "Executes the callable, and if not result.ok raises a RemoteWentWrong exception."
     result: Result = callable()
     if not result.ok:
         raise RemoteWentWrong(result.stderr)
-    return result
+
 
 class TestOnce(ABC):
     tested = False
 
     @classmethod
     def test(cls, c):
         if cls.tested:
@@ -618,20 +622,26 @@
             """
             )
             # Host github.com-ontwikkelstraat
             #         Hostname github.com
             #         IdentityFile=/home/ubuntu/.ssh/git-ontwikkelstraat.id_rsa
             c.put(io.StringIO(config), ".ssh/config")
 
-
+        # fix the .ssh/known_hosts
+        known_hosts = c.run(f"cat .ssh/known_hosts", warn=True).stdout
+        if GITHUB_KNOWN_HOSTS.strip() not in known_hosts:
+            known_hosts += GITHUB_KNOWN_HOSTS
+            print("Adding github.com signatures to .ssh/known_hosts")
+            c.put(io.StringIO(known_hosts), ".ssh/known_hosts")
         # respond_to_security=Responder(r'Are you sure you want to continue connecting \(yes/no/\[fingerprint\]\)\?.*','yes\n')
+        # failsafe(lambda:c.run(f'ssh -tN git@github.com', watchers=[respond_to_security]))
 
         # check als machine correcte git ssh verbinding kan maken
         # fingerprint
-        if "Permission denied (publickey)" in c.run("ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com", hide=True, warn=True).stderr:
+        if failsafe("Permission denied" in c.run("ssh -tt git@github.com", hide=True)).stderr:
             raise Exception("github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py")
 
         # test if the repo exists:
         if (
                 "fatal:"
                 in c.run(
             f"cd {target_directory or git_repo}; git status", warn=True, hide=True
@@ -639,15 +649,15 @@
         ):
             failsafe(
                 lambda: c.run(
                     f"git clone git@github.com-{git_repo}:{git_user}/{git_repo} {target_directory}"
                 )
             )
         else:
-            print(f"Repo {git_repo} already installed in {target_directory}, or a git repository exists higher-up")
+            print(f"Repo {git_repo} already installed")
         if branch:
             c.run(f"cd {target_directory}; git checkout {branch}")
     else:
         # anonymous git
         failsafe(lambda: c.run(f"git clone https://github.com/{git_user}/{git_repo}"))
```

### Comparing `edwh_server_provisioning_plugin-0.1.3/LICENSE.txt` & `edwh_server_provisioning_plugin-0.1.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3/pyproject.toml` & `edwh_server_provisioning_plugin-0.1.3b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3/readme.md` & `edwh_server_provisioning_plugin-0.1.3b1/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3/PKG-INFO` & `edwh_server_provisioning_plugin-0.1.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.1.3
+Version: 0.1.3b1
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

