# Comparing `tmp/swiftnav-gnss-0.4.1.tar.gz` & `tmp/swiftnav-gnss-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftnav-gnss-0.4.1.tar", last modified: Mon May  2 18:28:06 2022, max compression
+gzip compressed data, was "swiftnav-gnss-0.5.1.tar", last modified: Tue Apr 25 07:49:15 2023, max compression
```

## Comparing `swiftnav-gnss-0.4.1.tar` & `swiftnav-gnss-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/.github/
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/.github/workflows/
--rw-rw-r--   0 steve     (1000) steve     (1000)      456 2022-05-02 18:27:19.000000 swiftnav-gnss-0.4.1/.github/workflows/ci.yaml
--rw-rw-r--   0 steve     (1000) steve     (1000)     1176 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/.gitignore
--rw-rw-r--   0 steve     (1000) steve     (1000)     1073 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)      510 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     1230 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/README.md
--rw-rw-r--   0 steve     (1000) steve     (1000)     6006 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/asv.conf.json
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/benchmarks/
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/benchmarks/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      296 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/benchmarks/benchmarks.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/gnss/
--rw-rw-r--   0 steve     (1000) steve     (1000)      124 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/gnss/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9481 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/gnss/coord_system.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5985 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/gnss/gps_time.py
--rw-rw-r--   0 steve     (1000) steve     (1000)       67 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)      760 2022-05-02 18:26:27.000000 swiftnav-gnss-0.4.1/setup.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)      510 2022-05-02 18:28:06.000000 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      432 2022-05-02 18:28:06.000000 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-05-02 18:28:06.000000 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       47 2022-05-02 18:28:06.000000 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       16 2022-05-02 18:28:06.000000 swiftnav-gnss-0.4.1/swiftnav_gnss.egg-info/top_level.txt
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-05-02 18:28:06.726084 swiftnav-gnss-0.4.1/tests/
--rw-rw-r--   0 steve     (1000) steve     (1000)     4885 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/tests/test_coord_system.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3112 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/tests/test_gps_time.py
--rw-rw-r--   0 steve     (1000) steve     (1000)       66 2022-04-29 17:28:29.000000 swiftnav-gnss-0.4.1/tox.ini
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.955748 swiftnav-gnss-0.5.1/.github/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.955748 swiftnav-gnss-0.5.1/.github/workflows/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/.github/workflows/ci.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1186 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/.gitignore
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6006 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/asv.conf.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.955748 swiftnav-gnss-0.5.1/benchmarks/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/benchmarks/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      301 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/gnss/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      140 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/gnss/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10019 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/gnss/coord_system.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6608 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/gnss/gps_time.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/gnss/py.typed
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/mypy.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      839 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-04-25 07:49:15.000000 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-04-25 07:49:15.000000 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 07:49:15.000000 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-25 07:49:15.000000 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-04-25 07:49:15.000000 swiftnav-gnss-0.5.1/swiftnav_gnss.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 07:49:15.965748 swiftnav-gnss-0.5.1/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4851 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/tests/test_coord_system.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4256 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/tests/test_gps_time.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      107 2023-04-25 07:42:41.000000 swiftnav-gnss-0.5.1/tox.ini
```

### Comparing `swiftnav-gnss-0.4.1/.gitignore` & `swiftnav-gnss-0.5.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -96,7 +96,9 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # airspeed velocity
 .asv/
+
+.vscode/
```

### Comparing `swiftnav-gnss-0.4.1/LICENSE` & `swiftnav-gnss-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftnav-gnss-0.4.1/README.md` & `swiftnav-gnss-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # PyGNSS
 
 [![Build Status](https://travis-ci.org/swift-nav/pygnss.svg?branch=master)](https://travis-ci.org/swift-nav/pygnss)
 
-`PyGNSS` is a Python library which which provides various GNSS related utilites. `PyGNSS` runs on both Python 2 and 3. The coordinate system transformations are implemented based on the algorithms used by `libswiftnav`.
+`PyGNSS` is a Python library which which provides various GNSS related utilites.  The coordinate system transformations are implemented based on the algorithms used by `libswiftnav`.
 
-
-## Installation 
+## Installation
 
 It is recommended to install `pygnss` in a virtualenv to avoid polluting global system state.
 
 To install the latest version of `pygnss` from git:
 
-` $ pip install 'git+https://github.com/swift-nav/pygnss.git'`
-
+`$ pip install 'git+https://github.com/swift-nav/pygnss.git'`
 
 ## Usage
 
 Currently, `pygnss` provides functions for the following coordinate transformations:
+
 * `llh_from_ecef`
 * `ecef_from_llh`
 * `ned_from_ecef`
 * `azimuth_elevation_from_ecef`
 
-
 ## License
 
 Copyright (C) 2017 Swift Navigation Inc.
 
 Contact: Swift Navigation <dev@swiftnav.com>
 
 This source is subject to the license found in the file 'LICENSE' which must
```

### Comparing `swiftnav-gnss-0.4.1/asv.conf.json` & `swiftnav-gnss-0.5.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `swiftnav-gnss-0.4.1/gnss/coord_system.py` & `swiftnav-gnss-0.5.1/gnss/coord_system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Copyright (C) 2017 Swift Navigation Inc.
-# Contact: Swift Navigation <dev@swiftnav.com> 
+# Contact: Swift Navigation <dev@swiftnav.com>
 # This source is subject to the license found in the file 'LICENSE' which must
 # be be distributed together with this source. All other rights reserved.
 
 
+from typing import List, Tuple, Union
 import numpy as np
+import numpy.typing as npt
 
-WGS84_A = 6378137.0
-WGS84_IF = 298.257223563
-WGS84_F = (1 / WGS84_IF)
-WGS84_E = np.sqrt(2 * WGS84_F - WGS84_F * WGS84_F)
-WGS84_B = (WGS84_A * (1 - WGS84_F))
+ArrayLike = Union[List, Tuple, np.ndarray]
+Coordinate = Tuple[
+    npt.NDArray[np.float_], npt.NDArray[np.float_], npt.NDArray[np.float_]
+]
 
+WGS84_A: float = 6378137.0
+WGS84_IF: float = 298.257223563
+WGS84_F: float = 1 / WGS84_IF
+WGS84_E: float = np.sqrt(2 * WGS84_F - WGS84_F * WGS84_F)
+WGS84_B: float = WGS84_A * (1 - WGS84_F)
 
-def llh_from_ecef(ecef):
+
+def llh_from_ecef(ecef: ArrayLike) -> Coordinate:
     """Convert cartesian ECEF coords to geodetic coordinates.
 
     Converts from WGS84 Earth Centered, Earth Fixed (ECEF) Cartesian
     coordinates (X, Y and Z) into WGS84 geodetic coordinates (latitude,
     longitude and height).
 
 
@@ -47,56 +54,53 @@
     # Coordinates Transformations", Burtch R. R. (2006), American Congress for
     # Surveying and Mapping Annual Conference. Orlando, Florida.  -#
     # "Transformation from Cartesian to Geodetic Coordinates Accelerated by
     # Halleys Method", T. Fukushima (2006), Journal of Geodesy.
 
     x, y, z = ecef
 
-    lat, lon, alt = None, None, None
-
     # Distance from polar axis.
     p = np.linalg.norm((x, y))
 
     # Compute longitude first, this can be done exactly.
-    if p == 0:
-        lon = 0
+    if p == 0.0:
+        lon = np.zeros(np.array(x).shape, float)
     else:
         lon = np.arctan2(y, x)
 
     # If we are close to the pole then convergence is very slow, treat this is
     # a special case.
     if p < WGS84_A * 1e-16:
-        lat = np.copysign(np.pi / 2, z)
+        lat = np.copysign(np.pi / 2.0, z)
         alt = np.fabs(z) - WGS84_B
         return lat, lon, alt
 
     # Caluclate some other constants as defined in the Fukushima paper.
     P = p / WGS84_A
-    e_c = np.sqrt(1 - WGS84_E**2)
+    e_c = np.sqrt(1.0 - WGS84_E**2)
     Z = np.fabs(z) * e_c / WGS84_A
 
     # Initial values for S and C correspond to a zero height solution.
     S = Z
     C = e_c * P
 
     # Neither S nor C can be negative on the first iteration so
     # starting prev = -1 will not cause and early exit.
-    prev_C, prev_S = -1, -1
-    A_n, B_n, D_n, F_n = 0, 0, 0, 0
+    prev_C, prev_S = -1.0, -1.0
+    A_n, B_n, D_n, F_n = 0.0, 0.0, 0.0, 0.0
 
     # Iterate a maximum of 10 times. This should be way more than enough for
     # all sane inputs
     for i in range(10):
         # Calculate some intermmediate variables used in the update step based
         # on the current state.
         A_n = np.sqrt(S * S + C * C)
         D_n = Z * A_n * A_n * A_n + WGS84_E * WGS84_E * S * S * S
         F_n = P * A_n * A_n * A_n - WGS84_E * WGS84_E * C * C * C
-        B_n = 1.5 * WGS84_E * S * C * C * (A_n *
-                                           (P * S - Z * C) - WGS84_E * S * C)
+        B_n = 1.5 * WGS84_E * S * C * C * (A_n * (P * S - Z * C) - WGS84_E * S * C)
 
         # Update step.
         S = D_n * F_n - B_n * S
         C = F_n * F_n - B_n * C
 
         # The original algorithm as presented in the paper by Fukushima has
         # a problem with numerical stability. S and C can grow very large or
@@ -115,37 +119,38 @@
         # ensure that we do not divide by zero as only one of S or C should
         # ever be zero.
         #
         # This incurs an extra division each iteration which the author was
         # explicityl trying to avoid and it may be that this solution is just
         # reverting back to the method of iterating on T directly, perhaps this
         # bears more thought?
-        if (S > C):
+        if S > C:
             C = C / S
-            S = 1
+            S = 1.0
         else:
             S = S / C
-            C = 1
+            C = 1.0
 
         # Check for convergence and exit early if we have converged.
         if np.fabs(S - prev_S) < 1e-16 and np.fabs(C - prev_C) < 1e-16:
             break
         else:
             prev_S = S
             prev_C = C
 
     A_n = np.sqrt(S * S + C * C)
     lat = np.copysign(1.0, ecef[2]) * np.arctan(S / (e_c * C))
-    alt = (p * e_c * C + np.fabs(ecef[2]) * S - WGS84_A * e_c * A_n
-           ) / np.sqrt(e_c * e_c * C * C + S * S)
+    alt = (p * e_c * C + np.fabs(ecef[2]) * S - WGS84_A * e_c * A_n) / np.sqrt(
+        e_c * e_c * C * C + S * S
+    )
 
     return np.rad2deg(lat), np.rad2deg(lon), alt
 
 
-def ecef_from_llh(llh):
+def ecef_from_llh(llh: ArrayLike) -> Coordinate:
     """Convert geodetic LLH coordinates to ECEF coordinates.
 
     Converts from WGS84 geodetic coordinates (latitude, longitude and height)
     into WGS84 Earth Centered, Earth Fixed Cartesian (ECEF) coordinates
     (X, Y and Z).
 
     Parameters
@@ -160,24 +165,24 @@
     """
 
     lat, lon, alt = llh
     lat = np.deg2rad(lat)
     lon = np.deg2rad(lon)
 
     d = WGS84_E * np.sin(lat)
-    N = WGS84_A / np.sqrt(1. - d * d)
+    N = WGS84_A / np.sqrt(1.0 - d * d)
 
     x = (N + alt) * np.cos(lat) * np.cos(lon)
     y = (N + alt) * np.cos(lat) * np.sin(lon)
-    z = ((1 - WGS84_E * WGS84_E) * N + alt) * np.sin(lat)
+    z = ((1.0 - WGS84_E * WGS84_E) * N + alt) * np.sin(lat)
 
     return x, y, z
 
 
-def ecef_to_ned_matrix(ref_ecef):
+def ecef_to_ned_matrix(ref_ecef: ArrayLike) -> npt.NDArray[np.float_]:
     """Populates a provided 3x3 matrix with the appropriate rotation
     matrix to transform from ECEF to NED coordinates, given the
     provided ECEF reference vector.
     """
     M = np.empty([3, 3])
     llh = np.array(llh_from_ecef(ref_ecef))
 
@@ -198,21 +203,24 @@
     M[2][0] = -cos_lat * cos_lon
     M[2][1] = -cos_lat * sin_lon
     M[2][2] = -sin_lat
 
     return M
 
 
-def ned_from_ecef(ecef_vector, reference_location):
-    """Convert ECEF coordinates into NED frame of given reference.
-    """
+def ned_from_ecef(
+    ecef_vector: ArrayLike, reference_location: ArrayLike
+) -> npt.NDArray[np.float_]:
+    """Convert ECEF coordinates into NED frame of given reference."""
     return np.dot(ecef_to_ned_matrix(reference_location), ecef_vector)
 
 
-def relative_position_in_ned(ecef_target, ecef_reference):
+def relative_position_in_ned(
+    ecef_target: ArrayLike, ecef_reference: ArrayLike
+) -> npt.NDArray[np.float_]:
     """Returns the vector between two ECEF points in the NED frame of the
     reference.
 
     Parameters
     ----------
     ecef_target : array-like length 3
         A length three vector which corresponds to the target position,
@@ -225,18 +233,22 @@
     -------
     ned : array-like
         A length three vector which points from reference to target in the
         north/east/down reference frame centered at the reference position.
     """
     ecef_target = np.asarray(ecef_target)
     ecef_reference = np.asarray(ecef_reference)
-    return ned_from_ecef((ecef_target - ecef_reference), ecef_reference)
+    return ned_from_ecef(
+        np.transpose(np.transpose(ecef_target) - ecef_reference), ecef_reference
+    )
 
 
-def azimuth_elevation_from_ecef(ecef_target, ecef_reference):
+def azimuth_elevation_from_ecef(
+    ecef_target: ArrayLike, ecef_reference: ArrayLike
+) -> Tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
     """Returns the azimuth and elevation of a vector pointing from `ref_position`
     to `position` where both are given in ECEF
 
     Parameters
     ----------
     pos : array-like length 3
         The position in ECEF of the end point of the vector.  Typically
@@ -258,11 +270,11 @@
     ecef_target = np.asarray(ecef_target)
     ecef_reference = np.asarray(ecef_reference)
     # Calculate the vector from the reference point in the local North, East,
     # Down frame of the reference point. */
     ned = relative_position_in_ned(ecef_target, ecef_reference)
     # atan2 returns angle in range [-pi, pi], usually azimuth is defined in the
     # range [0, 2pi]. */
-    azimuth = np.mod(np.arctan2(ned[1], ned[0]), 2 * np.pi)
-    elevation = np.arcsin(-ned[2] / np.linalg.norm(ned))
+    azimuth = np.mod(np.arctan2(ned[1], ned[0]), 2.0 * np.pi)
+    elevation = np.arcsin(-ned[2] / np.linalg.norm(ned, axis=0))
 
     return np.rad2deg(azimuth), np.rad2deg(elevation)
```

### Comparing `swiftnav-gnss-0.4.1/gnss/gps_time.py` & `swiftnav-gnss-0.5.1/gnss/gps_time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,72 @@
+# type: ignore
 # Copyright (C) 2018 Swift Navigation Inc.
 # Contact: Swift Navigation <dev@swiftnav.com>
 # This source is subject to the license found in the file 'LICENSE' which must
 # be be distributed together with this source. All other rights reserved.
 
+from datetime import datetime
+
 import numpy as np
 import pandas as pd
 
 WEEK_SECS = 7 * 24 * 60 * 60
-GPS_WEEK_0 = np.datetime64('1980-01-06T00:00:00Z', 'ns')
+GPS_WEEK_0 = np.datetime64("1980-01-06T00:00:00", "ns")
+LEAP_SECOND_DATES = [
+    np.datetime64("1981-07-01T00:00:00", "ns"),
+    np.datetime64("1982-07-01T00:00:00", "ns"),
+    np.datetime64("1983-07-01T00:00:00", "ns"),
+    np.datetime64("1985-07-01T00:00:00", "ns"),
+    np.datetime64("1988-01-01T00:00:00", "ns"),
+    np.datetime64("1990-01-01T00:00:00", "ns"),
+    np.datetime64("1991-01-01T00:00:00", "ns"),
+    np.datetime64("1992-07-01T00:00:00", "ns"),
+    np.datetime64("1993-07-01T00:00:00", "ns"),
+    np.datetime64("1994-07-01T00:00:00", "ns"),
+    np.datetime64("1996-01-01T00:00:00", "ns"),
+    np.datetime64("1997-07-01T00:00:00", "ns"),
+    np.datetime64("1999-01-01T00:00:00", "ns"),
+    np.datetime64("2006-01-01T00:00:00", "ns"),
+    np.datetime64("2009-01-01T00:00:00", "ns"),
+    np.datetime64("2012-07-01T00:00:00", "ns"),
+    np.datetime64("2015-07-01T00:00:00", "ns"),
+    np.datetime64("2017-01-01T00:00:00", "ns"),
+]
 
 
 def gps_format_to_datetime(wn, tow):
     """
     Converts a time using week number and time of week representation
     into a python datetime object.  Note that this does NOT convert
     into UTC.  The resulting datetime object is still in GPS time
     and will have been rounded to nanosecond precision (which is
     too coarse to accurately compute timedeltas such as time of
-    flight.
+    flight).
 
     Parameters
     -----------
     wn : int
-      An integer corresponding to the week number of a time.
+      An integer (or array) corresponding to the week number of a time.
     tow : float
-      A float corresponding to the time of week (in seconds) from
-      the beginning of the week number (wn).
+      A float (or array) corresponding to the time of week (in seconds) from the
+      beginning of the week number (wn).
 
     Returns
     -------
-    utc : np.datetime64
-      Returns a np.datetime64 object (or an array of them) that holds
+    utc : pd.Timestamp
+      Returns a pd.Timestamp object (or an array of them) that holds
       the UTC representation of the corresponding gpst.
 
-    See also: gpst_to_utc, datetime_to_tow
+    See also: gpst_to_utc
     """
-    seconds = pd.to_timedelta(tow, 's')
-    weeks = pd.to_timedelta(np.array(wn) * WEEK_SECS, 's')
+    seconds = pd.to_timedelta(tow, "s")
+    weeks = pd.to_timedelta(np.array(wn) * WEEK_SECS, "s")
     return GPS_WEEK_0 + weeks + seconds
 
+
 def datetime_to_gps_format(t):
     """
     Converts from a datetime to week number and time of week format.
     NOTE: This does NOT convert between utc and gps time.  The result
     will still be in gps time (so will be off by some number of
     leap seconds).
 
@@ -54,60 +78,53 @@
       for more details).
 
     Returns
     --------
     wn_tow : dict
       Dictionary with attributes 'wn' and 'tow' corresponding to the
       week number and time of week.
-
-    See also: tow_to_datetime
     """
     t = pd.to_datetime(t)
-    delta = (t - GPS_WEEK_0)
+    delta = t - GPS_WEEK_0
     # compute week number
-    wn = np.floor(delta.total_seconds() / WEEK_SECS).astype('int64')
+    wn = np.floor(delta.total_seconds() / WEEK_SECS).astype("int64")
     # subtract the whole weeks from timedelta and get the remaining seconds
-    delta -= pd.to_timedelta(wn * WEEK_SECS, 's')
+    delta -= pd.to_timedelta(wn * WEEK_SECS, "s")
     seconds = delta.total_seconds()
-    return {'wn': wn, 'tow': seconds}
+    return {"wn": wn, "tow": seconds}
 
 
 def gps_minus_utc_seconds(gpst):
     """
     Returns current number of leap seconds between GPS time and UTC time.
 
     UTC leap second is added between 23:59:59 and 00:00:00 in UTC time.
     This function's input is gps time so the time offset changes e.g.
     between 00:00:16 and 00:00:17 in GPS time.
 
-    Supports dates from 1th Jul 2012.
-
     Parameters
     ----------
     gpst : np.datetime64, pd.Timestamp, datetime.datetime
       A datetime object (possibly an array) that is convertable to
       datetime64 objects using pd.to_datetime (see the pandas docs
       for more details) in GPS time.
 
     Returns
     -------
-    utc : float
+    utc : int
       Returns the number (or an array of them) of leap second values.
     """
 
-    delta_utc = np.zeros(gpst.shape, np.int)
-    delta_utc = np.array(delta_utc)
-    assert np.all(gpst >= np.datetime64('1999-01-01T00:00:13Z'))
-    # difference was 16 seconds on 1st July 2012, add the leap seconds since that
-    delta_utc += 13
-    delta_utc[gpst >= np.datetime64('2005-01-01T00:00:13Z')] += 1
-    delta_utc[gpst >= np.datetime64('2008-01-01T00:00:14Z')] += 1
-    delta_utc[gpst >= np.datetime64('2012-07-01T00:00:15Z')] += 1
-    delta_utc[gpst >= np.datetime64('2015-07-01T00:00:16Z')] += 1
-    delta_utc[gpst >= np.datetime64('2017-01-01T00:00:17Z')] += 1
+    delta_utc = np.zeros_like(gpst, int)
+    if isinstance(gpst, datetime):
+        gpst = np.datetime64(gpst)
+
+    for i, date in enumerate(LEAP_SECOND_DATES):
+        delta_utc[gpst >= (date + np.timedelta64(i, "s"))] += 1
+
     return delta_utc
 
 
 def gpst_to_utc(gpst):
     """
     Convert a GPS time either in datetime or week number, time of week
     format into UTC.
@@ -127,19 +144,23 @@
     Returns
     -------
     utc : np.datetime64
       Returns a np.datetime64 object (or an array of them) that holds
       the UTC representation of the corresponding gpst.
 
     """
+    if isinstance(gpst, dict):
+        gpst = gps_format_to_datetime(gpst["wn"], gpst["tow"])
+
+    gpst = pd.to_datetime(gpst)
     delta_utc = gps_minus_utc_seconds(gpst)
     delta_utc = np.asarray(delta_utc)
 
     # now subtract out the delta_utc value (which is given in float seconds)
-    return gpst - (delta_utc * 1e9).astype('timedelta64[ns]')
+    return gpst - (delta_utc * 1e9).astype("timedelta64[ns]")
 
 
 def utc_to_gpst(utc):
     """
     Converts from times in utc to the corresponding gps time in
     week number, time of week format.
 
@@ -156,18 +177,19 @@
 
     Returns
     -------
     gpst : dict
       A dictionary with attributes 'wn' and 'tow' holding the
       week number and time of week that correspond to the input utc times.
 
-    See also: datetime_to_tow, gpst_to_utc
+    See also: gpst_to_utc
     """
     # GPS-UTC offset is defined in GPS time, so some iteration is needed
+
     delta_utc_tmp = gps_minus_utc_seconds(utc)
     delta_utc_tmp = np.array(delta_utc_tmp)
-    gpst = utc + ((delta_utc_tmp) * 1e9).astype('timedelta64[ns]')
+    utc = pd.to_datetime(utc)
+    gpst = utc + ((delta_utc_tmp) * 1e9).astype("timedelta64[ns]")
 
     delta_utc = gps_minus_utc_seconds(gpst)
     delta_utc = np.array(delta_utc)
-    utc = pd.to_datetime(utc)
-    return datetime_to_gps_format(utc + (delta_utc * 1e9).astype('timedelta64[ns]'))
+    return datetime_to_gps_format(utc + (delta_utc * 1e9).astype("timedelta64[ns]"))
```

### Comparing `swiftnav-gnss-0.4.1/tests/test_coord_system.py` & `swiftnav-gnss-0.5.1/tests/test_coord_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,22 @@
     ((0, 180, 0), (-EARTH_A, 0, 0)),  # On the Equator
     ((0, 90, 0), (0, EARTH_A, 0)),  # On the Equator
     ((0, -90, 0), (0, -EARTH_A, 0)),  # On the Equator
     ((90, 0, 0), (0, 0, EARTH_B)),  # North Pole
     ((-90, 0, 0), (0, 0, -EARTH_B)),  # South Pole
     ((90, 0, 22), (0, 0, EARTH_B + 22)),  # 22m above north pole
     ((-90, 0, 22), (0, 0, -(EARTH_B + 22))),  # 22m above south pole
-    ((0, 0, 22), (EARTH_A + 22, 0, 0)),  # 22m above the equator end prime meridian
+    # 22m above the equator end prime meridian
+    ((0, 0, 22), (EARTH_A + 22, 0, 0)),
     ((0, 180, 22), (-(EARTH_A + 22), 0, 0)),  # 22m above the equator
     ((38, 122, 0), (-2666781.2433701, 4267742.1051642, 3905443.968419)),
 ]
 
 approx_dist = partial(approx, abs=1e-6)
-approx_deg = partial(approx, abs=np.deg2rad(1e-7/3600))
+approx_deg = partial(approx, abs=np.deg2rad(1e-7 / 3600))
 
 
 def llh_isclose(a, b):
     assert a[:2] == approx_deg(a[:2])
     assert a[2] == approx_dist(a[2])
 
 
@@ -54,57 +55,78 @@
 
 @given(st.tuples(lat_rad, lon_rad, alt_m))
 def test_llh_ecef_roundtrip(x):
     llh_isclose(cs.llh_from_ecef(cs.ecef_from_llh(x)), x)
 
 
 # generate coordinates outside a 800km sphere from the center of the earth
-st_ecef = st.floats(min_value=800*1000, max_value=4*EARTH_A) | st.floats(
-    min_value=-4*EARTH_A, max_value=-800*1000)
+st_ecef = st.floats(min_value=800 * 1000, max_value=4 * EARTH_A) | st.floats(
+    min_value=-4 * EARTH_A, max_value=-800 * 1000
+)
 
 
 @given(st.tuples(st_ecef, st_ecef, st_ecef))
 def test_ecef_llh_roundtrip(x):
     assert cs.ecef_from_llh(cs.llh_from_ecef(x)) == approx_dist(x)
 
 
-@pytest.mark.parametrize("vector,reference,expected",
-                         # this vector should be directly above the reference point so
-                         # we expect the north and east components to be zero and the down
-                         # component to be -1.
-                         [((1., 0, 0), (EARTH_A, 0, 0), (0., 0., -1.)),
-                          # Here the vector should be pointing due east, there may be
-                          # some second order error which translate into the down
-                          # component, hence the small magnitude.
-                          ((0., 0.01, 0.), (EARTH_A, 0, 0), (0., 0.01, 0)),
-                          # Here the vector should be pointing due east, there may be
-                          # some second order error which translate into the down
-                          # component, hence the small magnitude.
-                          ((0., 0., 0.01), (EARTH_A, 0, 0), (0.01, 0., 0.)),
-                          # Now try a spot check with angles
-                          ((1, 1, 1), (2, 2, 2), (1.13204490e-01, 1.11022302e-16, -1.72834740e+00))
-                         ])
+@pytest.mark.parametrize(
+    "vector,reference,expected",
+    # this vector should be directly above the reference point so
+    # we expect the north and east components to be zero and the down
+    # component to be -1.
+    [
+        ((1.0, 0, 0), (EARTH_A, 0, 0), (0.0, 0.0, -1.0)),
+        # Here the vector should be pointing due east, there may be
+        # some second order error which translate into the down
+        # component, hence the small magnitude.
+        ((0.0, 0.01, 0.0), (EARTH_A, 0, 0), (0.0, 0.01, 0)),
+        # Here the vector should be pointing due east, there may be
+        # some second order error which translate into the down
+        # component, hence the small magnitude.
+        ((0.0, 0.0, 0.01), (EARTH_A, 0, 0), (0.01, 0.0, 0.0)),
+        # Now try a spot check with angles
+        ((1, 1, 1), (2, 2, 2), (1.13204490e-01, 1.11022302e-16, -1.72834740e00)),
+    ],
+)
 def test_ned_from_ecef(vector, reference, expected):
     actual = cs.ned_from_ecef(vector, reference)
     assert actual == approx(expected)
 
 
-@pytest.mark.parametrize("target,reference,expected",
-                         # Here we place a target directly above the reference in
-                         # which case the elevation should be 90
-                         [((EARTH_A + SAT_ALTITUDE, 0, 0), (EARTH_A, 0, 0), (0., 90.)),
-                          # Satellite is directly East of the reference
-                          ((EARTH_A, SAT_ALTITUDE, 0), (EARTH_A, 0, 0), (90., 0.)),
-                          # Satellite is directly North of the reference
-                          ((EARTH_A, 0, SAT_ALTITUDE), (EARTH_A, 0, 0), (0., 0.)),
-                          # Satellite is east at elevation angle of 45.
-                          ((EARTH_A + SAT_ALTITUDE, 0, SAT_ALTITUDE), (EARTH_A, 0, 0), (0., 45.)),
-                          # Satellite is north east at elevation angle of tan^-1(1, sqrt(2))
-                          ((EARTH_A + SAT_ALTITUDE, SAT_ALTITUDE, SAT_ALTITUDE),
-                           (EARTH_A, 0, 0),
-                           (45., np.rad2deg(np.arctan2(1., np.sqrt(2))))),
-                         ])
+@pytest.mark.parametrize(
+    "target,reference,expected",
+    # Here we place a target directly above the reference in
+    # which case the elevation should be 90
+    [
+        ((EARTH_A + SAT_ALTITUDE, 0, 0), (EARTH_A, 0, 0), (0.0, 90.0)),
+        # Satellite is directly East of the reference
+        ((EARTH_A, SAT_ALTITUDE, 0), (EARTH_A, 0, 0), (90.0, 0.0)),
+        # Satellite is directly North of the reference
+        ((EARTH_A, 0, SAT_ALTITUDE), (EARTH_A, 0, 0), (0.0, 0.0)),
+        # Satellite is east at elevation angle of 45.
+        ((EARTH_A + SAT_ALTITUDE, 0, SAT_ALTITUDE), (EARTH_A, 0, 0), (0.0, 45.0)),
+        # Satellite is north east at elevation angle of tan^-1(1, sqrt(2))
+        (
+            (EARTH_A + SAT_ALTITUDE, SAT_ALTITUDE, SAT_ALTITUDE),
+            (EARTH_A, 0, 0),
+            (45.0, np.rad2deg(np.arctan2(1.0, np.sqrt(2)))),
+        ),
+    ],
+)
 def test_azimuth_elevation_from_ecef(target, reference, expected):
     azimuth, elevation = cs.azimuth_elevation_from_ecef(target, reference)
     assert azimuth == approx(expected[0])
     assert elevation == approx(expected[1])
-    
+
+
+def test_azimuth_elevation_from_ecef_vec():
+    target = (
+        [EARTH_A + SAT_ALTITUDE, EARTH_A, EARTH_A],
+        [0, SAT_ALTITUDE, 0],
+        [0, 0, SAT_ALTITUDE],
+    )
+    reference = (EARTH_A, 0, 0)
+    expected = ([0.0, 90.0, 0.0], [90.0, 0.0, 0.0])
+    azimuth, elevation = cs.azimuth_elevation_from_ecef(target, reference)
+    assert azimuth == approx(expected[0])
+    assert elevation == approx(expected[1])
```

