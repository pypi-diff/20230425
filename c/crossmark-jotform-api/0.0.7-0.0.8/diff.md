# Comparing `tmp/crossmark-jotform-api-0.0.7.tar.gz` & `tmp/crossmark-jotform-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.0.7.tar", last modified: Tue Apr 25 03:48:25 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.0.8.tar", last modified: Tue Apr 25 03:50:03 2023, max compression
```

## Comparing `crossmark-jotform-api-0.0.7.tar` & `crossmark-jotform-api-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.059958 crossmark-jotform-api-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1896 2023-04-25 03:48:25.058958 crossmark-jotform-api-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-04-25 03:48:03.000000 crossmark-jotform-api-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 03:48:25.060923 crossmark-jotform-api-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.044218 crossmark-jotform-api-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.048914 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    10812 2023-04-25 03:47:53.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.056959 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 03:50:03.413813 crossmark-jotform-api-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1896 2023-04-25 03:50:03.412821 crossmark-jotform-api-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-04-25 03:49:35.000000 crossmark-jotform-api-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:50:03.413813 crossmark-jotform-api-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 03:50:03.396780 crossmark-jotform-api-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 03:50:03.401818 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    10591 2023-04-25 03:49:11.000000 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:50:03.410780 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     1896 2023-04-25 03:50:03.000000 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-25 03:50:03.000000 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:50:03.000000 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-25 03:50:03.000000 crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.0.7/LICENSE` & `crossmark-jotform-api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.0.7/PKG-INFO` & `crossmark-jotform-api-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.0.7/pyproject.toml` & `crossmark-jotform-api-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.0.8/src/crossmark_jotform_api/jotForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,18 +122,15 @@
             self.url = "&".join(params)
         else:
             self.url += "&" + key + "=" + value
 
     def set_data(self):
         self.data = requests.get(self.url, timeout=15).json()
         re_count = self.data['resultSet']['count']
-        count = self.get_submissions_count()
-        print(f"count: {count}")
-        print(f"url: {self.url}")
-        print(f"re_count: {re_count}, self.submission_count: {self.submission_count}, self.submission_data: {len(self.submission_data['submissions'])}")
+        # count = self.get_submissions_count()
         self.submission_count += re_count
         self.submission_data["submissions"].update(
             self.__set_submission_data(
                 self.data['content']
             )
         )
         if re_count == self.data['resultSet']['limit']:
```

### Comparing `crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.0.8/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

