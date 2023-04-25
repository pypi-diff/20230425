# Comparing `tmp/skye-0.0.4.tar.gz` & `tmp/skye-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skye-0.0.4.tar", last modified: Fri Apr 21 01:26:03 2023, max compression
+gzip compressed data, was "skye-0.0.5.tar", last modified: Tue Apr 25 03:46:26 2023, max compression
```

## Comparing `skye-0.0.4.tar` & `skye-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.313087 skye-0.0.4/
--rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.4/LICENSE
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:26:03.312829 skye-0.0.4/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.4/README.md
--rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-21 01:26:03.313171 skye-0.0.4/setup.cfg
--rw-r--r--   0 iosefa     (501) staff       (20)     1063 2023-04-21 01:25:33.000000 skye-0.0.4/setup.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.310959 skye-0.0.4/skye/
--rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.4/skye/__init__.py
--rw-r--r--   0 iosefa     (501) staff       (20)     9463 2023-04-21 01:17:17.000000 skye-0.0.4/skye/core.py
--rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.4/skye/utils.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.312499 skye-0.0.4/skye.egg-info/
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      209 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/SOURCES.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/dependency_links.txt
--rw-r--r--   0 iosefa     (501) staff       (20)      168 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/requires.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/top_level.txt
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-25 03:46:26.746497 skye-0.0.5/
+-rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.5/LICENSE
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-25 03:46:26.746256 skye-0.0.5/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.5/README.md
+-rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-25 03:46:26.746575 skye-0.0.5/setup.cfg
+-rw-r--r--   0 iosefa     (501) staff       (20)     1063 2023-04-25 03:46:05.000000 skye-0.0.5/setup.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-25 03:46:26.744413 skye-0.0.5/skye/
+-rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.5/skye/__init__.py
+-rw-r--r--   0 iosefa     (501) staff       (20)    13470 2023-04-25 03:46:05.000000 skye-0.0.5/skye/core.py
+-rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.5/skye/utils.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-25 03:46:26.745951 skye-0.0.5/skye.egg-info/
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-25 03:46:26.000000 skye-0.0.5/skye.egg-info/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      209 2023-04-25 03:46:26.000000 skye-0.0.5/skye.egg-info/SOURCES.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-25 03:46:26.000000 skye-0.0.5/skye.egg-info/dependency_links.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)      168 2023-04-25 03:46:26.000000 skye-0.0.5/skye.egg-info/requires.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-25 03:46:26.000000 skye-0.0.5/skye.egg-info/top_level.txt
```

### Comparing `skye-0.0.4/LICENSE` & `skye-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `skye-0.0.4/PKG-INFO` & `skye-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.4
+Version: 0.0.5
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skye-0.0.4/setup.py` & `skye-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="skye",
-    version="0.0.4",
+    version="0.0.5",
     author="Iosefa Percival",
     author_email="ipercival@gmail.com",
     description="360-degree image analysis for forest ecology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iosefa/skye",
     project_urls={
```

### Comparing `skye-0.0.4/skye/core.py` & `skye-0.0.5/skye/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,40 +3,57 @@
 import warnings
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy
 
+from PIL.ExifTags import TAGS
 from IPython.core.display_functions import clear_output
 from tqdm.auto import tqdm
 from math import atan, pi, sqrt
 from PIL import Image
-from skimage import io
-from skimage.segmentation import quickshift
+from skimage.segmentation import quickshift, slic
 from skimage.segmentation import mark_boundaries
 from skimage.util import img_as_float
+from skimage import exposure
 from sklearn.ensemble import RandomForestClassifier
 
 from skye.utils import flatten
 
 
 def _load_image(img):
     try:
-        image = io.imread(img)
+        image = Image.open(img)
         return image
     except Exception as e:
         raise Exception(f'Could not import image. Original exception: {e}')
 
 
-def segment_image(img, ratio=0.85, sigma=0):
+def segment_image(img, segmentation_method='quickshift', **kwargs):
     img = np.array(img)
     img = img_as_float(img)
-    segments = quickshift(img, ratio=ratio, sigma=sigma)
-    return segments
+    if segmentation_method == 'quickshift':
+        segments = quickshift(img, **kwargs)
+        return segments
+    elif segmentation_method == 'slic':
+        segments = slic(img, **kwargs)
+        return segments
+    else:
+        raise Exception('An unknown segmentation method was requested.')
+
+
+def binarize(img, threshold):
+    gray_img = create_grayscale(img)
+    threshold = threshold * 255
+    binary_img = gray_img.copy()
+    binary_img[binary_img >= threshold] = 255
+    binary_img[binary_img < threshold] = 0
+    im = Image.fromarray(binary_img.astype(np.uint8))
+    return im
 
 
 def summary_statistics(segment_pixels):
     """
     For each band, compute: min, max, mean, variance, skewness, kurtosis
     """
     features = []
@@ -67,21 +84,77 @@
                 'id': segment_id,
                 'stats': segment_stats
             }
         )
     return objects
 
 
-def create_hemispherical(image_path):
+def enhance(image, clip_limit=3, grid_size=(4, 4)):
+    img = np.array(image)
+    lab = cv2.cvtColor(img, cv2.COLOR_BGR2LAB)
+    l, a, b = cv2.split(lab)
+
+    clahe = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=grid_size)
+    cl = clahe.apply(l)
+
+    cl_image = cv2.merge((cl, a, b))
+
+    enhanced_img = cv2.cvtColor(cl_image, cv2.COLOR_LAB2BGR)
+
+    h, w = enhanced_img.shape[:2]
+    mask = create_circular_mask(h, w)
+
+    masked_img = enhanced_img.copy()
+    masked_img[~mask] = 0
+
+    return Image.fromarray(masked_img)
+
+
+def enhance_full(image, clip_limit=3.5, grid_size=(2, 2)):
+    img = np.array(image)
+    lab = cv2.cvtColor(img, cv2.COLOR_BGR2LAB)
+    l, a, b = cv2.split(lab)
+
+    clahe = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=grid_size)
+    cl = clahe.apply(l)
+    ca = clahe.apply(a)
+    cb = clahe.apply(b)
+
+    clab_image = cv2.merge((cl, ca, cb))
+
+    enhanced_img = cv2.cvtColor(clab_image, cv2.COLOR_LAB2BGR)
+
+    h, w = enhanced_img.shape[:2]
+    mask = create_circular_mask(h, w)
+
+    masked_img = enhanced_img.copy()
+    masked_img[~mask] = 0
+
+    return Image.fromarray(masked_img)
+
+
+def get_metadata(img):
+    all_metadata = dict()
+    exifdata = img.getexif()
+    for tag_id in exifdata:
+        tag = TAGS.get(tag_id, tag_id)
+        data = exifdata.get(tag_id)
+        if isinstance(data, bytes):
+            data = data.decode()
+        all_metadata[tag] = data
+    return all_metadata
+
+
+def create_hemispherical(image):
     """
     Creates an equal-area hemispherical image from a 360 image.
-    :param image_path: path to 360 image.
+    :param image: PIL image.
     :return:
     """
-    img = _load_image(image_path)
+    img = np.array(image)
     dim1 = img.shape[0]
     img_h1 = np.zeros((dim1 + 1, dim1 + 1, 3))
     img_h2 = img_h1.copy()
     dim2 = int(dim1 / 2)
 
     for i in tqdm(range(-dim2, dim2), bar_format='{l_bar}{bar}', desc="Creating Hemispherical Photo"):
         for j in range(-dim2, dim2):
@@ -103,15 +176,22 @@
             iy = sqrt(i ** 2 + j ** 2)
             iy2 = round(dim2 * np.arcsin(iy / dim2 / np.sqrt(2)) / pi * 4)
             if 1 <= ix <= dim1 * 2 and 1 <= iy2 <= dim1 // 2:
                 img_h2[i + dim2, j + dim2] = img[iy2, ix - 1]
 
     im_b = np.concatenate((img_h2[:dim2], img_h2[dim2 + 2:]), axis=0)
     im_bb = np.concatenate((im_b[:, :dim2], im_b[:, dim2 + 2:]), axis=1)
-    img = Image.fromarray(im_bb.astype(np.uint8))
+
+    h, w = im_bb.shape[:2]
+    mask = create_circular_mask(h, w)
+
+    masked_img = im_bb.copy()
+    masked_img[~mask] = 0
+
+    img = Image.fromarray(masked_img.astype(np.uint8))
     return img
 
 
 def calculate_svf(img, bi_img):
     img = np.array(img)
     bi_img = np.array(bi_img)
     total_pixels = img.shape[0] * img.shape[0]
@@ -119,127 +199,180 @@
     outside_pixels = total_pixels - hemisphere_pixels
 
     black_pixels = total_pixels - np.sum(bi_img / 255) - outside_pixels
     svf = (hemisphere_pixels - black_pixels) / hemisphere_pixels
     return svf
 
 
-class SkyViewThreshold:
-    def __init__(
-        self,
-        image_path: str,
-        threshold=0.5
-    ):
-        self.image_path = image_path
-        self.img = create_hemispherical(image_path)
-        self.threshold = threshold * 255
-        self.gray_img = cv2.cvtColor(np.array(self.img), cv2.COLOR_RGB2GRAY)
-        self.binary_img = self.create_binary()
-        self.sky_view_factor = calculate_svf(self.img, self.binary_img)
-
-    def create_binary(self):
-        binary_img = self.gray_img.copy()
-        binary_img[binary_img >= self.threshold] = 255
-        binary_img[binary_img < self.threshold] = 0
-        im = Image.fromarray(binary_img.astype(np.uint8))
-        return im
+def gamma_correction(image, gamma=1, gain=1):
+    img = np.array(image)
+    right_shift = exposure.adjust_gamma(img, gamma=gamma, gain=gain)
+
+    h, w = right_shift.shape[:2]
+    mask = create_circular_mask(h, w)
 
-    def plot_binary(self, ax):
-        out = ax.imshow(self.binary_img)
-        return out
+    masked_img = right_shift.copy()
+    masked_img[~mask] = 0
 
+    return Image.fromarray(masked_img.astype(np.uint8))
+
+
+def create_grayscale(img):
+    img_array = np.array(img)
+    return cv2.cvtColor(img_array, cv2.COLOR_RGB2GRAY)
+
+
+def create_circular_mask(h, w, center=None, radius=None):
+
+    if center is None:
+        center = (int(w/2), int(h/2))
+    if radius is None:
+        radius = min(center[0], center[1], w-center[0], h-center[1])
+
+    Y, X = np.ogrid[:h, :w]
+    dist_from_center = np.sqrt((X - center[0])**2 + (Y-center[1])**2)
+
+    mask = dist_from_center <= radius
+    return mask
+
+
+class SkyView:
 
-class SkyViewClassified:
     def __init__(
-        self,
-        image_path: str,
-        training_data_path=None
+            self,
+            image_path: str,
+            enhance_image=False,
+            adjust_gamma=False,
+            segmentation_method='binarize',
+            gamma=1,
+            gain=1,
+            clip_limit=3,
+            grid_size=(4, 4),
+            training_data_path=None,
+            **kwargs
     ):
-        logging.info('Initializing Sky View Object. This will take some time...')
         self.image_path = image_path
-        self.img = create_hemispherical(image_path)
-        logging.info('Segmenting image...')
-        self.segments = segment_image(self.img)
+        img = _load_image(image_path)
+        self.metadata = get_metadata(img)
+        self.segmentation_params = kwargs
+
+        self.img = create_hemispherical(img)
+
+        self.segments = None
+        self.segmented_img = None
         self.classified_img = None
         self.sky_view_factor = None
-        self.objects = create_objects(self.img, self.segments)
-        self.objects_df = pd.DataFrame(
-            columns=['segment_id', 'nobs', 'b1_min', 'b1_max', 'b2_min', 'b2_max', 'b3_min', 'b3_max', 'b1_mean',
-                     'b2_mean', 'b3_mean', 'b1_variance', 'b2_variance', 'b3_variance', 'b1_skewness', 'b2_skewness',
-                     'b3_skewness', 'b1_kurtosis', 'b2_kurtosis', 'b3_kurtosis']
-        )
-        for i, obj in enumerate(tqdm(self.objects, bar_format='{l_bar}{bar}', desc="Creating object statistics dataframe")):
-            row = flatten(obj['stats'])
-            self.objects_df.loc[i] = [i] + row
-        self.objects_df_clean = self.objects_df.dropna()
-        if training_data_path:
-            logging.info('Classifying image...')
-            self.training_classes = pd.read_csv(training_data_path)
-            self.classified_img = self.classify()
-            logging.info('Calculating sky view factor...')
-            self.sky_view_factor = calculate_svf(self.img, self.classified_img)
+
+        if enhance_image:
+            self.img = enhance(self.img, clip_limit=clip_limit, grid_size=grid_size)
+        if adjust_gamma:
+            self.img = gamma_correction(self.img, gamma=gamma, gain=gain)
+
+        if segmentation_method == 'binarize':
+            self.classified_img = binarize(self.img, **kwargs)
+            self.segments = None
         else:
-            self.training_classes = pd.DataFrame(
-                columns=['class', 'nobs', 'b1_min', 'b1_max', 'b2_min', 'b2_max', 'b3_min', 'b3_max', 'b1_mean', 'b2_mean',
-                         'b3_mean', 'b1_variance', 'b2_variance', 'b3_variance', 'b1_skewness', 'b2_skewness',
+            self.segments = segment_image(self.img, segmentation_method=segmentation_method, **kwargs)
+            self.classified_img = None
+
+            self.segmented_img = self.create_segmented_img()
+
+            self.objects = create_objects(self.img, self.segments)
+            self.objects_df = pd.DataFrame(
+                columns=['segment_id', 'nobs', 'b1_min', 'b1_max', 'b2_min', 'b2_max', 'b3_min', 'b3_max', 'b1_mean',
+                         'b2_mean', 'b3_mean', 'b1_variance', 'b2_variance', 'b3_variance', 'b1_skewness', 'b2_skewness',
                          'b3_skewness', 'b1_kurtosis', 'b2_kurtosis', 'b3_kurtosis']
             )
-            logging.warning('You must create or import training data in order to calculate the sky view factor')
-
-    def plot_rgb(self, ax):
-        out = ax.imshow(self.img)
-        return out
+            for i, obj in enumerate(
+                    tqdm(self.objects, bar_format='{l_bar}{bar}', desc="Creating object statistics dataframe")):
+                row = flatten(obj['stats'])
+                self.objects_df.loc[i] = [i] + row
+            self.objects_df_clean = self.objects_df.dropna()
+
+            if training_data_path:
+                logging.info('Classifying image...')
+                self.training_classes = pd.read_csv(training_data_path)
+                self.classify()
+                logging.info('Calculating sky view factor...')
+                self.sky_view_factor = calculate_svf(self.img, self.classified_img)
+            else:
+                self.training_classes = pd.DataFrame(
+                    columns=['class', 'nobs', 'b1_min', 'b1_max', 'b2_min', 'b2_max', 'b3_min', 'b3_max', 'b1_mean',
+                             'b2_mean',
+                             'b3_mean', 'b1_variance', 'b2_variance', 'b3_variance', 'b1_skewness', 'b2_skewness',
+                             'b3_skewness', 'b1_kurtosis', 'b2_kurtosis', 'b3_kurtosis']
+                )
+                logging.warning('You must create or import training data in order to calculate the sky view factor')
 
-    def plot_segments(self, ax):
+    def create_segmented_img(self):
         img = np.array(self.img)
+
+        h, w = img.shape[:2]
+        mask = create_circular_mask(h, w)
+
         boundaries = mark_boundaries(img, self.segments)
-        out = ax.imshow(boundaries)
-        return out
+        boundaries_int = boundaries * 255
 
-    def plot_classified(self, ax):
-        if self.classified_img is None:
-            logging.warning('Image has not yet been classified. Aborting.')
-            return
-        out = ax.imshow(self.classified_img)
-        return out
+        masked_img = boundaries_int.copy()
+        masked_img[~mask] = 0
+        return Image.fromarray(masked_img.astype(np.uint8))
 
-    def create_training_data(self, n_samples=500, notebook=False):
+    def create_training_data(self, n_samples=500, notebook=False, save_segment_path=None):
         sample = random.sample(list(self.objects_df_clean['segment_id'].values), n_samples)
         img = np.array(self.img)
         img = img_as_float(img)
         for j, i in enumerate(sample):
-            print(f'working on segment {i} ({j}/500)')
+            print(f'working on segment {i} ({j}/{n_samples})')
             mask = np.ma.masked_where(self.segments != i, self.segments)
             valid_pixels = np.argwhere(~np.isnan(mask))
             y_min, x_min = tuple(np.min(valid_pixels, axis=0))
             y_max, x_max = tuple(np.max(valid_pixels, axis=0))
 
-            x_min = x_min if x_min - 100 < 0 else x_min - 100
-            y_min = y_min if y_min - 100 < 0 else y_min - 100
-            x_max = x_max if x_max + 100 > self.segments.shape[0] else x_max + 100
-            y_max = y_max if y_max + 100 > self.segments.shape[0] else y_max + 100
+            x_min = x_min if x_min - 75 < 0 else x_min - 75
+            y_min = y_min if y_min - 75 < 0 else y_min - 75
+            x_max = x_max if x_max + 75 > self.segments.shape[0] else x_max + 75
+            y_max = y_max if y_max + 75 > self.segments.shape[0] else y_max + 75
 
             fig = plt.figure(f"Segment {i}")
             ax = fig.add_subplot(1, 1, 1)
             ax.imshow(img)
             ax.imshow(mask)
             plt.axis("off")
 
-            ax.imshow(mark_boundaries(img, mask))
+            ax.imshow(mark_boundaries(img, mask, color=(255, 0, 0)))
             plt.axis([x_min, x_max, y_min, y_max])
+
+            segment_fig = plt.gcf()
             plt.show()
 
-            klass = input("Enter class or type 'I give up!' to end.")
-            if klass.lower() == 'i give up!':
+            while True:
+                klass = input(
+                    "Enter class ('0' for non-sky, '1' for sky) or type 'skip' to skip. To quit, enter 'I give up'.")
+
+                if klass.lower() not in ('1', '0', 'i give up', 'skip'):
+                    print("Not an appropriate response. You must enter either '1', '0', 'I give up', or 'skip'.")
+                else:
+                    break
+
+            if klass.lower() == 'i give up':
                 break
+            if klass == 'skip':
+                clear_output(wait=True)
+                continue
             self.training_classes.loc[len(self.training_classes)] = [klass] + list(
                 self.objects_df.loc[self.objects_df['segment_id'] == i].values[0]
             )[1:]
+            if save_segment_path:
+                # todo: get name from metadata instead
+                name = self.image_path.split('/')[-1].split('.')[0]
+                segment_fig.savefig(
+                    f"{save_segment_path}/{name}_{i}_{j}_r{len(self.training_classes)}_cl{klass}.jpg", dpi=72)
             if notebook:
                 clear_output(wait=True)
+        print('Congratulations! You did it!')
 
     def import_training_data(self, training_data_path):
         self.training_classes = pd.read_csv(training_data_path)
 
     def export_training_data(self, file_name='training.csv'):
         self.training_classes.to_csv(file_name, index=False)
 
@@ -252,10 +385,15 @@
         y_pred = rf.predict(x_test)
         segment_ids = list(self.objects_df_clean['segment_id'].values)
         classified_img = img_as_float(np.array(self.img)).copy()
         for i, segment_id in enumerate(segment_ids):
             idx = np.argwhere(self.segments == segment_id)
             for j in idx:
                 classified_img[j[0], j[1], 0] = y_pred[i]
-        clf = classified_img[:, :, 0]
+        clf = classified_img[:, :, 0] * 255
         im = Image.fromarray(clf.astype(np.uint8))
+        self.classified_img = im
         return im
+
+    def calculate_svf(self):
+        self.sky_view_factor = calculate_svf(self.img, self.classified_img)
+        return self.sky_view_factor
```

### Comparing `skye-0.0.4/skye/utils.py` & `skye-0.0.5/skye/utils.py`

 * *Files identical despite different names*

### Comparing `skye-0.0.4/skye.egg-info/PKG-INFO` & `skye-0.0.5/skye.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.4
+Version: 0.0.5
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

