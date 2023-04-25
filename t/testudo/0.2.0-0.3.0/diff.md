# Comparing `tmp/testudo-0.2.0.tar.gz` & `tmp/testudo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testudo-0.2.0.tar", last modified: Mon May 16 14:45:36 2022, max compression
+gzip compressed data, was "testudo-0.3.0.tar", last modified: Tue Apr 25 01:50:13 2023, max compression
```

## Comparing `testudo-0.2.0.tar` & `testudo-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    34500 2021-11-25 02:30:50.806492 testudo-0.2.0/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2370 2022-05-01 01:20:46.744670 testudo-0.2.0/README.md
--rw-r--r--   0 eugene    (1000) eugene    (1000)     2162 2022-05-16 14:44:38.387684 testudo-0.2.0/pyproject.toml
--rw-r--r--   0 eugene    (1000) eugene    (1000)      124 2022-05-01 02:16:27.092230 testudo-0.2.0/tests/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2929 2022-05-01 01:57:59.854262 testudo-0.2.0/tests/integration/test_reporter.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1589 2022-05-01 02:07:45.161421 testudo-0.2.0/tests/integration/test_runner.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2021-11-25 02:30:50.826493 testudo-0.2.0/tests/unit/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       35 2021-11-25 02:30:50.830493 testudo-0.2.0/tests/unit/resources/basic_config.yaml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1118 2021-12-16 02:41:52.522506 testudo-0.2.0/tests/unit/test_cli.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      788 2022-05-16 14:38:09.919274 testudo-0.2.0/tests/unit/test_config.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3497 2022-05-01 01:30:07.496756 testudo-0.2.0/tests/unit/test_reporter.py
--rw-r--r--   0 eugene    (1000) eugene    (1000)     2550 2022-05-16 14:30:52.888064 testudo-0.2.0/tests/unit/test_runner.py
--rw-r--r--   0 eugene    (1000) eugene    (1000)     3288 2022-01-02 21:57:45.167450 testudo-0.2.0/tests/unit/test_task_manager.py
--rw-r--r--   0 eugene    (1000) eugene    (1000)      256 2021-12-16 05:58:45.298634 testudo-0.2.0/tests/unit/utils.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2021-11-25 02:30:50.830493 testudo-0.2.0/testudo/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1762 2022-05-01 02:29:03.362445 testudo-0.2.0/testudo/cli.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      931 2022-05-16 14:13:31.766668 testudo-0.2.0/testudo/config.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1110 2022-05-01 02:25:07.892294 testudo-0.2.0/testudo/log.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3482 2022-05-01 02:24:46.772516 testudo-0.2.0/testudo/reporter.py
--rw-r--r--   0 eugene    (1000) eugene    (1000)     3857 2022-05-16 14:36:38.271295 testudo-0.2.0/testudo/runner.py
--rw-r--r--   0 eugene    (1000) eugene    (1000)     5134 2022-05-01 02:25:54.843839 testudo-0.2.0/testudo/task_manager.py
--rw-------   0 eugene    (1000) eugene    (1000)     4025 2022-05-16 14:45:36.063793 testudo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-03-25 23:45:23.607612 testudo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2370 2023-03-25 23:45:23.607612 testudo-0.3.0/README.md
+-rw-r--r--   0        0        0     1448 2023-04-25 01:04:47.119734 testudo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-25 01:04:47.119734 testudo-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2929 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/integration/test_reporter.py
+-rw-r--r--   0        0        0     1589 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/integration/test_runner.py
+-rw-r--r--   0        0        0        0 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0       35 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/resources/basic_config.yaml
+-rw-r--r--   0        0        0     1118 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      788 2023-04-25 01:22:53.120640 testudo-0.3.0/tests/unit/test_config.py
+-rw-r--r--   0        0        0     4569 2023-04-25 01:49:48.594171 testudo-0.3.0/tests/unit/test_reporter.py
+-rw-r--r--   0        0        0     2550 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_runner.py
+-rw-r--r--   0        0        0     3288 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_task_manager.py
+-rw-r--r--   0        0        0      256 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/utils.py
+-rw-r--r--   0        0        0        0 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/__init__.py
+-rw-r--r--   0        0        0     1762 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/cli.py
+-rw-r--r--   0        0        0      995 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/config.py
+-rw-r--r--   0        0        0      246 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/log.py
+-rw-r--r--   0        0        0     3837 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/reporter.py
+-rw-r--r--   0        0        0     3857 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/runner.py
+-rw-r--r--   0        0        0     5134 2023-04-25 01:36:29.661513 testudo-0.3.0/testudo/task_manager.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 testudo-0.3.0/PKG-INFO
```

### Comparing `testudo-0.2.0/LICENSE` & `testudo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/README.md` & `testudo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/pyproject.toml` & `testudo-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,53 @@
-[tool.pdm]
-includes = []
+[project]
+name = "testudo"
+version = "0.3.0"
+description = "A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory."
+authors = [
+    { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
+]
+dependencies = [
+    "click<9.0.0,>=8.0.3",
+    "legion-utils<1.0.0,>=0.3.0",
+]
+requires-python = ">=3.8.3,<4.0"
+readme = "README.md"
+
+[project.license]
+text = "GPL-3.0-or-later"
+
+[project.optional-dependencies]
+
+[project.scripts]
+testudo = "testudo.cli:main"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest>=7.1.2",
+    "pytest>=7.3.1",
     "pytest-cov>=3.0.0",
     "pytest-mock>=3.7.0",
     "pylint>=2.13.7",
-    "mypy>=0.950",
+    "mypy>=1.2.0",
     "flake8>=4.0.1",
     "bandit>=1.7.4",
     "black>=22.3.0",
-    "typeguard>=2.13.3",
+    "typeguard=4.0.0rc4",
     "pytest-xdist>=2.5.0",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
-[tool.pdm.scripts.publish]
-cmd = "twine upload dist/*"
+[tool.pdm.scripts.publish-prod]
+cmd = "twine upload -r pypi dist/*"
 
 [tool.pdm.scripts.test-deploy]
 shell = "pdm build && ssh typ-e -t 'rm /home/eugene/testudo-*-py3-none-any.whl'; rsync -Pparvzy dist/testudo-*-py3-none-any.whl typ-e:/home/eugene/ && ssh typ-e -t 'sudo pip3 install --force-reinstall /home/eugene/testudo-*-py3-none-any.whl && sudo supervisorctl restart borg-backup-to-ed-209'"
 
+[tool.pdm.build]
+includes = []
+
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-pep517>=1.0.4",
 ]
 build-backend = "pdm.pep517.api"
-
-[project]
-name = "testudo"
-version = "0.2.0"
-description = "A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory."
-authors = [
-    { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
-    { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
-]
-dependencies = [
-    "click<9.0.0,>=8.0.3",
-    "funcy<2.0,>=1.16",
-    "legion-utils<1.0.0,>=0.2.7",
-    "pyyaml<7.0,>=6.0",
-    "pydantic<2.0.0,>=1.8.2",
-    "typeguard<3.0.0,>=2.13.2",
-    "types-pyyaml>=6.0.7",
-    "logzero<2.0.0,>=1.7.0",
-]
-requires-python = ">=3.8,<4.0"
-readme = "README.md"
-license-expression = "GPL-3.0-only"
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-]
-
-[project.urls]
-repository = "https://gitlab.com/legion-robotnik/testudo"
-documentation = "https://gitlab.com/legion-robotnik/testudo"
-
-[project.scripts]
-testudo = "testudo.cli:main"
-
-[project.optional-dependencies]
```

### Comparing `testudo-0.2.0/tests/integration/test_reporter.py` & `testudo-0.3.0/tests/integration/test_reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/tests/integration/test_runner.py` & `testudo-0.3.0/tests/integration/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/tests/unit/test_cli.py` & `testudo-0.3.0/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/tests/unit/test_config.py` & `testudo-0.3.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/tests/unit/test_reporter.py` & `testudo-0.3.0/tests/unit/test_reporter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from legion_utils import Priority
+from time import sleep
 from yaml import safe_load
 
 from testudo.config import TaskConfig
 from testudo.reporter import report
 from testudo.task_manager import task_manager
 
 from tests.unit.utils import tempdir
@@ -19,14 +20,31 @@
     - num_failures: 2
       priority: WARNING
     - num_failures: 4
       priority: ERROR
     - num_failures: 6
       priority: CRITICAL'''))
 
+LONG_RUNNING_CONFIG = TaskConfig(**safe_load('''
+task_id: testing task
+delay_seconds: 1
+command: echo hello
+considered_successful_after_seconds: 0.1
+legion:
+  exchange: test
+  route: stuff
+  reporting_delay_seconds: 0.5
+  failure_priority_thresholds:
+    - num_failures: 2
+      priority: WARNING
+    - num_failures: 4
+      priority: ERROR
+    - num_failures: 6
+      priority: CRITICAL'''))
+
 
 def test_report_missing_task():
     with tempdir() as tmp_dir:
         with task_manager(tmp_dir / 'test.db') as tm:
             tm.insert_task_result('test', 'test output 1', 0, None)
             msg = report(tmp_dir / 'test.db', BASIC_CONFIG)
             assert msg.priority == Priority.ERROR
@@ -68,14 +86,27 @@
             tm.insert_task_result('testing task', 'test output 3', 1, None)
             tm.insert_task_result('testing task', 'test output 4', 1, None)
             msg = report(tmp_dir / 'test.db', BASIC_CONFIG)
             assert msg.priority == Priority.ERROR
             assert msg.contents['recent_output'] == 'test output 4'
 
 
+def test_not_reporting_failures_for_long_running_task():
+    with tempdir() as tmp_dir:
+        with task_manager(tmp_dir / 'test.db') as tm:
+            tm.insert_task_result('testing task', 'test output 1', 1, None)
+            tm.insert_task_result('testing task', 'test output 2', 1, None)
+            tm.insert_task_result('testing task', 'test output 3', 1, None)
+            tm.insert_task_result('testing task', 'test output 4', 1, None)
+            sleep(0.2)
+            msg = report(tmp_dir / 'test.db', LONG_RUNNING_CONFIG)
+            assert msg.priority == Priority.INFO
+            assert msg.contents['recent_output'] == 'test output 4'
+
+
 def test_report_critical_failures():
     with tempdir() as tmp_dir:
         with task_manager(tmp_dir / 'test.db') as tm:
             tm.insert_task_result('testing task', 'test output 1', 1, None)
             tm.insert_task_result('testing task', 'test output 2', 1, None)
             tm.insert_task_result('testing task', 'test output 3', 1, None)
             tm.insert_task_result('testing task', 'test output 4', 1, None)
```

### Comparing `testudo-0.2.0/tests/unit/test_runner.py` & `testudo-0.3.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/tests/unit/test_task_manager.py` & `testudo-0.3.0/tests/unit/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/testudo/cli.py` & `testudo-0.3.0/testudo/cli.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/testudo/config.py` & `testudo-0.3.0/testudo/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 
 @dataclass(config=Strict)
 class TaskConfig():
     task_id: str
     delay_seconds: float
     command: str
     legion: LegionConfig
+    considered_successful_after_seconds: Optional[float] = None
     acceptable_return_codes: Optional[List[int]] = None
     initial_delay_seconds: Optional[float] = None
     on_failure_delay_seconds: Optional[float] = None
```

### Comparing `testudo-0.2.0/testudo/reporter.py` & `testudo-0.3.0/testudo/reporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from math import ceil
 from pathlib import Path
 from pprint import pformat
 from socket import gethostname
 from threading import Thread, Event
+from time import time
 from traceback import format_exc
 from typing import Optional
 
 from funcy import first
 import legion_utils
 from legion_utils import Priority, NotificationMsg
 
@@ -16,25 +17,28 @@
 
 HOSTNAME = gethostname()
 
 
 def report(db: Path, task_config: TaskConfig) -> NotificationMsg:
     with task_manager(db) as tm:
         if recent_failures := list(f for f in tm.get_recent_failures(task_config.task_id)):
-            priority_thresholds = sorted(task_config.legion.failure_priority_thresholds,
-                                         key=lambda t: t.num_failures, reverse=True)
-            for threshold in priority_thresholds:
-                if len(recent_failures) >= threshold.num_failures:
-                    return NotificationMsg(contents={'src': HOSTNAME,
-                                                     'recent_output': recent_failures[0].output,
-                                                     'recent_exit_code': recent_failures[0].exit_code},
-                                           alert_key=f'[{HOSTNAME}][testudo][failure][{task_config.task_id}]',
-                                           desc=f'Task [{task_config.task_id}] failed {len(recent_failures)} times',
-                                           ttl=ceil(task_config.legion.reporting_delay_seconds * 2),
-                                           priority=threshold.priority)
+            # only bother alerting if failures are more recent than the "considered successful" threshold
+            if task_config.considered_successful_after_seconds is None or \
+               any(rf.timestamp >= (time() - task_config.considered_successful_after_seconds) for rf in recent_failures):
+                priority_thresholds = sorted(task_config.legion.failure_priority_thresholds,
+                                            key=lambda t: t.num_failures, reverse=True)
+                for threshold in priority_thresholds:
+                    if len(recent_failures) >= threshold.num_failures:
+                        return NotificationMsg(contents={'src': HOSTNAME,
+                                                        'recent_output': recent_failures[0].output,
+                                                        'recent_exit_code': recent_failures[0].exit_code},
+                                            alert_key=f'[{HOSTNAME}][testudo][failure][{task_config.task_id}]',
+                                            desc=f'Task [{task_config.task_id}] failed {len(recent_failures)} times',
+                                            ttl=ceil(task_config.legion.reporting_delay_seconds * 2),
+                                            priority=threshold.priority)
         if most_recent_run := first(tm.get_previous_results(task_config.task_id, limit=1)):
             return NotificationMsg(contents={'src': HOSTNAME,
                                              'recent_output': most_recent_run.output},
                                    desc=f'Task [{task_config.task_id} ran nominally',
                                    priority=Priority.INFO)
         return NotificationMsg(contents={'src': HOSTNAME},
                                alert_key=f'[{HOSTNAME}][testudo][unknown_task_id][{task_config.task_id}]',
```

### Comparing `testudo-0.2.0/testudo/runner.py` & `testudo-0.3.0/testudo/runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.2.0/testudo/task_manager.py` & `testudo-0.3.0/testudo/task_manager.py`

 * *Files identical despite different names*

