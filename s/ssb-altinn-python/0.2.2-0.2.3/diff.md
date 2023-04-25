# Comparing `tmp/ssb_altinn_python-0.2.2.tar.gz` & `tmp/ssb_altinn_python-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.2.2.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.2.3.tar", max compression
```

## Comparing `ssb_altinn_python-0.2.2.tar` & `ssb_altinn_python-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-24 21:09:47.158828 ssb_altinn_python-0.2.2/LICENSE
--rw-r--r--   0        0        0     3941 2023-04-24 21:09:47.158828 ssb_altinn_python-0.2.2/README.md
--rw-r--r--   0        0        0     1967 2023-04-24 21:10:10.655976 ssb_altinn_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      188 2023-04-24 21:10:10.655976 ssb_altinn_python-0.2.2/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-04-24 21:09:47.162828 ssb_altinn_python-0.2.2/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-04-24 21:09:47.162828 ssb_altinn_python-0.2.2/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-24 21:09:47.162828 ssb_altinn_python-0.2.2/src/altinn/flatten.py
--rw-r--r--   0        0        0     3809 2023-04-24 21:10:10.655976 ssb_altinn_python-0.2.2/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:47.162828 ssb_altinn_python-0.2.2/src/altinn/py.typed
--rw-r--r--   0        0        0      497 2023-04-24 21:09:47.162828 ssb_altinn_python-0.2.2/src/altinn/utils.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3941 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/README.md
+-rw-r--r--   0        0        0     1967 2023-04-25 06:42:40.414380 ssb_altinn_python-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/flatten.py
+-rw-r--r--   0        0        0     3824 2023-04-25 06:42:40.414380 ssb_altinn_python-0.2.3/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/py.typed
+-rw-r--r--   0        0        0      497 2023-04-25 06:42:26.714096 ssb_altinn_python-0.2.3/src/altinn/utils.py
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.3/PKG-INFO
```

### Comparing `ssb_altinn_python-0.2.2/LICENSE` & `ssb_altinn_python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.2/README.md` & `ssb_altinn_python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.2/pyproject.toml` & `ssb_altinn_python-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.2.2"
+version = "0.2.3"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.2.2/src/altinn/file.py` & `ssb_altinn_python-0.2.3/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.2/src/altinn/parser.py` & `ssb_altinn_python-0.2.3/src/altinn/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,22 +116,22 @@
 
         for file in fs.glob(os.path.join(self.folder_path, "**", "*.xml")):
             xml_files.append(file)
 
         return xml_files
 
     def to_dataframe(self) -> pd.DataFrame:
-        """Parse all XML files in the folder and it subfolders to a pandas DataFrame.
+        """Parse all XML files in the folder and its subfolders to a pandas DataFrame.
 
         Returns:
             pd.DataFrame: A DataFrame containing data from all XML files.
         """
         xml_files = self.get_xml_files()
         df_list = []
 
         for file in xml_files:
             parser = ParseSingleXml(file)
             df = parser.to_dataframe()
             df_list.append(df)
 
-        combined_df = pd.concat(df_list, ignore_index=True)
+        combined_df = pd.concat(df_list, ignore_index=True, join="outer")
         return combined_df
```

### Comparing `ssb_altinn_python-0.2.2/PKG-INFO` & `ssb_altinn_python-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

