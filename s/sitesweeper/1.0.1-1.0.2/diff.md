# Comparing `tmp/sitesweeper-1.0.1.tar.gz` & `tmp/sitesweeper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesweeper-1.0.1.tar", last modified: Tue Apr 25 08:42:08 2023, max compression
+gzip compressed data, was "sitesweeper-1.0.2.tar", last modified: Tue Apr 25 08:47:57 2023, max compression
```

## Comparing `sitesweeper-1.0.1.tar` & `sitesweeper-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.941511 sitesweeper-1.0.1/sitesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/sitesweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:47:57.330422 sitesweeper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 08:47:57.330422 sitesweeper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-25 08:47:44.000000 sitesweeper-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:47:57.330422 sitesweeper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 08:47:44.000000 sitesweeper-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:47:57.330422 sitesweeper-1.0.2/sitesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:47:44.000000 sitesweeper-1.0.2/sitesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 08:47:44.000000 sitesweeper-1.0.2/sitesweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-25 08:47:44.000000 sitesweeper-1.0.2/sitesweeper/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:47:57.330422 sitesweeper-1.0.2/sitesweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 08:47:57.000000 sitesweeper-1.0.2/sitesweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:47:57.000000 sitesweeper-1.0.2/sitesweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:47:57.000000 sitesweeper-1.0.2/sitesweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:47:57.000000 sitesweeper-1.0.2/sitesweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:47:57.000000 sitesweeper-1.0.2/sitesweeper.egg-info/top_level.txt
```

### Comparing `sitesweeper-1.0.1/PKG-INFO` & `sitesweeper-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesweeper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file
 Home-page: https://github.com/radityaharya/sitesweeper
 Author: Raditya Harya
 Author-email: contact@radityaharya.com
 Description-Content-Type: text/markdown
 
 
@@ -20,10 +20,10 @@
 ```bash
   pip install sitesweeper
 ```
     
 ## Usage
 
 ```bash
-sitesweeper https://example.com --output-path example
+python3.9 -m sitesweeper https://example.com --output-path example
 ```
```

### Comparing `sitesweeper-1.0.1/setup.py` & `sitesweeper-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_description = fh.read()
 else:
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
     name="sitesweeper",
-    version="1.0.1",
+    version="1.0.2",
     description="Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Raditya Harya",
     author_email="contact@radityaharya.com",
     url="https://github.com/radityaharya/sitesweeper",
     packages=find_packages(),
```

### Comparing `sitesweeper-1.0.1/sitesweeper/__main__.py` & `sitesweeper-1.0.2/sitesweeper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,54 +11,54 @@
 logger.setLevel(logging.DEBUG)
 logger.addHandler(RichHandler())
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Crawl a website and generate a PDF file"
     )
-    parser.add_argument("start-url", type=str, help="The starting URL for the crawl")
+    parser.add_argument("start_url", type=str, help="The starting URL for the crawl")
     parser.add_argument(
-        "--base-path", type=str, default="/", help="The base path for the crawl"
+        "--base_path", type=str, default="/", help="The base path for the crawl"
     )
     parser.add_argument(
         "--output-path",
         type=str,
         help="The output path for the PDF file (default: ./output)",
     )
     parser.add_argument(
         "--depth", type=int, default=100, help="The depth of the crawl (default: 100)"
     )
     parser.add_argument(
-        "--use-sitemap",
+        "--use_sitemap",
         action="store_true",
         help="Use the sitemap.xml file to crawl the website",
     )
     parser.add_argument(
-        "--merge-pdfs", action="store_true", help="Merge all PDF files into one"
+        "--merge_pdfs", action="store_true", help="Merge all PDF files into one"
     )
     parser.add_argument(
-        "--javascript-delay",
+        "--javascript_delay",
         type=int,
         default=3000,
         help="The delay for javascript to load (default: 3000)",
     )
     parser.add_argument(
-        "--page-size",
+        "--page_size",
         type=str,
         default="A4",
         help="The page size for the PDF (default: A4)",
     )
     parser.add_argument(
         "--encoding",
         type=str,
         default="UTF-8",
         help="The encoding for the PDF (default: UTF-8)",
     )
     parser.add_argument(
-        "--log-level", type=str, default="INFO", help="The log level (default: INFO)"
+        "--log_level", type=str, default="INFO", help="The log level (default: INFO)"
     )
     args = parser.parse_args()
 
     if args.output_path is None:
         args.output_path = os.getcwd() + "/output"
     
     if args.start_url.endswith("/"):
```

### Comparing `sitesweeper-1.0.1/sitesweeper/crawler.py` & `sitesweeper-1.0.2/sitesweeper/crawler.py`

 * *Files identical despite different names*

### Comparing `sitesweeper-1.0.1/sitesweeper.egg-info/PKG-INFO` & `sitesweeper-1.0.2/sitesweeper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesweeper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file
 Home-page: https://github.com/radityaharya/sitesweeper
 Author: Raditya Harya
 Author-email: contact@radityaharya.com
 Description-Content-Type: text/markdown
 
 
@@ -20,10 +20,10 @@
 ```bash
   pip install sitesweeper
 ```
     
 ## Usage
 
 ```bash
-sitesweeper https://example.com --output-path example
+python3.9 -m sitesweeper https://example.com --output-path example
 ```
```

