# Comparing `tmp/nctoolkit-0.9.1.tar.gz` & `tmp/nctoolkit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nctoolkit-0.9.1.tar", last modified: Wed Apr 19 16:51:49 2023, max compression
+gzip compressed data, was "nctoolkit-0.9.2.tar", last modified: Tue Apr 25 11:10:34 2023, max compression
```

## Comparing `nctoolkit-0.9.1.tar` & `nctoolkit-0.9.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.180344 nctoolkit-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-19 16:51:49.180344 nctoolkit-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.172344 nctoolkit-0.9.1/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (123)   257155 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/cheatsheet/nctoolkit_cheatsheet.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   362394 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/cheatsheet/nctoolkit_cheatsheet.pptx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.172344 nctoolkit-0.9.1/checklists/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-19 16:51:35.000000 nctoolkit-0.9.1/checklists/api_checker.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.176344 nctoolkit-0.9.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-04-19 16:51:36.000000 nctoolkit-0.9.1/data/geotiff.tif
--rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-04-19 16:51:36.000000 nctoolkit-0.9.1/data/test1.html
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-04-19 16:51:36.000000 nctoolkit-0.9.1/data/test2.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.180344 nctoolkit-0.9.1/nctoolkit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/add_etc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/anomaly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58911 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/append.py
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/cdo_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/cellareas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/centres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/clear.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7360 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/compare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/corr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/create_ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5265 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/distgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3666 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/esoteric.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/fill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/fldstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/format.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/generate_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/inttime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/masking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/matchpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/meridonials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/mp_adders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/mp_matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/mp_matchups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/nco_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/phenology.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2558 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/reduce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/reduce_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6416 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/regrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/rename.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/rollstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    46030 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/runthis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/setters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/split.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19270 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/static_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/strip_vars.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15954 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/sumall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/temporal_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/temporals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/thresholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/to_lonlat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/to_nc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3594 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/toxarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/tozlev.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/unify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22629 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/validator_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19600 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/verticals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/nctoolkit/zonals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:51:49.180344 nctoolkit-0.9.1/nctoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-19 16:51:49.000000 nctoolkit-0.9.1/nctoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:51:49.180344 nctoolkit-0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-04-19 16:51:37.000000 nctoolkit-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.764715 nctoolkit-0.9.2/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)   257155 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   362394 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pptx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.764715 nctoolkit-0.9.2/checklists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/checklists/api_checker.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.768715 nctoolkit-0.9.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/geotiff.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/test1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/test2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/nctoolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/add_etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/anomaly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58907 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/append.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cdo_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cellareas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/centres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/clear.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7360 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/compare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/corr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/create_ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5265 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/distgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3666 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/esoteric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/fill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/fldstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/format.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/generate_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/inttime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/matchpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/meridonials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_adders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_matchups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/nco_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/phenology.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2558 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/reduce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/reduce_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6416 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/regrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/rename.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/rollstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46030 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/runthis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/split.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19267 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/static_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/strip_vars.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15954 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/sumall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temporal_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temporals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/thresholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/to_lonlat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/to_nc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3594 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/toxarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/tozlev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/unify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22629 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/validator_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19600 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/verticals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/zonals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/nctoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-25 11:10:34.000000 nctoolkit-0.9.2/nctoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/setup.py
```

### Comparing `nctoolkit-0.9.1/CODE_OF_CONDUCT.md` & `nctoolkit-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/LICENSE` & `nctoolkit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/MANIFEST.in` & `nctoolkit-0.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/PKG-INFO` & `nctoolkit-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nctoolkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Fast and easy analysis of netCDF data in Python
 Home-page: https://github.com/pmlmodelling/nctoolkit
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/nctoolkit/issues
 Project-URL: Documentation, https://nctoolkit.readthedocs.io/en/stable
```

### Comparing `nctoolkit-0.9.1/README.md` & `nctoolkit-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/cheatsheet/nctoolkit_cheatsheet.pdf` & `nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/cheatsheet/nctoolkit_cheatsheet.pptx` & `nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pptx`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/checklists/api_checker.ipynb` & `nctoolkit-0.9.2/checklists/api_checker.ipynb`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/data/geotiff.tif` & `nctoolkit-0.9.2/data/geotiff.tif`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/data/test1.html` & `nctoolkit-0.9.2/data/test1.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/data/test2.html` & `nctoolkit-0.9.2/data/test2.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/__init__.py` & `nctoolkit-0.9.2/nctoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/add_etc.py` & `nctoolkit-0.9.2/nctoolkit/add_etc.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/anomaly.py` & `nctoolkit-0.9.2/nctoolkit/anomaly.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/api.py` & `nctoolkit-0.9.2/nctoolkit/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1836,15 +1836,15 @@
     from nctoolkit.nco_command import nco_command
 
     from nctoolkit.phenology import phenology
 
     # from nctoolkit.phenology import initiation
 
     from nctoolkit.plot import plot
-    #from nctoolkit.static_plot import static_plot
+    from nctoolkit.static_plot import pub_plot
 
     from nctoolkit.reduce import reduce_dims
 
     from nctoolkit.reduce_grid import reduce_grid
 
     from nctoolkit.regrid import regrid
```

### Comparing `nctoolkit-0.9.1/nctoolkit/append.py` & `nctoolkit-0.9.2/nctoolkit/append.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/assign.py` & `nctoolkit-0.9.2/nctoolkit/assign.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/cdo_command.py` & `nctoolkit-0.9.2/nctoolkit/cdo_command.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/cellareas.py` & `nctoolkit-0.9.2/nctoolkit/cellareas.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/centres.py` & `nctoolkit-0.9.2/nctoolkit/centres.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/checks.py` & `nctoolkit-0.9.2/nctoolkit/checks.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/cleanup.py` & `nctoolkit-0.9.2/nctoolkit/cleanup.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/clear.py` & `nctoolkit-0.9.2/nctoolkit/clear.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/compare.py` & `nctoolkit-0.9.2/nctoolkit/compare.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/compare_data.py` & `nctoolkit-0.9.2/nctoolkit/compare_data.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/corr.py` & `nctoolkit-0.9.2/nctoolkit/corr.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/create_ensemble.py` & `nctoolkit-0.9.2/nctoolkit/create_ensemble.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/crop.py` & `nctoolkit-0.9.2/nctoolkit/crop.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/distgrid.py` & `nctoolkit-0.9.2/nctoolkit/distgrid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/drop.py` & `nctoolkit-0.9.2/nctoolkit/drop.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/ensembles.py` & `nctoolkit-0.9.2/nctoolkit/ensembles.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/esoteric.py` & `nctoolkit-0.9.2/nctoolkit/esoteric.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/fldstat.py` & `nctoolkit-0.9.2/nctoolkit/fldstat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/format.py` & `nctoolkit-0.9.2/nctoolkit/format.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/generate_grid.py` & `nctoolkit-0.9.2/nctoolkit/generate_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/inttime.py` & `nctoolkit-0.9.2/nctoolkit/inttime.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/masking.py` & `nctoolkit-0.9.2/nctoolkit/masking.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/matchpoint.py` & `nctoolkit-0.9.2/nctoolkit/matchpoint.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/mergers.py` & `nctoolkit-0.9.2/nctoolkit/mergers.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/meridonials.py` & `nctoolkit-0.9.2/nctoolkit/meridonials.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/mp_adders.py` & `nctoolkit-0.9.2/nctoolkit/mp_adders.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/mp_matchers.py` & `nctoolkit-0.9.2/nctoolkit/mp_matchers.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/mp_matchups.py` & `nctoolkit-0.9.2/nctoolkit/mp_matchups.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/nco_command.py` & `nctoolkit-0.9.2/nctoolkit/nco_command.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/phenology.py` & `nctoolkit-0.9.2/nctoolkit/phenology.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/plot.py` & `nctoolkit-0.9.2/nctoolkit/plot.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/reduce.py` & `nctoolkit-0.9.2/nctoolkit/reduce.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/reduce_grid.py` & `nctoolkit-0.9.2/nctoolkit/reduce_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/regrid.py` & `nctoolkit-0.9.2/nctoolkit/regrid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/remove.py` & `nctoolkit-0.9.2/nctoolkit/remove.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/rename.py` & `nctoolkit-0.9.2/nctoolkit/rename.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/resample.py` & `nctoolkit-0.9.2/nctoolkit/resample.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/rollstat.py` & `nctoolkit-0.9.2/nctoolkit/rollstat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/run.py` & `nctoolkit-0.9.2/nctoolkit/run.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/runthis.py` & `nctoolkit-0.9.2/nctoolkit/runthis.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/session.py` & `nctoolkit-0.9.2/nctoolkit/session.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/set.py` & `nctoolkit-0.9.2/nctoolkit/set.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/setters.py` & `nctoolkit-0.9.2/nctoolkit/setters.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/shape.py` & `nctoolkit-0.9.2/nctoolkit/shape.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/shift.py` & `nctoolkit-0.9.2/nctoolkit/shift.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/show.py` & `nctoolkit-0.9.2/nctoolkit/show.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/split.py` & `nctoolkit-0.9.2/nctoolkit/split.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/static_plot.py` & `nctoolkit-0.9.2/nctoolkit/static_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if new_x == "(1/m)":
         new_x = "(m$^{-1}$)"
     if new_x == "(degC)":
         new_x = "(°C)"
     return new_x[1:-1]
 
 
-def static_plot(
+def pub_plot(
     ds,
     extent=None,
     title=None,
     legend=None,
     size="auto",
     land="auto",
     colours="auto",
```

### Comparing `nctoolkit-0.9.1/nctoolkit/strip_vars.py` & `nctoolkit-0.9.2/nctoolkit/strip_vars.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/subset.py` & `nctoolkit-0.9.2/nctoolkit/subset.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/sumall.py` & `nctoolkit-0.9.2/nctoolkit/sumall.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/temp_file.py` & `nctoolkit-0.9.2/nctoolkit/temp_file.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/temporal_stat.py` & `nctoolkit-0.9.2/nctoolkit/temporal_stat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/temporals.py` & `nctoolkit-0.9.2/nctoolkit/temporals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/thresholds.py` & `nctoolkit-0.9.2/nctoolkit/thresholds.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/to_lonlat.py` & `nctoolkit-0.9.2/nctoolkit/to_lonlat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/to_nc.py` & `nctoolkit-0.9.2/nctoolkit/to_nc.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/toxarray.py` & `nctoolkit-0.9.2/nctoolkit/toxarray.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/tozlev.py` & `nctoolkit-0.9.2/nctoolkit/tozlev.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/unify.py` & `nctoolkit-0.9.2/nctoolkit/unify.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/utils.py` & `nctoolkit-0.9.2/nctoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/validator.py` & `nctoolkit-0.9.2/nctoolkit/validator.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/validator_funs.py` & `nctoolkit-0.9.2/nctoolkit/validator_funs.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/verticals.py` & `nctoolkit-0.9.2/nctoolkit/verticals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit/zonals.py` & `nctoolkit-0.9.2/nctoolkit/zonals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/nctoolkit.egg-info/SOURCES.txt` & `nctoolkit-0.9.2/nctoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.1/setup.py` & `nctoolkit-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 extras_require["complete"] = ["geoviews", "rioxarray", "cfchecker", "geocube", "geopandas"]
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(name='nctoolkit',
-      version='0.9.1',
+      version='0.9.2',
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       python_requires='>=3.6.1',
       classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
```

