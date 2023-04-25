# Comparing `tmp/assignment-manager-0.1.0.tar.gz` & `tmp/assignment-manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.0.tar", last modified: Mon Apr 24 15:51:24 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.1.tar", last modified: Tue Apr 25 10:04:34 2023, max compression
```

## Comparing `assignment-manager-0.1.0.tar` & `assignment-manager-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.0/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       38 2023-04-24 09:48:54.000000 assignment-manager-0.1.0/MANIFEST.in
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.0/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       98 2023-04-23 16:36:52.000000 assignment-manager-0.1.0/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-24 15:51:08.000000 assignment-manager-0.1.0/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.0/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2793 2023-04-24 15:50:04.000000 assignment-manager-0.1.0/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      110 2023-04-24 15:46:58.000000 assignment-manager-0.1.0/src/assignment_manager/data.json
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      472 2023-04-24 09:54:30.000000 assignment-manager-0.1.0/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2210 2023-04-24 15:48:57.000000 assignment-manager-0.1.0/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      540 2023-04-24 15:44:30.000000 assignment-manager-0.1.0/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-24 15:51:24.769129 assignment-manager-0.1.0/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      538 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-24 15:51:24.000000 assignment-manager-0.1.0/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 10:04:34.044094 assignment-manager-0.1.1/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.1/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       38 2023-04-24 09:48:54.000000 assignment-manager-0.1.1/MANIFEST.in
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-25 10:04:34.044094 assignment-manager-0.1.1/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.1/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       98 2023-04-23 16:36:52.000000 assignment-manager-0.1.1/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-25 10:04:34.044094 assignment-manager-0.1.1/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-25 09:55:30.000000 assignment-manager-0.1.1/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 10:04:34.040094 assignment-manager-0.1.1/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 10:04:34.040094 assignment-manager-0.1.1/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.1/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2570 2023-04-25 09:44:09.000000 assignment-manager-0.1.1/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1284 2023-04-24 16:12:41.000000 assignment-manager-0.1.1/src/assignment_manager/data.json
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      472 2023-04-24 09:54:30.000000 assignment-manager-0.1.1/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2210 2023-04-24 15:48:57.000000 assignment-manager-0.1.1/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      535 2023-04-25 09:52:52.000000 assignment-manager-0.1.1/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 10:04:34.044094 assignment-manager-0.1.1/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      538 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-25 10:04:34.000000 assignment-manager-0.1.1/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.0/LICENSE` & `assignment-manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.0/PKG-INFO` & `assignment-manager-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.0/setup.py` & `assignment-manager-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.0",
+    version="0.1.1",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.0/src/assignment_manager/assignments.py` & `assignment-manager-0.1.1/src/assignment_manager/assignments.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,17 @@
                 data[key][cycle][1],
                 Progress(data[key][cycle][2]).name,
             ]
         )
     io.print_table(table_headers, table_rows)
 
 
-def show_specific_assignment(name):
+def show_specific_assignment():
     data = load_data()
-    if not name in data:
-        raise ValueError("The given course doesn't exist", name)
+    name = io.course_response(data.keys())
 
     table_headers = ["Start", "Deadline", "Progress"]
     table_rows = []
     for data_entry in data[name]:
         table_rows.append([data_entry[0], data_entry[1], Progress(data_entry[2]).name])
     io.print_table(table_headers, table_rows)
 
@@ -65,30 +64,26 @@
     data[params[0]] = progress
     write_data(data)
 
 
 def update_assignment():
     data = load_data()
     name = io.course_response(data.keys())
-    if name not in data.keys():
-        raise ValueError("Name doesn't exist!", name)
 
     cycle_choices = [d for d in data[name]]
     progress_choices = [p.name for p in Progress]
     cycle, progress = io.update_assignment_response(cycle_choices, progress_choices)
 
     data[name][cycle][2] = progress
     write_data(data)
 
 
 def remove_assignment():
     data = load_data()
     name = io.course_response(data.keys())
-    if name not in data.keys():
-        raise ValueError("Name doesn't exist!", name)
 
     confirmation_msg = "This will delete [bold]ALL[/bold] data for the course: [bold]{}[/bold]\n".format(
         name
     )
 
     if not io.confirmation_prompt(confirmation_msg):
         return
```

### Comparing `assignment-manager-0.1.0/src/assignment_manager/io.py` & `assignment-manager-0.1.1/src/assignment_manager/io.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.0/src/assignment_manager/main.py` & `assignment-manager-0.1.1/src/assignment_manager/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 @app.command()
 def add():
     assignments.add_assignment()
 
 
 @app.command()
-def show(name=""):
-    if name == "":
+def show(one:bool=False):
+    if one:
+        assignments.show_specific_assignment()
+    else:
         assignments.show_all_assignments()
-        return
-    assignments.show_specific_assignment(name)
 
 
 @app.command()
 def update():
     assignments.update_assignment()
```

### Comparing `assignment-manager-0.1.0/src/assignment_manager.egg-info/PKG-INFO` & `assignment-manager-0.1.1/src/assignment_manager.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.0/src/assignment_manager.egg-info/SOURCES.txt` & `assignment-manager-0.1.1/src/assignment_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

