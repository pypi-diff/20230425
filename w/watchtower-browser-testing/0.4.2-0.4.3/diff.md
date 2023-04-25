# Comparing `tmp/watchtower_browser_testing-0.4.2.tar.gz` & `tmp/watchtower_browser_testing-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.2.tar", last modified: Tue Apr 18 07:26:00 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.3.tar", last modified: Tue Apr 25 13:34:14 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.2.tar` & `watchtower_browser_testing-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.068505 watchtower_browser_testing-0.4.2/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6193 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.328711 watchtower_browser_testing-0.4.3/
+-rw-rw-rw-   0        0        0      310 2023-04-25 13:34:14.327710 watchtower_browser_testing-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:34:14.328711 watchtower_browser_testing-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.316519 watchtower_browser_testing-0.4.3/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.325666 watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6193 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    17323 2023-04-25 13:13:32.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-25 13:33:49.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.323492 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.2/setup.py` & `watchtower_browser_testing-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing/testsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,17 +451,31 @@
 
         for test in tests:
             structure['children'].append(test['class'].md_description(parent=name))
 
 
         return structure
 
-    def html_report(self, title='Measurement Plan', test_results=None):
-
-        jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
-        template = jenv.get_template('measurement_plan.html')
+    def html_report(self,
+                    title='Measurement Plan',
+                    test_results=None):
 
         content = self.md_description()
 
         test_results = test_results or {}
 
-        return template.render(title=title, content=content, test_results=test_results)
+        return self.render_html(title=title,
+                                content=content,
+                                test_results=test_results)
+
+    @classmethod
+    def render_html(cls,
+                    title,
+                    content,
+                    test_results,
+                    run_tests_token=None):
+
+        jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
+        template = jenv.get_template('measurement_plan.html')
+
+        return template.render(title=title, content=content,
+                               test_results=test_results, run_tests_token=run_tests_token)
```

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

