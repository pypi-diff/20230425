# Comparing `tmp/mobility-tools-0.0.1.tar.gz` & `tmp/mobility-tools-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobility-tools-0.0.1.tar", last modified: Fri Jun 10 10:07:06 2022, max compression
+gzip compressed data, was "mobility-tools-0.1.tar", last modified: Tue Apr 25 10:31:12 2023, max compression
```

## Comparing `mobility-tools-0.0.1.tar` & `mobility-tools-0.1.tar`

### file list

```diff
@@ -1,22 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-06-10 10:07:06.439957 mobility-tools-0.0.1/
--rw-rw-rw-   0        0        0     1091 2022-05-13 09:59:06.000000 mobility-tools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      433 2022-06-10 10:07:06.439957 mobility-tools-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-10 10:07:06.427831 mobility-tools-0.0.1/mobility/
--rw-rw-rw-   0        0        0       38 2022-06-10 09:31:54.000000 mobility-tools-0.0.1/mobility/__init__.py
--rw-rw-rw-   0        0        0     3467 2022-06-09 16:12:44.000000 mobility-tools-0.0.1/mobility/get_survey_data.py
-drwxrwxrwx   0        0        0        0 2022-06-10 10:07:06.429923 mobility-tools-0.0.1/mobility/parsers/
--rw-rw-rw-   0        0        0       82 2022-06-02 12:28:19.000000 mobility-tools-0.0.1/mobility/parsers/__init__.py
--rw-rw-rw-   0        0        0    20671 2022-06-10 09:18:40.000000 mobility-tools-0.0.1/mobility/parsers/emp_2019.py
--rw-rw-rw-   0        0        0    16436 2022-06-10 09:18:48.000000 mobility-tools-0.0.1/mobility/parsers/entd_2008.py
--rw-rw-rw-   0        0        0    11103 2022-06-09 16:01:21.000000 mobility-tools-0.0.1/mobility/trip_sampler.py
-drwxrwxrwx   0        0        0        0 2022-06-10 10:07:06.439957 mobility-tools-0.0.1/mobility_tools.egg-info/
--rw-rw-rw-   0        0        0      433 2022-06-10 10:07:05.000000 mobility-tools-0.0.1/mobility_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2022-06-10 10:07:06.000000 mobility-tools-0.0.1/mobility_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-10 10:07:05.000000 mobility-tools-0.0.1/mobility_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-06-10 10:07:06.000000 mobility-tools-0.0.1/mobility_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-06-10 10:07:06.000000 mobility-tools-0.0.1/mobility_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-10 10:07:06.439957 mobility-tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      598 2022-06-10 10:06:46.000000 mobility-tools-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-10 10:07:06.439957 mobility-tools-0.0.1/test/
--rw-rw-rw-   0        0        0      186 2022-06-10 09:15:18.000000 mobility-tools-0.0.1/test/test_parsers.py
--rw-rw-rw-   0        0        0      206 2022-06-10 09:32:49.000000 mobility-tools-0.0.1/test/test_trip_sampler.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:31:12.221003 mobility-tools-0.1/
+-rw-rw-rw-   0        0        0     1091 2022-05-13 09:59:06.000000 mobility-tools-0.1/LICENSE
+-rw-rw-rw-   0        0        0      421 2023-04-25 10:31:12.221003 mobility-tools-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3671 2023-04-25 10:26:45.000000 mobility-tools-0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 10:31:12.185280 mobility-tools-0.1/mobility/
+-rw-rw-rw-   0        0        0       38 2023-02-06 11:22:15.000000 mobility-tools-0.1/mobility/__init__.py
+-rw-rw-rw-   0        0        0     4309 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/carbon_computation.py
+-rw-rw-rw-   0        0        0     2051 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/coordonnees_communes.py
+-rw-rw-rw-   0        0        0     4274 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/get_insee_data.py
+-rw-rw-rw-   0        0        0     3536 2023-04-13 12:55:07.000000 mobility-tools-0.1/mobility/get_survey_data.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:31:12.205460 mobility-tools-0.1/mobility/parsers/
+-rw-rw-rw-   0        0        0      137 2023-04-13 12:55:02.000000 mobility-tools-0.1/mobility/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-04-21 07:30:21.000000 mobility-tools-0.1/mobility/parsers/ademe_base_carbone.py
+-rw-rw-rw-   0        0        0     1171 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/parsers/communes.py
+-rw-rw-rw-   0        0        0    29449 2023-04-21 07:30:21.000000 mobility-tools-0.1/mobility/parsers/emp_2019.py
+-rw-rw-rw-   0        0        0    23796 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/parsers/entd_2008.py
+-rw-rw-rw-   0        0        0     4143 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/parsers/job_active_population.py
+-rw-rw-rw-   0        0        0     5952 2023-04-13 12:55:02.000000 mobility-tools-0.1/mobility/parsers/permanent_db_facilities.py
+-rw-rw-rw-   0        0        0     1177 2023-04-13 12:55:02.000000 mobility-tools-0.1/mobility/parsers/work_home_flows.py
+-rw-rw-rw-   0        0        0    19280 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/radiation_departments.py
+-rw-rw-rw-   0        0        0    20862 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/radiation_model.py
+-rw-rw-rw-   0        0        0     1950 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/safe_sample.py
+-rw-rw-rw-   0        0        0    13629 2023-04-25 10:26:45.000000 mobility-tools-0.1/mobility/trip_sampler.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:31:12.216079 mobility-tools-0.1/mobility_tools.egg-info/
+-rw-rw-rw-   0        0        0      421 2023-04-25 10:31:11.000000 mobility-tools-0.1/mobility_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-04-25 10:31:12.000000 mobility-tools-0.1/mobility_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:31:11.000000 mobility-tools-0.1/mobility_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-25 10:31:11.000000 mobility-tools-0.1/mobility_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 10:31:11.000000 mobility-tools-0.1/mobility_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:31:12.221003 mobility-tools-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      578 2023-04-25 10:30:12.000000 mobility-tools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:31:12.221003 mobility-tools-0.1/test/
+-rw-rw-rw-   0        0        0      188 2023-04-13 12:55:07.000000 mobility-tools-0.1/test/test_parsers.py
+-rw-rw-rw-   0        0        0     1203 2023-04-25 10:26:45.000000 mobility-tools-0.1/test/test_radiation_model.py
+-rw-rw-rw-   0        0        0      890 2023-04-25 10:26:45.000000 mobility-tools-0.1/test/test_trip_sampler.py
```

### Comparing `mobility-tools-0.0.1/LICENSE` & `mobility-tools-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mobility-tools-0.0.1/mobility/get_survey_data.py` & `mobility-tools-0.1/mobility/get_survey_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,81 +2,83 @@
 import pandas as pd
 
 import os
 from pathlib import Path
 
 from mobility.parsers import prepare_entd_2008, prepare_emp_2019
 
+
 def get_survey_data(source="EMP-2019"):
     """
     This function transforms raw survey data into dataframes needed for the sampling procedures.
-    
+
     Args:
         source (str) : The source of the travels and trips data ("ENTD-2008" or "EMP-2019", the default).
 
     Returns:
         survey_data (dict) : a dict of dataframes.
             "short_trips" (pd.DataFrame)
             "days_trip" (pd.DataFrame)
             "long_trips" (pd.DataFrame)
             "travels" (pd.DataFrame)
             "n_travels" (pd.DataFrame)
             "p_immobility" (pd.DataFrame)
             "car_ownership_probability" (pd.DataFrame)
             "p_det_mode" (pd.DataFrame)
     """
-    
+
     # Tester si les fichiers parquet existent déjà pour la source demandée
     # Si oui, charger les parquet dans un dict
     # Si non, utiliser les fonctions de préparation pour les créer avant de les charger dans un dict
-    
-    data_folder_path = Path(os.path.dirname(__file__)).parent / "data"
-    
+
+    data_folder_path = Path(os.path.dirname(__file__)) / "data"
+
     if source == "ENTD-2008":
         path = data_folder_path / "surveys/entd-2008"
     elif source == "EMP-2019":
-        path = data_folder_path / "surveys/emp-2019" 
+        path = data_folder_path / "surveys/emp-2019"
     else:
         print("The source specified doesn't exist. The EMP 2019 is used by default")
-        source = "EMD-2018-2019"
+        source = "EMP-2019"
         path = data_folder_path / "surveys/emp-2019"
-    
+
     # Check if the parquet files already exist, if not writes them calling the corresponding funtion
     check_files = (path / "short_dist_trips.parquet").exists()
     check_files = check_files and (path / "days_trip.parquet").exists()
     check_files = check_files and (path / "immobility_probability.parquet").exists()
     check_files = check_files and (path / "long_dist_trips.parquet").exists()
     check_files = check_files and (path / "travels.parquet").exists()
     check_files = check_files and (path / "long_dist_travel_number.parquet").exists()
     check_files = check_files and (path / "car_ownership_probability.parquet").exists()
     check_files = check_files and (path / "insee_modes_to_entd_modes.parquet").exists()
 
-    if not(check_files) : # ie all the files are not here
+    if not (check_files):  # ie all the files are not here
         print("Writing the parquet files")
         if source == "ENTD-2008":
             prepare_entd_2008()
-        else :
+        elif source == "EMP-2019":
             prepare_emp_2019()
-    
+        else:
+            raise NotImplementedError("We do not have data for that source")
+
     # Load the files into a dict
     survey_data = {}
 
     df = pd.read_parquet(path / "short_dist_trips.parquet")
     days_trip = pd.read_parquet(path / "days_trip.parquet")
     df_long = pd.read_parquet(path / "long_dist_trips.parquet")
     travels = pd.read_parquet(path / "travels.parquet")
     n_travel_cs1 = pd.read_parquet(path / "long_dist_travel_number.parquet")
     p_immobility = pd.read_parquet(path / "immobility_probability.parquet")
     p_car = pd.read_parquet(path / "car_ownership_probability.parquet")
     p_det_mode = pd.read_parquet(path / "insee_modes_to_entd_modes.parquet")
-    
+
     survey_data["short_trips"] = df
     survey_data["days_trip"] = days_trip
     survey_data["long_trips"] = df_long
     survey_data["travels"] = travels
     survey_data["n_travels"] = n_travel_cs1
     survey_data["p_immobility"] = p_immobility
     survey_data["p_car"] = p_car
     survey_data["p_det_mode"] = p_det_mode
-    
-    return survey_data
 
+    return survey_data
```

### Comparing `mobility-tools-0.0.1/setup.py` & `mobility-tools-0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="mobility-tools",
-    version="0.0.1",
-    author="Antoine Gauchot, Anne-Sophie Girot, Louise Gontier, Félix Pouchain",
-    author_email="antoine.gauchot@arep.fr, a.girot@elioth.fr, l.gontier@elioth.fr, felix.pouchain@arep.fr",
+    version="0.1",
+    author="Louise Gontier, Félix Pouchain, Capucine-Marin Dubroca-Voisin",
+    author_email="l.gontier@elioth.fr, felix.pouchain@arep.fr, capucine-marin.dubroca-voisin@arep.fr",
     description="A tool to simulate the mobility behaviours of the inhabitants of a given region.",
     url="https://github.com/mobility-team/mobility",
     packages=setuptools.find_packages(),
-    python_requires='>=3.9',
-    install_requires=[
-        "numpy",
-        "pandas",
-        "requests"
-    ]
-)
+    python_requires=">=3.9",
+    install_requires=["numpy", "pandas", "requests", "pyarrow", "openpyxl"],
+)
```

