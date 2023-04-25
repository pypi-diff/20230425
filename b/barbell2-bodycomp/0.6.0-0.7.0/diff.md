# Comparing `tmp/barbell2_bodycomp-0.6.0.tar.gz` & `tmp/barbell2_bodycomp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbell2_bodycomp-0.6.0.tar", last modified: Tue Apr 18 13:15:19 2023, max compression
+gzip compressed data, was "barbell2_bodycomp-0.7.0.tar", last modified: Tue Apr 25 13:13:12 2023, max compression
```

## Comparing `barbell2_bodycomp-0.6.0.tar` & `barbell2_bodycomp-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.746585 barbell2_bodycomp-0.6.0/
--rw-r--r--   0 Ralph      (501) staff       (20)      802 2023-04-18 13:15:19.746323 barbell2_bodycomp-0.6.0/PKG-INFO
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.738920 barbell2_bodycomp-0.6.0/barbell2_bodycomp/
--rw-r--r--   0 Ralph      (501) staff       (20)      392 2023-04-18 13:15:13.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     4447 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/calculator.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.743760 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/
--rw-r--r--   0 Ralph      (501) staff       (20)      403 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2200 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1485 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1405 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 Ralph      (501) staff       (20)      853 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2030 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1059 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 Ralph      (501) staff       (20)      435 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2npy.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.744202 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     5705 2023-04-17 10:38:03.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/bodycomp.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6054 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/seg.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1394 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectroi.py
--rw-r--r--   0 Ralph      (501) staff       (20)     5804 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectslice.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1586 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/totalseg.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6246 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.741339 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 Ralph      (501) staff       (20)      802 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 Ralph      (501) staff       (20)      882 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 Ralph      (501) staff       (20)       68 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       18 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-04-18 13:15:19.746668 barbell2_bodycomp-0.6.0/setup.cfg
--rw-r--r--   0 Ralph      (501) staff       (20)     1456 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/setup.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.623622 barbell2_bodycomp-0.7.0/
+-rw-r--r--   0 Ralph      (501) staff       (20)      791 2023-04-25 13:13:12.623184 barbell2_bodycomp-0.7.0/PKG-INFO
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.616157 barbell2_bodycomp-0.7.0/barbell2_bodycomp/
+-rw-r--r--   0 Ralph      (501) staff       (20)      392 2023-04-25 13:13:08.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     4447 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.622032 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 Ralph      (501) staff       (20)      403 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     2200 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1485 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      558 2023-04-25 11:30:39.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2raw.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1405 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      853 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     2030 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1059 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      435 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2npy.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.622671 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/
+-rw-r--r--   0 Ralph      (501) staff       (20)        0 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6132 2023-04-25 12:54:52.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/bodycomp.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6054 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1394 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     5804 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1586 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6246 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.619478 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 Ralph      (501) staff       (20)      791 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 Ralph      (501) staff       (20)      919 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/entry_points.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 Ralph      (501) staff       (20)       68 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       18 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-04-25 13:13:12.623708 barbell2_bodycomp-0.7.0/setup.cfg
+-rw-r--r--   0 Ralph      (501) staff       (20)     1456 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/setup.py
```

### Comparing `barbell2_bodycomp-0.6.0/PKG-INFO` & `barbell2_bodycomp-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: barbell2_bodycomp
-Version: 0.6.0
+Version: 0.7.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
-Description: UNKNOWN
 Keywords: barbell2_bodycomp
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+
+UNKNOWN
+
```

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/calculator.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/calculator.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/bodycomp.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/bodycomp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import json
+import shutil
 import argparse
 
 from barbell2_bodycomp.convert import DicomToNifti
 from barbell2_bodycomp import TotalSegmentator, RoiSelector, SliceSelector, MuscleFatSegmentator, BodyCompositionCalculator
 
 
 class BodyCompositionPipeline:
@@ -50,14 +52,15 @@
                     ]
                     break
         if model_files is None:
             raise RuntimeError('could not find model files (searched /tmp, /tmp/mosamatic, /mnt/localscratch/cds/rbrecheisen/models/v2)')
         return model_files
 
     def execute(self):
+        os.makedirs(self.output_directory, exist_ok=True)
         if 'dicom2nifti' in self.steps:
             # convert dicoms to nifti
             d2n = DicomToNifti()
             d2n.input_directory = self.input_directory
             d2n.output_file = os.path.join(self.output_directory, 'file.nii.gz')
             nifti_file = d2n.execute()
             if 'totalsegmentator' in self.steps:
@@ -78,31 +81,35 @@
                         # select l3 slice
                         selector = SliceSelector()
                         selector.input_dicom_directory = self.input_directory
                         selector.input_roi = roi_file
                         selector.input_volume = nifti_file
                         selector.mode = SliceSelector.MEDIAN
                         l3_file = selector.execute()[0]
+                        shutil.copy(l3_file, self.output_directory)
                         if 'l3seg' in self.steps:
                             # run l3 through muscle/fat segmentation
                             segmentator = MuscleFatSegmentator()
                             segmentator.input_files = [l3_file]
                             segmentator.image_dimensions = (512, 512)
                             segmentator.model_files = self.model_files
                             segmentator.mode = self.mode
                             segmentator.output_directory = os.path.join(self.output_directory, 'segmentator')
                             output_files = segmentator.execute()
-                            for f in output_files:
-                                print(f)
                             if 'calculate' in self.steps:
                                 # calculte body composition metrics
+                                # todo: output to CSV
                                 calculator = BodyCompositionCalculator()
                                 calculator.input_files = segmentator.input_files
                                 calculator.input_segmentation_files = output_files
                                 output_metrics = calculator.execute()
+                                output_directory = os.path.join(self.output_directory, 'calculate')
+                                os.makedirs(output_directory, exist_ok=True)
+                                with open(l3_file + '.json', 'w') as f:
+                                    json.dump(output_metrics, f)
                                 print(output_metrics)
 
 
 if __name__ == '__main__':
     def main():
 
         parser = argparse.ArgumentParser()
@@ -118,8 +125,8 @@
             input_directory=args.input_directory,
             output_directory=args.output_directory, 
             model_files=args.model_files,
             steps=args.steps,
             mode=MuscleFatSegmentator.ARGMAX if args.mode == 'ARGMAX' else MuscleFatSegmentator.PROBABILITIES,
         )
         pipeline.execute()
-    main()
+    main()
```

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/seg.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/seg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectroi.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectroi.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectslice.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectslice.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/totalseg.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/totalseg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: barbell2-bodycomp
-Version: 0.6.0
+Version: 0.7.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
-Description: UNKNOWN
 Keywords: barbell2_bodycomp
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+
+UNKNOWN
+
```

### Comparing `barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 barbell2_bodycomp.egg-info/entry_points.txt
 barbell2_bodycomp.egg-info/not-zip-safe
 barbell2_bodycomp.egg-info/requires.txt
 barbell2_bodycomp.egg-info/top_level.txt
 barbell2_bodycomp/convert/__init__.py
 barbell2_bodycomp/convert/dcm2nifti.py
 barbell2_bodycomp/convert/dcm2npy.py
+barbell2_bodycomp/convert/dcm2raw.py
 barbell2_bodycomp/convert/npy2dcm.py
 barbell2_bodycomp/convert/npy2nrrd.py
 barbell2_bodycomp/convert/npy2png.py
 barbell2_bodycomp/convert/tag2dcm.py
 barbell2_bodycomp/convert/tag2npy.py
 barbell2_bodycomp/pipeline/__init__.py
 barbell2_bodycomp/pipeline/bodycomp.py
```

### Comparing `barbell2_bodycomp-0.6.0/setup.py` & `barbell2_bodycomp-0.7.0/setup.py`

 * *Files identical despite different names*

