# Comparing `tmp/pystorz-0.0.5.tar.gz` & `tmp/pystorz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.0.5.tar", last modified: Mon Apr 24 17:23:27 2023, max compression
+gzip compressed data, was "dist/pystorz-0.0.7.tar", last modified: Mon Apr 24 18:12:55 2023, max compression
```

## Comparing `pystorz-0.0.5.tar` & `pystorz-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.185231 pystorz-0.0.5/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.5/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 17:23:27.185050 pystorz-0.0.5/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.5/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.179028 pystorz-0.0.5/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.5/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.180277 pystorz-0.0.5/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.5/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.5/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.181551 pystorz-0.0.5/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.5/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.5/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4159 2023-04-24 14:46:41.000000 pystorz-0.0.5/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.183219 pystorz-0.0.5/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.5/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.5/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.5/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.183505 pystorz-0.0.5/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.5/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9384 2023-04-24 16:11:55.000000 pystorz-0.0.5/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.184540 pystorz-0.0.5/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.5/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.5/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.5/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2073 2023-04-24 15:41:15.000000 pystorz-0.0.5/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.179859 pystorz-0.0.5/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-24 17:23:27.185280 pystorz-0.0.5/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-24 17:23:01.000000 pystorz-0.0.5/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.989273 pystorz-0.0.7/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.7/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 18:12:55.989030 pystorz-0.0.7/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.7/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.977862 pystorz-0.0.7/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.7/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.978946 pystorz-0.0.7/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.7/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.7/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.981140 pystorz-0.0.7/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.7/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.7/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4159 2023-04-24 14:46:41.000000 pystorz-0.0.7/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.986550 pystorz-0.0.7/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.7/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.7/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.7/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.987101 pystorz-0.0.7/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.7/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9558 2023-04-24 18:11:22.000000 pystorz-0.0.7/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.988532 pystorz-0.0.7/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.7/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.7/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.7/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2073 2023-04-24 15:41:15.000000 pystorz-0.0.7/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.978671 pystorz-0.0.7/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-24 18:12:55.989332 pystorz-0.0.7/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-24 18:11:55.000000 pystorz-0.0.7/setup.py
```

### Comparing `pystorz-0.0.5/LICENSE` & `pystorz-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/PKG-INFO` & `pystorz-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.5
+Version: 0.0.7
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.5/README.md` & `pystorz-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/builder.py` & `pystorz-0.0.7/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/loader.py` & `pystorz-0.0.7/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/templates/structure.py` & `pystorz-0.0.7/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.0.7/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/test.py` & `pystorz-0.0.7/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/mgen/utils.py` & `pystorz-0.0.7/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/sql/store.py` & `pystorz-0.0.7/pystorz/sql/store.py`

 * *Files 17% similar despite different names*

```diff
@@ -208,14 +208,15 @@
             Type VARCHAR(25) NOT NULL,
             Object JSON,
             PRIMARY KEY (Pkey,Type));
         '''
 
         cursor.execute(create)
         cursor.close()
+        self.DB.commit()
 
     def _getIdentity(self, path):
         query = """SELECT Pkey, Type FROM IdIndex 
         WHERE Path='{}'""".format(path)
         cursor = self._do_query(query)
         result = cursor.fetchone()
 
@@ -237,22 +238,24 @@
         if existing_pkey is not None and existing_typ is not None:
             query = """UPDATE IdIndex SET Pkey='{}', Type='{}'
             WHERE Path='{}'""".format(pkey, typ.lower(), path)
         else:
             query = """INSERT INTO IdIndex (Pkey, Type, Path)
             VALUES ('{}', '{}', '{}')""".format(pkey, typ.lower(), path)
 
-        self._do_query(query)
-        # cursor.commit()
+        cursor = self._do_query(query)
+        cursor.close()
+        self.DB.commit()
 
     def _removeIdentity(self, path):
         query = """DELETE FROM IdIndex
         WHERE Path = '{}'""".format(path)
-        self._do_query(query)
-        # cursor.commit()
+        cursor = self._do_query(query)
+        cursor.close()
+        self.DB.commit()
 
     def _getObject(self, pkey, typ):
         query = """SELECT Object FROM Objects
         WHERE Pkey='{}' AND Type='{}'""".format(
             pkey, typ.lower())
         cursor = self._do_query(query)
         result = cursor.fetchone()
@@ -277,23 +280,26 @@
         if existing_obj is not None:
             query = """UPDATE Objects SET Object='{}'
             WHERE Pkey = '{}' AND Type = '{}'""".format(data, pkey, typ.lower())
         else:
             query = """INSERT INTO Objects (Object, Pkey, Type)
             VALUES ('{}', '{}', '{}')""".format(data, pkey, typ.lower())
 
-        self._do_query(query)
-        # cursor.commit()
+        cursor = self._do_query(query)
+        cursor.close()
+        self.DB.commit()
+        self.DB.commit()
 
     def _removeObject(self, pkey, typ):
         query = """DELETE FROM Objects
         WHERE Pkey = '{}' AND Type = '{}'""".format(pkey, typ.lower())
 
-        self._do_query(query)
-        # cursor.commit()
+        cursor = self._do_query(query)
+        cursor.close()
+        self.DB.commit()
 
     def _parseObjectRow(self, data, typ):
         return utils.unmarshal_object(data, self.Schema, typ)
 
     def _parseObjectRows(self, rows, typ):
         res = []
         for row in rows:
```

### Comparing `pystorz-0.0.5/pystorz/store/meta.py` & `pystorz-0.0.7/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/store/options.py` & `pystorz-0.0.7/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/store/store.py` & `pystorz-0.0.7/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz/store/utils.py` & `pystorz-0.0.7/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/pystorz.egg-info/PKG-INFO` & `pystorz-0.0.7/pystorz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.5
+Version: 0.0.7
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.5/pystorz.egg-info/SOURCES.txt` & `pystorz-0.0.7/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.5/setup.py` & `pystorz-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.0.5',
+    version='0.0.7',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

