# Comparing `tmp/bm_utilities-0.0.4.tar.gz` & `tmp/bm_utilities-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.4.tar", last modified: Mon Apr 24 20:58:05 2023, max compression
+gzip compressed data, was "bm_utilities-0.0.5.tar", last modified: Tue Apr 25 11:58:40 2023, max compression
```

## Comparing `bm_utilities-0.0.4.tar` & `bm_utilities-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 20:58:05.386622 bm_utilities-0.0.4/
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-04-24 20:58:05.386622 bm_utilities-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 20:58:05.374621 bm_utilities-0.0.4/bm_utilities/
--rw-rw-rw-   0        0        0      136 2023-04-24 20:57:17.000000 bm_utilities-0.0.4/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     5691 2023-04-24 20:56:58.000000 bm_utilities-0.0.4/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.4/bm_utilities/common.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:58:05.384621 bm_utilities-0.0.4/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-04-24 20:58:05.000000 bm_utilities-0.0.4/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-24 20:58:05.000000 bm_utilities-0.0.4/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 20:58:05.000000 bm_utilities-0.0.4/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 20:58:05.000000 bm_utilities-0.0.4/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-24 20:58:05.000000 bm_utilities-0.0.4/bm_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      420 2023-04-24 20:58:05.388638 bm_utilities-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-04-24 20:57:03.000000 bm_utilities-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 11:58:40.975780 bm_utilities-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-04-25 11:58:40.976780 bm_utilities-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 11:58:40.965780 bm_utilities-0.0.5/bm_utilities/
+-rw-rw-rw-   0        0        0      136 2023-04-25 11:52:03.000000 bm_utilities-0.0.5/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     5692 2023-04-25 11:51:12.000000 bm_utilities-0.0.5/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.5/bm_utilities/common.py
+drwxrwxrwx   0        0        0        0 2023-04-25 11:58:40.974780 bm_utilities-0.0.5/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-04-25 11:58:40.000000 bm_utilities-0.0.5/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-25 11:58:40.000000 bm_utilities-0.0.5/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 11:58:40.000000 bm_utilities-0.0.5/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-25 11:58:40.000000 bm_utilities-0.0.5/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-25 11:58:40.000000 bm_utilities-0.0.5/bm_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0      420 2023-04-25 11:58:40.977780 bm_utilities-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-04-25 11:51:42.000000 bm_utilities-0.0.5/setup.py
```

### Comparing `bm_utilities-0.0.4/LICENSE` & `bm_utilities-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.4/PKG-INFO` & `bm_utilities-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.4/README.md` & `bm_utilities-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.4/bm_utilities/bm_utilities.py` & `bm_utilities-0.0.5/bm_utilities/bm_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,26 +106,25 @@
       all_sub_regions['ADM3_AR'] = all_sub_regions['ADM3_AR'].apply(lambda x : re.sub('\n','',x))
       all_sub_regions.rename(columns={
       'ADM3_AR':'منطقة',
       'ADM2_AR':'قسم / مركز',
       'ADM1_AR':'محافظة',
       },inplace=True)
       self.polygons = all_sub_regions
+      self.address = []
     
     def find_address(self,data_0_100k,k):
-        portal = GIS()
-        portal
         for address_1 ,idz ,_ in zip(data_0_100k["full_address"], data_0_100k["CUSTOMER_ID"],tqdm(range(len(data_0_100k)))):
             single_line_address = " مصر "+ str(address_1)
             text_clean = TextCleaner()
             single_line_address = text_clean.clean_text(single_line_address)
             geocode_results = geocode(single_line_address)
             if len(geocode_results) != 0 :
                 country = geocode_results[0]["attributes"].get("Country",np.nan)
 
                 if country == 'EGY':
                     Latitude = geocode_results[0]["location"].get("y",np.NAN)
                     Longitude =  geocode_results[0]["location"].get("x",np.NAN)
                     input_data = pd.DataFrame({"Latitude":Latitude,"Longitude":Longitude,"address":address_1,"id":idz},index=[0])
                     get_polygon = PolygonFinder(self.polygons)
-                    address = get_polygon.get_closest_polygon(Latitude,Longitude)
-        return address
+                    self.address.append(get_polygon.get_closest_polygon(Latitude,Longitude))
+        return self.address
```

### Comparing `bm_utilities-0.0.4/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.0.5/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.4/setup.py` & `bm_utilities-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

