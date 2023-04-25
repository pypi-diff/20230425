# Comparing `tmp/aracnid_api-1.5.0.tar.gz` & `tmp/aracnid_api-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aracnid_api-1.5.0.tar", last modified: Fri Dec 17 20:13:54 2021, max compression
+gzip compressed data, was "aracnid_api-1.6.0.tar", max compression
```

## Comparing `aracnid_api-1.5.0.tar` & `aracnid_api-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rw-r--r--   0        0        0       87 2021-11-25 15:24:54.415552 aracnid_api-1.5.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-08-22 21:27:12.749605 aracnid_api-1.5.0/LICENSE
--rw-r--r--   0        0        0      355 2021-11-25 15:28:19.285530 aracnid_api-1.5.0/Pipfile
--rw-r--r--   0        0        0    11065 2021-11-25 15:29:05.385942 aracnid_api-1.5.0/Pipfile.lock
--rw-r--r--   0        0        0      972 2020-11-29 15:41:24.230790 aracnid_api-1.5.0/README.md
--rw-r--r--   0        0        0      136 2021-12-17 20:13:12.686029 aracnid_api-1.5.0/aracnid_api/__init__.py
--rw-r--r--   0        0        0     5932 2021-12-17 20:11:59.177609 aracnid_api-1.5.0/aracnid_api/i_airtable.py
--rw-r--r--   0        0        0      582 2020-11-30 12:55:42.503492 aracnid_api-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       33 2020-08-04 14:09:04.249096 aracnid_api-1.5.0/pytest.ini
--rw-r--r--   0        0        0     4632 2021-12-17 20:10:15.409016 aracnid_api-1.5.0/tests/test_i_airtable.py
--rw-r--r--   0        0        0      186 2020-11-29 16:29:11.779525 aracnid_api-1.5.0/tests/test_init.py
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 aracnid_api-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-08-22 21:27:12.749605 aracnid_api-1.6.0/LICENSE
+-rw-r--r--   0        0        0      976 2023-04-25 12:37:38.605000 aracnid_api-1.6.0/README.md
+-rw-r--r--   0        0        0      136 2023-04-25 12:37:38.605000 aracnid_api-1.6.0/aracnid_api/__init__.py
+-rw-r--r--   0        0        0     5937 2023-04-25 12:37:38.605000 aracnid_api-1.6.0/aracnid_api/i_airtable.py
+-rw-r--r--   0        0        0      727 2023-04-25 12:37:38.605000 aracnid_api-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 aracnid_api-1.6.0/setup.py
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 aracnid_api-1.6.0/PKG-INFO
```

### Comparing `aracnid_api-1.5.0/LICENSE` & `aracnid_api-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aracnid_api-1.5.0/README.md` & `aracnid_api-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 
 This package supports the following version of Python:
 
-- Python 3.8 or later
+- Python 3.10 or later
 
 ### Installing
 
-Install the latest package using pip. (We prefer pipenv.)
+Install the latest package using pip. (We prefer poetry.)
 
 ```
-$ pip install aracnid-api
+$ poetry install aracnid-api
 ```
 
 End with an example of getting some data out of the system or using it for a little demo
 
 ## Running the tests
 
 Explain how to run the automated tests for this system
```

### Comparing `aracnid_api-1.5.0/aracnid_api/i_airtable.py` & `aracnid_api-1.6.0/aracnid_api/i_airtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,23 +139,24 @@
         Args:
             table: The Airtable Table object.
             fields: The fields for the created record.
         """
         record = None
 
         record = table.insert(fields)
-        
+
         return record
 
     @classmethod
     def match_record(cls, table, field_name, field_value):
         """Returns a record that matches the specified field name and value.
 
         Tried using the .match() method, but this failed when apostrophes are passed.
-        I updated the source code for C:\\Users\\Public\\Documents\\dev\\virtualenvs\\labdb\\Lib\\site-packages\\airtable\\params.py
+        I updated the source code for C:\\Users\\Public\\Documents
+            \\dev\\virtualenvs\\labdb\\Lib\\site-packages\\airtable\\params.py
         I updated line 210 to the following, swapping the quotes around.
         field_value = '"{}"'.format(field_value)
         This will work for apostrophes now, but will fail on double quotes.
 
         Args:
             table: The Airtable Table object.
             field_name: The name of the record's field.
```

### Comparing `aracnid_api-1.5.0/PKG-INFO` & `aracnid_api-1.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 Metadata-Version: 2.1
-Name: aracnid_api
-Version: 1.5.0
-Summary: A simple customization of the Python Logging System.
+Name: aracnid-api
+Version: 1.6.0
+Summary: This package contains custom wrappers around a variety of Web App APIs.
 Home-page: https://github.com/aracnid/aracnid-api
-Keywords: api
+License: MIT
+Keywords: api,airtable
 Author: Jason Romano
 Author-email: aracnid@gmail.com
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: airtable-python-wrapper ~=0.15
-Requires-Dist: aracnid-logger
-Requires-Dist: python-dateutil ~=2.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airtable-python-wrapper (>=0.15,<0.16)
+Requires-Dist: aracnid-logger (>=1.0,<2.0)
+Requires-Dist: python-dateutil (==2.8.2)
+Project-URL: Repository, https://github.com/aracnid/aracnid-api
+Description-Content-Type: text/markdown
 
 # Aracnid API
 
 This package contains custom wrappers around a variety of Web App APIs.
 
 ## Getting Started
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 
 This package supports the following version of Python:
 
-- Python 3.8 or later
+- Python 3.10 or later
 
 ### Installing
 
-Install the latest package using pip. (We prefer pipenv.)
+Install the latest package using pip. (We prefer poetry.)
 
 ```
-$ pip install aracnid-api
+$ poetry install aracnid-api
 ```
 
 End with an example of getting some data out of the system or using it for a little demo
 
 ## Running the tests
 
 Explain how to run the automated tests for this system
```

