# Comparing `tmp/hey-mindsdb-0.0.2.tar.gz` & `tmp/hey-mindsdb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hey-mindsdb-0.0.2.tar", last modified: Sun Apr 23 08:05:24 2023, max compression
+gzip compressed data, was "hey-mindsdb-0.1.0.tar", last modified: Tue Apr 25 10:28:06 2023, max compression
```

## Comparing `hey-mindsdb-0.0.2.tar` & `hey-mindsdb-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437730 hey-mindsdb-0.0.2/
--rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey-mindsdb-0.0.2/LICENSE
--rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey-mindsdb-0.0.2/MANIFEST.in
--rw-r--r--   0 sadra      (501) staff       (20)     5060 2023-04-23 08:05:24.437778 hey-mindsdb-0.0.2/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)     3861 2023-04-23 08:00:16.000000 hey-mindsdb-0.0.2/README.md
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.434116 hey-mindsdb-0.0.2/hey/
--rw-r--r--   0 sadra      (501) staff       (20)      126 2023-04-23 08:05:04.000000 hey-mindsdb-0.0.2/hey/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2780 2023-04-23 05:58:41.000000 hey-mindsdb-0.0.2/hey/cli.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.434986 hey-mindsdb-0.0.2/hey/constants/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey-mindsdb-0.0.2/hey/constants/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      594 2023-04-22 16:01:00.000000 hey-mindsdb-0.0.2/hey/constants/informations.py
--rw-r--r--   0 sadra      (501) staff       (20)      130 2023-04-22 08:20:35.000000 hey-mindsdb-0.0.2/hey/constants/service.py
--rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey-mindsdb-0.0.2/hey/constants/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.435822 hey-mindsdb-0.0.2/hey/exceptions/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey-mindsdb-0.0.2/hey/exceptions/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey-mindsdb-0.0.2/hey/exceptions/auth.py
--rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey-mindsdb-0.0.2/hey/exceptions/connection.py
--rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey-mindsdb-0.0.2/hey/exceptions/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.436225 hey-mindsdb-0.0.2/hey/middlewares/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey-mindsdb-0.0.2/hey/middlewares/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2498 2023-04-23 06:45:03.000000 hey-mindsdb-0.0.2/hey/middlewares/mindsdb.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437190 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/
--rw-r--r--   0 sadra      (501) staff       (20)     5060 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)      626 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/SOURCES.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/dependency_links.txt
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/entry_points.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/not-zip-safe
--rw-r--r--   0 sadra      (501) staff       (20)       49 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/requires.txt
--rw-r--r--   0 sadra      (501) staff       (20)        4 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/top_level.txt
--rw-r--r--   0 sadra      (501) staff       (20)     1660 2023-04-23 08:05:24.438049 hey-mindsdb-0.0.2/setup.cfg
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey-mindsdb-0.0.2/setup.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437511 hey-mindsdb-0.0.2/tests/
--rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey-mindsdb-0.0.2/tests/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey-mindsdb-0.0.2/tests/test_accounts.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.957208 hey-mindsdb-0.1.0/
+-rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey-mindsdb-0.1.0/LICENSE
+-rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey-mindsdb-0.1.0/MANIFEST.in
+-rw-r--r--   0 sadra      (501) staff       (20)     5163 2023-04-25 10:28:06.957273 hey-mindsdb-0.1.0/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)     3964 2023-04-24 08:41:20.000000 hey-mindsdb-0.1.0/README.md
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.952882 hey-mindsdb-0.1.0/hey/
+-rw-r--r--   0 sadra      (501) staff       (20)      126 2023-04-25 10:27:53.000000 hey-mindsdb-0.1.0/hey/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2780 2023-04-23 05:58:41.000000 hey-mindsdb-0.1.0/hey/cli.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.953901 hey-mindsdb-0.1.0/hey/constants/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey-mindsdb-0.1.0/hey/constants/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      550 2023-04-23 16:07:39.000000 hey-mindsdb-0.1.0/hey/constants/informations.py
+-rw-r--r--   0 sadra      (501) staff       (20)      130 2023-04-22 08:20:35.000000 hey-mindsdb-0.1.0/hey/constants/service.py
+-rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey-mindsdb-0.1.0/hey/constants/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.954701 hey-mindsdb-0.1.0/hey/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey-mindsdb-0.1.0/hey/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey-mindsdb-0.1.0/hey/exceptions/auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey-mindsdb-0.1.0/hey/exceptions/connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey-mindsdb-0.1.0/hey/exceptions/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.955058 hey-mindsdb-0.1.0/hey/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey-mindsdb-0.1.0/hey/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2607 2023-04-24 16:07:38.000000 hey-mindsdb-0.1.0/hey/middlewares/mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.955362 hey-mindsdb-0.1.0/hey/templates/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-24 06:30:05.000000 hey-mindsdb-0.1.0/hey/templates/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      153 2023-04-24 07:25:14.000000 hey-mindsdb-0.1.0/hey/templates/mindsdb_queries.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.956609 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/
+-rw-r--r--   0 sadra      (501) staff       (20)     5163 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)      685 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/entry_points.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/not-zip-safe
+-rw-r--r--   0 sadra      (501) staff       (20)       49 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/requires.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        4 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/top_level.txt
+-rw-r--r--   0 sadra      (501) staff       (20)     1660 2023-04-25 10:28:06.957593 hey-mindsdb-0.1.0/setup.cfg
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey-mindsdb-0.1.0/setup.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.956975 hey-mindsdb-0.1.0/tests/
+-rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey-mindsdb-0.1.0/tests/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey-mindsdb-0.1.0/tests/test_accounts.py
```

### Comparing `hey-mindsdb-0.0.2/LICENSE` & `hey-mindsdb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.2/PKG-INFO` & `hey-mindsdb-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hey-mindsdb
-Version: 0.0.2
+Version: 0.1.0
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
 License: MIT license
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
@@ -51,14 +51,16 @@
 ```
 
 ##### Option B - Download from GitHub archive
 ```sh
 pip install git+http://github.com/lnxpy/hey.git
 ```
 
+> :warning:: Hey is POSIX-friendly. It might not work properly on the Windows machines at the moment.
+
 </details>
 
 <details>
   <summary><h4>2. Set the <code>MINDSDB_EMAIL_ADDRESS</code> environment variable</h4></summary>
 
 Once you got the package installed on your system, it's time to add the `MINDSDB_EMAIL_ADDRESS` environment variable. Create an account on [mindsdb.com](https://mindsdb.com/), train your GPT model and replace your email with `<EMAIL>` in the following options.
```

### Comparing `hey-mindsdb-0.0.2/README.md` & `hey-mindsdb-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 ```
 
 ##### Option B - Download from GitHub archive
 ```sh
 pip install git+http://github.com/lnxpy/hey.git
 ```
 
+> :warning:: Hey is POSIX-friendly. It might not work properly on the Windows machines at the moment.
+
 </details>
 
 <details>
   <summary><h4>2. Set the <code>MINDSDB_EMAIL_ADDRESS</code> environment variable</h4></summary>
 
 Once you got the package installed on your system, it's time to add the `MINDSDB_EMAIL_ADDRESS` environment variable. Create an account on [mindsdb.com](https://mindsdb.com/), train your GPT model and replace your email with `<EMAIL>` in the following options.
```

### Comparing `hey-mindsdb-0.0.2/hey/cli.py` & `hey-mindsdb-0.1.0/hey/cli.py`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.2/hey/constants/informations.py` & `hey-mindsdb-0.1.0/hey/constants/informations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # package description for argparse
 APPLICATION_DESCRIPTION = 'Hey is your AI-powered pair programming friend that helps you speed up your productivity.'
 
 # link to installation guide
-INSTALLATION_GUIDE = 'Check out https://imsadra/introducing-hey-your-ai-powered-pair-programming-friend/ for ' \
+INSTALLATION_GUIDE = 'Check out https://github.com/lnxpy/hey for ' \
                      'installation guide. '
 
 # epilog information
 EPILOG_DESCRIPTION = 'Hey is designed for Hashnode X MindsDB hackathon.'
 
 # `--version` option output pattern
 VERSION_INFO = '''
```

### Comparing `hey-mindsdb-0.0.2/hey/middlewares/mindsdb.py` & `hey-mindsdb-0.1.0/hey/middlewares/mindsdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,38 @@
+from getpass import getuser
+
 import mindsdb_sdk
 from mindsdb_sdk.server import Server, Database
 from pandas import DataFrame
 from requests.exceptions import HTTPError, ConnectionError
 from rich.markdown import Markdown
 
 from hey.constants.service import MINDSDB_HOST
 from hey.exceptions.auth import CredentialsError
 from hey.exceptions.connection import NetworkError
+from hey.templates.mindsdb_queries import SQL_ASK_QUERY
 
 
 def to_data(dataframe: DataFrame) -> str:
     """
-    takes a pandas dataframe and returns the first value from the first column
+    takes a pandas `DataFrame` and returns the first value from the first column
     Args:
-        dataframe:
+        dataframe: the dataframe returned from MindsDB that stores the answer in the first cell of column
 
     Returns:
-        first value of the first column of dataframe that GPT responses
+        first value of the first column of dataframe that MindsDB responses
     """
     return dataframe.iloc[:, 0].values[0]
 
 
 class MindsDB:
     """
     MindsDB manager class
     """
 
-    SQL_ASKING_QUERY = '''
-    SELECT response
-    FROM mindsdb.gpt_model
-    WHERE author_username = "mindsdb"
-    AND text = "{}";
-    '''
-
     def __init__(self, email: str, password: str) -> None:
         """
         initializer class.
         Args:
             email: MindsDB account email address (that is stored as an env var)
             password: MindsDB account password
         """
@@ -76,12 +72,16 @@
         takes the question and queries then converts the response into `rich.Markdown`
         Args:
             question: the value from `ask` positional argument
 
         Returns:
             response from MindsDB in Markdown format
         """
+
         return Markdown(to_data(
             self.database.query(
-                MindsDB.SQL_ASKING_QUERY.format(question)
+                SQL_ASK_QUERY.substitute(
+                    ask=question,
+                    user=getuser(),
+                )
             ).fetch()
         ))
```

### Comparing `hey-mindsdb-0.0.2/hey_mindsdb.egg-info/PKG-INFO` & `hey-mindsdb-0.1.0/hey_mindsdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hey-mindsdb
-Version: 0.0.2
+Version: 0.1.0
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
 License: MIT license
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
@@ -51,14 +51,16 @@
 ```
 
 ##### Option B - Download from GitHub archive
 ```sh
 pip install git+http://github.com/lnxpy/hey.git
 ```
 
+> :warning:: Hey is POSIX-friendly. It might not work properly on the Windows machines at the moment.
+
 </details>
 
 <details>
   <summary><h4>2. Set the <code>MINDSDB_EMAIL_ADDRESS</code> environment variable</h4></summary>
 
 Once you got the package installed on your system, it's time to add the `MINDSDB_EMAIL_ADDRESS` environment variable. Create an account on [mindsdb.com](https://mindsdb.com/), train your GPT model and replace your email with `<EMAIL>` in the following options.
```

### Comparing `hey-mindsdb-0.0.2/setup.cfg` & `hey-mindsdb-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 description = Your AI-powered pair programming friend.
 license = MIT license
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = hey
 name = hey-mindsdb
 url = https://github.com/lnxpy/hey
-version = 0.0.2
+version = 0.1.0
 
 [options]
 python_requires = >=3.6
 install_requires = 
 	mindsdb-sdk>=1.0.2
 	keyring>=23.13.1
 	rich>=13.3.4
@@ -45,15 +45,15 @@
 	hey.*
 
 [options.entry_points]
 console_scripts = 
 	hey=hey.cli:main
 
 [bumpversion]
-current_version = 0.0.2
+current_version = 0.1.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

