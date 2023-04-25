# Comparing `tmp/branch_time-0.1.1.tar.gz` & `tmp/branch_time-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branch_time-0.1.1.tar", max compression
+gzip compressed data, was "branch_time-0.1.2.tar", max compression
```

## Comparing `branch_time-0.1.1.tar` & `branch_time-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-24 22:18:33.510606 branch_time-0.1.1/branch_time/__init__,py
--rw-r--r--   0        0        0      238 2023-04-23 02:05:09.607644 branch_time-0.1.1/branch_time/GitRepositoryError.py
--rw-r--r--   0        0        0     3008 2023-04-24 22:24:35.018885 branch_time-0.1.1/branch_time/jira.py
--rw-r--r--   0        0        0       20 2023-04-24 21:48:29.650929 branch_time-0.1.1/LICENSE
--rw-r--r--   0        0        0     1046 2023-04-24 22:31:14.090585 branch_time-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      337 2023-04-23 00:38:39.956843 branch_time-0.1.1/README.md
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 branch_time-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-25 00:24:44.574088 branch_time-0.1.2/branch_time/__init__,py
+-rw-r--r--   0        0        0      238 2023-04-23 02:05:09.607644 branch_time-0.1.2/branch_time/GitRepositoryError.py
+-rw-r--r--   0        0        0     3144 2023-04-25 00:27:45.934680 branch_time-0.1.2/branch_time/jira.py
+-rw-r--r--   0        0        0       20 2023-04-24 21:48:29.650929 branch_time-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1102 2023-04-25 00:39:36.045865 branch_time-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-04-23 00:38:39.956843 branch_time-0.1.2/README.md
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 branch_time-0.1.2/PKG-INFO
```

### Comparing `branch_time-0.1.1/branch_time/jira.py` & `branch_time-0.1.2/branch_time/jira.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,59 +2,63 @@
 import io
 import subprocess
 import sys
 import time
 from datetime import date, datetime
 
 import typer
+from rich.console import Console
 
-from GitRepositoryError import GitRepositoryError
+from branch_time.GitRepositoryError import GitRepositoryError
 
 app = typer.Typer(help="Awesome CLI user manager.")
+console = Console()
 
 
 def is_not_same_branch(last_line, branch):
-    print(last_line)
+    console.print(last_line)
     return branch not in last_line
 
 
 def last_line_on_file(file) -> str:
     try:
         file.seek(io.SEEK_CUR)
         return file.readlines()[-1]
     except IndexError:
         return ""
 
 
 def time_change(time):
-    hora, minutos, sec = time.split(":")
-    data_atual = datetime.now()
+    hora, min, sec = time.split(":")
+    data_current = datetime.now()
     data_obj = datetime(
-        data_atual.year,
-        data_atual.month,
-        data_atual.day,
+        data_current.year,
+        data_current.month,
+        data_current.day,
         int(hora),
-        int(minutos),
+        int(min),
         int(sec),
     )
-    hour, min, seg = f"{data_atual - data_obj}".split(":")[:3]
+    hour, min, seg = f"{data_current - data_obj}".split(":")[:3]
     return f"{hour} {min} {seg.split('.')[0]}"
 
 
 def count_time(branch: str, last_line: str) -> str:
     try:
         time = last_line.split("Tempo:")[1].replace("\n", "")
         return f"Changer for Branch:{branch} after{time_change(time)}\n\n"
     except:
         return "\n"
 
 
 @app.command()
 def getFile(
-    repository: str = typer.Option('.', "--repository", "-r", help="Repository git"),
+    repository: str = typer.Argument(
+        ".", help="Repository git. Default: Current directory"
+    ),
     time_in_minute: int = typer.Option(
         5, "--time", "-t", help="Time for update current branch"
     ),
     output_file: str = typer.Option(
         date.today(),
         "--output",
         "-o",
@@ -75,25 +79,23 @@
                 if branch == "":
                     raise GitRepositoryError("")
 
                 last_line = last_line_on_file(file)
                 if is_not_same_branch(last_line, branch):
                     file.write(count_time(branch, last_line))
                     file.write(
-                        f"Branch:{branch} - Time:{now.hour}:{now.minute}:{now.second}\n"
+                        f"Branch: {branch} - Time: {now.hour}:{now.minute}:{now.second}\n"
                     )
                 time.sleep(time_in_minute)
             except NotADirectoryError:
-                print("Directory not found")
+                console.print("[red1]Directory not found")
                 sys.exit(1)
             except KeyboardInterrupt:
                 now = datetime.now()
                 file.write(f"FINISHED... {now.hour}:{now.minute}:{now.second}\n")
                 sys.exit(0)
             except GitRepositoryError as git_error:
-                print(git_error)
-                print("--repository parameter does not point to a git repository")
+                console.print(git_error)
+                console.print(
+                    "[red1]--repository parameter does not point to a git repository"
+                )
                 sys.exit(1)
-
-
-if __name__ == "__main__":
-    app()
```

### Comparing `branch_time-0.1.1/pyproject.toml` & `branch_time-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "branch-time"
-version = "0.1.1"
+version = "0.1.2"
 description = "Counts time in a branch"
 license="BeerWare"
 authors = ["Icaro Nunes"]
 readme = "README.md"
 packages = [{include = "branch_time"}]
 classifiers= [
     "Development Status :: 4 - Beta",
@@ -13,17 +13,19 @@
 
 [tool.poetry.dependencies]
 python = "^3"
 typer = "^0.7.0"
 typer-cli = "^0.0.13"
 click = "^8.0"
 pytest = "^7.3.1"
+rich = "^13.3.4"
 
 [tool.poetry.scripts]
 branchtime = "branch_time.jira:app"
+branch-time = "branch_time.jira:app"
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/icaronunes/branch-time" 
 "Bug Tracker" = "https://github.com/icaronunes/branch-time/issues"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
```

### Comparing `branch_time-0.1.1/PKG-INFO` & `branch_time-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branch-time
-Version: 0.1.1
+Version: 0.1.2
 Summary: Counts time in a branch
 License: Beerware
 Author: Icaro Nunes
 Requires-Python: >=3,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
 Project-URL: Bug Tracker, https://github.com/icaronunes/branch-time/issues
 Project-URL: Repository, https://github.com/icaronunes/branch-time
 Description-Content-Type: text/markdown
```

