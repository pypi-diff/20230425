# Comparing `tmp/django_cookiebanner-0.2.7.tar.gz` & `tmp/django_cookiebanner-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cookiebanner-0.2.7.tar", max compression
+gzip compressed data, was "django_cookiebanner-0.2.8.tar", max compression
```

## Comparing `django_cookiebanner-0.2.7.tar` & `django_cookiebanner-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      192 2022-11-01 14:06:26.599958 django_cookiebanner-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2020-10-31 10:29:29.010957 django_cookiebanner-0.2.7/LICENSE
--rw-r--r--   0        0        0     2262 2022-09-27 08:08:47.993288 django_cookiebanner-0.2.7/README.md
--rw-r--r--   0        0        0        0 2020-03-23 14:12:30.195000 django_cookiebanner-0.2.7/cookiebanner/__init__.py
--rw-r--r--   0        0        0      517 2021-03-17 15:56:38.580897 django_cookiebanner-0.2.7/cookiebanner/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      897 2021-03-17 15:56:38.580897 django_cookiebanner-0.2.7/cookiebanner/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5780 2021-03-17 16:10:08.245939 django_cookiebanner-0.2.7/cookiebanner/templates/cookiebanner/bootstrap4.html
--rw-r--r--   0        0        0     6746 2021-10-06 13:17:34.167380 django_cookiebanner-0.2.7/cookiebanner/templates/cookiebanner/vanilla.html
--rw-r--r--   0        0        0     1826 2022-09-27 08:15:50.827690 django_cookiebanner-0.2.7/cookiebanner/templatetags/cookiebanner.py
--rw-r--r--   0        0        0      833 2022-11-01 14:07:03.285088 django_cookiebanner-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 django_cookiebanner-0.2.7/setup.py
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 django_cookiebanner-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-04-25 08:57:36.360489 django_cookiebanner-0.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2020-10-31 10:29:29.010957 django_cookiebanner-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2387 2023-04-25 08:53:44.662870 django_cookiebanner-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2020-03-23 14:12:30.195000 django_cookiebanner-0.2.8/cookiebanner/__init__.py
+-rw-r--r--   0        0        0      517 2021-03-17 15:56:38.580897 django_cookiebanner-0.2.8/cookiebanner/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      897 2021-03-17 15:56:38.580897 django_cookiebanner-0.2.8/cookiebanner/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5780 2021-03-17 16:10:08.245939 django_cookiebanner-0.2.8/cookiebanner/templates/cookiebanner/bootstrap4.html
+-rw-r--r--   0        0        0     7163 2023-04-25 08:52:00.316311 django_cookiebanner-0.2.8/cookiebanner/templates/cookiebanner/vanilla.html
+-rw-r--r--   0        0        0     1826 2023-04-25 08:45:07.397913 django_cookiebanner-0.2.8/cookiebanner/templatetags/cookiebanner.py
+-rw-r--r--   0        0        0      842 2023-04-25 08:56:19.958644 django_cookiebanner-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 django_cookiebanner-0.2.8/PKG-INFO
```

### Comparing `django_cookiebanner-0.2.7/LICENSE` & `django_cookiebanner-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cookiebanner-0.2.7/README.md` & `django_cookiebanner-0.2.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ```djangotemplate
 {% load cookiebanner %}
 ...
 <body>
 {% cookiebanner_modal 'vanilla' %}
 ...
 
+<button onclick="document.querySelector('#cookiebannerModal').classList.remove('hidden')">change cookie preferences</button>
 
 {% cookie_accepted 'analytics' as cookie_analytics %}
 {% if cookie_analytics %}
 <script>... javascript for matomo ...</script>
 {% endif %}
 </body>
 ```
```

#### html2text {}

```diff
@@ -12,14 +12,14 @@
 "description": _("This cookie prevents Cross-Site-Request-Forgery attacks."),
 }, { "pattern": "sessionid", "description": _("This cookie is necessary to
 allow logging in, for example."), }, ], }, { "id": "analytics", "name": _
 ("Analytics"), "optional": True, "cookies": [ { "pattern": "_pk_.*",
 "description": _("Matomo cookie for website analysis."), }, ], }, ], } ``` * In
 your base template add the banner and the conditionals: ```djangotemplate {%
 load cookiebanner %} ...
-{% cookiebanner_modal 'vanilla' %} ... {% cookie_accepted 'analytics' as
-cookie_analytics %} {% if cookie_analytics %}
+{% cookiebanner_modal 'vanilla' %} ... change cookie preferences {%
+cookie_accepted 'analytics' as cookie_analytics %} {% if cookie_analytics %}
  {% endif %}
 ``` ### Custom Template You can create a custom template and use that instead
 of the default one. * Create a folder `cookiebanner/` and a file in one of your
 `templates/`-folders, e.g.: `templates/cookiebanner/mytemplate.html` * Use `{%
 cookiebanner_modal 'mytemplate' %}`
```

### Comparing `django_cookiebanner-0.2.7/cookiebanner/locale/de/LC_MESSAGES/django.mo` & `django_cookiebanner-0.2.8/cookiebanner/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_cookiebanner-0.2.7/cookiebanner/locale/de/LC_MESSAGES/django.po` & `django_cookiebanner-0.2.8/cookiebanner/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_cookiebanner-0.2.7/cookiebanner/templates/cookiebanner/bootstrap4.html` & `django_cookiebanner-0.2.8/cookiebanner/templates/cookiebanner/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_cookiebanner-0.2.7/cookiebanner/templates/cookiebanner/vanilla.html` & `django_cookiebanner-0.2.8/cookiebanner/templates/cookiebanner/vanilla.html`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,32 @@
     </div>
   </div>
 </div>
 
 <script>
   const cookiegroups = JSON.parse("{{ cookiegroups_json|escapejs }}");
 
+  const _keyValue = document.cookie.match('(^|;) ?cookiebanner=([^;]*)(;|$)');
+  const cookiebannerCookie = _keyValue ? decodeURIComponent(_keyValue[2]) : null;
+  const cookiebannerModal = document.getElementById("cookiebannerModal");
+
   document.addEventListener("DOMContentLoaded", function () {
-    let keyValue = document.cookie.match('(^|;) ?cookiebanner=([^;]*)(;|$)');
-    let cookiebannerCookie = keyValue ? decodeURIComponent(keyValue[2]) : null;
-    if (cookiebannerCookie) return;
+    if (!cookiebannerCookie) cookiebannerModal.classList.remove('hidden');
+  });
 
-    document.getElementById("cookiebannerModal").classList.remove('hidden');
+  new IntersectionObserver(([e]) => {
+    if (cookiebannerCookie) {
+      try {
+        cookiebannerCookie.split(',').forEach((sec) =>
+          document.querySelector(`input[name="${sec}"]`).checked = true
+        )
+      } catch {
+        console.warn("having trouble parsing the cookiebannerCookie or settings the checkboxes")
+      }
+    }
 
     document.querySelectorAll("a[data-toggle='cookiebannerCollapse']").forEach((a) => {
       a.addEventListener("click", () =>
         document.querySelector(a.hash).classList.toggle('show')
       )
     })
 
@@ -86,15 +98,15 @@
         }
         const max_age = (365 * 24 * 60 * 60);
         const secure = window.location.hostname === 'localhost' ? "" : "secure";
         document.cookie = `cookiebanner=${encodeURIComponent(enable_cookies)}; path=/; max-age=${max_age}; ${secure}`;
         location.reload();
       })
     })
-  });
+  }).observe(cookiebannerModal);
 </script>
 
 <style>
   p {
     margin: 0 0 0.2em;
   }
```

### Comparing `django_cookiebanner-0.2.7/cookiebanner/templatetags/cookiebanner.py` & `django_cookiebanner-0.2.8/cookiebanner/templatetags/cookiebanner.py`

 * *Files identical despite different names*

### Comparing `django_cookiebanner-0.2.7/pyproject.toml` & `django_cookiebanner-0.2.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cookiebanner"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Andreas Nüßlein <andreas@nuessle.in>", "Ralph Delfs <ralph.delfs@sinnwerkstatt.com>"]
 readme = "README.md"
 license = "GPL-3.0+"
 repository = "https://github.com/sinnwerkstatt/django-cookiebanner"
 keywords = ["django", "cookie", "gdpr", "dsgvo"]
 include = ["CHANGELOG.md"]
@@ -20,15 +20,15 @@
 [tool.poetry.dev-dependencies]
 pytest-django = "*"
 pytest-cov = "*"
 black = "*"
 
 [tool.black]
 line-length = 88
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | migrations
   | static-collected
```

### Comparing `django_cookiebanner-0.2.7/PKG-INFO` & `django_cookiebanner-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookiebanner
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Home-page: https://github.com/sinnwerkstatt/django-cookiebanner
 License: GPL-3.0+
 Keywords: django,cookie,gdpr,dsgvo
 Author: Andreas Nüßlein
 Author-email: andreas@nuessle.in
 Requires-Python: >=3.7
@@ -81,14 +81,15 @@
 ```djangotemplate
 {% load cookiebanner %}
 ...
 <body>
 {% cookiebanner_modal 'vanilla' %}
 ...
 
+<button onclick="document.querySelector('#cookiebannerModal').classList.remove('hidden')">change cookie preferences</button>
 
 {% cookie_accepted 'analytics' as cookie_analytics %}
 {% if cookie_analytics %}
 <script>... javascript for matomo ...</script>
 {% endif %}
 </body>
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-cookiebanner Version: 0.2.7 Summary: Home-
+Metadata-Version: 2.1 Name: django-cookiebanner Version: 0.2.8 Summary: Home-
 page: https://github.com/sinnwerkstatt/django-cookiebanner License: GPL-3.0+
 Keywords: django,cookie,gdpr,dsgvo Author: Andreas NÃ¼Ãlein Author-email:
 andreas@nuessle.in Requires-Python: >=3.7 Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -22,14 +22,14 @@
 "csrftoken", "description": _("This cookie prevents Cross-Site-Request-Forgery
 attacks."), }, { "pattern": "sessionid", "description": _("This cookie is
 necessary to allow logging in, for example."), }, ], }, { "id": "analytics",
 "name": _("Analytics"), "optional": True, "cookies": [ { "pattern": "_pk_.*",
 "description": _("Matomo cookie for website analysis."), }, ], }, ], } ``` * In
 your base template add the banner and the conditionals: ```djangotemplate {%
 load cookiebanner %} ...
-{% cookiebanner_modal 'vanilla' %} ... {% cookie_accepted 'analytics' as
-cookie_analytics %} {% if cookie_analytics %}
+{% cookiebanner_modal 'vanilla' %} ... change cookie preferences {%
+cookie_accepted 'analytics' as cookie_analytics %} {% if cookie_analytics %}
  {% endif %}
 ``` ### Custom Template You can create a custom template and use that instead
 of the default one. * Create a folder `cookiebanner/` and a file in one of your
 `templates/`-folders, e.g.: `templates/cookiebanner/mytemplate.html` * Use `{%
 cookiebanner_modal 'mytemplate' %}`
```

