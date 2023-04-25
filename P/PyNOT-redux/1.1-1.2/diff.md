# Comparing `tmp/PyNOT-redux-1.1.tar.gz` & `tmp/PyNOT-redux-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNOT-redux-1.1.tar", last modified: Sat Feb 25 17:34:12 2023, max compression
+gzip compressed data, was "PyNOT-redux-1.2.tar", last modified: Tue Apr 25 06:53:49 2023, max compression
```

## Comparing `PyNOT-redux-1.1.tar` & `PyNOT-redux-1.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.859151 PyNOT-redux-1.1/
--rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-02-24 19:14:34.000000 PyNOT-redux-1.1/.DS_Store
--rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/.gitattributes
--rw-r--r--   0 krogager   (501) staff       (20)     1878 2022-05-09 07:03:03.000000 PyNOT-redux-1.1/.gitignore
--rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-02-25 17:34:12.858972 PyNOT-redux-1.1/PKG-INFO
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.844821 PyNOT-redux-1.1/PyNOT_redux.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       42 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)      113 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-02-25 17:34:12.000000 PyNOT-redux-1.1/PyNOT_redux.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/README.md
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.850869 PyNOT-redux-1.1/pynot/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/.extract_msg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/.identify_msg
--rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.1/pynot/.instrument.cfg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/.response_msg
--rw-r--r--   0 krogager   (501) staff       (20)        4 2023-02-25 17:34:07.000000 PyNOT-redux-1.1/pynot/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.1/pynot/alfosc.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.854161 PyNOT-redux-1.1/pynot/calib/
--rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/HeAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/HeNe_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/ThAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/al-gr18_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/al-gr19_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/al-gr4_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/al-gr7_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/alfosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/default_options.yml
--rw-r--r--   0 krogager   (501) staff       (20)     3738 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/default_options_img.yml
--rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/ef-gr13_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/ef-gr14_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/ef-gr1_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/ef-gr3_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/efosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/lapalma.ext
--rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/lasilla.ext
--rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/paranal.ext
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.857425 PyNOT-redux-1.1/pynot/calib/std/
--rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/bd174708.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/bd262606.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/bd332642.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/bd75325.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/eg21.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/feige110.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/feige34.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/gd153.dat
--rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/gd50.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/gd71.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/hd19445.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/hd84937.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/hd93521.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/he3.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/hiltner600.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/ltt3864.dat
--rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/tcs_namelist.txt
--rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/calib/std/wolf1346.dat
--rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.1/pynot/calibs.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.858282 PyNOT-redux-1.1/pynot/data/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/alfosc.rules
--rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/efosc.rules
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-25 17:34:12.858759 PyNOT-redux-1.1/pynot/data/help/
--rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/help/welcome_msg_extract.html
--rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/help/welcome_msg_identify.html
--rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/help/welcome_msg_response.html
--rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/io.py
--rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/obs.py
--rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/data/organizer.py
--rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.1/pynot/efosc.py
--rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.1/pynot/extract_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.1/pynot/extraction.py
--rw-r--r--   0 krogager   (501) staff       (20)    16715 2022-06-13 08:58:42.000000 PyNOT-redux-1.1/pynot/fitsio.py
--rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/functions.py
--rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.1/pynot/identify_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.1/pynot/insconfig.py
--rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/logging.py
--rw-r--r--   0 krogager   (501) staff       (20)    44793 2023-02-25 17:33:44.000000 PyNOT-redux-1.1/pynot/main.py
--rw-r--r--   0 krogager   (501) staff       (20)    30199 2022-11-18 07:29:31.000000 PyNOT-redux-1.1/pynot/phot.py
--rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/phot_redux.py
--rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.1/pynot/redux.py
--rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/reports.py
--rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/response.py
--rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/response_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.1/pynot/scired.py
--rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.1/pynot/scombine.py
--rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/tasks.py
--rw-r--r--   0 krogager   (501) staff       (20)     9248 2022-06-07 07:35:54.000000 PyNOT-redux-1.1/pynot/transients.py
--rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.1/pynot/txtio.py
--rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/wavecal.py
--rw-r--r--   0 krogager   (501) staff       (20)    10804 2022-12-20 12:23:16.000000 PyNOT-redux-1.1/pynot/wcs.py
--rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pynot/welcome.py
--rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.1/pyproject.toml
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-02-25 17:34:12.859186 PyNOT-redux-1.1/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.1/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.379552 PyNOT-redux-1.2/
+-rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-04-24 12:09:15.000000 PyNOT-redux-1.2/.DS_Store
+-rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/.gitattributes
+-rw-r--r--   0 krogager   (501) staff       (20)     1878 2022-05-09 07:03:03.000000 PyNOT-redux-1.2/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 06:53:49.379227 PyNOT-redux-1.2/PKG-INFO
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.365605 PyNOT-redux-1.2/PyNOT_redux.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       42 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      113 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/README.md
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.372052 PyNOT-redux-1.2/pynot/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.extract_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.identify_msg
+-rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.2/pynot/.instrument.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.response_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        4 2023-04-25 06:53:37.000000 PyNOT-redux-1.2/pynot/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.2/pynot/alfosc.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.374581 PyNOT-redux-1.2/pynot/calib/
+-rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/HeAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/HeNe_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ThAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr18_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr19_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr4_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr7_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/alfosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/default_options.yml
+-rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/calib/default_options_img.yml
+-rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr13_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr14_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr1_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr3_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/efosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/lapalma.ext
+-rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/lasilla.ext
+-rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/paranal.ext
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.377807 PyNOT-redux-1.2/pynot/calib/std/
+-rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd174708.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd262606.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd332642.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd75325.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/eg21.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/feige110.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/feige34.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd153.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd50.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd71.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd19445.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd84937.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd93521.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/he3.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hiltner600.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/ltt3864.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/tcs_namelist.txt
+-rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/wolf1346.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.2/pynot/calibs.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.378590 PyNOT-redux-1.2/pynot/data/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/alfosc.rules
+-rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/efosc.rules
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.379022 PyNOT-redux-1.2/pynot/data/help/
+-rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_extract.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_identify.html
+-rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_response.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/io.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/obs.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/organizer.py
+-rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.2/pynot/efosc.py
+-rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.2/pynot/extract_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.2/pynot/extraction.py
+-rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/fitsio.py
+-rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/functions.py
+-rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.2/pynot/identify_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.2/pynot/insconfig.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/logging.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/main.py
+-rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.2/pynot/phot.py
+-rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/phot_redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.2/pynot/redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/reports.py
+-rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/response.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/response_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.2/pynot/scired.py
+-rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.2/pynot/scombine.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/tasks.py
+-rw-r--r--   0 krogager   (501) staff       (20)     9248 2022-06-07 07:35:54.000000 PyNOT-redux-1.2/pynot/transients.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.2/pynot/txtio.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/wavecal.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13375 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/wcs.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/welcome.py
+-rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pyproject.toml
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2023-04-25 06:53:49.379582 PyNOT-redux-1.2/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.2/setup.py
```

### Comparing `PyNOT-redux-1.1/.DS_Store` & `PyNOT-redux-1.2/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 000010a0: 6c69 7374 3030 d601 0203 0405 0607 0707  list00..........
 000010b0: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 000010c0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 000010d0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 000010e0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 000010f0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 00001100: 6f77 5369 6465 6261 7209 0909 095f 1019  owSidebar...._..
-00001110: 7b7b 3233 332c 2031 3338 7d2c 207b 3131  {{233, 138}, {11
+00001110: 7b7b 3339 322c 2031 3432 7d2c 207b 3131  {{392, 142}, {11
 00001120: 3230 2c20 3635 357d 7d09 0815 232f 3b52  20, 655}}...#/;R
 00001130: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
 00001140: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 8c00 0000 0400 6400 6f00  ............d.o.
 00001160: 6300 7376 5372 6e6c 6f6e 6700 0000 0100  c.svSrnlong.....
 00001170: 0000 0700 4c00 4900 4300 4500 4e00 5300  ....L.I.C.E.N.S.
 00001180: 4549 6c6f 6362 6c6f 6200 0000 1000 0001  EIlocblob.......
```

### Comparing `PyNOT-redux-1.1/.gitignore` & `PyNOT-redux-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/LICENSE` & `PyNOT-redux-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/PKG-INFO` & `PyNOT-redux-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.1
+Version: 1.2
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.1/PyNOT_redux.egg-info/PKG-INFO` & `PyNOT-redux-1.2/PyNOT_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.1
+Version: 1.2
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.1/PyNOT_redux.egg-info/SOURCES.txt` & `PyNOT-redux-1.2/PyNOT_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/README.md` & `PyNOT-redux-1.2/README.md`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/__init__.py` & `PyNOT-redux-1.2/pynot/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/alfosc.py` & `PyNOT-redux-1.2/pynot/alfosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/HeAr_linelist.dat` & `PyNOT-redux-1.2/pynot/calib/HeAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/HeNe_linelist.dat` & `PyNOT-redux-1.2/pynot/calib/HeNe_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/ThAr_linelist.dat` & `PyNOT-redux-1.2/pynot/calib/ThAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/alfosc_filters.dat` & `PyNOT-redux-1.2/pynot/calib/alfosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/default_options.yml` & `PyNOT-redux-1.2/pynot/calib/default_options.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/default_options_img.yml` & `PyNOT-redux-1.2/pynot/calib/default_options_img.yml`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,17 @@
   deblend_nthresh:  32       # Number of thresholds used for object deblending
   deblend_cont:     0.005    # Minimum contrast ratio used for object deblending. Disable deblending by setting to 1.0
   clean:            True     # Perform cleaning?
   clean_param:      1.0      # Cleaning parameter (see SExtractor manual)
   segmentation_map: True     # Create a segmentation map?
 
 wcs:
-  max_num:          60       # Maximum number of targets used to fit the WCS solution.
-  min_num:          10       # Minimum number of targets required.
+  min_num:          6        # Minimum number of targets required.
   G_lim:            15       # Bright limit of Gaia sources. Reject targets brighter than G < G_lim
   q_lim:            0.8      # Reject elliptical sources with axis ratio < `q_lim`
-  kappa:             3       # Threshold for projected distance filtering.
+  p_kde:            0.5      # Probability threshold for projected vector filtering.
+  kde_factor:       0.1      # Smoothing scale for the Gaussian kernel density estimator.
 
 sdss_flux:
   q_lim:            0.8      # Reject elliptical sources with axis ratio < `q_lim`
   kappa:              3      # Threshold for magnitude filtering.
   match_radius:       1      # Matching radius in arcsec for source catalog and SDSS catalog
```

### Comparing `PyNOT-redux-1.1/pynot/calib/efosc_filters.dat` & `PyNOT-redux-1.2/pynot/calib/efosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/lapalma.ext` & `PyNOT-redux-1.2/pynot/calib/lapalma.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/lasilla.ext` & `PyNOT-redux-1.2/pynot/calib/lasilla.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/paranal.ext` & `PyNOT-redux-1.2/pynot/calib/paranal.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/bd174708.dat` & `PyNOT-redux-1.2/pynot/calib/std/bd174708.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/bd262606.dat` & `PyNOT-redux-1.2/pynot/calib/std/bd262606.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/bd332642.dat` & `PyNOT-redux-1.2/pynot/calib/std/bd332642.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/bd75325.dat` & `PyNOT-redux-1.2/pynot/calib/std/bd75325.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/eg21.dat` & `PyNOT-redux-1.2/pynot/calib/std/eg21.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/feige110.dat` & `PyNOT-redux-1.2/pynot/calib/std/feige110.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/feige34.dat` & `PyNOT-redux-1.2/pynot/calib/std/feige34.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/gd153.dat` & `PyNOT-redux-1.2/pynot/calib/std/gd153.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/gd50.dat` & `PyNOT-redux-1.2/pynot/calib/std/gd50.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/gd71.dat` & `PyNOT-redux-1.2/pynot/calib/std/gd71.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/hd19445.dat` & `PyNOT-redux-1.2/pynot/calib/std/hd19445.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/hd84937.dat` & `PyNOT-redux-1.2/pynot/calib/std/hd84937.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/hd93521.dat` & `PyNOT-redux-1.2/pynot/calib/std/hd93521.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/he3.dat` & `PyNOT-redux-1.2/pynot/calib/std/he3.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/hiltner600.dat` & `PyNOT-redux-1.2/pynot/calib/std/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/ltt3864.dat` & `PyNOT-redux-1.2/pynot/calib/std/ltt3864.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calib/std/wolf1346.dat` & `PyNOT-redux-1.2/pynot/calib/std/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/calibs.py` & `PyNOT-redux-1.2/pynot/calibs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/alfosc.rules` & `PyNOT-redux-1.2/pynot/data/alfosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/efosc.rules` & `PyNOT-redux-1.2/pynot/data/efosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/help/welcome_msg_extract.html` & `PyNOT-redux-1.2/pynot/data/help/welcome_msg_extract.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/help/welcome_msg_identify.html` & `PyNOT-redux-1.2/pynot/data/help/welcome_msg_identify.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/help/welcome_msg_response.html` & `PyNOT-redux-1.2/pynot/data/help/welcome_msg_response.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/io.py` & `PyNOT-redux-1.2/pynot/data/io.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/obs.py` & `PyNOT-redux-1.2/pynot/data/obs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/data/organizer.py` & `PyNOT-redux-1.2/pynot/data/organizer.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/efosc.py` & `PyNOT-redux-1.2/pynot/efosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/extract_gui.py` & `PyNOT-redux-1.2/pynot/extract_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/extraction.py` & `PyNOT-redux-1.2/pynot/extraction.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/fitsio.py` & `PyNOT-redux-1.2/pynot/fitsio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # pynot/fitsio.py
 __author__ = "Jens-Kristian Krogager"
 
 import warnings
 from astropy.io import fits
 import numpy as np
+import os
+
+from pynot.functions import mad
 
 
 class MultipleSpectraWarning(Warning):
     """Throw warning when several FITS Table extensions or multiple IRAF objects are present"""
     pass
 
 class WavelengthError(Exception):
@@ -444,7 +447,92 @@
         if key in hdr:
             tbl_header += "# %s : %s \n" % (key, str(hdr[key]))
     tbl_header += "#-----------------------------------------\n"
     tbl_header += "# WAVE  FLUX  ERROR  MASK [0:good / 1:bad]\n"
     with open(output, 'w') as out:
         out.write(tbl_header)
         np.savetxt(out, data, fmt="%.4f  %+.4e  %.4e  %i")
+
+
+def append_extension(base_fname, data_fname, name='', data_ext=0):
+    """
+    Append the HDU in `data_fname` to the `base_fname` FITS file
+    
+    name : string
+        Name of the new extension
+    
+    create_error : bool  [default=False]
+        Estimate an error image by analysing the statistics of the `base_fname` file.
+        Assumes that the first extension of the `base_fname` file is the data image.
+    """
+    new_data = fits.getdata(data_fname, data_ext)
+    new_hdr = fits.getheader(data_fname, data_ext)
+    log = []
+    with fits.open(base_fname, mode='update') as hdu:
+        if name in hdu:
+            log.append("[WARNING] - Extension with name '%s' already exists!" % name)
+        ext = fits.ImageHDU(new_data, header=new_hdr, name=name)
+        hdu.append(ext)
+    log.append("          - Successfully appended extension %i of file: %s" % (data_ext, data_fname))
+    log.append("          - to the file: %s" % (base_fname))
+    output_msg = '\n'.join(log)
+    return output_msg
+
+
+def remove_extension(base_fname, ext):
+    """
+    Remove a given extension of the `base_fname` FITS file
+    
+    base_fname : string
+        Filename of the FITS file to modify
+
+    ext : int or string
+        Name of the extension to remove from the input file
+    """
+    log = []
+    with fits.open(base_fname) as hdu:
+        if ext.isnumeric():
+            ext = int(ext)
+            if ext >= len(hdu):
+                log.append(" [ERROR]  - Extension %i does not exist!" % ext)
+                return "\n".join(log)
+            hdu.pop(ext)
+        else:
+            if ext in hdu:
+                val = hdu[ext]
+                idx = hdu.index(val)
+                hdu.pop(idx)
+            else:
+                log.append(" [ERROR]  - Extension '%s' does not exist!" % ext)
+                return "\n".join(log)
+        hdu.writeto('_pynot_tmp.fits')
+    os.system("mv _pynot_tmp.fits %s" % base_fname)
+    log.append("          - Successfully removed extension %s of file: %s" % (ext, base_fname))
+    return '\n'.join(log)
+
+
+def create_error_image(base_fname, overwrite=False):
+    """
+    Create an error image based on the data in the `base_fname` FITS file
+    
+    overwrite : bool  [default=False]
+        Overwrite existing error image in the input file.
+        Only if the existing extension name is `ERR`.
+    """
+    
+    data = fits.getdata(base_fname)
+    new_hdr = fits.getheader(base_fname)
+    noise = mad(data) * 1.48
+    var = np.fabs(data) + noise**2
+    new_data = np.sqrt(var)
+    name = 'ERR'
+    ext = fits.ImageHDU(new_data, header=new_hdr, name=name)
+    with fits.open(base_fname, mode='update') as hdu:
+        if 'ERR' in hdu:
+            if overwrite:
+                hdu['ERR'] = ext
+            else:
+                return " [ERROR]  - ERR image extension already exists! Use option `-f` to overwrite"
+        else:
+            hdu.append(ext)
+    output_msg = "          - Successfully created an error image"
+    return output_msg
```

### Comparing `PyNOT-redux-1.1/pynot/functions.py` & `PyNOT-redux-1.2/pynot/functions.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/identify_gui.py` & `PyNOT-redux-1.2/pynot/identify_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/insconfig.py` & `PyNOT-redux-1.2/pynot/insconfig.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/logging.py` & `PyNOT-redux-1.2/pynot/logging.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/main.py` & `PyNOT-redux-1.2/pynot/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from copy import copy
 import os
 import sys
 import numpy as np
 import warnings
+import distutils
 
 from pynot.functions import get_options, get_option_descr, get_version_number
 
 code_dir = os.path.dirname(os.path.abspath(__file__))
 calib_dir = os.path.join(code_dir, 'calib/')
 defaults_fname_spec = os.path.join(calib_dir, 'default_options.yml')
 defaults_fname_phot = os.path.join(calib_dir, 'default_options_img.yml')
@@ -50,14 +51,16 @@
         if key in descriptions:
             par_descr = descriptions[key]
         else:
             par_descr = ''
 
         if val is None:
             value_type = default_type
+        if isinstance(val, bool):
+            value_type = lambda x: bool(distutils.util.strtobool(x))
         else:
             value_type = type(val)
 
         if key not in ignore_pars:
             parser.add_argument("--%s" % key, type=value_type, default=val, help=par_descr)
 
 
@@ -475,20 +478,22 @@
     set_default_pars(parser_sep, section='sep-extract', default_type=int, mode='img')
 
 
     parser_wcs = tasks.add_parser('wcs', formatter_class=set_help_width(30),
                                   help="Perform WCS calibration")
     parser_wcs.add_argument("input", type=str,
                             help="Input image to analyse")
-    parser_wcs.add_argument("table", type=str,
+    parser_wcs.add_argument("table", type=str, default='auto', nargs='?',
                             help="Source identification table from SEP (_phot.fits)")
     parser_wcs.add_argument('-o', "--output", type=str, default='',
                             help="Filename of WCS calibrated image (.fits)")
     parser_wcs.add_argument("--fig", type=str, default='',
                             help="Filename of diagnostic figure (.pdf)")
+    parser_wcs.add_argument("-d", "--debug", action='store_true',
+                            help="Enable debugging mode with additional diagnostic plots")
     set_default_pars(parser_wcs, section='wcs', default_type=int, mode='img')
 
 
     parser_autozp = tasks.add_parser('autozp', formatter_class=set_help_width(30),
                                      help="Perform auto-calibration of magnitude zero point using SDSS data")
     parser_autozp.add_argument("input", type=str,
                                help="Input WCS calibrated image to analyse")
@@ -539,14 +544,39 @@
     parser_f2a.add_argument('input', type=str,
                             help='Input filename of FITS spectrum (either table or MEF)')
     parser_f2a.add_argument('output', type=str,
                             help='Output filename of the ASCII table')
     parser_f2a.add_argument('--keys', type=str, nargs='+',
                             help='List of keywords from the FITS header to include (ESO keywords must use . not space delimiter)')
 
+    parser_fapp = tasks.add_parser('append-ext', formatter_class=set_help_width(30),
+                                   help="Append new data to FITS file or create error image")
+    parser_fapp.add_argument('input', type=str,
+                            help='Input filename of FITS image to which the new data will be appended')
+    parser_fapp.add_argument('data', type=str,
+                            help='Filename of the image to append to the `input` FITS file')
+    parser_fapp.add_argument('-n', '--name', type=str, default='',
+                            help='Name of the new FITS extension.')
+    parser_fapp.add_argument('-x', '--ext', type=int, default=0,
+                            help='Extension number of the data file which is appended to the `input` file')
+
+    parser_delext = tasks.add_parser('remove-ext', formatter_class=set_help_width(30),
+                                     help="Remove a given extension of a FITS file")
+    parser_delext.add_argument('input', type=str,
+                               help='Input filename of FITS image to which the new data will be appended')
+    parser_delext.add_argument('ext', type=str,
+                               help='Extension number or name to remove')
+
+    parser_adderr = tasks.add_parser('add-error', formatter_class=set_help_width(30),
+                                     help="Create and append error image for a single HDU FITS file")
+    parser_adderr.add_argument('input', type=str,
+                               help='Input filename of FITS image to which the new data will be appended')
+    parser_adderr.add_argument('-f', '--force', action='store_true',
+                               help='Overwrite existing error extension (if name is `ERR`)')
+
     args = parser.parse_args()
 
 
     # -- Define Workflow
     task = args.task
     log = ""
 
@@ -778,15 +808,19 @@
             image_region = detect_filter_edge(args.flat)
             print(" Automatically detected image edges:")
             print("  left=%i   right=%i  bottom=%i  top=%i" % image_region)
             print("")
         else:
             print(" Invalid input! Either '--flat' or '--edges' must be set!")
             return
-        input_list = np.loadtxt(args.input, dtype=str, usecols=(0,))
+        if args.input.endswith('.fits'):
+            input_list = [args.input]
+        else:
+            input_list = np.loadtxt(args.input, dtype=str, usecols=(0,))
+
         for fname in input_list:
             print("  Trimming image: %s" % fname)
             trim_filter_edge(fname, *image_region, output_dir=args.dir)
 
     elif task == 'imcombine':
         print("Running task: Image Combination")
         from pynot.phot import image_combine
@@ -823,15 +857,21 @@
     elif task == 'wcs':
         print("Running task: WCS calibration")
         from pynot.wcs import correct_wcs
         options = copy(vars(args))
         vars_to_remove = ['task', 'input', 'output', 'fig', 'table']
         for varname in vars_to_remove:
             options.pop(varname)
-        log = correct_wcs(args.input, args.table, output_fname=args.output, fig_fname=args.fig, **options)
+        if args.table == 'auto':
+            from pynot.phot import source_detection
+            phot_table, _, log = source_detection(args.input)
+            print(log)
+        else:
+            phot_table = args.table
+        log = correct_wcs(args.input, phot_table, output=args.output, fig_fname=args.fig, **options)
 
 
     elif task == 'autozp':
         print("Running task: Zero point auto-calibration (SDSS)")
         from pynot.phot import flux_calibration_sdss
         options = copy(vars(args))
         vars_to_remove = ['task', 'input', 'table', 'fig']
@@ -908,14 +948,26 @@
         io.save_database(database, pfc_fname)
         print(" [OUTPUT] - Saved file classification database: %s" % pfc_fname)
 
     elif task == 'fits2ascii':
         from pynot.fitsio import fits_to_ascii
         fits_to_ascii(args.input, args.output, args.keys)
 
+    elif task == 'append-ext':
+        from pynot.fitsio import append_extension
+        log = append_extension(args.input, args.data, name=args.name, data_ext=args.ext)
+
+    elif task == 'remove-ext':
+        from pynot.fitsio import remove_extension
+        log = remove_extension(args.input, args.ext)
+    
+    elif task == 'add-error':
+        from pynot.fitsio import create_error_image
+        log = create_error_image(args.input, overwrite=args.force)
+    
     else:
         import pynot
         print("Running PyNOT for instrument: %s\n" % pynot.instrument.name)
 
     if log:
         print(log)
```

### Comparing `PyNOT-redux-1.1/pynot/phot.py` & `PyNOT-redux-1.2/pynot/phot.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/phot_redux.py` & `PyNOT-redux-1.2/pynot/phot_redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/redux.py` & `PyNOT-redux-1.2/pynot/redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/reports.py` & `PyNOT-redux-1.2/pynot/reports.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/response.py` & `PyNOT-redux-1.2/pynot/response.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/response_gui.py` & `PyNOT-redux-1.2/pynot/response_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/scired.py` & `PyNOT-redux-1.2/pynot/scired.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/scombine.py` & `PyNOT-redux-1.2/pynot/scombine.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/tasks.py` & `PyNOT-redux-1.2/pynot/tasks.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/transients.py` & `PyNOT-redux-1.2/pynot/transients.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/txtio.py` & `PyNOT-redux-1.2/pynot/txtio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/wavecal.py` & `PyNOT-redux-1.2/pynot/wavecal.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/pynot/wcs.py` & `PyNOT-redux-1.2/pynot/wcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from astropy.wcs import WCS
 from astropy.io import fits
 from astropy.table import Table
 from astropy.utils.exceptions import AstropyWarning
 
 import numpy as np
+import scipy
 import matplotlib.pyplot as plt
 import warnings
 import os
 
 
 def update_WCS(coords, refs, crval, CD):
     # Solve equations:
@@ -64,21 +65,26 @@
     tmp = coords_pix - (x0-1)
     coords = p0 + CD.dot(tmp.T).T / proj
     return coords
 
 
 def match_catalogs(coords, refs):
     matched = list()
+    matches_in_coords = []
+    used_index = list()
     for xy in coords:
         index = np.argmin(np.sum((refs - xy)**2, axis=1))
+        # if index not in used_index:
         matched.append(refs[index])
-    return np.array(matched)
+        used_index.append(index)
+        matches_in_coords.append(xy)
+    return np.array(matches_in_coords), np.array(matched)
 
 
-def get_gaia_catalog(ra, dec, radius=4., limit=2000, catalog_fname='', database='edr3'):
+def get_gaia_catalog(ra, dec, radius=4., limit=2000, catalog_fname='', database='dr3'):
     """
     ra and dec: units of degrees
     radius: units of arcmin
     limit: max number of targets to retrieve
     """
     from astroquery.gaia import Gaia
     query_args = {'limit': limit, 'ra': ra, 'dec': dec, 'radius': radius/60., 'dr': database}
@@ -90,15 +96,16 @@
                                 output_file=catalog_fname)
     result = job.get_results()
     return result
 
 
 
 
-def correct_wcs(img_fname, sep_fname, output='', fig_fname='', max_num=60, min_num=10, G_lim=15, q_lim=0.8, kappa=3):
+def correct_wcs(img_fname, sep_fname, output='', fig_fname='', min_num=6, G_lim=15, q_lim=0.8, kde_factor=0.1,
+                p_kde=0.5, debug=False):
     """
     WCS calibration using Gaia
 
     Sources are matched using the initial WCS solution from the header. Outliers are rejected
     based on projected distance. The WCS solution is then matched to match the Gaia positions.
 
     Parameters
@@ -111,31 +118,33 @@
 
     output : string
         Filename of the WCS corrected image. Autogenerated by default.
 
     fig_fname : string
         Filename of the diagnostic figure. Autogenerated by default.
 
-    max_num : int  [default=60]
-        Maximum number of targets used to fit the WCS solution.
-
-    min_num : int  [default=10]
+    min_num : int  [default=6]
         Minimum number of targets required.
 
     G_lim : float  [default=15]
         Bright limit of Gaia sources. Reject targets brighter than G < G_lim as these are
         very likely saturated in the ALFOSC image.
 
     q_lim : float  [default=0.8]
         Reject elliptical sources with axis ratio < `q_lim`.
         Axis ratio is defined as minor/major.
 
-    kappa : float  [default=3]
-        Threshold for projected distance filtering. Sources are rejected if the distance differs
-        more then `kappa` times the median absolute deviation from the median of all distances.
+    kde_factor : float  [default=0.1]
+        Smoothing factor for the kernel density estimator used for source filtering
+        in the distance-orientation space.
+    
+    p_kde : float  [default=0.5]
+        Threshold for projected vector filtering. The clustering of sources in the distance-orientation space
+        is estimated using a kernel density estimator with a smoothing scale of `kde_factor`.
+        A given source is rejected if its KDE probability is less than this threshold.
 
     Returns
     -------
     output_msg : string
         Log of messages from the function call.
     """
     msg = list()
@@ -143,42 +152,41 @@
     img = fits.getdata(img_fname)
     hdr = fits.getheader(img_fname)
     msg.append("          - Loaded image: %s" % img_fname)
 
     # Prepare output filenames:
     base, ext = os.path.splitext(os.path.basename(img_fname))
     dirname = os.path.dirname(img_fname)
-    if output == '':
-        output_fname = img_fname
-        # output_fname = base + '_wcs' + ext
-        # output_fname = os.path.join(dirname, output_fname)
-    else:
-        output_fname = output
 
     if fig_fname == '':
         fig_fname = 'wcs_solution_' + base + '.pdf'
         fig_fname = os.path.join(dirname, fig_fname)
 
-    image_radius = np.sqrt(hdr['NAXIS1']**2 + hdr['NAXIS2']**2) / 2
+    image_radius = np.max([hdr['NAXIS1'], hdr['NAXIS2']]) / 2 * 0.95
     image_scale = np.sqrt(hdr['CD1_1']**2 + hdr['CD1_2']**2)
     deg_to_arcmin = 60.
     radius = image_scale * image_radius * deg_to_arcmin
     gaia_cat_name = 'gaia_source_%.2f%+.2f_%.1f.csv' % (hdr['CRVAL1'], hdr['CRVAL2'], radius)
     gaia_cat_name = os.path.join(dirname, gaia_cat_name)
-    gaia_dr = 'edr3'
+    gaia_dr = 'dr3'
     if os.path.exists(gaia_cat_name):
         ref_cat = Table.read(gaia_cat_name)
         msg.append("          - Loading Gaia source catalog: %s" % gaia_cat_name)
-        msg.append("          - Position: (ra, dec) = (%.5f ; %+.5f)  within %.1f arcmin" % (hdr['CRVAL1'], hdr['CRVAL2'], radius))
+        msg.append("          - Position: (ra, dec) = (%.5f ; %+.5f)  within %.1f arcmin" % (hdr['CRVAL1'],
+                                                                                             hdr['CRVAL2'],
+                                                                                             radius))
     else:
         # Download Gaia positions:
         msg.append("          - Downloading Gaia source catalog... (%s)" % gaia_dr.upper())
-        msg.append("          - Position: (ra, dec) = (%.5f ; %+.5f)  within %.1f arcmin" % (hdr['CRVAL1'], hdr['CRVAL2'], radius))
+        msg.append("          - Position: (ra, dec) = (%.5f ; %+.5f)  within %.1f arcmin" % (hdr['CRVAL1'],
+                                                                                             hdr['CRVAL2'],
+                                                                                             radius))
         try:
-            ref_cat = get_gaia_catalog(hdr['CRVAL1'], hdr['CRVAL2'], radius=radius, catalog_fname=gaia_cat_name, database=gaia_dr)
+            ref_cat = get_gaia_catalog(hdr['CRVAL1'], hdr['CRVAL2'],
+                                       radius=radius, catalog_fname=gaia_cat_name, database=gaia_dr)
             msg.append("          - Saving Gaia source catalog: %s" % gaia_cat_name)
         except:
             msg.append(" [ERROR]  - Could not reach Gaia server! Check your internet connection.")
             msg.append("")
             return "\n".join(msg)
 
     # reject brightest sources:
@@ -195,108 +203,153 @@
 
     # Pixel coordinates:
     sep_coords = np.array([sep_cat['x'], sep_cat['y']]).T
 
     # Convert to WCS:
     sep_wcs = pixel_to_radec(sep_coords, hdr)
     axis_ratio = sep_cat['b']/sep_cat['a']
+    
+    # Sort by source magnitude:
+    index = np.argsort(sep_cat['mag_auto'])
+    sep_wcs = sep_wcs[index]
 
     # Select only 'round' sources:
     axis_mask = axis_ratio > q_lim
     msg.append("          - Rejecting sources with axis ratio < %.2f" % q_lim)
 
-    if np.sum(axis_mask) < min_num:
-        msg.append(" [ERROR]  - Not enough targets found in the image!")
-        msg.append(" [ERROR]  - Found %i but expected at least %i" % (np.sum(axis_mask), min_num))
-        msg.append("")
-        return "\n".join(msg)
-
-    sep_wcs = sep_wcs[axis_mask]
     ref_coords = np.array([ref_cat['ra'], ref_cat['dec']]).T
     ref_coords = ref_coords[bright_cut]
+    N_gaia = len(ref_coords)
+
+    sep_wcs = sep_wcs[axis_mask]
+    sep_wcs = sep_wcs[:(N_gaia+10)]
 
     if len(ref_coords) < len(sep_wcs):
-        matched_sep = match_catalogs(ref_coords, sep_wcs)
-        matched_ref = ref_coords
+        matched_ref, matched_sep = match_catalogs(ref_coords, sep_wcs)
     else:
-        matched_ref = match_catalogs(sep_wcs, ref_coords)
-        matched_sep = sep_wcs
+        matched_sep, matched_ref = match_catalogs(sep_wcs, ref_coords)
 
     # Reject outliers:
     msg.append("          - Performing initial cross identification")
-    dist = np.sqrt(np.sum((matched_ref - matched_sep)**2, axis=1))
-    mask = np.abs(dist - np.median(dist)) < kappa*mad(dist)
-    msg.append("          - Rejecting outliers: > %.1f MAD (median abs. deviation)" % kappa)
-
+    msg.append("          - Found %s source%s" % (len(matched_ref),
+                                                  '' if len(matched_ref)==1 else 's'))
+    dist = np.sqrt(np.sum((matched_ref - matched_sep)**2, axis=1))*3600
+    dxdy = np.abs(matched_sep - matched_ref)
+    theta = np.arctan2(dxdy[:, 1], dxdy[:, 0])
+    values = np.vstack([dist, theta])
+    kernel = scipy.stats.gaussian_kde(values, bw_method=kde_factor)
+    
+    ymin = 0.
+    ymax = np.max(theta)*1.25
+    xmin = 0.
+    xmax = np.max(dist)*1.25
+    x = np.linspace(xmin, xmax, 200)
+    y = np.linspace(ymin, ymax, 200)
+    xx, yy = np.meshgrid(x, y)
+    positions = np.vstack([xx.ravel(), yy.ravel()])
+    pdf = np.reshape(kernel(positions).T, xx.shape)
+    p0 = pdf.max()
+    mask = (kernel(values) / p0) > p_kde
+    msg.append("          - Rejecting outliers with p-val > %.2f" % p_kde)
+    msg.append("          - Initial average WCS offset: %.3f arcsec" % (np.median(dist[mask])))
+    
+    if debug:
+        plt.close('all')
+        pdf = pdf/p0
+        peak = (pdf == pdf.max()).nonzero()
+        peak_dist = x[peak[1]]
+        peak_theta = y[peak[0]]
+        plt.contourf(xx, yy, pdf, cmap='Blues')
+        plt.contour(xx, yy, pdf, [p_kde, 1.0], colors=['r', 'r'])
+        plt.plot(dist, theta, 'k+')
+        plt.plot(dist[mask], theta[mask], 'ro', alpha=0.5)
+        plt.axvline(peak_dist, color='r', ls=':', alpha=0.5)
+        plt.axhline(peak_theta, color='r', ls=':', alpha=0.5)
+        plt.xlabel("Source distance (arcsec)")
+        plt.ylabel("Source orientation, $\\theta$ (radians)")
+        plt.show()
+    
     matched_sep = matched_sep[mask]
     matched_ref = matched_ref[mask]
 
+    if np.sum(mask) < min_num:
+        msg.append(" [ERROR]  - Not enough targets found in the image!")
+        msg.append(" [ERROR]  - Found %i but expected at least %i" % (np.sum(mask), min_num))
+        msg.append("")
+        return "\n".join(msg)
 
-    # Fit the WCS transformation:
+    # Fit the WCS transformation:    
     _, crval, CD, _ = get_WCS(hdr)
     msg.append("          - Fitting WCS transformation using %i sources" % len(matched_ref))
     wcs_keys = update_WCS(matched_sep, matched_ref, crval, CD)
     hdr.update(wcs_keys)
-    hdr.add_comment("PyNOT: WCS calibration using Gaia %s" % gaia_dr)
-    if 'RADESYSa' not in hdr:
-        if 'RADECSYS' in hdr:
-            hdr['RADESYSa'] = hdr['RADECSYS']
-        else:
-            msg.append("  [ERROR] - Could not find header keyword: RADECSYS or RADECSYSa")
-            output_msg = "\n".join(msg)
-            return output_msg
-
-    if 'RADECSYS' in hdr:
-        hdr.pop('RADECSYS')
+    hdr.add_comment("PyNOT: WCS calibration using Gaia %s" % gaia_dr.upper())
+    hdr['RADESYSa'] = 'ICRS'
+    hdr['RADECSYS'] = 'ICRS'
     msg.append("          - Updating WCS information")
 
 
     # -- Plot solution:
     plt.close('all')
     warnings.simplefilter('ignore', category=AstropyWarning)
     wcs_new = WCS(hdr)
     fig = plt.figure()
     ax = fig.add_subplot(111, projection=wcs_new)
     med_val = np.median(img)
     ax.imshow(img, vmin=med_val-1*mad(img), vmax=med_val+10*mad(img),
               origin='lower', cmap=plt.cm.gray_r)
     ax.scatter(matched_ref[:, 0], matched_ref[:, 1],
                transform=ax.get_transform('fk5'), edgecolor='r', facecolor='none', s=50)
+    if debug:
+        ax.scatter(matched_sep[:, 0], matched_sep[:, 1],
+                   transform=ax.get_transform('fk5'), edgecolor='green', facecolor='none', s=10, alpha=0.7)
+        for i, r in zip(matched_sep, matched_ref):
+            ax.plot([i[0], r[0]], [i[1], r[1]], 'k', alpha=0.5, transform=ax.get_transform('fk5'))
     ax.set_xlabel("Right Ascension")
     ax.set_ylabel("Declination")
-    # ax.set_title("WCS precision: %.3f arcsec" % wcs_resid)
     fig.savefig(fig_fname)
     msg.append(" [OUTPUT] - Saving WCS solution figure: %s" % fig_fname)
 
 
     # -- Calculate Dispersion in WCS Solution:
     sep_wcs = pixel_to_radec(sep_coords, hdr)
     ref_coords = np.array([ref_cat['ra'], ref_cat['dec']]).T
     ref_coords = ref_coords[bright_cut]
     if len(ref_coords) < len(sep_wcs):
-        matched_sep = match_catalogs(ref_coords, sep_wcs)
-        matched_ref = ref_coords
+        matched_ref, matched_sep = match_catalogs(ref_coords, sep_wcs)
     else:
-        matched_ref = match_catalogs(sep_wcs, ref_coords)
-        matched_sep = sep_wcs
-    dist = np.sqrt(np.sum((matched_ref - matched_sep)**2, axis=1))
-    mask = dist - np.median(dist) < kappa*mad(dist)
-    wcs_resid = np.std(dist[mask]) * 3600.
+        matched_sep, matched_ref = match_catalogs(sep_wcs, ref_coords)
+    dist = np.sqrt(np.sum((matched_ref - matched_sep)**2, axis=1)) * 3600
+    wcs_resid = mad(dist) * 1.48
+    wcs_offset = np.median(dist)
     msg.append("          - WCS precision: %.3f arcsec" % wcs_resid)
+    msg.append("          - average WCS offset: %.3f arcsec" % wcs_offset)
 
 
     # Update photometric table:
     sep_cat['ra'] = sep_wcs[:, 0]
     sep_cat['dec'] = sep_wcs[:, 1]
     sep_cat.write(sep_fname, format='fits', overwrite=True)
     msg.append(" [OUTPUT] - Updating source identification table: %s" % sep_fname)
 
 
     # -- Update image:
-    with fits.open(img_fname, mode='update') as hdu_list:
-        hdu_list['DATA'].header = hdr
-        hdu_list['ERR'].header.update(wcs_keys)
+    if output == '':
+        with fits.open(img_fname, mode='update') as hdu_list:
+            if 'DATA' not in hdu_list:
+                hdu_list[0].header = hdr
+            else:
+                hdu_list['DATA'].header = hdr
+            hdu_list['ERR'].header.update(wcs_keys)
+    else:
+        with fits.open(img_fname) as hdu_list:
+            if 'DATA' not in hdu_list:
+                hdu_list[0].header = hdr
+            else:
+                hdu_list['DATA'].header = hdr
+            hdu_list['ERR'].header.update(wcs_keys)
+            hdu_list.writeto(output, overwrite=True)
 
-    msg.append(" [OUTPUT] - Saving WCS calibrated image: %s" % output_fname)
+    msg.append(" [OUTPUT] - Saving WCS calibrated image: %s" % output)
     msg.append("")
     output_msg = "\n".join(msg)
     return output_msg
```

### Comparing `PyNOT-redux-1.1/pynot/welcome.py` & `PyNOT-redux-1.2/pynot/welcome.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.1/setup.py` & `PyNOT-redux-1.2/setup.py`

 * *Files identical despite different names*

