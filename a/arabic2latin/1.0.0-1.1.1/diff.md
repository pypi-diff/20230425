# Comparing `tmp/arabic2latin-1.0.0.tar.gz` & `tmp/arabic2latin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabic2latin-1.0.0.tar", last modified: Wed Apr 12 11:29:17 2023, max compression
+gzip compressed data, was "arabic2latin-1.1.1.tar", last modified: Tue Apr 25 07:22:14 2023, max compression
```

## Comparing `arabic2latin-1.0.0.tar` & `arabic2latin-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 11:29:17.013158 arabic2latin-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3221 2023-04-12 11:29:17.012154 arabic2latin-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-10 20:55:54.000000 arabic2latin-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 11:29:17.005505 arabic2latin-1.0.0/arabic2latin/
--rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.0.0/arabic2latin/__init__.py
--rw-rw-rw-   0        0        0     3816 2023-04-10 20:55:38.000000 arabic2latin-1.0.0/arabic2latin/arabic2latin.py
--rw-rw-rw-   0        0        0       23 2023-04-10 21:03:54.000000 arabic2latin-1.0.0/arabic2latin/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:29:17.012154 arabic2latin-1.0.0/arabic2latin.egg-info/
--rw-rw-rw-   0        0        0     3221 2023-04-12 11:29:16.000000 arabic2latin-1.0.0/arabic2latin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-12 11:29:16.000000 arabic2latin-1.0.0/arabic2latin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 11:29:16.000000 arabic2latin-1.0.0/arabic2latin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 11:29:16.000000 arabic2latin-1.0.0/arabic2latin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-04-12 11:04:01.000000 arabic2latin-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 11:29:17.013158 arabic2latin-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.038426 arabic2latin-1.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3221 2023-04-25 07:22:14.037498 arabic2latin-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-10 20:55:54.000000 arabic2latin-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.015653 arabic2latin-1.1.1/arabic2latin/
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.1/arabic2latin/__init__.py
+-rw-rw-rw-   0        0        0     3719 2023-04-22 16:01:53.000000 arabic2latin-1.1.1/arabic2latin/arabic2latin.py
+-rw-rw-rw-   0        0        0       23 2023-04-22 16:01:53.000000 arabic2latin-1.1.1/arabic2latin/version.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.035170 arabic2latin-1.1.1/arabic2latin.egg-info/
+-rw-rw-rw-   0        0        0     3221 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-04-25 07:20:51.000000 arabic2latin-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:22:14.038426 arabic2latin-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.1/setup.py
```

### Comparing `arabic2latin-1.0.0/LICENSE` & `arabic2latin-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.0.0/PKG-INFO` & `arabic2latin-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.0.0
+Version: 1.1.1
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.0.0/README.md` & `arabic2latin-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.0.0/arabic2latin/arabic2latin.py` & `arabic2latin-1.1.1/arabic2latin/arabic2latin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import random
-
 MAPPING = {
     'أ': 'a', 'إ': 'e', 'ا': 'a', 'آ': 'aa', 'ب': 'b', 'پ': 'p', 'ت': 't', 'ث': 'th',
     'ج': 'j', 'ح': 'h', 'خ': 'kh', 'د': 'd', 'ذ': 'th', 'ر': 'r', 'ز': 'z',
     'ُژ': 'j', 'س': 's', 'ش': 'sh', 'ص': 's', 'ض': 'dh', 'ط': 't', 'ظ': 'z', 'ع': 'aa',
     'غ': 'gh', 'ف': 'f', 'ق': 'q', 'ك': 'k', 'ک': 'k', 'گ': 'g', 'ل': 'l', 'م': 'm',
     'ن': 'n', 'ه': 'h', 'ة': 'ah', 'و': 'o', 'ؤ': 'o\'', 'ي': 'y', 'ی': 'y', 'ى': 'y',
     'ٰ': 'aa', 'َ': 'a', 'ُ': 'o', 'ِ': 'e', 'ٌ': 'on', 'ً': 'an', 'ٍ': 'en', 'ء': '', 'ئ': '\'e'
@@ -53,42 +51,42 @@
                     else:
                         result += "oo"
                     special_case = True
 
                 elif text[c-1] in "اىيی" or text[c+1] in "اىيی":
                     if result[-1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
                         if not no_vowel:
-                            result += random.choices(("e", "a"), weights=(1, 4))[0]
+                            result += "a"
                         else:
                             no_vowel = False
 
                     result += "v"
 
                 else:
                     result += MAPPING[char]
 
             elif char == "ه" and (c == n-1 or (c != n-1 and text[c+1] == " ")):
                 result += "ah"
 
             else:
                 if result[-1] not in VOWELS and MAPPING[char][:1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
                     if not no_vowel:
-                        result += random.choices(("e", "a"), weights=(1, 4))[0]
+                        result += "a"
                     else:
                         no_vowel = False
 
                 # prevent occurrence of a letter for more than two times
                 if not result.endswith(MAPPING[char] * 2):
                     # handle two character replacements
                     if result[-1] * 2 == MAPPING[char]:
                         result += MAPPING[char][0]
                     else:
                         result += MAPPING[char]
 
-        elif char == " ":
+        elif ord(char) < 128:
             result += char
 
         # tashdid:
         elif char == "ّ":
             # prevent occurrence of a letter for more than two times
             if result[-2:] != MAPPING[text[c-1]] * 2:
                 result += MAPPING[text[c - 1]]
```

### Comparing `arabic2latin-1.0.0/arabic2latin.egg-info/PKG-INFO` & `arabic2latin-1.1.1/arabic2latin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.0.0
+Version: 1.1.1
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.0.0/pyproject.toml` & `arabic2latin-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arabic2latin"
-version = "1.0.0"
+version = "1.1.1"
 description = "Convert Arabic characters to their Latin (English) homophones."
 readme = "README.md"
 requires-python = ">=3.6"
 license= {file = "LICENSE"}
 keywords=["arabic", "homophone", "arabic to english", "arabic to latin"]
 authors = [
   {email = "rexa222@outlook.com"},
```

### Comparing `arabic2latin-1.0.0/setup.py` & `arabic2latin-1.1.1/setup.py`

 * *Files identical despite different names*

