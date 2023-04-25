# Comparing `tmp/pymysql-pool-0.3.9.tar.gz` & `tmp/pymysql-pool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysql-pool-0.3.9.tar", last modified: Tue Apr 25 04:18:36 2023, max compression
+gzip compressed data, was "pymysql-pool-0.4.0.tar", last modified: Tue Apr 25 04:37:45 2023, max compression
```

## Comparing `pymysql-pool-0.3.9.tar` & `pymysql-pool-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:18:36.668549 pymysql-pool-0.3.9/
--rw-r--r--   0 kai        (501) staff       (20)    35149 2023-04-25 03:41:34.000000 pymysql-pool-0.3.9/LICENSE
--rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:18:36.668318 pymysql-pool-0.3.9/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)     5620 2023-04-25 03:41:34.000000 pymysql-pool-0.3.9/README.md
-drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:18:36.668008 pymysql-pool-0.3.9/pymysql_pool.egg-info/
--rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/PKG-INFO
--rw-r--r--   0 kai        (501) staff       (20)      220 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/SOURCES.txt
--rw-r--r--   0 kai        (501) staff       (20)        1 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/dependency_links.txt
--rw-r--r--   0 kai        (501) staff       (20)       16 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/requires.txt
--rw-r--r--   0 kai        (501) staff       (20)       12 2023-04-25 04:18:36.000000 pymysql-pool-0.3.9/pymysql_pool.egg-info/top_level.txt
--rw-r--r--   0 kai        (501) staff       (20)    12939 2023-04-25 03:44:49.000000 pymysql-pool-0.3.9/pymysqlpool.py
--rw-r--r--   0 kai        (501) staff       (20)       38 2023-04-25 04:18:36.668640 pymysql-pool-0.3.9/setup.cfg
--rw-r--r--   0 kai        (501) staff       (20)      642 2023-04-25 04:18:04.000000 pymysql-pool-0.3.9/setup.py
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:37:45.257938 pymysql-pool-0.4.0/
+-rw-r--r--   0 kai        (501) staff       (20)    35149 2023-04-25 03:41:34.000000 pymysql-pool-0.4.0/LICENSE
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:37:45.257656 pymysql-pool-0.4.0/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)     5620 2023-04-25 03:41:34.000000 pymysql-pool-0.4.0/README.md
+drwxr-xr-x   0 kai        (501) staff       (20)        0 2023-04-25 04:37:45.257289 pymysql-pool-0.4.0/pymysql_pool.egg-info/
+-rw-r--r--   0 kai        (501) staff       (20)     5989 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/PKG-INFO
+-rw-r--r--   0 kai        (501) staff       (20)      220 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/SOURCES.txt
+-rw-r--r--   0 kai        (501) staff       (20)        1 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/dependency_links.txt
+-rw-r--r--   0 kai        (501) staff       (20)       16 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/requires.txt
+-rw-r--r--   0 kai        (501) staff       (20)       12 2023-04-25 04:37:45.000000 pymysql-pool-0.4.0/pymysql_pool.egg-info/top_level.txt
+-rw-r--r--   0 kai        (501) staff       (20)    12924 2023-04-25 04:33:32.000000 pymysql-pool-0.4.0/pymysqlpool.py
+-rw-r--r--   0 kai        (501) staff       (20)       38 2023-04-25 04:37:45.258031 pymysql-pool-0.4.0/setup.cfg
+-rw-r--r--   0 kai        (501) staff       (20)      642 2023-04-25 04:37:02.000000 pymysql-pool-0.4.0/setup.py
```

### Comparing `pymysql-pool-0.3.9/LICENSE` & `pymysql-pool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.3.9/PKG-INFO` & `pymysql-pool-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.3.9
+Version: 0.4.0
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
 Requires-Python: >=3.6
```

### Comparing `pymysql-pool-0.3.9/README.md` & `pymysql-pool-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymysql-pool-0.3.9/pymysql_pool.egg-info/PKG-INFO` & `pymysql-pool-0.4.0/pymysql_pool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymysql-pool
-Version: 0.3.9
+Version: 0.4.0
 Summary: MySQL connection pool based pymysql
 Home-page: https://github.com/jkklee/pymysql-pool
 Author: ljk
 Author-email: chaoyuemyself@hotmail.com
 License: GPLv3
 Keywords: pymysql pool,mysql connection pool,mysql multi threads
 Requires-Python: >=3.6
```

### Comparing `pymysql-pool-0.3.9/pymysqlpool.py` & `pymysql-pool-0.4.0/pymysqlpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,23 +224,23 @@
             before return a connection, send a ping command to the Mysql server, if the connection is broken, reconnect it
         """
         if retry_num > 10:
             retry_num = 10  # retry_num hard limit
         try:
             conn = self._pool.pop()
         except IndexError:
-            if self.connection_num < self._size:
+            if self.total_num < self._size:
                 return self._create_connection()
             if retry_num > 0:
                 retry_num -= 1
                 time.sleep(retry_interval)
                 logger.debug('Retry to get connection from pool(%s)', self.name)
                 return self.get_connection(retry_num, retry_interval, pre_ping)
             else:
-                if self.connection_num < self.maxsize:
+                if self.total_num < self.maxsize:
                     return self._create_connection()
                 else:
                     raise GetConnectionFromPoolError("can't get connection from pool({}), due to pool lack.".format(self.name))
 
         # check con_lifetime
         if self._con_lifetime > 0 and int(time.time()) - conn._create_ts >= self._con_lifetime:
             conn._pool = None
@@ -270,15 +270,15 @@
                 conn._pool = None
                 try:
                     conn.close()
                 except:
                     conn._force_close()
                 self._created_num.pop()
                 logger.debug("Close connection in pool(%s) due to lifetime reached", self.name)
-                if self.connection_num >= self._size:
+                if self.total_num >= self._size:
                     conn._returned = True
                     return
                 conn = self._create_connection()
             self._pool.appendleft(conn)
             conn._returned = True
             logger.debug("Put connection back to pool(%s)", self.name)
         else:
```

### Comparing `pymysql-pool-0.3.9/setup.py` & `pymysql-pool-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 readme = 'README.md'
 setup(
     name="pymysql-pool",
-    version="0.3.9",
+    version="0.4.0",
     url="https://github.com/jkklee/pymysql-pool",
     author="ljk",
     py_modules=['pymysqlpool'],
     license="GPLv3",
     author_email="chaoyuemyself@hotmail.com",
     description="MySQL connection pool based pymysql",
     long_description=open(readme, encoding='utf-8').read(),
```

