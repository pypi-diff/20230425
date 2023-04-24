# Comparing `tmp/django-admin-search-0.3.8.tar.gz` & `tmp/django-admin-search-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-search-0.3.8.tar", last modified: Wed Oct 13 17:01:38 2021, max compression
+gzip compressed data, was "django-admin-search-0.3.9.tar", last modified: Sat Nov  6 14:02:08 2021, max compression
```

## Comparing `django-admin-search-0.3.8.tar` & `django-admin-search-0.3.9.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1076 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/LICENSE
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      231 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/MANIFEST.in
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     6921 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/PKG-INFO
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4709 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/README.md
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      222 2021-10-13 17:00:17.000000 django-admin-search-0.3.8/django_admin_search/__init__.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4065 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/admin.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      259 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/apps.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/locale/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/locale/pt_BR/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      578 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1400 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       78 2021-10-13 17:01:32.000000 django-admin-search-0.3.8/django_admin_search/meta.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/static/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/css/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1381 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/css/styles.css
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)    86659 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery/jquery.min.js
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_mask/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     8327 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_mask/jquery.mask.min.js
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_modal/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3201 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.css
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4953 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.js
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search/templates/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/django_admin_search/templates/admin/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      184 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/templates/admin/custom_change_list.html
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      568 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/templates/admin/custom_fieldset.html
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3720 2021-10-13 17:01:26.000000 django-admin-search-0.3.8/django_admin_search/templates/admin/custom_search_form.html
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/django_admin_search/templatetags/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        0 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/templatetags/__init__.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      719 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/templatetags/advanced_search_form.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      583 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/django_admin_search/utils.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-10-13 17:01:38.756968 django-admin-search-0.3.8/django_admin_search.egg-info/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     6921 2021-10-13 17:01:38.000000 django-admin-search-0.3.8/django_admin_search.egg-info/PKG-INFO
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1166 2021-10-13 17:01:38.000000 django-admin-search-0.3.8/django_admin_search.egg-info/SOURCES.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        1 2021-10-13 17:01:38.000000 django-admin-search-0.3.8/django_admin_search.egg-info/dependency_links.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       93 2021-10-13 17:01:38.000000 django-admin-search-0.3.8/django_admin_search.egg-info/requires.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       25 2021-10-13 17:01:38.000000 django-admin-search-0.3.8/django_admin_search.egg-info/top_level.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      111 2021-10-13 17:01:38.760968 django-admin-search-0.3.8/setup.cfg
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1617 2021-06-08 06:58:42.000000 django-admin-search-0.3.8/setup.py
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1076 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/LICENSE
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      231 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/MANIFEST.in
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     6921 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/PKG-INFO
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4709 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/README.md
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      263 2021-11-06 14:01:37.000000 django-admin-search-0.3.9/django_admin_search/__init__.py
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4065 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/admin.py
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      259 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/apps.py
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.078182 django-admin-search-0.3.9/django_admin_search/locale/
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.078182 django-admin-search-0.3.9/django_admin_search/locale/pt_BR/
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      578 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1400 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.078182 django-admin-search-0.3.9/django_admin_search/static/
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/css/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1381 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/css/styles.css
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)    86659 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery/jquery.min.js
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_mask/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     8327 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_mask/jquery.mask.min.js
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_modal/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3201 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.css
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     4953 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.js
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/templates/
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/templates/admin/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      184 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/templates/admin/custom_change_list.html
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      568 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/templates/admin/custom_fieldset.html
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3720 2021-10-13 17:01:26.000000 django-admin-search-0.3.9/django_admin_search/templates/admin/custom_search_form.html
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search/templatetags/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        0 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/templatetags/__init__.py
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      719 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/templatetags/advanced_search_form.py
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      583 2021-06-08 06:58:42.000000 django-admin-search-0.3.9/django_admin_search/utils.py
+drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/django_admin_search.egg-info/
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     6921 2021-11-06 14:02:07.000000 django-admin-search-0.3.9/django_admin_search.egg-info/PKG-INFO
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1138 2021-11-06 14:02:07.000000 django-admin-search-0.3.9/django_admin_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        1 2021-11-06 14:02:07.000000 django-admin-search-0.3.9/django_admin_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       93 2021-11-06 14:02:07.000000 django-admin-search-0.3.9/django_admin_search.egg-info/requires.txt
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       25 2021-11-06 14:02:07.000000 django-admin-search-0.3.9/django_admin_search.egg-info/top_level.txt
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      111 2021-11-06 14:02:08.082183 django-admin-search-0.3.9/setup.cfg
+-rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1615 2021-11-06 13:59:06.000000 django-admin-search-0.3.9/setup.py
```

### Comparing `django-admin-search-0.3.8/LICENSE` & `django-admin-search-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/PKG-INFO` & `django-admin-search-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-search
-Version: 0.3.8
+Version: 0.3.9
 Summary: The "Django Admin Search" is a advanced search modal for django admin
 Home-page: https://github.com/shinneider/django_admin_search
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
 Description: Django Admin Search
         ===================
```

### Comparing `django-admin-search-0.3.8/README.md` & `django-admin-search-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/admin.py` & `django-admin-search-0.3.9/django_admin_search/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/locale/pt_BR/LC_MESSAGES/django.mo` & `django-admin-search-0.3.9/django_admin_search/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/locale/pt_BR/LC_MESSAGES/django.po` & `django-admin-search-0.3.9/django_admin_search/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/static/django_admin_search/css/styles.css` & `django-admin-search-0.3.9/django_admin_search/static/django_admin_search/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery/jquery.min.js` & `django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_mask/jquery.mask.min.js` & `django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_mask/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.css` & `django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.js` & `django-admin-search-0.3.9/django_admin_search/static/django_admin_search/jquery_modal/jquery.modal.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/templates/admin/custom_fieldset.html` & `django-admin-search-0.3.9/django_admin_search/templates/admin/custom_fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/templates/admin/custom_search_form.html` & `django-admin-search-0.3.9/django_admin_search/templates/admin/custom_search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/templatetags/advanced_search_form.py` & `django-admin-search-0.3.9/django_admin_search/templatetags/advanced_search_form.py`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search/utils.py` & `django-admin-search-0.3.9/django_admin_search/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-search-0.3.8/django_admin_search.egg-info/PKG-INFO` & `django-admin-search-0.3.9/django_admin_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-search
-Version: 0.3.8
+Version: 0.3.9
 Summary: The "Django Admin Search" is a advanced search modal for django admin
 Home-page: https://github.com/shinneider/django_admin_search
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
 Description: Django Admin Search
         ===================
```

### Comparing `django-admin-search-0.3.8/django_admin_search.egg-info/SOURCES.txt` & `django-admin-search-0.3.9/django_admin_search.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_admin_search/__init__.py
 django_admin_search/admin.py
 django_admin_search/apps.py
-django_admin_search/meta.py
 django_admin_search/utils.py
 django_admin_search.egg-info/PKG-INFO
 django_admin_search.egg-info/SOURCES.txt
 django_admin_search.egg-info/dependency_links.txt
 django_admin_search.egg-info/requires.txt
 django_admin_search.egg-info/top_level.txt
 django_admin_search/locale/pt_BR/LC_MESSAGES/django.mo
```

### Comparing `django-admin-search-0.3.8/setup.py` & `django-admin-search-0.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 from io import open
 
 from setuptools import find_packages, setup
 
-from django_admin_search.meta import VERSION
+from django_admin_search import __version__
 
 extras_require = {
     'dev': [
         'django',
         'django_mock_queries',
         'pylint',
         'pytest-pylint',
@@ -16,15 +16,15 @@
         'pytest-cov',
         'pytest-watch'
     ]
 }
 
 setup(
     name='django-admin-search',
-    version=str(VERSION),
+    version=__version__,
     description='The "Django Admin Search" is a advanced search modal for django admin',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Shinneider Libanio da Silva',
     author_email='shinneider-libanio@hotmail.com',
     url='https://github.com/shinneider/django_admin_search',
     license='MIT',
```

