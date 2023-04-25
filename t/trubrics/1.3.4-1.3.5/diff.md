# Comparing `tmp/trubrics-1.3.4.tar.gz` & `tmp/trubrics-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.3.4.tar", last modified: Thu Apr 20 17:33:10 2023, max compression
+gzip compressed data, was "trubrics-1.3.5.tar", last modified: Tue Apr 25 12:42:39 2023, max compression
```

## Comparing `trubrics-1.3.4.tar` & `trubrics-1.3.5.tar`

### file list

```diff
@@ -1,79 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-20 17:33:00.000000 trubrics-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 17:33:10.468799 trubrics-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-20 17:33:00.000000 trubrics-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/my_new_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 17:33:00.000000 trubrics-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 17:33:00.000000 trubrics-1.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-20 17:33:10.468799 trubrics-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-20 17:33:00.000000 trubrics-1.3.4/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-25 12:42:28.000000 trubrics-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-25 12:42:39.696141 trubrics-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-25 12:42:28.000000 trubrics-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/examples/classification_titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/custom_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-25 12:42:28.000000 trubrics-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 12:42:28.000000 trubrics-1.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-25 12:42:39.696141 trubrics-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-25 12:42:28.000000 trubrics-1.3.5/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.3.4/LICENSE` & `trubrics-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/README.md` & `trubrics-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/examples/classification_titanic/custom_validator.py` & `trubrics-1.3.5/examples/classification_titanic/custom_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/setup.cfg` & `trubrics-1.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.3.4
+version = 1.3.5
 description = Combine data science knowledge with business user feedback to validate machine learning.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `trubrics-1.3.4/tests/test_context.py` & `trubrics-1.3.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/cli/main.py` & `trubrics-1.3.5/trubrics/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,31 +199,29 @@
         subprocess.call(["python3", filename])
 
 
 @app.command()
 def run(
     save_ui: bool = typer.Option(False, prompt="Would you like to save your trubric to the UI?"),
     run_context_path: str = typer.Option(
-        default="titanic-example-trubric", prompt="Enter the path to your trubric run .py file. Press enter for example"
-    ),
-    trubric_output_file_path: str = typer.Option(
-        "./my_new_trubric.json",
-        prompt="Enter a local path to save your output trubric file. Press enter for default path",
+        default="example", prompt="Enter the path to your trubric run .py file. Press enter for an"
     ),
+    trubric_output_file_path: str = "./my_new_trubric.json",
     raise_on_failure: bool = True,
 ):
     """Runs an example trubric (list of model validations) on the titanic dataset.
 
     Args:
         save_ui: whether to save validations to the UI with in app user authentication
         run_context_path: path to the trubrics run context
         trubric_output_file_path: path to save your output trubric file
+        raise_on_failure: raise an exception on failure of trubric
     """
     trubric_run_path = None
-    if run_context_path != "titanic-example-trubric":
+    if run_context_path != "example":
         trubric_run_path = Path(run_context_path).absolute()
         if not trubric_run_path.exists():
             rprint(f"[red]Path '{trubric_run_path}' not found.[red]")
             raise typer.Abort()
         rc = validate_trubric_run_context(str(trubric_run_path)).RUN_CONTEXT
     else:
         from trubrics.example.trubric_run import RUN_CONTEXT as rc  # type: ignore
```

### Comparing `trubrics-1.3.4/trubrics/cli/run.py` & `trubrics-1.3.5/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/context.py` & `trubrics-1.3.5/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/example/app_titanic_streamlit.py` & `trubrics-1.3.5/trubrics/example/app_titanic_streamlit.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/example/titanic.py` & `trubrics-1.3.5/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/example/titanic_data.csv` & `trubrics-1.3.5/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/example/trubric_run.py` & `trubrics-1.3.5/trubrics/example/trubric_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from trubrics.validations import Trubric
 from trubrics.validations.run import TrubricRun
 
 train_df, test_df, model = get_titanic_data_and_model()
 
 data_context = DataContext(
     name="titanic_dataset",
+    version="0.0.1",
     testing_data=test_df,
     minimum_functionality_data=test_df.iloc[:5],
     training_data=train_df,
     target="Survived",
 )
 
 # Note: This method of reading json is only necessary from within python package.
```

### Comparing `trubrics-1.3.4/trubrics/exceptions.py` & `trubrics-1.3.5/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/feedback/config.py` & `trubrics-1.3.5/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/feedback/dataclass.py` & `trubrics-1.3.5/trubrics/feedback/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/integrations/dash/collect.py` & `trubrics-1.3.5/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/integrations/gradio/collect.py` & `trubrics-1.3.5/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.3.5/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/integrations/streamlit/collect.py` & `trubrics-1.3.5/trubrics/integrations/streamlit/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.3.5/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/ui/auth.py` & `trubrics-1.3.5/trubrics/ui/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/ui/firestore.py` & `trubrics-1.3.5/trubrics/ui/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/ui/trubrics_config.py` & `trubrics-1.3.5/trubrics/ui/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/validations/dataclass.py` & `trubrics-1.3.5/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/validations/model/base.py` & `trubrics-1.3.5/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/validations/run.py` & `trubrics-1.3.5/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics/validations/validation_output.py` & `trubrics-1.3.5/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.4/trubrics.egg-info/SOURCES.txt` & `trubrics-1.3.5/trubrics.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 examples/__init__.py
 examples/classification_titanic/__init__.py
 examples/classification_titanic/custom_scorer.py
 examples/classification_titanic/custom_validator.py
-examples/classification_titanic/my_first_trubric.json
-examples/classification_titanic/my_new_trubric.json
 examples/classification_titanic/slicing_functions.py
 tests/test_context.py
 trubrics/__init__.py
 trubrics/context.py
 trubrics/exceptions.py
 trubrics/py.typed
 trubrics.egg-info/PKG-INFO
```

