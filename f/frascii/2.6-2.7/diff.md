# Comparing `tmp/frascii-2.6.tar.gz` & `tmp/frascii-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.6.tar", last modified: Mon Apr 24 20:43:12 2023, max compression
+gzip compressed data, was "frascii-2.7.tar", last modified: Tue Apr 25 07:42:25 2023, max compression
```

## Comparing `frascii-2.6.tar` & `frascii-2.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 20:43:12.907507 frascii-2.6/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12666 2023-04-24 20:42:46.000000 frascii-2.6/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.903508 frascii-2.6/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-24 20:43:05.000000 frascii-2.6/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7766 2023-04-24 20:38:11.000000 frascii-2.6/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.6/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.6/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.6/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.6/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.6/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3135 2023-04-24 20:36:12.000000 frascii-2.6/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.6/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.6/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2996 2023-04-24 20:34:17.000000 frascii-2.6/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.6/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.6/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.6/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.6/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-24 20:43:12.907507 frascii-2.6/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.6/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.519935 frascii-2.7/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 07:42:25.519935 frascii-2.7/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-2.7/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.515935 frascii-2.7/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-25 07:41:57.000000 frascii-2.7/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-2.7/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.519935 frascii-2.7/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.7/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.7/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.7/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.7/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.7/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3135 2023-04-25 07:39:18.000000 frascii-2.7/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.7/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.7/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2996 2023-04-25 07:39:18.000000 frascii-2.7/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.7/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.7/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.7/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.7/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-25 07:42:25.515935 frascii-2.7/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-25 07:42:25.000000 frascii-2.7/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-25 07:42:25.519935 frascii-2.7/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.7/setup.py
```

### Comparing `frascii-2.6/README.md` & `frascii-2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 `frascii peano_curve <n>`: Displays the n-th iteration of the [Peano Curve](https://en.wikipedia.org/wiki/Peano_curve).
 
 `frascii dragon_curve <n>`: Displays the n-th iteration of the [Dragon Curve](https://en.wikipedia.org/wiki/Dragon_curve).
 
 `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
 
-`frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
+`frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
 
-`frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
+`frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
 
 `frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
 
 
 more to come ...
 
 # Examples
@@ -39,14 +39,18 @@
 
 ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot.png)
 
 `frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style repeating`
 
 ![Mandelbrot set in terminal by frascii](readme_images/repeating.png)
 
+`frascii mandelbrot -x_radius 300 -y_radius 300 -explore`
+
+![Mandelbrot set in terminal by frascii](readme_images/explore.gif)
+
 `frascii mandelbrot -x -1.15 -y 0.26 -x_radius 200 -y_radius 70 -stepsize 3.7e-4 -max_iter 60`
 
 ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot2.png)
 
 `frascii mandelbrot`
 
 ```
```

### Comparing `frascii-2.6/frascii/__init__.py` & `frascii-2.7/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.6'
+__version__ = '2.7'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
```

### Comparing `frascii-2.6/frascii/commands.py` & `frascii-2.7/frascii/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 	mandelbrot_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.05)
 	mandelbrot_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=20)
 	mandelbrot_parser.add_argument("-style", type=str, help="style of the visualization",
 								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
 	mandelbrot_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
 								   choices=["square", "rect"], nargs="?", default="rect")
 	mandelbrot_parser.add_argument("-explore", help=("explore the mandelbrot set using mouse and keyboard. Use mouse or arrow keys to navigate."
-																 "Use page-up and page-down to zoom in and out."
-																 "Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
-																 "Exit with ESC or 'x'."),
-									action="store_true")
+																 " Use page-up and page-down to zoom in and out."
+																 " Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
+																 " Exit with ESC or 'x'."),
+								   action="store_true")
 	mandelbrot_parser.set_defaults(func=frascii.mandelbrot)
 
 	# Julia sub-command
 	julia_parser = subparsers.add_parser("julia", description="Wikipedia: https://en.wikipedia.org/wiki/Julia_set", formatter_class=fc)
 	julia_parser.add_argument("-f", type=str, help="complex function", nargs="?", default="z**2 - 0.4 + 0.6j")
 	julia_parser.add_argument("-x", type=float, help="real part of the images center", nargs="?", default=0)
 	julia_parser.add_argument("-y", type=float, help="imaginary part of the images center", nargs="?", default=0)
@@ -79,19 +79,19 @@
 	julia_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=18)
 	julia_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.033)
 	julia_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=40)
 	julia_parser.add_argument("-style", type=str, help="style of the visualization",
 								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
 	julia_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
 								   choices=["square", "rect"], nargs="?", default="rect")
-	julia_parser.add_argument("-explore", help=("explore the mandelbrot set using mouse and keyboard. Use mouse or arrow keys to navigate."
-																 "Use page-up and page-down to zoom in and out."
-																 "Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
-																 "Exit with ESC or 'x'."),
-									action="store_true")
+	julia_parser.add_argument("-explore", help=("explore the julia set using mouse and keyboard. Use mouse or arrow keys to navigate."
+																 " Use page-up and page-down to zoom in and out."
+																 " Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
+																 " Exit with ESC or 'x'."),
+							  action="store_true")
 	julia_parser.set_defaults(func=frascii.julia)
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
 	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
 	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
 	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
```

### Comparing `frascii-2.6/frascii/fractals/dragon_curve.py` & `frascii-2.7/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/fibonacci.py` & `frascii-2.7/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/hilbert_curve.py` & `frascii-2.7/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/julia.py` & `frascii-2.7/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/koch.py` & `frascii-2.7/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/l_system.py` & `frascii-2.7/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/mandelbrot.py` & `frascii-2.7/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/peano_curve.py` & `frascii-2.7/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii/fractals/sierpinski_carpet.py` & `frascii-2.7/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.6/frascii.egg-info/SOURCES.txt` & `frascii-2.7/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

