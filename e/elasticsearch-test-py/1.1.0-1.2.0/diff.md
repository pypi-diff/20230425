# Comparing `tmp/elasticsearch-test-py-1.1.0.tar.gz` & `tmp/elasticsearch-test-py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elasticsearch-test-py-1.1.0.tar", last modified: Thu Apr 11 08:56:40 2019, max compression
+gzip compressed data, was "elasticsearch-test-py-1.2.0.tar", last modified: Tue Apr 25 13:15:56 2023, max compression
```

## Comparing `elasticsearch-test-py-1.1.0.tar` & `elasticsearch-test-py-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/
--rw-rw-r--   0 maria     (1000) maria     (1000)     2467 2019-01-25 12:51:52.000000 elasticsearch-test-py-1.1.0/README.rst
--rw-rw-r--   0 maria     (1000) maria     (1000)     2467 2019-01-25 12:51:52.000000 elasticsearch-test-py-1.1.0/README
--rw-rw-r--   0 maria     (1000) maria     (1000)     4401 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)     1339 2019-04-11 08:53:08.000000 elasticsearch-test-py-1.1.0/setup.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/tests/
--rw-rw-r--   0 maria     (1000) maria     (1000)     1489 2019-01-25 09:55:23.000000 elasticsearch-test-py-1.1.0/tests/test_elasticsearch_test.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     1109 2019-01-25 12:51:52.000000 elasticsearch-test-py-1.1.0/LICENSE
--rw-rw-r--   0 maria     (1000) maria     (1000)      291 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/setup.cfg
--rw-rw-r--   0 maria     (1000) maria     (1000)      111 2019-01-25 12:51:52.000000 elasticsearch-test-py-1.1.0/MANIFEST.in
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/
--rw-rw-r--   0 maria     (1000) maria     (1000)      368 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/SOURCES.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)     4401 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)       40 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/requires.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       19 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/top_level.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        1 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/dependency_links.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2019-04-11 08:56:40.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test/
--rw-rw-r--   0 maria     (1000) maria     (1000)     3403 2019-04-11 08:52:25.000000 elasticsearch-test-py-1.1.0/src/elasticsearch_test/__init__.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1109 2023-03-28 12:24:06.000000 elasticsearch-test-py-1.2.0/LICENSE
+-rw-rw-r--   0 maria     (1000) maria     (1000)       43 2023-04-24 07:09:09.000000 elasticsearch-test-py-1.2.0/MANIFEST.in
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3405 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2568 2023-03-29 07:55:28.000000 elasticsearch-test-py-1.2.0/README
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2568 2023-03-29 07:55:28.000000 elasticsearch-test-py-1.2.0/README.rst
+-rw-rw-r--   0 maria     (1000) maria     (1000)      280 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/setup.cfg
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1208 2023-03-29 07:49:20.000000 elasticsearch-test-py-1.2.0/setup.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/src/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/src/elasticsearch_test/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3139 2023-04-25 12:58:07.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test/__init__.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3405 2023-04-25 13:15:55.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)      368 2023-04-25 13:15:56.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        1 2023-04-25 13:15:55.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       38 2023-04-25 13:15:55.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/requires.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       19 2023-04-25 13:15:55.000000 elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/top_level.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-04-25 13:15:56.045943 elasticsearch-test-py-1.2.0/tests/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1489 2023-03-28 12:24:06.000000 elasticsearch-test-py-1.2.0/tests/test_elasticsearch_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elasticsearch-test-py-1.1.0/README.rst` & `elasticsearch-test-py-1.2.0/README`

 * *Files 8% similar despite different names*

```diff
@@ -94,25 +94,31 @@
 
 Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
 
 1. Create a normal virtualenv and activate it
 
 2. Install extras ``pip install .[testing]``
 
-3. Install the needed Python versions using ``pyenv``: ``3.4``, ``3.5``, ``3.6``, ``3.7``
+3. Install the needed Python versions using ``pyenv``: ``3.8``, ``3.9``, ``3.10``, ``3.11``
 
-4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.4``
+4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.8``
 
     ::
 
-      $ pyenv virtualenv -p python3.5 3.5.6 py35
-      $ pyenv virtualenv -p python3.6 3.6.6 py36
-      $ pyenv virtualenv -p python3.7 3.7.1 py37
+      $ pyenv virtualenv -p python3.9 3.9.8 py39
+      $ pyenv virtualenv -p python3.10 3.10.8 py310
+      $ pyenv virtualenv -p python3.11 3.11.0 py311
 
-5. Activate everything and run `tox`:
+5. Setup path to Elasticsearch
 
     ::
 
-      $ pyenv shell py35 py36 py37
+      $ export ES_HOME=/opt/elasticsearch-6.8.23/
+
+6. Activate everything and run `tox`:
+
+    ::
+
+      $ pyenv shell py39 py310 py311
       $ source ./venv/bin/activate
       $ tox
```

### Comparing `elasticsearch-test-py-1.1.0/README` & `elasticsearch-test-py-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -94,25 +94,31 @@
 
 Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
 
 1. Create a normal virtualenv and activate it
 
 2. Install extras ``pip install .[testing]``
 
-3. Install the needed Python versions using ``pyenv``: ``3.4``, ``3.5``, ``3.6``, ``3.7``
+3. Install the needed Python versions using ``pyenv``: ``3.8``, ``3.9``, ``3.10``, ``3.11``
 
-4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.4``
+4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.8``
 
     ::
 
-      $ pyenv virtualenv -p python3.5 3.5.6 py35
-      $ pyenv virtualenv -p python3.6 3.6.6 py36
-      $ pyenv virtualenv -p python3.7 3.7.1 py37
+      $ pyenv virtualenv -p python3.9 3.9.8 py39
+      $ pyenv virtualenv -p python3.10 3.10.8 py310
+      $ pyenv virtualenv -p python3.11 3.11.0 py311
 
-5. Activate everything and run `tox`:
+5. Setup path to Elasticsearch
 
     ::
 
-      $ pyenv shell py35 py36 py37
+      $ export ES_HOME=/opt/elasticsearch-6.8.23/
+
+6. Activate everything and run `tox`:
+
+    ::
+
+      $ pyenv shell py39 py310 py311
       $ source ./venv/bin/activate
       $ tox
```

### Comparing `elasticsearch-test-py-1.1.0/PKG-INFO` & `elasticsearch-test-py-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,146 @@
 Metadata-Version: 2.1
 Name: elasticsearch-test-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Start Elasticsearch with Python (for testing or other purposes)
 Home-page: https://github.com/spraakbanken/elasticsearch-test-py
 Author: Språkbanken
 Author-email: maria.ohrman@gu.se
 License: MIT License
-Description: Python Elasticsearch Test
-        =========================
-        
-        Start Elasticsearch using Python.
-        
-        Settings
-        --------
-        
-        ::
-        
-            elasticsearch_test.ElasticsearchTest(
-              port=1234
-              es_path='/home/maria/elasticsearch-5.2.4'
-              data_dir='/home/maria/es-data'
-              es_java_opts='-Xms512m -Xmx512m'
-            )
-        
-        ``port``
-        
-        Default: ``9200``
-        
-        ``es_path``
-        
-        Path to the Elasticsearch directory (home of ``/bin``). Default: uses ``$ES_HOME``
-        
-        ``es_java_opts``
-        
-        Sets ``$ES_JAVA_OPTS`` for process to this value if present.
-        
-        
-        ``data_dir``
-        
-        Directory to place ``/data`` and ``/logs`` in. Default: uses ``tempfile``.
-        
-        Running
-        -------
-        
-        ::
-        
-            import time
-            import elasticsearch_test
-            instance = elasticsearch_test.ElasticsearchTest()
-        
-            # This blocks until either an error is found
-            # or Elasticsearch has been initialized.
-        
-            instance.start()
-        
-            # or
-        
-            instance.start(block=False)
-        
-            while True:
-                if instance.is_started():
-                    break
-                time.sleep(1)
-        
-        Testing
-        -------
-        
-        Use it as a resource:::
-        
-            import elasticsearch_test
-            import elasticsearch
-        
-            with elasticsearch_test.ElasticsearchTest() as instance:
-                connection_info = instance.get_connection_info()
-                client = elasticsearch.Elasticsearch(connection_info)
-        
-        
-        Use it as a Pytest fixture:::
-        
-            import elasticsearch_test
-        
-            @pytest.fixture(scope="session")
-            def es():
-                instance = elasticsearch_test.ElasticsearchTest()
-                instance.start()
-                yield instance
-                instance.stop()
-        
-        
-        When using ``data_dir``, if there are preexisting data in the directory,
-        you should also wait for the data to be initialized:::
-        
-            with elasticsearch_test.ElasticsearchTest(data_dir='my_data') as instance:
-                while not instance.is_data_initialized():
-                    time.sleep(1)
-                # do something!
-        
-        
-        Test this package
-        -----------------
-        
-        Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
-        
-        1. Create a normal virtualenv and activate it
-        
-        2. Install extras ``pip install .[testing]``
-        
-        3. Install the needed Python versions using ``pyenv``: ``3.4``, ``3.5``, ``3.6``, ``3.7``
-        
-        4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.4``
-        
-            ::
-        
-              $ pyenv virtualenv -p python3.5 3.5.6 py35
-              $ pyenv virtualenv -p python3.6 3.6.6 py36
-              $ pyenv virtualenv -p python3.7 3.7.1 py37
-        
-        5. Activate everything and run `tox`:
-        
-            ::
-        
-              $ pyenv shell py35 py36 py37
-              $ source ./venv/bin/activate
-              $ tox
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: testing
+License-File: LICENSE
+
+Python Elasticsearch Test
+=========================
+
+Start Elasticsearch using Python.
+
+Settings
+--------
+
+::
+
+    elasticsearch_test.ElasticsearchTest(
+      port=1234
+      es_path='/home/maria/elasticsearch-5.2.4'
+      data_dir='/home/maria/es-data'
+      es_java_opts='-Xms512m -Xmx512m'
+    )
+
+``port``
+
+Default: ``9200``
+
+``es_path``
+
+Path to the Elasticsearch directory (home of ``/bin``). Default: uses ``$ES_HOME``
+
+``es_java_opts``
+
+Sets ``$ES_JAVA_OPTS`` for process to this value if present.
+
+
+``data_dir``
+
+Directory to place ``/data`` and ``/logs`` in. Default: uses ``tempfile``.
+
+Running
+-------
+
+::
+
+    import time
+    import elasticsearch_test
+    instance = elasticsearch_test.ElasticsearchTest()
+
+    # This blocks until either an error is found
+    # or Elasticsearch has been initialized.
+
+    instance.start()
+
+    # or
+
+    instance.start(block=False)
+
+    while True:
+        if instance.is_started():
+            break
+        time.sleep(1)
+
+Testing
+-------
+
+Use it as a resource:::
+
+    import elasticsearch_test
+    import elasticsearch
+
+    with elasticsearch_test.ElasticsearchTest() as instance:
+        connection_info = instance.get_connection_info()
+        client = elasticsearch.Elasticsearch(connection_info)
+
+
+Use it as a Pytest fixture:::
+
+    import elasticsearch_test
+
+    @pytest.fixture(scope="session")
+    def es():
+        instance = elasticsearch_test.ElasticsearchTest()
+        instance.start()
+        yield instance
+        instance.stop()
+
+
+When using ``data_dir``, if there are preexisting data in the directory,
+you should also wait for the data to be initialized:::
+
+    with elasticsearch_test.ElasticsearchTest(data_dir='my_data') as instance:
+        while not instance.is_data_initialized():
+            time.sleep(1)
+        # do something!
+
+
+Test this package
+-----------------
+
+Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
+
+1. Create a normal virtualenv and activate it
+
+2. Install extras ``pip install .[testing]``
+
+3. Install the needed Python versions using ``pyenv``: ``3.8``, ``3.9``, ``3.10``, ``3.11``
+
+4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.8``
+
+    ::
+
+      $ pyenv virtualenv -p python3.9 3.9.8 py39
+      $ pyenv virtualenv -p python3.10 3.10.8 py310
+      $ pyenv virtualenv -p python3.11 3.11.0 py311
+
+5. Setup path to Elasticsearch
+
+    ::
+
+      $ export ES_HOME=/opt/elasticsearch-6.8.23/
+
+6. Activate everything and run `tox`:
+
+    ::
+
+      $ pyenv shell py39 py310 py311
+      $ source ./venv/bin/activate
+      $ tox
+
```

### Comparing `elasticsearch-test-py-1.1.0/setup.py` & `elasticsearch-test-py-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 from setuptools import setup
 
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Database",
     "Topic :: Software Development",
     "Topic :: Software Development :: Testing",
 ]
 
 setup(
     name='elasticsearch-test-py',
-    version='1.1.0',
+    version='1.2.0',
     description='Start Elasticsearch with Python (for testing or other purposes)',
     long_description=open('README.rst').read(),
     classifiers=classifiers,
     keywords=[],
     author='Språkbanken',
     author_email='maria.ohrman@gu.se',
     url='https://github.com/spraakbanken/elasticsearch-test-py',
@@ -35,12 +32,12 @@
     install_requires=[
     ],
     extras_require=dict(
         testing=[
             'tox',
             'pytest',
             'requests',
-            'coverage'
+            'flake8'
         ],
     ),
 
 )
```

### Comparing `elasticsearch-test-py-1.1.0/tests/test_elasticsearch_test.py` & `elasticsearch-test-py-1.2.0/tests/test_elasticsearch_test.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-test-py-1.1.0/LICENSE` & `elasticsearch-test-py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch-test-py-1.1.0/src/elasticsearch_test_py.egg-info/PKG-INFO` & `elasticsearch-test-py-1.2.0/src/elasticsearch_test_py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,146 @@
 Metadata-Version: 2.1
 Name: elasticsearch-test-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Start Elasticsearch with Python (for testing or other purposes)
 Home-page: https://github.com/spraakbanken/elasticsearch-test-py
 Author: Språkbanken
 Author-email: maria.ohrman@gu.se
 License: MIT License
-Description: Python Elasticsearch Test
-        =========================
-        
-        Start Elasticsearch using Python.
-        
-        Settings
-        --------
-        
-        ::
-        
-            elasticsearch_test.ElasticsearchTest(
-              port=1234
-              es_path='/home/maria/elasticsearch-5.2.4'
-              data_dir='/home/maria/es-data'
-              es_java_opts='-Xms512m -Xmx512m'
-            )
-        
-        ``port``
-        
-        Default: ``9200``
-        
-        ``es_path``
-        
-        Path to the Elasticsearch directory (home of ``/bin``). Default: uses ``$ES_HOME``
-        
-        ``es_java_opts``
-        
-        Sets ``$ES_JAVA_OPTS`` for process to this value if present.
-        
-        
-        ``data_dir``
-        
-        Directory to place ``/data`` and ``/logs`` in. Default: uses ``tempfile``.
-        
-        Running
-        -------
-        
-        ::
-        
-            import time
-            import elasticsearch_test
-            instance = elasticsearch_test.ElasticsearchTest()
-        
-            # This blocks until either an error is found
-            # or Elasticsearch has been initialized.
-        
-            instance.start()
-        
-            # or
-        
-            instance.start(block=False)
-        
-            while True:
-                if instance.is_started():
-                    break
-                time.sleep(1)
-        
-        Testing
-        -------
-        
-        Use it as a resource:::
-        
-            import elasticsearch_test
-            import elasticsearch
-        
-            with elasticsearch_test.ElasticsearchTest() as instance:
-                connection_info = instance.get_connection_info()
-                client = elasticsearch.Elasticsearch(connection_info)
-        
-        
-        Use it as a Pytest fixture:::
-        
-            import elasticsearch_test
-        
-            @pytest.fixture(scope="session")
-            def es():
-                instance = elasticsearch_test.ElasticsearchTest()
-                instance.start()
-                yield instance
-                instance.stop()
-        
-        
-        When using ``data_dir``, if there are preexisting data in the directory,
-        you should also wait for the data to be initialized:::
-        
-            with elasticsearch_test.ElasticsearchTest(data_dir='my_data') as instance:
-                while not instance.is_data_initialized():
-                    time.sleep(1)
-                # do something!
-        
-        
-        Test this package
-        -----------------
-        
-        Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
-        
-        1. Create a normal virtualenv and activate it
-        
-        2. Install extras ``pip install .[testing]``
-        
-        3. Install the needed Python versions using ``pyenv``: ``3.4``, ``3.5``, ``3.6``, ``3.7``
-        
-        4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.4``
-        
-            ::
-        
-              $ pyenv virtualenv -p python3.5 3.5.6 py35
-              $ pyenv virtualenv -p python3.6 3.6.6 py36
-              $ pyenv virtualenv -p python3.7 3.7.1 py37
-        
-        5. Activate everything and run `tox`:
-        
-            ::
-        
-              $ pyenv shell py35 py36 py37
-              $ source ./venv/bin/activate
-              $ tox
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: testing
+License-File: LICENSE
+
+Python Elasticsearch Test
+=========================
+
+Start Elasticsearch using Python.
+
+Settings
+--------
+
+::
+
+    elasticsearch_test.ElasticsearchTest(
+      port=1234
+      es_path='/home/maria/elasticsearch-5.2.4'
+      data_dir='/home/maria/es-data'
+      es_java_opts='-Xms512m -Xmx512m'
+    )
+
+``port``
+
+Default: ``9200``
+
+``es_path``
+
+Path to the Elasticsearch directory (home of ``/bin``). Default: uses ``$ES_HOME``
+
+``es_java_opts``
+
+Sets ``$ES_JAVA_OPTS`` for process to this value if present.
+
+
+``data_dir``
+
+Directory to place ``/data`` and ``/logs`` in. Default: uses ``tempfile``.
+
+Running
+-------
+
+::
+
+    import time
+    import elasticsearch_test
+    instance = elasticsearch_test.ElasticsearchTest()
+
+    # This blocks until either an error is found
+    # or Elasticsearch has been initialized.
+
+    instance.start()
+
+    # or
+
+    instance.start(block=False)
+
+    while True:
+        if instance.is_started():
+            break
+        time.sleep(1)
+
+Testing
+-------
+
+Use it as a resource:::
+
+    import elasticsearch_test
+    import elasticsearch
+
+    with elasticsearch_test.ElasticsearchTest() as instance:
+        connection_info = instance.get_connection_info()
+        client = elasticsearch.Elasticsearch(connection_info)
+
+
+Use it as a Pytest fixture:::
+
+    import elasticsearch_test
+
+    @pytest.fixture(scope="session")
+    def es():
+        instance = elasticsearch_test.ElasticsearchTest()
+        instance.start()
+        yield instance
+        instance.stop()
+
+
+When using ``data_dir``, if there are preexisting data in the directory,
+you should also wait for the data to be initialized:::
+
+    with elasticsearch_test.ElasticsearchTest(data_dir='my_data') as instance:
+        while not instance.is_data_initialized():
+            time.sleep(1)
+        # do something!
+
+
+Test this package
+-----------------
+
+Needed: ``pyenv`` and the plugin ``pyenv-virtualenv``.
+
+1. Create a normal virtualenv and activate it
+
+2. Install extras ``pip install .[testing]``
+
+3. Install the needed Python versions using ``pyenv``: ``3.8``, ``3.9``, ``3.10``, ``3.11``
+
+4. Setup virtualenvs for all but the Python version you are using, for example if you use ``3.8``
+
+    ::
+
+      $ pyenv virtualenv -p python3.9 3.9.8 py39
+      $ pyenv virtualenv -p python3.10 3.10.8 py310
+      $ pyenv virtualenv -p python3.11 3.11.0 py311
+
+5. Setup path to Elasticsearch
+
+    ::
+
+      $ export ES_HOME=/opt/elasticsearch-6.8.23/
+
+6. Activate everything and run `tox`:
+
+    ::
+
+      $ pyenv shell py39 py310 py311
+      $ source ./venv/bin/activate
+      $ tox
+
```

### Comparing `elasticsearch-test-py-1.1.0/src/elasticsearch_test/__init__.py` & `elasticsearch-test-py-1.2.0/src/elasticsearch_test/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 import os
 import tempfile
 import subprocess
 import string
 import random
 import json
 
-try:
-    from urllib.request import urlopen
-except ImportError:
-    # Python 2
-    from urllib import urlopen
+from urllib.request import urlopen
 
 name = "elasticsearch_test"
 
 
 class ElasticsearchTest:
 
     def __init__(self, port=9200, es_path=None, data_dir=None, es_java_opts=None):
@@ -42,27 +38,19 @@
             self.process = subprocess.Popen([executable, data_arg, logs_arg, port_arg, cluster_arg, host_arg],
                                             stdout=subprocess.PIPE,
                                             stderr=subprocess.PIPE,
                                             env=env_copy)
         except Exception:
             raise RuntimeError('Failed to start Elasticsearch')
         if block:
-            line = ''
             while True:
-                out = self.process.stdout.read(1)
-                if out == b'' and self.process.poll() is not None:
+                line = self.process.stdout.readline().decode()
+                if line == '' and self.process.poll() is not None:
                     raise RuntimeError('Failed to start Elasticsearch')
-                if out:
-                    char = out.decode()
-                    if char != '\n':
-                        line += char
-                    else:
-                        line = ''
-
-                if 'started' in line:
+                if 'Node' in line and 'started' in line:
                     self.started = True
                     break
 
     def is_started(self):
         return self._check_status(('green', 'yellow'))
 
     def is_data_initialized(self):
```

