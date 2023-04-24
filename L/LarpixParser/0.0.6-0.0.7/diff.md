# Comparing `tmp/LarpixParser-0.0.6.tar.gz` & `tmp/LarpixParser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LarpixParser-0.0.6.tar", last modified: Fri Apr  7 22:30:41 2023, max compression
+gzip compressed data, was "LarpixParser-0.0.7.tar", last modified: Mon Apr 24 23:01:34 2023, max compression
```

## Comparing `LarpixParser-0.0.6.tar` & `LarpixParser-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.974114 LarpixParser-0.0.6/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-04-07 06:11:46.000000 LarpixParser-0.0.6/LICENSE
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-07 22:30:41.970838 LarpixParser-0.0.6/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-04-07 06:11:46.000000 LarpixParser-0.0.6/README.md
--rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-04-07 22:30:41.972189 LarpixParser-0.0.6/setup.cfg
--rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-04-07 22:28:03.000000 LarpixParser-0.0.6/setup.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:40.522206 LarpixParser-0.0.6/src/
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.072965 LarpixParser-0.0.6/src/LarpixParser/
--rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/__init__.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/charge_calibration.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.625224 LarpixParser-0.0.6/src/LarpixParser/config_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1696 2023-04-07 21:59:13.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/2x2.yaml
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.840979 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/module0.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3851 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/ndlar-module.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/coord_transform.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1517 2023-04-07 22:23:31.000000 LarpixParser-0.0.6/src/LarpixParser/event_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/geom_to_dict.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_charge.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1986 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_raw_coord.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_vdrift.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/hit_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/units.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3737 2023-04-07 21:58:17.000000 LarpixParser-0.0.6/src/LarpixParser/util.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.296863 LarpixParser-0.0.6/src/LarpixParser.egg-info/
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/SOURCES.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/dependency_links.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/requires.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/top_level.txt
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.410316 LarpixParser-0.0.7/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/LICENSE
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-24 23:01:34.407021 LarpixParser-0.0.7/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/README.md
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-04-24 23:01:34.408553 LarpixParser-0.0.7/setup.cfg
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-04-24 22:59:56.000000 LarpixParser-0.0.7/setup.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.090033 LarpixParser-0.0.7/src/
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.116098 LarpixParser-0.0.7/src/LarpixParser/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/__init__.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/charge_calibration.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.245092 LarpixParser-0.0.7/src/LarpixParser/config_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1682 2023-04-24 21:06:45.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/2x2.yaml
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.267162 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/module0.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3880 2023-04-24 21:07:29.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/ndlar-module.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/coord_transform.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1847 2023-04-24 21:05:25.000000 LarpixParser-0.0.7/src/LarpixParser/event_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/geom_to_dict.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/get_charge.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1963 2023-04-24 21:44:16.000000 LarpixParser-0.0.7/src/LarpixParser/get_raw_coord.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/get_vdrift.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/hit_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/units.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3729 2023-04-24 21:06:21.000000 LarpixParser-0.0.7/src/LarpixParser/util.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.130975 LarpixParser-0.0.7/src/LarpixParser.egg-info/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/SOURCES.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/dependency_links.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/requires.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/top_level.txt
```

### Comparing `LarpixParser-0.0.6/LICENSE` & `LarpixParser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/PKG-INFO` & `LarpixParser-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.6/README.md` & `LarpixParser-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/setup.py` & `LarpixParser-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import setuptools
 
-VER = "0.0.6"
+VER = "0.0.7"
 
 setuptools.setup(
     name="LarpixParser",
     version=VER,
     author="Yifan C. and others",
     author_email="cyifan@slac.stanford.edu",
     description="A package parsing the larpix output to hit-level",
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser/charge_calibration.py` & `LarpixParser-0.0.7/src/LarpixParser/charge_calibration.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/2x2.yaml` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/2x2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,10 @@
   - [[16,14,12,10],[15,13,11,9]]
 module_to_io_groups:
   1: [1, 2]
   2: [3, 4]
   3: [5, 6]
   4: [7, 8]
 
-ifspill: True
 spill_spacing: 1.2e6          # microseconds
 beam_duration: 10             # microseconds
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/module0.yaml` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/module0.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/config_repo/ndlar-module.yaml` & `LarpixParser-0.0.7/src/LarpixParser/config_repo/ndlar-module.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -116,9 +116,9 @@
   33: [129, 130, 131, 132]
   34: [133, 134, 135, 136]
   35: [137, 138, 139, 140]
 
 
 module_to_tpcs: {0: [0, 1], 1: [2, 3], 2: [4, 5], 3: [6, 7], 4: [8, 9], 5: [10, 11], 6: [12, 13], 7: [14, 15], 8: [16, 17], 9: [18, 19], 10: [20, 21], 11: [22, 23], 12: [24, 25], 13: [26, 27], 14: [28, 29], 15: [30, 31], 16: [32, 33], 17: [34, 35], 18: [36, 37], 19: [38, 39], 20: [40, 41], 21: [42, 43], 22: [44, 45], 23: [46, 47], 24: [48, 49], 25: [50, 51], 26: [52, 53], 27: [54, 55], 28: [56, 57], 29: [58, 59], 30: [60, 61], 31: [62, 63], 32: [64, 65], 33: [66, 67], 34: [68, 69]}
 
-ifspill: False
 spill_spacing: 1.2e6          # microseconds
+beam_duration: 5             # microseconds
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser/event_parser.py` & `LarpixParser-0.0.7/src/LarpixParser/event_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 import numpy as np
 from sklearn.cluster import DBSCAN
 
-# still need to check what to do with non-beam simulation
-
-def get_t0(packets):
+def get_t0(packets, run_config):
 
     t0 = []
     pckts_t0 = packets[packets['packet_type'] == 7]['timestamp'] # external trigger # by default larnd-sim fills external trigger for each event
 
     pckts_t0_db = pckts_t0.reshape(-1,1)
 
     db = DBSCAN(eps=50, min_samples=2).fit(pckts_t0_db)
     labels = db.labels_
     n_clusters_ = len(set(labels)) - (1 if -1 in labels else 0)
     for i_ct in range(n_clusters_):
         ct_mask = labels == i_ct
-        t0.append(np.min(pckts_t0[ct_mask]))
+        t0.append(np.min(pckts_t0[ct_mask]) * run_config['CLOCK_CYCLE'])
+
+    t0 = np.array(t0)
+
+    threshold = 40 #us
+    t0_ev = np.delete(t0, np.argwhere(np.ediff1d(t0) <= threshold) + 1)
+
+    return t0_ev
+
+def get_t0_event(vertices, run_config, time_parser='t_event'):
+    try:
+        dt_window = run_config['beam_duration']
+    except:
+        dt_window = 0
+        print("Found no 'beam_duration' in the configuration file")
 
-    return np.array(t0)
+    if time_parser in vertices.dtype.names and not (np.all(vertices[time_parser]) == 0):
+        t0_ev = (np.unique(vertices[time_parser]) + dt_window *0.5)
+    else:
+        raise ValueError("True event time is not given!")
 
-def get_t0_spill(vertices, run_config):
-    dt_beam = run_config['beam_duration']
-    return (np.unique(vertices['t_spill']) + dt_beam *0.5) * 10
+    return t0_ev
 
-def packet_to_eventid(assn, tracks, ifspill):
+def packet_to_eventid(assn, tracks, event_parser='eventID'):
     '''
     Assoiciate packet to eventID.
     
     Arguments
     ---------
     assn : array_like
         packet to track association (`mc_packets_assn`) from `larnd-sim` output
@@ -42,13 +55,10 @@
         `len(event_ids)` equals to `len(packets)`
     '''
     track_ids = assn['track_ids'].max(axis=-1)
 
     event_ids = np.full_like(track_ids, -1, dtype=int)
     mask = track_ids != -1
 
-    if not ifspill:
-        event_ids[mask] = tracks['eventID'][track_ids[mask]]
-    if ifspill:
-        event_ids[mask] = tracks['spillID'][track_ids[mask]]
+    event_ids[mask] = tracks[event_parser][track_ids[mask]]
         
     return event_ids
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser/geom_to_dict.py` & `LarpixParser-0.0.7/src/LarpixParser/geom_to_dict.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/get_charge.py` & `LarpixParser-0.0.7/src/LarpixParser/get_charge.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/get_raw_coord.py` & `LarpixParser-0.0.7/src/LarpixParser/get_raw_coord.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,16 @@
         z.append(xyz[2] + z_offset)
         direction.append(xyz[3])
  
     return x, y, z, direction
 
 def get_t_drift(t0, packets_arr, run_config):
 
-    t = packets_arr['timestamp'].astype(float)
-    t_drift = t - t0 # ticks, 0.1us
-    t_drift *= run_config['CLOCK_CYCLE']
+    t = packets_arr['timestamp'].astype(float) * run_config['CLOCK_CYCLE']
+    t_drift = t - t0 # us
 
     return t_drift
 
 
 def get_hit3D_position_tdrift(t0,  packets, packets_arr, geom_dict, run_config, **kwargs):
 
     x, y, z_anode, direction = get_pixel_plane_position(packets_arr, geom_dict, run_config)
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser/get_vdrift.py` & `LarpixParser-0.0.7/src/LarpixParser/get_vdrift.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/hit_parser.py` & `LarpixParser-0.0.7/src/LarpixParser/hit_parser.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/units.py` & `LarpixParser-0.0.7/src/LarpixParser/units.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.6/src/LarpixParser/util.py` & `LarpixParser-0.0.7/src/LarpixParser/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     run_config['birks_Ab'] = run_yaml['birks_Ab'] 
     run_config['birks_kb'] = run_yaml['birks_kb'] 
 
     run_config['W_ion'] = run_yaml['W_ion'] #MeV
 
     run_config['lifetime'] = run_yaml['lifetime'] #us
 
-    run_config['ifspill'] = run_yaml['ifspill']
-    run_config['beam_duration'] = run_yaml['beam_duration'] #us
+    if 'beam_duration' in run_yaml:
+        run_config['beam_duration'] = run_yaml['beam_duration'] #us
 
     return run_config
 
 def configuration_keywords():
     return ['module0','2x2','ndlar']
 
 def detector_configuration(detector):
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser.egg-info/PKG-INFO` & `LarpixParser-0.0.7/src/LarpixParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.6/src/LarpixParser.egg-info/SOURCES.txt` & `LarpixParser-0.0.7/src/LarpixParser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

