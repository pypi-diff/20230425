# Comparing `tmp/robocorp_browser-0.1.0.tar.gz` & `tmp/robocorp_browser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_browser-0.2.0.tar", max compression
```

## Comparing `robocorp_browser-0.1.0.tar` & `robocorp_browser-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       94 2023-04-04 11:49:45.057278 robocorp_browser-0.1.0/README.md
--rw-r--r--   0        0        0      565 2023-04-04 11:49:45.057874 robocorp_browser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-04-04 11:49:45.058240 robocorp_browser-0.1.0/src/robo/libs/browser/__init__.py
--rw-r--r--   0        0        0     2436 2023-04-04 11:49:45.058546 robocorp_browser-0.1.0/src/robo/libs/browser/browser.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 robocorp_browser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-04-04 11:49:45.057278 robocorp_browser-0.2.0/README.md
+-rw-r--r--   0        0        0      553 2023-04-25 10:40:34.964275 robocorp_browser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-04-25 10:39:03.643383 robocorp_browser-0.2.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     3106 2023-04-25 10:39:03.643516 robocorp_browser-0.2.0/src/robocorp/browser/browser.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 robocorp_browser-0.2.0/PKG-INFO
```

### Comparing `robocorp_browser-0.1.0/pyproject.toml` & `robocorp_browser-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.1.0"
+version = "0.2.0"
 description = "Robocorp browser automation library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
-packages = [{include = "robo", from="src"}]
+packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 playwright = "^1.32.1"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = "..", develop = true}
+libs-devdeps = {path = ".."}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-0.1.0/src/robo/libs/browser/browser.py` & `robocorp_browser-0.2.0/src/robocorp/browser/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         location = winreg.HKEY_LOCAL_MACHINE
         browser_registry = (
             rf"SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\{browser}.exe"
         )
         key = winreg.OpenKeyEx(location, browser_registry)
         # empty string key gets the (Default) value
         path = winreg.QueryValueEx(key, "")
+        if isinstance(path, tuple):
+            path = path[0]
         assert path, f"Could not find {browser} path"
         return path
     raise RuntimeError("Not implemented for this OS")
 
 
 EXECUTABLE_PATHS = {
     "chrome": {
@@ -40,22 +42,33 @@
     if system == "Windows":
         return _registry_path(browser)
 
     system = platform.system()
     assert browser in EXECUTABLE_PATHS
     executable_path = EXECUTABLE_PATHS[browser][system]
     assert Path(executable_path).exists()
-    return executable_path
+    return str(executable_path)
 
 
 def open_browser(
     browser: Literal["firefox", "chrome"] = "chrome",
     headless=True
     # TODO: support more args
 ) -> Browser:
+    """Launches a Playwright browser instance.
+
+    Args:
+        browser: Specifies which browser to use. Supported browsers are: ``chrome`` and ``firefox``.
+        headless: If set to False a GUI is provided, otherwise it is hidden.
+
+    Returns:
+        Browser: A Browser instance.
+
+    """
+
     playwright = _sync_playwright().start()
 
     assert playwright
     # TODO: allow user to also pass their own custom path?
     executable_path = _get_executable_path(browser)
 
     if browser == "chrome":
@@ -64,14 +77,27 @@
     launched_browser = playwright[browser].launch(
         executable_path=executable_path, headless=headless
     )
     return launched_browser
 
 
 def open_url(url: str, headless=True) -> Page:
+    """Launches a Playwright browser instance and opens the given URL.
+
+    Note:
+        Uses the ``chrome`` browser.
+
+    Args:
+        url: Navigates to the provided URL.
+        headless: If set to False a GUI is provided, otherwise it is hidden.
+
+    Returns:
+        Page: A Page instance.
+
+    """
     browser = open_browser(headless=headless)
     page = browser.new_page()
     page.goto(url)
     return page
 
 
 # TODO: don't let playwright print directly into stdout, it's breaking console behaviour
```

### Comparing `robocorp_browser-0.1.0/PKG-INFO` & `robocorp_browser-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.1.0
+Version: 0.2.0
 Summary: Robocorp browser automation library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

