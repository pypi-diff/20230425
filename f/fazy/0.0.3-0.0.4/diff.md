# Comparing `tmp/fazy-0.0.3.tar.gz` & `tmp/fazy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazy-0.0.3.tar", last modified: Fri Apr 21 05:31:30 2023, max compression
+gzip compressed data, was "fazy-0.0.4.tar", last modified: Tue Apr 25 09:42:26 2023, max compression
```

## Comparing `fazy-0.0.3.tar` & `fazy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.929652 fazy-0.0.3/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.3/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)    12315 2023-04-21 05:31:30.929413 fazy-0.0.3/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)    11763 2023-04-21 04:18:58.000000 fazy-0.0.3/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.928039 fazy-0.0.3/f/
--rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.3/f/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.3/f/chain_unit.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.3/f/lazy_string.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     2405 2023-04-21 05:21:58.000000 fazy-0.0.3/f/proxy_module.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.929109 fazy-0.0.3/fazy.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)    12315 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-21 05:31:30.929713 fazy-0.0.3/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-04-21 05:31:02.000000 fazy-0.0.3/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.057125 fazy-0.0.4/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.4/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-04-25 09:42:26.056899 fazy-0.0.4/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)    13874 2023-04-25 09:34:57.000000 fazy-0.0.4/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.055685 fazy-0.0.4/f/
+-rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.4/f/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.4/f/chain_unit.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.4/f/lazy_string.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     5166 2023-04-25 09:22:32.000000 fazy-0.0.4/f/proxy_module.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.056641 fazy-0.0.4/fazy.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-04-25 09:42:26.000000 fazy-0.0.4/fazy.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-25 09:42:26.057179 fazy-0.0.4/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-04-21 18:39:23.000000 fazy-0.0.4/setup.py
```

### Comparing `fazy-0.0.3/LICENSE` & `fazy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fazy-0.0.3/PKG-INFO` & `fazy-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,14 +26,15 @@
 
 Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
+- [**Additional features**](#additional-features)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
 - [**Limitations**](#limitations)
 - [**Benchmark**](#benchmark)
 
 
 ## Quick start
@@ -46,18 +47,54 @@
 
 And use:
 
 ```python
 >>> import f
 >>>
 >>> number = 33
->>> print(f('{number} kittens drink milk'))
-33 kittens drink milk
+>>> f('{number} kittens drink milk')
+'33 kittens drink milk'
 ```
 
+## Additional features
+
+You can execute the string not in lazy mode:
+
+```python
+>>> f('{number} kittens drink milk', lazy=False)
+'33 kittens drink milk'
+```
+
+By default, you cannot use variables as templates. When you try to do this, you will see an `SyntaxError` (the example will not work in REPL and in the global scope, that's why you don't see `>>>`):
+
+```python
+def function():
+    number = 33
+    template = '{number} kittens drink milk'
+    print(f(template))
+
+function()
+# SyntaxError: Unsafe use of a variable as a template.
+```
+
+However, you can disable this check:
+
+```python
+template = '{number} kittens drink milk'
+f(template, safe=False)
+```
+
+All scopes of variable names are available to you, including variables declared in closures. If you disable data extraction from closures, you can greatly speed up the execution of the function:
+
+```python
+>>> f('{number} kittens drink milk', closures=False)
+'33 kittens drink milk'
+```
+
+
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
 
 The new way of writing logs is not very different from the old one. Try to execute this piece of code:
@@ -129,14 +166,16 @@
 
 1. **Local variables**.
 2. **Global variables**.
 3. **Intermediate variables** that are used, for example, when creating [closures](https://en.wikipedia.org/wiki/Closure_(computer_programming)). To give them a more precise definition, these are such local variables of all functions higher up the call stack, which refer to functions that in the code wrap the function being executed at the moment (I know this sentence may not be so easy to read and understand the first time). This means that, going through the call stack, we ignore all scopes with local variables for functions that are not the parents of the function being executed at the moment.
 
 As you might guess from the size of the description, the most interesting type of scopes is the third - intermediate variables. The expected approach to determine the nesting of functions is an analysis of the source code. However, compiling a large amount of source code just to figure out which function wraps another one would be too costly. Therefore, in this case, a hack is used based on knowledge of how memory management occurs inside the interpreter. The fact is that the garbage collector knows about all the objects that exist in memory, as well as about the links between them. The function in which a particular frame of the call stack is executed can be found by requesting from the gc all objects containing references to it. After retrieving the function object, you can determine whether it is the parent of the currently executed one. To do this, you just need to compare their full names (qualnames) stored in the metadata of the functions.
 
+Another couple of words deserves a description of protection from a call with a template in the form of a variable. As you could already understand from the description above, by default you can call the function `f` only with a string literal as an argument. This is necessary to protect the string from attacks that allow arbitrary code to be executed. Checking whether a string is a literal and not a variable is performed by analyzing an abstract syntax tree (AST). Through the stack, we find the function in which the code is currently running. Next, we analyze this code in search of situations where the function `f` is called without a literal as an argument. If such a situation occurs at least 1 time in the line in which the code is currently being executed, we raise `SyntaxError`. However, it should be borne in mind that this protection cannot work in REPL, because there are difficulties in extracting the source code of the function for AST analysis. There were also problems with how to extract data about the module in which the code is executed, so the protection will not work in the global scope either.
+
 
 ## Limitations
 
 Based on the description of the internal structure of the library, you can understand that there are some limitations that should be taken into account. Here are some of them:
 
 - **The performance is obviously less** than that of the original f-strings embedded in the interpreter. Read more about this in the section with [benchmark](#benchmark).
 - **Mutable objects can change their state between the time the references to them are saved and the final calculation of the string**. This means, for example, that if you create a `LazyString` object containing a reference to the list, then add another element to the list, and after that calculate the string - you will see the list in the already changed state in this line.
@@ -173,14 +212,14 @@
 
 for number in range(10000):
     str(f('the number is {number}'))
 
 print(perf_counter() - t1)
 ```
 
-On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2.4 seconds, that is, about **0.00024 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
+On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2 seconds, that is, about **0.0002 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
 
-> So, the original f-strings in this case turned out to be more than **1000 times faster**.
+> So, the original f-strings in this case turned out to be about **1000 times faster**.
 
 However, this does not mean that f-strings are faster in all cases. In real use, you should consider how fast the expressions that you insert into the f-strings are evaluated. If this is significantly slower than actually required for extrapolation, saving on deferred extrapolation may make sense.
 
 Most of the extrapolation time is actually taken not by the extrapolation itself, but by collecting various data for display from the stack and the garbage collector. Unfortunately, if you want to completely replicate the behavior of the original f-strings, these costs are unavoidable.
```

### Comparing `fazy-0.0.3/README.md` & `fazy-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
+- [**Additional features**](#additional-features)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
 - [**Limitations**](#limitations)
 - [**Benchmark**](#benchmark)
 
 
 ## Quick start
@@ -30,18 +31,54 @@
 
 And use:
 
 ```python
 >>> import f
 >>>
 >>> number = 33
->>> print(f('{number} kittens drink milk'))
-33 kittens drink milk
+>>> f('{number} kittens drink milk')
+'33 kittens drink milk'
 ```
 
+## Additional features
+
+You can execute the string not in lazy mode:
+
+```python
+>>> f('{number} kittens drink milk', lazy=False)
+'33 kittens drink milk'
+```
+
+By default, you cannot use variables as templates. When you try to do this, you will see an `SyntaxError` (the example will not work in REPL and in the global scope, that's why you don't see `>>>`):
+
+```python
+def function():
+    number = 33
+    template = '{number} kittens drink milk'
+    print(f(template))
+
+function()
+# SyntaxError: Unsafe use of a variable as a template.
+```
+
+However, you can disable this check:
+
+```python
+template = '{number} kittens drink milk'
+f(template, safe=False)
+```
+
+All scopes of variable names are available to you, including variables declared in closures. If you disable data extraction from closures, you can greatly speed up the execution of the function:
+
+```python
+>>> f('{number} kittens drink milk', closures=False)
+'33 kittens drink milk'
+```
+
+
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
 
 The new way of writing logs is not very different from the old one. Try to execute this piece of code:
@@ -113,14 +150,16 @@
 
 1. **Local variables**.
 2. **Global variables**.
 3. **Intermediate variables** that are used, for example, when creating [closures](https://en.wikipedia.org/wiki/Closure_(computer_programming)). To give them a more precise definition, these are such local variables of all functions higher up the call stack, which refer to functions that in the code wrap the function being executed at the moment (I know this sentence may not be so easy to read and understand the first time). This means that, going through the call stack, we ignore all scopes with local variables for functions that are not the parents of the function being executed at the moment.
 
 As you might guess from the size of the description, the most interesting type of scopes is the third - intermediate variables. The expected approach to determine the nesting of functions is an analysis of the source code. However, compiling a large amount of source code just to figure out which function wraps another one would be too costly. Therefore, in this case, a hack is used based on knowledge of how memory management occurs inside the interpreter. The fact is that the garbage collector knows about all the objects that exist in memory, as well as about the links between them. The function in which a particular frame of the call stack is executed can be found by requesting from the gc all objects containing references to it. After retrieving the function object, you can determine whether it is the parent of the currently executed one. To do this, you just need to compare their full names (qualnames) stored in the metadata of the functions.
 
+Another couple of words deserves a description of protection from a call with a template in the form of a variable. As you could already understand from the description above, by default you can call the function `f` only with a string literal as an argument. This is necessary to protect the string from attacks that allow arbitrary code to be executed. Checking whether a string is a literal and not a variable is performed by analyzing an abstract syntax tree (AST). Through the stack, we find the function in which the code is currently running. Next, we analyze this code in search of situations where the function `f` is called without a literal as an argument. If such a situation occurs at least 1 time in the line in which the code is currently being executed, we raise `SyntaxError`. However, it should be borne in mind that this protection cannot work in REPL, because there are difficulties in extracting the source code of the function for AST analysis. There were also problems with how to extract data about the module in which the code is executed, so the protection will not work in the global scope either.
+
 
 ## Limitations
 
 Based on the description of the internal structure of the library, you can understand that there are some limitations that should be taken into account. Here are some of them:
 
 - **The performance is obviously less** than that of the original f-strings embedded in the interpreter. Read more about this in the section with [benchmark](#benchmark).
 - **Mutable objects can change their state between the time the references to them are saved and the final calculation of the string**. This means, for example, that if you create a `LazyString` object containing a reference to the list, then add another element to the list, and after that calculate the string - you will see the list in the already changed state in this line.
@@ -157,14 +196,14 @@
 
 for number in range(10000):
     str(f('the number is {number}'))
 
 print(perf_counter() - t1)
 ```
 
-On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2.4 seconds, that is, about **0.00024 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
+On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2 seconds, that is, about **0.0002 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
 
-> So, the original f-strings in this case turned out to be more than **1000 times faster**.
+> So, the original f-strings in this case turned out to be about **1000 times faster**.
 
 However, this does not mean that f-strings are faster in all cases. In real use, you should consider how fast the expressions that you insert into the f-strings are evaluated. If this is significantly slower than actually required for extrapolation, saving on deferred extrapolation may make sense.
 
 Most of the extrapolation time is actually taken not by the extrapolation itself, but by collecting various data for display from the stack and the garbage collector. Unfortunately, if you want to completely replicate the behavior of the original f-strings, these costs are unavoidable.
```

### Comparing `fazy-0.0.3/f/lazy_string.py` & `fazy-0.0.4/f/lazy_string.py`

 * *Files identical despite different names*

### Comparing `fazy-0.0.3/fazy.egg-info/PKG-INFO` & `fazy-0.0.4/fazy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,14 +26,15 @@
 
 Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
+- [**Additional features**](#additional-features)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
 - [**Limitations**](#limitations)
 - [**Benchmark**](#benchmark)
 
 
 ## Quick start
@@ -46,18 +47,54 @@
 
 And use:
 
 ```python
 >>> import f
 >>>
 >>> number = 33
->>> print(f('{number} kittens drink milk'))
-33 kittens drink milk
+>>> f('{number} kittens drink milk')
+'33 kittens drink milk'
 ```
 
+## Additional features
+
+You can execute the string not in lazy mode:
+
+```python
+>>> f('{number} kittens drink milk', lazy=False)
+'33 kittens drink milk'
+```
+
+By default, you cannot use variables as templates. When you try to do this, you will see an `SyntaxError` (the example will not work in REPL and in the global scope, that's why you don't see `>>>`):
+
+```python
+def function():
+    number = 33
+    template = '{number} kittens drink milk'
+    print(f(template))
+
+function()
+# SyntaxError: Unsafe use of a variable as a template.
+```
+
+However, you can disable this check:
+
+```python
+template = '{number} kittens drink milk'
+f(template, safe=False)
+```
+
+All scopes of variable names are available to you, including variables declared in closures. If you disable data extraction from closures, you can greatly speed up the execution of the function:
+
+```python
+>>> f('{number} kittens drink milk', closures=False)
+'33 kittens drink milk'
+```
+
+
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
 
 The new way of writing logs is not very different from the old one. Try to execute this piece of code:
@@ -129,14 +166,16 @@
 
 1. **Local variables**.
 2. **Global variables**.
 3. **Intermediate variables** that are used, for example, when creating [closures](https://en.wikipedia.org/wiki/Closure_(computer_programming)). To give them a more precise definition, these are such local variables of all functions higher up the call stack, which refer to functions that in the code wrap the function being executed at the moment (I know this sentence may not be so easy to read and understand the first time). This means that, going through the call stack, we ignore all scopes with local variables for functions that are not the parents of the function being executed at the moment.
 
 As you might guess from the size of the description, the most interesting type of scopes is the third - intermediate variables. The expected approach to determine the nesting of functions is an analysis of the source code. However, compiling a large amount of source code just to figure out which function wraps another one would be too costly. Therefore, in this case, a hack is used based on knowledge of how memory management occurs inside the interpreter. The fact is that the garbage collector knows about all the objects that exist in memory, as well as about the links between them. The function in which a particular frame of the call stack is executed can be found by requesting from the gc all objects containing references to it. After retrieving the function object, you can determine whether it is the parent of the currently executed one. To do this, you just need to compare their full names (qualnames) stored in the metadata of the functions.
 
+Another couple of words deserves a description of protection from a call with a template in the form of a variable. As you could already understand from the description above, by default you can call the function `f` only with a string literal as an argument. This is necessary to protect the string from attacks that allow arbitrary code to be executed. Checking whether a string is a literal and not a variable is performed by analyzing an abstract syntax tree (AST). Through the stack, we find the function in which the code is currently running. Next, we analyze this code in search of situations where the function `f` is called without a literal as an argument. If such a situation occurs at least 1 time in the line in which the code is currently being executed, we raise `SyntaxError`. However, it should be borne in mind that this protection cannot work in REPL, because there are difficulties in extracting the source code of the function for AST analysis. There were also problems with how to extract data about the module in which the code is executed, so the protection will not work in the global scope either.
+
 
 ## Limitations
 
 Based on the description of the internal structure of the library, you can understand that there are some limitations that should be taken into account. Here are some of them:
 
 - **The performance is obviously less** than that of the original f-strings embedded in the interpreter. Read more about this in the section with [benchmark](#benchmark).
 - **Mutable objects can change their state between the time the references to them are saved and the final calculation of the string**. This means, for example, that if you create a `LazyString` object containing a reference to the list, then add another element to the list, and after that calculate the string - you will see the list in the already changed state in this line.
@@ -173,14 +212,14 @@
 
 for number in range(10000):
     str(f('the number is {number}'))
 
 print(perf_counter() - t1)
 ```
 
-On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2.4 seconds, that is, about **0.00024 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
+On my computer (a MacBook Pro with an Apple M1 Pro processor), the execution of this code takes about 2 seconds, that is, about **0.0002 seconds for 1 iteration**. However, if I replace `str(f('the number is {number}'))` with `str(f'the number is {number}')`, the execution time will be 0.0022 seconds, about **0.00000022 seconds for 1 iteration**.
 
-> So, the original f-strings in this case turned out to be more than **1000 times faster**.
+> So, the original f-strings in this case turned out to be about **1000 times faster**.
 
 However, this does not mean that f-strings are faster in all cases. In real use, you should consider how fast the expressions that you insert into the f-strings are evaluated. If this is significantly slower than actually required for extrapolation, saving on deferred extrapolation may make sense.
 
 Most of the extrapolation time is actually taken not by the extrapolation itself, but by collecting various data for display from the stack and the garbage collector. Unfortunately, if you want to completely replicate the behavior of the original f-strings, these costs are unavoidable.
```

### Comparing `fazy-0.0.3/setup.py` & `fazy-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as readme_file:
+with open('README.md', 'r') as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
-    name="fazy",
-    version="0.0.3",
-    author="Evgeniy Blinov",
-    author_email="zheni-b@yandex.ru",
-    description="Lazy f-strings for everyone",
+    name='fazy',
+    version='0.0.4',
+    author='Evgeniy Blinov',
+    author_email='zheni-b@yandex.ru',
+    description='Lazy f-strings for everyone',
     long_description=readme,
-    long_description_content_type="text/markdown",
-    url="https://github.com/pomponchik/fazy",
-    packages=find_packages(exclude=("tests",)),
+    long_description_content_type='text/markdown',
+    url='https://github.com/pomponchik/fazy',
+    packages=find_packages(exclude=('tests',)),
     install_requires=requirements,
     classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: MIT License',
     ],
 )
```

