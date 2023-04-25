# Comparing `tmp/python-observer-0.1.0.tar.gz` & `tmp/python-observer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-observer-0.1.0.tar", max compression
+gzip compressed data, was "python-observer-0.2.0.tar", max compression
```

## Comparing `python-observer-0.1.0.tar` & `python-observer-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      519 2023-04-24 10:11:36.890391 python-observer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.1.0/python_observer/__init__.py
--rw-r--r--   0        0        0     1979 2023-04-24 10:10:37.108188 python-observer-0.1.0/python_observer/cli.py
--rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.1.0/python_observer/constants.py
--rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.1.0/python_observer/date.py
--rw-r--r--   0        0        0      581 2023-04-24 10:10:37.153301 python-observer-0.1.0/python_observer/display.py
--rw-r--r--   0        0        0      547 2023-04-24 09:57:44.466878 python-observer-0.1.0/python_observer/misc.py
--rw-r--r--   0        0        0     2850 2023-04-24 10:10:37.186394 python-observer-0.1.0/python_observer/watch.py
--rw-r--r--   0        0        0      769 2023-04-24 10:12:49.723559 python-observer-0.1.0/setup.py
--rw-r--r--   0        0        0      526 2023-04-24 10:12:49.723559 python-observer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.2.0/LICENSE
+-rw-r--r--   0        0        0      541 2023-04-25 13:32:03.887748 python-observer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.2.0/python_observer/__init__.py
+-rw-r--r--   0        0        0     2259 2023-04-25 13:30:23.403543 python-observer-0.2.0/python_observer/cli.py
+-rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.2.0/python_observer/constants.py
+-rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.2.0/python_observer/date.py
+-rw-r--r--   0        0        0      595 2023-04-24 10:43:39.568229 python-observer-0.2.0/python_observer/display.py
+-rw-r--r--   0        0        0      437 2023-04-25 13:30:23.404545 python-observer-0.2.0/python_observer/misc.py
+-rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.2.0/python_observer/watch.py
+-rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.2.0/README.md
+-rw-r--r--   0        0        0      923 2023-04-25 13:33:03.025319 python-observer-0.2.0/setup.py
+-rw-r--r--   0        0        0      717 2023-04-25 13:33:03.026775 python-observer-0.2.0/PKG-INFO
```

### Comparing `python-observer-0.1.0/pyproject.toml` & `python-observer-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "python-observer"
-version = "0.1.0"
+version = "0.2.0"
 description = "Live reload for Python apps"
 authors = ["Skyascii <savioxavier112@gmail.com>"]
 license = "MIT"
+readme = "README.md"
 packages = [
     { include = "python_observer/**/*.py" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.3.4"
```

### Comparing `python-observer-0.1.0/python_observer/cli.py` & `python-observer-0.2.0/python_observer/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,25 +8,35 @@
 from .watch import watch_file
 
 
 def main():
     # sourcery skip: extract-method
     parser = argparse.ArgumentParser()
 
-    parser.add_argument("file", help="path to the file to watch")
+    parser.add_argument("script", help="the file to watch", type=str)
+    parser.add_argument(
+        "script_args",
+        nargs=argparse.REMAINDER,
+        help="additional arguments for the above file",
+    )
 
     args = parser.parse_args()
 
+    if not args.script:
+        parser.print_help()
+
     try:
-        if file_exists(args.file):
-            file_path = args.file
+        command = [args.script] + args.script_args
+
+        if file_exists(args.script):
+            file_path = args.script
         else:
             print(
                 observer_message(
-                    f"[red]Error: File {args.file} does not exist", style="red"
+                    f"[red]Error: File {args.script} does not exist", style="red"
                 ),
                 highlight=False,
             )
             exit()
 
         newline()
 
@@ -44,15 +54,15 @@
 
         newline()
         print_line(rule_style="cyan", char="━")
         newline()
 
         session_start_time = get_monotonic_time(as_seconds=True, should_round=False)
 
-        watch_file(file_path)
+        watch_file(command, file_path=args.script)
     except KeyboardInterrupt:
         session_end_time = get_monotonic_time(as_seconds=True, should_round=False)
         newline()
         print(
             observer_message(
                 f"[cyan]watch session took [yellow]{format_time(session_end_time - session_start_time)}"
             )
```

### Comparing `python-observer-0.1.0/python_observer/date.py` & `python-observer-0.2.0/python_observer/date.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.1.0/python_observer/display.py` & `python-observer-0.2.0/python_observer/display.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from rich.console import Console
 from rich.table import Table
+from .constants import DOT_CHAR
 
 console = Console()
 rich_print = console.print
 
-DOT_CHAR = "•"
-
 
 def newline():
     print("\n", end="")
 
 
 def print_both_sides(left, right):
     grid = Table.grid(expand=True)
```

### Comparing `python-observer-0.1.0/python_observer/watch.py` & `python-observer-0.2.0/python_observer/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .constants import DOT_CHAR, MIN_TIMEOUT_MILLISECONDS
 from .date import format_time, get_current_time, get_monotonic_time
 from .display import observer_message, print_both_sides, print_line
 from .misc import resolve_path, run_file
 
 
-def watch_file(file_path):
+def watch_file(command, file_path):
     def draw_process_lines(is_rerun=True):
         if is_rerun:
             last_save_text = f"{DOT_CHAR} [blue]since last save: [/blue]{format_time(end_save_time - start_save_time)}"
         else:
             last_save_text = ""
 
         if process.returncode != 0:
@@ -33,15 +33,15 @@
     )
 
     file_path = resolve_path(file_path)
 
     start_time = get_monotonic_time()
 
     # first run
-    process = run_file(file_path)
+    process = run_file(command)
 
     end_time = get_monotonic_time()
 
     draw_process_lines(is_rerun=False)
 
     # get the initial modification time of the file
     last_modified_time = os.stat(file_path).st_mtime
@@ -65,15 +65,15 @@
             )
 
             end_save_time = get_monotonic_time(as_seconds=True, should_round=False)
 
             start_time = get_monotonic_time()
 
             # run the file
-            process = run_file(file_path)
+            process = run_file(command)
 
             end_time = get_monotonic_time()
 
             # update the last modified time to the current time
             last_modified_time = current_modified_time
 
             draw_process_lines()
```

### Comparing `python-observer-0.1.0/setup.py` & `python-observer-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['humanfriendly>=10.0,<11.0', 'rich>=13.3.4,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['observer = python_observer.cli:main']}
 
 setup_kwargs = {
     'name': 'python-observer',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Live reload for Python apps',
-    'long_description': None,
+    'long_description': "# observer\n\n![observer image](https://i.imgur.com/ZoafdEY.png)\n\n> Live reload for Python apps\n\nDocs coming soon - I've ordered them via Amazon Prime\n",
     'author': 'Skyascii',
     'author_email': 'savioxavier112@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

