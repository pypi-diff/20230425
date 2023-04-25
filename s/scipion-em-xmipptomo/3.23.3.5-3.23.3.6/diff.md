# Comparing `tmp/scipion-em-xmipptomo-3.23.3.5.tar.gz` & `tmp/scipion-em-xmipptomo-3.23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipptomo-3.23.3.5.tar", last modified: Mon Apr 24 10:50:57 2023, max compression
+gzip compressed data, was "scipion-em-xmipptomo-3.23.3.6.tar", last modified: Tue Apr 25 08:38:29 2023, max compression
```

## Comparing `scipion-em-xmipptomo-3.23.3.5.tar` & `scipion-em-xmipptomo-3.23.3.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.951076 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_align_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_applyAlignmentTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_coords_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_resize_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_half_maps_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resizeTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_roiIJ.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_splitTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtomo_map_back.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtraction_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_xmipptomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/monotomo_tree_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_score_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.443014 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.443014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_align_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_applyAlignmentTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_coords_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_resize_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_half_maps_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resizeTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_roiIJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_splitTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtomo_map_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtraction_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_xmipptomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/monotomo_tree_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_score_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/xmipp_logo.png
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/CHANGES.txt` & `scipion-em-xmipptomo-3.23.3.6/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-V3.23.03.4:
+V3.23.03.6:
+ - Map back fix: works with "other tomograms"
+
+V3.23.03.5:
  - Map back fix: works with 3d classes
+
 V3.23.03.4:
  - Mapback waits now when scheduled and not the reference is needed (validation added)
 
 V3.23.03.3:
  - Fit vesicles removed (moved to tomo)
 
 V3.23.03.2:
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/LICENSE` & `scipion-em-xmipptomo-3.23.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.5
+Version: 3.23.3.6
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.5
+Version: 3.23.3.6
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/SOURCES.txt` & `scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/setup.py` & `scipion-em-xmipptomo-3.23.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/__init__.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # **************************************************************************
 import xmipp3
 import subprocess, os
 import pyworkflow.utils as pwutils
 
 _logo = "xmipp_logo.png"
 _references = ['delaRosaTrevin2013']
-__version__ = "3.23.03.5" #X.YY.MM.sv
+__version__ = "3.23.03.6" #X.YY.MM.sv
         # X.Y.M = version of the xmipp release associated.
         # sv = Set this to ".0" on each xmipp  release.
         # For not release version (hotfix) increase it --> ".1", ".2", ...
 
 class Plugin(xmipp3.Plugin):
 
     @classmethod
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/bibtex.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/__init__.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_align_transform.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_align_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_applyAlignmentTS.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_applyAlignmentTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_apply_alignment_subtomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_apply_alignment_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_cltomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_connected_components.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_connected_components.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_coords_roi.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_coords_roi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_resize_base.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_resize_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_tomograms.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_filter_coordinates_by_map.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_filter_coordinates_by_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_flexalign.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_flexalign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_half_maps_subtomos.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_half_maps_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_tomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_project_top.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_project_top.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resizeTS.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resizeTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resize_tomograms.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resize_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_roiIJ.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_roiIJ.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_coordinates.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_transform.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_splitTS.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_splitTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtomo_map_back.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtomo_map_back.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,73 +239,70 @@
 
     def _isInputASetOfCoordinates(self):
         """ Returns true if the input is a set of coordinates"""
         return isinstance(self.inputSubtomos.get(), SetOfCoordinates3D)
 
     def getTomogram(self, tsId):
         """ Returns a tomogram object based on its tsId"""
-        return self._getTomogramsInvolved()[tsId]
+        if self.inputTomograms.get() is None:
+
+            return self._getTomogramsInvolved()[tsId]
+        else:
+            return self.inputTomograms.get()[{Tomogram.TS_ID_FIELD:tsId}]
 
     def runMapBack(self, tsId, paintingType, removeBackground, threshold):
 
         tomo = self.getTomogram(tsId)
         self.debug("TomoInvolved: %s" % tomo)
 
         # Removing background
         self.removeTomogramBackground(tomo)
 
         input = self._getInput()
+        # Using subtomograms
+        usingSubtomograms = isinstance(input, SetOfSubTomograms)
 
-        inputSR = input.getSamplingRate()
+        inputSR=input.getCoordinates3D().getSamplingRate() if usingSubtomograms else input.getSamplingRate()
         tomoSR = tomo.getSamplingRate()
         scaleFactor = inputSR/tomoSR
+        self.info("Coordinates have to be multiplied by %s due to the sampling rate ratio"
+                  " between the coordinates and the tomograms used." % scaleFactor)
         mdGeometry = lib.MetaData()
 
         ref = self.getFinalRefName()
 
         if self.paintingType.get() == PAINTING_TYPES.COPY and self.constant.get() != 1:
             initialref = self.inputRef.get().getFileName()
             if initialref.endswith('.mrc'):
                 initialref += ':mrc'
             ref = self._getExtraPath("ref_mult.mrc")
             self.runJob("xmipp_image_operate", " -i %s  --mult %d -o %s" %
                         (initialref, self.constant.get(), ref))
 
-        # Using subtomograms
-        usingSubtomograms = isinstance(input, SetOfSubTomograms)
 
         where = "_coordinate._tomoId='%s'" if usingSubtomograms else "_tomoId='%s'"
         where = where % tsId
 
-        for item in input.iterItems(where=where):
-            self.debug("Mapping back %s" % item)
-            if usingSubtomograms:
-                coord = item.getCoordinate3D()
-                # A coordinte does not have an objId in this case, we set it
-                coord.setObjId(item.getObjId())
-                transform = item.getTransform(convention=MATRIX_CONVERSION.XMIPP)
-            else: # Coordinate
-                coord = item
-                transform = Transform(matrix=item.getMatrix(convention=MATRIX_CONVERSION.XMIPP))
-
-            if coord.getVolId() == tomo.getObjId() \
-                    or coord.getTomoId() == tomo.getTsId():
-                nRow = md.Row()
-                nRow.setValue(lib.MDL_ITEM_ID, int(coord.getObjId()))
-                coord.setVolume(tomo)
-                nRow.setValue(lib.MDL_XCOOR, int(coord.getX(const.BOTTOM_LEFT_CORNER)*scaleFactor))
-                nRow.setValue(lib.MDL_YCOOR, int(coord.getY(const.BOTTOM_LEFT_CORNER)*scaleFactor))
-                nRow.setValue(lib.MDL_ZCOOR, int(coord.getZ(const.BOTTOM_LEFT_CORNER)*scaleFactor))
-                # Compute inverse matrix
-                #A = subtomo.getTransform().getMatrix()
-                #subtomo.getTransform().setMatrix(np.linalg.inv(A))
-                # Convert transform matrix to Euler Angles (rot, tilt, psi)
-                from pwem import ALIGN_PROJ
-                alignmentToRow(transform, nRow, ALIGN_PROJ)
-                nRow.addToMd(mdGeometry)
+        for coord in input.iterCoordinates(volume=tomo):
+            self.debug("Mapping back %s" % coord)
+            transform = Transform(matrix=coord.getMatrix(convention=MATRIX_CONVERSION.XMIPP))
+
+            nRow = md.Row()
+            nRow.setValue(lib.MDL_ITEM_ID, int(coord.getObjId()))
+            nRow.setValue(lib.MDL_XCOOR, int(coord.getX(const.BOTTOM_LEFT_CORNER)*scaleFactor))
+            nRow.setValue(lib.MDL_YCOOR, int(coord.getY(const.BOTTOM_LEFT_CORNER)*scaleFactor))
+            nRow.setValue(lib.MDL_ZCOOR, int(coord.getZ(const.BOTTOM_LEFT_CORNER)*scaleFactor))
+            # Compute inverse matrix
+            #A = subtomo.getTransform().getMatrix()
+            #subtomo.getTransform().setMatrix(np.linalg.inv(A))
+            # Convert transform matrix to Euler Angles (rot, tilt, psi)
+            from pwem import ALIGN_PROJ
+            alignmentToRow(transform, nRow, ALIGN_PROJ)
+            nRow.addToMd(mdGeometry)
+
         fnGeometry = self._getExtraPath("geometry%s.xmd" % tsId)
         mdGeometry.write(fnGeometry)
 
         if scaleFactor != 1:
             args = "-i %s -o %s --scale %d" % (ref, ref, scaleFactor)
             self.runJob('xmipp_transform_geometry', args)
```

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtraction_subtomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtraction_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols.conf` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/__init__.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_monotomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_crop.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_crop.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_resize.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_xmipptomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_xmipptomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/utils.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/__init__.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/monotomo_tree_provider.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/monotomo_tree_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_cltomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_phantom_create.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_score_subtomos.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_score_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/wizards.py` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.5/xmipptomo/xmipp_logo.png` & `scipion-em-xmipptomo-3.23.3.6/xmipptomo/xmipp_logo.png`

 * *Files identical despite different names*

