# Comparing `tmp/textual_datepicker-0.2.2.tar.gz` & `tmp/textual_datepicker-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_datepicker-0.2.2.tar", max compression
+gzip compressed data, was "textual_datepicker-0.2.3.tar", max compression
```

## Comparing `textual_datepicker-0.2.2.tar` & `textual_datepicker-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2022-12-29 09:42:07.491839 textual_datepicker-0.2.2/LICENSE
--rw-r--r--   0        0        0     1234 2023-01-03 09:40:24.481457 textual_datepicker-0.2.2/README.md
--rw-r--r--   0        0        0     1052 2023-01-04 16:33:37.832941 textual_datepicker-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      160 2023-01-01 08:23:22.382258 textual_datepicker-0.2.2/textual_datepicker/__init__.py
--rw-r--r--   0        0        0    12732 2023-01-04 12:49:09.191848 textual_datepicker-0.2.2/textual_datepicker/_date_picker.py
--rw-r--r--   0        0        0     4777 2023-01-04 16:01:40.409212 textual_datepicker-0.2.2/textual_datepicker/_date_select.py
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 textual_datepicker-0.2.2/setup.py
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 textual_datepicker-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-12-29 09:42:07.491839 textual_datepicker-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1234 2023-01-03 09:40:24.481457 textual_datepicker-0.2.3/README.md
+-rw-r--r--   0        0        0     1072 2023-04-25 09:38:10.252606 textual_datepicker-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-01-01 08:23:22.382258 textual_datepicker-0.2.3/textual_datepicker/__init__.py
+-rw-r--r--   0        0        0    12732 2023-04-25 09:32:09.086266 textual_datepicker-0.2.3/textual_datepicker/_date_picker.py
+-rw-r--r--   0        0        0     4777 2023-01-04 16:01:40.409212 textual_datepicker-0.2.3/textual_datepicker/_date_select.py
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 textual_datepicker-0.2.3/setup.py
+-rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 textual_datepicker-0.2.3/PKG-INFO
```

### Comparing `textual_datepicker-0.2.2/LICENSE` & `textual_datepicker-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_datepicker-0.2.2/README.md` & `textual_datepicker-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `textual_datepicker-0.2.2/pyproject.toml` & `textual_datepicker-0.2.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-datepicker"
-version = "0.2.2"
+version = "0.2.3"
 description = "A datepicker widget for Textual."
 authors = ["Mischa Schindowski <mschindowski@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "textual_datepicker"}]
 repository = "https://github.com/mitosch/textual-datepicker"
 keywords = ["textual", "textual datepicker", "textual dateselect"]
@@ -20,18 +20,18 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pendulum = "*"
-textual = ">=0.6.0"
+textual = ">=0.10.0, <0.11.0"
 
 [tool.poetry.group.dev.dependencies]
-textual = { version = ">=0.6.0", extras = ["dev"] }
+textual = { version = ">=0.10.0, <0.11.0", extras = ["dev"] }
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `textual_datepicker-0.2.2/textual_datepicker/_date_picker.py` & `textual_datepicker-0.2.3/textual_datepicker/_date_picker.py`

 * *Files identical despite different names*

### Comparing `textual_datepicker-0.2.2/textual_datepicker/_date_select.py` & `textual_datepicker-0.2.3/textual_datepicker/_date_select.py`

 * *Files identical despite different names*

### Comparing `textual_datepicker-0.2.2/setup.py` & `textual_datepicker-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['textual_datepicker']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pendulum', 'textual>=0.6.0']
+['pendulum', 'textual>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'textual-datepicker',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A datepicker widget for Textual.',
     'long_description': '# Textual: DatePicker\n\nA DatePicker widget for [textual](https://github.com/Textualize/textual). It can be used standalone or with a DateSelect opening the dialog.\n\nDateSelect with DatePicker example:\n\n![DateSelect with DatePicker](https://user-images.githubusercontent.com/922559/209947716-3ee53f74-4d98-4d9c-a261-afb84955d519.png)\n\n\n## Usage\n\n```python\nfrom textual_datepicker import DateSelect\n\nDateSelect(\n  placeholder="please select",\n  format="YYYY-MM-DD",\n  picker_mount="#main_container"\n)\n```\n\nDefine an inital value:\n\n```python\nimport pendulum\nfrom textual_datepicker import DateSelect\n\nDateSelect(\n  placeholder="please select",\n  format="YYYY-MM-DD",\n  date=pendulum.parse("2023-02-14"),\n  picker_mount="#main_container"\n)\n```\n\n## Installation\n\n```bash\npip install textual-datepicker\n```\n\nRequires textual 0.6.0 or later.\n\n## Limitations\n\nThis textual widget is in early stage and has some limitations:\n\n* It can only open below, not above: Make sure to reserve space below for the dialog.\n* It needs a specific mount point (`picker_mount`) where the dialog\n  shall appear. This is needed because the container widget with the select\n  itself could be too small. Maybe in future versions this will no longer be\n  needed.\n',
     'author': 'Mischa Schindowski',
     'author_email': 'mschindowski@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mitosch/textual-datepicker',
```

### Comparing `textual_datepicker-0.2.2/PKG-INFO` & `textual_datepicker-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-datepicker
-Version: 0.2.2
+Version: 0.2.3
 Summary: A datepicker widget for Textual.
 Home-page: https://github.com/mitosch/textual-datepicker
 License: MIT
 Keywords: textual,textual datepicker,textual dateselect
 Author: Mischa Schindowski
 Author-email: mschindowski@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pendulum
-Requires-Dist: textual (>=0.6.0)
+Requires-Dist: textual (>=0.10.0,<0.11.0)
 Project-URL: Repository, https://github.com/mitosch/textual-datepicker
 Description-Content-Type: text/markdown
 
 # Textual: DatePicker
 
 A DatePicker widget for [textual](https://github.com/Textualize/textual). It can be used standalone or with a DateSelect opening the dialog.
```

