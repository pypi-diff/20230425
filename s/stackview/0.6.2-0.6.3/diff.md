# Comparing `tmp/stackview-0.6.2.tar.gz` & `tmp/stackview-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.6.2.tar", last modified: Wed Apr 19 19:49:46 2023, max compression
+gzip compressed data, was "stackview-0.6.3.tar", last modified: Tue Apr 25 13:10:05 2023, max compression
```

## Comparing `stackview-0.6.2.tar` & `stackview-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.926694 stackview-0.6.2/
--rw-rw-rw-   0        0        0     1549 2023-04-19 19:02:17.000000 stackview-0.6.2/LICENSE
--rw-rw-rw-   0        0        0    10414 2023-04-19 19:49:46.926694 stackview-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     9830 2023-04-19 19:02:17.000000 stackview-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 19:49:46.926694 stackview-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-04-19 19:49:26.000000 stackview-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.905159 stackview-0.6.2/stackview/
--rw-rw-rw-   0        0        0      586 2023-04-19 19:49:26.000000 stackview-0.6.2/stackview/__init__.py
--rw-rw-rw-   0        0        0     7781 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_assist.py
--rw-rw-rw-   0        0        0     5467 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_colormaps.py
--rw-rw-rw-   0        0        0     2060 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_context.py
--rw-rw-rw-   0        0        0     5487 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_crop.py
--rw-rw-rw-   0        0        0     4684 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_curtain.py
--rw-rw-rw-   0        0        0     4070 2023-04-19 19:44:22.000000 stackview-0.6.2/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     7544 2023-04-19 19:49:26.000000 stackview-0.6.2/stackview/_interact.py
--rw-rw-rw-   0        0        0     2124 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     3384 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_picker.py
--rw-rw-rw-   0        0        0     5023 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     2149 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_slice.py
--rw-rw-rw-   0        0        0     2350 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8266 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_static_view.py
--rw-rw-rw-   0        0        0     6146 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.925626 stackview-0.6.2/stackview.egg-info/
--rw-rw-rw-   0        0        0    10414 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:10:05.740350 stackview-0.6.3/
+-rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0    10414 2023-04-25 13:10:05.740350 stackview-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9830 2023-04-15 09:27:34.000000 stackview-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:10:05.740350 stackview-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-04-25 13:08:10.000000 stackview-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:10:05.681270 stackview-0.6.3/stackview/
+-rw-rw-rw-   0        0        0      586 2023-04-25 13:08:10.000000 stackview-0.6.3/stackview/__init__.py
+-rw-rw-rw-   0        0        0     7781 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.6.3/stackview/_assist.py
+-rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.6.3/stackview/_context.py
+-rw-rw-rw-   0        0        0     5487 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_crop.py
+-rw-rw-rw-   0        0        0     4684 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4070 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     7544 2023-04-25 12:57:45.000000 stackview-0.6.3/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2124 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3384 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5023 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2149 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2350 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8329 2023-04-25 13:08:10.000000 stackview-0.6.3/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6146 2023-04-15 09:27:34.000000 stackview-0.6.3/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.6.3/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.6.3/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:10:05.732351 stackview-0.6.3/stackview.egg-info/
+-rw-rw-rw-   0        0        0    10414 2023-04-25 13:10:05.000000 stackview-0.6.3/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-25 13:10:05.000000 stackview-0.6.3/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:10:05.000000 stackview-0.6.3/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-25 13:10:05.000000 stackview-0.6.3/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 13:10:05.000000 stackview-0.6.3/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.6.2/LICENSE` & `stackview-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/PKG-INFO` & `stackview-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.2
+Version: 0.6.3
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `stackview-0.6.2/README.md` & `stackview-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/setup.py` & `stackview-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.6.2",
+    version="0.6.3",
     author="Robert Haase",
     author_email="robert.haase@tu-dresden.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
```

### Comparing `stackview-0.6.2/stackview/__init__.py` & `stackview-0.6.3/stackview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
```

### Comparing `stackview-0.6.2/stackview/_annotate.py` & `stackview-0.6.3/stackview/_annotate.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_assist.py` & `stackview-0.6.3/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_colormaps.py` & `stackview-0.6.3/stackview/_colormaps.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_context.py` & `stackview-0.6.3/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_crop.py` & `stackview-0.6.3/stackview/_crop.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_curtain.py` & `stackview-0.6.3/stackview/_curtain.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_image_widget.py` & `stackview-0.6.3/stackview/_image_widget.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_interact.py` & `stackview-0.6.3/stackview/_interact.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_orthogonal.py` & `stackview-0.6.3/stackview/_orthogonal.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_picker.py` & `stackview-0.6.3/stackview/_picker.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_side_by_side.py` & `stackview-0.6.3/stackview/_side_by_side.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_slice.py` & `stackview-0.6.3/stackview/_slice.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_slice_viewer.py` & `stackview-0.6.3/stackview/_slice_viewer.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_static_view.py` & `stackview-0.6.3/stackview/_static_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,412 +106,416 @@
 00000690: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
 000006a0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
 000006b0: 2020 2020 2020 2020 2020 2020 2048 544d               HTM
 000006c0: 4c20 7465 7874 2077 6974 6820 7468 6520  L text with the 
 000006d0: 696d 6167 6520 616e 6420 736f 6d65 2070  image and some p
 000006e0: 726f 7065 7274 6965 732e 0d0a 2020 2020  roperties...    
 000006f0: 2020 2020 2020 2020 2020 2020 2222 220d              """.
-00000700: 0a0d 0a20 2020 2020 2020 2069 6d70 6f72  ...        impor
-00000710: 7420 6e75 6d70 7920 6173 206e 700d 0a20  t numpy as np.. 
-00000720: 2020 2020 2020 2073 697a 655f 696e 5f70         size_in_p
-00000730: 6978 656c 7320 3d20 6e70 2e70 726f 6428  ixels = np.prod(
-00000740: 7365 6c66 2e73 6861 7065 290d 0a20 2020  self.shape)..   
-00000750: 2020 2020 2073 697a 655f 696e 5f62 7974       size_in_byt
-00000760: 6573 203d 2073 697a 655f 696e 5f70 6978  es = size_in_pix
-00000770: 656c 7320 2a20 7365 6c66 2e64 7479 7065  els * self.dtype
-00000780: 2e69 7465 6d73 697a 650d 0a0d 0a20 2020  .itemsize....   
-00000790: 2020 2020 2066 726f 6d20 2e5f 696d 6167       from ._imag
-000007a0: 655f 7769 6467 6574 2069 6d70 6f72 7420  e_widget import 
-000007b0: 5f69 735f 6c61 6265 6c5f 696d 6167 650d  _is_label_image.
-000007c0: 0a20 2020 2020 2020 206c 6162 656c 7320  .        labels 
-000007d0: 3d20 5f69 735f 6c61 6265 6c5f 696d 6167  = _is_label_imag
-000007e0: 6528 7365 6c66 290d 0a0d 0a20 2020 2020  e(self)....     
-000007f0: 2020 2069 6d70 6f72 7420 6d61 7470 6c6f     import matplo
-00000800: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-00000810: 6c74 0d0a 2020 2020 2020 2020 5f69 6d73  lt..        _ims
-00000820: 686f 7728 7365 6c66 2c0d 0a20 2020 2020  how(self,..     
-00000830: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00000840: 733d 6c61 6265 6c73 2c0d 0a20 2020 2020  s=labels,..     
-00000850: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00000860: 6e75 655f 6472 6177 696e 673d 5472 7565  nue_drawing=True
-00000870: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000880: 2020 2063 6f6c 6f72 6261 723d 6e6f 7420     colorbar=not 
-00000890: 6c61 6265 6c73 290d 0a20 2020 2020 2020  labels)..       
-000008a0: 2069 6d61 6765 203d 205f 706e 675f 746f   image = _png_to
-000008b0: 5f68 746d 6c28 5f70 6c74 5f74 6f5f 706e  _html(_plt_to_pn
-000008c0: 6728 2929 0d0a 0d0a 2020 2020 2020 2020  g())....        
-000008d0: 6966 2073 697a 655f 696e 5f62 7974 6573  if size_in_bytes
-000008e0: 203e 2031 3032 343a 0d0a 2020 2020 2020   > 1024:..      
-000008f0: 2020 2020 2020 7369 7a65 5f69 6e5f 6279        size_in_by
-00000900: 7465 7320 3d20 7369 7a65 5f69 6e5f 6279  tes = size_in_by
-00000910: 7465 7320 2f20 3130 3234 0d0a 2020 2020  tes / 1024..    
-00000920: 2020 2020 2020 2020 6966 2073 697a 655f          if size_
-00000930: 696e 5f62 7974 6573 203e 2031 3032 343a  in_bytes > 1024:
-00000940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000950: 2020 7369 7a65 5f69 6e5f 6279 7465 7320    size_in_bytes 
-00000960: 3d20 7369 7a65 5f69 6e5f 6279 7465 7320  = size_in_bytes 
-00000970: 2f20 3130 3234 0d0a 2020 2020 2020 2020  / 1024..        
-00000980: 2020 2020 2020 2020 6966 2073 697a 655f          if size_
-00000990: 696e 5f62 7974 6573 203e 2031 3032 343a  in_bytes > 1024:
-000009a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000009b0: 2020 2020 2020 7369 7a65 5f69 6e5f 6279        size_in_by
-000009c0: 7465 7320 3d20 7369 7a65 5f69 6e5f 6279  tes = size_in_by
-000009d0: 7465 7320 2f20 3130 3234 0d0a 2020 2020  tes / 1024..    
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 7369 7a65 203d 2022 7b3a 2e31 667d 222e  size = "{:.1f}".
-00000a00: 666f 726d 6174 2873 697a 655f 696e 5f62  format(size_in_b
-00000a10: 7974 6573 2920 2b20 2220 4742 220d 0a20  ytes) + " GB".. 
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00000a30: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000a40: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
-00000a50: 2022 7b3a 2e31 667d 222e 666f 726d 6174   "{:.1f}".format
-00000a60: 2873 697a 655f 696e 5f62 7974 6573 2920  (size_in_bytes) 
-00000a70: 2b20 2220 4d42 220d 0a20 2020 2020 2020  + " MB"..       
-00000a80: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000a90: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00000aa0: 203d 2022 7b3a 2e31 667d 222e 666f 726d   = "{:.1f}".form
-00000ab0: 6174 2873 697a 655f 696e 5f62 7974 6573  at(size_in_bytes
-00000ac0: 2920 2b20 2220 6b42 220d 0a20 2020 2020  ) + " kB"..     
-00000ad0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000ae0: 2020 2020 2020 7369 7a65 203d 2022 7b3a        size = "{:
-00000af0: 2e31 667d 222e 666f 726d 6174 2873 697a  .1f}".format(siz
-00000b00: 655f 696e 5f62 7974 6573 2920 2b20 2220  e_in_bytes) + " 
-00000b10: 4222 0d0a 0d0a 2020 2020 2020 2020 6869  B"....        hi
-00000b20: 7374 6f67 7261 6d20 3d20 2222 0d0a 0d0a  stogram = ""....
-00000b30: 2020 2020 2020 2020 6966 2073 697a 655f          if size_
-00000b40: 696e 5f62 7974 6573 203c 2031 3030 202a  in_bytes < 100 *
-00000b50: 2031 3032 3420 2a20 3130 3234 3a0d 0a20   1024 * 1024:.. 
-00000b60: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00000b70: 7420 6c61 6265 6c73 3a0d 0a20 2020 2020  t labels:..     
-00000b80: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
-00000b90: 7420 6e75 6d70 7920 6173 206e 700d 0a0d  t numpy as np...
-00000ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bb0: 206e 756d 5f62 696e 7320 3d20 3332 0d0a   num_bins = 32..
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 682c 205f 203d 206e 702e 6869 7374 6f67  h, _ = np.histog
-00000be0: 7261 6d28 7365 6c66 2c20 6269 6e73 3d6e  ram(self, bins=n
-00000bf0: 756d 5f62 696e 7329 0d0a 0d0a 2020 2020  um_bins)....    
-00000c00: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00000c10: 6669 6775 7265 2866 6967 7369 7a65 3d28  figure(figsize=(
-00000c20: 312e 382c 2031 2e32 2929 0d0a 2020 2020  1.8, 1.2))..    
-00000c30: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00000c40: 6261 7228 7261 6e67 6528 302c 206c 656e  bar(range(0, len
-00000c50: 2868 2929 2c20 6829 0d0a 0d0a 2020 2020  (h)), h)....    
-00000c60: 2020 2020 2020 2020 2020 2020 2320 6869              # hi
-00000c70: 6465 2061 7869 7320 7465 7874 0d0a 2020  de axis text..  
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00000c90: 6874 7470 733a 2f2f 7374 6163 6b6f 7665  https://stackove
-00000ca0: 7266 6c6f 772e 636f 6d2f 7175 6573 7469  rflow.com/questi
-00000cb0: 6f6e 732f 3231 3736 3432 342f 6869 6469  ons/2176424/hidi
-00000cc0: 6e67 2d61 7869 732d 7465 7874 2d69 6e2d  ng-axis-text-in-
-00000cd0: 6d61 7470 6c6f 746c 6962 2d70 6c6f 7473  matplotlib-plots
-00000ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000cf0: 2020 2320 6874 7470 733a 2f2f 7079 7468    # https://pyth
-00000d00: 6f6e 6775 6964 6573 2e63 6f6d 2f6d 6174  onguides.com/mat
-00000d10: 706c 6f74 6c69 622d 7265 6d6f 7665 2d74  plotlib-remove-t
-00000d20: 6963 6b2d 6c61 6265 6c73 0d0a 2020 2020  ick-labels..    
-00000d30: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00000d40: 6531 203d 2070 6c74 2e67 6361 2829 0d0a  e1 = plt.gca()..
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 6672 616d 6531 2e61 7865 732e 7861 7869  frame1.axes.xaxi
-00000d70: 732e 7365 745f 7469 636b 6c61 6265 6c73  s.set_ticklabels
-00000d80: 285b 5d29 0d0a 2020 2020 2020 2020 2020  ([])..          
-00000d90: 2020 2020 2020 6672 616d 6531 2e61 7865        frame1.axe
-00000da0: 732e 7961 7869 732e 7365 745f 7469 636b  s.yaxis.set_tick
-00000db0: 6c61 6265 6c73 285b 5d29 0d0a 2020 2020  labels([])..    
-00000dc0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00000dd0: 7469 636b 5f70 6172 616d 7328 6c65 6674  tick_params(left
-00000de0: 3d46 616c 7365 2c20 626f 7474 6f6d 3d46  =False, bottom=F
-00000df0: 616c 7365 290d 0a0d 0a20 2020 2020 2020  alse)....       
-00000e00: 2020 2020 2020 2020 2068 6973 746f 6772           histogr
-00000e10: 616d 203d 205f 706e 675f 746f 5f68 746d  am = _png_to_htm
-00000e20: 6c28 5f70 6c74 5f74 6f5f 706e 6728 2929  l(_plt_to_png())
-00000e30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000e40: 6d69 6e5f 6d61 7820 3d20 223c 7472 3e3c  min_max = "<tr><
-00000e50: 7464 3e6d 696e 3c2f 7464 3e3c 7464 3e22  td>min</td><td>"
-00000e60: 202b 2073 7472 2873 656c 662e 6d69 6e28   + str(self.min(
-00000e70: 2929 202b 2022 3c2f 7464 3e3c 2f74 723e  )) + "</td></tr>
-00000e80: 2220 2b20 5c0d 0a20 2020 2020 2020 2020  " + \..         
-00000e90: 2020 2020 2020 2020 2020 2020 2022 3c74               "<t
-00000ea0: 723e 3c74 643e 6d61 783c 2f74 643e 3c74  r><td>max</td><t
-00000eb0: 643e 2220 2b20 7374 7228 7365 6c66 2e6d  d>" + str(self.m
-00000ec0: 6178 2829 2920 2b20 223c 2f74 643e 3c2f  ax()) + "</td></
-00000ed0: 7472 3e22 0d0a 0d0a 2020 2020 2020 2020  tr>"....        
-00000ee0: 656c 7365 3a0d 0a0d 0a20 2020 2020 2020  else:....       
-00000ef0: 2020 2020 206d 696e 5f6d 6178 203d 2022       min_max = "
-00000f00: 220d 0a0d 0a20 2020 2020 2020 2068 656c  "....        hel
-00000f10: 705f 7465 7874 203d 2022 220d 0a20 2020  p_text = ""..   
-00000f20: 2020 2020 2069 6620 7365 6c66 2e6c 6962       if self.lib
-00000f30: 7261 7279 5f6e 616d 6520 6973 206e 6f74  rary_name is not
-00000f40: 204e 6f6e 6520 616e 6420 6c65 6e28 7365   None and len(se
-00000f50: 6c66 2e6c 6962 7261 7279 5f6e 616d 6529  lf.library_name)
-00000f60: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00000f70: 2020 2073 656c 662e 6c69 6272 6172 795f     self.library_
-00000f80: 6e61 6d65 203d 2073 656c 662e 6c69 6272  name = self.libr
-00000f90: 6172 795f 6e61 6d65 202b 2022 206d 6164  ary_name + " mad
-00000fa0: 6520 220d 0a20 2020 2020 2020 2020 2020  e "..           
-00000fb0: 2069 6620 7365 6c66 2e68 656c 705f 7572   if self.help_ur
-00000fc0: 6c20 6973 206e 6f74 204e 6f6e 653a 0d0a  l is not None:..
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fe0: 6865 6c70 5f74 6578 7420 3d20 223c 623e  help_text = "<b>
-00000ff0: 3c61 2068 7265 663d 5c22 2220 2b20 7365  <a href=\"" + se
-00001000: 6c66 2e68 656c 705f 7572 6c20 2b20 225c  lf.help_url + "\
-00001010: 2220 7461 7267 6574 3d5c 225f 626c 616e  " target=\"_blan
-00001020: 6b5c 223e 2220 2b20 7365 6c66 2e6c 6962  k\">" + self.lib
-00001030: 7261 7279 5f6e 616d 6520 2b20 223c 2f61  rary_name + "</a
-00001040: 3e69 6d61 6765 3c2f 623e 3c62 722f 3e22  >image</b><br/>"
-00001050: 0d0a 0d0a 2020 2020 2020 2020 616c 6c20  ....        all 
-00001060: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-00001070: 2022 3c74 6162 6c65 3e22 2c0d 0a20 2020   "<table>",..   
-00001080: 2020 2020 2020 2020 2022 3c74 723e 222c           "<tr>",
-00001090: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
-000010a0: 7464 3e22 2c0d 0a20 2020 2020 2020 2020  td>",..         
-000010b0: 2020 2069 6d61 6765 2c0d 0a20 2020 2020     image,..     
-000010c0: 2020 2020 2020 2022 3c2f 7464 3e22 2c0d         "</td>",.
+00000700: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00000710: 7365 6c66 2e73 6861 7065 2920 3c20 323a  self.shape) < 2:
+00000720: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000730: 7475 726e 2073 7472 2873 656c 6629 0d0a  turn str(self)..
+00000740: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+00000750: 206e 756d 7079 2061 7320 6e70 0d0a 2020   numpy as np..  
+00000760: 2020 2020 2020 7369 7a65 5f69 6e5f 7069        size_in_pi
+00000770: 7865 6c73 203d 206e 702e 7072 6f64 2873  xels = np.prod(s
+00000780: 656c 662e 7368 6170 6529 0d0a 2020 2020  elf.shape)..    
+00000790: 2020 2020 7369 7a65 5f69 6e5f 6279 7465      size_in_byte
+000007a0: 7320 3d20 7369 7a65 5f69 6e5f 7069 7865  s = size_in_pixe
+000007b0: 6c73 202a 2073 656c 662e 6474 7970 652e  ls * self.dtype.
+000007c0: 6974 656d 7369 7a65 0d0a 0d0a 2020 2020  itemsize....    
+000007d0: 2020 2020 6672 6f6d 202e 5f69 6d61 6765      from ._image
+000007e0: 5f77 6964 6765 7420 696d 706f 7274 205f  _widget import _
+000007f0: 6973 5f6c 6162 656c 5f69 6d61 6765 0d0a  is_label_image..
+00000800: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
+00000810: 205f 6973 5f6c 6162 656c 5f69 6d61 6765   _is_label_image
+00000820: 2873 656c 6629 0d0a 0d0a 2020 2020 2020  (self)....      
+00000830: 2020 696d 706f 7274 206d 6174 706c 6f74    import matplot
+00000840: 6c69 622e 7079 706c 6f74 2061 7320 706c  lib.pyplot as pl
+00000850: 740d 0a20 2020 2020 2020 205f 696d 7368  t..        _imsh
+00000860: 6f77 2873 656c 662c 0d0a 2020 2020 2020  ow(self,..      
+00000870: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
+00000880: 3d6c 6162 656c 732c 0d0a 2020 2020 2020  =labels,..      
+00000890: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+000008a0: 7565 5f64 7261 7769 6e67 3d54 7275 652c  ue_drawing=True,
+000008b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000008c0: 2020 636f 6c6f 7262 6172 3d6e 6f74 206c    colorbar=not l
+000008d0: 6162 656c 7329 0d0a 2020 2020 2020 2020  abels)..        
+000008e0: 696d 6167 6520 3d20 5f70 6e67 5f74 6f5f  image = _png_to_
+000008f0: 6874 6d6c 285f 706c 745f 746f 5f70 6e67  html(_plt_to_png
+00000900: 2829 290d 0a0d 0a20 2020 2020 2020 2069  ())....        i
+00000910: 6620 7369 7a65 5f69 6e5f 6279 7465 7320  f size_in_bytes 
+00000920: 3e20 3130 3234 3a0d 0a20 2020 2020 2020  > 1024:..       
+00000930: 2020 2020 2073 697a 655f 696e 5f62 7974       size_in_byt
+00000940: 6573 203d 2073 697a 655f 696e 5f62 7974  es = size_in_byt
+00000950: 6573 202f 2031 3032 340d 0a20 2020 2020  es / 1024..     
+00000960: 2020 2020 2020 2069 6620 7369 7a65 5f69         if size_i
+00000970: 6e5f 6279 7465 7320 3e20 3130 3234 3a0d  n_bytes > 1024:.
+00000980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000990: 2073 697a 655f 696e 5f62 7974 6573 203d   size_in_bytes =
+000009a0: 2073 697a 655f 696e 5f62 7974 6573 202f   size_in_bytes /
+000009b0: 2031 3032 340d 0a20 2020 2020 2020 2020   1024..         
+000009c0: 2020 2020 2020 2069 6620 7369 7a65 5f69         if size_i
+000009d0: 6e5f 6279 7465 7320 3e20 3130 3234 3a0d  n_bytes > 1024:.
+000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009f0: 2020 2020 2073 697a 655f 696e 5f62 7974       size_in_byt
+00000a00: 6573 203d 2073 697a 655f 696e 5f62 7974  es = size_in_byt
+00000a10: 6573 202f 2031 3032 340d 0a20 2020 2020  es / 1024..     
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000a30: 697a 6520 3d20 227b 3a2e 3166 7d22 2e66  ize = "{:.1f}".f
+00000a40: 6f72 6d61 7428 7369 7a65 5f69 6e5f 6279  ormat(size_in_by
+00000a50: 7465 7329 202b 2022 2047 4222 0d0a 2020  tes) + " GB"..  
+00000a60: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00000a70: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000a80: 2020 2020 2020 2020 2073 697a 6520 3d20           size = 
+00000a90: 227b 3a2e 3166 7d22 2e66 6f72 6d61 7428  "{:.1f}".format(
+00000aa0: 7369 7a65 5f69 6e5f 6279 7465 7329 202b  size_in_bytes) +
+00000ab0: 2022 204d 4222 0d0a 2020 2020 2020 2020   " MB"..        
+00000ac0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000ad0: 2020 2020 2020 2020 2020 2073 697a 6520             size 
+00000ae0: 3d20 227b 3a2e 3166 7d22 2e66 6f72 6d61  = "{:.1f}".forma
+00000af0: 7428 7369 7a65 5f69 6e5f 6279 7465 7329  t(size_in_bytes)
+00000b00: 202b 2022 206b 4222 0d0a 2020 2020 2020   + " kB"..      
+00000b10: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000b20: 2020 2020 2073 697a 6520 3d20 227b 3a2e       size = "{:.
+00000b30: 3166 7d22 2e66 6f72 6d61 7428 7369 7a65  1f}".format(size
+00000b40: 5f69 6e5f 6279 7465 7329 202b 2022 2042  _in_bytes) + " B
+00000b50: 220d 0a0d 0a20 2020 2020 2020 2068 6973  "....        his
+00000b60: 746f 6772 616d 203d 2022 220d 0a0d 0a20  togram = "".... 
+00000b70: 2020 2020 2020 2069 6620 7369 7a65 5f69         if size_i
+00000b80: 6e5f 6279 7465 7320 3c20 3130 3020 2a20  n_bytes < 100 * 
+00000b90: 3130 3234 202a 2031 3032 343a 0d0a 2020  1024 * 1024:..  
+00000ba0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00000bb0: 206c 6162 656c 733a 0d0a 2020 2020 2020   labels:..      
+00000bc0: 2020 2020 2020 2020 2020 696d 706f 7274            import
+00000bd0: 206e 756d 7079 2061 7320 6e70 0d0a 0d0a   numpy as np....
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bf0: 6e75 6d5f 6269 6e73 203d 2033 320d 0a20  num_bins = 32.. 
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00000c10: 2c20 5f20 3d20 6e70 2e68 6973 746f 6772  , _ = np.histogr
+00000c20: 616d 2873 656c 662c 2062 696e 733d 6e75  am(self, bins=nu
+00000c30: 6d5f 6269 6e73 290d 0a0d 0a20 2020 2020  m_bins)....     
+00000c40: 2020 2020 2020 2020 2020 2070 6c74 2e66             plt.f
+00000c50: 6967 7572 6528 6669 6773 697a 653d 2831  igure(figsize=(1
+00000c60: 2e38 2c20 312e 3229 290d 0a20 2020 2020  .8, 1.2))..     
+00000c70: 2020 2020 2020 2020 2020 2070 6c74 2e62             plt.b
+00000c80: 6172 2872 616e 6765 2830 2c20 6c65 6e28  ar(range(0, len(
+00000c90: 6829 292c 2068 290d 0a0d 0a20 2020 2020  h)), h)....     
+00000ca0: 2020 2020 2020 2020 2020 2023 2068 6964             # hid
+00000cb0: 6520 6178 6973 2074 6578 740d 0a20 2020  e axis text..   
+00000cc0: 2020 2020 2020 2020 2020 2020 2023 2068               # h
+00000cd0: 7474 7073 3a2f 2f73 7461 636b 6f76 6572  ttps://stackover
+00000ce0: 666c 6f77 2e63 6f6d 2f71 7565 7374 696f  flow.com/questio
+00000cf0: 6e73 2f32 3137 3634 3234 2f68 6964 696e  ns/2176424/hidin
+00000d00: 672d 6178 6973 2d74 6578 742d 696e 2d6d  g-axis-text-in-m
+00000d10: 6174 706c 6f74 6c69 622d 706c 6f74 730d  atplotlib-plots.
+00000d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d30: 2023 2068 7474 7073 3a2f 2f70 7974 686f   # https://pytho
+00000d40: 6e67 7569 6465 732e 636f 6d2f 6d61 7470  nguides.com/matp
+00000d50: 6c6f 746c 6962 2d72 656d 6f76 652d 7469  lotlib-remove-ti
+00000d60: 636b 2d6c 6162 656c 730d 0a20 2020 2020  ck-labels..     
+00000d70: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+00000d80: 3120 3d20 706c 742e 6763 6128 290d 0a20  1 = plt.gca().. 
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000da0: 7261 6d65 312e 6178 6573 2e78 6178 6973  rame1.axes.xaxis
+00000db0: 2e73 6574 5f74 6963 6b6c 6162 656c 7328  .set_ticklabels(
+00000dc0: 5b5d 290d 0a20 2020 2020 2020 2020 2020  [])..           
+00000dd0: 2020 2020 2066 7261 6d65 312e 6178 6573       frame1.axes
+00000de0: 2e79 6178 6973 2e73 6574 5f74 6963 6b6c  .yaxis.set_tickl
+00000df0: 6162 656c 7328 5b5d 290d 0a20 2020 2020  abels([])..     
+00000e00: 2020 2020 2020 2020 2020 2070 6c74 2e74             plt.t
+00000e10: 6963 6b5f 7061 7261 6d73 286c 6566 743d  ick_params(left=
+00000e20: 4661 6c73 652c 2062 6f74 746f 6d3d 4661  False, bottom=Fa
+00000e30: 6c73 6529 0d0a 0d0a 2020 2020 2020 2020  lse)....        
+00000e40: 2020 2020 2020 2020 6869 7374 6f67 7261          histogra
+00000e50: 6d20 3d20 5f70 6e67 5f74 6f5f 6874 6d6c  m = _png_to_html
+00000e60: 285f 706c 745f 746f 5f70 6e67 2829 290d  (_plt_to_png()).
+00000e70: 0a0d 0a20 2020 2020 2020 2020 2020 206d  ...            m
+00000e80: 696e 5f6d 6178 203d 2022 3c74 723e 3c74  in_max = "<tr><t
+00000e90: 643e 6d69 6e3c 2f74 643e 3c74 643e 2220  d>min</td><td>" 
+00000ea0: 2b20 7374 7228 7365 6c66 2e6d 696e 2829  + str(self.min()
+00000eb0: 2920 2b20 223c 2f74 643e 3c2f 7472 3e22  ) + "</td></tr>"
+00000ec0: 202b 205c 0d0a 2020 2020 2020 2020 2020   + \..          
+00000ed0: 2020 2020 2020 2020 2020 2020 223c 7472              "<tr
+00000ee0: 3e3c 7464 3e6d 6178 3c2f 7464 3e3c 7464  ><td>max</td><td
+00000ef0: 3e22 202b 2073 7472 2873 656c 662e 6d61  >" + str(self.ma
+00000f00: 7828 2929 202b 2022 3c2f 7464 3e3c 2f74  x()) + "</td></t
+00000f10: 723e 220d 0a0d 0a20 2020 2020 2020 2065  r>"....        e
+00000f20: 6c73 653a 0d0a 0d0a 2020 2020 2020 2020  lse:....        
+00000f30: 2020 2020 6d69 6e5f 6d61 7820 3d20 2222      min_max = ""
+00000f40: 0d0a 0d0a 2020 2020 2020 2020 6865 6c70  ....        help
+00000f50: 5f74 6578 7420 3d20 2222 0d0a 2020 2020  _text = ""..    
+00000f60: 2020 2020 6966 2073 656c 662e 6c69 6272      if self.libr
+00000f70: 6172 795f 6e61 6d65 2069 7320 6e6f 7420  ary_name is not 
+00000f80: 4e6f 6e65 2061 6e64 206c 656e 2873 656c  None and len(sel
+00000f90: 662e 6c69 6272 6172 795f 6e61 6d65 2920  f.library_name) 
+00000fa0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+00000fb0: 2020 7365 6c66 2e6c 6962 7261 7279 5f6e    self.library_n
+00000fc0: 616d 6520 3d20 7365 6c66 2e6c 6962 7261  ame = self.libra
+00000fd0: 7279 5f6e 616d 6520 2b20 2220 6d61 6465  ry_name + " made
+00000fe0: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
+00000ff0: 6966 2073 656c 662e 6865 6c70 5f75 726c  if self.help_url
+00001000: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00001010: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00001020: 656c 705f 7465 7874 203d 2022 3c62 3e3c  elp_text = "<b><
+00001030: 6120 6872 6566 3d5c 2222 202b 2073 656c  a href=\"" + sel
+00001040: 662e 6865 6c70 5f75 726c 202b 2022 5c22  f.help_url + "\"
+00001050: 2074 6172 6765 743d 5c22 5f62 6c61 6e6b   target=\"_blank
+00001060: 5c22 3e22 202b 2073 656c 662e 6c69 6272  \">" + self.libr
+00001070: 6172 795f 6e61 6d65 202b 2022 3c2f 613e  ary_name + "</a>
+00001080: 696d 6167 653c 2f62 3e3c 6272 2f3e 220d  image</b><br/>".
+00001090: 0a0d 0a20 2020 2020 2020 2061 6c6c 203d  ...        all =
+000010a0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+000010b0: 223c 7461 626c 653e 222c 0d0a 2020 2020  "<table>",..    
+000010c0: 2020 2020 2020 2020 223c 7472 3e22 2c0d          "<tr>",.
 000010d0: 0a20 2020 2020 2020 2020 2020 2022 3c74  .            "<t
-000010e0: 6420 7374 796c 653d 5c22 7465 7874 2d61  d style=\"text-a
-000010f0: 6c69 676e 3a20 6365 6e74 6572 3b20 7665  lign: center; ve
-00001100: 7274 6963 616c 2d61 6c69 676e 3a20 746f  rtical-align: to
-00001110: 703b 5c22 3e22 2c0d 0a20 2020 2020 2020  p;\">",..       
-00001120: 2020 2020 2068 656c 705f 7465 7874 2c0d       help_text,.
-00001130: 0a20 2020 2020 2020 2020 2020 2022 3c74  .            "<t
-00001140: 6162 6c65 3e22 2c0d 0a20 2020 2020 2020  able>",..       
-00001150: 2020 2020 2022 3c74 723e 3c74 643e 7368       "<tr><td>sh
-00001160: 6170 653c 2f74 643e 3c74 643e 2220 2b20  ape</td><td>" + 
-00001170: 7374 7228 7365 6c66 2e73 6861 7065 292e  str(self.shape).
-00001180: 7265 706c 6163 6528 2220 222c 2022 266e  replace(" ", "&n
-00001190: 6273 703b 2229 202b 2022 3c2f 7464 3e3c  bsp;") + "</td><
-000011a0: 2f74 723e 222c 0d0a 2020 2020 2020 2020  /tr>",..        
-000011b0: 2020 2020 223c 7472 3e3c 7464 3e64 7479      "<tr><td>dty
-000011c0: 7065 3c2f 7464 3e3c 7464 3e22 202b 2073  pe</td><td>" + s
-000011d0: 7472 2873 656c 662e 6474 7970 6529 202b  tr(self.dtype) +
-000011e0: 2022 3c2f 7464 3e3c 2f74 723e 222c 0d0a   "</td></tr>",..
-000011f0: 2020 2020 2020 2020 2020 2020 223c 7472              "<tr
-00001200: 3e3c 7464 3e73 697a 653c 2f74 643e 3c74  ><td>size</td><t
-00001210: 643e 2220 2b20 7369 7a65 202b 2022 3c2f  d>" + size + "</
-00001220: 7464 3e3c 2f74 723e 222c 0d0a 2020 2020  td></tr>",..    
-00001230: 2020 2020 2020 2020 6d69 6e5f 6d61 782c          min_max,
-00001240: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
-00001250: 2f74 6162 6c65 3e22 2c0d 0a20 2020 2020  /table>",..     
-00001260: 2020 2020 2020 2068 6973 746f 6772 616d         histogram
-00001270: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001280: 3c2f 7464 3e22 2c0d 0a20 2020 2020 2020  </td>",..       
-00001290: 2020 2020 2022 3c2f 7472 3e22 2c0d 0a20       "</tr>",.. 
-000012a0: 2020 2020 2020 2020 2020 2022 3c2f 7461             "</ta
-000012b0: 626c 653e 222c 0d0a 2020 2020 2020 2020  ble>",..        
-000012c0: 5d0d 0a0d 0a20 2020 2020 2020 2072 6574  ]....        ret
-000012d0: 7572 6e20 225c 6e22 2e6a 6f69 6e28 616c  urn "\n".join(al
-000012e0: 6c29 0d0a 0d0a 0d0a 6465 6620 5f70 6e67  l)......def _png
-000012f0: 5f74 6f5f 6874 6d6c 2870 6e67 293a 0d0a  _to_html(png):..
-00001300: 2020 2020 696d 706f 7274 2062 6173 6536      import base6
-00001310: 340d 0a20 2020 2075 726c 203d 2027 6461  4..    url = 'da
-00001320: 7461 3a69 6d61 6765 2f70 6e67 3b62 6173  ta:image/png;bas
-00001330: 6536 342c 2720 2b20 6261 7365 3634 2e62  e64,' + base64.b
-00001340: 3634 656e 636f 6465 2870 6e67 292e 6465  64encode(png).de
-00001350: 636f 6465 2827 7574 662d 3827 290d 0a20  code('utf-8').. 
-00001360: 2020 2072 6574 7572 6e20 6627 3c69 6d67     return f'<img
-00001370: 2073 7263 3d22 7b75 726c 7d22 3e3c 2f69   src="{url}"></i
-00001380: 6d67 3e27 0d0a 0d0a 0d0a 2320 6164 6170  mg>'......# adap
-00001390: 7465 6420 6672 6f6d 2068 7474 7073 3a2f  ted from https:/
-000013a0: 2f67 6974 6875 622e 636f 6d2f 6e61 7061  /github.com/napa
-000013b0: 7269 2f6e 6170 6172 692f 626c 6f62 2f64  ri/napari/blob/d
-000013c0: 3662 6336 3833 6230 3139 6334 6133 6133  6bc683b019c4a3a3
-000013d0: 6336 6539 3336 3532 3665 3239 6262 6435  c6e936526e29bbd5
-000013e0: 3963 6361 3266 342f 6e61 7061 7269 2f75  9cca2f4/napari/u
-000013f0: 7469 6c73 2f6e 6f74 6562 6f6f 6b5f 6469  tils/notebook_di
-00001400: 7370 6c61 792e 7079 234c 3534 2d4c 3733  splay.py#L54-L73
-00001410: 0d0a 6465 6620 5f70 6c74 5f74 6f5f 706e  ..def _plt_to_pn
-00001420: 6728 293a 0d0a 2020 2020 2222 2250 4e47  g():..    """PNG
-00001430: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00001440: 6f66 2074 6865 2069 6d61 6765 206f 626a  of the image obj
-00001450: 6563 7420 666f 7220 4950 7974 686f 6e2e  ect for IPython.
-00001460: 0d0a 2020 2020 5265 7475 726e 730d 0a20  ..    Returns.. 
-00001470: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-00001480: 496e 206d 656d 6f72 7920 6269 6e61 7279  In memory binary
-00001490: 2073 7472 6561 6d20 636f 6e74 6169 6e69   stream containi
-000014a0: 6e67 2061 2050 4e47 206d 6174 706c 6f74  ng a PNG matplot
-000014b0: 6c69 6220 696d 6167 652e 0d0a 2020 2020  lib image...    
-000014c0: 2222 220d 0a20 2020 2069 6d70 6f72 7420  """..    import 
-000014d0: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-000014e0: 7420 6173 2070 6c74 0d0a 2020 2020 6672  t as plt..    fr
-000014f0: 6f6d 2069 6f20 696d 706f 7274 2042 7974  om io import Byt
-00001500: 6573 494f 0d0a 0d0a 2020 2020 7769 7468  esIO....    with
-00001510: 2042 7974 6573 494f 2829 2061 7320 6669   BytesIO() as fi
-00001520: 6c65 5f6f 626a 3a0d 0a20 2020 2020 2020  le_obj:..       
-00001530: 2070 6c74 2e73 6176 6566 6967 2866 696c   plt.savefig(fil
-00001540: 655f 6f62 6a2c 2066 6f72 6d61 743d 2770  e_obj, format='p
-00001550: 6e67 2729 0d0a 2020 2020 2020 2020 706c  ng')..        pl
-00001560: 742e 636c 6f73 6528 2920 2320 7375 7072  t.close() # supr
-00001570: 6573 7320 706c 6f74 206f 7574 7075 740d  ess plot output.
-00001580: 0a20 2020 2020 2020 2066 696c 655f 6f62  .        file_ob
-00001590: 6a2e 7365 656b 2830 290d 0a20 2020 2020  j.seek(0)..     
-000015a0: 2020 2070 6e67 203d 2066 696c 655f 6f62     png = file_ob
-000015b0: 6a2e 7265 6164 2829 0d0a 2020 2020 7265  j.read()..    re
-000015c0: 7475 726e 2070 6e67 0d0a 0d0a 0d0a 6465  turn png......de
-000015d0: 6620 5f69 6d73 686f 7728 696d 6167 652c  f _imshow(image,
-000015e0: 2074 6974 6c65 3a20 7374 7220 3d20 4e6f   title: str = No
-000015f0: 6e65 2c20 6c61 6265 6c73 3a20 626f 6f6c  ne, labels: bool
-00001600: 203d 2046 616c 7365 2c20 6d69 6e5f 6469   = False, min_di
-00001610: 7370 6c61 795f 696e 7465 6e73 6974 793a  splay_intensity:
-00001620: 2066 6c6f 6174 203d 204e 6f6e 652c 0d0a   float = None,..
-00001630: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00001640: 6469 7370 6c61 795f 696e 7465 6e73 6974  display_intensit
-00001650: 793a 2066 6c6f 6174 203d 204e 6f6e 652c  y: float = None,
-00001660: 2070 6c6f 743d 4e6f 6e65 2c20 636f 6c6f   plot=None, colo
-00001670: 7262 6172 3a20 626f 6f6c 203d 2046 616c  rbar: bool = Fal
-00001680: 7365 2c20 636f 6c6f 726d 6170 3d4e 6f6e  se, colormap=Non
-00001690: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000016a0: 616c 7068 613a 2066 6c6f 6174 203d 204e  alpha: float = N
-000016b0: 6f6e 652c 2063 6f6e 7469 6e75 655f 6472  one, continue_dr
-000016c0: 6177 696e 673a 2062 6f6f 6c20 3d20 4661  awing: bool = Fa
-000016d0: 6c73 6529 3a0d 0a20 2020 2022 2222 5669  lse):..    """Vi
-000016e0: 7375 616c 697a 6520 616e 2069 6d61 6765  sualize an image
-000016f0: 2c20 652e 672e 2069 6e20 4a75 7079 7465  , e.g. in Jupyte
-00001700: 7220 6e6f 7465 626f 6f6b 732e 0d0a 0d0a  r notebooks.....
-00001710: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00001720: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00001730: 2020 2020 696d 6167 653a 206e 702e 6e64      image: np.nd
-00001740: 6172 7261 790d 0a20 2020 2020 2020 206e  array..        n
-00001750: 756d 7079 206f 7220 4f70 656e 434c 2d62  umpy or OpenCL-b
-00001760: 6163 6b65 6420 696d 6167 6520 746f 2076  acked image to v
-00001770: 6973 7561 6c69 7a65 0d0a 2020 2020 7469  isualize..    ti
-00001780: 746c 653a 2073 7472 0d0a 2020 2020 2020  tle: str..      
-00001790: 2020 4f62 736f 6c65 7465 2028 6b65 7074    Obsolete (kept
-000017a0: 2066 6f72 2049 6d61 6765 4a2d 636f 6d70   for ImageJ-comp
-000017b0: 6174 6962 696c 6974 7929 0d0a 2020 2020  atibility)..    
-000017c0: 6c61 6265 6c73 3a20 626f 6f6c 0d0a 2020  labels: bool..  
-000017d0: 2020 2020 2020 5472 7565 3a20 696e 7465        True: inte
-000017e0: 6765 7220 6c61 6265 6c73 2077 696c 6c20  ger labels will 
-000017f0: 6265 2076 6973 7561 6c69 7a65 6420 7769  be visualized wi
-00001800: 7468 2063 6f6c 6f72 730d 0a20 2020 2020  th colors..     
-00001810: 2020 2046 616c 7365 3a20 5370 6563 6966     False: Specif
-00001820: 6965 6420 6f72 2064 6566 6175 6c74 2063  ied or default c
-00001830: 6f6c 6f72 6d61 7020 7769 6c6c 2062 6520  olormap will be 
-00001840: 7573 6564 2074 6f20 6469 7370 6c61 7920  used to display 
-00001850: 696e 7465 6e73 6974 6965 732e 0d0a 2020  intensities...  
-00001860: 2020 6d69 6e5f 6469 7370 6c61 795f 696e    min_display_in
-00001870: 7465 6e73 6974 793a 2066 6c6f 6174 0d0a  tensity: float..
-00001880: 2020 2020 2020 2020 6c6f 7765 7220 6c69          lower li
-00001890: 6d69 7420 666f 7220 6469 7370 6c61 7920  mit for display 
-000018a0: 7261 6e67 650d 0a20 2020 206d 6178 5f64  range..    max_d
-000018b0: 6973 706c 6179 5f69 6e74 656e 7369 7479  isplay_intensity
-000018c0: 3a20 666c 6f61 740d 0a20 2020 2020 2020  : float..       
-000018d0: 2075 7070 6572 206c 696d 6974 2066 6f72   upper limit for
-000018e0: 2064 6973 706c 6179 2072 616e 6765 0d0a   display range..
-000018f0: 2020 2020 636f 6c6f 725f 6d61 703a 2073      color_map: s
-00001900: 7472 0d0a 2020 2020 2020 2020 6465 7072  tr..        depr
-00001910: 6563 6174 6564 2c20 7573 6520 636f 6c6f  ecated, use colo
-00001920: 726d 6170 2069 6e73 7465 6164 0d0a 2020  rmap instead..  
-00001930: 2020 706c 6f74 3a20 6d61 7470 6c6f 746c    plot: matplotl
-00001940: 6962 2061 7869 730d 0a20 2020 2020 2020  ib axis..       
-00001950: 2050 6c6f 7420 6f62 6a65 6374 2077 6865   Plot object whe
-00001960: 7265 2074 6865 2069 6d61 6765 2073 686f  re the image sho
-00001970: 756c 6420 6265 2073 686f 776e 2e20 5573  uld be shown. Us
-00001980: 6566 756c 2066 6f72 2070 7574 7469 6e67  eful for putting
-00001990: 206d 756c 7469 706c 6520 696d 6167 6573   multiple images
-000019a0: 2069 6e20 7375 6266 6967 7572 6573 2e0d   in subfigures..
-000019b0: 0a20 2020 2063 6f6c 6f72 6261 723a 2062  .    colorbar: b
-000019c0: 6f6f 6c0d 0a20 2020 2020 2020 2054 7275  ool..        Tru
-000019d0: 6520 7075 7473 2061 2063 6f6c 6f72 6261  e puts a colorba
-000019e0: 7220 6e65 7874 2074 6f20 7468 6520 696d  r next to the im
-000019f0: 6167 652e 2057 696c 6c20 6e6f 7420 776f  age. Will not wo
-00001a00: 726b 2077 6974 6820 6c61 6265 6c20 696d  rk with label im
-00001a10: 6167 6573 2061 6e64 2077 6865 6e20 7669  ages and when vi
-00001a20: 7375 616c 697a 696e 6720 6d75 6c74 6970  sualizing multip
-00001a30: 6c65 0d0a 2020 2020 2020 2020 696d 6167  le..        imag
-00001a40: 6573 2028 636f 6e74 696e 7565 5f64 7261  es (continue_dra
-00001a50: 7769 6e67 3d54 7275 6529 2e0d 0a20 2020  wing=True)...   
-00001a60: 2063 6f6c 6f72 6d61 703a 2073 7472 206f   colormap: str o
-00001a70: 7220 6d61 7470 6c6f 746c 6962 2063 6f6c  r matplotlib col
-00001a80: 6f72 6d61 700d 0a20 2020 2061 6c70 6861  ormap..    alpha
-00001a90: 3a20 666c 6f61 740d 0a20 2020 2020 2020  : float..       
-00001aa0: 2061 6c70 6861 2062 6c65 6e64 696e 6720   alpha blending 
-00001ab0: 7661 6c75 650d 0a20 2020 2063 6f6e 7469  value..    conti
-00001ac0: 6e75 655f 6472 6177 696e 673a 2066 6c6f  nue_drawing: flo
-00001ad0: 6174 0d0a 2020 2020 2020 2020 5472 7565  at..        True
-00001ae0: 3a20 7468 6520 6e65 7874 2073 686f 776e  : the next shown
-00001af0: 2069 6d61 6765 2063 616e 2062 6520 7669   image can be vi
-00001b00: 7375 616c 697a 6564 206f 6e20 746f 7020  sualized on top 
-00001b10: 6f66 2074 6865 2063 7572 7265 6e74 206f  of the current o
-00001b20: 6e65 2c20 652e 672e 2077 6974 6820 616c  ne, e.g. with al
-00001b30: 7068 6120 3d20 302e 350d 0a20 2020 2022  pha = 0.5..    "
-00001b40: 2222 0d0a 2020 2020 696d 706f 7274 206e  ""..    import n
-00001b50: 756d 7079 2061 7320 6e70 0d0a 0d0a 2020  umpy as np....  
-00001b60: 2020 6966 206c 656e 2869 6d61 6765 2e73    if len(image.s
-00001b70: 6861 7065 2920 3d3d 2033 3a0d 0a20 2020  hape) == 3:..   
-00001b80: 2020 2020 2069 6d61 6765 203d 206e 702e       image = np.
-00001b90: 6173 6172 7261 7928 696d 6167 6529 2e6d  asarray(image).m
-00001ba0: 6178 2861 7869 733d 3029 0d0a 0d0a 2020  ax(axis=0)....  
-00001bb0: 2020 696d 6167 6520 3d20 6e70 2e61 7361    image = np.asa
-00001bc0: 7272 6179 2869 6d61 6765 290d 0a20 2020  rray(image)..   
-00001bd0: 2069 6620 6c65 6e28 696d 6167 652e 7368   if len(image.sh
-00001be0: 6170 6529 203d 3d20 313a 0d0a 2020 2020  ape) == 1:..    
-00001bf0: 2020 2020 696d 6167 6520 3d20 696d 6167      image = imag
-00001c00: 655b 6e70 2e6e 6577 6178 6973 5d0d 0a0d  e[np.newaxis]...
-00001c10: 0a20 2020 2069 6620 636f 6c6f 726d 6170  .    if colormap
-00001c20: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00001c30: 2020 2063 6f6c 6f72 6d61 7020 3d20 2247     colormap = "G
-00001c40: 7265 7973 5f72 220d 0a0d 0a20 2020 2063  reys_r"....    c
-00001c50: 6d61 7020 3d20 636f 6c6f 726d 6170 0d0a  map = colormap..
-00001c60: 2020 2020 6966 206c 6162 656c 733a 0d0a      if labels:..
-00001c70: 2020 2020 2020 2020 696d 706f 7274 206d          import m
-00001c80: 6174 706c 6f74 6c69 620d 0a20 2020 2020  atplotlib..     
-00001c90: 2020 2069 6d70 6f72 7420 6e75 6d70 7920     import numpy 
-00001ca0: 6173 206e 700d 0a0d 0a20 2020 2020 2020  as np....       
-00001cb0: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-00001cc0: 5f69 6d73 686f 772c 2022 6c61 6265 6c73  _imshow, "labels
-00001cd0: 5f63 6d61 7022 293a 0d0a 2020 2020 2020  _cmap"):..      
-00001ce0: 2020 2020 2020 6672 6f6d 202e 5f69 6d61        from ._ima
-00001cf0: 6765 5f77 6964 6765 7420 696d 706f 7274  ge_widget import
-00001d00: 205f 6c61 6265 6c73 5f6c 7574 0d0a 2020   _labels_lut..  
-00001d10: 2020 2020 2020 2020 2020 5f69 6d73 686f            _imsho
-00001d20: 772e 6c61 6265 6c73 5f63 6d61 7020 3d20  w.labels_cmap = 
-00001d30: 6d61 7470 6c6f 746c 6962 2e63 6f6c 6f72  matplotlib.color
-00001d40: 732e 4c69 7374 6564 436f 6c6f 726d 6170  s.ListedColormap
-00001d50: 285f 6c61 6265 6c73 5f6c 7574 2829 290d  (_labels_lut()).
-00001d60: 0a20 2020 2020 2020 2063 6d61 7020 3d20  .        cmap = 
-00001d70: 5f69 6d73 686f 772e 6c61 6265 6c73 5f63  _imshow.labels_c
-00001d80: 6d61 700d 0a0d 0a20 2020 2020 2020 2069  map....        i
-00001d90: 6620 6d69 6e5f 6469 7370 6c61 795f 696e  f min_display_in
-00001da0: 7465 6e73 6974 7920 6973 204e 6f6e 653a  tensity is None:
-00001db0: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-00001dc0: 6e5f 6469 7370 6c61 795f 696e 7465 6e73  n_display_intens
-00001dd0: 6974 7920 3d20 300d 0a20 2020 2020 2020  ity = 0..       
-00001de0: 2069 6620 6d61 785f 6469 7370 6c61 795f   if max_display_
-00001df0: 696e 7465 6e73 6974 7920 6973 204e 6f6e  intensity is Non
-00001e00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001e10: 6d61 785f 6469 7370 6c61 795f 696e 7465  max_display_inte
-00001e20: 6e73 6974 7920 3d20 3635 3533 360d 0a0d  nsity = 65536...
-00001e30: 0a20 2020 2069 6620 706c 6f74 2069 7320  .    if plot is 
-00001e40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-00001e50: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
-00001e60: 2e70 7970 6c6f 7420 6173 2070 6c74 0d0a  .pyplot as plt..
-00001e70: 2020 2020 2020 2020 706c 742e 696d 7368          plt.imsh
-00001e80: 6f77 2869 6d61 6765 2c20 636d 6170 3d63  ow(image, cmap=c
-00001e90: 6d61 702c 2076 6d69 6e3d 6d69 6e5f 6469  map, vmin=min_di
-00001ea0: 7370 6c61 795f 696e 7465 6e73 6974 792c  splay_intensity,
-00001eb0: 2076 6d61 783d 6d61 785f 6469 7370 6c61   vmax=max_displa
-00001ec0: 795f 696e 7465 6e73 6974 792c 0d0a 2020  y_intensity,..  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2069 6e74 6572 706f 6c61 7469 6f6e 3d27   interpolation='
-00001ef0: 6e65 6172 6573 7427 2c20 616c 7068 613d  nearest', alpha=
-00001f00: 616c 7068 6129 0d0a 2020 2020 2020 2020  alpha)..        
-00001f10: 6966 2063 6f6c 6f72 6261 723a 0d0a 2020  if colorbar:..  
-00001f20: 2020 2020 2020 2020 2020 706c 742e 636f            plt.co
-00001f30: 6c6f 7262 6172 2829 0d0a 2020 2020 2020  lorbar()..      
-00001f40: 2020 6966 206e 6f74 2063 6f6e 7469 6e75    if not continu
-00001f50: 655f 6472 6177 696e 673a 0d0a 2020 2020  e_drawing:..    
-00001f60: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
-00001f70: 2829 0d0a 2020 2020 656c 7365 3a0d 0a20  ()..    else:.. 
-00001f80: 2020 2020 2020 2070 6c6f 742e 696d 7368         plot.imsh
-00001f90: 6f77 2869 6d61 6765 2c20 636d 6170 3d63  ow(image, cmap=c
-00001fa0: 6d61 702c 2076 6d69 6e3d 6d69 6e5f 6469  map, vmin=min_di
-00001fb0: 7370 6c61 795f 696e 7465 6e73 6974 792c  splay_intensity,
-00001fc0: 2076 6d61 783d 6d61 785f 6469 7370 6c61   vmax=max_displa
-00001fd0: 795f 696e 7465 6e73 6974 792c 0d0a 2020  y_intensity,..  
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ff0: 2020 696e 7465 7270 6f6c 6174 696f 6e3d    interpolation=
-00002000: 276e 6561 7265 7374 272c 2061 6c70 6861  'nearest', alpha
-00002010: 3d61 6c70 6861 290d 0a20 2020 2020 2020  =alpha)..       
-00002020: 2069 6620 636f 6c6f 7262 6172 3a0d 0a20   if colorbar:.. 
-00002030: 2020 2020 2020 2020 2020 2070 6c6f 742e             plot.
-00002040: 636f 6c6f 7262 6172 2829                 colorbar()
+000010e0: 643e 222c 0d0a 2020 2020 2020 2020 2020  d>",..          
+000010f0: 2020 696d 6167 652c 0d0a 2020 2020 2020    image,..      
+00001100: 2020 2020 2020 223c 2f74 643e 222c 0d0a        "</td>",..
+00001110: 2020 2020 2020 2020 2020 2020 223c 7464              "<td
+00001120: 2073 7479 6c65 3d5c 2274 6578 742d 616c   style=\"text-al
+00001130: 6967 6e3a 2063 656e 7465 723b 2076 6572  ign: center; ver
+00001140: 7469 6361 6c2d 616c 6967 6e3a 2074 6f70  tical-align: top
+00001150: 3b5c 223e 222c 0d0a 2020 2020 2020 2020  ;\">",..        
+00001160: 2020 2020 6865 6c70 5f74 6578 742c 0d0a      help_text,..
+00001170: 2020 2020 2020 2020 2020 2020 223c 7461              "<ta
+00001180: 626c 653e 222c 0d0a 2020 2020 2020 2020  ble>",..        
+00001190: 2020 2020 223c 7472 3e3c 7464 3e73 6861      "<tr><td>sha
+000011a0: 7065 3c2f 7464 3e3c 7464 3e22 202b 2073  pe</td><td>" + s
+000011b0: 7472 2873 656c 662e 7368 6170 6529 2e72  tr(self.shape).r
+000011c0: 6570 6c61 6365 2822 2022 2c20 2226 6e62  eplace(" ", "&nb
+000011d0: 7370 3b22 2920 2b20 223c 2f74 643e 3c2f  sp;") + "</td></
+000011e0: 7472 3e22 2c0d 0a20 2020 2020 2020 2020  tr>",..         
+000011f0: 2020 2022 3c74 723e 3c74 643e 6474 7970     "<tr><td>dtyp
+00001200: 653c 2f74 643e 3c74 643e 2220 2b20 7374  e</td><td>" + st
+00001210: 7228 7365 6c66 2e64 7479 7065 2920 2b20  r(self.dtype) + 
+00001220: 223c 2f74 643e 3c2f 7472 3e22 2c0d 0a20  "</td></tr>",.. 
+00001230: 2020 2020 2020 2020 2020 2022 3c74 723e             "<tr>
+00001240: 3c74 643e 7369 7a65 3c2f 7464 3e3c 7464  <td>size</td><td
+00001250: 3e22 202b 2073 697a 6520 2b20 223c 2f74  >" + size + "</t
+00001260: 643e 3c2f 7472 3e22 2c0d 0a20 2020 2020  d></tr>",..     
+00001270: 2020 2020 2020 206d 696e 5f6d 6178 2c0d         min_max,.
+00001280: 0a20 2020 2020 2020 2020 2020 2022 3c2f  .            "</
+00001290: 7461 626c 653e 222c 0d0a 2020 2020 2020  table>",..      
+000012a0: 2020 2020 2020 6869 7374 6f67 7261 6d2c        histogram,
+000012b0: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
+000012c0: 2f74 643e 222c 0d0a 2020 2020 2020 2020  /td>",..        
+000012d0: 2020 2020 223c 2f74 723e 222c 0d0a 2020      "</tr>",..  
+000012e0: 2020 2020 2020 2020 2020 223c 2f74 6162            "</tab
+000012f0: 6c65 3e22 2c0d 0a20 2020 2020 2020 205d  le>",..        ]
+00001300: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00001310: 726e 2022 5c6e 222e 6a6f 696e 2861 6c6c  rn "\n".join(all
+00001320: 290d 0a0d 0a0d 0a64 6566 205f 706e 675f  )......def _png_
+00001330: 746f 5f68 746d 6c28 706e 6729 3a0d 0a20  to_html(png):.. 
+00001340: 2020 2069 6d70 6f72 7420 6261 7365 3634     import base64
+00001350: 0d0a 2020 2020 7572 6c20 3d20 2764 6174  ..    url = 'dat
+00001360: 613a 696d 6167 652f 706e 673b 6261 7365  a:image/png;base
+00001370: 3634 2c27 202b 2062 6173 6536 342e 6236  64,' + base64.b6
+00001380: 3465 6e63 6f64 6528 706e 6729 2e64 6563  4encode(png).dec
+00001390: 6f64 6528 2775 7466 2d38 2729 0d0a 2020  ode('utf-8')..  
+000013a0: 2020 7265 7475 726e 2066 273c 696d 6720    return f'<img 
+000013b0: 7372 633d 227b 7572 6c7d 223e 3c2f 696d  src="{url}"></im
+000013c0: 673e 270d 0a0d 0a0d 0a23 2061 6461 7074  g>'......# adapt
+000013d0: 6564 2066 726f 6d20 6874 7470 733a 2f2f  ed from https://
+000013e0: 6769 7468 7562 2e63 6f6d 2f6e 6170 6172  github.com/napar
+000013f0: 692f 6e61 7061 7269 2f62 6c6f 622f 6436  i/napari/blob/d6
+00001400: 6263 3638 3362 3031 3963 3461 3361 3363  bc683b019c4a3a3c
+00001410: 3665 3933 3635 3236 6532 3962 6264 3539  6e936526e29bbd59
+00001420: 6363 6132 6634 2f6e 6170 6172 692f 7574  cca2f4/napari/ut
+00001430: 696c 732f 6e6f 7465 626f 6f6b 5f64 6973  ils/notebook_dis
+00001440: 706c 6179 2e70 7923 4c35 342d 4c37 330d  play.py#L54-L73.
+00001450: 0a64 6566 205f 706c 745f 746f 5f70 6e67  .def _plt_to_png
+00001460: 2829 3a0d 0a20 2020 2022 2222 504e 4720  ():..    """PNG 
+00001470: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00001480: 6620 7468 6520 696d 6167 6520 6f62 6a65  f the image obje
+00001490: 6374 2066 6f72 2049 5079 7468 6f6e 2e0d  ct for IPython..
+000014a0: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
+000014b0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2049    -------..    I
+000014c0: 6e20 6d65 6d6f 7279 2062 696e 6172 7920  n memory binary 
+000014d0: 7374 7265 616d 2063 6f6e 7461 696e 696e  stream containin
+000014e0: 6720 6120 504e 4720 6d61 7470 6c6f 746c  g a PNG matplotl
+000014f0: 6962 2069 6d61 6765 2e0d 0a20 2020 2022  ib image...    "
+00001500: 2222 0d0a 2020 2020 696d 706f 7274 206d  ""..    import m
+00001510: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
+00001520: 2061 7320 706c 740d 0a20 2020 2066 726f   as plt..    fro
+00001530: 6d20 696f 2069 6d70 6f72 7420 4279 7465  m io import Byte
+00001540: 7349 4f0d 0a0d 0a20 2020 2077 6974 6820  sIO....    with 
+00001550: 4279 7465 7349 4f28 2920 6173 2066 696c  BytesIO() as fil
+00001560: 655f 6f62 6a3a 0d0a 2020 2020 2020 2020  e_obj:..        
+00001570: 706c 742e 7361 7665 6669 6728 6669 6c65  plt.savefig(file
+00001580: 5f6f 626a 2c20 666f 726d 6174 3d27 706e  _obj, format='pn
+00001590: 6727 290d 0a20 2020 2020 2020 2070 6c74  g')..        plt
+000015a0: 2e63 6c6f 7365 2829 2023 2073 7570 7265  .close() # supre
+000015b0: 7373 2070 6c6f 7420 6f75 7470 7574 0d0a  ss plot output..
+000015c0: 2020 2020 2020 2020 6669 6c65 5f6f 626a          file_obj
+000015d0: 2e73 6565 6b28 3029 0d0a 2020 2020 2020  .seek(0)..      
+000015e0: 2020 706e 6720 3d20 6669 6c65 5f6f 626a    png = file_obj
+000015f0: 2e72 6561 6428 290d 0a20 2020 2072 6574  .read()..    ret
+00001600: 7572 6e20 706e 670d 0a0d 0a0d 0a64 6566  urn png......def
+00001610: 205f 696d 7368 6f77 2869 6d61 6765 2c20   _imshow(image, 
+00001620: 7469 746c 653a 2073 7472 203d 204e 6f6e  title: str = Non
+00001630: 652c 206c 6162 656c 733a 2062 6f6f 6c20  e, labels: bool 
+00001640: 3d20 4661 6c73 652c 206d 696e 5f64 6973  = False, min_dis
+00001650: 706c 6179 5f69 6e74 656e 7369 7479 3a20  play_intensity: 
+00001660: 666c 6f61 7420 3d20 4e6f 6e65 2c0d 0a20  float = None,.. 
+00001670: 2020 2020 2020 2020 2020 206d 6178 5f64             max_d
+00001680: 6973 706c 6179 5f69 6e74 656e 7369 7479  isplay_intensity
+00001690: 3a20 666c 6f61 7420 3d20 4e6f 6e65 2c20  : float = None, 
+000016a0: 706c 6f74 3d4e 6f6e 652c 2063 6f6c 6f72  plot=None, color
+000016b0: 6261 723a 2062 6f6f 6c20 3d20 4661 6c73  bar: bool = Fals
+000016c0: 652c 2063 6f6c 6f72 6d61 703d 4e6f 6e65  e, colormap=None
+000016d0: 2c0d 0a20 2020 2020 2020 2020 2020 2061  ,..            a
+000016e0: 6c70 6861 3a20 666c 6f61 7420 3d20 4e6f  lpha: float = No
+000016f0: 6e65 2c20 636f 6e74 696e 7565 5f64 7261  ne, continue_dra
+00001700: 7769 6e67 3a20 626f 6f6c 203d 2046 616c  wing: bool = Fal
+00001710: 7365 293a 0d0a 2020 2020 2222 2256 6973  se):..    """Vis
+00001720: 7561 6c69 7a65 2061 6e20 696d 6167 652c  ualize an image,
+00001730: 2065 2e67 2e20 696e 204a 7570 7974 6572   e.g. in Jupyter
+00001740: 206e 6f74 6562 6f6f 6b73 2e0d 0a0d 0a20   notebooks..... 
+00001750: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+00001760: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00001770: 2020 2069 6d61 6765 3a20 6e70 2e6e 6461     image: np.nda
+00001780: 7272 6179 0d0a 2020 2020 2020 2020 6e75  rray..        nu
+00001790: 6d70 7920 6f72 204f 7065 6e43 4c2d 6261  mpy or OpenCL-ba
+000017a0: 636b 6564 2069 6d61 6765 2074 6f20 7669  cked image to vi
+000017b0: 7375 616c 697a 650d 0a20 2020 2074 6974  sualize..    tit
+000017c0: 6c65 3a20 7374 720d 0a20 2020 2020 2020  le: str..       
+000017d0: 204f 6273 6f6c 6574 6520 286b 6570 7420   Obsolete (kept 
+000017e0: 666f 7220 496d 6167 654a 2d63 6f6d 7061  for ImageJ-compa
+000017f0: 7469 6269 6c69 7479 290d 0a20 2020 206c  tibility)..    l
+00001800: 6162 656c 733a 2062 6f6f 6c0d 0a20 2020  abels: bool..   
+00001810: 2020 2020 2054 7275 653a 2069 6e74 6567       True: integ
+00001820: 6572 206c 6162 656c 7320 7769 6c6c 2062  er labels will b
+00001830: 6520 7669 7375 616c 697a 6564 2077 6974  e visualized wit
+00001840: 6820 636f 6c6f 7273 0d0a 2020 2020 2020  h colors..      
+00001850: 2020 4661 6c73 653a 2053 7065 6369 6669    False: Specifi
+00001860: 6564 206f 7220 6465 6661 756c 7420 636f  ed or default co
+00001870: 6c6f 726d 6170 2077 696c 6c20 6265 2075  lormap will be u
+00001880: 7365 6420 746f 2064 6973 706c 6179 2069  sed to display i
+00001890: 6e74 656e 7369 7469 6573 2e0d 0a20 2020  ntensities...   
+000018a0: 206d 696e 5f64 6973 706c 6179 5f69 6e74   min_display_int
+000018b0: 656e 7369 7479 3a20 666c 6f61 740d 0a20  ensity: float.. 
+000018c0: 2020 2020 2020 206c 6f77 6572 206c 696d         lower lim
+000018d0: 6974 2066 6f72 2064 6973 706c 6179 2072  it for display r
+000018e0: 616e 6765 0d0a 2020 2020 6d61 785f 6469  ange..    max_di
+000018f0: 7370 6c61 795f 696e 7465 6e73 6974 793a  splay_intensity:
+00001900: 2066 6c6f 6174 0d0a 2020 2020 2020 2020   float..        
+00001910: 7570 7065 7220 6c69 6d69 7420 666f 7220  upper limit for 
+00001920: 6469 7370 6c61 7920 7261 6e67 650d 0a20  display range.. 
+00001930: 2020 2063 6f6c 6f72 5f6d 6170 3a20 7374     color_map: st
+00001940: 720d 0a20 2020 2020 2020 2064 6570 7265  r..        depre
+00001950: 6361 7465 642c 2075 7365 2063 6f6c 6f72  cated, use color
+00001960: 6d61 7020 696e 7374 6561 640d 0a20 2020  map instead..   
+00001970: 2070 6c6f 743a 206d 6174 706c 6f74 6c69   plot: matplotli
+00001980: 6220 6178 6973 0d0a 2020 2020 2020 2020  b axis..        
+00001990: 506c 6f74 206f 626a 6563 7420 7768 6572  Plot object wher
+000019a0: 6520 7468 6520 696d 6167 6520 7368 6f75  e the image shou
+000019b0: 6c64 2062 6520 7368 6f77 6e2e 2055 7365  ld be shown. Use
+000019c0: 6675 6c20 666f 7220 7075 7474 696e 6720  ful for putting 
+000019d0: 6d75 6c74 6970 6c65 2069 6d61 6765 7320  multiple images 
+000019e0: 696e 2073 7562 6669 6775 7265 732e 0d0a  in subfigures...
+000019f0: 2020 2020 636f 6c6f 7262 6172 3a20 626f      colorbar: bo
+00001a00: 6f6c 0d0a 2020 2020 2020 2020 5472 7565  ol..        True
+00001a10: 2070 7574 7320 6120 636f 6c6f 7262 6172   puts a colorbar
+00001a20: 206e 6578 7420 746f 2074 6865 2069 6d61   next to the ima
+00001a30: 6765 2e20 5769 6c6c 206e 6f74 2077 6f72  ge. Will not wor
+00001a40: 6b20 7769 7468 206c 6162 656c 2069 6d61  k with label ima
+00001a50: 6765 7320 616e 6420 7768 656e 2076 6973  ges and when vis
+00001a60: 7561 6c69 7a69 6e67 206d 756c 7469 706c  ualizing multipl
+00001a70: 650d 0a20 2020 2020 2020 2069 6d61 6765  e..        image
+00001a80: 7320 2863 6f6e 7469 6e75 655f 6472 6177  s (continue_draw
+00001a90: 696e 673d 5472 7565 292e 0d0a 2020 2020  ing=True)...    
+00001aa0: 636f 6c6f 726d 6170 3a20 7374 7220 6f72  colormap: str or
+00001ab0: 206d 6174 706c 6f74 6c69 6220 636f 6c6f   matplotlib colo
+00001ac0: 726d 6170 0d0a 2020 2020 616c 7068 613a  rmap..    alpha:
+00001ad0: 2066 6c6f 6174 0d0a 2020 2020 2020 2020   float..        
+00001ae0: 616c 7068 6120 626c 656e 6469 6e67 2076  alpha blending v
+00001af0: 616c 7565 0d0a 2020 2020 636f 6e74 696e  alue..    contin
+00001b00: 7565 5f64 7261 7769 6e67 3a20 666c 6f61  ue_drawing: floa
+00001b10: 740d 0a20 2020 2020 2020 2054 7275 653a  t..        True:
+00001b20: 2074 6865 206e 6578 7420 7368 6f77 6e20   the next shown 
+00001b30: 696d 6167 6520 6361 6e20 6265 2076 6973  image can be vis
+00001b40: 7561 6c69 7a65 6420 6f6e 2074 6f70 206f  ualized on top o
+00001b50: 6620 7468 6520 6375 7272 656e 7420 6f6e  f the current on
+00001b60: 652c 2065 2e67 2e20 7769 7468 2061 6c70  e, e.g. with alp
+00001b70: 6861 203d 2030 2e35 0d0a 2020 2020 2222  ha = 0.5..    ""
+00001b80: 220d 0a20 2020 2069 6d70 6f72 7420 6e75  "..    import nu
+00001b90: 6d70 7920 6173 206e 700d 0a0d 0a20 2020  mpy as np....   
+00001ba0: 2069 6620 6c65 6e28 696d 6167 652e 7368   if len(image.sh
+00001bb0: 6170 6529 203d 3d20 333a 0d0a 2020 2020  ape) == 3:..    
+00001bc0: 2020 2020 696d 6167 6520 3d20 6e70 2e61      image = np.a
+00001bd0: 7361 7272 6179 2869 6d61 6765 292e 6d61  sarray(image).ma
+00001be0: 7828 6178 6973 3d30 290d 0a0d 0a20 2020  x(axis=0)....   
+00001bf0: 2069 6d61 6765 203d 206e 702e 6173 6172   image = np.asar
+00001c00: 7261 7928 696d 6167 6529 0d0a 2020 2020  ray(image)..    
+00001c10: 6966 206c 656e 2869 6d61 6765 2e73 6861  if len(image.sha
+00001c20: 7065 2920 3d3d 2031 3a0d 0a20 2020 2020  pe) == 1:..     
+00001c30: 2020 2069 6d61 6765 203d 2069 6d61 6765     image = image
+00001c40: 5b6e 702e 6e65 7761 7869 735d 0d0a 0d0a  [np.newaxis]....
+00001c50: 2020 2020 6966 2063 6f6c 6f72 6d61 7020      if colormap 
+00001c60: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00001c70: 2020 636f 6c6f 726d 6170 203d 2022 4772    colormap = "Gr
+00001c80: 6579 735f 7222 0d0a 0d0a 2020 2020 636d  eys_r"....    cm
+00001c90: 6170 203d 2063 6f6c 6f72 6d61 700d 0a20  ap = colormap.. 
+00001ca0: 2020 2069 6620 6c61 6265 6c73 3a0d 0a20     if labels:.. 
+00001cb0: 2020 2020 2020 2069 6d70 6f72 7420 6d61         import ma
+00001cc0: 7470 6c6f 746c 6962 0d0a 2020 2020 2020  tplotlib..      
+00001cd0: 2020 696d 706f 7274 206e 756d 7079 2061    import numpy a
+00001ce0: 7320 6e70 0d0a 0d0a 2020 2020 2020 2020  s np....        
+00001cf0: 6966 206e 6f74 2068 6173 6174 7472 285f  if not hasattr(_
+00001d00: 696d 7368 6f77 2c20 226c 6162 656c 735f  imshow, "labels_
+00001d10: 636d 6170 2229 3a0d 0a20 2020 2020 2020  cmap"):..       
+00001d20: 2020 2020 2066 726f 6d20 2e5f 696d 6167       from ._imag
+00001d30: 655f 7769 6467 6574 2069 6d70 6f72 7420  e_widget import 
+00001d40: 5f6c 6162 656c 735f 6c75 740d 0a20 2020  _labels_lut..   
+00001d50: 2020 2020 2020 2020 205f 696d 7368 6f77           _imshow
+00001d60: 2e6c 6162 656c 735f 636d 6170 203d 206d  .labels_cmap = m
+00001d70: 6174 706c 6f74 6c69 622e 636f 6c6f 7273  atplotlib.colors
+00001d80: 2e4c 6973 7465 6443 6f6c 6f72 6d61 7028  .ListedColormap(
+00001d90: 5f6c 6162 656c 735f 6c75 7428 2929 0d0a  _labels_lut())..
+00001da0: 2020 2020 2020 2020 636d 6170 203d 205f          cmap = _
+00001db0: 696d 7368 6f77 2e6c 6162 656c 735f 636d  imshow.labels_cm
+00001dc0: 6170 0d0a 0d0a 2020 2020 2020 2020 6966  ap....        if
+00001dd0: 206d 696e 5f64 6973 706c 6179 5f69 6e74   min_display_int
+00001de0: 656e 7369 7479 2069 7320 4e6f 6e65 3a0d  ensity is None:.
+00001df0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00001e00: 5f64 6973 706c 6179 5f69 6e74 656e 7369  _display_intensi
+00001e10: 7479 203d 2030 0d0a 2020 2020 2020 2020  ty = 0..        
+00001e20: 6966 206d 6178 5f64 6973 706c 6179 5f69  if max_display_i
+00001e30: 6e74 656e 7369 7479 2069 7320 4e6f 6e65  ntensity is None
+00001e40: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
+00001e50: 6178 5f64 6973 706c 6179 5f69 6e74 656e  ax_display_inten
+00001e60: 7369 7479 203d 2036 3535 3336 0d0a 0d0a  sity = 65536....
+00001e70: 2020 2020 6966 2070 6c6f 7420 6973 204e      if plot is N
+00001e80: 6f6e 653a 0d0a 2020 2020 2020 2020 696d  one:..        im
+00001e90: 706f 7274 206d 6174 706c 6f74 6c69 622e  port matplotlib.
+00001ea0: 7079 706c 6f74 2061 7320 706c 740d 0a20  pyplot as plt.. 
+00001eb0: 2020 2020 2020 2070 6c74 2e69 6d73 686f         plt.imsho
+00001ec0: 7728 696d 6167 652c 2063 6d61 703d 636d  w(image, cmap=cm
+00001ed0: 6170 2c20 766d 696e 3d6d 696e 5f64 6973  ap, vmin=min_dis
+00001ee0: 706c 6179 5f69 6e74 656e 7369 7479 2c20  play_intensity, 
+00001ef0: 766d 6178 3d6d 6178 5f64 6973 706c 6179  vmax=max_display
+00001f00: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 696e 7465 7270 6f6c 6174 696f 6e3d 276e  interpolation='n
+00001f30: 6561 7265 7374 272c 2061 6c70 6861 3d61  earest', alpha=a
+00001f40: 6c70 6861 290d 0a20 2020 2020 2020 2069  lpha)..        i
+00001f50: 6620 636f 6c6f 7262 6172 3a0d 0a20 2020  f colorbar:..   
+00001f60: 2020 2020 2020 2020 2070 6c74 2e63 6f6c           plt.col
+00001f70: 6f72 6261 7228 290d 0a20 2020 2020 2020  orbar()..       
+00001f80: 2069 6620 6e6f 7420 636f 6e74 696e 7565   if not continue
+00001f90: 5f64 7261 7769 6e67 3a0d 0a20 2020 2020  _drawing:..     
+00001fa0: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
+00001fb0: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+00001fc0: 2020 2020 2020 706c 6f74 2e69 6d73 686f        plot.imsho
+00001fd0: 7728 696d 6167 652c 2063 6d61 703d 636d  w(image, cmap=cm
+00001fe0: 6170 2c20 766d 696e 3d6d 696e 5f64 6973  ap, vmin=min_dis
+00001ff0: 706c 6179 5f69 6e74 656e 7369 7479 2c20  play_intensity, 
+00002000: 766d 6178 3d6d 6178 5f64 6973 706c 6179  vmax=max_display
+00002010: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2069 6e74 6572 706f 6c61 7469 6f6e 3d27   interpolation='
+00002040: 6e65 6172 6573 7427 2c20 616c 7068 613d  nearest', alpha=
+00002050: 616c 7068 6129 0d0a 2020 2020 2020 2020  alpha)..        
+00002060: 6966 2063 6f6c 6f72 6261 723a 0d0a 2020  if colorbar:..  
+00002070: 2020 2020 2020 2020 2020 706c 6f74 2e63            plot.c
+00002080: 6f6c 6f72 6261 7228 29                   olorbar()
```

### Comparing `stackview-0.6.2/stackview/_switch.py` & `stackview-0.6.3/stackview/_switch.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_uint_field.py` & `stackview-0.6.3/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview/_utilities.py` & `stackview-0.6.3/stackview/_utilities.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.2/stackview.egg-info/PKG-INFO` & `stackview-0.6.3/stackview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.2
+Version: 0.6.3
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `stackview-0.6.2/stackview.egg-info/SOURCES.txt` & `stackview-0.6.3/stackview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

