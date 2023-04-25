# Comparing `tmp/sara_compis1_tools-0.0.8.tar.gz` & `tmp/sara_compis1_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.8.tar", last modified: Mon Apr 24 06:12:25 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.9.tar", last modified: Mon Apr 24 14:03:49 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.8.tar` & `sara_compis1_tools-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.935989 sara_compis1_tools-0.0.8/
--rw-rw-rw-   0        0        0      357 2023-04-24 06:11:52.000000 sara_compis1_tools-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      956 2023-04-24 06:12:25.930874 sara_compis1_tools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/README.txt
--rw-rw-rw-   0        0        0     1947 2023-04-24 06:02:26.000000 sara_compis1_tools-0.0.8/generated.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.881622 sara_compis1_tools-0.0.8/sara_compis1_tools/
--rw-rw-rw-   0        0        0     4483 2023-04-24 01:35:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/AFD_tools.py
--rw-rw-rw-   0        0        0      155 2023-04-23 15:56:11.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Error.py
--rw-rw-rw-   0        0        0     6092 2023-04-24 03:38:02.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      263 2023-04-21 02:28:08.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0     1385 2023-04-23 04:32:41.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Visualizer.py
--rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0     7598 2023-04-24 06:11:03.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    10130 2023-04-24 06:09:40.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/lexEval.py
--rw-rw-rw-   0        0        0    17009 2023-04-24 06:09:16.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/lexGen.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.923139 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      956 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 06:12:25.936429 sara_compis1_tools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-24 06:12:07.000000 sara_compis1_tools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:03:49.337322 sara_compis1_tools-0.0.9/
+-rw-rw-rw-   0        0        0      357 2023-04-24 06:45:23.000000 sara_compis1_tools-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-04-24 14:03:49.334739 sara_compis1_tools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.9/README.txt
+-rw-rw-rw-   0        0        0     1947 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/generated.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:03:49.306204 sara_compis1_tools-0.0.9/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     4483 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/AFD_tools.py
+-rw-rw-rw-   0        0        0      155 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/Error.py
+-rw-rw-rw-   0        0        0     6278 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      263 2023-04-21 02:28:08.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0     1385 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/Visualizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0     7665 2023-04-24 14:00:46.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0     2923 2023-04-24 13:59:13.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/lexEval.py
+-rw-rw-rw-   0        0        0    17066 2023-04-24 06:45:24.000000 sara_compis1_tools-0.0.9/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:03:49.328273 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-04-24 14:03:48.000000 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-04-24 14:03:49.000000 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:03:48.000000 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 14:03:48.000000 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-24 14:03:48.000000 sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:03:49.337821 sara_compis1_tools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:02:54.000000 sara_compis1_tools-0.0.9/setup.py
```

### Comparing `sara_compis1_tools-0.0.8/LICENSE.txt` & `sara_compis1_tools-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/PKG-INFO` & `sara_compis1_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sara_compis1_tools-0.0.8/generated.py` & `sara_compis1_tools-0.0.9/generated.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/AFD_tools.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/AFD_tools.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/Format.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-
-class Format:
-    def __init__(self, regex):
-        self.regex = regex
-        self.sims = {'(': 1, '|': 2, '.': 3, '*': 4, '+': 4, '?': 4}
-
-
-    def prec(self, value):
-        return 5 if value.isalnum() else self.sims[value]
-
-
-    def idempotenciesApp(self):
-        regexStr = self.regex
-        i = 0
-        while i < len(regexStr)-1:
-            if regexStr[i] == regexStr[i+1] and regexStr[i] in "+?":
-                regexStr = regexStr[:i] + regexStr[i+1:]
-            else:
-                i += 1
-        self.regex = regexStr
-
-
-    def positiveId(self, regexx):
-        expression = regexx
-        count_plus = expression.count('+')
-        count_plus_lit = expression.count("'+'")
-        count_t = count_plus - count_plus_lit
-        while count_t > 0:
-
-            count_plus = expression.count('+')
-            count_plus_lit = expression.count("'+'")
-            count_t = count_plus - count_plus_lit
-            
-            for i in range(len(expression)):
-                if expression[i] == '+':
-                    if expression[i-1] == ')':
-                        j = i-2
-                        continuee = True
-                        closeParen = 1
-                        while continuee:
-                            if expression[j] == ')':
-                                closeParen += 1
-                            elif expression[j] == '(':
-                                closeParen -= 1
-                            j -= 1
-                            if closeParen == 0:
-                                continuee = False
-                        expression = f'{expression[:j+1]}{expression[j+1:i]*2}*{expression[i+1:]}'
-
-                    elif expression[i-1].isalnum():
-                        before = expression[:i-1]
-                        after = expression[i+1:]
-                        middle = expression[i-1]*2
-                        expression = f'{before}{middle}*{after}'    
-        return expression
-
-    
-    def zeroOrOneId(self, regexx):
-        expression = regexx
-        count_q = expression.count('?')
-        count_q_lit = expression.count("'?'")
-        count_t = count_q - count_q_lit
-        while count_t > 0:
-
-            count_q = expression.count('?')
-            count_q_lit = expression.count("'?'")
-            count_t = count_q - count_q_lit
-
-            for i in range(len(expression)):
-
-                
-
-                if expression[i] == '?':
-                    if expression[i-1] == ')':
-                        j = i-2
-                        continuee = True
-                        closeParen = 1
-                        while continuee:
-                            if expression[j] == ')':
-                                closeParen += 1
-                            elif expression[j] == '(':
-                                closeParen -= 1
-                            j -= 1
-                            if closeParen == 0:
-                                continuee = False
-                        expression = f'{expression[:j+1]}({expression[j+1:i]}|ε){expression[i+1:]}'
-
-                    elif expression[i-1].isalnum():
-                        before = expression[:i-1]
-                        after = expression[i+1:]
-                        middle = expression[i-1]
-                        expression = f'{before}({middle}|ε){after}' 
-                    elif i-2 >= 0:
-                        ck = expression[i-3:i]
-                        if ck[0] == "'" and ck[-1] == "'":
-                            expression = f'{expression[:i-3]}({ck}|ε){expression[i+1:]}'
-
-                               
-
-                    
-        return expression
-
-
-    def concat(self, regexx):
-        newRegex, ops = "", list(self.sims.keys())
-        ops.remove('(')
-
-        i = 0
-        while i < len(regexx):
-            val = regexx[i]
-            if i + 2 < len(regexx):
-                if regexx[i] == "'" and regexx[i + 2] == "'":
-                    val = regexx[i + 1]
-                    val = str(ord(val))
-                    if len(val) == 2:
-                        val = '0' + val
-                    elif len(val) == 1:
-                        val = '00' + val
-                    i += 2
-                elif val.isalnum() or val in ["#", '_', '^', '"']:
-                    val = str(ord(val))
-                    if len(val) == 2:
-                        val = '0' + val
-                    elif len(val) == 1:
-                        val = '00' + val
-
-            elif regexx[i].isalnum() or regexx[i] in ['#', '_', '^', '"']:
-                val = str(ord(val)) 
-                if len(val) == 2:
-                    val = '0' + val
-                elif len(val) == 1:
-                    val = '00' + val
-                    
-            if i + 1 < len(regexx):
-                val_p1 = regexx[i + 1]
-                newRegex += val
-
-                if val != '(' and val_p1 != ')' and val != '|' and val_p1 not in ops:
-                    newRegex += '.'
-
-            i += 1
-
-        if regexx[-1] == ')' or regexx[-1] in ops:
-            newRegex += regexx[-1]
-        else:
-            if len(str(ord(regexx[-1]))) == 1:
-                newRegex += '00' + str(ord(regexx[-1]))
-            elif len(str(ord(regexx[-1]))) == 2:
-                newRegex += '0' + str(ord(regexx[-1]))
-
-        return newRegex
-
-
-    def infixPostfix(self):
-        postfix, stack = '', []
-        concatRegex = self.concat()
-
-        for value in concatRegex:
-            if value == '(':
-                stack.append(value)
-
-            elif value == ')':
-                while stack[-1] != '(':
-                    postfix += stack.pop()
-                stack.pop()
-
-            else:
-                while stack and self.prec(value) <= self.prec(stack[-1]):
-                    postfix += stack.pop()
-                stack.append(value)
-
-        while stack:
-            postfix += stack.pop()
-        return postfix
-
-
-
-# a = Format("12c++(d|q)??e")
-# a.zeroOrOneSus()
-# a.positiveSus()
-# print(a.regex)
-# a.idempotenciesApp()
-# a.zeroOrOneId()
-# a.positiveId()
-# print(a.infixPostfix())
-# print(a.regex)
+
+class Format:
+    def __init__(self, regex):
+        self.regex = regex
+        self.sims = {'(': 1, '|': 2, '.': 3, '*': 4, '+': 4, '?': 4}
+
+
+    def prec(self, value):
+        return 5 if value.isalnum() else self.sims[value]
+
+
+    def idempotenciesApp(self):
+        regexStr = self.regex
+        i = 0
+        while i < len(regexStr)-1:
+            if regexStr[i] == regexStr[i+1] and regexStr[i] in "+?":
+                regexStr = regexStr[:i] + regexStr[i+1:]
+            else:
+                i += 1
+        self.regex = regexStr
+
+
+    def positiveId(self, regexx):
+        expression = regexx
+        count_plus = expression.count('+')
+        count_plus_lit = expression.count("'+'")
+        count_t = count_plus - count_plus_lit
+        while count_t > 0:
+
+            count_plus = expression.count('+')
+            count_plus_lit = expression.count("'+'")
+            count_t = count_plus - count_plus_lit
+            
+            for i in range(len(expression)):
+                if expression[i] == '+':
+                    if expression[i-1] == ')':
+                        j = i-2
+                        continuee = True
+                        closeParen = 1
+                        while continuee:
+                            if expression[j] == ')':
+                                closeParen += 1
+                            elif expression[j] == '(':
+                                closeParen -= 1
+                            j -= 1
+                            if closeParen == 0:
+                                continuee = False
+                        expression = f'{expression[:j+1]}{expression[j+1:i]*2}*{expression[i+1:]}'
+
+                    elif expression[i-1].isalnum():
+                        before = expression[:i-1]
+                        after = expression[i+1:]
+                        middle = expression[i-1]*2
+                        expression = f'{before}{middle}*{after}'    
+        return expression
+
+    
+    def zeroOrOneId(self, regexx):
+        expression = regexx
+        count_q = expression.count('?')
+        count_q_lit = expression.count("'?'")
+        count_t = count_q - count_q_lit
+        while count_t > 0:
+
+            count_q = expression.count('?')
+            count_q_lit = expression.count("'?'")
+            count_t = count_q - count_q_lit
+
+            for i in range(len(expression)):
+
+                
+
+                if expression[i] == '?':
+                    if expression[i-1] == ')':
+                        j = i-2
+                        continuee = True
+                        closeParen = 1
+                        while continuee:
+                            if expression[j] == ')':
+                                closeParen += 1
+                            elif expression[j] == '(':
+                                closeParen -= 1
+                            j -= 1
+                            if closeParen == 0:
+                                continuee = False
+                        expression = f'{expression[:j+1]}({expression[j+1:i]}|ε){expression[i+1:]}'
+
+                    elif expression[i-1].isalnum():
+                        before = expression[:i-1]
+                        after = expression[i+1:]
+                        middle = expression[i-1]
+                        expression = f'{before}({middle}|ε){after}' 
+                    elif i-2 >= 0:
+                        ck = expression[i-3:i]
+                        if ck[0] == "'" and ck[-1] == "'":
+                            expression = f'{expression[:i-3]}({ck}|ε){expression[i+1:]}'
+
+                               
+
+                    
+        return expression
+
+
+    def concat(self, regexx):
+        newRegex, ops = "", list(self.sims.keys())
+        ops.remove('(')
+
+        i = 0
+        while i < len(regexx):
+            val = regexx[i]
+            if i + 2 < len(regexx):
+                if regexx[i] == "'" and regexx[i + 2] == "'":
+                    val = regexx[i + 1]
+                    val = str(ord(val))
+                    if len(val) == 2:
+                        val = '0' + val
+                    elif len(val) == 1:
+                        val = '00' + val
+                    i += 2
+                elif val.isalnum() or val in ["#", '_', '^', '"']:
+                    val = str(ord(val))
+                    if len(val) == 2:
+                        val = '0' + val
+                    elif len(val) == 1:
+                        val = '00' + val
+
+            elif regexx[i].isalnum() or regexx[i] in ['#', '_', '^', '"']:
+                val = str(ord(val)) 
+                if len(val) == 2:
+                    val = '0' + val
+                elif len(val) == 1:
+                    val = '00' + val
+                    
+            if i + 1 < len(regexx):
+                val_p1 = regexx[i + 1]
+                newRegex += val
+
+                if val != '(' and val_p1 != ')' and val != '|' and val_p1 not in ops:
+                    newRegex += '.'
+
+            i += 1
+
+        if regexx[-1] == ')' or regexx[-1] in ops:
+            newRegex += regexx[-1]
+        else:
+            if len(str(ord(regexx[-1]))) == 1:
+                newRegex += '00' + str(ord(regexx[-1]))
+            elif len(str(ord(regexx[-1]))) == 2:
+                newRegex += '0' + str(ord(regexx[-1]))
+
+        return newRegex
+
+
+    def infixPostfix(self):
+        postfix, stack = '', []
+        concatRegex = self.concat()
+
+        for value in concatRegex:
+            if value == '(':
+                stack.append(value)
+
+            elif value == ')':
+                while stack[-1] != '(':
+                    postfix += stack.pop()
+                stack.pop()
+
+            else:
+                while stack and self.prec(value) <= self.prec(stack[-1]):
+                    postfix += stack.pop()
+                stack.append(value)
+
+        while stack:
+            postfix += stack.pop()
+        return postfix
+
+
+
+# a = Format("12c++(d|q)??e")
+# a.zeroOrOneSus()
+# a.positiveSus()
+# print(a.regex)
+# a.idempotenciesApp()
+# a.zeroOrOneId()
+# a.positiveId()
+# print(a.infixPostfix())
+# print(a.regex)
```

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/Visualizer.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/Visualizer.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.9/sara_compis1_tools/lexGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,16 +430,16 @@
     lexer.read()
     mega_content, errors = lexer.generate_automatas()
     mega_automata = lexer.unify(mega_content)
     lexer.change_values(mega_automata)
 
     with open('generated.py', 'w', encoding="utf-8") as file:
         file.write("from sara_compis1_tools.StateAFD import StateAFD\n")
-        file.write("from lexEval import LexEval\n")
-        file.write("from Error import Error\n")
+        file.write("from sara_compis1_tools.lexEval import LexEval\n")
+        file.write("from sara_compis1_tools.Error import Error\n")
         file.write("import sys\n\n")
         file.write("mega = [")
         for i, obj in enumerate(mega_automata):
             if obj.value:
                 value_str = repr(obj.value.line) if isinstance(obj.value.line, str) else str(obj.value.line)
             else:
                 value_str = None
@@ -461,11 +461,11 @@
         file.write("if len(sys.argv) < 2:\n\tprint('Por favor ingrese el archivo plano')\n\tsys.exit(1)\n")
         file.write("txt_file = sys.argv[1]\n\n")
         file.write("lex = LexEval(txt_file)\n")
 
         file.write("results = lex.evaluate(mega, errors)\n")
         file.write("lex.print_tokens(results)\n\n")
 
-        file.write("from Visualizer import Visualizer\n")
+        file.write("from sara_compis1_tools.Visualizer import Visualizer\n")
         file.write("v = Visualizer()\n")
         file.write("v.draw_mega_afd(mega)\n")
```

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/SOURCES.txt` & `sara_compis1_tools-0.0.9/sara_compis1_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.8/setup.py` & `sara_compis1_tools-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.8',
+    version='0.0.9',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab4',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

