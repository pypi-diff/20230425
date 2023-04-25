# Comparing `tmp/py-sls-lambda-toolkit-0.0.3.tar.gz` & `tmp/py-sls-lambda-toolkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sls-lambda-toolkit-0.0.3.tar", last modified: Sun Apr 23 18:26:19 2023, max compression
+gzip compressed data, was "py-sls-lambda-toolkit-0.0.4.tar", last modified: Tue Apr 25 01:46:58 2023, max compression
```

## Comparing `py-sls-lambda-toolkit-0.0.3.tar` & `py-sls-lambda-toolkit-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.3/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.3/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/PKG-INFO
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/
--rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/logger.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3350 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      604 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       33 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.3/pyproject.toml
--rw-rw-r--   0 julio     (1000) julio     (1000)      927 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/setup.cfg
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-25 01:46:58.951875 py-sls-lambda-toolkit-0.0.4/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.4/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.4/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-25 01:46:58.951875 py-sls-lambda-toolkit-0.0.4/PKG-INFO
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-25 01:46:58.951875 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      433 2023-04-25 01:10:01.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/crypto.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/http_event.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-24 15:55:29.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/http_response.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/logger.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/parsers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/status_code.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/validators.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-25 01:46:58.951875 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-25 01:46:58.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      636 2023-04-25 01:46:58.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-25 01:46:58.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       72 2023-04-25 01:46:58.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-25 01:46:58.000000 py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.4/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)      967 2023-04-25 01:46:58.951875 py-sls-lambda-toolkit-0.0.4/setup.cfg
```

### Comparing `py-sls-lambda-toolkit-0.0.3/LICENSE` & `py-sls-lambda-toolkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/PKG-INFO` & `py-sls-lambda-toolkit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,9 @@
-import boto3
 from boto3.dynamodb.conditions import Attr
 
-session = boto3.Session(
-    region_name='us-east-1',
-    aws_access_key_id='AKIA342VTCVHNZ52EGFG',
-    aws_secret_access_key='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'
-)
-
-dynamodb = session.resource('dynamodb')
-table = dynamodb.Table('users-prod')
-
-
 def equal(filter_expression, attribute, value):
     if bool(filter_expression):
         filter_expression &= Attr(attribute).eq(value)
     else:
         filter_expression = Attr(attribute).eq(value)
 
     return filter_expression
```

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/PKG-INFO` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/SOURCES.txt` & `py-sls-lambda-toolkit-0.0.4/py_sls_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
 setup.cfg
 py_sls_lambda_toolkit/__init__.py
+py_sls_lambda_toolkit/crypto.py
 py_sls_lambda_toolkit/dynamodb_shortcuts.py
 py_sls_lambda_toolkit/http_event.py
 py_sls_lambda_toolkit/http_response.py
 py_sls_lambda_toolkit/logger.py
 py_sls_lambda_toolkit/parsers.py
 py_sls_lambda_toolkit/scan_filter_builder.py
 py_sls_lambda_toolkit/status_code.py
```

### Comparing `py-sls-lambda-toolkit-0.0.3/setup.cfg` & `py-sls-lambda-toolkit-0.0.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-sls-lambda-toolkit
-version = 0.0.3
+version = 0.0.4
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
@@ -25,16 +25,17 @@
 	dynamodb
 	toolkit
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	boto3
-	jsonschema
-	camel_converter
+	boto3==1.26.118
+	jsonschema==4.17.3
+	camel-converter==3.0.0
+	bcrypt==4.0.1
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

