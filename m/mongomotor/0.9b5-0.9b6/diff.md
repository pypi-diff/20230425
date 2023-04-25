# Comparing `tmp/mongomotor-0.9b5.tar.gz` & `tmp/mongomotor-0.9b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mongomotor-0.9b5.tar", last modified: Mon Aug 22 07:09:44 2016, max compression
+gzip compressed data, was "dist/mongomotor-0.9b6.tar", last modified: Fri Aug 26 20:27:25 2016, max compression
```

## Comparing `mongomotor-0.9b5.tar` & `mongomotor-0.9b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-22 07:09:44.000000 mongomotor-0.9b5/
--rw-r--r--   0 juca      (1000) juca      (1000)       59 2016-08-22 07:09:44.000000 mongomotor-0.9b5/setup.cfg
--rw-r--r--   0 juca      (1000) juca      (1000)     1691 2016-08-20 13:16:28.000000 mongomotor-0.9b5/setup.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-22 07:09:44.000000 mongomotor-0.9b5/mongomotor/
--rw-r--r--   0 juca      (1000) juca      (1000)     2989 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/connection.py
--rw-r--r--   0 juca      (1000) juca      (1000)     8532 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/metaprogramming.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1095 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/utils.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3708 2016-08-22 06:55:01.000000 mongomotor-0.9b5/mongomotor/fields.py
--rw-r--r--   0 juca      (1000) juca      (1000)      836 2016-08-22 05:43:12.000000 mongomotor-0.9b5/mongomotor/exceptions.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3944 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/monkey.py
--rw-r--r--   0 juca      (1000) juca      (1000)     8373 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/core.py
--rw-r--r--   0 juca      (1000) juca      (1000)    23076 2016-08-22 05:44:19.000000 mongomotor-0.9b5/mongomotor/queryset.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1801 2016-08-16 02:45:46.000000 mongomotor-0.9b5/mongomotor/clients.py
--rw-r--r--   0 juca      (1000) juca      (1000)     6523 2016-08-16 08:16:58.000000 mongomotor-0.9b5/mongomotor/document.py
--rw-r--r--   0 juca      (1000) juca      (1000)      380 2016-08-22 07:03:32.000000 mongomotor-0.9b5/mongomotor/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1171 2016-08-22 07:09:44.000000 mongomotor-0.9b5/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      396 2016-08-19 11:37:59.000000 mongomotor-0.9b5/README
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-22 07:09:44.000000 mongomotor-0.9b5/mongomotor.egg-info/
--rw-r--r--   0 juca      (1000) juca      (1000)       11 2016-08-22 07:09:43.000000 mongomotor-0.9b5/mongomotor.egg-info/top_level.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       57 2016-08-22 07:09:43.000000 mongomotor-0.9b5/mongomotor.egg-info/requires.txt
--rw-r--r--   0 juca      (1000) juca      (1000)     1171 2016-08-22 07:09:43.000000 mongomotor-0.9b5/mongomotor.egg-info/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2016-08-22 07:09:43.000000 mongomotor-0.9b5/mongomotor.egg-info/dependency_links.txt
--rw-r--r--   0 juca      (1000) juca      (1000)      436 2016-08-22 07:09:43.000000 mongomotor-0.9b5/mongomotor.egg-info/SOURCES.txt
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-26 20:27:25.000000 mongomotor-0.9b6/
+-rw-r--r--   0 juca      (1000) juca      (1000)       59 2016-08-26 20:27:25.000000 mongomotor-0.9b6/setup.cfg
+-rw-r--r--   0 juca      (1000) juca      (1000)     1691 2016-08-20 13:16:28.000000 mongomotor-0.9b6/setup.py
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-26 20:27:25.000000 mongomotor-0.9b6/mongomotor/
+-rw-r--r--   0 juca      (1000) juca      (1000)     2989 2016-08-16 02:45:46.000000 mongomotor-0.9b6/mongomotor/connection.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     8532 2016-08-16 02:45:46.000000 mongomotor-0.9b6/mongomotor/metaprogramming.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1095 2016-08-16 02:45:46.000000 mongomotor-0.9b6/mongomotor/utils.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3708 2016-08-22 06:55:01.000000 mongomotor-0.9b6/mongomotor/fields.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      836 2016-08-22 05:43:12.000000 mongomotor-0.9b6/mongomotor/exceptions.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3944 2016-08-16 02:45:46.000000 mongomotor-0.9b6/mongomotor/monkey.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     8341 2016-08-26 16:44:37.000000 mongomotor-0.9b6/mongomotor/core.py
+-rw-r--r--   0 juca      (1000) juca      (1000)    29327 2016-08-26 20:19:21.000000 mongomotor-0.9b6/mongomotor/queryset.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1801 2016-08-16 02:45:46.000000 mongomotor-0.9b6/mongomotor/clients.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     8858 2016-08-26 19:46:40.000000 mongomotor-0.9b6/mongomotor/document.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      380 2016-08-26 20:26:41.000000 mongomotor-0.9b6/mongomotor/__init__.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1171 2016-08-26 20:27:25.000000 mongomotor-0.9b6/PKG-INFO
+-rw-r--r--   0 juca      (1000) juca      (1000)      396 2016-08-19 11:37:59.000000 mongomotor-0.9b6/README
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2016-08-26 20:27:25.000000 mongomotor-0.9b6/mongomotor.egg-info/
+-rw-r--r--   0 juca      (1000) juca      (1000)       11 2016-08-26 20:27:24.000000 mongomotor-0.9b6/mongomotor.egg-info/top_level.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)       57 2016-08-26 20:27:24.000000 mongomotor-0.9b6/mongomotor.egg-info/requires.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)     1171 2016-08-26 20:27:24.000000 mongomotor-0.9b6/mongomotor.egg-info/PKG-INFO
+-rw-r--r--   0 juca      (1000) juca      (1000)        1 2016-08-26 20:27:24.000000 mongomotor-0.9b6/mongomotor.egg-info/dependency_links.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)      436 2016-08-26 20:27:24.000000 mongomotor-0.9b6/mongomotor.egg-info/SOURCES.txt
```

### Comparing `mongomotor-0.9b5/setup.py` & `mongomotor-0.9b6/setup.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/connection.py` & `mongomotor-0.9b6/mongomotor/connection.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/metaprogramming.py` & `mongomotor-0.9b6/mongomotor/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/utils.py` & `mongomotor-0.9b6/mongomotor/utils.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/fields.py` & `mongomotor-0.9b6/mongomotor/fields.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/exceptions.py` & `mongomotor-0.9b6/mongomotor/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/monkey.py` & `mongomotor-0.9b6/mongomotor/monkey.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/core.py` & `mongomotor-0.9b6/mongomotor/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     # so I don't get a future as the return value and don't need to work
     # with mongoengine code.
     insert = OriginalDelegate()
     save = OriginalDelegate()
     update = OriginalDelegate()
     find_one = OriginalDelegate()
     find_and_modify = OriginalDelegate()
-    remove = OriginalDelegate()
     index_information = OriginalDelegate()
 
     def __init__(self, database, name):
 
         db_class = create_class_with_framework(
             MongoMotorAgnosticDatabase, self._framework, self.__module__)
```

### Comparing `mongomotor-0.9b5/mongomotor/queryset.py` & `mongomotor-0.9b6/mongomotor/queryset.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # along with mongomotor. If not, see <http://www.gnu.org/licenses/>.
 
 from bson.code import Code
 from bson import SON
 import functools
 import sys
 import textwrap
+from mongoengine import signals, DENY, CASCADE, NULLIFY, PULL
 from mongoengine.connection import get_db
 from mongoengine.document import MapReduceDocument
 from mongoengine.queryset.queryset import QuerySet as BaseQuerySet
 from mongoengine.errors import OperationError
 from motor.core import coroutine_annotation
 from mongomotor.exceptions import ConfusionError
 from mongomotor.metaprogramming import (get_future, AsyncGenericMetaclass,
@@ -33,15 +34,14 @@
 from mongomotor.monkey import MonkeyPatcher
 
 PY35 = sys.version_info[:2] >= (3, 5)
 
 
 class QuerySet(BaseQuerySet, metaclass=AsyncGenericMetaclass):
 
-    delete = Async()
     distinct = Async()
     explain = Async()
     in_bulk = Async()
     map_reduce = Async()
     modify = Async()
     update = Async()
 
@@ -187,14 +187,81 @@
                                        undo=False)
 
             future.add_done_callback(cb)
 
         return insert_future
 
     @coroutine_annotation
+    def delete(self, write_concern=None, _from_doc_delete=False,
+               cascade_refs=None):
+        """Deletes the documents matched by the query.
+
+        :param write_concern: Extra keyword arguments are passed down which
+            will be used as options for the resultant
+            ``getLastError`` command.  For example,
+            ``save(..., write_concern={w: 2, fsync: True}, ...)`` will
+            wait until at least two servers have recorded the write and
+            will force an fsync on the primary server.
+        :param _from_doc_delete: True when called from document delete
+          therefore signals will have been triggered so don't loop.
+
+        :returns number of deleted documents
+        """
+
+        queryset = self.clone()
+        doc = queryset._document
+
+        if write_concern is None:
+            write_concern = {}
+
+        # Handle deletes where skips or limits have been applied or
+        # there is an untriggered delete signal
+        has_delete_signal = signals.signals_available and (
+            signals.pre_delete.has_receivers_for(self._document) or
+            signals.post_delete.has_receivers_for(self._document))
+
+        call_document_delete = (queryset._skip or queryset._limit or
+                                has_delete_signal) and not _from_doc_delete
+
+        if call_document_delete:
+            async_method = asynchronize(self._document_delete)
+            return async_method(queryset, write_concern)
+
+        dr_future = self._check_delete_rules(doc, queryset, cascade_refs,
+                                             write_concern)
+
+        ret_future = get_future(self)
+
+        def dr_cb(dr_future):
+            """callback for _check_delete_rules future"""
+            try:
+                dr_future.result()
+
+                remove_future = queryset._collection.remove(
+                    queryset._query, **write_concern)
+
+                def r_cb(remove_future):
+                    """Callback for _collection.remove"""
+
+                    try:
+                        result = remove_future.result()
+                        if result:
+                            ret_future.set_result(result.get('n'))
+                    except Exception as e:
+                        ret_future.set_exception(e)
+
+                remove_future.add_done_callback(r_cb)
+
+            except Exception as e:
+                ret_future.set_exception(e)
+
+        dr_future.add_done_callback(dr_cb)
+        return ret_future
+
+    @coroutine_annotation
     def upsert_one(self, write_concern=None, **update):
         """Overwrite or add the first document matched by the query.
 
         :param write_concern: Extra keyword arguments are passed down which
             will be used as options for the resultant
             ``getLastError`` command.  For example,
             ``save(..., write_concern={w: 2, fsync: True}, ...)`` will
@@ -665,7 +732,98 @@
 
             out = SON(ordered_output)
 
         else:
             raise ConfusionError('Bad output type %r'.format(type(output)))
 
         return out
+
+    def _check_delete_rules(self, doc, queryset, cascade_refs, write_concern):
+        """Checks the delete rules for documents being deleted in a queryset.
+        Raises an exception if any document has a DENY rule."""
+
+        delete_rules = doc._meta.get('delete_rules') or {}
+        # Check for DENY rules before actually deleting/nullifying any other
+        # references
+        for rule_entry in delete_rules:
+            document_cls, field_name = rule_entry
+            if document_cls._meta.get('abstract'):
+                continue
+            rule = doc._meta['delete_rules'][rule_entry]
+            if rule == DENY and document_cls.objects(
+                    **{field_name + '__in': self}).count() > 0:
+                msg = ("Could not delete document (%s.%s refers to it)"
+                       % (document_cls.__name__, field_name))
+                raise OperationError(msg)
+
+        ret_future = get_future(self)
+
+        # We need to set result for the future if there's no rules otherwise
+        # the callbacks will never be called.
+        if not delete_rules:
+            ret_future.set_result(None)
+
+        for rule_entry in delete_rules:
+            document_cls, field_name = rule_entry
+            if document_cls._meta.get('abstract'):
+                continue
+            rule = doc._meta['delete_rules'][rule_entry]
+            if rule == CASCADE:
+                cascade_refs = set() if cascade_refs is None else cascade_refs
+                for ref in queryset:
+                    cascade_refs.add(ref.id)
+                ref_q = document_cls.objects(**{field_name + '__in': self,
+                                                'id__nin': cascade_refs})
+
+                ref_q_count_future = ref_q.count()
+
+                def count_cb(count_future):
+                    try:
+                        count = count_future.result()
+                        if count > 0:
+                            del_future = ref_q.delete(
+                                write_concern=write_concern,
+                                cascade_refs=cascade_refs)
+
+                            def del_cb(del_future):
+                                try:
+                                    r = del_future.result()
+                                    ret_future.set_result(r)
+                                except Exception as e:
+                                    ret_future.set_exception(e)
+
+                            del_future.add_done_callback(del_cb)
+                    except Exception as e:
+                        ret_future.set_exception(e)
+
+                ref_q_count_future.add_done_callback(count_cb)
+
+            elif rule in (NULLIFY, PULL):
+                if rule == NULLIFY:
+                    updatekw = {'unset__%s' % field_name: 1}
+                else:
+                    updatekw = {'pull_all__%s' % field_name: self}
+
+                update_future = document_cls.objects(
+                    **{field_name + '__in': self}).update(
+                        write_concern=write_concern, **updatekw)
+
+                def update_cb(update_future):
+                    try:
+                        result = update_future.result()
+                        ret_future.set_result(result)
+                    except Exception as e:
+                        ret_future.set_exception(e)
+
+                update_future.add_done_callback(update_cb)
+
+        return ret_future
+
+    def _document_delete(self, queryset, write_concern):
+        """Delete the documents in queryset by calling the document's delete
+        method."""
+
+        cnt = 0
+        for doc in queryset:
+            doc.delete(**write_concern)
+            cnt += 1
+        return cnt
```

### Comparing `mongomotor-0.9b5/mongomotor/clients.py` & `mongomotor-0.9b6/mongomotor/clients.py`

 * *Files identical despite different names*

### Comparing `mongomotor-0.9b5/mongomotor/document.py` & `mongomotor-0.9b6/mongomotor/document.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 # You should have received a copy of the GNU General Public License
 # along with mongomotor. If not, see <http://www.gnu.org/licenses/>.
 
 
 from mongoengine import (Document as DocumentBase,
                          DynamicDocument as DynamicDocumentBase)
+from mongoengine.errors import InvalidDocumentError, InvalidQueryError
 from mongomotor.fields import ReferenceField, ComplexBaseField
-from mongomotor.metaprogramming import AsyncDocumentMetaclass, Async, Sync
+from mongomotor.metaprogramming import (AsyncDocumentMetaclass, Async, Sync,
+                                        get_future)
 from mongomotor.queryset import QuerySet
 
 
 class Document(DocumentBase, metaclass=AsyncDocumentMetaclass):
     """The base class used for defining the structure and properties of
     collections of documents stored in MongoDB. Inherit from this class, and
     add fields as class attributes to define a document's structure.
@@ -115,25 +117,85 @@
                 field._auto_dereference = False
 
         super().__init__(*args, **kwargs)
         # and here we back things to normal
         for field, deref in fields:
             field._auto_dereference = deref
 
+    def modify(self, query={}, **update):
+        """Perform an atomic update of the document in the database and reload
+        the document object using updated version.
+
+        Returns True if the document has been updated or False if the document
+        in the database doesn't match the query.
+
+        .. note:: All unsaved changes that have been made to the document are
+            rejected if the method returns True.
+
+        :param query: the update will be performed only if the document in the
+            database matches the query
+        :param update: Django-style update keyword arguments
+        """
+
+        if self.pk is None:
+            raise InvalidDocumentError(
+                "The document does not have a primary key.")
+
+        id_field = self._meta["id_field"]
+        query = query.copy() if isinstance(
+            query, dict) else query.to_query(self)
+
+        if id_field not in query:
+            query[id_field] = self.pk
+        elif query[id_field] != self.pk:
+            msg = "Invalid document modify query: "
+            msg += "it must modify only this document."
+            raise InvalidQueryError(msg)
+
+        updated_future = self._qs(**query).modify(new=True, **update)
+        ret_future = get_future(self)
+
+        def updated_cb(updated_future):
+            try:
+                updated = updated_future.result()
+                if updated is None:
+                    ret_future.set_result(False)
+                    return
+
+                for field in self._fields_ordered:
+                    setattr(self, field, self._reload(field, updated[field]))
+
+                self._changed_fields = updated._changed_fields
+                self._created = False
+                ret_future.set_result(True)
+                return
+            except Exception as e:
+                ret_future.set_exception(e)
 
+        updated_future.add_done_callback(updated_cb)
+        return ret_future
 
     @classmethod
     def drop_collection(cls):
         """Drops the entire collection associated with this
         :class:`mongomotor.Document` type from the database.
         """
         cls._collection = None
         db = cls._get_db()
         return db.drop_collection(cls._get_collection_name())
 
+    @property
+    def _qs(self):
+        """
+        Returns the queryset to use for updating / reloading / deletions
+        """
+        if not hasattr(self, '__objects'):
+            self.__objects = QuerySet(self, self._get_collection())
+        return self.__objects
+
 
 class DynamicDocument(Document, DynamicDocumentBase,
                       metaclass=AsyncDocumentMetaclass):
 
     meta = {'abstract': True,
             'max_documents': None,
             'max_size': None,
```

### Comparing `mongomotor-0.9b5/PKG-INFO` & `mongomotor-0.9b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mongomotor
-Version: 0.9b5
+Version: 0.9b6
 Summary: 
 MongoMotor: An async document-object mapper for MongoDB
 
 Home-page: http://mongomotor.poraodojuca.net/
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: UNKNOWN
```

### Comparing `mongomotor-0.9b5/mongomotor.egg-info/PKG-INFO` & `mongomotor-0.9b6/mongomotor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mongomotor
-Version: 0.9b5
+Version: 0.9b6
 Summary: 
 MongoMotor: An async document-object mapper for MongoDB
 
 Home-page: http://mongomotor.poraodojuca.net/
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: UNKNOWN
```

