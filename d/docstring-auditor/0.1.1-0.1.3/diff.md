# Comparing `tmp/docstring_auditor-0.1.1.tar.gz` & `tmp/docstring_auditor-0.1.3.tar.gz`

## Comparing `docstring_auditor-0.1.1.tar` & `docstring_auditor-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/docstring_auditor/__init__.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/docstring_auditor/main.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_critique.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_extractor.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/tests/test_reporter.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/LICENSE
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 docstring_auditor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/Dockerfile
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/.github/workflows/image-latest.yml
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/.github/workflows/image-release.yml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/docstring_auditor/__init__.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/docstring_auditor/main.py
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/tests/test_critique.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/tests/test_extractor.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/tests/test_reporter.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/README.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 docstring_auditor-0.1.3/PKG-INFO
```

### Comparing `docstring_auditor-0.1.1/.github/workflows/test.yml` & `docstring_auditor-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.1/docstring_auditor/main.py` & `docstring_auditor-0.1.3/docstring_auditor/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+import os
 import click
 import ast
 import json
 from typing import List, Optional, Dict
 import openai
 
 
@@ -153,40 +154,103 @@
             )
             click.secho(f"{warning}\n", fg="yellow")
         if solution:
             click.secho(f"A proposed solution to these concerns is:\n\n{solution}\n\n")
         return True
 
 
-@click.command(name="DocstringAuditor")
-@click.argument(
-    "file_path", type=click.Path(exists=True, readable=True), default=__file__
-)
-def docstring_auditor(file_path: str):
+def process_file(file_path: str):
     """
-    Analyze Python functions' docstrings in a given file and provide critiques and suggestions for improvement.
-
-    This program reads a Python file, extracts the functions and their docstrings,
-    and then analyzes the docstrings for errors, warnings,
-    and possible improvements. The critiques and suggestions are then displayed to the user.
+    Process a single Python file and analyze its functions' docstrings.
 
     Parameters
     ----------
     file_path : str
         The path to the .py file to analyze the functions' docstrings.
 
     Returns
     -------
     None
         The function does not return any value. It prints the critiques and suggestions for the docstrings in the given file.
     """
     functions = extract_functions(file_path)
 
     for idx, function in enumerate(functions):
-        print(f"Processing function {idx + 1} of {len(functions)}...")
+        print(
+            f"Processing function {idx + 1} of {len(functions)} in file {file_path}..."
+        )
         assert isinstance(function, str)
         critique = ask_for_critique(function)
         report_concerns(critique)
 
 
+def process_directory(directory_path: str, ignore_dirs: Optional[List[str]] = None):
+    """
+    Recursively process all .py files in a directory and its subdirectories, ignoring specified directories.
+
+    Parameters
+    ----------
+    directory_path : str
+        The path to the directory containing .py files to analyze the functions' docstrings.
+
+    ignore_dirs : Optional[List[str]]
+        A list of directory names to ignore while processing .py files. By default, it ignores the "tests" directory.
+
+    Returns
+    -------
+    None
+        The function does not return any value. It prints the critiques and suggestions for the docstrings in the .py files.
+    """
+    if ignore_dirs is None:
+        ignore_dirs = ["tests"]
+
+    for root, dirs, files in os.walk(directory_path):
+        dirs[:] = [d for d in dirs if d not in ignore_dirs]
+
+        for file in files:
+            if file.endswith(".py"):
+                file_path = os.path.join(root, file)
+                process_file(file_path)
+
+
+@click.command(name="DocstringAuditor")
+@click.argument("path", type=click.Path(exists=True, readable=True), default=__file__)
+@click.option(
+    "--ignore-dirs",
+    type=click.STRING,
+    multiple=True,
+    default=["tests"],
+    help="A list of directory names to ignore while processing .py files. Separate multiple directories with a space.",
+)
+def docstring_auditor(path: str, ignore_dirs: List[str]):
+    """
+    Analyze Python functions' docstrings in a given file or directory and provide critiques and suggestions for improvement.
+
+    This program reads a Python file or directory, extracts the functions and their docstrings,
+    and then analyzes the docstrings for errors, warnings,
+    and possible improvements. The critiques and suggestions are then displayed to the user.
+
+    Parameters
+    ----------
+    path : str
+        The path to the .py file or directory to analyze the functions' docstrings.
+
+    ignore_dirs : List[str]
+        A list of directory names to ignore while processing .py files.
+
+    Returns
+    -------
+    None
+        The function does not return any value. It prints the critiques and suggestions for the docstrings in the given file or directory.
+    """
+    if os.path.isfile(path):
+        process_file(path)
+    elif os.path.isdir(path):
+        process_directory(path, ignore_dirs)
+    else:
+        click.secho(
+            "Invalid path. Please provide a valid file or directory path.", fg="red"
+        )
+
+
 if __name__ == "__main__":
     docstring_auditor()
```

### Comparing `docstring_auditor-0.1.1/tests/test_critique.py` & `docstring_auditor-0.1.3/tests/test_critique.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,21 +139,30 @@
                 }
             }
         ]
     }
     return response
 
 
-
-@pytest.fixture(params=[mock_chatcompletion_create_no_errors_warnings,
-                       mock_chatcompletion_create_only_warning,
-                       mock_chatcompletion_create_only_error,
-                       mock_chatcompletion_create_error_and_solution,
-                       mock_chatcompletion_create_warning_and_solution],
-                ids=["no_errors_warnings", "only_warning", "only_error", "error_and_solution", "warning_and_solution"])
+@pytest.fixture(
+    params=[
+        mock_chatcompletion_create_no_errors_warnings,
+        mock_chatcompletion_create_only_warning,
+        mock_chatcompletion_create_only_error,
+        mock_chatcompletion_create_error_and_solution,
+        mock_chatcompletion_create_warning_and_solution,
+    ],
+    ids=[
+        "no_errors_warnings",
+        "only_warning",
+        "only_error",
+        "error_and_solution",
+        "warning_and_solution",
+    ],
+)
 def openai_mock(monkeypatch, request):
     monkeypatch.setattr(openai.ChatCompletion, "create", request.param)
     return request  # Return the request object
 
 
 def test_ask_for_critique(openai_mock):
     function = (
@@ -161,15 +170,17 @@
         '    """This is a test function."""\n'
         "    return 'successful'\n"
     )
 
     response_dict = ask_for_critique(function)
     assert response_dict["function"].startswith("test_function_")
 
-    current_test_id = openai_mock.param.__name__  # Access the current mock function's name
+    current_test_id = (
+        openai_mock.param.__name__
+    )  # Access the current mock function's name
     if "no_errors_warnings" in current_test_id:
         assert response_dict["error"] == ""
         assert response_dict["warning"] == ""
         assert response_dict["solution"] == ""
     elif "only_warning" in current_test_id:
         assert response_dict["error"] == ""
         assert response_dict["warning"] == "A warning occurred."
@@ -181,8 +192,8 @@
     elif "error_and_solution" in current_test_id:
         assert response_dict["error"] == "An error occurred."
         assert response_dict["warning"] == ""
         assert response_dict["solution"] == "Updated docstring."
     elif "warning_and_solution" in current_test_id:
         assert response_dict["error"] == ""
         assert response_dict["warning"] == "A warning occurred."
-        assert response_dict["solution"] == "Updated docstring."
+        assert response_dict["solution"] == "Updated docstring."
```

### Comparing `docstring_auditor-0.1.1/tests/test_extractor.py` & `docstring_auditor-0.1.3/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.1/tests/test_reporter.py` & `docstring_auditor-0.1.3/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.1/.gitignore` & `docstring_auditor-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.1/LICENSE` & `docstring_auditor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.1/README.md` & `docstring_auditor-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # Docstring Auditor
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml)
+[![Release](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml)
 
-Introducing _Docstring Auditor_, a cutting-edge solution to ensure that your Python code documentation remains accurate and up-to-date.
-Tired of encountering misleading or outdated docstrings that no longer align with your code's functionality? You're not alone!
-That's why we've developed Docstring Auditor, a powerful tool that leverages the prowess of large language models
-to analyze and critique your docstrings, ensuring they accurately reflect your code's true purpose.
-Say goodbye to technical discrepancies and confusing descriptions.
-With Docstring Auditor, you can effortlessly bridge the gap between your code and its documentation,
-making it more accessible and understandable to both experts and novices alike.
-Step into the future of code documentation with Docstring Auditor – the ultimate companion for maintaining crystal-clear, precise, and informative docstrings.
-
-Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on.
-Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
-
-Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language.
-By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation.
-The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent.
-Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
+Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation. Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings, ensuring they align with your code's true purpose. Accessible to both experts and novices, Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings. Say hello to better code documentation!
+
+## Motivation
+
+Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on. Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
+
+Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language. By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation. The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent. Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
 
 With Docstring Auditor, you can trust that your documentation stays relevant, informative, and accessible to all members of your team, making collaboration smoother and more efficient than ever before.
 
 
 ## Features
 - Analyzes Python functions' docstrings in a given file
 - Identifies errors, warnings, and possible improvements
@@ -42,15 +35,15 @@
 
 ```bash
 docstring-auditor path/to/your/python_file.py
 ```
 
 The tool will then analyze the functions' docstrings in the specified file and display the critiques and suggestions for improvement.
 
-Example
+## Example
 Let's say you have a Python file called example.py with the following content:
 
 ```python
 
 def compute(a, b):
     """
     Add two numbers.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `docstring_auditor-0.1.1/pyproject.toml` & `docstring_auditor-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "docstring-auditor"
-version = "0.1.1"
+version = "0.1.3"
 authors = [{name = "Rob Luke", email = "code@robertluke.net"}]
 description = "A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement"
 readme = "README.md"
 keywords = ["docstring", "auditor", "openai", "gpt"]
 url = "https://github.com/rob-luke/docstring-auditor"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -23,18 +23,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.hatch.package]
 packages = ["docstring_auditor"]
 
-[tool.hatch.entry_points]
-console_scripts = [
-    "docstring-auditor = docstring_auditor:main",
-]
+[tool.hatch.envs.default.scripts]
+docstring-auditor = "python docstring_auditor/main.py {args}"
 
 [tool.hatch.envs.default]
 dependencies = [
     "click",
     "openai",
 ]
```

### Comparing `docstring_auditor-0.1.1/PKG-INFO` & `docstring_auditor-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstring-auditor
-Version: 0.1.1
+Version: 0.1.3
 Summary: A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement
 Author-email: Rob Luke <code@robertluke.net>
 License-File: LICENSE
 Keywords: auditor,docstring,gpt,openai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,32 +16,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Docstring Auditor
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml)
+[![Release](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml)
 
-Introducing _Docstring Auditor_, a cutting-edge solution to ensure that your Python code documentation remains accurate and up-to-date.
-Tired of encountering misleading or outdated docstrings that no longer align with your code's functionality? You're not alone!
-That's why we've developed Docstring Auditor, a powerful tool that leverages the prowess of large language models
-to analyze and critique your docstrings, ensuring they accurately reflect your code's true purpose.
-Say goodbye to technical discrepancies and confusing descriptions.
-With Docstring Auditor, you can effortlessly bridge the gap between your code and its documentation,
-making it more accessible and understandable to both experts and novices alike.
-Step into the future of code documentation with Docstring Auditor – the ultimate companion for maintaining crystal-clear, precise, and informative docstrings.
-
-Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on.
-Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
-
-Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language.
-By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation.
-The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent.
-Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
+Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation. Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings, ensuring they align with your code's true purpose. Accessible to both experts and novices, Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings. Say hello to better code documentation!
+
+## Motivation
+
+Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on. Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
+
+Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language. By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation. The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent. Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
 
 With Docstring Auditor, you can trust that your documentation stays relevant, informative, and accessible to all members of your team, making collaboration smoother and more efficient than ever before.
 
 
 ## Features
 - Analyzes Python functions' docstrings in a given file
 - Identifies errors, warnings, and possible improvements
@@ -62,15 +55,15 @@
 
 ```bash
 docstring-auditor path/to/your/python_file.py
 ```
 
 The tool will then analyze the functions' docstrings in the specified file and display the critiques and suggestions for improvement.
 
-Example
+## Example
 Let's say you have a Python file called example.py with the following content:
 
 ```python
 
 def compute(a, b):
     """
     Add two numbers.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

