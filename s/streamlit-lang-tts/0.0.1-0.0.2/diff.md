# Comparing `tmp/streamlit_lang_tts-0.0.1.tar.gz` & `tmp/streamlit_lang_tts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_lang_tts-0.0.1.tar", last modified: Mon Apr 24 13:18:04 2023, max compression
+gzip compressed data, was "streamlit_lang_tts-0.0.2.tar", last modified: Mon Apr 24 22:03:58 2023, max compression
```

## Comparing `streamlit_lang_tts-0.0.1.tar` & `streamlit_lang_tts-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.164149 streamlit_lang_tts-0.0.1/
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1063 2023-04-23 15:06:28.000000 streamlit_lang_tts-0.0.1/LICENSE
--rw-r--r--   0 ryanrapp   (501) staff       (20)       54 2023-04-24 13:06:22.000000 streamlit_lang_tts-0.0.1/MANIFEST.in
--rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 13:18:04.164033 streamlit_lang_tts-0.0.1/PKG-INFO
--rw-r--r--   0 ryanrapp   (501) staff       (20)       38 2023-04-24 13:18:04.164181 streamlit_lang_tts-0.0.1/setup.cfg
--rw-r--r--   0 ryanrapp   (501) staff       (20)      636 2023-04-24 13:10:58.000000 streamlit_lang_tts-0.0.1/setup.py
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.158039 streamlit_lang_tts-0.0.1/streamlit_lang_tts/
--rw-r--r--   0 ryanrapp   (501) staff       (20)     3491 2023-04-24 13:15:36.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/__init__.py
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.157374 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.159788 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/
--rw-r--r--   0 ryanrapp   (501) staff       (20)      691 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/asset-manifest.json
--rw-r--r--   0 ryanrapp   (501) staff       (20)   197459 2023-04-23 18:28:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/bootstrap.min.css
--rw-r--r--   0 ryanrapp   (501) staff       (20)     2081 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/index.html
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.157477 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.163806 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/
--rw-r--r--   0 ryanrapp   (501) staff       (20)   464201 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     2059 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.LICENSE.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)  1710252 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.map
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1852 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     6708 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js.map
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1578 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     8363 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 13:18:04.158749 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/
--rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 13:18:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/PKG-INFO
--rw-r--r--   0 ryanrapp   (501) staff       (20)      907 2023-04-24 13:18:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/SOURCES.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)        1 2023-04-24 13:18:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/dependency_links.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)       16 2023-04-24 13:18:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/requires.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)       19 2023-04-24 13:18:04.000000 streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/top_level.txt
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.820496 streamlit_lang_tts-0.0.2/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     1063 2023-04-23 15:06:28.000000 streamlit_lang_tts-0.0.2/LICENSE
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       54 2023-04-24 13:06:22.000000 streamlit_lang_tts-0.0.2/MANIFEST.in
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 22:03:58.820380 streamlit_lang_tts-0.0.2/PKG-INFO
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       38 2023-04-24 22:03:58.820528 streamlit_lang_tts-0.0.2/setup.cfg
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      636 2023-04-24 22:03:07.000000 streamlit_lang_tts-0.0.2/setup.py
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.814578 streamlit_lang_tts-0.0.2/streamlit_lang_tts/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     3514 2023-04-24 21:05:11.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/__init__.py
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.813898 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.816312 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      691 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/asset-manifest.json
+-rw-r--r--   0 ryanrapp   (501) staff       (20)   197459 2023-04-23 18:28:04.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/bootstrap.min.css
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     2081 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/index.html
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.813998 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.820189 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)   464201 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     2059 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.LICENSE.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)  1710252 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.map
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     1852 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     6708 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js.map
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     1578 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     8363 2023-04-23 18:28:06.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:03:58.815345 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 22:03:58.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/PKG-INFO
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      907 2023-04-24 22:03:58.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)        1 2023-04-24 22:03:58.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       16 2023-04-24 22:03:58.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/requires.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       19 2023-04-24 22:03:58.000000 streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/top_level.txt
```

### Comparing `streamlit_lang_tts-0.0.1/LICENSE` & `streamlit_lang_tts-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/setup.py` & `streamlit_lang_tts-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_lang_tts",
-    version="0.0.1",
+    version="0.0.2",
     author="Ryan Rapp",
     author_email="skies_midair0f@icloud.com",
     description="Streamlit extensions for text-to-speech",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/__init__.py` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
-def speak_text(name='', translation='', default='', key=None):
+def speak_text(name='', label='', translation='', default='', key=None):
     """Create a new instance of "my_component".
 
     Parameters
     ----------
     name: str
         The name of the thing we're saying hello to. The component will display
         the text "Hello, {name}!"
@@ -66,12 +66,12 @@
     """
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
-    component_value = _component_func(name=name, translation=translation, key=key, default=default)
+    component_value = _component_func(name=name, label=label, translation=translation, key=key, default=default)
 
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
```

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/asset-manifest.json` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/bootstrap.min.css` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/index.html` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.LICENSE.txt` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.map` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/2.d7bda64d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js.map` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/main.2cce2544.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.1/streamlit_lang_tts.egg-info/SOURCES.txt` & `streamlit_lang_tts-0.0.2/streamlit_lang_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

