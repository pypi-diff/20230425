# Comparing `tmp/mflike-0.8.2.tar.gz` & `tmp/mflike-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflike-0.8.2.tar", last modified: Wed Mar 15 12:45:12 2023, max compression
+gzip compressed data, was "mflike-0.8.3.tar", last modified: Tue Apr 25 08:52:52 2023, max compression
```

## Comparing `mflike-0.8.2.tar` & `mflike-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:45:12.748067 mflike-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-15 12:45:06.000000 mflike-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-15 12:45:06.000000 mflike-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-15 12:45:12.752067 mflike-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-03-15 12:45:06.000000 mflike-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:45:12.752067 mflike-0.8.2/mflike/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-03-15 12:45:06.000000 mflike-0.8.2/mflike/MFLike.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-15 12:45:06.000000 mflike-0.8.2/mflike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-15 12:45:12.752067 mflike-0.8.2/mflike/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-03-15 12:45:06.000000 mflike-0.8.2/mflike/mflike.py
--rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-03-15 12:45:06.000000 mflike-0.8.2/mflike/theoryforge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:45:12.748067 mflike-0.8.2/mflike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 12:45:12.000000 mflike-0.8.2/mflike.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-15 12:45:12.752067 mflike-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-15 12:45:06.000000 mflike-0.8.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-15 12:45:06.000000 mflike-0.8.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-25 08:52:49.000000 mflike-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 08:52:49.000000 mflike-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-25 08:52:52.383547 mflike-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-25 08:52:49.000000 mflike-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/MFLike.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/mflike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/theoryforge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 08:52:52.383547 mflike-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 08:52:49.000000 mflike-0.8.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:52:49.000000 mflike-0.8.3/versioneer.py
```

### Comparing `mflike-0.8.2/LICENSE` & `mflike-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mflike-0.8.2/PKG-INFO` & `mflike-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.2
+Version: 0.8.3
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mflike-0.8.2/README.rst` & `mflike-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `mflike-0.8.2/mflike/MFLike.yaml` & `mflike-0.8.3/mflike/MFLike.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # Specify default set of spectra and scale cuts
 # to be used
 defaults:
   # Which spectra?
   polarizations: [TT, TE, ET, EE]
   # Scale cuts (in ell) for each spectrum
   scales:
-    TT: [2, 5000]
-    TE: [2, 5000]
-    ET: [2, 5000]
-    EE: [2, 5000]
+    TT: [50, 5000]
+    TE: [50, 5000]
+    ET: [50, 5000]
+    EE: [50, 5000]
   # If True, TE' = (TE + ET) / 2 will be used
   # instead of TE and ET separately.
   symmetrize: false
 
 data:
   # List the names and frequencies of all the
   # relevant experiments.
@@ -67,14 +67,15 @@
 #     bandwidth can be a list if you want a different width for each band
 #     e.g. bandwidth: [0.3,0.2,0.3] for 3 bands
 # when top_hat_band is a null dict: no top-hat band is built and
 # bandpasses read from sacc file. Band integration is performed accordingly
 # (if bandpass in sacc is a single freq, no band integration)
 # the default is to read bandpasses from file, to build top-hat uncomment the
 # parameters of the block!
+# Bandpass has to be in RJ units
 top_hat_band:
 #  nsteps: 1
 #  bandwidth: 0
 
 # uncomment the block to include a systematic template
 # to be read from external file at "rootname"
 # default is systematic_template to be a null dict
```

### Comparing `mflike-0.8.2/mflike/mflike.py` & `mflike-0.8.3/mflike/mflike.py`

 * *Files identical despite different names*

### Comparing `mflike-0.8.2/mflike/theoryforge.py` & `mflike-0.8.3/mflike/theoryforge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 from itertools import product
 
 import numpy as np
 from cobaya.log import LoggedError
 
 
-# Converts from cmb units to brightness. Numerical factors not included,
+# Converts from cmb units to brightness.
+# There is an additional nu**2 factor to convert the bandpasses
+# from RJ to brightness units.
+# Numerical factors not included,
 # it needs proper normalization when used.
 def _cmb2bb(nu):
     # NB: numerical factors not included
     from scipy import constants
 
     T_CMB = 2.72548
     x = nu * constants.h * 1e9 / constants.k / T_CMB
@@ -74,14 +77,15 @@
                 if self.bandint_nsteps > 1 and np.any(np.array(self.bandint_width) == 0):
                     raise LoggedError(
                         self.log, "One band has width = 0, set a positive width and run again"
                     )
 
     # Takes care of the bandpass construction. It returns a list of nu-transmittance
     # for each frequency or an array with the effective freqs.
+    # bandpasses saved in the sacc file have to be in RJ units
     def _bandpass_construction(self, **params):
         data_are_monofreq = False
         self.bandint_freqs = []
         for iexp, exp in enumerate(self.experiments):
             bandpar = f"bandint_shift_{exp}"
             # Only temperature bandpass for the time being
             bands = self.bands[f"{exp}_s0"]
@@ -89,45 +93,48 @@
             # computing top-hat bandpass to make band integration
             if self.use_top_hat_band:
                 # Compute central frequency given bandpass in the sacc file
                 fr = nu_ghz @ bp / bp.sum()
                 if self.bandint_nsteps > 1:
                     bandlow = fr * (1 - self.bandint_width[iexp] * 0.5)
                     bandhigh = fr * (1 + self.bandint_width[iexp] * 0.5)
-                    nubtrue = np.linspace(bandlow, bandhigh, self.bandint_nsteps, dtype=float)
+                    #nubtrue = np.linspace(bandlow, bandhigh, self.bandint_nsteps, dtype=float)
                     nub = np.linspace(
                         bandlow + params[bandpar],
                         bandhigh + params[bandpar],
                         self.bandint_nsteps,
                         dtype=float,
                     )
                     tranb = _cmb2bb(nub)
-                    tranb_norm = np.trapz(_cmb2bb(nubtrue), nubtrue)
+                    # normalization integral to be evaluated at the shifted freqs 
+                    # in order to have cmb component calibrated to 1
+                    tranb_norm = np.trapz(_cmb2bb(nub), nub)
                     self.bandint_freqs.append([nub, tranb / tranb_norm])
                 # in case we don't want to do band integration, e.g. when we have multifreq bandpass in sacc file
                 if self.bandint_nsteps == 1:
                     nub = fr + params[bandpar]
                     data_are_monofreq = True
                     self.bandint_freqs.append(nub)
             # using the bandpass from sacc file
             else:
                 nub = nu_ghz + params[bandpar]
                 if len(bp) == 1:
                     # Monofrequency channel
                     data_are_monofreq = True
                     self.bandint_freqs.append(nub[0])
                 else:
-                    trans_norm = np.trapz(bp * _cmb2bb(nu_ghz), nu_ghz)
+                    trans_norm = np.trapz(bp * _cmb2bb(nub), nub)
                     trans = bp / trans_norm * _cmb2bb(nub)
                     self.bandint_freqs.append([nub, trans])
 
         # fgspectra can't mix monofrequency with [nu, bp]. If one channel is mono-frequency then we
         # assume all of them and pass to fgspectra an array (not list!!) of frequencies
         if data_are_monofreq:
             self.bandint_freqs = np.asarray(self.bandint_freqs)
+            self.log.info("bandpass is delta function, no band integration performed")
 
     def get_modified_theory(self, Dls, **params):
         fg_params = {k: params[k] for k in self.expected_params_fg}
         nuis_params = {k: params[k] for k in self.expected_params_nuis}
 
         # compute bandpasses at each step only if bandint_shift params are not null
         # and bandint_freqs has been computed at least once
```

### Comparing `mflike-0.8.2/mflike.egg-info/PKG-INFO` & `mflike-0.8.3/mflike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.2
+Version: 0.8.3
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mflike-0.8.2/setup.py` & `mflike-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `mflike-0.8.2/versioneer.py` & `mflike-0.8.3/versioneer.py`

 * *Files identical despite different names*

