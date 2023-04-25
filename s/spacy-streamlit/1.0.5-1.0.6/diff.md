# Comparing `tmp/spacy_streamlit-1.0.5.tar.gz` & `tmp/spacy_streamlit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_streamlit-1.0.5.tar", last modified: Mon Feb 27 08:34:07 2023, max compression
+gzip compressed data, was "spacy_streamlit-1.0.6.tar", last modified: Tue Apr 25 08:00:11 2023, max compression
```

## Comparing `spacy_streamlit-1.0.5.tar` & `spacy_streamlit-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-27 08:34:07.041283 spacy_streamlit-1.0.5/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)    22586 2023-02-27 08:34:07.041283 spacy_streamlit-1.0.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    22279 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-02-27 08:34:07.041283 spacy_streamlit-1.0.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      175 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-27 08:34:07.037283 spacy_streamlit-1.0.5/spacy_streamlit/
--rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/spacy_streamlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3147 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/spacy_streamlit/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14988 2023-02-27 08:33:35.000000 spacy_streamlit-1.0.5/spacy_streamlit/visualizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-27 08:34:07.041283 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    22586 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      346 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-27 08:34:07.000000 spacy_streamlit-1.0.5/spacy_streamlit.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-25 08:00:11.301076 spacy_streamlit-1.0.6/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)    22586 2023-04-25 08:00:11.301076 spacy_streamlit-1.0.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    22279 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-04-25 08:00:11.301076 spacy_streamlit-1.0.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      175 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-25 08:00:11.301076 spacy_streamlit-1.0.6/spacy_streamlit/
+-rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/spacy_streamlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3053 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/spacy_streamlit/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14988 2023-04-25 08:00:00.000000 spacy_streamlit-1.0.6/spacy_streamlit/visualizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-25 08:00:11.301076 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    22586 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      346 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-25 08:00:11.000000 spacy_streamlit-1.0.6/spacy_streamlit.egg-info/zip-safe
```

### Comparing `spacy_streamlit-1.0.5/LICENSE` & `spacy_streamlit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_streamlit-1.0.5/PKG-INFO` & `spacy_streamlit-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy_streamlit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Visualize spaCy with streamlit
 Home-page: https://github.com/explosion/spacy-streamlit
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy_streamlit Version: 1.0.5 Summary: Visualize
+Metadata-Version: 2.1 Name: spacy_streamlit Version: 1.0.6 Summary: Visualize
 spaCy with streamlit Home-page: https://github.com/explosion/spacy-streamlit
 Author: Explosion Author-email: contact@explosion.ai License: MIT Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 [https://explosion.ai/assets/img/logo.svg] # spacy-streamlit: spaCy building
 blocks for Streamlit apps This package contains utilities for visualizing
 [spaCy](https://spacy.io) models and building interactive spaCy-powered apps
 with [Streamlit](https://streamlit.io). It includes various building blocks you
```

### Comparing `spacy_streamlit-1.0.5/README.md` & `spacy_streamlit-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spacy_streamlit-1.0.5/setup.cfg` & `spacy_streamlit-1.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
-version = 1.0.5
+version = 1.0.6
 description = Visualize spaCy with streamlit
 url = https://github.com/explosion/spacy-streamlit
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = true
 python_requires = >=3.6
 install_requires = 
-	streamlit>=0.86.0
+	streamlit>=1.18.0
 	spacy>=3.0.0,<4.0.0
 	pandas
 
 [flake8]
 ignore = E203, E266, E501, E731, W503, E741
 max-line-length = 80
 select = B,C,E,F,W,T4,B9
```

### Comparing `spacy_streamlit-1.0.5/spacy_streamlit/util.py` & `spacy_streamlit-1.0.6/spacy_streamlit/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import streamlit as st
 import spacy
 import base64
 
 
-@st.cache(allow_output_mutation=True, suppress_st_warning=True)
+@st.cache_resource
 def load_model(name: str) -> spacy.language.Language:
     """Load a spaCy model."""
     return spacy.load(name)
 
 
-@st.cache(allow_output_mutation=True, suppress_st_warning=True)
+@st.cache_data
 def process_text(model_name: str, text: str) -> spacy.tokens.Doc:
     """Process a text and create a Doc object."""
     nlp = load_model(model_name)
     return nlp(text)
 
 
 def get_svg(svg: str, style: str = "", wrap: bool = True):
```

### Comparing `spacy_streamlit-1.0.5/spacy_streamlit/visualizer.py` & `spacy_streamlit-1.0.6/spacy_streamlit/visualizer.py`

 * *Files identical despite different names*

### Comparing `spacy_streamlit-1.0.5/spacy_streamlit.egg-info/PKG-INFO` & `spacy_streamlit-1.0.6/spacy_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-streamlit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Visualize spaCy with streamlit
 Home-page: https://github.com/explosion/spacy-streamlit
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-streamlit Version: 1.0.5 Summary: Visualize
+Metadata-Version: 2.1 Name: spacy-streamlit Version: 1.0.6 Summary: Visualize
 spaCy with streamlit Home-page: https://github.com/explosion/spacy-streamlit
 Author: Explosion Author-email: contact@explosion.ai License: MIT Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 [https://explosion.ai/assets/img/logo.svg] # spacy-streamlit: spaCy building
 blocks for Streamlit apps This package contains utilities for visualizing
 [spaCy](https://spacy.io) models and building interactive spaCy-powered apps
 with [Streamlit](https://streamlit.io). It includes various building blocks you
```

