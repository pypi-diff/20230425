# Comparing `tmp/clevertable-1.0.0.tar.gz` & `tmp/clevertable-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-1.0.0.tar", last modified: Fri Apr 21 12:26:16 2023, max compression
+gzip compressed data, was "clevertable-1.0.1.tar", last modified: Tue Apr 25 10:21:26 2023, max compression
```

## Comparing `clevertable-1.0.0.tar` & `clevertable-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 12:26:16.851981 clevertable-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9886 2023-04-21 12:26:16.851981 clevertable-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8137 2023-04-21 11:55:46.000000 clevertable-1.0.0/README.md
--rw-rw-rw-   0        0        0     1054 2023-04-21 11:55:46.000000 clevertable-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 12:26:16.851981 clevertable-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 12:26:16.820733 clevertable-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 12:26:16.836356 clevertable-1.0.0/src/clevertable/
--rw-rw-rw-   0        0        0       78 2023-04-21 12:02:37.000000 clevertable-1.0.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1355 2023-04-21 12:02:48.000000 clevertable-1.0.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0    12028 2023-04-21 11:55:46.000000 clevertable-1.0.0/src/clevertable/numerical_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 12:26:16.851981 clevertable-1.0.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0     9886 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 12:26:16.000000 clevertable-1.0.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:21:26.484122 clevertable-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10159 2023-04-25 10:21:26.484122 clevertable-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8410 2023-04-21 12:40:19.000000 clevertable-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1079 2023-04-25 10:18:47.000000 clevertable-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:21:26.484122 clevertable-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:21:26.436741 clevertable-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 10:21:26.468486 clevertable-1.0.1/src/clevertable/
+-rw-rw-rw-   0        0        0       78 2023-04-25 10:07:15.000000 clevertable-1.0.1/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1355 2023-04-21 12:02:48.000000 clevertable-1.0.1/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0    12100 2023-04-25 10:04:16.000000 clevertable-1.0.1/src/clevertable/numerical_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:21:26.484122 clevertable-1.0.1/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    10159 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 10:21:26.000000 clevertable-1.0.1/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-1.0.0/LICENSE` & `clevertable-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-1.0.0/PKG-INFO` & `clevertable-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -98,14 +98,22 @@
 to the constructor:
 ```python
 nc = NumericalConverter(ignore_unknown=True)
 ```
 However, it is safer to explicitly set the conversion
 method to `"ignore"` for all columns you want to ignore.
 
+## CLI
+
+`pip install clevertable` also makes the command `clevertable` available
+in the command line.
+It allows to quickly convert tables without even creating a Python script.
+Execute `clevertable -h` to see the possible arguments that can be passed
+to the tool.
+
 ## Supported Conversion Methods
 
 ### ignore
 
 Drops the column.
 
 ```python
```

### Comparing `clevertable-1.0.0/README.md` & `clevertable-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,22 @@
 to the constructor:
 ```python
 nc = NumericalConverter(ignore_unknown=True)
 ```
 However, it is safer to explicitly set the conversion
 method to `"ignore"` for all columns you want to ignore.
 
+## CLI
+
+`pip install clevertable` also makes the command `clevertable` available
+in the command line.
+It allows to quickly convert tables without even creating a Python script.
+Execute `clevertable -h` to see the possible arguments that can be passed
+to the tool.
+
 ## Supported Conversion Methods
 
 ### ignore
 
 Drops the column.
 
 ```python
```

### Comparing `clevertable-1.0.0/pyproject.toml` & `clevertable-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "1.0.0"
+version = "1.0.1"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,17 +24,17 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"']
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/clevertable/__init__.py" = ["{version}"]
```

### Comparing `clevertable-1.0.0/src/clevertable/__main__.py` & `clevertable-1.0.1/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-1.0.0/src/clevertable/numerical_converter.py` & `clevertable-1.0.1/src/clevertable/numerical_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
                 fixes = list(prefixes) + list(suffixes)
                 replace_expression = "|".join(fixes)
                 split_col = split_col.map(lambda l: [re.sub(replace_expression, "", s) for s in l])
 
                 if "values" not in args:
                     # infer values from data
                     possible_values = set(split_col.explode().unique())
+                    possible_values = possible_values.difference({""})
                     args["values"] = possible_values
                 for value in args["values"]:
                     new_df[f"{col_name}={value}"] = split_col.apply(lambda x: value in x)
                 continue
 
             if method == "map":
                 if "func" not in args:
```

### Comparing `clevertable-1.0.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-1.0.1/src/clevertable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -98,14 +98,22 @@
 to the constructor:
 ```python
 nc = NumericalConverter(ignore_unknown=True)
 ```
 However, it is safer to explicitly set the conversion
 method to `"ignore"` for all columns you want to ignore.
 
+## CLI
+
+`pip install clevertable` also makes the command `clevertable` available
+in the command line.
+It allows to quickly convert tables without even creating a Python script.
+Execute `clevertable -h` to see the possible arguments that can be passed
+to the tool.
+
 ## Supported Conversion Methods
 
 ### ignore
 
 Drops the column.
 
 ```python
```

