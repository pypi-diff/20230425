# Comparing `tmp/pymathematics-2023.4.24.tar.gz` & `tmp/pymathematics-2023.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.24.tar", last modified: Mon Apr 24 17:34:56 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.25.tar", last modified: Tue Apr 25 12:48:00 2023, max compression
```

## Comparing `pymathematics-2023.4.24.tar` & `pymathematics-2023.4.25.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.541397 pymathematics-2023.4.24/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.24/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-24 17:34:56.525775 pymathematics-2023.4.24/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-24 17:29:32.000000 pymathematics-2023.4.24/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.275771 pymathematics-2023.4.24/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    20051 2023-04-24 17:29:11.000000 pymathematics-2023.4.24/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-24 17:29:17.000000 pymathematics-2023.4.24/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.478916 pymathematics-2023.4.24/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-24 17:34:53.000000 pymathematics-2023.4.24/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-24 17:34:56.541397 pymathematics-2023.4.24/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-24 17:29:26.000000 pymathematics-2023.4.24/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:48:00.193707 pymathematics-2023.4.25/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.25/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-25 12:48:00.160705 pymathematics-2023.4.25/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-25 12:30:26.000000 pymathematics-2023.4.25/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:47:59.685701 pymathematics-2023.4.25/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    22007 2023-04-25 12:27:38.000000 pymathematics-2023.4.25/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-25 12:30:01.000000 pymathematics-2023.4.25/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:47:59.978706 pymathematics-2023.4.25/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-25 12:48:00.200708 pymathematics-2023.4.25/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-25 12:47:36.000000 pymathematics-2023.4.25/setup.py
```

### Comparing `pymathematics-2023.4.24/LICENSE` & `pymathematics-2023.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.24/pymathematics/__init__.py` & `pymathematics-2023.4.25/pymathematics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sympy
+
 from .info import (
     author,version,homepage
 )
 
 class about:
     author = author
     version = version
@@ -37,37 +39,46 @@
             raise ValueError("vector should have 3 directions")
         return vector.dot_product(vector1,vector2)/vector.magnitude(vector2)
 
     def angle_of_projection(vector1:list,vector2:list) -> float:
         return f"arccos({vector.dot_product(vector1,vector2)}/{(vector.magnitude(vector1)*vector.magnitude(vector2))})"
 
 class matrix:
-    def ismatrix(matrix_):
+    def ismatrix(matrix_) -> bool:
         if not isinstance(matrix_, list):
             return False
         if not all(isinstance(row, list) for row in matrix_):
             return False
         row_lengths = [len(row) for row in matrix_]
         if not all(length == row_lengths[0] for length in row_lengths):
             return False
         return True
+
+    def ifsquare(matrix_) -> bool:
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("elements of each rows aren't the same")
+        if len(matrix_) == len(matrix_[0]):
+            return True
+        return False
     
     def shape(matrix_):
-        if matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
         return len(matrix_),len(matrix_[0])
     
     def size(matrix_):
-        if matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_) == False:
             raise ValueError("elements of each rows aren't the same")
         return len(matrix_)*len(matrix_[0])
 
     def determinant(matrix_):
-        if matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
+        if not matrix.ifsquare(matrix_):
+            raise ValueError("determinant of a matrix is only defined for square matrices")
         if len(matrix_) == 1:
             return matrix_[0][0]
         elif len(matrix_) == 2:
             return matrix_[0][0]*matrix_[1][1]-matrix_[0][1]*matrix_[1][0]
         det = 0
         for x in range(len(matrix_)):
             minor = []
@@ -77,43 +88,69 @@
                     if z != x:
                         row.append(matrix_[y][z])
                 minor.append(row)
             det += (-1)**x*matrix_[0][x]*matrix.determinant(minor)
         return det
     
     def inverse(matrix_):
-        if matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
+        if not matrix.ifsquare(matrix_):
+            raise ValueError("inverse of a matrix is only defined for square matrices")
         identity = [[0 if x != y else 1 for y in range(len(matrix_))] for x in range(len(matrix_))]
         for x in range(len(matrix_)):
             pivot = matrix_[x][x]
             for y in range(len(matrix_)):
                 matrix_[x][y] /= pivot
                 identity[x][y] /= pivot
             for y in range(len(matrix_)):
                 if x != y:
                     factor = matrix_[y][x]
                     for k in range(len(matrix_)):
                         matrix_[y][k] -= factor * matrix_[x][k]
                         identity[y][k] -= factor * identity[x][k]
         return identity
     
+    def cofactor(matrix,row,col):
+        return [row[:col] + row[col+1:] for row in (matrix[:row] + matrix[row+1:])]
+
+    def adjoint(matrix_):
+        adj = []
+        for i in range(len(matrix_)):
+            adjRow = []
+            for j in range(len(matrix_)):
+                sign = (-1)**(i+j)
+                cofactor = matrix.determinant(matrix.cofactor(matrix_,i,j))
+                adjRow.append(sign*cofactor)
+            adj.append(adjRow)
+        return adj
+    
+    def trace(matrix_) -> int|float:
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("elements of each rows aren't the same")
+        if not matrix.ifsquare(matrix_):
+            raise ValueError("matrix should have same number of rows and cols")
+        trace = 0
+        for x in range(len(matrix_)):
+            trace += matrix_[x][x]
+        return trace
+
     def transpose(matrix_):
-        if matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
         rows = len(matrix_)
         cols = len(matrix_[0])
         res = [[0 for y in range(rows)]for x in range(cols)]
         for x in range(rows):
             for y in range(cols):
                 res[y][x] = matrix_[x][y]   
         return res
     
     def product(matrix1,matrix2):
-        if matrix.ismatrix(matrix1) == False or matrix.ismatrix(matrix2) == False:
+        if not matrix.ismatrix(matrix1) or not matrix.ismatrix(matrix2):
             raise ValueError("elements of each rows aren't the same")
         rows1 = len(matrix1)
         cols1 = len(matrix1[0])
         rows2 = len(matrix2)
         cols2 = len(matrix2[0])
         if cols1 != rows2:
             raise ValueError("number of columns of a first matrix should be equal to the rows of the second matrix")
@@ -174,14 +211,28 @@
         A = sets.toset(A)
         B = sets.toset(B)
         res = []
         for i in A:
             for j in B:
                 res.append([i,j])
         return res
+    
+class calculus:
+    def integral(eqn:str,wrt:str = "x",limits:list = [None,None]):
+        if len(limits) != 2:
+            raise ValueError(f"size of the limits should be 2, not {len(limits)}")
+        expr = sympy.sympify(eqn)
+        return sympy.integrate(expr,(wrt,limits[0],limits[1]))
+    
+    def derivative(eqn:str,wrt:str = "x",point:int|float = None):
+        expr = sympy.sympify(eqn)
+        answer = sympy.diff(expr,wrt)
+        if point == None:
+            return answer
+        return float(answer.evalf(subs = {wrt:point}))
 
 def factorial(number: int) -> int:
     if number == 0:
         return 1
     elif number < 0:
         raise ValueError("number can't be negative!")
     return number*factorial(number-1)
@@ -431,15 +482,15 @@
         return summation([array1[x]+array2[x] for x in range(array1)])
     raise ValueError(f"length of array1 and array2 aren't equal {len(array1)} != {array2}")
 
 def zscore(array:list,number:int) -> int|float:
     return (number-mean(array))*standard_deviation(array)
 
 def euclidean_distance(array1:list,array2:list) -> float:
-    if len(array1) < len(array2) < 3:
+    if len(array1) < 3 or len(array2) < 3:
         raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
     return sqrt(summation([(array1[x] - array2[x])**2 for x in range(len(array1))]))
 
 def manhattan_distance(array1:list,array2:list) -> float:
     if len(array1) < len(array2) < 3:
         raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
     return summation([absolute(array1[x] - array2[x]) for x in range(len(array1))])
```

### Comparing `pymathematics-2023.4.24/setup.py` & `pymathematics-2023.4.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.24",
+    version = "2023.4.25",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
-    install_requires = [],
+    install_requires = ["sympy"],
     url = "https://github.com/Sahil-Rajwar-2004/pymathematics",
     keywords = ["maths","mathematics"],
     classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Education",
     "Operating System :: OS Independent",
     ]
```

