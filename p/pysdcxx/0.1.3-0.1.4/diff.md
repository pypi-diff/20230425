# Comparing `tmp/pysdcxx-0.1.3.tar.gz` & `tmp/pysdcxx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdcxx-0.1.3.tar", last modified: Thu Mar 30 20:05:31 2023, max compression
+gzip compressed data, was "pysdcxx-0.1.4.tar", last modified: Tue Apr 25 11:46:10 2023, max compression
```

## Comparing `pysdcxx-0.1.3.tar` & `pysdcxx-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/
--rw-r--r--   0 vencik    (1000) vencik    (1000)     1480 2023-02-07 14:36:31.000000 pysdcxx-0.1.3/LICENSE
--rw-r--r--   0 vencik    (1000) vencik    (1000)       79 2023-02-24 18:25:14.000000 pysdcxx-0.1.3/MANIFEST.in
--rw-r--r--   0 vencik    (1000) vencik    (1000)    14188 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/PKG-INFO
--rw-r--r--   0 vencik    (1000) vencik    (1000)    11525 2023-03-30 19:57:12.000000 pysdcxx-0.1.3/README.adoc
--rw-r--r--   0 vencik    (1000) vencik    (1000)    11238 2023-03-30 20:05:30.000000 pysdcxx-0.1.3/README.md
--rw-r--r--   0 vencik    (1000) vencik    (1000)       81 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/setup.cfg
--rwxr-xr-x   0 vencik    (1000) vencik    (1000)     1567 2023-02-24 18:21:58.000000 pysdcxx-0.1.3/setup.py
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/src/
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/src/libpysdcxx/
--rw-r--r--   0 vencik    (1000) vencik    (1000)     4787 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libpysdcxx/bigram_multiset.cxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)     4389 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libpysdcxx/bigrams.cxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)     4678 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libpysdcxx/sequence_matcher.cxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)     5322 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libpysdcxx/unordered_bigram_multiset.cxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)     2515 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libpysdcxx/util.hxx
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/src/libsdcxx/
--rw-r--r--   0 vencik    (1000) vencik    (1000)    11523 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libsdcxx/bigram_multiset.hxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)    11378 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/libsdcxx/bigrams.hxx
--rw-r--r--   0 vencik    (1000) vencik    (1000)    23150 2023-03-30 19:57:12.000000 pysdcxx-0.1.3/src/libsdcxx/sequence_matcher.hxx
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/src/pysdcxx/
--rw-r--r--   0 vencik    (1000) vencik    (1000)      182 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/pysdcxx/__init__.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)     3626 2023-03-30 19:58:50.000000 pysdcxx-0.1.3/src/pysdcxx/bigram_multiset.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)     3435 2023-03-30 19:59:00.000000 pysdcxx-0.1.3/src/pysdcxx/bigrams.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)    12044 2023-02-24 13:18:35.000000 pysdcxx-0.1.3/src/pysdcxx/libpysdcxx.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)     7293 2023-02-27 12:44:42.000000 pysdcxx-0.1.3/src/pysdcxx/sequence_matcher.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)     4084 2023-03-30 19:59:43.000000 pysdcxx-0.1.3/src/pysdcxx/unordered_bigram_multiset.py
--rw-r--r--   0 vencik    (1000) vencik    (1000)     1153 2023-02-23 19:22:30.000000 pysdcxx-0.1.3/src/pysdcxx/util.py
-drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-03-30 20:05:31.074382 pysdcxx-0.1.3/src/pysdcxx.egg-info/
--rw-r--r--   0 vencik    (1000) vencik    (1000)    14188 2023-03-30 20:05:31.000000 pysdcxx-0.1.3/src/pysdcxx.egg-info/PKG-INFO
--rw-r--r--   0 vencik    (1000) vencik    (1000)      668 2023-03-30 20:05:31.000000 pysdcxx-0.1.3/src/pysdcxx.egg-info/SOURCES.txt
--rw-r--r--   0 vencik    (1000) vencik    (1000)        1 2023-03-30 20:05:31.000000 pysdcxx-0.1.3/src/pysdcxx.egg-info/dependency_links.txt
--rw-r--r--   0 vencik    (1000) vencik    (1000)       19 2023-03-30 20:05:31.000000 pysdcxx-0.1.3/src/pysdcxx.egg-info/top_level.txt
--rw-r--r--   0 vencik    (1000) vencik    (1000)       48 2023-02-24 18:22:51.000000 pysdcxx-0.1.3/version.txt
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     1480 2023-02-07 14:36:31.000000 pysdcxx-0.1.4/LICENSE
+-rw-r--r--   0 vencik    (1000) vencik    (1000)       79 2023-02-24 18:25:14.000000 pysdcxx-0.1.4/MANIFEST.in
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    14204 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/PKG-INFO
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    11531 2023-04-01 21:48:10.000000 pysdcxx-0.1.4/README.adoc
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    11246 2023-04-25 11:46:10.000000 pysdcxx-0.1.4/README.md
+-rw-r--r--   0 vencik    (1000) vencik    (1000)       81 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/setup.cfg
+-rwxr-xr-x   0 vencik    (1000) vencik    (1000)     1567 2023-02-24 18:21:58.000000 pysdcxx-0.1.4/setup.py
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.370932 pysdcxx-0.1.4/src/
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/src/libpysdcxx/
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     4787 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libpysdcxx/bigram_multiset.cxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     4389 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libpysdcxx/bigrams.cxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     4678 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libpysdcxx/sequence_matcher.cxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     5322 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libpysdcxx/unordered_bigram_multiset.cxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     2515 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libpysdcxx/util.hxx
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/src/libsdcxx/
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    11523 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libsdcxx/bigram_multiset.hxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    11378 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/libsdcxx/bigrams.hxx
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    23150 2023-03-30 19:57:12.000000 pysdcxx-0.1.4/src/libsdcxx/sequence_matcher.hxx
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/src/pysdcxx/
+-rw-r--r--   0 vencik    (1000) vencik    (1000)      182 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/pysdcxx/__init__.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     3626 2023-04-25 11:41:44.000000 pysdcxx-0.1.4/src/pysdcxx/bigram_multiset.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     3428 2023-04-25 11:41:35.000000 pysdcxx-0.1.4/src/pysdcxx/bigrams.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    12044 2023-02-24 13:18:35.000000 pysdcxx-0.1.4/src/pysdcxx/libpysdcxx.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     7293 2023-02-27 12:44:42.000000 pysdcxx-0.1.4/src/pysdcxx/sequence_matcher.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     4093 2023-04-25 11:41:55.000000 pysdcxx-0.1.4/src/pysdcxx/unordered_bigram_multiset.py
+-rw-r--r--   0 vencik    (1000) vencik    (1000)     1153 2023-02-23 19:22:30.000000 pysdcxx-0.1.4/src/pysdcxx/util.py
+drwxr-xr-x   0 vencik    (1000) vencik    (1000)        0 2023-04-25 11:46:10.374932 pysdcxx-0.1.4/src/pysdcxx.egg-info/
+-rw-r--r--   0 vencik    (1000) vencik    (1000)    14204 2023-04-25 11:46:10.000000 pysdcxx-0.1.4/src/pysdcxx.egg-info/PKG-INFO
+-rw-r--r--   0 vencik    (1000) vencik    (1000)      668 2023-04-25 11:46:10.000000 pysdcxx-0.1.4/src/pysdcxx.egg-info/SOURCES.txt
+-rw-r--r--   0 vencik    (1000) vencik    (1000)        1 2023-04-25 11:46:10.000000 pysdcxx-0.1.4/src/pysdcxx.egg-info/dependency_links.txt
+-rw-r--r--   0 vencik    (1000) vencik    (1000)       19 2023-04-25 11:46:10.000000 pysdcxx-0.1.4/src/pysdcxx.egg-info/top_level.txt
+-rw-r--r--   0 vencik    (1000) vencik    (1000)       48 2023-03-30 20:19:10.000000 pysdcxx-0.1.4/version.txt
```

### Comparing `pysdcxx-0.1.3/LICENSE` & `pysdcxx-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/PKG-INFO` & `pysdcxx-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdcxx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sørensen–Dice coefficient on string bigram multi-sets (in C++)
 Home-page: https://github.com/vencik/libsdcxx
 Author: Václav Krpec
 Author-email: vencik@razdva.cz
 License: BSD-3-Clause license
 Description: This library may be used to compare strings by a similarity measure,
         defined as Sørensen–Dice coefficient calculated on multi-sets of the
@@ -23,16 +23,15 @@
         (like a whitespace) to mitigate that problem.
         
         Using implementation of bigram multisets above, a sequence matcher
         implementation is also available. Given a sequence of text tokens, the
         matcher then allows "fuzzy" matching of strings (using their bigrams
         again) to sub-sequences of the text tokens.
         
-        See detailed documentation in `doc` directory. Rendered
-            documentation:
+        See detailed documentation in `doc` directory. Rendered documentation:
         
           - <https://htmlpreview.github.io/?https://github.com/vencik/libsdcxx/blob/master/doc/sequence_matcher.html>
         
         # List of features
         
           - Bigram multi-set objects implemented as sorted lists of character
             tuples with count (*O(n log n)* creation time complexity in terms of
@@ -80,43 +79,45 @@
         \# apt-get install g++ cmake make git \# apt-get install python3-pip
         python3-distutils \# unless you use pyenv $ pip install wheel pytest \#
         ditto, better do that in pyenv sandbox\</programlisting\>
         
         On Mac OS X, you’ll need Xcode tools and Homebrew. Then, install the
         required prerequisites by
         
-        $ brew install coreutils cmake make\</programlisting\>
+        $ brew install coreutils cmake make git\</programlisting\>
         
         If you do wish to use `pyenv` to create and manage project sandbox
         (which is advisable), see short intro to that in the subsection below.
         
         Anyhow, with all the prerequisites installed, clone the project:
         
         $ git clone https://github.com/vencik/libsdcxx.git\</programlisting\>
         
-        Build the project, run UTs and build Python package:
+        Build the project, run UTs and build Python packages:
         
-        $ cd libsdcxx $ ./build.sh -up\</programlisting\>
+        $ cd libsdcxx $ ./build.sh -ugp\</programlisting\>
         
         Note that the `build.sh` script has options; run `$ ./build.sh -h` to
         see them.
         
         Most importantly, run with `-s` or `--enable-pt` options to perform
         performance tests. Performance tests compare computation times of object
         construction, union operations and intersection size computations of the
         implementations. If you install `multiset` Python package (using `pip`),
         the perf. tests shall also produce results for pure-Python
         implementation using `multiset.Multiset` (not necessary).
         
-        > **Note**
-        > 
-        > The perf. tests are written on the Python level, so the measured times
-        > also contain some Python code runtime (and not trivial). I’d expect
-        > results in native code to be notably better; but the test code is
-        > identical, so the measurements should be meaningful for comparison.
+        <div class="note">
+        
+        The perf. tests are written on the Python level, so the measured times
+        also contain some Python code runtime (and not trivial). I’d expect
+        results in native code to be notably better; but the test code is
+        identical, so the measurements should be meaningful for comparison.
+        
+        </div>
         
         If you wish, use `pip` to install the Python package:
         
         \# pip install pysdcxx-\*.whl\</programlisting\>
         
         Note that it’s recommended to use `pyenv`, especially for development
         purposes.
```

### Comparing `pysdcxx-0.1.3/README.adoc` & `pysdcxx-0.1.4/README.adoc`

 * *Files 0% similar despite different names*

```diff
@@ -67,31 +67,31 @@
 $ pip install wheel pytest                       # ditto, better do that in pyenv sandbox
 ----
 
 On Mac OS X, you'll need Xcode tools and Homebrew.
 Then, install the required prerequisites by
 [source]
 ----
-$ brew install coreutils cmake make
+$ brew install coreutils cmake make git
 ----
 
 If you do wish to use `pyenv` to create and manage project sandbox (which is advisable),
 see short intro to that in the subsection below.
 
 Anyhow, with all the prerequisites installed, clone the project:
 [source]
 ----
 $ git clone https://github.com/vencik/libsdcxx.git
 ----
 
-Build the project, run UTs and build Python package:
+Build the project, run UTs and build Python packages:
 [source]
 ----
 $ cd libsdcxx
-$ ./build.sh -up
+$ ./build.sh -ugp
 ----
 
 Note that the `build.sh` script has options; run `$ ./build.sh -h` to see them.
 
 Most importantly, run with `-s` or `--enable-pt` options to perform performance tests.
 Performance tests compare computation times of object construction, union operations
 and intersection size computations of the implementations.
```

### Comparing `pysdcxx-0.1.3/README.md` & `pysdcxx-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 (like a whitespace) to mitigate that problem.
 
 Using implementation of bigram multisets above, a sequence matcher
 implementation is also available. Given a sequence of text tokens, the
 matcher then allows "fuzzy" matching of strings (using their bigrams
 again) to sub-sequences of the text tokens.
 
-See detailed documentation in `doc` directory. Rendered
-    documentation:
+See detailed documentation in `doc` directory. Rendered documentation:
 
   - <https://htmlpreview.github.io/?https://github.com/vencik/libsdcxx/blob/master/doc/sequence_matcher.html>
 
 # List of features
 
   - Bigram multi-set objects implemented as sorted lists of character
     tuples with count (*O(n log n)* creation time complexity in terms of
@@ -72,43 +71,45 @@
 \# apt-get install g++ cmake make git \# apt-get install python3-pip
 python3-distutils \# unless you use pyenv $ pip install wheel pytest \#
 ditto, better do that in pyenv sandbox\</programlisting\>
 
 On Mac OS X, you’ll need Xcode tools and Homebrew. Then, install the
 required prerequisites by
 
-$ brew install coreutils cmake make\</programlisting\>
+$ brew install coreutils cmake make git\</programlisting\>
 
 If you do wish to use `pyenv` to create and manage project sandbox
 (which is advisable), see short intro to that in the subsection below.
 
 Anyhow, with all the prerequisites installed, clone the project:
 
 $ git clone https://github.com/vencik/libsdcxx.git\</programlisting\>
 
-Build the project, run UTs and build Python package:
+Build the project, run UTs and build Python packages:
 
-$ cd libsdcxx $ ./build.sh -up\</programlisting\>
+$ cd libsdcxx $ ./build.sh -ugp\</programlisting\>
 
 Note that the `build.sh` script has options; run `$ ./build.sh -h` to
 see them.
 
 Most importantly, run with `-s` or `--enable-pt` options to perform
 performance tests. Performance tests compare computation times of object
 construction, union operations and intersection size computations of the
 implementations. If you install `multiset` Python package (using `pip`),
 the perf. tests shall also produce results for pure-Python
 implementation using `multiset.Multiset` (not necessary).
 
-> **Note**
-> 
-> The perf. tests are written on the Python level, so the measured times
-> also contain some Python code runtime (and not trivial). I’d expect
-> results in native code to be notably better; but the test code is
-> identical, so the measurements should be meaningful for comparison.
+<div class="note">
+
+The perf. tests are written on the Python level, so the measured times
+also contain some Python code runtime (and not trivial). I’d expect
+results in native code to be notably better; but the test code is
+identical, so the measurements should be meaningful for comparison.
+
+</div>
 
 If you wish, use `pip` to install the Python package:
 
 \# pip install pysdcxx-\*.whl\</programlisting\>
 
 Note that it’s recommended to use `pyenv`, especially for development
 purposes.
```

### Comparing `pysdcxx-0.1.3/setup.py` & `pysdcxx-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libpysdcxx/bigram_multiset.cxx` & `pysdcxx-0.1.4/src/libpysdcxx/bigram_multiset.cxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libpysdcxx/bigrams.cxx` & `pysdcxx-0.1.4/src/libpysdcxx/bigrams.cxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libpysdcxx/sequence_matcher.cxx` & `pysdcxx-0.1.4/src/libpysdcxx/sequence_matcher.cxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libpysdcxx/unordered_bigram_multiset.cxx` & `pysdcxx-0.1.4/src/libpysdcxx/unordered_bigram_multiset.cxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libpysdcxx/util.hxx` & `pysdcxx-0.1.4/src/libpysdcxx/util.hxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libsdcxx/bigram_multiset.hxx` & `pysdcxx-0.1.4/src/libsdcxx/bigram_multiset.hxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libsdcxx/bigrams.hxx` & `pysdcxx-0.1.4/src/libsdcxx/bigrams.hxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/libsdcxx/sequence_matcher.hxx` & `pysdcxx-0.1.4/src/libsdcxx/sequence_matcher.hxx`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/pysdcxx/bigram_multiset.py` & `pysdcxx-0.1.4/src/pysdcxx/bigram_multiset.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             if string is not None else _impl or libpysdcxx.new_wbigram_multiset()
 
     def __deepcopy__(self, memo):
         """
         Make a copy on the native level
         :param memo: IDs of already copied objects (unused, we're non-recursive)
         """
-        return self.__class__(_impl=libpysdcxx.new_wbigram_multiset_copy(self._impl))
+        return BigramMultiset(_impl=libpysdcxx.new_wbigram_multiset_copy(self._impl))
 
     def __copy__(self):
         """
         We don't do shallow copies
         """
         return self.__deepcopy__(None)
```

### Comparing `pysdcxx-0.1.3/src/pysdcxx/bigrams.py` & `pysdcxx-0.1.4/src/pysdcxx/bigrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             if string is not None else _impl or libpysdcxx.new_wbigrams()
 
     def __deepcopy__(self, memo):
         """
         Make a copy on the native level
         :param memo: IDs of already copied objects (unused, we're non-recursive)
         """
-        return self.__class__(_impl=libpysdcxx.new_wbigrams_copy(self._impl))
+        return Bigrams(_impl=libpysdcxx.new_wbigrams_copy(self._impl))
 
     def __copy__(self):
         """
         We don't do shallow copies
         """
         return self.__deepcopy__(None)
```

### Comparing `pysdcxx-0.1.3/src/pysdcxx/libpysdcxx.py` & `pysdcxx-0.1.4/src/pysdcxx/libpysdcxx.py`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/pysdcxx/sequence_matcher.py` & `pysdcxx-0.1.4/src/pysdcxx/sequence_matcher.py`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/pysdcxx/unordered_bigram_multiset.py` & `pysdcxx-0.1.4/src/pysdcxx/unordered_bigram_multiset.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             if string is not None else _impl or libpysdcxx.new_unordered_wbigram_multiset()
 
     def __deepcopy__(self, memo):
         """
         Make a copy on the native level
         :param memo: IDs of already copied objects (unused, we're non-recursive)
         """
-        return self.__class__(
+        return UnorderedBigramMultiset(
             _impl=libpysdcxx.new_unordered_wbigram_multiset_copy(self._impl))
 
     def __copy__(self):
         """
         We don't do shallow copies
         """
         return self.__deepcopy__(None)
```

### Comparing `pysdcxx-0.1.3/src/pysdcxx/util.py` & `pysdcxx-0.1.4/src/pysdcxx/util.py`

 * *Files identical despite different names*

### Comparing `pysdcxx-0.1.3/src/pysdcxx.egg-info/PKG-INFO` & `pysdcxx-0.1.4/src/pysdcxx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdcxx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sørensen–Dice coefficient on string bigram multi-sets (in C++)
 Home-page: https://github.com/vencik/libsdcxx
 Author: Václav Krpec
 Author-email: vencik@razdva.cz
 License: BSD-3-Clause license
 Description: This library may be used to compare strings by a similarity measure,
         defined as Sørensen–Dice coefficient calculated on multi-sets of the
@@ -23,16 +23,15 @@
         (like a whitespace) to mitigate that problem.
         
         Using implementation of bigram multisets above, a sequence matcher
         implementation is also available. Given a sequence of text tokens, the
         matcher then allows "fuzzy" matching of strings (using their bigrams
         again) to sub-sequences of the text tokens.
         
-        See detailed documentation in `doc` directory. Rendered
-            documentation:
+        See detailed documentation in `doc` directory. Rendered documentation:
         
           - <https://htmlpreview.github.io/?https://github.com/vencik/libsdcxx/blob/master/doc/sequence_matcher.html>
         
         # List of features
         
           - Bigram multi-set objects implemented as sorted lists of character
             tuples with count (*O(n log n)* creation time complexity in terms of
@@ -80,43 +79,45 @@
         \# apt-get install g++ cmake make git \# apt-get install python3-pip
         python3-distutils \# unless you use pyenv $ pip install wheel pytest \#
         ditto, better do that in pyenv sandbox\</programlisting\>
         
         On Mac OS X, you’ll need Xcode tools and Homebrew. Then, install the
         required prerequisites by
         
-        $ brew install coreutils cmake make\</programlisting\>
+        $ brew install coreutils cmake make git\</programlisting\>
         
         If you do wish to use `pyenv` to create and manage project sandbox
         (which is advisable), see short intro to that in the subsection below.
         
         Anyhow, with all the prerequisites installed, clone the project:
         
         $ git clone https://github.com/vencik/libsdcxx.git\</programlisting\>
         
-        Build the project, run UTs and build Python package:
+        Build the project, run UTs and build Python packages:
         
-        $ cd libsdcxx $ ./build.sh -up\</programlisting\>
+        $ cd libsdcxx $ ./build.sh -ugp\</programlisting\>
         
         Note that the `build.sh` script has options; run `$ ./build.sh -h` to
         see them.
         
         Most importantly, run with `-s` or `--enable-pt` options to perform
         performance tests. Performance tests compare computation times of object
         construction, union operations and intersection size computations of the
         implementations. If you install `multiset` Python package (using `pip`),
         the perf. tests shall also produce results for pure-Python
         implementation using `multiset.Multiset` (not necessary).
         
-        > **Note**
-        > 
-        > The perf. tests are written on the Python level, so the measured times
-        > also contain some Python code runtime (and not trivial). I’d expect
-        > results in native code to be notably better; but the test code is
-        > identical, so the measurements should be meaningful for comparison.
+        <div class="note">
+        
+        The perf. tests are written on the Python level, so the measured times
+        also contain some Python code runtime (and not trivial). I’d expect
+        results in native code to be notably better; but the test code is
+        identical, so the measurements should be meaningful for comparison.
+        
+        </div>
         
         If you wish, use `pip` to install the Python package:
         
         \# pip install pysdcxx-\*.whl\</programlisting\>
         
         Note that it’s recommended to use `pyenv`, especially for development
         purposes.
```

### Comparing `pysdcxx-0.1.3/src/pysdcxx.egg-info/SOURCES.txt` & `pysdcxx-0.1.4/src/pysdcxx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

