# Comparing `tmp/awehflow-2.2.3.1.tar.gz` & `tmp/awehflow-2.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awehflow-2.2.3.1.tar", last modified: Tue Apr 25 11:43:32 2023, max compression
+gzip compressed data, was "dist/awehflow-2.4.3.0.tar", last modified: Fri Mar 10 09:10:01 2023, max compression
```

## Comparing `awehflow-2.2.3.1.tar` & `awehflow-2.4.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10513 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10068 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow/alerts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/alerts/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/alerts/googlechat.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/alerts/slack.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/config.py
--rw-rw-rw-   0 root         (0) root         (0)    13093 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/events/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/events/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/events/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow/operators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5996 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/etl.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/flow.py
--rw-rw-rw-   0 root         (0) root         (0)    10398 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/gcs.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7215 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/operators/taxonomy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/sensors/http.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/sensors/sql_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/awehflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10513 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/awehflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:43:32.000000 awehflow-2.2.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-25 11:43:14.000000 awehflow-2.2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/googlechat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/slack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/operators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/etl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8454 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/gcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7215 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/taxonomy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/sql_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      778 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/setup.py
```

### Comparing `awehflow-2.2.3.1/LICENSE` & `awehflow-2.4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/PKG-INFO` & `awehflow-2.4.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awehflow
-Version: 2.2.3.1
+Version: 2.4.3.0
 Summary: Configuration based Apache Airflow
 Home-page: UNKNOWN
 Author: Philip Perold
 Author-email: philip@spatialedge.co.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,73 +20,14 @@
 ![coverage report](https://gitlab.com/spatialedge/awehflow/badges/master/coverage.svg)
 ![pipeline status](https://gitlab.com/spatialedge/awehflow/badges/master/pipeline.svg)
 
 Configuration based Airflow pipelines with metric logging and alerting out the box.
 
 ## Prerequisites
 
-### Development environment
-In order to develop awehflow for a given version of Airflow follow these steps
-1. Install and configure miniconda
-  1. On Mac, if running ARM create an x86 version of conda using the snippet below
-    ```bash
-    ### add this to ~/.zshrc (or ~/.bashrc if you're using Bash)
-    create_x86_conda_environment () {
-      # create a conda environment using x86 architecture
-      # first argument is environment name, all subsequent arguments will be passed to `conda create`
-      # example usage: create_x86_conda_environment myenv_x86 python=3.9
-      
-      CONDA_SUBDIR=osx-64 conda create $@
-      conda activate $2
-      conda config --env --set subdir osx-64
-    }
-  ```
-1. Define the version that you'd like to install
-  ```bash
-  export AIRFLOW_VERSION="2.1.4"
-  ```
-1. Create a conda environment for your version of Airflow, the bash below
-  ```bash
-  create_x86_conda_environment -n "airflow_$AIRFLOW_VERSION" "python=3.8.12"
-  ```
-1. Configure the AIRFLOW_HOME directory
-  ```bash
-  conda deactivate
-  conda activate "airflow_$AIRFLOW_VERSION"
-  conda env config vars set AIRFLOW_HOME="$HOME/airflow/airflow_$AIRFLOW_VERSION"
-  conda deactivate
-  conda activate airflow_"$AIRFLOW_VERSION"
-  echo "$AIRFLOW_HOME"
-  ```
-1. Install airflow using `pip`
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow==$AIRFLOW_VERSION"
-  ```
-1. Install required providers
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow[google]==$AIRFLOW_VERSION"
-  pip install --no-cache-dir "apache-airflow[postgres]==$AIRFLOW_VERSION"
-  ```
-  1. On MacOS ARM install the psycop binary
-    ```bash
-    pip install --no-cache-dir "psycopg2-binary==`pip list | grep -i 'psycopg2 ' | tr -s ' ' | cut -d' ' -f 2`"
-    ```
-1. Customisation per version
-  1. For `2.2.3`
-    1. force the MarkupSafe package version
-      ```bash
-      pip install --no-cache-dir markupsafe==2.0.1
-      ```
-1. Init the airflow db
-  ```bash
-  airflow db init
-  ```
-
 You will need the following to run this code:
   * Python 3
 
 ## Installation
 
 ```
 pip install awehflow[default]
```

### Comparing `awehflow-2.2.3.1/README.md` & `awehflow-2.4.3.0/awehflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,33 @@
+Metadata-Version: 2.1
+Name: awehflow
+Version: 2.4.3.0
+Summary: Configuration based Apache Airflow
+Home-page: UNKNOWN
+Author: Philip Perold
+Author-email: philip@spatialedge.co.za
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: default
+Provides-Extra: composer
+License-File: LICENSE
+
 # Awehflow
 
 ![coverage report](https://gitlab.com/spatialedge/awehflow/badges/master/coverage.svg)
 ![pipeline status](https://gitlab.com/spatialedge/awehflow/badges/master/pipeline.svg)
 
 Configuration based Airflow pipelines with metric logging and alerting out the box.
 
 ## Prerequisites
 
-### Development environment
-In order to develop awehflow for a given version of Airflow follow these steps
-1. Install and configure miniconda
-  1. On Mac, if running ARM create an x86 version of conda using the snippet below
-    ```bash
-    ### add this to ~/.zshrc (or ~/.bashrc if you're using Bash)
-    create_x86_conda_environment () {
-      # create a conda environment using x86 architecture
-      # first argument is environment name, all subsequent arguments will be passed to `conda create`
-      # example usage: create_x86_conda_environment myenv_x86 python=3.9
-      
-      CONDA_SUBDIR=osx-64 conda create $@
-      conda activate $2
-      conda config --env --set subdir osx-64
-    }
-  ```
-1. Define the version that you'd like to install
-  ```bash
-  export AIRFLOW_VERSION="2.1.4"
-  ```
-1. Create a conda environment for your version of Airflow, the bash below
-  ```bash
-  create_x86_conda_environment -n "airflow_$AIRFLOW_VERSION" "python=3.8.12"
-  ```
-1. Configure the AIRFLOW_HOME directory
-  ```bash
-  conda deactivate
-  conda activate "airflow_$AIRFLOW_VERSION"
-  conda env config vars set AIRFLOW_HOME="$HOME/airflow/airflow_$AIRFLOW_VERSION"
-  conda deactivate
-  conda activate airflow_"$AIRFLOW_VERSION"
-  echo "$AIRFLOW_HOME"
-  ```
-1. Install airflow using `pip`
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow==$AIRFLOW_VERSION"
-  ```
-1. Install required providers
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow[google]==$AIRFLOW_VERSION"
-  pip install --no-cache-dir "apache-airflow[postgres]==$AIRFLOW_VERSION"
-  ```
-  1. On MacOS ARM install the psycop binary
-    ```bash
-    pip install --no-cache-dir "psycopg2-binary==`pip list | grep -i 'psycopg2 ' | tr -s ' ' | cut -d' ' -f 2`"
-    ```
-1. Customisation per version
-  1. For `2.2.3`
-    1. force the MarkupSafe package version
-      ```bash
-      pip install --no-cache-dir markupsafe==2.0.1
-      ```
-1. Init the airflow db
-  ```bash
-  airflow db init
-  ```
-
 You will need the following to run this code:
   * Python 3
 
 ## Installation
 
 ```
 pip install awehflow[default]
@@ -297,7 +255,9 @@
 
 or to run code coverage too:
 
 ```bash
 coverage run -m unittest discover tests && coverage html
 ```
 
+
+
```

### Comparing `awehflow-2.2.3.1/awehflow/alerts/googlechat.py` & `awehflow-2.4.3.0/awehflow/alerts/googlechat.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/alerts/slack.py` & `awehflow-2.4.3.0/awehflow/alerts/slack.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/config.py` & `awehflow-2.4.3.0/awehflow/config.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/core.py` & `awehflow-2.4.3.0/awehflow/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import os
 from pyhocon import ConfigFactory
 
 import pendulum
 from pendulum.tz import timezone as pd_tz
 
 import yaml
-from airflow.version import version as airflow_version
-from airflow.models.dag import DAG
+from airflow import DAG
 from airflow.configuration import conf as airflow_config
 from airflow.utils.trigger_rule import TriggerRule
 from jinja2.utils import import_string
 
 from awehflow.config import Config
 from awehflow.events.alerts import AlertsEventHandler
 from awehflow.operators.flow import StartOperator
@@ -132,43 +131,28 @@
             'end_date': config.get('end_date'),
             'email_on_failure': False,
             'email_on_retry': False,
             'retries': 0,
             'on_failure_callback': self.generate_on_failure_callback(config, event_handlers)
         }, config.get('default_dag_args'))
 
-        local_airflow_version = int(airflow_version.replace('.', ''))
-
-        concurrency_default = None
-        if local_airflow_version < 220:
-            concurrency_default = airflow_config.getint('core', 'dag_concurrency')
-        else:
-            concurrency_default = airflow_config.getint('core', 'max_active_tasks_per_dag')
-
-        dag_kwargs = dict()
-        dag_kwargs['dag_id'] = config.get('dag_id') # type: ignore
-        dag_kwargs['description'] = config.get('description')
-        dag_kwargs['schedule_interval'] = config.get('schedule')
-        dag_kwargs['catchup'] = config.get('catchup', False)
-        dag_kwargs['template_searchpath'] = self.configs_path
-        dag_kwargs['user_defined_macros'] = self.generate_user_defined_macros(config)
-        dag_kwargs['default_args'] = default_dag_args
-        dag_kwargs['concurrency'] = config.get('concurrency', config.get('dag_concurrency', concurrency_default)) # type: ignore
-        
-        if local_airflow_version >= 220:
-            dag_kwargs['max_active_tasks'] = config.get('max_active_tasks', airflow_config.getint('core', 'max_active_tasks_per_dag'))
-        
-        dag_kwargs['max_active_runs'] = config.get('max_active_runs', airflow_config.getint('core', 'max_active_runs_per_dag'))
-        dag_kwargs['dagrun_timeout'] = config.get('dagrun_timeout', None)
-        dag_kwargs['doc_md'] = config.get('doc_md', None)
-        dag_kwargs['access_control'] = config.get('access_control', None)
-        dag_kwargs['is_paused_upon_creation'] = config.get('is_paused_upon_creation', None)
-        dag_kwargs['tags'] = config.get('tags', None)
-
-        dag = DAG(**dag_kwargs)
+        dag = DAG(dag_id=config.get('dag_id'), # type: ignore
+            description=config.get('description'),
+            schedule=config.get('schedule'),
+            catchup=config.get('catchup', False),
+            template_searchpath=self.configs_path,
+            user_defined_macros=self.generate_user_defined_macros(config),
+            default_args=default_dag_args,
+            max_active_tasks=config.get('max_active_tasks_per_dag', airflow_config.getint('core', 'max_active_tasks_per_dag')),
+            max_active_runs=config.get('max_active_runs_per_dag', airflow_config.getint('core', 'max_active_runs_per_dag')),
+            dagrun_timeout=config.get('dagrun_timeout', None),
+            doc_md=config.get('doc_md', None),
+            access_control=config.get('access_control', None),
+            is_paused_upon_creation=config.get('is_paused_upon_creation', None),
+            tags=config.get('tags', None))
 
         start = StartOperator(
             task_id='start',
             dag=dag,
             project=self.project,
             job_name=config.get('name'),
             engineers=config.get('engineers'),
```

### Comparing `awehflow-2.2.3.1/awehflow/events/base.py` & `awehflow-2.4.3.0/awehflow/events/base.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/events/gcp.py` & `awehflow-2.4.3.0/awehflow/events/gcp.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/events/postgres.py` & `awehflow-2.4.3.0/awehflow/events/postgres.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/operators/etl.py` & `awehflow-2.4.3.0/awehflow/operators/etl.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/operators/flow.py` & `awehflow-2.4.3.0/awehflow/operators/flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.decorators import apply_defaults
-from airflow.version import version as airflow_version
 
 from awehflow.utils import utc_now, JobStatus
 
 
 class EventEmittingOperator(BaseOperator):
     @apply_defaults
     def __init__(
@@ -52,28 +51,23 @@
         self.project = project
         self.job_name = job_name
         self.engineers = engineers
 
 
 class StartOperator(FlowOperator):
     def execute(self, context):
-        if int(airflow_version.replace('.', '')) < 220:
-            next_execution_date = context['next_execution_date']
-        else:
-            next_execution_date = context['data_interval_end']
-
         self.emit_event('start', {
             'run_id': context['dag_run'].run_id,
             'dag_id': self.dag.dag_id,
             'name': self.job_name,
             'project': self.project,
             'engineers': self.engineers,
             'status': JobStatus.RUNNING,
             'start_time': utc_now(),
-            'reference_time': next_execution_date
+            'reference_time': context['next_execution_date']
         })
 
 
 class SuccessOperator(FlowOperator):
     def execute(self, context):
         self.emit_event('success', {
             'run_id': context['dag_run'].run_id,
```

### Comparing `awehflow-2.2.3.1/awehflow/operators/gcp.py` & `awehflow-2.4.3.0/awehflow/operators/gcp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-from airflow.version import version as airflow_version
 from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 from airflow.providers.google.cloud.operators.bigquery import BigQueryExecuteQueryOperator
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
 from airflow.models.skipmixin import SkipMixin
 from airflow.utils.decorators import apply_defaults
 
@@ -23,60 +22,28 @@
                  **kwargs):
         super(BigQueryJobOperator, self).__init__(*args, **kwargs)
         self.cleanup_query = cleanup_query 
                 
 
     def execute(self, context):
         if self.hook is None:
-            hook_kwargs=dict()
-            hook_kwargs['gcp_conn_id'] = self.gcp_conn_id
-            hook_kwargs['use_legacy_sql'] = self.use_legacy_sql
-            hook_kwargs['location'] = self.location
-
-            if int(airflow_version.replace('.', '')) < 240:
-                hook_kwargs['delegate_to'] = self.delegate_to
-            else:
-                hook_kwargs['impersonation_chain'] = self.impersonation_chain
-
             self.hook = BigQueryHook(
-                **hook_kwargs
+                gcp_conn_id=self.gcp_conn_id,
+                use_legacy_sql=self.use_legacy_sql,
+                delegate_to=self.delegate_to,
+                location=self.location,
+                impersonation_chain=self.impersonation_chain,
             )
             credential_email = self.hook._get_credentials_email()
             self.log.info(f"Created BigQueryHook with account: {credential_email}")
 
         if self.cleanup_query:
-            if self.destination_dataset_table == None:
-                raise ValueError('No destination_dataset_table was given, set a destination_dataset_table in the following format: project_id.dataset_id.table_id')
-            
-            replaced_destination_dataset_table = self.destination_dataset_table.replace(':', '.')
-            split_destination_dataset_table = replaced_destination_dataset_table.split(".")
-
-            if len(split_destination_dataset_table) != 3:
-                raise ValueError('Please set a destination_dataset_table in the following format: project_id.dataset_id.table_id')
-        
-            project_id = split_destination_dataset_table[0]
-            dataset_id = split_destination_dataset_table[1]
-            table_id = split_destination_dataset_table[2]
-            
-            self.log.info('Checking if table exist: {}.{}.{}'.format(project_id, dataset_id, table_id))
-            
-            if self.hook.table_exists(project_id=project_id, dataset_id=dataset_id, table_id=table_id):
-                self.log.info('Table exists')
-
-                self.log.info('Executing cleanup query: {}'.format(self.cleanup_query))
-                cleanup_job_id = self.hook.run_query(sql=self.cleanup_query)
-            
-                qj = self.hook.get_job(job_id=cleanup_job_id)
-                while not qj.done():
-                    self.log.info(f'Waiting for job [{cleanup_job_id}] to complete...')
-                    time.sleep(1)
-
-                self.log.info('Completed execution of cleanup query')   
-            else:
-                self.log.info('Table does not exist, cleanup query was not executed') 
+            self.log.info('Executing cleanup query: {}'.format(self.cleanup_query))
+            self.hook.run(sql=self.cleanup_query)
+            self.log.info('Completed execution of cleanup query')
 
         if isinstance(self.sql, str):
             self.sql = [self.sql]
         
         job_id = []
         if isinstance(self.sql, Iterable):
             for s in self.sql:
@@ -118,15 +85,15 @@
     """
 
     @apply_defaults
     def __init__(
             self,
             task_ids: list=[],
             xcom_key: str='return_value',
-            bigquery_conn_id: str=None, # type: ignore
+            bigquery_conn_id: str=None,
             gcp_conn_id: str='google_cloud_default',
             *args, **kwargs):
         """
         :param task_ids: List of task_ids saying which tasks to sink their job_metrics for
         :param xcom_key: XCOM key used to pull the bigquery job id from the specified tasks
         """
         self.task_ids = task_ids
@@ -135,19 +102,14 @@
         if bigquery_conn_id:
             self.gcp_conn_id = bigquery_conn_id
 
         super(BigQueryJobTaskMetricOperator, self).__init__(*args, **kwargs)
 
 
     def execute(self, context):
-        if int(airflow_version.replace('.', '')) < 220:
-            next_execution_date = context['next_execution_date']
-        else:
-            next_execution_date = context['data_interval_end']
-    
         hook = BigQueryHook(
             gcp_conn_id=self.gcp_conn_id
         )
         credential_email = hook._get_credentials_email()
         self.log.info(f"Created BigQueryHook with account: {credential_email}")
 
         jobs = hook.get_service().jobs()
@@ -167,15 +129,15 @@
                     self.emit_event('task_metric', {
                         'run_id': context['dag_run'].run_id,
                         'dag_id': self.dag.dag_id,
                         'job_name': context['task'].params.get('job_name', ''),
                         'task_id': task_id,
                         'value': job,
                         'created_time': utc_now(),
-                        'reference_time': next_execution_date
+                        'reference_time': context['next_execution_date']
                     })
 
 
 class BigQueryShortCircuitOperator(BaseOperator, SkipMixin):
     """
     A "short circuit" operator that can be used a a "pre check" system.  The supplied sql statement should turn a single BOOL column.
 
@@ -188,15 +150,15 @@
     template_ext = ('.sql',)
 
     @apply_defaults
     def __init__(
             self,
             sql: str,
             gcp_conn_id: str='google_cloud_default',
-            bigquery_conn_id: str=None, # type: ignore
+            bigquery_conn_id: str=None,
             use_legacy_sql: bool=True,
             *args, **kwargs):
         
         self.sql = sql
         self.gcp_conn_id = gcp_conn_id
         if bigquery_conn_id:
             self.gcp_conn_id = bigquery_conn_id
```

### Comparing `awehflow-2.2.3.1/awehflow/operators/gcs.py` & `awehflow-2.4.3.0/awehflow/operators/gcs.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/operators/metrics.py` & `awehflow-2.4.3.0/awehflow/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/operators/taxonomy.py` & `awehflow-2.4.3.0/awehflow/operators/taxonomy.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/sensors/http.py` & `awehflow-2.4.3.0/awehflow/sensors/http.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow/sensors/sql_sensor.py` & `awehflow-2.4.3.0/awehflow/sensors/sql_sensor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from time import sleep
 from datetime import timedelta
-
-from airflow.version import version as airflow_version
 from airflow.utils import timezone
+
 from airflow.models.taskreschedule import TaskReschedule
 from airflow.exceptions import AirflowSensorTimeout, AirflowSkipException, AirflowRescheduleException
-
-if int(airflow_version.replace('.', '')) < 240:
-    from airflow.sensors.sql import SqlSensor
-else:
-    from airflow.providers.common.sql.sensors.sql import SqlSensor
+from airflow.providers.common.sql.sensors.sql import SqlSensor
 
 class SqlSensor(SqlSensor):
     """
     Override of the default SqlSensor with modified 'execute' logic.  Sensor now fails quitely in soft_fail mode
     """
     def execute(self, context):
         started_at = timezone.utcnow()
```

### Comparing `awehflow-2.2.3.1/awehflow/utils.py` & `awehflow-2.4.3.0/awehflow/utils.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/awehflow.egg-info/SOURCES.txt` & `awehflow-2.4.3.0/awehflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awehflow-2.2.3.1/setup.py` & `awehflow-2.4.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 with open('requirements.txt') as req:
     requirements = list(filter(None, [x if 'github.com' not in x else None for x in req.read().split('\n')]))
 
 EXCLUDE_FROM_PACKAGES = ['docs', 'tests*']
 
 EXTRAS_REQUIREMENTS = {
     'default': [
-        'apache-airflow==2.1.4'
+        'apache-airflow==1.10.9'
     ],
     'composer': [
-        'apache-airflow==2.1.4+composer'
+        'apache-airflow==1.10.9-composer'
     ]
 }
 
 setuptools.setup(
     name="awehflow",
     version=version.strip('v'),
     author="Philip Perold",
```

