# Comparing `tmp/pymysql-pool-0.3.7.tar.gz` & `tmp/pymysql-pool-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kai/github/pymysql-pool/dist/tmp9bjsoxrz/pymysql-pool-0.3.7.tar", last modified: Tue Mar  8 09:03:36 2022, max compression
+gzip compressed data, was "pymysql-pool-0.3.9.tar", last modified: Tue Apr 25 04:18:36 2023, max compression
```

## Comparing `pymysql-pool-0.3.7.tar` & `pymysql-pool-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/
--rw-r--r--   0 kai        (501) staff       (20)    35149 2022-02-09 08:00:58.000000 pymysql-pool-0.3.7/LICENSE
--rw-r--r--   0 kai        (501) staff       (20)     6009 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)     5620 2022-03-08 08:51:54.000000 pymysql-pool-0.3.7/README.md
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/
--rw-r--r--   0 kai        (501) staff       (20)     6009 2022-03-08 09:03:35.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)      220 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/SOURCES.txt
--rw-r--r--   0 kai        (501) staff       (20)        1 2022-03-08 09:03:35.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/dependency_links.txt
--rw-r--r--   0 kai        (501) staff       (20)       16 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/requires.txt
--rw-r--r--   0 kai        (501) staff       (20)       12 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/pymysql_pool.egg-info/top_level.txt
--rw-r--r--   0 kai        (501) staff       (20)    10926 2022-03-08 08:52:41.000000 pymysql-pool-0.3.7/pymysqlpool.py
--rw-r--r--   0 kai        (501) staff       (20)       38 2022-03-08 09:03:36.000000 pymysql-pool-0.3.7/setup.cfg
--rw-r--r--   0 kai        (501) staff       (20)      642 2022-03-07 02:26:37.000000 pymysql-pool-0.3.7/setup.py
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:18:36.668549 pymysql-pool-0.3.9/
+-rw-r--r--   0 kai        (501) staff       (20)    35149 2023-04-25 03:41:34.000000 pymysql-pool-0.3.9/LICENSE
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:18:36.668318 pymysql-pool-0.3.9/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)     5620 2023-04-25 03:41:34.000000 pymysql-pool-0.3.9/README.md
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:18:36.668008 pymysql-pool-0.3.9/pymysql_pool.egg-info/
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)      220 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/SOURCES.txt
+-rw-r--r--   0 kai        (501) staff       (20)        1 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/dependency_links.txt
+-rw-r--r--   0 kai        (501) staff       (20)       16 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/requires.txt
+-rw-r--r--   0 kai        (501) staff       (20)       12 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/top_level.txt
+-rw-r--r--   0 kai        (501) staff       (20)    12939 2023-04-25 03:44:49.000000 pymysql-pool-0.3.9/pymysqlpool.py
+-rw-r--r--   0 kai        (501) staff       (20)       38 2023-04-25 04:18:36.668640 pymysql-pool-0.3.9/setup.cfg
+-rw-r--r--   0 kai        (501) staff       (20)      642 2023-04-25 04:18:04.000000 pymysql-pool-0.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pymysql-pool-0.3.7/LICENSE` & `pymysql-pool-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.3.7/PKG-INFO` & `pymysql-pool-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.3.7
+Version: 0.3.9
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMySQL Connection Pool
 A simple but not simple mysql connection pool based on `PyMySQL`.
 
@@ -111,9 +110,7 @@
     2  # as we expect
 We can see that the module maintains the pool appropriately when (and only when) we call the close() method or use the Context Manager Protocol of the connection object.
 
 ## Note
 1. We should always use either the close() method or Context Manager Protocol of the connection object. Otherwise the pool will exhaust soon.
 
 2. The `Context Manager Protocol` is preferred. It can achieve an effect similar to the "multiplexing", means the more Fine-Grained use of pool, also do more with less connections.
-
-
```

### Comparing `pymysql-pool-0.3.7/README.md` & `pymysql-pool-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.3.7/pymysql_pool.egg-info/PKG-INFO` & `pymysql-pool-0.3.9/pymysql_pool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.3.7
+Version: 0.3.9
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMySQL Connection Pool
 A simple but not simple mysql connection pool based on `PyMySQL`.
 
@@ -111,9 +110,7 @@
     2  # as we expect
 We can see that the module maintains the pool appropriately when (and only when) we call the close() method or use the Context Manager Protocol of the connection object.
 
 ## Note
 1. We should always use either the close() method or Context Manager Protocol of the connection object. Otherwise the pool will exhaust soon.
 
 2. The `Context Manager Protocol` is preferred. It can achieve an effect similar to the "multiplexing", means the more Fine-Grained use of pool, also do more with less connections.
-
-
```

### Comparing `pymysql-pool-0.3.7/pymysqlpool.py` & `pymysql-pool-0.3.9/pymysqlpool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 """
 author: ljk
 email: chaoyuemyself@hotmail.com
 """
 import pymysql
 import warnings
 import logging
+import functools
+import inspect
 import time
 from collections import deque
 
 __all__ = ['Connection', 'ConnectionPool', 'logger']
 
 warnings.filterwarnings('error', category=pymysql.err.Warning)
+
 # use logging module for easy debug
-logging.basicConfig(format='%(asctime)s %(levelname)8s: %(message)s', datefmt='%m-%d %H:%M:%S')
-logger = logging.getLogger(__name__)
-logger.setLevel('WARNING')
+
+
+def _init_logger(level='WARNING'):
+    logger = logging.getLogger(__name__)
+    handler = logging.StreamHandler()
+    handler.setFormatter(logging.Formatter(fmt='%(asctime)s %(levelname)8s: %(message)s', datefmt='%m-%d %H:%M:%S'))
+    logger.addHandler(handler)
+    logger.setLevel(level)
+    return logger
+
+
+logger = _init_logger()
 
 
 class Connection(pymysql.connections.Connection):
     """
     Return a connection object with or without connection_pool feature.
+
     This is all the same with pymysql.connections.Connection instance except that with connection_pool feature:
         the __exit__() method additionally put the connection back to it's pool
     """
     _pool = None
     _reusable_expection = (pymysql.err.ProgrammingError, pymysql.err.IntegrityError, pymysql.err.NotSupportedError)
 
     def __init__(self, *args, **kwargs):
         pymysql.connections.Connection.__init__(self, *args, **kwargs)
         self.args = args
         self.kwargs = kwargs
+        self.cursorclass = Cursor
 
     def __exit__(self, exc, value, traceback):
         """
         Overwrite the __exit__() method of pymysql.connections.Connection
+
         Base action: on successful exit, commit. On exception, rollback
-        With pool additional action: put connection back to pool
+        With pool action: put connection back to pool
         """
         if self._pool is not None:
             if not exc or exc in self._reusable_expection:
                 '''reusable connection'''
                 self._pool._put_connection(self)
             else:
                 '''no reusable connection, close it and create a new one put to the pool'''
@@ -51,26 +66,28 @@
                     self._force_close()
         else:
             pymysql.connections.Connection.__exit__(self, exc, value, traceback)
 
     def close(self):
         """
         Overwrite the close() method of pymysql.connections.Connection
+
         With pool, put connection back to pool;
         Without pool, send the quit message and close the socket
         """
         if self._pool is not None:
             self._pool._put_connection(self)
         else:
             pymysql.connections.Connection.close(self)
 
     def ping(self, reconnect=True):
         """
         Overwrite the ping() method of pymysql.connections.Connection
         Check if the server is alive.
+
         :param reconnect: If the connection is closed, reconnect.
         :type reconnect: boolean
         :raise Error: If the connection is closed and reconnect=False.
         """
         if self._sock is None:
             if reconnect:
                 self.connect()
@@ -89,15 +106,17 @@
                 self.connect()
                 self.ping(False)
             else:
                 raise
 
     def execute_query(self, query, args=(), dictcursor=False, return_one=False, exec_many=False):
         """
+        Deprecated and will remove in the future: please use more friendly Cursor.db_query() and Cursor.db_modify().
         A wrapped method of pymysql's execute() or executemany().
+
         dictcursor: whether want use the dict cursor(cursor's default type is tuple)
         return_one: whether want only one row of the result
         exec_many: whether use pymysql's executemany() method
         """
         with self:
             cur = self.cursor() if not dictcursor else self.cursor(pymysql.cursors.DictCursor)
             try:
@@ -107,14 +126,47 @@
                     cur.execute(query, args)
             except Exception:
                 raise
             # if no record match the query, return () if return_one==False, else return None
             return cur.fetchone() if return_one else cur.fetchall()
 
 
+class Cursor(pymysql.cursors.Cursor):
+    def db_query(self, query, args=()):
+        """
+        A wrapped method of Cursor..fetchone() or Cursor..fetchall() when doing select query.
+        The outer layer of return data is always list(always use cursor.fetchall()), to display data with a unified structure.
+        """
+        # with self:
+        try:
+            # cur = self.cursor(cursorclass) if cursorclass else self.cursor()
+            self.execute(query, args)
+            return self.fetchall()
+        except Exception:
+            raise
+
+    def db_modify(self, query, args=(), exec_many=False):
+        """
+        A wrapped method of Cursor.execute() or Cursor.executemany() when doing modify query.
+        return: {'rowcount': xxx, 'lastrowid': xxx}
+
+        exec_many: whether use executemany() method
+        """
+        # with self:
+        try:
+            # cur = self.cursor()
+            if not exec_many:
+                rt = self.execute(query, args)
+            else:
+                rt = self.executemany(query, args)
+            return {'rowcount': self.rowcount, 'lastrowid': self.lastrowid}
+        except Exception:
+            raise
+
+
 class ConnectionPool:
     """
     Return connection_pool object, which has method can get connection from a pool with timeout and retry feature;
     put a reusable connection back to the pool, etc; also we can create different instance of this class that represent
     different pool of different DB Server or different user
     """
 
@@ -160,18 +212,18 @@
                 conn._returned = True
         else:
             self._args = args
             self._kwargs = kwargs
 
     def get_connection(self, retry_num=3, retry_interval=0.1, pre_ping=False):
         """
-        timeout: int
-            timeout of get a connection from pool, should be a int(0 means return or raise immediately)
         retry_num: int
             how many times will retry to get a connection
+        retry_interval: float
+            timeout of get a connection from pool(0 means return or raise immediately)
         pre_ping: bool
             before return a connection, send a ping command to the Mysql server, if the connection is broken, reconnect it
         """
         if retry_num > 10:
             retry_num = 10  # retry_num hard limit
         try:
             conn = self._pool.pop()
@@ -183,16 +235,15 @@
                 time.sleep(retry_interval)
                 logger.debug('Retry to get connection from pool(%s)', self.name)
                 return self.get_connection(retry_num, retry_interval, pre_ping)
             else:
                 if self.connection_num < self.maxsize:
                     return self._create_connection()
                 else:
-                    raise GetConnectionFromPoolError("can't get connection from pool({}), retry_interval={}(s)".format(
-                        self.name, retry_num, retry_interval))
+                    raise GetConnectionFromPoolError("can't get connection from pool({}), due to pool lack.".format(self.name))
 
         # check con_lifetime
         if self._con_lifetime > 0 and int(time.time()) - conn._create_ts >= self._con_lifetime:
             conn._pool = None
             try:
                 conn.close()
             except:
@@ -241,23 +292,38 @@
         # add attr indicate whether the connection has already return to pool, should not use any more
         conn._returned = False
         self._created_num.append(1)
         logger.debug('Create new connection in pool(%s)', self.name)
         return conn
 
     @property
-    def size(self):
+    def available_num(self):
         """available connections number for now"""
         return len(self._pool)
 
     @property
-    def connection_num(self):
+    def total_num(self):
         """total connections number of all used and available"""
         return len(self._created_num)
 
 
 class GetConnectionFromPoolError(Exception):
     """Exception related can't get connection from pool within timeout seconds."""
 
 
 class ReturnConnectionToPoolError(Exception):
     """Exception related can't return connection to pool."""
+
+
+def already_returned_conn(f):
+    @functools.wraps(f)
+    def wrapper(*args, **kwargs):
+        # args[0] means self(connection object)
+        if hasattr(args[0], '_returned') and args[0]._returned:
+            raise ReturnConnectionToPoolError("this connection has already returned to the pool({})".format(args[0]._pool.name))
+        return f(*args, **kwargs)
+    return wrapper
+
+
+for name, fn in inspect.getmembers(Connection, inspect.isfunction):
+    if not name.startswith('_'):
+        setattr(Connection, name, already_returned_conn(fn))
```

### Comparing `pymysql-pool-0.3.7/setup.py` & `pymysql-pool-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 readme = 'README.md'
 setup(
     name="pymysql-pool",
-    version="0.3.7",
+    version="0.3.9",
     url="https://github.com/jkklee/pymysql-pool",
     author="ljk",
     py_modules=['pymysqlpool'],
     license="GPLv3",
     author_email="chaoyuemyself@hotmail.com",
     description="MySQL connection pool based pymysql",
     long_description=open(readme, encoding='utf-8').read(),
```

