# Comparing `tmp/instater-0.8.0.tar.gz` & `tmp/instater-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/instater-0.8.0.tar", last modified: Sat Nov  6 16:27:57 2021, max compression
+gzip compressed data, was "dist/instater-0.9.0.tar", last modified: Wed Apr 13 04:13:11 2022, max compression
```

## Comparing `instater-0.8.0.tar` & `instater-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 16:27:57.000000 instater-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-11-06 16:27:38.000000 instater-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-11-06 16:27:38.000000 instater-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-11-06 16:27:38.000000 instater-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15524 2021-11-06 16:27:57.000000 instater-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2021-11-06 16:27:38.000000 instater-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 16:27:57.000000 instater-0.8.0/instater/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-06 16:27:38.000000 instater-0.8.0/instater/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-11-06 16:27:38.000000 instater-0.8.0/instater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2021-11-06 16:27:38.000000 instater-0.8.0/instater/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2021-11-06 16:27:38.000000 instater-0.8.0/instater/context.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-11-06 16:27:38.000000 instater-0.8.0/instater/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-11-06 16:27:38.000000 instater-0.8.0/instater/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7134 2021-11-06 16:27:38.000000 instater-0.8.0/instater/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 16:27:57.000000 instater-0.8.0/instater/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     5429 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/copy.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/git.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/pacman.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2021-11-06 16:27:38.000000 instater-0.8.0/instater/tasks/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-11-06 16:27:38.000000 instater-0.8.0/instater/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15524 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-06 16:27:57.000000 instater-0.8.0/instater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-06 16:27:38.000000 instater-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-06 16:27:57.000000 instater-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2021-11-06 16:27:38.000000 instater-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 04:13:11.000000 instater-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-04-13 04:12:46.000000 instater-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-13 04:12:46.000000 instater-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-13 04:12:46.000000 instater-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15847 2022-04-13 04:13:11.000000 instater-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-04-13 04:12:46.000000 instater-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 04:13:11.000000 instater-0.9.0/instater/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-13 04:12:46.000000 instater-0.9.0/instater/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-04-13 04:12:46.000000 instater-0.9.0/instater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-04-13 04:12:46.000000 instater-0.9.0/instater/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-04-13 04:12:46.000000 instater-0.9.0/instater/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-04-13 04:12:46.000000 instater-0.9.0/instater/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-04-13 04:12:46.000000 instater-0.9.0/instater/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8445 2022-04-13 04:12:46.000000 instater-0.9.0/instater/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 04:13:11.000000 instater-0.9.0/instater/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5429 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/pacman.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-04-13 04:12:46.000000 instater-0.9.0/instater/tasks/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-04-13 04:12:46.000000 instater-0.9.0/instater/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 04:13:11.000000 instater-0.9.0/instater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15847 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-13 04:13:10.000000 instater-0.9.0/instater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-04-13 04:12:46.000000 instater-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-13 04:13:11.000000 instater-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-04-13 04:12:46.000000 instater-0.9.0/setup.py
```

### Comparing `instater-0.8.0/LICENSE` & `instater-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/PKG-INFO` & `instater-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instater
-Version: 0.8.0
+Version: 0.9.0
 Summary: An easy solution for system/dotfile configuration
 Home-page: https://github.com/nayaverdier/instater
 Author: Naya Verdier
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -588,14 +588,22 @@
     groups: makepkg
     system: true
 ```
 
 
 # Changelog
 
+## 0.9.0 2022-04-12
+
+- Add check for manually installed pacman packages when using Arch Linux
+- Add `--skip-tasks` argument to skip all tasks (useful for the pacman
+  package check)
+- Fix bug where relative paths were not resolving when instater was run
+  from a directory other than the one containing the setup.yml file
+
 ## 0.8.0 2021-11-06
 
 - `command`: Support pipes between two commands
 
 ## 0.7.0 2021-11-04
 
 - Better support `when` argument so that undefined variables are
```

### Comparing `instater-0.8.0/README.md` & `instater-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/cli.py` & `instater-0.9.0/instater/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 
 def main():
     parser = ArgumentParser(description="An easy solution for system/dotfile configuration")
     parser.add_argument("--setup-file", default="setup.yml", help="The setup file to execute")
     parser.add_argument("--tags", nargs="*", help="Run only a subset of tasks by their tag")
     parser.add_argument("--vars", help="Variables to override prompts or variable files")
     parser.add_argument(
+        "--skip-tasks",
+        action="store_true",
+        help="Do not actually run tasks (useful for just checking for manually installed pacman packages)",
+    )
+    parser.add_argument(
         "--dry-run",
         action="store_true",
         help="Display operations that would be performed without actually running them",
     )
     parser.add_argument("--version", action="store_true", help="Display the version of instater")
 
     args = parser.parse_args()
@@ -51,12 +56,12 @@
         Console().print(f"Instater {VERSION}")
         return
 
     tags = args.tags
 
     try:
         variables = _parse_variables(args.vars)
-        run_tasks(args.setup_file, variables, tags, args.dry_run)
+        run_tasks(args.setup_file, variables, tags, args.dry_run, skip_tasks=args.skip_tasks)
     except InstaterError as e:
         console = Console()
         console.print(e, style="red")
         console.print("Exiting...", style="red bold")
```

### Comparing `instater-0.8.0/instater/context.py` & `instater-0.9.0/instater/context.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/importer.py` & `instater-0.9.0/instater/importer.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/main.py` & `instater-0.9.0/instater/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import getpass
+import shutil
 from glob import glob
 from pathlib import Path
 from typing import Iterable, List, Union
 
 import yaml  # type: ignore
 
 from . import util
 from .context import Context
 from .exceptions import InstaterError
-from .tasks import TASKS
+from .tasks import TASKS, pacman
 
 
 def _print_start(context: Context, setup_file: Path):
     context.print(f"Beginning instater execution from {setup_file.absolute()}", style="green bold")
     if context.tags:
         colored_tags = ", ".join(f"[bold]{tag}[/bold]" for tag in context.tags)
         context.print("Only executing specified tags:", colored_tags, style="blue")
@@ -90,21 +91,24 @@
         with file.open() as f:
             raw_vars = yaml.safe_load(f)
 
         for var, value in raw_vars.items():
             context.variables[var] = context.jinja_string(value)
 
 
-def _extract_with(task_args: dict) -> List[dict]:
+def _extract_with(context: Context, task_args: dict) -> List[dict]:
     fileglob = task_args.pop("with_fileglob", None)
 
     if not util.single_truthy(fileglob, allow_zero=True):
         raise InstaterError("Must provide at most one `with_*` looping attribute")
 
     if fileglob:
+        if not fileglob.startswith("/"):
+            fileglob = str(context.root_directory) + "/" + fileglob
+
         return [{"item": path} for path in glob(fileglob, recursive=True)]
 
     return [{}]
 
 
 def _load_task_item(args: dict, tags: List[str], item: dict, context: Context):
     tags = [context.jinja_string(tag, extra_vars=item) for tag in tags]
@@ -142,15 +146,15 @@
     except (InstaterError, TypeError) as e:
         name = args.get("name")
         error_name = f"'{name}' ({task_name})" if name else f"'{task_name}'"
         raise InstaterError(f"Error loading task {error_name}: {e}")
 
 
 def _load_task(task_args: dict, tags: List[str], context: Context):
-    with_items = _extract_with(task_args)
+    with_items = _extract_with(context, task_args)
     for item in with_items:
         _load_task_item(task_args.copy(), tags, item, context)
 
 
 def _load_tasks(task_list, context: Context, extra_tags: List[str] = None):
     if not task_list:
         return
@@ -183,15 +187,20 @@
         tags = [tags]
 
     tags.extend(parent_tags)
 
     _load_tasks(tasks, context, tags)
 
 
-def run_tasks(setup_file, override_variables: dict = None, tags: Iterable[str] = None, dry_run: bool = False):
+def _load_context(
+    setup_file,
+    override_variables: dict = None,
+    tags: Iterable[str] = None,
+    dry_run: bool = False,
+) -> Context:
     setup_file = Path(setup_file)
     context = Context(setup_file.parent, override_variables or {}, tags or (), dry_run)
 
     if not setup_file.exists():
         raise InstaterError(f"Setup file does not exist: {setup_file}")
 
     _print_start(context, setup_file)
@@ -204,13 +213,51 @@
             raise InstaterError(f"Cannot specify multiple root list items in {setup_file}")
         setup_data = setup_data[0]
 
     _prompt_variables(setup_data.get("vars_prompt"), context)
     _file_variables(setup_data.get("vars_files"), context)
     _load_tasks(setup_data.get("tasks"), context)
 
+    return context
+
+
+def _alert_pacman_manually_installed(context: Context):
+    packages = set()
+
     for task in context.tasks:
-        task.run_task(context)
+        if isinstance(task, pacman.Pacman):
+            for package in task.packages:
+                packages.update(pacman.get_package_or_group_packages(package))
+
+    explicitly_installed_packages = pacman.get_explicitly_installed_packages()
+    manually_installed = explicitly_installed_packages - packages
+
+    if manually_installed:
         print()
+        context.print(
+            ":warning: The following packages were manually installed and are not accounted for by instater",
+            style="yellow bold",
+        )
+        for package in manually_installed:
+            context.print("  - " + package, style="bold")
+
+
+def run_tasks(
+    setup_file,
+    override_variables: dict = None,
+    tags: Iterable[str] = None,
+    dry_run: bool = False,
+    skip_tasks: bool = False,
+):
+    context = _load_context(setup_file, override_variables, tags, dry_run)
+
+    if not skip_tasks:
+        for task in context.tasks:
+            task.run_task(context)
+            print()
 
     context.print_summary()
+
+    if shutil.which("pacman"):
+        _alert_pacman_manually_installed(context)
+
     return context
```

### Comparing `instater-0.8.0/instater/tasks/_task.py` & `instater-0.9.0/instater/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/command.py` & `instater-0.9.0/instater/tasks/command.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/copy.py` & `instater-0.9.0/instater/tasks/copy.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/file.py` & `instater-0.9.0/instater/tasks/file.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/git.py` & `instater-0.9.0/instater/tasks/git.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/group.py` & `instater-0.9.0/instater/tasks/group.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/pacman.py` & `instater-0.9.0/instater/tasks/pacman.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 import tempfile
-from typing import List, Union
+from typing import List, Set, Union
 
 from instater.exceptions import InstaterError
 
 from .. import util
 from ..context import Context
 from . import Task
 
@@ -79,7 +79,20 @@
         return True
 
 
 class Aur(Pacman):
     def __init__(self, **kwargs):
         kwargs["aur"] = True
         super().__init__(**kwargs)
+
+
+def get_explicitly_installed_packages() -> Set[str]:
+    output = util.shell(["pacman", "-Qe"])
+    return set(line.split()[0] for line in output.stdout.splitlines() if line)
+
+
+def get_package_or_group_packages(package: str) -> Set[str]:
+    group_output = util.shell(["pacman", "-Qg", package], valid_return_codes=(0, 1))
+    if group_output.return_code == 1:
+        return {package}
+    else:
+        return set(line.split()[1] for line in group_output.stdout.splitlines())
```

### Comparing `instater-0.8.0/instater/tasks/service.py` & `instater-0.9.0/instater/tasks/service.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/tasks/user.py` & `instater-0.9.0/instater/tasks/user.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater/util.py` & `instater-0.9.0/instater/util.py`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/instater.egg-info/PKG-INFO` & `instater-0.9.0/instater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instater
-Version: 0.8.0
+Version: 0.9.0
 Summary: An easy solution for system/dotfile configuration
 Home-page: https://github.com/nayaverdier/instater
 Author: Naya Verdier
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -588,14 +588,22 @@
     groups: makepkg
     system: true
 ```
 
 
 # Changelog
 
+## 0.9.0 2022-04-12
+
+- Add check for manually installed pacman packages when using Arch Linux
+- Add `--skip-tasks` argument to skip all tasks (useful for the pacman
+  package check)
+- Fix bug where relative paths were not resolving when instater was run
+  from a directory other than the one containing the setup.yml file
+
 ## 0.8.0 2021-11-06
 
 - `command`: Support pipes between two commands
 
 ## 0.7.0 2021-11-04
 
 - Better support `when` argument so that undefined variables are
```

### Comparing `instater-0.8.0/instater.egg-info/SOURCES.txt` & `instater-0.9.0/instater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instater-0.8.0/setup.py` & `instater-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 changelog = (ROOT_DIRECTORY / "CHANGELOG.md").read_text()
 long_description = readme + "\n\n" + changelog
 
 version = (ROOT_DIRECTORY / "instater" / "VERSION").read_text().strip()
 
 
 DEV_REQUIRES = [
-    "black==21.9b0",
+    "black==22.3.0",
     "coverage==6.0.2",
     "flake8==4.0.1",
     "flake8-bugbear==21.9.2",
     "isort==5.9.3",
     "mypy==0.910",
     "pytest==6.2.5",
     "pytest-cov==3.0.0",
```

