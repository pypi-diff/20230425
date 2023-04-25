# Comparing `tmp/branch_time-0.1.2.tar.gz` & `tmp/branch_time-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branch_time-0.1.2.tar", max compression
+gzip compressed data, was "branch_time-0.1.3.tar", max compression
```

## Comparing `branch_time-0.1.2.tar` & `branch_time-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-25 00:24:44.574088 branch_time-0.1.2/branch_time/__init__,py
--rw-r--r--   0        0        0      238 2023-04-23 02:05:09.607644 branch_time-0.1.2/branch_time/GitRepositoryError.py
--rw-r--r--   0        0        0     3144 2023-04-25 00:27:45.934680 branch_time-0.1.2/branch_time/jira.py
--rw-r--r--   0        0        0       20 2023-04-24 21:48:29.650929 branch_time-0.1.2/LICENSE
--rw-r--r--   0        0        0     1102 2023-04-25 00:39:36.045865 branch_time-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      337 2023-04-23 00:38:39.956843 branch_time-0.1.2/README.md
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 branch_time-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-25 00:24:44.574088 branch_time-0.1.3/branch_time/__init__,py
+-rw-r--r--   0        0        0      238 2023-04-23 02:05:09.607644 branch_time-0.1.3/branch_time/GitRepositoryError.py
+-rw-r--r--   0        0        0     3151 2023-04-25 01:44:02.508972 branch_time-0.1.3/branch_time/jira.py
+-rw-r--r--   0        0        0       20 2023-04-24 21:48:29.650929 branch_time-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1102 2023-04-25 01:42:12.009051 branch_time-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1622 2023-04-25 01:42:00.719033 branch_time-0.1.3/README.md
+-rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 branch_time-0.1.3/PKG-INFO
```

### Comparing `branch_time-0.1.2/branch_time/jira.py` & `branch_time-0.1.3/branch_time/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 
                 last_line = last_line_on_file(file)
                 if is_not_same_branch(last_line, branch):
                     file.write(count_time(branch, last_line))
                     file.write(
                         f"Branch: {branch} - Time: {now.hour}:{now.minute}:{now.second}\n"
                     )
-                time.sleep(time_in_minute)
+                time.sleep(time_in_minute * 60)
+
             except NotADirectoryError:
                 console.print("[red1]Directory not found")
                 sys.exit(1)
             except KeyboardInterrupt:
                 now = datetime.now()
                 file.write(f"FINISHED... {now.hour}:{now.minute}:{now.second}\n")
                 sys.exit(0)
```

### Comparing `branch_time-0.1.2/pyproject.toml` & `branch_time-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "branch-time"
-version = "0.1.2"
+version = "0.1.3"
 description = "Counts time in a branch"
 license="BeerWare"
 authors = ["Icaro Nunes"]
 readme = "README.md"
 packages = [{include = "branch_time"}]
 classifiers= [
     "Development Status :: 4 - Beta",
```

