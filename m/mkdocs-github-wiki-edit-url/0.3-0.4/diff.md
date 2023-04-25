# Comparing `tmp/mkdocs-github-wiki-edit-url-0.3.tar.gz` & `tmp/mkdocs-github-wiki-edit-url-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-github-wiki-edit-url-0.3.tar", last modified: Mon May 23 05:39:48 2022, max compression
+gzip compressed data, was "mkdocs-github-wiki-edit-url-0.4.tar", last modified: Tue Apr 25 12:36:05 2023, max compression
```

## Comparing `mkdocs-github-wiki-edit-url-0.3.tar` & `mkdocs-github-wiki-edit-url-0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-05-23 05:39:48.870024 mkdocs-github-wiki-edit-url-0.3/
--rw-rw-rw-   0        0        0      827 2022-05-23 05:39:48.870024 mkdocs-github-wiki-edit-url-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      528 2022-05-23 05:19:35.000000 mkdocs-github-wiki-edit-url-0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-05-23 05:39:48.869023 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/
--rw-rw-rw-   0        0        0      827 2022-05-23 05:39:48.000000 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2022-05-23 05:39:48.000000 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-23 05:39:48.000000 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2022-05-23 05:39:48.000000 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2022-05-23 05:39:48.000000 mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-23 05:39:48.870024 mkdocs-github-wiki-edit-url-0.3/setup.cfg
--rw-rw-rw-   0        0        0      560 2022-05-23 05:39:44.000000 mkdocs-github-wiki-edit-url-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:36:05.015514 mkdocs-github-wiki-edit-url-0.4/
+-rw-rw-rw-   0        0        0      802 2023-04-25 12:36:05.014512 mkdocs-github-wiki-edit-url-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2022-05-23 05:19:35.000000 mkdocs-github-wiki-edit-url-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 12:36:05.000514 mkdocs-github-wiki-edit-url-0.4/github_wiki_edit_url/
+-rw-rw-rw-   0        0        0       73 2022-05-22 11:42:25.000000 mkdocs-github-wiki-edit-url-0.4/github_wiki_edit_url/__init__.py
+-rw-rw-rw-   0        0        0      701 2022-05-22 18:41:29.000000 mkdocs-github-wiki-edit-url-0.4/github_wiki_edit_url/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:36:05.013513 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/
+-rw-rw-rw-   0        0        0      802 2023-04-25 12:36:04.000000 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 12:36:04.000000 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 12:36:04.000000 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-25 12:36:04.000000 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-25 12:36:04.000000 mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 12:36:05.015514 mkdocs-github-wiki-edit-url-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      580 2023-04-25 12:35:48.000000 mkdocs-github-wiki-edit-url-0.4/setup.py
```

### Comparing `mkdocs-github-wiki-edit-url-0.3/PKG-INFO` & `mkdocs-github-wiki-edit-url-0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: mkdocs-github-wiki-edit-url
-Version: 0.3
+Version: 0.4
 Summary: Use Edit URLs compatible with GitHub Wiki
 Home-page: https://github.com/MichelZ/mkdocs-github-wiki-edit-url
 Author: Michel Zehnder
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT
 Description-Content-Type: text/markdown
 
 # MKDocs GitHub Wiki Edit Url Support
 
 This plugin is to enable mkdocs to produce output that uses the GitHub Wiki-style edit URL's, e.g. https://github.com/project/repo/wiki/some/path/_edit  
 You will need to set repo_url to your wiki URL, e.g. https://github.com/project/repo/wiki. The plugin will use repo_url/<path>/_edit as the URL style.
 
@@ -19,8 +18,7 @@
 - Add the plugin to your `mkdocs.yml`, e.g.:
 ``` 
 plugins:
   - search
   - ezlinks
   - github-wiki-edit-url
 ```
-
```

### Comparing `mkdocs-github-wiki-edit-url-0.3/README.md` & `mkdocs-github-wiki-edit-url-0.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-github-wiki-edit-url-0.3/mkdocs_github_wiki_edit_url.egg-info/PKG-INFO` & `mkdocs-github-wiki-edit-url-0.4/mkdocs_github_wiki_edit_url.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: mkdocs-github-wiki-edit-url
-Version: 0.3
+Version: 0.4
 Summary: Use Edit URLs compatible with GitHub Wiki
 Home-page: https://github.com/MichelZ/mkdocs-github-wiki-edit-url
 Author: Michel Zehnder
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT
 Description-Content-Type: text/markdown
 
 # MKDocs GitHub Wiki Edit Url Support
 
 This plugin is to enable mkdocs to produce output that uses the GitHub Wiki-style edit URL's, e.g. https://github.com/project/repo/wiki/some/path/_edit  
 You will need to set repo_url to your wiki URL, e.g. https://github.com/project/repo/wiki. The plugin will use repo_url/<path>/_edit as the URL style.
 
@@ -19,8 +18,7 @@
 - Add the plugin to your `mkdocs.yml`, e.g.:
 ``` 
 plugins:
   - search
   - ezlinks
   - github-wiki-edit-url
 ```
-
```

### Comparing `mkdocs-github-wiki-edit-url-0.3/setup.py` & `mkdocs-github-wiki-edit-url-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import setuptools
 
 setuptools.setup(
     name="mkdocs-github-wiki-edit-url",
-    version='0.3',
+    version='0.4',
     url='https://github.com/MichelZ/mkdocs-github-wiki-edit-url',
     author='Michel Zehnder',
+    license='MIT',
     description='Use Edit URLs compatible with GitHub Wiki',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     entry_points={
         'mkdocs.plugins': [
             'github-wiki-edit-url=github_wiki_edit_url.plugin:GithubWikiEditUrlPlugin'
         ]
```

