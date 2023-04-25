# Comparing `tmp/led_calibration_plugin-1.2.0-py3-none-any.whl.zip` & `tmp/led_calibration_plugin-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10917 bytes, number of entries: 11
+Zip file size: 10916 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      258 b- defN 23-Apr-09 00:02 led_calibration_plugin/__init__.py
 -rw-r--r--  2.0 unx     4163 b- defN 22-Nov-02 00:25 led_calibration_plugin/calibrated_light_dark_cycle.py
 -rw-r--r--  2.0 unx    12926 b- defN 23-Mar-31 00:07 led_calibration_plugin/led_calibration.py
 -rw-r--r--  2.0 unx     6885 b- defN 23-Mar-30 23:51 led_calibration_plugin/test_led_calibration.py
--rw-r--r--  2.0 unx      518 b- defN 22-Nov-02 00:06 led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml
--rw-r--r--  2.0 unx     1062 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4152 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1115 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/RECORD
-11 files, 31263 bytes uncompressed, 8961 bytes compressed:  71.3%
+-rw-r--r--  2.0 unx      533 b- defN 23-Apr-23 00:47 led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml
+-rw-r--r--  2.0 unx     1062 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4152 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Apr-25 02:18 led_calibration_plugin-1.2.1.dist-info/RECORD
+11 files, 31278 bytes uncompressed, 8960 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: led_calibration_plugin/test_led_calibration.py
 Comment: 
 
 Filename: led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/LICENSE.txt
+Filename: led_calibration_plugin-1.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/METADATA
+Filename: led_calibration_plugin-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/WHEEL
+Filename: led_calibration_plugin-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/entry_points.txt
+Filename: led_calibration_plugin-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/top_level.txt
+Filename: led_calibration_plugin-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.2.0.dist-info/RECORD
+Filename: led_calibration_plugin-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml

```diff
@@ -5,14 +5,15 @@
 description: Turns on a 16h:8h light/dark cycle based on LED calibrations.
 fields:
   - key: duration
     default: 60
     unit: min
     label: Duration between checks
   - key: light_intensity
+    default: 0
     unit: AU
     label: Light intensity
   - key: light_duration_hours
     default: 16
     unit: h
     label: Light duration
   - key: dark_duration_hours
```

## Comparing `led_calibration_plugin-1.2.0.dist-info/LICENSE.txt` & `led_calibration_plugin-1.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `led_calibration_plugin-1.2.0.dist-info/METADATA` & `led_calibration_plugin-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: led-calibration-plugin
-Version: 1.2.0
+Version: 1.2.1
 Summary: Calibrate your LEDs using an external light probe.
 Home-page: https://github.com/pioreactor/pioreactor-led-calibration-plugin
 Author: Kelly Tran, Cameron Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `led_calibration_plugin-1.2.0.dist-info/RECORD` & `led_calibration_plugin-1.2.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 led_calibration_plugin/__init__.py,sha256=S8sdwK13ZJvxnOuaAd1u5YIF_jbPK2FeubcDgN3QEvE,258
 led_calibration_plugin/calibrated_light_dark_cycle.py,sha256=KSYmATQIqEuER7LdfohnLX2Bwk2XNJsGoZz0Vc5ywv4,4163
 led_calibration_plugin/led_calibration.py,sha256=nOLAQil4hK3jsgmkRxY389K3uTBuVVbrR-tH_KPLdzA,12926
 led_calibration_plugin/test_led_calibration.py,sha256=J2CqdM3SVxWQWzJBIOJHZ5xzU1X7E392XQ4rBrXuWSw,6885
-led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml,sha256=cmo03wMtqB7wKY6X3tevSl6KjUhRqLPEAjd5PtFppnI,518
-led_calibration_plugin-1.2.0.dist-info/LICENSE.txt,sha256=ipJf_7c1vobIyTbjJZBpBepQJtAIu2fAxMOP9SYjWps,1062
-led_calibration_plugin-1.2.0.dist-info/METADATA,sha256=YPTfFEYCCQc759TJmj2hEqrImH7hEbC3kPd_d56lbPY,4152
-led_calibration_plugin-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-led_calibration_plugin-1.2.0.dist-info/entry_points.txt,sha256=jjNBY8vhrvrlCrCQzmVlSzxqrbjlFT5oxqInfPF27rk,69
-led_calibration_plugin-1.2.0.dist-info/top_level.txt,sha256=aG26kKd4yawYfIL4rWWdKgkH6yv-VPTne3ld2CueFSQ,23
-led_calibration_plugin-1.2.0.dist-info/RECORD,,
+led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml,sha256=o8CaY_O52jjmW4zY5pQStf6qpweRxpbbPCdIbOhO2bc,533
+led_calibration_plugin-1.2.1.dist-info/LICENSE.txt,sha256=ipJf_7c1vobIyTbjJZBpBepQJtAIu2fAxMOP9SYjWps,1062
+led_calibration_plugin-1.2.1.dist-info/METADATA,sha256=QMn3tUzpPowoSnfJx003ZlrmsH8O9iWYJC9g-X06hNU,4152
+led_calibration_plugin-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+led_calibration_plugin-1.2.1.dist-info/entry_points.txt,sha256=jjNBY8vhrvrlCrCQzmVlSzxqrbjlFT5oxqInfPF27rk,69
+led_calibration_plugin-1.2.1.dist-info/top_level.txt,sha256=aG26kKd4yawYfIL4rWWdKgkH6yv-VPTne3ld2CueFSQ,23
+led_calibration_plugin-1.2.1.dist-info/RECORD,,
```

