# Comparing `tmp/jamstats-1.2.0.tar.gz` & `tmp/jamstats-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jamstats-1.2.0.tar", last modified: Sun Apr  2 23:23:23 2023, max compression
+gzip compressed data, was "dist/jamstats-1.2.1.tar", last modified: Tue Apr 25 03:04:58 2023, max compression
```

## Comparing `jamstats-1.2.0.tar` & `jamstats-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:23.000000 jamstats-1.2.0/
--rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-04-02 23:23:23.000000 jamstats-1.2.0/PKG-INFO
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/bin/
--rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.2.0/bin/jamstats
--rw-r--r--   0 damonmay   (501) staff       (20)     8445 2023-04-01 22:28:27.000000 jamstats-1.2.0/README.md
--rw-r--r--   0 damonmay   (501) staff       (20)      843 2023-04-02 22:56:56.000000 jamstats-1.2.0/setup.py
--rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-04-02 23:23:23.000000 jamstats-1.2.0/setup.cfg
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/
--rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)      784 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/SOURCES.txt
--rw-r--r--   0 damonmay   (501) staff       (20)      184 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/requires.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/top_level.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats.egg-info/dependency_links.txt
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:23.000000 jamstats-1.2.0/src/jamstats/util/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/util/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/util/resources.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:23.000000 jamstats-1.2.0/src/jamstats/web/
--rw-r--r--   0 damonmay   (501) staff       (20)    15284 2023-04-02 22:17:49.000000 jamstats-1.2.0/src/jamstats/web/statserver.py
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/web/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:23.000000 jamstats-1.2.0/src/jamstats/resources/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/resources/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats/io/
--rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/io/tsv_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2523 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/io/scoreboard_json_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/io/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9229 2023-04-02 20:51:40.000000 jamstats-1.2.0/src/jamstats/io/scoreboard_server_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:22.000000 jamstats-1.2.0/src/jamstats/data/
--rw-r--r--   0 damonmay   (501) staff       (20)    34676 2023-03-21 04:49:36.000000 jamstats-1.2.0/src/jamstats/data/json_to_pandas.py
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/data/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-1.2.0/src/jamstats/data/game_data.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-02 23:23:23.000000 jamstats-1.2.0/src/jamstats/plots/
--rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.2.0/src/jamstats/plots/plot_together.py
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.0/src/jamstats/plots/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9923 2023-04-02 05:53:22.000000 jamstats-1.2.0/src/jamstats/plots/skaterplots.py
--rw-r--r--   0 damonmay   (501) staff       (20)    42561 2023-04-02 22:40:16.000000 jamstats-1.2.0/src/jamstats/plots/jamplots.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.2.0/src/jamstats/plots/plot_util.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/
+-rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-04-25 03:04:58.000000 jamstats-1.2.1/PKG-INFO
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/bin/
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.2.1/bin/jamstats
+-rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-1.2.1/README.md
+-rw-r--r--   0 damonmay   (501) staff       (20)      843 2023-04-25 03:03:42.000000 jamstats-1.2.1/setup.py
+-rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-04-25 03:04:58.000000 jamstats-1.2.1/setup.cfg
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/
+-rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)      784 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/SOURCES.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)      184 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/requires.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/top_level.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats.egg-info/dependency_links.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/util/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/util/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/util/resources.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/web/
+-rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/web/statserver.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/web/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/resources/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/io/
+-rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/io/tsv_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/io/scoreboard_json_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/io/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/io/scoreboard_server_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/data/
+-rw-r--r--   0 damonmay   (501) staff       (20)    35851 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/data/json_to_pandas.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/data/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-1.2.1/src/jamstats/data/game_data.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-04-25 03:04:58.000000 jamstats-1.2.1/src/jamstats/plots/
+-rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.2.1/src/jamstats/plots/plot_together.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1/src/jamstats/plots/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/plots/skaterplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-1.2.1/src/jamstats/plots/jamplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.2.1/src/jamstats/plots/plot_util.py
```

### Comparing `jamstats-1.2.0/bin/jamstats` & `jamstats-1.2.1/bin/jamstats`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/README.md` & `jamstats-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,510 +19,532 @@
 00000120: 6c6f 7473 2066 726f 6d20 6761 6d65 204a  lots from game J
 00000130: 534f 4e20 6669 6c65 7320 2a2a 6f6e 6c69  SON files **onli
 00000140: 6e65 212a 2a20 4e6f 206e 6565 6420 746f  ne!** No need to
 00000150: 2069 6e73 7461 6c6c 2061 6e79 7468 696e   install anythin
 00000160: 672e 2043 6865 636b 206f 7574 205b 6a61  g. Check out [ja
 00000170: 6d73 7461 7473 2e6e 6574 5d28 6874 7470  mstats.net](http
 00000180: 733a 2f2f 6a61 6d73 7461 7473 2e6e 6574  s://jamstats.net
-00000190: 292e 200a 0a54 6865 206d 6169 6e20 7265  ). ..The main re
-000001a0: 6173 6f6e 2074 6f20 646f 776e 6c6f 6164  ason to download
-000001b0: 2061 6e64 2072 756e 204a 616d 7374 6174   and run Jamstat
-000001c0: 7320 6f6e 2079 6f75 7220 6c61 7074 6f70  s on your laptop
-000001d0: 2069 7320 746f 2063 6f6e 6e65 6374 2074   is to connect t
-000001e0: 6f20 6120 6c69 7665 2067 616d 6520 6f6e  o a live game on
-000001f0: 2061 2072 756e 6e69 6e67 2073 636f 7265   a running score
-00000200: 626f 6172 642e 2057 6879 3f20 5765 6c6c  board. Why? Well
-00000210: 2c20 666f 7220 6f6e 6520 7468 696e 672c  , for one thing,
-00000220: 202a 2a4a 616d 7374 6174 7320 6973 2067   **Jamstats is g
-00000230: 7265 6174 2066 6f72 2061 6e6e 6f75 6e63  reat for announc
-00000240: 6572 7321 2a2a 2053 6565 202a 2a77 686f  ers!** See **who
-00000250: 2773 206f 6e20 7468 6520 7472 6163 6b2a  's on the track*
-00000260: 2a20 2869 6e63 6c75 6469 6e67 2070 6f73  * (including pos
-00000270: 6974 696f 6e73 292c 2074 6865 206d 6f73  itions), the mos
-00000280: 7420 7265 6365 6e74 202a 2a70 656e 616c  t recent **penal
-00000290: 7469 6573 2a2a 2c20 616e 6420 2a2a 726f  ties**, and **ro
-000002a0: 7374 6572 732a 2a20 666f 7220 626f 7468  sters** for both
-000002b0: 2074 6561 6d73 2061 6e64 206f 6666 6963   teams and offic
-000002c0: 6961 6c73 2e20 596f 7520 6361 6e20 6576  ials. You can ev
-000002d0: 656e 205b 636f 6e6e 6563 7420 746f 2061  en [connect to a
-000002e0: 206c 6976 6520 7363 6f72 6562 6f61 7264   live scoreboard
-000002f0: 2066 726f 6d20 616e 7977 6865 7265 206f   from anywhere o
-00000300: 6e20 7468 6520 496e 7465 726e 6574 5d28  n the Internet](
-00000310: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000320: 6f6d 2f64 686d 6179 2f6a 616d 7374 6174  om/dhmay/jamstat
-00000330: 7323 636f 6e6e 6563 7469 6e67 2d74 6f2d  s#connecting-to-
-00000340: 612d 7072 6f78 6965 642d 7363 6f72 6562  a-proxied-scoreb
-00000350: 6f61 7264 2d66 726f 6d2d 7468 652d 696e  oard-from-the-in
-00000360: 7465 726e 6574 2920 7573 696e 6720 7773  ternet) using ws
-00000370: 7072 6f78 7921 0a0a 2323 2323 2046 6561  proxy!..#### Fea
-00000380: 7475 7265 730a 0a2a 2047 6574 2075 702d  tures..* Get up-
-00000390: 746f 2d64 6174 6520 6761 6d65 2064 6174  to-date game dat
-000003a0: 6120 6672 6f6d 2061 206c 6976 6520 7363  a from a live sc
-000003b0: 6f72 6562 6f61 7264 0a2a 2056 6973 7561  oreboard.* Visua
-000003c0: 6c69 7a65 2070 6f69 6e74 7320 7065 7220  lize points per 
-000003d0: 6a61 6d2c 206c 6561 642c 206d 6561 6e20  jam, lead, mean 
-000003e0: 6e65 7420 706f 696e 7473 2c20 6361 6c6c  net points, call
-000003f0: 6f66 6673 2c20 7469 6d65 2074 6f20 696e  offs, time to in
-00000400: 6974 6961 6c20 7061 7373 2c20 7065 6e61  itial pass, pena
-00000410: 6c74 6965 7320 616e 6420 6d75 6368 206d  lties and much m
-00000420: 6f72 650a 2a20 5265 6164 2069 6e20 4a53  ore.* Read in JS
-00000430: 4f4e 2066 696c 6573 2066 726f 6d20 636f  ON files from co
-00000440: 6d70 6c65 7465 6420 6761 6d65 7320 6f72  mpleted games or
-00000450: 2063 6f6e 6e65 6374 2074 6f20 6120 7275   connect to a ru
-00000460: 6e6e 696e 6720 7363 6f72 6562 6f61 7264  nning scoreboard
-00000470: 0a2a 2053 6176 6520 706c 6f74 7320 6173  .* Save plots as
-00000480: 2050 4446 2066 696c 6573 2c20 6f72 2073   PDF files, or s
-00000490: 7461 7274 2061 2077 6562 7365 7276 6572  tart a webserver
-000004a0: 2074 6861 7420 616e 796f 6e65 206f 6e20   that anyone on 
-000004b0: 796f 7572 206e 6574 776f 726b 2063 616e  your network can
-000004c0: 2062 726f 7773 6520 746f 0a0a 446f 2079   browse to..Do y
-000004d0: 6f75 2061 6c72 6561 6479 206c 6f76 6520  ou already love 
-000004e0: 4a61 6d73 7461 7473 3f20 5b54 656c 6c20  Jamstats? [Tell 
-000004f0: 7573 2061 626f 7574 2069 7421 5d28 6874  us about it!](ht
-00000500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000510: 2f64 686d 6179 2f6a 616d 7374 6174 732f  /dhmay/jamstats/
-00000520: 6973 7375 6573 2f6e 6577 3f61 7373 6967  issues/new?assig
-00000530: 6e65 6573 3d26 6c61 6265 6c73 3d74 6573  nees=&labels=tes
-00000540: 7469 6d6f 6e69 616c 2674 656d 706c 6174  timonial&templat
-00000550: 653d 7465 7374 696d 6f6e 6961 6c2e 6d64  e=testimonial.md
-00000560: 2674 6974 6c65 3d29 0a0a 0a23 2323 2320  &title=)...#### 
-00000570: 496e 7374 7275 6374 696f 6e73 0a0a 5175  Instructions..Qu
-00000580: 6963 6b73 7461 7274 3a20 646f 776e 6c6f  ickstart: downlo
-00000590: 6164 205b 7468 6520 6c61 7465 7374 2072  ad [the latest r
-000005a0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-000005b0: 6769 7468 7562 2e63 6f6d 2f64 686d 6179  github.com/dhmay
-000005c0: 2f6a 616d 7374 6174 732f 7265 6c65 6173  /jamstats/releas
-000005d0: 6573 2920 616e 6420 7275 6e20 6974 2e0a  es) and run it..
-000005e0: 0a49 6e20 6d6f 7265 2064 6574 6169 6c3a  .In more detail:
-000005f0: 0a0a 2a20 2a2a 5b49 6e73 7461 6c6c 6174  ..* **[Installat
-00000600: 696f 6e5d 2823 696e 7374 616c 6c61 7469  ion](#installati
-00000610: 6f6e 292a 2a0a 2a20 2a2a 5b55 7361 6765  on)**.* **[Usage
-00000620: 5d28 2375 7361 6765 292a 2a0a 0a23 2320  ](#usage)**..## 
-00000630: 5361 6d70 6c65 2070 6c6f 7473 0a0a 3c70  Sample plots..<p
-00000640: 2061 6c69 676e 3d22 6c65 6674 223e 3c69   align="left"><i
-00000650: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000660: 6769 7468 7562 2e63 6f6d 2f64 686d 6179  github.com/dhmay
-00000670: 2f6a 616d 7374 6174 732f 626c 6f62 2f6d  /jamstats/blob/m
-00000680: 6169 6e2f 7265 736f 7572 6365 732f 6375  ain/resources/cu
-00000690: 7272 656e 745f 736b 6174 6572 732e 706e  rrent_skaters.pn
-000006a0: 6722 2077 6964 7468 3d22 3530 3022 3e3c  g" width="500"><
-000006b0: 2f70 3e0a 0a3c 7020 616c 6967 6e3d 226c  /p>..<p align="l
-000006c0: 6566 7422 3e3c 696d 6720 7372 633d 2268  eft"><img src="h
-000006d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000006e0: 6d2f 6468 6d61 792f 6a61 6d73 7461 7473  m/dhmay/jamstats
-000006f0: 2f62 6c6f 622f 6d61 696e 2f72 6573 6f75  /blob/main/resou
-00000700: 7263 6573 2f63 756d 756c 6174 6976 655f  rces/cumulative_
-00000710: 7363 6f72 655f 6279 5f6a 616d 2e70 6e67  score_by_jam.png
-00000720: 2220 7769 6474 683d 2235 3030 223e 3c2f  " width="500"></
-00000730: 703e 0a0a 3c70 2061 6c69 676e 3d22 6c65  p>..<p align="le
-00000740: 6674 223e 3c69 6d67 2073 7263 3d22 6874  ft"><img src="ht
-00000750: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000760: 2f64 686d 6179 2f6a 616d 7374 6174 732f  /dhmay/jamstats/
-00000770: 626c 6f62 2f6d 6169 6e2f 7265 736f 7572  blob/main/resour
-00000780: 6365 732f 6a61 6d6d 6572 5f73 7461 7473  ces/jammer_stats
-00000790: 2e70 6e67 2220 7769 6474 683d 2235 3030  .png" width="500
-000007a0: 223e 3c2f 703e 0a0a 5768 6174 2070 656e  "></p>..What pen
-000007b0: 616c 7469 6573 2067 6f74 2079 6f75 2064  alties got you d
-000007c0: 6f77 6e20 7468 6520 6d6f 7374 3f0a 0a3c  own the most?..<
-000007d0: 7020 616c 6967 6e3d 226c 6566 7422 3e3c  p align="left"><
-000007e0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000007f0: 2f67 6974 6875 622e 636f 6d2f 6468 6d61  /github.com/dhma
-00000800: 792f 6a61 6d73 7461 7473 2f62 6c6f 622f  y/jamstats/blob/
-00000810: 6d61 696e 2f72 6573 6f75 7263 6573 2f74  main/resources/t
-00000820: 6561 6d5f 7065 6e61 6c74 795f 636f 756e  eam_penalty_coun
-00000830: 7473 2e70 6e67 2220 7769 6474 683d 2235  ts.png" width="5
-00000840: 3030 223e 3c2f 703e 0a0a 3c70 2061 6c69  00"></p>..<p ali
-00000850: 676e 3d22 6c65 6674 223e 3c69 6d67 2073  gn="left"><img s
-00000860: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-00000870: 7562 2e63 6f6d 2f64 686d 6179 2f6a 616d  ub.com/dhmay/jam
-00000880: 7374 6174 732f 626c 6f62 2f6d 6169 6e2f  stats/blob/main/
-00000890: 7265 736f 7572 6365 732f 736b 6174 6572  resources/skater
-000008a0: 5f73 7461 7473 2e70 6e67 2220 7769 6474  _stats.png" widt
-000008b0: 683d 2235 3030 223e 3c2f 703e 0a0a 3c70  h="500"></p>..<p
-000008c0: 2061 6c69 676e 3d22 6c65 6674 223e 3c69   align="left"><i
-000008d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000008e0: 6769 7468 7562 2e63 6f6d 2f64 686d 6179  github.com/dhmay
-000008f0: 2f6a 616d 7374 6174 732f 626c 6f62 2f6d  /jamstats/blob/m
-00000900: 6169 6e2f 7265 736f 7572 6365 732f 6a61  ain/resources/ja
-00000910: 6d5f 706f 696e 7473 5f62 6172 706c 6f74  m_points_barplot
-00000920: 2e70 6e67 2220 7769 6474 683d 2235 3030  .png" width="500
-00000930: 223e 3c2f 703e 0a0a 5573 6520 7468 6520  "></p>..Use the 
-00000940: 636f 6c6f 7273 2064 6566 696e 6564 2066  colors defined f
-00000950: 6f72 2065 6163 6820 7465 616d 2069 6e20  or each team in 
-00000960: 7468 6520 7363 6f72 6562 6f61 7264 2066  the scoreboard f
-00000970: 696c 652c 206f 7220 7072 6f76 6964 6520  ile, or provide 
-00000980: 796f 7572 206f 776e 206f 6e20 7468 6520  your own on the 
-00000990: 636f 6d6d 616e 6420 6c69 6e65 2e0a 0a3c  command line...<
-000009a0: 7020 616c 6967 6e3d 226c 6566 7422 3e3c  p align="left"><
-000009b0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000009c0: 2f67 6974 6875 622e 636f 6d2f 6468 6d61  /github.com/dhma
-000009d0: 792f 6a61 6d73 7461 7473 2f62 6c6f 622f  y/jamstats/blob/
-000009e0: 6d61 696e 2f72 6573 6f75 7263 6573 2f6c  main/resources/l
-000009f0: 6561 645f 7375 6d6d 6172 792e 706e 6722  ead_summary.png"
-00000a00: 2077 6964 7468 3d22 3530 3022 3e3c 2f70   width="500"></p
-00000a10: 3e0a 0a57 616e 7420 746f 2064 6f20 796f  >..Want to do yo
-00000a20: 7572 206f 776e 2061 6e61 6c79 7469 6373  ur own analytics
-00000a30: 3f20 5361 7665 2064 6f77 6e20 6120 7370  ? Save down a sp
-00000a40: 7265 6164 7368 6565 7420 616e 6420 646f  readsheet and do
-00000a50: 2079 6f75 7220 6f77 6e20 7468 696e 6720   your own thing 
-00000a60: 7769 7468 2069 7421 0a0a 3c70 2061 6c69  with it!..<p ali
-00000a70: 676e 3d22 6c65 6674 223e 3c69 6d67 2073  gn="left"><img s
-00000a80: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-00000a90: 7562 2e63 6f6d 2f64 686d 6179 2f6a 616d  ub.com/dhmay/jam
-00000aa0: 7374 6174 732f 626c 6f62 2f6d 6169 6e2f  stats/blob/main/
-00000ab0: 7265 736f 7572 6365 732f 7473 765f 6f75  resources/tsv_ou
-00000ac0: 7470 7574 5f73 6372 6565 6e73 686f 742e  tput_screenshot.
-00000ad0: 706e 6722 2077 6964 7468 3d22 3530 3022  png" width="500"
-00000ae0: 3e3c 2f70 3e0a 0a0a 2323 2049 6e73 7461  ></p>...## Insta
-00000af0: 6c6c 6174 696f 6e0a 0a2a 2057 696e 646f  llation..* Windo
-00000b00: 7773 3a20 676f 2074 6f20 7468 6520 5b6c  ws: go to the [l
-00000b10: 6174 6573 7420 7265 6c65 6173 655d 2868  atest release](h
-00000b20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b30: 6d2f 6468 6d61 792f 6a61 6d73 7461 7473  m/dhmay/jamstats
-00000b40: 2f72 656c 6561 7365 7329 2061 6e64 2064  /releases) and d
-00000b50: 6f77 6e6c 6f61 6420 606a 616d 7374 6174  ownload `jamstat
-00000b60: 732d 3c76 6572 7369 6f6e 3e2e 6578 6560  s-<version>.exe`
-00000b70: 0a2a 204d 6163 3a20 676f 2074 6f20 7468  .* Mac: go to th
-00000b80: 6520 5b6c 6174 6573 7420 7265 6c65 6173  e [latest releas
-00000b90: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000ba0: 622e 636f 6d2f 6468 6d61 792f 6a61 6d73  b.com/dhmay/jams
-00000bb0: 7461 7473 2f72 656c 6561 7365 7329 2061  tats/releases) a
-00000bc0: 6e64 2064 6f77 6e6c 6f61 6420 606a 616d  nd download `jam
-00000bd0: 7374 6174 732d 6d61 632d 3c76 6572 7369  stats-mac-<versi
-00000be0: 6f6e 3e2e 7a69 7060 2c20 7468 656e 2075  on>.zip`, then u
-00000bf0: 6e7a 6970 2074 6861 7420 6669 6c65 2069  nzip that file i
-00000c00: 6e74 6f20 796f 7572 2041 7070 6c69 6361  nto your Applica
-00000c10: 7469 6f6e 7320 6469 7265 6374 6f72 7920  tions directory 
-00000c20: 286f 7220 7768 6572 6576 6572 2079 6f75  (or wherever you
-00000c30: 2077 616e 7420 746f 2072 756e 204a 616d   want to run Jam
-00000c40: 7374 6174 7320 6672 6f6d 290a 2020 2020  stats from).    
-00000c50: 2a20 4e6f 7465 2074 6861 7420 7468 6520  * Note that the 
-00000c60: 4d61 6320 6170 7020 6973 2070 6172 7469  Mac app is parti
-00000c70: 6375 6c61 726c 7920 736c 6f77 2074 6f20  cularly slow to 
-00000c80: 7374 6172 7420 7570 0a2a 2041 6e79 2070  start up.* Any p
-00000c90: 6c61 7466 6f72 6d3a 2069 6e73 7461 6c6c  latform: install
-00000ca0: 2050 7974 686f 6e20 332e 3920 6f72 2068   Python 3.9 or h
-00000cb0: 6967 6865 722c 2074 6865 6e20 7275 6e20  igher, then run 
-00000cc0: 6070 6970 2069 6e73 7461 6c6c 206a 616d  `pip install jam
-00000cd0: 7374 6174 7360 2e20 5468 6174 2077 696c  stats`. That wil
-00000ce0: 6c20 7075 7420 606a 616d 7374 6174 7360  l put `jamstats`
-00000cf0: 206f 6e20 796f 7572 2070 6174 6820 736f   on your path so
-00000d00: 2079 6f75 2063 616e 2072 756e 2069 7420   you can run it 
-00000d10: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
-00000d20: 206c 696e 652e 0a0a 2323 2055 7361 6765   line...## Usage
-00000d30: 0a0a 5b46 756c 6c20 7573 6572 206d 616e  ..[Full user man
-00000d40: 7561 6c20 2850 4446 295d 2868 7474 7073  ual (PDF)](https
-00000d50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6468  ://github.com/dh
-00000d60: 6d61 792f 6a61 6d73 7461 7473 2f62 6c6f  may/jamstats/blo
-00000d70: 622f 6d61 696e 2f72 6573 6f75 7263 6573  b/main/resources
-00000d80: 2f6a 616d 7374 6174 735f 7573 6572 5f6d  /jamstats_user_m
-00000d90: 616e 7561 6c2e 7064 6629 2c20 696e 636c  anual.pdf), incl
-00000da0: 7564 696e 6720 686f 7720 746f 2073 7461  uding how to sta
-00000db0: 7274 204a 616d 7374 6174 7320 7570 2061  rt Jamstats up a
-00000dc0: 6e64 2068 6f77 2074 6f20 696e 7465 7270  nd how to interp
-00000dd0: 7265 7420 616c 6c20 7468 6520 706c 6f74  ret all the plot
-00000de0: 732e 0a0a 2323 2320 4472 6167 2d61 6e64  s...### Drag-and
-00000df0: 2d64 726f 700a 0a4f 6e20 5769 6e64 6f77  -drop..On Window
-00000e00: 7320 6f72 204d 6163 2c20 746f 2067 656e  s or Mac, to gen
-00000e10: 6572 6174 6520 6120 706c 6f74 7320 5044  erate a plots PD
-00000e20: 462c 2079 6f75 2063 616e 2073 696d 706c  F, you can simpl
-00000e30: 7920 2a2a 6472 6167 2061 6e64 2064 726f  y **drag and dro
-00000e40: 702a 2a20 796f 7572 2067 616d 6520 4a53  p** your game JS
-00000e50: 4f4e 2066 696c 6520 6f6e 746f 2074 6865  ON file onto the
-00000e60: 206a 616d 7374 6174 732e 6578 6520 6669   jamstats.exe fi
-00000e70: 6c65 206f 7220 4a61 6d73 7461 7473 2061  le or Jamstats a
-00000e80: 7070 2e20 5468 6174 2077 696c 6c20 6765  pp. That will ge
-00000e90: 6e65 7261 7465 2061 2060 2e70 6466 6020  nerate a `.pdf` 
-00000ea0: 6669 6c65 2069 6e20 7468 6520 7361 6d65  file in the same
-00000eb0: 2064 6972 6563 746f 7279 2061 7320 796f   directory as yo
-00000ec0: 7572 2060 2e6a 736f 6e60 2066 696c 652c  ur `.json` file,
-00000ed0: 2077 6974 6820 7468 6520 7361 6d65 206e   with the same n
-00000ee0: 616d 6520 6275 7420 7769 7468 2074 6865  ame but with the
-00000ef0: 2060 2e6a 736f 6e60 2065 7874 656e 7369   `.json` extensi
-00000f00: 6f6e 2072 6570 6c61 6365 6420 7769 7468  on replaced with
-00000f10: 2060 2e70 6466 602e 0a0a 2323 2320 4755   `.pdf`...### GU
-00000f20: 490a 0a44 6f75 626c 652d 636c 6963 6b20  I..Double-click 
-00000f30: 6f6e 2074 6865 206a 616d 7374 6174 7320  on the jamstats 
-00000f40: 6578 6563 7574 6162 6c65 2074 6f20 6f70  executable to op
-00000f50: 656e 2061 2067 7261 7068 6963 616c 2077  en a graphical w
-00000f60: 696e 646f 7720 746f 2073 7065 6369 6679  indow to specify
-00000f70: 2079 6f75 7220 7061 7261 6d65 7465 7273   your parameters
-00000f80: 2e20 0a0a 546f 2063 6f6e 6e65 6374 2074  . ..To connect t
-00000f90: 6f20 6120 7363 6f72 6562 6f61 7264 2c20  o a scoreboard, 
-00000fa0: 616c 6c20 796f 7520 6e65 6564 2074 6f20  all you need to 
-00000fb0: 7370 6563 6966 7920 6973 2060 7363 6f72  specify is `scor
-00000fc0: 6562 6f61 7264 7365 7276 6572 6020 2d2d  eboardserver` --
-00000fd0: 2067 6976 6520 7468 6174 2074 6865 2063   give that the c
-00000fe0: 6f6d 6269 6e65 6420 4950 2061 6464 7265  ombined IP addre
-00000ff0: 7373 2061 6e64 2070 6f72 7420 6e75 6d62  ss and port numb
-00001000: 6572 206f 6620 796f 7572 2073 636f 7265  er of your score
-00001010: 626f 6172 6420 7365 7276 6572 2028 652e  board server (e.
-00001020: 672e 2c20 6031 3732 2e32 312e 3132 2e37  g., `172.21.12.7
-00001030: 3a38 3030 3060 292c 2061 7320 7265 706f  :8000`), as repo
-00001040: 7274 6564 2069 6e20 7468 6520 7363 6f72  rted in the scor
-00001050: 6562 6f61 7264 2047 5549 2e0a 0a57 6974  eboard GUI...Wit
-00001060: 6820 7468 6174 2075 7361 6765 2c20 4a61  h that usage, Ja
-00001070: 6d73 7461 7473 2077 696c 6c20 7374 6172  mstats will star
-00001080: 7420 6974 7320 6f77 6e20 7365 7276 6572  t its own server
-00001090: 206f 6e20 796f 7572 206c 6170 746f 702c   on your laptop,
-000010a0: 2061 6e64 2074 6865 206f 7574 7075 7420   and the output 
-000010b0: 696e 2074 6865 2047 5549 2077 696e 646f  in the GUI windo
-000010c0: 7720 7769 6c6c 2074 656c 6c20 796f 7520  w will tell you 
-000010d0: 7768 6572 6520 746f 2070 6f69 6e74 2079  where to point y
-000010e0: 6f75 7220 6272 6f77 7365 722e 2042 7920  our browser. By 
-000010f0: 6465 6661 756c 742c 2074 6861 7427 7320  default, that's 
-00001100: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
-00001110: 743a 3830 3830 602c 2077 6869 6368 2077  t:8080`, which w
-00001120: 696c 6c20 6d61 6b65 204a 616d 7374 6174  ill make Jamstat
-00001130: 7320 6176 6169 6c61 626c 6520 6f6e 6c79  s available only
-00001140: 206f 6e20 796f 7572 206f 776e 206d 6163   on your own mac
-00001150: 6869 6e65 2e20 4966 2079 6f75 2077 616e  hine. If you wan
-00001160: 7420 746f 206d 616b 6520 4a61 6d73 7461  t to make Jamsta
-00001170: 7473 2061 7661 696c 6162 6c65 2074 6f20  ts available to 
-00001180: 6f74 6865 7220 6272 6f77 7365 7273 206f  other browsers o
-00001190: 6e20 796f 7572 206e 6574 776f 726b 2c20  n your network, 
-000011a0: 7365 7420 606a 616d 7374 6174 7369 7060  set `jamstatsip`
-000011b0: 2074 6f20 796f 7572 2063 6f6d 7075 7465   to your compute
-000011c0: 7227 7320 4950 2061 6464 7265 7373 2e0a  r's IP address..
-000011d0: 0a59 6f75 2063 616e 2061 6c73 6f20 7573  .You can also us
-000011e0: 6520 7468 6520 4755 4920 746f 2073 7065  e the GUI to spe
-000011f0: 6369 6679 2061 6c6c 206f 7468 6572 2061  cify all other a
-00001200: 7267 756d 656e 7473 2079 6f75 2063 6f75  rguments you cou
-00001210: 6c64 2073 7065 6369 6679 2066 726f 6d20  ld specify from 
-00001220: 7468 6520 636f 6d6d 616e 646c 696e 652e  the commandline.
-00001230: 0a0a 2323 2320 436f 6e6e 6563 7469 6e67  ..### Connecting
-00001240: 2074 6f20 6120 7072 6f78 6965 6420 7363   to a proxied sc
-00001250: 6f72 6562 6f61 7264 2066 726f 6d20 7468  oreboard from th
-00001260: 6520 496e 7465 726e 6574 0a0a 4974 2773  e Internet..It's
-00001270: 2070 6f73 7369 626c 6520 746f 2075 7365   possible to use
-00001280: 204a 616d 7374 6174 7320 6672 6f6d 2061   Jamstats from a
-00001290: 6e79 7768 6572 6520 696e 2074 6865 2077  nywhere in the w
-000012a0: 6f72 6c64 2074 6f20 636f 6e6e 6563 7420  orld to connect 
-000012b0: 746f 2061 2072 756e 6e69 6e67 2073 636f  to a running sco
-000012c0: 7265 626f 6172 6421 2054 6869 7320 6c65  reboard! This le
-000012d0: 7473 202a 2a72 656d 6f74 6520 616e 6e6f  ts **remote anno
-000012e0: 756e 6365 7273 2a2a 2075 7365 204a 616d  uncers** use Jam
-000012f0: 7374 6174 7320 746f 2068 656c 7020 7769  stats to help wi
-00001300: 7468 2063 616c 6c69 6e67 2067 616d 6573  th calling games
-00001310: 2e20 4865 7265 2773 2068 6f77 3a0a 0a23  . Here's how:..#
-00001320: 2323 2320 4174 2074 6865 2074 7261 636b  ### At the track
-00001330: 3a20 7365 7474 696e 6720 7570 2061 2070  : setting up a p
-00001340: 726f 7879 0a0a 312e 2044 6f77 6e6c 6f61  roxy..1. Downloa
-00001350: 6420 5b77 7370 726f 7879 5d28 6874 7470  d [wsproxy](http
-00001360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f44  s://github.com/D
-00001370: 6572 6279 5374 6174 732f 7773 7072 6f78  erbyStats/wsprox
-00001380: 7929 2061 6e64 2066 6f6c 6c6f 7720 6974  y) and follow it
-00001390: 7320 696e 7374 7275 6374 696f 6e73 2074  s instructions t
-000013a0: 6f20 7365 7420 7570 2061 2070 726f 7879  o set up a proxy
-000013b0: 2e20 5468 6973 2077 696c 6c20 6665 6564  . This will feed
-000013c0: 2079 6f75 7220 7363 6f72 6562 6f61 7264   your scoreboard
-000013d0: 2064 6174 612c 2072 6561 642d 6f6e 6c79   data, read-only
-000013e0: 2c20 746f 2074 6865 2049 6e74 6572 6e65  , to the Interne
-000013f0: 740a 2020 2020 2a20 4966 2079 6f75 2772  t.    * If you'r
-00001400: 6520 7573 696e 6720 7468 6520 6465 6661  e using the defa
-00001410: 756c 7420 7363 6f72 6562 6f61 7264 2073  ult scoreboard s
-00001420: 6574 7469 6e67 732c 2074 6865 2064 6566  ettings, the def
-00001430: 6175 6c74 2077 7370 726f 7879 2073 6574  ault wsproxy set
-00001440: 7469 6e67 7320 7769 6c6c 2077 6f72 6b20  tings will work 
-00001450: 6669 6e65 2e20 0a20 2020 202a 2049 6620  fine. .    * If 
-00001460: 6e6f 742c 2070 6179 2061 7474 656e 7469  not, pay attenti
-00001470: 6f6e 2074 6f20 7468 6520 706f 7274 2079  on to the port y
-00001480: 6f75 2772 6520 7275 6e6e 696e 6720 796f  ou're running yo
-00001490: 7572 2073 636f 7265 626f 6172 6420 6f6e  ur scoreboard on
-000014a0: 2c20 616e 6420 6368 616e 6765 2066 726f  , and change fro
-000014b0: 6d20 3830 3030 2074 6f20 7468 6174 2073  m 8000 to that s
-000014c0: 616d 6520 706f 7274 2069 6e20 7773 7072  ame port in wspr
-000014d0: 6f78 7927 7320 636f 6e66 6967 2e69 6e69  oxy's config.ini
-000014e0: 2066 696c 650a 322e 2059 6f75 7220 7072   file.2. Your pr
-000014f0: 6f78 7920 6361 6e20 7365 6e64 2079 6f75  oxy can send you
-00001500: 7220 7363 6f72 6562 6f61 7264 2064 6174  r scoreboard dat
-00001510: 6120 7768 6572 6576 6572 2079 6f75 2074  a wherever you t
-00001520: 656c 6c20 6974 2074 6f2e 204f 6e20 7468  ell it to. On th
-00001530: 6520 6f74 6865 7220 656e 642c 2074 6865  e other end, the
-00001540: 7265 206e 6565 6473 2074 6f20 6265 2061  re needs to be a
-00001550: 6e6f 7468 6572 2063 6f70 7920 6f66 2077  nother copy of w
-00001560: 7370 726f 7879 2072 756e 6e69 6e67 2e0a  sproxy running..
-00001570: 2020 2020 2a20 5769 7468 2074 6865 2064      * With the d
-00001580: 6566 6175 6c74 2063 6f6e 6669 6775 7261  efault configura
-00001590: 7469 6f6e 2c20 796f 7572 2070 726f 7879  tion, your proxy
-000015a0: 2064 6174 6120 7769 6c6c 2062 6520 7365   data will be se
-000015b0: 6e74 2074 6f20 6120 6e65 7720 7375 6264  nt to a new subd
-000015c0: 6f6d 6169 6e20 6f66 2060 6465 7262 7973  omain of `derbys
-000015d0: 7461 7473 2e65 7560 0a20 2020 2020 2020  tats.eu`.       
-000015e0: 202a 2065 2e67 2e2c 205b 6874 7470 733a   * e.g., [https:
-000015f0: 2f2f 7766 7464 6163 6365 7373 2e64 6572  //wftdaccess.der
-00001600: 6279 7374 6174 732e 6575 2f5d 2868 7474  bystats.eu/](htt
-00001610: 7073 3a2f 2f77 6674 6461 6363 6573 732e  ps://wftdaccess.
-00001620: 6465 7262 7973 7461 7473 2e65 752f 292c  derbystats.eu/),
-00001630: 2062 7574 2069 7420 7769 6c6c 2062 6520   but it will be 
-00001640: 736f 6d65 7468 696e 6720 656c 7365 2075  something else u
-00001650: 6e69 7175 6520 746f 2079 6f75 7220 7363  nique to your sc
-00001660: 6f72 6562 6f61 7264 0a20 2020 202a 2057  oreboard.    * W
-00001670: 6865 6e20 796f 7520 7374 6172 7420 7773  hen you start ws
-00001680: 7072 6f78 792c 2069 7420 7769 6c6c 2074  proxy, it will t
-00001690: 656c 6c20 796f 7520 7768 6572 6520 7468  ell you where th
-000016a0: 6520 6461 7461 2069 7320 676f 696e 672e  e data is going.
-000016b0: 200a 2020 2020 2020 2020 2a20 466f 7220   .        * For 
-000016c0: 6578 616d 706c 652c 2060 4469 7370 6c61  example, `Displa
-000016d0: 7920 5552 4c3a 2068 7474 7073 3a2f 2f6a  y URL: https://j
-000016e0: 616d 6d65 722d 6c61 6e65 2e64 6572 6279  ammer-lane.derby
-000016f0: 7374 6174 732e 6575 600a 2020 2020 2020  stats.eu`.      
-00001700: 2020 2a20 4769 7665 2074 6869 7320 746f    * Give this to
-00001710: 2074 6865 2070 6572 736f 6e20 7768 6f27   the person who'
-00001720: 6c6c 2062 6520 7275 6e6e 696e 6720 4a61  ll be running Ja
-00001730: 6d73 7461 7473 2072 656d 6f74 656c 792e  mstats remotely.
-00001740: 0a20 2020 2020 2020 200a 2323 2323 2052  .        .#### R
-00001750: 656d 6f74 656c 793a 2072 756e 6e69 6e67  emotely: running
-00001760: 204a 616d 7374 6174 7320 746f 2063 6f6e   Jamstats to con
-00001770: 6e65 6374 2074 6f20 6120 7072 6f78 790a  nect to a proxy.
-00001780: 0a31 2e20 4765 7420 7468 6520 2244 6973  .1. Get the "Dis
-00001790: 706c 6179 2055 524c 2220 6672 6f6d 2074  play URL" from t
-000017a0: 6865 2070 6572 736f 6e20 7768 6f20 7365  he person who se
-000017b0: 7420 7570 2077 7370 726f 7879 0a20 2020  t up wsproxy.   
-000017c0: 202a 2046 6f72 2065 7861 6d70 6c65 2c20   * For example, 
-000017d0: 6068 7474 7073 3a2f 2f6a 616d 6d65 722d  `https://jammer-
-000017e0: 6c61 6e65 2e64 6572 6279 7374 6174 732e  lane.derbystats.
-000017f0: 6575 600a 322e 2053 7461 7274 2075 7020  eu`.2. Start up 
-00001800: 4a61 6d73 7461 7473 2061 6e64 2067 6976  Jamstats and giv
-00001810: 6520 6974 2074 776f 2061 7267 756d 656e  e it two argumen
-00001820: 7473 2028 6569 7468 6572 2074 6872 6f75  ts (either throu
-00001830: 6768 2074 6865 2047 5549 206f 7220 6f6e  gh the GUI or on
-00001840: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00001850: 6529 3a0a 2020 2020 2a20 6073 636f 7265  e):.    * `score
-00001860: 626f 6172 6473 6572 7665 7260 3a20 6d61  boardserver`: ma
-00001870: 6b65 2074 6869 7320 7468 6520 6675 6c6c  ke this the full
-00001880: 2073 7562 646f 6d61 696e 206f 6620 7468   subdomain of th
-00001890: 6520 2244 6973 706c 6179 2055 524c 222c  e "Display URL",
-000018a0: 2077 6974 686f 7574 2074 6865 2060 6874   without the `ht
-000018b0: 7470 733a 2f2f 6020 7061 7274 2c20 7769  tps://` part, wi
-000018c0: 7468 2060 3a34 3433 6020 6164 6465 6420  th `:443` added 
-000018d0: 746f 2074 6865 2065 6e64 0a20 2020 2020  to the end.     
-000018e0: 2020 202a 2046 6f72 2065 7861 6d70 6c65     * For example
-000018f0: 3a20 606a 616d 6d65 722d 6c61 6e65 2e64  : `jammer-lane.d
-00001900: 6572 6279 7374 6174 732e 6575 3a34 3433  erbystats.eu:443
-00001910: 600a 2020 2020 2a20 6073 736c 603a 2073  `.    * `ssl`: s
-00001920: 6574 2074 6869 7320 746f 2060 7472 7565  et this to `true
-00001930: 6020 2864 6566 6175 6c74 2069 7320 6066  ` (default is `f
-00001940: 616c 7365 6029 0a0a 4578 616d 706c 6520  alse`)..Example 
-00001950: 6f66 2068 6f77 2074 6869 7320 6c6f 6f6b  of how this look
-00001960: 7320 6f6e 2074 6865 2063 6f6d 6d61 6e64  s on the command
-00001970: 6c69 6e65 3a0a 0a60 7079 7468 6f6e 2062  line:..`python b
-00001980: 696e 2f6a 616d 7374 6174 7320 2d2d 7363  in/jamstats --sc
-00001990: 6f72 6562 6f61 7264 7365 7276 6572 3d6a  oreboardserver=j
-000019a0: 616d 6d65 722d 6c61 6e65 2e64 6572 6279  ammer-lane.derby
-000019b0: 7374 6174 732e 6575 3a34 3433 202d 2d73  stats.eu:443 --s
-000019c0: 736c 600a 0a45 7861 6d70 6c65 206f 6620  sl`..Example of 
-000019d0: 686f 7720 7468 6973 206c 6f6f 6b73 2069  how this looks i
-000019e0: 6e20 7468 6520 4755 493a 0a0a 215b 696d  n the GUI:..![im
-000019f0: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-00001a00: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00001a10: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-00001a20: 3134 3037 372f 3232 3933 3131 3638 352d  14077/229311685-
-00001a30: 6234 3433 3539 6463 2d35 3530 312d 3433  b44359dc-5501-43
-00001a40: 3562 2d61 6534 342d 3930 3339 3331 3766  5b-ae44-9039317f
-00001a50: 3266 3039 2e70 6e67 290a 0a54 6861 7427  2f09.png)..That'
-00001a60: 7320 6974 2120 4966 2074 6861 7420 7365  s it! If that se
-00001a70: 7475 7020 616c 6c20 776f 726b 6564 2063  tup all worked c
-00001a80: 6f72 7265 6374 6c79 2c20 4a61 6d73 7461  orrectly, Jamsta
-00001a90: 7473 2073 686f 756c 6420 6e6f 7720 6265  ts should now be
-00001aa0: 6861 7665 2065 7861 6374 6c79 2061 7320  have exactly as 
-00001ab0: 7468 6f75 6768 2079 6f75 2077 6572 6520  though you were 
-00001ac0: 7269 6768 7420 7468 6572 6520 6174 2074  right there at t
-00001ad0: 6865 2074 7261 636b 2e0a 0a23 2323 2043  he track...### C
-00001ae0: 6f6d 6d61 6e64 6c69 6e65 0a0a 5468 6520  ommandline..The 
-00001af0: 636f 6d6d 616e 6420 796f 7527 6c6c 2075  command you'll u
-00001b00: 7365 2069 7320 7468 6520 7361 6d65 2061  se is the same a
-00001b10: 7320 7468 6520 6e61 6d65 206f 6620 7468  s the name of th
-00001b20: 6520 6669 6c65 2079 6f75 2064 6f77 6e6c  e file you downl
-00001b30: 6f61 6465 6420 2865 2e67 2e2c 2060 6a61  oaded (e.g., `ja
-00001b40: 6d73 7461 7473 2d76 302e 332e 342d 616c  mstats-v0.3.4-al
-00001b50: 7068 612e 6578 6560 206f 6e20 5769 6e64  pha.exe` on Wind
-00001b60: 6f77 732c 206f 7220 606a 616d 7374 6174  ows, or `jamstat
-00001b70: 732d 6d61 632d 7630 2e33 2e34 2d61 6c70  s-mac-v0.3.4-alp
-00001b80: 6861 6020 6f6e 204d 6163 292e 0a0a 2a49  ha` on Mac)...*I
-00001b90: 6e20 7468 6520 7573 6167 6520 6265 6c6f  n the usage belo
-00001ba0: 772c 2049 276d 2072 6570 6c61 6369 6e67  w, I'm replacing
-00001bb0: 2074 6861 7420 7769 7468 2073 696d 706c   that with simpl
-00001bc0: 7920 606a 616d 7374 6174 7360 2e20 4966  y `jamstats`. If
-00001bd0: 2079 6f75 2077 616e 7420 7468 6520 636f   you want the co
-00001be0: 6d6d 616e 6420 746f 2062 6520 606a 616d  mmand to be `jam
-00001bf0: 7374 6174 7360 2c20 7265 6e61 6d65 2079  stats`, rename y
-00001c00: 6f75 7220 6669 6c65 2074 6f20 606a 616d  our file to `jam
-00001c10: 7374 6174 7360 2e2a 0a0a 4765 7420 6675  stats`.*..Get fu
-00001c20: 6c6c 2063 6f6d 6d61 6e64 6c69 6e65 2068  ll commandline h
-00001c30: 656c 7020 7275 6e6e 696e 6720 7468 6520  elp running the 
-00001c40: 636f 6d6d 616e 6420 7769 7468 2074 6865  command with the
-00001c50: 2060 2d2d 6865 6c70 6020 6172 6775 6d65   `--help` argume
-00001c60: 6e74 2e0a 0a23 2323 2320 4f70 7469 6f6e  nt...#### Option
-00001c70: 2031 3a20 6765 7420 6761 6d65 2064 6174   1: get game dat
-00001c80: 6120 6672 6f6d 2061 204a 534f 4e20 6669  a from a JSON fi
-00001c90: 6c65 0a0a 606a 616d 7374 6174 7320 2d2d  le..`jamstats --
-00001ca0: 6a73 6f6e 6669 6c65 203c 4a53 4f4e 2066  jsonfile <JSON f
-00001cb0: 696c 653e 205b 6f70 7469 6f6e 616c 2061  ile> [optional a
-00001cc0: 7267 756d 656e 7473 5d60 0a0a 7768 6572  rguments]`..wher
-00001cd0: 653a 0a0a 2a20 603c 4a53 4f4e 2066 696c  e:..* `<JSON fil
-00001ce0: 653e 6020 6973 2074 6865 2070 6174 6820  e>` is the path 
-00001cf0: 746f 2061 2073 636f 7265 626f 6172 6420  to a scoreboard 
-00001d00: 4a53 4f4e 2066 696c 650a 2a20 605b 6f70  JSON file.* `[op
-00001d10: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-00001d20: 5d60 3a20 6279 2064 6566 6175 6c74 2c20  ]`: by default, 
-00001d30: 4a61 6d73 7461 7473 2077 696c 6c20 7772  Jamstats will wr
-00001d40: 6974 6520 7468 6520 6f75 7470 7574 2074  ite the output t
-00001d50: 6f20 7468 6520 7361 6d65 2070 6174 6820  o the same path 
-00001d60: 6173 2074 6865 2069 6e70 7574 2066 696c  as the input fil
-00001d70: 652c 2062 7574 2077 6974 6820 222e 6a73  e, but with ".js
-00001d80: 6f6e 2220 7265 706c 6163 6564 2077 6974  on" replaced wit
-00001d90: 6820 222e 7064 6622 2e20 596f 7520 6361  h ".pdf". You ca
-00001da0: 6e20 6164 6a75 7374 2074 6861 7420 6265  n adjust that be
-00001db0: 6861 7669 6f72 2062 7920 7370 6563 6966  havior by specif
-00001dc0: 7969 6e67 2061 6e20 6f75 7470 7574 2060  ying an output `
-00001dd0: 2d2d 6f75 7466 696c 6560 2066 696c 6520  --outfile` file 
-00001de0: 6f72 2075 7369 6e67 2074 6865 2060 2d2d  or using the `--
-00001df0: 6d6f 6465 3d77 6562 6020 6172 6775 6d65  mode=web` argume
-00001e00: 6e74 2074 6f20 7374 6172 7420 6120 7765  nt to start a we
-00001e10: 6273 6572 7665 7220 2873 6565 2062 656c  bserver (see bel
-00001e20: 6f77 292c 2069 6e73 7465 6164 2e0a 2020  ow), instead..  
-00001e30: 2020 2a20 7468 6572 6520 6172 6520 616c    * there are al
-00001e40: 736f 2073 6576 6572 616c 206f 7074 696f  so several optio
-00001e50: 6e73 2c20 6578 706c 6169 6e65 6420 696e  ns, explained in
-00001e60: 2074 6865 2068 656c 7020 6d65 7373 6167   the help messag
-00001e70: 652c 2074 6861 7420 6166 6665 6374 2074  e, that affect t
-00001e80: 6865 2063 6861 7274 7320 7468 6174 2061  he charts that a
-00001e90: 7265 2062 7569 6c74 2e0a 0a23 2323 2320  re built...#### 
-00001ea0: 4f70 7469 6f6e 2032 3a20 636f 6e6e 6563  Option 2: connec
-00001eb0: 7420 746f 2061 2072 756e 6e69 6e67 2073  t to a running s
-00001ec0: 636f 7265 626f 6172 6420 7365 7276 6572  coreboard server
-00001ed0: 0a0a 606a 616d 7374 6174 7320 2d2d 7363  ..`jamstats --sc
-00001ee0: 6f72 6562 6f61 7264 7365 7276 6572 203c  oreboardserver <
-00001ef0: 7365 7276 6572 3a70 6f72 743e 205b 6f70  server:port> [op
-00001f00: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-00001f10: 5d60 0a0a 7768 6572 653a 0a0a 2a20 603c  ]`..where:..* `<
-00001f20: 7365 7276 6572 3a70 6f72 743e 6020 6973  server:port>` is
-00001f30: 2074 6865 2073 6572 7665 7220 616e 6420   the server and 
-00001f40: 706f 7274 206e 756d 6265 7220 2865 2e67  port number (e.g
-00001f50: 2e2c 2060 3132 372e 302e 302e 313a 3830  ., `127.0.0.1:80
-00001f60: 3030 6029 206f 6620 6120 7275 6e6e 696e  00`) of a runnin
-00001f70: 6720 7363 6f72 6562 6f61 7264 2e20 6a61  g scoreboard. ja
-00001f80: 6d73 7461 7473 2077 696c 6c20 636f 6e6e  mstats will conn
-00001f90: 6563 7420 746f 2074 6865 2073 636f 7265  ect to the score
-00001fa0: 626f 6172 6420 616e 6420 646f 776e 6c6f  board and downlo
-00001fb0: 6164 2074 6865 2063 7572 7265 6e74 2067  ad the current g
-00001fc0: 616d 6520 7374 6174 652e 0a2a 2060 3c73  ame state..* `<s
-00001fd0: 6f6d 6520 6172 6775 6d65 6e74 7320 746f  ome arguments to
-00001fe0: 2064 6566 696e 6520 7468 6520 6f75 7470   define the outp
-00001ff0: 7574 3e60 3a20 7361 6d65 2061 7320 6162  ut>`: same as ab
-00002000: 6f76 652e 2059 6f75 2063 616e 2072 6f75  ove. You can rou
-00002010: 7465 2074 6865 206f 7574 7075 7420 746f  te the output to
-00002020: 2061 2050 4446 2066 696c 6520 6279 2073   a PDF file by s
-00002030: 7065 6369 6679 696e 6720 602d 2d6d 6f64  pecifying `--mod
-00002040: 653d 7064 6660 2e0a 0a0a 5c2a 202a 4920  e=pdf`....\* *I 
-00002050: 616d 206e 6f74 2061 2077 6562 2073 6563  am not a web sec
-00002060: 7572 6974 7920 6578 7065 7274 2c20 616e  urity expert, an
-00002070: 6420 4920 6d61 6b65 206e 6f20 6775 6172  d I make no guar
-00002080: 616e 7465 6573 2077 6861 7473 6f65 7665  antees whatsoeve
-00002090: 7220 6162 6f75 7420 7765 6273 6572 7665  r about webserve
-000020a0: 7220 7365 6375 7269 7479 2e20 4966 2079  r security. If y
-000020b0: 6f75 2772 6520 636f 6e63 6572 6e65 6420  ou're concerned 
-000020c0: 616e 6420 7761 6e74 2074 6f20 6865 6c70  and want to help
-000020d0: 206d 616b 6520 6974 206d 6f72 6520 7365   make it more se
-000020e0: 6375 7265 2c20 706c 6561 7365 206f 7065  cure, please ope
-000020f0: 6e20 616e 2069 7373 7565 212a 0a         n an issue!*.
+00000190: 292e 200a 0a53 6f2c 2077 6879 2064 6f77  ). ..So, why dow
+000001a0: 6e6c 6f61 6420 4a61 6d73 7461 7473 2061  nload Jamstats a
+000001b0: 6e64 2072 756e 2069 7420 6f6e 2079 6f75  nd run it on you
+000001c0: 7220 6c61 7074 6f70 3f20 546f 2063 6f6e  r laptop? To con
+000001d0: 6e65 6374 2074 6f20 6120 6c69 7665 2067  nect to a live g
+000001e0: 616d 6520 6f6e 2061 2072 756e 6e69 6e67  ame on a running
+000001f0: 2073 636f 7265 626f 6172 6421 200a 0a2a   scoreboard! ..*
+00000200: 2a4a 616d 7374 6174 7320 6973 2067 7265  *Jamstats is gre
+00000210: 6174 2066 6f72 2061 6e6e 6f75 6e63 6572  at for announcer
+00000220: 7321 2a2a 2053 6565 202a 2a77 686f 2773  s!** See **who's
+00000230: 206f 6e20 7468 6520 7472 6163 6b2a 2a20   on the track** 
+00000240: 2869 6e63 6c75 6469 6e67 2070 6f73 6974  (including posit
+00000250: 696f 6e73 2061 6e64 2070 656e 616c 7469  ions and penalti
+00000260: 6573 292c 2076 6974 616c 2067 616d 6520  es), vital game 
+00000270: 7374 6174 7320 616e 6420 2a2a 726f 7374  stats and **rost
+00000280: 6572 732a 2a20 666f 7220 626f 7468 2074  ers** for both t
+00000290: 6561 6d73 2061 6e64 206f 6666 6963 6961  eams and officia
+000002a0: 6c73 2e20 596f 7520 6361 6e20 6576 656e  ls. You can even
+000002b0: 2063 6f6e 6e65 6374 2074 6f20 6120 6c69   connect to a li
+000002c0: 7665 2073 636f 7265 626f 6172 6420 5b66  ve scoreboard [f
+000002d0: 726f 6d20 616e 7977 6865 7265 206f 6e20  rom anywhere on 
+000002e0: 7468 6520 496e 7465 726e 6574 5d28 6874  the Internet](ht
+000002f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000300: 2f64 686d 6179 2f6a 616d 7374 6174 7323  /dhmay/jamstats#
+00000310: 636f 6e6e 6563 7469 6e67 2d74 6f2d 612d  connecting-to-a-
+00000320: 7072 6f78 6965 642d 7363 6f72 6562 6f61  proxied-scoreboa
+00000330: 7264 2d66 726f 6d2d 7468 652d 696e 7465  rd-from-the-inte
+00000340: 726e 6574 2920 7573 696e 6720 7773 7072  rnet) using wspr
+00000350: 6f78 7921 0a0a 2323 2323 2046 6561 7475  oxy!..#### Featu
+00000360: 7265 730a 0a2a 2047 6574 2075 702d 746f  res..* Get up-to
+00000370: 2d64 6174 6520 6761 6d65 2064 6174 6120  -date game data 
+00000380: 6672 6f6d 2061 206c 6976 6520 7363 6f72  from a live scor
+00000390: 6562 6f61 7264 0a2a 2056 6973 7561 6c69  eboard.* Visuali
+000003a0: 7a65 2070 6f69 6e74 7320 7065 7220 6a61  ze points per ja
+000003b0: 6d2c 206c 6561 642c 206d 6561 6e20 6e65  m, lead, mean ne
+000003c0: 7420 706f 696e 7473 2c20 6361 6c6c 6f66  t points, callof
+000003d0: 6673 2c20 7469 6d65 2074 6f20 696e 6974  fs, time to init
+000003e0: 6961 6c20 7061 7373 2c20 7065 6e61 6c74  ial pass, penalt
+000003f0: 6965 7320 616e 6420 6d75 6368 206d 6f72  ies and much mor
+00000400: 650a 2a20 5265 6164 2069 6e20 4a53 4f4e  e.* Read in JSON
+00000410: 2066 696c 6573 2066 726f 6d20 636f 6d70   files from comp
+00000420: 6c65 7465 6420 6761 6d65 7320 6f72 2063  leted games or c
+00000430: 6f6e 6e65 6374 2074 6f20 6120 7275 6e6e  onnect to a runn
+00000440: 696e 6720 7363 6f72 6562 6f61 7264 0a2a  ing scoreboard.*
+00000450: 2053 6176 6520 706c 6f74 7320 6173 2050   Save plots as P
+00000460: 4446 2066 696c 6573 2c20 6f72 2073 7461  DF files, or sta
+00000470: 7274 2061 2077 6562 7365 7276 6572 2074  rt a webserver t
+00000480: 6861 7420 616e 796f 6e65 206f 6e20 796f  hat anyone on yo
+00000490: 7572 206e 6574 776f 726b 2063 616e 2062  ur network can b
+000004a0: 726f 7773 6520 746f 0a0a 446f 2079 6f75  rowse to..Do you
+000004b0: 2061 6c72 6561 6479 206c 6f76 6520 4a61   already love Ja
+000004c0: 6d73 7461 7473 3f20 5b54 656c 6c20 7573  mstats? [Tell us
+000004d0: 2061 626f 7574 2069 7421 5d28 6874 7470   about it!](http
+000004e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000004f0: 686d 6179 2f6a 616d 7374 6174 732f 6973  hmay/jamstats/is
+00000500: 7375 6573 2f6e 6577 3f61 7373 6967 6e65  sues/new?assigne
+00000510: 6573 3d26 6c61 6265 6c73 3d74 6573 7469  es=&labels=testi
+00000520: 6d6f 6e69 616c 2674 656d 706c 6174 653d  monial&template=
+00000530: 7465 7374 696d 6f6e 6961 6c2e 6d64 2674  testimonial.md&t
+00000540: 6974 6c65 3d29 0a0a 4a61 6d73 7461 7473  itle=)..Jamstats
+00000550: 2077 6173 2064 6576 656c 6f70 6564 2062   was developed b
+00000560: 7920 5b54 6865 444d 5d28 6874 7470 733a  y [TheDM](https:
+00000570: 2f2f 6769 7468 7562 2e63 6f6d 2f64 686d  //github.com/dhm
+00000580: 6179 292c 2077 6974 6820 5b53 6561 7474  ay), with [Seatt
+00000590: 6c65 2044 6572 6279 2042 7261 7473 5d28  le Derby Brats](
+000005a0: 6874 7470 733a 2f2f 7777 772e 7365 6174  https://www.seat
+000005b0: 746c 6564 6572 6279 6272 6174 732e 636f  tlederbybrats.co
+000005c0: 6d2f 646f 6e61 7469 6f6e 732f 292e 204c  m/donations/). L
+000005d0: 696b 6520 4a61 6d73 7461 7473 3f20 436f  ike Jamstats? Co
+000005e0: 6e73 6964 6572 2061 2064 6f6e 6174 696f  nsider a donatio
+000005f0: 6e20 746f 2053 4442 2c20 6120 3530 3128  n to SDB, a 501(
+00000600: 6329 2833 2920 6f72 6761 6e69 7a61 7469  c)(3) organizati
+00000610: 6f6e 210a 3c70 2061 6c69 676e 3d22 6c65  on!.<p align="le
+00000620: 6674 223e 3c61 2068 7265 663d 2268 7474  ft"><a href="htt
+00000630: 7073 3a2f 2f77 7777 2e73 6561 7474 6c65  ps://www.seattle
+00000640: 6465 7262 7962 7261 7473 2e63 6f6d 2f64  derbybrats.com/d
+00000650: 6f6e 6174 696f 6e73 2f22 3e3c 696d 6720  onations/"><img 
+00000660: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000670: 6875 622e 636f 6d2f 6468 6d61 792f 6a61  hub.com/dhmay/ja
+00000680: 6d73 7461 7473 2f62 6c6f 622f 6d61 696e  mstats/blob/main
+00000690: 2f72 6573 6f75 7263 6573 2f73 6462 5f6c  /resources/sdb_l
+000006a0: 6f67 6f5f 7768 6974 6562 6b67 726e 642e  ogo_whitebkgrnd.
+000006b0: 706e 6722 2077 6964 7468 3d22 3135 3022  png" width="150"
+000006c0: 3e3c 2f61 3e3c 2f70 3e0a 0a0a 0a23 2323  ></a></p>....###
+000006d0: 2320 496e 7374 7275 6374 696f 6e73 0a0a  # Instructions..
+000006e0: 5175 6963 6b73 7461 7274 3a20 646f 776e  Quickstart: down
+000006f0: 6c6f 6164 205b 7468 6520 6c61 7465 7374  load [the latest
+00000700: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+00000710: 2f2f 6769 7468 7562 2e63 6f6d 2f64 686d  //github.com/dhm
+00000720: 6179 2f6a 616d 7374 6174 732f 7265 6c65  ay/jamstats/rele
+00000730: 6173 6573 2920 616e 6420 7275 6e20 6974  ases) and run it
+00000740: 2e0a 0a49 6e20 6d6f 7265 2064 6574 6169  ...In more detai
+00000750: 6c3a 0a0a 2a20 2a2a 5b49 6e73 7461 6c6c  l:..* **[Install
+00000760: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
+00000770: 7469 6f6e 292a 2a0a 2a20 2a2a 5b55 7361  tion)**.* **[Usa
+00000780: 6765 5d28 2375 7361 6765 292a 2a0a 0a23  ge](#usage)**..#
+00000790: 2320 5361 6d70 6c65 2070 6c6f 7473 0a0a  # Sample plots..
+000007a0: 3c70 2061 6c69 676e 3d22 6c65 6674 223e  <p align="left">
+000007b0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000007c0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 686d  //github.com/dhm
+000007d0: 6179 2f6a 616d 7374 6174 732f 626c 6f62  ay/jamstats/blob
+000007e0: 2f6d 6169 6e2f 7265 736f 7572 6365 732f  /main/resources/
+000007f0: 6375 7272 656e 745f 736b 6174 6572 732e  current_skaters.
+00000800: 706e 6722 2077 6964 7468 3d22 3530 3022  png" width="500"
+00000810: 3e3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  ></p>..<p align=
+00000820: 226c 6566 7422 3e3c 696d 6720 7372 633d  "left"><img src=
+00000830: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000840: 636f 6d2f 6468 6d61 792f 6a61 6d73 7461  com/dhmay/jamsta
+00000850: 7473 2f62 6c6f 622f 6d61 696e 2f72 6573  ts/blob/main/res
+00000860: 6f75 7263 6573 2f63 756d 756c 6174 6976  ources/cumulativ
+00000870: 655f 7363 6f72 655f 6279 5f6a 616d 2e70  e_score_by_jam.p
+00000880: 6e67 2220 7769 6474 683d 2235 3030 223e  ng" width="500">
+00000890: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d22  </p>..<p align="
+000008a0: 6c65 6674 223e 3c69 6d67 2073 7263 3d22  left"><img src="
+000008b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000008c0: 6f6d 2f64 686d 6179 2f6a 616d 7374 6174  om/dhmay/jamstat
+000008d0: 732f 626c 6f62 2f6d 6169 6e2f 7265 736f  s/blob/main/reso
+000008e0: 7572 6365 732f 6a61 6d6d 6572 5f73 7461  urces/jammer_sta
+000008f0: 7473 2e70 6e67 2220 7769 6474 683d 2235  ts.png" width="5
+00000900: 3030 223e 3c2f 703e 0a0a 5768 6174 2070  00"></p>..What p
+00000910: 656e 616c 7469 6573 2067 6f74 2079 6f75  enalties got you
+00000920: 2064 6f77 6e20 7468 6520 6d6f 7374 3f0a   down the most?.
+00000930: 0a3c 7020 616c 6967 6e3d 226c 6566 7422  .<p align="left"
+00000940: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000950: 3a2f 2f67 6974 6875 622e 636f 6d2f 6468  ://github.com/dh
+00000960: 6d61 792f 6a61 6d73 7461 7473 2f62 6c6f  may/jamstats/blo
+00000970: 622f 6d61 696e 2f72 6573 6f75 7263 6573  b/main/resources
+00000980: 2f74 6561 6d5f 7065 6e61 6c74 795f 636f  /team_penalty_co
+00000990: 756e 7473 2e70 6e67 2220 7769 6474 683d  unts.png" width=
+000009a0: 2235 3030 223e 3c2f 703e 0a0a 3c70 2061  "500"></p>..<p a
+000009b0: 6c69 676e 3d22 6c65 6674 223e 3c69 6d67  lign="left"><img
+000009c0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+000009d0: 7468 7562 2e63 6f6d 2f64 686d 6179 2f6a  thub.com/dhmay/j
+000009e0: 616d 7374 6174 732f 626c 6f62 2f6d 6169  amstats/blob/mai
+000009f0: 6e2f 7265 736f 7572 6365 732f 736b 6174  n/resources/skat
+00000a00: 6572 5f73 7461 7473 2e70 6e67 2220 7769  er_stats.png" wi
+00000a10: 6474 683d 2235 3030 223e 3c2f 703e 0a0a  dth="500"></p>..
+00000a20: 3c70 2061 6c69 676e 3d22 6c65 6674 223e  <p align="left">
+00000a30: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000a40: 2f2f 6769 7468 7562 2e63 6f6d 2f64 686d  //github.com/dhm
+00000a50: 6179 2f6a 616d 7374 6174 732f 626c 6f62  ay/jamstats/blob
+00000a60: 2f6d 6169 6e2f 7265 736f 7572 6365 732f  /main/resources/
+00000a70: 6a61 6d5f 706f 696e 7473 5f62 6172 706c  jam_points_barpl
+00000a80: 6f74 2e70 6e67 2220 7769 6474 683d 2235  ot.png" width="5
+00000a90: 3030 223e 3c2f 703e 0a0a 5573 6520 7468  00"></p>..Use th
+00000aa0: 6520 636f 6c6f 7273 2064 6566 696e 6564  e colors defined
+00000ab0: 2066 6f72 2065 6163 6820 7465 616d 2069   for each team i
+00000ac0: 6e20 7468 6520 7363 6f72 6562 6f61 7264  n the scoreboard
+00000ad0: 2066 696c 652c 206f 7220 7072 6f76 6964   file, or provid
+00000ae0: 6520 796f 7572 206f 776e 206f 6e20 7468  e your own on th
+00000af0: 6520 636f 6d6d 616e 6420 6c69 6e65 2e0a  e command line..
+00000b00: 0a3c 7020 616c 6967 6e3d 226c 6566 7422  .<p align="left"
+00000b10: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000b20: 3a2f 2f67 6974 6875 622e 636f 6d2f 6468  ://github.com/dh
+00000b30: 6d61 792f 6a61 6d73 7461 7473 2f62 6c6f  may/jamstats/blo
+00000b40: 622f 6d61 696e 2f72 6573 6f75 7263 6573  b/main/resources
+00000b50: 2f6c 6561 645f 7375 6d6d 6172 792e 706e  /lead_summary.pn
+00000b60: 6722 2077 6964 7468 3d22 3530 3022 3e3c  g" width="500"><
+00000b70: 2f70 3e0a 0a57 616e 7420 746f 2064 6f20  /p>..Want to do 
+00000b80: 796f 7572 206f 776e 2061 6e61 6c79 7469  your own analyti
+00000b90: 6373 3f20 5361 7665 2064 6f77 6e20 6120  cs? Save down a 
+00000ba0: 7370 7265 6164 7368 6565 7420 616e 6420  spreadsheet and 
+00000bb0: 646f 2079 6f75 7220 6f77 6e20 7468 696e  do your own thin
+00000bc0: 6720 7769 7468 2069 7421 0a0a 3c70 2061  g with it!..<p a
+00000bd0: 6c69 676e 3d22 6c65 6674 223e 3c69 6d67  lign="left"><img
+00000be0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000bf0: 7468 7562 2e63 6f6d 2f64 686d 6179 2f6a  thub.com/dhmay/j
+00000c00: 616d 7374 6174 732f 626c 6f62 2f6d 6169  amstats/blob/mai
+00000c10: 6e2f 7265 736f 7572 6365 732f 7473 765f  n/resources/tsv_
+00000c20: 6f75 7470 7574 5f73 6372 6565 6e73 686f  output_screensho
+00000c30: 742e 706e 6722 2077 6964 7468 3d22 3530  t.png" width="50
+00000c40: 3022 3e3c 2f70 3e0a 0a0a 2323 2049 6e73  0"></p>...## Ins
+00000c50: 7461 6c6c 6174 696f 6e0a 0a2a 2057 696e  tallation..* Win
+00000c60: 646f 7773 3a20 676f 2074 6f20 7468 6520  dows: go to the 
+00000c70: 5b6c 6174 6573 7420 7265 6c65 6173 655d  [latest release]
+00000c80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000c90: 636f 6d2f 6468 6d61 792f 6a61 6d73 7461  com/dhmay/jamsta
+00000ca0: 7473 2f72 656c 6561 7365 7329 2061 6e64  ts/releases) and
+00000cb0: 2064 6f77 6e6c 6f61 6420 606a 616d 7374   download `jamst
+00000cc0: 6174 732d 3c76 6572 7369 6f6e 3e2e 6578  ats-<version>.ex
+00000cd0: 6560 0a2a 204d 6163 3a20 676f 2074 6f20  e`.* Mac: go to 
+00000ce0: 7468 6520 5b6c 6174 6573 7420 7265 6c65  the [latest rele
+00000cf0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+00000d00: 6875 622e 636f 6d2f 6468 6d61 792f 6a61  hub.com/dhmay/ja
+00000d10: 6d73 7461 7473 2f72 656c 6561 7365 7329  mstats/releases)
+00000d20: 2061 6e64 2064 6f77 6e6c 6f61 6420 606a   and download `j
+00000d30: 616d 7374 6174 732d 6d61 632d 3c76 6572  amstats-mac-<ver
+00000d40: 7369 6f6e 3e2e 7a69 7060 2c20 7468 656e  sion>.zip`, then
+00000d50: 2075 6e7a 6970 2074 6861 7420 6669 6c65   unzip that file
+00000d60: 2069 6e74 6f20 796f 7572 2041 7070 6c69   into your Appli
+00000d70: 6361 7469 6f6e 7320 6469 7265 6374 6f72  cations director
+00000d80: 7920 286f 7220 7768 6572 6576 6572 2079  y (or wherever y
+00000d90: 6f75 2077 616e 7420 746f 2072 756e 204a  ou want to run J
+00000da0: 616d 7374 6174 7320 6672 6f6d 290a 2020  amstats from).  
+00000db0: 2020 2a20 4e6f 7465 2074 6861 7420 7468    * Note that th
+00000dc0: 6520 4d61 6320 6170 7020 6973 2070 6172  e Mac app is par
+00000dd0: 7469 6375 6c61 726c 7920 736c 6f77 2074  ticularly slow t
+00000de0: 6f20 7374 6172 7420 7570 0a2a 2041 6e79  o start up.* Any
+00000df0: 2070 6c61 7466 6f72 6d3a 2069 6e73 7461   platform: insta
+00000e00: 6c6c 2050 7974 686f 6e20 332e 3920 6f72  ll Python 3.9 or
+00000e10: 2068 6967 6865 722c 2074 6865 6e20 7275   higher, then ru
+00000e20: 6e20 6070 6970 2069 6e73 7461 6c6c 206a  n `pip install j
+00000e30: 616d 7374 6174 7360 2e20 5468 6174 2077  amstats`. That w
+00000e40: 696c 6c20 7075 7420 606a 616d 7374 6174  ill put `jamstat
+00000e50: 7360 206f 6e20 796f 7572 2070 6174 6820  s` on your path 
+00000e60: 736f 2079 6f75 2063 616e 2072 756e 2069  so you can run i
+00000e70: 7420 6672 6f6d 2074 6865 2063 6f6d 6d61  t from the comma
+00000e80: 6e64 206c 696e 652e 0a0a 2323 2055 7361  nd line...## Usa
+00000e90: 6765 0a0a 5b46 756c 6c20 7573 6572 206d  ge..[Full user m
+00000ea0: 616e 7561 6c20 2850 4446 295d 2868 7474  anual (PDF)](htt
+00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ec0: 6468 6d61 792f 6a61 6d73 7461 7473 2f62  dhmay/jamstats/b
+00000ed0: 6c6f 622f 6d61 696e 2f72 6573 6f75 7263  lob/main/resourc
+00000ee0: 6573 2f6a 616d 7374 6174 735f 7573 6572  es/jamstats_user
+00000ef0: 5f6d 616e 7561 6c2e 7064 6629 2c20 696e  _manual.pdf), in
+00000f00: 636c 7564 696e 6720 686f 7720 746f 2073  cluding how to s
+00000f10: 7461 7274 204a 616d 7374 6174 7320 7570  tart Jamstats up
+00000f20: 2061 6e64 2068 6f77 2074 6f20 696e 7465   and how to inte
+00000f30: 7270 7265 7420 616c 6c20 7468 6520 706c  rpret all the pl
+00000f40: 6f74 732e 0a0a 2323 2320 4472 6167 2d61  ots...### Drag-a
+00000f50: 6e64 2d64 726f 700a 0a4f 6e20 5769 6e64  nd-drop..On Wind
+00000f60: 6f77 7320 6f72 204d 6163 2c20 746f 2067  ows or Mac, to g
+00000f70: 656e 6572 6174 6520 6120 706c 6f74 7320  enerate a plots 
+00000f80: 5044 462c 2079 6f75 2063 616e 2073 696d  PDF, you can sim
+00000f90: 706c 7920 2a2a 6472 6167 2061 6e64 2064  ply **drag and d
+00000fa0: 726f 702a 2a20 796f 7572 2067 616d 6520  rop** your game 
+00000fb0: 4a53 4f4e 2066 696c 6520 6f6e 746f 2074  JSON file onto t
+00000fc0: 6865 206a 616d 7374 6174 732e 6578 6520  he jamstats.exe 
+00000fd0: 6669 6c65 206f 7220 4a61 6d73 7461 7473  file or Jamstats
+00000fe0: 2061 7070 2e20 5468 6174 2077 696c 6c20   app. That will 
+00000ff0: 6765 6e65 7261 7465 2061 2060 2e70 6466  generate a `.pdf
+00001000: 6020 6669 6c65 2069 6e20 7468 6520 7361  ` file in the sa
+00001010: 6d65 2064 6972 6563 746f 7279 2061 7320  me directory as 
+00001020: 796f 7572 2060 2e6a 736f 6e60 2066 696c  your `.json` fil
+00001030: 652c 2077 6974 6820 7468 6520 7361 6d65  e, with the same
+00001040: 206e 616d 6520 6275 7420 7769 7468 2074   name but with t
+00001050: 6865 2060 2e6a 736f 6e60 2065 7874 656e  he `.json` exten
+00001060: 7369 6f6e 2072 6570 6c61 6365 6420 7769  sion replaced wi
+00001070: 7468 2060 2e70 6466 602e 0a0a 2323 2320  th `.pdf`...### 
+00001080: 4755 490a 0a44 6f75 626c 652d 636c 6963  GUI..Double-clic
+00001090: 6b20 6f6e 2074 6865 206a 616d 7374 6174  k on the jamstat
+000010a0: 7320 6578 6563 7574 6162 6c65 2074 6f20  s executable to 
+000010b0: 6f70 656e 2061 2067 7261 7068 6963 616c  open a graphical
+000010c0: 2077 696e 646f 7720 746f 2073 7065 6369   window to speci
+000010d0: 6679 2079 6f75 7220 7061 7261 6d65 7465  fy your paramete
+000010e0: 7273 2e20 0a0a 546f 2063 6f6e 6e65 6374  rs. ..To connect
+000010f0: 2074 6f20 6120 7363 6f72 6562 6f61 7264   to a scoreboard
+00001100: 2c20 616c 6c20 796f 7520 6e65 6564 2074  , all you need t
+00001110: 6f20 7370 6563 6966 7920 6973 2060 7363  o specify is `sc
+00001120: 6f72 6562 6f61 7264 7365 7276 6572 6020  oreboardserver` 
+00001130: 2d2d 2067 6976 6520 7468 6174 2074 6865  -- give that the
+00001140: 2063 6f6d 6269 6e65 6420 4950 2061 6464   combined IP add
+00001150: 7265 7373 2061 6e64 2070 6f72 7420 6e75  ress and port nu
+00001160: 6d62 6572 206f 6620 796f 7572 2073 636f  mber of your sco
+00001170: 7265 626f 6172 6420 7365 7276 6572 2028  reboard server (
+00001180: 652e 672e 2c20 6031 3732 2e32 312e 3132  e.g., `172.21.12
+00001190: 2e37 3a38 3030 3060 292c 2061 7320 7265  .7:8000`), as re
+000011a0: 706f 7274 6564 2069 6e20 7468 6520 7363  ported in the sc
+000011b0: 6f72 6562 6f61 7264 2047 5549 2e0a 0a57  oreboard GUI...W
+000011c0: 6974 6820 7468 6174 2075 7361 6765 2c20  ith that usage, 
+000011d0: 4a61 6d73 7461 7473 2077 696c 6c20 7374  Jamstats will st
+000011e0: 6172 7420 6974 7320 6f77 6e20 7365 7276  art its own serv
+000011f0: 6572 206f 6e20 796f 7572 206c 6170 746f  er on your lapto
+00001200: 702c 2061 6e64 2074 6865 206f 7574 7075  p, and the outpu
+00001210: 7420 696e 2074 6865 2047 5549 2077 696e  t in the GUI win
+00001220: 646f 7720 7769 6c6c 2074 656c 6c20 796f  dow will tell yo
+00001230: 7520 7768 6572 6520 746f 2070 6f69 6e74  u where to point
+00001240: 2079 6f75 7220 6272 6f77 7365 722e 2042   your browser. B
+00001250: 7920 6465 6661 756c 742c 2074 6861 7427  y default, that'
+00001260: 7320 6068 7474 703a 2f2f 6c6f 6361 6c68  s `http://localh
+00001270: 6f73 743a 3830 3830 602c 2077 6869 6368  ost:8080`, which
+00001280: 2077 696c 6c20 6d61 6b65 204a 616d 7374   will make Jamst
+00001290: 6174 7320 6176 6169 6c61 626c 6520 6f6e  ats available on
+000012a0: 6c79 206f 6e20 796f 7572 206f 776e 206d  ly on your own m
+000012b0: 6163 6869 6e65 2e20 4966 2079 6f75 2077  achine. If you w
+000012c0: 616e 7420 746f 206d 616b 6520 4a61 6d73  ant to make Jams
+000012d0: 7461 7473 2061 7661 696c 6162 6c65 2074  tats available t
+000012e0: 6f20 6f74 6865 7220 6272 6f77 7365 7273  o other browsers
+000012f0: 206f 6e20 796f 7572 206e 6574 776f 726b   on your network
+00001300: 2c20 7365 7420 606a 616d 7374 6174 7369  , set `jamstatsi
+00001310: 7060 2074 6f20 796f 7572 2063 6f6d 7075  p` to your compu
+00001320: 7465 7227 7320 4950 2061 6464 7265 7373  ter's IP address
+00001330: 2e0a 0a59 6f75 2063 616e 2061 6c73 6f20  ...You can also 
+00001340: 7573 6520 7468 6520 4755 4920 746f 2073  use the GUI to s
+00001350: 7065 6369 6679 2061 6c6c 206f 7468 6572  pecify all other
+00001360: 2061 7267 756d 656e 7473 2079 6f75 2063   arguments you c
+00001370: 6f75 6c64 2073 7065 6369 6679 2066 726f  ould specify fro
+00001380: 6d20 7468 6520 636f 6d6d 616e 646c 696e  m the commandlin
+00001390: 652e 0a0a 2323 2320 436f 6e6e 6563 7469  e...### Connecti
+000013a0: 6e67 2074 6f20 6120 7072 6f78 6965 6420  ng to a proxied 
+000013b0: 7363 6f72 6562 6f61 7264 2066 726f 6d20  scoreboard from 
+000013c0: 7468 6520 496e 7465 726e 6574 0a0a 4974  the Internet..It
+000013d0: 2773 2070 6f73 7369 626c 6520 746f 2075  's possible to u
+000013e0: 7365 204a 616d 7374 6174 7320 6672 6f6d  se Jamstats from
+000013f0: 2061 6e79 7768 6572 6520 696e 2074 6865   anywhere in the
+00001400: 2077 6f72 6c64 2074 6f20 636f 6e6e 6563   world to connec
+00001410: 7420 746f 2061 2072 756e 6e69 6e67 2073  t to a running s
+00001420: 636f 7265 626f 6172 6421 2054 6869 7320  coreboard! This 
+00001430: 6c65 7473 202a 2a72 656d 6f74 6520 616e  lets **remote an
+00001440: 6e6f 756e 6365 7273 2a2a 2075 7365 204a  nouncers** use J
+00001450: 616d 7374 6174 7320 746f 2068 656c 7020  amstats to help 
+00001460: 7769 7468 2063 616c 6c69 6e67 2067 616d  with calling gam
+00001470: 6573 2e20 4865 7265 2773 2068 6f77 3a0a  es. Here's how:.
+00001480: 0a23 2323 2320 4174 2074 6865 2074 7261  .#### At the tra
+00001490: 636b 3a20 7365 7474 696e 6720 7570 2061  ck: setting up a
+000014a0: 2070 726f 7879 0a0a 312e 2044 6f77 6e6c   proxy..1. Downl
+000014b0: 6f61 6420 5b77 7370 726f 7879 5d28 6874  oad [wsproxy](ht
+000014c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000014d0: 2f44 6572 6279 5374 6174 732f 7773 7072  /DerbyStats/wspr
+000014e0: 6f78 7929 2061 6e64 2066 6f6c 6c6f 7720  oxy) and follow 
+000014f0: 6974 7320 696e 7374 7275 6374 696f 6e73  its instructions
+00001500: 2074 6f20 7365 7420 7570 2061 2070 726f   to set up a pro
+00001510: 7879 2e20 5468 6973 2077 696c 6c20 6665  xy. This will fe
+00001520: 6564 2079 6f75 7220 7363 6f72 6562 6f61  ed your scoreboa
+00001530: 7264 2064 6174 612c 2072 6561 642d 6f6e  rd data, read-on
+00001540: 6c79 2c20 746f 2074 6865 2049 6e74 6572  ly, to the Inter
+00001550: 6e65 740a 2020 2020 2a20 4966 2079 6f75  net.    * If you
+00001560: 2772 6520 7573 696e 6720 7468 6520 6465  're using the de
+00001570: 6661 756c 7420 7363 6f72 6562 6f61 7264  fault scoreboard
+00001580: 2073 6574 7469 6e67 732c 2074 6865 2064   settings, the d
+00001590: 6566 6175 6c74 2077 7370 726f 7879 2073  efault wsproxy s
+000015a0: 6574 7469 6e67 7320 7769 6c6c 2077 6f72  ettings will wor
+000015b0: 6b20 6669 6e65 2e20 0a20 2020 202a 2049  k fine. .    * I
+000015c0: 6620 6e6f 742c 2070 6179 2061 7474 656e  f not, pay atten
+000015d0: 7469 6f6e 2074 6f20 7468 6520 706f 7274  tion to the port
+000015e0: 2079 6f75 2772 6520 7275 6e6e 696e 6720   you're running 
+000015f0: 796f 7572 2073 636f 7265 626f 6172 6420  your scoreboard 
+00001600: 6f6e 2c20 616e 6420 6368 616e 6765 2066  on, and change f
+00001610: 726f 6d20 3830 3030 2074 6f20 7468 6174  rom 8000 to that
+00001620: 2073 616d 6520 706f 7274 2069 6e20 7773   same port in ws
+00001630: 7072 6f78 7927 7320 636f 6e66 6967 2e69  proxy's config.i
+00001640: 6e69 2066 696c 650a 322e 2059 6f75 7220  ni file.2. Your 
+00001650: 7072 6f78 7920 6361 6e20 7365 6e64 2079  proxy can send y
+00001660: 6f75 7220 7363 6f72 6562 6f61 7264 2064  our scoreboard d
+00001670: 6174 6120 7768 6572 6576 6572 2079 6f75  ata wherever you
+00001680: 2074 656c 6c20 6974 2074 6f2e 204f 6e20   tell it to. On 
+00001690: 7468 6520 6f74 6865 7220 656e 642c 2074  the other end, t
+000016a0: 6865 7265 206e 6565 6473 2074 6f20 6265  here needs to be
+000016b0: 2061 6e6f 7468 6572 2063 6f70 7920 6f66   another copy of
+000016c0: 2077 7370 726f 7879 2072 756e 6e69 6e67   wsproxy running
+000016d0: 2e0a 2020 2020 2a20 5769 7468 2074 6865  ..    * With the
+000016e0: 2064 6566 6175 6c74 2063 6f6e 6669 6775   default configu
+000016f0: 7261 7469 6f6e 2c20 796f 7572 2070 726f  ration, your pro
+00001700: 7879 2064 6174 6120 7769 6c6c 2062 6520  xy data will be 
+00001710: 7365 6e74 2074 6f20 6120 6e65 7720 7375  sent to a new su
+00001720: 6264 6f6d 6169 6e20 6f66 2060 6465 7262  bdomain of `derb
+00001730: 7973 7461 7473 2e65 7560 0a20 2020 2020  ystats.eu`.     
+00001740: 2020 202a 2065 2e67 2e2c 2060 6874 7470     * e.g., `http
+00001750: 733a 2f2f 6a61 6d6d 6572 2d6c 616e 652e  s://jammer-lane.
+00001760: 6465 7262 7973 7461 7473 2e65 752f 602c  derbystats.eu/`,
+00001770: 2062 7574 2069 7420 7769 6c6c 202a 6e6f   but it will *no
+00001780: 7420 6265 2074 6861 742a 2c20 6974 2077  t be that*, it w
+00001790: 696c 6c20 6265 2073 6f6d 6574 6869 6e67  ill be something
+000017a0: 2065 6c73 6520 756e 6971 7565 2074 6f20   else unique to 
+000017b0: 796f 7572 2073 636f 7265 626f 6172 640a  your scoreboard.
+000017c0: 2020 2020 2a20 5768 656e 2079 6f75 2073      * When you s
+000017d0: 7461 7274 2077 7370 726f 7879 2c20 6974  tart wsproxy, it
+000017e0: 2077 696c 6c20 7465 6c6c 2079 6f75 2077   will tell you w
+000017f0: 6865 7265 2074 6865 2064 6174 6120 6973  here the data is
+00001800: 2067 6f69 6e67 2e20 0a20 2020 2020 2020   going. .       
+00001810: 202a 2046 6f72 2065 7861 6d70 6c65 2c20   * For example, 
+00001820: 6044 6973 706c 6179 2055 524c 3a20 6874  `Display URL: ht
+00001830: 7470 733a 2f2f 6a61 6d6d 6572 2d6c 616e  tps://jammer-lan
+00001840: 652e 6465 7262 7973 7461 7473 2e65 7560  e.derbystats.eu`
+00001850: 0a20 2020 2020 2020 202a 2047 6976 6520  .        * Give 
+00001860: 7468 6973 2074 6f20 7468 6520 7065 7273  this to the pers
+00001870: 6f6e 2077 686f 276c 6c20 6265 2072 756e  on who'll be run
+00001880: 6e69 6e67 204a 616d 7374 6174 7320 7265  ning Jamstats re
+00001890: 6d6f 7465 6c79 2e0a 2020 2020 2020 2020  motely..        
+000018a0: 0a23 2323 2320 5265 6d6f 7465 6c79 3a20  .#### Remotely: 
+000018b0: 7275 6e6e 696e 6720 4a61 6d73 7461 7473  running Jamstats
+000018c0: 2074 6f20 636f 6e6e 6563 7420 746f 2061   to connect to a
+000018d0: 2070 726f 7879 0a0a 312e 2047 6574 2074   proxy..1. Get t
+000018e0: 6865 2022 4469 7370 6c61 7920 5552 4c22  he "Display URL"
+000018f0: 2066 726f 6d20 7468 6520 7065 7273 6f6e   from the person
+00001900: 2077 686f 2073 6574 2075 7020 7773 7072   who set up wspr
+00001910: 6f78 790a 2020 2020 2a20 466f 7220 6578  oxy.    * For ex
+00001920: 616d 706c 652c 2060 6874 7470 733a 2f2f  ample, `https://
+00001930: 6a61 6d6d 6572 2d6c 616e 652e 6465 7262  jammer-lane.derb
+00001940: 7973 7461 7473 2e65 7560 0a32 2e20 5374  ystats.eu`.2. St
+00001950: 6172 7420 7570 204a 616d 7374 6174 7320  art up Jamstats 
+00001960: 616e 6420 6769 7665 2069 7420 7477 6f20  and give it two 
+00001970: 6172 6775 6d65 6e74 7320 2865 6974 6865  arguments (eithe
+00001980: 7220 7468 726f 7567 6820 7468 6520 4755  r through the GU
+00001990: 4920 6f72 206f 6e20 7468 6520 636f 6d6d  I or on the comm
+000019a0: 616e 6420 6c69 6e65 293a 0a20 2020 202a  and line):.    *
+000019b0: 2060 7363 6f72 6562 6f61 7264 7365 7276   `scoreboardserv
+000019c0: 6572 603a 206d 616b 6520 7468 6973 2074  er`: make this t
+000019d0: 6865 2066 756c 6c20 7375 6264 6f6d 6169  he full subdomai
+000019e0: 6e20 6f66 2074 6865 2022 4469 7370 6c61  n of the "Displa
+000019f0: 7920 5552 4c22 2c20 7769 7468 6f75 7420  y URL", without 
+00001a00: 7468 6520 6068 7474 7073 3a2f 2f60 2070  the `https://` p
+00001a10: 6172 742c 2077 6974 6820 603a 3434 3360  art, with `:443`
+00001a20: 2061 6464 6564 2074 6f20 7468 6520 656e   added to the en
+00001a30: 640a 2020 2020 2020 2020 2a20 466f 7220  d.        * For 
+00001a40: 6578 616d 706c 653a 2060 6a61 6d6d 6572  example: `jammer
+00001a50: 2d6c 616e 652e 6465 7262 7973 7461 7473  -lane.derbystats
+00001a60: 2e65 753a 3434 3360 0a20 2020 202a 2060  .eu:443`.    * `
+00001a70: 7373 6c60 3a20 7365 7420 7468 6973 2074  ssl`: set this t
+00001a80: 6f20 6074 7275 6560 2028 6465 6661 756c  o `true` (defaul
+00001a90: 7420 6973 2060 6661 6c73 6560 290a 0a45  t is `false`)..E
+00001aa0: 7861 6d70 6c65 206f 6620 686f 7720 7468  xample of how th
+00001ab0: 6973 206c 6f6f 6b73 206f 6e20 7468 6520  is looks on the 
+00001ac0: 636f 6d6d 616e 646c 696e 653a 0a0a 6070  commandline:..`p
+00001ad0: 7974 686f 6e20 6269 6e2f 6a61 6d73 7461  ython bin/jamsta
+00001ae0: 7473 202d 2d73 636f 7265 626f 6172 6473  ts --scoreboards
+00001af0: 6572 7665 723d 6a61 6d6d 6572 2d6c 616e  erver=jammer-lan
+00001b00: 652e 6465 7262 7973 7461 7473 2e65 753a  e.derbystats.eu:
+00001b10: 3434 3320 2d2d 7373 6c60 0a0a 4578 616d  443 --ssl`..Exam
+00001b20: 706c 6520 6f66 2068 6f77 2074 6869 7320  ple of how this 
+00001b30: 6c6f 6f6b 7320 696e 2074 6865 2047 5549  looks in the GUI
+00001b40: 3a0a 0a21 5b69 6d61 6765 5d28 6874 7470  :..![image](http
+00001b50: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00001b60: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001b70: 742e 636f 6d2f 3731 3430 3737 2f32 3239  t.com/714077/229
+00001b80: 3331 3136 3835 2d62 3434 3335 3964 632d  311685-b44359dc-
+00001b90: 3535 3031 2d34 3335 622d 6165 3434 2d39  5501-435b-ae44-9
+00001ba0: 3033 3933 3137 6632 6630 392e 706e 6729  039317f2f09.png)
+00001bb0: 0a0a 5468 6174 2773 2069 7421 2049 6620  ..That's it! If 
+00001bc0: 7468 6174 2073 6574 7570 2061 6c6c 2077  that setup all w
+00001bd0: 6f72 6b65 6420 636f 7272 6563 746c 792c  orked correctly,
+00001be0: 204a 616d 7374 6174 7320 7368 6f75 6c64   Jamstats should
+00001bf0: 206e 6f77 2062 6568 6176 6520 6578 6163   now behave exac
+00001c00: 746c 7920 6173 2074 686f 7567 6820 796f  tly as though yo
+00001c10: 7520 7765 7265 2072 6967 6874 2074 6865  u were right the
+00001c20: 7265 2061 7420 7468 6520 7472 6163 6b2e  re at the track.
+00001c30: 0a0a 2323 2320 436f 6d6d 616e 646c 696e  ..### Commandlin
+00001c40: 650a 0a54 6865 2063 6f6d 6d61 6e64 2079  e..The command y
+00001c50: 6f75 276c 6c20 7573 6520 6973 2074 6865  ou'll use is the
+00001c60: 2073 616d 6520 6173 2074 6865 206e 616d   same as the nam
+00001c70: 6520 6f66 2074 6865 2066 696c 6520 796f  e of the file yo
+00001c80: 7520 646f 776e 6c6f 6164 6564 2028 652e  u downloaded (e.
+00001c90: 672e 2c20 606a 616d 7374 6174 732d 7630  g., `jamstats-v0
+00001ca0: 2e33 2e34 2d61 6c70 6861 2e65 7865 6020  .3.4-alpha.exe` 
+00001cb0: 6f6e 2057 696e 646f 7773 2c20 6f72 2060  on Windows, or `
+00001cc0: 6a61 6d73 7461 7473 2d6d 6163 2d76 302e  jamstats-mac-v0.
+00001cd0: 332e 342d 616c 7068 6160 206f 6e20 4d61  3.4-alpha` on Ma
+00001ce0: 6329 2e0a 0a2a 496e 2074 6865 2075 7361  c)...*In the usa
+00001cf0: 6765 2062 656c 6f77 2c20 4927 6d20 7265  ge below, I'm re
+00001d00: 706c 6163 696e 6720 7468 6174 2077 6974  placing that wit
+00001d10: 6820 7369 6d70 6c79 2060 6a61 6d73 7461  h simply `jamsta
+00001d20: 7473 602e 2049 6620 796f 7520 7761 6e74  ts`. If you want
+00001d30: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
+00001d40: 6265 2060 6a61 6d73 7461 7473 602c 2072  be `jamstats`, r
+00001d50: 656e 616d 6520 796f 7572 2066 696c 6520  ename your file 
+00001d60: 746f 2060 6a61 6d73 7461 7473 602e 2a0a  to `jamstats`.*.
+00001d70: 0a47 6574 2066 756c 6c20 636f 6d6d 616e  .Get full comman
+00001d80: 646c 696e 6520 6865 6c70 2072 756e 6e69  dline help runni
+00001d90: 6e67 2074 6865 2063 6f6d 6d61 6e64 2077  ng the command w
+00001da0: 6974 6820 7468 6520 602d 2d68 656c 7060  ith the `--help`
+00001db0: 2061 7267 756d 656e 742e 0a0a 2323 2323   argument...####
+00001dc0: 204f 7074 696f 6e20 313a 2067 6574 2067   Option 1: get g
+00001dd0: 616d 6520 6461 7461 2066 726f 6d20 6120  ame data from a 
+00001de0: 4a53 4f4e 2066 696c 650a 0a60 6a61 6d73  JSON file..`jams
+00001df0: 7461 7473 202d 2d6a 736f 6e66 696c 6520  tats --jsonfile 
+00001e00: 3c4a 534f 4e20 6669 6c65 3e20 5b6f 7074  <JSON file> [opt
+00001e10: 696f 6e61 6c20 6172 6775 6d65 6e74 735d  ional arguments]
+00001e20: 600a 0a77 6865 7265 3a0a 0a2a 2060 3c4a  `..where:..* `<J
+00001e30: 534f 4e20 6669 6c65 3e60 2069 7320 7468  SON file>` is th
+00001e40: 6520 7061 7468 2074 6f20 6120 7363 6f72  e path to a scor
+00001e50: 6562 6f61 7264 204a 534f 4e20 6669 6c65  eboard JSON file
+00001e60: 0a2a 2060 5b6f 7074 696f 6e61 6c20 6172  .* `[optional ar
+00001e70: 6775 6d65 6e74 735d 603a 2062 7920 6465  guments]`: by de
+00001e80: 6661 756c 742c 204a 616d 7374 6174 7320  fault, Jamstats 
+00001e90: 7769 6c6c 2077 7269 7465 2074 6865 206f  will write the o
+00001ea0: 7574 7075 7420 746f 2074 6865 2073 616d  utput to the sam
+00001eb0: 6520 7061 7468 2061 7320 7468 6520 696e  e path as the in
+00001ec0: 7075 7420 6669 6c65 2c20 6275 7420 7769  put file, but wi
+00001ed0: 7468 2022 2e6a 736f 6e22 2072 6570 6c61  th ".json" repla
+00001ee0: 6365 6420 7769 7468 2022 2e70 6466 222e  ced with ".pdf".
+00001ef0: 2059 6f75 2063 616e 2061 646a 7573 7420   You can adjust 
+00001f00: 7468 6174 2062 6568 6176 696f 7220 6279  that behavior by
+00001f10: 2073 7065 6369 6679 696e 6720 616e 206f   specifying an o
+00001f20: 7574 7075 7420 602d 2d6f 7574 6669 6c65  utput `--outfile
+00001f30: 6020 6669 6c65 206f 7220 7573 696e 6720  ` file or using 
+00001f40: 7468 6520 602d 2d6d 6f64 653d 7765 6260  the `--mode=web`
+00001f50: 2061 7267 756d 656e 7420 746f 2073 7461   argument to sta
+00001f60: 7274 2061 2077 6562 7365 7276 6572 2028  rt a webserver (
+00001f70: 7365 6520 6265 6c6f 7729 2c20 696e 7374  see below), inst
+00001f80: 6561 642e 0a20 2020 202a 2074 6865 7265  ead..    * there
+00001f90: 2061 7265 2061 6c73 6f20 7365 7665 7261   are also severa
+00001fa0: 6c20 6f70 7469 6f6e 732c 2065 7870 6c61  l options, expla
+00001fb0: 696e 6564 2069 6e20 7468 6520 6865 6c70  ined in the help
+00001fc0: 206d 6573 7361 6765 2c20 7468 6174 2061   message, that a
+00001fd0: 6666 6563 7420 7468 6520 6368 6172 7473  ffect the charts
+00001fe0: 2074 6861 7420 6172 6520 6275 696c 742e   that are built.
+00001ff0: 0a0a 2323 2323 204f 7074 696f 6e20 323a  ..#### Option 2:
+00002000: 2063 6f6e 6e65 6374 2074 6f20 6120 7275   connect to a ru
+00002010: 6e6e 696e 6720 7363 6f72 6562 6f61 7264  nning scoreboard
+00002020: 2073 6572 7665 720a 0a60 6a61 6d73 7461   server..`jamsta
+00002030: 7473 202d 2d73 636f 7265 626f 6172 6473  ts --scoreboards
+00002040: 6572 7665 7220 3c73 6572 7665 723a 706f  erver <server:po
+00002050: 7274 3e20 5b6f 7074 696f 6e61 6c20 6172  rt> [optional ar
+00002060: 6775 6d65 6e74 735d 600a 0a77 6865 7265  guments]`..where
+00002070: 3a0a 0a2a 2060 3c73 6572 7665 723a 706f  :..* `<server:po
+00002080: 7274 3e60 2069 7320 7468 6520 7365 7276  rt>` is the serv
+00002090: 6572 2061 6e64 2070 6f72 7420 6e75 6d62  er and port numb
+000020a0: 6572 2028 652e 672e 2c20 6031 3237 2e30  er (e.g., `127.0
+000020b0: 2e30 2e31 3a38 3030 3060 2920 6f66 2061  .0.1:8000`) of a
+000020c0: 2072 756e 6e69 6e67 2073 636f 7265 626f   running scorebo
+000020d0: 6172 642e 206a 616d 7374 6174 7320 7769  ard. jamstats wi
+000020e0: 6c6c 2063 6f6e 6e65 6374 2074 6f20 7468  ll connect to th
+000020f0: 6520 7363 6f72 6562 6f61 7264 2061 6e64  e scoreboard and
+00002100: 2064 6f77 6e6c 6f61 6420 7468 6520 6375   download the cu
+00002110: 7272 656e 7420 6761 6d65 2073 7461 7465  rrent game state
+00002120: 2e0a 2a20 603c 736f 6d65 2061 7267 756d  ..* `<some argum
+00002130: 656e 7473 2074 6f20 6465 6669 6e65 2074  ents to define t
+00002140: 6865 206f 7574 7075 743e 603a 2073 616d  he output>`: sam
+00002150: 6520 6173 2061 626f 7665 2e20 596f 7520  e as above. You 
+00002160: 6361 6e20 726f 7574 6520 7468 6520 6f75  can route the ou
+00002170: 7470 7574 2074 6f20 6120 5044 4620 6669  tput to a PDF fi
+00002180: 6c65 2062 7920 7370 6563 6966 7969 6e67  le by specifying
+00002190: 2060 2d2d 6d6f 6465 3d70 6466 602e 0a0a   `--mode=pdf`...
+000021a0: 0a5c 2a20 2a49 2061 6d20 6e6f 7420 6120  .\* *I am not a 
+000021b0: 7765 6220 7365 6375 7269 7479 2065 7870  web security exp
+000021c0: 6572 742c 2061 6e64 2049 206d 616b 6520  ert, and I make 
+000021d0: 6e6f 2067 7561 7261 6e74 6565 7320 7768  no guarantees wh
+000021e0: 6174 736f 6576 6572 2061 626f 7574 2077  atsoever about w
+000021f0: 6562 7365 7276 6572 2073 6563 7572 6974  ebserver securit
+00002200: 792e 2049 6620 796f 7527 7265 2063 6f6e  y. If you're con
+00002210: 6365 726e 6564 2061 6e64 2077 616e 7420  cerned and want 
+00002220: 746f 2068 656c 7020 6d61 6b65 2069 7420  to help make it 
+00002230: 6d6f 7265 2073 6563 7572 652c 2070 6c65  more secure, ple
+00002240: 6173 6520 6f70 656e 2061 6e20 6973 7375  ase open an issu
+00002250: 6521 2a0a                                e!*.
```

### Comparing `jamstats-1.2.0/setup.py` & `jamstats-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats',
-    version='1.2.0',
+    version='1.2.1',
     description='Data processing, stats and plots on roller derby scoreboard JSON files',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=find_packages('src', exclude=['test']),
     scripts=['bin/jamstats'],
     install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'gooey>=1.0.8.1', 'websocket-client>=1.2.1',
```

### Comparing `jamstats-1.2.0/src/jamstats.egg-info/SOURCES.txt` & `jamstats-1.2.1/src/jamstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/src/jamstats/util/resources.py` & `jamstats-1.2.1/src/jamstats/util/resources.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/src/jamstats/web/statserver.py` & `jamstats-1.2.1/src/jamstats/web/statserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         PLOT_NAME_FUNC_MAP[name] = func
 PLOT_SECTION_NAMES_MAP = {
     section: list(amap.keys()) for section, amap in PLOT_SECTION_NAME_FUNC_MAP.items()
 }
 ALL_PLOT_NAMES = list(PLOT_NAME_FUNC_MAP.keys())
 
 HTML_PLOT_NAMES = list(PLOT_SECTION_NAME_FUNC_MAP["Tables"].keys())
-print(HTML_PLOT_NAMES)
 PLOT_NAME_TYPE_MAP = {
     plot_name: "html" if plot_name in HTML_PLOT_NAMES else "figure"
     for plot_name in ALL_PLOT_NAMES
 }
 
 PLOT_NAMES_TO_SHOW_BEFORE_GAME_START = [
     "Team Rosters",
@@ -199,14 +198,15 @@
     app.derby_game = derby_game
     app.game_update_time = datetime.now()
 
 
 @app.route("/")
 def index():
     logger.debug("Index page requested")
+
     if app.scoreboard_server is not None:
         logger.debug(f"Scoreboard server is {app.scoreboard_server}")
         if app.scoreboard_client is None:
             logger.debug("No scoreboard client. Creating one...")
             try:
                 app.scoreboard_client = ScoreboardClient(app.scoreboard_server, app.scoreboard_port)
                 # add listener to update webclient when game state changes
```

### Comparing `jamstats-1.2.0/src/jamstats/io/tsv_io.py` & `jamstats-1.2.1/src/jamstats/io/tsv_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/src/jamstats/io/scoreboard_json_io.py` & `jamstats-1.2.1/src/jamstats/io/scoreboard_json_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     This method is trivial, just loads the json. Putting it here in case more
     complicated things tneed to happen later.
 
     Returns:
         Dict[str, Any]: Game JSON
     """
     try:
-        with open(filepath) as game_file:
+        with open(filepath, 'r', errors='replace') as game_file:
             game_json = json.load(game_file)
             return game_json
     except Exception as e:
         logger.warn("Failed to parse game JSON file. Trying Windows encoding...")
-        with io.open(filepath, 'r', encoding='windows-1252') as game_file:
+        with io.open(filepath, 'r', errors='replace', encoding='windows-1252') as game_file:
             game_json = json.load(game_file)
             return game_json
 
 def load_inprogress_game_from_server(server: str, port: int) -> DerbyGame:
     """Connect to server at server:port, download the in-game JSON, make DerbyGame
 
     Args:
```

### Comparing `jamstats-1.2.0/src/jamstats/io/scoreboard_server_io.py` & `jamstats-1.2.1/src/jamstats/io/scoreboard_server_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import websocket
 import json
 import logging
 import traceback
 import ssl
 import time
+from pprint import pprint
 
 logger = logging.getLogger(__name__)
 
 
 class GameStateListener:
     def on_game_state_changed(self) -> None:
         """Called when the game state changes
@@ -130,25 +131,42 @@
                                               if message_game_state_dict[key] is None] 
                     for key in nullvalue_message_keys:
                         if key in self.game_json_dict["state"]:
                             del self.game_json_dict["state"][key]
                         for state_key in self.game_json_dict["state"]:
                             if state_key.startswith(key + "."):
                                 del self.game_json_dict["state"][state_key]
+
+                    # Special handling for current jammer. If the jam has just ended, null out
+                    # the current jammers. There are no known jammers until they're redefined
+                    # for the next jam.
+                    if 'ScoreBoard.Clock(Jam).Running' in message_game_state_dict and \
+                      not message_game_state_dict['ScoreBoard.Clock(Jam).Running']:
+                        for team_number in (1, 2):
+                            for akey in [
+                                f"ScoreBoard.Team({team_number}).Position(Jammer).Name",
+                                f"ScoreBoard.Team({team_number}).Position(Jammer).RosterNumber"
+                            ]:
+                                try:
+                                    del self.game_json_dict["state"][akey]
+                                except Exception:
+                                    pass
+
                     # now, add all the new data from the message.
                     for key in message_game_state_dict:
                         if message_game_state_dict[key] is not None:
                             self.game_json_dict["state"][key] = message_game_state_dict[key]
                 else:
                     logger.debug("Replacing game_json_dict with message_dict")
                     self.game_json_dict = message_dict
                 # determine whether there was a meaningful change to the game state
                 for key in message_game_state_dict:
                     if not key.startswith("ScoreBoard.CurrentGame.Clock") and key != "ScoreBoard.Version(release)":
                         self.game_state_dirty = True
+                        #pprint(message_dict, indent=4)
                         logger.debug(f"Setting game state dirty because {key}. Updating listeners.")
                         for listener in self.game_state_listeners:
                             listener.on_game_state_changed()
                         break
             #logger.debug("Loaded game state from message.")
         except Exception as e:
             self.exceptions.append(e)
@@ -177,15 +195,14 @@
             logger.info("ws closed.")
         except Exception as e:
             logger.warning(f"ws.close() failed: {e}")
         # wait a second
         time.sleep(1)
         
     def on_ping(self, ws):
-        print("on_ping")
         self.send_custom_message(ws, { "action": "Ping" })
 
     def on_open(self, ws):
         """Send the registration message to the server
 
         Args:
             ws (_type_): websocket
```

### Comparing `jamstats-1.2.0/src/jamstats/data/json_to_pandas.py` & `jamstats-1.2.1/src/jamstats/data/json_to_pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     game_data_dict = extract_game_data_dict(pdf_game_state)
     game_data_dict["scoreboard_version"] = json_version
 
     logger.debug("Extracting roster")
     pdf_roster = extract_roster(pdf_game_state,
                                 game_data_dict["team_1"],
                                 game_data_dict["team_2"])
+    logger.debug("Roster columns: " + str(pdf_roster.columns))
     pdf_ref_roster = extract_officials_roster(pdf_game_state, "Ref")
     pdf_nso_roster = extract_officials_roster(pdf_game_state, "Nso")
     logger.debug("Extracting jam data")
     pdf_game_data = extract_jam_data(pdf_game_state, pdf_roster)
     logger.debug("Extracting penalties")
     pdf_penalties = extract_penalties(pdf_game_state, pdf_roster,
                                       json_major_version)
@@ -193,18 +194,45 @@
             team_name_1 = team_name_1 + " (1)"
             team_name_2 = team_name_2 + " (1)"
 
     # Get rid of weird characters in team names
     team_name_1 = cleanup_team_name(team_name_1)
     team_name_2 = cleanup_team_name(team_name_2)
 
+    # Get team jammer names and numbers
+    team_1_jammer_name = ""
+    team_2_jammer_name = ""
+    team_1_jammer_number = ""
+    team_2_jammer_number = ""
+    try:
+        team_1_jammer_name = pdf_game_state[pdf_game_state.key == "ScoreBoard.Team(1).Position(Jammer).Name"].value.iloc[0]
+        team_1_jammer_number = pdf_game_state[pdf_game_state.key == "ScoreBoard.Team(1).Position(Jammer).RosterNumber"].value.iloc[0]
+    except Exception:
+        pass
+    try:
+        team_2_jammer_name = pdf_game_state[pdf_game_state.key == "ScoreBoard.Team(2).Position(Jammer).Name"].value.iloc[0]
+        team_2_jammer_number = pdf_game_state[pdf_game_state.key == "ScoreBoard.Team(2).Position(Jammer).RosterNumber"].value.iloc[0]
+    except Exception:
+        pass
+
+    jam_is_running = False
+    try:
+        jam_is_running = pdf_game_state[pdf_game_state.key == 'ScoreBoard.Clock(Jam).Running'].value.iloc[0]
+    except Exception:
+        pass
+
     return {
         "game_status": game_status,
         "team_1": team_name_1,
-        "team_2": team_name_2
+        "team_2": team_name_2,
+        "team_1_jammer_name": team_1_jammer_name,
+        "team_2_jammer_name": team_2_jammer_name,
+        "team_1_jammer_number": team_1_jammer_number,
+        "team_2_jammer_number": team_2_jammer_number,
+        "jam_is_running": jam_is_running
     }
 
 def extract_jam_data(pdf_game_state: pd.DataFrame,
                      pdf_roster: pd.DataFrame) -> pd.DataFrame:
     """Process all the jam-level data into a dataframe
     with one row per jam.
 
@@ -349,17 +377,19 @@
         pdf_jams_summary["PeriodClockElapsedStart"]) / 1000
     pdf_jams_summary["jam_starttime_seconds"] = pdf_jams_summary[
         "PeriodClockElapsedStart"] / 1000
     pdf_jams_summary["jam_endtime_seconds"] = pdf_jams_summary[
         "PeriodClockElapsedEnd"] / 1000
 
     # Drop a bunch of useless columns
-    pdf_jams_summary = pdf_jams_summary.drop(columns=[
-    "Duration", "Id", "Next", "PeriodClockDisplayEnd", "Previous", "Readonly",
-    "PeriodClockElapsedEnd", "PeriodClockElapsedStart"])
+    useless_columns = [
+        "Duration", "Id", "Next", "PeriodClockDisplayEnd", "Previous", "Readonly",
+        "PeriodClockElapsedEnd", "PeriodClockElapsedStart"]
+    pdf_jams_summary = pdf_jams_summary.drop(columns=[x for x in useless_columns
+                                                      if x in pdf_jams_summary.columns])
 
     return pdf_jams_summary
 
 def extract_roster(pdf_game_state: pd.DataFrame,
                    team_name_1: str, team_name_2: str) -> pd.DataFrame:
     """Extract a DataFrame representing the rosters of the two
     teams.
@@ -409,15 +439,15 @@
     pdf_game_state_roster["skater"] = [
         chunks[2][chunks[2].index("(") + 1:chunks[2].index(")")]
         for chunks in pdf_game_state_roster.key_chunks]
     pdf_game_state_roster["roster_key"] = [
         chunks[3] for chunks in pdf_game_state_roster.key_chunks]
     # dump a bunch of extraneous columns
     pdf_game_state_roster = pdf_game_state_roster[pdf_game_state_roster.roster_key.isin(
-        ["Id", "Name", "RosterNumber", "team"]
+        ["Id", "Name", "RosterNumber", "Number", "team"]
     )]
     pdf_roster = pdf_game_state_roster.pivot(index="skater", columns="roster_key", values="value")
     logger.debug("pdf_roster columns: " + str(pdf_roster.columns) + 
                  ". Before dropping nulls, length: " + str(len(pdf_roster)))
     pdf_roster = pdf_roster[pdf_roster.Id.notnull()]
     logger.debug("After dropping nulls, length: " + str(len(pdf_roster)))
 
@@ -471,26 +501,28 @@
     # add jammer info
     pdf_ateamjams_jammers = pdf_ateamjams_data[
         pdf_ateamjams_data.key.str.endswith("Fielding(Jammer).Skater")][
             ["prd_jam", "value"]].rename(columns={"value": "jammer_id"})
     pdf_ateamjams_summary = pdf_ateamjams_summary.merge(pdf_ateamjams_jammers,
         on="prd_jam", how="left")
     pdf_ateamjams_summary = pdf_ateamjams_summary.merge(pdf_roster.rename(
-        columns={"Id": "jammer_id", "Name": "jammer_name", "RosterNumber": "jammer_number"}),
+        columns={"Id": "jammer_id", "Name": "jammer_name", "RosterNumber": "jammer_number",
+                 "Number": "jammer_number"}),
         on="jammer_id", how="left")
     logger.debug(f"After adding jammer info: {len(pdf_ateamjams_summary)}")
 
     # add pivot info
     pdf_ateamjams_pivots = pdf_ateamjams_data[
         pdf_ateamjams_data.key.str.endswith("Fielding(Pivot).Skater")][
             ["prd_jam", "value"]].rename(columns={"value": "pivot_id"})
     pdf_ateamjams_summary = pdf_ateamjams_summary.merge(pdf_ateamjams_pivots,
         on="prd_jam", how="left")
     pdf_ateamjams_summary = pdf_ateamjams_summary.merge(pdf_roster.rename(
-        columns={"Id": "pivot_id", "Name": "pivot_name", "RosterNumber": "pivot_number"}),
+        columns={"Id": "pivot_id", "Name": "pivot_name", "RosterNumber": "pivot_number",
+                 "Number": "pivot_number"}),
         on="pivot_id", how="left")
     logger.debug(f"After adding pivot info: {len(pdf_ateamjams_summary)}")
 
     # add list of skater names per jam
     pdf_jam_skater_lists = extract_team_perjam_skaters(pdf_ateamjams_data, pdf_roster)
     pdf_ateamjams_summary = pdf_ateamjams_summary.merge(
         pdf_jam_skater_lists, on="prd_jam"
@@ -502,14 +534,15 @@
     logger.debug(f"Loaded {len(pdf_scoringtrips)} scoring trips.")
     scoringtrip_cols_to_rename = [x for x in pdf_scoringtrips.columns
                                   if x != "prd_jam"]
 
     pdf_ateamjams_summary_withscoringtrips = pdf_ateamjams_summary.merge(
         pdf_scoringtrips, on="prd_jam")
     logger.debug(f"After adding scoring trips: {len(pdf_ateamjams_summary_withscoringtrips)}")
+    logger.debug(pdf_ateamjams_summary_withscoringtrips.columns)
     pdf_ateamjams_summary_kept = pdf_ateamjams_summary_withscoringtrips[
         ["prd_jam"] + TEAMJAM_SUMMARY_COLUMNS + scoringtrip_cols_to_rename]
 
     pdf_ateamjams_summary_kept_colsrenamed = pdf_ateamjams_summary_kept.rename(
         columns={col: f"{col}_{team_number}"
                  for col in TEAMJAM_SUMMARY_COLUMNS + scoringtrip_cols_to_rename})
 
@@ -535,24 +568,18 @@
     pdf_ateamjams_data_skaters = pdf_ateamjams_data_fielding[
         pdf_ateamjams_data_fielding.keychunk_5 == "Skater"]
     pdf_ateamjams_data_skaters = pdf_ateamjams_data_skaters.rename(columns={
         "value": "Id"
     })
 
     logger.debug(f"    Before roster merge, team jam skater data: {len(pdf_ateamjams_data_skaters)}")
+    # left join to deal with completely or partially missing skater names
     pdf_ateamjams_data_skaters_withname = pdf_ateamjams_data_skaters.merge(
-        pdf_roster, on="Id")
-    # Sometimes, we're unable to get proper roster data, e.g., for an in-progress game.
-    # In that case, merging back to the roster gives us nothing.
-    # Let's limp along with a left join so we can show most of the plots.
-    if len(pdf_ateamjams_data_skaters_withname) == 0:
-        pdf_ateamjams_data_skaters_withname = pdf_ateamjams_data_skaters.merge(
-            pdf_roster, on="Id", how="left")
-        logger.debug("Failed to join skater data with roster. Merged with left join, "
-                    f"rows {len(pdf_ateamjams_data_skaters_withname)}")
+        pdf_roster, on="Id", how="left")
+    
     logger.debug(f"    After roster merge, team jam skater data: {len(pdf_ateamjams_data_skaters_withname)}")
     pdf_jam_skater_lists = pdf_ateamjams_data_skaters_withname.groupby(
         "prd_jam")["Name"].apply(list).reset_index()
     pdf_jam_skater_lists = pdf_jam_skater_lists.rename(columns={"Name": "Skaters"})
     logger.debug(f"    Jam skater lists length: {len(pdf_jam_skater_lists)}")
 
     return pdf_jam_skater_lists
@@ -671,15 +698,16 @@
         f"{period}:{'0' if (jam < 10) else ''}{jam}" 
         for period, jam in zip(*[pdf_penalties.PeriodNumber, pdf_penalties.JamNumber])]
     # cast is necessary if there are no penalties yet
     pdf_penalties = pdf_penalties.astype({"prd_jam": str})
     pdf_penalties = pdf_penalties.rename(columns={"Code": "penalty_code"})
 
     logger.debug(f"    Before merging with roster: {len(pdf_penalties)}")
-    pdf_penalties = pdf_penalties.merge(pdf_roster[["Id", "Name", "RosterNumber", "team"]], on="Id")
+    rosternumber_col = "RosterNumber" if "RosterNumber" in pdf_roster else "Number"
+    pdf_penalties = pdf_penalties.merge(pdf_roster[["Id", "Name", rosternumber_col, "team"]], on="Id")
     logger.debug(f"    After merging with roster: {len(pdf_penalties)}")
 
     # add penalty names
     pdf_penalty_codes_names = build_penalty_code_name_map(pdf_game_state, json_major_version)
     pdf_penalties = pdf_penalties.merge(pdf_penalty_codes_names, on="penalty_code")
     logger.debug(f"Extracted penalties: {len(pdf_penalties)} rows.")
     return pdf_penalties
```

### Comparing `jamstats-1.2.0/src/jamstats/data/game_data.py` & `jamstats-1.2.1/src/jamstats/data/game_data.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/src/jamstats/plots/plot_together.py` & `jamstats-1.2.1/src/jamstats/plots/plot_together.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.0/src/jamstats/plots/skaterplots.py` & `jamstats-1.2.1/src/jamstats/plots/skaterplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,25 +184,20 @@
             columns='Penalty', index='Skater', values="penalty_count")
 
         pdf_penalty_plot["skater_order"] = [skater_penaltycount_map[skater]
                                            for skater in pdf_penalty_plot.index]
         pdf_penalty_plot = pdf_penalty_plot.sort_values("skater_order", ascending=False)
         pdf_penalty_plot = pdf_penalty_plot.drop(columns=["skater_order"])
 
-        # sort skater data, too
-        
-        # this would be better done with a dataframe and a join. Eh.
-        pdf_skater_data["skater_order"] = [skater_penaltycount_map[skater]
-                                            for skater in pdf_skater_data.Skater]
-        pdf_skater_data = pdf_skater_data.sort_values("skater_order", ascending=False)
-        pdf_skater_data = pdf_skater_data.drop(columns=["skater_order"])
-
         # add penalties per jam
         pdf_skater_data["penalty_count"] = [skater_penaltycount_map[skater]
+                                            if skater in skater_penaltycount_map else 0
                                             for skater in pdf_skater_data.Skater]
+        # sort skater data, too
+        pdf_skater_data = pdf_skater_data.sort_values("penalty_count", ascending=False)
         pdf_skater_data["penalties_per_jam"] = (
             pdf_skater_data["penalty_count"] / pdf_skater_data["Jams"])
 
         penalty_plot_is_go = True
     except Exception as e:
         logger.warn(f"Failed to make skater penalty subplot:")
         logger.warn(traceback.format_exc())
```

### Comparing `jamstats-1.2.0/src/jamstats/plots/jamplots.py` & `jamstats-1.2.1/src/jamstats/plots/jamplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,21 +146,30 @@
         column: [pdf_game_teams_summary.loc[0, column],
                  pdf_game_teams_summary.loc[1, column],
                  abs(pdf_game_teams_summary.loc[0, column] -
                      pdf_game_teams_summary.loc[1, column])]
         if column != "Team"
         else [pdf_game_teams_summary.loc[0, column],
               pdf_game_teams_summary.loc[1, column],
-              "Absolute Difference"]
+              "Difference (absolute)"]
         for column in pdf_game_teams_summary.columns
     })
     styler = pdf_game_teams_summary.style.set_table_attributes("style='display:inline'").hide_index()
     html_game_summary = styler.render()
 
-    # build current jam table
+    # if we're *not* in a jam, show the jammers for the next jam
+    if not derby_game.game_data_dict["jam_is_running"]:
+        next_jam_section = "\n<p><b>Next jam's jammers:</b><br>\n"
+        next_jam_section = next_jam_section + f"<table width=100% style='padding: 5px'><tr><th>{derby_game.team_1_name}</th><th>{derby_game.team_2_name}</th></tr>\n"
+        next_jam_section += f"<tr><td>{derby_game.game_data_dict['team_1_jammer_number']} {derby_game.game_data_dict['team_1_jammer_name']}</td>\n"
+        next_jam_section += f"<td>{derby_game.game_data_dict['team_2_jammer_number']} {derby_game.game_data_dict['team_2_jammer_name']}</td></tr>\n"
+        next_jam_section += f"</table>\n"
+        html_game_summary = html_game_summary + next_jam_section
+        
+    # build most-recent jam table
     pdf_jams_sorted_desc = derby_game.pdf_jams_data.sort_values(["PeriodNumber", "Number"],
                                                                 ascending=False)
     pdf_jams_sorted_desc.index = range(len(pdf_jams_sorted_desc))
     html_current_jam = get_singlejam_skaters_html(derby_game, pdf_jams_sorted_desc.head(1),
                                                   anonymize_names=anonymize_names)
     
     result =  "<p>" + html_game_summary + "</p><p>" + html_current_jam
@@ -253,16 +262,21 @@
         table_htmls.append(styler.render())
 
     _, latest_jam_row_dict = next(pdf_one_jam.iterrows())
     period = latest_jam_row_dict["PeriodNumber"]
     number = latest_jam_row_dict["Number"]
     result = f"Period {period}, Jam {number}<br>"
 
-    result = result + f"<table width=0%><tr><td><h4>{derby_game.team_1_name}</h4>{table_htmls[0]}</td>"
-    result = result + f"<td><h4>{derby_game.team_2_name}</h4>{table_htmls[1]}</td></tr></table>\n"    
+    # extract current jam score per team
+    _, latest_jam_row_dict = next(pdf_one_jam.iterrows())
+    team_1_jamscore = latest_jam_row_dict["JamScore_1"]
+    team_2_jamscore = latest_jam_row_dict["JamScore_2"]
+
+    result = result + f"<table width=0%><tr><td><h5>{derby_game.team_1_name}: {team_1_jamscore}</h5>{table_htmls[0]}</td>"
+    result = result + f"<td><h5>{derby_game.team_2_name}: {team_2_jamscore}</h5>{table_htmls[1]}</td></tr></table>\n"    
     return result
 
 
 def get_team_jam_skaters_pdf(derby_game: DerbyGame, team_name: str,
                              pdf_one_jam: pd.DataFrame,
                              anonymize_names: bool = False,
                              include_alljam_serving_penalties: bool = True) -> pd.DataFrame:
```

### Comparing `jamstats-1.2.0/src/jamstats/plots/plot_util.py` & `jamstats-1.2.1/src/jamstats/plots/plot_util.py`

 * *Files identical despite different names*

