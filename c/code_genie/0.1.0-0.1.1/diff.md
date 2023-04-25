# Comparing `tmp/code_genie-0.1.0.tar.gz` & `tmp/code_genie-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.1.0.tar", last modified: Mon Apr 24 17:14:48 2023, max compression
+gzip compressed data, was "code_genie-0.1.1.tar", last modified: Tue Apr 25 12:25:43 2023, max compression
```

## Comparing `code_genie-0.1.0.tar` & `code_genie-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1831 2023-04-24 09:13:30.519550 code_genie-0.1.0/.gitignore
--rw-r--r--   0        0        0       91 2023-04-24 17:05:44.043619 code_genie-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.1.0/LICENSE
--rw-r--r--   0        0        0     1272 2023-04-24 17:02:47.125827 code_genie-0.1.0/README.md
--rw-r--r--   0        0        0      456 2023-04-24 17:13:38.720473 code_genie-0.1.0/TODO.md
--rw-r--r--   0        0        0       72 2023-04-24 13:56:08.341992 code_genie-0.1.0/code_genie/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-24 11:07:50.578272 code_genie-0.1.0/code_genie/client.py
--rw-r--r--   0        0        0     2353 2023-04-24 11:06:52.078817 code_genie-0.1.0/code_genie/genie.py
--rw-r--r--   0        0        0      998 2023-04-24 16:56:07.815930 code_genie-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 10:56:36.796006 code_genie-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      871 2023-04-24 12:49:34.403254 code_genie-0.1.0/tests/test_genie.py
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 code_genie-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1831 2023-04-25 05:29:52.444630 code_genie-0.1.1/.gitignore
+-rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1272 2023-04-25 12:24:46.974510 code_genie-0.1.1/README.md
+-rw-r--r--   0        0        0      456 2023-04-25 05:29:52.446244 code_genie-0.1.1/TODO.md
+-rw-r--r--   0        0        0       72 2023-04-25 12:24:52.813699 code_genie-0.1.1/code_genie/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-25 05:29:52.447321 code_genie-0.1.1/code_genie/client.py
+-rw-r--r--   0        0        0     2384 2023-04-25 12:24:52.814422 code_genie-0.1.1/code_genie/genie.py
+-rw-r--r--   0        0        0      998 2023-04-25 12:24:46.975841 code_genie-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-25 12:24:52.815053 code_genie-0.1.1/tests/test_genie.py
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 code_genie-0.1.1/PKG-INFO
```

### Comparing `code_genie-0.1.0/.gitignore` & `code_genie-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.0/LICENSE` & `code_genie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.0/README.md` & `code_genie-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.0/code_genie/client.py` & `code_genie-0.1.1/code_genie/client.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.0/code_genie/genie.py` & `code_genie-0.1.1/code_genie/genie.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     @classmethod
     def _extract_executable(cls, code: str, fn_name: str) -> Callable:
         # define function in memory
         mem = {}
         exec(code, mem)
         return mem[fn_name]
 
-    def __call__(self, **kwargs):
-        return self._executor(**kwargs)
+    def __call__(self, *args, **kwargs):
+        return self._executor(*args, **kwargs)
 
     @property
     def code(self):
         return self._code
 
 
 class Genie(GenieBase):
@@ -47,15 +47,15 @@
                                  allowed_imports=self._allowed_imports))
 
 
 class PandasGenie(GenieBase):
 
     def __init__(self,
                  instructions: Union[str, List[str]],
-                 columns: List[str],
+                 columns: Optional[List[str]] = None,
                  inputs: Optional[Dict[str, str]] = None,
                  allowed_imports: Optional[List[str]] = None,
                  client: Optional[Client] = None):
         self._columns = columns
         super().__init__(instructions, inputs, allowed_imports, client)
 
     def _get_code(self, client: Client) -> Tuple[str, str]:
```

### Comparing `code_genie-0.1.0/pyproject.toml` & `code_genie-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.0/tests/test_genie.py` & `code_genie-0.1.1/tests/test_genie.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def test_add(self):
         # use genie to get a method to add 2 numbers
         add = Genie(instructions="add num1 and num2",
                     inputs={"num1": "int", "num2": "int"},
                     allowed_imports=["math"])
         # call the method
         self.assertEqual(add(num1=1, num2=2), 3)
-        self.assertEqual(add(num1=6, num2=12), 18)
+        self.assertEqual(add(6, 12), 18)
 
     def test_pd_mean(self):
         # use genie to get a method to get the mean of a list of numbers
         mean_sum = PandasGenie(instructions="sum of mean of columns x and y",
                                columns=["x", "y"])
         df = pd.DataFrame({"x": [1, 2, 3], "y": [4, 5, 6]})
         # call the method
```

### Comparing `code_genie-0.1.0/PKG-INFO` & `code_genie-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.1.0
+Version: 0.1.1
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

