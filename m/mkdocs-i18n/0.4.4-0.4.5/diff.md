# Comparing `tmp/mkdocs-i18n-0.4.4.tar.gz` & `tmp/mkdocs-i18n-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-i18n-0.4.4.tar", last modified: Tue Feb 15 17:28:58 2022, max compression
+gzip compressed data, was "mkdocs-i18n-0.4.5.tar", last modified: Tue Apr 25 11:19:18 2023, max compression
```

## Comparing `mkdocs-i18n-0.4.4.tar` & `mkdocs-i18n-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-15 17:28:58.831860 mkdocs-i18n-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)    34523 2022-02-15 17:28:48.000000 mkdocs-i18n-0.4.4/COPYING
--rw-r--r--   0 root         (0) root         (0)     3889 2022-02-15 17:28:58.831860 mkdocs-i18n-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2938 2022-02-15 17:28:48.000000 mkdocs-i18n-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-15 17:28:58.828860 mkdocs-i18n-0.4.4/mkdocs_i18n/
--rwxrwxrwx   0 root         (0) root         (0)    10750 2022-02-15 17:28:48.000000 mkdocs-i18n-0.4.4/mkdocs_i18n/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-15 17:28:58.830860 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3889 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      262 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      120 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-02-15 17:28:58.000000 mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-15 17:28:58.831860 mkdocs-i18n-0.4.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2517 2022-02-15 17:28:48.000000 mkdocs-i18n-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/COPYING
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.519130 mkdocs-i18n-0.4.5/mkdocs_i18n/
+-rwxrwxrwx   0 root         (0) root         (0)    10722 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/mkdocs_i18n/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:19:18.522131 mkdocs-i18n-0.4.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2517 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/setup.py
```

### Comparing `mkdocs-i18n-0.4.4/COPYING` & `mkdocs-i18n-0.4.5/COPYING`

 * *Files identical despite different names*

### Comparing `mkdocs-i18n-0.4.4/PKG-INFO` & `mkdocs-i18n-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-i18n
-Version: 0.4.4
+Version: 0.4.5
 Summary: MkDocs i18n plugin
 Home-page: https://gitlab.com/mkdocs-i18n/mkdocs-i18n
 Author: Simó Albert i Beltran
 Author-email: sim6@bona.gent
 License: AGPL-3.0-or-later
 Project-URL: Bug Reports, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues
 Project-URL: Funding, https://liberapay.com/mkdocs-i18n/donate
```

### Comparing `mkdocs-i18n-0.4.4/README.md` & `mkdocs-i18n-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-i18n-0.4.4/mkdocs_i18n/__init__.py` & `mkdocs-i18n-0.4.5/mkdocs_i18n/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     config_scheme = (
         ("languages", Type(dict, required=True)),
         ("default_language", Type(str, required=True)),
         ("no_translation", Type(dict, default={})),
         ("translate_nav", Type(dict, default={})),
     )
 
-    # pylint: disable=no-self-use
     def on_config(self, config):
         """Adds attr_list markdown extension to configuration
 
         https://www.mkdocs.org/user-guide/plugins/#on_config
 
         :param config: global configuration object
         :return: global configuration object
@@ -111,15 +110,15 @@
                     "lang_name": lang_name,
                     "url": url,
                 }
             )
         return language_alternate
 
     # pylint: disable=unused-argument
-    def on_page_markdown(self, markdown, page, config, files):
+    def on_page_markdown(self, markdown, *, page, config, files):
         """Adds a list of configured languages at the top of page with links
         to translated pages
 
         https://www.mkdocs.org/user-guide/plugins/#on_page_markdown
 
         :param markdown: Markdown source text of page as string
         :param page: `mkdocs.nav.Page` instance
@@ -233,15 +232,15 @@
                             item.title = f"{item.title} ({page_lang_name})"
                 else:
                     item.title = self._translate_title(item.title, lang)
             if item.is_section:
                 self._translate_nav_items(item.children, lang)
 
     # pylint: disable=unused-argument
-    def on_page_context(self, context, page, config, nav):
+    def on_page_context(self, context, *, page, config, nav):
         """Removes from navigation pages of other languages if there is a page
         with current language
 
         https://www.mkdocs.org/user-guide/plugins/#on_page_context
 
         :param context: dict of template context variables
         :param page: `mkdocs.nav.Page` instance
```

### Comparing `mkdocs-i18n-0.4.4/mkdocs_i18n.egg-info/PKG-INFO` & `mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-i18n
-Version: 0.4.4
+Version: 0.4.5
 Summary: MkDocs i18n plugin
 Home-page: https://gitlab.com/mkdocs-i18n/mkdocs-i18n
 Author: Simó Albert i Beltran
 Author-email: sim6@bona.gent
 License: AGPL-3.0-or-later
 Project-URL: Bug Reports, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues
 Project-URL: Funding, https://liberapay.com/mkdocs-i18n/donate
```

### Comparing `mkdocs-i18n-0.4.4/setup.py` & `mkdocs-i18n-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from setuptools import find_packages, setup
 
 here = Path(__file__).parent.resolve()
 
 setup(
     name="mkdocs-i18n",
-    version="0.4.4",
+    version="0.4.5",
     description="MkDocs i18n plugin",
     long_description=(here / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://gitlab.com/mkdocs-i18n/mkdocs-i18n",
     author="Simó Albert i Beltran",
     author_email="sim6@bona.gent",
     classifiers=[
```

