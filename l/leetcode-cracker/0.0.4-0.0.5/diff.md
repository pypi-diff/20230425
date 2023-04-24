# Comparing `tmp/leetcode_cracker-0.0.4.tar.gz` & `tmp/leetcode_cracker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetcode_cracker-0.0.4.tar", last modified: Mon Apr 17 22:55:36 2023, max compression
+gzip compressed data, was "leetcode_cracker-0.0.5.tar", last modified: Mon Apr 24 22:55:35 2023, max compression
```

## Comparing `leetcode_cracker-0.0.4.tar` & `leetcode_cracker-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.905677 leetcode_cracker-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2276 2023-04-17 22:55:36.898683 leetcode_cracker-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1797 2023-04-15 09:14:08.000000 leetcode_cracker-0.0.4/README.md
--rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 22:55:36.906675 leetcode_cracker-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.210407 leetcode_cracker-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.814512 leetcode_cracker-0.0.4/src/leetcode_cracker/
--rw-rw-rw-   0        0        0       21 2023-04-17 22:46:56.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-04-13 09:41:16.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_121.py
--rw-rw-rw-   0        0        0      923 2023-04-12 00:35:15.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_169.py
--rw-rw-rw-   0        0        0      780 2023-04-11 01:29:59.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_268.py
--rw-rw-rw-   0        0        0     1149 2023-04-12 00:18:35.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_283.py
--rw-rw-rw-   0        0        0     1206 2023-04-11 01:28:11.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_392.py
--rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.894746 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/
--rw-rw-rw-   0        0        0     2276 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 22:55:35.114344 leetcode_cracker-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3253 2023-04-24 22:55:35.112351 leetcode_cracker-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2774 2023-04-24 02:14:52.000000 leetcode_cracker-0.0.5/README.md
+-rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 22:55:35.114344 leetcode_cracker-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 22:55:34.846797 leetcode_cracker-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 22:55:35.097496 leetcode_cracker-0.0.5/src/leetcode_cracker/
+-rw-rw-rw-   0        0        0       21 2023-04-24 22:54:28.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-04-24 02:22:22.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_1.py
+-rw-rw-rw-   0        0        0      572 2023-04-22 23:53:42.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_1137.py
+-rw-rw-rw-   0        0        0      721 2023-04-24 01:37:55.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_118.py
+-rw-rw-rw-   0        0        0      741 2023-04-22 23:56:23.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_119.py
+-rw-rw-rw-   0        0        0     1050 2023-04-13 09:41:16.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_121.py
+-rw-rw-rw-   0        0        0      613 2023-04-24 02:08:31.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_1480.py
+-rw-rw-rw-   0        0        0      923 2023-04-12 00:35:15.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_169.py
+-rw-rw-rw-   0        0        0      728 2023-04-24 01:40:07.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_217.py
+-rw-rw-rw-   0        0        0      895 2023-04-24 01:44:24.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_22.py
+-rw-rw-rw-   0        0        0      371 2023-04-24 02:19:53.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_2235.py
+-rw-rw-rw-   0        0        0      615 2023-04-24 02:04:18.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_231.py
+-rw-rw-rw-   0        0        0      747 2023-04-15 09:15:16.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_2469.py
+-rw-rw-rw-   0        0        0     1081 2023-04-24 02:11:23.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_258.py
+-rw-rw-rw-   0        0        0      965 2023-04-24 01:57:28.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_263.py
+-rw-rw-rw-   0        0        0      780 2023-04-11 01:29:59.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_268.py
+-rw-rw-rw-   0        0        0     1169 2023-04-24 01:41:28.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_278.py
+-rw-rw-rw-   0        0        0     1149 2023-04-12 00:18:35.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_283.py
+-rw-rw-rw-   0        0        0      621 2023-04-24 02:01:06.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_326.py
+-rw-rw-rw-   0        0        0      614 2023-04-24 02:03:01.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_342.py
+-rw-rw-rw-   0        0        0      719 2023-04-24 01:43:10.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_35.py
+-rw-rw-rw-   0        0        0      734 2023-04-24 01:49:08.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_367.py
+-rw-rw-rw-   0        0        0      401 2023-04-24 01:50:45.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_371.py
+-rw-rw-rw-   0        0        0     1206 2023-04-11 01:28:11.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_392.py
+-rw-rw-rw-   0        0        0     1085 2023-04-18 01:45:44.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_415.py
+-rw-rw-rw-   0        0        0      563 2023-04-24 02:05:16.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_43.py
+-rw-rw-rw-   0        0        0      459 2023-04-24 02:10:11.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_46.py
+-rw-rw-rw-   0        0        0      508 2023-04-24 02:10:35.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_47.py
+-rw-rw-rw-   0        0        0      362 2023-04-24 02:07:52.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_50.py
+-rw-rw-rw-   0        0        0      715 2023-04-24 01:47:43.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_509.py
+-rw-rw-rw-   0        0        0      599 2023-04-24 02:16:46.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_58.py
+-rw-rw-rw-   0        0        0      676 2023-04-24 02:18:57.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_66.py
+-rw-rw-rw-   0        0        0      506 2023-04-24 02:17:43.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_67.py
+-rw-rw-rw-   0        0        0      587 2023-04-24 01:46:11.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_70.py
+-rw-rw-rw-   0        0        0     1190 2023-04-23 01:20:37.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_728.py
+-rw-rw-rw-   0        0        0      383 2023-04-24 02:21:28.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/question_9.py
+-rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.5/src/leetcode_cracker/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 22:55:35.110355 leetcode_cracker-0.0.5/src/leetcode_cracker.egg-info/
+-rw-rw-rw-   0        0        0     3253 2023-04-24 22:55:34.000000 leetcode_cracker-0.0.5/src/leetcode_cracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2023-04-24 22:55:34.000000 leetcode_cracker-0.0.5/src/leetcode_cracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 22:55:34.000000 leetcode_cracker-0.0.5/src/leetcode_cracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 22:55:34.000000 leetcode_cracker-0.0.5/src/leetcode_cracker.egg-info/top_level.txt
```

### Comparing `leetcode_cracker-0.0.4/LICENSE` & `leetcode_cracker-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/PKG-INFO` & `leetcode_cracker-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: leetcode_cracker
-Version: 0.0.4
-Summary: package to assist in solving Leetcode Problems
-Author-email: Albert <albertyqyao@gmail.com>
-Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Leetcode Cracker Info
 Leetcode Cracker is a Python package that allows you to get LeetCode question explanations and answers. LeetCode is a popular online platform for practicing coding skills and preparing for technical interviews. LeetCode offers hundreds of problems covering various topics, such as arrays, strings, trees, graphs, dynamic programming, etc. However, sometimes the official solutions and explanations are not clear enough or not available at all. Leetcode Cracker solves this problem by providing you with detailed and easy-to-understand explanations and answers for any LeetCode question. You can soon use Leetcode Cracker to:
 
 - Search for a specific question by its title or ID
 - Get a summary of the question, including its difficulty level, acceptance rate, tags, and company frequency
 - Get a step-by-step explanation of the optimal solution, along with the time and space complexity analysis
 - Get the Python code for the optimal solution, along with comments and test cases
@@ -30,13 +17,44 @@
 4. Call for solution: `question_392.print_solution()`
 5. Call for solution stats `question_392.solution_stats()`
 
 # Question Database
 
 # Easy
 
-Question 121 - Best time to buy and sell stock
-Question 169 - Majority Element
-Question 268 - Missing Number
-Question 283 - Moving Zeros
-Question 392 - Is Subsequence
-Question 2469 - Convert the Tempreture
+* Question 1 - Two Sum
+* Question 9 - Palindrome Number
+* Question 35 - Search Insert Position
+* Question 58 - Length of last word
+* Question 66 - Plus One
+* Question 67 - Add Binary
+* Question 70 - Climbing Stairs
+* Question 118 - Pascal Triangle
+* Question 119 - Pascal Triangle 2
+* Question 121 - Best time to buy and sell stock
+* Question 169 - Majority Element
+* Question 217 - Comtains Duplicate
+* Question 231 - Power of two
+* Question 258 - Add Digits
+* Question 263 - Ugly Number
+* Question 268 - Missing Number
+* Question 278 - First bad version
+* Question 283 - Moving Zeros
+* Question 326 - Power of three
+* Question 342 - Power of Four
+* Question 367 - Valid Perfect Square
+* Question 392 - Is Subsequence
+* Question 509 - Fibbinachi Numbers
+* Question 728 - Self Dividing Numbers
+* Question 1137 - Tribonacci Number
+* Question 1480 - Running Sum of 1d array
+* Question 2235 - Add Two Integers
+* Question 2469 - Convert the Tempreture
+
+# Medium
+
+* Question 22 - Generate Parantheses
+* Question 43 - Multiply Strings
+* Question 46 - Permutations
+* Question 47 - Permutations 2
+* Question 50 - Pow(x, n)
+* Question 371 - Sum of two integers
```

### Comparing `leetcode_cracker-0.0.4/pyproject.toml` & `leetcode_cracker-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker/question_121.py` & `leetcode_cracker-0.0.5/src/leetcode_cracker/question_121.py`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker/question_169.py` & `leetcode_cracker-0.0.5/src/leetcode_cracker/question_169.py`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker/question_268.py` & `leetcode_cracker-0.0.5/src/leetcode_cracker/question_268.py`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker/question_283.py` & `leetcode_cracker-0.0.5/src/leetcode_cracker/question_283.py`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker/question_392.py` & `leetcode_cracker-0.0.5/src/leetcode_cracker/question_392.py`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/PKG-INFO` & `leetcode_cracker-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: leetcode-cracker
-Version: 0.0.4
+Name: leetcode_cracker
+Version: 0.0.5
 Summary: package to assist in solving Leetcode Problems
 Author-email: Albert <albertyqyao@gmail.com>
 Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -30,13 +30,44 @@
 4. Call for solution: `question_392.print_solution()`
 5. Call for solution stats `question_392.solution_stats()`
 
 # Question Database
 
 # Easy
 
-Question 121 - Best time to buy and sell stock
-Question 169 - Majority Element
-Question 268 - Missing Number
-Question 283 - Moving Zeros
-Question 392 - Is Subsequence
-Question 2469 - Convert the Tempreture
+* Question 1 - Two Sum
+* Question 9 - Palindrome Number
+* Question 35 - Search Insert Position
+* Question 58 - Length of last word
+* Question 66 - Plus One
+* Question 67 - Add Binary
+* Question 70 - Climbing Stairs
+* Question 118 - Pascal Triangle
+* Question 119 - Pascal Triangle 2
+* Question 121 - Best time to buy and sell stock
+* Question 169 - Majority Element
+* Question 217 - Comtains Duplicate
+* Question 231 - Power of two
+* Question 258 - Add Digits
+* Question 263 - Ugly Number
+* Question 268 - Missing Number
+* Question 278 - First bad version
+* Question 283 - Moving Zeros
+* Question 326 - Power of three
+* Question 342 - Power of Four
+* Question 367 - Valid Perfect Square
+* Question 392 - Is Subsequence
+* Question 509 - Fibbinachi Numbers
+* Question 728 - Self Dividing Numbers
+* Question 1137 - Tribonacci Number
+* Question 1480 - Running Sum of 1d array
+* Question 2235 - Add Two Integers
+* Question 2469 - Convert the Tempreture
+
+# Medium
+
+* Question 22 - Generate Parantheses
+* Question 43 - Multiply Strings
+* Question 46 - Permutations
+* Question 47 - Permutations 2
+* Question 50 - Pow(x, n)
+* Question 371 - Sum of two integers
```

