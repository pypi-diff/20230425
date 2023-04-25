# Comparing `tmp/frascii-2.7.tar.gz` & `tmp/frascii-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.7.tar", last modified: Tue Apr 25 07:42:25 2023, max compression
+gzip compressed data, was "frascii-2.8.tar", last modified: Tue Apr 25 11:03:00 2023, max compression
```

## Comparing `frascii-2.7.tar` & `frascii-2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.519935 frascii-2.7/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 07:42:25.519935 frascii-2.7/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-2.7/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.515935 frascii-2.7/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-25 07:41:57.000000 frascii-2.7/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-2.7/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.519935 frascii-2.7/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.7/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.7/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.7/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.7/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.7/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3135 2023-04-25 07:39:18.000000 frascii-2.7/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.7/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.7/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2996 2023-04-25 07:39:18.000000 frascii-2.7/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.7/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.7/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.7/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.7/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.515935 frascii-2.7/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-25 07:42:25.519935 frascii-2.7/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.7/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 11:03:00.063898 frascii-2.8/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 11:03:00.063898 frascii-2.8/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-2.8/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 11:03:00.055898 frascii-2.8/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-25 11:02:35.000000 frascii-2.8/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-2.8/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 11:03:00.059898 frascii-2.8/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.8/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.8/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.8/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.8/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.8/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3693 2023-04-25 11:01:27.000000 frascii-2.8/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.8/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.8/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3559 2023-04-25 11:01:42.000000 frascii-2.8/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.8/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.8/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.8/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.8/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 11:03:00.059898 frascii-2.8/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 11:03:00.000000 frascii-2.8/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-25 11:03:00.000000 frascii-2.8/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-25 11:03:00.000000 frascii-2.8/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-25 11:03:00.000000 frascii-2.8/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-25 11:03:00.000000 frascii-2.8/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-25 11:03:00.063898 frascii-2.8/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.8/setup.py
```

### Comparing `frascii-2.7/README.md` & `frascii-2.8/README.md`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/__init__.py` & `frascii-2.8/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.7'
+__version__ = '2.8'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
```

### Comparing `frascii-2.7/frascii/commands.py` & `frascii-2.8/frascii/commands.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/dragon_curve.py` & `frascii-2.8/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/fibonacci.py` & `frascii-2.8/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/hilbert_curve.py` & `frascii-2.8/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/koch.py` & `frascii-2.8/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/l_system.py` & `frascii-2.8/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/peano_curve.py` & `frascii-2.8/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii/fractals/sierpinski_carpet.py` & `frascii-2.8/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.7/frascii.egg-info/SOURCES.txt` & `frascii-2.8/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

