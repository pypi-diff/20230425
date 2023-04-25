# Comparing `tmp/ssb_altinn_python-0.2.4.tar.gz` & `tmp/ssb_altinn_python-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.2.4.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.2.5.tar", max compression
```

## Comparing `ssb_altinn_python-0.2.4.tar` & `ssb_altinn_python-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-25 09:52:46.668146 ssb_altinn_python-0.2.4/LICENSE
--rw-r--r--   0        0        0     3941 2023-04-25 09:52:46.668146 ssb_altinn_python-0.2.4/README.md
--rw-r--r--   0        0        0     1967 2023-04-25 09:53:01.724350 ssb_altinn_python-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      188 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/flatten.py
--rw-r--r--   0        0        0     3867 2023-04-25 09:53:01.724350 ssb_altinn_python-0.2.4/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/py.typed
--rw-r--r--   0        0        0      497 2023-04-25 09:52:46.672146 ssb_altinn_python-0.2.4/src/altinn/utils.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-25 10:41:51.132461 ssb_altinn_python-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3941 2023-04-25 10:41:51.132461 ssb_altinn_python-0.2.5/README.md
+-rw-r--r--   0        0        0     1967 2023-04-25 10:42:11.672673 ssb_altinn_python-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/flatten.py
+-rw-r--r--   0        0        0     3918 2023-04-25 10:42:11.672673 ssb_altinn_python-0.2.5/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/py.typed
+-rw-r--r--   0        0        0      497 2023-04-25 10:41:51.136461 ssb_altinn_python-0.2.5/src/altinn/utils.py
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.5/PKG-INFO
```

### Comparing `ssb_altinn_python-0.2.4/LICENSE` & `ssb_altinn_python-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.4/README.md` & `ssb_altinn_python-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.4/pyproject.toml` & `ssb_altinn_python-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.2.4"
+version = "0.2.5"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.2.4/src/altinn/file.py` & `ssb_altinn_python-0.2.5/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.4/src/altinn/parser.py` & `ssb_altinn_python-0.2.5/src/altinn/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,13 +124,16 @@
     def to_dataframe(self) -> pd.DataFrame:
         """Parse all XML files in the folder and its subfolders to a pandas DataFrame.
 
         Returns:
             pd.DataFrame: A DataFrame containing data from all XML files.
         """
         xml_files = self.get_xml_files()
-        pool = multiprocessing.Pool(processes=multiprocessing.cpu_count())
-        df_list = pool.map(lambda file: ParseSingleXml(file).to_dataframe(), xml_files)
+
+        def parse_single_xml(file):
+            return ParseSingleXml(file).to_dataframe()
+
+        with multiprocessing.Pool(processes=multiprocessing.cpu_count()) as pool:
+            df_list = pool.map(parse_single_xml, xml_files)
         combined_df = pd.concat(df_list, ignore_index=True, join="outer")
-        pool.close()
 
         return combined_df
```

### Comparing `ssb_altinn_python-0.2.4/PKG-INFO` & `ssb_altinn_python-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.2.4
+Version: 0.2.5
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

