# Comparing `tmp/terka-1.6.4.8.tar.gz` & `tmp/terka-1.6.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.8.tar", last modified: Mon Apr 24 19:07:00 2023, max compression
+gzip compressed data, was "terka-1.6.4.9.tar", last modified: Mon Apr 24 19:07:55 2023, max compression
```

## Comparing `terka-1.6.4.8.tar` & `terka-1.6.4.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.631281 terka-1.6.4.8/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:00.627281 terka-1.6.4.8/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-24 19:07:00.631281 terka-1.6.4.8/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      905 2023-04-24 19:06:52.000000 terka-1.6.4.8/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.8/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.8/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.8/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.8/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.8/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.8/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.8/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.8/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.8/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.8/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.8/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.8/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.8/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.8/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.8/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.8/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.8/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.8/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2182 2023-04-24 19:06:39.000000 terka-1.6.4.8/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.8/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.8/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.8/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.8/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.8/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.8/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.8/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.8/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.8/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-24 18:36:30.000000 terka-1.6.4.8/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-23 14:24:46.000000 terka-1.6.4.8/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:00.627281 terka-1.6.4.8/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-24 19:07:00.000000 terka-1.6.4.8/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:55.551545 terka-1.6.4.9/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-24 19:07:55.551545 terka-1.6.4.9/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      905 2023-04-24 19:07:53.000000 terka-1.6.4.9/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.9/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.9/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.9/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.9/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.9/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.9/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.9/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.9/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.9/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.9/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.9/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.9/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.9/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.9/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.9/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2120 2023-04-24 19:07:46.000000 terka-1.6.4.9/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.9/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.9/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.9/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.9/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.9/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.9/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.9/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.9/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-24 18:36:30.000000 terka-1.6.4.9/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-23 14:24:46.000000 terka-1.6.4.9/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/top_level.txt
```

### Comparing `terka-1.6.4.8/setup.py` & `terka-1.6.4.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4.8",
+    version="1.6.4.9",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.4.8/terka/adapters/orm.py` & `terka-1.6.4.9/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/adapters/repository.py` & `terka-1.6.4.9/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/collaborators.py` & `terka-1.6.4.9/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/commands.py` & `terka-1.6.4.9/terka/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/commentary.py` & `terka-1.6.4.9/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/epic.py` & `terka-1.6.4.9/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/event_history.py` & `terka-1.6.4.9/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/project.py` & `terka-1.6.4.9/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/sprint.py` & `terka-1.6.4.9/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/story.py` & `terka-1.6.4.9/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/tag.py` & `terka-1.6.4.9/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/domain/task.py` & `terka-1.6.4.9/terka/domain/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,16 +52,14 @@
         else:
             self.due_date = due_date
         self.status = self._validate_status(status)
         if priority and priority not in [p.name for p in TaskPriority]:
             raise ValueError(f"{priority} is invalid priority")
         else:
             self.priority = priority
-        self.commentaries  = None
-        self.history = None
 
     @property
     def last_modified(self):
         # TODO: return 
         pass
 
     def _validate_status(self, status):
```

### Comparing `terka-1.6.4.8/terka/domain/time_tracker.py` & `terka-1.6.4.9/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/entrypoints/cli.py` & `terka-1.6.4.9/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/service_layer/printer.py` & `terka-1.6.4.9/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/service_layer/services.py` & `terka-1.6.4.9/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/service_layer/ui.py` & `terka-1.6.4.9/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/service_layer/vertical_layout.css` & `terka-1.6.4.9/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/service_layer/views.py` & `terka-1.6.4.9/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka/utils.py` & `terka-1.6.4.9/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.8/terka.egg-info/SOURCES.txt` & `terka-1.6.4.9/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

