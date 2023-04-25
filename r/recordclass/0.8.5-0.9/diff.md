# Comparing `tmp/recordclass-0.8.5.tar.gz` & `tmp/recordclass-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recordclass-0.8.5.tar", last modified: Tue Jan 22 10:56:25 2019, max compression
+gzip compressed data, was "dist/recordclass-0.9.tar", last modified: Thu Jan 24 10:48:26 2019, max compression
```

## Comparing `recordclass-0.8.5.tar` & `recordclass-0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/
--rw-r--r--   0 intellimath   (501) staff       (20)     1116 2019-01-22 10:49:04.000000 recordclass-0.8.5/LICENSE.txt
--rw-r--r--   0 intellimath   (501) staff       (20)      299 2019-01-11 07:46:00.000000 recordclass-0.8.5/MANIFEST.in
--rw-r--r--   0 intellimath   (501) staff       (20)    13846 2019-01-22 10:56:25.000000 recordclass-0.8.5/PKG-INFO
--rw-r--r--   0 intellimath   (501) staff       (20)    10558 2019-01-21 18:13:04.000000 recordclass-0.8.5/README.md
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/recordclass/
--rw-r--r--   0 intellimath   (501) staff       (20)     1520 2019-01-15 13:18:46.000000 recordclass-0.8.5/lib/recordclass/__init__.py
--rw-r--r--   0 intellimath   (501) staff       (20)     1634 2019-01-19 10:24:44.000000 recordclass-0.8.5/lib/recordclass/arrayclass.py
--rw-r--r--   0 intellimath   (501) staff       (20)   667940 2019-01-22 10:47:32.000000 recordclass-0.8.5/lib/recordclass/dataobject.c
--rw-r--r--   0 intellimath   (501) staff       (20)     2604 2019-01-22 10:47:32.000000 recordclass-0.8.5/lib/recordclass/dataobject.h
--rw-r--r--   0 intellimath   (501) staff       (20)    32976 2018-12-18 17:11:47.000000 recordclass-0.8.5/lib/recordclass/memoryslots.c
--rw-r--r--   0 intellimath   (501) staff       (20)     8417 2019-01-19 20:10:12.000000 recordclass-0.8.5/lib/recordclass/recordclass.py
--rw-r--r--   0 intellimath   (501) staff       (20)     7641 2019-01-21 19:22:30.000000 recordclass-0.8.5/lib/recordclass/structclass.py
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/recordclass/test/
--rw-r--r--   0 intellimath   (501) staff       (20)      454 2019-01-15 13:21:19.000000 recordclass-0.8.5/lib/recordclass/test/__init__.py
--rw-r--r--   0 intellimath   (501) staff       (20)     2686 2019-01-19 19:45:17.000000 recordclass-0.8.5/lib/recordclass/test/test_arrayclass.py
--rw-r--r--   0 intellimath   (501) staff       (20)     3900 2019-01-15 13:19:46.000000 recordclass-0.8.5/lib/recordclass/test/test_memoryslots.py
--rw-r--r--   0 intellimath   (501) staff       (20)    13680 2019-01-19 18:29:27.000000 recordclass-0.8.5/lib/recordclass/test/test_recordclass.py
--rw-r--r--   0 intellimath   (501) staff       (20)    15342 2019-01-21 18:21:03.000000 recordclass-0.8.5/lib/recordclass/test/test_structclass.py
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/recordclass/test/typing/
--rw-r--r--   0 intellimath   (501) staff       (20)      193 2018-12-27 12:06:09.000000 recordclass-0.8.5/lib/recordclass/test/typing/__init__.py
--rw-r--r--   0 intellimath   (501) staff       (20)     5933 2019-01-19 20:28:04.000000 recordclass-0.8.5/lib/recordclass/test/typing/test_recordclass.py
--rw-r--r--   0 intellimath   (501) staff       (20)     5605 2019-01-19 20:28:13.000000 recordclass-0.8.5/lib/recordclass/test/typing/test_structclass.py
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/recordclass/typing/
--rw-r--r--   0 intellimath   (501) staff       (20)     5647 2019-01-19 20:25:10.000000 recordclass-0.8.5/lib/recordclass/typing/__init__.py
-drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-22 10:56:25.000000 recordclass-0.8.5/lib/recordclass.egg-info/
--rw-r--r--   0 intellimath   (501) staff       (20)    13846 2019-01-22 10:56:23.000000 recordclass-0.8.5/lib/recordclass.egg-info/PKG-INFO
--rw-r--r--   0 intellimath   (501) staff       (20)      805 2019-01-22 10:56:23.000000 recordclass-0.8.5/lib/recordclass.egg-info/SOURCES.txt
--rw-r--r--   0 intellimath   (501) staff       (20)        1 2019-01-22 10:56:23.000000 recordclass-0.8.5/lib/recordclass.egg-info/dependency_links.txt
--rw-r--r--   0 intellimath   (501) staff       (20)       12 2019-01-22 10:56:23.000000 recordclass-0.8.5/lib/recordclass.egg-info/top_level.txt
--rw-r--r--   0 intellimath   (501) staff       (20)       38 2019-01-22 10:56:25.000000 recordclass-0.8.5/setup.cfg
--rw-r--r--   0 intellimath   (501) staff       (20)     3695 2019-01-22 10:56:05.000000 recordclass-0.8.5/setup.py
--rw-r--r--   0 intellimath   (501) staff       (20)     1220 2018-11-13 19:29:12.000000 recordclass-0.8.5/test_all.py
--rw-r--r--   0 intellimath   (501) staff       (20)     3988 2019-01-02 14:09:40.000000 recordclass-0.8.5/test_performance.py
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:26.000000 recordclass-0.9/
+-rw-r--r--   0 intellimath   (501) staff       (20)     1116 2019-01-22 10:49:04.000000 recordclass-0.9/LICENSE.txt
+-rw-r--r--   0 intellimath   (501) staff       (20)      299 2019-01-11 07:46:00.000000 recordclass-0.9/MANIFEST.in
+-rw-r--r--   0 intellimath   (501) staff       (20)    13965 2019-01-24 10:48:26.000000 recordclass-0.9/PKG-INFO
+-rw-r--r--   0 intellimath   (501) staff       (20)    10639 2019-01-24 10:37:14.000000 recordclass-0.9/README.md
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/recordclass/
+-rw-r--r--   0 intellimath   (501) staff       (20)     1518 2019-01-24 10:33:35.000000 recordclass-0.9/lib/recordclass/__init__.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     1634 2019-01-19 10:24:44.000000 recordclass-0.9/lib/recordclass/arrayclass.py
+-rw-r--r--   0 intellimath   (501) staff       (20)   664759 2019-01-24 10:46:32.000000 recordclass-0.9/lib/recordclass/dataobject.c
+-rw-r--r--   0 intellimath   (501) staff       (20)     2604 2019-01-24 10:46:32.000000 recordclass-0.9/lib/recordclass/dataobject.h
+-rw-r--r--   0 intellimath   (501) staff       (20)    32974 2019-01-24 08:11:05.000000 recordclass-0.9/lib/recordclass/memoryslots.c
+-rw-r--r--   0 intellimath   (501) staff       (20)     8417 2019-01-19 20:10:12.000000 recordclass-0.9/lib/recordclass/recordclass.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     7641 2019-01-21 19:22:30.000000 recordclass-0.9/lib/recordclass/structclass.py
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/recordclass/test/
+-rw-r--r--   0 intellimath   (501) staff       (20)      454 2019-01-15 13:21:19.000000 recordclass-0.9/lib/recordclass/test/__init__.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     2686 2019-01-19 19:45:17.000000 recordclass-0.9/lib/recordclass/test/test_arrayclass.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     3900 2019-01-15 13:19:46.000000 recordclass-0.9/lib/recordclass/test/test_memoryslots.py
+-rw-r--r--   0 intellimath   (501) staff       (20)    13680 2019-01-19 18:29:27.000000 recordclass-0.9/lib/recordclass/test/test_recordclass.py
+-rw-r--r--   0 intellimath   (501) staff       (20)    15342 2019-01-21 18:21:03.000000 recordclass-0.9/lib/recordclass/test/test_structclass.py
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/recordclass/test/typing/
+-rw-r--r--   0 intellimath   (501) staff       (20)      193 2018-12-27 12:06:09.000000 recordclass-0.9/lib/recordclass/test/typing/__init__.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     5933 2019-01-19 20:28:04.000000 recordclass-0.9/lib/recordclass/test/typing/test_recordclass.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     5605 2019-01-19 20:28:13.000000 recordclass-0.9/lib/recordclass/test/typing/test_structclass.py
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/recordclass/typing/
+-rw-r--r--   0 intellimath   (501) staff       (20)     5647 2019-01-19 20:25:10.000000 recordclass-0.9/lib/recordclass/typing/__init__.py
+drwxr-xr-x   0 intellimath   (501) staff       (20)        0 2019-01-24 10:48:25.000000 recordclass-0.9/lib/recordclass.egg-info/
+-rw-r--r--   0 intellimath   (501) staff       (20)    13965 2019-01-24 10:48:23.000000 recordclass-0.9/lib/recordclass.egg-info/PKG-INFO
+-rw-r--r--   0 intellimath   (501) staff       (20)      805 2019-01-24 10:48:23.000000 recordclass-0.9/lib/recordclass.egg-info/SOURCES.txt
+-rw-r--r--   0 intellimath   (501) staff       (20)        1 2019-01-24 10:48:23.000000 recordclass-0.9/lib/recordclass.egg-info/dependency_links.txt
+-rw-r--r--   0 intellimath   (501) staff       (20)       12 2019-01-24 10:48:23.000000 recordclass-0.9/lib/recordclass.egg-info/top_level.txt
+-rw-r--r--   0 intellimath   (501) staff       (20)       38 2019-01-24 10:48:26.000000 recordclass-0.9/setup.cfg
+-rw-r--r--   0 intellimath   (501) staff       (20)     3693 2019-01-24 10:48:07.000000 recordclass-0.9/setup.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     1220 2018-11-13 19:29:12.000000 recordclass-0.9/test_all.py
+-rw-r--r--   0 intellimath   (501) staff       (20)     3972 2019-01-24 10:20:18.000000 recordclass-0.9/test_performance.py
```

### Comparing `recordclass-0.8.5/LICENSE.txt` & `recordclass-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/PKG-INFO` & `recordclass-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recordclass
-Version: 0.8.5
+Version: 0.9
 Summary: Mutable variants of tuple (memoryslots) and collections.namedtuple (recordclass), which support assignments and more memory saving variants (arrayclass and structclass)
 Home-page: http://intellimath.bitbucket.org/recordclass
 Author: Zaur Shibzukhov
 Author-email: szport@gmail.com
 License: MIT License
 Download-URL: https://bitbucket.org/intellimath/recordclass
 Description: # Recordclass library
@@ -39,27 +39,27 @@
         
         ## Quick start:
         
         First load inventory:
         
             >>> from recordclass import recordclass, RecordClass
         
-        Simple example with `recordclass`:
+        Example with `recordclass`:
         
             >>> Point = recordclass('Point', 'x y')
             >>> p = Point(1,2)
             >>> print(p)
             Point(1, 2)
             >>> print(p.x, p.y)
             1 2
             >>> p.x, p.y = 10, 20
             >>> print(p)
             Point(10, 20)
             
-        Simple example with `RecordClass` and typehints::
+        Example with `RecordClass` and typehints::
         
             class Point(RecordClass):
                x: int
                y: int
         
             >>> ptint(Point.__annotations__)
             {'x': <class 'int'>, 'y': <class 'int'>}
@@ -180,15 +180,20 @@
         |   `new`   |    739±24 ns  |     915±35 ns    |   763±21 ns   |    889±34 ns  |
         | `getattr` |   84.0±1.7 ns |    42.8±1.5 ns   |   39.5±1.0 ns |   41.7±1.1 ns |
         | `setattr` |               |     50.5±1.7 ns  |   50.9±1.5 ns |   48.8±1.0 ns |
         
         
         ### Changes:
         
-        ### 0.8.5
+        #### 0.9
+        
+        * Change version to 0.9 to indicate a step forward.
+        * Cleanup dataobject.__cinit__
+        
+        #### 0.8.5
         
         * Make `arrayclass`-based objects support setitem/getitem and `structclass`-based objects able 
           to not support them. By default, as before `structclass`-based objects support setitem/getitem protocol.
         * Now only instances of `dataobject` are comparable to 'arrayclass'-based and `structclass`-based instances.
         * Now generated classes can be hashable.
```

### Comparing `recordclass-0.8.5/README.md` & `recordclass-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 
 ## Quick start:
 
 First load inventory:
 
     >>> from recordclass import recordclass, RecordClass
 
-Simple example with `recordclass`:
+Example with `recordclass`:
 
     >>> Point = recordclass('Point', 'x y')
     >>> p = Point(1,2)
     >>> print(p)
     Point(1, 2)
     >>> print(p.x, p.y)
     1 2
     >>> p.x, p.y = 10, 20
     >>> print(p)
     Point(10, 20)
     
-Simple example with `RecordClass` and typehints::
+Example with `RecordClass` and typehints::
 
     class Point(RecordClass):
        x: int
        y: int
 
     >>> ptint(Point.__annotations__)
     {'x': <class 'int'>, 'y': <class 'int'>}
@@ -171,15 +171,20 @@
 |   `new`   |    739±24 ns  |     915±35 ns    |   763±21 ns   |    889±34 ns  |
 | `getattr` |   84.0±1.7 ns |    42.8±1.5 ns   |   39.5±1.0 ns |   41.7±1.1 ns |
 | `setattr` |               |     50.5±1.7 ns  |   50.9±1.5 ns |   48.8±1.0 ns |
 
 
 ### Changes:
 
-### 0.8.5
+#### 0.9
+
+* Change version to 0.9 to indicate a step forward.
+* Cleanup dataobject.__cinit__
+
+#### 0.8.5
 
 * Make `arrayclass`-based objects support setitem/getitem and `structclass`-based objects able 
   to not support them. By default, as before `structclass`-based objects support setitem/getitem protocol.
 * Now only instances of `dataobject` are comparable to 'arrayclass'-based and `structclass`-based instances.
 * Now generated classes can be hashable.
```

### Comparing `recordclass-0.8.5/lib/recordclass/__init__.py` & `recordclass-0.9/lib/recordclass/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 from .dataobject import sequenceproxy, dataobject
 from .recordclass import recordclass
 from .structclass import structclass, join_classes
 from .arrayclass import arrayclass
 if _PY36:
     from .typing import RecordClass, StructClass
 
-__version__ = '0.8.5'
+__version__ = '0.9'
```

### Comparing `recordclass-0.8.5/lib/recordclass/arrayclass.py` & `recordclass-0.9/lib/recordclass/arrayclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/dataobject.c` & `recordclass-0.9/lib/recordclass/dataobject.c`

 * *Files 1% similar despite different names*

```diff
@@ -610,16 +610,18 @@
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 
     #define C_DIV(a,b) ((a)/(b))
 
     #define dataobject_items(op) ((PyObject**)((char*)(op) + sizeof(PyObject)))
-    #define dataobject_dictptr(op, tp) ((PyObject**)((char*)op + tp->tp_dictoffset))
-    #define dataobject_weaklistptr(op, tp) ((PyObject**)((char*)op + tp->tp_weaklistoffset))    
+    #define dataobject_dictptr(op, tp) ((PyObject**)((char*)(op) + tp->tp_dictoffset))
+    #define dataobject_weaklistptr(op, tp) ((PyObject**)((char*)op + tp->tp_weaklistoffset))
+    #define dataobject_hasdict(op) ((Py_TYPE((PyObject*)(op)))->tp_dictoffset != 0)
+    #define dataobject_hasweaklist(op) ((Py_TYPE((PyObject*)(op)))->tp_weaklistoffset != 0)
     
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -836,55 +838,55 @@
 struct DataObjectGet;
 struct SequenceProxyObject;
 struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic;
 struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct_1_genexpr;
 struct __pyx_opt_args_11recordclass_10dataobject__type_configure_basic;
 struct __pyx_opt_args_11recordclass_10dataobject__type_configure_getsetitem;
 
-/* "recordclass/dataobject.pyx":624
+/* "recordclass/dataobject.pyx":612
  *         return ob
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,             # <<<<<<<<<<<<<<
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  */
 struct __pyx_opt_args_11recordclass_10dataobject__type_configure_basic {
   int __pyx_n;
   PyObject *usedict;
   PyObject *gc;
   PyObject *weakref;
   PyObject *hashable;
 };
 
-/* "recordclass/dataobject.pyx":668
+/* "recordclass/dataobject.pyx":656
  *     tp.tp_init = NULL
  * 
  * cdef _type_configure_getsetitem "_type_configure_getsetitem"(ob, readonly=False):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  * 
  */
 struct __pyx_opt_args_11recordclass_10dataobject__type_configure_getsetitem {
   int __pyx_n;
   PyObject *readonly;
 };
 
-/* "recordclass/dataobject.pyx":447
+/* "recordclass/dataobject.pyx":437
  * 
  * @cython.auto_pickle(False)
  * cdef public class dataobject[object DataObject, type DataObjectType]:             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, *args, **kw):
  */
 struct DataObject {
   PyObject_HEAD
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) DataObjectType;
 
-/* "recordclass/dataobject.pyx":787
+/* "recordclass/dataobject.pyx":775
  * 
  * @cython.final
  * cdef public class dataobjectiter[object DataObjectIter, type DataObjectIterType]:             # <<<<<<<<<<<<<<
  *     cdef PyObject *op "op"
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectIter {
@@ -892,71 +894,71 @@
   PyObject *op;
   Py_ssize_t i;
   Py_ssize_t n;
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) DataObjectIterType;
 
-/* "recordclass/dataobject.pyx":809
+/* "recordclass/dataobject.pyx":797
  * 
  * @cython.final
  * cdef public class dataobjectgetset[object DataObjectGetSet, type DataObjectGetSetType]:             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectGetSet {
   PyObject_HEAD
   Py_ssize_t i;
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) DataObjectGetSetType;
 
-/* "recordclass/dataobject.pyx":827
+/* "recordclass/dataobject.pyx":815
  * 
  * @cython.final
  * cdef public class dataobjectget[object DataObjectGet, type DataObjectGetType]:             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectGet {
   PyObject_HEAD
   Py_ssize_t i;
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) DataObjectGetType;
 
-/* "recordclass/dataobject.pyx":840
+/* "recordclass/dataobject.pyx":828
  * 
  * @cython.final
  * cdef public class SequenceProxy[object SequenceProxyObject, type SequenceProxyType]:             # <<<<<<<<<<<<<<
  *     cdef object ob "ob"
  *     cdef Py_hash_t hash "hash"
  */
 struct SequenceProxyObject {
   PyObject_HEAD
   PyObject *ob;
   Py_hash_t hash;
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) SequenceProxyType;
 
-/* "recordclass/dataobject.pyx":624
+/* "recordclass/dataobject.pyx":612
  *         return ob
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,             # <<<<<<<<<<<<<<
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  */
 struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic {
   PyObject_HEAD
   PyTypeObject *tp;
 };
 
 
-/* "recordclass/dataobject.pyx":633
+/* "recordclass/dataobject.pyx":621
  * 
  *     if tp.tp_bases:
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)             # <<<<<<<<<<<<<<
  *     else:
  *         all_AC = False
  */
 struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct_1_genexpr {
@@ -1112,14 +1114,41 @@
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
 
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* UnpackUnboundCMethod.proto */
+typedef struct {
+    PyObject *type;
+    PyObject **method_name;
+    PyCFunction func;
+    PyObject *method;
+    int flag;
+} __Pyx_CachedCFunction;
+
+/* CallUnboundCMethod1.proto */
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#else
+#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
+#endif
+
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
@@ -1142,49 +1171,22 @@
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* UnpackUnboundCMethod.proto */
-typedef struct {
-    PyObject *type;
-    PyObject **method_name;
-    PyCFunction func;
-    PyObject *method;
-    int flag;
-} __Pyx_CachedCFunction;
-
-/* CallUnboundCMethod1.proto */
-static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#else
-#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
-#endif
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
@@ -1588,15 +1590,14 @@
 static PyTypeObject *__pyx_ptype_11recordclass_10dataobject_SequenceProxy = 0;
 static PyTypeObject *__pyx_ptype_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic = 0;
 static PyTypeObject *__pyx_ptype_11recordclass_10dataobject___pyx_scope_struct_1_genexpr = 0;
 static PyObject *slotsgetset_cache = 0;
 static PyObject *slotsget_cache = 0;
 static PyObject *dataobject_alloc(PyTypeObject *, Py_ssize_t); /*proto*/
 static void dataobject_free(void *); /*proto*/
-static int dataobject_hasdict(PyObject *); /*proto*/
 static CYTHON_INLINE Py_ssize_t dataobject_len(PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *dataobject_item(PyObject *, Py_ssize_t); /*proto*/
 static CYTHON_INLINE int dataobject_ass_item(PyObject *, Py_ssize_t, PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *dataobject_subscript(PyObject *, PyObject *); /*proto*/
 static CYTHON_INLINE int dataobject_ass_subscript(PyObject *, PyObject *, PyObject *); /*proto*/
 static CYTHON_INLINE int dataobject_clear(PyObject *); /*proto*/
 static CYTHON_INLINE int dataobject_traverse(PyObject *, visitproc, void *); /*proto*/
@@ -1898,15 +1899,15 @@
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__20;
 static PyObject *__pyx_codeobj__22;
 static PyObject *__pyx_codeobj__24;
 static PyObject *__pyx_codeobj__26;
 /* Late includes */
 
-/* "recordclass/dataobject.pyx":152
+/* "recordclass/dataobject.pyx":157
  * from cpython.object cimport Py_TPFLAGS_HAVE_GC
  * 
  * cdef inline int py_visit(PyObject *ob, visitproc visit, void *arg) except -1:             # <<<<<<<<<<<<<<
  *     cdef int vret
  *     if ob:
  */
 
@@ -1914,83 +1915,83 @@
   int __pyx_v_vret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("py_visit", 0);
 
-  /* "recordclass/dataobject.pyx":154
+  /* "recordclass/dataobject.pyx":159
  * cdef inline int py_visit(PyObject *ob, visitproc visit, void *arg) except -1:
  *     cdef int vret
  *     if ob:             # <<<<<<<<<<<<<<
  *         vret = visit(ob, arg)
  *         if vret:
  */
   __pyx_t_1 = (__pyx_v_ob != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":155
+    /* "recordclass/dataobject.pyx":160
  *     cdef int vret
  *     if ob:
  *         vret = visit(ob, arg)             # <<<<<<<<<<<<<<
  *         if vret:
  *             return vret
  */
-    __pyx_t_2 = __pyx_v_visit(__pyx_v_ob, __pyx_v_arg); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_visit(__pyx_v_ob, __pyx_v_arg); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 160, __pyx_L1_error)
     __pyx_v_vret = __pyx_t_2;
 
-    /* "recordclass/dataobject.pyx":156
+    /* "recordclass/dataobject.pyx":161
  *     if ob:
  *         vret = visit(ob, arg)
  *         if vret:             # <<<<<<<<<<<<<<
  *             return vret
  *     return 0
  */
     __pyx_t_1 = (__pyx_v_vret != 0);
     if (__pyx_t_1) {
 
-      /* "recordclass/dataobject.pyx":157
+      /* "recordclass/dataobject.pyx":162
  *         vret = visit(ob, arg)
  *         if vret:
  *             return vret             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
       __pyx_r = __pyx_v_vret;
       goto __pyx_L0;
 
-      /* "recordclass/dataobject.pyx":156
+      /* "recordclass/dataobject.pyx":161
  *     if ob:
  *         vret = visit(ob, arg)
  *         if vret:             # <<<<<<<<<<<<<<
  *             return vret
  *     return 0
  */
     }
 
-    /* "recordclass/dataobject.pyx":154
+    /* "recordclass/dataobject.pyx":159
  * cdef inline int py_visit(PyObject *ob, visitproc visit, void *arg) except -1:
  *     cdef int vret
  *     if ob:             # <<<<<<<<<<<<<<
  *         vret = visit(ob, arg)
  *         if vret:
  */
   }
 
-  /* "recordclass/dataobject.pyx":158
+  /* "recordclass/dataobject.pyx":163
  *         if vret:
  *             return vret
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef PyObject* dataobject_alloc "dataobject_alloc"(PyTypeObject *tp, Py_ssize_t n):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":152
+  /* "recordclass/dataobject.pyx":157
  * from cpython.object cimport Py_TPFLAGS_HAVE_GC
  * 
  * cdef inline int py_visit(PyObject *ob, visitproc visit, void *arg) except -1:             # <<<<<<<<<<<<<<
  *     cdef int vret
  *     if ob:
  */
 
@@ -1999,15 +2000,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.py_visit", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":160
+/* "recordclass/dataobject.pyx":165
  *     return 0
  * 
  * cdef PyObject* dataobject_alloc "dataobject_alloc"(PyTypeObject *tp, Py_ssize_t n):             # <<<<<<<<<<<<<<
  *     cdef PyObject *op "op"
  *     cdef Py_ssize_t size "size" = tp.tp_basicsize
  */
 
@@ -2018,189 +2019,180 @@
   PyObject *__pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3;
   __Pyx_RefNannySetupContext("dataobject_alloc", 0);
 
-  /* "recordclass/dataobject.pyx":162
+  /* "recordclass/dataobject.pyx":167
  * cdef PyObject* dataobject_alloc "dataobject_alloc"(PyTypeObject *tp, Py_ssize_t n):
  *     cdef PyObject *op "op"
  *     cdef Py_ssize_t size "size" = tp.tp_basicsize             # <<<<<<<<<<<<<<
  *     cdef bint is_gc "is_gc"
  * 
  */
   __pyx_t_1 = __pyx_v_tp->tp_basicsize;
   size = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":165
+  /* "recordclass/dataobject.pyx":170
  *     cdef bint is_gc "is_gc"
  * 
  *     is_gc = PyType_IS_GC(tp)             # <<<<<<<<<<<<<<
  *     if is_gc:
  *         op = _PyObject_GC_Malloc(size)
  */
   is_gc = PyType_IS_GC(__pyx_v_tp);
 
-  /* "recordclass/dataobject.pyx":166
+  /* "recordclass/dataobject.pyx":171
  * 
  *     is_gc = PyType_IS_GC(tp)
  *     if is_gc:             # <<<<<<<<<<<<<<
  *         op = _PyObject_GC_Malloc(size)
  *     else:
  */
   __pyx_t_2 = (is_gc != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":167
+    /* "recordclass/dataobject.pyx":172
  *     is_gc = PyType_IS_GC(tp)
  *     if is_gc:
  *         op = _PyObject_GC_Malloc(size)             # <<<<<<<<<<<<<<
  *     else:
  *         op = <PyObject*>PyObject_Malloc(size)
  */
     op = _PyObject_GC_Malloc(size);
 
-    /* "recordclass/dataobject.pyx":166
+    /* "recordclass/dataobject.pyx":171
  * 
  *     is_gc = PyType_IS_GC(tp)
  *     if is_gc:             # <<<<<<<<<<<<<<
  *         op = _PyObject_GC_Malloc(size)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "recordclass/dataobject.pyx":169
+  /* "recordclass/dataobject.pyx":174
  *         op = _PyObject_GC_Malloc(size)
  *     else:
  *         op = <PyObject*>PyObject_Malloc(size)             # <<<<<<<<<<<<<<
  * 
  *     if op == NULL:
  */
   /*else*/ {
     op = ((PyObject *)PyObject_Malloc(size));
   }
   __pyx_L3:;
 
-  /* "recordclass/dataobject.pyx":171
+  /* "recordclass/dataobject.pyx":176
  *         op = <PyObject*>PyObject_Malloc(size)
  * 
  *     if op == NULL:             # <<<<<<<<<<<<<<
  *         return PyErr_NoMemory()
  * 
  */
   __pyx_t_2 = ((op == NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":172
+    /* "recordclass/dataobject.pyx":177
  * 
  *     if op == NULL:
  *         return PyErr_NoMemory()             # <<<<<<<<<<<<<<
  * 
- *     memset(op, 0, size)
+ *     #memset(op, 0, size)
  */
-    __pyx_t_3 = PyErr_NoMemory(); if (unlikely(__pyx_t_3 == ((PyObject *)NULL))) __PYX_ERR(0, 172, __pyx_L1_error)
+    __pyx_t_3 = PyErr_NoMemory(); if (unlikely(__pyx_t_3 == ((PyObject *)NULL))) __PYX_ERR(0, 177, __pyx_L1_error)
     __pyx_r = __pyx_t_3;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":171
+    /* "recordclass/dataobject.pyx":176
  *         op = <PyObject*>PyObject_Malloc(size)
  * 
  *     if op == NULL:             # <<<<<<<<<<<<<<
  *         return PyErr_NoMemory()
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":174
- *         return PyErr_NoMemory()
- * 
- *     memset(op, 0, size)             # <<<<<<<<<<<<<<
- * 
- *     if tp.tp_flags & Py_TPFLAGS_HEAPTYPE:
- */
-  (void)(memset(op, 0, size));
-
-  /* "recordclass/dataobject.pyx":176
- *     memset(op, 0, size)
+  /* "recordclass/dataobject.pyx":181
+ *     #memset(op, 0, size)
  * 
  *     if tp.tp_flags & Py_TPFLAGS_HEAPTYPE:             # <<<<<<<<<<<<<<
  *         Py_INCREF(<PyObject*>tp)
  * 
  */
   __pyx_t_2 = ((__pyx_v_tp->tp_flags & Py_TPFLAGS_HEAPTYPE) != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":177
+    /* "recordclass/dataobject.pyx":182
  * 
  *     if tp.tp_flags & Py_TPFLAGS_HEAPTYPE:
  *         Py_INCREF(<PyObject*>tp)             # <<<<<<<<<<<<<<
  * 
  *     PyObject_INIT(op, tp)
  */
     Py_INCREF(((PyObject *)__pyx_v_tp));
 
-    /* "recordclass/dataobject.pyx":176
- *     memset(op, 0, size)
+    /* "recordclass/dataobject.pyx":181
+ *     #memset(op, 0, size)
  * 
  *     if tp.tp_flags & Py_TPFLAGS_HEAPTYPE:             # <<<<<<<<<<<<<<
  *         Py_INCREF(<PyObject*>tp)
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":179
+  /* "recordclass/dataobject.pyx":184
  *         Py_INCREF(<PyObject*>tp)
  * 
  *     PyObject_INIT(op, tp)             # <<<<<<<<<<<<<<
  * 
  *     if is_gc:
  */
   PyObject_INIT(op, __pyx_v_tp);
 
-  /* "recordclass/dataobject.pyx":181
+  /* "recordclass/dataobject.pyx":186
  *     PyObject_INIT(op, tp)
  * 
  *     if is_gc:             # <<<<<<<<<<<<<<
  *         PyObject_GC_Track(op)
  * 
  */
   __pyx_t_2 = (is_gc != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":182
+    /* "recordclass/dataobject.pyx":187
  * 
  *     if is_gc:
  *         PyObject_GC_Track(op)             # <<<<<<<<<<<<<<
  * 
  *     return op
  */
     PyObject_GC_Track(op);
 
-    /* "recordclass/dataobject.pyx":181
+    /* "recordclass/dataobject.pyx":186
  *     PyObject_INIT(op, tp)
  * 
  *     if is_gc:             # <<<<<<<<<<<<<<
  *         PyObject_GC_Track(op)
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":184
+  /* "recordclass/dataobject.pyx":189
  *         PyObject_GC_Track(op)
  * 
  *     return op             # <<<<<<<<<<<<<<
  * 
  * # cdef PyObject* dataobject_new(PyTypeObject *tp, PyObject *args, PyObject *kw):
  */
   __pyx_r = op;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":160
+  /* "recordclass/dataobject.pyx":165
  *     return 0
  * 
  * cdef PyObject* dataobject_alloc "dataobject_alloc"(PyTypeObject *tp, Py_ssize_t n):             # <<<<<<<<<<<<<<
  *     cdef PyObject *op "op"
  *     cdef Py_ssize_t size "size" = tp.tp_basicsize
  */
 
@@ -2209,278 +2201,204 @@
   __Pyx_WriteUnraisable("recordclass.dataobject.dataobject_alloc", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":234
+/* "recordclass/dataobject.pyx":239
  * #     return op
  * 
  * cdef void dataobject_free "dataobject_free"(void *op):             # <<<<<<<<<<<<<<
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):
  *         PyObject_GC_UnTrack(<PyObject*>op)
  */
 
 static void dataobject_free(void *__pyx_v_op) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("dataobject_free", 0);
 
-  /* "recordclass/dataobject.pyx":235
+  /* "recordclass/dataobject.pyx":240
  * 
  * cdef void dataobject_free "dataobject_free"(void *op):
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):             # <<<<<<<<<<<<<<
  *         PyObject_GC_UnTrack(<PyObject*>op)
  *         PyObject_GC_Del(<PyObject*>op)
  */
   __pyx_t_1 = (PyType_IS_GC(Py_TYPE(((PyObject *)__pyx_v_op))) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":236
+    /* "recordclass/dataobject.pyx":241
  * cdef void dataobject_free "dataobject_free"(void *op):
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):
  *         PyObject_GC_UnTrack(<PyObject*>op)             # <<<<<<<<<<<<<<
  *         PyObject_GC_Del(<PyObject*>op)
  *     else:
  */
     PyObject_GC_UnTrack(((PyObject *)__pyx_v_op));
 
-    /* "recordclass/dataobject.pyx":237
+    /* "recordclass/dataobject.pyx":242
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):
  *         PyObject_GC_UnTrack(<PyObject*>op)
  *         PyObject_GC_Del(<PyObject*>op)             # <<<<<<<<<<<<<<
  *     else:
  *         PyObject_Del(<PyObject*>op)
  */
     PyObject_GC_Del(((PyObject *)__pyx_v_op));
 
-    /* "recordclass/dataobject.pyx":235
+    /* "recordclass/dataobject.pyx":240
  * 
  * cdef void dataobject_free "dataobject_free"(void *op):
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):             # <<<<<<<<<<<<<<
  *         PyObject_GC_UnTrack(<PyObject*>op)
  *         PyObject_GC_Del(<PyObject*>op)
  */
     goto __pyx_L3;
   }
 
-  /* "recordclass/dataobject.pyx":239
+  /* "recordclass/dataobject.pyx":244
  *         PyObject_GC_Del(<PyObject*>op)
  *     else:
  *         PyObject_Del(<PyObject*>op)             # <<<<<<<<<<<<<<
  * 
- * # cdef inline PyObject** dataobject_items(PyObject *op):
+ * cdef inline Py_ssize_t dataobject_len "dataobject_len"(PyObject *op):
  */
   /*else*/ {
     PyObject_Del(((PyObject *)__pyx_v_op));
   }
   __pyx_L3:;
 
-  /* "recordclass/dataobject.pyx":234
+  /* "recordclass/dataobject.pyx":239
  * #     return op
  * 
  * cdef void dataobject_free "dataobject_free"(void *op):             # <<<<<<<<<<<<<<
  *     if PyType_IS_GC(Py_TYPE(<PyObject*>op)):
  *         PyObject_GC_UnTrack(<PyObject*>op)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "recordclass/dataobject.pyx":250
- * #     return <PyObject**>(<char*>op + tp.tp_weaklistoffset)
- * 
- * cdef bint dataobject_hasdict "dataobject_hasdict"(PyObject *op):             # <<<<<<<<<<<<<<
- *     return (Py_TYPE(<PyObject*>op)).tp_dictoffset != 0
- * 
- */
-
-static int dataobject_hasdict(PyObject *__pyx_v_op) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("dataobject_hasdict", 0);
-
-  /* "recordclass/dataobject.pyx":251
- * 
- * cdef bint dataobject_hasdict "dataobject_hasdict"(PyObject *op):
- *     return (Py_TYPE(<PyObject*>op)).tp_dictoffset != 0             # <<<<<<<<<<<<<<
- * 
- * cdef bint dataobject_hasweaklist "dataobject_hasweaklist"(PyObject *op):
- */
-  __pyx_r = (Py_TYPE(((PyObject *)__pyx_v_op))->tp_dictoffset != 0);
-  goto __pyx_L0;
-
-  /* "recordclass/dataobject.pyx":250
- * #     return <PyObject**>(<char*>op + tp.tp_weaklistoffset)
- * 
- * cdef bint dataobject_hasdict "dataobject_hasdict"(PyObject *op):             # <<<<<<<<<<<<<<
- *     return (Py_TYPE(<PyObject*>op)).tp_dictoffset != 0
- * 
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "recordclass/dataobject.pyx":253
- *     return (Py_TYPE(<PyObject*>op)).tp_dictoffset != 0
- * 
- * cdef bint dataobject_hasweaklist "dataobject_hasweaklist"(PyObject *op):             # <<<<<<<<<<<<<<
- *     return (Py_TYPE(<PyObject*>op)).tp_weaklistoffset != 0
- * 
- */
-
-static int dataobject_hasweaklist(PyObject *__pyx_v_op) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("dataobject_hasweaklist", 0);
-
-  /* "recordclass/dataobject.pyx":254
- * 
- * cdef bint dataobject_hasweaklist "dataobject_hasweaklist"(PyObject *op):
- *     return (Py_TYPE(<PyObject*>op)).tp_weaklistoffset != 0             # <<<<<<<<<<<<<<
- * 
- * cdef inline Py_ssize_t dataobject_len "dataobject_len"(PyObject *op):
- */
-  __pyx_r = (Py_TYPE(((PyObject *)__pyx_v_op))->tp_weaklistoffset != 0);
-  goto __pyx_L0;
-
-  /* "recordclass/dataobject.pyx":253
- *     return (Py_TYPE(<PyObject*>op)).tp_dictoffset != 0
- * 
- * cdef bint dataobject_hasweaklist "dataobject_hasweaklist"(PyObject *op):             # <<<<<<<<<<<<<<
- *     return (Py_TYPE(<PyObject*>op)).tp_weaklistoffset != 0
- * 
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "recordclass/dataobject.pyx":256
- *     return (Py_TYPE(<PyObject*>op)).tp_weaklistoffset != 0
+/* "recordclass/dataobject.pyx":246
+ *         PyObject_Del(<PyObject*>op)
  * 
  * cdef inline Py_ssize_t dataobject_len "dataobject_len"(PyObject *op):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp = Py_TYPE(op)
  *     cdef Py_ssize_t size
  */
 
 static CYTHON_INLINE Py_ssize_t dataobject_len(PyObject *__pyx_v_op) {
   PyTypeObject *__pyx_v_tp;
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("dataobject_len", 0);
 
-  /* "recordclass/dataobject.pyx":257
+  /* "recordclass/dataobject.pyx":247
  * 
  * cdef inline Py_ssize_t dataobject_len "dataobject_len"(PyObject *op):
  *     cdef PyTypeObject *tp = Py_TYPE(op)             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t size
  * 
  */
   __pyx_v_tp = Py_TYPE(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":260
+  /* "recordclass/dataobject.pyx":250
  *     cdef Py_ssize_t size
  * 
  *     size = C_DIV(tp.tp_basicsize - sizeof(PyObject), sizeof(PyObject*))             # <<<<<<<<<<<<<<
  *     if tp.tp_dictoffset != 0:
  *         size -= 1
  */
   __pyx_v_size = C_DIV((__pyx_v_tp->tp_basicsize - (sizeof(PyObject))), (sizeof(PyObject *)));
 
-  /* "recordclass/dataobject.pyx":261
+  /* "recordclass/dataobject.pyx":251
  * 
  *     size = C_DIV(tp.tp_basicsize - sizeof(PyObject), sizeof(PyObject*))
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         size -= 1
  *     if tp.tp_weaklistoffset != 0:
  */
   __pyx_t_1 = ((__pyx_v_tp->tp_dictoffset != 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":262
+    /* "recordclass/dataobject.pyx":252
  *     size = C_DIV(tp.tp_basicsize - sizeof(PyObject), sizeof(PyObject*))
  *     if tp.tp_dictoffset != 0:
  *         size -= 1             # <<<<<<<<<<<<<<
  *     if tp.tp_weaklistoffset != 0:
  *         size -= 1
  */
     __pyx_v_size = (__pyx_v_size - 1);
 
-    /* "recordclass/dataobject.pyx":261
+    /* "recordclass/dataobject.pyx":251
  * 
  *     size = C_DIV(tp.tp_basicsize - sizeof(PyObject), sizeof(PyObject*))
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         size -= 1
  *     if tp.tp_weaklistoffset != 0:
  */
   }
 
-  /* "recordclass/dataobject.pyx":263
+  /* "recordclass/dataobject.pyx":253
  *     if tp.tp_dictoffset != 0:
  *         size -= 1
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         size -= 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_tp->tp_weaklistoffset != 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":264
+    /* "recordclass/dataobject.pyx":254
  *         size -= 1
  *     if tp.tp_weaklistoffset != 0:
  *         size -= 1             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size - 1);
 
-    /* "recordclass/dataobject.pyx":263
+    /* "recordclass/dataobject.pyx":253
  *     if tp.tp_dictoffset != 0:
  *         size -= 1
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         size -= 1
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":266
+  /* "recordclass/dataobject.pyx":256
  *         size -= 1
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * cdef inline PyObject* dataobject_item "dataobject_item"(PyObject *op, Py_ssize_t i):
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":256
- *     return (Py_TYPE(<PyObject*>op)).tp_weaklistoffset != 0
+  /* "recordclass/dataobject.pyx":246
+ *         PyObject_Del(<PyObject*>op)
  * 
  * cdef inline Py_ssize_t dataobject_len "dataobject_len"(PyObject *op):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp = Py_TYPE(op)
  *     cdef Py_ssize_t size
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":268
+/* "recordclass/dataobject.pyx":258
  *     return size
  * 
  * cdef inline PyObject* dataobject_item "dataobject_item"(PyObject *op, Py_ssize_t i):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t n
  *     cdef PyObject* val
  */
 
@@ -2490,61 +2408,61 @@
   PyObject **__pyx_v_items;
   PyObject *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("dataobject_item", 0);
 
-  /* "recordclass/dataobject.pyx":273
+  /* "recordclass/dataobject.pyx":263
  *     cdef PyObject **items
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *     items = dataobject_items(op)
  * 
  */
   __pyx_v_n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":274
+  /* "recordclass/dataobject.pyx":264
  * 
  *     n = dataobject_len(op)
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     if i < 0:
  */
   __pyx_v_items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":276
+  /* "recordclass/dataobject.pyx":266
  *     items = dataobject_items(op)
  * 
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i < 0 or i >= n:
  */
   __pyx_t_1 = ((__pyx_v_i < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":277
+    /* "recordclass/dataobject.pyx":267
  * 
  *     if i < 0:
  *         i += n             # <<<<<<<<<<<<<<
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  */
     __pyx_v_i = (__pyx_v_i + __pyx_v_n);
 
-    /* "recordclass/dataobject.pyx":276
+    /* "recordclass/dataobject.pyx":266
  *     items = dataobject_items(op)
  * 
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i < 0 or i >= n:
  */
   }
 
-  /* "recordclass/dataobject.pyx":278
+  /* "recordclass/dataobject.pyx":268
  *     if i < 0:
  *         i += n
  *     if i < 0 or i >= n:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL
  */
   __pyx_t_2 = ((__pyx_v_i < 0) != 0);
@@ -2554,85 +2472,85 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_i >= __pyx_v_n) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":279
+    /* "recordclass/dataobject.pyx":269
  *         i += n
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
     PyErr_SetString(PyExc_IndexError, ((char *)"index out of range"));
 
-    /* "recordclass/dataobject.pyx":280
+    /* "recordclass/dataobject.pyx":270
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL             # <<<<<<<<<<<<<<
  * 
  *     val = items[i]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":278
+    /* "recordclass/dataobject.pyx":268
  *     if i < 0:
  *         i += n
  *     if i < 0 or i >= n:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL
  */
   }
 
-  /* "recordclass/dataobject.pyx":282
+  /* "recordclass/dataobject.pyx":272
  *         return NULL
  * 
  *     val = items[i]             # <<<<<<<<<<<<<<
  *     Py_INCREF(val)
  *     return val
  */
   __pyx_v_val = (__pyx_v_items[__pyx_v_i]);
 
-  /* "recordclass/dataobject.pyx":283
+  /* "recordclass/dataobject.pyx":273
  * 
  *     val = items[i]
  *     Py_INCREF(val)             # <<<<<<<<<<<<<<
  *     return val
  * 
  */
   Py_INCREF(__pyx_v_val);
 
-  /* "recordclass/dataobject.pyx":284
+  /* "recordclass/dataobject.pyx":274
  *     val = items[i]
  *     Py_INCREF(val)
  *     return val             # <<<<<<<<<<<<<<
  * 
  * cdef inline int dataobject_ass_item "dataobject_ass_item"(PyObject *op, Py_ssize_t i, PyObject *val):
  */
   __pyx_r = __pyx_v_val;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":268
+  /* "recordclass/dataobject.pyx":258
  *     return size
  * 
  * cdef inline PyObject* dataobject_item "dataobject_item"(PyObject *op, Py_ssize_t i):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t n
  *     cdef PyObject* val
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":286
+/* "recordclass/dataobject.pyx":276
  *     return val
  * 
  * cdef inline int dataobject_ass_item "dataobject_ass_item"(PyObject *op, Py_ssize_t i, PyObject *val):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t n
  *     cdef PyObject **items
  */
 
@@ -2641,61 +2559,61 @@
   PyObject **__pyx_v_items;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("dataobject_ass_item", 0);
 
-  /* "recordclass/dataobject.pyx":290
+  /* "recordclass/dataobject.pyx":280
  *     cdef PyObject **items
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *     items = dataobject_items(op)
  * 
  */
   __pyx_v_n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":291
+  /* "recordclass/dataobject.pyx":281
  * 
  *     n = dataobject_len(op)
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     if i < 0:
  */
   __pyx_v_items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":293
+  /* "recordclass/dataobject.pyx":283
  *     items = dataobject_items(op)
  * 
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i < 0 or i >= n:
  */
   __pyx_t_1 = ((__pyx_v_i < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":294
+    /* "recordclass/dataobject.pyx":284
  * 
  *     if i < 0:
  *         i += n             # <<<<<<<<<<<<<<
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  */
     __pyx_v_i = (__pyx_v_i + __pyx_v_n);
 
-    /* "recordclass/dataobject.pyx":293
+    /* "recordclass/dataobject.pyx":283
  *     items = dataobject_items(op)
  * 
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i < 0 or i >= n:
  */
   }
 
-  /* "recordclass/dataobject.pyx":295
+  /* "recordclass/dataobject.pyx":285
  *     if i < 0:
  *         i += n
  *     if i < 0 or i >= n:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0
  */
   __pyx_t_2 = ((__pyx_v_i < 0) != 0);
@@ -2705,85 +2623,85 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_i >= __pyx_v_n) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":296
+    /* "recordclass/dataobject.pyx":286
  *         i += n
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     PyErr_SetString(PyExc_IndexError, ((char *)"index out of range"));
 
-    /* "recordclass/dataobject.pyx":297
+    /* "recordclass/dataobject.pyx":287
  *     if i < 0 or i >= n:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     Py_INCREF(val)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":295
+    /* "recordclass/dataobject.pyx":285
  *     if i < 0:
  *         i += n
  *     if i < 0 or i >= n:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0
  */
   }
 
-  /* "recordclass/dataobject.pyx":299
+  /* "recordclass/dataobject.pyx":289
  *         return 0
  * 
  *     Py_INCREF(val)             # <<<<<<<<<<<<<<
  *     items[i] = val
  *     return 0
  */
   Py_INCREF(__pyx_v_val);
 
-  /* "recordclass/dataobject.pyx":300
+  /* "recordclass/dataobject.pyx":290
  * 
  *     Py_INCREF(val)
  *     items[i] = val             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   (__pyx_v_items[__pyx_v_i]) = __pyx_v_val;
 
-  /* "recordclass/dataobject.pyx":301
+  /* "recordclass/dataobject.pyx":291
  *     Py_INCREF(val)
  *     items[i] = val
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef inline PyObject* dataobject_subscript "dataobject_subscript"(PyObject *op, PyObject *ind):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":286
+  /* "recordclass/dataobject.pyx":276
  *     return val
  * 
  * cdef inline int dataobject_ass_item "dataobject_ass_item"(PyObject *op, Py_ssize_t i, PyObject *val):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t n
  *     cdef PyObject **items
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":303
+/* "recordclass/dataobject.pyx":293
  *     return 0
  * 
  * cdef inline PyObject* dataobject_subscript "dataobject_subscript"(PyObject *op, PyObject *ind):             # <<<<<<<<<<<<<<
  *     cdef PyObject *val
  *     cdef Py_ssize_t i, n
  */
 
@@ -2795,71 +2713,71 @@
   PyObject *__pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("dataobject_subscript", 0);
 
-  /* "recordclass/dataobject.pyx":308
+  /* "recordclass/dataobject.pyx":298
  *     cdef PyObject **items
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *     items = dataobject_items(op)
  * 
  */
   __pyx_v_n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":309
+  /* "recordclass/dataobject.pyx":299
  * 
  *     n = dataobject_len(op)
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  */
   __pyx_v_items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":311
+  /* "recordclass/dataobject.pyx":301
  *     items = dataobject_items(op)
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)             # <<<<<<<<<<<<<<
  *     if i < 0:
  *         i += n
  */
-  __pyx_t_1 = PyNumber_AsSsize_t(__pyx_v_ind, ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_AsSsize_t(__pyx_v_ind, ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
   __pyx_v_i = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":312
+  /* "recordclass/dataobject.pyx":302
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i >= n or i < 0:
  */
   __pyx_t_2 = ((__pyx_v_i < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":313
+    /* "recordclass/dataobject.pyx":303
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:
  *         i += n             # <<<<<<<<<<<<<<
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  */
     __pyx_v_i = (__pyx_v_i + __pyx_v_n);
 
-    /* "recordclass/dataobject.pyx":312
+    /* "recordclass/dataobject.pyx":302
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i >= n or i < 0:
  */
   }
 
-  /* "recordclass/dataobject.pyx":314
+  /* "recordclass/dataobject.pyx":304
  *     if i < 0:
  *         i += n
  *     if i >= n or i < 0:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL
  */
   __pyx_t_3 = ((__pyx_v_i >= __pyx_v_n) != 0);
@@ -2869,71 +2787,71 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_3 = ((__pyx_v_i < 0) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":315
+    /* "recordclass/dataobject.pyx":305
  *         i += n
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
     PyErr_SetString(PyExc_IndexError, ((char *)"index out of range"));
 
-    /* "recordclass/dataobject.pyx":316
+    /* "recordclass/dataobject.pyx":306
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL             # <<<<<<<<<<<<<<
  * 
  *     val = items[i]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":314
+    /* "recordclass/dataobject.pyx":304
  *     if i < 0:
  *         i += n
  *     if i >= n or i < 0:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return NULL
  */
   }
 
-  /* "recordclass/dataobject.pyx":318
+  /* "recordclass/dataobject.pyx":308
  *         return NULL
  * 
  *     val = items[i]             # <<<<<<<<<<<<<<
  *     Py_INCREF(val)
  *     return val
  */
   __pyx_v_val = (__pyx_v_items[__pyx_v_i]);
 
-  /* "recordclass/dataobject.pyx":319
+  /* "recordclass/dataobject.pyx":309
  * 
  *     val = items[i]
  *     Py_INCREF(val)             # <<<<<<<<<<<<<<
  *     return val
  * 
  */
   Py_INCREF(__pyx_v_val);
 
-  /* "recordclass/dataobject.pyx":320
+  /* "recordclass/dataobject.pyx":310
  *     val = items[i]
  *     Py_INCREF(val)
  *     return val             # <<<<<<<<<<<<<<
  * 
  * cdef inline int dataobject_ass_subscript "dataobject_ass_subscript"(PyObject *op, PyObject *ind, PyObject *val):
  */
   __pyx_r = __pyx_v_val;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":303
+  /* "recordclass/dataobject.pyx":293
  *     return 0
  * 
  * cdef inline PyObject* dataobject_subscript "dataobject_subscript"(PyObject *op, PyObject *ind):             # <<<<<<<<<<<<<<
  *     cdef PyObject *val
  *     cdef Py_ssize_t i, n
  */
 
@@ -2942,15 +2860,15 @@
   __Pyx_WriteUnraisable("recordclass.dataobject.dataobject_subscript", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":322
+/* "recordclass/dataobject.pyx":312
  *     return val
  * 
  * cdef inline int dataobject_ass_subscript "dataobject_ass_subscript"(PyObject *op, PyObject *ind, PyObject *val):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i "i", n "n"
  *     cdef PyObject **items "items"
  */
 
@@ -2961,71 +2879,71 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("dataobject_ass_subscript", 0);
 
-  /* "recordclass/dataobject.pyx":326
+  /* "recordclass/dataobject.pyx":316
  *     cdef PyObject **items "items"
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *     items = dataobject_items(op)
  * 
  */
   n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":327
+  /* "recordclass/dataobject.pyx":317
  * 
  *     n = dataobject_len(op)
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  */
   items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":329
+  /* "recordclass/dataobject.pyx":319
  *     items = dataobject_items(op)
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)             # <<<<<<<<<<<<<<
  *     if i < 0:
  *         i += n
  */
-  __pyx_t_1 = PyNumber_AsSsize_t(__pyx_v_ind, ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_AsSsize_t(__pyx_v_ind, ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
   i = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":330
+  /* "recordclass/dataobject.pyx":320
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i >= n or i < 0:
  */
   __pyx_t_2 = ((i < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":331
+    /* "recordclass/dataobject.pyx":321
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:
  *         i += n             # <<<<<<<<<<<<<<
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  */
     i = (i + n);
 
-    /* "recordclass/dataobject.pyx":330
+    /* "recordclass/dataobject.pyx":320
  * 
  *     i = PyNumber_AsSsize_t(ind, <PyObject*>PyExc_IndexError)
  *     if i < 0:             # <<<<<<<<<<<<<<
  *         i += n
  *     if i >= n or i < 0:
  */
   }
 
-  /* "recordclass/dataobject.pyx":332
+  /* "recordclass/dataobject.pyx":322
  *     if i < 0:
  *         i += n
  *     if i >= n or i < 0:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0
  */
   __pyx_t_3 = ((i >= n) != 0);
@@ -3035,71 +2953,71 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_3 = ((i < 0) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":333
+    /* "recordclass/dataobject.pyx":323
  *         i += n
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     PyErr_SetString(PyExc_IndexError, ((char *)"index out of range"));
 
-    /* "recordclass/dataobject.pyx":334
+    /* "recordclass/dataobject.pyx":324
  *     if i >= n or i < 0:
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     Py_INCREF(val)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":332
+    /* "recordclass/dataobject.pyx":322
  *     if i < 0:
  *         i += n
  *     if i >= n or i < 0:             # <<<<<<<<<<<<<<
  *         PyErr_SetString(PyExc_IndexError, "index out of range")
  *         return 0
  */
   }
 
-  /* "recordclass/dataobject.pyx":336
+  /* "recordclass/dataobject.pyx":326
  *         return 0
  * 
  *     Py_INCREF(val)             # <<<<<<<<<<<<<<
  *     items[i] = val
  *     return 0
  */
   Py_INCREF(__pyx_v_val);
 
-  /* "recordclass/dataobject.pyx":337
+  /* "recordclass/dataobject.pyx":327
  * 
  *     Py_INCREF(val)
  *     items[i] = val             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   (items[i]) = __pyx_v_val;
 
-  /* "recordclass/dataobject.pyx":338
+  /* "recordclass/dataobject.pyx":328
  *     Py_INCREF(val)
  *     items[i] = val
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef inline int dataobject_clear "dataobject_clear"(PyObject *op) except -1:
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":322
+  /* "recordclass/dataobject.pyx":312
  *     return val
  * 
  * cdef inline int dataobject_ass_subscript "dataobject_ass_subscript"(PyObject *op, PyObject *ind, PyObject *val):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i "i", n "n"
  *     cdef PyObject **items "items"
  */
 
@@ -3108,15 +3026,15 @@
   __Pyx_WriteUnraisable("recordclass.dataobject.dataobject_ass_subscript", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":340
+/* "recordclass/dataobject.pyx":330
  *     return 0
  * 
  * cdef inline int dataobject_clear "dataobject_clear"(PyObject *op) except -1:             # <<<<<<<<<<<<<<
  *     cdef PyObject **items "items"
  *     cdef PyObject **temp "temp"
  */
 
@@ -3132,261 +3050,261 @@
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   __Pyx_RefNannySetupContext("dataobject_clear", 0);
 
-  /* "recordclass/dataobject.pyx":344
+  /* "recordclass/dataobject.pyx":334
  *     cdef PyObject **temp "temp"
  *     cdef PyObject *ob "ob"
  *     cdef PyTypeObject *tp "tp" = Py_TYPE(op)             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i "i", n "n"
  * 
  */
   tp = Py_TYPE(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":347
+  /* "recordclass/dataobject.pyx":337
  *     cdef Py_ssize_t i "i", n "n"
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *     items = dataobject_items(op)
  * 
  */
   n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":348
+  /* "recordclass/dataobject.pyx":338
  * 
  *     n = dataobject_len(op)
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
   items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":350
+  /* "recordclass/dataobject.pyx":340
  *     items = dataobject_items(op)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         ob = items[i]
  *         Py_XDECREF(ob)
  */
   __pyx_t_1 = n;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     i = __pyx_t_3;
 
-    /* "recordclass/dataobject.pyx":351
+    /* "recordclass/dataobject.pyx":341
  * 
  *     for i in range(n):
  *         ob = items[i]             # <<<<<<<<<<<<<<
  *         Py_XDECREF(ob)
  *         Py_INCREF(Py_None)
  */
     ob = (items[i]);
 
-    /* "recordclass/dataobject.pyx":352
+    /* "recordclass/dataobject.pyx":342
  *     for i in range(n):
  *         ob = items[i]
  *         Py_XDECREF(ob)             # <<<<<<<<<<<<<<
  *         Py_INCREF(Py_None)
  *         items[i] = Py_None
  */
     Py_XDECREF(ob);
 
-    /* "recordclass/dataobject.pyx":353
+    /* "recordclass/dataobject.pyx":343
  *         ob = items[i]
  *         Py_XDECREF(ob)
  *         Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  *         items[i] = Py_None
  * 
  */
     Py_INCREF(Py_None);
 
-    /* "recordclass/dataobject.pyx":354
+    /* "recordclass/dataobject.pyx":344
  *         Py_XDECREF(ob)
  *         Py_INCREF(Py_None)
  *         items[i] = Py_None             # <<<<<<<<<<<<<<
  * 
  *     if tp.tp_dictoffset != 0:
  */
     (items[i]) = Py_None;
   }
 
-  /* "recordclass/dataobject.pyx":356
+  /* "recordclass/dataobject.pyx":346
  *         items[i] = Py_None
  * 
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_dictptr(op, tp)
  *         ob = temp[0]
  */
   __pyx_t_4 = ((tp->tp_dictoffset != 0) != 0);
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":357
+    /* "recordclass/dataobject.pyx":347
  * 
  *     if tp.tp_dictoffset != 0:
  *         temp = dataobject_dictptr(op, tp)             # <<<<<<<<<<<<<<
  *         ob = temp[0]
  *         if ob:
  */
     temp = dataobject_dictptr(__pyx_v_op, tp);
 
-    /* "recordclass/dataobject.pyx":358
+    /* "recordclass/dataobject.pyx":348
  *     if tp.tp_dictoffset != 0:
  *         temp = dataobject_dictptr(op, tp)
  *         ob = temp[0]             # <<<<<<<<<<<<<<
  *         if ob:
  *             (<dict>ob).clear()
  */
     ob = (temp[0]);
 
-    /* "recordclass/dataobject.pyx":359
+    /* "recordclass/dataobject.pyx":349
  *         temp = dataobject_dictptr(op, tp)
  *         ob = temp[0]
  *         if ob:             # <<<<<<<<<<<<<<
  *             (<dict>ob).clear()
  *         Py_XDECREF(ob)
  */
     __pyx_t_4 = (ob != 0);
     if (__pyx_t_4) {
 
-      /* "recordclass/dataobject.pyx":360
+      /* "recordclass/dataobject.pyx":350
  *         ob = temp[0]
  *         if ob:
  *             (<dict>ob).clear()             # <<<<<<<<<<<<<<
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None
  */
       if (unlikely(((PyObject *)ob) == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-        __PYX_ERR(0, 360, __pyx_L1_error)
+        __PYX_ERR(0, 350, __pyx_L1_error)
       }
-      __pyx_t_5 = __Pyx_PyDict_Clear(((PyObject*)ob)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 360, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_Clear(((PyObject*)ob)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 350, __pyx_L1_error)
 
-      /* "recordclass/dataobject.pyx":359
+      /* "recordclass/dataobject.pyx":349
  *         temp = dataobject_dictptr(op, tp)
  *         ob = temp[0]
  *         if ob:             # <<<<<<<<<<<<<<
  *             (<dict>ob).clear()
  *         Py_XDECREF(ob)
  */
     }
 
-    /* "recordclass/dataobject.pyx":361
+    /* "recordclass/dataobject.pyx":351
  *         if ob:
  *             (<dict>ob).clear()
  *         Py_XDECREF(ob)             # <<<<<<<<<<<<<<
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)
  */
     Py_XDECREF(ob);
 
-    /* "recordclass/dataobject.pyx":362
+    /* "recordclass/dataobject.pyx":352
  *             (<dict>ob).clear()
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None             # <<<<<<<<<<<<<<
  *         Py_INCREF(Py_None)
  *     if tp.tp_weaklistoffset != 0:
  */
     (temp[0]) = Py_None;
 
-    /* "recordclass/dataobject.pyx":363
+    /* "recordclass/dataobject.pyx":353
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  *     if tp.tp_weaklistoffset != 0:
  *         temp = dataobject_weaklistptr(op, tp)
  */
     Py_INCREF(Py_None);
 
-    /* "recordclass/dataobject.pyx":356
+    /* "recordclass/dataobject.pyx":346
  *         items[i] = Py_None
  * 
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_dictptr(op, tp)
  *         ob = temp[0]
  */
   }
 
-  /* "recordclass/dataobject.pyx":364
+  /* "recordclass/dataobject.pyx":354
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  */
   __pyx_t_4 = ((tp->tp_weaklistoffset != 0) != 0);
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":365
+    /* "recordclass/dataobject.pyx":355
  *         Py_INCREF(Py_None)
  *     if tp.tp_weaklistoffset != 0:
  *         temp = dataobject_weaklistptr(op, tp)             # <<<<<<<<<<<<<<
  *         ob = temp[0]
  *         Py_XDECREF(ob)
  */
     temp = dataobject_weaklistptr(__pyx_v_op, tp);
 
-    /* "recordclass/dataobject.pyx":366
+    /* "recordclass/dataobject.pyx":356
  *     if tp.tp_weaklistoffset != 0:
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]             # <<<<<<<<<<<<<<
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None
  */
     ob = (temp[0]);
 
-    /* "recordclass/dataobject.pyx":367
+    /* "recordclass/dataobject.pyx":357
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  *         Py_XDECREF(ob)             # <<<<<<<<<<<<<<
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)
  */
     Py_XDECREF(ob);
 
-    /* "recordclass/dataobject.pyx":368
+    /* "recordclass/dataobject.pyx":358
  *         ob = temp[0]
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None             # <<<<<<<<<<<<<<
  *         Py_INCREF(Py_None)
  * 
  */
     (temp[0]) = Py_None;
 
-    /* "recordclass/dataobject.pyx":369
+    /* "recordclass/dataobject.pyx":359
  *         Py_XDECREF(ob)
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     Py_INCREF(Py_None);
 
-    /* "recordclass/dataobject.pyx":364
+    /* "recordclass/dataobject.pyx":354
  *         temp[0] = Py_None
  *         Py_INCREF(Py_None)
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  */
   }
 
-  /* "recordclass/dataobject.pyx":371
+  /* "recordclass/dataobject.pyx":361
  *         Py_INCREF(Py_None)
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * # cdef inline void dataobject_dealloc(PyObject *op):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":340
+  /* "recordclass/dataobject.pyx":330
  *     return 0
  * 
  * cdef inline int dataobject_clear "dataobject_clear"(PyObject *op) except -1:             # <<<<<<<<<<<<<<
  *     cdef PyObject **items "items"
  *     cdef PyObject **temp "temp"
  */
 
@@ -3395,15 +3313,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.dataobject_clear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":401
+/* "recordclass/dataobject.pyx":391
  * 
  * 
  * cdef inline int dataobject_traverse "dataobject_traverse"(PyObject *op, visitproc visit, void *arg) except -1:             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  *     cdef PyObject **items "items"
  */
 
@@ -3426,416 +3344,416 @@
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("dataobject_traverse", 0);
 
-  /* "recordclass/dataobject.pyx":402
+  /* "recordclass/dataobject.pyx":392
  * 
  * cdef inline int dataobject_traverse "dataobject_traverse"(PyObject *op, visitproc visit, void *arg) except -1:
  *     cdef PyTypeObject *tp "tp" = Py_TYPE(op)             # <<<<<<<<<<<<<<
  *     cdef PyObject **items "items"
  *     cdef PyObject **temp "temp"
  */
   tp = Py_TYPE(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":410
+  /* "recordclass/dataobject.pyx":400
  *     cdef int vret "vret"
  * 
  *     n = dataobject_len(op)             # <<<<<<<<<<<<<<
  * 
  *     items = dataobject_items(op)
  */
   n = dataobject_len(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":412
+  /* "recordclass/dataobject.pyx":402
  *     n = dataobject_len(op)
  * 
  *     items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
   items = dataobject_items(__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":414
+  /* "recordclass/dataobject.pyx":404
  *     items = dataobject_items(op)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         ob = items[i]
  *         if ob:
  */
   __pyx_t_1 = n;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     i = __pyx_t_3;
 
-    /* "recordclass/dataobject.pyx":415
+    /* "recordclass/dataobject.pyx":405
  * 
  *     for i in range(n):
  *         ob = items[i]             # <<<<<<<<<<<<<<
  *         if ob:
  *             vret = visit(ob, arg)
  */
     ob = (items[i]);
 
-    /* "recordclass/dataobject.pyx":416
+    /* "recordclass/dataobject.pyx":406
  *     for i in range(n):
  *         ob = items[i]
  *         if ob:             # <<<<<<<<<<<<<<
  *             vret = visit(ob, arg)
  *             if vret:
  */
     __pyx_t_4 = (ob != 0);
     if (__pyx_t_4) {
 
-      /* "recordclass/dataobject.pyx":417
+      /* "recordclass/dataobject.pyx":407
  *         ob = items[i]
  *         if ob:
  *             vret = visit(ob, arg)             # <<<<<<<<<<<<<<
  *             if vret:
  *                 return vret
  */
-      __pyx_t_5 = __pyx_v_visit(ob, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_5 = __pyx_v_visit(ob, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 407, __pyx_L1_error)
       vret = __pyx_t_5;
 
-      /* "recordclass/dataobject.pyx":418
+      /* "recordclass/dataobject.pyx":408
  *         if ob:
  *             vret = visit(ob, arg)
  *             if vret:             # <<<<<<<<<<<<<<
  *                 return vret
  * 
  */
       __pyx_t_4 = (vret != 0);
       if (__pyx_t_4) {
 
-        /* "recordclass/dataobject.pyx":419
+        /* "recordclass/dataobject.pyx":409
  *             vret = visit(ob, arg)
  *             if vret:
  *                 return vret             # <<<<<<<<<<<<<<
  * 
  *     if tp.tp_dictoffset != 0:
  */
         __pyx_r = vret;
         goto __pyx_L0;
 
-        /* "recordclass/dataobject.pyx":418
+        /* "recordclass/dataobject.pyx":408
  *         if ob:
  *             vret = visit(ob, arg)
  *             if vret:             # <<<<<<<<<<<<<<
  *                 return vret
  * 
  */
       }
 
-      /* "recordclass/dataobject.pyx":416
+      /* "recordclass/dataobject.pyx":406
  *     for i in range(n):
  *         ob = items[i]
  *         if ob:             # <<<<<<<<<<<<<<
  *             vret = visit(ob, arg)
  *             if vret:
  */
     }
   }
 
-  /* "recordclass/dataobject.pyx":421
+  /* "recordclass/dataobject.pyx":411
  *                 return vret
  * 
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_dictptr(op, tp)
  *         if temp[0]:
  */
   __pyx_t_4 = ((tp->tp_dictoffset != 0) != 0);
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":422
+    /* "recordclass/dataobject.pyx":412
  * 
  *     if tp.tp_dictoffset != 0:
  *         temp = dataobject_dictptr(op, tp)             # <<<<<<<<<<<<<<
  *         if temp[0]:
  *             obj = <object>temp[0]
  */
     temp = dataobject_dictptr(__pyx_v_op, tp);
 
-    /* "recordclass/dataobject.pyx":423
+    /* "recordclass/dataobject.pyx":413
  *     if tp.tp_dictoffset != 0:
  *         temp = dataobject_dictptr(op, tp)
  *         if temp[0]:             # <<<<<<<<<<<<<<
  *             obj = <object>temp[0]
  *             for key in obj:
  */
     __pyx_t_4 = ((temp[0]) != 0);
     if (__pyx_t_4) {
 
-      /* "recordclass/dataobject.pyx":424
+      /* "recordclass/dataobject.pyx":414
  *         temp = dataobject_dictptr(op, tp)
  *         if temp[0]:
  *             obj = <object>temp[0]             # <<<<<<<<<<<<<<
  *             for key in obj:
  *                 v = <PyObject*>obj[key]
  */
       __pyx_t_6 = ((PyObject *)(temp[0]));
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_obj = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "recordclass/dataobject.pyx":425
+      /* "recordclass/dataobject.pyx":415
  *         if temp[0]:
  *             obj = <object>temp[0]
  *             for key in obj:             # <<<<<<<<<<<<<<
  *                 v = <PyObject*>obj[key]
  *                 if v:
  */
       if (likely(PyList_CheckExact(__pyx_v_obj)) || PyTuple_CheckExact(__pyx_v_obj)) {
         __pyx_t_6 = __pyx_v_obj; __Pyx_INCREF(__pyx_t_6); __pyx_t_1 = 0;
         __pyx_t_7 = NULL;
       } else {
-        __pyx_t_1 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_obj); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 425, __pyx_L1_error)
+        __pyx_t_1 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_obj); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 425, __pyx_L1_error)
+        __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 415, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_7)) {
           if (likely(PyList_CheckExact(__pyx_t_6))) {
             if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_1); __Pyx_INCREF(__pyx_t_8); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
+            __pyx_t_8 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_1); __Pyx_INCREF(__pyx_t_8); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
             #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_6, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
+            __pyx_t_8 = PySequence_ITEM(__pyx_t_6, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 415, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
             #endif
           } else {
             if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_1); __Pyx_INCREF(__pyx_t_8); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
+            __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_1); __Pyx_INCREF(__pyx_t_8); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
             #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_6, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
+            __pyx_t_8 = PySequence_ITEM(__pyx_t_6, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 415, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
             #endif
           }
         } else {
           __pyx_t_8 = __pyx_t_7(__pyx_t_6);
           if (unlikely(!__pyx_t_8)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 425, __pyx_L1_error)
+              else __PYX_ERR(0, 415, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_8);
         }
         __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_8);
         __pyx_t_8 = 0;
 
-        /* "recordclass/dataobject.pyx":426
+        /* "recordclass/dataobject.pyx":416
  *             obj = <object>temp[0]
  *             for key in obj:
  *                 v = <PyObject*>obj[key]             # <<<<<<<<<<<<<<
  *                 if v:
  *                     vret = visit(v, arg)
  */
-        __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_obj, __pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 426, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_obj, __pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 416, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         v = ((PyObject *)__pyx_t_8);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "recordclass/dataobject.pyx":427
+        /* "recordclass/dataobject.pyx":417
  *             for key in obj:
  *                 v = <PyObject*>obj[key]
  *                 if v:             # <<<<<<<<<<<<<<
  *                     vret = visit(v, arg)
  *                     if vret:
  */
         __pyx_t_4 = (v != 0);
         if (__pyx_t_4) {
 
-          /* "recordclass/dataobject.pyx":428
+          /* "recordclass/dataobject.pyx":418
  *                 v = <PyObject*>obj[key]
  *                 if v:
  *                     vret = visit(v, arg)             # <<<<<<<<<<<<<<
  *                     if vret:
  *                         return vret
  */
-          __pyx_t_5 = __pyx_v_visit(v, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
+          __pyx_t_5 = __pyx_v_visit(v, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 418, __pyx_L1_error)
           vret = __pyx_t_5;
 
-          /* "recordclass/dataobject.pyx":429
+          /* "recordclass/dataobject.pyx":419
  *                 if v:
  *                     vret = visit(v, arg)
  *                     if vret:             # <<<<<<<<<<<<<<
  *                         return vret
  * 
  */
           __pyx_t_4 = (vret != 0);
           if (__pyx_t_4) {
 
-            /* "recordclass/dataobject.pyx":430
+            /* "recordclass/dataobject.pyx":420
  *                     vret = visit(v, arg)
  *                     if vret:
  *                         return vret             # <<<<<<<<<<<<<<
  * 
  *     if tp.tp_weaklistoffset != 0:
  */
             __pyx_r = vret;
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             goto __pyx_L0;
 
-            /* "recordclass/dataobject.pyx":429
+            /* "recordclass/dataobject.pyx":419
  *                 if v:
  *                     vret = visit(v, arg)
  *                     if vret:             # <<<<<<<<<<<<<<
  *                         return vret
  * 
  */
           }
 
-          /* "recordclass/dataobject.pyx":427
+          /* "recordclass/dataobject.pyx":417
  *             for key in obj:
  *                 v = <PyObject*>obj[key]
  *                 if v:             # <<<<<<<<<<<<<<
  *                     vret = visit(v, arg)
  *                     if vret:
  */
         }
 
-        /* "recordclass/dataobject.pyx":425
+        /* "recordclass/dataobject.pyx":415
  *         if temp[0]:
  *             obj = <object>temp[0]
  *             for key in obj:             # <<<<<<<<<<<<<<
  *                 v = <PyObject*>obj[key]
  *                 if v:
  */
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "recordclass/dataobject.pyx":423
+      /* "recordclass/dataobject.pyx":413
  *     if tp.tp_dictoffset != 0:
  *         temp = dataobject_dictptr(op, tp)
  *         if temp[0]:             # <<<<<<<<<<<<<<
  *             obj = <object>temp[0]
  *             for key in obj:
  */
     }
 
-    /* "recordclass/dataobject.pyx":421
+    /* "recordclass/dataobject.pyx":411
  *                 return vret
  * 
  *     if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_dictptr(op, tp)
  *         if temp[0]:
  */
   }
 
-  /* "recordclass/dataobject.pyx":432
+  /* "recordclass/dataobject.pyx":422
  *                         return vret
  * 
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  */
   __pyx_t_4 = ((tp->tp_weaklistoffset != 0) != 0);
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":433
+    /* "recordclass/dataobject.pyx":423
  * 
  *     if tp.tp_weaklistoffset != 0:
  *         temp = dataobject_weaklistptr(op, tp)             # <<<<<<<<<<<<<<
  *         ob = temp[0]
  *         if ob:
  */
     temp = dataobject_weaklistptr(__pyx_v_op, tp);
 
-    /* "recordclass/dataobject.pyx":434
+    /* "recordclass/dataobject.pyx":424
  *     if tp.tp_weaklistoffset != 0:
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]             # <<<<<<<<<<<<<<
  *         if ob:
  *             vret = visit(ob, arg)
  */
     ob = (temp[0]);
 
-    /* "recordclass/dataobject.pyx":435
+    /* "recordclass/dataobject.pyx":425
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  *         if ob:             # <<<<<<<<<<<<<<
  *             vret = visit(ob, arg)
  *             if vret:
  */
     __pyx_t_4 = (ob != 0);
     if (__pyx_t_4) {
 
-      /* "recordclass/dataobject.pyx":436
+      /* "recordclass/dataobject.pyx":426
  *         ob = temp[0]
  *         if ob:
  *             vret = visit(ob, arg)             # <<<<<<<<<<<<<<
  *             if vret:
  *                 return vret
  */
-      __pyx_t_5 = __pyx_v_visit(ob, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_5 = __pyx_v_visit(ob, __pyx_v_arg); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 426, __pyx_L1_error)
       vret = __pyx_t_5;
 
-      /* "recordclass/dataobject.pyx":437
+      /* "recordclass/dataobject.pyx":427
  *         if ob:
  *             vret = visit(ob, arg)
  *             if vret:             # <<<<<<<<<<<<<<
  *                 return vret
  * 
  */
       __pyx_t_4 = (vret != 0);
       if (__pyx_t_4) {
 
-        /* "recordclass/dataobject.pyx":438
+        /* "recordclass/dataobject.pyx":428
  *             vret = visit(ob, arg)
  *             if vret:
  *                 return vret             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
         __pyx_r = vret;
         goto __pyx_L0;
 
-        /* "recordclass/dataobject.pyx":437
+        /* "recordclass/dataobject.pyx":427
  *         if ob:
  *             vret = visit(ob, arg)
  *             if vret:             # <<<<<<<<<<<<<<
  *                 return vret
  * 
  */
       }
 
-      /* "recordclass/dataobject.pyx":435
+      /* "recordclass/dataobject.pyx":425
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  *         if ob:             # <<<<<<<<<<<<<<
  *             vret = visit(ob, arg)
  *             if vret:
  */
     }
 
-    /* "recordclass/dataobject.pyx":432
+    /* "recordclass/dataobject.pyx":422
  *                         return vret
  * 
  *     if tp.tp_weaklistoffset != 0:             # <<<<<<<<<<<<<<
  *         temp = dataobject_weaklistptr(op, tp)
  *         ob = temp[0]
  */
   }
 
-  /* "recordclass/dataobject.pyx":440
+  /* "recordclass/dataobject.pyx":430
  *                 return vret
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_hash_t dataobject_hash "dataobject_hash"(PyObject *op):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":401
+  /* "recordclass/dataobject.pyx":391
  * 
  * 
  * cdef inline int dataobject_traverse "dataobject_traverse"(PyObject *op, visitproc visit, void *arg) except -1:             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  *     cdef PyObject **items "items"
  */
 
@@ -3848,52 +3766,52 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":442
+/* "recordclass/dataobject.pyx":432
  *     return 0
  * 
  * cdef inline Py_hash_t dataobject_hash "dataobject_hash"(PyObject *op):             # <<<<<<<<<<<<<<
  *     t = tuple(<object>op)
  *     return <Py_hash_t>PyObject_Hash(<PyObject*>t)
  */
 
 static CYTHON_INLINE Py_hash_t dataobject_hash(PyObject *__pyx_v_op) {
   PyObject *__pyx_v_t = NULL;
   Py_hash_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("dataobject_hash", 0);
 
-  /* "recordclass/dataobject.pyx":443
+  /* "recordclass/dataobject.pyx":433
  * 
  * cdef inline Py_hash_t dataobject_hash "dataobject_hash"(PyObject *op):
  *     t = tuple(<object>op)             # <<<<<<<<<<<<<<
  *     return <Py_hash_t>PyObject_Hash(<PyObject*>t)
  * 
  */
-  __pyx_t_1 = __Pyx_PySequence_Tuple(((PyObject *)__pyx_v_op)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PySequence_Tuple(((PyObject *)__pyx_v_op)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_t = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":444
+  /* "recordclass/dataobject.pyx":434
  * cdef inline Py_hash_t dataobject_hash "dataobject_hash"(PyObject *op):
  *     t = tuple(<object>op)
  *     return <Py_hash_t>PyObject_Hash(<PyObject*>t)             # <<<<<<<<<<<<<<
  * 
  * @cython.auto_pickle(False)
  */
   __pyx_r = ((Py_hash_t)PyObject_Hash(((PyObject *)__pyx_v_t)));
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":442
+  /* "recordclass/dataobject.pyx":432
  *     return 0
  * 
  * cdef inline Py_hash_t dataobject_hash "dataobject_hash"(PyObject *op):             # <<<<<<<<<<<<<<
  *     t = tuple(<object>op)
  *     return <Py_hash_t>PyObject_Hash(<PyObject*>t)
  */
 
@@ -3904,15 +3822,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":449
+/* "recordclass/dataobject.pyx":439
  * cdef public class dataobject[object DataObject, type DataObjectType]:
  * 
  *     def __cinit__(self, *args, **kw):             # <<<<<<<<<<<<<<
  *         cdef PyObject *op "op"=<PyObject*>self
  *         cdef PyObject **items "items"
  */
 
@@ -3946,326 +3864,302 @@
   PyObject *v;
   Py_ssize_t i;
   Py_ssize_t n;
   PyObject *t = 0;
   PyObject *vv = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "recordclass/dataobject.pyx":450
+  /* "recordclass/dataobject.pyx":440
  * 
  *     def __cinit__(self, *args, **kw):
  *         cdef PyObject *op "op"=<PyObject*>self             # <<<<<<<<<<<<<<
  *         cdef PyObject **items "items"
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  */
   op = ((PyObject *)__pyx_v_self);
 
-  /* "recordclass/dataobject.pyx":452
+  /* "recordclass/dataobject.pyx":442
  *         cdef PyObject *op "op"=<PyObject*>self
  *         cdef PyObject **items "items"
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)             # <<<<<<<<<<<<<<
  *         cdef PyObject **dictptr "dictptr"
  *         cdef PyObject *v "v"
  */
   tp = Py_TYPE(op);
 
-  /* "recordclass/dataobject.pyx":459
+  /* "recordclass/dataobject.pyx":449
  *         cdef dict vv "vv"
  * 
  *         n = dataobject_len(op)             # <<<<<<<<<<<<<<
  *         items = dataobject_items(op)
  * 
  */
   n = dataobject_len(op);
 
-  /* "recordclass/dataobject.pyx":460
+  /* "recordclass/dataobject.pyx":450
  * 
  *         n = dataobject_len(op)
  *         items = dataobject_items(op)             # <<<<<<<<<<<<<<
  * 
- *         if type(args) is tuple:
+ *         if Py_TYPE(<PyObject*>args) == &PyTuple_Type:
  */
   items = dataobject_items(op);
 
-  /* "recordclass/dataobject.pyx":462
+  /* "recordclass/dataobject.pyx":452
  *         items = dataobject_items(op)
  * 
- *         if type(args) is tuple:             # <<<<<<<<<<<<<<
+ *         if Py_TYPE(<PyObject*>args) == &PyTuple_Type:             # <<<<<<<<<<<<<<
  *             t = args
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_v_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__pyx_t_1 == ((PyObject *)(&PyTuple_Type)));
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_1 = ((Py_TYPE(((PyObject *)__pyx_v_args)) == (&PyTuple_Type)) != 0);
+  if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":463
+    /* "recordclass/dataobject.pyx":453
  * 
- *         if type(args) is tuple:
+ *         if Py_TYPE(<PyObject*>args) == &PyTuple_Type:
  *             t = args             # <<<<<<<<<<<<<<
  *         else:
  *             t = tuple(args)
  */
     __Pyx_INCREF(__pyx_v_args);
     t = __pyx_v_args;
 
-    /* "recordclass/dataobject.pyx":462
+    /* "recordclass/dataobject.pyx":452
  *         items = dataobject_items(op)
  * 
- *         if type(args) is tuple:             # <<<<<<<<<<<<<<
+ *         if Py_TYPE(<PyObject*>args) == &PyTuple_Type:             # <<<<<<<<<<<<<<
  *             t = args
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "recordclass/dataobject.pyx":465
+  /* "recordclass/dataobject.pyx":455
  *             t = args
  *         else:
  *             t = tuple(args)             # <<<<<<<<<<<<<<
  * 
- *         if n != len(t):
+ *         if n != Py_SIZE(<PyObject*>t):
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_args);
     t = __pyx_v_args;
   }
   __pyx_L3:;
 
-  /* "recordclass/dataobject.pyx":467
+  /* "recordclass/dataobject.pyx":457
  *             t = tuple(args)
  * 
- *         if n != len(t):             # <<<<<<<<<<<<<<
+ *         if n != Py_SIZE(<PyObject*>t):             # <<<<<<<<<<<<<<
  *             raise TypeError("Invalid length of args")
  * 
  */
-  __pyx_t_4 = PyTuple_GET_SIZE(t); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 467, __pyx_L1_error)
-  __pyx_t_3 = ((n != __pyx_t_4) != 0);
-  if (unlikely(__pyx_t_3)) {
+  __pyx_t_1 = ((n != Py_SIZE(((PyObject *)t))) != 0);
+  if (unlikely(__pyx_t_1)) {
 
-    /* "recordclass/dataobject.pyx":468
+    /* "recordclass/dataobject.pyx":458
  * 
- *         if n != len(t):
+ *         if n != Py_SIZE(<PyObject*>t):
  *             raise TypeError("Invalid length of args")             # <<<<<<<<<<<<<<
  * 
- *         if n > 0:
+ *         if n:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 458, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":467
+    /* "recordclass/dataobject.pyx":457
  *             t = tuple(args)
  * 
- *         if n != len(t):             # <<<<<<<<<<<<<<
+ *         if n != Py_SIZE(<PyObject*>t):             # <<<<<<<<<<<<<<
  *             raise TypeError("Invalid length of args")
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":470
+  /* "recordclass/dataobject.pyx":460
  *             raise TypeError("Invalid length of args")
  * 
- *         if n > 0:             # <<<<<<<<<<<<<<
- *             v = items[0]
- *             Py_XDECREF(v)
- */
-  __pyx_t_3 = ((n > 0) != 0);
-  if (__pyx_t_3) {
-
-    /* "recordclass/dataobject.pyx":471
- * 
- *         if n > 0:
- *             v = items[0]             # <<<<<<<<<<<<<<
- *             Py_XDECREF(v)
- *             for i in range(n):
- */
-    v = (items[0]);
-
-    /* "recordclass/dataobject.pyx":472
- *         if n > 0:
- *             v = items[0]
- *             Py_XDECREF(v)             # <<<<<<<<<<<<<<
+ *         if n:             # <<<<<<<<<<<<<<
  *             for i in range(n):
  *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)
  */
-    Py_XDECREF(v);
+  __pyx_t_1 = (n != 0);
+  if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":473
- *             v = items[0]
- *             Py_XDECREF(v)
+    /* "recordclass/dataobject.pyx":461
+ * 
+ *         if n:
  *             for i in range(n):             # <<<<<<<<<<<<<<
  *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)
  *                 Py_INCREF(v)
  */
-    __pyx_t_4 = n;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      i = __pyx_t_6;
+    __pyx_t_3 = n;
+    __pyx_t_4 = __pyx_t_3;
+    for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+      i = __pyx_t_5;
 
-      /* "recordclass/dataobject.pyx":474
- *             Py_XDECREF(v)
+      /* "recordclass/dataobject.pyx":462
+ *         if n:
  *             for i in range(n):
  *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)             # <<<<<<<<<<<<<<
  *                 Py_INCREF(v)
  *                 items[i] = v
  */
       v = PyTuple_GET_ITEM(((PyObject *)t), i);
 
-      /* "recordclass/dataobject.pyx":475
+      /* "recordclass/dataobject.pyx":463
  *             for i in range(n):
  *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)
  *                 Py_INCREF(v)             # <<<<<<<<<<<<<<
  *                 items[i] = v
  * 
  */
       Py_INCREF(v);
 
-      /* "recordclass/dataobject.pyx":476
+      /* "recordclass/dataobject.pyx":464
  *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)
  *                 Py_INCREF(v)
  *                 items[i] = v             # <<<<<<<<<<<<<<
  * 
- *         if tp.tp_dictoffset != 0:
+ *         if tp.tp_dictoffset:
  */
       (items[i]) = v;
     }
 
-    /* "recordclass/dataobject.pyx":470
+    /* "recordclass/dataobject.pyx":460
  *             raise TypeError("Invalid length of args")
  * 
- *         if n > 0:             # <<<<<<<<<<<<<<
- *             v = items[0]
- *             Py_XDECREF(v)
+ *         if n:             # <<<<<<<<<<<<<<
+ *             for i in range(n):
+ *                 v = PyTuple_GET_ITEM(<PyObject*>t, i)
  */
   }
 
-  /* "recordclass/dataobject.pyx":478
+  /* "recordclass/dataobject.pyx":466
  *                 items[i] = v
  * 
- *         if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
+ *         if tp.tp_dictoffset:             # <<<<<<<<<<<<<<
  *             dictptr = dataobject_dictptr(op, tp)
  *             vv = {}
  */
-  __pyx_t_3 = ((tp->tp_dictoffset != 0) != 0);
-  if (__pyx_t_3) {
+  __pyx_t_1 = (tp->tp_dictoffset != 0);
+  if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":479
+    /* "recordclass/dataobject.pyx":467
  * 
- *         if tp.tp_dictoffset != 0:
+ *         if tp.tp_dictoffset:
  *             dictptr = dataobject_dictptr(op, tp)             # <<<<<<<<<<<<<<
  *             vv = {}
  *             if kw:
  */
     dictptr = dataobject_dictptr(op, tp);
 
-    /* "recordclass/dataobject.pyx":480
- *         if tp.tp_dictoffset != 0:
+    /* "recordclass/dataobject.pyx":468
+ *         if tp.tp_dictoffset:
  *             dictptr = dataobject_dictptr(op, tp)
  *             vv = {}             # <<<<<<<<<<<<<<
  *             if kw:
  *                 vv.update(kw)
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    vv = ((PyObject*)__pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    vv = ((PyObject*)__pyx_t_2);
+    __pyx_t_2 = 0;
 
-    /* "recordclass/dataobject.pyx":481
+    /* "recordclass/dataobject.pyx":469
  *             dictptr = dataobject_dictptr(op, tp)
  *             vv = {}
  *             if kw:             # <<<<<<<<<<<<<<
  *                 vv.update(kw)
  *             Py_INCREF(<PyObject*>vv)
  */
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_kw); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 481, __pyx_L1_error)
-    if (__pyx_t_3) {
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_kw); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 469, __pyx_L1_error)
+    if (__pyx_t_1) {
 
-      /* "recordclass/dataobject.pyx":482
+      /* "recordclass/dataobject.pyx":470
  *             vv = {}
  *             if kw:
  *                 vv.update(kw)             # <<<<<<<<<<<<<<
  *             Py_INCREF(<PyObject*>vv)
  *             dictptr[0] = <PyObject*>vv
  */
-      __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, vv, __pyx_v_kw); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_2 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, vv, __pyx_v_kw); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "recordclass/dataobject.pyx":481
+      /* "recordclass/dataobject.pyx":469
  *             dictptr = dataobject_dictptr(op, tp)
  *             vv = {}
  *             if kw:             # <<<<<<<<<<<<<<
  *                 vv.update(kw)
  *             Py_INCREF(<PyObject*>vv)
  */
     }
 
-    /* "recordclass/dataobject.pyx":483
+    /* "recordclass/dataobject.pyx":471
  *             if kw:
  *                 vv.update(kw)
  *             Py_INCREF(<PyObject*>vv)             # <<<<<<<<<<<<<<
  *             dictptr[0] = <PyObject*>vv
  * 
  */
     Py_INCREF(((PyObject *)vv));
 
-    /* "recordclass/dataobject.pyx":484
+    /* "recordclass/dataobject.pyx":472
  *                 vv.update(kw)
  *             Py_INCREF(<PyObject*>vv)
  *             dictptr[0] = <PyObject*>vv             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
     (dictptr[0]) = ((PyObject *)vv);
 
-    /* "recordclass/dataobject.pyx":478
+    /* "recordclass/dataobject.pyx":466
  *                 items[i] = v
  * 
- *         if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
+ *         if tp.tp_dictoffset:             # <<<<<<<<<<<<<<
  *             dictptr = dataobject_dictptr(op, tp)
  *             vv = {}
  */
   }
 
-  /* "recordclass/dataobject.pyx":449
+  /* "recordclass/dataobject.pyx":439
  * cdef public class dataobject[object DataObject, type DataObjectType]:
  * 
  *     def __cinit__(self, *args, **kw):             # <<<<<<<<<<<<<<
  *         cdef PyObject *op "op"=<PyObject*>self
  *         cdef PyObject **items "items"
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("recordclass.dataobject.dataobject.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(t);
   __Pyx_XDECREF(vv);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":486
+/* "recordclass/dataobject.pyx":474
  *             dictptr[0] = <PyObject*>vv
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef PyObject* op "op" = <PyObject*>self
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  */
 
@@ -4292,160 +4186,160 @@
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "recordclass/dataobject.pyx":487
+  /* "recordclass/dataobject.pyx":475
  * 
  *     def __dealloc__(self):
  *         cdef PyObject* op "op" = <PyObject*>self             # <<<<<<<<<<<<<<
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  *         cdef PyObject **items "items"
  */
   op = ((PyObject *)__pyx_v_self);
 
-  /* "recordclass/dataobject.pyx":488
+  /* "recordclass/dataobject.pyx":476
  *     def __dealloc__(self):
  *         cdef PyObject* op "op" = <PyObject*>self
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)             # <<<<<<<<<<<<<<
  *         cdef PyObject **items "items"
  *         cdef PyObject *v "v"
  */
   tp = Py_TYPE(op);
 
-  /* "recordclass/dataobject.pyx":493
+  /* "recordclass/dataobject.pyx":481
  *         cdef Py_ssize_t i "i", n "n"
  * 
  *         n = dataobject_len(op)             # <<<<<<<<<<<<<<
  * 
  *         if n > 0:
  */
   n = dataobject_len(op);
 
-  /* "recordclass/dataobject.pyx":495
+  /* "recordclass/dataobject.pyx":483
  *         n = dataobject_len(op)
  * 
  *         if n > 0:             # <<<<<<<<<<<<<<
  *             items = dataobject_items(op)
  *             for i in range(0,n):
  */
   __pyx_t_1 = ((n > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":496
+    /* "recordclass/dataobject.pyx":484
  * 
  *         if n > 0:
  *             items = dataobject_items(op)             # <<<<<<<<<<<<<<
  *             for i in range(0,n):
  *                 Py_CLEAR(items[i])
  */
     items = dataobject_items(op);
 
-    /* "recordclass/dataobject.pyx":497
+    /* "recordclass/dataobject.pyx":485
  *         if n > 0:
  *             items = dataobject_items(op)
  *             for i in range(0,n):             # <<<<<<<<<<<<<<
  *                 Py_CLEAR(items[i])
  * 
  */
     __pyx_t_2 = n;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       i = __pyx_t_4;
 
-      /* "recordclass/dataobject.pyx":498
+      /* "recordclass/dataobject.pyx":486
  *             items = dataobject_items(op)
  *             for i in range(0,n):
  *                 Py_CLEAR(items[i])             # <<<<<<<<<<<<<<
  * 
  *         if tp.tp_dictoffset != 0:
  */
       Py_CLEAR((items[i]));
     }
 
-    /* "recordclass/dataobject.pyx":495
+    /* "recordclass/dataobject.pyx":483
  *         n = dataobject_len(op)
  * 
  *         if n > 0:             # <<<<<<<<<<<<<<
  *             items = dataobject_items(op)
  *             for i in range(0,n):
  */
   }
 
-  /* "recordclass/dataobject.pyx":500
+  /* "recordclass/dataobject.pyx":488
  *                 Py_CLEAR(items[i])
  * 
  *         if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *             dictptr = dataobject_dictptr(op, tp)
  *             v = dictptr[0]
  */
   __pyx_t_1 = ((tp->tp_dictoffset != 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":501
+    /* "recordclass/dataobject.pyx":489
  * 
  *         if tp.tp_dictoffset != 0:
  *             dictptr = dataobject_dictptr(op, tp)             # <<<<<<<<<<<<<<
  *             v = dictptr[0]
  *             (<dict>v).clear()
  */
     __pyx_v_dictptr = dataobject_dictptr(op, tp);
 
-    /* "recordclass/dataobject.pyx":502
+    /* "recordclass/dataobject.pyx":490
  *         if tp.tp_dictoffset != 0:
  *             dictptr = dataobject_dictptr(op, tp)
  *             v = dictptr[0]             # <<<<<<<<<<<<<<
  *             (<dict>v).clear()
  *             Py_XDECREF(<PyObject*>v)
  */
     v = (__pyx_v_dictptr[0]);
 
-    /* "recordclass/dataobject.pyx":503
+    /* "recordclass/dataobject.pyx":491
  *             dictptr = dataobject_dictptr(op, tp)
  *             v = dictptr[0]
  *             (<dict>v).clear()             # <<<<<<<<<<<<<<
  *             Py_XDECREF(<PyObject*>v)
  *             dictptr[0] = NULL
  */
     if (unlikely(((PyObject *)v) == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-      __PYX_ERR(0, 503, __pyx_L1_error)
+      __PYX_ERR(0, 491, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_Clear(((PyObject*)v)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 503, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_Clear(((PyObject*)v)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 491, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":504
+    /* "recordclass/dataobject.pyx":492
  *             v = dictptr[0]
  *             (<dict>v).clear()
  *             Py_XDECREF(<PyObject*>v)             # <<<<<<<<<<<<<<
  *             dictptr[0] = NULL
  * 
  */
     Py_XDECREF(((PyObject *)v));
 
-    /* "recordclass/dataobject.pyx":505
+    /* "recordclass/dataobject.pyx":493
  *             (<dict>v).clear()
  *             Py_XDECREF(<PyObject*>v)
  *             dictptr[0] = NULL             # <<<<<<<<<<<<<<
  * 
  * #     def __getitem__(ob, ind):
  */
     (__pyx_v_dictptr[0]) = NULL;
 
-    /* "recordclass/dataobject.pyx":500
+    /* "recordclass/dataobject.pyx":488
  *                 Py_CLEAR(items[i])
  * 
  *         if tp.tp_dictoffset != 0:             # <<<<<<<<<<<<<<
  *             dictptr = dataobject_dictptr(op, tp)
  *             v = dictptr[0]
  */
   }
 
-  /* "recordclass/dataobject.pyx":486
+  /* "recordclass/dataobject.pyx":474
  *             dictptr[0] = <PyObject*>vv
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef PyObject* op "op" = <PyObject*>self
  *         cdef PyTypeObject *tp "tp" = Py_TYPE(op)
  */
 
@@ -4453,15 +4347,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("recordclass.dataobject.dataobject.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "recordclass/dataobject.pyx":541
+/* "recordclass/dataobject.pyx":529
  * #         Py_INCREF(<PyObject*>val)
  * 
  *     def __len__(ob):             # <<<<<<<<<<<<<<
  *         return dataobject_len(<PyObject*>ob)
  * 
  */
 
@@ -4479,39 +4373,39 @@
 }
 
 static Py_ssize_t __pyx_pf_11recordclass_10dataobject_10dataobject_4__len__(struct DataObject *__pyx_v_ob) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "recordclass/dataobject.pyx":542
+  /* "recordclass/dataobject.pyx":530
  * 
  *     def __len__(ob):
  *         return dataobject_len(<PyObject*>ob)             # <<<<<<<<<<<<<<
  * 
  *     def __nonzero__(self):
  */
   __pyx_r = dataobject_len(((PyObject *)__pyx_v_ob));
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":541
+  /* "recordclass/dataobject.pyx":529
  * #         Py_INCREF(<PyObject*>val)
  * 
  *     def __len__(ob):             # <<<<<<<<<<<<<<
  *         return dataobject_len(<PyObject*>ob)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":544
+/* "recordclass/dataobject.pyx":532
  *         return dataobject_len(<PyObject*>ob)
  * 
  *     def __nonzero__(self):             # <<<<<<<<<<<<<<
  *         if dataobject_len(<PyObject*>self):
  *             return True
  */
 
@@ -4531,87 +4425,87 @@
 static int __pyx_pf_11recordclass_10dataobject_10dataobject_6__nonzero__(struct DataObject *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__nonzero__", 0);
 
-  /* "recordclass/dataobject.pyx":545
+  /* "recordclass/dataobject.pyx":533
  * 
  *     def __nonzero__(self):
  *         if dataobject_len(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return True
  *         if dataobject_hasdict(<PyObject*>self):
  */
   __pyx_t_1 = (dataobject_len(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":546
+    /* "recordclass/dataobject.pyx":534
  *     def __nonzero__(self):
  *         if dataobject_len(<PyObject*>self):
  *             return True             # <<<<<<<<<<<<<<
  *         if dataobject_hasdict(<PyObject*>self):
  *             return bool(self.__dict__)
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":545
+    /* "recordclass/dataobject.pyx":533
  * 
  *     def __nonzero__(self):
  *         if dataobject_len(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return True
  *         if dataobject_hasdict(<PyObject*>self):
  */
   }
 
-  /* "recordclass/dataobject.pyx":547
+  /* "recordclass/dataobject.pyx":535
  *         if dataobject_len(<PyObject*>self):
  *             return True
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return bool(self.__dict__)
  *         return False
  */
   __pyx_t_1 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":548
+    /* "recordclass/dataobject.pyx":536
  *             return True
  *         if dataobject_hasdict(<PyObject*>self):
  *             return bool(self.__dict__)             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = (!(!__pyx_t_1));
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":547
+    /* "recordclass/dataobject.pyx":535
  *         if dataobject_len(<PyObject*>self):
  *             return True
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return bool(self.__dict__)
  *         return False
  */
   }
 
-  /* "recordclass/dataobject.pyx":549
+  /* "recordclass/dataobject.pyx":537
  *         if dataobject_hasdict(<PyObject*>self):
  *             return bool(self.__dict__)
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     def __richcmp__(self, other, int flag):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":544
+  /* "recordclass/dataobject.pyx":532
  *         return dataobject_len(<PyObject*>ob)
  * 
  *     def __nonzero__(self):             # <<<<<<<<<<<<<<
  *         if dataobject_len(<PyObject*>self):
  *             return True
  */
 
@@ -4621,15 +4515,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.dataobject.__nonzero__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":551
+/* "recordclass/dataobject.pyx":539
  *         return False
  * 
  *     def __richcmp__(self, other, int flag):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i "i", n_self "n_self", n_other "n_other"
  *         cdef object v_self "v_self", v_other "v_other"
  */
 
@@ -4661,423 +4555,423 @@
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   PyObject *__pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   __Pyx_RefNannySetupContext("__richcmp__", 0);
 
-  /* "recordclass/dataobject.pyx":555
+  /* "recordclass/dataobject.pyx":543
  *         cdef object v_self "v_self", v_other "v_other"
  * 
  *         n_self = len(self)             # <<<<<<<<<<<<<<
  *         n_other = len(other)
  * 
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 543, __pyx_L1_error)
   n_self = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":556
+  /* "recordclass/dataobject.pyx":544
  * 
  *         n_self = len(self)
  *         n_other = len(other)             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(other, dataobject):
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_other); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 556, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_other); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 544, __pyx_L1_error)
   n_other = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":558
+  /* "recordclass/dataobject.pyx":546
  *         n_other = len(other)
  * 
  *         if not isinstance(other, dataobject):             # <<<<<<<<<<<<<<
  *             raise TypeError("Types are not comparable")
  * 
  */
   __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_11recordclass_10dataobject_dataobject); 
   __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "recordclass/dataobject.pyx":559
+    /* "recordclass/dataobject.pyx":547
  * 
  *         if not isinstance(other, dataobject):
  *             raise TypeError("Types are not comparable")             # <<<<<<<<<<<<<<
  * 
  *         if flag == 2: # ==
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 559, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 547, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 559, __pyx_L1_error)
+    __PYX_ERR(0, 547, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":558
+    /* "recordclass/dataobject.pyx":546
  *         n_other = len(other)
  * 
  *         if not isinstance(other, dataobject):             # <<<<<<<<<<<<<<
  *             raise TypeError("Types are not comparable")
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":561
+  /* "recordclass/dataobject.pyx":549
  *             raise TypeError("Types are not comparable")
  * 
  *         if flag == 2: # ==             # <<<<<<<<<<<<<<
  *             if n_self != n_other:
  *                 return False
  */
   switch (__pyx_v_flag) {
     case 2:
 
-    /* "recordclass/dataobject.pyx":562
+    /* "recordclass/dataobject.pyx":550
  * 
  *         if flag == 2: # ==
  *             if n_self != n_other:             # <<<<<<<<<<<<<<
  *                 return False
  *             for i in range(n_self):
  */
     __pyx_t_3 = ((n_self != n_other) != 0);
     if (__pyx_t_3) {
 
-      /* "recordclass/dataobject.pyx":563
+      /* "recordclass/dataobject.pyx":551
  *         if flag == 2: # ==
  *             if n_self != n_other:
  *                 return False             # <<<<<<<<<<<<<<
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_False);
       __pyx_r = Py_False;
       goto __pyx_L0;
 
-      /* "recordclass/dataobject.pyx":562
+      /* "recordclass/dataobject.pyx":550
  * 
  *         if flag == 2: # ==
  *             if n_self != n_other:             # <<<<<<<<<<<<<<
  *                 return False
  *             for i in range(n_self):
  */
     }
 
-    /* "recordclass/dataobject.pyx":564
+    /* "recordclass/dataobject.pyx":552
  *             if n_self != n_other:
  *                 return False
  *             for i in range(n_self):             # <<<<<<<<<<<<<<
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  */
     __pyx_t_1 = n_self;
     __pyx_t_5 = __pyx_t_1;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       i = __pyx_t_6;
 
-      /* "recordclass/dataobject.pyx":565
+      /* "recordclass/dataobject.pyx":553
  *                 return False
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)             # <<<<<<<<<<<<<<
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:
  */
       __pyx_t_7 = dataobject_item(((PyObject *)__pyx_v_self), i);
       __pyx_t_4 = ((PyObject *)__pyx_t_7);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_XDECREF_SET(v_self, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "recordclass/dataobject.pyx":566
+      /* "recordclass/dataobject.pyx":554
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)             # <<<<<<<<<<<<<<
  *                 if v_self != v_other:
  *                     return False
  */
       __pyx_t_7 = dataobject_item(((PyObject *)__pyx_v_other), i);
       __pyx_t_4 = ((PyObject *)__pyx_t_7);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_XDECREF_SET(v_other, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "recordclass/dataobject.pyx":567
+      /* "recordclass/dataobject.pyx":555
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:             # <<<<<<<<<<<<<<
  *                     return False
  *             if dataobject_hasdict(<PyObject*>self):
  */
-      __pyx_t_4 = PyObject_RichCompare(v_self, v_other, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
-      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(v_self, v_other, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_3) {
 
-        /* "recordclass/dataobject.pyx":568
+        /* "recordclass/dataobject.pyx":556
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:
  *                     return False             # <<<<<<<<<<<<<<
  *             if dataobject_hasdict(<PyObject*>self):
  *                 return self.__dict__ == other.__dict__
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(Py_False);
         __pyx_r = Py_False;
         goto __pyx_L0;
 
-        /* "recordclass/dataobject.pyx":567
+        /* "recordclass/dataobject.pyx":555
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:             # <<<<<<<<<<<<<<
  *                     return False
  *             if dataobject_hasdict(<PyObject*>self):
  */
       }
     }
 
-    /* "recordclass/dataobject.pyx":569
+    /* "recordclass/dataobject.pyx":557
  *                 if v_self != v_other:
  *                     return False
  *             if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *                 return self.__dict__ == other.__dict__
  *             else:
  */
     __pyx_t_3 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
     if (__pyx_t_3) {
 
-      /* "recordclass/dataobject.pyx":570
+      /* "recordclass/dataobject.pyx":558
  *                     return False
  *             if dataobject_hasdict(<PyObject*>self):
  *                 return self.__dict__ == other.__dict__             # <<<<<<<<<<<<<<
  *             else:
  *                 return True
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 570, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 570, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = PyObject_RichCompare(__pyx_t_4, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 570, __pyx_L1_error)
+      __pyx_t_9 = PyObject_RichCompare(__pyx_t_4, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_r = __pyx_t_9;
       __pyx_t_9 = 0;
       goto __pyx_L0;
 
-      /* "recordclass/dataobject.pyx":569
+      /* "recordclass/dataobject.pyx":557
  *                 if v_self != v_other:
  *                     return False
  *             if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *                 return self.__dict__ == other.__dict__
  *             else:
  */
     }
 
-    /* "recordclass/dataobject.pyx":572
+    /* "recordclass/dataobject.pyx":560
  *                 return self.__dict__ == other.__dict__
  *             else:
  *                 return True             # <<<<<<<<<<<<<<
  *         elif flag == 3: # !=
  *             if n_self != n_other:
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_True);
       __pyx_r = Py_True;
       goto __pyx_L0;
     }
 
-    /* "recordclass/dataobject.pyx":561
+    /* "recordclass/dataobject.pyx":549
  *             raise TypeError("Types are not comparable")
  * 
  *         if flag == 2: # ==             # <<<<<<<<<<<<<<
  *             if n_self != n_other:
  *                 return False
  */
     break;
     case 3:
 
-    /* "recordclass/dataobject.pyx":574
+    /* "recordclass/dataobject.pyx":562
  *                 return True
  *         elif flag == 3: # !=
  *             if n_self != n_other:             # <<<<<<<<<<<<<<
  *                 return True
  *             for i in range(n_self):
  */
     __pyx_t_3 = ((n_self != n_other) != 0);
     if (__pyx_t_3) {
 
-      /* "recordclass/dataobject.pyx":575
+      /* "recordclass/dataobject.pyx":563
  *         elif flag == 3: # !=
  *             if n_self != n_other:
  *                 return True             # <<<<<<<<<<<<<<
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_True);
       __pyx_r = Py_True;
       goto __pyx_L0;
 
-      /* "recordclass/dataobject.pyx":574
+      /* "recordclass/dataobject.pyx":562
  *                 return True
  *         elif flag == 3: # !=
  *             if n_self != n_other:             # <<<<<<<<<<<<<<
  *                 return True
  *             for i in range(n_self):
  */
     }
 
-    /* "recordclass/dataobject.pyx":576
+    /* "recordclass/dataobject.pyx":564
  *             if n_self != n_other:
  *                 return True
  *             for i in range(n_self):             # <<<<<<<<<<<<<<
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  */
     __pyx_t_1 = n_self;
     __pyx_t_5 = __pyx_t_1;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       i = __pyx_t_6;
 
-      /* "recordclass/dataobject.pyx":577
+      /* "recordclass/dataobject.pyx":565
  *                 return True
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)             # <<<<<<<<<<<<<<
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:
  */
       __pyx_t_7 = dataobject_item(((PyObject *)__pyx_v_self), i);
       __pyx_t_9 = ((PyObject *)__pyx_t_7);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_XDECREF_SET(v_self, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "recordclass/dataobject.pyx":578
+      /* "recordclass/dataobject.pyx":566
  *             for i in range(n_self):
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)             # <<<<<<<<<<<<<<
  *                 if v_self != v_other:
  *                     return True
  */
       __pyx_t_7 = dataobject_item(((PyObject *)__pyx_v_other), i);
       __pyx_t_9 = ((PyObject *)__pyx_t_7);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_XDECREF_SET(v_other, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "recordclass/dataobject.pyx":579
+      /* "recordclass/dataobject.pyx":567
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:             # <<<<<<<<<<<<<<
  *                     return True
  *             if dataobject_hasdict(<PyObject*>self):
  */
-      __pyx_t_9 = PyObject_RichCompare(v_self, v_other, Py_NE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 579, __pyx_L1_error)
-      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 579, __pyx_L1_error)
+      __pyx_t_9 = PyObject_RichCompare(v_self, v_other, Py_NE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 567, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (__pyx_t_3) {
 
-        /* "recordclass/dataobject.pyx":580
+        /* "recordclass/dataobject.pyx":568
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:
  *                     return True             # <<<<<<<<<<<<<<
  *             if dataobject_hasdict(<PyObject*>self):
  *                 return self.__dict__ != other.__dict__
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(Py_True);
         __pyx_r = Py_True;
         goto __pyx_L0;
 
-        /* "recordclass/dataobject.pyx":579
+        /* "recordclass/dataobject.pyx":567
  *                 v_self = <object>dataobject_item(<PyObject*>self, i)
  *                 v_other = <object>dataobject_item(<PyObject*>other, i)
  *                 if v_self != v_other:             # <<<<<<<<<<<<<<
  *                     return True
  *             if dataobject_hasdict(<PyObject*>self):
  */
       }
     }
 
-    /* "recordclass/dataobject.pyx":581
+    /* "recordclass/dataobject.pyx":569
  *                 if v_self != v_other:
  *                     return True
  *             if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *                 return self.__dict__ != other.__dict__
  *             else:
  */
     __pyx_t_3 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
     if (__pyx_t_3) {
 
-      /* "recordclass/dataobject.pyx":582
+      /* "recordclass/dataobject.pyx":570
  *                     return True
  *             if dataobject_hasdict(<PyObject*>self):
  *                 return self.__dict__ != other.__dict__             # <<<<<<<<<<<<<<
  *             else:
  *                 return False
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 582, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 570, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 582, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 570, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_9, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_t_9, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 570, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L0;
 
-      /* "recordclass/dataobject.pyx":581
+      /* "recordclass/dataobject.pyx":569
  *                 if v_self != v_other:
  *                     return True
  *             if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *                 return self.__dict__ != other.__dict__
  *             else:
  */
     }
 
-    /* "recordclass/dataobject.pyx":584
+    /* "recordclass/dataobject.pyx":572
  *                 return self.__dict__ != other.__dict__
  *             else:
  *                 return False             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError('The type support only != and ==')
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_False);
       __pyx_r = Py_False;
       goto __pyx_L0;
     }
 
-    /* "recordclass/dataobject.pyx":573
+    /* "recordclass/dataobject.pyx":561
  *             else:
  *                 return True
  *         elif flag == 3: # !=             # <<<<<<<<<<<<<<
  *             if n_self != n_other:
  *                 return True
  */
     break;
     default:
 
-    /* "recordclass/dataobject.pyx":586
+    /* "recordclass/dataobject.pyx":574
  *                 return False
  *         else:
  *             raise TypeError('The type support only != and ==')             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 586, __pyx_L1_error)
+    __PYX_ERR(0, 574, __pyx_L1_error)
     break;
   }
 
-  /* "recordclass/dataobject.pyx":551
+  /* "recordclass/dataobject.pyx":539
  *         return False
  * 
  *     def __richcmp__(self, other, int flag):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i "i", n_self "n_self", n_other "n_other"
  *         cdef object v_self "v_self", v_other "v_other"
  */
 
@@ -5092,15 +4986,15 @@
   __Pyx_XDECREF(v_self);
   __Pyx_XDECREF(v_other);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":588
+/* "recordclass/dataobject.pyx":576
  *             raise TypeError('The type support only != and ==')
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return dataobjectiter(self)
  * 
  */
 
@@ -5119,29 +5013,29 @@
 
 static PyObject *__pyx_pf_11recordclass_10dataobject_10dataobject_10__iter__(struct DataObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "recordclass/dataobject.pyx":589
+  /* "recordclass/dataobject.pyx":577
  * 
  *     def __iter__(self):
  *         return dataobjectiter(self)             # <<<<<<<<<<<<<<
  * 
  *     def __getstate__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectiter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectiter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":588
+  /* "recordclass/dataobject.pyx":576
  *             raise TypeError('The type support only != and ==')
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return dataobjectiter(self)
  * 
  */
 
@@ -5152,15 +5046,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":591
+/* "recordclass/dataobject.pyx":579
  *         return dataobjectiter(self)
  * 
  *     def __getstate__(self):             # <<<<<<<<<<<<<<
  *         'Exclude the OrderedDict from pickling'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5181,61 +5075,61 @@
 static PyObject *__pyx_pf_11recordclass_10dataobject_10dataobject_12__getstate__(struct DataObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__getstate__", 0);
 
-  /* "recordclass/dataobject.pyx":593
+  /* "recordclass/dataobject.pyx":581
  *     def __getstate__(self):
  *         'Exclude the OrderedDict from pickling'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return self.__dict__
  *         else:
  */
   __pyx_t_1 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":594
+    /* "recordclass/dataobject.pyx":582
  *         'Exclude the OrderedDict from pickling'
  *         if dataobject_hasdict(<PyObject*>self):
  *             return self.__dict__             # <<<<<<<<<<<<<<
  *         else:
  *             return None
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":593
+    /* "recordclass/dataobject.pyx":581
  *     def __getstate__(self):
  *         'Exclude the OrderedDict from pickling'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return self.__dict__
  *         else:
  */
   }
 
-  /* "recordclass/dataobject.pyx":596
+  /* "recordclass/dataobject.pyx":584
  *             return self.__dict__
  *         else:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *     def __setstate__(self, state):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "recordclass/dataobject.pyx":591
+  /* "recordclass/dataobject.pyx":579
  *         return dataobjectiter(self)
  * 
  *     def __getstate__(self):             # <<<<<<<<<<<<<<
  *         'Exclude the OrderedDict from pickling'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5246,15 +5140,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":598
+/* "recordclass/dataobject.pyx":586
  *             return None
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         'Update __dict__ if that exists'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5277,63 +5171,63 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("__setstate__", 0);
 
-  /* "recordclass/dataobject.pyx":600
+  /* "recordclass/dataobject.pyx":588
  *     def __setstate__(self, state):
  *         'Update __dict__ if that exists'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             self.__dict__.update(state)
  * 
  */
   __pyx_t_1 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":601
+    /* "recordclass/dataobject.pyx":589
  *         'Update __dict__ if that exists'
  *         if dataobject_hasdict(<PyObject*>self):
  *             self.__dict__.update(state)             # <<<<<<<<<<<<<<
  * 
  *     def __getnewargs__(self):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_update); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 601, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_update); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_state);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "recordclass/dataobject.pyx":600
+    /* "recordclass/dataobject.pyx":588
  *     def __setstate__(self, state):
  *         'Update __dict__ if that exists'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             self.__dict__.update(state)
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":598
+  /* "recordclass/dataobject.pyx":586
  *             return None
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         'Update __dict__ if that exists'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5348,15 +5242,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":603
+/* "recordclass/dataobject.pyx":591
  *             self.__dict__.update(state)
  * 
  *     def __getnewargs__(self):             # <<<<<<<<<<<<<<
  *         'Return self as a plain tuple.  Used by copy and pickle.'
  *         return tuple(self)
  */
 
@@ -5376,29 +5270,29 @@
 
 static PyObject *__pyx_pf_11recordclass_10dataobject_10dataobject_16__getnewargs__(struct DataObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__getnewargs__", 0);
 
-  /* "recordclass/dataobject.pyx":605
+  /* "recordclass/dataobject.pyx":593
  *     def __getnewargs__(self):
  *         'Return self as a plain tuple.  Used by copy and pickle.'
  *         return tuple(self)             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_1 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":603
+  /* "recordclass/dataobject.pyx":591
  *             self.__dict__.update(state)
  * 
  *     def __getnewargs__(self):             # <<<<<<<<<<<<<<
  *         'Return self as a plain tuple.  Used by copy and pickle.'
  *         return tuple(self)
  */
 
@@ -5409,15 +5303,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":607
+/* "recordclass/dataobject.pyx":595
  *         return tuple(self)
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         'Reduce'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5441,89 +5335,89 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
-  /* "recordclass/dataobject.pyx":609
+  /* "recordclass/dataobject.pyx":597
  *     def __reduce__(self):
  *         'Reduce'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return type(self), tuple(self), self.__dict__
  *         else:
  */
   __pyx_t_1 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":610
+    /* "recordclass/dataobject.pyx":598
  *         'Reduce'
  *         if dataobject_hasdict(<PyObject*>self):
  *             return type(self), tuple(self), self.__dict__             # <<<<<<<<<<<<<<
  *         else:
  *             return type(self), tuple(self)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
+    __pyx_t_3 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 610, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":609
+    /* "recordclass/dataobject.pyx":597
  *     def __reduce__(self):
  *         'Reduce'
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             return type(self), tuple(self), self.__dict__
  *         else:
  */
   }
 
-  /* "recordclass/dataobject.pyx":612
+  /* "recordclass/dataobject.pyx":600
  *             return type(self), tuple(self), self.__dict__
  *         else:
  *             return type(self), tuple(self)             # <<<<<<<<<<<<<<
  * 
  *     def __copy__(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_4 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "recordclass/dataobject.pyx":607
+  /* "recordclass/dataobject.pyx":595
  *         return tuple(self)
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         'Reduce'
  *         if dataobject_hasdict(<PyObject*>self):
  */
 
@@ -5537,15 +5431,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":614
+/* "recordclass/dataobject.pyx":602
  *             return type(self), tuple(self)
  * 
  *     def __copy__(self):             # <<<<<<<<<<<<<<
  *         cdef object args "args"
  *         cdef object ob "ob"
  */
 
@@ -5571,108 +5465,108 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__copy__", 0);
 
-  /* "recordclass/dataobject.pyx":618
+  /* "recordclass/dataobject.pyx":606
  *         cdef object ob "ob"
  * 
  *         args = tuple(self)             # <<<<<<<<<<<<<<
  *         ob = self.__class__(*args)
  *         if dataobject_hasdict(<PyObject*>self):
  */
-  __pyx_t_1 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
+  __pyx_t_1 = PySequence_Tuple(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   args = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":619
+  /* "recordclass/dataobject.pyx":607
  * 
  *         args = tuple(self)
  *         ob = self.__class__(*args)             # <<<<<<<<<<<<<<
  *         if dataobject_hasdict(<PyObject*>self):
  *             ob.__dict__.update(self.__dict__)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PySequence_Tuple(args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PySequence_Tuple(args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   ob = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "recordclass/dataobject.pyx":620
+  /* "recordclass/dataobject.pyx":608
  *         args = tuple(self)
  *         ob = self.__class__(*args)
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             ob.__dict__.update(self.__dict__)
  *         return ob
  */
   __pyx_t_4 = (dataobject_hasdict(((PyObject *)__pyx_v_self)) != 0);
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":621
+    /* "recordclass/dataobject.pyx":609
  *         ob = self.__class__(*args)
  *         if dataobject_hasdict(<PyObject*>self):
  *             ob.__dict__.update(self.__dict__)             # <<<<<<<<<<<<<<
  *         return ob
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(ob, __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(ob, __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_update); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_update); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "recordclass/dataobject.pyx":620
+    /* "recordclass/dataobject.pyx":608
  *         args = tuple(self)
  *         ob = self.__class__(*args)
  *         if dataobject_hasdict(<PyObject*>self):             # <<<<<<<<<<<<<<
  *             ob.__dict__.update(self.__dict__)
  *         return ob
  */
   }
 
-  /* "recordclass/dataobject.pyx":622
+  /* "recordclass/dataobject.pyx":610
  *         if dataobject_hasdict(<PyObject*>self):
  *             ob.__dict__.update(self.__dict__)
  *         return ob             # <<<<<<<<<<<<<<
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(ob);
   __pyx_r = ob;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":614
+  /* "recordclass/dataobject.pyx":602
  *             return type(self), tuple(self)
  * 
  *     def __copy__(self):             # <<<<<<<<<<<<<<
  *         cdef object args "args"
  *         cdef object ob "ob"
  */
 
@@ -5689,15 +5583,15 @@
   __Pyx_XDECREF(ob);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_11recordclass_10dataobject_21_type_configure_basic_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "recordclass/dataobject.pyx":633
+/* "recordclass/dataobject.pyx":621
  * 
  *     if tp.tp_bases:
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)             # <<<<<<<<<<<<<<
  *     else:
  *         all_AC = False
  */
 
@@ -5706,23 +5600,23 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct_1_genexpr *)__pyx_tp_new_11recordclass_10dataobject___pyx_scope_struct_1_genexpr(__pyx_ptype_11recordclass_10dataobject___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 633, __pyx_L1_error)
+    __PYX_ERR(0, 621, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11recordclass_10dataobject_21_type_configure_basic_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_type_configure_basic_locals_gen, __pyx_n_s_recordclass_dataobject); if (unlikely(!gen)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11recordclass_10dataobject_21_type_configure_basic_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_type_configure_basic_locals_gen, __pyx_n_s_recordclass_dataobject); if (unlikely(!gen)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5749,49 +5643,49 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 633, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 621, __pyx_L1_error)
   if (likely(PyList_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->tp->tp_bases))) || PyTuple_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->tp->tp_bases))) {
     __pyx_t_1 = ((PyObject *)__pyx_cur_scope->__pyx_outer_scope->tp->tp_bases); __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->tp->tp_bases)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->tp->tp_bases)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 633, __pyx_L1_error)
+          else __PYX_ERR(0, 621, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_c);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_4);
@@ -5830,26 +5724,26 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":624
+/* "recordclass/dataobject.pyx":612
  *         return ob
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,             # <<<<<<<<<<<<<<
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  */
 
 static PyObject *_type_configure_basic(PyObject *__pyx_v_ob, PyObject *__pyx_v_n, struct __pyx_opt_args_11recordclass_10dataobject__type_configure_basic *__pyx_optional_args) {
   struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic *__pyx_cur_scope;
 
-  /* "recordclass/dataobject.pyx":625
+  /* "recordclass/dataobject.pyx":613
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,
  *             usedict=False, gc=False, weakref=False, hashable=False):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  *     cdef Py_ssize_t size "size" = PyNumber_AsSsize_t(<PyObject*>n, <PyObject*>PyExc_IndexError)
  */
   PyObject *__pyx_v_usedict = ((PyObject *)Py_False);
@@ -5867,15 +5761,15 @@
   int __pyx_t_5;
   int __pyx_t_6;
   __Pyx_RefNannySetupContext("_type_configure_basic", 0);
   __pyx_cur_scope = (struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic *)__pyx_tp_new_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic(__pyx_ptype_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 624, __pyx_L1_error)
+    __PYX_ERR(0, 612, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_usedict = __pyx_optional_args->usedict;
       if (__pyx_optional_args->__pyx_n > 1) {
@@ -5886,355 +5780,355 @@
             __pyx_v_hashable = __pyx_optional_args->hashable;
           }
         }
       }
     }
   }
 
-  /* "recordclass/dataobject.pyx":626
+  /* "recordclass/dataobject.pyx":614
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t size "size" = PyNumber_AsSsize_t(<PyObject*>n, <PyObject*>PyExc_IndexError)
  * 
  */
   __pyx_cur_scope->tp = ((PyTypeObject *)__pyx_v_ob);
 
-  /* "recordclass/dataobject.pyx":627
+  /* "recordclass/dataobject.pyx":615
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  *     cdef Py_ssize_t size "size" = PyNumber_AsSsize_t(<PyObject*>n, <PyObject*>PyExc_IndexError)             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_basicsize = size * sizeof(PyObject*) + sizeof(PyObject)
  */
-  __pyx_t_1 = PyNumber_AsSsize_t(((PyObject *)__pyx_v_n), ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_AsSsize_t(((PyObject *)__pyx_v_n), ((PyObject *)PyExc_IndexError)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L) && PyErr_Occurred())) __PYX_ERR(0, 615, __pyx_L1_error)
   size = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":629
+  /* "recordclass/dataobject.pyx":617
  *     cdef Py_ssize_t size "size" = PyNumber_AsSsize_t(<PyObject*>n, <PyObject*>PyExc_IndexError)
  * 
  *     tp.tp_basicsize = size * sizeof(PyObject*) + sizeof(PyObject)             # <<<<<<<<<<<<<<
  *     tp.tp_itemsize = 0
  * 
  */
   __pyx_cur_scope->tp->tp_basicsize = ((size * (sizeof(PyObject *))) + (sizeof(PyObject)));
 
-  /* "recordclass/dataobject.pyx":630
+  /* "recordclass/dataobject.pyx":618
  * 
  *     tp.tp_basicsize = size * sizeof(PyObject*) + sizeof(PyObject)
  *     tp.tp_itemsize = 0             # <<<<<<<<<<<<<<
  * 
  *     if tp.tp_bases:
  */
   __pyx_cur_scope->tp->tp_itemsize = 0;
 
-  /* "recordclass/dataobject.pyx":632
+  /* "recordclass/dataobject.pyx":620
  *     tp.tp_itemsize = 0
  * 
  *     if tp.tp_bases:             # <<<<<<<<<<<<<<
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)
  *     else:
  */
   __pyx_t_2 = (__pyx_cur_scope->tp->tp_bases != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":633
+    /* "recordclass/dataobject.pyx":621
  * 
  *     if tp.tp_bases:
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)             # <<<<<<<<<<<<<<
  *     else:
  *         all_AC = False
  */
-    __pyx_t_3 = __pyx_pf_11recordclass_10dataobject_21_type_configure_basic_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_11recordclass_10dataobject_21_type_configure_basic_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_Generator_Next(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Generator_Next(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_all_AC = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "recordclass/dataobject.pyx":632
+    /* "recordclass/dataobject.pyx":620
  *     tp.tp_itemsize = 0
  * 
  *     if tp.tp_bases:             # <<<<<<<<<<<<<<
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "recordclass/dataobject.pyx":635
+  /* "recordclass/dataobject.pyx":623
  *         all_AC = all(c is dataobject for c in <object>tp.tp_bases)
  *     else:
  *         all_AC = False             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_dictoffset = 0
  */
   /*else*/ {
     __Pyx_INCREF(Py_False);
     __pyx_v_all_AC = Py_False;
   }
   __pyx_L3:;
 
-  /* "recordclass/dataobject.pyx":637
+  /* "recordclass/dataobject.pyx":625
  *         all_AC = False
  * 
  *     tp.tp_dictoffset = 0             # <<<<<<<<<<<<<<
  *     if usedict or not all_AC:
  *         tp.tp_dictoffset = tp.tp_basicsize
  */
   __pyx_cur_scope->tp->tp_dictoffset = 0;
 
-  /* "recordclass/dataobject.pyx":638
+  /* "recordclass/dataobject.pyx":626
  * 
  *     tp.tp_dictoffset = 0
  *     if usedict or not all_AC:             # <<<<<<<<<<<<<<
  *         tp.tp_dictoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_usedict); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_usedict); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 626, __pyx_L1_error)
   if (!__pyx_t_5) {
   } else {
     __pyx_t_2 = __pyx_t_5;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_all_AC); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_all_AC); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 626, __pyx_L1_error)
   __pyx_t_6 = ((!__pyx_t_5) != 0);
   __pyx_t_2 = __pyx_t_6;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":639
+    /* "recordclass/dataobject.pyx":627
  *     tp.tp_dictoffset = 0
  *     if usedict or not all_AC:
  *         tp.tp_dictoffset = tp.tp_basicsize             # <<<<<<<<<<<<<<
  *         tp.tp_basicsize += sizeof(PyObject*)
  * 
  */
     __pyx_t_1 = __pyx_cur_scope->tp->tp_basicsize;
     __pyx_cur_scope->tp->tp_dictoffset = __pyx_t_1;
 
-    /* "recordclass/dataobject.pyx":640
+    /* "recordclass/dataobject.pyx":628
  *     if usedict or not all_AC:
  *         tp.tp_dictoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_weaklistoffset = 0
  */
     __pyx_cur_scope->tp->tp_basicsize = (__pyx_cur_scope->tp->tp_basicsize + (sizeof(PyObject *)));
 
-    /* "recordclass/dataobject.pyx":638
+    /* "recordclass/dataobject.pyx":626
  * 
  *     tp.tp_dictoffset = 0
  *     if usedict or not all_AC:             # <<<<<<<<<<<<<<
  *         tp.tp_dictoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)
  */
   }
 
-  /* "recordclass/dataobject.pyx":642
+  /* "recordclass/dataobject.pyx":630
  *         tp.tp_basicsize += sizeof(PyObject*)
  * 
  *     tp.tp_weaklistoffset = 0             # <<<<<<<<<<<<<<
  *     if weakref:
  *         tp.tp_weaklistoffset = tp.tp_basicsize
  */
   __pyx_cur_scope->tp->tp_weaklistoffset = 0;
 
-  /* "recordclass/dataobject.pyx":643
+  /* "recordclass/dataobject.pyx":631
  * 
  *     tp.tp_weaklistoffset = 0
  *     if weakref:             # <<<<<<<<<<<<<<
  *         tp.tp_weaklistoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_weakref); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_weakref); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 631, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":644
+    /* "recordclass/dataobject.pyx":632
  *     tp.tp_weaklistoffset = 0
  *     if weakref:
  *         tp.tp_weaklistoffset = tp.tp_basicsize             # <<<<<<<<<<<<<<
  *         tp.tp_basicsize += sizeof(PyObject*)
  * 
  */
     __pyx_t_1 = __pyx_cur_scope->tp->tp_basicsize;
     __pyx_cur_scope->tp->tp_weaklistoffset = __pyx_t_1;
 
-    /* "recordclass/dataobject.pyx":645
+    /* "recordclass/dataobject.pyx":633
  *     if weakref:
  *         tp.tp_weaklistoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)             # <<<<<<<<<<<<<<
  * 
  *     if gc:
  */
     __pyx_cur_scope->tp->tp_basicsize = (__pyx_cur_scope->tp->tp_basicsize + (sizeof(PyObject *)));
 
-    /* "recordclass/dataobject.pyx":643
+    /* "recordclass/dataobject.pyx":631
  * 
  *     tp.tp_weaklistoffset = 0
  *     if weakref:             # <<<<<<<<<<<<<<
  *         tp.tp_weaklistoffset = tp.tp_basicsize
  *         tp.tp_basicsize += sizeof(PyObject*)
  */
   }
 
-  /* "recordclass/dataobject.pyx":647
+  /* "recordclass/dataobject.pyx":635
  *         tp.tp_basicsize += sizeof(PyObject*)
  * 
  *     if gc:             # <<<<<<<<<<<<<<
  *         if not tp.tp_flags & Py_TPFLAGS_HAVE_GC:
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_gc); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 647, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_gc); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 635, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":648
+    /* "recordclass/dataobject.pyx":636
  * 
  *     if gc:
  *         if not tp.tp_flags & Py_TPFLAGS_HAVE_GC:             # <<<<<<<<<<<<<<
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  *     else:
  */
     __pyx_t_2 = ((!((__pyx_cur_scope->tp->tp_flags & Py_TPFLAGS_HAVE_GC) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "recordclass/dataobject.pyx":649
+      /* "recordclass/dataobject.pyx":637
  *     if gc:
  *         if not tp.tp_flags & Py_TPFLAGS_HAVE_GC:
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC             # <<<<<<<<<<<<<<
  *     else:
  *         if tp.tp_flags & Py_TPFLAGS_HAVE_GC:
  */
       __pyx_cur_scope->tp->tp_flags = (__pyx_cur_scope->tp->tp_flags | Py_TPFLAGS_HAVE_GC);
 
-      /* "recordclass/dataobject.pyx":648
+      /* "recordclass/dataobject.pyx":636
  * 
  *     if gc:
  *         if not tp.tp_flags & Py_TPFLAGS_HAVE_GC:             # <<<<<<<<<<<<<<
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  *     else:
  */
     }
 
-    /* "recordclass/dataobject.pyx":647
+    /* "recordclass/dataobject.pyx":635
  *         tp.tp_basicsize += sizeof(PyObject*)
  * 
  *     if gc:             # <<<<<<<<<<<<<<
  *         if not tp.tp_flags & Py_TPFLAGS_HAVE_GC:
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  */
     goto __pyx_L8;
   }
 
-  /* "recordclass/dataobject.pyx":651
+  /* "recordclass/dataobject.pyx":639
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  *     else:
  *         if tp.tp_flags & Py_TPFLAGS_HAVE_GC:             # <<<<<<<<<<<<<<
  *             tp.tp_flags ^= Py_TPFLAGS_HAVE_GC
  * 
  */
   /*else*/ {
     __pyx_t_2 = ((__pyx_cur_scope->tp->tp_flags & Py_TPFLAGS_HAVE_GC) != 0);
     if (__pyx_t_2) {
 
-      /* "recordclass/dataobject.pyx":652
+      /* "recordclass/dataobject.pyx":640
  *     else:
  *         if tp.tp_flags & Py_TPFLAGS_HAVE_GC:
  *             tp.tp_flags ^= Py_TPFLAGS_HAVE_GC             # <<<<<<<<<<<<<<
  * 
  *     if hashable:
  */
       __pyx_cur_scope->tp->tp_flags = (__pyx_cur_scope->tp->tp_flags ^ Py_TPFLAGS_HAVE_GC);
 
-      /* "recordclass/dataobject.pyx":651
+      /* "recordclass/dataobject.pyx":639
  *             tp.tp_flags |= Py_TPFLAGS_HAVE_GC
  *     else:
  *         if tp.tp_flags & Py_TPFLAGS_HAVE_GC:             # <<<<<<<<<<<<<<
  *             tp.tp_flags ^= Py_TPFLAGS_HAVE_GC
  * 
  */
     }
   }
   __pyx_L8:;
 
-  /* "recordclass/dataobject.pyx":654
+  /* "recordclass/dataobject.pyx":642
  *             tp.tp_flags ^= Py_TPFLAGS_HAVE_GC
  * 
  *     if hashable:             # <<<<<<<<<<<<<<
  *         tp.tp_hash = dataobject_hash
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_hashable); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_hashable); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 642, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":655
+    /* "recordclass/dataobject.pyx":643
  * 
  *     if hashable:
  *         tp.tp_hash = dataobject_hash             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_alloc = dataobject_alloc
  */
     __pyx_cur_scope->tp->tp_hash = dataobject_hash;
 
-    /* "recordclass/dataobject.pyx":654
+    /* "recordclass/dataobject.pyx":642
  *             tp.tp_flags ^= Py_TPFLAGS_HAVE_GC
  * 
  *     if hashable:             # <<<<<<<<<<<<<<
  *         tp.tp_hash = dataobject_hash
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":657
+  /* "recordclass/dataobject.pyx":645
  *         tp.tp_hash = dataobject_hash
  * 
  *     tp.tp_alloc = dataobject_alloc             # <<<<<<<<<<<<<<
  *     #tp.tp_new = dataobject_new
  * 
  */
   __pyx_cur_scope->tp->tp_alloc = dataobject_alloc;
 
-  /* "recordclass/dataobject.pyx":660
+  /* "recordclass/dataobject.pyx":648
  *     #tp.tp_new = dataobject_new
  * 
  *     tp.tp_traverse = dataobject_traverse             # <<<<<<<<<<<<<<
  *     tp.tp_clear = dataobject_clear
  * 
  */
   __pyx_cur_scope->tp->tp_traverse = dataobject_traverse;
 
-  /* "recordclass/dataobject.pyx":661
+  /* "recordclass/dataobject.pyx":649
  * 
  *     tp.tp_traverse = dataobject_traverse
  *     tp.tp_clear = dataobject_clear             # <<<<<<<<<<<<<<
  * 
  *     #tp.tp_dealloc = dataobject_dealloc
  */
   __pyx_cur_scope->tp->tp_clear = dataobject_clear;
 
-  /* "recordclass/dataobject.pyx":664
+  /* "recordclass/dataobject.pyx":652
  * 
  *     #tp.tp_dealloc = dataobject_dealloc
  *     tp.tp_free = dataobject_free             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_init = NULL
  */
   __pyx_cur_scope->tp->tp_free = dataobject_free;
 
-  /* "recordclass/dataobject.pyx":666
+  /* "recordclass/dataobject.pyx":654
  *     tp.tp_free = dataobject_free
  * 
  *     tp.tp_init = NULL             # <<<<<<<<<<<<<<
  * 
  * cdef _type_configure_getsetitem "_type_configure_getsetitem"(ob, readonly=False):
  */
   __pyx_cur_scope->tp->tp_init = NULL;
 
-  /* "recordclass/dataobject.pyx":624
+  /* "recordclass/dataobject.pyx":612
  *         return ob
  * 
  * cdef _type_configure_basic "_type_configure_basic"(ob, n,             # <<<<<<<<<<<<<<
  *             usedict=False, gc=False, weakref=False, hashable=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  */
 
@@ -6250,15 +6144,15 @@
   __Pyx_XDECREF(__pyx_v_all_AC);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":668
+/* "recordclass/dataobject.pyx":656
  *     tp.tp_init = NULL
  * 
  * cdef _type_configure_getsetitem "_type_configure_getsetitem"(ob, readonly=False):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  * 
  */
 
@@ -6271,124 +6165,124 @@
   __Pyx_RefNannySetupContext("_type_configure_getsetitem", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_readonly = __pyx_optional_args->readonly;
     }
   }
 
-  /* "recordclass/dataobject.pyx":669
+  /* "recordclass/dataobject.pyx":657
  * 
  * cdef _type_configure_getsetitem "_type_configure_getsetitem"(ob, readonly=False):
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_as_sequence.sq_item = dataobject_item
  */
   tp = ((PyTypeObject *)__pyx_v_ob);
 
-  /* "recordclass/dataobject.pyx":671
+  /* "recordclass/dataobject.pyx":659
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  * 
  *     tp.tp_as_sequence.sq_item = dataobject_item             # <<<<<<<<<<<<<<
  *     if readonly:
  *        tp.tp_as_sequence.sq_ass_item = NULL
  */
   tp->tp_as_sequence->sq_item = dataobject_item;
 
-  /* "recordclass/dataobject.pyx":672
+  /* "recordclass/dataobject.pyx":660
  * 
  *     tp.tp_as_sequence.sq_item = dataobject_item
  *     if readonly:             # <<<<<<<<<<<<<<
  *        tp.tp_as_sequence.sq_ass_item = NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_readonly); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 672, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_readonly); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 660, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":673
+    /* "recordclass/dataobject.pyx":661
  *     tp.tp_as_sequence.sq_item = dataobject_item
  *     if readonly:
  *        tp.tp_as_sequence.sq_ass_item = NULL             # <<<<<<<<<<<<<<
  *     else:
  *        tp.tp_as_sequence.sq_ass_item = dataobject_ass_item
  */
     tp->tp_as_sequence->sq_ass_item = NULL;
 
-    /* "recordclass/dataobject.pyx":672
+    /* "recordclass/dataobject.pyx":660
  * 
  *     tp.tp_as_sequence.sq_item = dataobject_item
  *     if readonly:             # <<<<<<<<<<<<<<
  *        tp.tp_as_sequence.sq_ass_item = NULL
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "recordclass/dataobject.pyx":675
+  /* "recordclass/dataobject.pyx":663
  *        tp.tp_as_sequence.sq_ass_item = NULL
  *     else:
  *        tp.tp_as_sequence.sq_ass_item = dataobject_ass_item             # <<<<<<<<<<<<<<
  * 
  *     tp.tp_as_mapping.mp_subscript = dataobject_subscript
  */
   /*else*/ {
     tp->tp_as_sequence->sq_ass_item = dataobject_ass_item;
   }
   __pyx_L3:;
 
-  /* "recordclass/dataobject.pyx":677
+  /* "recordclass/dataobject.pyx":665
  *        tp.tp_as_sequence.sq_ass_item = dataobject_ass_item
  * 
  *     tp.tp_as_mapping.mp_subscript = dataobject_subscript             # <<<<<<<<<<<<<<
  *     if readonly:
  *        tp.tp_as_mapping.mp_ass_subscript = NULL
  */
   tp->tp_as_mapping->mp_subscript = dataobject_subscript;
 
-  /* "recordclass/dataobject.pyx":678
+  /* "recordclass/dataobject.pyx":666
  * 
  *     tp.tp_as_mapping.mp_subscript = dataobject_subscript
  *     if readonly:             # <<<<<<<<<<<<<<
  *        tp.tp_as_mapping.mp_ass_subscript = NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_readonly); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_readonly); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 666, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":679
+    /* "recordclass/dataobject.pyx":667
  *     tp.tp_as_mapping.mp_subscript = dataobject_subscript
  *     if readonly:
  *        tp.tp_as_mapping.mp_ass_subscript = NULL             # <<<<<<<<<<<<<<
  *     else:
  *        tp.tp_as_mapping.mp_ass_subscript = dataobject_ass_subscript
  */
     tp->tp_as_mapping->mp_ass_subscript = NULL;
 
-    /* "recordclass/dataobject.pyx":678
+    /* "recordclass/dataobject.pyx":666
  * 
  *     tp.tp_as_mapping.mp_subscript = dataobject_subscript
  *     if readonly:             # <<<<<<<<<<<<<<
  *        tp.tp_as_mapping.mp_ass_subscript = NULL
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "recordclass/dataobject.pyx":681
+  /* "recordclass/dataobject.pyx":669
  *        tp.tp_as_mapping.mp_ass_subscript = NULL
  *     else:
  *        tp.tp_as_mapping.mp_ass_subscript = dataobject_ass_subscript             # <<<<<<<<<<<<<<
  * 
  * cdef dict slotsgetset_cache "slotsgetset_cache" = {}
  */
   /*else*/ {
     tp->tp_as_mapping->mp_ass_subscript = dataobject_ass_subscript;
   }
   __pyx_L4:;
 
-  /* "recordclass/dataobject.pyx":668
+  /* "recordclass/dataobject.pyx":656
  *     tp.tp_init = NULL
  * 
  * cdef _type_configure_getsetitem "_type_configure_getsetitem"(ob, readonly=False):             # <<<<<<<<<<<<<<
  *     cdef PyTypeObject *tp "tp" = <PyTypeObject*>ob;
  * 
  */
 
@@ -6400,15 +6294,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":688
+/* "recordclass/dataobject.pyx":676
  * class structclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
 
@@ -6447,31 +6341,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 1); __PYX_ERR(0, 688, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 1); __PYX_ERR(0, 676, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 2); __PYX_ERR(0, 688, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 2); __PYX_ERR(0, 676, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ns)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 3); __PYX_ERR(0, 688, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 3); __PYX_ERR(0, 676, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(0, 688, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(0, 676, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -6480,15 +6374,15 @@
     __pyx_v_tp = values[0];
     __pyx_v_name = values[1];
     __pyx_v_bases = values[2];
     __pyx_v_ns = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 688, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 676, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.structclasstype.__new__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_15structclasstype___new__(__pyx_self, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns);
 
@@ -6533,24 +6427,24 @@
   PyObject *(*__pyx_t_15)(PyObject *);
   PyObject *__pyx_t_16 = NULL;
   struct __pyx_opt_args_11recordclass_10dataobject__type_configure_basic __pyx_t_17;
   struct __pyx_opt_args_11recordclass_10dataobject__type_configure_getsetitem __pyx_t_18;
   int __pyx_t_19;
   __Pyx_RefNannySetupContext("__new__", 0);
 
-  /* "recordclass/dataobject.pyx":704
+  /* "recordclass/dataobject.pyx":692
  *         cdef object attrname "attrname"
  * 
  *         options = ns.pop('__options__', {})             # <<<<<<<<<<<<<<
  *         readonly = options.get('readonly', False)
  *         usedict = options.get('usedict', False)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 692, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 692, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6559,146 +6453,146 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_options, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_options, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 704, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 692, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_options);
     __Pyx_GIVEREF(__pyx_n_u_options);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_n_u_options);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   options = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":705
+  /* "recordclass/dataobject.pyx":693
  * 
  *         options = ns.pop('__options__', {})
  *         readonly = options.get('readonly', False)             # <<<<<<<<<<<<<<
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   readonly = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":706
+  /* "recordclass/dataobject.pyx":694
  *         options = ns.pop('__options__', {})
  *         readonly = options.get('readonly', False)
  *         usedict = options.get('usedict', False)             # <<<<<<<<<<<<<<
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   usedict = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":707
+  /* "recordclass/dataobject.pyx":695
  *         readonly = options.get('readonly', False)
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)             # <<<<<<<<<<<<<<
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   gc = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":708
+  /* "recordclass/dataobject.pyx":696
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)             # <<<<<<<<<<<<<<
  *         hashable = options.get('hashable', True)
  *         assequence = options.get('assequence', True)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   weakref = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":709
+  /* "recordclass/dataobject.pyx":697
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)             # <<<<<<<<<<<<<<
  *         assequence = options.get('assequence', True)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   hashable = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":710
+  /* "recordclass/dataobject.pyx":698
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)
  *         assequence = options.get('assequence', True)             # <<<<<<<<<<<<<<
  * 
  *         if readonly and not hashable:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   assequence = __pyx_t_7;
 
-  /* "recordclass/dataobject.pyx":712
+  /* "recordclass/dataobject.pyx":700
  *         assequence = options.get('assequence', True)
  * 
  *         if readonly and not hashable:             # <<<<<<<<<<<<<<
  *             hashable = True
  * 
  */
   __pyx_t_8 = (readonly != 0);
@@ -6708,40 +6602,40 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_8 = ((!(hashable != 0)) != 0);
   __pyx_t_7 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_7) {
 
-    /* "recordclass/dataobject.pyx":713
+    /* "recordclass/dataobject.pyx":701
  * 
  *         if readonly and not hashable:
  *             hashable = True             # <<<<<<<<<<<<<<
  * 
  *         cls = type.__new__(tp, name, bases, ns)
  */
     hashable = 1;
 
-    /* "recordclass/dataobject.pyx":712
+    /* "recordclass/dataobject.pyx":700
  *         assequence = options.get('assequence', True)
  * 
  *         if readonly and not hashable:             # <<<<<<<<<<<<<<
  *             hashable = True
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":715
+  /* "recordclass/dataobject.pyx":703
  *             hashable = True
  * 
  *         cls = type.__new__(tp, name, bases, ns)             # <<<<<<<<<<<<<<
  * 
  *         if not hasattr(cls, "__attrs__"):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6750,29 +6644,29 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 703, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 703, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_3 = PyTuple_New(4+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 715, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(4+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 703, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_v_tp);
     __Pyx_GIVEREF(__pyx_v_tp);
     PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_5, __pyx_v_tp);
@@ -6781,149 +6675,149 @@
     PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_5, __pyx_v_name);
     __Pyx_INCREF(__pyx_v_bases);
     __Pyx_GIVEREF(__pyx_v_bases);
     PyTuple_SET_ITEM(__pyx_t_3, 2+__pyx_t_5, __pyx_v_bases);
     __Pyx_INCREF(__pyx_v_ns);
     __Pyx_GIVEREF(__pyx_v_ns);
     PyTuple_SET_ITEM(__pyx_t_3, 3+__pyx_t_5, __pyx_v_ns);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 703, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   cls = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":717
+  /* "recordclass/dataobject.pyx":705
  *         cls = type.__new__(tp, name, bases, ns)
  * 
  *         if not hasattr(cls, "__attrs__"):             # <<<<<<<<<<<<<<
  *             raise TypeError('Class is missing __attrs__')
  * 
  */
-  __pyx_t_7 = __Pyx_HasAttr(cls, __pyx_n_u_attrs); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 717, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_HasAttr(cls, __pyx_n_u_attrs); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 705, __pyx_L1_error)
   __pyx_t_8 = ((!(__pyx_t_7 != 0)) != 0);
   if (unlikely(__pyx_t_8)) {
 
-    /* "recordclass/dataobject.pyx":718
+    /* "recordclass/dataobject.pyx":706
  * 
  *         if not hasattr(cls, "__attrs__"):
  *             raise TypeError('Class is missing __attrs__')             # <<<<<<<<<<<<<<
  * 
  *         fields = cls.__attrs__
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 718, __pyx_L1_error)
+    __PYX_ERR(0, 706, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":717
+    /* "recordclass/dataobject.pyx":705
  *         cls = type.__new__(tp, name, bases, ns)
  * 
  *         if not hasattr(cls, "__attrs__"):             # <<<<<<<<<<<<<<
  *             raise TypeError('Class is missing __attrs__')
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":720
+  /* "recordclass/dataobject.pyx":708
  *             raise TypeError('Class is missing __attrs__')
  * 
  *         fields = cls.__attrs__             # <<<<<<<<<<<<<<
  *         for base in bases:
  *             if type(base) is dataobject:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(cls, __pyx_n_s_attrs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(cls, __pyx_n_s_attrs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   fields = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":721
+  /* "recordclass/dataobject.pyx":709
  * 
  *         fields = cls.__attrs__
  *         for base in bases:             # <<<<<<<<<<<<<<
  *             if type(base) is dataobject:
  *                 continue
  */
   if (likely(PyList_CheckExact(__pyx_v_bases)) || PyTuple_CheckExact(__pyx_v_bases)) {
     __pyx_t_1 = __pyx_v_bases; __Pyx_INCREF(__pyx_t_1); __pyx_t_9 = 0;
     __pyx_t_10 = NULL;
   } else {
-    __pyx_t_9 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_bases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 721, __pyx_L1_error)
+    __pyx_t_9 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_bases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_10 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 721, __pyx_L1_error)
+    __pyx_t_10 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 709, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_10)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 721, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 709, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 721, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 721, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 709, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 721, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_10(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 721, __pyx_L1_error)
+          else __PYX_ERR(0, 709, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_base, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "recordclass/dataobject.pyx":722
+    /* "recordclass/dataobject.pyx":710
  *         fields = cls.__attrs__
  *         for base in bases:
  *             if type(base) is dataobject:             # <<<<<<<<<<<<<<
  *                 continue
  *             try:
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_v_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_v_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_8 = (__pyx_t_2 == ((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobject));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = (__pyx_t_8 != 0);
     if (__pyx_t_7) {
 
-      /* "recordclass/dataobject.pyx":723
+      /* "recordclass/dataobject.pyx":711
  *         for base in bases:
  *             if type(base) is dataobject:
  *                 continue             # <<<<<<<<<<<<<<
  *             try:
  *                 base_fields = base.__attrs__
  */
       goto __pyx_L7_continue;
 
-      /* "recordclass/dataobject.pyx":722
+      /* "recordclass/dataobject.pyx":710
  *         fields = cls.__attrs__
  *         for base in bases:
  *             if type(base) is dataobject:             # <<<<<<<<<<<<<<
  *                 continue
  *             try:
  */
     }
 
-    /* "recordclass/dataobject.pyx":724
+    /* "recordclass/dataobject.pyx":712
  *             if type(base) is dataobject:
  *                 continue
  *             try:             # <<<<<<<<<<<<<<
  *                 base_fields = base.__attrs__
  *                 flag = False
  */
     {
@@ -6931,186 +6825,186 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_13);
       /*try:*/ {
 
-        /* "recordclass/dataobject.pyx":725
+        /* "recordclass/dataobject.pyx":713
  *                 continue
  *             try:
  *                 base_fields = base.__attrs__             # <<<<<<<<<<<<<<
  *                 flag = False
  *                 for f in base_fields:
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_base, __pyx_n_s_attrs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 725, __pyx_L10_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_base, __pyx_n_s_attrs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 713, __pyx_L10_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_XDECREF_SET(__pyx_v_base_fields, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "recordclass/dataobject.pyx":726
+        /* "recordclass/dataobject.pyx":714
  *             try:
  *                 base_fields = base.__attrs__
  *                 flag = False             # <<<<<<<<<<<<<<
  *                 for f in base_fields:
  *                     if f in fields:
  */
         __Pyx_INCREF(Py_False);
         __Pyx_XDECREF_SET(flag, Py_False);
 
-        /* "recordclass/dataobject.pyx":727
+        /* "recordclass/dataobject.pyx":715
  *                 base_fields = base.__attrs__
  *                 flag = False
  *                 for f in base_fields:             # <<<<<<<<<<<<<<
  *                     if f in fields:
  *                         flag = True
  */
         if (likely(PyList_CheckExact(__pyx_v_base_fields)) || PyTuple_CheckExact(__pyx_v_base_fields)) {
           __pyx_t_2 = __pyx_v_base_fields; __Pyx_INCREF(__pyx_t_2); __pyx_t_14 = 0;
           __pyx_t_15 = NULL;
         } else {
-          __pyx_t_14 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_base_fields); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L10_error)
+          __pyx_t_14 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_base_fields); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L10_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_15 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 727, __pyx_L10_error)
+          __pyx_t_15 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 715, __pyx_L10_error)
         }
         for (;;) {
           if (likely(!__pyx_t_15)) {
             if (likely(PyList_CheckExact(__pyx_t_2))) {
               if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_2)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_3); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 727, __pyx_L10_error)
+              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_3); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 715, __pyx_L10_error)
               #else
-              __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 727, __pyx_L10_error)
+              __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 715, __pyx_L10_error)
               __Pyx_GOTREF(__pyx_t_3);
               #endif
             } else {
               if (__pyx_t_14 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_3); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 727, __pyx_L10_error)
+              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_3); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 715, __pyx_L10_error)
               #else
-              __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 727, __pyx_L10_error)
+              __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 715, __pyx_L10_error)
               __Pyx_GOTREF(__pyx_t_3);
               #endif
             }
           } else {
             __pyx_t_3 = __pyx_t_15(__pyx_t_2);
             if (unlikely(!__pyx_t_3)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 727, __pyx_L10_error)
+                else __PYX_ERR(0, 715, __pyx_L10_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_3);
           }
           __Pyx_XDECREF_SET(f, __pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "recordclass/dataobject.pyx":728
+          /* "recordclass/dataobject.pyx":716
  *                 flag = False
  *                 for f in base_fields:
  *                     if f in fields:             # <<<<<<<<<<<<<<
  *                         flag = True
  *                         break
  */
-          __pyx_t_7 = (__Pyx_PySequence_ContainsTF(f, fields, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 728, __pyx_L10_error)
+          __pyx_t_7 = (__Pyx_PySequence_ContainsTF(f, fields, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 716, __pyx_L10_error)
           __pyx_t_8 = (__pyx_t_7 != 0);
           if (__pyx_t_8) {
 
-            /* "recordclass/dataobject.pyx":729
+            /* "recordclass/dataobject.pyx":717
  *                 for f in base_fields:
  *                     if f in fields:
  *                         flag = True             # <<<<<<<<<<<<<<
  *                         break
  *                 if flag:
  */
             __Pyx_INCREF(Py_True);
             __Pyx_DECREF_SET(flag, Py_True);
 
-            /* "recordclass/dataobject.pyx":730
+            /* "recordclass/dataobject.pyx":718
  *                     if f in fields:
  *                         flag = True
  *                         break             # <<<<<<<<<<<<<<
  *                 if flag:
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)
  */
             goto __pyx_L19_break;
 
-            /* "recordclass/dataobject.pyx":728
+            /* "recordclass/dataobject.pyx":716
  *                 flag = False
  *                 for f in base_fields:
  *                     if f in fields:             # <<<<<<<<<<<<<<
  *                         flag = True
  *                         break
  */
           }
 
-          /* "recordclass/dataobject.pyx":727
+          /* "recordclass/dataobject.pyx":715
  *                 base_fields = base.__attrs__
  *                 flag = False
  *                 for f in base_fields:             # <<<<<<<<<<<<<<
  *                     if f in fields:
  *                         flag = True
  */
         }
         __pyx_L19_break:;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "recordclass/dataobject.pyx":731
+        /* "recordclass/dataobject.pyx":719
  *                         flag = True
  *                         break
  *                 if flag:             # <<<<<<<<<<<<<<
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)
  *                 fields = fields + base_fields
  */
-        __pyx_t_8 = __Pyx_PyObject_IsTrue(flag); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 731, __pyx_L10_error)
+        __pyx_t_8 = __Pyx_PyObject_IsTrue(flag); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 719, __pyx_L10_error)
         if (unlikely(__pyx_t_8)) {
 
-          /* "recordclass/dataobject.pyx":732
+          /* "recordclass/dataobject.pyx":720
  *                         break
  *                 if flag:
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)             # <<<<<<<<<<<<<<
  *                 fields = fields + base_fields
  *             except AttributeError:
  */
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_base, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 732, __pyx_L10_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_base, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L10_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = PyNumber_Add(__pyx_kp_u_Duplicate_field_with_class, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 732, __pyx_L10_error)
+          __pyx_t_3 = PyNumber_Add(__pyx_kp_u_Duplicate_field_with_class, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 720, __pyx_L10_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 732, __pyx_L10_error)
+          __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L10_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_Raise(__pyx_t_2, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __PYX_ERR(0, 732, __pyx_L10_error)
+          __PYX_ERR(0, 720, __pyx_L10_error)
 
-          /* "recordclass/dataobject.pyx":731
+          /* "recordclass/dataobject.pyx":719
  *                         flag = True
  *                         break
  *                 if flag:             # <<<<<<<<<<<<<<
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)
  *                 fields = fields + base_fields
  */
         }
 
-        /* "recordclass/dataobject.pyx":733
+        /* "recordclass/dataobject.pyx":721
  *                 if flag:
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)
  *                 fields = fields + base_fields             # <<<<<<<<<<<<<<
  *             except AttributeError:
  *                 pass
  */
-        __pyx_t_2 = PyNumber_Add(fields, __pyx_v_base_fields); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 733, __pyx_L10_error)
+        __pyx_t_2 = PyNumber_Add(fields, __pyx_v_base_fields); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 721, __pyx_L10_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF_SET(fields, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "recordclass/dataobject.pyx":724
+        /* "recordclass/dataobject.pyx":712
  *             if type(base) is dataobject:
  *                 continue
  *             try:             # <<<<<<<<<<<<<<
  *                 base_fields = base.__attrs__
  *                 flag = False
  */
       }
@@ -7120,30 +7014,30 @@
       goto __pyx_L17_try_end;
       __pyx_L10_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "recordclass/dataobject.pyx":734
+      /* "recordclass/dataobject.pyx":722
  *                     raise AttributeError('Duplicate field with class ' +  base.__name__)
  *                 fields = fields + base_fields
  *             except AttributeError:             # <<<<<<<<<<<<<<
  *                 pass
  * 
  */
       __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_AttributeError);
       if (__pyx_t_5) {
         __Pyx_ErrRestore(0,0,0);
         goto __pyx_L11_exception_handled;
       }
       goto __pyx_L12_except_error;
       __pyx_L12_except_error:;
 
-      /* "recordclass/dataobject.pyx":724
+      /* "recordclass/dataobject.pyx":712
  *             if type(base) is dataobject:
  *                 continue
  *             try:             # <<<<<<<<<<<<<<
  *                 base_fields = base.__attrs__
  *                 flag = False
  */
       __Pyx_XGIVEREF(__pyx_t_11);
@@ -7155,337 +7049,337 @@
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_XGIVEREF(__pyx_t_13);
       __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
       __pyx_L17_try_end:;
     }
 
-    /* "recordclass/dataobject.pyx":721
+    /* "recordclass/dataobject.pyx":709
  * 
  *         fields = cls.__attrs__
  *         for base in bases:             # <<<<<<<<<<<<<<
  *             if type(base) is dataobject:
  *                 continue
  */
     __pyx_L7_continue:;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":737
+  /* "recordclass/dataobject.pyx":725
  *                 pass
  * 
  *         cls.__attrs__ = fields             # <<<<<<<<<<<<<<
  *         _type_configure_basic(cls, len(fields), usedict, gc, weakref, hashable)
  *         if assequence:
  */
-  if (__Pyx_PyObject_SetAttrStr(cls, __pyx_n_s_attrs, fields) < 0) __PYX_ERR(0, 737, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(cls, __pyx_n_s_attrs, fields) < 0) __PYX_ERR(0, 725, __pyx_L1_error)
 
-  /* "recordclass/dataobject.pyx":738
+  /* "recordclass/dataobject.pyx":726
  * 
  *         cls.__attrs__ = fields
  *         _type_configure_basic(cls, len(fields), usedict, gc, weakref, hashable)             # <<<<<<<<<<<<<<
  *         if assequence:
  *             _type_configure_getsetitem(cls, readonly)
  */
-  __pyx_t_9 = PyObject_Length(fields); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 738, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_9 = PyObject_Length(fields); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(usedict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(usedict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyBool_FromLong(gc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(gc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyBool_FromLong(weakref); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBool_FromLong(weakref); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyBool_FromLong(hashable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBool_FromLong(hashable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_17.__pyx_n = 4;
   __pyx_t_17.usedict = __pyx_t_2;
   __pyx_t_17.gc = __pyx_t_3;
   __pyx_t_17.weakref = __pyx_t_6;
   __pyx_t_17.hashable = __pyx_t_4;
-  __pyx_t_16 = _type_configure_basic(cls, __pyx_t_1, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_16 = _type_configure_basic(cls, __pyx_t_1, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-  /* "recordclass/dataobject.pyx":739
+  /* "recordclass/dataobject.pyx":727
  *         cls.__attrs__ = fields
  *         _type_configure_basic(cls, len(fields), usedict, gc, weakref, hashable)
  *         if assequence:             # <<<<<<<<<<<<<<
  *             _type_configure_getsetitem(cls, readonly)
  * 
  */
   __pyx_t_8 = (assequence != 0);
   if (__pyx_t_8) {
 
-    /* "recordclass/dataobject.pyx":740
+    /* "recordclass/dataobject.pyx":728
  *         _type_configure_basic(cls, len(fields), usedict, gc, weakref, hashable)
  *         if assequence:
  *             _type_configure_getsetitem(cls, readonly)             # <<<<<<<<<<<<<<
  * 
  *         for index, attrname in enumerate(fields):
  */
-    __pyx_t_16 = __Pyx_PyBool_FromLong(readonly); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 740, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyBool_FromLong(readonly); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 728, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18.__pyx_n = 1;
     __pyx_t_18.readonly = __pyx_t_16;
-    __pyx_t_4 = _type_configure_getsetitem(cls, &__pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 740, __pyx_L1_error)
+    __pyx_t_4 = _type_configure_getsetitem(cls, &__pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 728, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "recordclass/dataobject.pyx":739
+    /* "recordclass/dataobject.pyx":727
  *         cls.__attrs__ = fields
  *         _type_configure_basic(cls, len(fields), usedict, gc, weakref, hashable)
  *         if assequence:             # <<<<<<<<<<<<<<
  *             _type_configure_getsetitem(cls, readonly)
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":742
+  /* "recordclass/dataobject.pyx":730
  *             _type_configure_getsetitem(cls, readonly)
  * 
  *         for index, attrname in enumerate(fields):             # <<<<<<<<<<<<<<
  *             if readonly:
  *                 item_object = slotsget_cache.get(index, None)
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_4 = __pyx_int_0;
   if (likely(PyList_CheckExact(fields)) || PyTuple_CheckExact(fields)) {
     __pyx_t_16 = fields; __Pyx_INCREF(__pyx_t_16); __pyx_t_9 = 0;
     __pyx_t_10 = NULL;
   } else {
-    __pyx_t_9 = -1; __pyx_t_16 = PyObject_GetIter(fields); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 742, __pyx_L1_error)
+    __pyx_t_9 = -1; __pyx_t_16 = PyObject_GetIter(fields); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 730, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
-    __pyx_t_10 = Py_TYPE(__pyx_t_16)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 742, __pyx_L1_error)
+    __pyx_t_10 = Py_TYPE(__pyx_t_16)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 730, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_10)) {
       if (likely(PyList_CheckExact(__pyx_t_16))) {
         if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_16)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_16, __pyx_t_9); __Pyx_INCREF(__pyx_t_6); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 742, __pyx_L1_error)
+        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_16, __pyx_t_9); __Pyx_INCREF(__pyx_t_6); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 730, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_16, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 742, __pyx_L1_error)
+        __pyx_t_6 = PySequence_ITEM(__pyx_t_16, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 730, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       } else {
         if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_16)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_9); __Pyx_INCREF(__pyx_t_6); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 742, __pyx_L1_error)
+        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_9); __Pyx_INCREF(__pyx_t_6); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 730, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_16, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 742, __pyx_L1_error)
+        __pyx_t_6 = PySequence_ITEM(__pyx_t_16, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 730, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       }
     } else {
       __pyx_t_6 = __pyx_t_10(__pyx_t_16);
       if (unlikely(!__pyx_t_6)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 742, __pyx_L1_error)
+          else __PYX_ERR(0, 730, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_6);
     }
     __Pyx_XDECREF_SET(attrname, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_XDECREF_SET(index, __pyx_t_4);
-    __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 742, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 730, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4);
     __pyx_t_4 = __pyx_t_6;
     __pyx_t_6 = 0;
 
-    /* "recordclass/dataobject.pyx":743
+    /* "recordclass/dataobject.pyx":731
  * 
  *         for index, attrname in enumerate(fields):
  *             if readonly:             # <<<<<<<<<<<<<<
  *                 item_object = slotsget_cache.get(index, None)
  *                 if item_object is None:
  */
     __pyx_t_8 = (readonly != 0);
     if (__pyx_t_8) {
 
-      /* "recordclass/dataobject.pyx":744
+      /* "recordclass/dataobject.pyx":732
  *         for index, attrname in enumerate(fields):
  *             if readonly:
  *                 item_object = slotsget_cache.get(index, None)             # <<<<<<<<<<<<<<
  *                 if item_object is None:
  *                     item_object = dataobjectget(index)
  */
       if (unlikely(slotsget_cache == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-        __PYX_ERR(0, 744, __pyx_L1_error)
+        __PYX_ERR(0, 732, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_PyDict_GetItemDefault(slotsget_cache, index, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 744, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItemDefault(slotsget_cache, index, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 732, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(item_object, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "recordclass/dataobject.pyx":745
+      /* "recordclass/dataobject.pyx":733
  *             if readonly:
  *                 item_object = slotsget_cache.get(index, None)
  *                 if item_object is None:             # <<<<<<<<<<<<<<
  *                     item_object = dataobjectget(index)
  *                     slotsget_cache[index] = item_object
  */
       __pyx_t_8 = (item_object == Py_None);
       __pyx_t_7 = (__pyx_t_8 != 0);
       if (__pyx_t_7) {
 
-        /* "recordclass/dataobject.pyx":746
+        /* "recordclass/dataobject.pyx":734
  *                 item_object = slotsget_cache.get(index, None)
  *                 if item_object is None:
  *                     item_object = dataobjectget(index)             # <<<<<<<<<<<<<<
  *                     slotsget_cache[index] = item_object
  *             else:
  */
-        __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectget), index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 746, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectget), index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 734, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF_SET(item_object, __pyx_t_6);
         __pyx_t_6 = 0;
 
-        /* "recordclass/dataobject.pyx":747
+        /* "recordclass/dataobject.pyx":735
  *                 if item_object is None:
  *                     item_object = dataobjectget(index)
  *                     slotsget_cache[index] = item_object             # <<<<<<<<<<<<<<
  *             else:
  *                 item_object = slotsgetset_cache.get(index)
  */
         if (unlikely(slotsget_cache == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 747, __pyx_L1_error)
+          __PYX_ERR(0, 735, __pyx_L1_error)
         }
-        if (unlikely(PyDict_SetItem(slotsget_cache, index, item_object) < 0)) __PYX_ERR(0, 747, __pyx_L1_error)
+        if (unlikely(PyDict_SetItem(slotsget_cache, index, item_object) < 0)) __PYX_ERR(0, 735, __pyx_L1_error)
 
-        /* "recordclass/dataobject.pyx":745
+        /* "recordclass/dataobject.pyx":733
  *             if readonly:
  *                 item_object = slotsget_cache.get(index, None)
  *                 if item_object is None:             # <<<<<<<<<<<<<<
  *                     item_object = dataobjectget(index)
  *                     slotsget_cache[index] = item_object
  */
       }
 
-      /* "recordclass/dataobject.pyx":743
+      /* "recordclass/dataobject.pyx":731
  * 
  *         for index, attrname in enumerate(fields):
  *             if readonly:             # <<<<<<<<<<<<<<
  *                 item_object = slotsget_cache.get(index, None)
  *                 if item_object is None:
  */
       goto __pyx_L25;
     }
 
-    /* "recordclass/dataobject.pyx":749
+    /* "recordclass/dataobject.pyx":737
  *                     slotsget_cache[index] = item_object
  *             else:
  *                 item_object = slotsgetset_cache.get(index)             # <<<<<<<<<<<<<<
  *                 if item_object is None:
  *                     item_object = dataobjectgetset(index)
  */
     /*else*/ {
       if (unlikely(slotsgetset_cache == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-        __PYX_ERR(0, 749, __pyx_L1_error)
+        __PYX_ERR(0, 737, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_PyDict_GetItemDefault(slotsgetset_cache, index, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 749, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItemDefault(slotsgetset_cache, index, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 737, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(item_object, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "recordclass/dataobject.pyx":750
+      /* "recordclass/dataobject.pyx":738
  *             else:
  *                 item_object = slotsgetset_cache.get(index)
  *                 if item_object is None:             # <<<<<<<<<<<<<<
  *                     item_object = dataobjectgetset(index)
  *                     slotsgetset_cache[index] = item_object
  */
       __pyx_t_7 = (item_object == Py_None);
       __pyx_t_8 = (__pyx_t_7 != 0);
       if (__pyx_t_8) {
 
-        /* "recordclass/dataobject.pyx":751
+        /* "recordclass/dataobject.pyx":739
  *                 item_object = slotsgetset_cache.get(index)
  *                 if item_object is None:
  *                     item_object = dataobjectgetset(index)             # <<<<<<<<<<<<<<
  *                     slotsgetset_cache[index] = item_object
  *             setattr(cls, attrname, item_object)
  */
-        __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectgetset), index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 751, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_dataobjectgetset), index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 739, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF_SET(item_object, __pyx_t_6);
         __pyx_t_6 = 0;
 
-        /* "recordclass/dataobject.pyx":752
+        /* "recordclass/dataobject.pyx":740
  *                 if item_object is None:
  *                     item_object = dataobjectgetset(index)
  *                     slotsgetset_cache[index] = item_object             # <<<<<<<<<<<<<<
  *             setattr(cls, attrname, item_object)
  * 
  */
         if (unlikely(slotsgetset_cache == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 752, __pyx_L1_error)
+          __PYX_ERR(0, 740, __pyx_L1_error)
         }
-        if (unlikely(PyDict_SetItem(slotsgetset_cache, index, item_object) < 0)) __PYX_ERR(0, 752, __pyx_L1_error)
+        if (unlikely(PyDict_SetItem(slotsgetset_cache, index, item_object) < 0)) __PYX_ERR(0, 740, __pyx_L1_error)
 
-        /* "recordclass/dataobject.pyx":750
+        /* "recordclass/dataobject.pyx":738
  *             else:
  *                 item_object = slotsgetset_cache.get(index)
  *                 if item_object is None:             # <<<<<<<<<<<<<<
  *                     item_object = dataobjectgetset(index)
  *                     slotsgetset_cache[index] = item_object
  */
       }
     }
     __pyx_L25:;
 
-    /* "recordclass/dataobject.pyx":753
+    /* "recordclass/dataobject.pyx":741
  *                     item_object = dataobjectgetset(index)
  *                     slotsgetset_cache[index] = item_object
  *             setattr(cls, attrname, item_object)             # <<<<<<<<<<<<<<
  * 
  *         return cls
  */
-    __pyx_t_19 = PyObject_SetAttr(cls, attrname, item_object); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 753, __pyx_L1_error)
+    __pyx_t_19 = PyObject_SetAttr(cls, attrname, item_object); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 741, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":742
+    /* "recordclass/dataobject.pyx":730
  *             _type_configure_getsetitem(cls, readonly)
  * 
  *         for index, attrname in enumerate(fields):             # <<<<<<<<<<<<<<
  *             if readonly:
  *                 item_object = slotsget_cache.get(index, None)
  */
   }
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "recordclass/dataobject.pyx":755
+  /* "recordclass/dataobject.pyx":743
  *             setattr(cls, attrname, item_object)
  * 
  *         return cls             # <<<<<<<<<<<<<<
  * 
  * class arrayclasstype(type):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(cls);
   __pyx_r = cls;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":688
+  /* "recordclass/dataobject.pyx":676
  * class structclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
 
@@ -7511,15 +7405,15 @@
   __Pyx_XDECREF(__pyx_v_base);
   __Pyx_XDECREF(__pyx_v_base_fields);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":759
+/* "recordclass/dataobject.pyx":747
  * class arrayclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
 
@@ -7558,31 +7452,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 1); __PYX_ERR(0, 759, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 1); __PYX_ERR(0, 747, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 2); __PYX_ERR(0, 759, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 2); __PYX_ERR(0, 747, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ns)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 3); __PYX_ERR(0, 759, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, 3); __PYX_ERR(0, 747, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(0, 759, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(0, 747, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7591,15 +7485,15 @@
     __pyx_v_tp = values[0];
     __pyx_v_name = values[1];
     __pyx_v_bases = values[2];
     __pyx_v_ns = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 759, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__new__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 747, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.arrayclasstype.__new__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_14arrayclasstype___new__(__pyx_self, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns);
 
@@ -7626,132 +7520,132 @@
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   struct __pyx_opt_args_11recordclass_10dataobject__type_configure_basic __pyx_t_8;
   struct __pyx_opt_args_11recordclass_10dataobject__type_configure_getsetitem __pyx_t_9;
   __Pyx_RefNannySetupContext("__new__", 0);
 
-  /* "recordclass/dataobject.pyx":769
+  /* "recordclass/dataobject.pyx":757
  *         cdef object n "n"
  * 
  *         n = ns.pop('__size__')             # <<<<<<<<<<<<<<
  *         options = ns.pop('__options__')
  *         readonly = options['readonly']
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 769, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 757, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_size) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_size);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 769, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 757, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   n = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":770
+  /* "recordclass/dataobject.pyx":758
  * 
  *         n = ns.pop('__size__')
  *         options = ns.pop('__options__')             # <<<<<<<<<<<<<<
  *         readonly = options['readonly']
  *         usedict = options['usedict']
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ns, __pyx_n_s_pop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_options) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_options);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 770, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   options = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":771
+  /* "recordclass/dataobject.pyx":759
  *         n = ns.pop('__size__')
  *         options = ns.pop('__options__')
  *         readonly = options['readonly']             # <<<<<<<<<<<<<<
  *         usedict = options['usedict']
  *         gc = options['gc']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_readonly); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 771, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_readonly); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 771, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 759, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   readonly = __pyx_t_4;
 
-  /* "recordclass/dataobject.pyx":772
+  /* "recordclass/dataobject.pyx":760
  *         options = ns.pop('__options__')
  *         readonly = options['readonly']
  *         usedict = options['usedict']             # <<<<<<<<<<<<<<
  *         gc = options['gc']
  *         weakref = options['weakref']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_usedict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_usedict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 760, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 772, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 760, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   usedict = __pyx_t_4;
 
-  /* "recordclass/dataobject.pyx":773
+  /* "recordclass/dataobject.pyx":761
  *         readonly = options['readonly']
  *         usedict = options['usedict']
  *         gc = options['gc']             # <<<<<<<<<<<<<<
  *         weakref = options['weakref']
  *         hashable = options["hashable"]
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_gc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_gc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 761, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   gc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":774
+  /* "recordclass/dataobject.pyx":762
  *         usedict = options['usedict']
  *         gc = options['gc']
  *         weakref = options['weakref']             # <<<<<<<<<<<<<<
  *         hashable = options["hashable"]
  *         if readonly and not hashable:
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 762, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   weakref = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":775
+  /* "recordclass/dataobject.pyx":763
  *         gc = options['gc']
  *         weakref = options['weakref']
  *         hashable = options["hashable"]             # <<<<<<<<<<<<<<
  *         if readonly and not hashable:
  *             hashable = True
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_hashable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 775, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(options, __pyx_n_u_hashable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 763, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 763, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   hashable = __pyx_t_4;
 
-  /* "recordclass/dataobject.pyx":776
+  /* "recordclass/dataobject.pyx":764
  *         weakref = options['weakref']
  *         hashable = options["hashable"]
  *         if readonly and not hashable:             # <<<<<<<<<<<<<<
  *             hashable = True
  * 
  */
   __pyx_t_5 = (readonly != 0);
@@ -7761,40 +7655,40 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_5 = ((!(hashable != 0)) != 0);
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "recordclass/dataobject.pyx":777
+    /* "recordclass/dataobject.pyx":765
  *         hashable = options["hashable"]
  *         if readonly and not hashable:
  *             hashable = True             # <<<<<<<<<<<<<<
  * 
  *         cls = type.__new__(tp, name, bases, ns)
  */
     hashable = 1;
 
-    /* "recordclass/dataobject.pyx":776
+    /* "recordclass/dataobject.pyx":764
  *         weakref = options['weakref']
  *         hashable = options["hashable"]
  *         if readonly and not hashable:             # <<<<<<<<<<<<<<
  *             hashable = True
  * 
  */
   }
 
-  /* "recordclass/dataobject.pyx":779
+  /* "recordclass/dataobject.pyx":767
  *             hashable = True
  * 
  *         cls = type.__new__(tp, name, bases, ns)             # <<<<<<<<<<<<<<
  * 
  *         _type_configure_basic(cls, n, usedict, gc, weakref, hashable)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7803,29 +7697,29 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_3, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_3, __pyx_v_tp, __pyx_v_name, __pyx_v_bases, __pyx_v_ns};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_tp);
     __Pyx_GIVEREF(__pyx_v_tp);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_tp);
@@ -7834,73 +7728,73 @@
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_name);
     __Pyx_INCREF(__pyx_v_bases);
     __Pyx_GIVEREF(__pyx_v_bases);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_v_bases);
     __Pyx_INCREF(__pyx_v_ns);
     __Pyx_GIVEREF(__pyx_v_ns);
     PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_6, __pyx_v_ns);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   cls = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":781
+  /* "recordclass/dataobject.pyx":769
  *         cls = type.__new__(tp, name, bases, ns)
  * 
  *         _type_configure_basic(cls, n, usedict, gc, weakref, hashable)             # <<<<<<<<<<<<<<
  *         _type_configure_getsetitem(cls, readonly)
  * 
  */
-  __pyx_t_1 = __Pyx_PyBool_FromLong(usedict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 781, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(usedict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(hashable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 781, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(hashable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8.__pyx_n = 4;
   __pyx_t_8.usedict = __pyx_t_1;
   __pyx_t_8.gc = gc;
   __pyx_t_8.weakref = weakref;
   __pyx_t_8.hashable = __pyx_t_2;
-  __pyx_t_7 = _type_configure_basic(cls, n, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 781, __pyx_L1_error)
+  __pyx_t_7 = _type_configure_basic(cls, n, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "recordclass/dataobject.pyx":782
+  /* "recordclass/dataobject.pyx":770
  * 
  *         _type_configure_basic(cls, n, usedict, gc, weakref, hashable)
  *         _type_configure_getsetitem(cls, readonly)             # <<<<<<<<<<<<<<
  * 
  *         return cls
  */
-  __pyx_t_7 = __Pyx_PyBool_FromLong(readonly); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 782, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBool_FromLong(readonly); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9.__pyx_n = 1;
   __pyx_t_9.readonly = __pyx_t_7;
-  __pyx_t_2 = _type_configure_getsetitem(cls, &__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 782, __pyx_L1_error)
+  __pyx_t_2 = _type_configure_getsetitem(cls, &__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "recordclass/dataobject.pyx":784
+  /* "recordclass/dataobject.pyx":772
  *         _type_configure_getsetitem(cls, readonly)
  * 
  *         return cls             # <<<<<<<<<<<<<<
  * 
  * @cython.final
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(cls);
   __pyx_r = cls;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":759
+  /* "recordclass/dataobject.pyx":747
  * class arrayclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
 
@@ -7919,15 +7813,15 @@
   __Pyx_XDECREF(cls);
   __Pyx_XDECREF(n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":792
+/* "recordclass/dataobject.pyx":780
  *     cdef Py_ssize_t n "n"
  * 
  *     def __init__(self, op):             # <<<<<<<<<<<<<<
  *         self.op = <PyObject*>op
  *         self.i = 0
  */
 
@@ -7953,26 +7847,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_op)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 792, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 780, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_op = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 792, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 780, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectiter.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_14dataobjectiter___init__(((struct DataObjectIter *)__pyx_v_self), __pyx_v_op);
 
@@ -7982,56 +7876,56 @@
 }
 
 static int __pyx_pf_11recordclass_10dataobject_14dataobjectiter___init__(struct DataObjectIter *__pyx_v_self, PyObject *__pyx_v_op) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "recordclass/dataobject.pyx":793
+  /* "recordclass/dataobject.pyx":781
  * 
  *     def __init__(self, op):
  *         self.op = <PyObject*>op             # <<<<<<<<<<<<<<
  *         self.i = 0
  *         self.n = dataobject_len(self.op)
  */
   __pyx_v_self->op = ((PyObject *)__pyx_v_op);
 
-  /* "recordclass/dataobject.pyx":794
+  /* "recordclass/dataobject.pyx":782
  *     def __init__(self, op):
  *         self.op = <PyObject*>op
  *         self.i = 0             # <<<<<<<<<<<<<<
  *         self.n = dataobject_len(self.op)
  * 
  */
   __pyx_v_self->i = 0;
 
-  /* "recordclass/dataobject.pyx":795
+  /* "recordclass/dataobject.pyx":783
  *         self.op = <PyObject*>op
  *         self.i = 0
  *         self.n = dataobject_len(self.op)             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __pyx_v_self->n = dataobject_len(__pyx_v_self->op);
 
-  /* "recordclass/dataobject.pyx":792
+  /* "recordclass/dataobject.pyx":780
  *     cdef Py_ssize_t n "n"
  * 
  *     def __init__(self, op):             # <<<<<<<<<<<<<<
  *         self.op = <PyObject*>op
  *         self.i = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":797
+/* "recordclass/dataobject.pyx":785
  *         self.n = dataobject_len(self.op)
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.i < self.n:
  *             ob = <object>dataobject_item(self.op, self.i)
  */
 
@@ -8053,80 +7947,80 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "recordclass/dataobject.pyx":798
+  /* "recordclass/dataobject.pyx":786
  * 
  *     def __next__(self):
  *         if self.i < self.n:             # <<<<<<<<<<<<<<
  *             ob = <object>dataobject_item(self.op, self.i)
  *             self.i += 1
  */
   __pyx_t_1 = ((__pyx_v_self->i < __pyx_v_self->n) != 0);
   if (likely(__pyx_t_1)) {
 
-    /* "recordclass/dataobject.pyx":799
+    /* "recordclass/dataobject.pyx":787
  *     def __next__(self):
  *         if self.i < self.n:
  *             ob = <object>dataobject_item(self.op, self.i)             # <<<<<<<<<<<<<<
  *             self.i += 1
  *             return ob
  */
     __pyx_t_2 = dataobject_item(__pyx_v_self->op, __pyx_v_self->i);
     __pyx_t_3 = ((PyObject *)__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_ob = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "recordclass/dataobject.pyx":800
+    /* "recordclass/dataobject.pyx":788
  *         if self.i < self.n:
  *             ob = <object>dataobject_item(self.op, self.i)
  *             self.i += 1             # <<<<<<<<<<<<<<
  *             return ob
  *         else:
  */
     __pyx_v_self->i = (__pyx_v_self->i + 1);
 
-    /* "recordclass/dataobject.pyx":801
+    /* "recordclass/dataobject.pyx":789
  *             ob = <object>dataobject_item(self.op, self.i)
  *             self.i += 1
  *             return ob             # <<<<<<<<<<<<<<
  *         else:
  *             raise StopIteration
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_ob);
     __pyx_r = __pyx_v_ob;
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":798
+    /* "recordclass/dataobject.pyx":786
  * 
  *     def __next__(self):
  *         if self.i < self.n:             # <<<<<<<<<<<<<<
  *             ob = <object>dataobject_item(self.op, self.i)
  *             self.i += 1
  */
   }
 
-  /* "recordclass/dataobject.pyx":803
+  /* "recordclass/dataobject.pyx":791
  *             return ob
  *         else:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   /*else*/ {
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 803, __pyx_L1_error)
+    __PYX_ERR(0, 791, __pyx_L1_error)
   }
 
-  /* "recordclass/dataobject.pyx":797
+  /* "recordclass/dataobject.pyx":785
  *         self.n = dataobject_len(self.op)
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.i < self.n:
  *             ob = <object>dataobject_item(self.op, self.i)
  */
 
@@ -8138,15 +8032,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ob);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":805
+/* "recordclass/dataobject.pyx":793
  *             raise StopIteration
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -8164,27 +8058,27 @@
 }
 
 static PyObject *__pyx_pf_11recordclass_10dataobject_14dataobjectiter_4__iter__(struct DataObjectIter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "recordclass/dataobject.pyx":806
+  /* "recordclass/dataobject.pyx":794
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  * @cython.final
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":805
+  /* "recordclass/dataobject.pyx":793
  *             raise StopIteration
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -8300,15 +8194,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectiter.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":813
+/* "recordclass/dataobject.pyx":801
  *     cdef Py_ssize_t i "i"
  * 
  *     def __init__(self, i):             # <<<<<<<<<<<<<<
  *         self.i = i
  * 
  */
 
@@ -8334,26 +8228,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 813, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 801, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_i = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 813, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 801, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectgetset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_16dataobjectgetset___init__(((struct DataObjectGetSet *)__pyx_v_self), __pyx_v_i);
 
@@ -8364,25 +8258,25 @@
 
 static int __pyx_pf_11recordclass_10dataobject_16dataobjectgetset___init__(struct DataObjectGetSet *__pyx_v_self, PyObject *__pyx_v_i) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "recordclass/dataobject.pyx":814
+  /* "recordclass/dataobject.pyx":802
  * 
  *     def __init__(self, i):
  *         self.i = i             # <<<<<<<<<<<<<<
  * 
  *     def __get__(self, ob, tp):
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 802, __pyx_L1_error)
   __pyx_v_self->i = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":813
+  /* "recordclass/dataobject.pyx":801
  *     cdef Py_ssize_t i "i"
  * 
  *     def __init__(self, i):             # <<<<<<<<<<<<<<
  *         self.i = i
  * 
  */
 
@@ -8393,15 +8287,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectgetset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":816
+/* "recordclass/dataobject.pyx":804
  *         self.i = i
  * 
  *     def __get__(self, ob, tp):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             return self
  */
 
@@ -8422,75 +8316,75 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "recordclass/dataobject.pyx":817
+  /* "recordclass/dataobject.pyx":805
  * 
  *     def __get__(self, ob, tp):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  */
   __pyx_t_1 = (__pyx_v_ob == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":818
+    /* "recordclass/dataobject.pyx":806
  *     def __get__(self, ob, tp):
  *         if ob is None:
  *             return self             # <<<<<<<<<<<<<<
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":817
+    /* "recordclass/dataobject.pyx":805
  * 
  *     def __get__(self, ob, tp):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  */
   }
 
-  /* "recordclass/dataobject.pyx":819
+  /* "recordclass/dataobject.pyx":807
  *         if ob is None:
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)             # <<<<<<<<<<<<<<
  * 
  *     def __set__(self, ob, val):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_3 = dataobject_item(((PyObject *)__pyx_v_ob), __pyx_v_self->i);
   __Pyx_INCREF(((PyObject *)__pyx_t_3));
   __pyx_r = ((PyObject *)__pyx_t_3);
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":816
+  /* "recordclass/dataobject.pyx":804
  *         self.i = i
  * 
  *     def __get__(self, ob, tp):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             return self
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":821
+/* "recordclass/dataobject.pyx":809
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  * 
  *     def __set__(self, ob, val):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             raise ValueError('None object')
  */
 
@@ -8511,57 +8405,57 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "recordclass/dataobject.pyx":822
+  /* "recordclass/dataobject.pyx":810
  * 
  *     def __set__(self, ob, val):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             raise ValueError('None object')
  *         dataobject_ass_item(<PyObject*>ob, self.i, <PyObject*>val)
  */
   __pyx_t_1 = (__pyx_v_ob == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "recordclass/dataobject.pyx":823
+    /* "recordclass/dataobject.pyx":811
  *     def __set__(self, ob, val):
  *         if ob is None:
  *             raise ValueError('None object')             # <<<<<<<<<<<<<<
  *         dataobject_ass_item(<PyObject*>ob, self.i, <PyObject*>val)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 823, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 823, __pyx_L1_error)
+    __PYX_ERR(0, 811, __pyx_L1_error)
 
-    /* "recordclass/dataobject.pyx":822
+    /* "recordclass/dataobject.pyx":810
  * 
  *     def __set__(self, ob, val):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             raise ValueError('None object')
  *         dataobject_ass_item(<PyObject*>ob, self.i, <PyObject*>val)
  */
   }
 
-  /* "recordclass/dataobject.pyx":824
+  /* "recordclass/dataobject.pyx":812
  *         if ob is None:
  *             raise ValueError('None object')
  *         dataobject_ass_item(<PyObject*>ob, self.i, <PyObject*>val)             # <<<<<<<<<<<<<<
  * 
  * @cython.final
  */
   (void)(dataobject_ass_item(((PyObject *)__pyx_v_ob), __pyx_v_self->i, ((PyObject *)__pyx_v_val)));
 
-  /* "recordclass/dataobject.pyx":821
+  /* "recordclass/dataobject.pyx":809
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  * 
  *     def __set__(self, ob, val):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             raise ValueError('None object')
  */
 
@@ -8867,15 +8761,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":831
+/* "recordclass/dataobject.pyx":819
  *     cdef Py_ssize_t i "i"
  * 
  *     def __init__(self, i):             # <<<<<<<<<<<<<<
  *         self.i = i
  * 
  */
 
@@ -8901,26 +8795,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 831, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 819, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_i = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 831, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 819, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectget.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_13dataobjectget___init__(((struct DataObjectGet *)__pyx_v_self), __pyx_v_i);
 
@@ -8931,25 +8825,25 @@
 
 static int __pyx_pf_11recordclass_10dataobject_13dataobjectget___init__(struct DataObjectGet *__pyx_v_self, PyObject *__pyx_v_i) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "recordclass/dataobject.pyx":832
+  /* "recordclass/dataobject.pyx":820
  * 
  *     def __init__(self, i):
  *         self.i = i             # <<<<<<<<<<<<<<
  * 
  *     def __get__(self, ob, tp):
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 832, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 820, __pyx_L1_error)
   __pyx_v_self->i = __pyx_t_1;
 
-  /* "recordclass/dataobject.pyx":831
+  /* "recordclass/dataobject.pyx":819
  *     cdef Py_ssize_t i "i"
  * 
  *     def __init__(self, i):             # <<<<<<<<<<<<<<
  *         self.i = i
  * 
  */
 
@@ -8960,15 +8854,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.dataobjectget.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":834
+/* "recordclass/dataobject.pyx":822
  *         self.i = i
  * 
  *     def __get__(self, ob, tp):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             return self
  */
 
@@ -8989,60 +8883,60 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "recordclass/dataobject.pyx":835
+  /* "recordclass/dataobject.pyx":823
  * 
  *     def __get__(self, ob, tp):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  */
   __pyx_t_1 = (__pyx_v_ob == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "recordclass/dataobject.pyx":836
+    /* "recordclass/dataobject.pyx":824
  *     def __get__(self, ob, tp):
  *         if ob is None:
  *             return self             # <<<<<<<<<<<<<<
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "recordclass/dataobject.pyx":835
+    /* "recordclass/dataobject.pyx":823
  * 
  *     def __get__(self, ob, tp):
  *         if ob is None:             # <<<<<<<<<<<<<<
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)
  */
   }
 
-  /* "recordclass/dataobject.pyx":837
+  /* "recordclass/dataobject.pyx":825
  *         if ob is None:
  *             return self
  *         return <object>dataobject_item(<PyObject*>ob, self.i)             # <<<<<<<<<<<<<<
  * 
  * @cython.final
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_3 = dataobject_item(((PyObject *)__pyx_v_ob), __pyx_v_self->i);
   __Pyx_INCREF(((PyObject *)__pyx_t_3));
   __pyx_r = ((PyObject *)__pyx_t_3);
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":834
+  /* "recordclass/dataobject.pyx":822
  *         self.i = i
  * 
  *     def __get__(self, ob, tp):             # <<<<<<<<<<<<<<
  *         if ob is None:
  *             return self
  */
 
@@ -9343,15 +9237,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":845
+/* "recordclass/dataobject.pyx":833
  * 
  *     @property
  *     def obj(self):             # <<<<<<<<<<<<<<
  *         return self.ob
  * 
  */
 
@@ -9369,42 +9263,42 @@
 }
 
 static PyObject *__pyx_pf_11recordclass_10dataobject_13SequenceProxy_3obj___get__(struct SequenceProxyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "recordclass/dataobject.pyx":846
+  /* "recordclass/dataobject.pyx":834
  *     @property
  *     def obj(self):
  *         return self.ob             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, ob):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->ob);
   __pyx_r = __pyx_v_self->ob;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":845
+  /* "recordclass/dataobject.pyx":833
  * 
  *     @property
  *     def obj(self):             # <<<<<<<<<<<<<<
  *         return self.ob
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":848
+/* "recordclass/dataobject.pyx":836
  *         return self.ob
  * 
  *     def __init__(self, ob):             # <<<<<<<<<<<<<<
  *         self.ob = ob
  *         self.hash = 0
  */
 
@@ -9430,26 +9324,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ob)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 848, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 836, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_ob = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 848, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 836, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.SequenceProxy.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11recordclass_10dataobject_13SequenceProxy___init__(((struct SequenceProxyObject *)__pyx_v_self), __pyx_v_ob);
 
@@ -9459,51 +9353,51 @@
 }
 
 static int __pyx_pf_11recordclass_10dataobject_13SequenceProxy___init__(struct SequenceProxyObject *__pyx_v_self, PyObject *__pyx_v_ob) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "recordclass/dataobject.pyx":849
+  /* "recordclass/dataobject.pyx":837
  * 
  *     def __init__(self, ob):
  *         self.ob = ob             # <<<<<<<<<<<<<<
  *         self.hash = 0
  * 
  */
   __Pyx_INCREF(__pyx_v_ob);
   __Pyx_GIVEREF(__pyx_v_ob);
   __Pyx_GOTREF(__pyx_v_self->ob);
   __Pyx_DECREF(__pyx_v_self->ob);
   __pyx_v_self->ob = __pyx_v_ob;
 
-  /* "recordclass/dataobject.pyx":850
+  /* "recordclass/dataobject.pyx":838
  *     def __init__(self, ob):
  *         self.ob = ob
  *         self.hash = 0             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, ind):
  */
   __pyx_v_self->hash = 0;
 
-  /* "recordclass/dataobject.pyx":848
+  /* "recordclass/dataobject.pyx":836
  *         return self.ob
  * 
  *     def __init__(self, ob):             # <<<<<<<<<<<<<<
  *         self.ob = ob
  *         self.hash = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":852
+/* "recordclass/dataobject.pyx":840
  *         self.hash = 0
  * 
  *     def __getitem__(self, ind):             # <<<<<<<<<<<<<<
  *         return self.ob.__getitem__(ind)
  * 
  */
 
@@ -9524,44 +9418,44 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "recordclass/dataobject.pyx":853
+  /* "recordclass/dataobject.pyx":841
  * 
  *     def __getitem__(self, ind):
  *         return self.ob.__getitem__(ind)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_getitem); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 853, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_getitem); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_ind) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_ind);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 853, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":852
+  /* "recordclass/dataobject.pyx":840
  *         self.hash = 0
  * 
  *     def __getitem__(self, ind):             # <<<<<<<<<<<<<<
  *         return self.ob.__getitem__(ind)
  * 
  */
 
@@ -9574,15 +9468,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":855
+/* "recordclass/dataobject.pyx":843
  *         return self.ob.__getitem__(ind)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self.ob.__len__()
  * 
  */
 
@@ -9604,44 +9498,44 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "recordclass/dataobject.pyx":856
+  /* "recordclass/dataobject.pyx":844
  * 
  *     def __len__(self):
  *         return self.ob.__len__()             # <<<<<<<<<<<<<<
  * 
  *     def __hash__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_len); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 856, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_len); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 856, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 856, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":855
+  /* "recordclass/dataobject.pyx":843
  *         return self.ob.__getitem__(ind)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self.ob.__len__()
  * 
  */
 
@@ -9653,15 +9547,15 @@
   __Pyx_AddTraceback("recordclass.dataobject.SequenceProxy.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":858
+/* "recordclass/dataobject.pyx":846
  *         return self.ob.__len__()
  * 
  *     def __hash__(self):             # <<<<<<<<<<<<<<
  *         if self.hash == 0:
  *             self.hash = hash(tuple(self.ob))
  */
 
@@ -9682,57 +9576,57 @@
   Py_hash_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_hash_t __pyx_t_3;
   __Pyx_RefNannySetupContext("__hash__", 0);
 
-  /* "recordclass/dataobject.pyx":859
+  /* "recordclass/dataobject.pyx":847
  * 
  *     def __hash__(self):
  *         if self.hash == 0:             # <<<<<<<<<<<<<<
  *             self.hash = hash(tuple(self.ob))
  *         return self.hash
  */
   __pyx_t_1 = ((__pyx_v_self->hash == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "recordclass/dataobject.pyx":860
+    /* "recordclass/dataobject.pyx":848
  *     def __hash__(self):
  *         if self.hash == 0:
  *             self.hash = hash(tuple(self.ob))             # <<<<<<<<<<<<<<
  *         return self.hash
  * 
  */
-    __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_v_self->ob); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 860, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_v_self->ob); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 848, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyObject_Hash(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_hash_t)-1))) __PYX_ERR(0, 860, __pyx_L1_error)
+    __pyx_t_3 = PyObject_Hash(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_hash_t)-1))) __PYX_ERR(0, 848, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_self->hash = __pyx_t_3;
 
-    /* "recordclass/dataobject.pyx":859
+    /* "recordclass/dataobject.pyx":847
  * 
  *     def __hash__(self):
  *         if self.hash == 0:             # <<<<<<<<<<<<<<
  *             self.hash = hash(tuple(self.ob))
  *         return self.hash
  */
   }
 
-  /* "recordclass/dataobject.pyx":861
+  /* "recordclass/dataobject.pyx":849
  *         if self.hash == 0:
  *             self.hash = hash(tuple(self.ob))
  *         return self.hash             # <<<<<<<<<<<<<<
  * 
  *     def __richcmp__(self, other, flag):
  */
   __pyx_r = __pyx_v_self->hash;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":858
+  /* "recordclass/dataobject.pyx":846
  *         return self.ob.__len__()
  * 
  *     def __hash__(self):             # <<<<<<<<<<<<<<
  *         if self.hash == 0:
  *             self.hash = hash(tuple(self.ob))
  */
 
@@ -9743,30 +9637,30 @@
   __pyx_r = -1;
   __pyx_L0:;
   if (unlikely(__pyx_r == -1) && !PyErr_Occurred()) __pyx_r = -2;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":863
+/* "recordclass/dataobject.pyx":851
  *         return self.hash
  * 
  *     def __richcmp__(self, other, flag):             # <<<<<<<<<<<<<<
  *         return self.ob.__richcmp__(other, flag)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_11recordclass_10dataobject_13SequenceProxy_9__richcmp__(PyObject *__pyx_v_self, PyObject *__pyx_v_other, int __pyx_arg_flag); /*proto*/
 static PyObject *__pyx_pw_11recordclass_10dataobject_13SequenceProxy_9__richcmp__(PyObject *__pyx_v_self, PyObject *__pyx_v_other, int __pyx_arg_flag) {
   PyObject *__pyx_v_flag = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__richcmp__ (wrapper)", 0);
-  __pyx_v_flag = __Pyx_PyInt_From_int(__pyx_arg_flag); if (unlikely(!__pyx_v_flag)) __PYX_ERR(0, 863, __pyx_L3_error)
+  __pyx_v_flag = __Pyx_PyInt_From_int(__pyx_arg_flag); if (unlikely(!__pyx_v_flag)) __PYX_ERR(0, 851, __pyx_L3_error)
   __Pyx_GOTREF(__pyx_v_flag);
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("recordclass.dataobject.SequenceProxy.__richcmp__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -9784,23 +9678,23 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__richcmp__", 0);
 
-  /* "recordclass/dataobject.pyx":864
+  /* "recordclass/dataobject.pyx":852
  * 
  *     def __richcmp__(self, other, flag):
  *         return self.ob.__richcmp__(other, flag)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_richcmp); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ob, __pyx_n_s_richcmp); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 852, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9809,49 +9703,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_other, __pyx_v_flag};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_other, __pyx_v_flag};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_other);
     __Pyx_GIVEREF(__pyx_v_other);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_other);
     __Pyx_INCREF(__pyx_v_flag);
     __Pyx_GIVEREF(__pyx_v_flag);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_flag);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":863
+  /* "recordclass/dataobject.pyx":851
  *         return self.hash
  * 
  *     def __richcmp__(self, other, flag):             # <<<<<<<<<<<<<<
  *         return self.ob.__richcmp__(other, flag)
  * 
  */
 
@@ -9865,15 +9759,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":866
+/* "recordclass/dataobject.pyx":854
  *         return self.ob.__richcmp__(other, flag)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self.ob)
  * 
  */
 
@@ -9893,32 +9787,32 @@
 static PyObject *__pyx_pf_11recordclass_10dataobject_13SequenceProxy_10__iter__(struct SequenceProxyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "recordclass/dataobject.pyx":867
+  /* "recordclass/dataobject.pyx":855
  * 
  *     def __iter__(self):
  *         return iter(self.ob)             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->ob;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 867, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":866
+  /* "recordclass/dataobject.pyx":854
  *         return self.ob.__richcmp__(other, flag)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self.ob)
  * 
  */
 
@@ -9930,15 +9824,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":869
+/* "recordclass/dataobject.pyx":857
  *         return iter(self.ob)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  */
 
@@ -9958,38 +9852,38 @@
 static PyObject *__pyx_pf_11recordclass_10dataobject_13SequenceProxy_12__repr__(struct SequenceProxyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "recordclass/dataobject.pyx":870
+  /* "recordclass/dataobject.pyx":858
  * 
  *     def __repr__(self):
  *         return "sequenceproxy(" + repr(self.ob) + ")"             # <<<<<<<<<<<<<<
  * 
  * def sequenceproxy(ob):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->ob;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Repr(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Repr(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_sequenceproxy, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_sequenceproxy, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_kp_u__14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_kp_u__14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":869
+  /* "recordclass/dataobject.pyx":857
  *         return iter(self.ob)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  */
 
@@ -10299,15 +10193,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recordclass/dataobject.pyx":872
+/* "recordclass/dataobject.pyx":860
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  * def sequenceproxy(ob):             # <<<<<<<<<<<<<<
  *     return SequenceProxy(ob)
  * 
  */
 
@@ -10328,28 +10222,28 @@
 
 static PyObject *__pyx_pf_11recordclass_10dataobject_sequenceproxy(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_ob) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("sequenceproxy", 0);
 
-  /* "recordclass/dataobject.pyx":873
+  /* "recordclass/dataobject.pyx":861
  * 
  * def sequenceproxy(ob):
  *     return SequenceProxy(ob)             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_SequenceProxy), __pyx_v_ob); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 873, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_11recordclass_10dataobject_SequenceProxy), __pyx_v_ob); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 861, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "recordclass/dataobject.pyx":872
+  /* "recordclass/dataobject.pyx":860
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  * def sequenceproxy(ob):             # <<<<<<<<<<<<<<
  *     return SequenceProxy(ob)
  * 
  */
 
@@ -12412,136 +12306,136 @@
   {&__pyx_n_s_usedict, __pyx_k_usedict, sizeof(__pyx_k_usedict), 0, 0, 1, 1},
   {&__pyx_n_u_usedict, __pyx_k_usedict, sizeof(__pyx_k_usedict), 0, 1, 0, 1},
   {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
   {&__pyx_n_u_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 350, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 468, __pyx_L1_error)
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 732, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 742, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 803, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 730, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 791, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 811, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "recordclass/dataobject.pyx":468
+  /* "recordclass/dataobject.pyx":458
  * 
- *         if n != len(t):
+ *         if n != Py_SIZE(<PyObject*>t):
  *             raise TypeError("Invalid length of args")             # <<<<<<<<<<<<<<
  * 
- *         if n > 0:
+ *         if n:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Invalid_length_of_args); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Invalid_length_of_args); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "recordclass/dataobject.pyx":559
+  /* "recordclass/dataobject.pyx":547
  * 
  *         if not isinstance(other, dataobject):
  *             raise TypeError("Types are not comparable")             # <<<<<<<<<<<<<<
  * 
  *         if flag == 2: # ==
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Types_are_not_comparable); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Types_are_not_comparable); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "recordclass/dataobject.pyx":586
+  /* "recordclass/dataobject.pyx":574
  *                 return False
  *         else:
  *             raise TypeError('The type support only != and ==')             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_The_type_support_only_and); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_The_type_support_only_and); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "recordclass/dataobject.pyx":705
+  /* "recordclass/dataobject.pyx":693
  * 
  *         options = ns.pop('__options__', {})
  *         readonly = options.get('readonly', False)             # <<<<<<<<<<<<<<
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_readonly, Py_False); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_readonly, Py_False); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "recordclass/dataobject.pyx":706
+  /* "recordclass/dataobject.pyx":694
  *         options = ns.pop('__options__', {})
  *         readonly = options.get('readonly', False)
  *         usedict = options.get('usedict', False)             # <<<<<<<<<<<<<<
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)
  */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_usedict, Py_False); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_usedict, Py_False); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "recordclass/dataobject.pyx":707
+  /* "recordclass/dataobject.pyx":695
  *         readonly = options.get('readonly', False)
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)             # <<<<<<<<<<<<<<
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)
  */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_u_gc, Py_False); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_u_gc, Py_False); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "recordclass/dataobject.pyx":708
+  /* "recordclass/dataobject.pyx":696
  *         usedict = options.get('usedict', False)
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)             # <<<<<<<<<<<<<<
  *         hashable = options.get('hashable', True)
  *         assequence = options.get('assequence', True)
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_weakref, Py_False); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_weakref, Py_False); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "recordclass/dataobject.pyx":709
+  /* "recordclass/dataobject.pyx":697
  *         gc = options.get('gc', False)
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)             # <<<<<<<<<<<<<<
  *         assequence = options.get('assequence', True)
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_hashable, Py_True); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_hashable, Py_True); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "recordclass/dataobject.pyx":710
+  /* "recordclass/dataobject.pyx":698
  *         weakref = options.get('weakref', False)
  *         hashable = options.get('hashable', True)
  *         assequence = options.get('assequence', True)             # <<<<<<<<<<<<<<
  * 
  *         if readonly and not hashable:
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_assequence, Py_True); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_assequence, Py_True); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "recordclass/dataobject.pyx":718
+  /* "recordclass/dataobject.pyx":706
  * 
  *         if not hasattr(cls, "__attrs__"):
  *             raise TypeError('Class is missing __attrs__')             # <<<<<<<<<<<<<<
  * 
  *         fields = cls.__attrs__
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Class_is_missing___attrs); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Class_is_missing___attrs); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 706, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.op cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -12556,60 +12450,60 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.op cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_self_op_cannot_be_converted_to_a); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "recordclass/dataobject.pyx":823
+  /* "recordclass/dataobject.pyx":811
  *     def __set__(self, ob, val):
  *         if ob is None:
  *             raise ValueError('None object')             # <<<<<<<<<<<<<<
  *         dataobject_ass_item(<PyObject*>ob, self.i, <PyObject*>val)
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_None_object); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_None_object); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "recordclass/dataobject.pyx":688
+  /* "recordclass/dataobject.pyx":676
  * class structclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
-  __pyx_tuple__15 = PyTuple_Pack(20, __pyx_n_s_tp, __pyx_n_s_name, __pyx_n_s_bases, __pyx_n_s_ns, __pyx_n_s_options_2, __pyx_n_s_readonly, __pyx_n_s_usedict, __pyx_n_s_gc, __pyx_n_s_weakref, __pyx_n_s_hashable, __pyx_n_s_assequence, __pyx_n_s_cls, __pyx_n_s_fields, __pyx_n_s_flag, __pyx_n_s_f, __pyx_n_s_item_object, __pyx_n_s_index, __pyx_n_s_attrname, __pyx_n_s_base, __pyx_n_s_base_fields); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(20, __pyx_n_s_tp, __pyx_n_s_name, __pyx_n_s_bases, __pyx_n_s_ns, __pyx_n_s_options_2, __pyx_n_s_readonly, __pyx_n_s_usedict, __pyx_n_s_gc, __pyx_n_s_weakref, __pyx_n_s_hashable, __pyx_n_s_assequence, __pyx_n_s_cls, __pyx_n_s_fields, __pyx_n_s_flag, __pyx_n_s_f, __pyx_n_s_item_object, __pyx_n_s_index, __pyx_n_s_attrname, __pyx_n_s_base, __pyx_n_s_base_fields); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_new, 688, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_new, 676, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 676, __pyx_L1_error)
 
-  /* "recordclass/dataobject.pyx":759
+  /* "recordclass/dataobject.pyx":747
  * class arrayclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
-  __pyx_tuple__17 = PyTuple_Pack(12, __pyx_n_s_tp, __pyx_n_s_name, __pyx_n_s_bases, __pyx_n_s_ns, __pyx_n_s_options_2, __pyx_n_s_readonly, __pyx_n_s_usedict, __pyx_n_s_hashable, __pyx_n_s_gc, __pyx_n_s_weakref, __pyx_n_s_cls, __pyx_n_s_n); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(12, __pyx_n_s_tp, __pyx_n_s_name, __pyx_n_s_bases, __pyx_n_s_ns, __pyx_n_s_options_2, __pyx_n_s_readonly, __pyx_n_s_usedict, __pyx_n_s_hashable, __pyx_n_s_gc, __pyx_n_s_weakref, __pyx_n_s_cls, __pyx_n_s_n); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(4, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_new, 759, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(4, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_new, 747, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 747, __pyx_L1_error)
 
-  /* "recordclass/dataobject.pyx":872
+  /* "recordclass/dataobject.pyx":860
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  * def sequenceproxy(ob):             # <<<<<<<<<<<<<<
  *     return SequenceProxy(ob)
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_ob); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 872, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_ob); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_sequenceproxy_2, 872, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 872, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_recordclass_dataobject_pyx, __pyx_n_s_sequenceproxy_2, 860, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 860, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_dataobjectgetset(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -12691,60 +12585,60 @@
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_11recordclass_10dataobject_type) __PYX_ERR(0, 18, __pyx_L1_error)
-  if (PyType_Ready(&DataObjectType) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
+  if (PyType_Ready(&DataObjectType) < 0) __PYX_ERR(0, 437, __pyx_L1_error)
   DataObjectType.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!DataObjectType.tp_dictoffset && DataObjectType.tp_getattro == PyObject_GenericGetAttr)) {
     DataObjectType.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobject, (PyObject *)&DataObjectType) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobject, (PyObject *)&DataObjectType) < 0) __PYX_ERR(0, 437, __pyx_L1_error)
   __pyx_ptype_11recordclass_10dataobject_dataobject = &DataObjectType;
-  if (PyType_Ready(&DataObjectIterType) < 0) __PYX_ERR(0, 787, __pyx_L1_error)
+  if (PyType_Ready(&DataObjectIterType) < 0) __PYX_ERR(0, 775, __pyx_L1_error)
   DataObjectIterType.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!DataObjectIterType.tp_dictoffset && DataObjectIterType.tp_getattro == PyObject_GenericGetAttr)) {
     DataObjectIterType.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectiter, (PyObject *)&DataObjectIterType) < 0) __PYX_ERR(0, 787, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&DataObjectIterType) < 0) __PYX_ERR(0, 787, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectiter, (PyObject *)&DataObjectIterType) < 0) __PYX_ERR(0, 775, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&DataObjectIterType) < 0) __PYX_ERR(0, 775, __pyx_L1_error)
   __pyx_ptype_11recordclass_10dataobject_dataobjectiter = &DataObjectIterType;
-  if (PyType_Ready(&DataObjectGetSetType) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
+  if (PyType_Ready(&DataObjectGetSetType) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
   DataObjectGetSetType.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!DataObjectGetSetType.tp_dictoffset && DataObjectGetSetType.tp_getattro == PyObject_GenericGetAttr)) {
     DataObjectGetSetType.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectgetset, (PyObject *)&DataObjectGetSetType) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&DataObjectGetSetType) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectgetset, (PyObject *)&DataObjectGetSetType) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&DataObjectGetSetType) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
   __pyx_ptype_11recordclass_10dataobject_dataobjectgetset = &DataObjectGetSetType;
-  if (PyType_Ready(&DataObjectGetType) < 0) __PYX_ERR(0, 827, __pyx_L1_error)
+  if (PyType_Ready(&DataObjectGetType) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
   DataObjectGetType.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!DataObjectGetType.tp_dictoffset && DataObjectGetType.tp_getattro == PyObject_GenericGetAttr)) {
     DataObjectGetType.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectget, (PyObject *)&DataObjectGetType) < 0) __PYX_ERR(0, 827, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&DataObjectGetType) < 0) __PYX_ERR(0, 827, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_dataobjectget, (PyObject *)&DataObjectGetType) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&DataObjectGetType) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
   __pyx_ptype_11recordclass_10dataobject_dataobjectget = &DataObjectGetType;
-  if (PyType_Ready(&SequenceProxyType) < 0) __PYX_ERR(0, 840, __pyx_L1_error)
+  if (PyType_Ready(&SequenceProxyType) < 0) __PYX_ERR(0, 828, __pyx_L1_error)
   SequenceProxyType.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!SequenceProxyType.tp_dictoffset && SequenceProxyType.tp_getattro == PyObject_GenericGetAttr)) {
     SequenceProxyType.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SequenceProxy, (PyObject *)&SequenceProxyType) < 0) __PYX_ERR(0, 840, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&SequenceProxyType) < 0) __PYX_ERR(0, 840, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SequenceProxy, (PyObject *)&SequenceProxyType) < 0) __PYX_ERR(0, 828, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&SequenceProxyType) < 0) __PYX_ERR(0, 828, __pyx_L1_error)
   __pyx_ptype_11recordclass_10dataobject_SequenceProxy = &SequenceProxyType;
-  if (PyType_Ready(&__pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic) < 0) __PYX_ERR(0, 624, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic) < 0) __PYX_ERR(0, 612, __pyx_L1_error)
   __pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic.tp_dictoffset && __pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic = &__pyx_type_11recordclass_10dataobject___pyx_scope_struct___type_configure_basic;
-  if (PyType_Ready(&__pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 633, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 621, __pyx_L1_error)
   __pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr.tp_print = 0;
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11recordclass_10dataobject___pyx_scope_struct_1_genexpr = &__pyx_type_11recordclass_10dataobject___pyx_scope_struct_1_genexpr;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
@@ -12992,140 +12886,140 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "recordclass/dataobject.pyx":683
+  /* "recordclass/dataobject.pyx":671
  *        tp.tp_as_mapping.mp_ass_subscript = dataobject_ass_subscript
  * 
  * cdef dict slotsgetset_cache "slotsgetset_cache" = {}             # <<<<<<<<<<<<<<
  * cdef dict slotsget_cache "slotsget_cache" = {}
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(slotsgetset_cache);
   __Pyx_DECREF_SET(slotsgetset_cache, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":684
+  /* "recordclass/dataobject.pyx":672
  * 
  * cdef dict slotsgetset_cache "slotsgetset_cache" = {}
  * cdef dict slotsget_cache "slotsget_cache" = {}             # <<<<<<<<<<<<<<
  * 
  * class structclasstype(type):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(slotsget_cache);
   __Pyx_DECREF_SET(slotsget_cache, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":686
+  /* "recordclass/dataobject.pyx":674
  * cdef dict slotsget_cache "slotsget_cache" = {}
  * 
  * class structclasstype(type):             # <<<<<<<<<<<<<<
  *     #
  *     def __new__(tp, name, bases, ns):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_structclasstype, __pyx_n_s_structclasstype, (PyObject *) NULL, __pyx_n_s_recordclass_dataobject, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_structclasstype, __pyx_n_s_structclasstype, (PyObject *) NULL, __pyx_n_s_recordclass_dataobject, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "recordclass/dataobject.pyx":688
+  /* "recordclass/dataobject.pyx":676
  * class structclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
-  __pyx_t_4 = __Pyx_CyFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_15structclasstype_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_structclasstype___new, NULL, __pyx_n_s_recordclass_dataobject, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_15structclasstype_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_structclasstype___new, NULL, __pyx_n_s_recordclass_dataobject, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_new, __pyx_t_4) < 0) __PYX_ERR(0, 688, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_new, __pyx_t_4) < 0) __PYX_ERR(0, 676, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "recordclass/dataobject.pyx":686
+  /* "recordclass/dataobject.pyx":674
  * cdef dict slotsget_cache "slotsget_cache" = {}
  * 
  * class structclasstype(type):             # <<<<<<<<<<<<<<
  *     #
  *     def __new__(tp, name, bases, ns):
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_structclasstype, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_structclasstype, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_structclasstype, __pyx_t_4) < 0) __PYX_ERR(0, 686, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_structclasstype, __pyx_t_4) < 0) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":757
+  /* "recordclass/dataobject.pyx":745
  *         return cls
  * 
  * class arrayclasstype(type):             # <<<<<<<<<<<<<<
  *     #
  *     def __new__(tp, name, bases, ns):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_ptype_11recordclass_10dataobject_type));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_arrayclasstype, __pyx_n_s_arrayclasstype, (PyObject *) NULL, __pyx_n_s_recordclass_dataobject, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_arrayclasstype, __pyx_n_s_arrayclasstype, (PyObject *) NULL, __pyx_n_s_recordclass_dataobject, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "recordclass/dataobject.pyx":759
+  /* "recordclass/dataobject.pyx":747
  * class arrayclasstype(type):
  *     #
  *     def __new__(tp, name, bases, ns):             # <<<<<<<<<<<<<<
  *         cdef object options "options"
  *         cdef bint readonly "readonly"
  */
-  __pyx_t_4 = __Pyx_CyFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_14arrayclasstype_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_arrayclasstype___new, NULL, __pyx_n_s_recordclass_dataobject, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_14arrayclasstype_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_arrayclasstype___new, NULL, __pyx_n_s_recordclass_dataobject, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_new, __pyx_t_4) < 0) __PYX_ERR(0, 759, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_new, __pyx_t_4) < 0) __PYX_ERR(0, 747, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "recordclass/dataobject.pyx":757
+  /* "recordclass/dataobject.pyx":745
  *         return cls
  * 
  * class arrayclasstype(type):             # <<<<<<<<<<<<<<
  *     #
  *     def __new__(tp, name, bases, ns):
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_arrayclasstype, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_arrayclasstype, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_arrayclasstype, __pyx_t_4) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_arrayclasstype, __pyx_t_4) < 0) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "recordclass/dataobject.pyx":872
+  /* "recordclass/dataobject.pyx":860
  *         return "sequenceproxy(" + repr(self.ob) + ")"
  * 
  * def sequenceproxy(ob):             # <<<<<<<<<<<<<<
  *     return SequenceProxy(ob)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_1sequenceproxy, NULL, __pyx_n_s_recordclass_dataobject); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_11recordclass_10dataobject_1sequenceproxy, NULL, __pyx_n_s_recordclass_dataobject); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sequenceproxy_2, __pyx_t_1) < 0) __PYX_ERR(0, 872, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sequenceproxy_2, __pyx_t_1) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_dataobjectgetset(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -13457,156 +13351,14 @@
     #else
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-#endif
-
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
@@ -13619,74 +13371,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
-    }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-#endif
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -13910,14 +13602,216 @@
     result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
 #endif
 bad:
     Py_XDECREF(args);
     return result;
 }
 
+/* PyCFunctionFastCall */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    }
+}
+#endif
+
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+#endif
+
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectCallOneArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *result;
+    PyObject *args = PyTuple_New(1);
+    if (unlikely(!args)) return NULL;
+    Py_INCREF(arg);
+    PyTuple_SET_ITEM(args, 0, arg);
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+    }
+#endif
+    if (likely(PyCFunction_Check(func))) {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+            return __Pyx_PyObject_CallMethO(func, arg);
+#if CYTHON_FAST_PYCCALL
+        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+#endif
+        }
+    }
+    return __Pyx__PyObject_CallOneArg(func, arg);
+}
+#else
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *result;
+    PyObject *args = PyTuple_Pack(1, arg);
+    if (unlikely(!args)) return NULL;
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
+    return result;
+}
+#endif
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
```

### Comparing `recordclass-0.8.5/lib/recordclass/dataobject.h` & `recordclass-0.9/lib/recordclass/dataobject.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,64 +5,64 @@
 
 struct DataObject;
 struct DataObjectIter;
 struct DataObjectGetSet;
 struct DataObjectGet;
 struct SequenceProxyObject;
 
-/* "recordclass/dataobject.pyx":447
+/* "recordclass/dataobject.pyx":437
  * 
  * @cython.auto_pickle(False)
  * cdef public class dataobject[object DataObject, type DataObjectType]:             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, *args, **kw):
  */
 struct DataObject {
   PyObject_HEAD
 };
 
-/* "recordclass/dataobject.pyx":787
+/* "recordclass/dataobject.pyx":775
  * 
  * @cython.final
  * cdef public class dataobjectiter[object DataObjectIter, type DataObjectIterType]:             # <<<<<<<<<<<<<<
  *     cdef PyObject *op "op"
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectIter {
   PyObject_HEAD
   PyObject *op;
   Py_ssize_t i;
   Py_ssize_t n;
 };
 
-/* "recordclass/dataobject.pyx":809
+/* "recordclass/dataobject.pyx":797
  * 
  * @cython.final
  * cdef public class dataobjectgetset[object DataObjectGetSet, type DataObjectGetSetType]:             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectGetSet {
   PyObject_HEAD
   Py_ssize_t i;
 };
 
-/* "recordclass/dataobject.pyx":827
+/* "recordclass/dataobject.pyx":815
  * 
  * @cython.final
  * cdef public class dataobjectget[object DataObjectGet, type DataObjectGetType]:             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t i "i"
  */
 struct DataObjectGet {
   PyObject_HEAD
   Py_ssize_t i;
 };
 
-/* "recordclass/dataobject.pyx":840
+/* "recordclass/dataobject.pyx":828
  * 
  * @cython.final
  * cdef public class SequenceProxy[object SequenceProxyObject, type SequenceProxyType]:             # <<<<<<<<<<<<<<
  *     cdef object ob "ob"
  *     cdef Py_hash_t hash "hash"
  */
 struct SequenceProxyObject {
```

### Comparing `recordclass-0.8.5/lib/recordclass/memoryslots.c` & `recordclass-0.9/lib/recordclass/memoryslots.c`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return NULL;
     }
         
     op = (PyMemorySlotsObject*)_PyObject_GC_NewVar(&PyMemorySlots_Type, size);
     if (op == NULL)
         return NULL;
 
-    //memset(op->ob_item, 0, Py_SIZE(op)*sizeof(void*));
+    memset(op->ob_item, 0, Py_SIZE(op)*sizeof(void*));
 
     PyObject_GC_Track(op);
     
     return (PyObject*)op;
 }
 
 static PyObject *
```

### Comparing `recordclass-0.8.5/lib/recordclass/recordclass.py` & `recordclass-0.9/lib/recordclass/recordclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/structclass.py` & `recordclass-0.9/lib/recordclass/structclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/test_arrayclass.py` & `recordclass-0.9/lib/recordclass/test/test_arrayclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/test_memoryslots.py` & `recordclass-0.9/lib/recordclass/test/test_memoryslots.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/test_recordclass.py` & `recordclass-0.9/lib/recordclass/test/test_recordclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/test_structclass.py` & `recordclass-0.9/lib/recordclass/test/test_structclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/typing/test_recordclass.py` & `recordclass-0.9/lib/recordclass/test/typing/test_recordclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/test/typing/test_structclass.py` & `recordclass-0.9/lib/recordclass/test/typing/test_structclass.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass/typing/__init__.py` & `recordclass-0.9/lib/recordclass/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/lib/recordclass.egg-info/PKG-INFO` & `recordclass-0.9/lib/recordclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recordclass
-Version: 0.8.5
+Version: 0.9
 Summary: Mutable variants of tuple (memoryslots) and collections.namedtuple (recordclass), which support assignments and more memory saving variants (arrayclass and structclass)
 Home-page: http://intellimath.bitbucket.org/recordclass
 Author: Zaur Shibzukhov
 Author-email: szport@gmail.com
 License: MIT License
 Download-URL: https://bitbucket.org/intellimath/recordclass
 Description: # Recordclass library
@@ -39,27 +39,27 @@
         
         ## Quick start:
         
         First load inventory:
         
             >>> from recordclass import recordclass, RecordClass
         
-        Simple example with `recordclass`:
+        Example with `recordclass`:
         
             >>> Point = recordclass('Point', 'x y')
             >>> p = Point(1,2)
             >>> print(p)
             Point(1, 2)
             >>> print(p.x, p.y)
             1 2
             >>> p.x, p.y = 10, 20
             >>> print(p)
             Point(10, 20)
             
-        Simple example with `RecordClass` and typehints::
+        Example with `RecordClass` and typehints::
         
             class Point(RecordClass):
                x: int
                y: int
         
             >>> ptint(Point.__annotations__)
             {'x': <class 'int'>, 'y': <class 'int'>}
@@ -180,15 +180,20 @@
         |   `new`   |    739±24 ns  |     915±35 ns    |   763±21 ns   |    889±34 ns  |
         | `getattr` |   84.0±1.7 ns |    42.8±1.5 ns   |   39.5±1.0 ns |   41.7±1.1 ns |
         | `setattr` |               |     50.5±1.7 ns  |   50.9±1.5 ns |   48.8±1.0 ns |
         
         
         ### Changes:
         
-        ### 0.8.5
+        #### 0.9
+        
+        * Change version to 0.9 to indicate a step forward.
+        * Cleanup dataobject.__cinit__
+        
+        #### 0.8.5
         
         * Make `arrayclass`-based objects support setitem/getitem and `structclass`-based objects able 
           to not support them. By default, as before `structclass`-based objects support setitem/getitem protocol.
         * Now only instances of `dataobject` are comparable to 'arrayclass'-based and `structclass`-based instances.
         * Now generated classes can be hashable.
```

### Comparing `recordclass-0.8.5/lib/recordclass.egg-info/SOURCES.txt` & `recordclass-0.9/lib/recordclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/setup.py` & `recordclass-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 packages=['recordclass', 'recordclass.test']
 if _PY36:
     packages.append('recordclass.test.typing')
     packages.append('recordclass.typing')
 
 setup(
     name = 'recordclass',
-    version = '0.8.5',
+    version = '0.9',
     description = description,
     author = 'Zaur Shibzukhov',
     author_email = 'szport@gmail.com',
     # maintainer = 'Zaur Shibzukhov',
     # maintainer_email = 'szport@gmail.com',
     license = "MIT License",
     cmdclass = {'build_ext': build_ext},
```

### Comparing `recordclass-0.8.5/test_all.py` & `recordclass-0.9/test_all.py`

 * *Files identical despite different names*

### Comparing `recordclass-0.8.5/test_performance.py` & `recordclass-0.9/test_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,48 +37,48 @@
 key = 10
 
 runner = perf.Runner()
 
 ### new ###
 res = runner.timeit(
     "namedtuple.new",
-    stmt="r = R(1,2,3,4,5,6,7,8,9,10,11)",
+    stmt="R(1,2,3,4,5,6,7,8,9,10,11)",
     setup="""
 from collections import namedtuple
 R = namedtuple('R', 'a b c d e f g h i j k')
 """
 )
 
 res = runner.timeit(
     "Recordclass.new",
-    stmt="r = R(1,2,3,4,5,6,7,8,9,10,11)",
+    stmt="R(1,2,3,4,5,6,7,8,9,10,11)",
     setup="""
 from recordclass import recordclass
 R = recordclass('R', 'a b c d e f g h i j k')
 """
 )
 
 runner.timeit(
     "__slots__.new",
-    stmt="r = R(1,2,3,4,5,6,7,8,9,10,11)",
+    stmt="R(1,2,3,4,5,6,7,8,9,10,11)",
     setup="""
 class R(object):
     __slots__ = ["a","b","c","d","e","f","g","h","i","j","k"]
 
     def __init__(self, a, b, c, d, e, f, g, h, i, j, k):
         self.a = a; self.b = b; self.c = c
         self.d = d; self.e = e; self.f = f
         self.g = g; self.h = h; self.i = i
         self.j = j; self.k = k
 """
 )
 
 runner.timeit(
     "Structclass.new",
-    stmt="r = R(1,2,3,4,5,6,7,8,9,10,11)",
+    stmt="R(1,2,3,4,5,6,7,8,9,10,11)",
     setup="""
 from recordclass import structclass
 R = structclass('R', 'a b c d e f g h i j k')
 """
 )
 
 ### getattr ###
```

