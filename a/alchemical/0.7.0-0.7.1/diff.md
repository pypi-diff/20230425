# Comparing `tmp/alchemical-0.7.0.tar.gz` & `tmp/alchemical-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemical-0.7.0.tar", last modified: Sat Mar 18 15:35:22 2023, max compression
+gzip compressed data, was "alchemical-0.7.1.tar", last modified: Mon Apr 24 23:05:08 2023, max compression
```

## Comparing `alchemical-0.7.0.tar` & `alchemical-0.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.840268 alchemical-0.7.0/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2021-05-30 15:56:21.000000 alchemical-0.7.0/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       51 2022-11-27 15:05:05.000000 alchemical-0.7.0/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1104 2023-03-18 15:35:22.840530 alchemical-0.7.0/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      538 2021-07-06 22:28:03.000000 alchemical-0.7.0/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-05-30 15:56:36.000000 alchemical-0.7.0/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      766 2023-03-18 15:35:22.841686 alchemical-0.7.0/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-05-30 15:56:31.000000 alchemical-0.7.0/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.812280 alchemical-0.7.0/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.821305 alchemical-0.7.0/src/alchemical/
--rw-r--r--   0 mgrinberg   (502) staff       (20)       43 2021-08-01 09:16:33.000000 alchemical-0.7.0/src/alchemical/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5747 2023-03-16 23:18:22.000000 alchemical-0.7.0/src/alchemical/aio.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.829132 alchemical-0.7.0/src/alchemical/alembic/
--rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2022-11-26 23:31:47.000000 alchemical-0.7.0/src/alchemical/alembic/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1154 2022-11-27 17:09:09.000000 alchemical-0.7.0/src/alchemical/alembic/cli.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4742 2022-11-27 17:15:39.000000 alchemical-0.7.0/src/alchemical/alembic/env.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.813262 alchemical-0.7.0/src/alchemical/alembic/templates/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.834248 alchemical-0.7.0/src/alchemical/alembic/templates/generic/
--rw-r--r--   0 mgrinberg   (502) staff       (20)       37 2022-11-27 00:06:47.000000 alchemical-0.7.0/src/alchemical/alembic/templates/generic/README
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3478 2022-11-27 12:11:34.000000 alchemical-0.7.0/src/alchemical/alembic/templates/generic/alembic.ini.mako
--rw-r--r--   0 mgrinberg   (502) staff       (20)      954 2022-11-27 14:17:50.000000 alchemical-0.7.0/src/alchemical/alembic/templates/generic/env.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      965 2022-11-26 23:33:15.000000 alchemical-0.7.0/src/alchemical/alembic/templates/generic/script.py.mako
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10404 2023-03-16 23:21:30.000000 alchemical-0.7.0/src/alchemical/core.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2726 2021-10-03 15:43:23.000000 alchemical-0.7.0/src/alchemical/flask.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.826635 alchemical-0.7.0/src/alchemical.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1104 2023-03-18 15:35:22.000000 alchemical-0.7.0/src/alchemical.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      769 2023-03-18 15:35:22.000000 alchemical-0.7.0/src/alchemical.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-03-18 15:35:22.000000 alchemical-0.7.0/src/alchemical.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-05-30 16:00:37.000000 alchemical-0.7.0/src/alchemical.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       19 2023-03-18 15:35:22.000000 alchemical-0.7.0/src/alchemical.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       11 2023-03-18 15:35:22.000000 alchemical-0.7.0/src/alchemical.egg-info/top_level.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-18 15:35:22.839176 alchemical-0.7.0/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6605 2022-11-27 14:19:56.000000 alchemical-0.7.0/tests/test_aio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6597 2022-11-27 18:30:43.000000 alchemical-0.7.0/tests/test_alembic.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6843 2022-11-27 14:19:39.000000 alchemical-0.7.0/tests/test_core.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5070 2022-01-22 00:17:41.000000 alchemical-0.7.0/tests/test_flask.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.924647 alchemical-0.7.1/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2021-05-30 15:56:21.000000 alchemical-0.7.1/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       51 2022-11-27 15:05:05.000000 alchemical-0.7.1/MANIFEST.in
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1104 2023-04-24 23:05:08.924923 alchemical-0.7.1/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      538 2021-07-06 22:28:03.000000 alchemical-0.7.1/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-05-30 15:56:36.000000 alchemical-0.7.1/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      766 2023-04-24 23:05:08.926144 alchemical-0.7.1/setup.cfg
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-05-30 15:56:31.000000 alchemical-0.7.1/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.891591 alchemical-0.7.1/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.901366 alchemical-0.7.1/src/alchemical/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       43 2021-08-01 09:16:33.000000 alchemical-0.7.1/src/alchemical/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6655 2023-04-24 22:59:29.000000 alchemical-0.7.1/src/alchemical/aio.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.909826 alchemical-0.7.1/src/alchemical/alembic/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2022-11-26 23:31:47.000000 alchemical-0.7.1/src/alchemical/alembic/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1154 2022-11-27 17:09:09.000000 alchemical-0.7.1/src/alchemical/alembic/cli.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4742 2022-11-27 17:15:39.000000 alchemical-0.7.1/src/alchemical/alembic/env.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.892402 alchemical-0.7.1/src/alchemical/alembic/templates/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.917544 alchemical-0.7.1/src/alchemical/alembic/templates/generic/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       37 2022-11-27 00:06:47.000000 alchemical-0.7.1/src/alchemical/alembic/templates/generic/README
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3478 2022-11-27 12:11:34.000000 alchemical-0.7.1/src/alchemical/alembic/templates/generic/alembic.ini.mako
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      954 2022-11-27 14:17:50.000000 alchemical-0.7.1/src/alchemical/alembic/templates/generic/env.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      965 2022-11-26 23:33:15.000000 alchemical-0.7.1/src/alchemical/alembic/templates/generic/script.py.mako
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    11089 2023-04-24 23:01:00.000000 alchemical-0.7.1/src/alchemical/core.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2726 2021-10-03 15:43:23.000000 alchemical-0.7.1/src/alchemical/flask.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.906883 alchemical-0.7.1/src/alchemical.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1104 2023-04-24 23:05:08.000000 alchemical-0.7.1/src/alchemical.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      769 2023-04-24 23:05:08.000000 alchemical-0.7.1/src/alchemical.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-24 23:05:08.000000 alchemical-0.7.1/src/alchemical.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-05-30 16:00:37.000000 alchemical-0.7.1/src/alchemical.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       19 2023-04-24 23:05:08.000000 alchemical-0.7.1/src/alchemical.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       11 2023-04-24 23:05:08.000000 alchemical-0.7.1/src/alchemical.egg-info/top_level.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-24 23:05:08.923303 alchemical-0.7.1/tests/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6709 2023-04-24 22:56:31.000000 alchemical-0.7.1/tests/test_aio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6597 2022-11-27 18:30:43.000000 alchemical-0.7.1/tests/test_alembic.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6947 2023-04-24 22:56:23.000000 alchemical-0.7.1/tests/test_core.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5070 2022-01-22 00:17:41.000000 alchemical-0.7.1/tests/test_flask.py
```

### Comparing `alchemical-0.7.0/LICENSE` & `alchemical-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/PKG-INFO` & `alchemical-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical
-Version: 0.7.0
+Version: 0.7.1
 Summary: Modern SQLAlchemy simplified
 Home-page: https://github.com/miguelgrinberg/alchemical
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/alchemical/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alchemical-0.7.0/README.md` & `alchemical-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/setup.cfg` & `alchemical-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alchemical
-version = 0.7.0
+version = 0.7.1
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Modern SQLAlchemy simplified
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/alchemical
 project_urls =
```

### Comparing `alchemical-0.7.0/src/alchemical/aio.py` & `alchemical-0.7.1/src/alchemical/aio.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,33 +20,45 @@
     :param url: the database URL.
     :param binds: a dictionary with additional databases to manage with this
                   instance. The keys are the names, and the values are the
                   database URLs. A model is then assigned to a specific bind
                   with the ``__bind_key__`` class attribute.
     :param engine_options: a dictionary with additional engine options to
                            pass to SQLAlchemy.
+    :param session_options: a dictionary with additional session options to
+                            use when creating sessions.
     :param model_class: a custom declarative base to use as parent class for
                         ``db.Model``.
-
-    The database instances can be initialized without arguments, in which case
-    the :func:`Alchemical.initialize` method must be called later to perform
-    the initialization.
+    :param naming_convention: a dictionary with naming conventions to pass to
+                              SQLAlchemy. The naming convention recommended in
+                              the SQLAlchemy documentation is used by default.
+                              Pass an empty dictionary to disable naming
+                              conventions.
+
+    The database instances can be initialized in two phases, in which case the
+    :func:`Alchemical.initialize` method must be called later to complete the
+    initialization. Note that the `model_class` and `naming_convention`
+    arguments can only be passed in this first phase, while the remaining
+    arguments can be passed in either phase.
     """
 
     prefix_map = {
         'sqlite': 'sqlite+aiosqlite',
         'mysql': 'mysql+aiomysql',
         'postgres': 'postgresql+asyncpg',
         'postgresql': 'postgresql+asyncpg'
     }
 
     def __init__(self, url=None, binds=None, engine_options=None,
-                 model_class=None):
+                 session_options=None, model_class=None,
+                 naming_convention=None):
         super().__init__(url=url, binds=binds, engine_options=engine_options,
-                         model_class=model_class)
+                         session_options=session_options,
+                         model_class=model_class,
+                         naming_convention=naming_convention)
         self._sync = None
 
     def _create_engine(self, url, *args, **kwargs):
         return create_async_engine(url, *args, **kwargs)
 
     async def create_all(self):
         """Create the database tables.
@@ -89,17 +101,18 @@
 
             session = db.Session()
 
         When the session is created in this way, ``await session.close()`` must
         be called when the session isn't needed anymore.
         """
         if self.session_class is None:
+            options = {'future': True, 'expire_on_commit': False}
+            options.update(self.session_options)
             self.session_class = async_sessionmaker(
-                bind=self.get_engine(), binds=self.table_binds, future=True,
-                expire_on_commit=False)
+                bind=self.get_engine(), binds=self.table_binds, **options)
         return self.session_class
 
     @asynccontextmanager
     async def begin(self):
         """Context manager for a database transaction.
 
         Upon entering the context manager block, a new session is created and
```

### Comparing `alchemical-0.7.0/src/alchemical/alembic/cli.py` & `alchemical-0.7.1/src/alchemical/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical/alembic/env.py` & `alchemical-0.7.1/src/alchemical/alembic/env.py`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical/alembic/templates/generic/alembic.ini.mako` & `alchemical-0.7.1/src/alchemical/alembic/templates/generic/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical/alembic/templates/generic/env.py` & `alchemical-0.7.1/src/alchemical/alembic/templates/generic/env.py`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical/alembic/templates/generic/script.py.mako` & `alchemical-0.7.1/src/alchemical/alembic/templates/generic/script.py.mako`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical/core.py` & `alchemical-0.7.1/src/alchemical/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,66 +66,79 @@
     :param url: the database URL.
     :param binds: a dictionary with additional databases to manage with this
                   instance. The keys are the names, and the values are the
                   database URLs. A model is then assigned to a specific bind
                   with the ``__bind_key__`` class attribute.
     :param engine_options: a dictionary with additional engine options to
                            pass to SQLAlchemy.
+    :param session_options: a dictionary with additional session options to
+                            use when creating sessions.
     :param model_class: a custom declarative base to use as parent class for
                         ``db.Model``.
     :param naming_convention: a dictionary with naming conventions to pass to
                               SQLAlchemy. The naming convention recommended in
                               the SQLAlchemy documentation is used by default.
                               Pass an empty dictionary to disable naming
                               conventions.
-    The database instances can be initialized without arguments, in which case
-    the :func:`Alchemical.initialize` method must be called later to perform
-    the initialization.
+
+    The database instances can be initialized in two phases, in which case the
+    :func:`Alchemical.initialize` method must be called later to complete the
+    initialization. Note that the `model_class` and `naming_convention`
+    arguments can only be passed in this first phase, while the remaining
+    arguments can be passed in either phase.
     """
 
     prefix_map = {'postgres': 'postgresql'}
 
     def __init__(self, url=None, binds=None, engine_options=None,
-                 model_class=None, naming_convention=None):
-        self.metadatas = {}
+                 session_options=None, model_class=None,
+                 naming_convention=None):
+        self.engine_options = engine_options or {}
+        self.session_options = session_options or {}
         self.naming_convention = DEFAULT_NAMING_CONVENTION \
             if naming_convention is None else naming_convention
-        self._setup_sqlalchemy(model_class)
+
+        self.metadatas = {}
         self.lock = Lock()
         self.url = None
         self.binds = None
-        self.engine_options = {}
         self.session_class = None
         self.engines = None
         self.table_binds = None
+
+        self._setup_sqlalchemy(model_class)
+        self.metadatas[None] = self.Model.metadata
+
         if url or binds:
-            self.initialize(url, binds=binds, engine_options=engine_options)
-        elif engine_options:
-            raise ValueError('"url" and/or "binds" must be set')
+            self.initialize(url, binds=binds)
 
-    def initialize(self, url=None, binds=None, engine_options=None):
+    def initialize(self, url=None, binds=None, engine_options=None,
+                   session_options=None):
         """Initialize the database instance.
 
         :param url: the database URL.
         :param binds: a dictionary with additional databases to manage with
                       this instance. The keys are the names, and the values are
                       the database URLs. A model is then assigned to a specific
                       bind with the `__bind_key__` class attribute.
         :param engine_options: a dictionary with additional engine options to
                                pass to SQLAlchemy.
+        :param session_options: a dictionary with additional session options to
+                                use when creating sessions.
 
-        This method must be used when the instance is created without
-        arguments.
+        This method must be called explicitly to complete the initialization of
+        the instance the two-phase initialization method is used.
         """
         if url is None and binds is None:
             raise ValueError('"url" and/or "binds" must be set')
+
         self.url = url or self.url
         self.binds = binds or self.binds
         self.engine_options = engine_options or self.engine_options
-        self.metadatas[None] = self.Model.metadata
+        self.session_options = session_options or self.session_options
 
     def _setup_sqlalchemy(self, model_class):
         metaclass = type(model_class) if model_class else DeclarativeMeta
 
         class Meta(metaclass):
             def __init__(cls, name, bases, d, **kwargs):
                 bind_key = d.pop('__bind_key__', None)
@@ -243,16 +256,18 @@
 
             session = db.Session()
 
         When the session is created in this way, ``session.close()`` must be
         called when the session isn't needed anymore.
         """
         if self.session_class is None:
+            options = {'future': True}
+            options.update(self.session_options)
             self.session_class = sessionmaker(
-                bind=self.get_engine(), binds=self.table_binds, future=True)
+                bind=self.get_engine(), binds=self.table_binds, **options)
         return self.session_class
 
     @contextmanager
     def begin(self):
         """Context manager for a database transaction.
 
         Upon entering the context manager block, a new session is created and
```

### Comparing `alchemical-0.7.0/src/alchemical/flask.py` & `alchemical-0.7.1/src/alchemical/flask.py`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/src/alchemical.egg-info/PKG-INFO` & `alchemical-0.7.1/src/alchemical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical
-Version: 0.7.0
+Version: 0.7.1
 Summary: Modern SQLAlchemy simplified
 Home-page: https://github.com/miguelgrinberg/alchemical
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/alchemical/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alchemical-0.7.0/src/alchemical.egg-info/SOURCES.txt` & `alchemical-0.7.1/src/alchemical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/tests/test_aio.py` & `alchemical-0.7.1/tests/test_aio.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,13 +178,14 @@
 
         await db.create_all()
         assert db.bind_names() == ['one', 'two']
         assert db.metadata.tables.keys() == {'users', 'user2', 'address'}
         assert db.get_engine() is None
         await db.drop_all()
 
-    def test_bad_init_arguments(self):
-        with pytest.raises(ValueError):
-            Alchemical(engine_options={'foo': 'bar'})
-        with pytest.raises(ValueError):
-            db = Alchemical()
-            db.initialize(engine_options={'foo': 'bar'})
+    def test_two_phase(self):
+        db = Alchemical(engine_options={'foo': 'bar'},
+                        session_options={'bar': 'foo'})
+        db.initialize('sqlite://', engine_options={'foo': 'baz'},
+                      session_options={'baz': 'foo'})
+        assert db.engine_options == {'foo': 'baz'}
+        assert db.session_options == {'baz': 'foo'}
```

### Comparing `alchemical-0.7.0/tests/test_alembic.py` & `alchemical-0.7.1/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `alchemical-0.7.0/tests/test_core.py` & `alchemical-0.7.1/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,20 +165,21 @@
 
         db.create_all()
         assert db.bind_names() == ['one', 'two']
         assert db.metadata.tables.keys() == {'users', 'user2', 'address'}
         assert db.get_engine() is None
         db.drop_all()
 
-    def test_bad_init_arguments(self):
-        with pytest.raises(ValueError):
-            Alchemical(engine_options={'foo': 'bar'})
-        with pytest.raises(ValueError):
-            db = Alchemical()
-            db.initialize(engine_options={'foo': 'bar'})
+    def test_two_phase(self):
+        db = Alchemical(engine_options={'foo': 'bar'},
+                        session_options={'bar': 'foo'})
+        db.initialize('sqlite://', engine_options={'foo': 'baz'},
+                      session_options={'baz': 'foo'})
+        assert db.engine_options == {'foo': 'baz'}
+        assert db.session_options == {'baz': 'foo'}
 
 
 class TestCoreWithCustomBase(TestCore):
     def create_alchemical(self, url=None, binds=None):
         class CustomModel:
             def foo(self):
                 return 42
```

### Comparing `alchemical-0.7.0/tests/test_flask.py` & `alchemical-0.7.1/tests/test_flask.py`

 * *Files identical despite different names*

