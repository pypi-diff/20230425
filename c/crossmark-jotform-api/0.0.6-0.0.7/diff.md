# Comparing `tmp/crossmark-jotform-api-0.0.6.tar.gz` & `tmp/crossmark-jotform-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.0.6.tar", last modified: Tue Apr 25 03:45:30 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.0.7.tar", last modified: Tue Apr 25 03:48:25 2023, max compression
```

## Comparing `crossmark-jotform-api-0.0.6.tar` & `crossmark-jotform-api-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:45:30.166303 crossmark-jotform-api-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1896 2023-04-25 03:45:30.165299 crossmark-jotform-api-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-04-25 03:16:14.000000 crossmark-jotform-api-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 03:45:30.167302 crossmark-jotform-api-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 03:45:30.152300 crossmark-jotform-api-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 03:45:30.156299 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    10644 2023-04-25 03:42:53.000000 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:45:30.163300 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-04-25 03:45:30.000000 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-25 03:45:30.000000 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:45:30.000000 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-25 03:45:30.000000 crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.059958 crossmark-jotform-api-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1896 2023-04-25 03:48:25.058958 crossmark-jotform-api-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-04-25 03:48:03.000000 crossmark-jotform-api-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:48:25.060923 crossmark-jotform-api-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.044218 crossmark-jotform-api-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.048914 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    10812 2023-04-25 03:47:53.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:48:25.056959 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     1896 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-25 03:48:25.000000 crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.0.6/LICENSE` & `crossmark-jotform-api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.0.6/PKG-INFO` & `crossmark-jotform-api-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.0.6/pyproject.toml` & `crossmark-jotform-api-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.0.6/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.0.7/src/crossmark_jotform_api/jotForm.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         self.submission_data["submissions"] = {}
         self.set_data()
         self.get_submission_ids()
 
     def __set_submission_data(self, submission_data):
         submissions_dict = {}
         for i in submission_data:
-            if i["id"] not in submissions_dict:
-                submissions_dict[i["id"]] = jotFormSubmission(i)
+            submissions_dict[i["id"]] = jotFormSubmission(i)
         return submissions_dict
 
     def get_submission_ids(self):
         self.update()
         for submission in self.submissions:
             self.submission_ids.append(submission["id"])
         return self.submission_ids
@@ -123,15 +122,18 @@
             self.url = "&".join(params)
         else:
             self.url += "&" + key + "=" + value
 
     def set_data(self):
         self.data = requests.get(self.url, timeout=15).json()
         re_count = self.data['resultSet']['count']
-        # count = self.get_submissions_count()
+        count = self.get_submissions_count()
+        print(f"count: {count}")
+        print(f"url: {self.url}")
+        print(f"re_count: {re_count}, self.submission_count: {self.submission_count}, self.submission_data: {len(self.submission_data['submissions'])}")
         self.submission_count += re_count
         self.submission_data["submissions"].update(
             self.__set_submission_data(
                 self.data['content']
             )
         )
         if re_count == self.data['resultSet']['limit']:
```

### Comparing `crossmark-jotform-api-0.0.6/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.0.7/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

