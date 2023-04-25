# Comparing `tmp/huscy.project_consents-0.4.0a7.tar.gz` & `tmp/huscy.project_consents-0.4.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.4.0a7.tar", last modified: Mon Apr 24 10:37:45 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.4.0a8.tar", last modified: Tue Apr 25 09:19:42 2023, max compression
```

## Comparing `huscy.project_consents-0.4.0a7.tar` & `huscy.project_consents-0.4.0a8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a7/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-24 10:37:15.000000 huscy.project_consents-0.4.0a7/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a7/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-24 10:37:32.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-24 10:37:42.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/services.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      731 2023-04-21 09:45:41.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2919 2023-04-21 12:54:19.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      920 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-24 10:36:29.000000 huscy.project_consents-0.4.0a7/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a7/tests/test_viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a8/LICENSE
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-24 10:37:15.000000 huscy.project_consents-0.4.0a8/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a8/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-25 09:19:06.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/api_urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/0001_initial.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/services.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      731 2023-04-21 09:45:41.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/projectconsenttoken.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2937 2023-04-24 14:00:00.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      920 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/setup.cfg
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-24 10:36:29.000000 huscy.project_consents-0.4.0a8/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/tests/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/tests/test_project_consent_category_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/tests/test_project_consent_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a8/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a7/LICENSE` & `huscy.project_consents-0.4.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/PKG-INFO` & `huscy.project_consents-0.4.0a8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.4.0a7
+Version: 0.4.0a8
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/forms.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/0001_initial.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-04-24 10:37
+# Generated by Django 4.2 on 2023-04-25 09:19
 
 from django.db import migrations, models
 import django.db.models.deletion
 import uuid
 
 
 class Migration(migrations.Migration):
```

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/models.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/serializer.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/services.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html` & `huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/projectconsenttoken.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/views.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,16 @@
             project=form.cleaned_data.get('project'),
             subject=form.cleaned_data.get('subject'),
         )
         return HttpResponseRedirect(
             '{}?token={}'.format(reverse('create-project-consent-token'), token.id)
         )
 
-    def get_context_data(self):
-        context = super().get_context_data()
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
         if 'token' in self.request.GET:
             token = get_object_or_404(ProjectConsentToken, pk=self.request.GET.get('token'))
             context['sign_project_consent_url'] = '{protocol}://{host}{url}'.format(
                 protocol=self.request.scheme,
                 host=self.request.get_host(),
                 url=reverse('sign-project-consent', kwargs=dict(token=token.id))
             )
```

### Comparing `huscy.project_consents-0.4.0a7/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.4.0a8/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.4.0a7
+Version: 0.4.0a8
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/setup.py` & `huscy.project_consents-0.4.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.4.0a8/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.4.0a8/tests/test_project_consent_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a7/tests/test_viewsets.py` & `huscy.project_consents-0.4.0a8/tests/test_viewsets.py`

 * *Files identical despite different names*

