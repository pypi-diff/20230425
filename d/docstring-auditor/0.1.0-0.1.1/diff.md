# Comparing `tmp/docstring_auditor-0.1.0.tar.gz` & `tmp/docstring_auditor-0.1.1.tar.gz`

## Comparing `docstring_auditor-0.1.0.tar` & `docstring_auditor-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/docstring_auditor/__init__.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/docstring_auditor/main.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/tests/test_critique.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/tests/test_extractor.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/tests/test_reporter.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/LICENSE
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 docstring_auditor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/docstring_auditor/__init__.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/docstring_auditor/main.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_critique.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_extractor.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_reporter.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/PKG-INFO
```

### Comparing `docstring_auditor-0.1.0/.github/workflows/test.yml` & `docstring_auditor-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/docstring_auditor/main.py` & `docstring_auditor-0.1.1/docstring_auditor/main.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/tests/test_critique.py` & `docstring_auditor-0.1.1/tests/test_critique.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/tests/test_extractor.py` & `docstring_auditor-0.1.1/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/tests/test_reporter.py` & `docstring_auditor-0.1.1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/.gitignore` & `docstring_auditor-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/LICENSE` & `docstring_auditor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.0/README.md` & `docstring_auditor-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 That's why we've developed Docstring Auditor, a powerful tool that leverages the prowess of large language models
 to analyze and critique your docstrings, ensuring they accurately reflect your code's true purpose.
 Say goodbye to technical discrepancies and confusing descriptions.
 With Docstring Auditor, you can effortlessly bridge the gap between your code and its documentation,
 making it more accessible and understandable to both experts and novices alike.
 Step into the future of code documentation with Docstring Auditor – the ultimate companion for maintaining crystal-clear, precise, and informative docstrings.
 
+Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on.
+Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
+
+Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language.
+By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation.
+The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent.
+Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
+
+With Docstring Auditor, you can trust that your documentation stays relevant, informative, and accessible to all members of your team, making collaboration smoother and more efficient than ever before.
+
+
 ## Features
 - Analyzes Python functions' docstrings in a given file
 - Identifies errors, warnings, and possible improvements
 - Provides detailed critiques and suggestions for better docstrings
 - Powered by OpenAI's GPT for accurate and insightful analysis
 - Easy to use command-line interface
```

### Comparing `docstring_auditor-0.1.0/pyproject.toml` & `docstring_auditor-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "docstring-auditor"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "Rob Luke", email = "code@robertluke.net"}]
 description = "A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement"
 readme = "README.md"
 keywords = ["docstring", "auditor", "openai", "gpt"]
 url = "https://github.com/rob-luke/docstring-auditor"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `docstring_auditor-0.1.0/PKG-INFO` & `docstring_auditor-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstring-auditor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement
 Author-email: Rob Luke <code@robertluke.net>
 License-File: LICENSE
 Keywords: auditor,docstring,gpt,openai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,14 +27,25 @@
 That's why we've developed Docstring Auditor, a powerful tool that leverages the prowess of large language models
 to analyze and critique your docstrings, ensuring they accurately reflect your code's true purpose.
 Say goodbye to technical discrepancies and confusing descriptions.
 With Docstring Auditor, you can effortlessly bridge the gap between your code and its documentation,
 making it more accessible and understandable to both experts and novices alike.
 Step into the future of code documentation with Docstring Auditor – the ultimate companion for maintaining crystal-clear, precise, and informative docstrings.
 
+Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on.
+Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
+
+Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language.
+By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation.
+The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent.
+Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
+
+With Docstring Auditor, you can trust that your documentation stays relevant, informative, and accessible to all members of your team, making collaboration smoother and more efficient than ever before.
+
+
 ## Features
 - Analyzes Python functions' docstrings in a given file
 - Identifies errors, warnings, and possible improvements
 - Provides detailed critiques and suggestions for better docstrings
 - Powered by OpenAI's GPT for accurate and insightful analysis
 - Easy to use command-line interface
```

