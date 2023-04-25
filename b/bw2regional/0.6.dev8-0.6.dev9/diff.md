# Comparing `tmp/bw2regional-0.6.dev8.tar.gz` & `tmp/bw2regional-0.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2regional-0.6.dev8.tar", last modified: Tue Apr 25 05:33:08 2023, max compression
+gzip compressed data, was "bw2regional-0.6.dev9.tar", last modified: Tue Apr 25 12:25:39 2023, max compression
```

## Comparing `bw2regional-0.6.dev8.tar` & `bw2regional-0.6.dev9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.913667 bw2regional-0.6.dev8/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.903198 bw2regional-0.6.dev8/.github/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 chrismutel   (501) staff       (20)     1203 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.gitignore
--rw-r--r--   0 chrismutel   (501) staff       (20)      142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.hgignore
--rw-r--r--   0 chrismutel   (501) staff       (20)     1614 2023-04-25 05:24:34.000000 bw2regional-0.6.dev8/CHANGES.md
--rw-r--r--   0 chrismutel   (501) staff       (20)     1457 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/LICENSE.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       81 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 05:33:08.913547 bw2regional-0.6.dev8/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      419 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.906574 bw2regional-0.6.dev8/bw2regional/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2257 2023-04-25 05:20:45.000000 bw2regional-0.6.dev8/bw2regional/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4747 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/base_data.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2130 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/databases.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2157 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/density.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1113 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7298 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/export.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5336 2023-04-25 05:27:04.000000 bw2regional-0.6.dev8/bw2regional/gis_tasks.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      314 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/hashing.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2549 2023-04-25 05:20:21.000000 bw2regional-0.6.dev8/bw2regional/intersection.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.907946 bw2regional-0.6.dev8/bw2regional/lca/
--rw-r--r--   0 chrismutel   (501) staff       (20)      255 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9619 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/base_class.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    12923 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/extension_tables.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2170 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/one_spatial_scale.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3145 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3656 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales_weighting.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1825 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/loading.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1958 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/meta.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9405 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/pandarus.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    10293 2023-04-24 21:18:52.000000 bw2regional-0.6.dev8/bw2regional/pandarus_remote.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2818 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/topography.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8910 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/validate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       25 2023-04-24 21:18:56.000000 bw2regional-0.6.dev8/bw2regional/version.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1601 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/xtables.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.907157 bw2regional-0.6.dev8/bw2regional.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1937 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)      138 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.909265 bw2regional-0.6.dev8/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6786 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/Makefile
--rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/base-data.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     1079 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/common.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     9331 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8777 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/formats.rst
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.909379 bw2regional-0.6.dev8/docs/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)   149543 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/images/mnglr.png
--rw-r--r--   0 chrismutel   (501) staff       (20)     8945 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/index.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     4846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/lca.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     1994 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/libraries.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     6713 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/make.bat
--rw-r--r--   0 chrismutel   (501) staff       (20)      846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/technical.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)       40 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/pytest.ini
--rw-r--r--   0 chrismutel   (501) staff       (20)        9 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/requirements.rtd.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)      139 2023-04-25 05:23:45.000000 bw2regional-0.6.dev8/requirements.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-25 05:33:08.913697 bw2regional-0.6.dev8/setup.cfg
--rw-r--r--   0 chrismutel   (501) staff       (20)     1562 2023-04-25 05:24:03.000000 bw2regional-0.6.dev8/setup.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.911368 bw2regional-0.6.dev8/tests/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.913342 bw2regional-0.6.dev8/tests/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2600 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-cfs.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      213 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-countries.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      491 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-topo.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)     4698 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/density_fixture.tiff
--rw-r--r--   0 chrismutel   (501) staff       (20)     1635 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-countries-cfs.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      477 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-countries-provinces.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)     4215 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-topo-cfs.json.bz2
--rwxr-xr-x   0 chrismutel   (501) staff       (20)      523 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/pandarus-commands.sh
--rw-r--r--   0 chrismutel   (501) staff       (20)   131072 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_countries.gpkg
--rw-r--r--   0 chrismutel   (501) staff       (20)   225280 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_provinces.gpkg
--rw-r--r--   0 chrismutel   (501) staff       (20)     3936 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_raster_cfs.tif
--rw-r--r--   0 chrismutel   (501) staff       (20)     1336 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_raster_loading.tif
--rw-r--r--   0 chrismutel   (501) staff       (20)      220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_topo_mapping.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     5837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_density.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      861 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_intersections.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1239 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_lca.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1175 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_loading.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2304 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_meta.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_one_spatial_scale.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1438 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_pandarus.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3054 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_setup.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      185 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_topography.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6242 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_two_spatial_scales.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7705 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_two_spatial_scales_weighting.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1517 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      212 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_xtables.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.050553 bw2regional-0.6.dev9/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.036531 bw2regional-0.6.dev9/.github/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1203 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.gitignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)      142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.hgignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1672 2023-04-25 12:25:29.000000 bw2regional-0.6.dev9/CHANGES.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1457 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/LICENSE.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       81 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 12:25:39.050423 bw2regional-0.6.dev9/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      419 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.040406 bw2regional-0.6.dev9/bw2regional/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2257 2023-04-25 05:20:45.000000 bw2regional-0.6.dev9/bw2regional/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4747 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/base_data.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2130 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/databases.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2157 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1113 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7298 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/export.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5358 2023-04-25 12:20:54.000000 bw2regional-0.6.dev9/bw2regional/gis_tasks.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      314 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/hashing.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2549 2023-04-25 05:20:21.000000 bw2regional-0.6.dev9/bw2regional/intersection.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.043002 bw2regional-0.6.dev9/bw2regional/lca/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      255 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9619 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/base_class.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    12923 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/extension_tables.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2170 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3145 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3656 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1825 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1958 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9405 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10293 2023-04-24 21:18:52.000000 bw2regional-0.6.dev9/bw2regional/pandarus_remote.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2818 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8910 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/validate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       25 2023-04-25 12:21:01.000000 bw2regional-0.6.dev9/bw2regional/version.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1601 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/xtables.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.041365 bw2regional-0.6.dev9/bw2regional.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1937 2023-04-25 12:25:39.000000 bw2regional-0.6.dev9/bw2regional.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      138 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.044864 bw2regional-0.6.dev9/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6786 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/Makefile
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/base-data.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1079 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/common.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9331 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8777 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/formats.rst
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.044998 bw2regional-0.6.dev9/docs/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   149543 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/images/mnglr.png
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8945 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/index.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/lca.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1994 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/libraries.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6713 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/make.bat
+-rw-r--r--   0 chrismutel   (501) staff       (20)      846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/technical.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)       40 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/pytest.ini
+-rw-r--r--   0 chrismutel   (501) staff       (20)        9 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/requirements.rtd.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      139 2023-04-25 05:23:45.000000 bw2regional-0.6.dev9/requirements.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-25 12:25:39.050590 bw2regional-0.6.dev9/setup.cfg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1562 2023-04-25 05:24:03.000000 bw2regional-0.6.dev9/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.047659 bw2regional-0.6.dev9/tests/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.050189 bw2regional-0.6.dev9/tests/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2600 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      213 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-countries.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      491 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-topo.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4698 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/density_fixture.tiff
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1635 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-countries-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      477 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-countries-provinces.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4215 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-topo-cfs.json.bz2
+-rwxr-xr-x   0 chrismutel   (501) staff       (20)      523 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/pandarus-commands.sh
+-rw-r--r--   0 chrismutel   (501) staff       (20)   131072 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_countries.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)   225280 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_provinces.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3936 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_raster_cfs.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1336 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_raster_loading.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)      220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_topo_mapping.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      861 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_intersections.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1239 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_lca.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1175 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2304 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1438 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3054 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_setup.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      185 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6242 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7705 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1517 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      212 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_xtables.py
```

### Comparing `bw2regional-0.6.dev8/.github/CODE_OF_CONDUCT.md` & `bw2regional-0.6.dev9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/.gitignore` & `bw2regional-0.6.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/CHANGES.md` & `bw2regional-0.6.dev9/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # regional Changelog
 
+## 0.6.DEV9 (2023-04-25)
+
+* Fix bug in calling Geopandas
+
 ## 0.6.DEV8 (2023-04-24)
 
 * Add `calculate_needed_intersections` function
 * Add `rasterstats` engine to `raster_as_extension_table`
 * Added `rasterstats` dependency
 * Don't error out on jobs which are skipped because already done
```

### Comparing `bw2regional-0.6.dev8/LICENSE.txt` & `bw2regional-0.6.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/PKG-INFO` & `bw2regional-0.6.dev9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev8
+Version: 0.6.dev9
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2regional-0.6.dev8/bw2regional/__init__.py` & `bw2regional-0.6.dev9/bw2regional/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/base_data.py` & `bw2regional-0.6.dev9/bw2regional/base_data.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/databases.py` & `bw2regional-0.6.dev9/bw2regional/databases.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/density.py` & `bw2regional-0.6.dev9/bw2regional/density.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/errors.py` & `bw2regional-0.6.dev9/bw2regional/errors.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/export.py` & `bw2regional-0.6.dev9/bw2regional/export.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/gis_tasks.py` & `bw2regional-0.6.dev9/bw2regional/gis_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         df1 = gp.read_file(geocollections[first]["filepath"])
         df2 = gp.read_file(geocollections[second]["filepath"])
         id1 = geocollections[first]["field"]
         id2 = geocollections[second]["field"]
 
         assert id1 != id2, "Conflicting ID labels"
 
-        intersection = gp.overlay(df1, df2)
+        intersection = gp.overlay(df1, df2, keep_geom_type=False)
         areas = intersection.to_crs(
             "esri:54009"
         ).area  # World Mollweidge in square meters
 
         data = []
         for index, feature in intersection.iterrows():
             data.append(((first, feature[id1]), (second, feature[id2]), areas[index]))
```

### Comparing `bw2regional-0.6.dev8/bw2regional/intersection.py` & `bw2regional-0.6.dev9/bw2regional/intersection.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/lca/base_class.py` & `bw2regional-0.6.dev9/bw2regional/lca/base_class.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/lca/extension_tables.py` & `bw2regional-0.6.dev9/bw2regional/lca/extension_tables.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/lca/one_spatial_scale.py` & `bw2regional-0.6.dev9/bw2regional/lca/one_spatial_scale.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales.py` & `bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales_weighting.py` & `bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales_weighting.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/loading.py` & `bw2regional-0.6.dev9/bw2regional/loading.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/meta.py` & `bw2regional-0.6.dev9/bw2regional/meta.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/pandarus.py` & `bw2regional-0.6.dev9/bw2regional/pandarus.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/pandarus_remote.py` & `bw2regional-0.6.dev9/bw2regional/pandarus_remote.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/topography.py` & `bw2regional-0.6.dev9/bw2regional/topography.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/utils.py` & `bw2regional-0.6.dev9/bw2regional/utils.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/validate.py` & `bw2regional-0.6.dev9/bw2regional/validate.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional/xtables.py` & `bw2regional-0.6.dev9/bw2regional/xtables.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/bw2regional.egg-info/PKG-INFO` & `bw2regional-0.6.dev9/bw2regional.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev8
+Version: 0.6.dev9
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2regional-0.6.dev8/bw2regional.egg-info/SOURCES.txt` & `bw2regional-0.6.dev9/bw2regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/Makefile` & `bw2regional-0.6.dev9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/base-data.rst` & `bw2regional-0.6.dev9/docs/base-data.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/common.rst` & `bw2regional-0.6.dev9/docs/common.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/conf.py` & `bw2regional-0.6.dev9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/formats.rst` & `bw2regional-0.6.dev9/docs/formats.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/images/mnglr.png` & `bw2regional-0.6.dev9/docs/images/mnglr.png`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/index.rst` & `bw2regional-0.6.dev9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/lca.rst` & `bw2regional-0.6.dev9/docs/lca.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/libraries.rst` & `bw2regional-0.6.dev9/docs/libraries.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/make.bat` & `bw2regional-0.6.dev9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/docs/technical.rst` & `bw2regional-0.6.dev9/docs/technical.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/setup.py` & `bw2regional-0.6.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/areas-cfs.json.bz2` & `bw2regional-0.6.dev9/tests/data/areas-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/density_fixture.tiff` & `bw2regional-0.6.dev9/tests/data/density_fixture.tiff`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/intersect-countries-cfs.json.bz2` & `bw2regional-0.6.dev9/tests/data/intersect-countries-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/intersect-topo-cfs.json.bz2` & `bw2regional-0.6.dev9/tests/data/intersect-topo-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/pandarus-commands.sh` & `bw2regional-0.6.dev9/tests/data/pandarus-commands.sh`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/test_countries.gpkg` & `bw2regional-0.6.dev9/tests/data/test_countries.gpkg`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/test_provinces.gpkg` & `bw2regional-0.6.dev9/tests/data/test_provinces.gpkg`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/test_raster_cfs.tif` & `bw2regional-0.6.dev9/tests/data/test_raster_cfs.tif`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/data/test_raster_loading.tif` & `bw2regional-0.6.dev9/tests/data/test_raster_loading.tif`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_density.py` & `bw2regional-0.6.dev9/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_intersections.py` & `bw2regional-0.6.dev9/tests/test_intersections.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_lca.py` & `bw2regional-0.6.dev9/tests/test_lca.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_loading.py` & `bw2regional-0.6.dev9/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_meta.py` & `bw2regional-0.6.dev9/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_one_spatial_scale.py` & `bw2regional-0.6.dev9/tests/test_one_spatial_scale.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_pandarus.py` & `bw2regional-0.6.dev9/tests/test_pandarus.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_setup.py` & `bw2regional-0.6.dev9/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_two_spatial_scales.py` & `bw2regional-0.6.dev9/tests/test_two_spatial_scales.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_two_spatial_scales_weighting.py` & `bw2regional-0.6.dev9/tests/test_two_spatial_scales_weighting.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev8/tests/test_utils.py` & `bw2regional-0.6.dev9/tests/test_utils.py`

 * *Files identical despite different names*

