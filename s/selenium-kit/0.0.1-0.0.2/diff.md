# Comparing `tmp/selenium-kit-0.0.1.tar.gz` & `tmp/selenium-kit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-kit-0.0.1.tar", last modified: Tue Apr 25 12:21:27 2023, max compression
+gzip compressed data, was "selenium-kit-0.0.2.tar", last modified: Tue Apr 25 12:23:35 2023, max compression
```

## Comparing `selenium-kit-0.0.1.tar` & `selenium-kit-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:21:27.635061 selenium-kit-0.0.1/
--rw-r--r--   0 evabotml-002   (501) staff       (20)     1066 2023-04-25 10:46:59.000000 selenium-kit-0.0.1/LICENSE
--rw-r--r--   0 evabotml-002   (501) staff       (20)     1051 2023-04-25 12:21:27.634918 selenium-kit-0.0.1/PKG-INFO
--rw-r--r--   0 evabotml-002   (501) staff       (20)      786 2023-04-25 11:08:02.000000 selenium-kit-0.0.1/README.md
-drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:21:27.633988 selenium-kit-0.0.1/selenium-kit/
--rw-r--r--   0 evabotml-002   (501) staff       (20)       37 2023-04-25 11:06:16.000000 selenium-kit-0.0.1/selenium-kit/__init__.py
--rw-r--r--   0 evabotml-002   (501) staff       (20)     1412 2023-04-25 11:02:52.000000 selenium-kit-0.0.1/selenium-kit/selenium.py
-drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:21:27.634710 selenium-kit-0.0.1/selenium_kit.egg-info/
--rw-r--r--   0 evabotml-002   (501) staff       (20)     1051 2023-04-25 12:21:27.000000 selenium-kit-0.0.1/selenium_kit.egg-info/PKG-INFO
--rw-r--r--   0 evabotml-002   (501) staff       (20)      220 2023-04-25 12:21:27.000000 selenium-kit-0.0.1/selenium_kit.egg-info/SOURCES.txt
--rw-r--r--   0 evabotml-002   (501) staff       (20)        1 2023-04-25 12:21:27.000000 selenium-kit-0.0.1/selenium_kit.egg-info/dependency_links.txt
--rw-r--r--   0 evabotml-002   (501) staff       (20)       13 2023-04-25 12:21:27.000000 selenium-kit-0.0.1/selenium_kit.egg-info/top_level.txt
--rw-r--r--   0 evabotml-002   (501) staff       (20)       38 2023-04-25 12:21:27.635100 selenium-kit-0.0.1/setup.cfg
--rw-r--r--   0 evabotml-002   (501) staff       (20)      521 2023-04-25 10:59:06.000000 selenium-kit-0.0.1/setup.py
+drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:23:35.588666 selenium-kit-0.0.2/
+-rw-r--r--   0 evabotml-002   (501) staff       (20)     1066 2023-04-25 10:46:59.000000 selenium-kit-0.0.2/LICENSE
+-rw-r--r--   0 evabotml-002   (501) staff       (20)     1064 2023-04-25 12:23:35.588517 selenium-kit-0.0.2/PKG-INFO
+-rw-r--r--   0 evabotml-002   (501) staff       (20)      799 2023-04-25 12:22:30.000000 selenium-kit-0.0.2/README.md
+drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:23:35.587510 selenium-kit-0.0.2/selenium-kit/
+-rw-r--r--   0 evabotml-002   (501) staff       (20)       37 2023-04-25 11:06:16.000000 selenium-kit-0.0.2/selenium-kit/__init__.py
+-rw-r--r--   0 evabotml-002   (501) staff       (20)     1412 2023-04-25 11:02:52.000000 selenium-kit-0.0.2/selenium-kit/selenium.py
+drwxr-xr-x   0 evabotml-002   (501) staff       (20)        0 2023-04-25 12:23:35.588251 selenium-kit-0.0.2/selenium_kit.egg-info/
+-rw-r--r--   0 evabotml-002   (501) staff       (20)     1064 2023-04-25 12:23:35.000000 selenium-kit-0.0.2/selenium_kit.egg-info/PKG-INFO
+-rw-r--r--   0 evabotml-002   (501) staff       (20)      220 2023-04-25 12:23:35.000000 selenium-kit-0.0.2/selenium_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 evabotml-002   (501) staff       (20)        1 2023-04-25 12:23:35.000000 selenium-kit-0.0.2/selenium_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 evabotml-002   (501) staff       (20)       13 2023-04-25 12:23:35.000000 selenium-kit-0.0.2/selenium_kit.egg-info/top_level.txt
+-rw-r--r--   0 evabotml-002   (501) staff       (20)       38 2023-04-25 12:23:35.588712 selenium-kit-0.0.2/setup.cfg
+-rw-r--r--   0 evabotml-002   (501) staff       (20)      521 2023-04-25 12:23:31.000000 selenium-kit-0.0.2/setup.py
```

### Comparing `selenium-kit-0.0.1/LICENSE` & `selenium-kit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-kit-0.0.1/PKG-INFO` & `selenium-kit-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-kit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Selenium kit
 Home-page: https://github.com/yash0307jain/selenium-kit
 Author: Yash Jain
 Author-email: yash0307jain@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 Selenium toolkit to download the selenium drivers automatically and to use the selenium drivers with all the necessary functions.
 
 Sample Code
 
 ```python
 # Import selenium drivers
-from selenium-kit import S
+from selenium-kit import SeleniumDriver
 
 # Create the selenium object
 selenium = SeleniumDriver()
 
 # Call the url
 url = "https://www.imdb.com/"
 selenium.callURL(url)
```

### Comparing `selenium-kit-0.0.1/README.md` & `selenium-kit-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Selenium toolkit to download the selenium drivers automatically and to use the selenium drivers with all the necessary functions.
 
 Sample Code
 
 ```python
 # Import selenium drivers
-from selenium-kit import S
+from selenium-kit import SeleniumDriver
 
 # Create the selenium object
 selenium = SeleniumDriver()
 
 # Call the url
 url = "https://www.imdb.com/"
 selenium.callURL(url)
```

### Comparing `selenium-kit-0.0.1/selenium-kit/selenium.py` & `selenium-kit-0.0.2/selenium-kit/selenium.py`

 * *Files identical despite different names*

### Comparing `selenium-kit-0.0.1/selenium_kit.egg-info/PKG-INFO` & `selenium-kit-0.0.2/selenium_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-kit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Selenium kit
 Home-page: https://github.com/yash0307jain/selenium-kit
 Author: Yash Jain
 Author-email: yash0307jain@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 Selenium toolkit to download the selenium drivers automatically and to use the selenium drivers with all the necessary functions.
 
 Sample Code
 
 ```python
 # Import selenium drivers
-from selenium-kit import S
+from selenium-kit import SeleniumDriver
 
 # Create the selenium object
 selenium = SeleniumDriver()
 
 # Call the url
 url = "https://www.imdb.com/"
 selenium.callURL(url)
```

### Comparing `selenium-kit-0.0.1/setup.py` & `selenium-kit-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="selenium-kit",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     author="Yash Jain",
     author_email="yash0307jain@gmail.com",
     description="Selenium kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

