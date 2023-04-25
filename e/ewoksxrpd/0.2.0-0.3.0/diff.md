# Comparing `tmp/ewoksxrpd-0.2.0.tar.gz` & `tmp/ewoksxrpd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksxrpd-0.2.0.tar", last modified: Sat Mar 11 16:59:06 2023, max compression
+gzip compressed data, was "dist/ewoksxrpd-0.3.0.tar", last modified: Tue Apr 25 12:03:30 2023, max compression
```

## Comparing `ewoksxrpd-0.2.0.tar` & `ewoksxrpd-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1299 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-11 16:55:59.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-11 16:58:59.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20304 2023-03-11 16:27:33.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/plots.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/gui/trigger_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/init_matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/background.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)    15723 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/convolution.py
--rw-rw-rw-   0 root         (0) root         (0)     1859 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/data_access.py
--rw-rw-rw-   0 root         (0) root         (0)     8789 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    13236 2023-03-11 16:46:12.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/mask.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/morphology.py
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-03-11 16:27:33.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-03-11 14:18:51.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-11 16:58:59.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9454 2023-03-11 16:27:33.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2023-03-11 16:46:12.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-11 16:58:59.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5818 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_batch_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
--rw-rw-rw-   0 root         (0) root         (0)    10366 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)    20665 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_calint_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     4297 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/ewoksxrpd/tests/xrpd_theory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1299 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2668 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      259 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-11 16:59:05.000000 ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/background.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-03-11 16:27:33.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-03-11 16:27:33.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
--rw-rw-rw-   0 root         (0) root         (0)    11135 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
--rw-rw-rw-   0 root         (0) root         (0)     7826 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-11 16:58:59.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/category.png
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/widget.png
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1958 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-03-11 13:04:29.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 16:59:06.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-11 16:58:59.000000 ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20304 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/trigger_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/init_matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/background.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)    15723 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/convolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/data_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     8789 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    14901 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/morphology.py
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/pyfaiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2745 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9454 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4419 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5823 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_batch_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
+-rw-rw-rw-   0 root         (0) root         (0)    10366 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20665 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calint_workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     4297 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/xrpd_theory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      257 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    11135 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
+-rw-rw-rw-   0 root         (0) root         (0)     7826 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/category.png
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/widget.png
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1958 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
```

### Comparing `ewoksxrpd-0.2.0/LICENSE.md` & `ewoksxrpd-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/PKG-INFO` & `ewoksxrpd-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
```

### Comparing `ewoksxrpd-0.2.0/README.md` & `ewoksxrpd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/setup.cfg` & `ewoksxrpd-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy
 	scipy
 	silx >=1.1.0
-	pyfai >=2023.1,!=2023.2
-	ewoksdata >=0.0.3a0
 	pyopencl
+	pyfai >=2023.1,!=2023.2
+	ewoksdata >=0.2.5
 	ewoks[orange] >=0.1.2
 namespace_packages = 
 	orangecontrib
 
 [options.packages.find]
 where = src
```

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/gui/forms.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/forms.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/gui/plots.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/plots.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/gui/serialize.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/serialize.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/gui/trigger_widget.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/init_matplotlib.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/init_matplotlib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/ascii.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/background.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/calibrate.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/calibrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/data_access.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/data_access.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,12 +44,16 @@
 
     def get_image(self, *args, **kw):
         kw.update(self.get_retry_options())
         return bliss.get_image(*args, **kw)
 
     def iter_bliss_data(self, *args, **kw):
         kw.update(self.get_retry_options())
-        yield from bliss.iter_bliss_data(*args, **kw)
+        yield from bliss.iter_bliss_scan_data(*args, **kw)
+
+    def iter_bliss_data_from_memory(self, *args, **kw):
+        kw.update(self.get_retry_options())
+        yield from bliss.iter_bliss_scan_data_from_memory(*args, **kw)
 
     def link_bliss_scan(self, *args, **kw):
         kw.update(self.get_retry_options())
         return data_utils.link_bliss_scan(*args, **kw)
```

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/diagnostics.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/integrate.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/integrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from numbers import Number
 from contextlib import contextmanager, ExitStack
 from typing import Union, Tuple
 
 import numpy
 import h5py
 from ewoksdata.data.hdf5.dataset_writer import DatasetWriter
@@ -11,14 +12,17 @@
 from .utils import data_utils, xrpd_utils, pyfai_utils, integrate_utils
 from .data_access import TaskWithDataAccess
 
 
 __all__ = ["Integrate1D", "IntegrateBlissScan", "IntegrateBlissScanWithoutSaving"]
 
 
+logger = logging.getLogger(__name__)
+
+
 class _BaseIntegrate(
     TaskWithDataAccess,
     input_names=["detector", "geometry", "energy"],
     optional_input_names=[
         "detector_config",
         "mask",
         "integration_options",
@@ -138,17 +142,19 @@
         "counter_names",
         "monitor_name",
         "reference",
         "subscan",
         "retry_timeout",
         "retry_period",
         "demo",
+        "scan_memory_url",
         "nxprocess_name",
         "nxmeasurement_name",
         "nxprocess_as_default",
+        "flush_period",
     ],
 ):
     """1D or 2D integration of a single detector in a single Bliss scan with saving."""
 
     def run(self):
         if self.inputs.counter_names:
             counter_names = list(self.inputs.counter_names)
@@ -166,32 +172,49 @@
             if reference not in counter_names:
                 counter_names.append(reference)
 
         scan = self.inputs.scan
         subscan = self.get_input_value("subscan", 1)
         output_url = f"silx://{self.inputs.output_filename}?path=/{scan}.{subscan}"
         input_url = f"silx://{self.inputs.filename}?path=/{scan}.{subscan}"
+        flush_period = self.get_input_value("flush_period", None)
 
         with ExitStack() as stack:
             worker = None
             parent = None
             nxprocess = None
             measurement = None
 
             intensity_writer = None
             error_writer = None
             ctr_writers = dict()
 
-            for index, ptdata in self.iter_bliss_data(
-                self.inputs.filename,
-                self.inputs.scan,
-                lima_names=[detector_name],
-                counter_names=counter_names,
-                subscan=subscan,
-            ):
+            if self.inputs.scan_memory_url:
+                logger.info("PyFAI integrate data from %r", self.inputs.scan_memory_url)
+                data_iterator = self.iter_bliss_data_from_memory(
+                    self.inputs.scan_memory_url,
+                    lima_names=[detector_name],
+                    counter_names=counter_names,
+                )
+            else:
+                logger.info(
+                    "PyFAI integrate data from '%s::%d.%d'",
+                    self.inputs.filename,
+                    self.inputs.scan,
+                    subscan,
+                )
+                data_iterator = self.iter_bliss_data(
+                    self.inputs.filename,
+                    self.inputs.scan,
+                    lima_names=[detector_name],
+                    counter_names=counter_names,
+                    subscan=subscan,
+                )
+
+            for ptdata in data_iterator:
                 if worker is None:
                     # Start the worker + open the output file only after
                     # the first image is read
                     worker, config = stack.enter_context(self._worker())
                     info = pyfai_utils.compile_integration_info(
                         config, reference=reference
                     )
@@ -222,23 +245,25 @@
                         nxprocess,
                         result.intensity.ndim + 1,  # +1 for the scan dimension
                         result.radial,
                         result.unit,
                         result.azimuthal if result.intensity.ndim == 2 else None,
                     )
                     intensity_writer = stack.enter_context(
-                        DatasetWriter(nxdata, "intensity")
+                        DatasetWriter(nxdata, "intensity", flush_period=flush_period)
                     )
                     if result.sigma is not None:
                         error_writer = stack.enter_context(
-                            DatasetWriter(nxdata, "intensity_errors")
+                            DatasetWriter(
+                                nxdata, "intensity_errors", flush_period=flush_period
+                            )
                         )
                     for name in counter_names:
                         ctr_writers[name] = stack.enter_context(
-                            DatasetWriter(measurement, name)
+                            DatasetWriter(measurement, name, flush_period=flush_period)
                         )
 
                 flush = intensity_writer.add_point(result.intensity)
                 if result.sigma is not None:
                     flush |= error_writer.add_point(result.sigma)
                 for name in counter_names:
                     flush |= ctr_writers[name].add_point(ptdata[name])
@@ -288,14 +313,15 @@
         "counter_names",
         "monitor_name",
         "reference",
         "subscan",
         "retry_timeout",
         "retry_period",
         "demo",
+        "scan_memory_url",
     ],
     output_names=[
         "radial",
         "azimuthal",
         "intensity",
         "intensity_error",
         "radial_units",
@@ -324,21 +350,37 @@
 
             intensities = []
             sigmas = []
             radial = None
             unit = None
             azimuthal = None
 
-            for index, ptdata in self.iter_bliss_data(
-                self.inputs.filename,
-                self.inputs.scan,
-                lima_names=[detector_name],
-                counter_names=counter_names,
-                subscan=subscan,
-            ):
+            if self.inputs.scan_memory_url:
+                logger.info("PyFAI integrate data from %r", self.inputs.scan_memory_url)
+                data_iterator = self.iter_bliss_data_from_memory(
+                    self.inputs.scan_memory_url,
+                    lima_names=[detector_name],
+                    counter_names=counter_names,
+                )
+            else:
+                logger.info(
+                    "PyFAI integrate data from '%s::%d.%s'",
+                    self.inputs.filename,
+                    self.inputs.scan,
+                    subscan,
+                )
+                data_iterator = self.iter_bliss_data(
+                    self.inputs.filename,
+                    self.inputs.scan,
+                    lima_names=[detector_name],
+                    counter_names=counter_names,
+                    subscan=subscan,
+                )
+
+            for ptdata in data_iterator:
                 normalization_factor, *_ = self._pyfai_normalization_factor(
                     ptdata.get(monitor_name), ptdata.get(reference_name, reference)
                 )
                 image = ptdata[detector_name]
                 if self.inputs.demo:
                     image = image[:-1, :-1]
                 result = worker.process(
```

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/mask.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/morphology.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/morphology.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/nexus.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/pyfaiconfig.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/pyfaiconfig.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/data_utils.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tasks/worker.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/worker.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/conftest.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         sequence="multiply",
     )
 
 
 @pytest.fixture(scope="session")
 def bliss_task_inputs(bliss_lab6_scan, setup1) -> dict:
     return {
-        "filename": bliss_lab6_scan,
+        "filename": str(bliss_lab6_scan),
         "scan": 2,
         "detector": setup1.detector,
         "energy": setup1.energy,
         "geometry": setup1.geometry,
         "detector_name": "p3",
         "monitor_name": "monitor",
         "reference": 1.0,
```

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_ascii.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_background.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_batch_integrate.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_batch_integrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_calibrate.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_calint_workflow.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calint_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_integrate.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_mask.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_nexus.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_nexus_integrated.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/test_pyfai_utils.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_pyfai_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd/tests/xrpd_theory.py` & `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/xrpd_theory.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/PKG-INFO` & `ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
```

### Comparing `ewoksxrpd-0.2.0/src/ewoksxrpd.egg-info/SOURCES.txt` & `ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/__init__.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/ascii.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/background.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/batchintegrate.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/batchintegrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calculategeometry.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calculategeometry.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calibratemulti.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratemulti.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/calibratesingle.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratesingle.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/category.png` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/category.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/icons/widget.png` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/widget.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/integrate1d.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/integrate1d.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/mask.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/nexus.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.2.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py` & `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py`

 * *Files identical despite different names*

