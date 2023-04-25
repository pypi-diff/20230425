# Comparing `tmp/ms_reader-1.4.1.tar.gz` & `tmp/ms_reader-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_reader-1.4.1.tar", last modified: Mon Apr  3 11:29:06 2023, max compression
+gzip compressed data, was "ms_reader-1.4.2.tar", last modified: Tue Apr 25 13:03:15 2023, max compression
```

## Comparing `ms_reader-1.4.1.tar` & `ms_reader-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:06.299797 ms_reader-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-04-03 11:28:55.000000 ms_reader-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-03 11:29:06.299797 ms_reader-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-03 11:28:55.000000 ms_reader-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:06.299797 ms_reader-1.4.1/ms_reader/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 11:28:55.000000 ms_reader-1.4.1/ms_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-03 11:28:55.000000 ms_reader-1.4.1/ms_reader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-03 11:28:55.000000 ms_reader-1.4.1/ms_reader/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    43866 2023-04-03 11:28:55.000000 ms_reader-1.4.1/ms_reader/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-03 11:28:55.000000 ms_reader-1.4.1/ms_reader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:06.299797 ms_reader-1.4.1/ms_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 11:29:06.000000 ms_reader-1.4.1/ms_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-03 11:28:55.000000 ms_reader-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-03 11:29:06.299797 ms_reader-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:06.299797 ms_reader-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-04-03 11:28:55.000000 ms_reader-1.4.1/tests/test_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:03:15.629543 ms_reader-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-04-25 13:03:04.000000 ms_reader-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 13:03:15.629543 ms_reader-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-25 13:03:04.000000 ms_reader-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:03:15.629543 ms_reader-1.4.2/ms_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 13:03:04.000000 ms_reader-1.4.2/ms_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-25 13:03:04.000000 ms_reader-1.4.2/ms_reader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-25 13:03:04.000000 ms_reader-1.4.2/ms_reader/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43921 2023-04-25 13:03:04.000000 ms_reader-1.4.2/ms_reader/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-25 13:03:04.000000 ms_reader-1.4.2/ms_reader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:03:15.629543 ms_reader-1.4.2/ms_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 13:03:15.000000 ms_reader-1.4.2/ms_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 13:03:04.000000 ms_reader-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 13:03:15.633543 ms_reader-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:03:15.629543 ms_reader-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-04-25 13:03:04.000000 ms_reader-1.4.2/tests/test_extractor.py
```

### Comparing `ms_reader-1.4.1/LICENSE` & `ms_reader-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_reader-1.4.1/PKG-INFO` & `ms_reader-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_reader
-Version: 1.4.1
+Version: 1.4.2
 Summary: Package for parsing a Tracefinder file containing processed Mass Spectrometry data
 Home-page: https://github.com/llegregam/MSReader
 Author: Loïc Le Grégam
 Author-email: legregam@insa-toulouse.fr
 Project-URL: Bug Tracker, https://github.com/llegregam/MSReader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ms_reader-1.4.1/ms_reader/__main__.py` & `ms_reader-1.4.2/ms_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `ms_reader-1.4.1/ms_reader/app.py` & `ms_reader-1.4.2/ms_reader/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,18 +196,25 @@
         destination = st.text_input("Input destination path for excel files")
         preview = st.form_submit_button("Preview")
         submit_export = st.form_submit_button("Export selection")
         submit_stat_out = st.form_submit_button("Export stat output")
         submit_pca_out = st.form_submit_button("Export stat output for PCA")
 
     if reader.calib_data is not None:
-        reader.handle_calibration()
-
+        try:
+            reader.handle_calibration()
+        except Exception as e:
+            st.error("There was an error while handling the calibration data")
+            raise
     if report_box:
-        reader.generate_report(metabolites_to_drop)
+        try:
+            reader.generate_report(metabolites_to_drop)
+        except Exception as e:
+            st.error("There was an error while generating the report")
+            raise
         if preview:
             with st.expander("Show report"):
                 st.dataframe(reader.calrep)
     if areas_box:
         reader.generate_areas_table()
         if preview:
             with st.expander("Show C12 Areas"):
```

### Comparing `ms_reader-1.4.1/ms_reader/extract.py` & `ms_reader-1.4.2/ms_reader/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,15 +917,15 @@
         self.stream.seek(0)
         with open(f"{destination}\\file.log", "w") as log:
             print(self.stream.getvalue(), file=log)
 
     def export_stat_output(self, path, pca=False):
 
         dest = Path(path)
-        dest = dest / "output_for_graphstat.tsv"
+        dest = dest / "output_for_graphstat.tsv" if not pca else dest / "ouptput_for_graphstat_PCA.tsv"
         stat_out = self._build_stat_output(pca)
         stat_out.to_csv(str(dest), sep="\t", index=False, encoding='utf-8-sig')
         self._output_log(path)
 
     def export_final_excel(self, path):
 
         dest_path = Path(path)
```

### Comparing `ms_reader-1.4.1/ms_reader.egg-info/PKG-INFO` & `ms_reader-1.4.2/ms_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-reader
-Version: 1.4.1
+Version: 1.4.2
 Summary: Package for parsing a Tracefinder file containing processed Mass Spectrometry data
 Home-page: https://github.com/llegregam/MSReader
 Author: Loïc Le Grégam
 Author-email: legregam@insa-toulouse.fr
 Project-URL: Bug Tracker, https://github.com/llegregam/MSReader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ms_reader-1.4.1/setup.cfg` & `ms_reader-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms_reader-1.4.1/tests/test_extractor.py` & `ms_reader-1.4.2/tests/test_extractor.py`

 * *Files identical despite different names*

