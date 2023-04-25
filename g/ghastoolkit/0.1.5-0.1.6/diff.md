# Comparing `tmp/ghastoolkit-0.1.5.tar.gz` & `tmp/ghastoolkit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.5.tar", last modified: Mon Apr 24 18:35:30 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.6.tar", last modified: Tue Apr 25 00:17:50 2023, max compression
```

## Comparing `ghastoolkit-0.1.5.tar` & `ghastoolkit-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.770317 ghastoolkit-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.770317 ghastoolkit-0.1.5/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/octokit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.547539 ghastoolkit-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.547539 ghastoolkit-0.1.6/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.547539 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 00:17:50.000000 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 00:17:50.000000 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:17:50.000000 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 00:17:50.000000 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 00:17:50.000000 ghastoolkit-0.1.6/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:17:50.551539 ghastoolkit-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 00:17:16.000000 ghastoolkit-0.1.6/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.1.5/LICENSE` & `ghastoolkit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/pyproject.toml` & `ghastoolkit-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/__init__.py` & `ghastoolkit-0.1.6/src/ghastoolkit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -16,14 +16,15 @@
 __author__ = "GeekMasher"
 
 
 # Octokit
 from ghastoolkit.octokit.github import GitHub
 from ghastoolkit.octokit.octokit import Octokit, RestRequest, GraphQLRequest
 from ghastoolkit.octokit.codescanning import CodeScanning
+from ghastoolkit.octokit.secretscanning import SecretScanning
 from ghastoolkit.octokit.dependencygraph import (
     DependencyGraph,
     Dependencies,
     Dependency,
 )
 
 # CodeQL
```

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.6/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.6/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.6/src/ghastoolkit/octokit/codescanning.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,57 @@
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
 class CodeScanning:
-    def __init__(self, repository: Repository) -> None:
-        """GitHub Code Scanning REST API"""
-        self.repository = repository
-        self.rest = RestRequest(repository)
+    def __init__(self, repository: Optional[Repository] = None) -> None:
+        """GitHub Code Scanning REST API
 
-    def getOrgAlerts(self, state: str = "open") -> list[dict[Any, Any]]:
-        """Get Organization Alerts"""
+        https://docs.github.com/en/rest/code-scanning
+        """
+        self.repository = repository or GitHub.repository
+        if not self.repository:
+            raise Exception("CodeScanning requires Repository to be set")
+        self.rest = RestRequest(self.repository)
+
+    def getOrganizationAlerts(self, state: str = "open") -> list[dict[Any, Any]]:
+        """Get Organization Alerts
+
+        https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-an-organization
+        """
         results = self.rest.get(
             "/orgs/{org}/code-scanning/alerts", {"state": state}, authenticated=True
         )
         if isinstance(results, list):
             return results
         raise Exception(f"Error getting alerts from Organization")
 
     def getAlerts(
         self, state: str = "open", tool_name: Optional[str] = None
     ) -> list[dict]:
         """Get a code scanning alert
 
-        https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#get-a-code-scanning-alert
+        https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-a-repository
         """
         results = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts",
             {"state": state, "tool_name": tool_name},
             authenticated=True,
         )
         if isinstance(results, list):
             return results
         raise Exception(f"Error getting list of alerts")
 
     def getAlert(self, alert_number: int) -> dict:
-        """Get Single Alert"""
+        """Get Single Alert
+
+        https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
+        """
         results = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}",
             {"alert_number": alert_number},
             authenticated=True,
         )
         if isinstance(results, dict):
             return results
```

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.6/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.6/src/ghastoolkit/octokit/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,21 @@
     owner: str
     repo: str
     reference: Optional[str] = None
     branch: Optional[str] = None
 
     sha: Optional[str] = None
 
+    def __post_init__(self) -> None:
+        if self.reference and not self.branch:
+            _, _, branch = self.reference.split("/", 3)
+            self.branch = branch
+        if self.branch and not self.reference:
+            self.reference = f"refs/heads/{self.branch}"
+
     def __str__(self) -> str:
         return f"{self.owner}/{self.repo}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def display(self):
@@ -33,15 +40,15 @@
             ref = f"refs/heads/{branch}"
 
         owner, repo = name.split("/", 1)
         return Repository(owner, repo, reference=ref, branch=branch)
 
 
 class GitHub:
-    repository: Optional[Repository] = None
+    repository: Repository = Repository("GeekMasher", "ghastoolkit")
     token: Optional[str] = None
 
     # URLs
     instance: str = "https://github.com"
     api_rest: str = "https://api.github.com"
     api_graphql: str = "https://api.github.com/graphql"
```

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.6/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.6/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,11 +12,14 @@
 src/ghastoolkit/codeql/consts.py
 src/ghastoolkit/codeql/databases.py
 src/ghastoolkit/octokit/__init__.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
+src/ghastoolkit/octokit/secretscanning.py
 tests/test_codeqldb.py
+tests/test_codescanning.py
 tests/test_depgraph.py
 tests/test_github.py
-tests/test_octokit.py
+tests/test_octokit.py
+tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.1.5/tests/test_codeqldb.py` & `ghastoolkit-0.1.6/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/tests/test_depgraph.py` & `ghastoolkit-0.1.6/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.5/tests/test_github.py` & `ghastoolkit-0.1.6/tests/test_github.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,13 @@
         repo = Repository.parseRepository("GeekMasher/ghastoolkit@main")
         self.assertEqual(repo.owner, "GeekMasher")
         self.assertEqual(repo.repo, "ghastoolkit")
         self.assertEqual(repo.branch, "main")
         self.assertEqual(repo.reference, "refs/heads/main")
 
 
+class TestRepository(unittest.TestCase):
+    def test_branch(self):
+        repo = Repository("GeekMasher", "ghastoolkit", reference="refs/heads/main")
+        self.assertEqual(repo.reference, "refs/heads/main")
+        self.assertEqual(repo.branch, "main")
+
```

### Comparing `ghastoolkit-0.1.5/tests/test_octokit.py` & `ghastoolkit-0.1.6/tests/test_octokit.py`

 * *Files identical despite different names*

