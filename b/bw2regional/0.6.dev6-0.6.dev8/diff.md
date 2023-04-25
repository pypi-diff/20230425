# Comparing `tmp/bw2regional-0.6.dev6.tar.gz` & `tmp/bw2regional-0.6.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2regional-0.6.dev6.tar", last modified: Wed Apr 27 05:25:06 2022, max compression
+gzip compressed data, was "bw2regional-0.6.dev8.tar", last modified: Tue Apr 25 05:33:08 2023, max compression
```

## Comparing `bw2regional-0.6.dev6.tar` & `bw2regional-0.6.dev8.tar`

### file list

```diff
@@ -1,44 +1,88 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-04-27 05:25:06.595020 bw2regional-0.6.dev6/
--rw-r--r--   0 cmutel     (501) staff       (20)     1276 2022-04-27 05:23:25.000000 bw2regional-0.6.dev6/CHANGES.md
--rw-r--r--   0 cmutel     (501) staff       (20)     3220 2021-10-13 07:56:05.000000 bw2regional-0.6.dev6/CODE_OF_CONDUCT.md
--rw-r--r--   0 cmutel     (501) staff       (20)     1457 2021-10-13 07:56:05.000000 bw2regional-0.6.dev6/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       81 2021-10-13 07:56:05.000000 bw2regional-0.6.dev6/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     1394 2022-04-27 05:25:06.594479 bw2regional-0.6.dev6/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      419 2021-10-19 17:33:36.000000 bw2regional-0.6.dev6/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-04-27 05:25:06.583458 bw2regional-0.6.dev6/bw2regional/
--rw-r--r--   0 cmutel     (501) staff       (20)     2187 2022-04-24 06:56:31.000000 bw2regional-0.6.dev6/bw2regional/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4747 2022-04-24 06:01:11.000000 bw2regional-0.6.dev6/bw2regional/base_data.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2130 2021-10-28 08:07:23.000000 bw2regional-0.6.dev6/bw2regional/databases.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2157 2022-04-24 06:01:11.000000 bw2regional-0.6.dev6/bw2regional/density.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1113 2021-10-13 07:59:21.000000 bw2regional-0.6.dev6/bw2regional/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7298 2022-04-25 12:19:23.000000 bw2regional-0.6.dev6/bw2regional/export.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4307 2022-04-24 06:01:11.000000 bw2regional-0.6.dev6/bw2regional/gis_tasks.py
--rw-r--r--   0 cmutel     (501) staff       (20)      314 2021-10-19 17:49:39.000000 bw2regional-0.6.dev6/bw2regional/hashing.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1445 2022-04-22 19:11:18.000000 bw2regional-0.6.dev6/bw2regional/intersection.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-04-27 05:25:06.592902 bw2regional-0.6.dev6/bw2regional/lca/
--rw-r--r--   0 cmutel     (501) staff       (20)      255 2021-10-19 19:57:05.000000 bw2regional-0.6.dev6/bw2regional/lca/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9619 2022-04-24 05:59:39.000000 bw2regional-0.6.dev6/bw2regional/lca/base_class.py
--rw-r--r--   0 cmutel     (501) staff       (20)    12923 2022-04-24 06:01:12.000000 bw2regional-0.6.dev6/bw2regional/lca/extension_tables.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2170 2022-04-23 16:04:05.000000 bw2regional-0.6.dev6/bw2regional/lca/one_spatial_scale.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3145 2022-04-23 16:10:51.000000 bw2regional-0.6.dev6/bw2regional/lca/two_spatial_scales.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3656 2022-04-23 16:12:26.000000 bw2regional-0.6.dev6/bw2regional/lca/two_spatial_scales_weighting.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1825 2022-04-22 09:42:22.000000 bw2regional-0.6.dev6/bw2regional/loading.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1958 2021-10-19 17:56:03.000000 bw2regional-0.6.dev6/bw2regional/meta.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9405 2022-04-24 06:01:12.000000 bw2regional-0.6.dev6/bw2regional/pandarus.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9870 2022-04-24 06:01:12.000000 bw2regional-0.6.dev6/bw2regional/pandarus_remote.py
--rw-r--r--   0 cmutel     (501) staff       (20)      649 2021-10-13 08:08:13.000000 bw2regional-0.6.dev6/bw2regional/tests.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2865 2021-10-20 07:03:35.000000 bw2regional-0.6.dev6/bw2regional/topography.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8910 2022-04-26 06:19:26.000000 bw2regional-0.6.dev6/bw2regional/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1142 2021-10-13 08:08:13.000000 bw2regional-0.6.dev6/bw2regional/validate.py
--rw-r--r--   0 cmutel     (501) staff       (20)       25 2022-04-27 05:23:20.000000 bw2regional-0.6.dev6/bw2regional/version.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1601 2022-04-27 05:22:12.000000 bw2regional-0.6.dev6/bw2regional/xtables.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-04-27 05:25:06.585890 bw2regional-0.6.dev6/bw2regional.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     1394 2022-04-27 05:25:05.000000 bw2regional-0.6.dev6/bw2regional.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      954 2022-04-27 05:25:06.000000 bw2regional-0.6.dev6/bw2regional.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2022-04-27 05:25:05.000000 bw2regional-0.6.dev6/bw2regional.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      126 2022-04-27 05:25:06.000000 bw2regional-0.6.dev6/bw2regional.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2022-04-27 05:25:06.000000 bw2regional-0.6.dev6/bw2regional.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        9 2021-10-19 20:07:34.000000 bw2regional-0.6.dev6/requirements.rtd.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      127 2021-10-28 07:46:30.000000 bw2regional-0.6.dev6/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2022-04-27 05:25:06.595161 bw2regional-0.6.dev6/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1543 2022-04-23 20:20:33.000000 bw2regional-0.6.dev6/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.913667 bw2regional-0.6.dev8/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.903198 bw2regional-0.6.dev8/.github/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1203 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.gitignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)      142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/.hgignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1614 2023-04-25 05:24:34.000000 bw2regional-0.6.dev8/CHANGES.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1457 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/LICENSE.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       81 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 05:33:08.913547 bw2regional-0.6.dev8/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      419 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.906574 bw2regional-0.6.dev8/bw2regional/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2257 2023-04-25 05:20:45.000000 bw2regional-0.6.dev8/bw2regional/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4747 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/base_data.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2130 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/databases.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2157 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1113 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7298 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/export.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5336 2023-04-25 05:27:04.000000 bw2regional-0.6.dev8/bw2regional/gis_tasks.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      314 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/hashing.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2549 2023-04-25 05:20:21.000000 bw2regional-0.6.dev8/bw2regional/intersection.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.907946 bw2regional-0.6.dev8/bw2regional/lca/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      255 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9619 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/base_class.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    12923 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/extension_tables.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2170 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3145 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3656 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1825 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1958 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9405 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10293 2023-04-24 21:18:52.000000 bw2regional-0.6.dev8/bw2regional/pandarus_remote.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2818 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8910 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/validate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       25 2023-04-24 21:18:56.000000 bw2regional-0.6.dev8/bw2regional/version.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1601 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/bw2regional/xtables.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.907157 bw2regional-0.6.dev8/bw2regional.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1937 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      138 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-25 05:33:08.000000 bw2regional-0.6.dev8/bw2regional.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.909265 bw2regional-0.6.dev8/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6786 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/Makefile
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/base-data.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1079 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/common.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9331 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8777 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/formats.rst
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.909379 bw2regional-0.6.dev8/docs/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   149543 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/images/mnglr.png
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8945 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/index.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/lca.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1994 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/libraries.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6713 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/make.bat
+-rw-r--r--   0 chrismutel   (501) staff       (20)      846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/docs/technical.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)       40 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/pytest.ini
+-rw-r--r--   0 chrismutel   (501) staff       (20)        9 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/requirements.rtd.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      139 2023-04-25 05:23:45.000000 bw2regional-0.6.dev8/requirements.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-25 05:33:08.913697 bw2regional-0.6.dev8/setup.cfg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1562 2023-04-25 05:24:03.000000 bw2regional-0.6.dev8/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.911368 bw2regional-0.6.dev8/tests/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 05:33:08.913342 bw2regional-0.6.dev8/tests/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2600 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      213 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-countries.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      491 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/areas-topo.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4698 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/density_fixture.tiff
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1635 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-countries-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      477 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-countries-provinces.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4215 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/intersect-topo-cfs.json.bz2
+-rwxr-xr-x   0 chrismutel   (501) staff       (20)      523 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/pandarus-commands.sh
+-rw-r--r--   0 chrismutel   (501) staff       (20)   131072 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_countries.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)   225280 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_provinces.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3936 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_raster_cfs.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1336 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_raster_loading.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)      220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/data/test_topo_mapping.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      861 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_intersections.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1239 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_lca.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1175 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2304 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1438 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3054 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_setup.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      185 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6242 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7705 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1517 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      212 2023-04-24 18:26:16.000000 bw2regional-0.6.dev8/tests/test_xtables.py
```

### Comparing `bw2regional-0.6.dev6/CHANGES.md` & `bw2regional-0.6.dev8/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# regional Changelog
+
+## 0.6.DEV8 (2023-04-24)
+
+* Add `calculate_needed_intersections` function
+* Add `rasterstats` engine to `raster_as_extension_table`
+* Added `rasterstats` dependency
+* Don't error out on jobs which are skipped because already done
+
+## 0.6.DEV7 (2023-04-24)
+
+* Don't raise errors for `AlreadyExists`
+* Fix path error
+
 ## 0.6.DEV6 (2022-04-27)
 
 * Allow masking when importing maps as extension tables
 
 ## 0.6.DEV5 (2022-04-26)
 
 * Re-enable some pandarus functionality
```

### Comparing `bw2regional-0.6.dev6/CODE_OF_CONDUCT.md` & `bw2regional-0.6.dev8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/LICENSE.txt` & `bw2regional-0.6.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/PKG-INFO` & `bw2regional-0.6.dev8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev6
-Summary: UNKNOWN
+Version: 0.6.dev8
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,9 +25,7 @@
 
 This package provides a regionalized LCA calculations for the [Brightway2 life cycle assessment framework](https://brightway.dev). [Online documentation](https://brightway2-regional.readthedocs.io/) is available, and the source code is hosted on [Github](https://github.com/brightway-lca/brightway2-regional).
 
 ## Contributors
 
 * Chris Mutel (https://chris.mutel.org/)
 * Estelle Louineau
-
-
```

### Comparing `bw2regional-0.6.dev6/bw2regional/__init__.py` & `bw2regional-0.6.dev8/bw2regional/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = (
     "cg",
+    "calculate_needed_intersections",
     "create_ecoinvent_collections",
     "create_empty_intersection",
     "create_restofworlds_collections",
     "create_world_collections",
     "divide_by_area",
     "extension_tables",
     "ExtensionTable",
@@ -50,15 +51,15 @@
 from .meta import (
     extension_tables,
     geocollections,
     intersections,
     loadings,
     topocollections,
 )
-from .intersection import Intersection
+from .intersection import Intersection, calculate_needed_intersections
 from .xtables import ExtensionTable
 from .databases import label_activity_geocollections
 from .density import divide_by_area
 from .lca import (
     ExtensionTablesLCA,
     OneSpatialScaleLCA,
     TwoSpatialScalesLCA,
```

### Comparing `bw2regional-0.6.dev6/bw2regional/base_data.py` & `bw2regional-0.6.dev8/bw2regional/base_data.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/databases.py` & `bw2regional-0.6.dev8/bw2regional/databases.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/density.py` & `bw2regional-0.6.dev8/bw2regional/density.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/errors.py` & `bw2regional-0.6.dev8/bw2regional/errors.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/export.py` & `bw2regional-0.6.dev8/bw2regional/export.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/gis_tasks.py` & `bw2regional-0.6.dev8/bw2regional/gis_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,87 @@
 import bw2data as bd
 
+import geopandas as gp
+import rasterstats
+
 from . import (
     Intersection,
     extension_tables,
+    ExtensionTable,
     geocollections,
     intersections,
     topocollections,
 )
 from .pandarus import import_from_pandarus, import_xt_from_rasterstats
 from .pandarus_remote import PandarusRemote, remote, run_job
 
 try:
     import pandarus
 except ImportError:
     pandarus = None
 import multiprocessing
-import os
-
-import geopandas as gp
 
 CPU_COUNT = multiprocessing.cpu_count()
 
 
 def raster_as_extension_table(
-    vector, raster, name=None, engine=remote, overwrite=False
+    vector, raster, name=None, engine=remote, overwrite=False, mask_negative=True
 ):
     if vector not in geocollections or raster not in geocollections:
         raise ValueError("Vector or raster not a valid geocollection")
     if vector in topocollections:
         raise ValueError(
             "this function only works with geocollections, not topocollections"
         )
 
     if name is None:
         name = vector + " - " + raster
 
     dirpath = bd.projects.request_directory("regional")
-    fp = str(dirpath / name + ".json")
+    fp = str(dirpath / (name + ".json"))
 
     if name in extension_tables and not overwrite:
         return
 
     if isinstance(engine, PandarusRemote):
         print("Calculating raster statistics")
         run_job(engine.calculate_rasterstats(vector, raster))
 
         print("Creating Extension Table")
         return engine.rasterstats_as_xt(vector, raster, name)
-
+    elif engine == "rasterstats":
+        if mask_negative:
+            func = lambda array: array[array >= 0]
+        else:
+            func = lambda array: array
+
+        stats = rasterstats.zonal_stats(
+            geocollections[vector]['filepath'],
+            geocollections[raster]['filepath'],
+            geojson_out=True,
+            nodata=geocollections[raster].get('nodata', -1),
+            zone_func=func
+        )
+        xt = ExtensionTable(name)
+        md = {
+            "filepath": fp,
+            "vector": geocollections[vector]['filepath'],
+            "raster": geocollections[raster]['filepath'],
+            "geocollection": vector,
+        }
+        xt.register(**md)
+        field = geocollections[vector]['field']
+        xt.write(
+            [
+                (row.properties['mean'], (vector, row.properties[field]))
+                for row in stats
+                if row.properties['mean'] is not None
+            ]
+        )
+        return xt
     elif engine == "pandarus":
         if not pandarus:
             raise ImportError("`pandarus` library required for this function")
 
         vector_fp, vector_field = (
             geocollections[vector]["filepath"],
             geocollections[vector]["field"],
```

### Comparing `bw2regional-0.6.dev6/bw2regional/intersection.py` & `bw2regional-0.6.dev8/bw2regional/intersection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import warnings
+import itertools
 
 from bw2data import geomapping
 from bw2data.ia_data_store import ImpactAssessmentDataStore
 
 from .meta import intersections
 from .utils import create_certain_datapackage
 from .validate import intersection_validator
@@ -40,7 +41,31 @@
         data = self.load()
         create_certain_datapackage(
             [(geomapping[line[0]], geomapping[line[1]]) for line in data],
             [line[2] for line in data],
             self,
             **extra_metadata
         )
+
+
+def calculate_needed_intersections(functional_unit, lcia_method, xtable=None, engine='geopandas'):
+    from . import extension_tables
+    from .gis_tasks import calculate_intersection
+    from .lca.base_class import RegionalizationBase
+
+    RB = RegionalizationBase(demand=functional_unit)
+    RB.method = lcia_method
+    inv_geocollections = RB.get_inventory_geocollections()
+    ia_geocollections = RB.get_ia_geocollections()
+
+    if xtable is None:
+        for (x, y) in itertools.product(inv_geocollections, ia_geocollections):
+            if (x, y) not in intersections:
+                calculate_intersection(x, y, engine=engine)
+    else:
+        xt_geocollections = [extension_tables[xtable]['geocollection']]
+        for (x, y) in itertools.product(inv_geocollections, xt_geocollections):
+            if (x, y) not in intersections:
+                calculate_intersection(x, y, engine=engine)
+        for (x, y) in itertools.product(xt_geocollections, ia_geocollections):
+            if (x, y) not in intersections:
+                calculate_intersection(x, y, engine=engine)
```

### Comparing `bw2regional-0.6.dev6/bw2regional/lca/base_class.py` & `bw2regional-0.6.dev8/bw2regional/lca/base_class.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/lca/extension_tables.py` & `bw2regional-0.6.dev8/bw2regional/lca/extension_tables.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/lca/one_spatial_scale.py` & `bw2regional-0.6.dev8/bw2regional/lca/one_spatial_scale.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/lca/two_spatial_scales.py` & `bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/lca/two_spatial_scales_weighting.py` & `bw2regional-0.6.dev8/bw2regional/lca/two_spatial_scales_weighting.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/loading.py` & `bw2regional-0.6.dev8/bw2regional/loading.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/meta.py` & `bw2regional-0.6.dev8/bw2regional/meta.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/pandarus.py` & `bw2regional-0.6.dev8/bw2regional/pandarus.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/pandarus_remote.py` & `bw2regional-0.6.dev8/bw2regional/pandarus_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,19 @@
                     break
         except KeyboardInterrupt:
             pass
         finally:
             print("\nJob ended with status '{}'".format(self.status))
 
 
-def run_job(job):
+def run_job(job=None):
     """Handler that blocks until job is finished."""
+    if job is None:
+        # Calculated already, job submission skipped
+        return
     job.poll(interval=2)
     if job.status != "finished":
         raise ValueError("Calculation job finished with status '{}'".format(job.status))
 
 
 @wrapt.decorator
 def check_alive(wrapped, instance, args, kwargs):
@@ -145,15 +148,16 @@
 
         try:
             collection_hash = metadata["sha256"]
         except KeyError:
             collection_hash = hash_collection(collection)
 
         if collection_hash in {obj[1] for obj in self.catalog()["files"]}:
-            raise AlreadyExists
+            print(f"Geocollection {collection} is already uploaded")
+            return
 
         url = self.url + "/upload"
         data = {
             "layer": metadata.get("layer") or "",
             "field": metadata.get("field") or "",
             "band": metadata.get("band") or "",
             "sha256": collection_hash,
@@ -262,30 +266,37 @@
         first = self.hash_and_upload(vector, catalog)
         second = self.hash_and_upload(raster, catalog)
 
         resp = requests.post(
             self.url + "/calculate-rasterstats",
             data={"vector": first, "raster": second},
         )
-        self.handle_errors(resp)
+        try:
+            self.handle_errors(resp)
+        except AlreadyExists:
+            print(f"Rasterstats for {vector} and {raster} already calculated")
+            return
 
         print("Calculation job submitted.")
         return PendingJob(self.url + resp.text)
 
     @check_alive
     def calculate_intersection(self, collection_one, collection_two):
         catalog = self.catalog()
         first = self.hash_and_upload(collection_one, catalog)
         second = self.hash_and_upload(collection_two, catalog)
 
         resp = requests.post(
             self.url + "/calculate-intersection",
             data={"first": first, "second": second},
         )
-        self.handle_errors(resp)
+        try:
+            self.handle_errors(resp)
+        except:
+            print(f"Intersection for {collection_one} and {collection_two} already calculated")
 
         print("Calculation job submitted.")
         return PendingJob(self.url + resp.text)
 
     def hash_and_upload(self, collection, catalog=None):
         hashes = {obj[1] for obj in (catalog or self.catalog())["files"]}
         hashed = hash_collection(collection)
```

### Comparing `bw2regional-0.6.dev6/bw2regional/topography.py` & `bw2regional-0.6.dev8/bw2regional/topography.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     The data format for mapping data is ``{feature field value: [list of topo field values (usually id numbers)]}``.
 
     Here is a code sample for using the test data in `bw2regional`:
 
     .. code-block:: python
 
         from bw2regional import Topography, geocollections
-        from bw2regional.tests import data_dir
         import json
 
         geocollections['countries'] = {
             'filepath': os.path.join(data_dir, "test_countries.gpkg"),
             'field': 'name'
         }
         topocollections['countries-topo'] = {
```

### Comparing `bw2regional-0.6.dev6/bw2regional/utils.py` & `bw2regional-0.6.dev8/bw2regional/utils.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/validate.py` & `bw2regional-0.6.dev8/bw2regional/validate.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional/xtables.py` & `bw2regional-0.6.dev8/bw2regional/xtables.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev6/bw2regional.egg-info/PKG-INFO` & `bw2regional-0.6.dev8/bw2regional.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev6
-Summary: UNKNOWN
+Version: 0.6.dev8
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,9 +25,7 @@
 
 This package provides a regionalized LCA calculations for the [Brightway2 life cycle assessment framework](https://brightway.dev). [Online documentation](https://brightway2-regional.readthedocs.io/) is available, and the source code is hosted on [Github](https://github.com/brightway-lca/brightway2-regional).
 
 ## Contributors
 
 * Chris Mutel (https://chris.mutel.org/)
 * Estelle Louineau
-
-
```

### Comparing `bw2regional-0.6.dev6/setup.py` & `bw2regional-0.6.dev8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 requirements = [
     "bw2calc>=2.0.dev6",
     "bw2data>=4.0.dev12",
     "constructive_geometries",
     "fiona",
     "geopandas",
     "rasterio",
+    "rasterstats",
     "requests",
-    'rower',
     "shapely",
     "voluptuous",
     "wrapt",
+    'rower',
 ]
 
 v_temp = {}
 with open("bw2regional/version.py") as fp:
     exec(fp.read(), v_temp)
 version = ".".join((str(x) for x in v_temp["version"]))
```

