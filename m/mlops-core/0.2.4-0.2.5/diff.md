# Comparing `tmp/mlops_core-0.2.4.tar.gz` & `tmp/mlops_core-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_core-0.2.4.tar", max compression
+gzip compressed data, was "mlops_core-0.2.5.tar", max compression
```

## Comparing `mlops_core-0.2.4.tar` & `mlops_core-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       13 2023-04-25 04:25:05.336475 mlops_core-0.2.4/README.md
--rw-r--r--   0        0        0      449 2023-04-25 04:25:05.337086 mlops_core-0.2.4/mlops_core/bootstrap.py
--rw-r--r--   0        0        0     5483 2023-04-25 04:25:05.337678 mlops_core-0.2.4/mlops_core/connectivity/networking.py
--rw-r--r--   0        0        0      878 2023-04-25 04:25:05.338269 mlops_core-0.2.4/mlops_core/connector/kaggle.py
--rw-r--r--   0        0        0      973 2023-04-25 04:25:05.338982 mlops_core-0.2.4/mlops_core/detection/project_arguments.py
--rw-r--r--   0        0        0     3654 2023-04-25 04:25:05.339441 mlops_core-0.2.4/mlops_core/detection/project_configurations.py
--rw-r--r--   0        0        0     4251 2023-04-25 04:25:05.339927 mlops_core-0.2.4/mlops_core/detection/project_structure.py
--rw-r--r--   0        0        0     6616 2023-04-25 04:25:05.340638 mlops_core-0.2.4/mlops_core/generator/project_generator.py
--rw-r--r--   0        0        0      165 2023-04-25 04:25:05.341011 mlops_core-0.2.4/mlops_core/runtime.py
--rw-r--r--   0        0        0      366 2023-04-25 04:25:05.341616 mlops_core-0.2.4/mlops_core/utils/strings.py
--rw-r--r--   0        0        0      441 2023-04-25 05:06:20.856114 mlops_core-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      143 2023-04-25 04:25:05.343114 mlops_core-0.2.4/templates/ISSUE_TEMPLATE.md.jinja
--rw-r--r--   0        0        0       46 2023-04-25 04:25:05.343455 mlops_core-0.2.4/templates/PULL_REQUEST_TEMPLATE.md.jinja
--rw-r--r--   0        0        0       20 2023-04-25 04:25:05.343741 mlops_core-0.2.4/templates/README.md.jinja
--rw-r--r--   0        0        0      266 2023-04-25 04:25:05.344084 mlops_core-0.2.4/templates/devcontainer.json
--rw-r--r--   0        0        0      737 2023-04-25 04:25:05.344644 mlops_core-0.2.4/templates/src/evaluate.py.jinja
--rw-r--r--   0        0        0      560 2023-04-25 04:25:05.345020 mlops_core-0.2.4/templates/src/ingestion.py.jinja
--rw-r--r--   0        0        0     1155 2023-04-25 04:25:05.345373 mlops_core-0.2.4/templates/src/train.py.jinja
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 mlops_core-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-25 04:25:05.336475 mlops_core-0.2.5/README.md
+-rw-r--r--   0        0        0      449 2023-04-25 04:25:05.337086 mlops_core-0.2.5/mlops_core/bootstrap.py
+-rw-r--r--   0        0        0     5483 2023-04-25 04:25:05.337678 mlops_core-0.2.5/mlops_core/connectivity/networking.py
+-rw-r--r--   0        0        0      878 2023-04-25 04:25:05.338269 mlops_core-0.2.5/mlops_core/connector/kaggle.py
+-rw-r--r--   0        0        0      973 2023-04-25 04:25:05.338982 mlops_core-0.2.5/mlops_core/detection/project_arguments.py
+-rw-r--r--   0        0        0     3654 2023-04-25 04:25:05.339441 mlops_core-0.2.5/mlops_core/detection/project_configurations.py
+-rw-r--r--   0        0        0     4251 2023-04-25 04:25:05.339927 mlops_core-0.2.5/mlops_core/detection/project_structure.py
+-rw-r--r--   0        0        0     6616 2023-04-25 04:25:05.340638 mlops_core-0.2.5/mlops_core/generator/project_generator.py
+-rw-r--r--   0        0        0      165 2023-04-25 04:25:05.341011 mlops_core-0.2.5/mlops_core/runtime.py
+-rw-r--r--   0        0        0      366 2023-04-25 04:25:05.341616 mlops_core-0.2.5/mlops_core/utils/strings.py
+-rw-r--r--   0        0        0      441 2023-04-25 05:08:08.118246 mlops_core-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-04-25 04:25:05.343114 mlops_core-0.2.5/templates/ISSUE_TEMPLATE.md.jinja
+-rw-r--r--   0        0        0       46 2023-04-25 04:25:05.343455 mlops_core-0.2.5/templates/PULL_REQUEST_TEMPLATE.md.jinja
+-rw-r--r--   0        0        0       20 2023-04-25 04:25:05.343741 mlops_core-0.2.5/templates/README.md.jinja
+-rw-r--r--   0        0        0      266 2023-04-25 04:25:05.344084 mlops_core-0.2.5/templates/devcontainer.json
+-rw-r--r--   0        0        0      737 2023-04-25 04:25:05.344644 mlops_core-0.2.5/templates/src/evaluate.py.jinja
+-rw-r--r--   0        0        0      560 2023-04-25 04:25:05.345020 mlops_core-0.2.5/templates/src/ingestion.py.jinja
+-rw-r--r--   0        0        0     1155 2023-04-25 04:25:05.345373 mlops_core-0.2.5/templates/src/train.py.jinja
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 mlops_core-0.2.5/PKG-INFO
```

### Comparing `mlops_core-0.2.4/mlops_core/connectivity/networking.py` & `mlops_core-0.2.5/mlops_core/connectivity/networking.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/mlops_core/connector/kaggle.py` & `mlops_core-0.2.5/mlops_core/connector/kaggle.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/mlops_core/detection/project_arguments.py` & `mlops_core-0.2.5/mlops_core/detection/project_arguments.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/mlops_core/detection/project_configurations.py` & `mlops_core-0.2.5/mlops_core/detection/project_configurations.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/mlops_core/detection/project_structure.py` & `mlops_core-0.2.5/mlops_core/detection/project_structure.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/mlops_core/generator/project_generator.py` & `mlops_core-0.2.5/mlops_core/generator/project_generator.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/templates/src/evaluate.py.jinja` & `mlops_core-0.2.5/templates/src/evaluate.py.jinja`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/templates/src/ingestion.py.jinja` & `mlops_core-0.2.5/templates/src/ingestion.py.jinja`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.4/templates/src/train.py.jinja` & `mlops_core-0.2.5/templates/src/train.py.jinja`

 * *Files identical despite different names*

