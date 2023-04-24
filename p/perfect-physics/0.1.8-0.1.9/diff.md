# Comparing `tmp/perfect_physics-0.1.8-py3-none-any.whl.zip` & `tmp/perfect_physics-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 369270 bytes, number of entries: 25
+Zip file size: 369297 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat      319 b- defN 22-Nov-22 03:19 perfect_physics/__init__.py
 -rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-18 15:33 perfect_physics/_circle.py
--rw-rw-rw-  2.0 fat     2863 b- defN 23-Apr-20 02:11 perfect_physics/_misc.py
+-rw-rw-rw-  2.0 fat     2962 b- defN 23-Apr-24 22:27 perfect_physics/_misc.py
 -rw-rw-rw-  2.0 fat    14658 b- defN 23-Apr-24 22:11 perfect_physics/_physics.py
 -rw-rw-rw-  2.0 fat     3334 b- defN 23-Apr-24 22:11 perfect_physics/_timeline.py
 -rw-rw-rw-  2.0 fat      904 b- defN 22-Nov-18 02:58 perfect_physics/_wall.py
--rw-rw-rw-  2.0 fat    26573 b- defN 23-Apr-24 22:11 perfect_physics/_world.py
+-rw-rw-rw-  2.0 fat    26620 b- defN 23-Apr-24 22:28 perfect_physics/_world.py
 -rw-rw-rw-  2.0 fat     8653 b- defN 10-Mar-23 21:08 perfect_physics/data/Electronic Button.mp3
 -rw-rw-rw-  2.0 fat     5958 b- defN 10-Mar-23 21:08 perfect_physics/data/Flash Beep.mp3
 -rw-rw-rw-  2.0 fat    37384 b- defN 22-Nov-04 21:14 perfect_physics/data/ball_ball.wav
 -rw-rw-rw-  2.0 fat   149152 b- defN 22-Nov-16 18:36 perfect_physics/data/bumper.wav
 -rw-rw-rw-  2.0 fat     9928 b- defN 22-Nov-09 15:59 perfect_physics/data/cc_time_solutions.sympy
 -rw-rw-rw-  2.0 fat     9148 b- defN 22-Nov-11 02:53 perfect_physics/data/cc_velocity_solution.sympy
 -rw-rw-rw-  2.0 fat     1505 b- defN 22-Nov-09 23:07 perfect_physics/data/cw_time_solutions.sympy
 -rw-rw-rw-  2.0 fat     1925 b- defN 22-Nov-11 18:01 perfect_physics/data/cw_velocity_limits.sympy
 -rw-rw-rw-  2.0 fat     5315 b- defN 22-Nov-12 15:43 perfect_physics/data/instant_speed.sympy
 -rw-rw-rw-  2.0 fat     6740 b- defN 22-Nov-12 15:45 perfect_physics/data/instant_speed_wall.sympy
 -rw-rw-rw-  2.0 fat   283896 b- defN 22-Nov-19 18:05 perfect_physics/data/reverse.wav
 -rw-rw-rw-  2.0 fat    53278 b- defN 22-Nov-04 21:17 perfect_physics/data/stick_cue.wav
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-27 19:29 perfect_physics/tests/__init__.py
 -rw-rw-rw-  2.0 fat     5518 b- defN 22-Nov-22 03:19 perfect_physics/tests/test_perfect_physics.py
--rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 22:19 perfect_physics-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 22:19 perfect_physics-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 22:19 perfect_physics-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2262 b- defN 23-Apr-24 22:19 perfect_physics-0.1.8.dist-info/RECORD
-25 files, 632944 bytes uncompressed, 365564 bytes compressed:  42.2%
+-rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 23:13 perfect_physics-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 23:13 perfect_physics-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 23:13 perfect_physics-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2262 b- defN 23-Apr-24 23:13 perfect_physics-0.1.9.dist-info/RECORD
+25 files, 633090 bytes uncompressed, 365591 bytes compressed:  42.3%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: perfect_physics/tests/__init__.py
 Comment: 
 
 Filename: perfect_physics/tests/test_perfect_physics.py
 Comment: 
 
-Filename: perfect_physics-0.1.8.dist-info/METADATA
+Filename: perfect_physics-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: perfect_physics-0.1.8.dist-info/WHEEL
+Filename: perfect_physics-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: perfect_physics-0.1.8.dist-info/top_level.txt
+Filename: perfect_physics-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: perfect_physics-0.1.8.dist-info/RECORD
+Filename: perfect_physics-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perfect_physics/_misc.py

```diff
@@ -44,14 +44,15 @@
     ylim=(-5, 5),
     figsize=(19.2 / 4, 10.8 / 4),
     font_scale=4,
     colors=["tab:blue"],
     draw_wall_points=False,
     draw_radius=1.0,
     label_fun=None,
+    show_fun=None,
 ):
     sns.set()
     figure = Figure(figsize=figsize)
     axes = figure.add_subplot()
     axes.set_aspect(1)
     axes.set_xlim(float(xlim[0]), float(xlim[1]))
     axes.set_ylim(float(ylim[0]), float(ylim[1]))
@@ -94,9 +95,12 @@
 
     if show:
         new_manager = plt.figure().canvas.manager
         new_manager.canvas.figure = figure
         figure.set_canvas(new_manager.canvas)
         figure.set_dpi(100 * font_scale)
         figure.tight_layout()
-        figure.show()
+        if show_fun is None:
+            figure.show()
+        else:
+            show_fun(figure)
     return figure
```

## perfect_physics/_world.py

```diff
@@ -42,24 +42,25 @@
         self.clock = 0
         self.physics = Physics()
         # if rng is integer, use it as a seed for a random number generator
         if isinstance(rng, int):
             rng = random.Random(rng)
         self.rng = rng
 
-    def figure(self, font_scale=1, label_fun=None, **kwargs):
+    def figure(self, font_scale=1, label_fun=None, show_fun=None, **kwargs):
         return plot(
             show=False,
             circle_list=self.circle_list,
             wall_list=self.wall_list,
             clock=self.clock,
             font_scale=font_scale,
             xlim=self.xlim,
             ylim=self.ylim,
             label_fun=label_fun,
+            show_fun=show_fun,
             **kwargs,
         )
 
     def show(self, font_scale=1, show=True, draw_radius=1.0, **kwargs):
         if not show:
             return
         return plot(
```

## Comparing `perfect_physics-0.1.8.dist-info/METADATA` & `perfect_physics-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.8
+Version: 0.1.9
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 Requires-Dist: numpy
```

## Comparing `perfect_physics-0.1.8.dist-info/RECORD` & `perfect_physics-0.1.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 perfect_physics/__init__.py,sha256=7qZEJu1mRKkDQiy6bKCSlBP-XtoaJGIPMYTbWjH1_Z4,319
 perfect_physics/_circle.py,sha256=Re97mYXct8XTECR_CGLEj5QNTIp076ra9RDH3ipeC_4,1959
-perfect_physics/_misc.py,sha256=wb-eP_61aOzu6Y8CipgCzqDnG1HtgFUN-GILe0QuqHM,2863
+perfect_physics/_misc.py,sha256=tJ7RC3Lrub7IQMokMXRv7a5jCarWhSEeJWQGsCUr9rw,2962
 perfect_physics/_physics.py,sha256=wlA2GTQDkV2ezBo2AljhB9J7_6O9pEoScFO1SnoEGqE,14658
 perfect_physics/_timeline.py,sha256=Tff9MWf8TUw_y15U_4YB_A8uJcnkKcBpytitgir3hek,3334
 perfect_physics/_wall.py,sha256=Aja12LIleDdS28d4su-culGbchZNVjDBd7MIyCP_zvg,904
-perfect_physics/_world.py,sha256=Pa2yaIq4ZyR1nl-vMKkaqk_0G2MlynYPAWwFFkwMb7k,26573
+perfect_physics/_world.py,sha256=Idwn5y7KKG2vFjt_8-QBhEiPK2ioTgY5LYDFAmFHJ9c,26620
 perfect_physics/data/Electronic Button.mp3,sha256=Eurq00KisW9yQO_zCPOfEwfKmsivP4wLzLu_3wPPZK8,8653
 perfect_physics/data/Flash Beep.mp3,sha256=b1qd5QfeMLUKdJhg5KZc2ZDaIFC28FyrxxKb3J4wnNk,5958
 perfect_physics/data/ball_ball.wav,sha256=5uCXwGKf2Oo3WVZwIltaDiQ1MM20CP4--NcapitmBfM,37384
 perfect_physics/data/bumper.wav,sha256=Tlme9Y55oBiS33JdOKNuq6Ef2GuvnlKiYZeCjKbBWDE,149152
 perfect_physics/data/cc_time_solutions.sympy,sha256=_P1NJrjVnN_GXSmTyqi8aSd65WIbqB72cFc5RcB2ekE,9928
 perfect_physics/data/cc_velocity_solution.sympy,sha256=kwx7C83q1NTNj1Elxftjm8z6sJQPgn1d0FFDG8DiMaM,9148
 perfect_physics/data/cw_time_solutions.sympy,sha256=94soYQeDhI-mfl2YNn5yY7XZF1WgHjZu2CJ17vWuc8k,1505
 perfect_physics/data/cw_velocity_limits.sympy,sha256=fr2z9kBiL1rx9wyljRvzfKgaSEuMDrKX2WVxdipa8-I,1925
 perfect_physics/data/instant_speed.sympy,sha256=QWBCRTvy2xFWO5SWcUFijZI1GHr3zwBSUuDEnvyg_-g,5315
 perfect_physics/data/instant_speed_wall.sympy,sha256=T-X6mJvX_EGl561sOs_SokoK5gujT6QBWeW8w8uFX8Y,6740
 perfect_physics/data/reverse.wav,sha256=sV2D1c-gppp9B14SMHHQzyTQdHvErChhTbCzCFS2cTk,283896
 perfect_physics/data/stick_cue.wav,sha256=IHtQ0xh9lCTw77UnlMXl9IzLKgkS27olI-E5vY8Axy8,53278
 perfect_physics/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 perfect_physics/tests/test_perfect_physics.py,sha256=9beQyniYwd12yOqmWnzIm2y6mnpEKUOdDfim3dlGyPc,5518
-perfect_physics-0.1.8.dist-info/METADATA,sha256=Lf5zp5m7IjGRIhwRJM1w2gWZ34etFAVxrVLBVgd0js4,1564
-perfect_physics-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-perfect_physics-0.1.8.dist-info/top_level.txt,sha256=YPJm-PTeYqkpkjC02iVbWPmnxXc-ZL8A3-EQtBHNWdY,16
-perfect_physics-0.1.8.dist-info/RECORD,,
+perfect_physics-0.1.9.dist-info/METADATA,sha256=TtWTsgT2fuwGhgdg36gDXhxgiaGz670mdnfTcCW442M,1564
+perfect_physics-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+perfect_physics-0.1.9.dist-info/top_level.txt,sha256=YPJm-PTeYqkpkjC02iVbWPmnxXc-ZL8A3-EQtBHNWdY,16
+perfect_physics-0.1.9.dist-info/RECORD,,
```

