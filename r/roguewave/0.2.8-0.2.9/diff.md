# Comparing `tmp/roguewave-0.2.8.tar.gz` & `tmp/roguewave-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roguewave-0.2.8.tar", last modified: Tue Mar  7 22:19:06 2023, max compression
+gzip compressed data, was "dist/roguewave-0.2.9.tar", last modified: Tue Mar  7 22:33:13 2023, max compression
```

## Comparing `roguewave-0.2.8.tar` & `roguewave-0.2.9.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.796912 roguewave-0.2.8/
--rw-r--r--   0 pietersmit   (501) staff       (20)    11357 2022-03-27 16:45:22.000000 roguewave-0.2.8/LICENSE
--rw-r--r--   0 pietersmit   (501) staff       (20)     3416 2023-03-07 22:19:06.796390 roguewave-0.2.8/PKG-INFO
--rw-r--r--   0 pietersmit   (501) staff       (20)     2807 2022-11-14 18:58:40.000000 roguewave-0.2.8/README.md
--rw-r--r--   0 pietersmit   (501) staff       (20)       38 2023-03-07 22:19:06.797095 roguewave-0.2.8/setup.cfg
--rw-r--r--   0 pietersmit   (501) staff       (20)     1256 2023-03-07 22:18:38.000000 roguewave-0.2.8/setup.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.634114 roguewave-0.2.8/src/
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.640381 roguewave-0.2.8/src/roguewave/
--rw-r--r--   0 pietersmit   (501) staff       (20)     1856 2023-02-13 05:11:46.000000 roguewave-0.2.8/src/roguewave/__init__.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.646465 roguewave-0.2.8/src/roguewave/colocate/
--rw-r--r--   0 pietersmit   (501) staff       (20)      215 2023-01-17 19:40:01.000000 roguewave-0.2.8/src/roguewave/colocate/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5859 2022-11-29 20:26:57.000000 roguewave-0.2.8/src/roguewave/colocate/bulk.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5610 2023-01-17 19:40:01.000000 roguewave-0.2.8/src/roguewave/colocate/pointdata.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3218 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/colocate/spectra.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.654256 roguewave-0.2.8/src/roguewave/filecache/
--rw-r--r--   0 pietersmit   (501) staff       (20)      211 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/filecache/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    27100 2023-02-13 16:53:53.000000 roguewave-0.2.8/src/roguewave/filecache/cache_object.py
--rw-r--r--   0 pietersmit   (501) staff       (20)       53 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/filecache/exceptions.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     7141 2023-01-17 23:06:00.000000 roguewave-0.2.8/src/roguewave/filecache/filecache.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4677 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/filecache/remote_resources.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.663990 roguewave-0.2.8/src/roguewave/interpolate/
--rw-r--r--   0 pietersmit   (501) staff       (20)      261 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1084 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/cluster.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4866 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/dataarray.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1397 2022-11-29 21:56:50.000000 roguewave-0.2.8/src/roguewave/interpolate/dataframe.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6626 2023-03-06 19:15:26.000000 roguewave-0.2.8/src/roguewave/interpolate/dataset.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3669 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/general.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     9185 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/interpolate/geometry.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10632 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/nd_interp.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5654 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/interpolate/points.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.665180 roguewave-0.2.8/src/roguewave/io/
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/io/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10017 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/io/io.py
--rw-r--r--   0 pietersmit   (501) staff       (20)      970 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/log.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.672901 roguewave-0.2.8/src/roguewave/modeldata/
--rw-r--r--   0 pietersmit   (501) staff       (20)      539 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2440 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/extract.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6349 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/keygeneration.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     9910 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/modelinformation.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    11887 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/open_remote.py
--rw-r--r--   0 pietersmit   (501) staff       (20)      505 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/open_remote_restart_files.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5365 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/remote_point_data.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.677453 roguewave-0.2.8/src/roguewave/modeldata/sofar_api/
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2021-07-26 18:37:33.000000 roguewave-0.2.8/src/roguewave/modeldata/sofar_api/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2203 2021-12-02 00:17:47.000000 roguewave-0.2.8/src/roguewave/modeldata/sofar_api/environment.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    11647 2022-08-21 16:18:16.000000 roguewave-0.2.8/src/roguewave/modeldata/sofar_api/sofar_api.py
--rw-r--r--   0 pietersmit   (501) staff       (20)      865 2021-08-02 17:54:16.000000 roguewave-0.2.8/src/roguewave/modeldata/sofar_api/utils.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4751 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/sofarspectralapi.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    15113 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/modeldata/timebase.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.681661 roguewave-0.2.8/src/roguewave/observations/
--rw-r--r--   0 pietersmit   (501) staff       (20)       67 2023-01-06 04:27:36.000000 roguewave-0.2.8/src/roguewave/observations/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    14309 2023-02-13 05:11:46.000000 roguewave-0.2.8/src/roguewave/observations/satellite.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.687406 roguewave-0.2.8/src/roguewave/spotter/
--rw-r--r--   0 pietersmit   (501) staff       (20)      454 2022-12-06 04:33:42.000000 roguewave-0.2.8/src/roguewave/spotter/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6636 2023-03-06 19:16:47.000000 roguewave-0.2.8/src/roguewave/spotter/analysis.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.702477 roguewave-0.2.8/src/roguewave/spotter/file_formats/
--rw-r--r--   0 pietersmit   (501) staff       (20)      384 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/BARO.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      480 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/BARO_RAW.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      715 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/FLT.json
--rw-r--r--   0 pietersmit   (501) staff       (20)     3484 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/GMN.json
--rw-r--r--   0 pietersmit   (501) staff       (20)     1058 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/GPS.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      630 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/LOC.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      379 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/RAINDB.json
--rw-r--r--   0 pietersmit   (501) staff       (20)   131399 2022-12-06 04:33:42.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/SPC.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      383 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/SST.json
--rw-r--r--   0 pietersmit   (501) staff       (20)      630 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/TIME.json
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-12-06 19:03:16.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10025 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/_create_formats.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1621 2022-12-06 04:33:42.000000 roguewave-0.2.8/src/roguewave/spotter/file_formats/_create_spectral_format.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    14211 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/parser.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    20265 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/spotter/read_csv_data.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.711298 roguewave-0.2.8/src/roguewave/spotterapi/
--rw-r--r--   0 pietersmit   (501) staff       (20)      210 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/spotterapi/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)      283 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/spotterapi/exceptions.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5516 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/spotterapi/helper_functions.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6250 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/spotterapi/search_endpoint.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     9464 2023-01-17 19:40:01.000000 roguewave-0.2.8/src/roguewave/spotterapi/spotter_cache.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    15861 2023-03-05 22:18:47.000000 roguewave-0.2.8/src/roguewave/spotterapi/spotterapi.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2208 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/spotterapi/spottersdcard.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.715861 roguewave-0.2.8/src/roguewave/timeseries_analysis/
--rw-r--r--   0 pietersmit   (501) staff       (20)      135 2022-12-02 00:56:29.000000 roguewave-0.2.8/src/roguewave/timeseries_analysis/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10869 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/timeseries_analysis/filtering.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6646 2023-03-05 18:32:57.000000 roguewave-0.2.8/src/roguewave/timeseries_analysis/pipeline.py
--rw-r--r--   0 pietersmit   (501) staff       (20)      516 2022-12-02 00:56:29.000000 roguewave-0.2.8/src/roguewave/timeseries_analysis/upsampling.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    14460 2022-12-21 18:43:38.000000 roguewave-0.2.8/src/roguewave/timeseries_analysis/welch.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.725562 roguewave-0.2.8/src/roguewave/tools/
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/tools/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2218 2023-03-06 19:23:48.000000 roguewave-0.2.8/src/roguewave/tools/grid.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1110 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/tools/math.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5190 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/tools/solvers.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5378 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/tools/time.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    12058 2023-03-06 19:21:35.000000 roguewave-0.2.8/src/roguewave/tools/time_integration.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.733546 roguewave-0.2.8/src/roguewave/wavephysics/
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavephysics/__init__.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.759681 roguewave-0.2.8/src/roguewave/wavephysics/balance/
--rw-r--r--   0 pietersmit   (501) staff       (20)      412 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1945 2023-03-02 00:56:14.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/balance.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5915 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/dissipation.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2176 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/factory.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     9582 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/generation.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    13782 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/jb23_tail_stress.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     7508 2023-03-06 19:24:06.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/jb23_wind_input.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5639 2023-02-13 05:11:46.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/romero_wave_breaking.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     8712 2023-03-04 18:15:14.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/solvers.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1421 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/source_term.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     8096 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_swell_dissipation.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    12525 2023-02-06 22:52:10.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_wave_breaking.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     7094 2023-03-06 19:16:47.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_wind_input.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3988 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/st6_wave_breaking.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6048 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/st6_wind_input.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10618 2023-03-06 19:16:47.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/stress.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5978 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/wam_tail_stress.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    16409 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/balance/wind_inversion.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     1436 2023-03-04 18:15:14.000000 roguewave-0.2.8/src/roguewave/wavephysics/fluidproperties.py
--rw-r--r--   0 pietersmit   (501) staff       (20)        0 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/growth_laws.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3052 2023-02-06 22:52:10.000000 roguewave-0.2.8/src/roguewave/wavephysics/roughness.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     7375 2023-03-02 00:57:17.000000 roguewave-0.2.8/src/roguewave/wavephysics/train_wind_estimate.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     8506 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavephysics/windestimate.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.771885 roguewave-0.2.8/src/roguewave/wavespectra/
--rw-r--r--   0 pietersmit   (501) staff       (20)      479 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     6475 2023-03-06 19:16:47.000000 roguewave-0.2.8/src/roguewave/wavespectra/_tools.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.778060 roguewave-0.2.8/src/roguewave/wavespectra/estimators/
--rw-r--r--   0 pietersmit   (501) staff       (20)      734 2023-02-13 05:11:46.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4634 2023-03-06 19:16:47.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/estimate.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3489 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/loglikelyhood.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     5487 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/mem.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    23651 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/mem2.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3369 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/estimators/utils.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4031 2022-11-22 18:47:00.000000 roguewave-0.2.8/src/roguewave/wavespectra/operations.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    11830 2023-03-02 00:52:20.000000 roguewave-0.2.8/src/roguewave/wavespectra/parametric.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.782688 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/
--rw-r--r--   0 pietersmit   (501) staff       (20)      321 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10321 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/classifiers.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4656 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/observations.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    18153 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/partitioning.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    17872 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavespectra/partitioning/wavefields.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    53420 2023-03-07 22:18:30.000000 roguewave-0.2.8/src/roguewave/wavespectra/spectrum.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     2674 2023-03-04 19:04:46.000000 roguewave-0.2.8/src/roguewave/wavespectra/timeseries.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.785959 roguewave-0.2.8/src/roguewave/wavetheory/
--rw-r--r--   0 pietersmit   (501) staff       (20)      127 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavetheory/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     3771 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavetheory/lineardispersion.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.795284 roguewave-0.2.8/src/roguewave/wavewatch3/
--rw-r--r--   0 pietersmit   (501) staff       (20)      623 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/__init__.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4994 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/fortran_types.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     8843 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/grid_tools.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    14306 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/io.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     8955 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/model_definition.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    13206 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/resources.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    20889 2022-11-22 19:40:49.000000 roguewave-0.2.8/src/roguewave/wavewatch3/restart_file.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4369 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_cache.py
--rw-r--r--   0 pietersmit   (501) staff       (20)     4441 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_metadata.py
--rw-r--r--   0 pietersmit   (501) staff       (20)    10615 2022-11-14 18:58:40.000000 roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_time_stack.py
-drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:19:06.643145 roguewave-0.2.8/src/roguewave.egg-info/
--rw-r--r--   0 pietersmit   (501) staff       (20)     3416 2023-03-07 22:19:05.000000 roguewave-0.2.8/src/roguewave.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (501) staff       (20)     5580 2023-03-07 22:19:06.000000 roguewave-0.2.8/src/roguewave.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (501) staff       (20)        1 2023-03-07 22:19:05.000000 roguewave-0.2.8/src/roguewave.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (501) staff       (20)      118 2023-03-07 22:19:06.000000 roguewave-0.2.8/src/roguewave.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (501) staff       (20)       10 2023-03-07 22:19:06.000000 roguewave-0.2.8/src/roguewave.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.987189 roguewave-0.2.9/
+-rw-r--r--   0 pietersmit   (501) staff       (20)    11357 2022-03-27 16:45:22.000000 roguewave-0.2.9/LICENSE
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3416 2023-03-07 22:33:13.986870 roguewave-0.2.9/PKG-INFO
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2807 2022-11-14 18:58:40.000000 roguewave-0.2.9/README.md
+-rw-r--r--   0 pietersmit   (501) staff       (20)       38 2023-03-07 22:33:13.987299 roguewave-0.2.9/setup.cfg
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1256 2023-03-07 22:33:07.000000 roguewave-0.2.9/setup.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.894898 roguewave-0.2.9/src/
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.899460 roguewave-0.2.9/src/roguewave/
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1856 2023-02-13 05:11:46.000000 roguewave-0.2.9/src/roguewave/__init__.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.902687 roguewave-0.2.9/src/roguewave/colocate/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      215 2023-01-17 19:40:01.000000 roguewave-0.2.9/src/roguewave/colocate/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5859 2022-11-29 20:26:57.000000 roguewave-0.2.9/src/roguewave/colocate/bulk.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5610 2023-01-17 19:40:01.000000 roguewave-0.2.9/src/roguewave/colocate/pointdata.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3218 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/colocate/spectra.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.904401 roguewave-0.2.9/src/roguewave/filecache/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      211 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/filecache/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    27100 2023-02-13 16:53:53.000000 roguewave-0.2.9/src/roguewave/filecache/cache_object.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)       53 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/filecache/exceptions.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     7141 2023-01-17 23:06:00.000000 roguewave-0.2.9/src/roguewave/filecache/filecache.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4677 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/filecache/remote_resources.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.908270 roguewave-0.2.9/src/roguewave/interpolate/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      261 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1084 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/cluster.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4866 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/dataarray.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1397 2022-11-29 21:56:50.000000 roguewave-0.2.9/src/roguewave/interpolate/dataframe.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6626 2023-03-06 19:15:26.000000 roguewave-0.2.9/src/roguewave/interpolate/dataset.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3669 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/general.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     9185 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/interpolate/geometry.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10632 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/nd_interp.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5654 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/interpolate/points.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.909126 roguewave-0.2.9/src/roguewave/io/
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/io/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10017 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/io/io.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)      970 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/log.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.913796 roguewave-0.2.9/src/roguewave/modeldata/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      539 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2440 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/extract.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6349 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/keygeneration.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     9910 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/modelinformation.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    11887 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/open_remote.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)      505 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/open_remote_restart_files.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5365 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/remote_point_data.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.915614 roguewave-0.2.9/src/roguewave/modeldata/sofar_api/
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2021-07-26 18:37:33.000000 roguewave-0.2.9/src/roguewave/modeldata/sofar_api/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2203 2021-12-02 00:17:47.000000 roguewave-0.2.9/src/roguewave/modeldata/sofar_api/environment.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    11647 2022-08-21 16:18:16.000000 roguewave-0.2.9/src/roguewave/modeldata/sofar_api/sofar_api.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)      865 2021-08-02 17:54:16.000000 roguewave-0.2.9/src/roguewave/modeldata/sofar_api/utils.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4751 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/sofarspectralapi.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    15113 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/modeldata/timebase.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.918006 roguewave-0.2.9/src/roguewave/observations/
+-rw-r--r--   0 pietersmit   (501) staff       (20)       67 2023-01-06 04:27:36.000000 roguewave-0.2.9/src/roguewave/observations/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    14309 2023-02-13 05:11:46.000000 roguewave-0.2.9/src/roguewave/observations/satellite.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.921110 roguewave-0.2.9/src/roguewave/spotter/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      454 2022-12-06 04:33:42.000000 roguewave-0.2.9/src/roguewave/spotter/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6636 2023-03-06 19:16:47.000000 roguewave-0.2.9/src/roguewave/spotter/analysis.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.929496 roguewave-0.2.9/src/roguewave/spotter/file_formats/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      384 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/BARO.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      480 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/BARO_RAW.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      715 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/FLT.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3484 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/GMN.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1058 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/GPS.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      630 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/LOC.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      379 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/RAINDB.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)   131399 2022-12-06 04:33:42.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/SPC.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      383 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/SST.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)      630 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/TIME.json
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-12-06 19:03:16.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10025 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/_create_formats.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1621 2022-12-06 04:33:42.000000 roguewave-0.2.9/src/roguewave/spotter/file_formats/_create_spectral_format.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    14211 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/parser.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    20265 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/spotter/read_csv_data.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.936084 roguewave-0.2.9/src/roguewave/spotterapi/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      210 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/spotterapi/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)      283 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/spotterapi/exceptions.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5516 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/spotterapi/helper_functions.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6250 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/spotterapi/search_endpoint.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     9464 2023-01-17 19:40:01.000000 roguewave-0.2.9/src/roguewave/spotterapi/spotter_cache.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    15861 2023-03-05 22:18:47.000000 roguewave-0.2.9/src/roguewave/spotterapi/spotterapi.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2208 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/spotterapi/spottersdcard.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.939145 roguewave-0.2.9/src/roguewave/timeseries_analysis/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      135 2022-12-02 00:56:29.000000 roguewave-0.2.9/src/roguewave/timeseries_analysis/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10869 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/timeseries_analysis/filtering.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6646 2023-03-05 18:32:57.000000 roguewave-0.2.9/src/roguewave/timeseries_analysis/pipeline.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)      516 2022-12-02 00:56:29.000000 roguewave-0.2.9/src/roguewave/timeseries_analysis/upsampling.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    14460 2022-12-21 18:43:38.000000 roguewave-0.2.9/src/roguewave/timeseries_analysis/welch.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.942149 roguewave-0.2.9/src/roguewave/tools/
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/tools/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2218 2023-03-06 19:23:48.000000 roguewave-0.2.9/src/roguewave/tools/grid.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1110 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/tools/math.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5190 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/tools/solvers.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5378 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/tools/time.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    12058 2023-03-06 19:21:35.000000 roguewave-0.2.9/src/roguewave/tools/time_integration.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.945738 roguewave-0.2.9/src/roguewave/wavephysics/
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavephysics/__init__.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.960743 roguewave-0.2.9/src/roguewave/wavephysics/balance/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      412 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1945 2023-03-02 00:56:14.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/balance.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5915 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/dissipation.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2176 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/factory.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     9582 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/generation.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    13782 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/jb23_tail_stress.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     7508 2023-03-06 19:24:06.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/jb23_wind_input.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5639 2023-02-13 05:11:46.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/romero_wave_breaking.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     8712 2023-03-04 18:15:14.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/solvers.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1421 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/source_term.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     8096 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_swell_dissipation.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    12525 2023-02-06 22:52:10.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_wave_breaking.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     7094 2023-03-06 19:16:47.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_wind_input.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3988 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/st6_wave_breaking.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     6048 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/st6_wind_input.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10618 2023-03-06 19:16:47.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/stress.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5978 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/wam_tail_stress.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    16409 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/balance/wind_inversion.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     1436 2023-03-04 18:15:14.000000 roguewave-0.2.9/src/roguewave/wavephysics/fluidproperties.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)        0 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/growth_laws.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3052 2023-02-06 22:52:10.000000 roguewave-0.2.9/src/roguewave/wavephysics/roughness.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     7375 2023-03-02 00:57:17.000000 roguewave-0.2.9/src/roguewave/wavephysics/train_wind_estimate.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     8506 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavephysics/windestimate.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.967241 roguewave-0.2.9/src/roguewave/wavespectra/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      479 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    14094 2023-03-07 22:31:36.000000 roguewave-0.2.9/src/roguewave/wavespectra/_tools.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.970754 roguewave-0.2.9/src/roguewave/wavespectra/estimators/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      734 2023-02-13 05:11:46.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4634 2023-03-06 19:16:47.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/estimate.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3489 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/loglikelyhood.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5487 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/mem.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    23651 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/mem2.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3369 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/estimators/utils.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4031 2022-11-22 18:47:00.000000 roguewave-0.2.9/src/roguewave/wavespectra/operations.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    11830 2023-03-02 00:52:20.000000 roguewave-0.2.9/src/roguewave/wavespectra/parametric.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.974053 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      321 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10321 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/classifiers.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4656 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/observations.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    18153 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/partitioning.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    17872 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavespectra/partitioning/wavefields.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    46073 2023-03-07 22:31:39.000000 roguewave-0.2.9/src/roguewave/wavespectra/spectrum.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     2674 2023-03-04 19:04:46.000000 roguewave-0.2.9/src/roguewave/wavespectra/timeseries.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.977843 roguewave-0.2.9/src/roguewave/wavetheory/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      127 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavetheory/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3771 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavetheory/lineardispersion.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.986278 roguewave-0.2.9/src/roguewave/wavewatch3/
+-rw-r--r--   0 pietersmit   (501) staff       (20)      623 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/__init__.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4994 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/fortran_types.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     8843 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/grid_tools.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    14306 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/io.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     8955 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/model_definition.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    13206 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/resources.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    20889 2022-11-22 19:40:49.000000 roguewave-0.2.9/src/roguewave/wavewatch3/restart_file.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4369 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_cache.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)     4441 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_metadata.py
+-rw-r--r--   0 pietersmit   (501) staff       (20)    10615 2022-11-14 18:58:40.000000 roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_time_stack.py
+drwxr-xr-x   0 pietersmit   (501) staff       (20)        0 2023-03-07 22:33:13.900972 roguewave-0.2.9/src/roguewave.egg-info/
+-rw-r--r--   0 pietersmit   (501) staff       (20)     3416 2023-03-07 22:33:13.000000 roguewave-0.2.9/src/roguewave.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (501) staff       (20)     5580 2023-03-07 22:33:13.000000 roguewave-0.2.9/src/roguewave.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (501) staff       (20)        1 2023-03-07 22:33:13.000000 roguewave-0.2.9/src/roguewave.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (501) staff       (20)      118 2023-03-07 22:33:13.000000 roguewave-0.2.9/src/roguewave.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (501) staff       (20)       10 2023-03-07 22:33:13.000000 roguewave-0.2.9/src/roguewave.egg-info/top_level.txt
```

### Comparing `roguewave-0.2.8/LICENSE` & `roguewave-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/PKG-INFO` & `roguewave-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewave
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package to interact with Sofar wave data
 Home-page: https://github.com/sofarocean/roguewave.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Platform: UNKNOWN
```

### Comparing `roguewave-0.2.8/README.md` & `roguewave-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/setup.py` & `roguewave-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="roguewave",
-    version="0.2.8",
+    version="0.2.9",
     license="Apache 2 License",
     install_requires=[
         "pysofar>=0.1.13",
         "numpy",
         "netCDF4",
         "pandas",
         "scipy",
```

### Comparing `roguewave-0.2.8/src/roguewave/__init__.py` & `roguewave-0.2.9/src/roguewave/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/colocate/bulk.py` & `roguewave-0.2.9/src/roguewave/colocate/bulk.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/colocate/pointdata.py` & `roguewave-0.2.9/src/roguewave/colocate/pointdata.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/colocate/spectra.py` & `roguewave-0.2.9/src/roguewave/colocate/spectra.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/filecache/cache_object.py` & `roguewave-0.2.9/src/roguewave/filecache/cache_object.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/filecache/filecache.py` & `roguewave-0.2.9/src/roguewave/filecache/filecache.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/filecache/remote_resources.py` & `roguewave-0.2.9/src/roguewave/filecache/remote_resources.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/cluster.py` & `roguewave-0.2.9/src/roguewave/interpolate/cluster.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/dataarray.py` & `roguewave-0.2.9/src/roguewave/interpolate/dataarray.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/dataframe.py` & `roguewave-0.2.9/src/roguewave/interpolate/dataframe.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/dataset.py` & `roguewave-0.2.9/src/roguewave/interpolate/dataset.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/general.py` & `roguewave-0.2.9/src/roguewave/interpolate/general.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/geometry.py` & `roguewave-0.2.9/src/roguewave/interpolate/geometry.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/nd_interp.py` & `roguewave-0.2.9/src/roguewave/interpolate/nd_interp.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/interpolate/points.py` & `roguewave-0.2.9/src/roguewave/interpolate/points.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/io/io.py` & `roguewave-0.2.9/src/roguewave/io/io.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/log.py` & `roguewave-0.2.9/src/roguewave/log.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/__init__.py` & `roguewave-0.2.9/src/roguewave/modeldata/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/extract.py` & `roguewave-0.2.9/src/roguewave/modeldata/extract.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/keygeneration.py` & `roguewave-0.2.9/src/roguewave/modeldata/keygeneration.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/modelinformation.py` & `roguewave-0.2.9/src/roguewave/modeldata/modelinformation.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/open_remote.py` & `roguewave-0.2.9/src/roguewave/modeldata/open_remote.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/remote_point_data.py` & `roguewave-0.2.9/src/roguewave/modeldata/remote_point_data.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/sofar_api/environment.py` & `roguewave-0.2.9/src/roguewave/modeldata/sofar_api/environment.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/sofar_api/sofar_api.py` & `roguewave-0.2.9/src/roguewave/modeldata/sofar_api/sofar_api.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/sofar_api/utils.py` & `roguewave-0.2.9/src/roguewave/modeldata/sofar_api/utils.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/sofarspectralapi.py` & `roguewave-0.2.9/src/roguewave/modeldata/sofarspectralapi.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/modeldata/timebase.py` & `roguewave-0.2.9/src/roguewave/modeldata/timebase.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/observations/satellite.py` & `roguewave-0.2.9/src/roguewave/observations/satellite.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/analysis.py` & `roguewave-0.2.9/src/roguewave/spotter/analysis.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/FLT.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/FLT.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/GMN.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/GMN.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/GPS.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/GPS.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/LOC.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/LOC.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/SPC.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/SPC.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/TIME.json` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/TIME.json`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/_create_formats.py` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/_create_formats.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/file_formats/_create_spectral_format.py` & `roguewave-0.2.9/src/roguewave/spotter/file_formats/_create_spectral_format.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/parser.py` & `roguewave-0.2.9/src/roguewave/spotter/parser.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotter/read_csv_data.py` & `roguewave-0.2.9/src/roguewave/spotter/read_csv_data.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotterapi/helper_functions.py` & `roguewave-0.2.9/src/roguewave/spotterapi/helper_functions.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotterapi/search_endpoint.py` & `roguewave-0.2.9/src/roguewave/spotterapi/search_endpoint.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotterapi/spotter_cache.py` & `roguewave-0.2.9/src/roguewave/spotterapi/spotter_cache.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotterapi/spotterapi.py` & `roguewave-0.2.9/src/roguewave/spotterapi/spotterapi.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/spotterapi/spottersdcard.py` & `roguewave-0.2.9/src/roguewave/spotterapi/spottersdcard.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/timeseries_analysis/filtering.py` & `roguewave-0.2.9/src/roguewave/timeseries_analysis/filtering.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/timeseries_analysis/pipeline.py` & `roguewave-0.2.9/src/roguewave/timeseries_analysis/pipeline.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/timeseries_analysis/upsampling.py` & `roguewave-0.2.9/src/roguewave/timeseries_analysis/upsampling.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/timeseries_analysis/welch.py` & `roguewave-0.2.9/src/roguewave/timeseries_analysis/welch.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/tools/grid.py` & `roguewave-0.2.9/src/roguewave/tools/grid.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/tools/math.py` & `roguewave-0.2.9/src/roguewave/tools/math.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/tools/solvers.py` & `roguewave-0.2.9/src/roguewave/tools/solvers.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/tools/time.py` & `roguewave-0.2.9/src/roguewave/tools/time.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/tools/time_integration.py` & `roguewave-0.2.9/src/roguewave/tools/time_integration.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/balance.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/balance.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/dissipation.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/dissipation.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/factory.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/factory.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/generation.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/generation.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/jb23_tail_stress.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/jb23_tail_stress.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/jb23_wind_input.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/jb23_wind_input.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/romero_wave_breaking.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/romero_wave_breaking.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/solvers.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/solvers.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/source_term.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/source_term.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_swell_dissipation.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_swell_dissipation.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_wave_breaking.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_wave_breaking.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/st4_wind_input.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/st4_wind_input.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/st6_wave_breaking.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/st6_wave_breaking.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/st6_wind_input.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/st6_wind_input.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/stress.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/stress.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/wam_tail_stress.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/wam_tail_stress.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/balance/wind_inversion.py` & `roguewave-0.2.9/src/roguewave/wavephysics/balance/wind_inversion.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/fluidproperties.py` & `roguewave-0.2.9/src/roguewave/wavephysics/fluidproperties.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/roughness.py` & `roguewave-0.2.9/src/roguewave/wavephysics/roughness.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/train_wind_estimate.py` & `roguewave-0.2.9/src/roguewave/wavephysics/train_wind_estimate.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavephysics/windestimate.py` & `roguewave-0.2.9/src/roguewave/wavephysics/windestimate.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/__init__.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/estimate.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/estimate.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/loglikelyhood.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/loglikelyhood.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/mem.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/mem.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/mem2.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/mem2.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/estimators/utils.py` & `roguewave-0.2.9/src/roguewave/wavespectra/estimators/utils.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/operations.py` & `roguewave-0.2.9/src/roguewave/wavespectra/operations.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/parametric.py` & `roguewave-0.2.9/src/roguewave/wavespectra/parametric.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/partitioning/classifiers.py` & `roguewave-0.2.9/src/roguewave/wavespectra/partitioning/classifiers.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/partitioning/observations.py` & `roguewave-0.2.9/src/roguewave/wavespectra/partitioning/observations.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/partitioning/partitioning.py` & `roguewave-0.2.9/src/roguewave/wavespectra/partitioning/partitioning.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/partitioning/wavefields.py` & `roguewave-0.2.9/src/roguewave/wavespectra/partitioning/wavefields.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/spectrum.py` & `roguewave-0.2.9/src/roguewave/wavespectra/spectrum.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     DataArray,
     open_dataset,
     concat,
     ones_like,
     where,
     zeros_like,
 )
-from roguewave.tools.grid import midpoint_rule_step
 from xarray.core.coordinates import DatasetCoordinates
 from warnings import warn
-from scipy.interpolate import CubicSpline, Akima1DInterpolator, make_interp_spline
-from roguewave.wavespectra._tools import numba_fill_zeros_or_nan_in_tail
+from roguewave.wavespectra._tools import (
+    numba_fill_zeros_or_nan_in_tail,
+    cumulative_frequency_interpolation_1d_variable,
+    spline_peak_frequency,
+)
 
 NAME_F: Literal["frequency"] = "frequency"
 NAME_D: Literal["direction"] = "direction"
 NAME_T: Literal["time"] = "time"
 NAME_E: Literal["variance_density"] = "variance_density"
 NAME_a1: Literal["a1"] = "a1"
 NAME_b1: Literal["b1"] = "b1"
@@ -1419,201 +1421,7 @@
     for name in spectrum.dataset:
         if name in SPECTRAL_VARS:
             continue
         else:
             dataset = dataset.assign({name: spectrum.dataset[name]})
 
     return FrequencySpectrum(dataset)
-
-
-def cumulative_frequency_interpolation_1d_variable(
-    interpolation_frequency, dataset: Dataset
-):
-    """
-    To interpolate the spectrum we first calculate a cumulative density function from the spectrum (which is essentialy
-    a pdf). We then interpolate the CDF function with a spline and differentiate the result.
-
-    :param interpolation_frequency:
-    :param dataset:
-    :return:
-    """
-
-    _dataset = Dataset()
-
-    # Copy over all non spectral vars
-    for name in dataset:
-        _name = str(name)
-        if _name not in SPECTRAL_VARS:
-            _dataset = _dataset.assign({_name: dataset[_name]})
-
-    coords = {
-        str(_coor_name): dataset[str(_coor_name)]
-        for _coor_name in dataset[NAME_E].coords
-    }
-    coords[NAME_F] = interpolation_frequency
-    dims = dataset[NAME_E].dims
-
-    # Interpolate energy
-    interpolated_energy = _cdf_interpolate(
-        interpolation_frequency,
-        dataset[NAME_F].values,
-        dataset[NAME_E].values,
-        interpolating_spline_order=3,
-        positive=True,
-    )
-
-    _dataset = _dataset.assign(
-        {
-            NAME_E: DataArray(
-                data=interpolated_energy,
-                coords=coords,
-                dims=dims,
-            )
-        }
-    )
-
-    # Interpolate scaling energy, to be used to renormalize moments.
-    interpolated_energy = _cdf_interpolate(
-        interpolation_frequency,
-        dataset[NAME_F].values,
-        dataset[NAME_E].values,
-        interpolating_spline_order=1,
-        positive=False,
-    )
-
-    for _name in SPECTRAL_MOMENTS:
-        interpolated_densities = (
-            _cdf_interpolate(
-                interpolation_frequency,
-                dataset[NAME_F].values,
-                dataset[_name].values * dataset[NAME_E].values,
-                interpolating_spline_order=1,
-                positive=False,
-            )
-            / interpolated_energy
-        )
-
-        _dataset = _dataset.assign(
-            {
-                _name: DataArray(
-                    data=interpolated_densities,
-                    coords=coords,
-                    dims=dims,
-                )
-            }
-        )
-
-    return _dataset
-
-
-def _cdf_interpolate(
-    interpolation_frequency: numpy.ndarray,
-    frequency: numpy.ndarray,
-    frequency_spectrum: numpy.ndarray,
-    interpolating_spline_order: int = 3,
-    positive: bool = False,
-) -> numpy.ndarray:
-    """
-    Interpolate the spectrum using the cdf.
-
-    :param interpolation_frequency: frequencies to estimate the spectrum at.
-    :param frequency: Frequencies of the spectrum. Shape = ( nf, )
-    :param frequency_spectrum: Frequency Variance density spectrum. Shape = ( np , nf )
-    :param interpolating_spline_order: Order of the spline to use in the interpolation (max 5 supported by scipy)
-    :param positive: Ensure the output is positive (e.g. for A1 or B1 densities output need not be strictly positive).
-    :return:
-    """
-    #
-    frequency_step = midpoint_rule_step(frequency)
-    integration_frequencies = numpy.concatenate(([0], numpy.cumsum(frequency_step)))
-    integration_frequencies = (
-        integration_frequencies - frequency_step[0] / 2 + frequency[0]
-    )
-
-    cumsum = numpy.cumsum(frequency_spectrum * frequency_step, axis=-1)
-    cumsum = numpy.concatenate((numpy.zeros((cumsum.shape[0], 1)), cumsum), axis=-1)
-
-    interpolator = make_interp_spline(
-        integration_frequencies, cumsum, axis=-1, k=interpolating_spline_order
-    ).derivative()
-    interpolated_densities = interpolator(interpolation_frequency)
-
-    if positive:
-        mask = interpolated_densities < 0.0
-        if numpy.any(mask):
-            monotone_interpolator = Akima1DInterpolator(
-                integration_frequencies, cumsum, axis=-1
-            ).derivative()
-            positive_densities = monotone_interpolator(interpolation_frequency)
-            interpolated_densities[mask] = positive_densities[mask]
-
-    return interpolated_densities
-
-
-def spline_peak_frequency(
-    frequency: numpy.ndarray, frequency_spectrum: numpy.ndarray
-) -> numpy.ndarray:
-    """
-    Estimate the peak frequency of the spectrum based on a cubic spline interpolation of the partially integrated
-    variance.
-
-    :param frequency: Frequencies of the spectrum. Shape = ( nf, )
-    :param frequency_spectrum: Frequency Variance density spectrum. Shape = ( np , nf )
-    :return: peak frequencies. Shape = ( np, )
-    """
-    #
-
-    # Calculate the binsize for each of the frequency bins. We assume that the given frequencies represent the center
-    # of a bin, and that the bin width at frequency i is determined as the sum of half the up and downwind differences:
-    #
-    #  frequency_step[i]   =  (frequency_step[i] - frequency_step[i-1])/2 + (frequency_step[i+1] - frequency_step[i])/2
-    #
-    # At boundaries we simply take twice the up or downwind difference, e.g.:
-    #
-    # frequency_step[0] = (frequency_step[1] - frequency_step[0])
-    #
-    frequency_step = midpoint_rule_step(frequency)
-
-    # Whereas the given frequencies represent the center, we assume that cumulative function is sampled at the bin
-    # edges. First create the cumulative sum frequency relative to the start...
-    integration_frequencies = numpy.concatenate(([0], numpy.cumsum(frequency_step)))
-
-    # and then add the origin (first bin centered frequency minus half the step size.
-    integration_frequencies = (
-        integration_frequencies - frequency_step[0] / 2 + frequency[0]
-    )
-
-    # Since spectra are typicall given as densities, muliply with the step to get the bin integrated values.
-    bin_integrated_values = frequency_spectrum * frequency_step
-
-    # calculate the cumulative function
-    cumsum = numpy.cumsum(bin_integrated_values, axis=-1)
-
-    # Add leading 0s as at the first frequency the integration is 0.
-    cumsum = numpy.concatenate((numpy.zeros((cumsum.shape[0], 1)), cumsum), axis=-1)
-
-    # Construct a cubic spline interpolator, and then differentiate to get the density function.
-    interpolator = CubicSpline(integration_frequencies, cumsum, axis=-1).derivative()
-
-    # Find the maxima of the density function by setting dEdf = 0, and finding the roots of all the splines representing
-    # the density function.
-    list_of_roots_for_all_spectra = interpolator.derivative().roots()
-
-    # initialize output memory
-    peak_frequency = numpy.zeros(len(list_of_roots_for_all_spectra))
-
-    # We now have a list in which each entry contains all the roots for that given spectrum. Loop over each spectrum
-    # and..
-    for index, root in enumerate(list_of_roots_for_all_spectra):
-        # ..evaluate density spectrum at those roots.
-        values_at_roots = interpolator(root)
-
-        # Because the interpolator returns values at the current roots evaluated at _all_ spectra, we still have to
-        # select the values at the spectrum of interest. This implementation is silly, adds computational costs, and can
-        # probably be improved. It seems "fast enough" so that I'll punt that to another time.
-        values_at_roots = values_at_roots[index, :]
-
-        # ... get the root that corresponds to the largest peak.
-        index_peak = numpy.argmax(values_at_roots)
-        peak_frequency[index] = root[index_peak]
-
-    return peak_frequency
```

### Comparing `roguewave-0.2.8/src/roguewave/wavespectra/timeseries.py` & `roguewave-0.2.9/src/roguewave/wavespectra/timeseries.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavetheory/lineardispersion.py` & `roguewave-0.2.9/src/roguewave/wavetheory/lineardispersion.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/__init__.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/fortran_types.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/fortran_types.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/grid_tools.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/grid_tools.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/io.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/io.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/model_definition.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/model_definition.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/resources.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/resources.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/restart_file.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/restart_file.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_cache.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_cache.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_metadata.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_metadata.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave/wavewatch3/restart_file_time_stack.py` & `roguewave-0.2.9/src/roguewave/wavewatch3/restart_file_time_stack.py`

 * *Files identical despite different names*

### Comparing `roguewave-0.2.8/src/roguewave.egg-info/PKG-INFO` & `roguewave-0.2.9/src/roguewave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewave
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package to interact with Sofar wave data
 Home-page: https://github.com/sofarocean/roguewave.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Platform: UNKNOWN
```

### Comparing `roguewave-0.2.8/src/roguewave.egg-info/SOURCES.txt` & `roguewave-0.2.9/src/roguewave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

