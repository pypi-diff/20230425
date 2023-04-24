# Comparing `tmp/perfect_physics-0.1.5-py3-none-any.whl.zip` & `tmp/perfect_physics-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,15 @@
-Zip file size: 19992 bytes, number of entries: 19
+Zip file size: 16056 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      319 b- defN 22-Nov-22 03:19 perfect_physics/__init__.py
 -rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-18 15:33 perfect_physics/_circle.py
 -rw-rw-rw-  2.0 fat     2863 b- defN 23-Apr-20 02:11 perfect_physics/_misc.py
 -rw-rw-rw-  2.0 fat    14665 b- defN 23-Apr-24 02:04 perfect_physics/_physics.py
 -rw-rw-rw-  2.0 fat     3341 b- defN 23-Apr-24 02:13 perfect_physics/_timeline.py
 -rw-rw-rw-  2.0 fat      904 b- defN 22-Nov-18 02:58 perfect_physics/_wall.py
 -rw-rw-rw-  2.0 fat    26580 b- defN 23-Apr-24 02:26 perfect_physics/_world.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-27 19:29 perfect_physics/tests/__init__.py
 -rw-rw-rw-  2.0 fat     5518 b- defN 22-Nov-22 03:19 perfect_physics/tests/test_perfect_physics.py
--rw-rw-rw-  2.0 fat     9928 b- defN 22-Nov-09 15:59 perfect_physics-0.1.5.data/data/data/cc_time_solutions.sympy
--rw-rw-rw-  2.0 fat     9148 b- defN 22-Nov-11 02:53 perfect_physics-0.1.5.data/data/data/cc_velocity_solution.sympy
--rw-rw-rw-  2.0 fat     1505 b- defN 22-Nov-09 23:07 perfect_physics-0.1.5.data/data/data/cw_time_solutions.sympy
--rw-rw-rw-  2.0 fat     1925 b- defN 22-Nov-11 18:01 perfect_physics-0.1.5.data/data/data/cw_velocity_limits.sympy
--rw-rw-rw-  2.0 fat     5315 b- defN 22-Nov-12 15:43 perfect_physics-0.1.5.data/data/data/instant_speed.sympy
--rw-rw-rw-  2.0 fat     6740 b- defN 22-Nov-12 15:45 perfect_physics-0.1.5.data/data/data/instant_speed_wall.sympy
--rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 16:50 perfect_physics-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 16:50 perfect_physics-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 16:50 perfect_physics-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1802 b- defN 23-Apr-24 16:50 perfect_physics-0.1.5.dist-info/RECORD
-19 files, 94184 bytes uncompressed, 16966 bytes compressed:  82.0%
+-rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 17:09 perfect_physics-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 17:09 perfect_physics-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 17:09 perfect_physics-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1099 b- defN 23-Apr-24 17:09 perfect_physics-0.1.6.dist-info/RECORD
+13 files, 58920 bytes uncompressed, 14208 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -21,38 +21,20 @@
 
 Filename: perfect_physics/tests/__init__.py
 Comment: 
 
 Filename: perfect_physics/tests/test_perfect_physics.py
 Comment: 
 
-Filename: perfect_physics-0.1.5.data/data/data/cc_time_solutions.sympy
+Filename: perfect_physics-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: perfect_physics-0.1.5.data/data/data/cc_velocity_solution.sympy
+Filename: perfect_physics-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: perfect_physics-0.1.5.data/data/data/cw_time_solutions.sympy
+Filename: perfect_physics-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: perfect_physics-0.1.5.data/data/data/cw_velocity_limits.sympy
-Comment: 
-
-Filename: perfect_physics-0.1.5.data/data/data/instant_speed.sympy
-Comment: 
-
-Filename: perfect_physics-0.1.5.data/data/data/instant_speed_wall.sympy
-Comment: 
-
-Filename: perfect_physics-0.1.5.dist-info/METADATA
-Comment: 
-
-Filename: perfect_physics-0.1.5.dist-info/WHEEL
-Comment: 
-
-Filename: perfect_physics-0.1.5.dist-info/top_level.txt
-Comment: 
-
-Filename: perfect_physics-0.1.5.dist-info/RECORD
+Filename: perfect_physics-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `perfect_physics-0.1.5.dist-info/METADATA` & `perfect_physics-0.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.5
+Version: 0.1.6
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 Requires-Dist: numpy
```

