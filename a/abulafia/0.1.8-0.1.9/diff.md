# Comparing `tmp/abulafia-0.1.8.tar.gz` & `tmp/abulafia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abulafia-0.1.8.tar", last modified: Fri Dec  2 11:37:35 2022, max compression
+gzip compressed data, was "abulafia-0.1.9.tar", last modified: Thu Jan 19 11:45:29 2023, max compression
```

## Comparing `abulafia-0.1.8.tar` & `abulafia-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.822964 abulafia-0.1.8/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     1073 2022-09-21 10:53:07.000000 abulafia-0.1.8/LICENSE
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2022-12-02 11:37:35.822533 abulafia-0.1.8/PKG-INFO
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    12761 2022-11-18 08:02:32.000000 abulafia-0.1.8/README.md
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      503 2022-12-02 11:33:36.000000 abulafia-0.1.8/pyproject.toml
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       38 2022-12-02 11:37:35.823051 abulafia-0.1.8/setup.cfg
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       37 2022-08-23 07:22:48.000000 abulafia-0.1.8/setup.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.792165 abulafia-0.1.8/src/
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.796168 abulafia-0.1.8/src/abulafia/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       22 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/__init__.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.815683 abulafia-0.1.8/src/abulafia/actions/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       64 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/actions/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    23580 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/actions/actions.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.818274 abulafia-0.1.8/src/abulafia/functions/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       31 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/functions/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    24719 2022-12-02 11:33:36.000000 abulafia-0.1.8/src/abulafia/functions/core_functions.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.819566 abulafia-0.1.8/src/abulafia/observers/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       25 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/observers/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     4601 2022-09-21 13:16:09.000000 abulafia-0.1.8/src/abulafia/observers/observers.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.822116 abulafia-0.1.8/src/abulafia/task_specs/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       75 2022-08-23 07:22:48.000000 abulafia-0.1.8/src/abulafia/task_specs/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    47569 2022-12-01 07:49:20.000000 abulafia-0.1.8/src/abulafia/task_specs/core_task.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    15826 2022-09-21 10:53:07.000000 abulafia-0.1.8/src/abulafia/task_specs/pipeline.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    51668 2022-12-02 11:33:36.000000 abulafia-0.1.8/src/abulafia/task_specs/task_specs.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2022-12-02 11:37:35.809767 abulafia-0.1.8/src/abulafia.egg-info/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2022-12-02 11:37:35.000000 abulafia-0.1.8/src/abulafia.egg-info/PKG-INFO
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      604 2022-12-02 11:37:35.000000 abulafia-0.1.8/src/abulafia.egg-info/SOURCES.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        1 2022-12-02 11:37:35.000000 abulafia-0.1.8/src/abulafia.egg-info/dependency_links.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       76 2022-12-02 11:37:35.000000 abulafia-0.1.8/src/abulafia.egg-info/requires.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        9 2022-12-02 11:37:35.000000 abulafia-0.1.8/src/abulafia.egg-info/top_level.txt
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.228820 abulafia-0.1.9/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     1073 2022-09-21 10:53:07.000000 abulafia-0.1.9/LICENSE
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2023-01-19 11:45:29.228364 abulafia-0.1.9/PKG-INFO
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    12761 2022-11-18 08:02:32.000000 abulafia-0.1.9/README.md
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      503 2023-01-19 11:45:06.000000 abulafia-0.1.9/pyproject.toml
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       38 2023-01-19 11:45:29.228919 abulafia-0.1.9/setup.cfg
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       37 2022-08-23 07:22:48.000000 abulafia-0.1.9/setup.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.216377 abulafia-0.1.9/src/
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.218973 abulafia-0.1.9/src/abulafia/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       22 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/__init__.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.222590 abulafia-0.1.9/src/abulafia/actions/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       64 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/actions/__init__.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    23580 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/actions/actions.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.224424 abulafia-0.1.9/src/abulafia/functions/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       31 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/functions/__init__.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    24719 2022-12-02 11:46:39.000000 abulafia-0.1.9/src/abulafia/functions/core_functions.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.225536 abulafia-0.1.9/src/abulafia/observers/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       25 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/observers/__init__.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     4601 2022-09-21 13:16:09.000000 abulafia-0.1.9/src/abulafia/observers/observers.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.227755 abulafia-0.1.9/src/abulafia/task_specs/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       75 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/task_specs/__init__.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    46063 2023-01-19 11:42:16.000000 abulafia-0.1.9/src/abulafia/task_specs/core_task.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    15826 2022-09-21 10:53:07.000000 abulafia-0.1.9/src/abulafia/task_specs/pipeline.py
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    51668 2023-01-19 11:42:16.000000 abulafia-0.1.9/src/abulafia/task_specs/task_specs.py
+drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.220773 abulafia-0.1.9/src/abulafia.egg-info/
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/PKG-INFO
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      604 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/SOURCES.txt
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        1 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/dependency_links.txt
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       76 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/requires.txt
+-rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        9 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/top_level.txt
```

### Comparing `abulafia-0.1.8/LICENSE` & `abulafia-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/PKG-INFO` & `abulafia-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abulafia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for fair and reproducible crowdsourcing using Toloka
 Author: Tuomo Hiippala, Helmiina Hotti, Rosa Suviranta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 𝚊𝚋𝚞𝚕𝚊𝚏𝚒𝚊: A tool for fair and reproducible crowdsourcing
```

### Comparing `abulafia-0.1.8/README.md` & `abulafia-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia/actions/actions.py` & `abulafia-0.1.9/src/abulafia/actions/actions.py`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia/functions/core_functions.py` & `abulafia-0.1.9/src/abulafia/functions/core_functions.py`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia/observers/observers.py` & `abulafia-0.1.9/src/abulafia/observers/observers.py`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia/task_specs/core_task.py` & `abulafia-0.1.9/src/abulafia/task_specs/core_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -798,43 +798,14 @@
                         self.pool.quality_control.add_action(
                             collector=toloka.collectors.UsersAssessment(),
                             conditions=[toloka.conditions.PoolAccessRevokedReason
                                         == toloka.conditions.PoolAccessRevokedReason.RESTRICTION],
                             action=toloka.actions.ChangeOverlap(delta=1, open_pool=True)
                         )
 
-                # Set up captcha quality control
-                if 'captcha' in self.qual_conf:
-
-                    # Unpack rules into variables 
-                    freq = self.qual_conf['captcha']['frequency'].upper()
-                    success_rate = self.qual_conf['captcha']['success_rate']
-                    duration = self.qual_conf['captcha']['ban_duration']
-                    units = self.qual_conf['captcha']['ban_units'].upper()
-
-                    # Set captcha frequency according to configuration
-                    self.pool.set_captcha_frequency(freq)
-
-                    # Add quality control rule to the pool
-                    self.pool.quality_control.add_action(
-                        collector=toloka.collectors.Captcha(),
-                        conditions=[toloka.conditions.SuccessRate < success_rate],
-                        action=toloka.actions.RestrictionV2(
-                            scope=toloka.user_restriction.UserRestriction.PROJECT,
-                            duration=duration,
-                            duration_unit=units,
-                            private_comment="Too many Captcha mistakes"
-                        )
-                    )
-
-                    # Print status message
-                    msg.good(f"Added quality control rule: ban for {duration} {units.lower()} if "
-                             f"user's CAPTCHA success rate is less than {success_rate}%. "
-                             f"CAPTCHA frequency is set to {freq}.")
-
                 # Set up GoldenSet quality control (performance on control tasks)
                 if 'golden_set' in self.qual_conf:
 
                     # How many previous answers to control tasks to consider
                     history_size = self.qual_conf['golden_set']['history_size']
 
                     # Ban user if they fail control tasks with a rate higher than the threshold
```

### Comparing `abulafia-0.1.8/src/abulafia/task_specs/pipeline.py` & `abulafia-0.1.9/src/abulafia/task_specs/pipeline.py`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia/task_specs/task_specs.py` & `abulafia-0.1.9/src/abulafia/task_specs/task_specs.py`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.8/src/abulafia.egg-info/PKG-INFO` & `abulafia-0.1.9/src/abulafia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abulafia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for fair and reproducible crowdsourcing using Toloka
 Author: Tuomo Hiippala, Helmiina Hotti, Rosa Suviranta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 𝚊𝚋𝚞𝚕𝚊𝚏𝚒𝚊: A tool for fair and reproducible crowdsourcing
```

### Comparing `abulafia-0.1.8/src/abulafia.egg-info/SOURCES.txt` & `abulafia-0.1.9/src/abulafia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

