# Comparing `tmp/llmwrite-0.1.4.tar.gz` & `tmp/llmwrite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmwrite-0.1.4.tar", max compression
+gzip compressed data, was "llmwrite-0.1.5.tar", max compression
```

## Comparing `llmwrite-0.1.4.tar` & `llmwrite-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 llmwrite-0.1.4/LICENSE
--rw-r--r--   0        0        0      888 2023-04-14 16:45:09.409762 llmwrite-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 llmwrite-0.1.4/llmwrite/__init__.py
--rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 llmwrite-0.1.4/llmwrite/accepted_language.py
--rw-r--r--   0        0        0     4489 2023-04-25 10:01:18.125732 llmwrite-0.1.4/llmwrite/core.py
--rw-r--r--   0        0        0     1119 2023-04-15 03:22:27.871876 llmwrite-0.1.4/llmwrite/lang_conf.py
--rw-r--r--   0        0        0     1030 2023-04-15 18:25:58.177088 llmwrite-0.1.4/llmwrite/locales/messages.en.yaml
--rw-r--r--   0        0        0     1302 2023-04-15 18:25:33.664997 llmwrite-0.1.4/llmwrite/locales/messages.ja.yaml
--rwxr-xr-x   0        0        0     1858 2023-04-25 10:01:31.073161 llmwrite-0.1.4/llmwrite/main.py
--rw-r--r--   0        0        0     2644 2023-04-15 19:23:30.754745 llmwrite-0.1.4/llmwrite/prompts.py
--rw-r--r--   0        0        0     2773 2023-04-25 10:01:46.596492 llmwrite-0.1.4/llmwrite/questionary_ui.py
--rw-r--r--   0        0        0      852 2023-04-25 10:00:49.404987 llmwrite-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 llmwrite-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 llmwrite-0.1.5/LICENSE
+-rw-r--r--   0        0        0      940 2023-04-25 11:16:03.003865 llmwrite-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 llmwrite-0.1.5/llmwrite/__init__.py
+-rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 llmwrite-0.1.5/llmwrite/accepted_language.py
+-rw-r--r--   0        0        0     4489 2023-04-25 10:01:18.125732 llmwrite-0.1.5/llmwrite/core.py
+-rw-r--r--   0        0        0     1119 2023-04-15 03:22:27.871876 llmwrite-0.1.5/llmwrite/lang_conf.py
+-rw-r--r--   0        0        0     1030 2023-04-15 18:25:58.177088 llmwrite-0.1.5/llmwrite/locales/messages.en.yaml
+-rw-r--r--   0        0        0     1302 2023-04-15 18:25:33.664997 llmwrite-0.1.5/llmwrite/locales/messages.ja.yaml
+-rwxr-xr-x   0        0        0     1858 2023-04-25 10:01:31.073161 llmwrite-0.1.5/llmwrite/main.py
+-rw-r--r--   0        0        0     2644 2023-04-15 19:23:30.754745 llmwrite-0.1.5/llmwrite/prompts.py
+-rw-r--r--   0        0        0     2773 2023-04-25 10:01:46.596492 llmwrite-0.1.5/llmwrite/questionary_ui.py
+-rw-r--r--   0        0        0      852 2023-04-25 11:17:11.796959 llmwrite-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 llmwrite-0.1.5/PKG-INFO
```

### Comparing `llmwrite-0.1.4/LICENSE` & `llmwrite-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/README.md` & `llmwrite-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# GPT-Write :writing_hand:
+# LLM-Write (powered by GPT-3) :writing_hand:
 
-__GPT make writing an article brazing fast :fire:.__
+__LLM make writing an article brazing fast :fire:.__
 
 PyPi:
-- https://pypi.org/project/gptwrite/
+- https://pypi.org/project/llmwrite/
 
-![GPT-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
+![LLM-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
 
 ## :telescope: Overview
-- GPT-Write is the CLI tool for Intractive Automated Article Writing.  
+- This app is built with GPT-3.
+- LLM-Write is the CLI tool for Intractive Automated Article Writing.  
 - You can create articles, just answer the questions.   
-- Since the language is specified in the GPT prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.  
+- Since the language is specified in the LLM prompt and LLM is allowed to generate the text, it could theoretically be used in a variety of languages.  
     - However, the supported languages in the shell messages are only English and Japanese.
 
 
 ## :runner: Installation
 ```sh
-pip install gptwrite
+pip install llmwrite
 ```
 
 ## :computer: Usage
 
 ```sh
 # Set Environment "OPENAI_API_KEY"
 export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxx
 
 # Run
 gptwrite
 ? Language? <Select Language>
 # ...(Lots of questions come in to the interactive.)
-```
+```
```

### Comparing `llmwrite-0.1.4/llmwrite/accepted_language.py` & `llmwrite-0.1.5/llmwrite/accepted_language.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/core.py` & `llmwrite-0.1.5/llmwrite/core.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/lang_conf.py` & `llmwrite-0.1.5/llmwrite/lang_conf.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/locales/messages.en.yaml` & `llmwrite-0.1.5/llmwrite/locales/messages.en.yaml`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/locales/messages.ja.yaml` & `llmwrite-0.1.5/llmwrite/locales/messages.ja.yaml`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/main.py` & `llmwrite-0.1.5/llmwrite/main.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/prompts.py` & `llmwrite-0.1.5/llmwrite/prompts.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/llmwrite/questionary_ui.py` & `llmwrite-0.1.5/llmwrite/questionary_ui.py`

 * *Files identical despite different names*

### Comparing `llmwrite-0.1.4/pyproject.toml` & `llmwrite-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmwrite"
-version = "0.1.4"
+version = "0.1.5"
 description = "CLI for Automated article writing (Powered by GPT-3)"
 authors = ["otakumesi <bakednt@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/otakumesi/llm-write"
 repository = "https://github.com/otakumesi/llm-write"
 readme = "README.md"
 keywords = ["gpt", "openai", "cli", "article", "writing"]
@@ -13,23 +13,23 @@
 python = "^3.8"
 click = "*"
 openai = "*"
 python-i18n = {extras = ["yaml"], version = "*"}
 iso639-lang = "*"
 questionary = "^1.10.0"
 yaspin = "^2.3.0"
-pytest-mock = "^3.10.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "*"
 black = "*"
 pyright = "^1.1.303"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 llmwrite = "llmwrite.main:write"
```

### Comparing `llmwrite-0.1.4/PKG-INFO` & `llmwrite-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmwrite
-Version: 0.1.4
+Version: 0.1.5
 Summary: CLI for Automated article writing (Powered by GPT-3)
 Home-page: https://github.com/otakumesi/llm-write
 License: MIT
 Keywords: gpt,openai,cli,article,writing
 Author: otakumesi
 Author-email: bakednt@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,46 +13,47 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click
 Requires-Dist: iso639-lang
 Requires-Dist: openai
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: python-i18n[yaml]
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Repository, https://github.com/otakumesi/llm-write
 Description-Content-Type: text/markdown
 
-# GPT-Write :writing_hand:
+# LLM-Write (powered by GPT-3) :writing_hand:
 
-__GPT make writing an article brazing fast :fire:.__
+__LLM make writing an article brazing fast :fire:.__
 
 PyPi:
-- https://pypi.org/project/gptwrite/
+- https://pypi.org/project/llmwrite/
 
-![GPT-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
+![LLM-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
 
 ## :telescope: Overview
-- GPT-Write is the CLI tool for Intractive Automated Article Writing.  
+- This app is built with GPT-3.
+- LLM-Write is the CLI tool for Intractive Automated Article Writing.  
 - You can create articles, just answer the questions.   
-- Since the language is specified in the GPT prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.  
+- Since the language is specified in the LLM prompt and LLM is allowed to generate the text, it could theoretically be used in a variety of languages.  
     - However, the supported languages in the shell messages are only English and Japanese.
 
 
 ## :runner: Installation
 ```sh
-pip install gptwrite
+pip install llmwrite
 ```
 
 ## :computer: Usage
 
 ```sh
 # Set Environment "OPENAI_API_KEY"
 export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxx
 
 # Run
 gptwrite
 ? Language? <Select Language>
 # ...(Lots of questions come in to the interactive.)
 ```
+
```

