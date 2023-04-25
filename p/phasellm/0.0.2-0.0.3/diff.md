# Comparing `tmp/phasellm-0.0.2.tar.gz` & `tmp/phasellm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.2.tar", last modified: Mon Apr 24 16:34:50 2023, max compression
+gzip compressed data, was "phasellm-0.0.3.tar", last modified: Tue Apr 25 05:59:21 2023, max compression
```

## Comparing `phasellm-0.0.2.tar` & `phasellm-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-24 16:33:56.000000 phasellm-0.0.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-24 16:34:50.928490 phasellm-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4632 2023-04-24 16:33:56.000000 phasellm-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/eval/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3500 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/eval/eval.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/llms/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/llms/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/llms/llms.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-24 16:34:50.928490 phasellm-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-24 16:34:41.000000 phasellm-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-25 05:58:31.000000 phasellm-0.0.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-25 05:59:21.888495 phasellm-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-04-25 05:58:31.000000 phasellm-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/eval/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3500 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/eval/eval.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/llms/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/llms/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13829 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/llms/llms.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 05:59:21.888495 phasellm-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-25 05:59:11.000000 phasellm-0.0.3/setup.py
```

### Comparing `phasellm-0.0.2/LICENSE` & `phasellm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.2/PKG-INFO` & `phasellm-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.2/README.md` & `phasellm-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 You can install PhaseLLM via pip:
 
 ```
 pip install phasellm
 ```
 
+Installing from PyPI does not download the sample demos and products in the `demos-and-products` folder. Clone this repository and follow instructions in the `README.md` file in each product folder to run those.
+
 ## Introduction
 
 The coming months and years will bring thousands of new products and experienced powered by large language models (LLMs) like ChatGPT or its increasing number of variants. Whether you're using OpenAI's ChatGPT, Anthropic's Claude, or something else all together, you'll want to test how well your models and prompts perform against user needs. As more models are launched, you'll also have a bigger range of options.
 
 PhaseLLM is a framework designed to help manage and test LLM-driven experiences -- products, content, or other experiences that product and brand managers might be driving for their users.
 
 Here's what PhaseLLM does:
```

### Comparing `phasellm-0.0.2/phasellm/eval/eval.py` & `phasellm-0.0.3/phasellm/eval/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.2/phasellm/llms/llms.py` & `phasellm-0.0.3/phasellm/llms/llms.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
         prompt_text = _clean_messages_to_prompt(messages)
         if append_role is not None and len(append_role) > 0:
             prompt_text += f"\n{append_role}: "
 
         r_data = {"prompt": prompt_text,
                   "model": self.model,
-                  "max_tokens_to_sample": 300, 
+                  "max_tokens_to_sample": 500,
                   "stop_sequences": _get_stop_sequences_from_messages(messages)
                 }
 
         resp = requests.post("https://api.anthropic.com/v1/complete", headers=r_headers, json=r_data)
         completion = json.loads(resp.text)["completion"].strip()
 
         return completion
@@ -245,14 +245,15 @@
         """
         Completes text based on provided prompt.
         """
 
         r_headers = {"X-API-Key":self.apikey, "Accept":"application/json"}
         r_data = {"prompt": prompt,
                   "model": self.model,
+                  "max_tokens_to_sample": 500,
                   "stop_sequences": stop_sequences
                 }
 
         resp = requests.post("https://api.anthropic.com/v1/complete", headers=r_headers, json=r_data)
         completion = json.loads(resp.text)["completion"].strip()
         return completion
```

### Comparing `phasellm-0.0.2/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.3/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.2/setup.py` & `phasellm-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

