# Comparing `tmp/pymysql-pool-0.4.0.tar.gz` & `tmp/pymysql-pool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysql-pool-0.4.0.tar", last modified: Tue Apr 25 04:37:45 2023, max compression
+gzip compressed data, was "pymysql-pool-0.4.1.tar", last modified: Tue Apr 25 06:34:38 2023, max compression
```

## Comparing `pymysql-pool-0.4.0.tar` & `pymysql-pool-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:37:45.257938 pymysql-pool-0.4.0/
--rw-r--r--   0 kai        (501) staff       (20)    35149 2023-04-25 03:41:34.000000 pymysql-pool-0.4.0/LICENSE
--rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:37:45.257656 pymysql-pool-0.4.0/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)     5620 2023-04-25 03:41:34.000000 pymysql-pool-0.4.0/README.md
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:37:45.257289 pymysql-pool-0.4.0/pymysql_pool.egg-info/
--rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)      220 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/SOURCES.txt
--rw-r--r--   0 kai        (501) staff       (20)        1 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/dependency_links.txt
--rw-r--r--   0 kai        (501) staff       (20)       16 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/requires.txt
--rw-r--r--   0 kai        (501) staff       (20)       12 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/top_level.txt
--rw-r--r--   0 kai        (501) staff       (20)    12924 2023-04-25 04:33:32.000000 pymysql-pool-0.4.0/pymysqlpool.py
--rw-r--r--   0 kai        (501) staff       (20)       38 2023-04-25 04:37:45.258031 pymysql-pool-0.4.0/setup.cfg
--rw-r--r--   0 kai        (501) staff       (20)      642 2023-04-25 04:37:02.000000 pymysql-pool-0.4.0/setup.py
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 06:34:38.228163 pymysql-pool-0.4.1/
+-rw-r--r--   0 kai        (501) staff       (20)    35149 2023-04-25 03:41:34.000000 pymysql-pool-0.4.1/LICENSE
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 06:34:38.227919 pymysql-pool-0.4.1/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)     5620 2023-04-25 03:41:34.000000 pymysql-pool-0.4.1/README.md
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 06:34:38.227438 pymysql-pool-0.4.1/pymysql_pool.egg-info/
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 06:34:38.000000 pymysql-pool-0.4.1/pymysql_pool.egg-info/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)      220 2023-04-25 06:34:38.000000 pymysql-pool-0.4.1/pymysql_pool.egg-info/SOURCES.txt
+-rw-r--r--   0 kai        (501) staff       (20)        1 2023-04-25 06:34:38.000000 pymysql-pool-0.4.1/pymysql_pool.egg-info/dependency_links.txt
+-rw-r--r--   0 kai        (501) staff       (20)       16 2023-04-25 06:34:38.000000 pymysql-pool-0.4.1/pymysql_pool.egg-info/requires.txt
+-rw-r--r--   0 kai        (501) staff       (20)       12 2023-04-25 06:34:38.000000 pymysql-pool-0.4.1/pymysql_pool.egg-info/top_level.txt
+-rw-r--r--   0 kai        (501) staff       (20)    12925 2023-04-25 06:29:03.000000 pymysql-pool-0.4.1/pymysqlpool.py
+-rw-r--r--   0 kai        (501) staff       (20)       38 2023-04-25 06:34:38.228225 pymysql-pool-0.4.1/setup.cfg
+-rw-r--r--   0 kai        (501) staff       (20)      642 2023-04-25 06:32:01.000000 pymysql-pool-0.4.1/setup.py
```

### Comparing `pymysql-pool-0.4.0/LICENSE` & `pymysql-pool-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.4.0/PKG-INFO` & `pymysql-pool-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.4.0
+Version: 0.4.1
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
 Requires-Python: >=3.6
```

### Comparing `pymysql-pool-0.4.0/README.md` & `pymysql-pool-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.4.0/pymysql_pool.egg-info/PKG-INFO` & `pymysql-pool-0.4.1/pymysql_pool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.4.0
+Version: 0.4.1
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
 Requires-Python: >=3.6
```

### Comparing `pymysql-pool-0.4.0/pymysqlpool.py` & `pymysql-pool-0.4.1/pymysqlpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     _pool = None
     _reusable_expection = (pymysql.err.ProgrammingError, pymysql.err.IntegrityError, pymysql.err.NotSupportedError)
 
     def __init__(self, *args, **kwargs):
         pymysql.connections.Connection.__init__(self, *args, **kwargs)
         self.args = args
         self.kwargs = kwargs
-        self.cursorclass = Cursor
+        #self.cursorclass = Cursor
 
     def __exit__(self, exc, value, traceback):
         """
         Overwrite the __exit__() method of pymysql.connections.Connection
 
         Base action: on successful exit, commit. On exception, rollback
         With pool action: put connection back to pool
@@ -238,29 +238,29 @@
             else:
                 if self.total_num < self.maxsize:
                     return self._create_connection()
                 else:
                     raise GetConnectionFromPoolError("can't get connection from pool({}), due to pool lack.".format(self.name))
 
         # check con_lifetime
+        conn._returned = False
         if self._con_lifetime > 0 and int(time.time()) - conn._create_ts >= self._con_lifetime:
             conn._pool = None
             try:
                 conn.close()
             except:
                 conn._force_close()
             self._created_num.pop()
             logger.debug("Close connection in pool(%s) due to lifetime reached", self.name)
             # loss one, create one
             return self._create_connection()
         else:
             if pre_ping:
                 conn.ping(reconnect=True)
 
-        conn._returned = False
         logger.debug('Get connection from pool(%s)', self.name)
         return conn
 
     def _put_connection(self, conn):
         if not hasattr(conn, '_pool') or conn._pool is None:
             return
         conn.cursor().close()
```

### Comparing `pymysql-pool-0.4.0/setup.py` & `pymysql-pool-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 readme = 'README.md'
 setup(
     name="pymysql-pool",
-    version="0.4.0",
+    version="0.4.1",
     url="https://github.com/jkklee/pymysql-pool",
     author="ljk",
     py_modules=['pymysqlpool'],
     license="GPLv3",
     author_email="chaoyuemyself@hotmail.com",
     description="MySQL connection pool based pymysql",
     long_description=open(readme, encoding='utf-8').read(),
```

