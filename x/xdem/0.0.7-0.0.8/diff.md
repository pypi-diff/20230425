# Comparing `tmp/xdem-0.0.7.tar.gz` & `tmp/xdem-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdem-0.0.7.tar", last modified: Thu Aug 25 13:10:51 2022, max compression
+gzip compressed data, was "xdem-0.0.8.tar", last modified: Mon Apr 24 23:51:30 2023, max compression
```

## Comparing `xdem-0.0.7.tar` & `xdem-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 13:10:51.126997 xdem-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-25 13:10:36.000000 xdem-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5728 2022-08-25 13:10:51.126997 xdem-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-08-25 13:10:36.000000 xdem-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-25 13:10:36.000000 xdem-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 13:10:51.126997 xdem-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-08-25 13:10:36.000000 xdem-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 13:10:51.126997 xdem-0.0.7/xdem/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    84292 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/coreg.py
--rw-r--r--   0 runner    (1001) docker     (121)     7482 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/ddem.py
--rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/dem.py
--rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/demcollection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    17653 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)   128315 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/spatialstats.py
--rw-r--r--   0 runner    (1001) docker     (121)    66679 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/terrain.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-25 13:10:50.000000 xdem-0.0.7/xdem/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    34229 2022-08-25 13:10:36.000000 xdem-0.0.7/xdem/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 13:10:51.126997 xdem-0.0.7/xdem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5728 2022-08-25 13:10:51.000000 xdem-0.0.7/xdem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-25 13:10:51.000000 xdem-0.0.7/xdem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 13:10:51.000000 xdem-0.0.7/xdem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 13:10:50.000000 xdem-0.0.7/xdem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-25 13:10:51.000000 xdem-0.0.7/xdem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-25 13:10:51.000000 xdem-0.0.7/xdem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-24 23:51:10.000000 xdem-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 23:51:30.849684 xdem-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-24 23:51:10.000000 xdem-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 23:51:10.000000 xdem-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:51:30.849684 xdem-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 23:51:10.000000 xdem-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.845684 xdem-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_coreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_ddem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_demcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55340 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_spatialstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/xdem/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101810 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/coreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/ddem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/demcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152648 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/spatialstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67439 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33365 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/xdem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/top_level.txt
```

### Comparing `xdem-0.0.7/LICENSE` & `xdem-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xdem-0.0.7/PKG-INFO` & `xdem-0.0.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,94 @@
 Metadata-Version: 2.1
 Name: xdem
-Version: 0.0.7
+Version: 0.0.8
 Summary: Set of tools to manipulate Digital Elevation Models (DEMs) 
 Home-page: https://github.com/GlacioHack/xdem
 Author: The GlacioHack Team
 Author-email: this-is-not-an-email@a.com
 License: BSD-3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rioxarray
 Provides-Extra: richdem
 Provides-Extra: opencv
 Provides-Extra: pytransform3d
 License-File: LICENSE
 
-# xdem
-Set of tools to manipulate Digital Elevation Models (DEMs)
-
-More documentation to come!
+# xDEM: robust analysis of DEMs in Python.
 
 [![Documentation Status](https://readthedocs.org/projects/xdem/badge/?version=latest)](https://xdem.readthedocs.io/en/latest/?badge=latest)
 [![build](https://github.com/GlacioHack/xdem/actions/workflows/python-package.yml/badge.svg)](https://github.com/GlacioHack/xdem/actions/workflows/python-package.yml)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
+[![PyPI version](https://badge.fury.io/py/xdem.svg)](https://badge.fury.io/py/xdem)
 [![Coverage Status](https://coveralls.io/repos/github/GlacioHack/xdem/badge.svg?branch=main)](https://coveralls.io/github/GlacioHack/xdem?branch=main)
 
-To cite this package: [![Zenodo](https://zenodo.org/badge/doi/10.5281/zenodo.4809697.svg)](https://zenodo.org/record/4809698)
-
-## Installation
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GlacioHack/xdem/main)
+[![Pre-Commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+**xDEM** is an open source project to develop a core Python package for the analysis of digital elevation models (DEMs).
+
+It aims at **providing modular and robust tools for the most common analyses needed with DEMs**, including both geospatial
+operations specific to DEMs and a wide range of 3D alignment and correction methods from published, peer-reviewed studies.
+The core manipulation of DEMs (e.g., vertical alignment, terrain analysis) are **conveniently centered around `DEM` and `dDEM` classes** (that, notably, re-implements all tools
+of [gdalDEM](https://gdal.org/programs/gdaldem.html)). More complex pipelines (e.g., 3D rigid coregistration, bias corrections, filtering) are **built around
+modular `Coreg`, `BiasCorr` and `Filter` classes that easily interface between themselves**. Finally, xDEM includes advanced
+uncertainty analysis tools based on spatial statistics of [SciKit-GStat](https://scikit-gstat.readthedocs.io/en/latest/).
+
+Additionally, xDEM inherits many convenient functionalities from [GeoUtils](https://github.com/GlacioHack/geoutils) such as
+**implicit loading**, **numerical interfacing** and **convenient object-based geospatial methods** to easily perform
+the most common higher-level tasks needed by geospatial users (e.g., reprojection, cropping, vector masking). Through [GeoUtils](https://github.com/GlacioHack/geoutils), xDEM
+relies on [Rasterio](https://github.com/rasterio/rasterio), [GeoPandas](https://github.com/geopandas/geopandas) and [Pyproj](https://github.com/pyproj4/pyproj)
+for georeferenced calculations, and on [NumPy](https://github.com/numpy/numpy) and [Xarray](https://github.com/pydata/xarray) for numerical analysis. It allows easy access to
+the functionalities of these packages through interfacing or composition, and quick inter-operability through object conversion.
+
+If you are looking for an accessible Python package to write the Python equivalent of your [GDAL](https://gdal.org/) command lines, or of your
+[QGIS](https://www.qgis.org/en/site/) analysis pipeline **without a steep learning curve** on Python GIS syntax, xDEM is perfect for you! For more advanced
+users, xDEM also aims at being efficient and scalable by supporting lazy loading and parallel computing (ongoing).
 
-### With conda (recommended)
-```bash
-conda install -c conda-forge --strict-channel-priority xdem
-```
-The `--strict-channel-priority` flag seems essential for Windows installs to function correctly, and is recommended for UNIX-based systems as well.
-
-Solving dependencies can take a long time with `conda`. To speed up this, consider installing `mamba`:
-
-```bash
-conda install mamba -n base -c conda-forge
-```
+## Documentation
 
-Once installed, the same commands can be run by simply replacing `conda` by `mamba`. More details available through the [mamba project](https://github.com/mamba-org/mamba).
+For a quick start, full feature description or search through the API, see xDEM's documentation at: https://xdem.readthedocs.io.
 
-If running into the `sklearn` error `ImportError: dlopen: cannot load any more object with static TLS`, your system 
-needs to update its `glibc` (see details [here](https://github.com/scikit-learn/scikit-learn/issues/14485#issuecomment-822678559)).
-If you have no administrator right on the system, you might be able to circumvent this issue by installing a working 
-environment with specific downgraded versions of `scikit-learn` and `numpy`:
-```bash
-conda create -n xdem-env -c conda-forge xdem scikit-learn==0.20.3 numpy==1.19.*
-```
-On very old systems, if the above install results in segmentation faults, try setting more specifically 
-`numpy==1.19.2=py37h54aff64_0` (worked with Debian 8.11, GLIBC 2.19).
+## Installation
 
-### Installing with pip
-**NOTE**: Setting up GDAL and PROJ may need some extra steps, depending on your operating system and configuration.
 ```bash
-pip install xdem
-```
-
-### Installing for contributors
-Recommended: Use conda for depencency solving.
-```
-$ git clone https://github.com/GlacioHack/xdem.git
-$ cd ./xdem
-$ conda env create -f dev-environment.yml
-$ conda activate xdem
-$ pip install -e .
-```
-After installing, we recommend to check that everything is working by running the tests:
-
+mamba install -c conda-forge xdem
 ```
-$ pytest -rA
-```
-
-## Structure 
-
-xdem are for now composed of three libraries:
-- `coreg.py` with tools covering differet aspects of DEM coregistration
-- `spatial_tools.py` for spatial operations on DEMs
-- `dem.py` for DEM-specific operations, such as vertical datum correction.
-
-## How to contribute
-
-You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/xdem/issues) section. All contributions are welcome.
-To avoid conflicts, it is suggested to use separate branches for each implementation. All changes must then be submitted to the dev branch using pull requests. Each PR must be reviewed by at least one other person.
-
-Please see our [contribution page](CONTRIBUTING.md) for more detailed instructions.
-
-### Documentation
-See the documentation at https://xdem.readthedocs.io
-
-### Testing - again please read!
-These tools are only valuable if we can rely on them to perform exactly as we expect. So, we need testing. Please create tests for every function that you make, as much as you are able. Guidance/examples here for the moment: https://github.com/GeoUtils/georaster/blob/master/test/test_georaster.py
-https://github.com/corteva/rioxarray/blob/master/test/integration/test_integration__io.py
-
+See [mamba's documentation](https://mamba.readthedocs.io/en/latest/) to install `mamba`, which will solve your environment much faster than `conda`.
 
+## Citing methods implemented in the package
 
-### Examples
+When using a method implemented in xDEM, please **cite both the package and the related study**:
 
-**Coregister a DEM to another DEM**
-```python
-import xdem
+Citing xDEM: [![Zenodo](https://zenodo.org/badge/doi/10.5281/zenodo.4809697.svg)](https://zenodo.org/record/4809698)
 
-reference_dem = xdem.DEM("path/to/reference.tif")
-dem_to_be_aligned = xdem.DEM("path/to/dem.tif")
+Citing the related study:
 
-nuth_kaab = xdem.coreg.NuthKaab()
+- **Coregistration**:
+  - Horizontal shift from aspect/slope relationship of *[Nuth and Kääb (2011)](https://doi.org/10.5194/tc-5-271-2011)*,
+  - Iterative closest point (ICP) of *[Besl and McKay (1992)](http://dx.doi.org/10.1109/34.121791)*,
+- **Bias correction**:
+  - Along-track multi-sinusoidal noise by basin-hopping of *[Girod et al. (2017)](https://doi.org/10.3390/rs9070704)*,
+- **Uncertainty analysis**:
+  - Heteroscedasticity and multi-range correlations from stable terrain of *[Hugonnet et al. (2022)](https://doi.org/10.1109/JSTARS.2022.3188922)*,
+- **Terrain attributes**:
+  - Slope, aspect and hillshade of either *[Horn (1981)](http://dx.doi.org/10.1109/PROC.1981.11918)* or *[Zevenbergen and Thorne (1987)](http://dx.doi.org/10.1002/esp.3290120107)*,
+  - Profile, plan and maximum curvature of *[Zevenbergen and Thorne (1987)](http://dx.doi.org/10.1002/esp.3290120107)*,
+  - Topographic position index of *[Weiss (2001)](http://www.jennessent.com/downloads/TPI-poster-TNC_18x22.pdf)*,
+  - Terrain ruggedness index of either *[Riley et al. (1999)](http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf)* or *[Wilson et al. (2007)](http://dx.doi.org/10.1080/01490410701295962)*,
+  - Roughness of *[Dartnell (2000)](http://dx.doi.org/10.14358/PERS.70.9.1081)*,
+  - Rugosity of *[Jenness (2004)](https://doi.org/10.2193/0091-7648(2004)032[0829:CLSAFD]2.0.CO;2)*,
+  - Fractal roughness of *[Taud et Parrot (2005)](https://doi.org/10.4000/geomorphologie.622)*.
 
-nuth_kaab.fit(reference_dem.data, dem_to_be_aligned.data, transform=reference_dem.transform)
+## Start contributing
 
+1. Fork the repository, make a feature branch and push changes.
+2. When ready, submit a pull request from the feature branch of your fork to `GlacioHack/geoutils:main`.
+3. The PR will be reviewed by at least one maintainer, discussed, then merged.
 
-aligned_dem = xdem.DEM.from_array(
-	nuth_kaab.apply(dem_to_be_aligned.data, transform=dem_to_be_aligned.transform),
-	transform=dem_to_be_aligned.transform,
-	crs=dem_to_be_aligned.crs
-)
-
-aligned_dem.save("path/to/coreg.tif")
-```
-This is an implementation of the [Nuth and Kääb (2011)](https://doi.org/10.5194/tc-5-271-2011) approach.
-[Please see the documentation](https://xdem.readthedocs.io/en/latest/coregistration.html) for more approaches.
-
-**Subtract one DEM with another**
-```python
-import xdem
-
-first_dem = xdem.DEM("path/to/first.tif")
-second_dem = xdem.DEM("path/to/second.tif")
-
-difference = first_dem - second_dem
-
-difference.save("path/to/difference.tif")
-```
-By default, `second_dem` is reprojected to fit `first_dem`.
-This can be switched with the keyword argument `reference="second"`.
-The resampling method can also be changed (e.g. `resampling_method="nearest"`) from the default `"cubic_spline"`.
-
+More info on [our contributing page](CONTRIBUTING.md).
```

### Comparing `xdem-0.0.7/setup.py` & `xdem-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from __future__ import annotations
+
 import os
-import subprocess
-import sys
 
 from setuptools import setup
-from setuptools.command.install import install
 
-FULLVERSION = "0.0.7"
+FULLVERSION = "0.0.8"
 VERSION = FULLVERSION
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as infile:
     LONG_DESCRIPTION = infile.read()
 
 setup(
     name="xdem",
@@ -43,15 +42,15 @@
     scripts=[],
     zip_safe=False,
 )
 
 write_version = True
 
 
-def write_version_py(filename=None):
+def write_version_py(filename: str | None = None) -> None:
     cnt = """\
 version = '%s'
 short_version = '%s'
 """
     if not filename:
         filename = os.path.join(os.path.dirname(__file__), "xdem", "version.py")
```

### Comparing `xdem-0.0.7/xdem/coreg.py` & `xdem-0.0.8/xdem/coreg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,86 @@
 """DEM coregistration classes and functions."""
 from __future__ import annotations
 
-import copy
 import concurrent.futures
-import json
-import os
-import subprocess
-import tempfile
+import copy
 import warnings
-from enum import Enum
-from typing import Any, Callable, Optional, overload, Union, Sequence, TypeVar
+from typing import Any, Callable, Generator, TypedDict, TypeVar, overload
 
 try:
     import cv2
+
     _has_cv2 = True
 except ImportError:
     _has_cv2 = False
 import fiona
 import geoutils as gu
-from geoutils.georaster import RasterType
-from geoutils import spatial_tools
+import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import rasterio as rio
 import rasterio.warp  # pylint: disable=unused-import
 import rasterio.windows  # pylint: disable=unused-import
 import scipy
 import scipy.interpolate
 import scipy.ndimage
 import scipy.optimize
 import skimage.transform
+from geoutils._typing import AnyNumber
+from geoutils.raster import (
+    Mask,
+    RasterType,
+    get_array_and_mask,
+    raster,
+    subdivide_array,
+    subsample_array,
+)
 from rasterio import Affine
-from tqdm import trange, tqdm
-import pandas as pd
+from tqdm import tqdm, trange
 
 import xdem
+from xdem._typing import MArrayf, NDArrayf
 
 try:
-    from pytransform3d.transform_manager import TransformManager
     import pytransform3d.transformations
+    from pytransform3d.transform_manager import TransformManager
+
     _HAS_P3D = True
 except ImportError:
     _HAS_P3D = False
 
 
-def filter_by_range(ds: rio.DatasetReader, rangelim: tuple[float, float]):
-    """
-    Function to filter values using a range.
+def _calculate_slope_and_aspect_nuthkaab(dem: NDArrayf) -> tuple[NDArrayf, NDArrayf]:
     """
-    print('Excluding values outside of range: {0:f} to {1:f}'.format(*rangelim))
-    out = np.ma.masked_outside(ds, *rangelim)
-    out.set_fill_value(ds.fill_value)
-    return out
-
-
-def filtered_slope(ds_slope, slope_lim=(0.1, 40)):
-    print("Slope filter: %0.2f - %0.2f" % slope_lim)
-    print("Initial count: %i" % ds_slope.count())
-    flt_slope = filter_by_range(ds_slope, slope_lim)
-    print(flt_slope.count())
-    return flt_slope
-
+    Calculate the tangent of slope and aspect of a DEM, in radians, as needed for the Nuth & Kaab algorithm.
 
-def apply_xy_shift(ds: rio.DatasetReader, dx: float, dy: float) -> np.ndarray:
-    """
-    Apply horizontal shift to rio dataset using Transform affine matrix
-    :param ds: DEM
-    :param dx: dx shift value
-    :param dy: dy shift value
+    :param dem: A numpy array of elevation values.
 
-    Returns:
-    Rio Dataset with updated transform
+    :returns:  The tangent of slope and aspect (in radians) of the DEM.
     """
-    print("X shift: ", dx)
-    print("Y shift: ", dy)
-
-    # Update geotransform
-    ds_meta = ds.meta
-    gt_orig = ds.transform
-    gt_align = Affine(gt_orig.a, gt_orig.b, gt_orig.c+dx,
-                      gt_orig.d, gt_orig.e, gt_orig.f+dy)
-
-    print("Original transform:", gt_orig)
-    print("Updated transform:", gt_align)
-
-    # Update ds Geotransform
-    ds_align = ds
-    meta_update = ds.meta.copy()
-    meta_update({"driver": "GTiff", "height": ds.shape[1],
-                 "width": ds.shape[2], "transform": gt_align, "crs": ds.crs})
-    # to split this part in two?
-    with rasterio.open(ds_align, "w", **meta_update) as dest:
-        dest.write(ds_align)
+    # Old implementation
+    # # Calculate the gradient of the slope
+    gradient_y, gradient_x = np.gradient(dem)
+    slope_tan = np.sqrt(gradient_x**2 + gradient_y**2)
+    aspect = np.arctan2(-gradient_x, gradient_y)
+    aspect += np.pi
 
-    return ds_align
+    # xdem implementation
+    # slope, aspect = xdem.terrain.get_terrain_attribute(
+    #     dem, attribute=["slope", "aspect"], resolution=1, degrees=False
+    # )
+    # slope_tan = np.tan(slope)
+    # aspect = (aspect + np.pi) % (2 * np.pi)
+
+    return slope_tan, aspect
 
 
-def apply_z_shift(ds: rio.DatasetReader, dz: float):
-    """
-    Apply vertical shift to rio dataset using Transform affine matrix
-    :param ds: DEM
-    :param dx: dz shift value
-    """
-    src_dem = rio.open(ds)
-    a = src_dem.read(1)
-    ds_shift = a + dz
-    return ds_shift
-
-
-def get_horizontal_shift(elevation_difference: np.ndarray, slope: np.ndarray, aspect: np.ndarray,
-                         min_count: int = 20) -> tuple[float, float, float]:
+def get_horizontal_shift(
+    elevation_difference: NDArrayf, slope: NDArrayf, aspect: NDArrayf, min_count: int = 20
+) -> tuple[float, float, float]:
     """
     Calculate the horizontal shift between two DEMs using the method presented in Nuth and Kääb (2011).
 
     :param elevation_difference: The elevation difference (reference_dem - aligned_dem).
     :param slope: A slope map with the same shape as elevation_difference (units = pixels?).
     :param aspect: An aspect map with the same shape as elevation_difference (units = radians).
     :param min_count: The minimum allowed bin size to consider valid.
@@ -154,30 +122,30 @@
     y_medians = y_medians[count > min_count]
     slice_bounds = slice_bounds[count > min_count]
 
     if slice_bounds.shape[0] < 10:
         raise ValueError("Less than 10 different cells exist.")
 
     # Make an initial guess of the a, b, and c parameters
-    initial_guess: tuple[float, float, float] = (3 * np.std(y_medians) / (2 ** 0.5), 0.0, np.mean(y_medians))
+    initial_guess: tuple[float, float, float] = (3 * np.std(y_medians) / (2**0.5), 0.0, np.mean(y_medians))
 
-    def estimate_ys(x_values: np.ndarray, parameters: tuple[float, float, float]) -> np.ndarray:
+    def estimate_ys(x_values: NDArrayf, parameters: tuple[float, float, float]) -> NDArrayf:
         """
         Estimate y-values from x-values and the current parameters.
 
         y(x) = a * cos(b - x) + c
 
         :param x_values: The x-values to feed the above function.
         :param parameters: The a, b, and c parameters to feed the above function
 
         :returns: Estimated y-values with the same shape as the given x-values
         """
         return parameters[0] * np.cos(parameters[1] - x_values) + parameters[2]
 
-    def residuals(parameters: tuple[float, float, float], y_values: np.ndarray, x_values: np.ndarray):
+    def residuals(parameters: tuple[float, float, float], y_values: NDArrayf, x_values: NDArrayf) -> NDArrayf:
         """
         Get the residuals between the estimated and measured values using the given parameters.
 
         err(x, y) = est_y(x) - y
 
         :param parameters: The a, b, and c parameters to use for the estimation.
         :param y_values: The measured y-values.
@@ -185,154 +153,183 @@
 
         :returns: An array of residuals with the same shape as the input arrays.
         """
         err = estimate_ys(x_values, parameters) - y_values
         return err
 
     # Estimate the a, b, and c parameters with least square minimisation
-    plsq = scipy.optimize.leastsq(func=residuals, x0=initial_guess, args=(y_medians, slice_bounds), full_output=1)
+    results = scipy.optimize.least_squares(
+        fun=residuals, x0=initial_guess, args=(y_medians, slice_bounds), xtol=1e-8, gtol=None, ftol=None
+    )
 
-    a_parameter, b_parameter, c_parameter = plsq[0]
+    # Round results above the tolerance to get fixed results on different OS
+    a_parameter, b_parameter, c_parameter = results.x
+    a_parameter = np.round(a_parameter, 2)
+    b_parameter = np.round(b_parameter, 2)
 
     # Calculate the easting and northing offsets from the above parameters
     east_offset = a_parameter * np.sin(b_parameter)
     north_offset = a_parameter * np.cos(b_parameter)
 
     return east_offset, north_offset, c_parameter
 
 
-def calculate_slope_and_aspect(dem: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+def apply_xy_shift(transform: rio.transform.Affine, dx: float, dy: float) -> rio.transform.Affine:
     """
-    Calculate the slope and aspect of a DEM.
-
-    :param dem: A numpy array of elevation values.
+    Apply horizontal shift to a rasterio Affine transform
+    :param transform: The Affine transform of the raster
+    :param dx: dx shift value
+    :param dy: dy shift value
 
-    :returns:  The slope (in pixels??) and aspect (in radians) of the DEM.
+    Returns: Updated transform
     """
-    # TODO: Figure out why slope is called slope_px. What unit is it in?
-    # TODO: Change accordingly in the get_horizontal_shift docstring.
-
-    # Calculate the gradient of the slope
-    gradient_y, gradient_x = np.gradient(dem)
-
-    slope_px = np.sqrt(gradient_x ** 2 + gradient_y ** 2)
-    aspect = np.arctan2(-gradient_x, gradient_y)
-    aspect += np.pi
+    transform_shifted = Affine(transform.a, transform.b, transform.c + dx, transform.d, transform.e, transform.f + dy)
+    return transform_shifted
 
-    return slope_px, aspect
 
-
-def deramping(elevation_difference, x_coordinates: np.ndarray, y_coordinates: np.ndarray,
-              degree: int, verbose: bool = False,
-              metadata: Optional[dict[str, Any]] = None) -> Callable[[np.ndarray, np.ndarray], np.ndarray]:
-    """
-    Calculate a deramping function to account for rotational and non-rigid components of the elevation difference.
-
-    :param elevation_difference: The elevation difference array to analyse.
-    :param x_coordinates: x-coordinates of the above array (must have the same shape as elevation_difference)
-    :param y_coordinates: y-coordinates of the above array (must have the same shape as elevation_difference)
+def calculate_ddem_stats(
+    ddem: NDArrayf | MArrayf,
+    inlier_mask: NDArrayf | None = None,
+    stats_list: tuple[Callable[[NDArrayf], AnyNumber], ...] | None = None,
+    stats_labels: tuple[str, ...] | None = None,
+) -> dict[str, float]:
+    """
+    Calculate standard statistics of ddem, e.g., to be used to compare before/after coregistration.
+    Default statistics are: count, mean, median, NMAD and std.
+
+    :param ddem: The DEM difference to be analyzed.
+    :param inlier_mask: 2D boolean array of areas to include in the analysis (inliers=True).
+    :param stats_list: Statistics to compute on the DEM difference.
+    :param stats_labels: Labels of the statistics to compute (same length as stats_list).
+
+    Returns: a dictionary containing the statistics
+    """
+    # Default stats - Cannot be put in default args due to circular import with xdem.spatialstats.nmad.
+    if (stats_list is None) or (stats_labels is None):
+        stats_list = (np.size, np.mean, np.median, xdem.spatialstats.nmad, np.std)
+        stats_labels = ("count", "mean", "median", "nmad", "std")
+
+    # Check that stats_list and stats_labels are correct
+    if len(stats_list) != len(stats_labels):
+        raise ValueError("Number of items in `stats_list` and `stats_labels` should be identical.")
+    for stat, label in zip(stats_list, stats_labels):
+        if not callable(stat):
+            raise ValueError(f"Item {stat} in `stats_list` should be a callable/function.")
+        if not isinstance(label, str):
+            raise ValueError(f"Item {label} in `stats_labels` should be a string.")
+
+    # Get the mask of valid and inliers pixels
+    nan_mask = ~np.isfinite(ddem)
+    if inlier_mask is None:
+        inlier_mask = np.ones(ddem.shape, dtype="bool")
+    valid_ddem = ddem[~nan_mask & inlier_mask]
+
+    # Calculate stats
+    stats = {}
+    for stat, label in zip(stats_list, stats_labels):
+        stats[label] = stat(valid_ddem)
+
+    return stats
+
+
+def deramping(
+    ddem: NDArrayf | MArrayf,
+    x_coords: NDArrayf,
+    y_coords: NDArrayf,
+    degree: int,
+    subsample: float | int = 1.0,
+    verbose: bool = False,
+) -> tuple[Callable[[NDArrayf, NDArrayf], NDArrayf], tuple[NDArrayf, int]]:
+    """
+    Calculate a deramping function to remove spatially correlated elevation differences that can be explained by \
+    a polynomial of degree `degree`.
+
+    :param ddem: The elevation difference array to analyse.
+    :param x_coords: x-coordinates of the above array (must have the same shape as elevation_difference)
+    :param y_coords: y-coordinates of the above array (must have the same shape as elevation_difference)
     :param degree: The polynomial degree to estimate the ramp.
+    :param subsample: Subsample the input to increase performance. <1 is parsed as a fraction. >1 is a pixel count.
     :param verbose: Print the least squares optimization progress.
-    :param metadata: Optional. A metadata dictionary that will be updated with the key "deramp".
 
-    :returns: A callable function to estimate the ramp.
+    :returns: A callable function to estimate the ramp and the output of scipy.optimize.leastsq
     """
-    #warnings.warn("This function is deprecated in favour of the new Coreg class.", DeprecationWarning)
-    # Extract only the finite values of the elevation difference and corresponding coordinates.
-    valid_diffs = elevation_difference[np.isfinite(elevation_difference)]
-    valid_x_coords = x_coordinates[np.isfinite(elevation_difference)]
-    valid_y_coords = y_coordinates[np.isfinite(elevation_difference)]
-
-    # Randomly subsample the values if there are more than 500,000 of them.
-    if valid_x_coords.shape[0] > 500_000:
-        random_indices = np.random.randint(0, valid_x_coords.shape[0] - 1, 500_000)
-        valid_diffs = valid_diffs[random_indices]
-        valid_x_coords = valid_x_coords[random_indices]
-        valid_y_coords = valid_y_coords[random_indices]
-
-    # Create a function whose residuals will be attempted to minimise
-    def estimate_values(x_coordinates: np.ndarray, y_coordinates: np.ndarray,
-                        coefficients: np.ndarray, degree: int) -> np.ndarray:
+    # Extract only valid pixels
+    valid_mask = np.isfinite(ddem)
+    ddem = ddem[valid_mask]
+    x_coords = x_coords[valid_mask]
+    y_coords = y_coords[valid_mask]
+
+    # Formulate the 2D polynomial whose coefficients will be solved for.
+    def poly2d(x_coords: NDArrayf, y_coords: NDArrayf, coefficients: NDArrayf) -> NDArrayf:
         """
         Estimate values from a 2D-polynomial.
 
-        :param x_coordinates: x-coordinates of the difference array (must have the same shape as elevation_difference).
-        :param y_coordinates: y-coordinates of the difference array (must have the same shape as elevation_difference).
+        :param x_coords: x-coordinates of the difference array (must have the same shape as
+            elevation_difference).
+        :param y_coords: y-coordinates of the difference array (must have the same shape as
+            elevation_difference).
         :param coefficients: The coefficients (a, b, c, etc.) of the polynomial.
         :param degree: The degree of the polynomial.
 
         :raises ValueError: If the length of the coefficients list is not compatible with the degree.
 
         :returns: The values estimated by the polynomial.
         """
         # Check that the coefficient size is correct.
         coefficient_size = (degree + 1) * (degree + 2) / 2
         if len(coefficients) != coefficient_size:
             raise ValueError()
 
-        # Do Amaury's black magic to estimate the values.
-        estimated_values = np.sum([coefficients[k * (k + 1) // 2 + j] * x_coordinates ** (k - j) *
-                                   y_coordinates ** j for k in range(degree + 1) for j in range(k + 1)], axis=0)
+        # Build the polynomial of degree `degree`
+        estimated_values = np.sum(
+            [
+                coefficients[k * (k + 1) // 2 + j] * x_coords ** (k - j) * y_coords**j
+                for k in range(degree + 1)
+                for j in range(k + 1)
+            ],
+            axis=0,
+        )
         return estimated_values  # type: ignore
 
-    # Creat the error function
-    def residuals(coefficients: np.ndarray, values: np.ndarray, x_coordinates: np.ndarray,
-                  y_coordinates: np.ndarray, degree: int) -> np.ndarray:
-        """
-        Calculate the difference between the estimated and measured values.
+    def residuals(coefs: NDArrayf, x_coords: NDArrayf, y_coords: NDArrayf, targets: NDArrayf) -> NDArrayf:
+        """Return the optimization residuals"""
+        res = targets - poly2d(x_coords, y_coords, coefs)
+        return res[np.isfinite(res)]
 
-        :param coefficients: Coefficients for the estimation.
-        :param values: The measured values.
-        :param x_coordinates: The x-coordinates of the values.
-        :param y_coordinates: The y-coordinates of the values.
-        :param degree: The degree of the polynomial to estimate.
-
-        :returns: An array of residuals.
-        """
-        error = estimate_values(x_coordinates, y_coordinates, coefficients, degree) - values
-        error = error[np.isfinite(error)]
-
-        return error
-
-    # Run a least-squares minimisation to estimate the correct coefficients.
-    # TODO: Maybe remove the full_output?
-    initial_guess = np.zeros(shape=((degree + 1) * (degree + 2) // 2))
     if verbose:
-        print("Deramping...")
-    coefficients = scipy.optimize.least_squares(
-        fun=residuals,
-        x0=initial_guess,
-        args=(valid_diffs, valid_x_coords, valid_y_coords, degree),
-        verbose=2 if verbose and degree > 1 else 0
-    ).x
+        print("Estimating deramp function...")
 
-    # Generate the return-function which can correctly estimate the ramp
+    # reduce number of elements for speed
+    rand_indices = subsample_array(x_coords, subsample=subsample, return_indices=True)
+    x_coords = x_coords[rand_indices]
+    y_coords = y_coords[rand_indices]
+    ddem = ddem[rand_indices]
+
+    # Optimize polynomial parameters
+    coefs = scipy.optimize.leastsq(
+        func=residuals,
+        x0=np.zeros(shape=((degree + 1) * (degree + 2) // 2)),
+        args=(x_coords, y_coords, ddem),
+    )
 
-    def ramp(x_coordinates: np.ndarray, y_coordinates: np.ndarray) -> np.ndarray:
+    def fit_ramp(x: NDArrayf, y: NDArrayf) -> NDArrayf:
         """
-        Get the values of the ramp that corresponds to given coordinates.
+        Get the elevation difference biases (ramp) at the given coordinates.
 
         :param x_coordinates: x-coordinates of interest.
         :param y_coordinates: y-coordinates of interest.
 
-        :returns: The estimated ramp offsets.
+        :returns: The estimated elevation difference bias.
         """
-        return estimate_values(x_coordinates, y_coordinates, coefficients, degree)
+        return poly2d(x, y, coefs[0])
 
-    if metadata is not None:
-        metadata["deramp"] = {
-            "coefficients": coefficients,
-            "nmad": xdem.spatialstats.nmad(residuals(coefficients, valid_diffs, valid_x_coords, valid_y_coords, degree))
-        }
-
-    # Return the function which can be used later.
-    return ramp
+    return fit_ramp, coefs
 
 
-def mask_as_array(reference_raster: gu.georaster.Raster, mask: Union[str, gu.geovector.Vector, gu.georaster.Raster]) -> np.ndarray:
+def mask_as_array(reference_raster: gu.Raster, mask: str | gu.Vector | gu.Raster) -> NDArrayf:
     """
     Convert a given mask into an array.
 
     :param reference_raster: The raster to use for rasterizing the mask if the mask is a vector.
     :param mask: A valid Vector, Raster or a respective filepath to a mask.
 
     :raises: ValueError: If the mask path is invalid.
@@ -340,143 +337,182 @@
 
     :returns: The mask as a squeezed array.
     """
     # Try to load the mask file if it's a filepath
     if isinstance(mask, str):
         # First try to load it as a Vector
         try:
-            mask = gu.geovector.Vector(mask)
+            mask = gu.Vector(mask)
         # If the format is unsopported, try loading as a Raster
         except fiona.errors.DriverError:
             try:
-                mask = gu.georaster.Raster(mask)
+                mask = gu.Raster(mask)
             # If that fails, raise an error
             except rio.errors.RasterioIOError:
                 raise ValueError(f"Mask path not in a supported Raster or Vector format: {mask}")
 
     # At this point, the mask variable is either a Raster or a Vector
     # Now, convert the mask into an array by either rasterizing a Vector or by fetching a Raster's data
-    if isinstance(mask, gu.geovector.Vector):
-        mask_array = mask.create_mask(reference_raster)
-    elif isinstance(mask, gu.georaster.Raster):
+    if isinstance(mask, gu.Vector):
+        mask_array = mask.create_mask(reference_raster, as_array=True)
+    elif isinstance(mask, gu.Raster):
         # The true value is the maximum value in the raster, unless the maximum value is 0 or False
         true_value = np.nanmax(mask.data) if not np.nanmax(mask.data) in [0, False] else True
         mask_array = (mask.data == true_value).squeeze()
     else:
         raise TypeError(
-            f"Mask has invalid type: {type(mask)}. Expected one of: "
-            f"{[gu.georaster.Raster, gu.geovector.Vector, str, type(None)]}"
+            f"Mask has invalid type: {type(mask)}. Expected one of: " f"{[gu.Raster, gu.Vector, str, type(None)]}"
         )
 
     return mask_array
 
 
-def _transform_to_bounds_and_res(shape: tuple[int, ...],
-                                 transform: rio.transform.Affine) -> tuple[rio.coords.BoundingBox, float]:
+def _transform_to_bounds_and_res(
+    shape: tuple[int, ...], transform: rio.transform.Affine
+) -> tuple[rio.coords.BoundingBox, float]:
     """Get the bounding box and (horizontal) resolution from a transform and the shape of a DEM."""
-    bounds = rio.coords.BoundingBox(
-        *rio.transform.array_bounds(shape[0], shape[1], transform=transform))
+    bounds = rio.coords.BoundingBox(*rio.transform.array_bounds(shape[0], shape[1], transform=transform))
     resolution = (bounds.right - bounds.left) / shape[1]
 
     return bounds, resolution
 
 
-def _get_x_and_y_coords(shape: tuple[int, ...], transform: rio.transform.Affine):
+def _get_x_and_y_coords(shape: tuple[int, ...], transform: rio.transform.Affine) -> tuple[NDArrayf, NDArrayf]:
     """Generate center coordinates from a transform and the shape of a DEM."""
     bounds, resolution = _transform_to_bounds_and_res(shape, transform)
     x_coords, y_coords = np.meshgrid(
         np.linspace(bounds.left + resolution / 2, bounds.right - resolution / 2, num=shape[1]),
-        np.linspace(bounds.bottom + resolution / 2, bounds.top - resolution / 2, num=shape[0])[::-1]
+        np.linspace(bounds.bottom + resolution / 2, bounds.top - resolution / 2, num=shape[0])[::-1],
     )
     return x_coords, y_coords
 
 
 CoregType = TypeVar("CoregType", bound="Coreg")
 
+
+class CoregDict(TypedDict, total=False):
+    """
+    Defining the type of each possible key in the metadata dictionary of Coreg classes.
+    The parameter total=False means that the key are not required. In the recent PEP 655 (
+    https://peps.python.org/pep-0655/) there is an easy way to specific Required or NotRequired for each key, if we
+    want to change this in the future.
+    """
+
+    bias_func: Callable[[NDArrayf], np.floating[Any]]
+    func: Callable[[NDArrayf, NDArrayf], NDArrayf]
+    bias: np.floating[Any] | float | np.integer[Any] | int
+    matrix: NDArrayf
+    centroid: tuple[float, float, float]
+    offset_east_px: float
+    offset_north_px: float
+    coefficients: NDArrayf
+    coreg_meta: list[Any]
+    resolution: float
+    # The pipeline metadata can have any value of the above
+    pipeline: list[Any]
+
+
 class Coreg:
     """
     Generic Coreg class.
 
     Made to be subclassed.
     """
 
     _fit_called: bool = False  # Flag to check if the .fit() method has been called.
-    _is_affine: Optional[bool] = None
+    _is_affine: bool | None = None
 
-    def __init__(self, meta: Optional[dict[str, Any]] = None, matrix: Optional[np.ndarray] = None):
+    def __init__(self, meta: CoregDict | None = None, matrix: NDArrayf | None = None) -> None:
         """Instantiate a generic Coreg method."""
-        self._meta: dict[str, Any] = meta or {}  # All __init__ functions should instantiate an empty dict.
+        self._meta: CoregDict = meta or {}  # All __init__ functions should instantiate an empty dict.
 
         if matrix is not None:
             with warnings.catch_warnings():
                 # This error is fixed in the upcoming 1.8
                 warnings.filterwarnings("ignore", message="`np.float` is a deprecated alias for the builtin `float`")
                 valid_matrix = pytransform3d.transformations.check_transform(matrix)
             self._meta["matrix"] = valid_matrix
 
-    def fit(self: CoregType, reference_dem: np.ndarray | np.ma.masked_array | RasterType,
-            dem_to_be_aligned: np.ndarray | np.ma.masked_array | RasterType,
-            inlier_mask: Optional[np.ndarray] = None,
-            transform: Optional[rio.transform.Affine] = None,
-            weights: Optional[np.ndarray] = None,
-            subsample: Union[float, int] = 1.0,
-            verbose: bool = False) -> CoregType:
+    def fit(
+        self: CoregType,
+        reference_dem: NDArrayf | MArrayf | RasterType,
+        dem_to_be_aligned: NDArrayf | MArrayf | RasterType,
+        inlier_mask: NDArrayf | Mask | None = None,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+        weights: NDArrayf | None = None,
+        subsample: float | int = 1.0,
+        verbose: bool = False,
+        random_state: None | np.random.RandomState | np.random.Generator | int = None,
+    ) -> CoregType:
         """
         Estimate the coregistration transform on the given DEMs.
 
-        :param reference_dem: 2D array of elevation values acting reference. 
+        :param reference_dem: 2D array of elevation values acting reference.
         :param dem_to_be_aligned: 2D array of elevation values to be aligned.
         :param inlier_mask: Optional. 2D boolean array of areas to include in the analysis (inliers=True).
-        :param transform: Optional. Transform of the reference_dem. Mandatory in some cases.
+        :param transform: Optional. Transform of the reference_dem. Mandatory if DEM provided as array.
+        :param crs: Optional. CRS of the reference_dem. Mandatory if DEM provided as array.
         :param weights: Optional. Per-pixel weights for the coregistration.
         :param subsample: Subsample the input to increase performance. <1 is parsed as a fraction. >1 is a pixel count.
         :param verbose: Print progress messages to stdout.
+        :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
         """
 
         if weights is not None:
             raise NotImplementedError("Weights have not yet been implemented")
 
         # Validate that both inputs are valid array-like (or Raster) types.
-        if not all(hasattr(dem, "__array_interface__") for dem in (reference_dem, dem_to_be_aligned)):
+        if not all(isinstance(dem, (np.ndarray, gu.Raster)) for dem in (reference_dem, dem_to_be_aligned)):
             raise ValueError(
                 "Both DEMs need to be array-like (implement a numpy array interface)."
                 f"'reference_dem': {reference_dem}, 'dem_to_be_aligned': {dem_to_be_aligned}"
             )
 
         # If both DEMs are Rasters, validate that 'dem_to_be_aligned' is in the right grid. Then extract its data.
         if isinstance(dem_to_be_aligned, gu.Raster) and isinstance(reference_dem, gu.Raster):
             dem_to_be_aligned = dem_to_be_aligned.reproject(reference_dem, silent=True).data
 
         # If any input is a Raster, use its transform if 'transform is None'.
         # If 'transform' was given and any input is a Raster, trigger a warning.
         # Finally, extract only the data of the raster.
         for name, dem in [("reference_dem", reference_dem), ("dem_to_be_aligned", dem_to_be_aligned)]:
-            if hasattr(dem, "transform"):
+            if isinstance(dem, gu.Raster):
                 if transform is None:
-                    transform = getattr(dem, "transform")
+                    transform = dem.transform
                 elif transform is not None:
                     warnings.warn(f"'{name}' of type {type(dem)} overrides the given 'transform'")
+                if crs is None:
+                    crs = dem.crs
+                elif crs is not None:
+                    warnings.warn(f"'{name}' of type {type(dem)} overrides the given 'crs'")
 
                 """
                 if name == "reference_dem":
                     reference_dem = dem.data
                 else:
                     dem_to_be_aligned = dem.data
                 """
 
         if transform is None:
             raise ValueError("'transform' must be given if both DEMs are array-like.")
 
-        ref_dem, ref_mask = spatial_tools.get_array_and_mask(reference_dem)
-        tba_dem, tba_mask = spatial_tools.get_array_and_mask(dem_to_be_aligned)
+        if crs is None:
+            raise ValueError("'crs' must be given if both DEMs are array-like.")
+
+        ref_dem, ref_mask = get_array_and_mask(reference_dem)
+        tba_dem, tba_mask = get_array_and_mask(dem_to_be_aligned)
 
         # Make sure that the mask has an expected format.
         if inlier_mask is not None:
-            inlier_mask = np.asarray(inlier_mask).squeeze()
-            assert inlier_mask.dtype == bool, f"Invalid mask dtype: '{inlier_mask.dtype}'. Expected 'bool'"
+            if isinstance(inlier_mask, Mask):
+                inlier_mask = inlier_mask.data.filled(False).squeeze()
+            else:
+                inlier_mask = np.asarray(inlier_mask).squeeze()
+                assert inlier_mask.dtype == bool, f"Invalid mask dtype: '{inlier_mask.dtype}'. Expected 'bool'"
 
             if np.all(~inlier_mask):
                 raise ValueError("'inlier_mask' had no inliers.")
 
             ref_dem[~inlier_mask] = np.nan
             tba_dem[~inlier_mask] = np.nan
 
@@ -484,134 +520,200 @@
             raise ValueError("'reference_dem' had only NaNs")
         if np.all(tba_mask):
             raise ValueError("'dem_to_be_aligned' had only NaNs")
 
         # If subsample is not equal to one, subsampling should be performed.
         if subsample != 1.0:
             # The full mask (inliers=True) is the inverse of the above masks and the provided mask.
-            full_mask = (~ref_mask & ~tba_mask & (np.asarray(inlier_mask) if inlier_mask is not None else True)).squeeze()
-            # If subsample is less than one, it is parsed as a fraction (e.g. 0.8 => retain 80% of the values)
-            if subsample < 1.0:
-                subsample = int(np.count_nonzero(full_mask) * (1 - subsample))
-
-            # Randomly pick N inliers in the full_mask where N=subsample
-            random_falses = np.random.choice(np.argwhere(full_mask.flatten()).squeeze(), int(subsample), replace=False)
-            # Convert the 1D indices to 2D indices
-            cols = (random_falses // full_mask.shape[0]).astype(int)
-            rows = random_falses % full_mask.shape[0]
-            # Set the N random inliers to be parsed as outliers instead.
-            full_mask[rows, cols] = False
-
+            full_mask = (
+                ~ref_mask & ~tba_mask & (np.asarray(inlier_mask) if inlier_mask is not None else True)
+            ).squeeze()
+            random_indices = subsample_array(full_mask, subsample=subsample, return_indices=True)
+            full_mask[random_indices] = False
 
         # Run the associated fitting function
-        self._fit_func(ref_dem=ref_dem, tba_dem=tba_dem, transform=transform, weights=weights, verbose=verbose)
+        self._fit_func(ref_dem=ref_dem, tba_dem=tba_dem, transform=transform, crs=crs, weights=weights, verbose=verbose)
 
         # Flag that the fitting function has been called.
         self._fit_called = True
 
         return self
 
     @overload
-    def apply(self, dem: RasterType, transform: rio.transform.Affine | None, **kwargs) -> RasterType: ...
+    def apply(
+        self,
+        dem: MArrayf,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+        resample: bool = True,
+        **kwargs: Any,
+    ) -> tuple[MArrayf, rio.transform.Affine]:
+        ...
 
     @overload
-    def apply(self, dem: np.ndarray, transform: rio.transform.Affine | None, **kwargs) -> np.ndarray: ...
+    def apply(
+        self,
+        dem: NDArrayf,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+        resample: bool = True,
+        **kwargs: Any,
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
+        ...
 
     @overload
-    def apply(self, dem: np.ma.masked_array, transform: rio.transform.Affine | None, **kwargs) -> np.ma.masked_array: ...
-
-
-    def apply(self, dem: np.ndarray | np.ma.masked_array | RasterType,
-              transform: rio.transform.Affine | None = None, **kwargs) -> RasterType | np.ndarray | np.ma.masked_array:
+    def apply(
+        self,
+        dem: RasterType,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+        resample: bool = True,
+        **kwargs: Any,
+    ) -> RasterType:
+        ...
+
+    def apply(
+        self,
+        dem: RasterType | NDArrayf | MArrayf,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+        resample: bool = True,
+        **kwargs: Any,
+    ) -> RasterType | tuple[NDArrayf, rio.transform.Affine] | tuple[MArrayf, rio.transform.Affine]:
         """
         Apply the estimated transform to a DEM.
 
         :param dem: A DEM array or Raster to apply the transform on.
-        :param transform: The transform object of the DEM. Required if 'dem' is an array and not a Raster.
+        :param transform: Optional. The transform object of the DEM. Mandatory if 'dem' provided as array.
+        :param crs: Optional. CRS of the reference_dem. Mandatory if 'dem' provided as array.
+        :param resample: If set to True, will reproject output Raster on the same grid as input. Otherwise, \
+        only the transform might be updated and no resampling is done.
         :param kwargs: Any optional arguments to be passed to either self._apply_func or apply_matrix.
+        Kwarg `resampling` can be set to any rio.warp.Resampling to use a different resampling in case \
+        `resample` is True, default is bilinear.
 
         :returns: The transformed DEM.
         """
         if not self._fit_called and self._meta.get("matrix") is None:
             raise AssertionError(".fit() does not seem to have been called yet")
 
         if isinstance(dem, gu.Raster):
             if transform is None:
                 transform = dem.transform
             else:
                 warnings.warn(f"DEM of type {type(dem)} overrides the given 'transform'")
+            if crs is None:
+                crs = dem.crs
+            else:
+                warnings.warn(f"DEM of type {type(dem)} overrides the given 'crs'")
+
         else:
             if transform is None:
                 raise ValueError("'transform' must be given if DEM is array-like.")
+            if crs is None:
+                raise ValueError("'crs' must be given if DEM is array-like.")
 
         # The array to provide the functions will be an ndarray with NaNs for masked out areas.
-        dem_array, dem_mask = spatial_tools.get_array_and_mask(dem)
+        dem_array, dem_mask = get_array_and_mask(dem)
 
         if np.all(dem_mask):
             raise ValueError("'dem' had only NaNs")
 
         # See if a _apply_func exists
         try:
+            # arg `resample` must be passed to _apply_func, otherwise will be overwritten in CoregPipeline
+            kwargs["resample"] = resample
+
             # Run the associated apply function
-            applied_dem = self._apply_func(dem_array, transform, **kwargs)  # pylint: disable=assignment-from-no-return
+            applied_dem, out_transform = self._apply_func(
+                dem_array, transform, crs, **kwargs
+            )  # pylint: disable=assignment-from-no-return
+
         # If it doesn't exist, use apply_matrix()
         except NotImplementedError:
+
+            # In this case, resampling is necessary
+            if not resample:
+                raise NotImplementedError(f"Option `resample=False` not implemented for coreg method {self.__class__}")
+            kwargs.pop("resample")  # Need to removed before passing to apply_matrix
+
             if self.is_affine:  # This only works on it's affine, however.
-                # If dilate_mask is not specified, set it to True by default
-                if "dilate_mask" in kwargs.keys():
-                    dilate_mask = kwargs["dilate_mask"]
-                    kwargs.pop("dilate_mask")
-                else:
-                    dilate_mask = True
 
                 # Apply the matrix around the centroid (if defined, otherwise just from the center).
                 applied_dem = apply_matrix(
                     dem_array,
                     transform=transform,
                     matrix=self.to_matrix(),
                     centroid=self._meta.get("centroid"),
-                    dilate_mask=dilate_mask,
-                    **kwargs
+                    **kwargs,
                 )
+                out_transform = transform
             else:
                 raise ValueError("Coreg method is non-rigid but has no implemented _apply_func")
 
+        # Ensure the dtype is OK
+        applied_dem = applied_dem.astype("float32")
+
+        # Set default dst_nodata
+        if isinstance(dem, gu.Raster):
+            dst_nodata = dem.nodata
+        else:
+            dst_nodata = raster._default_nodata(applied_dem.dtype)
+
+        # Resample the array on the original grid
+        if resample:
+            # Set default resampling method if not specified in kwargs
+            resampling = kwargs.get("resampling", rio.warp.Resampling.bilinear)
+            if not isinstance(resampling, rio.warp.Resampling):
+                raise ValueError("`resampling` must be a rio.warp.Resampling algorithm")
+
+            applied_dem, out_transform = rio.warp.reproject(
+                applied_dem,
+                destination=applied_dem,
+                src_transform=out_transform,
+                dst_transform=transform,
+                src_crs=crs,
+                dst_crs=crs,
+                resampling=resampling,
+                dst_nodata=dst_nodata,
+            )
+
         # Calculate final mask
-        final_mask = dem_mask + np.isnan(applied_dem)
+        final_mask = np.logical_or(~np.isfinite(applied_dem), applied_dem == dst_nodata)
 
         # If the DEM was a masked_array, copy the mask to the new DEM
-        if hasattr(dem, "mask"):
-            applied_dem = np.ma.masked_array(applied_dem, mask=final_mask)  # type: ignore
-        # If the DEM was a Raster with a mask, copy the mask to the new DEM
-        elif hasattr(dem, "data") and hasattr(dem.data, "mask"):
+        if isinstance(dem, (np.ma.masked_array, gu.Raster)):
             applied_dem = np.ma.masked_array(applied_dem, mask=final_mask)  # type: ignore
         else:
             applied_dem[final_mask] = np.nan
 
-        # If the input was a Raster, return a Raster as well.
+        # If the input was a Raster, returns a Raster, else returns array and transform
         if isinstance(dem, gu.Raster):
-            return dem.from_array(applied_dem, transform, dem.crs, nodata=dem.nodata)
-
-        return applied_dem
+            out_dem = dem.from_array(applied_dem, out_transform, crs, nodata=dem.nodata)
+            return out_dem
+        else:
+            return applied_dem, out_transform
 
-    def apply_pts(self, coords: np.ndarray) -> np.ndarray:
+    def apply_pts(self, coords: NDArrayf) -> NDArrayf:
         """
         Apply the estimated transform to a set of 3D points.
 
         :param coords: A (N, 3) array of X/Y/Z coordinates or one coordinate of shape (3,).
 
         :returns: The transformed coordinates.
         """
         if not self._fit_called and self._meta.get("matrix") is None:
             raise AssertionError(".fit() does not seem to have been called yet")
         # If the coordinates represent just one coordinate
         if np.shape(coords) == (3,):
             coords = np.reshape(coords, (1, 3))
 
-        assert len(np.shape(coords)) == 2 and np.shape(coords)[1] == 3, f"'coords' shape must be (N, 3). Given shape: {np.shape(coords)}"
+        assert (
+            len(np.shape(coords)) == 2 and np.shape(coords)[1] == 3
+        ), f"'coords' shape must be (N, 3). Given shape: {np.shape(coords)}"
 
         coords_c = coords.copy()
 
         # See if an _apply_pts_func exists
         try:
             transformed_points = self._apply_pts_func(coords)
         # If it doesn't exist, use opencv's perspectiveTransform
@@ -639,47 +741,52 @@
                 self.to_matrix()
                 self._is_affine = True
             except (ValueError, NotImplementedError):
                 self._is_affine = False
 
         return self._is_affine
 
-    def to_matrix(self) -> np.ndarray:
+    def to_matrix(self) -> NDArrayf:
         """Convert the transform to a 4x4 transformation matrix."""
         return self._to_matrix_func()
 
-    def centroid(self) -> Optional[tuple[float, float, float]]:
+    def centroid(self) -> tuple[float, float, float] | None:
         """Get the centroid of the coregistration, if defined."""
         meta_centroid = self._meta.get("centroid")
 
         if meta_centroid is None:
             return None
 
         # Unpack the centroid in case it is in an unexpected format (an array, list or something else).
-        return (meta_centroid[0], meta_centroid[1], meta_centroid[2])
+        return meta_centroid[0], meta_centroid[1], meta_centroid[2]
 
-    def residuals(self, reference_dem: Union[np.ndarray, np.ma.masked_array],
-                  dem_to_be_aligned: Union[np.ndarray, np.ma.masked_array],
-                  inlier_mask: Optional[np.ndarray] = None,
-                  transform: Optional[rio.transform.Affine] = None) -> np.ndarray:
+    def residuals(
+        self,
+        reference_dem: NDArrayf,
+        dem_to_be_aligned: NDArrayf,
+        inlier_mask: NDArrayf | None = None,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+    ) -> NDArrayf:
         """
         Calculate the residual offsets (the difference) between two DEMs after applying the transformation.
 
-        :param reference_dem: 2D array of elevation values acting reference. 
+        :param reference_dem: 2D array of elevation values acting reference.
         :param dem_to_be_aligned: 2D array of elevation values to be aligned.
         :param inlier_mask: Optional. 2D boolean array of areas to include in the analysis (inliers=True).
         :param transform: Optional. Transform of the reference_dem. Mandatory in some cases.
+        :param crs: Optional. CRS of the reference_dem. Mandatory in some cases.
 
         :returns: A 1D array of finite residuals.
         """
         # Use the transform to correct the DEM to be aligned.
-        aligned_dem = self.apply(dem_to_be_aligned, transform=transform)
+        aligned_dem, _ = self.apply(dem_to_be_aligned, transform=transform, crs=crs)
 
         # Format the reference DEM
-        ref_arr, ref_mask = spatial_tools.get_array_and_mask(reference_dem)
+        ref_arr, ref_mask = get_array_and_mask(reference_dem)
 
         if inlier_mask is None:
             inlier_mask = np.ones(ref_arr.shape, dtype=bool)
 
         # Create the full inlier mask (manual inliers plus non-nans)
         full_mask = (~ref_mask) & np.isfinite(aligned_dem) & inlier_mask
 
@@ -689,67 +796,110 @@
         # Sometimes, the float minimum (for float32 = -3.4028235e+38) is returned. This and inf should be excluded.
         if "float" in str(diff.dtype):
             full_mask[(diff == np.finfo(diff.dtype).min) | np.isinf(diff)] = False
 
         # Return the difference values within the full inlier mask
         return diff[full_mask]
 
-    def error(self, reference_dem: Union[np.ndarray, np.ma.masked_array],
-              dem_to_be_aligned: Union[np.ndarray, np.ma.masked_array],
-              error_type: str | list[str] = "nmad",
-              inlier_mask: Optional[np.ndarray] = None,
-              transform: Optional[rio.transform.Affine] = None) -> float | list[float]:
+    @overload
+    def error(
+        self,
+        reference_dem: NDArrayf,
+        dem_to_be_aligned: NDArrayf,
+        error_type: list[str],
+        inlier_mask: NDArrayf | None = None,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+    ) -> list[np.floating[Any] | float | np.integer[Any] | int]:
+        ...
+
+    @overload
+    def error(
+        self,
+        reference_dem: NDArrayf,
+        dem_to_be_aligned: NDArrayf,
+        error_type: str = "nmad",
+        inlier_mask: NDArrayf | None = None,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+    ) -> np.floating[Any] | float | np.integer[Any] | int:
+        ...
+
+    def error(
+        self,
+        reference_dem: NDArrayf,
+        dem_to_be_aligned: NDArrayf,
+        error_type: str | list[str] = "nmad",
+        inlier_mask: NDArrayf | None = None,
+        transform: rio.transform.Affine | None = None,
+        crs: rio.crs.CRS | None = None,
+    ) -> np.floating[Any] | float | np.integer[Any] | int | list[np.floating[Any] | float | np.integer[Any] | int]:
         """
         Calculate the error of a coregistration approach.
 
         Choices:
             - "nmad": Default. The Normalized Median Absolute Deviation of the residuals.
             - "median": The median of the residuals.
             - "mean": The mean/average of the residuals
             - "std": The standard deviation of the residuals.
             - "rms": The root mean square of the residuals.
             - "mae": The mean absolute error of the residuals.
             - "count": The residual count.
 
-        :param reference_dem: 2D array of elevation values acting reference. 
+        :param reference_dem: 2D array of elevation values acting reference.
         :param dem_to_be_aligned: 2D array of elevation values to be aligned.
-        :param error_type: The type of error meaure to calculate. May be a list of error types.
+        :param error_type: The type of error measure to calculate. May be a list of error types.
         :param inlier_mask: Optional. 2D boolean array of areas to include in the analysis (inliers=True).
         :param transform: Optional. Transform of the reference_dem. Mandatory in some cases.
+        :param crs: Optional. CRS of the reference_dem. Mandatory in some cases.
 
         :returns: The error measure of choice for the residuals.
         """
         if isinstance(error_type, str):
             error_type = [error_type]
 
-        residuals = self.residuals(reference_dem=reference_dem, dem_to_be_aligned=dem_to_be_aligned,
-                                   inlier_mask=inlier_mask, transform=transform)
+        residuals = self.residuals(
+            reference_dem=reference_dem,
+            dem_to_be_aligned=dem_to_be_aligned,
+            inlier_mask=inlier_mask,
+            transform=transform,
+            crs=crs,
+        )
+
+        def rms(res: NDArrayf) -> np.floating[Any]:
+            return np.sqrt(np.mean(np.square(res)))
+
+        def mae(res: NDArrayf) -> np.floating[Any]:
+            return np.mean(np.abs(res))
+
+        def count(res: NDArrayf) -> int:
+            return res.size
 
-        error_functions = {
+        error_functions: dict[str, Callable[[NDArrayf], np.floating[Any] | float | np.integer[Any] | int]] = {
             "nmad": xdem.spatialstats.nmad,
             "median": np.median,
             "mean": np.mean,
             "std": np.std,
-            "rms": lambda residuals: np.sqrt(np.mean(np.square(residuals))),
-            "mae": lambda residuals: np.mean(np.abs(residuals)),
-            "count": lambda residuals: residuals.size
+            "rms": rms,
+            "mae": mae,
+            "count": count,
         }
 
         try:
             errors = [error_functions[err_type](residuals) for err_type in error_type]
         except KeyError as exception:
             raise ValueError(
-                    f"Invalid 'error_type'{'s' if len(error_type) > 1 else ''}: "
-                    f"'{error_type}'. Choices: {list(error_functions.keys())}"
-                    ) from exception
+                f"Invalid 'error_type'{'s' if len(error_type) > 1 else ''}: "
+                f"'{error_type}'. Choices: {list(error_functions.keys())}"
+            ) from exception
 
         return errors if len(errors) > 1 else errors[0]
 
     @classmethod
-    def from_matrix(cls, matrix: np.ndarray):
+    def from_matrix(cls, matrix: NDArrayf) -> Coreg:
         """
         Instantiate a generic Coreg class from a transformation matrix.
 
         :param matrix: A 4x4 transformation matrix. Shape must be (4,4).
 
         :raises ValueError: If the matrix is incorrectly formatted.
 
@@ -760,15 +910,15 @@
         with warnings.catch_warnings():
             # This error is fixed in the upcoming 1.8
             warnings.filterwarnings("ignore", message="`np.float` is a deprecated alias for the builtin `float`")
             valid_matrix = pytransform3d.transformations.check_transform(matrix)
         return cls(matrix=valid_matrix)
 
     @classmethod
-    def from_translation(cls, x_off: float = 0.0, y_off: float = 0.0, z_off: float = 0.0):
+    def from_translation(cls, x_off: float = 0.0, y_off: float = 0.0, z_off: float = 0.0) -> Coreg:
         """
         Instantiate a generic Coreg class from a X/Y/Z translation.
 
         :param x_off: The offset to apply in the X (west-east) direction.
         :param y_off: The offset to apply in the Y (south-north) direction.
         :param z_off: The offset to apply in the Z (vertical) direction.
 
@@ -793,75 +943,109 @@
 
     def __add__(self, other: Coreg) -> CoregPipeline:
         """Return a pipeline consisting of self and the other coreg function."""
         if not isinstance(other, Coreg):
             raise ValueError(f"Incompatible add type: {type(other)}. Expected 'Coreg' subclass")
         return CoregPipeline([self, other])
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         # FOR DEVELOPERS: This function needs to be implemented.
         raise NotImplementedError("This should have been implemented by subclassing")
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _to_matrix_func(self) -> NDArrayf:
         # FOR DEVELOPERS: This function needs to be implemented if the `self._meta['matrix']` keyword is not None.
 
         # Try to see if a matrix exists.
         meta_matrix = self._meta.get("matrix")
         if meta_matrix is not None:
             assert meta_matrix.shape == (4, 4), f"Invalid _meta matrix shape. Expected: (4, 4), got {meta_matrix.shape}"
             return meta_matrix
 
         raise NotImplementedError("This should be implemented by subclassing")
 
-    def _apply_func(self, dem: np.ndarray, transform: rio.transform.Affine, **kwargs) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
         # FOR DEVELOPERS: This function is only needed for non-rigid transforms.
         raise NotImplementedError("This should have been implemented by subclassing")
 
-    def _apply_pts_func(self, coords: np.ndarray) -> np.ndarray:
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
         # FOR DEVELOPERS: This function is only needed for non-rigid transforms.
         raise NotImplementedError("This should have been implemented by subclassing")
 
 
 class BiasCorr(Coreg):
     """
     DEM bias correction.
 
     Estimates the mean (or median, weighted avg., etc.) offset between two DEMs.
     """
 
-    def __init__(self, bias_func=np.average):  # pylint: disable=super-init-not-called
+    def __init__(self, bias_func: Callable[[NDArrayf], np.floating[Any]] = np.average) -> None:  # pylint:
+        # disable=super-init-not-called
         """
         Instantiate a bias correction object.
 
         :param bias_func: The function to use for calculating the bias. Default: (weighted) average.
         """
+        self._meta: CoregDict = {}  # All __init__ functions should instantiate an empty dict.
+
         super().__init__(meta={"bias_func": bias_func})
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Estimate the bias using the bias_func."""
         if verbose:
             print("Estimating bias...")
         diff = ref_dem - tba_dem
         diff = diff[np.isfinite(diff)]
 
         if np.count_nonzero(np.isfinite(diff)) == 0:
             raise ValueError("No finite values in bias comparison.")
 
         # Use weights if those were provided.
-        bias = self._meta["bias_func"](diff) if weights is None \
-            else self._meta["bias_func"](diff, weights=weights)
+        bias = (
+            self._meta["bias_func"](diff) if weights is None else self._meta["bias_func"](diff, weights)  # type: ignore
+        )
+        # TODO: We might need to define the type of bias_func with Callback protocols to get the optional argument,
+        # TODO: once we have the weights implemented
 
         if verbose:
             print("Bias estimated")
 
         self._meta["bias"] = bias
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
+        """Apply the BiasCorr function to a DEM."""
+        return dem + self._meta["bias"], transform
+
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
+        """Apply the BiasCorr function to a set of points."""
+        new_coords = coords.copy()
+        new_coords[:, 2] += self._meta["bias"]
+        return new_coords
+
+    def _to_matrix_func(self) -> NDArrayf:
         """Convert the bias to a transform matrix."""
         empty_matrix = np.diag(np.ones(4, dtype=float))
 
         empty_matrix[2, 3] += self._meta["bias"]
 
         return empty_matrix
 
@@ -870,18 +1054,20 @@
     """
     Iterative Closest Point DEM coregistration.
     Based on 3D registration of Besl and McKay (1992), https://doi.org/10.1117/12.57955.
 
     Estimates a rigid transform (rotation + translation) between two DEMs.
 
     Requires 'opencv'
-    See opencv docs for more info: https://docs.opencv.org/master/dc/d9b/classcv_1_1ppf__match__3d_1_1ICP.html
+    See opencv doc for more info: https://docs.opencv.org/master/dc/d9b/classcv_1_1ppf__match__3d_1_1ICP.html
     """
 
-    def __init__(self, max_iterations=100, tolerance=0.05, rejection_scale=2.5, num_levels=6):
+    def __init__(
+        self, max_iterations: int = 100, tolerance: float = 0.05, rejection_scale: float = 2.5, num_levels: int = 6
+    ) -> None:
         """
         Instantiate an ICP coregistration object.
 
         :param max_iterations: The maximum allowed iterations before stopping.
         :param tolerance: The residual change threshold after which to stop the iterations.
         :param rejection_scale: The threshold (std * rejection_scale) to consider points as outliers.
         :param num_levels: Number of octree levels to consider. A higher number is faster but may be more inaccurate.
@@ -891,67 +1077,75 @@
         self.max_iterations = max_iterations
         self.tolerance = tolerance
         self.rejection_scale = rejection_scale
         self.num_levels = num_levels
 
         super().__init__()
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Estimate the rigid transform from tba_dem to ref_dem."""
 
         if weights is not None:
             warnings.warn("ICP was given weights, but does not support it.")
 
-
         bounds, resolution = _transform_to_bounds_and_res(ref_dem.shape, transform)
-        points: dict[str, np.ndarray] = {}
+        points: dict[str, NDArrayf] = {}
         # Generate the x and y coordinates for the reference_dem
         x_coords, y_coords = _get_x_and_y_coords(ref_dem.shape, transform)
 
-        centroid = np.array([np.mean([bounds.left, bounds.right]), np.mean([bounds.bottom, bounds.top]), 0.0])
+        centroid = (np.mean([bounds.left, bounds.right]), np.mean([bounds.bottom, bounds.top]), 0.0)
         # Subtract by the bounding coordinates to avoid float32 rounding errors.
         x_coords -= centroid[0]
         y_coords -= centroid[1]
         for key, dem in zip(["ref", "tba"], [ref_dem, tba_dem]):
 
             gradient_x, gradient_y = np.gradient(dem)
 
             normal_east = np.sin(np.arctan(gradient_y / resolution)) * -1
             normal_north = np.sin(np.arctan(gradient_x / resolution))
             normal_up = 1 - np.linalg.norm([normal_east, normal_north], axis=0)
 
             valid_mask = ~np.isnan(dem) & ~np.isnan(normal_east) & ~np.isnan(normal_north)
 
-            point_cloud = np.dstack([
-                x_coords[valid_mask],
-                y_coords[valid_mask],
-                dem[valid_mask],
-                normal_east[valid_mask],
-                normal_north[valid_mask],
-                normal_up[valid_mask]
-            ]).squeeze()
+            point_cloud = np.dstack(
+                [
+                    x_coords[valid_mask],
+                    y_coords[valid_mask],
+                    dem[valid_mask],
+                    normal_east[valid_mask],
+                    normal_north[valid_mask],
+                    normal_up[valid_mask],
+                ]
+            ).squeeze()
 
             points[key] = point_cloud[~np.any(np.isnan(point_cloud), axis=1)].astype("float32")
 
             icp = cv2.ppf_match_3d_ICP(self.max_iterations, self.tolerance, self.rejection_scale, self.num_levels)
         if verbose:
             print("Running ICP...")
         try:
             _, residual, matrix = icp.registerModelToScene(points["tba"], points["ref"])
         except cv2.error as exception:
             if "(expected: 'n > 0'), where" not in str(exception):
                 raise exception
 
             raise ValueError(
-                    "Not enough valid points in input data."
-                    f"'reference_dem' had {points['ref'].size} valid points."
-                    f"'dem_to_be_aligned' had {points['tba'].size} valid points."
+                "Not enough valid points in input data."
+                f"'reference_dem' had {points['ref'].size} valid points."
+                f"'dem_to_be_aligned' had {points['tba'].size} valid points."
             )
-    
+
         if verbose:
             print("ICP finished")
 
         assert residual < 1000, f"ICP coregistration failed: residual={residual}, threshold: 1000"
 
         self._meta["centroid"] = centroid
         self._meta["matrix"] = matrix
@@ -960,120 +1154,73 @@
 class Deramp(Coreg):
     """
     Polynomial DEM deramping.
 
     Estimates an n-D polynomial between the difference of two DEMs.
     """
 
-    def __init__(self, degree: int = 1, subsample: Union[int, float] = 5e5):
+    def __init__(self, degree: int = 1, subsample: int | float = 5e5) -> None:
         """
         Instantiate a deramping correction object.
 
         :param degree: The polynomial degree to estimate. degree=0 is a simple bias correction.
         :param subsample: Factor for subsampling the input raster for speed-up.
             If <= 1, will be considered a fraction of valid pixels to extract.
             If > 1 will be considered the number of pixels to extract.
 
         """
         self.degree = degree
         self.subsample = subsample
 
         super().__init__()
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Fit the dDEM between the DEMs to a least squares polynomial equation."""
-        x_coords, y_coords = _get_x_and_y_coords(ref_dem.shape, transform)
-
         ddem = ref_dem - tba_dem
-        valid_mask = np.isfinite(ddem)
-        ddem = ddem[valid_mask]
-        x_coords = x_coords[valid_mask]
-        y_coords = y_coords[valid_mask]
-
-        # Formulate the 2D polynomial whose coefficients will be solved for.
-        def poly2d(x_coordinates: np.ndarray, y_coordinates: np.ndarray,
-                   coefficients: np.ndarray) -> np.ndarray:
-            """
-            Estimate values from a 2D-polynomial.
-
-            :param x_coordinates: x-coordinates of the difference array (must have the same shape as elevation_difference).
-            :param y_coordinates: y-coordinates of the difference array (must have the same shape as elevation_difference).
-            :param coefficients: The coefficients (a, b, c, etc.) of the polynomial.
-            :param degree: The degree of the polynomial.
-
-            :raises ValueError: If the length of the coefficients list is not compatible with the degree.
-
-            :returns: The values estimated by the polynomial.
-            """
-            # Check that the coefficient size is correct.
-            coefficient_size = (self.degree + 1) * (self.degree + 2) / 2
-            if len(coefficients) != coefficient_size:
-                raise ValueError()
-
-            # Do Amaury's black magic to formulate and calculate the polynomial equation.
-            estimated_values = np.sum([coefficients[k * (k + 1) // 2 + j] * x_coordinates ** (k - j) *
-                                       y_coordinates ** j for k in range(self.degree + 1) for j in range(k + 1)], axis=0)
-            return estimated_values  # type: ignore
-
-        def residuals(coefs: np.ndarray, x_coords: np.ndarray, y_coords: np.ndarray, targets: np.ndarray):
-            res = targets - poly2d(x_coords, y_coords, coefs)
-            return res[np.isfinite(res)]
-
-        if verbose:
-            print("Estimating deramp function...")
-
-        # reduce number of elements for speed
-        # Get number of points to extract
-        max_points = np.size(x_coords)
-        if (self.subsample <= 1) & (self.subsample >= 0):
-            npoints = int(self.subsample * max_points)
-        elif self.subsample > 1:
-            npoints = int(self.subsample)
-        else:
-            raise ValueError("`subsample` must be >= 0")
-
-        if max_points > npoints:
-            indices = np.random.choice(max_points, npoints, replace=False)
-            x_coords = x_coords[indices]
-            y_coords = y_coords[indices]
-            ddem = ddem[indices]
-
-        # Optimize polynomial parameters
-        coefs = scipy.optimize.leastsq(
-            func=residuals,
-            x0=np.zeros(shape=((self.degree + 1) * (self.degree + 2) // 2)),
-            args=(x_coords, y_coords, ddem)
+        x_coords, y_coords = _get_x_and_y_coords(ref_dem.shape, transform)
+        fit_ramp, coefs = deramping(
+            ddem, x_coords, y_coords, degree=self.degree, subsample=self.subsample, verbose=verbose
         )
 
         self._meta["coefficients"] = coefs[0]
-        self._meta["func"] = lambda x, y: poly2d(x, y, coefs[0])
+        self._meta["func"] = fit_ramp
 
-    def _apply_func(self, dem: np.ndarray, transform: rio.transform.Affine, **kwargs) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
         """Apply the deramp function to a DEM."""
         x_coords, y_coords = _get_x_and_y_coords(dem.shape, transform)
 
         ramp = self._meta["func"](x_coords, y_coords)
 
-        return dem + ramp
+        return dem + ramp, transform
 
-    def _apply_pts_func(self, coords: np.ndarray) -> np.ndarray:
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
         """Apply the deramp function to a set of points."""
         new_coords = coords.copy()
 
         new_coords[:, 2] += self._meta["func"](new_coords[:, 0], new_coords[:, 1])
 
         return new_coords
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _to_matrix_func(self) -> NDArrayf:
         """Return a transform matrix if possible."""
         if self.degree > 1:
             raise ValueError(
                 "Nonlinear deramping degrees cannot be represented as transformation matrices."
-                f" (max 1, given: {self.degree})")
+                f" (max 1, given: {self.degree})"
+            )
         if self.degree == 1:
             raise NotImplementedError("Vertical shift, rotation and horizontal scaling has to be implemented.")
 
         # If degree==0, it's just a bias correction
         empty_matrix = np.diag(np.ones(4, dtype=float))
 
         empty_matrix[2, 3] += self._meta["coefficients"][0]
@@ -1082,67 +1229,77 @@
 
 
 class CoregPipeline(Coreg):
     """
     A sequential set of coregistration steps.
     """
 
-    def __init__(self, pipeline: list[Coreg]):
+    def __init__(self, pipeline: list[Coreg]) -> None:
         """
         Instantiate a new coregistration pipeline.
 
         :param: Coregistration steps to run in the sequence they are given.
         """
         self.pipeline = pipeline
 
         super().__init__()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"CoregPipeline: {self.pipeline}"
 
     def copy(self: CoregType) -> CoregType:
         """Return an identical copy of the class."""
         new_coreg = self.__new__(type(self))
 
         new_coreg.__dict__ = {key: copy.copy(value) for key, value in self.__dict__.items() if key != "pipeline"}
         new_coreg.pipeline = [step.copy() for step in self.pipeline]
 
         return new_coreg
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Fit each coregistration step with the previously transformed DEM."""
         tba_dem_mod = tba_dem.copy()
 
         for i, coreg in enumerate(self.pipeline):
             if verbose:
                 print(f"Running pipeline step: {i + 1} / {len(self.pipeline)}")
-            coreg._fit_func(ref_dem, tba_dem_mod, transform=transform, weights=weights, verbose=verbose)
+            coreg._fit_func(ref_dem, tba_dem_mod, transform=transform, crs=crs, weights=weights, verbose=verbose)
             coreg._fit_called = True
 
-            tba_dem_mod = coreg.apply(tba_dem_mod, transform)
+            tba_dem_mod, out_transform = coreg.apply(tba_dem_mod, transform, crs)
 
-    def _apply_func(self, dem: np.ndarray, transform: rio.transform.Affine, **kwargs) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
         """Apply the coregistration steps sequentially to a DEM."""
         dem_mod = dem.copy()
+        out_transform = copy.copy(transform)
         for coreg in self.pipeline:
-            dem_mod = coreg.apply(dem_mod, transform, **kwargs)
+            dem_mod, out_transform = coreg.apply(dem_mod, out_transform, crs, **kwargs)
 
-        return dem_mod
+        return dem_mod, out_transform
 
-    def _apply_pts_func(self, coords: np.ndarray) -> np.ndarray:
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
         """Apply the coregistration steps sequentially to a set of points."""
         coords_mod = coords.copy()
 
         for coreg in self.pipeline:
             coords_mod = coreg.apply_pts(coords_mod).reshape(coords_mod.shape)
 
         return coords_mod
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _to_matrix_func(self) -> NDArrayf:
         """Try to join the coregistration steps to a single transformation matrix."""
         if not _HAS_P3D:
             raise ValueError("Optional dependency needed. Install 'pytransform3d'")
 
         transform_mgr = TransformManager()
 
         with warnings.catch_warnings():
@@ -1151,20 +1308,19 @@
             for i, coreg in enumerate(self.pipeline):
                 new_matrix = coreg.to_matrix()
 
                 transform_mgr.add_transform(i, i + 1, new_matrix)
 
             return transform_mgr.get_transform(0, len(self.pipeline))
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[Coreg, None, None]:
         """Iterate over the pipeline steps."""
-        for coreg in self.pipeline:
-            yield coreg
+        yield from self.pipeline
 
-    def __add__(self, other: Union[list[Coreg], Coreg, CoregPipeline]) -> CoregPipeline:
+    def __add__(self, other: list[Coreg] | Coreg | CoregPipeline) -> CoregPipeline:
         """Append Coreg(s) or a CoregPipeline to the pipeline."""
         if not isinstance(other, Coreg):
             other = list(other)
         else:
             other = [other]
 
         pipelines = self.pipeline + other
@@ -1176,40 +1332,56 @@
     """
     Nuth and Kääb (2011) DEM coregistration.
 
     Implemented after the paper:
     https://doi.org/10.5194/tc-5-271-2011
     """
 
-    def __init__(self, max_iterations: int = 10, offset_threshold: float = 0.05):
+    def __init__(self, max_iterations: int = 10, offset_threshold: float = 0.05) -> None:
         """
         Instantiate a new Nuth and Kääb (2011) coregistration object.
 
         :param max_iterations: The maximum allowed iterations before stopping.
         :param offset_threshold: The residual offset threshold after which to stop the iterations.
         """
+        self._meta: CoregDict
         self.max_iterations = max_iterations
         self.offset_threshold = offset_threshold
 
         super().__init__()
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Estimate the x/y/z offset between two DEMs."""
         if verbose:
             print("Running Nuth and Kääb (2011) coregistration")
 
         bounds, resolution = _transform_to_bounds_and_res(ref_dem.shape, transform)
         # Make a new DEM which will be modified inplace
         aligned_dem = tba_dem.copy()
 
+        # Check that DEM CRS is projected, otherwise slope is not correctly calculated
+        if not crs.is_projected:
+            raise NotImplementedError(
+                f"DEMs CRS is {crs}. NuthKaab coregistration only works with \
+projected CRS. First, reproject your DEMs in a local projected CRS, e.g. UTM, and re-run."
+            )
+
         # Calculate slope and aspect maps from the reference DEM
         if verbose:
             print("   Calculate slope and aspect")
-        slope, aspect = calculate_slope_and_aspect(ref_dem)
+
+        slope_tan, aspect = _calculate_slope_and_aspect_nuthkaab(ref_dem)
 
         # Make index grids for the east and north dimensions
         east_grid = np.arange(ref_dem.shape[1])
         north_grid = np.arange(ref_dem.shape[0])
 
         # Make a function to estimate the aligned DEM (used to construct an offset DEM)
         elevation_function = scipy.interpolate.RectBivariateSpline(
@@ -1219,46 +1391,44 @@
         # Make a function to estimate nodata gaps in the aligned DEM (used to fix the estimated offset DEM)
         # Use spline degree 1, as higher degrees will create instabilities around 1 and mess up the nodata mask
         nodata_function = scipy.interpolate.RectBivariateSpline(
             x=north_grid, y=east_grid, z=np.isnan(aligned_dem), kx=1, ky=1
         )
 
         # Initialise east and north pixel offset variables (these will be incremented up and down)
-        offset_east, offset_north, bias = 0.0, 0.0, 0.0
+        offset_east, offset_north = 0.0, 0.0
 
         # Calculate initial dDEM statistics
         elevation_difference = ref_dem - aligned_dem
         bias = np.nanmedian(elevation_difference)
         nmad_old = xdem.spatialstats.nmad(elevation_difference)
         if verbose:
             print("   Statistics on initial dh:")
-            print("      Median = {:.2f} - NMAD = {:.2f}".format(bias, nmad_old))
+            print(f"      Median = {bias:.2f} - NMAD = {nmad_old:.2f}")
 
         # Iteratively run the analysis until the maximum iterations or until the error gets low enough
         if verbose:
-            print("   Iteratively estimating horizontal shit:")
+            print("   Iteratively estimating horizontal shift:")
 
         # If verbose is True, will use progressbar and print additional statements
         pbar = trange(self.max_iterations, disable=not verbose, desc="   Progress")
         for i in pbar:
 
             # Calculate the elevation difference and the residual (NMAD) between them.
             elevation_difference = ref_dem - aligned_dem
             bias = np.nanmedian(elevation_difference)
             # Correct potential biases
             elevation_difference -= bias
 
             # Estimate the horizontal shift from the implementation by Nuth and Kääb (2011)
             east_diff, north_diff, _ = get_horizontal_shift(  # type: ignore
-                elevation_difference=elevation_difference,
-                slope=slope,
-                aspect=aspect
+                elevation_difference=elevation_difference, slope=slope_tan, aspect=aspect
             )
             if verbose:
-                pbar.write("      #{:d} - Offset in pixels : ({:.2f}, {:.2f})".format(i + 1, east_diff, north_diff))
+                pbar.write(f"      #{i + 1:d} - Offset in pixels : ({east_diff:.2f}, {north_diff:.2f})")
 
             # Increment the offsets with the overall offset
             offset_east += east_diff
             offset_north += north_diff
 
             # Calculate new elevations from the offset x- and y-coordinates
             new_elevation = elevation_function(y=east_grid + offset_east, x=north_grid - offset_north)
@@ -1270,69 +1440,99 @@
             # Assign the newly calculated elevations to the aligned_dem
             aligned_dem = new_elevation
 
             # Update statistics
             elevation_difference = ref_dem - aligned_dem
             bias = np.nanmedian(elevation_difference)
             nmad_new = xdem.spatialstats.nmad(elevation_difference)
-            nmad_gain = (nmad_new - nmad_old) / nmad_old*100
+            nmad_gain = (nmad_new - nmad_old) / nmad_old * 100
 
             if verbose:
-                pbar.write("      Median = {:.2f} - NMAD = {:.2f}  ==>  Gain = {:.2f}%".format(bias, nmad_new, nmad_gain))
+                pbar.write(f"      Median = {bias:.2f} - NMAD = {nmad_new:.2f}  ==>  Gain = {nmad_gain:.2f}%")
 
             # Stop if the NMAD is low and a few iterations have been made
             assert ~np.isnan(nmad_new), (offset_east, offset_north)
 
             offset = np.sqrt(east_diff**2 + north_diff**2)
             if i > 1 and offset < self.offset_threshold:
                 if verbose:
-                    pbar.write(f"   Last offset was below the residual offset threshold of {self.offset_threshold} -> stopping")
+                    pbar.write(
+                        f"   Last offset was below the residual offset threshold of {self.offset_threshold} -> stopping"
+                    )
                 break
 
             nmad_old = nmad_new
 
         # Print final results
         if verbose:
-            print("\n   Final offset in pixels (east, north) : ({:f}, {:f})".format(offset_east, offset_north))
+            print(f"\n   Final offset in pixels (east, north) : ({offset_east:f}, {offset_north:f})")
             print("   Statistics on coregistered dh:")
-            print("      Median = {:.2f} - NMAD = {:.2f}".format(bias, nmad_new))
+            print(f"      Median = {bias:.2f} - NMAD = {nmad_new:.2f}")
 
         self._meta["offset_east_px"] = offset_east
         self._meta["offset_north_px"] = offset_north
         self._meta["bias"] = bias
         self._meta["resolution"] = resolution
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _to_matrix_func(self) -> NDArrayf:
         """Return a transformation matrix from the estimated offsets."""
         offset_east = self._meta["offset_east_px"] * self._meta["resolution"]
         offset_north = self._meta["offset_north_px"] * self._meta["resolution"]
 
         matrix = np.diag(np.ones(4, dtype=float))
         matrix[0, 3] += offset_east
         matrix[1, 3] += offset_north
         matrix[2, 3] += self._meta["bias"]
 
         return matrix
 
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
+        """Apply the Nuth & Kaab shift to a DEM."""
+        offset_east = self._meta["offset_east_px"] * self._meta["resolution"]
+        offset_north = self._meta["offset_north_px"] * self._meta["resolution"]
 
-def invert_matrix(matrix: np.ndarray) -> np.ndarray:
+        updated_transform = apply_xy_shift(transform, -offset_east, -offset_north)
+        bias = self._meta["bias"]
+        return dem + bias, updated_transform
+
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
+        """Apply the Nuth & Kaab shift to a set of points."""
+        offset_east = self._meta["offset_east_px"] * self._meta["resolution"]
+        offset_north = self._meta["offset_north_px"] * self._meta["resolution"]
+
+        new_coords = coords.copy()
+        new_coords[:, 0] += offset_east
+        new_coords[:, 1] += offset_north
+        new_coords[:, 2] += self._meta["bias"]
+
+        return new_coords
+
+
+def invert_matrix(matrix: NDArrayf) -> NDArrayf:
     """Invert a transformation matrix."""
     with warnings.catch_warnings():
         # Deprecation warning from pytransform3d. Let's hope that is fixed in the near future.
         warnings.filterwarnings("ignore", message="`np.float` is a deprecated alias for the builtin `float`")
 
         checked_matrix = pytransform3d.transformations.check_matrix(matrix)
         # Invert the transform if wanted.
         return pytransform3d.transformations.invert_transform(checked_matrix)
 
 
-def apply_matrix(dem: np.ndarray, transform: rio.transform.Affine, matrix: np.ndarray, invert: bool = False,
-                 centroid: Optional[tuple[float, float, float]] = None,
-                 resampling: Union[int, str] = "bilinear",
-                 dilate_mask: bool = False, **kwargs) -> np.ndarray:
+def apply_matrix(
+    dem: NDArrayf,
+    transform: rio.transform.Affine,
+    matrix: NDArrayf,
+    invert: bool = False,
+    centroid: tuple[float, float, float] | None = None,
+    resampling: int | str = "bilinear",
+    fill_max_search: int = 0,
+) -> NDArrayf:
     """
     Apply a 3D transformation matrix to a 2.5D DEM.
 
     The transformation is applied as a value correction using linear deramping, and 2D image warping.
 
     1. Convert the DEM into a point cloud (not for gridding; for estimating the DEM shifts).
     2. Transform the point cloud in 3D using the 4x4 matrix.
@@ -1344,15 +1544,17 @@
 
     :param dem: The DEM to transform.
     :param transform: The Affine transform object (georeferencing) of the DEM.
     :param matrix: A 4x4 transformation matrix to apply to the DEM.
     :param invert: Invert the transformation matrix.
     :param centroid: The X/Y/Z transformation centroid. Irrelevant for pure translations. Defaults to the midpoint (Z=0)
     :param resampling: The resampling method to use. Can be `nearest`, `bilinear`, `cubic` or an integer from 0-5.
-    :param dilate_mask: Dilate the nan mask to exclude edge pixels that could be wrong.
+    :param fill_max_search: Set to > 0 value to fill the DEM before applying the transformation, to avoid spreading\
+    gaps. The DEM will be filled with rasterio.fill.fillnodata with max_search_distance set to fill_max_search.\
+    This is experimental, use at your own risk !
 
     :returns: The transformed DEM with NaNs as nodata values (replaces a potential mask of the input `dem`).
     """
     # Parse the resampling argument given.
     if isinstance(resampling, (int, np.integer)):
         resampling_order = resampling
     elif resampling == "cubic":
@@ -1375,18 +1577,21 @@
     if np.mean(np.abs(empty_matrix - matrix)) == 0.0:
         return demc + matrix[2, 3]
 
     # Opencv is required down from here
     if not _has_cv2:
         raise ValueError("Optional dependency needed. Install 'opencv'")
 
-    nan_mask = spatial_tools.get_mask(dem)
+    nan_mask = ~np.isfinite(dem)
     assert np.count_nonzero(~nan_mask) > 0, "Given DEM had all nans."
-    # Create a filled version of the DEM. (skimage doesn't like nans)
-    filled_dem = np.where(~nan_mask, demc, np.nan)
+    # Optionally, fill DEM around gaps to reduce spread of gaps
+    if fill_max_search > 0:
+        filled_dem = rio.fill.fillnodata(demc, mask=(~nan_mask).astype("uint8"), max_search_distance=fill_max_search)
+    else:
+        filled_dem = demc  # np.where(~nan_mask, demc, np.nan)  # I don't know why this was needed - to delete
 
     # Get the centre coordinates of the DEM pixels.
     x_coords, y_coords = _get_x_and_y_coords(demc.shape, transform)
 
     bounds, resolution = _transform_to_bounds_and_res(dem.shape, transform)
 
     # If a centroid was not given, default to the center of the DEM (at Z=0).
@@ -1411,26 +1616,28 @@
     # Transform the point cloud using the matrix.
     transformed_points = cv2.perspectiveTransform(
         point_cloud.reshape((1, -1, 3)),
         matrix,
     ).reshape(point_cloud.shape)
 
     # Estimate the vertical difference of old and new point cloud elevations.
-    deramp = deramping(
+    deramp, coeffs = deramping(
         (point_cloud[:, :, 2] - transformed_points[:, :, 2])[~nan_mask].flatten(),
         point_cloud[:, :, 0][~nan_mask].flatten(),
         point_cloud[:, :, 1][~nan_mask].flatten(),
-        degree=1
+        degree=1,
     )
     # Shift the elevation values of the soon-to-be-warped DEM.
     filled_dem -= deramp(x_coords, y_coords)
 
-    # Create gap-free arrays of x and y coordinates to be converted into index coordinates.
-    x_inds = rio.fill.fillnodata(transformed_points[:, :, 0].copy(), mask=(~nan_mask).astype("uint8"))
-    y_inds = rio.fill.fillnodata(transformed_points[:, :, 1].copy(), mask=(~nan_mask).astype("uint8"))
+    # Create arrays of x and y coordinates to be converted into index coordinates.
+    x_inds = transformed_points[:, :, 0].copy()
+    x_inds[x_inds == 0] = np.nan
+    y_inds = transformed_points[:, :, 1].copy()
+    y_inds[y_inds == 0] = np.nan
 
     # Divide the coordinates by the resolution to create index coordinates.
     x_inds /= resolution
     y_inds /= resolution
     # Shift the x coords so that bounds.left is equivalent to xindex -0.5
     x_inds -= x_coords.min() / resolution
     # Shift the y coords so that bounds.top is equivalent to yindex -0.5
@@ -1440,36 +1647,16 @@
     inds = np.vstack((y_inds.reshape((1,) + y_inds.shape), x_inds.reshape((1,) + x_inds.shape)))
 
     with warnings.catch_warnings():
         # An skimage warning that will hopefully be fixed soon. (2021-07-30)
         warnings.filterwarnings("ignore", message="Passing `np.nan` to mean no clipping in np.clip")
         # Warp the DEM
         transformed_dem = skimage.transform.warp(
-            filled_dem,
-            inds,
-            order=resampling_order,
-            mode="constant",
-            cval=np.nan,
-            preserve_range=True
+            filled_dem, inds, order=resampling_order, mode="constant", cval=np.nan, preserve_range=True
         )
-        # Warp the NaN mask, setting true to all values outside the new frame.
-        tr_nan_mask = skimage.transform.warp(
-            nan_mask.astype("uint8"),
-            inds,
-            order=resampling_order,
-            mode="constant",
-            cval=1,
-            preserve_range=True
-        ) > 0
-
-    if dilate_mask:
-        tr_nan_mask = scipy.ndimage.binary_dilation(tr_nan_mask, iterations=resampling_order)
-
-    # Apply the transformed nan_mask
-    transformed_dem[tr_nan_mask] = np.nan
 
     assert np.count_nonzero(~np.isnan(transformed_dem)) > 0, "Transformed DEM has all nans."
 
     return transformed_dem
 
 
 class ZScaleCorr(Coreg):
@@ -1478,105 +1665,123 @@
 
     Often useful for nadir image DEM correction, where the focal length is slightly miscalculated.
 
     DISCLAIMER: This function may introduce error when correcting non-photogrammetric biases.
     See Gardelle et al. (2012) (Figure 2), http://dx.doi.org/10.3189/2012jog11j175, for curvature-related biases.
     """
 
-    def __init__(self, degree=1, bin_count=100):
+    def __init__(self, degree: float = 1, bin_count: int = 100) -> None:
         """
         Instantiate a elevation scale correction object.
 
         :param degree: The polynomial degree to estimate.
         :param bin_count: The amount of bins to divide the elevation change in.
         """
         self.degree = degree
         self.bin_count = bin_count
 
         super().__init__()
 
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: Optional[rio.transform.Affine],
-                  weights: Optional[np.ndarray], verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Estimate the scale difference between the two DEMs."""
         ddem = ref_dem - tba_dem
 
-        medians = xdem.volume.hypsometric_binning(
-            ddem=ddem,
-            ref_dem=tba_dem,
-            bins=self.bin_count,
-            kind="count"
-        )["value"]
+        medians = xdem.volume.hypsometric_binning(ddem=ddem, ref_dem=tba_dem, bins=self.bin_count, kind="count")[
+            "value"
+        ]
 
         coefficients = np.polyfit(medians.index.mid, medians.values, deg=self.degree)
         self._meta["coefficients"] = coefficients
 
-    def _apply_func(self, dem: np.ndarray, transform: rio.transform.Affine, **kwargs) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
         """Apply the scaling model to a DEM."""
         model = np.poly1d(self._meta["coefficients"])
 
-        return dem + model(dem)
+        return dem + model(dem), transform
 
-    def _apply_pts_func(self, coords: np.ndarray) -> np.ndarray:
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
         """Apply the scaling model to a set of points."""
         model = np.poly1d(self._meta["coefficients"])
 
         new_coords = coords.copy()
         new_coords[:, 2] += model(new_coords[:, 2])
         return new_coords
 
-    def _to_matrix_func(self) -> np.ndarray:
+    def _to_matrix_func(self) -> NDArrayf:
         """Convert the transform to a matrix, if possible."""
         if self.degree == 0:  # If it's just a bias correction.
             return self._meta["coefficients"][-1]
         elif self.degree < 2:
             raise NotImplementedError
         else:
             raise ValueError("A 2nd degree or higher ZScaleCorr cannot be described as a 4x4 matrix!")
 
+
 class BlockwiseCoreg(Coreg):
     """
     Block-wise coreg class for nonlinear estimations.
 
     A coreg class of choice is run on an arbitrary subdivision of the raster. When later applying the coregistration,\
         the optimal warping is interpolated based on X/Y/Z shifts from the coreg algorithm at the grid points.
 
     E.g. a subdivision of 4 means to divide the DEM in four equally sized parts. These parts are then coregistered\
         separately, creating four Coreg.fit results. If the subdivision is not divisible by the raster shape,\
         subdivision is made as best as possible to have approximately equal pixel counts.
     """
 
-    def __init__(self, coreg: Coreg | CoregPipeline, subdivision: int, success_threshold: float = 0.8, n_threads: int | None = None, warn_failures: bool = False):
+    def __init__(
+        self,
+        coreg: Coreg | CoregPipeline,
+        subdivision: int,
+        success_threshold: float = 0.8,
+        n_threads: int | None = None,
+        warn_failures: bool = False,
+    ) -> None:
         """
         Instantiate a blockwise coreg object.
 
         :param coreg: An instantiated coreg object to fit in the subdivided DEMs.
         :param subdivision: The number of chunks to divide the DEMs in. E.g. 4 means four different transforms.
         :param success_threshold: Raise an error if fewer chunks than the fraction failed for any reason.
         :param n_threads: The maximum amount of threads to use. Default=auto
         :param warn_failures: Trigger or ignore warnings for each exception/warning in each block.
         """
         if isinstance(coreg, type):
             raise ValueError(
-                    "The 'coreg' argument must be an instantiated Coreg subclass. "
-                    "Hint: write e.g. ICP() instead of ICP"
+                "The 'coreg' argument must be an instantiated Coreg subclass. " "Hint: write e.g. ICP() instead of ICP"
             )
         self.coreg = coreg
         self.subdivision = subdivision
         self.success_threshold = success_threshold
         self.n_threads = n_threads
         self.warn_failures = warn_failures
 
         super().__init__()
 
-        self._meta["coreg_meta"] = []
+        self._meta: CoregDict = {"coreg_meta": []}
 
-
-
-    def _fit_func(self, ref_dem: np.ndarray, tba_dem: np.ndarray, transform: rio.transform.Affine | None,
-                  weights: np.ndarray | None, verbose: bool = False):
+    def _fit_func(
+        self,
+        ref_dem: NDArrayf,
+        tba_dem: NDArrayf,
+        transform: rio.transform.Affine,
+        crs: rio.crs.CRS,
+        weights: NDArrayf | None,
+        verbose: bool = False,
+    ) -> None:
         """Fit the coreg approach for each subdivision."""
 
         groups = self.subdivide_array(tba_dem.shape)
 
         indices = np.unique(groups)
 
         progress_bar = tqdm(total=indices.size, desc="Coregistering chunks", disable=(not verbose))
@@ -1590,53 +1795,53 @@
                 * If it fails: The associated exception.
                 * If the block is empty: None
             """
             inlier_mask = groups == i
 
             # Find the corresponding slice of the inlier_mask to subset the data
             rows, cols = np.where(inlier_mask)
-            arrayslice = np.s_[rows.min():rows.max() + 1, cols.min(): cols.max() + 1]
+            arrayslice = np.s_[rows.min() : rows.max() + 1, cols.min() : cols.max() + 1]
 
             # Copy a subset of the two DEMs, the mask, the coreg instance, and make a new subset transform
             ref_subset = ref_dem[arrayslice].copy()
             tba_subset = tba_dem[arrayslice].copy()
 
             if any(np.all(~np.isfinite(dem)) for dem in (ref_subset, tba_subset)):
                 return None
             mask_subset = inlier_mask[arrayslice].copy()
             west, top = rio.transform.xy(transform, min(rows), min(cols), offset="ul")
             transform_subset = rio.transform.from_origin(west, top, transform.a, -transform.e)
             coreg = self.coreg.copy()
 
-
             # Try to run the coregistration. If it fails for any reason, skip it and save the exception.
             try:
                 coreg.fit(
                     reference_dem=ref_subset,
                     dem_to_be_aligned=tba_subset,
                     transform=transform_subset,
-                    inlier_mask=mask_subset
+                    inlier_mask=mask_subset,
+                    crs=crs,
                 )
-
                 nmad, median = coreg.error(
                     reference_dem=ref_subset,
                     dem_to_be_aligned=tba_subset,
                     error_type=["nmad", "median"],
                     inlier_mask=mask_subset,
-                    transform=transform_subset
+                    transform=transform_subset,
+                    crs=crs,
                 )
             except Exception as exception:
                 return exception
 
             meta: dict[str, Any] = {
                 "i": i,
                 "transform": transform_subset,
                 "inlier_count": np.count_nonzero(mask_subset & np.isfinite(ref_subset) & np.isfinite(tba_subset)),
                 "nmad": nmad,
-                "median": median
+                "median": median,
             }
             # Find the center of the inliers.
             inlier_positions = np.argwhere(mask_subset)
             mid_row = np.mean(inlier_positions[:, 0]).astype(int)
             mid_col = np.mean(inlier_positions[:, 1]).astype(int)
 
             # Find the indices of all finites within the mask
@@ -1644,24 +1849,33 @@
             # Calculate the distance between the approximate center and all finite indices
             distances = np.linalg.norm(finites - np.array([mid_row, mid_col]), axis=1)
             # Find the index representing the closest finite value to the center.
             closest = np.argwhere(distances == distances.min())
 
             # Assign the closest finite value as the representative point
             representative_row, representative_col = finites[closest][0][0]
-            meta["representative_x"], meta["representative_y"] = rio.transform.xy(transform_subset, representative_row, representative_col)
-            meta["representative_val"] = ref_subset[representative_row, representative_col]
+            meta["representative_x"], meta["representative_y"] = rio.transform.xy(
+                transform_subset, representative_row, representative_col
+            )
+
+            repr_val = ref_subset[representative_row, representative_col]
+            if ~np.isfinite(repr_val):
+                repr_val = 0
+            meta["representative_val"] = repr_val
 
             # If the coreg is a pipeline, copy its metadatas to the output meta
             if hasattr(coreg, "pipeline"):
                 meta["pipeline"] = [step._meta.copy() for step in coreg.pipeline]
 
-            # Copy all current metadata (except for the alreay existing keys like "i", "min_row", etc, and the "coreg_meta" key)
+            # Copy all current metadata (except for the already existing keys like "i", "min_row", etc, and the
+            # "coreg_meta" key)
             # This can then be iteratively restored when the apply function should be called.
-            meta.update({key: value for key, value in coreg._meta.items() if key not in ["coreg_meta"] + list(meta.keys())})
+            meta.update(
+                {key: value for key, value in coreg._meta.items() if key not in ["coreg_meta"] + list(meta.keys())}
+            )
 
             progress_bar.update()
 
             return meta.copy()
 
         # Catch warnings; only show them if
         exceptions: list[BaseException | warnings.WarningMessage] = []
@@ -1683,69 +1897,71 @@
                 self._meta["coreg_meta"].append(result)
 
         progress_bar.close()
 
         # Stop if the success rate was below the threshold
         if ((len(self._meta["coreg_meta"]) + empty_blocks) / self.subdivision) <= self.success_threshold:
             raise ValueError(
-                f"Fitting failed for {len(exceptions)} chunks:\n" +
-                "\n".join(map(str, exceptions[:5])) +
-                f"\n... and {len(exceptions) - 5} more" if len(exceptions) > 5 else ""
+                f"Fitting failed for {len(exceptions)} chunks:\n"
+                + "\n".join(map(str, exceptions[:5]))
+                + f"\n... and {len(exceptions) - 5} more"
+                if len(exceptions) > 5
+                else ""
             )
 
         if self.warn_failures:
             for exception in exceptions:
                 warnings.warn(str(exception))
 
         # Set the _fit_called parameters (only identical copies of self.coreg have actually been called)
         self.coreg._fit_called = True
-        if hasattr(self.coreg, "pipeline"):
+        if isinstance(self.coreg, CoregPipeline):
             for step in self.coreg.pipeline:
                 step._fit_called = True
 
-    def _restore_metadata(self, meta: dict[str, Any]) -> None:
+    def _restore_metadata(self, meta: CoregDict) -> None:
         """
         Given some metadata, set it in the right place.
 
         :param meta: A metadata file to update self._meta
         """
         self.coreg._meta.update(meta)
 
-        if hasattr(self.coreg, "pipeline") and "pipeline" in meta:
+        if isinstance(self.coreg, CoregPipeline) and "pipeline" in meta:
             for i, step in enumerate(self.coreg.pipeline):
                 step._meta.update(meta["pipeline"][i])
 
-    def to_points(self) -> np.ndarray:
+    def to_points(self) -> NDArrayf:
         """
         Convert the blockwise coregistration matrices to 3D (source -> destination) points.
 
         The returned shape is (N, 3, 2) where the dimensions represent:
             0. The point index where N is equal to the amount of subdivisions.
             1. The X/Y/Z coordinate of the point.
             2. The old/new position of the point.
 
         To acquire the first point's original position: points[0, :, 0]
         To acquire the first point's new position: points[0, :, 1]
         To acquire the first point's Z difference: points[0, 2, 1] - points[0, 2, 0]
 
-        :returns: An array of 3D source -> destionation points.
+        :returns: An array of 3D source -> destination points.
         """
         if len(self._meta["coreg_meta"]) == 0:
             raise AssertionError("No coreg results exist. Has '.fit()' been called?")
         points = np.empty(shape=(0, 3, 2))
         for meta in self._meta["coreg_meta"]:
             self._restore_metadata(meta)
 
-            #x_coord, y_coord = rio.transform.xy(meta["transform"], meta["representative_row"], meta["representative_col"])
+            # x_coord, y_coord = rio.transform.xy(meta["transform"], meta["representative_row"],
+            # meta["representative_col"])
             x_coord, y_coord = meta["representative_x"], meta["representative_y"]
 
-
             old_position = np.reshape([x_coord, y_coord, meta["representative_val"]], (1, 3))
             new_position = self.coreg.apply_pts(old_position)
-        
+
             points = np.append(points, np.dstack((old_position, new_position)), axis=0)
 
         return points
 
     def stats(self) -> pd.DataFrame:
         """
         Return statistics for each chunk in the blockwise coregistration.
@@ -1774,68 +1990,75 @@
                     "center_y": points[i, 1, 0],
                     "center_z": points[i, 2, 0],
                     "x_off": points[i, 0, 1] - points[i, 0, 0],
                     "y_off": points[i, 1, 1] - points[i, 1, 0],
                     "z_off": points[i, 2, 1] - points[i, 2, 0],
                     "inlier_count": chunk_meta[i]["inlier_count"],
                     "nmad": chunk_meta[i]["nmad"],
-                    "median": chunk_meta[i]["median"]
+                    "median": chunk_meta[i]["median"],
                 }
             )
 
         stats_df = pd.DataFrame(statistics)
         stats_df.index.name = "chunk"
 
         return stats_df
-            
 
-    def subdivide_array(self, shape: tuple[int, ...]) -> np.ndarray:
+    def subdivide_array(self, shape: tuple[int, ...]) -> NDArrayf:
         """
         Return the grid subdivision for a given DEM shape.
 
         :param shape: The shape of the input DEM.
-        
+
         :returns: An array of shape 'shape' with 'self.subdivision' unique indices.
         """
         if len(shape) == 3 and shape[0] == 1:  # Account for (1, row, col) shapes
             shape = (shape[1], shape[2])
-        return spatial_tools.subdivide_array(shape, count=self.subdivision)
-
+        return subdivide_array(shape, count=self.subdivision)
 
-    def _apply_func(self, dem: np.ndarray, transform: rio.transform.Affine, **kwargs) -> np.ndarray:
+    def _apply_func(
+        self, dem: NDArrayf, transform: rio.transform.Affine, crs: rio.crs.CRS, **kwargs: Any
+    ) -> tuple[NDArrayf, rio.transform.Affine]:
+
+        if np.count_nonzero(np.isfinite(dem)) == 0:
+            return dem, transform
+
+        # Other option than resample=True is not implemented for this case
+        if "resample" in kwargs and kwargs["resample"] is not True:
+            raise NotImplementedError()
 
         points = self.to_points()
 
         bounds, resolution = _transform_to_bounds_and_res(dem.shape, transform)
-        
+
         representative_height = np.nanmean(dem)
-        edges_source = np.array([
-            [bounds.left + resolution / 2, bounds.top - resolution / 2, representative_height],
-            [bounds.right - resolution / 2, bounds.top - resolution / 2, representative_height],
-            [bounds.left + resolution / 2, bounds.bottom + resolution / 2, representative_height],
-            [bounds.right - resolution / 2, bounds.bottom + resolution / 2, representative_height]
-        ])
+        edges_source = np.array(
+            [
+                [bounds.left + resolution / 2, bounds.top - resolution / 2, representative_height],
+                [bounds.right - resolution / 2, bounds.top - resolution / 2, representative_height],
+                [bounds.left + resolution / 2, bounds.bottom + resolution / 2, representative_height],
+                [bounds.right - resolution / 2, bounds.bottom + resolution / 2, representative_height],
+            ]
+        )
         edges_dest = self.apply_pts(edges_source)
         edges = np.dstack((edges_source, edges_dest))
 
         all_points = np.append(points, edges, axis=0)
 
         warped_dem = warp_dem(
             dem=dem,
             transform=transform,
             source_coords=all_points[:, :, 0],
             destination_coords=all_points[:, :, 1],
-            resampling="linear"
+            resampling="linear",
         )
 
-        return warped_dem
-
+        return warped_dem, transform
 
-
-    def _apply_pts_func(self, coords: np.ndarray) -> np.ndarray:
+    def _apply_pts_func(self, coords: NDArrayf) -> NDArrayf:
         """Apply the scaling model to a set of points."""
         points = self.to_points()
 
         new_coords = coords.copy()
 
         for dim in range(0, 3):
             with warnings.catch_warnings():
@@ -1850,22 +2073,22 @@
 
             new_coords[:, dim] += model(coords[:, 0], coords[:, 1])
 
         return new_coords
 
 
 def warp_dem(
-        dem: np.ndarray,
-        transform: rio.transform.Affine,
-        source_coords: np.ndarray,
-        destination_coords: np.ndarray,
-        resampling: str = "cubic",
-        trim_border: bool = True,
-        dilate_mask: bool = True,
-    ) -> np.ndarray:
+    dem: NDArrayf,
+    transform: rio.transform.Affine,
+    source_coords: NDArrayf,
+    destination_coords: NDArrayf,
+    resampling: str = "cubic",
+    trim_border: bool = True,
+    dilate_mask: bool = True,
+) -> NDArrayf:
     """
     Warp a DEM using a set of source-destination 2D or 3D coordinates.
 
     :param dem: The DEM to warp. Allowed shapes are (1, row, col) or (row, col)
     :param transform: The Affine transform of the DEM.
     :param source_coords: The source 2D or 3D points. must be X/Y/(Z) coords of shape (N, 2) or (N, 3).
     :param destination_coords: The destination 2D or 3D points. Must have the exact same shape as 'source_coords'
@@ -1881,63 +2104,53 @@
     if source_coords.shape != destination_coords.shape:
         raise ValueError(
             f"Incompatible shapes: source_coords '({source_coords.shape})' and "
             f"destination_coords '({destination_coords.shape})' shapes must be the same"
         )
     if (len(source_coords.shape) > 2) or (source_coords.shape[1] < 2) or (source_coords.shape[1] > 3):
         raise ValueError(
-                "Invalid coordinate shape. Expected 2D or 3D coordinates of shape (N, 2) or (N, 3). "
-                f"Got '{source_coords.shape}'"
+            "Invalid coordinate shape. Expected 2D or 3D coordinates of shape (N, 2) or (N, 3). "
+            f"Got '{source_coords.shape}'"
         )
     allowed_resampling_strs = ["nearest", "linear", "cubic"]
     if resampling not in allowed_resampling_strs:
         raise ValueError(f"Resampling type '{resampling}' not understood. Choices: {allowed_resampling_strs}")
 
-    dem_arr, dem_mask = spatial_tools.get_array_and_mask(dem)
+    dem_arr, dem_mask = get_array_and_mask(dem)
 
     bounds, resolution = _transform_to_bounds_and_res(dem_arr.shape, transform)
 
-    no_horizontal =  np.sum(np.linalg.norm(destination_coords[:, :2] - source_coords[:, :2], axis=1)) < 1e-6
+    no_horizontal = np.sum(np.linalg.norm(destination_coords[:, :2] - source_coords[:, :2], axis=1)) < 1e-6
     no_vertical = source_coords.shape[1] > 2 and np.sum(np.abs(destination_coords[:, 2] - source_coords[:, 2])) < 1e-6
 
     if no_horizontal and no_vertical:
         warnings.warn("No difference between source and destination coordinates. Returning self.")
         return dem
 
     source_coords_scaled = source_coords.copy()
     destination_coords_scaled = destination_coords.copy()
     # Scale the coordinates to index-space
     for coords in (source_coords_scaled, destination_coords_scaled):
-        coords[:, 0] = (
-            dem_arr.shape[1] *
-            (coords[:, 0] - bounds.left) /
-            (bounds.right - bounds.left)
-        )
-        coords[:, 1] = (
-            dem_arr.shape[0] *
-            (1 - (
-                coords[:, 1] - bounds.bottom) /
-                (bounds.top - bounds.bottom)
-            )
-        )
+        coords[:, 0] = dem_arr.shape[1] * (coords[:, 0] - bounds.left) / (bounds.right - bounds.left)
+        coords[:, 1] = dem_arr.shape[0] * (1 - (coords[:, 1] - bounds.bottom) / (bounds.top - bounds.bottom))
 
     # Generate a grid of x and y index coordinates.
-    grid_y, grid_x = np.mgrid[0:dem_arr.shape[0], 0:dem_arr.shape[1]]
+    grid_y, grid_x = np.mgrid[0 : dem_arr.shape[0], 0 : dem_arr.shape[1]]
 
     if no_horizontal:
         warped = dem_arr.copy()
     else:
         # Interpolate the sparse source-destination points to a grid.
         # (row, col, 0) represents the destination y-coordinates of the pixels.
         # (row, col, 1) represents the destination x-coordinates of the pixels.
         new_indices = scipy.interpolate.griddata(
             source_coords_scaled[:, [1, 0]],
             destination_coords_scaled[:, [1, 0]],  # Coordinates should be in y/x (not x/y) for some reason..
             (grid_y, grid_x),
-            method="linear"
+            method="linear",
         )
 
         # If the border should not be trimmed, just assign the original indices to the missing values.
         if not trim_border:
             missing_ys = np.isnan(new_indices[:, :, 0])
             missing_xs = np.isnan(new_indices[:, :, 1])
             new_indices[:, :, 0][missing_ys] = grid_y[missing_ys]
@@ -1950,39 +2163,314 @@
             warnings.filterwarnings("ignore", message="Passing `np.nan` to mean no clipping in np.clip")
             warped = skimage.transform.warp(
                 image=np.where(dem_mask, np.nan, dem_arr),
                 inverse_map=np.moveaxis(new_indices, 2, 0),
                 output_shape=dem_arr.shape,
                 preserve_range=True,
                 order=order[resampling],
-                cval=np.nan
+                cval=np.nan,
+            )
+            new_mask = (
+                skimage.transform.warp(
+                    image=dem_mask, inverse_map=np.moveaxis(new_indices, 2, 0), output_shape=dem_arr.shape, cval=False
+                )
+                > 0
             )
-            new_mask = skimage.transform.warp(
-                image=dem_mask,
-                inverse_map=np.moveaxis(new_indices, 2, 0),
-                output_shape=dem_arr.shape,
-                cval=False
-            ) > 0
 
         if dilate_mask:
             new_mask = scipy.ndimage.binary_dilation(new_mask, iterations=order[resampling]).astype(new_mask.dtype)
 
         warped[new_mask] = np.nan
 
-
     # If the coordinates are 3D (N, 3), apply a Z correction as well.
     if not no_vertical:
         grid_offsets = scipy.interpolate.griddata(
             points=destination_coords_scaled[:, :2],
             values=destination_coords_scaled[:, 2] - source_coords_scaled[:, 2],
             xi=(grid_x, grid_y),
             method=resampling,
-            fill_value=np.nan
+            fill_value=np.nan,
         )
         if not trim_border:
             grid_offsets[np.isnan(grid_offsets)] = np.nanmean(grid_offsets)
 
         warped += grid_offsets
 
     assert not np.all(np.isnan(warped)), "All-NaN output."
 
     return warped.reshape(dem.shape)
+
+
+def create_inlier_mask(
+    src_dem: RasterType,
+    ref_dem: RasterType,
+    shp_list: list[str | gu.Vector | None] | tuple[str | gu.Vector] | tuple[()] = (),
+    inout: list[int] | tuple[int] | tuple[()] = (),
+    filtering: bool = True,
+    dh_max: AnyNumber = None,
+    nmad_factor: AnyNumber = 5,
+    slope_lim: list[AnyNumber] | tuple[AnyNumber, AnyNumber] = (0.1, 40),
+) -> NDArrayf:
+    """
+    Create a mask of inliers pixels to be used for coregistration. The following pixels can be excluded:
+    - pixels within polygons of file(s) in shp_list (with corresponding inout element set to 1) - useful for \
+    masking unstable terrain like glaciers.
+    - pixels outside polygons of file(s) in shp_list (with corresponding inout element set to -1) - useful to \
+delineate a known stable area.
+    - pixels with absolute dh (=src-ref) are larger than a given threshold
+    - pixels where absolute dh differ from the mean dh by more than a set threshold (with \
+filtering=True and nmad_factor)
+    - pixels with low/high slope (with filtering=True and set slope_lim values)
+
+    :param src_dem: the source DEM to be coregistered, as a Raster or DEM instance.
+    :param ref_dem: the reference DEM, must have same grid as src_dem. To be used for filtering only.
+    :param shp_list: a list of one or several paths to shapefiles to use for masking. Default is none.
+    :param inout: a list of same size as shp_list. For each shapefile, set to 1 (resp. -1) to specify whether \
+to mask inside (resp. outside) of the polygons. Defaults to masking inside polygons for all shapefiles.
+    :param filtering: if set to True, pixels will be removed based on dh values or slope (see next arguments).
+    :param dh_max: remove pixels where abs(src - ref) is more than this value.
+    :param nmad_factor: remove pixels where abs(src - ref) differ by nmad_factor * NMAD from the median.
+    :param slope_lim: a list/tuple of min and max slope values, in degrees. Pixels outside this slope range will \
+be excluded.
+
+    :returns: an boolean array of same shape as src_dem set to True for inlier pixels
+    """
+    # - Sanity check on inputs - #
+    # Check correct input type of shp_list
+    if not isinstance(shp_list, (list, tuple)):
+        raise ValueError("`shp_list` must be a list/tuple")
+    for el in shp_list:
+        if not isinstance(el, (str, gu.Vector)):
+            raise ValueError("`shp_list` must be a list/tuple of strings or geoutils.Vector instance")
+
+    # Check correct input type of inout
+    if not isinstance(inout, (list, tuple)):
+        raise ValueError("`inout` must be a list/tuple")
+
+    if len(shp_list) > 0:
+        if len(inout) == 0:
+            # Fill inout with 1
+            inout = [1] * len(shp_list)
+        elif len(inout) == len(shp_list):
+            # Check that inout contains only 1 and -1
+            not_valid = [el for el in np.unique(inout) if ((el != 1) & (el != -1))]
+            if len(not_valid) > 0:
+                raise ValueError("`inout` must contain only 1 and -1")
+        else:
+            raise ValueError("`inout` must be of same length as shp")
+
+    # Check slope_lim type
+    if not isinstance(slope_lim, (list, tuple)):
+        raise ValueError("`slope_lim` must be a list/tuple")
+    if len(slope_lim) != 2:
+        raise ValueError("`slope_lim` must contain 2 elements")
+    for el in slope_lim:
+        if (not isinstance(el, (int, float, np.integer, np.floating))) or (el < 0) or (el > 90):
+            raise ValueError("`slope_lim` must be a tuple/list of 2 elements in the range [0-90]")
+
+    # Initialize inlier_mask with no masked pixel
+    inlier_mask = np.ones(src_dem.data.shape, dtype="bool")
+
+    # - Create mask based on shapefiles - #
+    if len(shp_list) > 0:
+        for k, shp in enumerate(shp_list):
+            if isinstance(shp, str):
+                outlines = gu.Vector(shp)
+            else:
+                outlines = shp
+            mask_temp = outlines.create_mask(src_dem, as_array=True).reshape(np.shape(inlier_mask))
+            # Append mask for given shapefile to final mask
+            if inout[k] == 1:
+                inlier_mask[mask_temp] = False
+            elif inout[k] == -1:
+                inlier_mask[~mask_temp] = False
+
+    # - Filter possible outliers - #
+    if filtering:
+        # Calculate dDEM
+        ddem = src_dem - ref_dem
+
+        # Remove gross blunders with absolute threshold
+        if dh_max is not None:
+            inlier_mask[np.abs(ddem.data) > dh_max] = False
+
+        # Remove blunders where dh differ by nmad_factor * NMAD from the median
+        nmad = xdem.spatialstats.nmad(ddem.data[inlier_mask])
+        med = np.ma.median(ddem.data[inlier_mask])
+        inlier_mask = inlier_mask & (np.abs(ddem.data - med) < nmad_factor * nmad).filled(False)
+
+        # Exclude steep slopes for coreg
+        slope = xdem.terrain.slope(ref_dem)
+        inlier_mask[slope.data < slope_lim[0]] = False
+        inlier_mask[slope.data > slope_lim[1]] = False
+
+    return inlier_mask
+
+
+def dem_coregistration(
+    src_dem_path: str | RasterType,
+    ref_dem_path: str | RasterType,
+    out_dem_path: str | None = None,
+    coreg_method: Coreg | None = NuthKaab() + BiasCorr(),
+    grid: str = "ref",
+    resample: bool = False,
+    resampling: rio.warp.Resampling | None = rio.warp.Resampling.bilinear,
+    shp_list: list[str | gu.Vector] | tuple[str | gu.Vector] | tuple[()] = (),
+    inout: list[int] | tuple[int] | tuple[()] = (),
+    filtering: bool = True,
+    dh_max: AnyNumber = None,
+    nmad_factor: AnyNumber = 5,
+    slope_lim: list[AnyNumber] | tuple[AnyNumber, AnyNumber] = (0.1, 40),
+    plot: bool = False,
+    out_fig: str = None,
+    verbose: bool = False,
+) -> tuple[xdem.DEM, xdem.coreg.Coreg, pd.DataFrame, NDArrayf]:
+    """
+    A one-line function to coregister a selected DEM to a reference DEM.
+
+    Reads both DEMs, reprojects them on the same grid, mask pixels based on shapefile(s), filter steep slopes and \
+outliers, run the coregistration, returns the coregistered DEM and some statistics.
+    Optionally, save the coregistered DEM to file and make a figure.
+    For details on masking options, see `create_inlier_mask` function.
+
+    :param src_dem_path: Path to the input DEM to be coregistered
+    :param ref_dem_path: Path to the reference DEM
+    :param out_dem_path: Path where to save the coregistered DEM. If set to None (default), will not save to file.
+    :param coreg_method: The xdem coregistration method, or pipeline.
+    :param grid: The grid to be used during coregistration, set either to "ref" or "src".
+    :param resample: If set to True, will reproject output Raster on the same grid as input. Otherwise, only \
+the array/transform will be updated (if possible) and no resampling is done. Useful to avoid spreading data gaps.
+    :param resampling: The resampling algorithm to be used if `resample` is True. Default is bilinear.
+    :param shp_list: A list of one or several paths to shapefiles to use for masking.
+    :param inout: A list of same size as shp_list. For each shapefile, set to 1 (resp. -1) to specify whether \
+to mask inside (resp. outside) of the polygons. Defaults to masking inside polygons for all shapefiles.
+    :param filtering: If set to True, filtering will be applied prior to coregistration.
+    :param dh_max: Remove pixels where abs(src - ref) is more than this value.
+    :param nmad_factor: Remove pixels where abs(src - ref) differ by nmad_factor * NMAD from the median.
+    :param slope_lim: A list/tuple of min and max slope values, in degrees. Pixels outside this slope range will \
+be excluded.
+    :param plot: Set to True to plot a figure of elevation diff before/after coregistration.
+    :param out_fig: Path to the output figure. If None will display to screen.
+    :param verbose: Set to True to print details on screen during coregistration.
+
+    :returns: A tuple containing 1) coregistered DEM as an xdem.DEM instance 2) the coregistration method \
+3) DataFrame of coregistration statistics (count of obs, median and NMAD over stable terrain) before and after \
+coregistration and 4) the inlier_mask used.
+    """
+    # Check inputs
+    if not isinstance(coreg_method, xdem.coreg.Coreg):
+        raise ValueError("`coreg_method` must be an xdem.coreg instance (e.g. xdem.coreg.NuthKaab())")
+
+    if isinstance(ref_dem_path, str):
+        if not isinstance(src_dem_path, str):
+            raise ValueError(
+                f"`ref_dem_path` is string but `src_dem_path` has type {type(src_dem_path)}."
+                "Both must have same type."
+            )
+    elif isinstance(ref_dem_path, gu.Raster):
+        if not isinstance(src_dem_path, gu.Raster):
+            raise ValueError(
+                f"`ref_dem_path` is of Raster type but `src_dem_path` has type {type(src_dem_path)}."
+                "Both must have same type."
+            )
+    else:
+        raise ValueError("`ref_dem_path` must be either a string or a Raster")
+
+    if grid not in ["ref", "src"]:
+        raise ValueError(f"`grid` must be either 'ref' or 'src' - currently set to {grid}")
+
+    # Load both DEMs
+    if verbose:
+        print("Loading and reprojecting input data")
+
+    if isinstance(ref_dem_path, str):
+        if grid == "ref":
+            ref_dem, src_dem = gu.raster.load_multiple_rasters([ref_dem_path, src_dem_path], ref_grid=0)
+        elif grid == "src":
+            ref_dem, src_dem = gu.raster.load_multiple_rasters([ref_dem_path, src_dem_path], ref_grid=1)
+    else:
+        ref_dem = ref_dem_path
+        src_dem = src_dem_path
+        if grid == "ref":
+            src_dem = src_dem.reproject(ref_dem, silent=True)
+        elif grid == "src":
+            ref_dem = ref_dem.reproject(src_dem, silent=True)
+
+    # Convert to DEM instance with Float32 dtype
+    # TODO: Could only convert types int into float, but any other float dtype should yield very similar results
+    ref_dem = xdem.DEM(ref_dem.astype(np.float32))
+    src_dem = xdem.DEM(src_dem.astype(np.float32))
+
+    # Create raster mask
+    if verbose:
+        print("Creating mask of inlier pixels")
+
+    inlier_mask = create_inlier_mask(
+        src_dem,
+        ref_dem,
+        shp_list=shp_list,
+        inout=inout,
+        filtering=filtering,
+        dh_max=dh_max,
+        nmad_factor=nmad_factor,
+        slope_lim=slope_lim,
+    )
+
+    # Calculate dDEM
+    ddem = src_dem - ref_dem
+
+    # Calculate dDEM statistics on pixels used for coreg
+    inlier_data = ddem.data[inlier_mask].compressed()
+    nstable_orig, mean_orig = len(inlier_data), np.mean(inlier_data)
+    med_orig, nmad_orig = np.median(inlier_data), xdem.spatialstats.nmad(inlier_data)
+
+    # Coregister to reference - Note: this will spread NaN
+    coreg_method.fit(ref_dem, src_dem, inlier_mask, verbose=verbose)
+    dem_coreg = coreg_method.apply(src_dem, resample=resample, resampling=resampling)
+
+    # Calculate coregistered ddem (might need resampling if resample set to False), needed for stats and plot only
+    ddem_coreg = dem_coreg.reproject(ref_dem, silent=True) - ref_dem
+
+    # Calculate new stats
+    inlier_data = ddem_coreg.data[inlier_mask].compressed()
+    nstable_coreg, mean_coreg = len(inlier_data), np.mean(inlier_data)
+    med_coreg, nmad_coreg = np.median(inlier_data), xdem.spatialstats.nmad(inlier_data)
+
+    # Plot results
+    if plot:
+        # Max colorbar value - 98th percentile rounded to nearest 5
+        vmax = np.percentile(np.abs(ddem.data.compressed()), 98) // 5 * 5
+
+        plt.figure(figsize=(11, 5))
+
+        ax1 = plt.subplot(121)
+        plt.imshow(ddem.data.squeeze(), cmap="coolwarm_r", vmin=-vmax, vmax=vmax)
+        cb = plt.colorbar()
+        cb.set_label("Elevation change (m)")
+        ax1.set_title(f"Before coreg\n\nmean = {mean_orig:.1f} m - med = {med_orig:.1f} m - NMAD = {nmad_orig:.1f} m")
+
+        ax2 = plt.subplot(122, sharex=ax1, sharey=ax1)
+        plt.imshow(ddem_coreg.data.squeeze(), cmap="coolwarm_r", vmin=-vmax, vmax=vmax)
+        cb = plt.colorbar()
+        cb.set_label("Elevation change (m)")
+        ax2.set_title(
+            f"After coreg\n\n\nmean = {mean_coreg:.1f} m - med = {med_coreg:.1f} m - NMAD = {nmad_coreg:.1f} m"
+        )
+
+        plt.tight_layout()
+        if out_fig is None:
+            plt.show()
+        else:
+            plt.savefig(out_fig, dpi=200)
+            plt.close()
+
+    # Save coregistered DEM
+    if out_dem_path is not None:
+        dem_coreg.save(out_dem_path, tiled=True)
+
+    # Save stats to DataFrame
+    out_stats = pd.DataFrame(
+        ((nstable_orig, med_orig, nmad_orig, nstable_coreg, med_coreg, nmad_coreg),),
+        columns=("nstable_orig", "med_orig", "nmad_orig", "nstable_coreg", "med_coreg", "nmad_coreg"),
+    )
+
+    return dem_coreg, coreg_method, out_stats, inlier_mask
```

### Comparing `xdem-0.0.7/xdem/ddem.py` & `xdem-0.0.8/xdem/ddem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Difference of DEMs classes and functions."""
 from __future__ import annotations
 
-import copy
 import warnings
-from typing import Any, Optional, Union
+from typing import Any
 
 import geoutils as gu
-from geoutils import spatial_tools
 import numpy as np
 import shapely
+from geoutils.raster import RasterType, get_array_and_mask
+from rasterio.crs import CRS
+from rasterio.warp import Affine
 
 import xdem
+from xdem._typing import NDArrayf
 
 
-class dDEM(xdem.dem.DEM):   # pylint: disable=invalid-name
+class dDEM(xdem.dem.DEM):  # pylint: disable=invalid-name
     """A difference-DEM object."""
 
-    def __init__(self, raster: gu.Raster, start_time: np.datetime64, end_time: np.datetime64,
-                 error: Optional[Any] = None):
+    def __init__(self, raster: gu.Raster, start_time: np.datetime64, end_time: np.datetime64, error: Any | None = None):
         """
         Create a dDEM object from a Raster.
 
         :param raster: A georeferenced Raster object.
         :param start_time: The starting time of the dDEM.
         :param end_time: The end time of the dDEM.
         :param error: An error measure for the dDEM (UNUSED).
@@ -30,28 +31,33 @@
         """
         # super().__init__(raster)
 
         self.__dict__ = raster.__dict__
         self.start_time = start_time
         self.end_time = end_time
         self.error = error
-        self._filled_data: Optional[np.ndarray] = None
+        self._filled_data: NDArrayf | None = None
         self._fill_method = ""
+        self.nodata: int | float | None = None
 
     def __str__(self) -> str:
         """Return a summary of the dDEM."""
         return f"dDEM from {self.start_time} to {self.end_time}.\n\n{super().__str__()}"
 
-    def copy(self) -> dDEM:
+    def copy(self, new_array: NDArrayf = None) -> dDEM:
         """Return a copy of the DEM."""
-        new_ddem = dDEM.from_array(self.data.copy(), self.transform, self.crs, self.start_time, self.end_time)
+
+        if new_array is None:
+            new_array = self.data.copy()
+
+        new_ddem = dDEM.from_array(new_array, self.transform, self.crs, self.start_time, self.end_time)
         return new_ddem
 
     @property
-    def filled_data(self) -> Optional[np.ndarray]:
+    def filled_data(self) -> NDArrayf | None:
         """
         Get the filled data array if it exists, or else the original data if it has no nans.
 
         Returns None if the filled_data array does not exist, and the original data has nans.
 
         :returns: An array or None
         """
@@ -59,60 +65,70 @@
             return self._filled_data
         if (isinstance(self.data, np.ma.masked_array) and np.any(self.data.mask)) or np.any(np.isnan(self.data)):
             return None
 
         return np.asarray(self.data)
 
     @filled_data.setter
-    def filled_data(self, array: np.ndarray):
+    def filled_data(self, array: NDArrayf) -> None:
         """Set the filled_data attribute and make sure that it is valid."""
 
-        assert self.data.size == array.size, f"Array shape '{array.shape}' differs from the data shape '{self.data.shape}'"
+        assert (
+            self.data.size == array.size
+        ), f"Array shape '{array.shape}' differs from the data shape '{self.data.shape}'"
 
         self._filled_data = np.asarray(array).reshape(self.data.shape)
 
     @property
     def fill_method(self) -> str:
         """Return the fill method used for the filled_data."""
         return self._fill_method
 
     @property
     def time(self) -> np.timedelta64:
         """Get the time duration."""
         return self.end_time - self.start_time
 
-    def from_array(data: np.ndarray, transform, crs, start_time, end_time, error=None, nodata=None) -> dDEM:
+    @classmethod
+    def from_array(
+        cls: type[RasterType],
+        data: NDArrayf,
+        transform: tuple[float, ...] | Affine,
+        crs: CRS | int | None,
+        start_time: np.datetime64,
+        end_time: np.datetime64,
+        error: float = None,
+        nodata: int | float | None = None,
+    ) -> dDEM:
         """
         Create a new dDEM object from an array.
 
         :param data: The dDEM data array.
         :param transform: A geometric transform.
         :param crs: The coordinate reference system of the dDEM.
         :param start_time: The starting time of the dDEM.
         :param end_time: The end time of the dDEM.
         :param error: An error measure for the dDEM.
         :param nodata: The nodata value.
 
         :returns: A new dDEM instance.
         """
         return dDEM(
-            gu.georaster.Raster.from_array(
-                data=data,
-                transform=transform,
-                crs=crs,
-                nodata=nodata
-            ),
+            gu.Raster.from_array(data=data, transform=transform, crs=crs, nodata=nodata),
             start_time=start_time,
             end_time=end_time,
             error=error,
         )
 
-    def interpolate(self, method: str = "linear",
-                    reference_elevation: Optional[Union[np.ndarray, np.ma.masked_array, xdem.DEM]] = None,
-                    mask: Optional[Union[np.ndarray, xdem.DEM, gu.Vector]] = None):
+    def interpolate(
+        self,
+        method: str = "linear",
+        reference_elevation: NDArrayf | np.ma.masked_array[Any, np.dtype[np.floating[Any]]] | xdem.DEM = None,
+        mask: NDArrayf | xdem.DEM | gu.Vector = None,
+    ) -> NDArrayf | None:
         """
         Interpolate the dDEM using the given method.
 
         :param method: The method to use for interpolation.
         :param reference_elevation: Reference DEM. Only required for hypsometric approaches.
         """
         if reference_elevation is not None:
@@ -135,31 +151,31 @@
         elif method == "local_hypsometric":
             assert reference_elevation is not None
             assert mask is not None
 
             if not isinstance(mask, gu.Vector):
                 mask = gu.Vector(mask)
 
-            interpolated_ddem, nans = spatial_tools.get_array_and_mask(self.data.copy())
+            interpolated_ddem, nans = get_array_and_mask(self.data.copy())
             entries = mask.ds[mask.ds.intersects(shapely.geometry.box(*self.bounds))]
 
             ddem_mask = nans.copy().squeeze()
             for i in entries.index:
-                feature_mask = (gu.Vector(entries.loc[entries.index == i]).create_mask(
-                    self)).reshape(interpolated_ddem.shape)
+                feature_mask = (gu.Vector(entries.loc[entries.index == i]).create_mask(self, as_array=True)).reshape(
+                    interpolated_ddem.shape
+                )
                 if np.count_nonzero(feature_mask) == 0:
                     continue
                 try:
                     with warnings.catch_warnings():
                         warnings.filterwarnings("ignore", "Not enough valid bins")
+                        warnings.filterwarnings("ignore", "invalid value encountered in divide")
                         interpolated_ddem = np.asarray(
                             xdem.volume.hypsometric_interpolation(
-                                interpolated_ddem,
-                                reference_elevation.data,
-                                mask=feature_mask
+                                interpolated_ddem, reference_elevation.data, mask=feature_mask
                             )
                         )
                 except ValueError as exception:
                     # Skip the feature if too few glacier values exist.
                     if "x and y arrays must have at least 2 entries" in str(exception):
                         continue
                     raise exception
@@ -178,16 +194,14 @@
         elif method == "regional_hypsometric":
             assert reference_elevation is not None
             assert mask is not None
 
             mask_array = xdem.coreg.mask_as_array(self, mask).reshape(self.data.shape)
 
             self.filled_data = xdem.volume.hypsometric_interpolation(
-                self.data,
-                reference_elevation.data,
-                mask=mask_array
+                self.data, reference_elevation.data, mask=mask_array
             ).data
 
         else:
             raise NotImplementedError(f"Interpolation method '{method}' not supported")
 
         return self.filled_data
```

### Comparing `xdem-0.0.7/xdem/dem.py` & `xdem-0.0.8/xdem/dem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,241 +1,255 @@
 """DEM class and functions."""
 from __future__ import annotations
 
+import json
 import os
-import pyproj
+import subprocess
 import warnings
-from geoutils.georaster import Raster
-from geoutils.satimg import SatelliteImage
-import geoutils as gu
-import numpy as np
+from typing import Any
+
+import pyproj
+import rasterio as rio
+from geoutils import SatelliteImage
+from geoutils.raster import RasterType
 from pyproj import Transformer
-import json
-import subprocess
 
-def parse_vref_from_product(product: str) -> str:
+from xdem._typing import NDArrayf
+
+
+def parse_vref_from_product(product: str) -> str | None:
     """
 
     :param product: Product name (typically from satimg.parse_metadata_from_fn)
 
     :return: vref_name: Vertical reference name
     """
     # Sources for defining vertical references:
     # AW3D30: https://www.eorc.jaxa.jp/ALOS/en/aw3d30/aw3d30v11_format_e.pdf
     # SRTMGL1: https://lpdaac.usgs.gov/documents/179/SRTM_User_Guide_V3.pdf
     # SRTMv4.1: http://www.cgiar-csi.org/data/srtm-90m-digital-elevation-database-v4-1
     # ASTGTM2/ASTGTM3: https://lpdaac.usgs.gov/documents/434/ASTGTM_User_Guide_V3.pdf
-    # NASADEM: https://lpdaac.usgs.gov/documents/592/NASADEM_User_Guide_V1.pdf !! HGTS is ellipsoid, HGT is EGM96 geoid !!
+    # NASADEM: https://lpdaac.usgs.gov/documents/592/NASADEM_User_Guide_V1.pdf, HGTS is ellipsoid, HGT is EGM96 geoid !!
     # ArcticDEM (mosaic and strips): https://www.pgc.umn.edu/data/arcticdem/
     # REMA (mosaic and strips): https://www.pgc.umn.edu/data/rema/
     # TanDEM-X 90m global: https://geoservice.dlr.de/web/dataguide/tdm90/
     # COPERNICUS DEM: https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198
 
-    if product in ['ArcticDEM/REMA','TDM1','NASADEM-HGTS']:
-        vref_name = 'WGS84'
-    elif product in ['AW3D30','SRTMv4.1','SRTMGL1','ASTGTM2','NASADEM-HGT']:
-        vref_name = 'EGM96'
-    elif product in ['COPDEM']:
-        vref_name = 'EGM08'
+    if product in ["ArcticDEM/REMA", "TDM1", "NASADEM-HGTS"]:
+        vref_name = "WGS84"
+    elif product in ["AW3D30", "SRTMv4.1", "SRTMGL1", "ASTGTM2", "NASADEM-HGT"]:
+        vref_name = "EGM96"
+    elif product in ["COPDEM"]:
+        vref_name = "EGM08"
     else:
         vref_name = None
 
     return vref_name
 
 
-dem_attrs = ['vref','vref_grid','_ccrs']
+dem_attrs = ["vref", "vref_grid", "_ccrs"]
 
-class DEM(SatelliteImage):
 
-    def __init__(self, filename_or_dataset, vref_name=None, vref_grid=None, silent=True, **kwargs):
+class DEM(SatelliteImage):  # type: ignore
+    def __init__(
+        self,
+        filename_or_dataset: str | RasterType | rio.io.DatasetReader | rio.io.MemoryFile,
+        vref_name: str | None = None,
+        vref_grid: str | None = None,
+        silent: bool = True,
+        **kwargs: Any,
+    ) -> None:
         """
-        Load digital elevation model data through the Raster class, parse additional attributes from filename or metadata
-        trougth the SatelliteImage class, and then parse vertical reference from DEM product name.
+        Load digital elevation model data through the Raster class, parse additional attributes from filename or
+        metadata through the SatelliteImage class, and then parse vertical reference from DEM product name.
         For manual input, only one of "vref", "vref_grid" or "ccrs" is necessary to set the vertical reference.
 
         :param filename_or_dataset: The filename of the dataset.
-        :type filename_or_dataset: str, DEM, SatelliteImage, Raster, rio.io.Dataset, rio.io.MemoryFile
         :param vref_name: Vertical reference name
-        :type vref_name: str
         :param vref_grid: Vertical reference grid (any grid file in https://github.com/OSGeo/PROJ-data)
-        :type vref_grid: str
         :param silent: Whether to display vertical reference setting
         :param silent: boolean
         """
 
+        self.data: NDArrayf
+
         # If DEM is passed, simply point back to DEM
         if isinstance(filename_or_dataset, DEM):
             for key in filename_or_dataset.__dict__:
                 setattr(self, key, filename_or_dataset.__dict__[key])
             return
         # Else rely on parent SatelliteImage class options (including raised errors)
         else:
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", message="Parse metadata from file not implemented")
                 super().__init__(filename_or_dataset, silent=silent, **kwargs)
 
-        # self.nbands can be None when data is not loaded through the Raster class
-        if self.nbands is not None and self.nbands > 1:
-            raise ValueError('DEM rasters should be composed of one band only')
+        # self.indexes can be None when data is not loaded through the Raster class
+        if self.indexes is not None and len(self.indexes) > 1:
+            raise ValueError("DEM rasters should be composed of one band only")
 
         # user input
         self.vref = vref_name
         self.vref_grid = vref_grid
         self._ccrs = None
 
         # trying to get vref from product name (priority to user input)
         self.__parse_vref_from_fn(silent=silent)
 
-    def copy(self, new_array: np.ndarray | None = None) -> DEM:
+    def copy(self, new_array: NDArrayf | None = None) -> DEM:
 
-        new_dem = super().copy(new_array=new_array) # type: ignore
+        new_dem = super().copy(new_array=new_array)  # type: ignore
         # The rest of attributes are immutable, including pyproj.CRS
         # dem_attrs = ['vref','vref_grid','ccrs'] #taken outside of class
         for attrs in dem_attrs:
             setattr(new_dem, attrs, getattr(self, attrs))
 
-        return new_dem
+        return new_dem  # type: ignore
 
-    def __parse_vref_from_fn(self, silent: bool = False):
+    def __parse_vref_from_fn(self, silent: bool = False) -> None:
         """Attempts to pull vertical reference from product name identified by SatImg."""
 
         if self.product is not None:
             vref = parse_vref_from_product(self.product)
             if vref is not None and self.vref is None:
                 if not silent:
-                    print('From product name "'+ str(self.product)+'": setting vertical reference as ' + str(vref))
+                    print('From product name "' + str(self.product) + '": setting vertical reference as ' + str(vref))
                 self.vref = vref
             elif vref is not None and self.vref is not None:
                 if not silent:
-                    print('Leaving user input of ' + str(self.vref) + ' for vertical reference despite reading ' + str(
-                        vref) + ' from product name')
+                    print(
+                        "Leaving user input of "
+                        + str(self.vref)
+                        + " for vertical reference despite reading "
+                        + str(vref)
+                        + " from product name"
+                    )
             else:
                 if not silent:
-                    print('Could not find a vertical reference based on product name: "'+str(self.product)+'"')
+                    print('Could not find a vertical reference based on product name: "' + str(self.product) + '"')
 
     @property
-    def ccrs(self):
+    def ccrs(self) -> pyproj.CRS:
         """Set compound CRS, i.e. horizontal and vertical references"""
 
         # Temporary fix for some CRS with proj < 7.2
         def get_crs(filepath: str) -> pyproj.CRS:
             """Get the CRS of a raster with the given filepath."""
             info = subprocess.run(
-                ["gdalinfo", "-json", filepath],
-                stdout=subprocess.PIPE,
-                check=True,
-                encoding="utf-8"
+                ["gdalinfo", "-json", filepath], stdout=subprocess.PIPE, check=True, encoding="utf-8"
             ).stdout
 
             wkt_string = json.loads(info)["coordinateSystem"]["wkt"]
 
             return pyproj.CRS.from_wkt(wkt_string)
 
         # Temporary fix to get all types of CRS
         if pyproj.proj_version_str >= "7.2.0":
             crs = self.crs
         else:
             crs = get_crs(self.filename)
 
-        if self.vref == 'WGS84':
+        if self.vref == "WGS84":
             # The WGS84 ellipsoid corresponds to no vertical reference in pyproj
             self._ccrs = pyproj.CRS(crs)
         elif self.vref_grid is not None:
             # For other vrefs, keep same horizontal projection and add geoid grid (the "dirty" way: because init is so
             # practical and still going to be used for a while)
-            # see https://gis.stackexchange.com/questions/352277/including-geoidgrids-when-initializing-projection-via-epsg/352300#352300
+            # see https://gis.stackexchange.com/questions/352277/
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", module="pyproj")
                 self._ccrs = pyproj.Proj(init="EPSG:" + str(int(crs.to_epsg())), geoidgrids=self.vref_grid).crs
         else:
             self._ccrs = None
 
         return self._ccrs
 
-
-    def set_vref(self, vref_name: str | None = None, vref_grid: str | None = None):
+    def set_vref(self, vref_name: str | None = None, vref_grid: str | None = None) -> None:
         """
         Set vertical reference with a name or with a grid.
 
         :param vref_name: Vertical reference name
         :param vref_grid: Vertical reference grid (any grid file in https://github.com/OSGeo/PROJ-data)
 
         :return:
         """
 
         # Using vref_name only for WGS84 ellipsoid or the EGM96/EGM08 geoids (used 99% of the time)
         if isinstance(vref_grid, str):
 
             # Default behaviour: use grid if both name and grid are provided
             if isinstance(vref_name, str):
-                print('Both a vertical reference name and vertical grid are provided: defaulting to using grid only.')
+                print("Both a vertical reference name and vertical grid are provided: defaulting to using grid only.")
 
-            if vref_grid == 'us_nga_egm08_25.tif':
-                self.vref = 'EGM08'
+            if vref_grid == "us_nga_egm08_25.tif":
+                self.vref = "EGM08"
                 self.vref_grid = vref_grid
-            elif vref_grid == 'us_nga_egm96_15.tif':
-                self.vref = 'EGM96'
+            elif vref_grid == "us_nga_egm96_15.tif":
+                self.vref = "EGM96"
                 self.vref_grid = vref_grid
             else:
-                if os.path.exists(os.path.join(pyproj.datadir.get_data_dir(),vref_grid)):
-                    self.vref = 'Unknown vertical reference name from: '+vref_grid
+                if os.path.exists(os.path.join(pyproj.datadir.get_data_dir(), vref_grid)):
+                    self.vref = "Unknown vertical reference name from: " + vref_grid
                     self.vref_grid = vref_grid
                 else:
-                    raise ValueError('Grid not found in '+str(pyproj.datadir.get_data_dir())+': check if proj-data is '
-                         'installed via conda-forge, the pyproj.datadir, and that you are using a grid available at '
-                         'https://github.com/OSGeo/PROJ-data')
+                    raise ValueError(
+                        "Grid not found in " + str(pyproj.datadir.get_data_dir()) + ": check if proj-data is "
+                        "installed via conda-forge, the pyproj.datadir, and that you are using a grid available at "
+                        "https://github.com/OSGeo/PROJ-data"
+                    )
 
         # Otherwise, use name provided
-        elif isinstance(vref_name,str):
-            if vref_name == 'WGS84':
+        elif isinstance(vref_name, str):
+            if vref_name == "WGS84":
                 self.vref_grid = None
-                self.vref = 'WGS84'  # WGS84 ellipsoid
-            elif vref_name == 'EGM08':
-                self.vref_grid = 'us_nga_egm08_25.tif'  # EGM2008 at 2.5 minute resolution
-                self.vref = 'EGM08'
-            elif vref_name == 'EGM96':
-                self.vref_grid = 'us_nga_egm96_15.tif'  # EGM1996 at 15 minute resolution
-                self.vref = 'EGM96'
+                self.vref = "WGS84"  # WGS84 ellipsoid
+            elif vref_name == "EGM08":
+                self.vref_grid = "us_nga_egm08_25.tif"  # EGM2008 at 2.5 minute resolution
+                self.vref = "EGM08"
+            elif vref_name == "EGM96":
+                self.vref_grid = "us_nga_egm96_15.tif"  # EGM1996 at 15 minute resolution
+                self.vref = "EGM96"
             else:
                 raise ValueError(
                     'Vertical reference name must be either "WGS84", "EGM96" or "EGM08". Otherwise, provide'
-                    ' a geoid grid from PROJ DATA: https://github.com/OSGeo/PROJ-data')
+                    " a geoid grid from PROJ DATA: https://github.com/OSGeo/PROJ-data"
+                )
 
         # Else, return an error
         else:
-            raise ValueError('Vertical reference name or vertical grid must be a string')
-
+            raise ValueError("Vertical reference name or vertical grid must be a string")
 
-    def to_vref(self, vref_name: str = 'EGM96', vref_grid: str | None = None):
+    def to_vref(self, vref_name: str = "EGM96", vref_grid: str | None = None) -> None:
 
         """
         Convert between vertical references: ellipsoidal heights or geoid grids.
 
         :param vref_name: Vertical reference name
         :param vref_grid: Vertical reference grid (any grid file in https://github.com/OSGeo/PROJ-data)
 
         :return:
         """
 
         # All transformations grids file are described here: https://github.com/OSGeo/PROJ-data
         if self.vref is None and self.vref_grid is None:
-            raise ValueError('The current DEM has not vertical reference: need to set one before attempting a conversion '
-                             'towards another vertical reference.')
+            raise ValueError(
+                "The current DEM has not vertical reference: need to set one before attempting a conversion "
+                "towards another vertical reference."
+            )
 
-        # Inital ccrs
+        # Initial ccrs
         ccrs_init = self.ccrs
 
         # Destination crs: first, set the new reference (before calculation doesn't change anything,
         # we need to update the data manually anyway)
         self.set_vref(vref_name=vref_name, vref_grid=vref_grid)
         ccrs_dest = self.ccrs
 
         # Transform the grid
         transformer = Transformer.from_crs(ccrs_init, ccrs_dest)
-        meta = self.ds.meta
         zz = self.data
-        xx, yy = self.coords(offset='center')
-        zz_trans = transformer.transform(xx,yy,zz[0,:])[2]
-        zz[0,:] = zz_trans
+        xx, yy = self.coords(offset="center")
+        zz_trans = transformer.transform(xx, yy, zz[0, :])[2]
+        zz[0, :] = zz_trans
 
         # Update raster
-        self._update(metadata=meta,imgdata=zz)
+        self.data = zz
```

### Comparing `xdem-0.0.7/xdem/demcollection.py` & `xdem-0.0.8/xdem/demcollection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 """DEM collection class and functions."""
 from __future__ import annotations
 
 import datetime
 import warnings
-from typing import Optional, Union
 
 import geoutils as gu
 import numpy as np
 import pandas as pd
 
 import xdem
+from xdem._typing import NDArrayf
 
 
 class DEMCollection:
     """A temporal collection of DEMs."""
 
-    def __init__(self, dems: Union[list[gu.georaster.Raster], list[xdem.DEM]],
-                 timestamps: Optional[list[datetime.datetime]] = None,
-                 outlines: Optional[Union[gu.geovector.Vector, dict[datetime.datetime, gu.geovector.Vector]]] = None,
-                 reference_dem: Union[int, gu.georaster.Raster] = 0):
+    def __init__(
+        self,
+        dems: list[gu.Raster] | list[xdem.DEM],
+        timestamps: list[datetime.datetime] | None = None,
+        outlines: gu.Vector | dict[datetime.datetime, gu.Vector] | None = None,
+        reference_dem: int | gu.Raster = 0,
+    ):
         """
         Create a new temporal DEM collection.
 
         :param dems: A list of DEMs.
         :param timestamps: A list of DEM timestamps.
         :param outlines: Polygons to separate the changing area of interest. Could for example be glacier outlines.
         :param reference_dem: An instance or index of which DEM in the 'dems' list is the reference.
 
         :returns: A new DEMCollection instance.
         """
         # If timestamps is not given, try to parse it from the (potential) 'datetime' attribute of each DEM.
         if timestamps is None:
             timestamp_attributes = [dem.datetime for dem in dems]
-            if any([stamp is None for stamp in timestamp_attributes]):
+            if any(stamp is None for stamp in timestamp_attributes):
                 raise ValueError("'timestamps' not provided and the given DEMs do not all have datetime attributes")
 
             timestamps = timestamp_attributes
 
         if not all(isinstance(dem, xdem.DEM) for dem in dems):
             dems = [xdem.DEM.from_array(dem.data, dem.transform, dem.crs, dem.nodata) for dem in dems]
 
         assert len(dems) == len(timestamps), "The 'dem' and 'timestamps' len differ."
 
         # Convert the timestamps to datetime64
         self.timestamps = np.array(timestamps).astype("datetime64[ns]")
 
         # Find the sort indices from the timestamps
         indices = np.argsort(self.timestamps.astype("int64"))
-        self.dems = np.empty(len(dems), dtype=object)
-        self.dems[:] = [dems[i] for i in indices]
+        self.dems = [dems[i] for i in indices]
         self.ddems: list[xdem.dDEM] = []
         # The reference index changes place when sorted
         if isinstance(reference_dem, (int, np.integer)):
             self.reference_index = np.argwhere(indices == reference_dem)[0][0]
-        elif isinstance(reference_dem, gu.georaster.Raster):
+        elif isinstance(reference_dem, gu.Raster):
             self.reference_index = [i for i, dem in enumerate(self.dems) if dem is reference_dem][0]
 
         if outlines is None:
-            self.outlines: dict[np.datetime64, gu.geovector.Vector] = {}
-        elif isinstance(outlines, gu.geovector.Vector):
+            self.outlines: dict[np.datetime64, gu.Vector] = {}
+        elif isinstance(outlines, gu.Vector):
             self.outlines = {self.timestamps[self.reference_index]: outlines}
-        elif all(isinstance(value, gu.geovector.Vector) for value in outlines.values()):
+        elif all(isinstance(value, gu.Vector) for value in outlines.values()):
             self.outlines = dict(zip(np.array(list(outlines.keys())).astype("datetime64[ns]"), outlines.values()))
         else:
-            raise ValueError(f"Invalid format on 'outlines': {type(outlines)},"
-                             " expected one of ['gu.geovector.Vector', 'dict[datetime.datetime, gu.geovector.Vector']")
+            raise ValueError(
+                f"Invalid format on 'outlines': {type(outlines)},"
+                " expected one of ['gu.Vector', 'dict[datetime.datetime, gu.Vector']"
+            )
 
     @property
-    def reference_dem(self) -> gu.georaster.Raster:
+    def reference_dem(self) -> gu.Raster:
         """Get the DEM acting reference."""
         return self.dems[self.reference_index]
 
     @property
     def reference_timestamp(self) -> np.datetime64:
         """Get the reference DEM timestamp."""
         return self.timestamps[self.reference_index]
@@ -85,48 +89,48 @@
         :returns: A list of dDEM objects.
         """
         ddems: list[xdem.dDEM] = []
 
         # Subtract every DEM that is available.
         for i, dem in enumerate(self.dems):
             # If the reference DEM is encountered, make a dDEM where dH == 0 (to keep length consistency).
-            if dem == self.reference_dem:
+            if dem.raster_equal(self.reference_dem):
                 ddem_raster = self.reference_dem.copy()
                 ddem_raster.data[:] = 0.0
                 ddem = xdem.dDEM(
                     ddem_raster,
                     start_time=self.reference_timestamp,
                     end_time=self.reference_timestamp,
                     error=0,
                 )
             else:
                 ddem = xdem.dDEM(
                     self.reference_dem - dem.reproject(resampling=resampling_method, silent=True),
                     start_time=min(self.reference_timestamp, self.timestamps[i]),
                     end_time=max(self.reference_timestamp, self.timestamps[i]),
-                    error=None
+                    error=None,
                 )
             ddems.append(ddem)
 
         self.ddems = ddems
         return self.ddems
 
-    def interpolate_ddems(self, method="linear"):
+    def interpolate_ddems(self, method: str = "linear") -> list[NDArrayf]:
         """
         Interpolate all the dDEMs in the DEMCollection object using the chosen interpolation method.
 
         :param method: The chosen interpolation method.
         """
         # TODO: Change is loop to run concurrently
         for ddem in self.ddems:
             ddem.interpolate(method=method, reference_elevation=self.reference_dem, mask=self.get_ddem_mask(ddem))
 
         return [ddem.filled_data for ddem in self.ddems]
 
-    def get_ddem_mask(self, ddem: xdem.dDEM, outlines_filter: Optional[str] = None) -> np.ndarray:
+    def get_ddem_mask(self, ddem: xdem.dDEM, outlines_filter: str | None = None) -> NDArrayf:
         """
         Get a fitting dDEM mask for a provided dDEM.
 
         The mask is created by evaluating these factors, in order:
 
         If self.outlines do not exist, a full True boolean mask is returned.
         If self.outlines have keys for the start and end time, their union is returned.
@@ -147,45 +151,46 @@
             outlines = {key: gu.Vector(outline.ds.copy()) for key, outline in self.outlines.items()}
             for key in outlines:
                 outlines[key].ds = outlines[key].ds.query(outlines_filter)
 
         # If both the start and end time outlines exist, a mask is created from their union.
         if ddem.start_time in outlines and ddem.end_time in outlines:
             mask = np.logical_or(
-                outlines[ddem.start_time].create_mask(ddem),
-                outlines[ddem.end_time].create_mask(ddem)
+                outlines[ddem.start_time].create_mask(ddem, as_array=True),
+                outlines[ddem.end_time].create_mask(ddem, as_array=True),
             )
         # If only start time outlines exist, these should be used as a mask
         elif ddem.start_time in outlines:
-            mask = outlines[ddem.start_time].create_mask(ddem)
+            mask = outlines[ddem.start_time].create_mask(ddem, as_array=True)
         # If only one outlines file exist, use that as a mask.
         elif len(outlines) == 1:
-            mask = list(outlines.values())[0].create_mask(ddem)
+            mask = list(outlines.values())[0].create_mask(ddem, as_array=True)
         # If no fitting outlines were found, make a full true boolean mask in its stead.
         else:
             mask = np.ones(shape=ddem.data.shape, dtype=bool)
         return mask.reshape(ddem.data.shape)
 
-    def get_dh_series(self, outlines_filter: Optional[str] = None, mask: Optional[np.ndarray] = None,
-                      nans_ok: bool = False) -> pd.DataFrame:
+    def get_dh_series(
+        self, outlines_filter: str | None = None, mask: NDArrayf | None = None, nans_ok: bool = False
+    ) -> pd.DataFrame:
         """
         Return a dataframe of mean dDEM values and respective areas for every timestamp.
 
         The values are always compared to the reference DEM timestamp.
 
         :param mask: Optional. A mask for areas of interest. Overrides potential outlines of the same date.
         :param nans_ok: Warn if NaNs are encountered in a dDEM (it should have been gap-filled).
 
         :returns: A dataframe of dH values and respective areas with an Interval[Timestamp] index.
         """
         if len(self.ddems) == 0:
             raise ValueError("dDEMs have not yet been calculated")
 
         dh_values = pd.DataFrame(columns=["dh", "area"], dtype=float)
-        for i, ddem in enumerate(self.ddems):
+        for _, ddem in enumerate(self.ddems):
             # Skip if the dDEM is a self-comparison
             if float(ddem.time) == 0:
                 continue
 
             # Use the provided mask unless it's None, otherwise make a dDEM mask.
             ddem_mask = mask if mask is not None else self.get_ddem_mask(ddem, outlines_filter=outlines_filter)
 
@@ -198,16 +203,17 @@
             mean_dh = np.nanmean(data)
             area = np.count_nonzero(ddem_mask) * self.reference_dem.res[0] * self.reference_dem.res[1]
 
             dh_values.loc[pd.Interval(pd.Timestamp(ddem.start_time), pd.Timestamp(ddem.end_time))] = mean_dh, area
 
         return dh_values
 
-    def get_dv_series(self, outlines_filter: Optional[str] = None,
-                      mask: Optional[np.ndarray] = None, nans_ok: bool = False) -> pd.Series:
+    def get_dv_series(
+        self, outlines_filter: str | None = None, mask: NDArrayf | None = None, nans_ok: bool = False
+    ) -> pd.Series:
         """
         Return a series of mean volume change (dV) for every timestamp.
 
         The values are always compared to the reference DEM timestamp.
 
         :param outlines_filter: A query to filter the outline vectors. Example: "name_column == 'specific glacier'".
         :param mask: Optional. A mask for areas of interest. Overrides potential outlines of the same date.
@@ -215,17 +221,21 @@
 
         :returns: A series of dV values with an Interval[Timestamp] index.
         """
         dh_values = self.get_dh_series(outlines_filter=outlines_filter, mask=mask, nans_ok=nans_ok)
 
         return dh_values["area"] * dh_values["dh"]
 
-    def get_cumulative_series(self, kind: str = "dh", outlines_filter: Optional[str] = None,
-                              mask: Optional[np.ndarray] = None,
-                              nans_ok: bool = False) -> pd.Series:
+    def get_cumulative_series(
+        self,
+        kind: str = "dh",
+        outlines_filter: str | None = None,
+        mask: NDArrayf | None = None,
+        nans_ok: bool = False,
+    ) -> pd.Series:
         """
         Get the cumulative dH (elevation) or dV (volume) since the first timestamp.
 
         :param kind: The kind of series. Can be dh or dv.
         :param outlines_filter: A query to filter the outline vectors. Example: "name_column == 'specific glacier'".
         :param mask: Optional. A mask for areas of interest.
         :param nans_ok: Warn if NaNs are encountered in a dDEM (it should have been gap-filled).
@@ -237,15 +247,15 @@
             d_series = self.get_dh_series(mask=mask, outlines_filter=outlines_filter, nans_ok=nans_ok)["dh"]
         elif kind.lower() == "dv":
             # Get the dV series (where all indices are: "year to reference_year")
             d_series = self.get_dv_series(mask=mask, outlines_filter=outlines_filter, nans_ok=nans_ok)
         else:
             raise ValueError("Invalid argument: '{dh=}'. Choices: ['dh', 'dv']")
 
-        # Simplify the index to just "year" (implictly still the same as above)
+        # Simplify the index to just "year" (implicitly still the same as above)
         cumulative_dh = pd.Series(dtype=d_series.dtype)
         cumulative_dh[self.reference_timestamp] = 0.0
         for i, value in zip(d_series.index, d_series.values):
             non_reference_year = [date for date in [i.left, i.right] if date != self.reference_timestamp][0]
             cumulative_dh.loc[non_reference_year] = -value
 
         # Sort the dates (just to be sure. It should already be sorted)
```

### Comparing `xdem-0.0.7/xdem/examples.py` & `xdem-0.0.8/xdem/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 """Utility functions to download and find example data."""
-import errno
 import os
-import shutil
 import tarfile
 import tempfile
 import urllib.request
 from distutils.dir_util import copy_tree
 
-import numpy as np
-
 import geoutils as gu
+
 import xdem
 
-EXAMPLES_DIRECTORY = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "examples/data"))
+_EXAMPLES_DIRECTORY = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "examples", "data"))
 # Absolute filepaths to the example files.
-FILEPATHS_DATA = {
-    "longyearbyen_ref_dem": os.path.join(EXAMPLES_DIRECTORY, "Longyearbyen","data","DEM_2009_ref.tif"),
-    "longyearbyen_tba_dem": os.path.join(EXAMPLES_DIRECTORY, "Longyearbyen","data","DEM_1990.tif"),
+_FILEPATHS_DATA = {
+    "longyearbyen_ref_dem": os.path.join(_EXAMPLES_DIRECTORY, "Longyearbyen", "data", "DEM_2009_ref.tif"),
+    "longyearbyen_tba_dem": os.path.join(_EXAMPLES_DIRECTORY, "Longyearbyen", "data", "DEM_1990.tif"),
     "longyearbyen_glacier_outlines": os.path.join(
-        EXAMPLES_DIRECTORY,
-        "Longyearbyen","data","glacier_mask","CryoClim_GAO_SJ_1990.shp"
+        _EXAMPLES_DIRECTORY, "Longyearbyen", "data", "glacier_mask", "CryoClim_GAO_SJ_1990.shp"
     ),
     "longyearbyen_glacier_outlines_2010": os.path.join(
-        EXAMPLES_DIRECTORY,
-        "Longyearbyen","data","glacier_mask","CryoClim_GAO_SJ_2010.shp"
-    )}
-
-FILEPATHS_PROCESSED = {
-    "longyearbyen_ddem": os.path.join(EXAMPLES_DIRECTORY, "Longyearbyen","processed","dDEM_2009_minus_1990.tif"),
-    "longyearbyen_tba_dem_coreg": os.path.join(EXAMPLES_DIRECTORY, "Longyearbyen", "processed", "DEM_1990_coreg.tif")
+        _EXAMPLES_DIRECTORY, "Longyearbyen", "data", "glacier_mask", "CryoClim_GAO_SJ_2010.shp"
+    ),
 }
 
+_FILEPATHS_PROCESSED = {
+    "longyearbyen_ddem": os.path.join(_EXAMPLES_DIRECTORY, "Longyearbyen", "processed", "dDEM_2009_minus_1990.tif"),
+    "longyearbyen_tba_dem_coreg": os.path.join(_EXAMPLES_DIRECTORY, "Longyearbyen", "processed", "DEM_1990_coreg.tif"),
+}
 
-def download_longyearbyen_examples(overwrite: bool = False):
+available = list(_FILEPATHS_DATA.keys()) + list(_FILEPATHS_PROCESSED.keys())
+
+
+def download_longyearbyen_examples(overwrite: bool = False) -> None:
     """
     Fetch the Longyearbyen example files.
 
     :param overwrite: Do not download the files again if they already exist.
     """
-    if not overwrite and all(map(os.path.isfile, list(FILEPATHS_DATA.values()))):
+    if not overwrite and all(map(os.path.isfile, list(_FILEPATHS_DATA.values()))):
         # print("Datasets exist")
         return
 
+    # If we ask for overwrite, also remove the processed test data
+    if overwrite:
+        for fn in list(_FILEPATHS_PROCESSED.values()):
+            if os.path.exists(fn):
+                os.remove(fn)
+
     # Static commit hash to be bumped every time it needs to be.
-    commit = "321f84d5a67666f45a196a31a2697e22bfaf3c59"
+    commit = "fd832bc2e366cf2ba8b543f7e43f90ee02384f4f"
     # The URL from which to download the repository
     url = f"https://github.com/GlacioHack/xdem-data/tarball/main#commit={commit}"
 
     # Create a temporary directory to extract the tarball in.
     temp_dir = tempfile.TemporaryDirectory()
     tar_path = os.path.join(temp_dir.name, "data.tar.gz")
 
@@ -63,75 +67,76 @@
     with tarfile.open(tar_path) as tar:
         tar.extractall(temp_dir.name)
 
     # Find the first directory in the temp_dir (should only be one) and construct the Longyearbyen data dir path.
     dir_name = os.path.join(
         temp_dir.name,
         [dirname for dirname in os.listdir(temp_dir.name) if os.path.isdir(os.path.join(temp_dir.name, dirname))][0],
-        "data","Longyearbyen"
+        "data",
+        "Longyearbyen",
     )
 
     # Copy the data to the examples directory.
-    copy_tree(dir_name, os.path.join(EXAMPLES_DIRECTORY, "Longyearbyen","data"))
+    copy_tree(dir_name, os.path.join(_EXAMPLES_DIRECTORY, "Longyearbyen", "data"))
 
-def process_coregistered_examples(overwrite: bool =False):
+
+def process_coregistered_examples(name: str, overwrite: bool = False) -> None:
     """
-       Process the Longyearbyen example files into a dDEM (to avoid repeating this in many test/documentation steps).
+    Process the Longyearbyen example files into a dDEM (to avoid repeating this in many test/documentation steps).
 
-       :param overwrite: Do not download the files again if they already exist.
-       """
+    :param name: Name of test data
+    :param overwrite: Do not download the files again if they already exist.
+    """
 
-    if not overwrite and all(map(os.path.isfile, list(FILEPATHS_PROCESSED.values()))):
-        # print("Processed data exists")
+    # If the file called already exists and overwrite is False, do nothing
+    if not overwrite and os.path.isfile(_FILEPATHS_PROCESSED[name]):
         return
 
+    # Check that data is downloaded before attempting processing
     download_longyearbyen_examples(overwrite=False)
 
-    # Run the coregistration if it hasn't been made yet.
-    reference_raster = gu.georaster.Raster(FILEPATHS_DATA["longyearbyen_ref_dem"])
-    to_be_aligned_raster = gu.georaster.Raster(FILEPATHS_DATA["longyearbyen_tba_dem"])
-    glacier_mask = gu.geovector.Vector(FILEPATHS_DATA["longyearbyen_glacier_outlines"])
-    inlier_mask = ~glacier_mask.create_mask(reference_raster)
-
-    nuth_kaab = xdem.coreg.NuthKaab()
-    nuth_kaab.fit(reference_raster.data, to_be_aligned_raster.data,
-                  inlier_mask=inlier_mask, transform=reference_raster.transform)
-    aligned_raster = nuth_kaab.apply(to_be_aligned_raster.data, transform=reference_raster.transform)
-    aligned_raster.data[~np.isfinite(aligned_raster)] = reference_raster.nodata
-
-    diff = reference_raster - \
-           gu.Raster.from_array(aligned_raster.data, transform=reference_raster.transform, crs=reference_raster.crs, nodata=reference_raster.nodata)
-
-    # Save it so that future calls won't need to recreate the file
-    os.makedirs(os.path.dirname(FILEPATHS_PROCESSED['longyearbyen_ddem']), exist_ok=True)
-    diff.save(FILEPATHS_PROCESSED['longyearbyen_ddem'])
+    # If the ddem file does not exist, create it
+    if not os.path.isfile(_FILEPATHS_PROCESSED["longyearbyen_ddem"]):
+        reference_raster = gu.Raster(_FILEPATHS_DATA["longyearbyen_ref_dem"])
+        to_be_aligned_raster = gu.Raster(_FILEPATHS_DATA["longyearbyen_tba_dem"])
+        glacier_mask = gu.Vector(_FILEPATHS_DATA["longyearbyen_glacier_outlines"])
+        inlier_mask = ~glacier_mask.create_mask(reference_raster)
+
+        nuth_kaab = xdem.coreg.NuthKaab()
+        nuth_kaab.fit(reference_raster, to_be_aligned_raster, inlier_mask=inlier_mask)
+        aligned_raster = nuth_kaab.apply(to_be_aligned_raster, resample=True)
+
+        diff = reference_raster - aligned_raster
+
+        # Save it so that future calls won't need to recreate the file
+        os.makedirs(os.path.dirname(_FILEPATHS_PROCESSED["longyearbyen_ddem"]), exist_ok=True)
+        diff.save(_FILEPATHS_PROCESSED["longyearbyen_ddem"])
 
+    # If the tba_dem_coreg file does not exist, create it
+    if not os.path.isfile(_FILEPATHS_PROCESSED["longyearbyen_tba_dem_coreg"]):
 
-def _get_longyearbyen_tba_coreg_dem() -> str:
-    if not os.path.isfile(FILEPATHS_PROCESSED["longyearbyen_tba_dem_coreg"]):
         dem_2009 = xdem.DEM(get_path("longyearbyen_ref_dem"), silent=True)
         ddem = xdem.DEM(get_path("longyearbyen_ddem"), silent=True)
 
-        (dem_2009 - ddem).save(FILEPATHS_PROCESSED["longyearbyen_tba_dem_coreg"])
-
-    return FILEPATHS_PROCESSED["longyearbyen_tba_dem_coreg"]
-
+        # Save it so that future calls won't need to recreate the file
+        (dem_2009 - ddem).save(_FILEPATHS_PROCESSED["longyearbyen_tba_dem_coreg"])
 
 
 def get_path(name: str) -> str:
     """
-    Get path of example data
-    :param name: Name of test data (listed in xdem/examples.py)
+    Get path of example data. List of available files can be found in "examples.available".
+    :param name: Name of test data
     :return:
     """
-    if name == "longyearbyen_tba_dem_coreg":
-        return _get_longyearbyen_tba_coreg_dem()
 
-    if name in list(FILEPATHS_DATA.keys()):
+    if name in list(_FILEPATHS_DATA.keys()):
         download_longyearbyen_examples()
-        return FILEPATHS_DATA[name]
-    elif name in list(FILEPATHS_PROCESSED.keys()):
-        process_coregistered_examples()
-        return FILEPATHS_PROCESSED[name]
+        return _FILEPATHS_DATA[name]
+    elif name in list(_FILEPATHS_PROCESSED.keys()):
+        process_coregistered_examples(name)
+        return _FILEPATHS_PROCESSED[name]
     else:
-        raise ValueError('Data name should be one of "'+'" , "'.join(list(FILEPATHS_DATA.keys())+list(FILEPATHS_PROCESSED.keys()))+'".')
-
+        raise ValueError(
+            'Data name should be one of "'
+            + '" , "'.join(list(_FILEPATHS_DATA.keys()) + list(_FILEPATHS_PROCESSED.keys()))
+            + '".'
+        )
```

### Comparing `xdem-0.0.7/xdem/filters.py` & `xdem-0.0.8/xdem/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Filters to remove outliers and reduce noise in DEMs."""
 from __future__ import annotations
 
-import cv2 as cv
+import warnings
+
+try:
+    import cv2
+
+    _has_cv2 = True
+except ImportError:
+    _has_cv2 = False
 import numpy as np
 import scipy
-import warnings
 
+from xdem._typing import NDArrayf
 
-# Gaussian filters
 
-def gaussian_filter_scipy(array: np.ndarray, sigma: float) -> np.ndarray:
+def gaussian_filter_scipy(array: NDArrayf, sigma: float) -> NDArrayf:
     """
     Apply a Gaussian filter to a raster that may contain NaNs, using scipy's implementation.
     gaussian_filter_cv is recommended as it is usually faster, but this depends on the value of sigma.
 
     N.B: kernel_size is set automatically based on sigma.
 
     :param array: the input array to be filtered.
     :param sigma: the sigma of the Gaussian kernel
 
     :returns: the filtered array (same shape as input)
     """
     # Check that array dimension is 2 or 3
     if np.ndim(array) not in [2, 3]:
-        raise ValueError(
-            f"Invalid array shape given: {array.shape}. Expected 2D or 3D array"
-        )
+        raise ValueError(f"Invalid array shape given: {array.shape}. Expected 2D or 3D array")
 
     # In case array does not contain NaNs, use scipy's gaussian filter directly
     if np.count_nonzero(np.isnan(array)) == 0:
         return scipy.ndimage.gaussian_filter(array, sigma=sigma)
 
     # If array contain NaNs, need a more sophisticated approach
     # Inspired by https://stackoverflow.com/a/36307291
@@ -50,59 +54,60 @@
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="invalid value encountered")
             gauss = gauss_no_nan / gauss_mask
 
         return gauss
 
 
-def gaussian_filter_cv(array: np.ndarray, sigma) -> np.ndarray:
+def gaussian_filter_cv(array: NDArrayf, sigma: float) -> NDArrayf:
     """
     Apply a Gaussian filter to a raster that may contain NaNs, using OpenCV's implementation.
     Arguments are for now hard-coded to be identical to scipy.
 
     N.B: kernel_size is set automatically based on sigma
 
     :param array: the input array to be filtered.
     :param sigma: the sigma of the Gaussian kernel
 
     :returns: the filtered array (same shape as input)
     """
+    if not _has_cv2:
+        raise ValueError("Optional dependency needed. Install 'opencv'")
+
     # Check that array dimension is 2, or can be squeezed to 2D
     orig_shape = array.shape
     if len(orig_shape) == 2:
         pass
     elif len(orig_shape) == 3:
         if orig_shape[0] == 1:
             array = array.squeeze()
         else:
             raise NotImplementedError("Case of array of dimension 3 not implemented")
     else:
-        raise ValueError(
-            f"Invalid array shape given: {orig_shape}. Expected 2D or 3D array"
-        )
+        raise ValueError(f"Invalid array shape given: {orig_shape}. Expected 2D or 3D array")
 
     # In case array does not contain NaNs, use OpenCV's gaussian filter directly
     # With kernel size (0, 0), i.e. set to default, and borderType=BORDER_REFLECT, the output is equivalent to scipy
     if np.count_nonzero(np.isnan(array)) == 0:
-        gauss = cv.GaussianBlur(array, (0, 0), sigmaX=sigma, borderType=cv.BORDER_REFLECT)
+        gauss = cv2.GaussianBlur(array, (0, 0), sigmaX=sigma, borderType=cv2.BORDER_REFLECT)
 
     # If array contain NaNs, need a more sophisticated approach
     # Inspired by https://stackoverflow.com/a/36307291
     else:
 
         # Run filter on a copy with NaNs set to 0
         array_no_nan = array.copy()
         array_no_nan[np.isnan(array)] = 0
-        gauss_no_nan = cv.GaussianBlur(array_no_nan, (0, 0), sigmaX=sigma, borderType=cv.BORDER_REFLECT)
+        gauss_no_nan = cv2.GaussianBlur(array_no_nan, (0, 0), sigmaX=sigma, borderType=cv2.BORDER_REFLECT)
         del array_no_nan
 
         # Mask of NaN values
         nan_mask = 0 * array.copy() + 1
         nan_mask[np.isnan(array)] = 0
-        gauss_mask = cv.GaussianBlur(nan_mask, (0, 0), sigmaX=sigma, borderType=cv.BORDER_REFLECT)
+        gauss_mask = cv2.GaussianBlur(nan_mask, (0, 0), sigmaX=sigma, borderType=cv2.BORDER_REFLECT)
         del nan_mask
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="invalid value encountered")
             gauss = gauss_no_nan / gauss_mask
 
     return gauss.reshape(orig_shape)
@@ -113,15 +118,15 @@
 # To be added
 
 # Min/max filters
 
 # To be added
 
 
-def distance_filter(array: np.ndarray, radius: float, outlier_threshold: float) -> np.ndarray:
+def distance_filter(array: NDArrayf, radius: float, outlier_threshold: float) -> NDArrayf:
     """
     Filter out pixels whose value is distant more than a set threshold from the average value of all neighbor \
 pixels within a given radius.
     Filtered pixels are set to NaN.
 
     TO DO: Add an option on how the "average" value should be calculated, i.e. using a Gaussian, median etc filter.
```

### Comparing `xdem-0.0.7/xdem/fit.py` & `xdem-0.0.8/xdem/fit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,211 @@
 """
 Functions to perform normal, weighted and robust fitting.
 """
 from __future__ import annotations
 
 import inspect
-from typing import Callable, Union, Sized, Optional
 import warnings
+from typing import Any, Callable
 
 import numpy as np
 import pandas as pd
 import scipy.optimize
+from geoutils.raster import subsample_array
 
+from xdem._typing import NDArrayf
 from xdem.spatialstats import nd_binning
-from geoutils.spatial_tools import subsample_raster
 
 try:
-    from sklearn.metrics import mean_squared_error, median_absolute_error
     from sklearn.linear_model import (
-        LinearRegression, TheilSenRegressor, RANSACRegressor, HuberRegressor)
+        HuberRegressor,
+        LinearRegression,
+        RANSACRegressor,
+        TheilSenRegressor,
+    )
+    from sklearn.metrics import median_absolute_error
     from sklearn.pipeline import make_pipeline
-    from sklearn.preprocessing import PolynomialFeatures, RobustScaler
+    from sklearn.preprocessing import PolynomialFeatures
+
     _has_sklearn = True
 except ImportError:
     _has_sklearn = False
 
-def rmse(z: np.ndarray) -> float:
+
+def rmse(z: NDArrayf) -> float:
     """
     Return root mean square error
     :param z: Residuals between predicted and true value
     :return: Root Mean Square Error
     """
     return np.sqrt(np.nanmean(np.square(z)))
 
-def huber_loss(z: np.ndarray) -> float:
+
+def huber_loss(z: NDArrayf) -> float:
     """
     Huber loss cost (reduces the weight of outliers)
     :param z: Residuals between predicted and true values
     :return: Huber cost
     """
     out = np.where(z > 1, 2 * np.sqrt(z[np.where(z > 1)]) - 1, np.square(z))
 
     return out.sum()
 
-def soft_loss(z: np.ndarray, scale = 0.5) -> float:
+
+def soft_loss(z: NDArrayf, scale: float = 0.5) -> float:
     """
     Soft loss cost (reduces the weight of outliers)
     :param z: Residuals between predicted and true values
     :param scale: Scale factor
     :return: Soft loss cost
     """
-    return np.sum(np.square(scale) * 2 * (np.sqrt(1 + np.square(z/scale)) - 1))
+    return np.sum(np.square(scale) * 2 * (np.sqrt(1 + np.square(z / scale)) - 1))
+
 
-def _costfun_sumofsin(p, x, y, cost_func):
+def _cost_sumofsin(
+    p: NDArrayf,
+    x: NDArrayf,
+    y: NDArrayf,
+    cost_func: Callable[[NDArrayf], float],
+) -> float:
     """
     Calculate robust cost function for sum of sinusoids
     """
     z = y - _sumofsinval(x, p)
     return cost_func(z)
 
 
-def _choice_best_order(cost: np.ndarray, margin_improvement : float = 20., verbose: bool = False) -> int:
+def _choice_best_order(cost: NDArrayf, margin_improvement: float = 20.0, verbose: bool = False) -> int:
     """
     Choice of the best order (polynomial, sum of sinusoids) with a margin of improvement. The best cost value does
     not necessarily mean the best predictive fit because high-degree polynomials tend to overfit, and sum of sinusoids
     as well. To mitigate this issue, we should choose the lesser order from which improvement becomes negligible.
+
     :param cost: cost function residuals to the polynomial
     :param margin_improvement: improvement margin (percentage) below which the lesser degree polynomial is kept
     :param verbose: if text should be printed
 
     :return: degree: degree for the best-fit polynomial
     """
 
-    # get percentage of spread from the minimal cost
+    # Get percentage of spread from the minimal cost
     ind_min = cost.argmin()
     min_cost = cost[ind_min]
     perc_cost_improv = (cost - min_cost) / min_cost
 
-    # costs below threshold and lesser degrees
-    below_margin = np.logical_and(perc_cost_improv < margin_improvement / 100., np.arange(len(cost))<=ind_min)
-    costs_below_thresh = cost[below_margin]
-    # minimal costs
-    subindex = costs_below_thresh.argmin()
-    # corresponding index (degree)
-    ind = np.arange(len(cost))[below_margin][subindex]
+    # Keep only good-performance costs that are within 20% of the minimal cost
+    below_margin = np.logical_and(perc_cost_improv < margin_improvement / 100.0, np.arange(len(cost)) <= ind_min)
+
+    # Choose the good-performance cost with lowest degree
+    ind = next((i for i, j in enumerate(below_margin) if j))
 
     if verbose:
-        print('Order '+str(ind_min+1)+ ' has the minimum cost value of '+str(min_cost))
-        print('Order '+str(ind+1)+ ' is selected within a '+str(margin_improvement)+' % margin of'
-            ' the minimum cost, with a cost value of '+str(min_cost))
+        print("Order " + str(ind_min + 1) + " has the minimum cost value of " + str(min_cost))
+        print(
+            "Order " + str(ind + 1) + " is selected as its cost is within a " + str(margin_improvement) + "% margin of"
+            " the minimum cost"
+        )
 
     return ind
 
-def _wrapper_scipy_leastsquares(residual_func, p0, x, y, verbose, **kwargs):
+
+def _wrapper_scipy_leastsquares(
+    residual_func: Callable[[NDArrayf, NDArrayf, NDArrayf], NDArrayf],
+    p0: NDArrayf,
+    x: NDArrayf,
+    y: NDArrayf,
+    verbose: bool = False,
+    **kwargs: Any,
+) -> tuple[float, NDArrayf]:
     """
     Wrapper function for scipy.optimize.least_squares: passes down keyword, extracts cost and final parameters, print
     statements in the console
 
     :param residual_func: Residual function to fit
     :param p0: Initial guess
     :param x: X vector
     :param y: Y vector
     :param verbose: Whether to print out statements
     :return:
     """
 
     # Get arguments of scipy.optimize
-    fun_args = scipy.optimize.least_squares.__code__.co_varnames[:scipy.optimize.least_squares.__code__.co_argcount]
+    fun_args = scipy.optimize.least_squares.__code__.co_varnames[: scipy.optimize.least_squares.__code__.co_argcount]
     # Check no other argument is left to be passed
     remaining_kwargs = kwargs.copy()
     for arg in fun_args:
         remaining_kwargs.pop(arg, None)
     if len(remaining_kwargs) != 0:
-        warnings.warn('Keyword arguments: ' + ','.join(list(remaining_kwargs.keys())) + ' were not used.')
+        warnings.warn("Keyword arguments: " + ",".join(list(remaining_kwargs.keys())) + " were not used.")
     # Filter corresponding arguments before passing
     filtered_kwargs = {k: kwargs[k] for k in fun_args if k in kwargs}
 
     # Run function with associated keyword arguments
-    myresults = scipy.optimize.least_squares(residual_func, p0, args=(x, y), **filtered_kwargs)
+    myresults = scipy.optimize.least_squares(
+        residual_func,
+        p0,
+        args=(x, y),
+        xtol=1e-7,
+        gtol=None,
+        ftol=None,
+        **filtered_kwargs,
+    )
+
+    # Round results above the tolerance to get fixed results on different OS
+    coefs = np.array([np.round(coef, 5) for coef in myresults.x])
+
     if verbose:
         print("Initial Parameters: ", p0)
         print("Status: ", myresults.success, " - ", myresults.status)
         print(myresults.message)
         print("Lowest cost:", myresults.cost)
-        print("Parameters:", myresults.x)
+        print("Parameters:", coefs)
     cost = myresults.cost
-    coefs = myresults.x
 
     return cost, coefs
 
-def _wrapper_sklearn_robustlinear(model, estimator_name, cost_func, x, y, **kwargs):
+
+def _wrapper_sklearn_robustlinear(
+    model: PolynomialFeatures,
+    cost_func: Callable[[NDArrayf, NDArrayf], float],
+    x: NDArrayf,
+    y: NDArrayf,
+    estimator_name: str = "Linear",
+    **kwargs: Any,
+) -> tuple[float, NDArrayf]:
     """
     Wrapper function of sklearn.linear_models: passes down keyword, extracts cost and final parameters, sets random
     states, scales input and de-scales output data, prints out statements
 
     :param model: Function model to fit (e.g., Polynomial features)
-    :param estimator_name: Linear estimator to use (one of "Linear", "Theil-Sen", "RANSAC" and "Huber")
     :param cost_func: Cost function to use for optimization
     :param x: X vector
     :param y: Y vector
+    :param estimator_name: Linear estimator to use (one of "Linear", "Theil-Sen", "RANSAC" and "Huber")
     :return:
     """
     # Select sklearn estimator
-    dict_estimators = {'Linear': LinearRegression, 'Theil-Sen': TheilSenRegressor,
-                       'RANSAC': RANSACRegressor, 'Huber': HuberRegressor}
+    dict_estimators = {
+        "Linear": LinearRegression,
+        "Theil-Sen": TheilSenRegressor,
+        "RANSAC": RANSACRegressor,
+        "Huber": HuberRegressor,
+    }
 
     est = dict_estimators[estimator_name]
 
     # Get existing arguments of the sklearn estimator and model
     estimator_args = list(inspect.signature(est.__init__).parameters.keys())
 
     # Check no other argument is left to be passed
     remaining_kwargs = kwargs.copy()
     for arg in estimator_args:
         remaining_kwargs.pop(arg, None)
     if len(remaining_kwargs) != 0:
-        warnings.warn('Keyword arguments: ' + ','.join(list(remaining_kwargs.keys())) + ' were not used.')
+        warnings.warn("Keyword arguments: " + ",".join(list(remaining_kwargs.keys())) + " were not used.")
     # Filter corresponding arguments before passing
     filtered_kwargs = {k: kwargs[k] for k in estimator_args if k in kwargs}
 
     # TODO: Find out how to re-scale polynomial coefficient + doc on what is the best scaling for polynomials
     # # Scale output data (important for ML algorithms):
     # robust_scaler = RobustScaler().fit(x.reshape(-1,1))
     # x_scaled = robust_scaler.transform(x.reshape(-1,1))
@@ -176,27 +223,36 @@
     pipeline.fit(x.reshape(-1, 1), y)
     y_pred = pipeline.predict(x.reshape(-1, 1))
 
     # Calculate cost
     cost = cost_func(y_pred, y)
 
     # Get polynomial coefficients estimated with the estimators Linear, Theil-Sen and Huber
-    if estimator_name in ['Linear','Theil-Sen','Huber']:
+    if estimator_name in ["Linear", "Theil-Sen", "Huber"]:
         coefs = init_estimator.coef_
     # For some reason RANSAC doesn't store coef at the same place
     else:
         coefs = init_estimator.estimator_.coef_
 
     return cost, coefs
 
 
-def robust_polynomial_fit(x: np.ndarray, y: np.ndarray, max_order: int = 6, estimator_name: str  = 'Theil-Sen',
-                          cost_func: Callable = median_absolute_error, margin_improvement : float = 20.,
-                          subsample: Union[float,int] = 25000, linear_pkg = 'sklearn', verbose: bool = False,
-                          random_state: None | np.random.RandomState | np.random.Generator | int = None, **kwargs) -> tuple[np.ndarray,int]:
+def robust_polynomial_fit(
+    x: NDArrayf,
+    y: NDArrayf,
+    max_order: int = 6,
+    estimator_name: str = "Theil-Sen",
+    cost_func: Callable[[NDArrayf, NDArrayf], float] = median_absolute_error,
+    margin_improvement: float = 20.0,
+    subsample: float | int = 25000,
+    linear_pkg: str = "sklearn",
+    verbose: bool = False,
+    random_state: None | np.random.RandomState | np.random.Generator | int = None,
+    **kwargs: Any,
+) -> tuple[NDArrayf, int]:
     """
     Given 1D vectors x and y, compute a robust polynomial fit to the data. Order is chosen automatically by comparing
     residuals for multiple fit orders of a given estimator.
     Any keyword argument will be passed down to scipy.optimize.least_squares and sklearn linear estimators.
 
     :param x: input x data (N,)
     :param y: input y data (N,)
@@ -208,42 +264,44 @@
     If > 1 will be considered the number of pixels to extract.
     :param linear_pkg: package to use for Linear estimator, one of 'scipy' and 'sklearn'
     :param random_state: random seed for testing purposes
     :param verbose: if text should be printed
 
     :returns coefs, degree: polynomial coefficients and degree for the best-fit polynomial
     """
-    if not isinstance(estimator_name, str) or estimator_name not in ['Linear','Theil-Sen','RANSAC','Huber']:
+    if not isinstance(estimator_name, str) or estimator_name not in ["Linear", "Theil-Sen", "RANSAC", "Huber"]:
         raise ValueError('Attribute estimator must be one of "Linear", "Theil-Sen", "RANSAC" or "Huber".')
-    if not isinstance(linear_pkg, str) or linear_pkg not in ['sklearn','scipy']:
+    if not isinstance(linear_pkg, str) or linear_pkg not in ["sklearn", "scipy"]:
         raise ValueError('Attribute linear_pkg must be one of "scipy" or "sklearn".')
 
     # Remove NaNs
     valid_data = np.logical_and(np.isfinite(y), np.isfinite(x))
     x = x[valid_data]
     y = y[valid_data]
 
     # Subsample data
-    subsamp = subsample_raster(x, subsample=subsample, return_indices=True, random_state=random_state)
+    subsamp = subsample_array(x, subsample=subsample, return_indices=True, random_state=random_state)
     x = x[subsamp]
     y = y[subsamp]
 
     # Initialize cost function and output coefficients
     list_costs = np.empty(max_order)
     list_coeffs = np.zeros((max_order, max_order + 1))
     # Loop on polynomial degrees
     for deg in np.arange(1, max_order + 1):
         # If method is linear and package scipy
-        if estimator_name == 'Linear' and linear_pkg == 'scipy':
+        if estimator_name == "Linear" and linear_pkg == "scipy":
 
             # Define the residual function to optimize with scipy
-            def fitfun_polynomial(xx, params):
-                return sum([p * (xx ** i) for i, p in enumerate(params)])
-            def residual_func(p, xx, yy):
+            def fitfun_polynomial(xx: NDArrayf, params: NDArrayf) -> float:
+                return sum(p * (xx**i) for i, p in enumerate(params))
+
+            def residual_func(p: NDArrayf, xx: NDArrayf, yy: NDArrayf) -> NDArrayf:
                 return fitfun_polynomial(xx, p) - yy
+
             # Define the initial guess
             p0 = np.polyfit(x, y, deg)
 
             # Run the linear method with scipy
             cost, coef = _wrapper_scipy_leastsquares(residual_func, p0, x, y, verbose=verbose, **kwargs)
 
         else:
@@ -251,45 +309,55 @@
             if not _has_sklearn:
                 raise ValueError("Optional dependency needed. Install 'scikit-learn'")
 
             # Define the polynomial model to insert in the pipeline
             model = PolynomialFeatures(degree=deg)
 
             # Run the linear method with sklearn
-            cost, coef = _wrapper_sklearn_robustlinear(model, estimator_name=estimator_name, cost_func=cost_func,
-                                                       x=x, y=y, **kwargs)
+            cost, coef = _wrapper_sklearn_robustlinear(
+                model, estimator_name=estimator_name, cost_func=cost_func, x=x, y=y, **kwargs
+            )
 
         list_costs[deg - 1] = cost
-        list_coeffs[deg - 1, 0:coef.size] = coef
+        list_coeffs[deg - 1, 0 : coef.size] = coef
 
     # Choose the best polynomial with a margin of improvement on the cost
     final_index = _choice_best_order(cost=list_costs, margin_improvement=margin_improvement, verbose=verbose)
 
     # The degree of the best polynomial corresponds to the index plus one
-    return np.trim_zeros(list_coeffs[final_index], 'b'), final_index + 1
+    return np.trim_zeros(list_coeffs[final_index], "b"), final_index + 1
 
 
-def _sumofsinval(x: np.array, params: np.ndarray) -> np.ndarray:
+def _sumofsinval(x: NDArrayf, params: NDArrayf) -> NDArrayf:
     """
     Function for a sum of N frequency sinusoids
     :param x: array of coordinates (N,)
     :param p: list of tuples with amplitude, frequency and phase parameters
     """
     aix = np.arange(0, params.size, 3)
     bix = np.arange(1, params.size, 3)
     cix = np.arange(2, params.size, 3)
 
     val = np.sum(params[aix] * np.sin(2 * np.pi / params[bix] * x[:, np.newaxis] + params[cix]), axis=1)
 
     return val
 
-def robust_sumsin_fit(x: np.ndarray, y: np.ndarray, nb_frequency_max: int = 3,
-                      bounds_amp_freq_phase: Optional[list[tuple[float,float], tuple[float,float], tuple[float,float]]] = None,
-                      cost_func: Callable = soft_loss, subsample: Union[float,int] = 25000, hop_length : Optional[float] = None,
-                      random_state: None | np.random.RandomState | np.random.Generator | int = None, verbose: bool = False) -> tuple[np.ndarray,int]:
+
+def robust_sumsin_fit(
+    x: NDArrayf,
+    y: NDArrayf,
+    nb_frequency_max: int = 3,
+    bounds_amp_freq_phase: list[tuple[float, float]] | None = None,
+    cost_func: Callable[[NDArrayf], float] = soft_loss,
+    subsample: float | int = 25000,
+    hop_length: float | None = None,
+    random_state: None | np.random.RandomState | np.random.Generator | int = None,
+    verbose: bool = False,
+    **kwargs: Any,
+) -> tuple[NDArrayf, int]:
     """
     Given 1D vectors x and y, compute a robust sum of sinusoid fit to the data. The number of frequency is chosen
     automatically by comparing residuals for multiple fit orders of a given estimator.
     Any keyword argument will be passed down to scipy.optimize.basinhopping.
 
     :param x: input x data (N,)
     :param y: input y data (N,)
@@ -299,104 +367,125 @@
     :param hop_length: jump in function values to optimize basinhopping algorithm search (for best results, should be
     comparable to the separation (in function value) between local minima)
     :param cost_func: cost function taking as input two vectors y (true y), y' (predicted y) of same length
     :param subsample: If <= 1, will be considered a fraction of valid pixels to extract.
     If > 1 will be considered the number of pixels to extract.
     :param random_state: random seed for testing purposes
     :param verbose: if text should be printed
+    :param kwargs: Keyword arguments to pass to scipy.optimize.basinhopping
 
-    :returns coefs, degree: polynomial coefficients and degree for the best-fit polynomial
+    :returns coefs, degree: sinusoid coefficients (amplitude, frequency, phase) x N, Number N of summed sinusoids
     """
 
-    def wrapper_costfun_sumofsin(p, x, y):
-        return _costfun_sumofsin(p, x, y, cost_func=cost_func)
+    # Check if there is a number of iterations to stop the run if the global minimum candidate remains the same.
+    if "niter_success" not in kwargs.keys():
+        # Check if there is a number of basin-hopping iterations passed down to the function.
+        if "niter" not in kwargs.keys():
+            niter_success = 40
+        else:
+            niter_success = min(40, kwargs.get("niter"))  # type: ignore
+
+        kwargs.update({"niter_success": niter_success})
+
+    def wrapper_cost_sumofsin(p: NDArrayf, x: NDArrayf, y: NDArrayf) -> float:
+        return _cost_sumofsin(p, x, y, cost_func=cost_func)
 
     # First, remove NaNs
     valid_data = np.logical_and(np.isfinite(y), np.isfinite(x))
     x = x[valid_data]
     y = y[valid_data]
 
     # If no significant resolution is provided, assume that it is the mean difference between sampled X values
     if hop_length is None:
         x_sorted = np.sort(x)
         hop_length = np.mean(np.diff(x_sorted))
 
     # Use binned statistics for first guess
     nb_bin = int((x.max() - x.min()) / (5 * hop_length))
-    df = nd_binning(y, [x], ['var'], list_var_bins=nb_bin, statistics=[np.nanmedian])
+    df = nd_binning(y, [x], ["var"], list_var_bins=nb_bin, statistics=[np.nanmedian])
     # Compute first guess for x and y
-    x_fg = pd.IntervalIndex(df['var']).mid.values
-    y_fg = df['nanmedian']
-    valid_fg = np.logical_and(np.isfinite(x_fg),np.isfinite(y_fg))
+    x_fg = pd.IntervalIndex(df["var"]).mid.values
+    y_fg = df["nanmedian"]
+    valid_fg = np.logical_and(np.isfinite(x_fg), np.isfinite(y_fg))
     x_fg = x_fg[valid_fg]
     y_fg = y_fg[valid_fg]
 
     # Loop on all frequencies
     costs = np.empty(nb_frequency_max)
-    amp_freq_phase = np.zeros((nb_frequency_max, 3*nb_frequency_max)) * np.nan
+    amp_freq_phase = np.zeros((nb_frequency_max, 3 * nb_frequency_max)) * np.nan
 
-    for nb_freq in np.arange(1, nb_frequency_max+1):
+    for nb_freq in np.arange(1, nb_frequency_max + 1):
 
         b = bounds_amp_freq_phase
         # If bounds are not provided, define as the largest possible bounds
         if b is None:
             lb_amp = 0
             ub_amp = (y_fg.max() - y_fg.min()) / 2
             # Define for phase
             lb_phase = 0
             ub_phase = 2 * np.pi
             # Define for the frequency, we need at least 5 points to see any kind of periodic signal
             lb_frequency = 1 / (5 * (x.max() - x.min()))
             ub_frequency = 1 / (5 * hop_length)
 
             b = []
-            for i in range(nb_freq):
-                b += [(lb_amp,ub_amp),(lb_frequency,ub_frequency),(lb_phase,ub_phase)]
+            for _i in range(nb_freq):
+                b += [(lb_amp, ub_amp), (lb_frequency, ub_frequency), (lb_phase, ub_phase)]
 
         # Format lower and upper bounds for scipy
-        lb = np.asarray(([b[i][0] for i in range(3*nb_freq)]))
-        ub = np.asarray(([b[i][1] for i in range(3*nb_freq)]))
+        lb = np.asarray([b[i][0] for i in range(3 * nb_freq)])
+        ub = np.asarray([b[i][1] for i in range(3 * nb_freq)])
         # Insert in a scipy bounds object
         scipy_bounds = scipy.optimize.Bounds(lb, ub)
         # First guess for the mean parameters
         p0 = np.divide(lb + ub, 2)
 
         # Initialize with the first guess
-        init_args = dict(args=(x_fg, y_fg), method="L-BFGS-B",
-                         bounds=scipy_bounds, options={"ftol": 1E-6})
-        init_results = scipy.optimize.basinhopping(wrapper_costfun_sumofsin, p0, disp=verbose,
-                                                   T=hop_length, minimizer_kwargs=init_args, seed=random_state)
+        init_args = dict(args=(x_fg, y_fg), method="L-BFGS-B", bounds=scipy_bounds, options={"ftol": 1e-6})
+        init_results = scipy.optimize.basinhopping(
+            wrapper_cost_sumofsin,
+            p0,
+            disp=verbose,
+            T=hop_length,
+            minimizer_kwargs=init_args,
+            seed=random_state,
+            **kwargs,
+        )
         init_results = init_results.lowest_optimization_result
+        init_x = np.array([np.round(ini, 5) for ini in init_results.x])
 
         # Subsample the final raster
-        subsamp = subsample_raster(x, subsample=subsample, return_indices=True, random_state=random_state)
+        subsamp = subsample_array(x, subsample=subsample, return_indices=True, random_state=random_state)
         x = x[subsamp]
         y = y[subsamp]
 
         # Minimize the globalization with a larger number of points
-        minimizer_kwargs = dict(args=(x, y),
-                                method="L-BFGS-B",
-                                bounds=scipy_bounds,
-                                options={"ftol": 1E-6})
-        myresults = scipy.optimize.basinhopping(wrapper_costfun_sumofsin, init_results.x, disp=verbose,
-                                                T=5 * hop_length, niter_success=40,
-                                                minimizer_kwargs=minimizer_kwargs, seed=random_state)
+        minimizer_kwargs = dict(args=(x, y), method="L-BFGS-B", bounds=scipy_bounds, options={"ftol": 1e-6})
+        myresults = scipy.optimize.basinhopping(
+            wrapper_cost_sumofsin,
+            init_x,
+            disp=verbose,
+            T=5 * hop_length,
+            minimizer_kwargs=minimizer_kwargs,
+            seed=random_state,
+            **kwargs,
+        )
         myresults = myresults.lowest_optimization_result
+        myresults_x = np.array([np.round(myres, 5) for myres in myresults.x])
         # Write results for this number of frequency
-        costs[nb_freq-1] = wrapper_costfun_sumofsin(myresults.x,x,y)
-        amp_freq_phase[nb_freq -1, 0:3*nb_freq] = myresults.x
+        costs[nb_freq - 1] = wrapper_cost_sumofsin(myresults_x, x, y)
+        amp_freq_phase[nb_freq - 1, 0 : 3 * nb_freq] = myresults_x
 
     final_index = _choice_best_order(cost=costs)
 
-    final_coefs =  amp_freq_phase[final_index][~np.isnan(amp_freq_phase[final_index])]
+    final_coefs = amp_freq_phase[final_index][~np.isnan(amp_freq_phase[final_index])]
 
     # If an amplitude coefficient is almost zero, remove the coefs of that frequency and lower the degree
     final_degree = final_index + 1
-    for i in range(final_index+1):
-        if np.abs(final_coefs[3*i]) < (np.nanpercentile(x, 90) - np.nanpercentile(x, 10))/1000:
-            final_coefs = np.delete(final_coefs, slice(3*i,3*i+3))
+    for i in range(final_index + 1):
+        if np.abs(final_coefs[3 * i]) < (np.nanpercentile(x, 90) - np.nanpercentile(x, 10)) / 1000:
+            final_coefs = np.delete(final_coefs, slice(3 * i, 3 * i + 3))
             final_degree -= 1
             break
 
     # The number of frequencies corresponds to the final index plus one
     return final_coefs, final_degree
-
```

### Comparing `xdem-0.0.7/xdem/spatialstats.py` & `xdem-0.0.8/xdem/spatialstats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,195 +1,226 @@
 """Spatial statistical tools to estimate uncertainties related to DEMs"""
 from __future__ import annotations
 
 import inspect
+import itertools
 import math as m
 import multiprocessing as mp
-import os
 import warnings
-from functools import partial
-
-from typing import Callable, Union, Iterable, Optional, Sequence, Any, overload
+from typing import Any, Callable, Iterable, Literal, TypedDict, overload
 
-import itertools
+import geopandas as gpd
 import matplotlib
-import matplotlib.pyplot as plt
 import matplotlib.colors as colors
-from numba import njit
+import matplotlib.pyplot as plt
+import numba
 import numpy as np
 import pandas as pd
-import geopandas as gpd
+from geoutils.raster import (
+    Mask,
+    Raster,
+    RasterType,
+    get_array_and_mask,
+    subsample_array,
+)
+from geoutils.vector import Vector, VectorType
+from numba import jit
+from numpy.typing import ArrayLike
 from scipy import integrate
+from scipy.interpolate import RegularGridInterpolator, griddata
 from scipy.optimize import curve_fit
+from scipy.signal import fftconvolve
 from scipy.spatial.distance import pdist, squareform
-from skimage.draw import disk
-from scipy.interpolate import RegularGridInterpolator, LinearNDInterpolator, griddata
 from scipy.stats import binned_statistic, binned_statistic_2d, binned_statistic_dd
-from geoutils.spatial_tools import subsample_raster, get_array_and_mask
-from geoutils.georaster import RasterType, Raster
-from geoutils.geovector import VectorType, Vector
+from skimage.draw import disk
+
+from xdem._typing import NDArrayf
 
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import skgstat as skg
-    from skgstat import models
 
-def nmad(data: np.ndarray, nfact: float = 1.4826) -> float:
+
+def nmad(data: NDArrayf | RasterType, nfact: float = 1.4826) -> np.floating[Any]:
     """
     Calculate the normalized median absolute deviation (NMAD) of an array.
     Default scaling factor is 1.4826 to scale the median absolute deviation (MAD) to the dispersion of a normal
     distribution (see https://en.wikipedia.org/wiki/Median_absolute_deviation#Relation_to_standard_deviation, and
     e.g. Höhle and Höhle (2009), http://dx.doi.org/10.1016/j.isprsjprs.2009.02.003)
 
-    :param data: Input data
+    :param data: Input array or raster
     :param nfact: Normalization factor for the data
 
     :returns nmad: (normalized) median absolute deviation of data.
     """
     if isinstance(data, np.ma.masked_array):
         data_arr = get_array_and_mask(data, check_shape=False)[0]
+    elif isinstance(data, Raster):
+        data_arr = data
     else:
         data_arr = np.asarray(data)
     return nfact * np.nanmedian(np.abs(data_arr - np.nanmedian(data_arr)))
 
 
-def nd_binning(values: np.ndarray, list_var: Iterable[np.ndarray], list_var_names=Iterable[str], list_var_bins: Optional[Union[int,Iterable[Iterable]]] = None,
-                     statistics: Iterable[Union[str, Callable, None]] = ['count', np.nanmedian, nmad], list_ranges : Optional[Iterable[Sequence]] = None) \
-        -> pd.DataFrame:
+def nd_binning(
+    values: NDArrayf,
+    list_var: list[NDArrayf],
+    list_var_names: list[str],
+    list_var_bins: int | tuple[int, ...] | tuple[NDArrayf] | None = None,
+    statistics: Iterable[str | Callable[[NDArrayf], np.floating[Any]]] = ("count", np.nanmedian, nmad),
+    list_ranges: list[float] | None = None,
+) -> pd.DataFrame:
     """
     N-dimensional binning of values according to one or several explanatory variables with computed statistics in
     each bin. By default, the sample count, the median and the normalized absolute median deviation (NMAD). The count
     is always computed, no matter user input.
     Values input is a (N,) array and variable input is a L-sized list of flattened arrays of similar dimensions (N,).
     For more details on the format of input variables, see documentation of scipy.stats.binned_statistic_dd.
 
     :param values: Values array of size (N,)
     :param list_var: List of size (L) of explanatory variables array of size (N,)
     :param list_var_names: List of size (L) of names of the explanatory variables
-    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory variables; defaults to 10 bins
+    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory
+        variables; defaults to 10 bins
     :param statistics: List of size (X) of statistics to be computed; defaults to count, median and nmad
-    :param list_ranges: List of size (L) of minimum and maximum ranges to bin the explanatory variables; defaults to min/max of the data
+    :param list_ranges: List of size (L) of minimum and maximum ranges to bin the explanatory variables; defaults to
+        min/max of the data
     :return:
     """
 
-    # We separate 1d, 2d and nd binning, because propagating statistics between different dimensional binning is not always feasible
-    # using scipy because it allows for several dimensional binning, while it's not straightforward in pandas
+    # We separate 1d, 2d and nd binning, because propagating statistics between different dimensional binning is not
+    # always feasible using scipy because it allows for several dimensional binning, while it's not straightforward in
+    # pandas
     if list_var_bins is None:
         list_var_bins = (10,) * len(list_var_names)
     elif isinstance(list_var_bins, (int, np.integer)):
         list_var_bins = (list_var_bins,) * len(list_var_names)
 
     # Flatten the arrays if this has not been done by the user
     values = values.ravel()
     list_var = [var.ravel() for var in list_var]
 
     # Remove no data values
-    valid_data = np.logical_and.reduce([np.isfinite(values)]+[np.isfinite(var) for var in list_var])
+    valid_data = np.logical_and.reduce([np.isfinite(values)] + [np.isfinite(var) for var in list_var])
     values = values[valid_data]
     list_var = [var[valid_data] for var in list_var]
 
     statistics = list(statistics)
     # In case the statistics are user-defined, and they forget count, we add it for later calculation or plotting
-    if 'count' not in statistics:
-        statistics = ['count'] + statistics
+    if "count" not in statistics:
+        statistics.insert(0, "count")
 
     statistics_name = [f if isinstance(f, str) else f.__name__ for f in statistics]
 
     # Get binned statistics in 1d: a simple loop is sufficient
     list_df_1d = []
     for i, var in enumerate(list_var):
         df_stats_1d = pd.DataFrame()
         # Get statistics
         for j, statistic in enumerate(statistics):
-            stats_binned_1d, bedges_1d = binned_statistic(var,values,statistic=statistic,bins=list_var_bins[i],range=list_ranges)[:2]
+            stats_binned_1d, bedges_1d = binned_statistic(
+                x=var, values=values, statistic=statistic, bins=list_var_bins[i], range=list_ranges
+            )[:2]
             # Save in a dataframe
             df_stats_1d[statistics_name[j]] = stats_binned_1d
         # We need to get the middle of the bins from the edges, to get the same dimension length
-        df_stats_1d[list_var_names[i]] = pd.IntervalIndex.from_breaks(bedges_1d,closed='left')
+        df_stats_1d[list_var_names[i]] = pd.IntervalIndex.from_breaks(bedges_1d, closed="left")
         # Report number of dimensions used
-        df_stats_1d.insert(0, 'nd', 1)
+        df_stats_1d.insert(0, "nd", 1)
 
         list_df_1d.append(df_stats_1d)
 
     # Get binned statistics in 2d: all possible 2d combinations
     list_df_2d = []
-    if len(list_var)>1:
+    if len(list_var) > 1:
         combs = list(itertools.combinations(list_var_names, 2))
-        for i, comb in enumerate(combs):
+        for _, comb in enumerate(combs):
             var1_name, var2_name = comb
             # Corresponding variables indexes
             i1, i2 = list_var_names.index(var1_name), list_var_names.index(var2_name)
             df_stats_2d = pd.DataFrame()
             for j, statistic in enumerate(statistics):
-                stats_binned_2d, bedges_var1, bedges_var2 = binned_statistic_2d(list_var[i1],list_var[i2],values,statistic=statistic
-                                                             ,bins=[list_var_bins[i1],list_var_bins[i2]]
-                                                             ,range=list_ranges)[:3]
+                stats_binned_2d, bedges_var1, bedges_var2 = binned_statistic_2d(
+                    x=list_var[i1],
+                    y=list_var[i2],
+                    values=values,
+                    statistic=statistic,
+                    bins=[list_var_bins[i1], list_var_bins[i2]],
+                    range=list_ranges,
+                )[:3]
                 # Get statistics
                 df_stats_2d[statistics_name[j]] = stats_binned_2d.flatten()
             # Derive interval indexes and convert bins into 2d indexes
-            ii1 = pd.IntervalIndex.from_breaks(bedges_var1,closed='left')
-            ii2 = pd.IntervalIndex.from_breaks(bedges_var2,closed='left')
+            ii1 = pd.IntervalIndex.from_breaks(bedges_var1, closed="left")
+            ii2 = pd.IntervalIndex.from_breaks(bedges_var2, closed="left")
             df_stats_2d[var1_name] = [i1 for i1 in ii1 for i2 in ii2]
             df_stats_2d[var2_name] = [i2 for i1 in ii1 for i2 in ii2]
             # Report number of dimensions used
-            df_stats_2d.insert(0, 'nd', 2)
+            df_stats_2d.insert(0, "nd", 2)
 
             list_df_2d.append(df_stats_2d)
 
-
     # Get binned statistics in nd, without redoing the same stats
     df_stats_nd = pd.DataFrame()
-    if len(list_var)>2:
+    if len(list_var) > 2:
         for j, statistic in enumerate(statistics):
-            stats_binned_2d, list_bedges = binned_statistic_dd(list_var,values,statistic=statistic,bins=list_var_bins,range=list_ranges)[0:2]
+            stats_binned_2d, list_bedges = binned_statistic_dd(
+                sample=list_var, values=values, statistic=statistic, bins=list_var_bins, range=list_ranges
+            )[0:2]
             df_stats_nd[statistics_name[j]] = stats_binned_2d.flatten()
         list_ii = []
         # Loop through the bin edges and create IntervalIndexes from them (to get both
         for bedges in list_bedges:
-            list_ii.append(pd.IntervalIndex.from_breaks(bedges,closed='left'))
+            list_ii.append(pd.IntervalIndex.from_breaks(bedges, closed="left"))
 
         # Create nd indexes in nd-array and flatten for each variable
         iind = np.meshgrid(*list_ii)
         for i, var_name in enumerate(list_var_names):
             df_stats_nd[var_name] = iind[i].flatten()
 
         # Report number of dimensions used
-        df_stats_nd.insert(0, 'nd', len(list_var_names))
+        df_stats_nd.insert(0, "nd", len(list_var_names))
 
     # Concatenate everything
     list_all_dfs = list_df_1d + list_df_2d + [df_stats_nd]
     df_concat = pd.concat(list_all_dfs)
     # commenting for now: pd.MultiIndex can be hard to use
     # df_concat = df_concat.set_index(list_var_names)
 
     return df_concat
 
 
-def interp_nd_binning(df: pd.DataFrame, list_var_names: Union[str, Iterable[str]], statistic : Union[str, Callable[[np.ndarray],float]] = nmad,
-                      min_count: Optional[int] = 100) -> Callable[[tuple[np.ndarray, ...]], np.ndarray]:
+def interp_nd_binning(
+    df: pd.DataFrame,
+    list_var_names: str | list[str],
+    statistic: str | Callable[[NDArrayf], np.floating[Any]] = nmad,
+    min_count: int | None = 100,
+) -> Callable[[tuple[ArrayLike, ...]], NDArrayf]:
     """
     Estimate an interpolant function for an N-dimensional binning. Preferably based on the output of nd_binning.
     For more details on the input dataframe, and associated list of variable name and statistic, see nd_binning.
 
-    If the variable pd.DataSeries corresponds to an interval (as the output of nd_binning), uses the middle of the interval.
+    If the variable pd.DataSeries corresponds to an interval (as the output of nd_binning), uses the middle of the
+    interval.
     Otherwise, uses the variable as such.
 
     Workflow of the function:
-    Fills the no-data present on the regular N-D binning grid with nearest neighbour from scipy.griddata, then provides an
-    interpolant function that linearly interpolates/extrapolates using scipy.RegularGridInterpolator.
+    Fills the no-data present on the regular N-D binning grid with nearest neighbour from scipy.griddata, then provides
+    an interpolant function that linearly interpolates/extrapolates using scipy.RegularGridInterpolator.
 
-    :param df: Dataframe with statistic of binned values according to explanatory variables (preferably output of nd_binning)
-    :param list_var_names: Explanatory variable data series to select from the dataframe (containing interval or float dtype)
+    :param df: Dataframe with statistic of binned values according to explanatory variables
+    :param list_var_names: Explanatory variable data series to select from the dataframe
     :param statistic: Statistic to interpolate, stored as a data series in the dataframe
     :param min_count: Minimum number of samples to be used as a valid statistic (replaced by nodata)
     :return: N-dimensional interpolant function
 
     :examples
     # Using a dataframe created from scratch
-    >>> df = pd.DataFrame({"var1": [1, 2, 3, 1, 2, 3, 1, 2, 3], "var2": [1, 1, 1, 2, 2, 2, 3, 3, 3], "statistic": [1, 2, 3, 4, 5, 6, 7, 8, 9]})
+    >>> df = pd.DataFrame({"var1": [1, 2, 3, 1, 2, 3, 1, 2, 3], "var2": [1, 1, 1, 2, 2, 2, 3, 3, 3],
+    ... "statistic": [1, 2, 3, 4, 5, 6, 7, 8, 9]})
 
     # In 2 dimensions, the statistic array looks like this
     # array([
     #     [1, 2, 3],
     #     [4, 5, 6],
     #     [7, 8, 9]
     #     ])
@@ -210,92 +241,130 @@
     # If list of variable input is simply a string
     if isinstance(list_var_names, str):
         list_var_names = [list_var_names]
 
     # Check that the dataframe contains what we need
     for var in list_var_names:
         if var not in df.columns:
-            raise ValueError('Variable "'+var+'" does not exist in the provided dataframe.')
+            raise ValueError('Variable "' + var + '" does not exist in the provided dataframe.')
     statistic_name = statistic if isinstance(statistic, str) else statistic.__name__
     if statistic_name not in df.columns:
         raise ValueError('Statistic "' + statistic_name + '" does not exist in the provided dataframe.')
-    if min_count is not None and 'count' not in df.columns:
+    if min_count is not None and "count" not in df.columns:
         raise ValueError('Statistic "count" is not in the provided dataframe, necessary to use the min_count argument.')
     if df.empty:
-        raise ValueError('Dataframe is empty.')
+        raise ValueError("Dataframe is empty.")
 
     df_sub = df.copy()
 
     # If the dataframe is an output of nd_binning, keep only the dimension of interest
-    if 'nd' in df_sub.columns:
+    if "nd" in df_sub.columns:
         df_sub = df_sub[df_sub.nd == len(list_var_names)]
 
+    # Function to convert IntervalIndex written to str in csv back to pd.Interval
+    # from: https://github.com/pandas-dev/pandas/issues/28210
+    def to_interval(istr: str) -> float | pd.Interval:
+        if isinstance(istr, float):
+            return np.nan
+        else:
+            c_left = istr[0] == "["
+            c_right = istr[-1] == "]"
+            closed = {(True, False): "left", (False, True): "right", (True, True): "both", (False, False): "neither"}[
+                c_left, c_right
+            ]
+            left, right = map(float, istr[1:-1].split(","))
+            try:
+                return pd.Interval(left, right, closed)
+            except Exception:
+                return np.nan
+
     # Compute the middle values instead of bin interval if the variable is a pandas interval type
     for var in list_var_names:
-        check_any_interval = [isinstance(x, pd.Interval) for x in df_sub[var].values]
-        if any(check_any_interval):
+
+        # Check if all value are numeric (NaN counts as integer), if yes leave as is
+        if all(isinstance(x, (int, float, np.integer, np.floating)) for x in df_sub[var].values):
+            pass
+        # Check if any value is a pandas interval (NaN do not count, so using any), if yes compute the middle values
+        elif any(isinstance(x, pd.Interval) for x in df_sub[var].values):
             df_sub[var] = pd.IntervalIndex(df_sub[var]).mid.values
-        # Otherwise, leave as is
+        # Check for any unformatted interval (saving and reading a pd.DataFrame without MultiIndexing transforms
+        # pd.Interval into strings)
+        elif any(isinstance(to_interval(x), pd.Interval) for x in df_sub[var].values):
+            intervalindex_vals = [to_interval(x) for x in df_sub[var].values]
+            df_sub[var] = pd.IntervalIndex(intervalindex_vals).mid.values
+        else:
+            raise ValueError("The variable columns must be provided as numerical mid values, or pd.Interval values.")
 
     # Check that explanatory variables have valid binning values which coincide along the dataframe
     df_sub = df_sub[np.logical_and.reduce([np.isfinite(df_sub[var].values) for var in list_var_names])]
     if df_sub.empty:
-        raise ValueError('Dataframe does not contain a nd binning with the variables corresponding to the list of variables.')
+        raise ValueError(
+            "Dataframe does not contain a nd binning with the variables corresponding to the list of variables."
+        )
     # Check that the statistic data series contain valid data
     if all(~np.isfinite(df_sub[statistic_name].values)):
-        raise ValueError('Dataframe does not contain any valid statistic values.')
+        raise ValueError("Dataframe does not contain any valid statistic values.")
 
     # Remove statistic values calculated with a sample count under the minimum count
     if min_count is not None:
-        df_sub.loc[df_sub['count'] < min_count, statistic_name] = np.nan
+        df_sub.loc[df_sub["count"] < min_count, statistic_name] = np.nan
 
     values = df_sub[statistic_name].values
     ind_valid = np.isfinite(values)
 
     # Re-check that the statistic data series contain valid data after filtering with min_count
     if all(~ind_valid):
-        raise ValueError("Dataframe does not contain any valid statistic values after filtering with min_count = "+str(min_count)+".")
+        raise ValueError(
+            "Dataframe does not contain any valid statistic values after filtering with min_count = "
+            + str(min_count)
+            + "."
+        )
 
     # Get a list of middle values for the binning coordinates, to define a nd grid
     list_bmid = []
     shape = []
     for var in list_var_names:
         bmid = sorted(np.unique(df_sub[var][ind_valid]))
         list_bmid.append(bmid)
         shape.append(len(bmid))
 
     # Use griddata first to perform nearest interpolation with NaNs (irregular grid)
     # Valid values
     values = values[ind_valid]
     # coordinates of valid values
-    points_valid = tuple([df_sub[var].values[ind_valid] for var in list_var_names])
+    points_valid = tuple(df_sub[var].values[ind_valid] for var in list_var_names)
     # Grid coordinates
-    bmid_grid = np.meshgrid(*list_bmid, indexing='ij')
-    points_grid = tuple([bmid_grid[i].flatten() for i in range(len(list_var_names))])
+    bmid_grid = np.meshgrid(*list_bmid, indexing="ij")
+    points_grid = tuple(bmid_grid[i].flatten() for i in range(len(list_var_names)))
     # Fill grid no data with nearest neighbour
-    values_grid = griddata(points_valid, values, points_grid, method='nearest')
+    values_grid = griddata(points_valid, values, points_grid, method="nearest")
     values_grid = values_grid.reshape(shape)
 
     # RegularGridInterpolator to perform linear interpolation/extrapolation on the grid
     # (will extrapolate only outside of boundaries not filled with the nearest of griddata as fill_value = None)
-    interp_fun = RegularGridInterpolator(tuple(list_bmid), values_grid, method='linear', bounds_error=False, fill_value=None)
-
-    return interp_fun
+    interp_fun = RegularGridInterpolator(
+        tuple(list_bmid), values_grid, method="linear", bounds_error=False, fill_value=None
+    )
+
+    return interp_fun  # type: ignore
 
 
-def two_step_standardization(dvalues: np.ndarray, list_var: Iterable[np.ndarray],
-                unscaled_error_fun: Callable[[tuple[np.ndarray, ...]], np.ndarray],
-                spread_statistic: Callable = nmad,
-                fac_spread_outliers: float | None = 7
-                ) -> tuple[np.ndarray, Callable[[tuple[np.ndarray, ...]], np.ndarray]]:
+def two_step_standardization(
+    dvalues: NDArrayf,
+    list_var: list[NDArrayf],
+    unscaled_error_fun: Callable[[tuple[ArrayLike, ...]], NDArrayf],
+    spread_statistic: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    fac_spread_outliers: float | None = 7,
+) -> tuple[NDArrayf, Callable[[tuple[ArrayLike, ...]], NDArrayf]]:
     """
     Standardize the proxy differenced values using the modelled heteroscedasticity, re-scaled to the spread statistic,
     and generate the final standardization function.
 
-    :param dvalues: Proxy values as array of size (N,) (i.e., differenced values where signal should be zero such as elevation differences on stable terrain)
+    :param dvalues: Proxy values as array of size (N,) (i.e., differenced values where signal should be zero such as
+        elevation differences on stable terrain)
     :param list_var: List of size (L) of explanatory variables array of size (N,)
     :param unscaled_error_fun: Function of the spread with explanatory variables not yet re-scaled
     :param spread_statistic: Statistic to be computed for the spread; defaults to nmad
     :param fac_spread_outliers: Exclude outliers outside this spread after standardizing; pass None to ignore.
 
     :return: Standardized values array of size (N,), Function to destandardize
     """
@@ -312,205 +381,331 @@
     # z-score exactly equal to one due to approximations of N-D binning, interpolating and due to the outlier filtering
     zscore_nmad = spread_statistic(zscores)
 
     # Re-standardize
     zscores /= zscore_nmad
 
     # Define the exact function for de-standardization to pass as output
-    def error_fun(*args):
+    def error_fun(*args: tuple[ArrayLike, ...]) -> NDArrayf:
         return zscore_nmad * unscaled_error_fun(*args)
 
     return zscores, error_fun
 
 
-def estimate_model_heteroscedasticity(dvalues: np.ndarray, list_var: Iterable[np.ndarray], list_var_names: Iterable[str],
-                                      spread_statistic: Callable = nmad,
-                                      list_var_bins: Optional[Union[int,Iterable[Iterable]]] = None,
-                                      min_count: Optional[int] = 100,
-                                      fac_spread_outliers: float | None = 7
-                                      ) -> tuple[pd.DataFrame, Callable[[tuple[np.ndarray, ...]], np.ndarray]]:
+def estimate_model_heteroscedasticity(
+    dvalues: NDArrayf,
+    list_var: list[NDArrayf],
+    list_var_names: list[str],
+    spread_statistic: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    list_var_bins: int | tuple[int, ...] | tuple[NDArrayf] | None = None,
+    min_count: int | None = 100,
+    fac_spread_outliers: float | None = 7,
+) -> tuple[pd.DataFrame, Callable[[tuple[NDArrayf, ...]], NDArrayf]]:
     """
     Estimate and model the heteroscedasticity (i.e., variability in error) according to a list of explanatory variables
     from a proxy of differenced values (e.g., elevation differences), if possible compared to a source of higher
     precision.
 
     This function performs N-D data binning with the list of explanatory variable for a spread statistic, then
     performs N-D interpolation on this statistic, scales the output with a two-step standardization to return an error
     function of the explanatory variables.
 
     The functions used are `nd_binning`, `interp_nd_binning` and `two_step_standardization`.
 
-    :param dvalues: Proxy values as array of size (N,) (i.e., differenced values where signal should be zero such as elevation differences on stable terrain)
+    :param dvalues: Proxy values as array of size (N,) (i.e., differenced values where signal should be zero such as
+        elevation differences on stable terrain)
     :param list_var: List of size (L) of explanatory variables array of size (N,)
     :param list_var_names: List of size (L) of names of the explanatory variables
     :param spread_statistic: Statistic to be computed for the spread; defaults to nmad
-    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory variables; defaults to 10 bins
+    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory
+        variables; defaults to 10 bins
     :param min_count: Minimum number of samples to be used as a valid statistic (replaced by nodata)
     :param fac_spread_outliers: Exclude outliers outside this spread after standardizing; pass None to ignore.
 
     :return: Dataframe of binned spread statistic with explanatory variables, Error function with explanatory variables
     """
 
     # Perform N-D binning with the differenced values computing the spread statistic
-    df = nd_binning(values=dvalues, list_var=list_var, list_var_names=list_var_names, statistics=[spread_statistic],
-                    list_var_bins=list_var_bins)
+    df = nd_binning(
+        values=dvalues,
+        list_var=list_var,
+        list_var_names=list_var_names,
+        statistics=[spread_statistic],
+        list_var_bins=list_var_bins,
+    )
 
     # Perform N-D linear interpolation for the spread statistic
     fun = interp_nd_binning(df, list_var_names=list_var_names, statistic=spread_statistic.__name__, min_count=min_count)
 
     # Get the final function based on a two-step standardization
-    final_fun = two_step_standardization(dvalues=dvalues, list_var=list_var, unscaled_error_fun=fun,
-                                         spread_statistic=spread_statistic, fac_spread_outliers=fac_spread_outliers)[1]
+    final_fun = two_step_standardization(
+        dvalues=dvalues,
+        list_var=list_var,
+        unscaled_error_fun=fun,
+        spread_statistic=spread_statistic,
+        fac_spread_outliers=fac_spread_outliers,
+    )[1]
 
     return df, final_fun
 
 
 @overload
-def infer_heteroscedasticity_from_stable(dvalues: np.ndarray, list_var: list[np.ndarray | RasterType],
-                                         stable_mask: np.ndarray | VectorType | gpd.GeoDataFrame,
-                                         unstable_mask: np.ndarray | VectorType | gpd.GeoDataFrame,
-                                         list_var_names: Iterable[str],
-                                         spread_statistic: Callable,
-                                         list_var_bins: Optional[Union[int,Iterable[Iterable]]],
-                                         min_count: Optional[int],
-                                         factor_spread_exclude_outliers: float | None,
-                                         ) -> tuple[np.ndarray,
-                                            pd.DataFrame,
-                                            Callable[[tuple[np.ndarray, ...]], np.ndarray]]: ...
-
-@overload
-def infer_heteroscedasticity_from_stable(dvalues: RasterType, list_var: list[np.ndarray | RasterType],
-                                         stable_mask: np.ndarray | VectorType | gpd.GeoDataFrame,
-                                         unstable_mask: np.ndarray | VectorType | gpd.GeoDataFrame,
-                                         list_var_names: Iterable[str],
-                                         spread_statistic: Callable,
-                                         list_var_bins: Optional[Union[int,Iterable[Iterable]]],
-                                         min_count: Optional[int],
-                                         factor_spread_exclude_outliers: float | None,
-                                         ) -> tuple[RasterType,
-                                            pd.DataFrame,
-                                            Callable[[tuple[np.ndarray, ...]], np.ndarray]]: ...
-
-def infer_heteroscedasticity_from_stable(dvalues: np.ndarray | RasterType, list_var: list[np.ndarray | RasterType],
-                                         stable_mask: np.ndarray | VectorType | gpd.GeoDataFrame = None,
-                                         unstable_mask: np.ndarray | VectorType | gpd.GeoDataFrame = None,
-                                         list_var_names: Iterable[str] = None,
-                                         spread_statistic: Callable = nmad,
-                                         list_var_bins: Optional[Union[int,Iterable[Iterable]]] = None,
-                                         min_count: Optional[int] = 100,
-                                         fac_spread_outliers: float | None = 7,
-                                         ) -> tuple[np.ndarray | RasterType,
-                                            pd.DataFrame,
-                                            Callable[[tuple[np.ndarray, ...]], np.ndarray]]:
-    """
-    Infer heteroscedasticity from differenced values on stable terrain and a list of explanatory variables.
-
-    This function returns an error map, a dataframe of spread values and the error function with explanatory variables.
-    It is a convenience wrapper for `estimate_model_heteroscedasticity` to work on either Raster or array, compute the
-    stable mask and return an error map.
+def _preprocess_values_with_mask_to_array(  # type: ignore
+    values: list[NDArrayf | RasterType],
+    include_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    exclude_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    gsd: float | None = None,
+    preserve_shape: bool = True,
+) -> tuple[list[NDArrayf], float]:
+    ...
 
-    If no stable or unstable mask is provided to mask in or out the values, all terrain is used.
 
-    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as elevation differences on stable terrain)
-    :param list_var: List of size (L) of explanatory variables as array or Raster of same shape as dvalues
-    :param stable_mask: Vector shapefile of stable terrain (if dvalues is Raster), or boolean array of same shape as dvalues
-    :param unstable_mask: Vector shapefile of unstable terrain (if dvalues is Raster), or boolean array of same shape as dvalues
-    :param list_var_names: List of size (L) of names of the explanatory variables, otherwise named var1, var2, etc.
-    :param spread_statistic: Statistic to be computed for the spread; defaults to nmad
-    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory variables; defaults to 10 bins
-    :param min_count: Minimum number of samples to be used as a valid statistic (replaced by nodata)
-    :param fac_spread_outliers: Exclude outliers outside this spread after standardizing; pass None to ignore.
-
-    :return: Inferred error map (array or Raster, same as input proxy values),
-        Dataframe of binned spread statistic with explanatory variables,
-        Error function with explanatory variables
-    """
-
-    # Check inputs
-    if not isinstance(dvalues, (Raster, np.ndarray)):
-        raise ValueError('The dvalues must be a Raster or NumPy array.')
-    if stable_mask is not None and not isinstance(stable_mask, (np.ndarray, Vector, gpd.GeoDataFrame)):
-        raise ValueError('The stable mask must be a Vector, GeoDataFrame or NumPy array.')
-    if unstable_mask is not None and not isinstance(unstable_mask, (np.ndarray, Vector, gpd.GeoDataFrame)):
-        raise ValueError('The unstable mask must be a Vector, GeoDataFrame or NumPy array.')
+@overload
+def _preprocess_values_with_mask_to_array(
+    values: NDArrayf | RasterType,
+    include_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    exclude_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    gsd: float | None = None,
+    preserve_shape: bool = True,
+) -> tuple[NDArrayf, float]:
+    ...
+
+
+def _preprocess_values_with_mask_to_array(
+    values: list[NDArrayf | RasterType] | NDArrayf | RasterType,
+    include_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    exclude_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    gsd: float | None = None,
+    preserve_shape: bool = True,
+) -> tuple[list[NDArrayf] | NDArrayf, float]:
+    """
+    Preprocess input values provided as Raster or ndarray with a stable and/or unstable mask provided as Vector or
+    ndarray into an array of stable values.
+
+    By default, the shape is preserved and the masked values converted to NaNs.
+
+    :param values: Values or list of values as a Raster, array or a list of Raster/arrays
+    :param include_mask: Vector shapefile of mask to include (if values is Raster), or boolean array of same shape as
+        values
+    :param exclude_mask: Vector shapefile of mask to exclude (if values is Raster), or boolean array of same shape
+        as values
+    :param gsd: Ground sampling distance, if all the input values are provided as array
+    :param preserve_shape: If True, masks unstable values with NaN. If False, returns a 1D array of stable values.
+
+    :return: Array of stable terrain values, Ground sampling distance
+    """
+
+    # Check inputs: needs to be Raster, array or a list of those
+    if not isinstance(values, (Raster, np.ndarray, list)) or (
+        isinstance(values, list) and not all(isinstance(val, (Raster, np.ndarray)) for val in values)
+    ):
+        raise ValueError("The values must be a Raster or NumPy array, or a list of those.")
+    # Masks need to be an array, Vector or GeoPandas dataframe
+    if include_mask is not None and not isinstance(include_mask, (np.ndarray, Vector, Mask, gpd.GeoDataFrame)):
+        raise ValueError("The stable mask must be a Vector, Mask, GeoDataFrame or NumPy array.")
+    if exclude_mask is not None and not isinstance(exclude_mask, (np.ndarray, Vector, Mask, gpd.GeoDataFrame)):
+        raise ValueError("The unstable mask must be a Vector, Mask, GeoDataFrame or NumPy array.")
 
     # Check that input stable mask can only be a georeferenced vector if the proxy values are a Raster to project onto
-    if not isinstance(dvalues, Raster) and (isinstance(stable_mask, (Vector, gpd.GeoDataFrame)) or isinstance(unstable_mask,  (Vector, gpd.GeoDataFrame))):
-        raise ValueError('The stable mask can only passed as a Vector or GeoDataFrame if the input dvalues is a Raster.')
-
-    # Create placeholder variables names if those don't exist
-    if list_var_names is None:
-        list_var_names = ['var'+str(i+1) for i in range(len(list_var))]
+    if isinstance(values, list):
+        any_raster = any(isinstance(val, Raster) for val in values)
+    else:
+        any_raster = isinstance(values, Raster)
+    if not any_raster and isinstance(include_mask, (Vector, gpd.GeoDataFrame)):
+        raise ValueError(
+            "The stable mask can only passed as a Vector or GeoDataFrame if the input values contain a Raster."
+        )
 
-    # Get the arrays for proxy values and explanatory variables
-    if isinstance(dvalues, Raster):
-        dvalues_arr = get_array_and_mask(dvalues)[0]
+    # If there is only one array or Raster, put alone in a list
+    if not isinstance(values, list):
+        return_unlist = True
+        values = [values]
+    else:
+        return_unlist = False
+
+    # Get the arrays
+    values_arr = [get_array_and_mask(val)[0] if isinstance(val, Raster) else val for val in values]
+
+    # Get the ground sampling distance from the first Raster if there is one
+    if gsd is None and any_raster:
+        for i in range(len(values)):
+            if isinstance(values[i], Raster):
+                first_raster = values[i]
+                break
+        # Looks like mypy cannot trace the isinstance here... ignoring
+        gsd = first_raster.res[0]  # type: ignore
+    elif gsd is not None:
+        gsd = gsd
     else:
-        dvalues_arr = dvalues
-    list_var_arr = [get_array_and_mask(var)[0] if isinstance(var, Raster) else var
-                    for var in list_var if isinstance(var, Raster)]
+        raise ValueError("The ground sampling distance must be provided if no Raster object is passed.")
 
     # If the stable mask is not an array, create it
-    if stable_mask is None:
-        stable_mask_arr = np.ones(np.shape(dvalues_arr), dtype=bool)
-    elif not isinstance(stable_mask, np.ndarray):
+    if include_mask is None:
+        include_mask_arr = np.ones(np.shape(values_arr[0]), dtype=bool)
+    elif isinstance(include_mask, (Vector, gpd.GeoDataFrame)):
 
         # If the stable mask is a geopandas dataframe, wrap it in a Vector object
-        if isinstance(stable_mask, gpd.GeoDataFrame):
-            stable_vector = Vector(stable_mask)
+        if isinstance(include_mask, gpd.GeoDataFrame):
+            stable_vector = Vector(include_mask)
         else:
-            stable_vector = stable_mask
+            stable_vector = include_mask
 
         # Create the mask
-        stable_mask_arr = stable_vector.create_mask(dvalues)
+        include_mask_arr = stable_vector.create_mask(first_raster, as_array=True)
+    # If the mask is a Mask
+    elif isinstance(include_mask, Mask):
+        include_mask_arr = include_mask.data.filled(False)
     # If the mask is already an array, just pass it
     else:
-        stable_mask_arr = stable_mask
+        include_mask_arr = include_mask
 
     # If the unstable mask is not an array, create it
-    if unstable_mask is None:
-        unstable_mask_arr = np.zeros(np.shape(dvalues_arr), dtype=bool)
-    elif not isinstance(unstable_mask, np.ndarray):
+    if exclude_mask is None:
+        exclude_mask_arr = np.zeros(np.shape(values_arr[0]), dtype=bool)
+    elif isinstance(exclude_mask, (Vector, gpd.GeoDataFrame)):
 
         # If the unstable mask is a geopandas dataframe, wrap it in a Vector object
-        if isinstance(unstable_mask, gpd.GeoDataFrame):
-            unstable_vector = Vector(unstable_mask)
+        if isinstance(exclude_mask, gpd.GeoDataFrame):
+            unstable_vector = Vector(exclude_mask)
         else:
-            unstable_vector = unstable_mask
+            unstable_vector = exclude_mask
 
         # Create the mask
-        unstable_mask_arr = unstable_vector.create_mask(dvalues)
+        exclude_mask_arr = unstable_vector.create_mask(first_raster, as_array=True)
     # If the mask is already an array, just pass it
+    # If the mask is a Mask
+    elif isinstance(exclude_mask, Mask):
+        exclude_mask_arr = exclude_mask.data.filled(False)
     else:
-        unstable_mask_arr = unstable_mask
+        exclude_mask_arr = exclude_mask
+
+    include_mask_arr = np.logical_and(include_mask_arr, ~exclude_mask_arr).squeeze()
+
+    if preserve_shape:
+        # Need to preserve the shape, so setting as NaNs all points not on stable terrain
+        values_stable_arr = []
+        for val in values_arr:
+            val_stable = val.copy()
+            val_stable[~include_mask_arr] = np.nan
+            values_stable_arr.append(val_stable)
+    else:
+        values_stable_arr = [val_arr[include_mask_arr] for val_arr in values_arr]
+
+    # If input was a list, give a list. If it was a single array, give a single array.
+    if return_unlist:
+        values_stable_arr = values_stable_arr[0]
+
+    return values_stable_arr, gsd
+
+
+@overload
+def infer_heteroscedasticity_from_stable(
+    dvalues: NDArrayf,
+    list_var: list[NDArrayf | RasterType],
+    stable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    list_var_names: list[str] = None,
+    spread_statistic: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    list_var_bins: int | tuple[int, ...] | tuple[NDArrayf] | None = None,
+    min_count: int | None = 100,
+    fac_spread_outliers: float | None = 7,
+) -> tuple[NDArrayf, pd.DataFrame, Callable[[tuple[NDArrayf, ...]], NDArrayf]]:
+    ...
+
+
+@overload
+def infer_heteroscedasticity_from_stable(
+    dvalues: RasterType,
+    list_var: list[NDArrayf | RasterType],
+    stable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    list_var_names: list[str] = None,
+    spread_statistic: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    list_var_bins: int | tuple[int, ...] | tuple[NDArrayf] | None = None,
+    min_count: int | None = 100,
+    fac_spread_outliers: float | None = 7,
+) -> tuple[RasterType, pd.DataFrame, Callable[[tuple[NDArrayf, ...]], NDArrayf]]:
+    ...
+
+
+def infer_heteroscedasticity_from_stable(
+    dvalues: NDArrayf | RasterType,
+    list_var: list[NDArrayf | RasterType],
+    stable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    list_var_names: list[str] = None,
+    spread_statistic: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    list_var_bins: int | tuple[int, ...] | tuple[NDArrayf] | None = None,
+    min_count: int | None = 100,
+    fac_spread_outliers: float | None = 7,
+) -> tuple[NDArrayf | RasterType, pd.DataFrame, Callable[[tuple[NDArrayf, ...]], NDArrayf]]:
+    """
+    Infer heteroscedasticity from differenced values on stable terrain and a list of explanatory variables.
+
+    This function returns an error map, a dataframe of spread values and the error function with explanatory variables.
+    It is a convenience wrapper for `estimate_model_heteroscedasticity` to work on either Raster or array, compute the
+    stable mask and return an error map.
 
-    stable_mask_arr = np.logical_and(stable_mask_arr, ~unstable_mask_arr).squeeze()
+    If no stable or unstable mask is provided to mask in or out the values, all terrain is used.
+
+    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as
+        elevation differences on stable terrain)
+    :param list_var: List of size (L) of explanatory variables as array or Raster of same shape as dvalues
+    :param stable_mask: Vector shapefile of stable terrain (if dvalues is Raster), or boolean array of same shape as
+        dvalues
+    :param unstable_mask: Vector shapefile of unstable terrain (if dvalues is Raster), or boolean array of same shape
+        as dvalues
+    :param list_var_names: List of size (L) of names of the explanatory variables, otherwise named var1, var2, etc.
+    :param spread_statistic: Statistic to be computed for the spread; defaults to nmad
+    :param list_var_bins: Count of size (1), or list of size (L) of counts or custom bin edges for the explanatory
+        variables; defaults to 10 bins
+    :param min_count: Minimum number of samples to be used as a valid statistic (replaced by nodata)
+    :param fac_spread_outliers: Exclude outliers outside this spread after standardizing; pass None to ignore.
+
+    :return: Inferred error map (array or Raster, same as input proxy values),
+        Dataframe of binned spread statistic with explanatory variables,
+        Error function with explanatory variables
+    """
 
-    # Get the subsets on stable terrain
-    dvalues_stable_arr = dvalues_arr[stable_mask_arr]
-    list_var_stable_arr = [var_arr[stable_mask_arr] for var_arr in list_var_arr]
+    # Create placeholder variables names if those don't exist
+    if list_var_names is None:
+        list_var_names = ["var" + str(i + 1) for i in range(len(list_var))]
+
+    # Get the arrays for proxy values and explanatory variables
+    list_all_arr, gsd = _preprocess_values_with_mask_to_array(
+        values=[dvalues] + list_var, include_mask=stable_mask, exclude_mask=unstable_mask, preserve_shape=False
+    )
+    dvalues_stable_arr = list_all_arr[0]
+    list_var_stable_arr = list_all_arr[1:]
 
     # Estimate and model the heteroscedasticity using only stable terrain
-    df, fun = estimate_model_heteroscedasticity(dvalues=dvalues_stable_arr, list_var=list_var_stable_arr,
-                                                list_var_names=list_var_names, spread_statistic=spread_statistic,
-                                                list_var_bins=list_var_bins, min_count=min_count,
-                                                fac_spread_outliers=fac_spread_outliers)
+    df, fun = estimate_model_heteroscedasticity(
+        dvalues=dvalues_stable_arr,
+        list_var=list_var_stable_arr,
+        list_var_names=list_var_names,
+        spread_statistic=spread_statistic,
+        list_var_bins=list_var_bins,
+        min_count=min_count,
+        fac_spread_outliers=fac_spread_outliers,
+    )
 
     # Use the standardization function to get the error array for the entire input array (not only stable)
+    list_var_arr = [get_array_and_mask(var)[0] if isinstance(var, Raster) else var for var in list_var]
     error = fun(tuple(list_var_arr))
 
     # Return the right type, depending on dvalues input
     if isinstance(dvalues, Raster):
         return dvalues.copy(new_array=error), df, fun
     else:
         return error, df, fun
 
 
-def _create_circular_mask(shape: Union[int, Sequence[int]], center: Optional[list[float]] = None,
-                         radius: Optional[float] = None) -> np.ndarray:
+def _create_circular_mask(
+    shape: tuple[int, int], center: tuple[int, int] | None = None, radius: float | None = None
+) -> NDArrayf:
     """
     Create circular mask on a raster, defaults to the center of the array and its half width
 
     :param shape: shape of array
     :param center: center
     :param radius: radius
     :return:
@@ -522,298 +717,375 @@
         center = (int(w / 2), int(h / 2))
     if radius is None:  # use the smallest distance between the center and image walls
         radius = min(center[0], center[1], w - center[0], h - center[1])
 
     # Skimage disk is not inclusive (correspond to distance_from_center < radius and not <= radius)
     mask = np.zeros(shape, dtype=bool)
     with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", "invalid value encountered in true_divide")
-        rr, cc = disk(center=center,radius=radius,shape=shape)
+        warnings.filterwarnings("ignore", "invalid value encountered in *divide")
+        rr, cc = disk(center=center, radius=radius, shape=shape)
     mask[rr, cc] = True
 
     # manual solution
     # Y, X = np.ogrid[:h, :w]
     # dist_from_center = np.sqrt((X - center[0]) ** 2 + (Y - center[1]) ** 2)
     # mask = dist_from_center < radius
 
     return mask
 
-def _create_ring_mask(shape: Union[int, Sequence[int]], center: Optional[list[float]] = None, in_radius: float = 0.,
-                     out_radius: Optional[float] = None) -> np.ndarray:
+
+def _create_ring_mask(
+    shape: tuple[int, int],
+    center: tuple[int, int] | None = None,
+    in_radius: float = 0,
+    out_radius: float | None = None,
+) -> NDArrayf:
     """
     Create ring mask on a raster, defaults to the center of the array and a circle mask of half width of the array
 
     :param shape: shape of array
     :param center: center
     :param in_radius: inside radius
     :param out_radius: outside radius
     :return:
     """
 
     w, h = shape
 
-    if out_radius is None:
+    if center is None:
         center = (int(w / 2), int(h / 2))
+    if out_radius is None:
         out_radius = min(center[0], center[1], w - center[0], h - center[1])
 
     with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", "invalid value encountered in true_divide")
-        mask_inside = _create_circular_mask((w,h),center=center,radius=in_radius)
-        mask_outside = _create_circular_mask((w,h),center=center,radius=out_radius)
+        warnings.filterwarnings("ignore", "invalid value encountered in *divide")
+        mask_inside = _create_circular_mask((w, h), center=center, radius=in_radius)
+        mask_outside = _create_circular_mask((w, h), center=center, radius=out_radius)
 
-    mask_ring = np.logical_and(~mask_inside,mask_outside)
+    mask_ring = np.logical_and(~mask_inside, mask_outside)
 
     return mask_ring
 
 
-def _subsample_wrapper(values: np.ndarray, coords: np.ndarray, shape: tuple[int,int] = None, subsample: int = 10000,
-                       subsample_method: str = 'pdist_ring', inside_radius = None, outside_radius = None,
-                       random_state: None | np.random.RandomState | np.random.Generator | int = None) -> tuple[np.ndarray, np.ndarray]:
+def _random_state_definition(
+    random_state: None | np.random.RandomState | int = None,
+) -> np.random.RandomState | np.random.Generator:
     """
-    (Not used by default)
-    Wrapper for subsampling pdist methods
+    Define random state based on input
+    :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
+    :return:
     """
-    nx, ny = shape
 
-    # Define state for random subsampling (to fix results during testing)
     if random_state is None:
-        rnd = np.random.default_rng()
-    elif isinstance(random_state, (np.random.RandomState, np.random.Generator)):
+        rnd: np.random.RandomState | np.random.Generator = np.random.default_rng()
+    elif isinstance(random_state, np.random.RandomState):
         rnd = random_state
     else:
         rnd = np.random.RandomState(np.random.MT19937(np.random.SeedSequence(random_state)))
 
+    return rnd
+
+
+def _subsample_wrapper(
+    values: NDArrayf,
+    coords: NDArrayf,
+    shape: tuple[int, int],
+    subsample: int = 10000,
+    subsample_method: str = "pdist_ring",
+    inside_radius: float = 0,
+    outside_radius: float = None,
+    random_state: None | np.random.RandomState | int = None,
+) -> tuple[NDArrayf, NDArrayf]:
+    """
+    (Not used by default)
+    Wrapper for subsampling pdist methods
+    """
+    nx, ny = shape
+
+    rnd = _random_state_definition(random_state=random_state)
+
     # Subsample spatially for disk/ring methods
-    if subsample_method in ['pdist_disk', 'pdist_ring']:
+    if subsample_method in ["pdist_disk", "pdist_ring"]:
         # Select random center coordinates
         center_x = rnd.choice(nx, 1)[0]
         center_y = rnd.choice(ny, 1)[0]
-        if subsample_method == 'pdist_ring':
-            subindex = _create_ring_mask((nx, ny), center=[center_x, center_y], in_radius=inside_radius,
-                                          out_radius=outside_radius)
+        if subsample_method == "pdist_ring":
+            subindex = _create_ring_mask(
+                (nx, ny), center=(center_x, center_y), in_radius=inside_radius, out_radius=outside_radius
+            )
         else:
-            subindex = _create_circular_mask((nx, ny), center=[center_x, center_y], radius=inside_radius)
+            subindex = _create_circular_mask((nx, ny), center=(center_x, center_y), radius=outside_radius)
 
         index = subindex.flatten()
         values_sp = values[index]
         coords_sp = coords[index, :]
 
     else:
         values_sp = values
         coords_sp = coords
 
-    index = subsample_raster(values_sp, subsample=subsample, return_indices=True, random_state=rnd)
+    index = subsample_array(values_sp, subsample=subsample, return_indices=True, random_state=rnd)
     values_sub = values_sp[index[0]]
     coords_sub = coords_sp[index[0], :]
 
     return values_sub, coords_sub
 
-def _aggregate_pdist_empirical_variogram(values: np.ndarray, coords: np.ndarray, subsample: int, shape: tuple,
-                                         subsample_method: str, gsd: float,
-                                         pdist_multi_ranges: Optional[list[float]] = None, **kwargs) -> pd.DataFrame:
+
+def _aggregate_pdist_empirical_variogram(
+    values: NDArrayf,
+    coords: NDArrayf,
+    subsample: int,
+    shape: tuple[int, int],
+    subsample_method: str,
+    gsd: float,
+    pdist_multi_ranges: list[float] | None = None,
+    # **kwargs: **EmpiricalVariogramKArgs, # This will work in Python 3.12, fails in the meantime, some ignore will be
+    # removable then in this function
+    **kwargs: Any,
+) -> pd.DataFrame:
     """
     (Not used by default)
     Aggregating subfunction of sample_empirical_variogram for pdist methods.
     The pairwise differences are calculated within each subsample.
     """
 
     # If no multi_ranges are provided, define a logical default behaviour with the pixel size and grid size
-    if subsample_method in ['pdist_disk', 'pdist_ring']:
+    if subsample_method in ["pdist_disk", "pdist_ring"]:
 
         if pdist_multi_ranges is None:
 
             # Define list of ranges as exponent 2 of the resolution until the maximum range
             pdist_multi_ranges = []
             # We start at 10 times the ground sampling distance
             new_range = gsd * 10
-            while new_range < kwargs.get('maxlag') / 2:
+            while new_range < kwargs.get("maxlag") / 2:  # type: ignore
                 pdist_multi_ranges.append(new_range)
                 new_range *= 2
-            pdist_multi_ranges.append(kwargs.get('maxlag'))
-
+            pdist_multi_ranges.append(kwargs.get("maxlag"))  # type: ignore
 
         # Define subsampling parameters
-        list_inside_radius, list_outside_radius = ([] for i in range(2))
-        binned_ranges = [0] + pdist_multi_ranges
+        list_inside_radius = []
+        list_outside_radius: list[float | None] = []
+        binned_ranges = [0.0] + pdist_multi_ranges
         for i in range(len(binned_ranges) - 1):
 
             # Radiuses need to be passed as pixel sizes, dividing by ground sampling distance
-            outside_radius = binned_ranges[i + 1]/gsd
-            if subsample_method == 'pdist_ring':
-                inside_radius = binned_ranges[i]/gsd
+            outside_radius = binned_ranges[i + 1] / gsd
+            if subsample_method == "pdist_ring":
+                inside_radius = binned_ranges[i] / gsd
             else:
-                inside_radius = None
+                inside_radius = 0.0
 
             list_outside_radius.append(outside_radius)
             list_inside_radius.append(inside_radius)
     else:
         # For random point selection, no need for multi-range parameters
-        pdist_multi_ranges = [kwargs.get('maxlag')]
+        pdist_multi_ranges = [kwargs.get("maxlag")]  # type: ignore
         list_outside_radius = [None]
-        list_inside_radius = [None]
+        list_inside_radius = [0.0]
 
     # Estimate variogram with specific subsampling at multiple ranges
     list_df_range = []
     for j in range(len(pdist_multi_ranges)):
 
-        values_sub, coords_sub = _subsample_wrapper(values, coords, shape = shape, subsample = subsample,
-                                                    subsample_method = subsample_method,
-                                                    inside_radius = list_inside_radius[j],
-                                                    outside_radius = list_outside_radius[j],
-                                                    random_state= kwargs.get('random_state'))
+        values_sub, coords_sub = _subsample_wrapper(
+            values,
+            coords,
+            shape=shape,
+            subsample=subsample,
+            subsample_method=subsample_method,
+            inside_radius=list_inside_radius[j],
+            outside_radius=list_outside_radius[j],
+            random_state=kwargs.get("random_state"),
+        )
         if len(values_sub) == 0:
             continue
         df_range = _get_pdist_empirical_variogram(values=values_sub, coords=coords_sub, **kwargs)
 
         # Aggregate runs
         list_df_range.append(df_range)
 
     df = pd.concat(list_df_range)
 
     return df
 
 
-def _get_pdist_empirical_variogram(values: np.ndarray, coords: np.ndarray, **kwargs) -> pd.DataFrame:
+def _get_pdist_empirical_variogram(values: NDArrayf, coords: NDArrayf, **kwargs: Any) -> pd.DataFrame:
     """
     Get empirical variogram from skgstat.Variogram object calculating pairwise distances within the sample
 
     :param values: Values
     :param coords: Coordinates
     :return: Empirical variogram (variance, upper bound of lag bin, counts)
 
     """
 
     # Remove random_state keyword argument that is not used
-    kwargs.pop('random_state')
+    kwargs.pop("random_state")
 
     # Get arguments of Variogram class init function
-    variogram_args = skg.Variogram.__init__.__code__.co_varnames[:skg.Variogram.__init__.__code__.co_argcount]
+    variogram_args = skg.Variogram.__init__.__code__.co_varnames[: skg.Variogram.__init__.__code__.co_argcount]
     # Check no other argument is left to be passed
     remaining_kwargs = kwargs.copy()
     for arg in variogram_args:
         remaining_kwargs.pop(arg, None)
     if len(remaining_kwargs) != 0:
-        warnings.warn('Keyword arguments: '+','.join(list(remaining_kwargs.keys()))+ ' were not used.')
+        warnings.warn("Keyword arguments: " + ",".join(list(remaining_kwargs.keys())) + " were not used.")
     # Filter corresponding arguments before passing
-    filtered_kwargs =  {k:kwargs[k] for k in variogram_args if k in kwargs}
+    filtered_kwargs = {k: kwargs[k] for k in variogram_args if k in kwargs}
 
     # Derive variogram with default MetricSpace (equivalent to scipy.pdist)
     V = skg.Variogram(coordinates=coords, values=values, normalize=False, fit_method=None, **filtered_kwargs)
 
     # Get bins, empirical variogram values, and bin count
     bins, exp = V.get_empirical()
     count = V.bin_count
 
     # Write to dataframe
     df = pd.DataFrame()
     df = df.assign(exp=exp, bins=bins, count=count)
 
     return df
 
-def _choose_cdist_equidistant_sampling_parameters(**kwargs):
+
+def _choose_cdist_equidistant_sampling_parameters(**kwargs: Any) -> tuple[int, int, float]:
     """
     Add a little calculation to partition the "subsample" argument automatically into the "run" and "samples"
     arguments of RasterEquidistantMetricSpace, to have a similar number of points than with a classic pdist method.
 
+    We compute the arguments to match a N0**2/2 number of pairwise comparison, N0 being the "subsample" input, and
+    forcing the number of rings to 10 by default. This corresponds to 10 independent rings with equal number of samples
+    compared pairwise against a central disk. We force this number of sample to be at least 2 (skgstat raises an error
+    if there is only one). Additionally, if samples permit, we compute 10 independent runs, maximum 100 to limit
+    processing times when aggregating different runs in sparse matrixes. If even more sample permit (default case), we
+    increase the number of subsamples in rings and runs simultaneously.
+
     The number of pairwise samples for a classic pdist is N0(N0-1)/2 with N0 the number of samples of the ensemble. For
     the cdist equidistant calculation it is M*N*R where N are the subsamples in the center disk, M is the number of
     samples in the rings which amounts to X*N where X is the number of rings in the grid extent, as each ring draws N
     samples. And R is the number of runs with a different random center point.
-    X is fixed by the extent and ratio_subsample parameters, and so N0**2/(2X) = N**2*R, and we want at least 30 runs
-    with 10 subsamples.
+    X is fixed by the extent and ratio_subsample parameters, and so N0**2/2 = R*X*N**2, and we want at least 10 rings
+    and, if possible, 10 runs.
+
+    !! Different variables: !! The "samples" of RasterEquidistantMetricSpace is N, while the "subsample" passed is N0.
     """
 
     # First, we extract the extent, shape and subsample values from the keyword arguments
-    extent = kwargs['extent']
-    shape = kwargs['shape']
-    subsample = kwargs['subsample']
-    # We derive the maximum distance and resolution automatically derived in skgstat.RasterEquidistantMetricSpace
+    extent = kwargs["extent"]
+    shape = kwargs["shape"]
+    subsample = kwargs["subsample"]
+
+    # We define the number of rings to 10 in order to get a decent equidistant sampling, we'll later adjust the
+    # ratio_sampling to force that number to 10
+    if "nb_rings" in kwargs.keys():
+        nb_rings = kwargs["nb_rings"]
+    else:
+        nb_rings = 10
+    # For one run (R=1), and two samples per disk/ring (N=2), and the number of rings X=10, this requires N0 to be at
+    # least 10:
+    min_subsample = np.ceil(np.sqrt(2 * nb_rings * 2**2) + 1)
+    if subsample < min_subsample:
+        raise ValueError(f"The number of subsamples needs to be at least {min_subsample:.0f}.")
+
+    # The pairwise comparisons can be deduced from the number of rings: R * N**2 = N0**2/(2*X)
+    pairwise_comp_per_disk = np.ceil(subsample**2 / (2 * nb_rings))
+
+    # With R*N**2 = N0**2/2, and minimum 2 samples N, we compute the number of runs R forcing at least
+    # 10 runs and maximum 100
+    if pairwise_comp_per_disk < 10:
+        runs = int(pairwise_comp_per_disk / 2**2)
+    else:
+        runs = int(min(100, 10 * np.ceil((pairwise_comp_per_disk / (2**2 * 10)) ** (1 / 3))))
+
+    # Now we can derive the number of samples N, which will always be at least 2
+    subsample_per_disk_per_run = int(np.ceil(np.sqrt(pairwise_comp_per_disk / runs)))
+
+    # Finally, we need to force the ratio_subsample to get exactly 10 rings
+
+    # We first derive the maximum distance and resolution the same way as in skgstat.RasterEquidistantMetricSpace
     maxdist = np.sqrt((extent[1] - extent[0]) ** 2 + (extent[3] - extent[2]) ** 2)
     res = np.mean([(extent[1] - extent[0]) / (shape[0] - 1), (extent[3] - extent[2]) / (shape[1] - 1)])
-    # Then, we compute the radius from the center ensemble with the default value of subsample ratio in the function
-    # skgstat.RasterEquidistantMetricSpace
-    ratio_subsample = 0.2
-    center_radius = np.sqrt(1. / ratio_subsample * subsample / np.pi) * res
-    # Now, we can derive the number of successive disks that are going to be sampled in the grid
-    equidistant_radii = [0.]
-    increasing_rad = center_radius
-    while increasing_rad < maxdist:
-        equidistant_radii.append(increasing_rad)
-        increasing_rad *= np.sqrt(2)
-    nb_disk_samples = len(equidistant_radii)
-
-    # We divide the number of samples by the number of disks
-    pairwise_comp_per_disk = np.ceil(subsample**2 / (2*nb_disk_samples))
-
-    # Using the equation in the function description, we compute the number of runs (minimum 30)
-    runs = int(max(np.ceil(pairwise_comp_per_disk**(1/3)), 30))
-    # Then we deduce the number of samples per disk (and per ring)
-    subsample_per_disk_per_run = int(np.ceil(np.sqrt(pairwise_comp_per_disk/runs)))
-
-    final_pairwise_comparisons = runs*subsample_per_disk_per_run**2*nb_disk_samples
-
-    if kwargs['verbose']:
-        print('Equidistant circular sampling will be performed for {} runs (random center points) with pairwise '
-              'comparison between {} samples (points) of the central disk and again {} samples times {} independent '
-              'rings centered on the same center point. This results in approximately {} pairwise comparisons (duplicate'
-              ' pairwise points randomly selected will be removed).'.format(runs, subsample_per_disk_per_run,
-                                                                            subsample_per_disk_per_run, nb_disk_samples,
-                                                                            final_pairwise_comparisons))
 
-    return runs, subsample_per_disk_per_run
-
-def _get_cdist_empirical_variogram(values: np.ndarray, coords: np.ndarray, subsample_method: str,
-                                   **kwargs) -> pd.DataFrame:
+    # Then, we derive the subsample ratio. We have:
+    # 1) radius * sqrt(2)**X = maxdist, and
+    # 2) pi * radius**2 = res**2 * N / sub_ratio
+    # From which we can deduce: sub_ratio = res**2 * N / (pi * maxdist**2 / sqrt(2)**(2X) )
+    ratio_subsample = res**2 * subsample_per_disk_per_run / (np.pi * maxdist**2 / np.sqrt(2) ** (2 * nb_rings))
+
+    # And the number of total pairwise comparison
+    total_pairwise_comparison = runs * subsample_per_disk_per_run**2 * nb_rings
+
+    if kwargs["verbose"]:
+        print(
+            "Equidistant circular sampling will be performed for {} runs (random center points) with pairwise "
+            "comparison between {} samples (points) of the central disk and again {} samples times {} independent "
+            "rings centered on the same center point. This results in approximately {} pairwise comparisons (duplicate"
+            " pairwise points randomly selected will be removed).".format(
+                runs, subsample_per_disk_per_run, subsample_per_disk_per_run, nb_rings, total_pairwise_comparison
+            )
+        )
+
+    return runs, subsample_per_disk_per_run, ratio_subsample
+
+
+def _get_cdist_empirical_variogram(
+    values: NDArrayf, coords: NDArrayf, subsample_method: str, **kwargs: Any
+) -> pd.DataFrame:
     """
     Get empirical variogram from skgstat.Variogram object calculating pairwise distances between two sample collections
     of a MetricSpace (see scikit-gstat documentation for more details)
 
     :param values: Values
     :param coords: Coordinates
     :return: Empirical variogram (variance, upper bound of lag bin, counts)
 
     """
 
-    if subsample_method == 'cdist_equidistant' and 'runs' not in kwargs.keys() and 'samples' not in kwargs.keys():
+    if subsample_method == "cdist_equidistant" and "runs" not in kwargs.keys() and "samples" not in kwargs.keys():
 
         # We define subparameters for the equidistant technique to match the number of pairwise comparison
         # that would have a classic "subsample" with pdist, except if those parameters are already user-defined
-        runs, samples = _choose_cdist_equidistant_sampling_parameters(**kwargs)
+        runs, samples, ratio_subsample = _choose_cdist_equidistant_sampling_parameters(**kwargs)
 
-        kwargs['runs'] = runs
+        kwargs["runs"] = runs
         # The "samples" argument is used by skgstat Metric subclasses (and not "subsample")
-        kwargs['samples'] = samples
-        kwargs.pop('subsample')
+        kwargs["samples"] = samples
+        kwargs["ratio_subsample"] = ratio_subsample
+        kwargs.pop("subsample")
 
-    elif subsample_method == 'cdist_point':
+    elif subsample_method == "cdist_point":
 
         # We set the samples to match the subsample argument if the method is random points
-        kwargs['samples'] = kwargs.pop('subsample')
+        kwargs["samples"] = kwargs.pop("subsample")
 
     # Rename the "random_state" argument into "rnd", also used by skgstat Metric subclasses
-    kwargs['rnd'] = kwargs.pop('random_state')
+    kwargs["rnd"] = kwargs.pop("random_state")
 
     # Define MetricSpace function to be used, fetch possible keywords arguments
-    if subsample_method == 'cdist_point':
+    if subsample_method == "cdist_point":
         # List keyword arguments of the Probabilistic class init function
-        ms_args = skg.ProbabalisticMetricSpace.__init__.__code__.co_varnames[:skg.ProbabalisticMetricSpace.__init__.__code__.co_argcount]
+        ms_args = skg.ProbabalisticMetricSpace.__init__.__code__.co_varnames[
+            : skg.ProbabalisticMetricSpace.__init__.__code__.co_argcount
+        ]
         ms = skg.ProbabalisticMetricSpace
     else:
         # List keyword arguments of the RasterEquidistant class init function
-        ms_args = skg.RasterEquidistantMetricSpace.__init__.__code__.co_varnames[:skg.RasterEquidistantMetricSpace.__init__.__code__.co_argcount]
+        ms_args = skg.RasterEquidistantMetricSpace.__init__.__code__.co_varnames[
+            : skg.RasterEquidistantMetricSpace.__init__.__code__.co_argcount
+        ]
         ms = skg.RasterEquidistantMetricSpace
 
     # Get arguments of Variogram class init function
-    variogram_args = skg.Variogram.__init__.__code__.co_varnames[:skg.Variogram.__init__.__code__.co_argcount]
+    variogram_args = skg.Variogram.__init__.__code__.co_varnames[: skg.Variogram.__init__.__code__.co_argcount]
     # Check no other argument is left to be passed, accounting for MetricSpace arguments
     remaining_kwargs = kwargs.copy()
     for arg in variogram_args + ms_args:
         remaining_kwargs.pop(arg, None)
     if len(remaining_kwargs) != 0:
-        warnings.warn('Keyword arguments: ' + ', '.join(list(remaining_kwargs.keys())) + ' were not used.')
+        warnings.warn("Keyword arguments: " + ", ".join(list(remaining_kwargs.keys())) + " were not used.")
 
     # Filter corresponding arguments before passing to MetricSpace function
     filtered_ms_kwargs = {k: kwargs[k] for k in ms_args if k in kwargs}
     M = ms(coords=coords, **filtered_ms_kwargs)
 
     # Filter corresponding arguments before passing to Variogram function
     filtered_var_kwargs = {k: kwargs[k] for k in variogram_args if k in kwargs}
@@ -826,69 +1098,89 @@
     # Write to dataframe
     df = pd.DataFrame()
     df = df.assign(exp=exp, bins=bins, count=count)
 
     return df
 
 
-def _wrapper_get_empirical_variogram(argdict: dict) -> pd.DataFrame:
+def _wrapper_get_empirical_variogram(argdict: dict[str, Any]) -> pd.DataFrame:
     """
     Multiprocessing wrapper for get_pdist_empirical_variogram and get_cdist_empirical variogram
 
     :param argdict: Keyword argument to pass to get_pdist/cdist_empirical_variogram
     :return: Empirical variogram (variance, upper bound of lag bin, counts)
 
     """
-    if argdict['verbose']:
-        print('Working on run '+str(argdict['i']) + ' out of '+str(argdict['imax']))
-    argdict.pop('i')
-    argdict.pop('imax')
+    if argdict["verbose"]:
+        print("Working on run " + str(argdict["i"]) + " out of " + str(argdict["imax"]))
+    argdict.pop("i")
+    argdict.pop("imax")
 
-    if argdict['subsample_method'] in ['cdist_equidistant', 'cdist_point']:
+    if argdict["subsample_method"] in ["cdist_equidistant", "cdist_point"]:
         # Simple wrapper for the skgstat Variogram function for cdist methods
-        get_variogram = _get_cdist_empirical_variogram
+        return _get_cdist_empirical_variogram(**argdict)
     else:
         # Aggregating several skgstat Variogram after iterative subsampling of specific points in the Raster
-        get_variogram = _aggregate_pdist_empirical_variogram
-
-    return get_variogram(**argdict)
+        return _aggregate_pdist_empirical_variogram(**argdict)
 
 
-def sample_empirical_variogram(values: Union[np.ndarray, RasterType], gsd: float = None, coords: np.ndarray = None,
-                               subsample: int = 1000, subsample_method: str = 'cdist_equidistant',
-                               n_variograms: int = 1, n_jobs: int = 1, verbose = False,
-                               random_state: None | np.random.RandomState | np.random.Generator | int = None,
-                               **kwargs) -> pd.DataFrame:
+class EmpiricalVariogramKArgs(TypedDict, total=False):
+    runs: int
+    pdist_multi_ranges: list[float]
+    ratio_subsample: float
+    samples: int
+    nb_rings: int
+    maxlag: float
+    bin_func: Any
+    estimator: str
+
+
+def sample_empirical_variogram(
+    values: NDArrayf | RasterType,
+    gsd: float = None,
+    coords: NDArrayf = None,
+    subsample: int = 1000,
+    subsample_method: str = "cdist_equidistant",
+    n_variograms: int = 1,
+    n_jobs: int = 1,
+    verbose: bool = False,
+    random_state: None | np.random.RandomState | int = None,
+    # **kwargs: **EmpiricalVariogramKArgs, # This will work in Python 3.12, fails in the meantime, we'll be able to
+    # remove some type ignores from this function in the future
+    **kwargs: int | list[float] | float | str | Any,
+) -> pd.DataFrame:
     """
-    Sample empirical variograms with binning adaptable to multiple ranges and spatial subsampling adapted for raster data.
+    Sample empirical variograms with binning adaptable to multiple ranges and spatial subsampling adapted for raster
+    data.
     Returns an empirical variogram (empirical variance, upper bound of spatial lag bin, count of pairwise samples).
 
+    If values are provided as a Raster subclass, nothing else is required.
+    If values are provided as a 2D array (M,N), a ground sampling distance is sufficient to derive the pairwise
+    distances.
+    If values are provided as a 1D array (N), an array of coordinates (N,2) or (2,N) is expected. If the coordinates
+    do not correspond to points of a grid, a ground sampling distance is needed to correctly get the grid size.
+
     By default, the subsampling is based on RasterEquidistantMetricSpace implemented in scikit-gstat. This method
     samples more effectively large grid data by isolating pairs of spatially equidistant ensembles for distributed
     pairwise comparison. In practice, two subsamples are drawn for pairwise comparison: one from a disk of certain
     radius within the grid, and another one from rings of larger radii that increase steadily between the pixel size
     and the extent of the raster. Those disks and rings are sampled several times across the grid using random centers.
-
     See more details in Hugonnet et al. (2022), https://doi.org/10.1109/jstars.2022.3188922, in particular on
     Supplementary Fig. 13. for the subsampling scheme.
 
     The "subsample" argument determines the number of samples for each method to yield a number of pairwise comparisons
     close to that of a pdist calculation, that is N*(N-1)/2 where N is the subsample argument.
     For the cdist equidistant method, the "runs" (random centers) and "samples" (subsample of a disk/ring) are set
-    automatically to get close to N*(N-1)/2 pairwise samples. But those can be more finely adjusted by passing the
-    argument "runs", "samples" and "ratio_subsample" to kwargs. Further details can be found in the description of
-    skgstat.MetricSpace.RasterEquidistantMetricSpace.
-
-    If values are provided as a Raster subclass, nothing else is required.
-    If values are provided as a 2D array (M,N), a ground sampling distance is sufficient to derive the pairwise distances.
-    If values are provided as a 1D array (N), an array of coordinates (N,2) or (2,N) is expected. If the coordinates
-    do not correspond to points of a grid, a ground sampling distance is needed to correctly get the grid size.
+    automatically to get close to N*(N-1)/2 pairwise samples, fixing a number of rings "nb_rings" to 10. Those can be
+    more finely adjusted by passing the argument "runs", "samples" and "nb_rings" to kwargs. Further details can be
+    found in the description of skgstat.MetricSpace.RasterEquidistantMetricSpace or
+    _choose_cdist_equidistant_sampling_parameters.
 
-    Spatial subsampling method argument subsample_method can be one of "cdist_equidistant", "cdist_point", "pdist_point",
-    "pdist_disk" and "pdist_ring".
+    Spatial subsampling method argument subsample_method can be one of "cdist_equidistant", "cdist_point",
+    "pdist_point", "pdist_disk" and "pdist_ring".
     The cdist methods use MetricSpace classes of scikit-gstat and do pairwise comparison between two distinct ensembles
     as in scipy.spatial.cdist. For the cdist methods, the variogram is estimated in a single run from the MetricSpace.
 
     The pdist methods use methods to subsample the Raster points directly and do pairwise comparison within a single
     ensemble as in scipy.spatial.pdist. For the pdist methods, an iterative process is required: a list of ranges
     subsampled independently is used.
 
@@ -910,42 +1202,48 @@
     :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
 
     :return: Empirical variogram (variance, upper bound of lag bin, counts)
     """
     # First, check all that the values provided are OK
     if isinstance(values, Raster):
         gsd = values.res[0]
-        values, mask = get_array_and_mask(values.data)
+        values, mask = get_array_and_mask(values)
     elif isinstance(values, (np.ndarray, np.ma.masked_array)):
         values, mask = get_array_and_mask(values)
     else:
-        raise ValueError('Values must be of type np.ndarray, np.ma.masked_array or Raster subclass.')
+        raise ValueError("Values must be of type NDArrayf, np.ma.masked_array or Raster subclass.")
     values = values.squeeze()
 
     # Then, check if the logic between values, coords and gsd is respected
-    if (gsd is not None or subsample_method in ['cdist_equidistant', 'pdist_disk','pdist_ring']) and values.ndim == 1:
-        raise ValueError('Values array must be 2D when using any of the "cdist_equidistant", "pdist_disk" and '
-                        '"pdist_ring" methods, or providing a ground sampling distance instead of coordinates.')
+    if (gsd is not None or subsample_method in ["cdist_equidistant", "pdist_disk", "pdist_ring"]) and values.ndim == 1:
+        raise ValueError(
+            'Values array must be 2D when using any of the "cdist_equidistant", "pdist_disk" and '
+            '"pdist_ring" methods, or providing a ground sampling distance instead of coordinates.'
+        )
     elif coords is not None and values.ndim != 1:
-        raise ValueError('Values array must be 1D when providing coordinates.')
+        raise ValueError("Values array must be 1D when providing coordinates.")
     elif coords is not None and (coords.shape[0] != 2 and coords.shape[1] != 2):
-        raise ValueError('The coordinates array must have one dimension with length equal to 2')
+        raise ValueError("The coordinates array must have one dimension with length equal to 2")
     elif values.ndim == 2 and gsd is None:
-        raise ValueError('The ground sampling distance must be defined when passing a 2D values array.')
+        raise ValueError("The ground sampling distance must be defined when passing a 2D values array.")
 
     # Check the subsample method provided exists, otherwise list options
-    if subsample_method not in ['cdist_equidistant','cdist_point','pdist_point','pdist_disk','pdist_ring']:
-        raise TypeError('The subsampling method must be one of "cdist_equidistant, "cdist_point", "pdist_point", '
-                        '"pdist_disk" or "pdist_ring".')
+    if subsample_method not in ["cdist_equidistant", "cdist_point", "pdist_point", "pdist_disk", "pdist_ring"]:
+        raise TypeError(
+            'The subsampling method must be one of "cdist_equidistant, "cdist_point", "pdist_point", '
+            '"pdist_disk" or "pdist_ring".'
+        )
     # Check that, for several runs, the binning function is an Iterable, otherwise skgstat might provide variogram
     # values over slightly different binnings due to randomly changing subsample maximum lags
-    if n_variograms > 1 and 'bin_func' in kwargs.keys() and not isinstance(kwargs.get('bin_func'), Iterable):
-        warnings.warn('Using a named binning function of scikit-gstat might provide different binnings for each '
-                      'independent run. To remediate that issue, pass bin_func as an Iterable of right bin edges, '
-                      '(or use default bin_func).')
+    if n_variograms > 1 and "bin_func" in kwargs.keys() and not isinstance(kwargs.get("bin_func"), Iterable):
+        warnings.warn(
+            "Using a named binning function of scikit-gstat might provide different binnings for each "
+            "independent run. To remediate that issue, pass bin_func as an Iterable of right bin edges, "
+            "(or use default bin_func)."
+        )
 
     # Defaulting to coordinates if those are provided
     if coords is not None:
         nx = None
         ny = None
         # Making the shape of coordinates consistent if they are transposed
         if coords.shape[0] == 2 and coords.shape[1] != 2:
@@ -961,561 +1259,593 @@
     # Get the ground sampling distance from the coordinates before keeping only valid data, if it was not provided
     if gsd is None:
         gsd = np.mean([coords[0, 0] - coords[0, 1], coords[0, 0] - coords[1, 0]])
     # Get extent
     extent = (np.min(coords[:, 0]), np.max(coords[:, 0]), np.min(coords[:, 1]), np.max(coords[:, 1]))
 
     # Get the maximum lag from the coordinates before keeping only valid data, if it was not provided
-    if 'maxlag' not in kwargs.keys():
+    if "maxlag" not in kwargs.keys():
         # We define maximum lag as the maximum distance between coordinates (needed to provide custom bins, otherwise
         # skgstat rewrites the maxlag with the subsample of coordinates provided)
-        maxlag = np.sqrt((np.max(coords[:, 0])-np.min(coords[:, 1]))**2
-                         + (np.max(coords[:, 1]) - np.min(coords[:, 1]))**2)
-        kwargs.update({'maxlag': maxlag})
+        maxlag = np.sqrt(
+            (np.max(coords[:, 0]) - np.min(coords[:, 0])) ** 2 + (np.max(coords[:, 1]) - np.min(coords[:, 1])) ** 2
+        )
+        kwargs.update({"maxlag": maxlag})
 
     # Keep only valid data for cdist methods, remove later for pdist methods
-    if 'cdist' in subsample_method:
+    if "cdist" in subsample_method:
         ind_valid = np.isfinite(values)
         values = values[ind_valid]
         coords = coords[ind_valid, :]
 
-    if 'bin_func' not in kwargs.keys():
+    if "bin_func" not in kwargs.keys():
         # If no bin_func is provided, we provide an Iterable to provide a custom binning function to skgstat,
-        # because otherwise bins might be unconsistent across runs
+        # because otherwise bins might be inconsistent across runs
         bin_func = []
         right_bin_edge = np.sqrt(2) * gsd
-        while right_bin_edge < kwargs.get('maxlag'):
+        while right_bin_edge < kwargs.get("maxlag"):
             bin_func.append(right_bin_edge)
             # We use the default exponential increasing factor of RasterEquidistantMetricSpace, adapted for grids
             right_bin_edge *= np.sqrt(2)
-        bin_func.append(kwargs.get('maxlag'))
-        kwargs.update({'bin_func': bin_func})
+        bin_func.append(kwargs.get("maxlag"))
+        kwargs.update({"bin_func": bin_func})
 
     # Prepare necessary arguments to pass to variogram subfunctions
-    args = {'values': values, 'coords': coords, 'subsample_method': subsample_method, 'subsample': subsample,
-            'verbose': verbose}
-    if subsample_method in ['cdist_equidistant','pdist_ring','pdist_disk', 'pdist_point']:
+    args = {
+        "values": values,
+        "coords": coords,
+        "subsample_method": subsample_method,
+        "subsample": subsample,
+        "verbose": verbose,
+    }
+    if subsample_method in ["cdist_equidistant", "pdist_ring", "pdist_disk", "pdist_point"]:
         # The shape is needed for those three methods
-        args.update({'shape': (nx, ny)})
-        if subsample_method == 'cdist_equidistant':
+        args.update({"shape": (nx, ny)})
+        if subsample_method == "cdist_equidistant":
             # The coordinate extent is needed for this method
-            args.update({'extent':extent})
+            args.update({"extent": extent})
         else:
-            args.update({'gsd': gsd})
+            args.update({"gsd": gsd})
 
     # If a random_state is passed, each run needs to be passed an independent child random state, otherwise they will
     # provide exactly the same sampling and results
     if random_state is not None:
         # Define the random state if only a seed is provided
-        if isinstance(random_state, (np.random.RandomState, np.random.Generator)):
+        if isinstance(random_state, np.random.RandomState):
             rnd = random_state
+        elif isinstance(random_state, np.random.Generator):
+            rnd = np.random.RandomState(random_state)
         else:
             rnd = np.random.RandomState(np.random.MT19937(np.random.SeedSequence(random_state)))
 
         # Create a list of child random states
         if n_variograms == 1:
             # No issue if there is only one variogram run
-            list_random_state = [rnd]
+            list_random_state: list[None | np.random.RandomState] = [rnd]
         else:
             # Otherwise, pass a list of seeds
             list_random_state = list(rnd.choice(n_variograms, n_variograms, replace=False))
     else:
         list_random_state = [None for i in range(n_variograms)]
 
     # Derive the variogram
     # Differentiate between 1 core and several cores for multiple runs
     # All variogram runs have random sampling inherent to their subfunctions, so we provide the same input arguments
     if n_jobs == 1:
         if verbose:
-            print('Using 1 core...')
+            print("Using 1 core...")
 
         list_df_run = []
         for i in range(n_variograms):
 
-            argdict = {'i': i, 'imax': n_variograms, 'random_state': list_random_state[i], **args, **kwargs}
+            argdict = {
+                "i": i,
+                "imax": n_variograms,
+                "random_state": list_random_state[i],
+                **args,
+                **kwargs,  # type: ignore
+            }
             df_run = _wrapper_get_empirical_variogram(argdict=argdict)
 
             list_df_run.append(df_run)
     else:
         if verbose:
-            print('Using ' + str(n_jobs) + ' cores...')
+            print("Using " + str(n_jobs) + " cores...")
 
         pool = mp.Pool(n_jobs, maxtasksperchild=1)
-        argdict = [{'i': i, 'imax': n_variograms, 'random_state': list_random_state[i], **args, **kwargs} for i in range(n_variograms)]
-        list_df_run = pool.map(_wrapper_get_empirical_variogram, argdict, chunksize=1)
+        list_argdict = [
+            {"i": i, "imax": n_variograms, "random_state": list_random_state[i], **args, **kwargs}  # type: ignore
+            for i in range(n_variograms)
+        ]
+        list_df_run = pool.map(_wrapper_get_empirical_variogram, list_argdict, chunksize=1)
         pool.close()
         pool.join()
 
     # Aggregate multiple ranges subsampling
     df = pd.concat(list_df_run)
 
     # For a single run, no multi-run sigma estimated
     if n_variograms == 1:
-        df = df.rename(columns={'bins': 'lags'})
-        df['err_exp'] = np.nan
+        df = df.rename(columns={"bins": "lags"})
+        df["err_exp"] = np.nan
     # For several runs, group results, use mean as empirical variogram, estimate sigma, and sum the counts
     else:
-        df_grouped = df.groupby('bins', dropna=False)
-        df_mean = df_grouped[['exp']].mean()
-        df_std = df_grouped[['exp']].std()
-        df_count = df_grouped[['count']].sum()
-        df_mean['lags'] = df_mean.index.values
-        df_mean['err_exp'] = df_std['exp'] / np.sqrt(n_variograms)
-        df_mean['count'] = df_count['count']
+        df_grouped = df.groupby("bins", dropna=False)
+        df_mean = df_grouped[["exp"]].mean()
+        df_std = df_grouped[["exp"]].std()
+        df_count = df_grouped[["count"]].sum()
+        df_mean["lags"] = df_mean.index.values
+        df_mean["err_exp"] = df_std["exp"] / np.sqrt(n_variograms)
+        df_mean["count"] = df_count["count"]
         df = df_mean
 
     # Remove the last spatial lag bin which is always undersampled
-    # TODO: Solve this problem at the root: how the spatial lag binning is defined, probably?
     df.drop(df.tail(1).index, inplace=True)
 
+    # Force output dtype (default differs on different OS)
+    df = df.astype({"exp": "float64", "err_exp": "float64", "lags": "float64", "count": "int64"})
+
     return df
 
-def _get_skgstat_variogram_model_name(model: str | Callable) -> str:
-    """Fonction to identify a SciKit-GStat variogram model from a string or a function"""
 
-    list_supported_models = ['spherical', 'gaussian', 'exponential', 'cubic', 'stable', 'matern']
+def _get_skgstat_variogram_model_name(model: str | Callable[[NDArrayf, float, float], NDArrayf]) -> str:
+    """Function to identify a SciKit-GStat variogram model from a string or a function"""
+
+    list_supported_models = ["spherical", "gaussian", "exponential", "cubic", "stable", "matern"]
 
     if callable(model):
-        if inspect.getmodule(model).__name__ == 'skgstat.models':
+        if inspect.getmodule(model).__name__ == "skgstat.models":  # type: ignore
             model_name = model.__name__
         else:
-            raise ValueError('Variogram models can only be passed as functions of the skgstat.models package.')
+            raise ValueError("Variogram models can only be passed as functions of the skgstat.models package.")
 
     elif isinstance(model, str):
-        model_name = None
+        model_name = "None"
         for supp_model in list_supported_models:
             if model.lower() in [supp_model[0:3], supp_model]:
                 model_name = supp_model.lower()
-        if model_name is None:
-            raise ValueError('Variogram model name {} not recognized. Supported models are: '.format(model)+
-                             ', '.join(list_supported_models)+'.')
+        if model_name == "None":
+            raise ValueError(
+                f"Variogram model name {model} not recognized. Supported models are: "
+                + ", ".join(list_supported_models)
+                + "."
+            )
 
     else:
-        raise ValueError('Variogram models can be passed as strings or skgstat.models function. '
-                         'Supported models are: '+', '.join(list_supported_models)+'.')
+        raise ValueError(
+            "Variogram models can be passed as strings or skgstat.models function. "
+            "Supported models are: " + ", ".join(list_supported_models) + "."
+        )
 
     return model_name
 
-def get_variogram_model_func(params_variogram_model: pd.DataFrame) -> Callable[[np.ndarray], np.ndarray]:
+
+def get_variogram_model_func(params_variogram_model: pd.DataFrame) -> Callable[[NDArrayf], NDArrayf]:
     """
     Construct the sum of spatial variogram function from a dataframe of variogram parameters.
 
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
 
     :return: Function of sum of variogram with spatial lags.
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
     # Define the function of sum of variogram models of h (spatial lag) to return
-    def sum_model(h: np.ndarray) -> np.ndarray:
+    def sum_model(h: NDArrayf) -> NDArrayf:
 
         fn = np.zeros(np.shape(h))
 
         for i in range(len(params_variogram_model)):
             # Get scikit-gstat model from name or Callable
-            model_name = _get_skgstat_variogram_model_name(params_variogram_model['model'].values[i])
+            model_name = _get_skgstat_variogram_model_name(params_variogram_model["model"].values[i])
             model_function = getattr(skg.models, model_name)
-            r = params_variogram_model['range'].values[i]
-            p = params_variogram_model['psill'].values[i]
+            r = params_variogram_model["range"].values[i]
+            p = params_variogram_model["psill"].values[i]
             # For models that expect 2 parameters
-            if model_name in ['spherical', 'gaussian', 'exponential', 'cubic']:
+            if model_name in ["spherical", "gaussian", "exponential", "cubic"]:
                 fn += model_function(h, r, p)
             # For models that expect 3 parameters
-            elif model_name in ['stable', 'matern']:
-                s = params_variogram_model['smooth'].values[i]
+            elif model_name in ["stable", "matern"]:
+                s = params_variogram_model["smooth"].values[i]
                 fn += model_function(h, r, p, s)
         return fn
 
     return sum_model
 
-def covariance_from_variogram(params_variogram_model: pd.DataFrame) -> Callable[[np.ndarray], np.ndarray]:
+
+def covariance_from_variogram(params_variogram_model: pd.DataFrame) -> Callable[[NDArrayf], NDArrayf]:
     """
     Construct the spatial covariance function from a dataframe of variogram parameters.
     The covariance function is the sum of partial sills "PS" minus the sum of associated variograms "gamma":
     C = PS - gamma
 
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
 
     :return: Covariance function with spatial lags
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
     # Get total sill
-    total_sill = np.sum(params_variogram_model['psill'])
+    total_sill = np.sum(params_variogram_model["psill"])
 
     # Get function from sum of variogram
     sum_variogram = get_variogram_model_func(params_variogram_model)
 
-    def cov(h):
+    def cov(h: NDArrayf) -> NDArrayf:
         return total_sill - sum_variogram(h)
 
     return cov
 
-def correlation_from_variogram(params_variogram_model: pd.DataFrame)-> Callable[[np.ndarray], np.ndarray]:
+
+def correlation_from_variogram(params_variogram_model: pd.DataFrame) -> Callable[[NDArrayf], NDArrayf]:
     """
     Construct the spatial correlation function from a dataframe of variogram parameters.
     The correlation function is the covariance function "C" divided by the sum of partial sills "PS": rho = C / PS
 
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
 
     :return: Correlation function with spatial lags
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
     # Get total sill
-    total_sill = np.sum(params_variogram_model['psill'].values)
+    total_sill = np.sum(params_variogram_model["psill"].values)
 
     # Get covariance from sum of variogram
     cov = covariance_from_variogram(params_variogram_model)
 
-    def rho(h):
-        return cov(h)/total_sill
+    def rho(h: NDArrayf) -> NDArrayf:
+        return cov(h) / total_sill
 
     return rho
 
 
-def fit_sum_model_variogram(list_models: list[str | Callable], empirical_variogram: pd.DataFrame,
-                            bounds: list[tuple[float, float]] = None,
-                            p0: list[float] = None) -> tuple[Callable[[np.ndarray], np.ndarray], pd.DataFrame]:
+def fit_sum_model_variogram(
+    list_models: list[str | Callable[[NDArrayf, float, float], NDArrayf]],
+    empirical_variogram: pd.DataFrame,
+    bounds: list[tuple[float, float]] = None,
+    p0: list[float] = None,
+) -> tuple[Callable[[NDArrayf], NDArrayf], pd.DataFrame]:
     """
     Fit a sum of variogram models to an empirical variogram, with weighted least-squares based on sampling errors. To
     use preferably with the empirical variogram dataframe returned by the `sample_empirical_variogram` function.
 
     :param list_models: List of K variogram models to sum for the fit in order from short to long ranges. Can either be
         a 3-letter string, full string of the variogram name or SciKit-GStat model function (e.g., for a
         spherical model "Sph", "Spherical" or skgstat.models.spherical).
     :param empirical_variogram: Empirical variogram, formatted as a dataframe with count (pairwise sample count), lags
         (upper bound of spatial lag bin), exp (experimental variance), and err_exp (error on experimental variance).
-    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper, sill lower, sill upper).
+    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper, sill
+        lower, sill upper).
     :param p0: Initial guess of ranges and sills each model (shape K x 2 = K x range first guess, sill first guess).
 
     :return: Function of sum of variogram, Dataframe of optimized coefficients.
     """
 
     # Define a function of a sum of variogram model forms, with undetermined arguments
-    def variogram_sum(h, *args):
-        fn = 0
+    def variogram_sum(h: float, *args: list[float]) -> float:
+        fn = 0.0
         i = 0
         for model in list_models:
             # Get the model name and convert to SciKit-GStat function
             model_name = _get_skgstat_variogram_model_name(model)
             model_function = getattr(skg.models, model_name)
             # For models that expect 2 parameters
-            if model_name in ['spherical', 'gaussian', 'exponential', 'cubic']:
-                fn += model_function(h, args[i], args[i+1])
+            if model_name in ["spherical", "gaussian", "exponential", "cubic"]:
+                fn += model_function(h, args[i], args[i + 1])
                 i += 2
             # For models that expect 3 parameters
-            elif model_name in ['stable', 'matern']:
-                fn += model_function(h, args[i], args[i+1], args[i+2])
+            elif model_name in ["stable", "matern"]:
+                fn += model_function(h, args[i], args[i + 1], args[i + 2])
                 i += 3
 
         return fn
 
     # First, filter outliers
     empirical_variogram = empirical_variogram[np.isfinite(empirical_variogram.exp.values)]
 
     # Use shape of empirical variogram to assess rough boundaries/first estimates
     n_average = np.ceil(len(empirical_variogram.exp.values) / 10)
-    exp_movaverage = np.convolve(empirical_variogram.exp.values, np.ones(int(n_average)) / n_average, mode='valid')
-    grad = np.gradient(exp_movaverage, 2)
+    exp_movaverage = np.convolve(empirical_variogram.exp.values, np.ones(int(n_average)) / n_average, mode="valid")
     # Maximum variance of the process
     max_var = np.max(exp_movaverage)
 
     # Simplify things for scipy: let's provide boundaries and first guesses
     if bounds is None:
-        bounds = []
-        for i in range(len(list_models)):
+        bounds = [(0, empirical_variogram.lags.values[-1]), (0, max_var)] * len(list_models)
 
-            # Use largest boundaries possible for our problem
-            psill_bound = [0, max_var]
-            range_bound = [0, empirical_variogram.lags.values[-1]]
-
-            # Add bounds and guesses with same order as function arguments
-            bounds.append(range_bound)
-            bounds.append(psill_bound)
     if p0 is None:
         p0 = []
         for i in range(len(list_models)):
             # Use psill evenly distributed
-            psill_p0 = ((i+1)/len(list_models))*max_var
+            psill_p0 = ((i + 1) / len(list_models)) * max_var
 
             # Use corresponding ranges
             # !! This fails when no empirical value crosses this (too wide binning/nugget)
             # ind = np.array(np.abs(exp_movaverage-psill_p0)).argmin()
             # range_p0 = empirical_variogram.lags.values[ind]
-            range_p0 = ((i+1)/len(list_models)) * empirical_variogram.lags.values[-1]
+            range_p0 = ((i + 1) / len(list_models)) * empirical_variogram.lags.values[-1]
 
             p0.append(range_p0)
             p0.append(psill_p0)
 
-    bounds = np.transpose(np.array(bounds))
+    final_bounds = np.transpose(np.array(bounds))
 
     # If the error provided is all NaNs (single variogram run), or all zeros (two variogram runs), run without weights
     if np.all(np.isnan(empirical_variogram.err_exp.values)) or np.all(empirical_variogram.err_exp.values == 0):
-        cof, cov = curve_fit(variogram_sum, empirical_variogram.lags.values, empirical_variogram.exp.values, method='trf',
-                             p0=p0, bounds=bounds)
+        cof, cov = curve_fit(
+            variogram_sum,
+            empirical_variogram.lags.values,
+            empirical_variogram.exp.values,
+            method="trf",
+            p0=p0,
+            bounds=final_bounds,
+        )
     # Otherwise, use a weighted fit
     else:
         # We need to filter for possible no data in the error
         valid = np.isfinite(empirical_variogram.err_exp.values)
-        cof, cov = curve_fit(variogram_sum, empirical_variogram.lags.values[valid], empirical_variogram.exp.values[valid],
-                             method='trf', p0=p0, bounds=bounds, sigma=empirical_variogram.err_exp.values[valid])
+        cof, cov = curve_fit(
+            variogram_sum,
+            empirical_variogram.lags.values[valid],
+            empirical_variogram.exp.values[valid],
+            method="trf",
+            p0=p0,
+            bounds=final_bounds,
+            sigma=empirical_variogram.err_exp.values[valid],
+        )
 
     # Store optimized parameters
     list_df = []
     i = 0
     for model in list_models:
         model_name = _get_skgstat_variogram_model_name(model)
         # For models that expect 2 parameters
-        if model_name in ['spherical', 'gaussian', 'exponential', 'cubic']:
+        if model_name in ["spherical", "gaussian", "exponential", "cubic"]:
             df = pd.DataFrame()
-            df = df.assign(model=[model_name], range=[cof[i]], psill=[cof[i+1]])
+            df = df.assign(model=[model_name], range=[cof[i]], psill=[cof[i + 1]])
             i += 2
         # For models that expect 3 parameters
-        elif model_name in ['stable', 'matern']:
+        elif model_name in ["stable", "matern"]:
             df = pd.DataFrame()
-            df = df.assign(model=[model_name], range=[cof[i]], psill=[cof[i + 1]], smooth=[cof[i+2]])
+            df = df.assign(model=[model_name], range=[cof[i]], psill=[cof[i + 1]], smooth=[cof[i + 2]])
             i += 3
         list_df.append(df)
     df_params = pd.concat(list_df)
 
     # Also pass the function of sum of variogram
     variogram_sum_fit = get_variogram_model_func(df_params)
 
     return variogram_sum_fit, df_params
 
-def estimate_model_spatial_correlation(dvalues: Union[np.ndarray, RasterType], list_models: list[str | Callable],
-                                       estimator = 'dowd', gsd: float = None, coords: np.ndarray = None, subsample: int = 1000,
-                                       subsample_method: str = 'cdist_equidistant', n_variograms: int = 1,
-                                       n_jobs: int = 1, verbose = False,
-                                       random_state: None | np.random.RandomState | np.random.Generator | int = None,
-                                       bounds: list[tuple[float, float]] = None, p0: list[float] = None,
-                                       **kwargs) -> tuple[pd.DataFrame, pd.DataFrame, Callable[[np.ndarray], np.ndarray]]:
+
+def estimate_model_spatial_correlation(
+    dvalues: NDArrayf | RasterType,
+    list_models: list[str | Callable[[NDArrayf, float, float], NDArrayf]],
+    estimator: str = "dowd",
+    gsd: float = None,
+    coords: NDArrayf = None,
+    subsample: int = 1000,
+    subsample_method: str = "cdist_equidistant",
+    n_variograms: int = 1,
+    n_jobs: int = 1,
+    verbose: bool = False,
+    random_state: None | np.random.RandomState | int = None,
+    bounds: list[tuple[float, float]] = None,
+    p0: list[float] = None,
+    **kwargs: Any,
+) -> tuple[pd.DataFrame, pd.DataFrame, Callable[[NDArrayf], NDArrayf]]:
 
     """
     Estimate and model the spatial correlation of the input variable by empirical variogram sampling and fitting of a
     sum of variogram model.
 
     The spatial correlation is returned as a function of spatial lags (in units of the input coordinates) which gives a
     correlation value between 0 and 1.
 
     This function samples an empirical variogram using skgstat.Variogram, then optimizes by weighted least-squares the
     sum of a defined number of models, using the functions `sample_empirical_variogram` and `fit_sum_model_variogram`.
 
-    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as elevation differences on stable terrain)
+    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as
+        elevation differences on stable terrain)
     :param list_models: List of K variogram models to sum for the fit in order from short to long ranges. Can either be
         a 3-letter string, full string of the variogram name or SciKit-GStat model function (e.g., for a
         spherical model "Sph", "Spherical" or skgstat.models.spherical).
     :param estimator: Estimator for the empirical variogram; default to Dowd's variogram (see skgstat.Variogram for
         the list of available estimators).
     :param gsd: Ground sampling distance
     :param coords: Coordinates
     :param subsample: Number of samples to randomly draw from the values
     :param subsample_method: Spatial subsampling method
     :param n_variograms: Number of independent empirical variogram estimations (to estimate empirical variogram spread)
     :param n_jobs: Number of processing cores
     :param verbose: Print statements during processing
     :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
-    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper, sill lower, sill upper).
+    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper,
+        sill lower, sill upper).
     :param p0: Initial guess of ranges and sills each model (shape K x 2 = K x range first guess, sill first guess).
 
-    :return: Dataframe of empirical variogram, Dataframe of optimized model parameters, Function of spatial correlation (0 to 1) with spatial lags
+    :return: Dataframe of empirical variogram, Dataframe of optimized model parameters, Function of spatial correlation
+        (0 to 1) with spatial lags
     """
 
-    empirical_variogram = sample_empirical_variogram(values=dvalues, estimator=estimator, gsd=gsd, coords=coords,
-                                                     subsample=subsample, subsample_method=subsample_method,
-                                                     n_variograms=n_variograms, n_jobs=n_jobs, verbose=verbose,
-                                                     random_state=random_state, **kwargs)
-
-    params_variogram_model = fit_sum_model_variogram(list_models=list_models, empirical_variogram=empirical_variogram,
-                                             bounds=bounds, p0=p0)[1]
+    empirical_variogram = sample_empirical_variogram(
+        values=dvalues,
+        estimator=estimator,
+        gsd=gsd,
+        coords=coords,
+        subsample=subsample,
+        subsample_method=subsample_method,
+        n_variograms=n_variograms,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        random_state=random_state,
+        **kwargs,
+    )
+
+    params_variogram_model = fit_sum_model_variogram(
+        list_models=list_models, empirical_variogram=empirical_variogram, bounds=bounds, p0=p0
+    )[1]
 
     spatial_correlation_func = correlation_from_variogram(params_variogram_model=params_variogram_model)
 
     return empirical_variogram, params_variogram_model, spatial_correlation_func
 
-def infer_spatial_correlation_from_stable(dvalues: np.ndarray | RasterType,
-                                          list_models: list[str | Callable],
-                                          stable_mask: np.ndarray | VectorType | gpd.GeoDataFrame = None,
-                                          unstable_mask: np.ndarray | VectorType | gpd.GeoDataFrame = None,
-                                          errors: np.ndarray | RasterType = None,
-                                          estimator = 'dowd', gsd: float = None, coords: np.ndarray = None,
-                                          subsample: int = 1000, subsample_method: str = 'cdist_equidistant',
-                                          n_variograms: int = 1, n_jobs: int = 1, verbose = False,
-                                          bounds: list[tuple[float, float]] = None, p0: list[float] = None,
-                                          random_state: None | np.random.RandomState | np.random.Generator | int = None,
-                                          **kwargs
-                                          ) -> tuple[pd.DataFrame, pd.DataFrame, Callable[[np.ndarray], np.ndarray]]:
+
+def infer_spatial_correlation_from_stable(
+    dvalues: NDArrayf | RasterType,
+    list_models: list[str | Callable[[NDArrayf, float, float], NDArrayf]],
+    stable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | Mask | VectorType | gpd.GeoDataFrame = None,
+    errors: NDArrayf | RasterType = None,
+    estimator: str = "dowd",
+    gsd: float = None,
+    coords: NDArrayf = None,
+    subsample: int = 1000,
+    subsample_method: str = "cdist_equidistant",
+    n_variograms: int = 1,
+    n_jobs: int = 1,
+    verbose: bool = False,
+    bounds: list[tuple[float, float]] = None,
+    p0: list[float] = None,
+    random_state: None | np.random.RandomState | int = None,
+    **kwargs: Any,
+) -> tuple[pd.DataFrame, pd.DataFrame, Callable[[NDArrayf], NDArrayf]]:
     """
     Infer spatial correlation of errors from differenced values on stable terrain and a list of variogram model to fit
     as a sum.
 
     This function returns a dataframe of the empirical variogram, a dataframe of optimized model parameters, and a
     spatial correlation function. The spatial correlation is returned as a function of spatial lags
     (in units of the input coordinates) which gives a correlation value between 0 and 1.
     It is a convenience wrapper for `estimate_model_spatial_correlation` to work on either Raster or array and compute
     the stable mask.
 
     If no stable or unstable mask is provided to mask in or out the values, all terrain is used.
 
-    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as elevation differences on stable terrain)
+    :param dvalues: Proxy values as array or Raster (i.e., differenced values where signal should be zero such as
+        elevation differences on stable terrain)
     :param list_models: List of K variogram models to sum for the fit in order from short to long ranges. Can either be
         a 3-letter string, full string of the variogram name or SciKit-GStat model function (e.g., for a
         spherical model "Sph", "Spherical" or skgstat.models.spherical).
-    :param stable_mask: Vector shapefile of stable terrain (if dvalues is Raster), or boolean array of same shape as dvalues
-    :param unstable_mask: Vector shapefile of unstable terrain (if dvalues is Raster), or boolean array of same shape as dvalues
+    :param stable_mask: Vector shapefile of stable terrain (if dvalues is Raster), or boolean array of same shape as
+        dvalues
+    :param unstable_mask: Vector shapefile of unstable terrain (if dvalues is Raster), or boolean array of same shape
+        as dvalues
     :param errors: Error values to account for heteroscedasticity (ignored if None).
     :param estimator: Estimator for the empirical variogram; default to Dowd's variogram (see skgstat.Variogram for
         the list of available estimators).
-    :param gsd: Ground sampling distance
+    :param gsd: Ground sampling distance, if input values are provided as array
     :param coords: Coordinates
     :param subsample: Number of samples to randomly draw from the values
     :param subsample_method: Spatial subsampling method
     :param n_variograms: Number of independent empirical variogram estimations (to estimate empirical variogram spread)
     :param n_jobs: Number of processing cores
     :param verbose: Print statements during processing
-    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper, sill lower, sill upper).
+    :param bounds: Bounds of range and sill parameters for each model (shape K x 4 = K x range lower, range upper,
+        sill lower, sill upper).
     :param p0: Initial guess of ranges and sills each model (shape K x 2 = K x range first guess, sill first guess).
     :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
 
-    :return: Dataframe of empirical variogram, Dataframe of optimized model parameters, Function of spatial correlation (0 to 1) with spatial lags
+    :return: Dataframe of empirical variogram, Dataframe of optimized model parameters, Function of spatial correlation
+        (0 to 1) with spatial lags
     """
 
-    # Check inputs
-    if not isinstance(dvalues, (Raster, np.ndarray)):
-        raise ValueError('The dvalues must be a Raster or NumPy array.')
-    if stable_mask is not None and not isinstance(stable_mask, (np.ndarray, Vector, gpd.GeoDataFrame)):
-        raise ValueError('The stable mask must be a Vector, GeoDataFrame or NumPy array.')
-    if unstable_mask is not None and not isinstance(unstable_mask, (np.ndarray, Vector, gpd.GeoDataFrame)):
-        raise ValueError('The unstable mask must be a Vector, GeoDataFrame or NumPy array.')
-
-    # Check that input stable mask can only be a georeferenced vector if the proxy values are a Raster to project onto
-    if not isinstance(dvalues, Raster) and isinstance(stable_mask, (Vector, gpd.GeoDataFrame)):
-        raise ValueError(
-            'The stable mask can only passed as a Vector or GeoDataFrame if the input dvalues is a Raster.')
-
-    # Get array if input is a Raster
-    if isinstance(dvalues, Raster):
-        dvalues_arr = get_array_and_mask(dvalues)[0]
-        gsd = dvalues.res[0]
-    else:
-        dvalues_arr = dvalues
-
-    # If the stable mask is not an array, create it
-    if stable_mask is None:
-        stable_mask_arr = np.ones(np.shape(dvalues_arr), dtype=bool)
-    elif not isinstance(stable_mask, np.ndarray):
-
-        # If the stable mask is a geopandas dataframe, wrap it in a Vector object
-        if isinstance(stable_mask, gpd.GeoDataFrame):
-            stable_vector = Vector(stable_mask)
-        else:
-            stable_vector = stable_mask
-
-        # Create the mask
-        stable_mask_arr = stable_vector.create_mask(dvalues)
-    # If the mask is already an array, just pass it
-    else:
-        stable_mask_arr = stable_mask
-
-    # If the unstable mask is not an array, create it
-    if unstable_mask is None:
-        unstable_mask_arr = np.zeros(np.shape(dvalues_arr), dtype=bool)
-    elif not isinstance(unstable_mask, np.ndarray):
-
-        # If the unstable mask is a geopandas dataframe, wrap it in a Vector object
-        if isinstance(unstable_mask, gpd.GeoDataFrame):
-            unstable_vector = Vector(unstable_mask)
-        else:
-            unstable_vector = unstable_mask
-
-        # Create the mask
-        unstable_mask_arr = unstable_vector.create_mask(dvalues)
-    # If the mask is already an array, just pass it
-    else:
-        unstable_mask_arr = unstable_mask
-
-    stable_mask_arr = np.logical_and(stable_mask_arr, ~unstable_mask_arr).squeeze()
-
-    # Need to preserve the shape, so setting as NaNs all points not on stable terrain
-    dvalues_stable_arr = dvalues_arr.copy()
-    dvalues_stable_arr[~stable_mask_arr] = np.nan
+    dvalues_stable_arr, gsd = _preprocess_values_with_mask_to_array(
+        values=dvalues, include_mask=stable_mask, exclude_mask=unstable_mask, gsd=gsd
+    )
 
     # Perform standardization if error array is provided
     if errors is not None:
         if isinstance(errors, Raster):
             errors_arr = get_array_and_mask(errors)[0]
         else:
             errors_arr = errors
 
         # Standardize
         dvalues_stable_arr /= errors_arr
 
     # Estimate and model spatial correlations
     empirical_variogram, params_variogram_model, spatial_correlation_func = estimate_model_spatial_correlation(
-        dvalues=dvalues_stable_arr, list_models=list_models, estimator=estimator, gsd=gsd, coords=coords,
-        subsample=subsample, subsample_method=subsample_method, n_variograms=n_variograms, n_jobs=n_jobs,
-        verbose=verbose, random_state=random_state, bounds=bounds, p0=p0, **kwargs)
+        dvalues=dvalues_stable_arr,
+        list_models=list_models,
+        estimator=estimator,
+        gsd=gsd,
+        coords=coords,
+        subsample=subsample,
+        subsample_method=subsample_method,
+        n_variograms=n_variograms,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        random_state=random_state,
+        bounds=bounds,
+        p0=p0,
+        **kwargs,
+    )
 
     return empirical_variogram, params_variogram_model, spatial_correlation_func
 
 
-def _check_validity_params_variogram(params_variogram_model: pd.DataFrame):
+def _check_validity_params_variogram(params_variogram_model: pd.DataFrame) -> None:
     """Check the validity of the modelled variogram parameters dataframe (mostly in the case it is passed manually)."""
 
     # Check that expected columns exists
-    expected_columns = ['model', 'range', 'psill']
-    if not all([c in params_variogram_model for c in expected_columns]):
-        raise ValueError('The dataframe with variogram parameters must contain the columns "model", "range" and "psill".')
+    expected_columns = ["model", "range", "psill"]
+    if not all(c in params_variogram_model for c in expected_columns):
+        raise ValueError(
+            'The dataframe with variogram parameters must contain the columns "model", "range" and "psill".'
+        )
 
     # Check that the format of variogram models are correct
-    for m in params_variogram_model['model'].values:
-        _get_skgstat_variogram_model_name(m)
+    for model in params_variogram_model["model"].values:
+        _get_skgstat_variogram_model_name(model)
 
     # Check that the format of ranges, sills are correct
-    for r in params_variogram_model['range'].values:
+    for r in params_variogram_model["range"].values:
         if not isinstance(r, (float, np.floating, int, np.integer)):
-            raise ValueError('The variogram ranges must be float or integer.')
+            raise ValueError("The variogram ranges must be float or integer.")
         if r <= 0:
-            raise ValueError('The variogram ranges must have non-zero, positive values.')
+            raise ValueError("The variogram ranges must have non-zero, positive values.")
 
     # Check that the format of ranges, sills are correct
-    for p in params_variogram_model['psill'].values:
+    for p in params_variogram_model["psill"].values:
         if not isinstance(p, (float, np.floating, int, np.integer)):
-            raise ValueError('The variogram partial sills must be float or integer.')
+            raise ValueError("The variogram partial sills must be float or integer.")
         if p <= 0:
-            raise ValueError('The variogram partial sills must have non-zero, positive values.')
+            raise ValueError("The variogram partial sills must have non-zero, positive values.")
 
-    # Check that the mattern smoothness factor exist and is rightly formatted
-    if ['stable'] in params_variogram_model['model'].values or ['matern'] in params_variogram_model['model'].values:
-        if 'smooth' not in params_variogram_model:
-            raise ValueError('The dataframe with variogram parameters must contain the column "smooth" for '
-                             'the smoothness factor when using Matern or Stable models.')
+    # Check that the matern smoothness factor exist and is rightly formatted
+    if ["stable"] in params_variogram_model["model"].values or ["matern"] in params_variogram_model["model"].values:
+        if "smooth" not in params_variogram_model:
+            raise ValueError(
+                'The dataframe with variogram parameters must contain the column "smooth" for '
+                "the smoothness factor when using Matern or Stable models."
+            )
         for i in range(len(params_variogram_model)):
-            if params_variogram_model['model'].values[i] in ['stable', 'matern']:
-                s = params_variogram_model['smooth'].values[i]
+            if params_variogram_model["model"].values[i] in ["stable", "matern"]:
+                s = params_variogram_model["smooth"].values[i]
                 if not isinstance(s, (float, np.floating, int, np.integer)):
-                    raise ValueError('The variogram smoothness parameter must be float or integer.')
+                    raise ValueError("The variogram smoothness parameter must be float or integer.")
                 if s <= 0:
-                    raise ValueError('The variogram smoothness parameter must have non-zero, positive values.')
+                    raise ValueError("The variogram smoothness parameter must have non-zero, positive values.")
 
 
 def neff_circular_approx_theoretical(area: float, params_variogram_model: pd.DataFrame) -> float:
     """
     Number of effective samples approximated from exact disk integration of a sum of any number of variogram models
     of spherical, gaussian, exponential or cubic form over a disk of a certain area. This approximation performs best
     for areas with a shape close to that of a disk.
@@ -1523,164 +1853,180 @@
     The input variogram parameters match the format of the dataframe returned by `fit_sum_variogram_models`, also
     detailed in the parameter description to be passed manually.
 
     This function contains the exact integrated formulas and is mostly used for testing the numerical integration
     of any number and forms of variograms provided by the function `neff_circular_approx_numerical`.
 
     The number of effective samples serves to convert between standard deviation and standard error. For example, with
-    two models: if SE is the standard error, SD the standard deviation and N_eff the number of effective samples, we have:
+    two models: if SE is the standard error, SD the standard deviation and N_eff the number of effective samples:
     SE = SD / sqrt(N_eff) => N_eff = SD^2 / SE^2 => N_eff = (PS1 + PS2)/SE^2 where PS1 and PS2 are the partial sills
     estimated from the variogram models, and SE is estimated by integrating the variogram models with parameters PS1/PS2
     and R1/R2 where R1/R2 are the correlation ranges.
 
     :param area: Area (in square unit of the variogram ranges)
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
 
     :return: Number of effective samples
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
-    # Lag l equal to the radius needed for a disk of area A
-    l = np.sqrt(area / np.pi)
+    # Lag l_equiv equal to the radius needed for a disk of equivalent area A
+    l_equiv = np.sqrt(area / np.pi)
 
     # Below, we list exact integral functions over an area A assumed a disk integrated radially from the center
 
     # Formulas of h * covariance = h * ( psill - variogram ) for each form, then its integral for each form to yield
     # the standard error SE. a1 = range and c1 = partial sill.
 
-    # Spherical: h * covariance = c1 * h * ( 1 - 3/2 * h / a1 + 1/2 * (h/a1)**3 ) = c1 * (h - 3/2 * h**2 / a1 + 1/2 * h**4 / a1**3)
-    # Spherical: radial integral of above from 0 to L: SE**2 = 2 / (L**2) * c1 * (L**2 / 2 - 3/2 * L**3 / 3 / a1 + 1/2 * 1/5 * L**5 / a1**3)
+    # Spherical: h * covariance = c1 * h * ( 1 - 3/2 * h / a1 + 1/2 * (h/a1)**3 )
+    # = c1 * (h - 3/2 * h**2 / a1 + 1/2 * h**4 / a1**3)
+    # Spherical: radial integral of above from 0 to L:
+    # SE**2 = 2 / (L**2) * c1 * (L**2 / 2 - 3/2 * L**3 / 3 / a1 + 1/2 * 1/5 * L**5 / a1**3)
     # which leads to SE**2 =  c1 * (1 - L / a1 + 1/5 * (L/a1)**3 )
     # If spherical model is above the spherical range a1: SE**2 = c1 /5 * (a1/L)**2
 
-    def spherical_exact_integral(a1, c1, L):
-        if l <= a1:
-            squared_se = c1 * (1 - L/a1 + 1/5 * (L/a1)**3)
+    def spherical_exact_integral(a1: float, c1: float, L: float) -> float:
+        if l_equiv <= a1:
+            squared_se = c1 * (1 - L / a1 + 1 / 5 * (L / a1) ** 3)
         else:
-            squared_se = c1 / 5 * (a1/L)**2
+            squared_se = c1 / 5 * (a1 / L) ** 2
         return squared_se
 
     # Exponential: h * covariance = c1 * h * exp(-h/a); a = a1/3
     # Exponential: radial integral of above from 0 to L: SE**2 =  2 / (L**2) * c1 * a * (a - exp(-L/a) * (a + L))
 
-    def exponential_exact_integral(a1, c1, L):
+    def exponential_exact_integral(a1: float, c1: float, L: float) -> float:
         a = a1 / 3
-        squared_se = 2 * c1 * (a/L)**2 * (1 - np.exp(-L/a) * (1 + L/a))
+        squared_se = 2 * c1 * (a / L) ** 2 * (1 - np.exp(-L / a) * (1 + L / a))
         return squared_se
 
     # Gaussian: h * covariance = c1 * h * exp(-h**2/a**2) ; a = a1/2
     # Gaussian: radial integral of above from 0 to L: SE**2 = 2 / (L**2) * c1 * 1/2 * a**2 * (1 - exp(-L**2/a**2))
 
-    def gaussian_exact_integral(a1, c1, L):
+    def gaussian_exact_integral(a1: float, c1: float, L: float) -> float:
         a = a1 / 2
-        squared_se = c1 * (a/L)**2 * (1 - np.exp(-L**2 / a**2))
+        squared_se = c1 * (a / L) ** 2 * (1 - np.exp(-(L**2) / a**2))
         return squared_se
 
     # Cubic: h * covariance = c1 * h * (1 - (7 * (h**2 / a**2)) + ((35 / 4) * (h**3 / a**3)) -
     #                          ((7 / 2) * (h**5 / a**5)) + ((3 / 4) * (h**7 / a**7)))
-    # Cubic: radial integral of above from 0 to L: SE**2 = c1 * (6*a**7 -21*a**5*L**2 + 21*a**4*L**3 - 6*a**2*L**5 + L**7) / (6*a**7)
+    # Cubic: radial integral of above from 0 to L:
+    # SE**2 = c1 * (6*a**7 -21*a**5*L**2 + 21*a**4*L**3 - 6*a**2*L**5 + L**7) / (6*a**7)
 
-    def cubic_exact_integral(a1, c1, L):
-        if l <= a1:
-            squared_se = c1 * (6*a1**7 -21*a1**5*L**2 + 21*a1**4*L**3 - 6*a1**2*L**5 + L**7) / (6*a1**7)
+    def cubic_exact_integral(a1: float, c1: float, L: float) -> float:
+        if l_equiv <= a1:
+            squared_se = (
+                c1
+                * (6 * a1**7 - 21 * a1**5 * L**2 + 21 * a1**4 * L**3 - 6 * a1**2 * L**5 + L**7)
+                / (6 * a1**7)
+            )
         else:
-            squared_se = 1/6 * c1 * a1**2 / L**2
+            squared_se = 1 / 6 * c1 * a1**2 / L**2
         return squared_se
 
-    squared_se = 0
-    valid_models = ['spherical', 'exponential', 'gaussian', 'cubic']
-    exact_integrals = [spherical_exact_integral, exponential_exact_integral, gaussian_exact_integral, cubic_exact_integral]
-    for i in np.arange((len(params_variogram_model))):
-        model_name = _get_skgstat_variogram_model_name(params_variogram_model['model'].values[i])
-        r = params_variogram_model['range'].values[i]
-        p = params_variogram_model['psill'].values[i]
+    squared_se = 0.0
+    valid_models = ["spherical", "exponential", "gaussian", "cubic"]
+    exact_integrals = [
+        spherical_exact_integral,
+        exponential_exact_integral,
+        gaussian_exact_integral,
+        cubic_exact_integral,
+    ]
+    for i in np.arange(len(params_variogram_model)):
+        model_name = _get_skgstat_variogram_model_name(params_variogram_model["model"].values[i])
+        r = params_variogram_model["range"].values[i]
+        p = params_variogram_model["psill"].values[i]
         if model_name in valid_models:
             exact_integral = exact_integrals[valid_models.index(model_name)]
-            squared_se += exact_integral(r, p, l)
+            squared_se += exact_integral(r, p, l_equiv)
 
     # We sum all partial sill to get the total sill
     total_sill = np.nansum(params_variogram_model.psill)
     # The number of effective sample is the fraction of total sill by squared standard error
-    neff = total_sill/squared_se
+    neff = total_sill / squared_se
 
     return neff
 
-def _integrate_fun(fun: Callable, low_b: float, upp_b: float) -> float:
+
+def _integrate_fun(fun: Callable[[NDArrayf], NDArrayf], low_b: float, upp_b: float) -> float:
     """
     Numerically integrate function between an upper and lower bounds
     :param fun: Function to integrate
     :param low_b: Lower bound
     :param upp_b: Upper bound
 
     :return: Integral between lower and upper bound
     """
     return integrate.quad(fun, low_b, upp_b)[0]
 
-def neff_circular_approx_numerical(area: float, params_variogram_model: pd.DataFrame) -> float:
+
+def neff_circular_approx_numerical(area: float | int, params_variogram_model: pd.DataFrame) -> float:
     """
     Number of effective samples derived from numerical integration for any sum of variogram models over a circular area.
     This is a generalization of Rolstad et al. (2009): http://dx.doi.org/10.3189/002214309789470950, which is verified
     against exact integration of `neff_circular_approx_theoretical`. This approximation performs best for areas with
     a shape close to that of a disk.
     The input variogram parameters match the format of the dataframe returned by `fit_sum_variogram_models`, also
     detailed in the parameter description to be passed manually.
 
     The number of effective samples N_eff serves to convert between standard deviation and standard error
     over the area: SE = SD / sqrt(N_eff) if SE is the standard error, SD the standard deviation.
 
     :param area: Area (in square unit of the variogram ranges)
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
 
     :returns: Number of effective samples
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
     # Get the total sill from the sum of partial sills
     total_sill = np.nansum(params_variogram_model.psill)
 
     # Define the covariance sum function times the spatial lag, for later integration
-    def hcov_sum(h):
+    def hcov_sum(h: NDArrayf) -> NDArrayf:
         return h * covariance_from_variogram(params_variogram_model)(h)
 
     # Get a radius for which the circle as the defined area
     h_equiv = np.sqrt(area / np.pi)
 
     # Integrate the covariance function between the center and the radius
     full_int = _integrate_fun(hcov_sum, 0, h_equiv)
 
     # Get the standard error, and return the number of effective samples
-    squared_se = 2*np.pi*full_int / area
+    squared_se = 2 * np.pi * full_int / area
 
     # The number of effective sample is the fraction of total sill by squared standard error
-    neff = total_sill/squared_se
+    neff = total_sill / squared_se
 
     return neff
 
 
-def neff_exact(coords: np.ndarray, errors: np.ndarray, params_variogram_model: pd.DataFrame, vectorized: bool = True) -> float:
+def neff_exact(
+    coords: NDArrayf, errors: NDArrayf, params_variogram_model: pd.DataFrame, vectorized: bool = True
+) -> float:
     """
      Exact number of effective samples derived from a double sum of covariance with euclidean coordinates based on
      the provided variogram parameters. This method works for any shape of area.
 
     :param coords: Center coordinates with size (N,2) for each spatial support (typically, pixel)
     :param errors: Errors at the coordinates with size (N,) for each spatial support (typically, pixel)
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
     :param vectorized: Perform the vectorized calculation (used for testing).
 
     :return: Number of effective samples
     """
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
@@ -1691,71 +2037,75 @@
     # Get number of points and pairwise distance compacted matrix from scipy.pdist
     n = len(coords)
     pds = pdist(coords)
 
     # Now we compute the double covariance sum
     # Either using for-loop-version
     if not vectorized:
-        var = 0
+        var = 0.0
         for i in range(n):
             for j in range(n):
 
                 # For index calculation of the pairwise distance,
                 # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html
                 if i == j:
                     d = 0
                 elif i < j:
                     ind = n * i + j - ((i + 2) * (i + 1)) // 2
                     d = pds[ind]
                 else:
                     ind = n * j + i - ((j + 2) * (j + 1)) // 2
                     d = pds[ind]
 
-                var += rho(d) * errors[i] * errors[j]
+                var += rho(d) * errors[i] * errors[j]  # type: ignore
 
     # Or vectorized version
     else:
         # Convert the compact pairwise distance into a square matrix
         pds_matrix = squareform(pds)
         # Vectorize calculation
-        var = np.sum(errors.reshape((-1, 1)) @ errors.reshape((1, -1)) * rho(pds_matrix.flatten()).reshape(pds_matrix.shape))
+        var = np.sum(
+            errors.reshape((-1, 1)) @ errors.reshape((1, -1)) * rho(pds_matrix.flatten()).reshape(pds_matrix.shape)
+        )
 
     # The number of effective sample is the fraction of total sill by squared standard error
-    squared_se_dsc = var / n ** 2
-    neff = np.mean(errors)**2/squared_se_dsc
+    squared_se_dsc = var / n**2
+    neff = np.mean(errors) ** 2 / squared_se_dsc
 
     return neff
 
-def neff_hugonnet_approx(coords: np.ndarray, errors: np.ndarray, params_variogram_model: pd.DataFrame, subsample: int = 1000,
-                         vectorized: bool = True, random_state: None | np.random.RandomState | np.random.Generator | int = None) -> float:
+
+def neff_hugonnet_approx(
+    coords: NDArrayf,
+    errors: NDArrayf,
+    params_variogram_model: pd.DataFrame,
+    subsample: int = 1000,
+    vectorized: bool = True,
+    random_state: None | np.random.RandomState | int = None,
+) -> float:
     """
     Approximated number of effective samples derived from a double sum of covariance subsetted on one of the two sums,
     based on euclidean coordinates with the provided variogram parameters. This method works for any shape of area.
     See Hugonnet et al. (2022), https://doi.org/10.1109/jstars.2022.3188922, in particular Supplementary Fig. S16.
 
     :param coords: Center coordinates with size (N,2) for each spatial support (typically, pixel)
     :param errors: Errors at the coordinates with size (N,) for each spatial support (typically, pixel)
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
     :param subsample: Number of samples to subset the calculation
     :param vectorized: Perform the vectorized calculation (used for testing).
     :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
 
     :return: Number of effective samples
     """
 
-    # Define state for random subsampling (to fix results during testing)
-    if random_state is None:
-        rnd = np.random.default_rng()
-    elif isinstance(random_state, (np.random.RandomState, np.random.Generator)):
-        rnd = random_state
-    else:
-        rnd = np.random.RandomState(np.random.MT19937(np.random.SeedSequence(random_state)))
+    # Define random state
+    rnd = _random_state_definition(random_state=random_state)
 
     # Check input dataframe
     _check_validity_params_variogram(params_variogram_model)
 
     # Get spatial correlation function from variogram parameters
     rho = correlation_from_variogram(params_variogram_model)
 
@@ -1768,15 +2118,15 @@
 
     # Get random subset of points for one of the sums
     rand_points = rnd.choice(n, size=subsample, replace=False)
 
     # Now we compute the double covariance sum
     # Either using for-loop-version
     if not vectorized:
-        var = 0
+        var = 0.0
         for ind_sub in range(subsample):
             for j in range(n):
 
                 i = rand_points[ind_sub]
                 # For index calculation of the pairwise distance,
                 # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html
                 if i == j:
@@ -1784,158 +2134,176 @@
                 elif i < j:
                     ind = n * i + j - ((i + 2) * (i + 1)) // 2
                     d = pds[ind]
                 else:
                     ind = n * j + i - ((j + 2) * (j + 1)) // 2
                     d = pds[ind]
 
-                var += rho(d) * errors[i] * errors[j]
+                var += rho(d) * errors[i] * errors[j]  # type: ignore
 
     # Or vectorized version
     else:
         # We subset the points used in one dimension, for errors and pairwise distances computed
         errors_sub = errors[rand_points]
         pds_matrix = squareform(pds)
         pds_matrix_sub = pds_matrix[:, rand_points]
         # Vectorized calculation
-        var = np.sum(errors.reshape((-1, 1)) @ errors_sub.reshape((1, -1)) * rho(pds_matrix_sub.flatten()).reshape(pds_matrix_sub.shape))
+        var = np.sum(
+            errors.reshape((-1, 1))
+            @ errors_sub.reshape((1, -1))
+            * rho(pds_matrix_sub.flatten()).reshape(pds_matrix_sub.shape)
+        )
 
     # The number of effective sample is the fraction of total sill by squared standard error
     squared_se_dsc = var / (n * subsample)
-    neff = np.mean(errors)**2 / squared_se_dsc
+    neff = np.mean(errors) ** 2 / squared_se_dsc
 
     return neff
 
-def number_effective_samples(area: float | int | VectorType | gpd.GeoDataFrame, params_variogram_model: pd.DataFrame,
-                             rasterize_resolution: RasterType | float = None, **kwargs) -> float:
+
+def number_effective_samples(
+    area: float | int | VectorType | gpd.GeoDataFrame,
+    params_variogram_model: pd.DataFrame,
+    rasterize_resolution: RasterType | float = None,
+    **kwargs: Any,
+) -> float:
     """
     Compute the number of effective samples, i.e. the number of uncorrelated samples, in an area accounting for spatial
     correlations described by a sum of variogram models.
 
     This function wraps two methods:
 
     - A discretized integration method that provides the exact estimate for any shape of area using a double sum of
-        covariance. By default, this method is approximated using Equation 18 of Hugonnet et al. (2022), https://doi.org/10.1109/jstars.2022.3188922
-        to decrease computing times while preserving a good approximation.
+        covariance. By default, this method is approximated using Equation 18 of Hugonnet et al. (2022),
+        https://doi.org/10.1109/jstars.2022.3188922 to decrease computing times while preserving a good approximation.
 
     - A continuous integration method that provides a conservative (i.e., slightly overestimated) value for a disk
-        area shape, based on a generalization of the approach of Rolstad et al. (2009), http://dx.doi.org/10.3189/002214309789470950.
+        area shape, based on a generalization of the approach of Rolstad et al. (2009),
+        http://dx.doi.org/10.3189/002214309789470950.
 
     By default, if a numeric value is passed for an area, the continuous method is used considering a disk shape. If a
     vector is passed, the discretized method is computed on that shape. If the discretized method is used, a resolution
     for rasterization is generally expected, otherwise is arbitrarily chosen as a fifth of the shortest correlation
     range to ensure a sufficiently fine grid for propagation of the shortest range.
 
     :param area: Area of interest either as a numeric value of surface in the same unit as the variogram ranges (will
         assume a circular shape), or as a vector (shapefile) of the area
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
-    :param rasterize_resolution: Resolution to rasterize the area if passed as a vector. Can be a float value or a Raster.
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
+    :param rasterize_resolution: Resolution to rasterize the area if passed as a vector. Can be a float value or a
+        Raster.
     :param kwargs: Keyword argument to pass to the `neff_hugonnet_approx` function.
 
     :return: Number of effective samples
     """
 
     # Check input for variogram parameters
     _check_validity_params_variogram(params_variogram_model=params_variogram_model)
 
     # If area is numeric, run the continuous circular approximation
-    if isinstance(area, (float, int, np.floating, np.integer)):
+    if isinstance(area, (float, int)):
         neff = neff_circular_approx_numerical(area=area, params_variogram_model=params_variogram_model)
 
     # Otherwise, run the discrete sum of covariance
     elif isinstance(area, (Vector, gpd.GeoDataFrame)):
 
         # If the input is a geopandas dataframe, put into a Vector object
         if isinstance(area, gpd.GeoDataFrame):
             V = Vector(area)
         else:
             V = area
 
         if rasterize_resolution is None:
-            rasterize_resolution =  np.min(params_variogram_model['range'].values)/5.
-            warnings.warn('Resolution for vector rasterization is not defined and thus set at 20% of the shortest '
-                'correlation range, which might result in large memory usage.')
+            rasterize_resolution = np.min(params_variogram_model["range"].values) / 5.0
+            warnings.warn(
+                "Resolution for vector rasterization is not defined and thus set at 20% of the shortest "
+                "correlation range, which might result in large memory usage."
+            )
 
         # Rasterize with numeric resolution or Raster metadata
         if isinstance(rasterize_resolution, (float, int, np.floating, np.integer)):
 
             # We only need relative mask and coordinates, not absolute
-            mask = V.create_mask(xres=rasterize_resolution)
+            mask = V.create_mask(xres=rasterize_resolution, as_array=True)
             x = rasterize_resolution * np.arange(0, mask.shape[0])
             y = rasterize_resolution * np.arange(0, mask.shape[1])
             coords = np.array(np.meshgrid(y, x))
             coords_on_mask = coords[:, mask].T
 
         elif isinstance(rasterize_resolution, Raster):
 
             # With a Raster we can get the coordinates directly
-            mask = V.create_mask(rst=rasterize_resolution).squeeze()
+            mask = V.create_mask(rst=rasterize_resolution, as_array=True).squeeze()
             coords = np.array(rasterize_resolution.coords())
             coords_on_mask = coords[:, mask].T
 
         else:
-            raise ValueError('The rasterize resolution must be a float, integer or Raster subclass.')
+            raise ValueError("The rasterize resolution must be a float, integer or Raster subclass.")
 
         # Here we don't care about heteroscedasticity, so all errors are standardized to one
         errors_on_mask = np.ones(len(coords_on_mask))
 
-        neff = neff_hugonnet_approx(coords=coords_on_mask, errors=errors_on_mask,
-                                    params_variogram_model=params_variogram_model, **kwargs)
+        neff = neff_hugonnet_approx(
+            coords=coords_on_mask, errors=errors_on_mask, params_variogram_model=params_variogram_model, **kwargs
+        )
 
     else:
-        raise ValueError('Area must be a float, integer, Vector subclass or geopandas dataframe.')
+        raise ValueError("Area must be a float, integer, Vector subclass or geopandas dataframe.")
 
     return neff
 
-def spatial_error_propagation(areas: list[float | VectorType | gpd.GeoDataFrame],
-                              errors: RasterType,
-                              params_variogram_model: pd.Dataframe,
-                              **kwargs) -> list[float]:
+
+def spatial_error_propagation(
+    areas: list[float | VectorType | gpd.GeoDataFrame],
+    errors: RasterType,
+    params_variogram_model: pd.Dataframe,
+    **kwargs: Any,
+) -> list[float]:
     """
     Spatial propagation of elevation errors to an area using the estimated heteroscedasticity and spatial correlations.
 
     This function is based on the `number_effective_samples` function to estimate uncorrelated samples. If given a
     vector area, it uses Equation 18 of Hugonnet et al. (2022), https://doi.org/10.1109/jstars.2022.3188922. If given
     a numeric area, it uses a generalization of Rolstad et al. (2009), http://dx.doi.org/10.3189/002214309789470950.
 
     The standard error SE (1-sigma) is then computed as SE = mean(SD) / Neff, where mean(SD) is the mean of errors in
     the area of interest which accounts for heteroscedasticity, and Neff is the number of effective samples.
 
     :param areas: Area of interest either as a numeric value of surface in the same unit as the variogram ranges (will
         assume a circular shape), or as a vector (shapefile) of the area.
     :param errors: Errors from heteroscedasticity estimation and modelling, as an array or Raster.
-    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the model types
-        (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for the partial
-        sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model (e.g.,
-        [None, 0.2]).
+    :param params_variogram_model: Dataframe of variogram models to sum with three to four columns, "model" for the
+        model types (e.g., ["spherical", "matern"]), "range" for the correlation ranges (e.g., [2, 100]), "psill" for
+        the partial sills (e.g., [0.8, 0.2]) and "smooth" for the smoothness parameter if it exists for this model
+        (e.g., [None, 0.2]).
     :param kwargs: Keyword argument to pass to the `neff_hugonnet_approx` function.
 
     :return: List of standard errors (1-sigma) for the input areas
     """
 
     standard_errors = []
     errors_arr = get_array_and_mask(errors)[0]
     for area in areas:
         # We estimate the number of effective samples in the area
-        neff = number_effective_samples(area=area, params_variogram_model=params_variogram_model,
-                                        rasterize_resolution=errors, **kwargs)
+        neff = number_effective_samples(
+            area=area, params_variogram_model=params_variogram_model, rasterize_resolution=errors, **kwargs
+        )
 
         # We compute the average error in this area
         # If the area is only a value, take the average error over the entire Raster
         if isinstance(area, float):
             average_spread = np.nanmean(errors_arr)
         else:
             if isinstance(area, gpd.GeoDataFrame):
                 area_vector = Vector(area)
             else:
                 area_vector = area
-            area_mask = area_vector.create_mask(errors).squeeze()
+            area_mask = area_vector.create_mask(errors, as_array=True).squeeze()
 
             average_spread = np.nanmean(errors_arr[area_mask])
 
         # Compute the standard error from those two values
         standard_error = average_spread / np.sqrt(neff)
         standard_errors.append(standard_error)
 
@@ -1963,15 +2331,15 @@
     :param neff: number of effective samples
 
     :return: standard error
     """
     return std * np.sqrt(1 / neff)
 
 
-def _distance_latlon(tup1: tuple, tup2: tuple, earth_rad: float = 6373000) -> float:
+def _distance_latlon(tup1: tuple[float, float], tup2: tuple[float, float], earth_rad: float = 6373000) -> float:
     """
     Distance between two lat/lon coordinates projected on a spheroid
     ref: https://stackoverflow.com/questions/19412462/getting-distance-between-two-points-based-on-latitude-longitude
     :param tup1: lon/lat coordinates of first point
     :param tup2: lon/lat coordinates of second point
     :param earth_rad: radius of the earth in meters
 
@@ -1981,158 +2349,585 @@
     lon1 = m.radians(abs(tup1[0]))
     lat2 = m.radians(abs(tup2[1]))
     lon2 = m.radians(abs(tup2[0]))
 
     dlon = lon2 - lon1
     dlat = lat2 - lat1
 
-    a = m.sin(dlat / 2)**2 + m.cos(lat1) * m.cos(lat2) * m.sin(dlon / 2)**2
+    a = m.sin(dlat / 2) ** 2 + m.cos(lat1) * m.cos(lat2) * m.sin(dlon / 2) ** 2
     c = 2 * m.atan2(m.sqrt(a), m.sqrt(1 - a))
 
     distance = earth_rad * c
 
     return distance
 
-def patches_method(values: np.ndarray, gsd: float, area: float, mask: Optional[np.ndarray] = None,
-                   perc_min_valid: float = 80., statistics: Iterable[Union[str, Callable, None]] = ['count', np.nanmedian ,nmad],
-                   patch_shape: str = 'circular', n_patches: int = 1000, verbose: bool = False,
-                   random_state: None | int | np.random.RandomState | np.random.Generator = None) -> pd.DataFrame:
 
+def _scipy_convolution(imgs: NDArrayf, filters: NDArrayf, output: NDArrayf) -> None:
+    """
+    Scipy convolution on a number n_N of 2D images of size N1 x N2 using a number of kernels n_M of sizes M1 x M2.
+
+    :param imgs: Input array of size (n_N, N1, N2) with n_N images of size N1 x N2
+    :param filters: Input array of filters of size (n_M, M1, M2) with n_M filters of size M1 x M2
+    :param output: Initialized output array of size (n_N, n_M, N1, N2)
+    """
+
+    for i_N in np.arange(imgs.shape[0]):
+        for i_M in np.arange(filters.shape[0]):
+            output[i_N, i_M, :, :] = fftconvolve(imgs[i_N, :, :], filters[i_M, :, :], mode="same")
+
+
+nd4type = numba.double[:, :, :, :]
+nd3type = numba.double[:, :, :]
+
+
+@jit((nd3type, nd3type, nd4type))  # type: ignore
+def _numba_convolution(imgs: NDArrayf, filters: NDArrayf, output: NDArrayf) -> None:
+    """
+    Numba convolution on a number n_N of 2D images of size N1 x N2 using a number of kernels n_M of sizes M1 x M2.
+
+    :param imgs: Input array of size (n_N, N1, N2) with n_N images of size N1 x N2
+    :param filters: Input array of filters of size (n_M, M1, M2) with n_M filters of size M1 x M2
+    :param output: Initialized output array of size (n_N, n_M, N1, N2)
+    """
+    n_rows, n_cols, n_imgs = imgs.shape
+    height, width, n_filters = filters.shape
+
+    for ii in range(n_imgs):
+        for rr in range(n_rows - height + 1):
+            for cc in range(n_cols - width + 1):
+                for hh in range(height):
+                    for ww in range(width):
+                        for ff in range(n_filters):
+                            imgval = imgs[rr + hh, cc + ww, ii]
+                            filterval = filters[hh, ww, ff]
+                            output[rr, cc, ii, ff] += imgval * filterval
+
+
+def convolution(imgs: NDArrayf, filters: NDArrayf, method: str = "scipy") -> NDArrayf:
+    """
+    Convolution on a number n_N of 2D images of size N1 x N2 using a number of kernels n_M of sizes M1 x M2, using
+    either scipy.signal.fftconvolve or accelerated numba loops.
+    Note that the indexes on n_M and n_N correspond to first axes on the array to speed up computations (prefetching).
+    Inspired by: https://laurentperrinet.github.io/sciblog/posts/2017-09-20-the-fastest-2d-convolution-in-the-world.html
+
+    :param imgs: Input array of size (n_N, N1, N2) with n_N images of size N1 x N2
+    :param filters: Input array of filters of size (n_M, M1, M2) with n_M filters of size M1 x M2
+    :param method: Method to perform the convolution: "scipy" or "numba"
+
+    :return: Filled array of outputs of size (n_N, n_M, N1, N2)
+    """
+
+    # Initialize output array according to input shapes
+    n_N, N1, N2 = imgs.shape
+    n_M, M1, M2 = filters.shape
+    output = np.zeros((n_N, n_M, N1, N2))
+
+    if method.lower() == "scipy":
+        _scipy_convolution(imgs=imgs, filters=filters, output=output)
+    elif method.lower() == "numba":
+        _numba_convolution(
+            imgs=imgs.astype(dtype=np.double),
+            filters=filters.astype(dtype=np.double),
+            output=output.astype(dtype=np.double),
+        )
+    else:
+        raise ValueError('Method must be "scipy" or "numba".')
+
+    return output
+
+
+def mean_filter_nan(
+    img: NDArrayf, kernel_size: int, kernel_shape: str = "circular", method: str = "scipy"
+) -> tuple[NDArrayf, NDArrayf, int]:
+    """
+    Apply a mean filter to an image with a square or circular kernel of size p and with NaN values ignored.
+
+    :param img: Input array of size (N1, N2)
+    :param kernel_size: Size M of kernel, which will be a symmetrical (M, M) kernel
+    :param kernel_shape: Shape of kernel, either "square" or "circular"
+    :param method: Method to perform the convolution: "scipy" or "numba"
+
+    :return: Array of size (N1, N2) with mean values, Array of size (N1, N2) with number of valid pixels, Number of
+        pixels in the kernel
+    """
+
+    # Simplify kernel size notation
+    p = kernel_size
+
+    # Copy the array and replace NaNs by zeros before summing them in the convolution
+    img_zeroed = img.copy()
+    img_zeroed[~np.isfinite(img_zeroed)] = 0
+
+    # Define square kernel
+    if kernel_shape.lower() == "square":
+        kernel = np.ones((p, p), dtype="uint8")
+
+    # Circle kernel
+    elif kernel_shape.lower() == "circular":
+        kernel = _create_circular_mask((p, p)).astype("uint8")
+    else:
+        raise ValueError('Kernel shape should be "square" or "circular".')
+
+    # Run convolution to compute the sum of img values
+    summed_img = convolution(
+        imgs=img_zeroed.reshape((1, img_zeroed.shape[0], img_zeroed.shape[1])),
+        filters=kernel.reshape((1, kernel.shape[0], kernel.shape[1])),
+        method=method,
+    ).squeeze()
+
+    # Construct a boolean array for nodatas
+    nodata_img = np.ones(np.shape(img), dtype=np.int8)
+    nodata_img[~np.isfinite(img)] = 0
+
+    # Count the number of valid pixels in the kernel with a convolution
+    nb_valid_img = convolution(
+        imgs=nodata_img.reshape((1, nodata_img.shape[0], nodata_img.shape[1])),
+        filters=kernel.reshape((1, kernel.shape[0], kernel.shape[1])),
+        method=method,
+    ).squeeze()
+
+    # Compute the final mean filter which accounts for no data
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", "divide by zero encountered in *divide")
+        mean_img = summed_img / nb_valid_img
+
+    # Compute the number of pixel per kernel
+    nb_pixel_per_kernel = np.count_nonzero(kernel)
+
+    return mean_img, nb_valid_img, nb_pixel_per_kernel
+
+
+def _patches_convolution(
+    values: NDArrayf,
+    gsd: float,
+    area: float,
+    perc_min_valid: float = 80.0,
+    patch_shape: str = "circular",
+    method: str = "scipy",
+    statistic_between_patches: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    verbose: bool = False,
+    return_in_patch_statistics: bool = False,
+) -> tuple[float, float, float] | tuple[float, float, float, pd.DataFrame]:
+    """
+
+    :param values: Values as array of shape (N1, N2) with NaN for masked values
+    :param gsd: Ground sampling distance
+    :param area: Size of integration area (squared unit of ground sampling distance)
+    :param perc_min_valid: Minimum valid area in the patch
+    :param patch_shape: Shape of patch, either "circular" or "square"
+    :param method: Method to perform the convolution, "scipy" or "numba"
+    :param statistic_between_patches: Statistic to compute between all patches, typically a measure of spread, applied
+        to the first in-patch statistic, which is typically the mean
+    :param verbose: Print statement to console
+    :param return_in_patch_statistics: Whether to return the dataframe of statistics for all patches and areas
+
+
+    :return: Statistic between patches, Number of patches, Exact discretized area, (Optional) Dataframe of per-patch
+        statistics
+    """
+
+    # Get kernel size to match area
+    # If circular, it corresponds to the diameter
+    if patch_shape.lower() == "circular":
+        kernel_size = int(np.round(2 * np.sqrt(area / np.pi) / gsd, decimals=0))
+    # If square, to the side length
+    elif patch_shape.lower() == "square":
+        kernel_size = int(np.round(np.sqrt(area) / gsd, decimals=0))
+
+    else:
+        raise ValueError('Kernel shape should be "square" or "circular".')
+
+    if verbose:
+        print("Computing the convolution on the entire array...")
+    mean_img, nb_valid_img, nb_pixel_per_kernel = mean_filter_nan(
+        img=values, kernel_size=kernel_size, kernel_shape=patch_shape, method=method
+    )
+
+    # Exclude mean values if number of valid pixels is less than a percentage of the kernel size
+    mean_img[nb_valid_img < nb_pixel_per_kernel * perc_min_valid / 100.0] = np.nan
+
+    # A problem with the convolution method compared to the quadrant one is that patches are not independent, which
+    # can bias the estimation of spread. To remedy this, we compute spread statistics on patches separated by the
+    # kernel size (i.e., the diameter of the circular patch, or side of the square patch) to ensure no dependency
+
+    # There are as many combinations for this calculation as the square of the kernel_size
+    if verbose:
+        print("Computing statistic between patches for all independent combinations...")
+    list_statistic_estimates = []
+    list_nb_independent_patches = []
+    for i in range(kernel_size):
+        for j in range(kernel_size):
+            statistic = statistic_between_patches(mean_img[i::kernel_size, j::kernel_size].ravel())
+            nb_patches = np.count_nonzero(np.isfinite(mean_img[i::kernel_size, j::kernel_size]))
+            list_statistic_estimates.append(statistic)
+            list_nb_independent_patches.append(nb_patches)
+
+    if return_in_patch_statistics:
+        # Create dataframe of independent patches for one independent setting
+        df = pd.DataFrame(
+            data={
+                "nanmean": mean_img[::kernel_size, ::kernel_size].ravel(),
+                "count": nb_valid_img[::kernel_size, ::kernel_size].ravel(),
+            }
+        )
+
+    # We then use the average of the statistic computed for different sets of independent patches to get a more robust
+    # estimate
+    average_statistic = float(np.nanmean(np.asarray(list_statistic_estimates)))
+    nb_independent_patches = float(np.nanmean(np.asarray(list_nb_independent_patches)))
+    exact_area = nb_pixel_per_kernel * gsd**2
+
+    if return_in_patch_statistics:
+        return average_statistic, nb_independent_patches, exact_area, df
+    else:
+        return average_statistic, nb_independent_patches, exact_area
+
+
+def _patches_loop_quadrants(
+    values: NDArrayf,
+    gsd: float,
+    area: float,
+    patch_shape: str = "circular",
+    n_patches: int = 1000,
+    perc_min_valid: float = 80.0,
+    statistics_in_patch: Iterable[Callable[[NDArrayf], np.floating[Any]] | str] = (np.nanmean,),
+    statistic_between_patches: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    verbose: bool = False,
+    random_state: None | int | np.random.RandomState = None,
+    return_in_patch_statistics: bool = False,
+) -> tuple[float, float, float] | tuple[float, float, float, pd.DataFrame]:
     """
     Patches method for empirical estimation of the standard error over an integration area
 
-    :param values: Values
+
+    :param values: Values as array of shape (N1, N2) with NaN for masked values
     :param gsd: Ground sampling distance
-    :param mask: Mask of sampled terrain
-    :param area: Size of integration area
+    :param area: Size of integration area (squared unit of ground sampling distance)
     :param perc_min_valid: Minimum valid area in the patch
-    :param statistics: List of statistics to compute in the patch
-    :param patch_shape: Shape of patch ['circular' or 'rectangular']
+    :param statistics_in_patch: List of statistics to compute in each patch (count is computed by default; only the
+    first statistic is used by statistic_between_patches)
+    :param statistic_between_patches: Statistic to compute between all patches, typically a measure of spread, applied
+        to the first in-patch statistic, which is typically the mean
+    :param patch_shape: Shape of patch, either "circular" or "square".
     :param n_patches: Maximum number of patches to sample
     :param verbose: Print statement to console
     :param random_state: Random state or seed number to use for calculations (to fix random sampling during testing)
+    :param return_in_patch_statistics: Whether to return the dataframe of statistics for all patches and areas
 
-    :return: tile, mean, median, std and count of each patch
+    :return: Statistic between patches, Number of patches, Exact discretized area, Dataframe of per-patch statistics
     """
 
-    # Define state for random subsampling (to fix results during testing)
-    if random_state is None:
-        rnd = np.random.default_rng()
-    elif isinstance(random_state, (np.random.RandomState, np.random.Generator)):
-        rnd = random_state
-    else:
-        rnd = np.random.RandomState(np.random.MT19937(np.random.SeedSequence(random_state)))
+    list_statistics_in_patch = list(statistics_in_patch)
+    # Add count by default
+    list_statistics_in_patch.append("count")
 
-    statistics_name = [f if isinstance(f, str) else f.__name__ for f in statistics]
+    # Get statistic name
+    statistics_name = [f if isinstance(f, str) else f.__name__ for f in list_statistics_in_patch]
 
-    values, mask_values = get_array_and_mask(values)
+    # Define random state
+    rnd = _random_state_definition(random_state=random_state)
 
-    values = values.squeeze()
+    # Divide raster in quadrants where we can sample
+    nx, ny = np.shape(values)
 
-    # Use all grid if no mask is provided
-    if mask is None:
-        mask = np.ones(np.shape(values),dtype=bool)
-
-    # First, remove non sampled area (but we need to keep the 2D shape of raster for patch sampling)
-    valid_mask = np.logical_and(~mask_values, mask)
-    values[~valid_mask] = np.nan
+    kernel_size = int(np.round(np.sqrt(area) / gsd, decimals=0))
 
-    # Divide raster in cadrants where we can sample
-    nx, ny = np.shape(values)
-    valid_count = len(values[~np.isnan(values)])
-    count = nx * ny
-    if verbose:
-        print('Number of valid pixels: ' + str(count))
-    nb_cadrant = int(np.floor(np.sqrt((count * gsd ** 2) / area) + 1))
     # For rectangular quadrants
-    nx_sub = int(np.floor((nx - 1) / nb_cadrant))
-    ny_sub = int(np.floor((ny - 1) / nb_cadrant))
+    nx_sub = int(np.floor((nx - 1) / kernel_size))
+    ny_sub = int(np.floor((ny - 1) / kernel_size))
     # For circular patches
-    rad = np.sqrt(area/np.pi) / gsd
+    rad = int(np.round(np.sqrt(area / np.pi) / gsd, decimals=0))
+
+    # Compute exact area to provide to checks and return
+    if patch_shape.lower() == "square":
+        nb_pixel_exact = nx_sub * ny_sub
+        exact_area = nb_pixel_exact * gsd**2
+    elif patch_shape.lower() == "circular":
+        nb_pixel_exact = np.count_nonzero(_create_circular_mask(shape=(nx, ny), radius=rad))
+        exact_area = nb_pixel_exact * gsd**2
 
-    # Create list of all possible cadrants
-    list_cadrant = [[i, j] for i in range(nb_cadrant) for j in range(nb_cadrant)]
+    # Create list of all possible quadrants
+    list_quadrant = [[i, j] for i in range(nx_sub) for j in range(ny_sub)]
     u = 0
-    # Keep sampling while there is cadrants left and below maximum number of patch to sample
+    # Keep sampling while there is quadrants left and below maximum number of patch to sample
     remaining_nsamp = n_patches
     list_df = []
-    while len(list_cadrant) > 0 and u < n_patches:
+    while len(list_quadrant) > 0 and u < n_patches:
 
-        # Draw a random coordinate from the list of cadrants, select more than enough random points to avoid drawing
+        # Draw a random coordinate from the list of quadrants, select more than enough random points to avoid drawing
         # randomly and differencing lists several times
-        list_idx_cadrant = rnd.choice(len(list_cadrant), size=min(len(list_cadrant), 10*remaining_nsamp))
+        list_idx_quadrant = rnd.choice(len(list_quadrant), size=min(len(list_quadrant), 10 * remaining_nsamp))
 
-        for idx_cadrant in list_idx_cadrant:
+        for idx_quadrant in list_idx_quadrant:
 
             if verbose:
-                print('Working on a new cadrant')
+                print("Working on a new quadrant")
 
             # Select center coordinates
-            i = list_cadrant[idx_cadrant][0]
-            j = list_cadrant[idx_cadrant][1]
+            i = list_quadrant[idx_quadrant][0]
+            j = list_quadrant[idx_quadrant][1]
 
-            if patch_shape == 'rectangular':
-                patch = values[nx_sub * i:nx_sub * (i + 1), ny_sub * j:ny_sub * (j + 1)].flatten()
-            elif patch_shape == 'circular':
-                center_x = np.floor(nx_sub*(i+1/2))
-                center_y = np.floor(ny_sub*(j+1/2))
-                mask = _create_circular_mask((nx, ny), center=[center_x, center_y], radius=rad)
+            # Get patch by masking the square or circular quadrant
+            if patch_shape.lower() == "square":
+                patch = values[
+                    kernel_size * i : kernel_size * (i + 1), kernel_size * j : kernel_size * (j + 1)
+                ].flatten()
+            elif patch_shape.lower() == "circular":
+                center_x = np.floor(kernel_size * (i + 1 / 2))
+                center_y = np.floor(kernel_size * (j + 1 / 2))
+                mask = _create_circular_mask((nx, ny), center=(center_x, center_y), radius=rad)
                 patch = values[mask]
             else:
-                raise ValueError('Patch method must be rectangular or circular.')
+                raise ValueError("Patch method must be square or circular.")
 
+            # Check that the patch is complete and has the minimum number of valid values
             nb_pixel_total = len(patch)
             nb_pixel_valid = len(patch[np.isfinite(patch)])
-            if nb_pixel_valid >= np.ceil(perc_min_valid / 100. * nb_pixel_total):
-                u=u+1
+            if nb_pixel_valid >= np.ceil(perc_min_valid / 100.0 * nb_pixel_total) and nb_pixel_total == nb_pixel_exact:
+                u = u + 1
                 if u > n_patches:
                     break
                 if verbose:
-                    print('Found valid cadrant ' + str(u) + ' (maximum: ' + str(n_patches) + ')')
+                    print("Found valid quadrant " + str(u) + " (maximum: " + str(n_patches) + ")")
 
                 df = pd.DataFrame()
-                df = df.assign(tile=[str(i) + '_' + str(j)])
-                for j, statistic in enumerate(statistics):
+                df = df.assign(tile=[str(i) + "_" + str(j)])
+                for j, statistic in enumerate(list_statistics_in_patch):
                     if isinstance(statistic, str):
-                        if statistic == 'count':
+                        if statistic == "count":
                             df[statistic] = [nb_pixel_valid]
                         else:
                             raise ValueError('No other string than "count" are supported for named statistics.')
                     else:
-                        df[statistics_name[j]] = [statistic(patch)]
+                        df[statistics_name[j]] = [statistic(patch[np.isfinite(patch)].astype("float64"))]
 
                 list_df.append(df)
 
         # Get remaining samples to draw
         remaining_nsamp = n_patches - u
-        # Remove cadrants already sampled from list
-        list_cadrant = [c for j, c in enumerate(list_cadrant) if j not in list_idx_cadrant]
+        # Remove quadrants already sampled from list
+        list_quadrant = [c for j, c in enumerate(list_quadrant) if j not in list_idx_quadrant]
 
-    if len(list_df)>0:
+    if len(list_df) > 0:
         df_all = pd.concat(list_df)
+        # The average statistic is computed on the first in-patch statistic
+        average_statistic = float(statistic_between_patches(df_all[statistics_name[0]].values))
+        nb_independent_patches = np.count_nonzero(np.isfinite(df_all[statistics_name[0]].values))
     else:
-        warnings.warn('No valid patch found covering this area: returning dataframe containing only nans' )
         df_all = pd.DataFrame()
-        for j, statistic in enumerate(statistics):
+        for j, _ in enumerate(list_statistics_in_patch):
             df_all[statistics_name[j]] = [np.nan]
+        average_statistic = np.nan
+        nb_independent_patches = 0
+        warnings.warn("No valid patch found covering this area size, returning NaN for statistic.")
 
-    return df_all
+    if return_in_patch_statistics:
+        return average_statistic, nb_independent_patches, exact_area, df_all
+    else:
+        return average_statistic, nb_independent_patches, exact_area
 
 
-def plot_variogram(df: pd.DataFrame, list_fit_fun: Optional[list[Callable[[np.ndarray], np.ndarray]]] = None,
-                   list_fit_fun_label: Optional[list[str]] = None, ax: matplotlib.axes.Axes | None = None,
-                   xscale='linear', xscale_range_split: Optional[list] = None,
-                   xlabel = None, ylabel = None, xlim = None, ylim = None):
+@overload
+def patches_method(
+    values: NDArrayf | RasterType,
+    areas: list[float],
+    gsd: float = None,
+    stable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    statistics_in_patch: tuple[Callable[[NDArrayf], np.floating[Any]] | str] = (np.nanmean,),
+    statistic_between_patches: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    perc_min_valid: float = 80.0,
+    patch_shape: str = "circular",
+    vectorized: bool = True,
+    convolution_method: str = "scipy",
+    n_patches: int = 1000,
+    verbose: bool = False,
+    *,
+    return_in_patch_statistics: Literal[False] = False,
+    random_state: None | int | np.random.RandomState = None,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def patches_method(
+    values: NDArrayf | RasterType,
+    areas: list[float],
+    gsd: float = None,
+    stable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    statistics_in_patch: tuple[Callable[[NDArrayf], np.floating[Any]] | str] = (np.nanmean,),
+    statistic_between_patches: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    perc_min_valid: float = 80.0,
+    patch_shape: str = "circular",
+    vectorized: bool = True,
+    convolution_method: str = "scipy",
+    n_patches: int = 1000,
+    verbose: bool = False,
+    *,
+    return_in_patch_statistics: Literal[True],
+    random_state: None | int | np.random.RandomState = None,
+) -> tuple[pd.DataFrame, pd.DataFrame]:
+    ...
+
+
+def patches_method(
+    values: NDArrayf | RasterType,
+    areas: list[float],
+    gsd: float = None,
+    stable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    unstable_mask: NDArrayf | VectorType | gpd.GeoDataFrame = None,
+    statistics_in_patch: tuple[Callable[[NDArrayf], np.floating[Any]] | str] = (np.nanmean,),
+    statistic_between_patches: Callable[[NDArrayf], np.floating[Any]] = nmad,
+    perc_min_valid: float = 80.0,
+    patch_shape: str = "circular",
+    vectorized: bool = True,
+    convolution_method: str = "scipy",
+    n_patches: int = 1000,
+    verbose: bool = False,
+    return_in_patch_statistics: bool = False,
+    random_state: None | int | np.random.RandomState = None,
+) -> pd.DataFrame | tuple[pd.DataFrame, pd.DataFrame]:
+
+    """
+    Monte Carlo patches method that samples multiple patches of terrain, square or circular, of a certain area and
+    computes a statistic in each patch. Then, another statistic is computed between all patches. Typically, a statistic
+    of central tendency (e.g., the mean) is computed for each patch, then a statistic of spread (e.g., the NMAD) is
+    computed on the central tendency of all the patches. This specific procedure gives an empirical estimate of the
+    standard error of the mean.
+
+    The function returns the exact areas of the patches, which might differ from the input due to rasterization of the
+    shapes.
+
+    By default, the fast vectorized method based on a convolution of all pixels is used, but only works with the mean.
+    To compute other statistics (possibly a list), the non-vectorized method that randomly samples quadrants of the
+    input array up to a certain number of patches "n_patches" can be used.
+
+    The per-patch statistics can be returned as a concatenated dataframe using the "return_in_patch_statistics"
+    argument, not done by default due to large sizes.
+
+    :param values: Values as array or Raster
+    :param areas: List of patch areas to process (squared unit of ground sampling distance; exact patch areas might not
+        always match these accurately due to rasterization, and are returned as outputs)
+    :param gsd: Ground sampling distance
+    :param stable_mask: Vector shapefile of stable terrain (if values is Raster), or boolean array of same shape as
+        values
+    :param unstable_mask: Vector shapefile of unstable terrain (if values is Raster), or boolean array of same shape
+        as values
+    :param statistics_in_patch: List of statistics to compute in each patch (count is computed by default;
+        only mean and count supported for vectorized version)
+    :param statistic_between_patches: Statistic to compute between all patches, typically a measure of spread, applied
+        to the first in-patch statistic, which is typically the mean
+    :param perc_min_valid: Minimum valid area in the patch
+    :param patch_shape: Shape of patch, either "circular" or "square"
+    :param vectorized: Whether to use the vectorized (convolution) method or the for loop in quadrants
+    :param convolution_method: Convolution method to use, either "scipy" or "numba" (only for vectorized)
+    :param n_patches: Maximum number of patches to sample (only for non-vectorized)
+    :param verbose: Print statement to console
+    :param return_in_patch_statistics: Whether to return the dataframe of statistics for all patches and areas
+    :param random_state: Random state or seed number to use for calculations (only for non-vectorized, for testing)
+
+    :return: Dataframe of statistic between patches with independent patches count and exact areas,
+        (Optional) Dataframe of per-patch statistics
+    """
+
+    # Get values with NaNs on unstable terrain, preserving the shape by default
+    values_arr, gsd = _preprocess_values_with_mask_to_array(
+        values=values, include_mask=stable_mask, exclude_mask=unstable_mask, gsd=gsd
+    )
+
+    # Initialize list of dataframe for the statistic on all patches
+    list_stats = []
+    list_nb_patches = []
+    list_exact_areas = []
+
+    # Initialize a list to concatenate full dataframes if we want to return them
+    if return_in_patch_statistics:
+        list_df = []
+
+    # Looping on areas
+    for area in areas:
+        # If vectorized, we run the convolution which only supports mean and count statistics
+        if vectorized:
+            outputs = _patches_convolution(
+                values=values_arr,
+                gsd=gsd,
+                area=area,
+                perc_min_valid=perc_min_valid,
+                patch_shape=patch_shape,
+                method=convolution_method,
+                statistic_between_patches=statistic_between_patches,
+                verbose=verbose,
+                return_in_patch_statistics=return_in_patch_statistics,
+            )
+
+        # If not, we run the quadrant loop method that supports any statistic
+        else:
+            outputs = _patches_loop_quadrants(
+                values=values_arr,
+                gsd=gsd,
+                area=area,
+                patch_shape=patch_shape,
+                n_patches=n_patches,
+                perc_min_valid=perc_min_valid,
+                statistics_in_patch=statistics_in_patch,
+                statistic_between_patches=statistic_between_patches,
+                verbose=verbose,
+                return_in_patch_statistics=return_in_patch_statistics,
+                random_state=random_state,
+            )
+
+        list_stats.append(outputs[0])
+        list_nb_patches.append(outputs[1])
+        list_exact_areas.append(outputs[2])
+        if return_in_patch_statistics:
+            # Here we'd need to write overload for all the patch subfunctions... maybe we can do this more easily with
+            # the function behaviour, ignoring for now.
+            df: pd.DataFrame = outputs[3]  # type: ignore
+            df["areas"] = area
+            df["exact_areas"] = outputs[2]
+            list_df.append(df)
+
+    # Produce final dataframe of statistic between patches per area
+    df_statistic = pd.DataFrame(
+        data={
+            statistic_between_patches.__name__: list_stats,
+            "nb_indep_patches": list_nb_patches,
+            "exact_areas": list_exact_areas,
+            "areas": areas,
+        }
+    )
+
+    if return_in_patch_statistics:
+        # Concatenate the complete dataframe
+        df_tot = pd.concat(list_df)
+        return df_statistic, df_tot
+    else:
+        return df_statistic
+
+
+def plot_variogram(
+    df: pd.DataFrame,
+    list_fit_fun: list[Callable[[NDArrayf], NDArrayf]] = None,
+    list_fit_fun_label: list[str] = None,
+    ax: matplotlib.axes.Axes = None,
+    xscale: str = "linear",
+    xscale_range_split: list[float] = None,
+    xlabel: str = None,
+    ylabel: str = None,
+    xlim: str = None,
+    ylim: str = None,
+) -> None:
     """
     Plot empirical variogram, and optionally also plot one or several model fits.
     Input dataframe is expected to be the output of xdem.spatialstats.sample_empirical_variogram.
     Input function model is expected to be the output of xdem.spatialstats.fit_sum_model_variogram.
 
     :param df: Empirical variogram, formatted as a dataframe with count (pairwise sample count), lags
-        (upper bound of spatial lag bin), exp (experimental variance), and err_exp (error on experimental variance).
+        (upper bound of spatial lag bin), exp (experimental variance), and err_exp (error on experimental variance)
     :param list_fit_fun: List of model function fits
     :param list_fit_fun_label: List of model function fits labels
     :param ax: Plotting ax to use, creates a new one by default
     :param xscale: Scale of X-axis
     :param xscale_range_split: List of ranges at which to split the figure
     :param xlabel: Label of X-axis
     :param ylabel: Label of Y-axis
@@ -2147,149 +2942,165 @@
         ax = plt.subplot(111)
     elif isinstance(ax, matplotlib.axes.Axes):
         fig = ax.figure
     else:
         raise ValueError("ax must be a matplotlib.axes.Axes instance or None")
 
     # Check format of input dataframe
-    expected_values = ['exp', 'lags', 'count']
+    expected_values = ["exp", "lags", "count"]
     for val in expected_values:
         if val not in df.columns.values:
-            raise ValueError('The expected variable "{}" is not part of the provided dataframe column names.'.format(val))
+            raise ValueError(f'The expected variable "{val}" is not part of the provided dataframe column names.')
 
     # Hide axes for the main subplot (which will be subdivded)
     ax.axis("off")
 
     if ylabel is None:
-        ylabel = r'Variance [$\mu$ $\pm \sigma$]'
+        ylabel = r"Variance [$\mu$ $\pm \sigma$]"
     if xlabel is None:
-        xlabel = 'Spatial lag (m)'
+        xlabel = "Spatial lag (m)"
 
     init_gridsize = [10, 10]
     # Create parameters to split x axis into different linear scales
     # If there is no split, get parameters for a single subplot
     if xscale_range_split is None:
-        nb_subpanels=1
-        if xscale == 'log':
-            xmin = [np.min(df.lags)/2]
+        nb_subpanels = 1
+        if xscale == "log":
+            xmin = [np.min(df.lags) / 2]
         else:
             xmin = [0]
         xmax = [np.max(df.lags)]
         xgridmin = [0]
         xgridmax = [init_gridsize[0]]
         gridsize = init_gridsize
     # Otherwise, derive a list for each subplot
     else:
         # Add initial zero if not in input
         if xscale_range_split[0] != 0:
-            if xscale == 'log':
-                first_xmin = np.min(df.lags)/2
+            if xscale == "log":
+                first_xmin = np.min(df.lags) / 2
             else:
                 first_xmin = 0
             xscale_range_split = [first_xmin] + xscale_range_split
         # Add maximum distance if not in input
         if xscale_range_split[-1] != np.max(df.lags):
             xscale_range_split.append(np.max(df.lags))
 
         # Scale grid size by the number of subpanels
-        nb_subpanels = len(xscale_range_split)-1
+        nb_subpanels = len(xscale_range_split) - 1
         gridsize = init_gridsize.copy()
         gridsize[0] *= nb_subpanels
         # Create list of parameters to pass to ax/grid objects of subpanels
-        xmin, xmax, xgridmin, xgridmax = ([] for i in range(4))
+        xmin = []
+        xmax = []
+        xgridmin = []
+        xgridmax = []
         for i in range(nb_subpanels):
             xmin.append(xscale_range_split[i])
-            xmax.append(xscale_range_split[i+1])
-            xgridmin.append(init_gridsize[0]*i)
-            xgridmax.append(init_gridsize[0]*(i+1))
+            xmax.append(xscale_range_split[i + 1])
+            xgridmin.append(init_gridsize[0] * i)
+            xgridmax.append(init_gridsize[0] * (i + 1))
 
     # Need a grid plot to show the sample count and the statistic
     grid = plt.GridSpec(gridsize[1], gridsize[0], wspace=0.5, hspace=0.5)
 
     # Loop over each subpanel
     for k in range(nb_subpanels):
         # First, an axis to plot the sample histogram
-        ax0 = ax.inset_axes(grid[:3, xgridmin[k]:xgridmax[k]].get_position(fig).bounds)
+        ax0 = ax.inset_axes(grid[:3, xgridmin[k] : xgridmax[k]].get_position(fig).bounds)
         ax0.set_xscale(xscale)
         ax0.set_xticks([])
 
         # Plot the histogram manually with fill_between
         interval_var = [0] + list(df.lags)
         for i in range(len(df)):
-            count = df['count'].values[i]
-            ax0.fill_between([interval_var[i], interval_var[i+1]], [0] * 2, [count] * 2,
-                             facecolor=plt.cm.Greys(0.75), alpha=1,
-                             edgecolor='white', linewidth=0.5)
+            count = df["count"].values[i]
+            ax0.fill_between(
+                [interval_var[i], interval_var[i + 1]],
+                [0] * 2,
+                [count] * 2,
+                facecolor=plt.cm.Greys(0.75),
+                alpha=1,
+                edgecolor="white",
+                linewidth=0.5,
+            )
         if k == 0:
-            ax0.set_ylabel('Sample count')
-        # Scientific format to avoid undesired additional space on the label side
-            ax0.ticklabel_format(axis='y', style='sci', scilimits=(0, 0))
+            ax0.set_ylabel("Sample count")
+            # Scientific format to avoid undesired additional space on the label side
+            ax0.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
         else:
             ax0.set_yticks([])
         # Ignore warnings for log scales
         ax0.set_xlim((xmin[k], xmax[k]))
 
         # Now, plot the statistic of the data
-        ax1 = ax.inset_axes(grid[3:, xgridmin[k]:xgridmax[k]].get_position(fig).bounds)
+        ax1 = ax.inset_axes(grid[3:, xgridmin[k] : xgridmax[k]].get_position(fig).bounds)
 
         # Get the lags bin centers
         bins_center = np.subtract(df.lags, np.diff([0] + df.lags.tolist()) / 2)
 
         # If all the estimated errors are all NaN (single run), simply plot the empirical variogram
         if np.all(np.isnan(df.err_exp)):
-            ax1.scatter(bins_center, df.exp, label='Empirical variogram', color='blue', marker='x')
+            ax1.scatter(bins_center, df.exp, label="Empirical variogram", color="blue", marker="x")
         # Otherwise, plot the error estimates through multiple runs
         else:
-            ax1.errorbar(bins_center, df.exp, yerr=df.err_exp, label='Empirical variogram (1-sigma s.d)', fmt='x')
+            ax1.errorbar(bins_center, df.exp, yerr=df.err_exp, label="Empirical variogram (1-sigma std error)", fmt="x")
 
         # If a list of functions is passed, plot the modelled variograms
         if list_fit_fun is not None:
             for i, fit_fun in enumerate(list_fit_fun):
                 x = np.linspace(xmin[k], xmax[k], 1000)
                 y = fit_fun(x)
 
                 if list_fit_fun_label is not None:
-                    ax1.plot(x, y, linestyle='dashed', label=list_fit_fun_label[i], zorder=30)
+                    ax1.plot(x, y, linestyle="dashed", label=list_fit_fun_label[i], zorder=30)
                 else:
-                    ax1.plot(x, y, linestyle='dashed', color='black', zorder=30)
+                    ax1.plot(x, y, linestyle="dashed", color="black", zorder=30)
 
             if list_fit_fun_label is None:
-                ax1.plot([],[],linestyle='dashed',color='black',label='Model fit')
+                ax1.plot([], [], linestyle="dashed", color="black", label="Model fit")
 
         ax1.set_xscale(xscale)
-        if nb_subpanels>1 and k == (nb_subpanels-1):
+        if nb_subpanels > 1 and k == (nb_subpanels - 1):
             ax1.xaxis.set_ticks(np.linspace(xmin[k], xmax[k], 3))
-        elif nb_subpanels>1:
-            ax1.xaxis.set_ticks(np.linspace(xmin[k],xmax[k],3)[:-1])
+        elif nb_subpanels > 1:
+            ax1.xaxis.set_ticks(np.linspace(xmin[k], xmax[k], 3)[:-1])
 
         if xlim is None:
             ax1.set_xlim((xmin[k], xmax[k]))
         else:
             ax1.set_xlim(xlim)
 
         if ylim is not None:
             ax1.set_ylim(ylim)
         else:
             if np.all(np.isnan(df.err_exp)):
-                ax1.set_ylim((0, 1.05*np.nanmax(df.exp)))
+                ax1.set_ylim((0, 1.05 * np.nanmax(df.exp)))
             else:
-                ax1.set_ylim((0, np.nanmax(df.exp)+np.nanmean(df.err_exp)))
+                ax1.set_ylim((0, np.nanmax(df.exp) + np.nanmean(df.err_exp)))
 
-        if k == int(nb_subpanels/2):
+        if k == int(nb_subpanels / 2):
             ax1.set_xlabel(xlabel)
         if k == nb_subpanels - 1:
-            ax1.legend(loc='lower right')
+            ax1.legend(loc="lower right")
         if k == 0:
             ax1.set_ylabel(ylabel)
         else:
             ax1.set_yticks([])
 
 
-def plot_1d_binning(df: pd.DataFrame, var_name: str, statistic_name: str, label_var: Optional[str] = None,
-                    label_statistic: Optional[str] = None, min_count: int = 30, ax: matplotlib.axes.Axes | None = None):
+def plot_1d_binning(
+    df: pd.DataFrame,
+    var_name: str,
+    statistic_name: str,
+    label_var: str | None = None,
+    label_statistic: str | None = None,
+    min_count: int = 30,
+    ax: matplotlib.axes.Axes | None = None,
+) -> None:
     """
     Plot a statistic and its count along a single binning variable.
     Input is expected to be formatted as the output of the xdem.spatialstats.nd_binning function.
 
     :param df: Output dataframe of nd_binning
     :param var_name: Name of binning variable to plot
     :param statistic_name: Name of statistic of interest to plot
@@ -2305,71 +3116,98 @@
         ax = plt.subplot(111)
     elif isinstance(ax, matplotlib.axes.Axes):
         fig = ax.figure
     else:
         raise ValueError("ax must be a matplotlib.axes.Axes instance or None.")
 
     if var_name not in df.columns.values:
-        raise ValueError('The variable "{}" is not part of the provided dataframe column names.'.format(var_name))
+        raise ValueError(f'The variable "{var_name}" is not part of the provided dataframe column names.')
 
     if statistic_name not in df.columns.values:
-        raise ValueError('The statistic "{}" is not part of the provided dataframe column names.'.format(statistic_name))
+        raise ValueError(f'The statistic "{statistic_name}" is not part of the provided dataframe column names.')
 
     # Hide axes for the main subplot (which will be subdivded)
     ax.axis("off")
 
     if label_var is None:
         label_var = var_name
     if label_statistic is None:
         label_statistic = statistic_name
 
     # Subsample to 1D and for the variable of interest
     df_sub = df[np.logical_and(df.nd == 1, np.isfinite(pd.IntervalIndex(df[var_name]).mid))].copy()
     # Remove statistic calculated in bins with too low count
-    df_sub.loc[df_sub['count']<min_count, statistic_name] = np.nan
+    df_sub.loc[df_sub["count"] < min_count, statistic_name] = np.nan
 
     # Need a grid plot to show the sample count and the statistic
     grid = plt.GridSpec(10, 10, wspace=0.5, hspace=0.5)
 
     # First, an axis to plot the sample histogram
     ax0 = ax.inset_axes(grid[:3, :].get_position(fig).bounds)
     ax0.set_xticks([])
 
     # Plot the histogram manually with fill_between
     interval_var = pd.IntervalIndex(df_sub[var_name])
-    for i in range(len(df_sub) ):
-        count = df_sub['count'].values[i]
-        ax0.fill_between([interval_var[i].left, interval_var[i].right], [0] * 2, [count] * 2, facecolor=plt.cm.Greys(0.75), alpha=1,
-                         edgecolor='white',linewidth=0.5)
-    ax0.set_ylabel('Sample count')
+    for i in range(len(df_sub)):
+        count = df_sub["count"].values[i]
+        ax0.fill_between(
+            [interval_var[i].left, interval_var[i].right],
+            [0] * 2,
+            [count] * 2,
+            facecolor=plt.cm.Greys(0.75),
+            alpha=1,
+            edgecolor="white",
+            linewidth=0.5,
+        )
+    ax0.set_ylabel("Sample count")
     # Scientific format to avoid undesired additional space on the label side
-    ax0.ticklabel_format(axis='y',style='sci',scilimits=(0,0))
+    ax0.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
 
     # Try to identify if the count is always the same
     # (np.quantile can have a couple undesired effet, so leave an error margin of 2 wrong bins and 5 count difference)
-    if np.sum(~(np.abs(df_sub['count'].values[0] - df_sub['count'].values) < 5)) <= 2:
-        ax0.text(0.5, 0.5, "Fixed number of\n samples: "+'{:,}'.format(int(df_sub['count'].values[0])), ha='center', va='center',
-                 fontweight='bold', transform=ax0.transAxes, bbox=dict(facecolor='white', alpha=0.8))
+    if np.sum(~(np.abs(df_sub["count"].values[0] - df_sub["count"].values) < 5)) <= 2:
+        ax0.text(
+            0.5,
+            0.5,
+            "Fixed number of\n samples: " + "{:,}".format(int(df_sub["count"].values[0])),
+            ha="center",
+            va="center",
+            fontweight="bold",
+            transform=ax0.transAxes,
+            bbox=dict(facecolor="white", alpha=0.8),
+        )
 
-    ax0.set_ylim((0,1.1*np.max(df_sub['count'].values)))
-    ax0.set_xlim((np.min(interval_var.left),np.max(interval_var.right)))
+    ax0.set_ylim((0, 1.1 * np.max(df_sub["count"].values)))
+    ax0.set_xlim((np.min(interval_var.left), np.max(interval_var.right)))
 
     # Now, plot the statistic of the data
     ax1 = ax.inset_axes(grid[3:, :].get_position(fig).bounds)
-    ax1.scatter(interval_var.mid, df_sub[statistic_name],marker='x')
+    ax1.scatter(interval_var.mid, df_sub[statistic_name], marker="x")
     ax1.set_xlabel(label_var)
     ax1.set_ylabel(label_statistic)
-    ax1.set_xlim((np.min(interval_var.left),np.max(interval_var.right)))
+    ax1.set_xlim((np.min(interval_var.left), np.max(interval_var.right)))
 
 
-def plot_2d_binning(df: pd.DataFrame, var_name_1: str, var_name_2: str, statistic_name: str,
-                    label_var_name_1: Optional[str] = None, label_var_name_2: Optional[str] = None,
-                    label_statistic: Optional[str] = None, cmap: matplotlib.colors.Colormap = plt.cm.Reds, min_count: int = 30,
-                    scale_var_1: str = 'linear', scale_var_2: str = 'linear', vmin: float = None, vmax: float = None,
-                    nodata_color: Union[str,tuple[float,float,float,float]] = 'yellow', ax: matplotlib.axes.Axes | None = None):
+def plot_2d_binning(
+    df: pd.DataFrame,
+    var_name_1: str,
+    var_name_2: str,
+    statistic_name: str,
+    label_var_name_1: str | None = None,
+    label_var_name_2: str | None = None,
+    label_statistic: str | None = None,
+    cmap: matplotlib.colors.Colormap = plt.cm.Reds,
+    min_count: int = 30,
+    scale_var_1: str = "linear",
+    scale_var_2: str = "linear",
+    vmin: np.floating[Any] = None,
+    vmax: np.floating[Any] = None,
+    nodata_color: str | tuple[float, float, float, float] = "yellow",
+    ax: matplotlib.axes.Axes | None = None,
+) -> None:
     """
     Plot one statistic and its count along two binning variables.
     Input is expected to be formatted as the output of the xdem.spatialstats.nd_binning function.
 
     :param df: Output dataframe of nd_binning
     :param var_name_1: Name of first binning variable to plot
     :param var_name_2: Name of second binning variable to plot
@@ -2385,37 +3223,44 @@
     :param vmax: Maximum statistic value in colormap range
     :param nodata_color: Color for no data bins
     :param ax: Plotting ax to use, creates a new one by default
     """
 
     # Create axes
     if ax is None:
-        fig = plt.figure(figsize=(8,6))
+        fig = plt.figure(figsize=(8, 6))
         ax = plt.subplot(111)
     elif isinstance(ax, matplotlib.axes.Axes):
         fig = ax.figure
     else:
         raise ValueError("ax must be a matplotlib.axes.Axes instance or None.")
 
     if var_name_1 not in df.columns.values:
-        raise ValueError('The variable "{}" is not part of the provided dataframe column names.'.format(var_name_1))
+        raise ValueError(f'The variable "{var_name_1}" is not part of the provided dataframe column names.')
     elif var_name_2 not in df.columns.values:
-        raise ValueError('The variable "{}" is not part of the provided dataframe column names.'.format(var_name_2))
+        raise ValueError(f'The variable "{var_name_2}" is not part of the provided dataframe column names.')
 
     if statistic_name not in df.columns.values:
-        raise ValueError('The statistic "{}" is not part of the provided dataframe column names.'.format(statistic_name))
+        raise ValueError(f'The statistic "{statistic_name}" is not part of the provided dataframe column names.')
 
     # Hide axes for the main subplot (which will be subdivded)
     ax.axis("off")
 
     # Subsample to 2D and for the variables of interest
-    df_sub = df[np.logical_and.reduce((df.nd == 2, np.isfinite(pd.IntervalIndex(df[var_name_1]).mid),
-                                       np.isfinite(pd.IntervalIndex(df[var_name_2]).mid)))].copy()
+    df_sub = df[
+        np.logical_and.reduce(
+            (
+                df.nd == 2,
+                np.isfinite(pd.IntervalIndex(df[var_name_1]).mid),
+                np.isfinite(pd.IntervalIndex(df[var_name_2]).mid),
+            )
+        )
+    ].copy()
     # Remove statistic calculated in bins with too low count
-    df_sub.loc[df_sub['count']<min_count, statistic_name] = np.nan
+    df_sub.loc[df_sub["count"] < min_count, statistic_name] = np.nan
 
     # Let's do a 4 panel figure:
     # two histograms for the binning variables
     # + a colored grid to display the statistic calculated on the value of interest
     # + a legend panel with statistic colormap and nodata color
 
     # For some reason the scientific notation displays weirdly for default figure size
@@ -2424,134 +3269,172 @@
     # First, an horizontal axis on top to plot the sample histogram of the first variable
     ax0 = ax.inset_axes(grid[:3, :-3].get_position(fig).bounds)
     ax0.set_xscale(scale_var_1)
     ax0.set_xticklabels([])
 
     # Plot the histogram manually with fill_between
     interval_var_1 = pd.IntervalIndex(df_sub[var_name_1])
-    df_sub['var1_mid'] = interval_var_1.mid.values
+    df_sub["var1_mid"] = interval_var_1.mid.values
     unique_var_1 = np.unique(df_sub.var1_mid)
     list_counts = []
     for i in range(len(unique_var_1)):
         df_var1 = df_sub[df_sub.var1_mid == unique_var_1[i]]
-        count = np.nansum(df_var1['count'].values)
+        count = np.nansum(df_var1["count"].values)
         list_counts.append(count)
-        ax0.fill_between([df_var1[var_name_1].values[0].left, df_var1[var_name_1].values[0].right], [0] * 2, [count] * 2, facecolor=plt.cm.Greys(0.75), alpha=1,
-                         edgecolor='white', linewidth=0.5)
-    ax0.set_ylabel('Sample count')
+        ax0.fill_between(
+            [df_var1[var_name_1].values[0].left, df_var1[var_name_1].values[0].right],
+            [0] * 2,
+            [count] * 2,
+            facecolor=plt.cm.Greys(0.75),
+            alpha=1,
+            edgecolor="white",
+            linewidth=0.5,
+        )
+    ax0.set_ylabel("Sample count")
     # In case the axis value does not agree with the scale (e.g., 0 for log scale)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        ax0.set_ylim((0,1.1*np.max(list_counts)))
-        ax0.set_xlim((np.min(interval_var_1.left),np.max(interval_var_1.right)))
-    ax0.ticklabel_format(axis='y',style='sci',scilimits=(0,0))
-    ax0.spines['top'].set_visible(False)
-    ax0.spines['right'].set_visible(False)
+        ax0.set_ylim((0, 1.1 * np.max(list_counts)))
+        ax0.set_xlim((np.min(interval_var_1.left), np.max(interval_var_1.right)))
+    ax0.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
+    ax0.spines["top"].set_visible(False)
+    ax0.spines["right"].set_visible(False)
     # Try to identify if the count is always the same
     if np.sum(~(np.abs(list_counts[0] - np.array(list_counts)) < 5)) <= 2:
-        ax0.text(0.5, 0.5, "Fixed number of\nsamples: " + '{:,}'.format(int(list_counts[0])), ha='center', va='center',
-                 fontweight='bold', transform=ax0.transAxes, bbox=dict(facecolor='white', alpha=0.8))
+        ax0.text(
+            0.5,
+            0.5,
+            "Fixed number of\nsamples: " + f"{int(list_counts[0]):,}",
+            ha="center",
+            va="center",
+            fontweight="bold",
+            transform=ax0.transAxes,
+            bbox=dict(facecolor="white", alpha=0.8),
+        )
 
     # Second, a vertical axis on the right to plot the sample histogram of the second variable
     ax1 = ax.inset_axes(grid[3:, -3:].get_position(fig).bounds)
     ax1.set_yscale(scale_var_2)
     ax1.set_yticklabels([])
 
     # Plot the histogram manually with fill_between
     interval_var_2 = pd.IntervalIndex(df_sub[var_name_2])
-    df_sub['var2_mid'] = interval_var_2.mid.values
+    df_sub["var2_mid"] = interval_var_2.mid.values
     unique_var_2 = np.unique(df_sub.var2_mid)
     list_counts = []
     for i in range(len(unique_var_2)):
         df_var2 = df_sub[df_sub.var2_mid == unique_var_2[i]]
-        count = np.nansum(df_var2['count'].values)
+        count = np.nansum(df_var2["count"].values)
         list_counts.append(count)
-        ax1.fill_between([0, count], [df_var2[var_name_2].values[0].left] * 2, [df_var2[var_name_2].values[0].right] * 2, facecolor=plt.cm.Greys(0.75),
-                         alpha=1, edgecolor='white', linewidth=0.5)
-    ax1.set_xlabel('Sample count')
+        ax1.fill_between(
+            [0, count],
+            [df_var2[var_name_2].values[0].left] * 2,
+            [df_var2[var_name_2].values[0].right] * 2,
+            facecolor=plt.cm.Greys(0.75),
+            alpha=1,
+            edgecolor="white",
+            linewidth=0.5,
+        )
+    ax1.set_xlabel("Sample count")
     # In case the axis value does not agree with the scale (e.g., 0 for log scale)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        ax1.set_xlim((0,1.1*np.max(list_counts)))
-        ax1.set_ylim((np.min(interval_var_2.left),np.max(interval_var_2.right)))
-    ax1.ticklabel_format(axis='x',style='sci',scilimits=(0,0))
-    ax1.spines['top'].set_visible(False)
-    ax1.spines['right'].set_visible(False)
+        ax1.set_xlim((0, 1.1 * np.max(list_counts)))
+        ax1.set_ylim((np.min(interval_var_2.left), np.max(interval_var_2.right)))
+    ax1.ticklabel_format(axis="x", style="sci", scilimits=(0, 0))
+    ax1.spines["top"].set_visible(False)
+    ax1.spines["right"].set_visible(False)
     # Try to identify if the count is always the same
     if np.sum(~(np.abs(list_counts[0] - np.array(list_counts)) < 5)) <= 2:
-        ax1.text(0.5, 0.5, "Fixed number of\nsamples: " + '{:,}'.format(int(list_counts[0])), ha='center', va='center',
-                 fontweight='bold', transform=ax1.transAxes, rotation=90, bbox=dict(facecolor='white', alpha=0.8))
+        ax1.text(
+            0.5,
+            0.5,
+            "Fixed number of\nsamples: " + f"{int(list_counts[0]):,}",
+            ha="center",
+            va="center",
+            fontweight="bold",
+            transform=ax1.transAxes,
+            rotation=90,
+            bbox=dict(facecolor="white", alpha=0.8),
+        )
 
     # Third, an axis to plot the data as a colored grid
     ax2 = ax.inset_axes(grid[3:, :-3].get_position(fig).bounds)
 
     # Define limits of colormap is none are provided, robust max and min using percentiles
     if vmin is None and vmax is None:
         vmax = np.nanpercentile(df_sub[statistic_name].values, 99)
         vmin = np.nanpercentile(df_sub[statistic_name].values, 1)
 
     # Create custom colormap
-    col_bounds = np.array([vmin, np.mean([vmin,vmax]), vmax])
+    col_bounds = np.array([vmin, np.mean(np.asarray([vmin, vmax])), vmax])
     cb = []
     cb_val = np.linspace(0, 1, len(col_bounds))
     for j in range(len(cb_val)):
         cb.append(cmap(cb_val[j]))
-    cmap_cus = colors.LinearSegmentedColormap.from_list('my_cb', list(
-        zip((col_bounds - min(col_bounds)) / (max(col_bounds - min(col_bounds))), cb)), N=1000)
+    cmap_cus = colors.LinearSegmentedColormap.from_list(
+        "my_cb", list(zip((col_bounds - min(col_bounds)) / (max(col_bounds - min(col_bounds))), cb)), N=1000
+    )
 
     # Plot a 2D colored grid using fill_between
     for i in range(len(unique_var_1)):
         for j in range(len(unique_var_2)):
             df_both = df_sub[np.logical_and(df_sub.var1_mid == unique_var_1[i], df_sub.var2_mid == unique_var_2[j])]
 
             stat = df_both[statistic_name].values[0]
             if np.isfinite(stat):
-                stat_col = max(0.0001,min(0.9999,(stat - min(col_bounds))/(max(col_bounds)-min(col_bounds))))
+                stat_col = max(0.0001, min(0.9999, (stat - min(col_bounds)) / (max(col_bounds) - min(col_bounds))))
                 col = cmap_cus(stat_col)
             else:
                 col = nodata_color
 
-            ax2.fill_between([df_both[var_name_1].values[0].left, df_both[var_name_1].values[0].right], [df_both[var_name_2].values[0].left] * 2,
-                            [df_both[var_name_2].values[0].right] * 2, facecolor=col, alpha=1, edgecolor='white')
+            ax2.fill_between(
+                [df_both[var_name_1].values[0].left, df_both[var_name_1].values[0].right],
+                [df_both[var_name_2].values[0].left] * 2,
+                [df_both[var_name_2].values[0].right] * 2,
+                facecolor=col,
+                alpha=1,
+                edgecolor="white",
+            )
 
     ax2.set_xlabel(label_var_name_1)
     ax2.set_ylabel(label_var_name_2)
     ax2.set_xscale(scale_var_1)
     ax2.set_yscale(scale_var_2)
     # In case the axis value does not agree with the scale (e.g., 0 for log scale)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        ax2.set_xlim((np.min(interval_var_1.left),np.max(interval_var_1.right)))
-        ax2.set_ylim((np.min(interval_var_2.left),np.max(interval_var_2.right)))
+        ax2.set_xlim((np.min(interval_var_1.left), np.max(interval_var_1.right)))
+        ax2.set_ylim((np.min(interval_var_2.left), np.max(interval_var_2.right)))
 
     # Fourth and finally, add a colormap and nodata color to the legend
     axcmap = ax.inset_axes(grid[:3, -3:].get_position(fig).bounds)
 
     # Remove ticks, labels, frame
     axcmap.set_xticks([])
     axcmap.set_yticks([])
-    axcmap.spines['top'].set_visible(False)
-    axcmap.spines['left'].set_visible(False)
-    axcmap.spines['right'].set_visible(False)
-    axcmap.spines['bottom'].set_visible(False)
+    axcmap.spines["top"].set_visible(False)
+    axcmap.spines["left"].set_visible(False)
+    axcmap.spines["right"].set_visible(False)
+    axcmap.spines["bottom"].set_visible(False)
 
     # Create an inset axis to manage the scale of the colormap
-    cbaxes = axcmap.inset_axes([0, 0.75, 1, 0.2], label='cmap')
+    cbaxes = axcmap.inset_axes([0, 0.75, 1, 0.2], label="cmap")
 
     # Create colormap object and plot
     norm = colors.Normalize(vmin=min(col_bounds), vmax=max(col_bounds))
     sm = plt.cm.ScalarMappable(cmap=cmap_cus, norm=norm)
     sm.set_array([])
-    cb = plt.colorbar(sm, cax=cbaxes, orientation='horizontal', extend='both', shrink=0.8)
+    cb = plt.colorbar(sm, cax=cbaxes, orientation="horizontal", extend="both", shrink=0.8)
     cb.ax.tick_params(width=0.5, length=2)
     cb.set_label(label_statistic)
 
     # Create an inset axis to manage the scale of the nodata legend
-    nodata = axcmap.inset_axes([0.4, 0.1, 0.2, 0.2], label='nodata')
+    nodata = axcmap.inset_axes([0.4, 0.1, 0.2, 0.2], label="nodata")
 
     # Plot a nodata legend
     nodata.fill_between([0, 1], [0, 0], [1, 1], facecolor=nodata_color)
     nodata.set_xlim((0, 1))
     nodata.set_ylim((0, 1))
     nodata.set_xticks([])
     nodata.set_yticks([])
-    nodata.text(0.5, -0.25, 'No data', ha='center',va='top')
+    nodata.text(0.5, -0.25, "No data", ha="center", va="top")
```

### Comparing `xdem-0.0.7/xdem/terrain.py` & `xdem-0.0.8/xdem/terrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 """Terrain attribute calculations, such as slope, aspect, hillshade, curvature and ruggedness indexes."""
 from __future__ import annotations
 
 import warnings
 from typing import Sized, overload
 
+import geoutils as gu
 import numba
 import numpy as np
-import rasterio as rio
+from geoutils.raster import Raster, RasterType
 
-import geoutils as gu
-from geoutils.georaster import RasterType, Raster
+from xdem._typing import MArrayf, NDArrayf
 
 try:
     import richdem as rd
+
     _has_rd = True
 except ImportError:
     _has_rd = False
 
 
-def _rio_to_rda(ds: rio.DatasetReader) -> rd.rdarray:
+def _raster_to_rda(rst: RasterType) -> rd.rdarray:
     """
-    Get georeferenced richDEM array from rasterio dataset
-    :param ds: DEM
+    Get georeferenced richDEM array from geoutils.Raster
+    :param rst: DEM as raster
     :return: DEM
     """
-    arr = ds.read(1)
-    rda = rd.rdarray(arr, no_data=ds.get_nodatavals()[0])
-    rda.geotransform = ds.get_transform()
-    rda.projection = ds.get_gcps()
+    arr = rst.data.filled(rst.nodata).squeeze()
+    rda = rd.rdarray(arr, no_data=rst.nodata)
+    rda.geotransform = rst.transform.to_gdal()
 
     return rda
 
 
-def _get_terrainattr_richdem(ds: rio.DatasetReader, attribute='slope_radians') -> np.ndarray:
+def _get_terrainattr_richdem(rst: RasterType, attribute: str = "slope_radians") -> NDArrayf:
     """
     Derive terrain attribute for DEM opened with rasterio. One of "slope_degrees", "slope_percentage", "aspect",
     "profile_curvature", "planform_curvature", "curvature" and others (see RichDEM documentation).
-    :param ds: DEM
+    :param rst: DEM as raster
     :param attribute: RichDEM terrain attribute
     :return:
     """
-    rda = _rio_to_rda(ds)
+    rda = _raster_to_rda(rst)
     terrattr = rd.TerrainAttribute(rda, attrib=attribute)
 
     return np.array(terrattr)
 
 
-@numba.njit(parallel=True)
+@numba.njit(parallel=True)  # type: ignore
 def _get_quadric_coefficients(
-    dem: np.ndarray, resolution: float, fill_method: str = "none", edge_method: str = "none",
-        make_rugosity: bool = False) -> np.ndarray:
+    dem: NDArrayf,
+    resolution: float,
+    fill_method: str = "none",
+    edge_method: str = "none",
+    make_rugosity: bool = False,
+) -> NDArrayf:
     """
     Run the pixel-wise analysis in parallel for a 3x3 window using the resolution.
 
     See the xdem.terrain.get_quadric_coefficients() docstring for more info.
     """
     # Rename the resolution
     L = resolution
@@ -105,15 +109,14 @@
                     row_indexer = row + k
                     col_indexer = col + j
                 Z[count] = dem[row_indexer, col_indexer]
                 count += 1
 
         # Get a mask of all invalid (nan or inf) values.
         invalids = ~np.isfinite(Z)
-        n_invalid = np.count_nonzero(invalids)
 
         # Skip the pixel if it and all of its neighbours are invalid
         if np.all(invalids):
             continue
 
         if np.count_nonzero(invalids) > 0:
             if fill_method_n == 0:
@@ -146,15 +149,15 @@
                     # Skip if this is the center pixel
                     if j == 0 and k == 0:
                         count_all += 1
                         continue
                     # The first eight elevation differences from the cell center
                     dzs[count_without_center] = Z[4] - Z[count_all]
                     # The first eight planimetric length that can be diagonal or straight from the center
-                    dls[count_without_center] = np.sqrt(j ** 2 + k ** 2)*L
+                    dls[count_without_center] = np.sqrt(j**2 + k**2) * L
                     count_all += 1
                     count_without_center += 1
 
             # Manually for the remaining eight segments between surrounding pixels:
             # First, four elevation differences along the x axis
             dzs[8] = Z[0] - Z[1]
             dzs[9] = Z[1] - Z[2]
@@ -165,18 +168,18 @@
             dzs[13] = Z[3] - Z[6]
             dzs[14] = Z[2] - Z[5]
             dzs[15] = Z[5] - Z[8]
             # For the planimetric lengths, all are equal to one
             dls[8:] = L
 
             # Finally, the half-surface length of each segment
-            hsl = np.sqrt(dzs ** 2 + dls ** 2) / 2
+            hsl = np.sqrt(dzs**2 + dls**2) / 2
 
-            # Starting from up direction anticlockwise, every triangle has 2 segments between center and surrounding pixels
-            # and 1 segment between surrounding pixels; pixel 4 is the center
+            # Starting from up direction anticlockwise, every triangle has 2 segments between center and surrounding
+            # pixels and 1 segment between surrounding pixels; pixel 4 is the center
             # above 4 the index of center-surrounding segment decrease by 1, as the center pixel was skipped
             # Triangle 1: pixels 3 and 0
             T1 = [hsl[3], hsl[0], hsl[12]]
             # Triangle 2: pixels 0 and 1
             T2 = [hsl[0], hsl[1], hsl[8]]
             # Triangle 3: pixels 1 and 2
             T3 = [hsl[1], hsl[2], hsl[9]]
@@ -202,20 +205,20 @@
                 # Surface area of triangle
                 A[count] = np.sqrt(hs * (hs - T[0]) * (hs - T[1]) * (hs - T[2]))
                 count += 1
 
         # Assign the A, B, C, D etc., factors to the output. This ugly syntax is needed to make parallel numba happy.
 
         # Coefficients of Zevenberg and Thorne (1987), Equations 3 to 11
-        output[0, row, col] = ((Z[0] + Z[2] + Z[6] + Z[8]) / 4 - (Z[1] + Z[3] + Z[5] + Z[7]) / 2 + Z[4]) / (L ** 4)  # A
-        output[1, row, col] = ((Z[0] + Z[2] - Z[6] - Z[8]) / 4 - (Z[1] - Z[7]) / 2) / (L ** 3)  # B
-        output[2, row, col] = ((-Z[0] + Z[2] - Z[6] + Z[8]) / 4 + (Z[3] - Z[5]) / 2) / (L ** 3)  # C
-        output[3, row, col] = ((Z[3] + Z[5]) / 2 - Z[4]) / (L ** 2)  # D
-        output[4, row, col] = ((Z[1] + Z[7]) / 2 - Z[4]) / (L ** 2)  # E
-        output[5, row, col] = (-Z[0] + Z[2] + Z[6] - Z[8]) / (4 * L ** 2)  # F
+        output[0, row, col] = ((Z[0] + Z[2] + Z[6] + Z[8]) / 4 - (Z[1] + Z[3] + Z[5] + Z[7]) / 2 + Z[4]) / (L**4)  # A
+        output[1, row, col] = ((Z[0] + Z[2] - Z[6] - Z[8]) / 4 - (Z[1] - Z[7]) / 2) / (L**3)  # B
+        output[2, row, col] = ((-Z[0] + Z[2] - Z[6] + Z[8]) / 4 + (Z[3] - Z[5]) / 2) / (L**3)  # C
+        output[3, row, col] = ((Z[3] + Z[5]) / 2 - Z[4]) / (L**2)  # D
+        output[4, row, col] = ((Z[1] + Z[7]) / 2 - Z[4]) / (L**2)  # E
+        output[5, row, col] = (-Z[0] + Z[2] + Z[6] - Z[8]) / (4 * L**2)  # F
         output[6, row, col] = (-Z[3] + Z[5]) / (2 * L)  # G
         output[7, row, col] = (Z[1] - Z[7]) / (2 * L)  # H
         output[8, row, col] = Z[4]  # I
 
         # Refined coefficients for slope of Horn (1981), page 18 bottom left equations.
         output[9, row, col] = ((Z[6] + 2 * Z[7] + Z[8]) - (Z[0] + 2 * Z[1] + Z[2])) / (8 * L)
         output[10, row, col] = ((Z[6] + 2 * Z[3] + Z[0]) - (Z[8] + 2 * Z[5] + Z[2])) / (8 * L)
@@ -224,16 +227,20 @@
         if make_rugosity:
             output[11, row, col] = sum(A) / L**2
 
     return output
 
 
 def get_quadric_coefficients(
-    dem: np.ndarray, resolution: float, fill_method: str = "none", edge_method: str = "none",
-        make_rugosity : bool = False) -> np.ndarray:
+    dem: NDArrayf,
+    resolution: float,
+    fill_method: str = "none",
+    edge_method: str = "none",
+    make_rugosity: bool = False,
+) -> NDArrayf:
     """
     Computes quadric and other coefficients on a fixed 3x3 pixel window, and that depends on the resolution.
     Returns the 9 coefficients of a quadric surface fit to every pixel in the raster, the 2 coefficients of optimized
     slope gradient, and the rugosity.
 
     For the quadric surface, based on Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107, also
     described in the documentation:
@@ -289,15 +296,15 @@
         array([0., 0.])
         >>> coeffs[11, 1, 1]
         1.4142135623730954
 
     :returns: An array of coefficients for each pixel of shape (9, row, col).
     """
     # This function only formats and validates the inputs. For the true functionality, see _get_quadric_coefficients()
-    dem_arr = gu.spatial_tools.get_array_and_mask(dem)[0]
+    dem_arr = gu.raster.get_array_and_mask(dem)[0]
 
     if len(dem_arr.shape) != 2:
         raise ValueError(
             f"Invalid input array shape: {dem.shape}, parsed into {dem_arr.shape}. "
             "Expected 2D array or 3D array of shape (1, row, col)"
         )
 
@@ -315,25 +322,34 @@
     ):
         if value.lower() not in allowed:
             raise ValueError(f"Invalid {name} method: '{value}'. Choices: {allowed}")
 
     # Try to run the numba JIT code. It should never fail at this point, so if it does, it should be reported!
     try:
         coeffs = _get_quadric_coefficients(
-            dem_arr, resolution, fill_method=fill_method.lower(), edge_method=edge_method.lower(),
-            make_rugosity=make_rugosity)
+            dem_arr,
+            resolution,
+            fill_method=fill_method.lower(),
+            edge_method=edge_method.lower(),
+            make_rugosity=make_rugosity,
+        )
     except Exception as exception:
         raise RuntimeError("Unhandled numba exception. Please raise an issue of what happened.") from exception
 
     return coeffs
 
-@numba.njit(parallel=True)
+
+@numba.njit(parallel=True)  # type: ignore
 def _get_windowed_indexes(
-    dem: np.ndarray, fill_method: str = "median", edge_method: str = "nearest", window_size: int = 3,
-    make_fractal_roughness: bool = False) -> np.ndarray:
+    dem: NDArrayf,
+    fill_method: str = "median",
+    edge_method: str = "nearest",
+    window_size: int = 3,
+    make_fractal_roughness: bool = False,
+) -> NDArrayf:
     """
     Run the pixel-wise analysis in parallel for any window size without using the resolution.
 
     See the xdem.terrain.get_windowed_indexes() docstring for more info.
     """
 
     # Allocate the outputs.
@@ -369,16 +385,16 @@
         count = 0
 
         # If edge_method == "none", validate that it's not near an edge. If so, leave the nans without filling.
         if edge_method_n == 2:
             if (row < hw) or (row >= (dem.shape[0] - hw)) or (col < hw) or (col >= (dem.shape[1] - hw)):
                 continue
 
-        for j in range(-hw, -hw+window_size):
-            for k in range(-hw, -hw+window_size):
+        for j in range(-hw, -hw + window_size):
+            for k in range(-hw, -hw + window_size):
                 # Here the "nearest" edge_method is performed.
                 if edge_method_n == 0:
                     row_indexer = min(max(row + k, 0), dem.shape[0] - 1)
                     col_indexer = min(max(col + j, 0), dem.shape[1] - 1)
                 elif edge_method_n == 1:
                     row_indexer = (row + k) % dem.shape[0]
                     col_indexer = (col + j) % dem.shape[1]
@@ -386,15 +402,14 @@
                     row_indexer = row + k
                     col_indexer = col + j
                 Z[count] = dem[row_indexer, col_indexer]
                 count += 1
 
         # Get a mask of all invalid (nan or inf) values.
         invalids = ~np.isfinite(Z)
-        n_invalid = np.count_nonzero(invalids)
 
         # Skip the pixel if it and all of its neighbours are invalid
         if np.all(invalids):
             continue
 
         if np.count_nonzero(invalids) > 0:
             if fill_method_n == 0:
@@ -408,56 +423,56 @@
                 continue
             else:
                 # This should not occur.
                 pass
 
         # Difference pixels between specific cells: only useful for Terrain Ruggedness Index
         count = 0
-        index_middle_pixel = int((window_size**2 - 1)/2)
+        index_middle_pixel = int((window_size**2 - 1) / 2)
         S = np.empty((window_size**2,))
-        for j in range(-hw, -hw + window_size):
-            for k in range(-hw, -hw + window_size):
+        for _j in range(-hw, -hw + window_size):
+            for _k in range(-hw, -hw + window_size):
                 S[count] = np.abs(Z[count] - Z[index_middle_pixel])
                 count += 1
 
         if make_fractal_roughness:
             # Fractal roughness computation according to the box-counting method of Taud and Parrot (2005)
             # First, we compute the number of voxels for each pixel of Equation 4
             count = 0
             V = np.empty((window_size, window_size))
             for j in range(-hw, -hw + window_size):
                 for k in range(-hw, -hw + window_size):
-                    T = (Z[count] - Z[index_middle_pixel])
+                    T = Z[count] - Z[index_middle_pixel]
                     # The following is the equivalent of np.clip, written like this for numba
                     if T < 0:
                         V[hw + j, hw + k] = 0
                     elif T > window_size:
                         V[hw + j, hw + k] = window_size
                     else:
                         V[hw + j, hw + k] = T
                     count += 1
 
-            # Then, we compute the maximum number of voxels for varying box splitting of the cube of side the window size,
-            # following Equation 5
+            # Then, we compute the maximum number of voxels for varying box splitting of the cube of side the window
+            # size, following Equation 5
 
             # Get all the divisors of the half window size
             list_box_sizes = []
             for j in range(1, hw + 1):
                 if hw % j == 0:
                     list_box_sizes.append(j)
 
             Ns = np.empty((len(list_box_sizes),))
-            for l in range(0, len(list_box_sizes)):
+            for l0 in range(0, len(list_box_sizes)):
                 # We loop over boxes of size q x q in the cube
-                q = list_box_sizes[l]
+                q = list_box_sizes[l0]
                 sumNs = 0
-                for j in range(0, int((window_size-1)/q)):
-                    for k in range(0, int((window_size-1)/q)):
-                        sumNs += np.max(V[slice(j*q, (j+1)*q), slice(k*q, (k+1)*q)].flatten())
-                Ns[l] = sumNs / q
+                for j in range(0, int((window_size - 1) / q)):
+                    for k in range(0, int((window_size - 1) / q)):
+                        sumNs += np.max(V[slice(j * q, (j + 1) * q), slice(k * q, (k + 1) * q)].flatten())
+                Ns[l0] = sumNs / q
 
             # Finally, we calculate the slope of the logarithm of Ns with q
             # We do the linear regression manually, as np.polyfit is not supported by numba
             x = np.log(np.array(list_box_sizes))
             y = np.log(Ns)
             # The number of observations
             n = len(x)
@@ -477,35 +492,41 @@
         # differences between center and neighbouring pixels
         output[0, row, col] = np.sqrt(np.sum(S**2))
         # Second output is the Terrain Ruggedness Index from Wilson et al. (2007): mean difference between center
         # and neighbouring pixels
         output[1, row, col] = np.sum(S) / (window_size**2 - 1)
         # Third output is the Topographic Position Index from Weiss (2001): difference between center and mean of
         # neighbouring pixels
-        output[2, row, col] =  Z[index_middle_pixel] - (np.sum(Z) - Z[index_middle_pixel]) / (window_size**2 - 1)
+        output[2, row, col] = Z[index_middle_pixel] - (np.sum(Z) - Z[index_middle_pixel]) / (window_size**2 - 1)
         # Fourth output is the Roughness from Dartnell (2000): difference between maximum and minimum of the window
         output[3, row, col] = np.max(Z) - np.min(Z)
 
         if make_fractal_roughness:
             # Fifth output is the Fractal Roughness from Taud et Parrot (2005): estimate of the fractal dimension
             # based on volume box-counting
             output[4, row, col] = D
 
     return output
 
 
 def get_windowed_indexes(
-    dem: np.ndarray, fill_method: str = "none", edge_method: str = "none", window_size: int = 3,
-    make_fractal_roughness: bool = False) -> np.ndarray:
+    dem: NDArrayf,
+    fill_method: str = "none",
+    edge_method: str = "none",
+    window_size: int = 3,
+    make_fractal_roughness: bool = False,
+) -> NDArrayf:
     """
     Return terrain indexes based on a windowed calculation of variable size, independent of the resolution.
 
     Includes:
 
-    - Terrain Ruggedness Index from Riley et al. (1999),  http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf, for topography and from Wilson et al. (2007), http://dx.doi.org/10.1080/01490410701295962, for bathymetry.
+    - Terrain Ruggedness Index from Riley et al. (1999),
+        http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf, for topography and from Wilson
+        et al. (2007), http://dx.doi.org/10.1080/01490410701295962, for bathymetry.
     - Topographic Position Index from Weiss (2001), http://www.jennessent.com/downloads/TPI-poster-TNC_18x22.pdf.
     - Roughness from Dartnell (2000), http://dx.doi.org/10.14358/PERS.70.9.1081.
     - Fractal roughness from Taud et Parrot (2005), https://doi.org/10.4000/geomorphologie.622.
 
     Nearly all are also referenced in Wilson et al. (2007).
 
     Where Z is the elevation, x is the distance from left-right and y is the distance from top-bottom.
@@ -547,15 +568,15 @@
         (5, 3, 3)
         >>> indexes[:4, 1, 1]
         array([2.82842712, 1.        , 1.        , 1.        ])
 
     :returns: An array of coefficients for each pixel of shape (5, row, col).
     """
     # This function only formats and validates the inputs. For the true functionality, see _get_quadric_coefficients()
-    dem_arr = gu.spatial_tools.get_array_and_mask(dem)[0]
+    dem_arr = gu.raster.get_array_and_mask(dem)[0]
 
     if len(dem_arr.shape) != 2:
         raise ValueError(
             f"Invalid input array shape: {dem.shape}, parsed into {dem_arr.shape}. "
             "Expected 2D array or 3D array of shape (1, row, col)"
         )
 
@@ -572,120 +593,127 @@
     ):
         if value.lower() not in allowed:
             raise ValueError(f"Invalid {name} method: '{value}'. Choices: {allowed}")
 
     # Try to run the numba JIT code. It should never fail at this point, so if it does, it should be reported!
     try:
         indexes = _get_windowed_indexes(
-            dem_arr, fill_method=fill_method.lower(), edge_method=edge_method.lower(),
-            window_size=window_size, make_fractal_roughness=make_fractal_roughness
+            dem_arr,
+            fill_method=fill_method.lower(),
+            edge_method=edge_method.lower(),
+            window_size=window_size,
+            make_fractal_roughness=make_fractal_roughness,
         )
     except Exception as exception:
         raise RuntimeError("Unhandled numba exception. Please raise an issue of what happened.") from exception
 
     return indexes
 
 
 @overload
 def get_terrain_attribute(
-    dem: np.ndarray | np.ma.masked_array,
+    dem: NDArrayf | MArrayf,
     attribute: str,
-    resolution: tuple[float, float] | float | None,
-    degrees: bool,
-    hillshade_altitude: float,
-    hillshade_azimuth: float,
-    hillshade_z_factor: float,
-    slope_method: str,
-    tri_method: str,
-    fill_method: str,
-    edge_method: str,
-    use_richdem: bool,
-    window_size: int
-) -> np.ndarray:
+    resolution: tuple[float, float] | float | None = None,
+    degrees: bool = True,
+    hillshade_altitude: float = 45.0,
+    hillshade_azimuth: float = 315.0,
+    hillshade_z_factor: float = 1.0,
+    slope_method: str = "Horn",
+    tri_method: str = "Riley",
+    fill_method: str = "none",
+    edge_method: str = "none",
+    use_richdem: bool = False,
+    window_size: int = 3,
+) -> NDArrayf:
     ...
 
 
 @overload
 def get_terrain_attribute(
-    dem: np.ndarray | np.ma.masked_array,
+    dem: NDArrayf | MArrayf,
     attribute: list[str],
-    resolution: tuple[float, float] | float | None,
-    degrees: bool,
-    hillshade_altitude: float,
-    hillshade_azimuth: float,
-    hillshade_z_factor: float,
-    slope_method: str,
-    tri_method: str,
-    fill_method: str,
-    edge_method: str,
-    use_richdem: bool,
-    window_size: int
-) -> list[np.ndarray]:
+    resolution: tuple[float, float] | float | None = None,
+    degrees: bool = True,
+    hillshade_altitude: float = 45.0,
+    hillshade_azimuth: float = 315.0,
+    hillshade_z_factor: float = 1.0,
+    slope_method: str = "Horn",
+    tri_method: str = "Riley",
+    fill_method: str = "none",
+    edge_method: str = "none",
+    use_richdem: bool = False,
+    window_size: int = 3,
+) -> list[NDArrayf]:
     ...
 
+
 @overload
 def get_terrain_attribute(
     dem: RasterType,
-    attribute: str,
-    resolution: tuple[float, float] | float | None,
-    degrees: bool,
-    hillshade_altitude: float,
-    hillshade_azimuth: float,
-    hillshade_z_factor: float,
-    slope_method: str,
-    tri_method: str,
-    fill_method: str,
-    edge_method: str,
-    use_richdem: bool,
-    window_size: int
-) -> Raster:
+    attribute: list[str],
+    resolution: tuple[float, float] | float | None = None,
+    degrees: bool = True,
+    hillshade_altitude: float = 45.0,
+    hillshade_azimuth: float = 315.0,
+    hillshade_z_factor: float = 1.0,
+    slope_method: str = "Horn",
+    tri_method: str = "Riley",
+    fill_method: str = "none",
+    edge_method: str = "none",
+    use_richdem: bool = False,
+    window_size: int = 3,
+) -> list[RasterType]:
     ...
 
+
 @overload
 def get_terrain_attribute(
     dem: RasterType,
-    attribute: list[str],
-    resolution: tuple[float, float] | float | None,
-    degrees: bool,
-    hillshade_altitude: float,
-    hillshade_azimuth: float,
-    hillshade_z_factor: float,
-    slope_method: str,
-    tri_method: str,
-    fill_method: str,
-    edge_method: str,
-    use_richdem: bool,
-    window_size: int
-) -> list[Raster]:
+    attribute: str,
+    resolution: tuple[float, float] | float | None = None,
+    degrees: bool = True,
+    hillshade_altitude: float = 45.0,
+    hillshade_azimuth: float = 315.0,
+    hillshade_z_factor: float = 1.0,
+    slope_method: str = "Horn",
+    tri_method: str = "Riley",
+    fill_method: str = "none",
+    edge_method: str = "none",
+    use_richdem: bool = False,
+    window_size: int = 3,
+) -> RasterType:
     ...
 
 
 def get_terrain_attribute(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     attribute: str | list[str],
     resolution: tuple[float, float] | float | None = None,
     degrees: bool = True,
     hillshade_altitude: float = 45.0,
     hillshade_azimuth: float = 315.0,
     hillshade_z_factor: float = 1.0,
     slope_method: str = "Horn",
     tri_method: str = "Riley",
     fill_method: str = "none",
     edge_method: str = "none",
     use_richdem: bool = False,
-    window_size: int = 3
-) -> np.ndarray | list[np.ndarray] | Raster | list[Raster]:
+    window_size: int = 3,
+) -> NDArrayf | list[NDArrayf] | RasterType | list[RasterType]:
     """
     Derive one or multiple terrain attributes from a DEM.
     The attributes are based on:
 
     - Slope, aspect, hillshade (first method) from Horn (1981), http://dx.doi.org/10.1109/PROC.1981.11918,
-    - Slope, aspect, hillshade (second method), and terrain curvatures from Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
+    - Slope, aspect, hillshade (second method), and terrain curvatures from Zevenbergen and Thorne (1987),
+        http://dx.doi.org/10.1002/esp.3290120107.
     - Topographic Position Index from Weiss (2001), http://www.jennessent.com/downloads/TPI-poster-TNC_18x22.pdf.
-    - Terrain Ruggedness Index (topography) from Riley et al. (1999), http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf.
+    - Terrain Ruggedness Index (topography) from Riley et al. (1999),
+        http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf.
     - Terrain Ruggedness Index (bathymetry) from Wilson et al. (2007), http://dx.doi.org/10.1080/01490410701295962.
     - Roughness from Dartnell (2000), http://dx.doi.org/10.14358/PERS.70.9.1081.
     - Rugosity from Jenness (2004), https://doi.org/10.2193/0091-7648(2004)032[0829:CLSAFD]2.0.CO;2.
     - Fractal roughness from Taud et Parrot (2005), https://doi.org/10.4000/geomorphologie.622.
 
     Aspect and hillshade are derived using the slope, and thus depend on the same method.
     More details on the equations in the functions get_quadric_coefficients() and get_windowed_indexes().
@@ -697,16 +725,19 @@
     * 'aspect': The slope aspect in degrees or radians (degs: 0=N, 90=E, 180=S, 270=W).
     * 'hillshade': The shaded slope in relation to its aspect.
     * 'curvature': The second derivative of elevation (the rate of slope change per pixel), multiplied by 100.
     * 'planform_curvature': The curvature perpendicular to the direction of the slope, multiplied by 100.
     * 'profile_curvature': The curvature parallel to the direction of the slope, multiplied by 100.
     * 'maximum_curvature': The maximum curvature.
     * 'surface_fit': A quadric surface fit for each individual pixel.
-    * 'topographic_position_index': The topographic position index defined by a difference to the average of neighbouring pixels.
-    * 'terrain_ruggedness_index': The terrain ruggedness index. For topography, defined by the squareroot of squared differences to neighbouring pixels. For bathymetry, defined by the mean absolute difference to neighbouring pixels. Default method: "Riley" (topography).
+    * 'topographic_position_index': The topographic position index defined by a difference to the average of
+        neighbouring pixels.
+    * 'terrain_ruggedness_index': The terrain ruggedness index. For topography, defined by the squareroot of squared
+        differences to neighbouring pixels. For bathymetry, defined by the mean absolute difference to neighbouring
+        pixels. Default method: "Riley" (topography).
     * 'roughness': The roughness, i.e. maximum difference between neighbouring pixels.
     * 'rugosity': The rugosity, i.e. difference between real and planimetric surface area.
     * 'fractal_roughness': The roughness based on a volume box-counting estimate of the fractal dimension.
 
     :param dem: The DEM to analyze.
     :param attribute: The terrain attribute(s) to calculate.
     :param resolution: The X/Y or (X, Y) resolution of the DEM.
@@ -746,46 +777,63 @@
             resolution = dem.res
 
     # Validate and format the inputs
     if isinstance(attribute, str):
         attribute = [attribute]
 
     # These require the get_quadric_coefficients() function, which require the same X/Y resolution.
-    list_requiring_surface_fit = ["curvature", "planform_curvature", "profile_curvature", "maximum_curvature",
-                                  "slope", "hillshade", "aspect", "surface_fit", "rugosity"]
+    list_requiring_surface_fit = [
+        "curvature",
+        "planform_curvature",
+        "profile_curvature",
+        "maximum_curvature",
+        "slope",
+        "hillshade",
+        "aspect",
+        "surface_fit",
+        "rugosity",
+    ]
     attributes_requiring_surface_fit = [attr for attr in attribute if attr in list_requiring_surface_fit]
 
     if use_richdem:
 
         if not _has_rd:
             raise ValueError("Optional dependency needed. Install 'richdem'")
 
-        if ("slope" in attribute or "aspect" in attribute) and slope_method == 'ZevenbergThorne':
+        if ("slope" in attribute or "aspect" in attribute) and slope_method == "ZevenbergThorne":
             raise ValueError("RichDEM can only compute the slope and aspect using the default method of Horn (1981)")
 
-        list_requiring_richdem = ["slope", "aspect", "hillshade", "curvature", "planform_curvature",
-                                  "profile curvature", "maximum_curvature"]
+        list_requiring_richdem = [
+            "slope",
+            "aspect",
+            "hillshade",
+            "curvature",
+            "planform_curvature",
+            "profile curvature",
+            "maximum_curvature",
+        ]
         attributes_using_richdem = [attr for attr in attribute if attr in list_requiring_richdem]
         for attr in attributes_using_richdem:
             attributes_requiring_surface_fit.remove(attr)
 
-        if isinstance(dem, gu.Raster):
-            # Prepare rasterio.Dataset to pass to RichDEM
-            ds = dem.ds
-        else:
+        if not isinstance(dem, gu.Raster):
             # Here, maybe we could pass the geotransform based on the resolution, and add a "default" projection as
             # this is mandated but likely not used by the rdarray format of RichDEM...
             # For now, not supported
             raise ValueError("To derive RichDEM attributes, the DEM passed must be a Raster object")
 
-    list_requiring_windowed_index = ["terrain_ruggedness_index", "topographic_position_index", "roughness",
-                                     "fractal_roughness"]
+    list_requiring_windowed_index = [
+        "terrain_ruggedness_index",
+        "topographic_position_index",
+        "roughness",
+        "fractal_roughness",
+    ]
     attributes_requiring_windowed_index = [attr for attr in attribute if attr in list_requiring_windowed_index]
 
-    if resolution is None and len(attributes_requiring_surface_fit)>1:
+    if resolution is None and len(attributes_requiring_surface_fit) > 1:
         raise ValueError(f"'resolution' must be provided as an argument for attributes: {list_requiring_surface_fit}")
 
     choices = list_requiring_surface_fit + list_requiring_windowed_index
     for attr in attribute:
         if attr not in choices:
             raise ValueError(f"Attribute '{attr}' is not supported. Choices: {choices}")
 
@@ -794,102 +842,112 @@
         raise ValueError(f"Slope method '{slope_method}' is not supported. Must be one of: {list_slope_methods}")
     list_tri_methods = ["Riley", "Wilson"]
     if tri_method.lower() not in [tm.lower() for tm in list_tri_methods]:
         raise ValueError(f"TRI method '{tri_method}' is not supported. Must be one of: {list_tri_methods}")
     if (hillshade_azimuth < 0.0) or (hillshade_azimuth > 360.0):
         raise ValueError(f"Azimuth must be a value between 0 and 360 degrees (given value: {hillshade_azimuth})")
     if (hillshade_altitude < 0.0) or (hillshade_altitude > 90):
-        raise ValueError("Altitude must be a value between 0 and 90 degress (given value: {altitude})")
+        raise ValueError("Altitude must be a value between 0 and 90 degrees (given value: {altitude})")
     if (hillshade_z_factor < 0.0) or not np.isfinite(hillshade_z_factor):
         raise ValueError(f"z_factor must be a non-negative finite value (given value: {hillshade_z_factor})")
 
     # Initialize the terrain_attributes dictionary, which will be filled with the requested values.
-    terrain_attributes: dict[str, np.ndarray] = {}
+    terrain_attributes: dict[str, NDArrayf] = {}
 
     # Check which products should be made to optimize the processing
     make_aspect = any(attr in attribute for attr in ["aspect", "hillshade"])
     make_slope = any(
-        attr in attribute for attr in ["slope", "hillshade", "planform_curvature", "aspect", "profile_curvature",
-                                       "maximum_curvature"]
+        attr in attribute
+        for attr in ["slope", "hillshade", "planform_curvature", "aspect", "profile_curvature", "maximum_curvature"]
     )
     make_hillshade = "hillshade" in attribute
     make_surface_fit = len(attributes_requiring_surface_fit) > 0
     make_curvature = "curvature" in attribute
     make_planform_curvature = "planform_curvature" in attribute or "maximum_curvature" in attribute
-    make_profile_curvature = "profile_curvature" in attribute or  "maximum_curvature" in attribute
+    make_profile_curvature = "profile_curvature" in attribute or "maximum_curvature" in attribute
     make_maximum_curvature = "maximum_curvature" in attribute
     make_windowed_index = len(attributes_requiring_windowed_index) > 0
     make_topographic_position = "topographic_position_index" in attribute
     make_terrain_ruggedness = "terrain_ruggedness_index" in attribute
     make_roughness = "roughness" in attribute
     make_rugosity = "rugosity" in attribute
     make_fractal_roughness = "fractal_roughness" in attribute
 
     # Get array of DEM
-    dem_arr = gu.spatial_tools.get_array_and_mask(dem)[0]
+    dem_arr = gu.raster.get_array_and_mask(dem)[0]
 
     if make_surface_fit:
         if not isinstance(resolution, Sized):
-            resolution = (float(resolution), float(resolution))
+            resolution = (float(resolution), float(resolution))  # type: ignore
         if resolution[0] != resolution[1]:
             raise ValueError(
                 f"Quadric surface fit requires the same X and Y resolution ({resolution} was given). "
                 f"This was required by: {attributes_requiring_surface_fit}"
             )
         terrain_attributes["surface_fit"] = get_quadric_coefficients(
-            dem=dem_arr, resolution=resolution[0], fill_method=fill_method, edge_method=edge_method,
-            make_rugosity=make_rugosity)
+            dem=dem_arr,
+            resolution=resolution[0],
+            fill_method=fill_method,
+            edge_method=edge_method,
+            make_rugosity=make_rugosity,
+        )
 
     if make_slope:
 
         if use_richdem:
-            terrain_attributes["slope"] = _get_terrainattr_richdem(ds, attribute="slope_radians")
+            terrain_attributes["slope"] = _get_terrainattr_richdem(dem, attribute="slope_radians")
 
         else:
             if slope_method == "Horn":
-                # This calculation is based on page 18 (bottom left) and 20-21 of Horn (1981), http://dx.doi.org/10.1109/PROC.1981.11918.
+                # This calculation is based on page 18 (bottom left) and 20-21 of Horn (1981),
+                # http://dx.doi.org/10.1109/PROC.1981.11918.
                 terrain_attributes["slope"] = np.arctan(
-                    (terrain_attributes["surface_fit"][9, :, :] ** 2 + terrain_attributes["surface_fit"][10, :, :] ** 2) ** 0.5
+                    (terrain_attributes["surface_fit"][9, :, :] ** 2 + terrain_attributes["surface_fit"][10, :, :] ** 2)
+                    ** 0.5
                 )
 
             elif slope_method == "ZevenbergThorne":
-                # This calculation is based on Equation 13 of Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
+                # This calculation is based on Equation 13 of Zevenbergen and Thorne (1987),
+                # http://dx.doi.org/10.1002/esp.3290120107.
                 # SLOPE = ARCTAN((G²+H²)**(1/2))
                 terrain_attributes["slope"] = np.arctan(
-                    (terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2) ** 0.5
+                    (terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2)
+                    ** 0.5
                 )
 
-
     if make_aspect:
 
         if use_richdem:
             # The aspect of RichDEM is returned in degrees, we convert to radians to match the others
-            terrain_attributes["aspect"] = np.deg2rad(_get_terrainattr_richdem(ds, attribute="aspect"))
+            terrain_attributes["aspect"] = np.deg2rad(_get_terrainattr_richdem(dem, attribute="aspect"))
             # For flat slopes, RichDEM returns a 90° aspect by default, while GDAL return a 180° aspect
             # We stay consistent with GDAL
-            slope_tmp = _get_terrainattr_richdem(ds, attribute="slope_radians")
+            slope_tmp = _get_terrainattr_richdem(dem, attribute="slope_radians")
             terrain_attributes["aspect"][slope_tmp == 0] = np.pi
 
         else:
             # ASPECT = ARCTAN(-H/-G)  # This did not work
             # ASPECT = (ARCTAN2(-G, H) + 0.5PI) % 2PI  did work.
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", "invalid value encountered in remainder")
                 if slope_method == "Horn":
                     # This uses the estimates from Horn (1981).
-                    terrain_attributes["aspect"] = (-
-                                                           np.arctan2(-terrain_attributes["surface_fit"][9, :, :],
-                                                                      terrain_attributes["surface_fit"][10, :, :])
-                                                           -  np.pi
-                                                   ) % (2 * np.pi)
+                    terrain_attributes["aspect"] = (
+                        -np.arctan2(
+                            -terrain_attributes["surface_fit"][9, :, :], terrain_attributes["surface_fit"][10, :, :]
+                        )
+                        - np.pi
+                    ) % (2 * np.pi)
 
                 elif slope_method == "ZevenbergThorne":
                     # This uses the slope estimate from Zevenbergen and Thorne (1987).
                     terrain_attributes["aspect"] = (
-                        np.arctan2(-terrain_attributes["surface_fit"][6, :, :], terrain_attributes["surface_fit"][7, :, :])
+                        np.arctan2(
+                            -terrain_attributes["surface_fit"][6, :, :], terrain_attributes["surface_fit"][7, :, :]
+                        )
                         + np.pi / 2
                     ) % (2 * np.pi)
 
     if make_hillshade:
         # If a different z-factor was given, slopemap with exaggerated gradients.
         if hillshade_z_factor != 1.0:
             slopemap = np.arctan(np.tan(terrain_attributes["slope"]) * hillshade_z_factor)
@@ -898,97 +956,110 @@
 
         azimuth_rad = np.deg2rad(360 - hillshade_azimuth)
         altitude_rad = np.deg2rad(hillshade_altitude)
 
         # The operation below yielded the closest hillshade to GDAL (multiplying by 255 did not work)
         # As 0 is generally no data for this uint8, we add 1 and then 0.5 for the rounding to occur between 1 and 255
         terrain_attributes["hillshade"] = np.clip(
-            1.5 + 254
+            1.5
+            + 254
             * (
                 np.sin(altitude_rad) * np.cos(slopemap)
                 + np.cos(altitude_rad) * np.sin(slopemap) * np.sin(azimuth_rad - terrain_attributes["aspect"])
             ),
             0,
             255,
         ).astype("float32")
 
     if make_curvature:
 
         if use_richdem:
-            terrain_attributes["curvature"] = _get_terrainattr_richdem(ds, attribute="curvature")
+            terrain_attributes["curvature"] = _get_terrainattr_richdem(dem, attribute="curvature")
 
         else:
             # Curvature is the second derivative of the surface fit equation.
             # (URL in get_quadric_coefficients() docstring)
             # Curvature = -2(D + E) * 100
             terrain_attributes["curvature"] = (
                 -2 * (terrain_attributes["surface_fit"][3, :, :] + terrain_attributes["surface_fit"][4, :, :]) * 100
             )
 
     if make_planform_curvature:
 
         if use_richdem:
-            terrain_attributes["planform_curvature"] = _get_terrainattr_richdem(ds, attribute="planform_curvature")
+            terrain_attributes["planform_curvature"] = _get_terrainattr_richdem(dem, attribute="planform_curvature")
 
         else:
             # PLANC = 2(DH² + EG² -FGH)/(G²+H²)
             with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", "invalid value encountered in true_divide")
+                warnings.filterwarnings("ignore", "invalid value encountered in *divide")
                 terrain_attributes["planform_curvature"] = (
-                    - 2
+                    -2
                     * (
                         terrain_attributes["surface_fit"][3, :, :] * terrain_attributes["surface_fit"][7, :, :] ** 2
                         + terrain_attributes["surface_fit"][4, :, :] * terrain_attributes["surface_fit"][6, :, :] ** 2
                         - terrain_attributes["surface_fit"][5, :, :]
                         * terrain_attributes["surface_fit"][6, :, :]
                         * terrain_attributes["surface_fit"][7, :, :]
                     )
-                    / (terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2)
+                    / (
+                        terrain_attributes["surface_fit"][6, :, :] ** 2
+                        + terrain_attributes["surface_fit"][7, :, :] ** 2
+                    )
                     * 100
                 )
 
             # Completely flat surfaces trigger the warning above. These need to be set to zero
-            terrain_attributes["planform_curvature"][terrain_attributes["surface_fit"][6, :, :] ** 2 +
-                                                     terrain_attributes["surface_fit"][7, :, :] ** 2 == 0.0] = 0.0
+            terrain_attributes["planform_curvature"][
+                terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2 == 0.0
+            ] = 0.0
 
     if make_profile_curvature:
 
         if use_richdem:
-            terrain_attributes["profile_curvature"] = _get_terrainattr_richdem(ds, attribute="profile_curvature")
+            terrain_attributes["profile_curvature"] = _get_terrainattr_richdem(dem, attribute="profile_curvature")
 
         else:
             # PROFC = -2(DG² + EH² + FGH)/(G²+H²)
             with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", "invalid value encountered in true_divide")
+                warnings.filterwarnings("ignore", "invalid value encountered in *divide")
                 terrain_attributes["profile_curvature"] = (
                     2
                     * (
                         terrain_attributes["surface_fit"][3, :, :] * terrain_attributes["surface_fit"][6, :, :] ** 2
                         + terrain_attributes["surface_fit"][4, :, :] * terrain_attributes["surface_fit"][7, :, :] ** 2
                         + terrain_attributes["surface_fit"][5, :, :]
                         * terrain_attributes["surface_fit"][6, :, :]
                         * terrain_attributes["surface_fit"][7, :, :]
                     )
-                    / (terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2)
+                    / (
+                        terrain_attributes["surface_fit"][6, :, :] ** 2
+                        + terrain_attributes["surface_fit"][7, :, :] ** 2
+                    )
                     * 100
                 )
 
             # Completely flat surfaces trigger the warning above. These need to be set to zero
-            terrain_attributes["profile_curvature"][terrain_attributes["surface_fit"][6, :, :] ** 2 +
-                                                     terrain_attributes["surface_fit"][7, :, :] ** 2 == 0.0] = 0.0
+            terrain_attributes["profile_curvature"][
+                terrain_attributes["surface_fit"][6, :, :] ** 2 + terrain_attributes["surface_fit"][7, :, :] ** 2 == 0.0
+            ] = 0.0
 
     if make_maximum_curvature:
         minc = np.minimum(terrain_attributes["profile_curvature"], terrain_attributes["planform_curvature"])
         maxc = np.maximum(terrain_attributes["profile_curvature"], terrain_attributes["planform_curvature"])
-        terrain_attributes["maximum_curvature"] = np.where(np.abs(minc)>maxc, minc, maxc)
+        terrain_attributes["maximum_curvature"] = np.where(np.abs(minc) > maxc, minc, maxc)
 
     if make_windowed_index:
-        terrain_attributes["windowed_indexes"] = \
-            get_windowed_indexes(dem=dem_arr, fill_method=fill_method, edge_method=edge_method,
-                                 window_size=window_size, make_fractal_roughness=make_fractal_roughness)
+        terrain_attributes["windowed_indexes"] = get_windowed_indexes(
+            dem=dem_arr,
+            fill_method=fill_method,
+            edge_method=edge_method,
+            window_size=window_size,
+            make_fractal_roughness=make_fractal_roughness,
+        )
 
     if make_topographic_position:
         terrain_attributes["topographic_position_index"] = terrain_attributes["windowed_indexes"][2, :, :]
 
     if make_terrain_ruggedness:
 
         if tri_method == "Riley":
@@ -1012,43 +1083,51 @@
             if attr not in terrain_attributes:
                 continue
             terrain_attributes[attr] = np.rad2deg(terrain_attributes[attr])
 
     output_attributes = [terrain_attributes[key].reshape(dem.shape) for key in attribute]
 
     if isinstance(dem, gu.Raster):
-        output_attributes = [gu.Raster.from_array(attr, transform=dem.transform, crs=dem.crs, nodata=None) for attr in output_attributes]
+        output_attributes = [
+            gu.Raster.from_array(attr, transform=dem.transform, crs=dem.crs, nodata=-99999)
+            for attr in output_attributes
+        ]
 
     return output_attributes if len(output_attributes) > 1 else output_attributes[0]
 
+
 @overload
 def slope(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-    method: str,
-    degrees: bool,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    method: str = "Horn",
+    degrees: bool = True,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def slope(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-    method: str,
-    degrees: bool,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    method: str = "Horn",
+    degrees: bool = True,
+    use_richdem: bool = False,
+) -> Raster:
+    ...
+
 
 def slope(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     resolution: float | tuple[float, float] | None = None,
     method: str = "Horn",
     degrees: bool = True,
-    use_richdem: bool = False
-) -> np.ndarray | Raster:
+    use_richdem: bool = False,
+) -> NDArrayf | Raster:
     """
     Generate a slope map for a DEM, returned in degrees by default.
 
     Based on Horn (1981), http://dx.doi.org/10.1109/PROC.1981.11918 and on Zevenbergen and Thorne (1987),
     http://dx.doi.org/10.1002/esp.3290120107.
 
     :param dem: The DEM to generate a slope map for.
@@ -1061,43 +1140,50 @@
         >>> dem = np.repeat(np.arange(3), 3).reshape(3, 3)
         >>> dem
         array([[0, 0, 0],
                [1, 1, 1],
                [2, 2, 2]])
         >>> slope(dem, resolution=1, degrees=True)[1, 1] # Slope in degrees
         45.0
-        >>> np.tan(slope(dem, resolution=2, degrees=True)[1, 1] * np.pi / 180.) # Slope in percentage
+        >>> np.round(np.tan(slope(dem, resolution=2, degrees=True)[1, 1] * np.pi / 180.), 1) # Slope in percentage
         0.5
 
     :returns: A slope map of the same shape as 'dem' in degrees or radians.
     """
-    return get_terrain_attribute(dem, attribute="slope", slope_method=method, resolution=resolution, degrees=degrees,
-                                 use_richdem=use_richdem)
+    return get_terrain_attribute(
+        dem, attribute="slope", slope_method=method, resolution=resolution, degrees=degrees, use_richdem=use_richdem
+    )
+
 
 @overload
 def aspect(
-    dem: np.ndarray | np.ma.masked_array,
-    method: str,
-    degrees: bool,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: NDArrayf | MArrayf,
+    method: str = "Horn",
+    degrees: bool = True,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def aspect(
     dem: RasterType,
-    method: str,
-    degrees: bool,
-    use_richdem: bool,
-) -> Raster: ...
-
-def aspect(dem: np.ndarray | np.ma.masked_array | RasterType,
-           method: str = "Horn",
-           degrees: bool = True,
-           use_richdem: bool = False,
-           ) -> np.ndarray | Raster:
+    method: str = "Horn",
+    degrees: bool = True,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
+
+def aspect(
+    dem: NDArrayf | MArrayf | RasterType,
+    method: str = "Horn",
+    degrees: bool = True,
+    use_richdem: bool = False,
+) -> NDArrayf | Raster:
     """
     Calculate the aspect of each cell in a DEM, returned in degrees by default. The aspect of flat slopes is 180° by
     default (as in GDAL).
 
     Based on Horn (1981), http://dx.doi.org/10.1109/PROC.1981.11918 and on Zevenbergen and Thorne (1987),
     http://dx.doi.org/10.1002/esp.3290120107.
 
@@ -1120,48 +1206,54 @@
         array([[0, 1, 2],
                [0, 1, 2],
                [0, 1, 2]])
         >>> aspect(dem.T, degrees=True)[1, 1]
         270.0
 
     """
-    return get_terrain_attribute(dem, attribute="aspect", slope_method=method, resolution=1.0, degrees=degrees,
-                                 use_richdem=use_richdem)
+    return get_terrain_attribute(
+        dem, attribute="aspect", slope_method=method, resolution=1.0, degrees=degrees, use_richdem=use_richdem
+    )
+
 
 @overload
 def hillshade(
-    dem: RasterType,
-    resolution: float | tuple[float, float],
-    method: str,
-    azimuth: float,
-    altitude: float,
-    z_factor: float,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    method: str = "Horn",
+    azimuth: float = 315.0,
+    altitude: float = 45.0,
+    z_factor: float = 1.0,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def hillshade(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float],
-    method: str,
-    azimuth: float,
-    altitude: float,
-    z_factor: float,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    method: str = "Horn",
+    azimuth: float = 315.0,
+    altitude: float = 45.0,
+    z_factor: float = 1.0,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
 
 def hillshade(
-    dem: np.ndarray | np.ma.masked_array,
+    dem: NDArrayf | MArrayf,
     resolution: float | tuple[float, float] | None = None,
     method: str = "Horn",
     azimuth: float = 315.0,
     altitude: float = 45.0,
     z_factor: float = 1.0,
     use_richdem: bool = False,
-) -> np.ndarray | Raster:
+) -> NDArrayf | RasterType:
     """
     Generate a hillshade from the given DEM. The value 0 is used for nodata, and 1 to 255 for hillshading.
 
     Based on Horn (1981), http://dx.doi.org/10.1109/PROC.1981.11918.
 
     :param dem: The input DEM to calculate the hillshade from.
     :param resolution: One or two values specifying the resolution of the DEM.
@@ -1181,36 +1273,41 @@
         dem,
         attribute="hillshade",
         resolution=resolution,
         slope_method=method,
         hillshade_azimuth=azimuth,
         hillshade_altitude=altitude,
         hillshade_z_factor=z_factor,
-        use_richdem=use_richdem
+        use_richdem=use_richdem,
     )
 
+
 @overload
 def curvature(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def curvature(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
 
 def curvature(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     resolution: float | tuple[float, float] | None = None,
     use_richdem: bool = False,
-) -> np.ndarray | Raster:
+) -> NDArrayf | RasterType:
     """
     Calculate the terrain curvature (second derivative of elevation) in m-1 multiplied by 100.
 
     Based on Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
 
     Information:
        * Curvature is positive on convex surfaces and negative on concave surfaces.
@@ -1236,31 +1333,35 @@
     :returns: The curvature array of the DEM.
     """
     return get_terrain_attribute(dem=dem, attribute="curvature", resolution=resolution, use_richdem=use_richdem)
 
 
 @overload
 def planform_curvature(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def planform_curvature(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
 
 def planform_curvature(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     resolution: float | tuple[float, float] | None = None,
     use_richdem: bool = False,
-) -> np.ndarray | Raster:
+) -> NDArrayf | RasterType:
     """
     Calculate the terrain curvature perpendicular to the direction of the slope in m-1 multiplied by 100.
 
     Based on Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
 
     :param dem: The DEM to calculate the curvature from.
     :param resolution: The X/Y resolution of the DEM.
@@ -1278,36 +1379,42 @@
         ...                 [1, 2, 4],
         ...                 [1, 4, 8]], dtype="float32")
         >>> planform_curvature(dem, resolution=1.0)[1, 1] / 100.
         -4.0
 
     :returns: The planform curvature array of the DEM.
     """
-    return get_terrain_attribute(dem=dem, attribute="planform_curvature", resolution=resolution, use_richdem=use_richdem)
+    return get_terrain_attribute(
+        dem=dem, attribute="planform_curvature", resolution=resolution, use_richdem=use_richdem
+    )
 
 
 @overload
 def profile_curvature(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def profile_curvature(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
 
 def profile_curvature(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     resolution: float | tuple[float, float] | None = None,
     use_richdem: bool = False,
-) -> np.ndarray | Raster:
+) -> NDArrayf | RasterType:
     """
     Calculate the terrain curvature parallel to the direction of the slope in m-1 multiplied by 100.
 
     Based on Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
 
     :param dem: The DEM to calculate the curvature from.
     :param resolution: The X/Y resolution of the DEM.
@@ -1330,31 +1437,35 @@
     :returns: The profile curvature array of the DEM.
     """
     return get_terrain_attribute(dem=dem, attribute="profile_curvature", resolution=resolution, use_richdem=use_richdem)
 
 
 @overload
 def maximum_curvature(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> NDArrayf:
+    ...
+
 
 @overload
 def maximum_curvature(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-    use_richdem: bool,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+    use_richdem: bool = False,
+) -> RasterType:
+    ...
+
 
 def maximum_curvature(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
+    dem: NDArrayf | MArrayf | RasterType,
     resolution: float | tuple[float, float] | None = None,
     use_richdem: bool = False,
-) -> np.ndarray | Raster:
+) -> NDArrayf | RasterType:
     """
     Calculate the signed maximum profile or planform curvature parallel to the direction of the slope in m-1
     multiplied by 100.
 
     Based on Zevenbergen and Thorne (1987), http://dx.doi.org/10.1002/esp.3290120107.
 
     :param dem: The DEM to calculate the curvature from.
@@ -1363,32 +1474,26 @@
 
     :raises ValueError: If the inputs are poorly formatted.
 
     :returns: The profile curvature array of the DEM.
     """
     return get_terrain_attribute(dem=dem, attribute="maximum_curvature", resolution=resolution, use_richdem=use_richdem)
 
+
 @overload
-def topographic_position_index(
-    dem: RasterType,
-    window_size: int,
-) -> Raster: ...
+def topographic_position_index(dem: NDArrayf | MArrayf, window_size: int = 3) -> NDArrayf:
+    ...
 
 
 @overload
-def topographic_position_index(
-    dem: np.ndarray | np.ma.masked_array,
-    window_size: int,
-) -> np.ndarray: ...
+def topographic_position_index(dem: RasterType, window_size: int = 3) -> RasterType:
+    ...
 
 
-def topographic_position_index(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
-    window_size: int = 3
-) -> np.ndarray | Raster:
+def topographic_position_index(dem: NDArrayf | MArrayf | RasterType, window_size: int = 3) -> NDArrayf | RasterType:
     """
     Calculates the Topographic Position Index, the difference to the average of neighbouring pixels. Output is in the
     unit of the DEM (typically meters).
 
     Based on: Weiss (2001), http://www.jennessent.com/downloads/TPI-poster-TNC_18x22.pdf.
 
     :param dem: The DEM to calculate the topographic position index from.
@@ -1410,40 +1515,36 @@
 
     :returns: The topographic position index array of the DEM (unit of the DEM).
     """
     return get_terrain_attribute(dem=dem, attribute="topographic_position_index", window_size=window_size)
 
 
 @overload
-def terrain_ruggedness_index(
-    dem: RasterType,
-    method: str,
-    window_size: int
-) -> Raster: ...
+def terrain_ruggedness_index(dem: NDArrayf | MArrayf, method: str = "Riley", window_size: int = 3) -> NDArrayf:
+    ...
+
 
 @overload
-def terrain_ruggedness_index(
-    dem: np.ndarray | np.ma.masked_array,
-    method: str,
-    window_size: int
-) -> np.ndarray: ...
+def terrain_ruggedness_index(dem: RasterType, method: str = "Riley", window_size: int = 3) -> RasterType:
+    ...
+
 
 def terrain_ruggedness_index(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
-    method: str = "Riley",
-    window_size: int = 3
-) -> np.ndarray | Raster:
+    dem: NDArrayf | MArrayf | RasterType, method: str = "Riley", window_size: int = 3
+) -> NDArrayf | RasterType:
     """
     Calculates the Terrain Ruggedness Index, the cumulated differences to neighbouring pixels. Output is in the
     unit of the DEM (typically meters).
 
     Based either on:
 
-    * Riley et al. (1999), http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf that derives the squareroot of squared differences to neighbouring pixels, preferred for topography.
-    * Wilson et al. (2007), http://dx.doi.org/10.1080/01490410701295962 that derives the mean absolute difference to neighbouring pixels, preferred for bathymetry.
+    * Riley et al. (1999), http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf that derives
+        the squareroot of squared differences to neighbouring pixels, preferred for topography.
+    * Wilson et al. (2007), http://dx.doi.org/10.1080/01490410701295962 that derives the mean absolute difference to
+        neighbouring pixels, preferred for bathymetry.
 
     :param dem: The DEM to calculate the terrain ruggedness index from.
     :param method: The algorithm used ("Riley" for topography or "Wilson" for bathymetry).
     :param window_size: The size of the window for deriving the metric.
 
     :raises ValueError: If the inputs are poorly formatted.
 
@@ -1457,35 +1558,30 @@
         ...                 [1, 1, 1],
         ...                 [1, 1, 1]], dtype="float32")
         >>> terrain_ruggedness_index(dem)[1, 1]
         0.0
 
     :returns: The terrain ruggedness index array of the DEM (unit of the DEM).
     """
-    return get_terrain_attribute(dem=dem, attribute="terrain_ruggedness_index", tri_method=method, window_size=window_size)
+    return get_terrain_attribute(
+        dem=dem, attribute="terrain_ruggedness_index", tri_method=method, window_size=window_size
+    )
 
 
 @overload
-def roughness(
-    dem: RasterType,
-    window_size: int
-) -> Raster: ...
+def roughness(dem: NDArrayf | MArrayf, window_size: int = 3) -> NDArrayf:
+    ...
 
 
 @overload
-def roughness(
-    dem: np.ndarray | np.ma.masked_array,
-    window_size: int
-) -> np.ndarray: ...
+def roughness(dem: RasterType, window_size: int = 3) -> RasterType:
+    ...
 
 
-def roughness(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
-    window_size: int = 3
-) -> np.ndarray | Raster:
+def roughness(dem: NDArrayf | MArrayf | RasterType, window_size: int = 3) -> NDArrayf | RasterType:
     """
     Calculates the roughness, the maximum difference between neighbouring pixels, for any window size. Output is in the
     unit of the DEM (typically meters).
 
     Based on: Dartnell (2000), http://dx.doi.org/10.14358/PERS.70.9.1081.
 
     :param dem: The DEM to calculate the roughness from.
@@ -1508,30 +1604,31 @@
     :returns: The roughness array of the DEM (unit of the DEM).
     """
     return get_terrain_attribute(dem=dem, attribute="roughness", window_size=window_size)
 
 
 @overload
 def rugosity(
-    dem: RasterType,
-    resolution: float | tuple[float, float] | None,
-) -> Raster: ...
+    dem: NDArrayf | MArrayf,
+    resolution: float | tuple[float, float] | None = None,
+) -> NDArrayf:
+    ...
 
 
 @overload
 def rugosity(
-    dem: np.ndarray | np.ma.masked_array,
-    resolution: float | tuple[float, float] | None,
-) -> np.ndarray: ...
+    dem: RasterType,
+    resolution: float | tuple[float, float] | None = None,
+) -> RasterType:
+    ...
 
 
 def rugosity(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
-    resolution: float | tuple[float, float] | None = None
-) -> np.ndarray | Raster:
+    dem: NDArrayf | MArrayf | RasterType, resolution: float | tuple[float, float] | None = None
+) -> NDArrayf | RasterType:
     """
     Calculates the rugosity, the ratio between real area and planimetric area. Only available for a 3x3 window. The
     output is unitless.
 
     Based on: Jenness (2004), https://doi.org/10.2193/0091-7648(2004)032[0829:CLSAFD]2.0.CO;2.
 
     :param dem: The DEM to calculate the rugosity from.
@@ -1553,31 +1650,24 @@
 
     :returns: The rugosity array of the DEM (unitless).
     """
     return get_terrain_attribute(dem=dem, attribute="rugosity", resolution=resolution)
 
 
 @overload
-def fractal_roughness(
-    dem: RasterType,
-    window_size: int
-) -> Raster: ...
+def fractal_roughness(dem: NDArrayf | MArrayf, window_size: int = 13) -> NDArrayf:
+    ...
 
 
 @overload
-def fractal_roughness(
-    dem: np.ndarray | np.ma.masked_array,
-    window_size: int
-) -> np.ndarray: ...
+def fractal_roughness(dem: RasterType, window_size: int = 13) -> RasterType:
+    ...
 
 
-def fractal_roughness(
-    dem: np.ndarray | np.ma.masked_array | RasterType,
-    window_size: int = 13
-) -> np.ndarray | Raster:
+def fractal_roughness(dem: NDArrayf | MArrayf | RasterType, window_size: int = 13) -> NDArrayf | RasterType:
     """
     Calculates the fractal roughness, the local 3D fractal dimension. Can only be computed on window sizes larger or
     equal to 5x5, defaults to 13x13. Output unit is a fractal dimension between 1 and 3.
 
     Based on: Taud et Parrot (2005), https://doi.org/10.4000/geomorphologie.622.
 
     :param dem: The DEM to calculate the roughness from.
```

### Comparing `xdem-0.0.7/xdem/volume.py` & `xdem-0.0.8/xdem/volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Volume change calculation tools (aimed for glaciers)."""
 from __future__ import annotations
 
 import warnings
-from typing import Callable, Optional, Union
+from typing import Any, Callable
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import rasterio.fill
 import scipy.interpolate
+from geoutils.raster import RasterType, get_array_and_mask, get_mask, get_valid_extent
 from tqdm import tqdm
 
 import xdem
-from geoutils import spatial_tools
+from xdem._typing import MArrayf, NDArrayf
 
 
-def hypsometric_binning(ddem: np.ndarray, ref_dem: np.ndarray, bins: Union[float, np.ndarray] = 50.0,
-                        kind: str = "fixed", aggregation_function: Callable = np.median) -> pd.DataFrame:
+def hypsometric_binning(
+    ddem: NDArrayf,
+    ref_dem: NDArrayf,
+    bins: float | np.ndarray[Any, np.dtype[np.floating[Any] | np.integer[Any]]] = 50.0,
+    kind: str = "fixed",
+    aggregation_function: Callable[[NDArrayf], float] = np.median,
+) -> pd.DataFrame:
     """
     Separate the dDEM in discrete elevation bins.
     The elevation bins will be calculated based on all ref_dem valid pixels.
     ddem may contain NaN/masked values over the same area, they will be excluded before the aggregation.
 
     It is assumed that the dDEM is calculated as 'ref_dem - dem' (not 'dem - ref_dem').
 
@@ -32,36 +38,33 @@
     :param aggregation_function: The function to aggregate the elevation values within a bin. Defaults to the median.
 
     :returns: A Pandas DataFrame with elevation bins and dDEM statistics.
     """
     assert ddem.shape == ref_dem.shape
 
     # Convert ddem mask into NaN
-    ddem, _ = spatial_tools.get_array_and_mask(ddem)
+    ddem, _ = get_array_and_mask(ddem)
 
     # Extract only the valid values, i.e. valid in ref_dem
-    valid_mask = ~spatial_tools.get_mask(ref_dem)
+    valid_mask = ~get_mask(ref_dem)
     ddem = np.array(ddem[valid_mask])
     ref_dem = np.array(ref_dem.squeeze()[valid_mask])
 
     if isinstance(bins, np.ndarray):
         zbins = bins
     elif kind == "fixed":
         zbins = np.arange(ref_dem.min(), ref_dem.max() + bins + 1e-6, step=bins)  # +1e-6 in case min=max (1 point)
     elif kind == "count":
         # Make bins between mean_dem.min() and a little bit above mean_dem.max().
         # The bin count has to be bins + 1 because zbins[0] will be a "below min value" bin, which will be irrelevant.
         zbins = np.linspace(ref_dem.min(), ref_dem.max() + 1e-6 / bins, num=int(bins + 1))
     elif kind == "quantile":
         # Make the percentile steps. The bins + 1 is explained above.
         steps = np.linspace(0, 100, num=int(bins) + 1)
-        zbins = np.fromiter(
-            (np.percentile(ref_dem, step) for step in steps),
-            dtype=float
-        )
+        zbins = np.fromiter((np.percentile(ref_dem, step) for step in steps), dtype=float)
         # The uppermost bin needs to be a tiny amount larger than the highest value to include it.
         zbins[-1] += 1e-6
     elif kind == "custom":
         zbins = bins  # type: ignore
     else:
         raise ValueError(f"Invalid bin kind: {kind}. Choices: ['fixed', 'count', 'quantile', 'custom']")
 
@@ -90,36 +93,38 @@
             # If custom bins were added, i may exceed the bin range, which will be silently ignored.
             if kind == "custom" and "out of bounds" in str(exception):
                 continue
             raise exception
 
     # Collect the results in a dataframe
     output = pd.DataFrame(
-        index=pd.IntervalIndex.from_breaks(zbins),
-        data=np.vstack([
-            values, counts
-        ]).T,
-        columns=["value", "count"]
+        index=pd.IntervalIndex.from_breaks(zbins), data=np.vstack([values, counts]).T, columns=["value", "count"]
     )
 
     return output
 
 
-def interpolate_hypsometric_bins(hypsometric_bins: pd.DataFrame, value_column="value", method="polynomial", order=3,
-                                 count_threshold: Optional[int] = None) -> pd.DataFrame:
+def interpolate_hypsometric_bins(
+    hypsometric_bins: pd.DataFrame,
+    value_column: str = "value",
+    method: str = "polynomial",
+    order: int = 3,
+    count_threshold: int | None = None,
+) -> pd.DataFrame:
     """
     Interpolate hypsometric bins using any valid Pandas interpolation technique.
 
     NOTE: It will not extrapolate!
 
     :param hypsometric_bins: Bins where nans will be interpolated.
     :param value_column: The name of the column in 'hypsometric_bins' to use as values.
     :param method: Any valid Pandas interpolation technique (e.g. 'linear', 'polynomial', 'ffill', 'bfill').
     :param order: The polynomial order to use. Only used if method='polynomial'.
-    :param count_threshold: Optional. A pixel count threshold to exclude during the curve fit (requires a 'count' column).
+    :param count_threshold: Optional. A pixel count threshold to exclude during the curve fit (requires a 'count'
+        column).
     :returns: Bins interpolated with the chosen interpolation method.
     """
     # Copy the bins that will be filled.
     bins = hypsometric_bins.copy()
     # Temporarily set the index to be the midpoint (for interpolation)
     bins.index = bins.index.mid
 
@@ -146,71 +151,76 @@
 
     # Return the index to intervals instead of the midpoint.
     bins.index = hypsometric_bins.index
 
     return bins
 
 
-def fit_hypsometric_bins_poly(hypsometric_bins: pd.DataFrame, value_column: str = "value", degree: int = 3,
-                              iterations: int = 1, count_threshold: Optional[int] = None) -> pd.Series:
+def fit_hypsometric_bins_poly(
+    hypsometric_bins: pd.DataFrame,
+    value_column: str = "value",
+    degree: int = 3,
+    iterations: int = 1,
+    count_threshold: int | None = None,
+) -> pd.Series:
     """
     Fit a polynomial to the hypsometric bins.
 
     :param hypsometric_bins: Bins where nans will be interpolated.
     :param value_column: The name of the column in 'hypsometric_bins' to use as values.
     :param degree: The degree of the polynomial to use.
     :param iterations: The number of iterations to run. \
  At each iteration, values with residuals larger than 3 times the residuals' standard deviation are excluded.
-    :param count_threshold: Optional. A pixel count threshold to exclude during the curve fit (requires a 'count' column).
+    :param count_threshold: Optional. A pixel count threshold to exclude during the curve fit (requires a 'count'
+        column).
     :returns: Bins replaced by the polynomial fit.
     """
     bins = hypsometric_bins.copy()
     bins.index = bins.index.mid
 
     if count_threshold is not None:
-        assert "count" in hypsometric_bins.columns, f"'count' not a column in the dataframe"
+        assert "count" in hypsometric_bins.columns, "'count' not a column in the dataframe"
         bins_under_threshold = bins["count"] < count_threshold
         bins.loc[bins_under_threshold, value_column] = np.nan
 
     # Remove invalid bins
     valids = np.isfinite(np.asarray(bins[value_column]))
 
-    for k in range(iterations):
+    for _k in range(iterations):
 
         # Fit polynomial
         x = bins.index[valids]
         y = bins[value_column][valids]
         pcoeff = np.polyfit(x, y, deg=degree)
 
         # Calculate residuals
         interpolated_values = np.polyval(pcoeff, bins.index)
         residuals = interpolated_values - bins[value_column]
         residuals_std = np.nanstd(residuals.values)
 
         # Filter outliers further than 3 std
         valids_old = np.copy(valids)
-        valids[np.abs(residuals.values) > 3*residuals_std] = False
+        valids[np.abs(residuals.values) > 3 * residuals_std] = False
         if np.array_equal(valids, valids_old):
             break
 
     # Save as pandas' DataFrame
     output = pd.DataFrame(
-        index=hypsometric_bins.index,
-        data=np.vstack([
-            interpolated_values, bins["count"]
-        ]).T,
-        columns=["value", "count"]
+        index=hypsometric_bins.index, data=np.vstack([interpolated_values, bins["count"]]).T, columns=["value", "count"]
     )
 
     return output
 
 
-def calculate_hypsometry_area(ddem_bins: Union[pd.Series, pd.DataFrame], ref_dem: np.ndarray,
-                              pixel_size: Union[float, tuple[float, float]],
-                              timeframe: str = "reference") -> pd.Series:
+def calculate_hypsometry_area(
+    ddem_bins: pd.Series | pd.DataFrame,
+    ref_dem: NDArrayf,
+    pixel_size: float | tuple[float, float],
+    timeframe: str = "reference",
+) -> pd.Series:
     """
     Calculate the associated representative area of the given dDEM bins.
 
     By default, the area bins will be representative of the mean timing between the reference and nonreference DEM:
     elevations = ref_dem - (h_vs_dh_funcion(ref_dem) / 2)
     This can be changed to either "reference":
     elevations = ref_dem
@@ -233,156 +243,161 @@
         ddem_bins = ddem_bins["value"]
 
     # For timeframe "mean" or "nonreference", check that ddem_bins values can be interpolated at any altitude
     if timeframe in ["mean", "nonreference"]:
         assert not np.any(np.isnan(ddem_bins.values)), "The dDEM bins cannot contain NaNs. Remove or fill them first."
 
         # Generate a continuous elevation vs. dDEM function
-        ddem_func = scipy.interpolate.interp1d(ddem_bins.index.mid, ddem_bins.values,
-                                               kind="linear", fill_value="extrapolate")
+        ddem_func = scipy.interpolate.interp1d(
+            ddem_bins.index.mid, ddem_bins.values, kind="linear", fill_value="extrapolate"
+        )
 
     # Generate average elevations by subtracting half of the dDEM's values to the reference DEM
     if timeframe == "mean":
         elevations = ref_dem - (ddem_func(ref_dem.data) / 2)
     elif timeframe == "reference":
         elevations = ref_dem
     elif timeframe == "nonreference":
         elevations = ref_dem - ddem_func(ref_dem.data)
 
     # Extract the bins from the dDEM series and compute the frequency of points in the bins.
     bins = np.r_[[ddem_bins.index.left[0]], ddem_bins.index.right]
     bin_counts = np.histogram(elevations, bins=bins)[0]
 
     # Multiply the bin counts with the pixel area to get the full area.
-    bin_area = bin_counts * (pixel_size ** 2 if not isinstance(pixel_size, tuple) else pixel_size[0] * pixel_size[1])
+    bin_area = bin_counts * (pixel_size**2 if not isinstance(pixel_size, tuple) else pixel_size[0] * pixel_size[1])
 
     # Put this in a series which will be returned.
     output = pd.Series(index=ddem_bins.index, data=bin_area)
 
     return output
 
 
-def linear_interpolation(array: Union[np.ndarray, np.ma.masked_array], max_search_distance: int = 10,
-                         extrapolate: bool = False, force_fill: bool = False) -> np.ndarray:
+def linear_interpolation(
+    array: NDArrayf | MArrayf,
+    max_search_distance: int = 10,
+    extrapolate: bool = False,
+    force_fill: bool = False,
+) -> NDArrayf:
     """
     Interpolate a 2D array using rasterio's fillnodata.
 
     :param array: An array with NaNs or a masked array to interpolate.
     :param max_search_distance: The maximum number of pixels to search in all directions to find values \
 to interpolate from. The default is 10.
     :param extrapolate: if False, will remove pixels that have been extrapolated by fillnodata. Default is False.
     :param force_fill: if True, will replace all remaining gaps by the median of all valid values. Default is False.
 
     :returns: A filled array with no NaNs
     """
     # Create a mask for where nans exist
-    nan_mask = spatial_tools.get_mask(array)
+    nan_mask = get_mask(array)
 
-    interpolated_array = rasterio.fill.fillnodata(array.copy(), mask=(~nan_mask).astype("uint8"),
-                                                  max_search_distance=max_search_distance)
+    interpolated_array = rasterio.fill.fillnodata(
+        array.copy(), mask=(~nan_mask).astype("uint8"), max_search_distance=max_search_distance
+    )
 
     # Remove extrapolated values: gaps up to the size of max_search_distance are kept,
-    # but surfaces that artifically grow on the edges are removed
+    # but surfaces that artificially grow on the edges are removed
     if not extrapolate:
-        interp_mask = cv2.morphologyEx((~nan_mask).squeeze().astype('uint8'), cv2.MORPH_CLOSE,
-                                       kernel=np.ones((max_search_distance - 1, )*2)).astype('bool')
+        interp_mask = cv2.morphologyEx(
+            (~nan_mask).squeeze().astype("uint8"), cv2.MORPH_CLOSE, kernel=np.ones((max_search_distance - 1,) * 2)
+        ).astype("bool")
         if np.ndim(array) == 3:
             interpolated_array[:, ~interp_mask] = np.nan
         else:
             interpolated_array[~interp_mask] = np.nan
 
     # Fill the nans (values outside of the value boundaries) with the median value
     # This triggers a warning with np.masked_array's because it ignores the mask
     if force_fill:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             interpolated_array[np.isnan(interpolated_array)] = np.nanmedian(array)
     else:
         # If input is masked array, return a masked array
-        extrap_mask = (interpolated_array != array.data)
+        extrap_mask = interpolated_array != array.data
         if isinstance(array, np.ma.masked_array):
             interpolated_array = np.ma.masked_array(interpolated_array, mask=(nan_mask & ~extrap_mask))
 
     return interpolated_array.reshape(array.shape)
 
 
-def hypsometric_interpolation(voided_ddem: Union[np.ndarray, np.ma.masked_array],
-                              ref_dem: Union[np.ndarray, np.ma.masked_array],
-                              mask: np.ndarray) -> np.ma.masked_array:
+def hypsometric_interpolation(
+    voided_ddem: NDArrayf | MArrayf,
+    ref_dem: NDArrayf | MArrayf,
+    mask: NDArrayf,
+) -> MArrayf:
     """
     Interpolate a dDEM using hypsometric interpolation within the given mask.
 
     Using `ref_dem`, elevation bins of constant height (hard-coded to 50 m for now) are created.
     Gaps in `voided-ddem`, within the provided `mask`, are filled with the median dDEM value within that bin.
 
     :param voided_ddem: A dDEM with voids (either an array with nans or a masked array).
     :param ref_dem: The reference DEM in the dDEM comparison.
     :param mask: A mask to delineate the area that will be interpolated (True means hypsometric will be used).
     """
     # Get ddem array with invalid pixels converted to NaN and mask of invalid pixels
-    ddem, ddem_mask = spatial_tools.get_array_and_mask(voided_ddem)
+    ddem, ddem_mask = get_array_and_mask(voided_ddem)
 
     # Get ref_dem array with invalid pixels converted to NaN and mask of invalid pixels
-    dem, dem_mask = spatial_tools.get_array_and_mask(ref_dem)
+    dem, dem_mask = get_array_and_mask(ref_dem)
 
     # Make sure the mask does not have e.g. the shape (1, height, width)
     mask = mask.squeeze()
 
     # A mask of inlier values: The union of the mask and the inverted exclusion masks of both rasters.
     inlier_mask = mask & (~ddem_mask & ~dem_mask)
     if np.count_nonzero(inlier_mask) == 0:
         warnings.warn("No valid data found within mask, returning copy", UserWarning)
-        return np.copy(ddem)
+        return np.ma.masked_array(data=voided_ddem)
 
     # Estimate the elevation dependent gradient.
-    gradient = xdem.volume.hypsometric_binning(
-        ddem[inlier_mask],
-        dem[inlier_mask]
-    )
+    gradient = xdem.volume.hypsometric_binning(ddem[inlier_mask], dem[inlier_mask])
 
     # Interpolate possible missing elevation bins in 1D - no extrapolation done here
     interpolated_gradient = xdem.volume.interpolate_hypsometric_bins(gradient)
 
     gradient_model = scipy.interpolate.interp1d(
-        interpolated_gradient.index.mid,
-        interpolated_gradient["value"].values,
-        fill_value="extrapolate"
+        interpolated_gradient.index.mid, interpolated_gradient["value"].values, fill_value="extrapolate"
     )
 
     # Create an idealized dDEM using the relationship between elevation and dDEM
     idealized_ddem = np.zeros_like(dem)
     idealized_ddem[mask] = gradient_model(dem[mask])
 
     # Replace ddem gaps with idealized hypsometric ddem, but only within mask
     corrected_ddem = np.where(ddem_mask & mask, idealized_ddem, ddem)
 
-    output = np.ma.masked_array(
-        corrected_ddem,
-        mask=~np.isfinite(corrected_ddem)
-    )
+    output = np.ma.masked_array(corrected_ddem, mask=~np.isfinite(corrected_ddem))
 
     assert output is not None
 
     return output
 
 
-def local_hypsometric_interpolation(voided_ddem: Union[np.ndarray, np.ma.masked_array],
-                                    ref_dem: Union[np.ndarray, np.ma.masked_array],
-                                    mask: np.ndarray, min_coverage: float = 0.2,
-                                    count_threshold: Optional[int] = 1, nodata: Union[float, int] = -9999,
-                                    plot: bool = False) -> np.ma.masked_array:
+def local_hypsometric_interpolation(
+    voided_ddem: NDArrayf | MArrayf,
+    ref_dem: NDArrayf | MArrayf,
+    mask: NDArrayf,
+    min_coverage: float = 0.2,
+    count_threshold: int | None = 1,
+    nodata: float | int = -9999,
+    plot: bool = False,
+) -> MArrayf:
     """
     Interpolate a dDEM using local hypsometric interpolation.
     The algorithm loops through each features in the vector file.
 
     The dDEM is assumed to have been created as "voided_ddem = reference_dem - other_dem".
 
     :param voided_ddem: A dDEM with voids (either an array with nans or a masked array).
     :param ref_dem: The reference DEM in the dDEM comparison.
-    :param mask: A raster of same shape as voided_ddem and ref_dem, containing a diferent non-0 pixel value for \
+    :param mask: A raster of same shape as voided_ddem and ref_dem, containing a different non-0 pixel value for \
 each geometry on which to loop.
     :param min_coverage: Optional. The minimum coverage fraction to be considered for interpolation.
     :param count_threshold: Optional. A pixel count threshold to exclude during the hypsometric curve fit.
     :param nodata: Optional. No data value to be used for the output masked_array.
     :param plot: Set to True to display intermediate plots.
 
     :returns: A dDEM with gaps filled by applying a hypsometric interpolation for each geometry in mask, \
@@ -394,105 +409,102 @@
     ref_dem = ref_dem.squeeze()
     mask = mask.squeeze()
 
     # Check that all arrays have same dimensions
     assert voided_ddem.shape == ref_dem.shape == mask.shape
 
     # Get ddem array with invalid pixels converted to NaN and mask of invalid pixels
-    ddem, ddem_mask = spatial_tools.get_array_and_mask(voided_ddem)
+    ddem, ddem_mask = get_array_and_mask(voided_ddem)
 
     # Get ref_dem array with invalid pixels converted to NaN and mask of invalid pixels
-    dem, dem_mask = spatial_tools.get_array_and_mask(ref_dem)
+    dem, dem_mask = get_array_and_mask(ref_dem)
 
     # A mask of inlier values: The union of the mask and the inverted exclusion masks of both rasters.
     inlier_mask = (mask != 0) & (~ddem_mask & ~dem_mask)
     if np.count_nonzero(inlier_mask) == 0:
         warnings.warn("No valid data found within mask, returning copy", UserWarning)
-        return np.copy(ddem)
+        return np.ma.masked_array(voided_ddem)
 
     if plot:
         plt.matshow(inlier_mask)
         plt.title("inlier mask")
         plt.show()
 
     # List of indexes to loop on
     geometry_index = np.unique(mask[mask != 0])
-    print("Found {:d} geometries".format(len(geometry_index)))
+    print(f"Found {len(geometry_index):d} geometries")
 
     # Get fraction of valid pixels for each geometry
     coverage = np.zeros(len(geometry_index))
     for k, index in enumerate(geometry_index):
         local_inlier_mask = inlier_mask & (mask == index)
-        total_pixels = np.count_nonzero((mask == index))
+        total_pixels = np.count_nonzero(mask == index)
         valid_pixels = np.count_nonzero(local_inlier_mask)
-        coverage[k] = valid_pixels/float(total_pixels)
+        coverage[k] = valid_pixels / float(total_pixels)
 
     # Filter geometries with too little coverage
     valid_geometry_index = geometry_index[coverage >= min_coverage]
-    print("Found {:d} geometries with sufficient coverage".format(len(valid_geometry_index)))
+    print(f"Found {len(valid_geometry_index):d} geometries with sufficient coverage")
 
     idealized_ddem = nodata * np.ones_like(dem)
 
-    for k, index in enumerate(valid_geometry_index):
+    for _k, index in enumerate(valid_geometry_index):
 
         # Mask of valid pixel within geometry
-        local_mask = (mask == index)
+        local_mask = mask == index
         local_inlier_mask = inlier_mask & (local_mask)
 
         # Estimate the elevation dependent gradient
-        gradient = xdem.volume.hypsometric_binning(
-            ddem[local_mask],
-            dem[local_mask]
-        )
+        gradient = xdem.volume.hypsometric_binning(ddem[local_mask], dem[local_mask])
 
         # Remove bins with loo low count
         filt_gradient = gradient.copy()
-        if count_threshold > 1:
-            bins_under_threshold = filt_gradient["count"] < count_threshold
-            filt_gradient.loc[bins_under_threshold, "value"] = np.nan
+        if count_threshold is not None:
+            if count_threshold > 1:
+                bins_under_threshold = filt_gradient["count"] < count_threshold
+                filt_gradient.loc[bins_under_threshold, "value"] = np.nan
 
         # Interpolate missing elevation bins
         interpolated_gradient = xdem.volume.interpolate_hypsometric_bins(filt_gradient)
 
         # At least 2 points needed for interp1d, if not skip feature
-        nvalues = len(interpolated_gradient['value'].values)
+        nvalues = len(interpolated_gradient["value"].values)
         if nvalues < 2:
             warnings.warn(
-                "Not enough valid bins for feature with index {:d} -> skipping interpolation".format(index),
-                UserWarning
+                f"Not enough valid bins for feature with index {index:d} -> skipping interpolation", UserWarning
             )
             continue
 
         # Create a model for 2D interpolation
         gradient_model = scipy.interpolate.interp1d(
-            interpolated_gradient.index.mid,
-            interpolated_gradient['value'].values,
-            fill_value="extrapolate"
+            interpolated_gradient.index.mid, interpolated_gradient["value"].values, fill_value="extrapolate"
         )
 
         if plot:
             local_ddem = np.where(local_inlier_mask, ddem, np.nan)
             vmax = max(np.abs(np.nanpercentile(local_ddem, [2, 98])))
-            rowmin, rowmax, colmin, colmax = spatial_tools.get_valid_extent(mask == index)
+            rowmin, rowmax, colmin, colmax = get_valid_extent(mask == index)
 
-            fig = plt.figure(figsize=(12, 8))
+            plt.figure(figsize=(12, 8))
             plt.subplot(121)
-            plt.imshow((mask == index)[rowmin:rowmax, colmin:colmax], cmap='Greys',
-                       vmin=0, vmax=2, interpolation='none')
+            plt.imshow(
+                (mask == index)[rowmin:rowmax, colmin:colmax], cmap="Greys", vmin=0, vmax=2, interpolation="none"
+            )
 
-            plt.imshow(local_ddem[rowmin:rowmax, colmin:colmax], cmap='RdYlBu',
-                       vmin=-vmax, vmax=vmax, interpolation='none')
+            plt.imshow(
+                local_ddem[rowmin:rowmax, colmin:colmax], cmap="RdYlBu", vmin=-vmax, vmax=vmax, interpolation="none"
+            )
             plt.colorbar()
-            plt.title("ddem for geometry # {:d}".format(index))
+            plt.title(f"ddem for geometry # {index:d}")
 
             plt.subplot(122)
-            plt.plot(gradient["value"], gradient.index.mid, label='raw')
-            plt.plot(interpolated_gradient, gradient.index.mid, label='interpolated', ls='--')
-            plt.xlabel('ddem')
-            plt.ylabel('Elevation')
+            plt.plot(gradient["value"], gradient.index.mid, label="raw")
+            plt.plot(interpolated_gradient, gradient.index.mid, label="interpolated", ls="--")
+            plt.xlabel("ddem")
+            plt.ylabel("Elevation")
             plt.legend()
             plt.title("Average ddem per elevation bin")
             plt.tight_layout()
             plt.show()
 
         # Create an idealized dDEM (only considering the dH gradient)
         idealized_ddem[mask == index] = gradient_model(dem[mask == index])
@@ -509,42 +521,46 @@
     # Correct the idealized dDEM with the difference to the original dDEM.
     corrected_ddem = idealized_ddem + interpolated_ddem_diff
 
     # Set Nans to nodata
     corrected_ddem[~np.isfinite(corrected_ddem)] = nodata
 
     output = np.ma.masked_array(
-        corrected_ddem,
-        mask=(corrected_ddem == nodata)  # mask=((mask != 0) & (ddem_mask | dem_mask))
+        corrected_ddem, mask=(corrected_ddem == nodata)  # mask=((mask != 0) & (ddem_mask | dem_mask))
     ).reshape(orig_shape)
 
     assert output is not None
 
     return output
 
 
-def get_regional_hypsometric_signal(ddem: Union[np.ndarray, np.ma.masked_array],
-                                    ref_dem: Union[np.ndarray, np.ma.masked_array],
-                                    glacier_index_map: np.ndarray, n_bins: int = 20,
-                                    verbose: bool = False, min_coverage: float = 0.05) -> pd.DataFrame:
+def get_regional_hypsometric_signal(
+    ddem: NDArrayf | MArrayf | RasterType,
+    ref_dem: NDArrayf | MArrayf | RasterType,
+    glacier_index_map: NDArrayf | RasterType,
+    n_bins: int = 20,
+    verbose: bool = False,
+    min_coverage: float = 0.05,
+) -> pd.DataFrame:
     """
     Get the normalized regional hypsometric elevation change signal, read "the general shape of it".
 
     :param ddem: The dDEM to analyse.
     :param ref_dem: A void-free reference DEM.
     :param glacier_index_map: An array glacier indices of the same shape as the previous inputs.
     :param verbose: Show progress bar.
     n_bins = 20  # TODO: This should be an argument.
     :param n_bins: The number of elevation bins to subdivide each glacier in.
 
     :returns: A DataFrame of bin statistics, scaled by elevation and elevation change.
     """
     # Extract the array and mask representations of the arrays.
-    ddem_arr, ddem_mask = spatial_tools.get_array_and_mask(ddem.squeeze())
-    ref_arr, ref_mask = spatial_tools.get_array_and_mask(ref_dem.squeeze())
+    ddem_arr, ddem_mask = get_array_and_mask(ddem)
+    ref_arr, ref_mask = get_array_and_mask(ref_dem)
+    glacier_index_map, _ = get_array_and_mask(glacier_index_map)
 
     # The reference DEM should be void free
     assert np.count_nonzero(ref_mask) == 0, "Reference DEM has voids"
 
     # The unique indices are the unique glaciers.
     unique_indices = np.unique(glacier_index_map)
 
@@ -556,15 +572,15 @@
     count = 0
     # Loop over each unique glacier.
     for i in tqdm(np.unique(glacier_index_map), desc="Finding regional signal", disable=(not verbose)):
         # If i ==0, it's assumed to be periglacial.
         if i == 0:
             continue
         # Create a mask representing a particular glacier.
-        glacier_values = (glacier_index_map == i)
+        glacier_values = glacier_index_map == i
 
         # Stop if the "glacier" is tiny. It might be a cropped glacier outline for example.
         if np.count_nonzero(glacier_values) < 10:
             continue
 
         # The inlier mask is where that particular glacier is and where nans don't exist.
         inlier_mask = glacier_values & ~ddem_mask
@@ -576,23 +592,25 @@
         # Extract only the difference and elevation values that correspond to the glacier.
         differences = ddem_arr[inlier_mask]
         elevations = ref_arr[inlier_mask]
 
         # Run the hypsometric binning.
         try:
             bins = hypsometric_binning(differences, elevations, bins=n_bins, kind="count")
-        except ValueError:  # ValueError: zero-size array to reduction operation minimum which has no identity on "zbins=" call
+        except ValueError:
+            # ValueError: zero-size array to reduction operation minimum which has no identity on "zbins=" call
             continue
 
         # Min-max scale by elevation.
         bins.index = (bins.index.mid - bins.index.left.min()) / (bins.index.right.max() - bins.index.left.min())
 
         # Scale by difference.
-        bins["value"] = (bins["value"] - np.nanmin(bins["value"])) / \
-            (np.nanmax(bins["value"]) - np.nanmin(bins["value"]))
+        bins["value"] = (bins["value"] - np.nanmin(bins["value"])) / (
+            np.nanmax(bins["value"]) - np.nanmin(bins["value"])
+        )
 
         # Assign the values and counts to the output array.
         values[:, count] = bins["value"]
         counts[:, count] = bins["count"]
 
         count += 1
 
@@ -609,22 +627,24 @@
         },
         index=pd.IntervalIndex.from_breaks(np.linspace(0, 1, n_bins + 1, dtype="float64")),
     )
 
     return output
 
 
-def norm_regional_hypsometric_interpolation(voided_ddem: Union[np.ndarray, np.ma.masked_array],
-                                            ref_dem: Union[np.ndarray, np.ma.masked_array],
-                                            glacier_index_map: np.ndarray,
-                                            min_coverage: float = 0.1,
-                                            regional_signal: Optional[pd.DataFrame] = None,
-                                            verbose: bool = False,
-                                            min_elevation_range: float = 0.33,
-                                            idealized_ddem: bool = False) -> np.ndarray:
+def norm_regional_hypsometric_interpolation(
+    voided_ddem: NDArrayf | MArrayf | RasterType,
+    ref_dem: NDArrayf | MArrayf | RasterType,
+    glacier_index_map: NDArrayf | RasterType,
+    min_coverage: float = 0.1,
+    regional_signal: pd.DataFrame | None = None,
+    verbose: bool = False,
+    min_elevation_range: float = 0.33,
+    idealized_ddem: bool = False,
+) -> NDArrayf:
     """
     Interpolate missing values by scaling the normalized regional hypsometric signal to each glacier separately.
 
     Only missing values are interpolated. The rest of the glacier's values are fixed.
 
     :param voided_ddem: The voided dDEM to fill NaNs in.
     :param ref_dem: A void-free reference DEM.
@@ -637,40 +657,38 @@
     :param idealized_ddem: Replace observed glacier values with the hypsometric signal. Good for error assessments.
 
     :raises AssertionError: If `ref_dem` has voids.
 
     :returns: A dDEM where glacier's that fit the min_coverage criterion are interpolated.
     """
     # Extract the array and nan parts of the inputs.
-    ddem_arr, ddem_nans = spatial_tools.get_array_and_mask(voided_ddem)
-    ref_arr, ref_nans = spatial_tools.get_array_and_mask(ref_dem)
+    ddem_arr, ddem_nans = get_array_and_mask(voided_ddem)
+    ref_arr, ref_nans = get_array_and_mask(ref_dem)
+    glacier_index_map, _ = get_array_and_mask(glacier_index_map)
 
     # The reference DEM should be void free
     assert np.count_nonzero(ref_nans) == 0, "Reference DEM has voids"
 
     # If the regional signal was not given as an argument, find it from the dDEM.
     if regional_signal is None:
         regional_signal = get_regional_hypsometric_signal(
-            ddem=ddem_arr,
-            ref_dem=ref_arr,
-            glacier_index_map=glacier_index_map,
-            verbose=verbose
+            ddem=ddem_arr, ref_dem=ref_arr, glacier_index_map=glacier_index_map, verbose=verbose
         )
 
     # The unique indices are the unique glaciers.
     unique_indices = np.unique(glacier_index_map)
 
     # Make a copy of the dDEM which will be filled iteratively.
     ddem_filled = ddem_arr.copy()
     # Loop over all glaciers and fill the dDEM accordingly.
     for i in tqdm(unique_indices, desc="Interpolating dDEM", disable=(not verbose)):
         if i == 0:  # i==0 is assumed to mean stable ground.
             continue
         # Create a mask representing a particular glacier.
-        glacier_values = (glacier_index_map == i)
+        glacier_values = glacier_index_map == i
 
         # The inlier mask is where that particular glacier is and where nans don't exist.
         inlier_mask = glacier_values & ~ddem_nans
 
         # If the fractional coverage is smaller than the given threshold, skip the glacier.
         if (np.count_nonzero(inlier_mask) / np.count_nonzero(glacier_values)) < min_coverage:
             continue
@@ -694,22 +712,22 @@
         signal.index = pd.IntervalIndex.from_arrays(left=midpoints - step / 2, right=midpoints + step / 2)
 
         # Find the hypsometric bins of the glacier.
         hypsometric_bins = hypsometric_binning(
             ddem=differences,
             ref_dem=elevations,
             bins=np.r_[[signal.index.left[0]], signal.index.right],  # This will generate the same steps as the signal.
-            kind="custom"
+            kind="custom",
         )
         bin_stds = hypsometric_binning(
             ddem=differences,
             ref_dem=elevations,
             bins=np.r_[[signal.index.left[0]], signal.index.right],
             kind="custom",
-            aggregation_function=np.nanstd
+            aggregation_function=np.nanstd,
         )
         # Check which of the bins were non-empty.
         non_empty_bins = np.isfinite(hypsometric_bins["value"])
 
         non_empty_range = np.sum(non_empty_bins[non_empty_bins].index.length)
         full_range = np.sum(hypsometric_bins.index.length)
 
@@ -717,16 +735,17 @@
             continue
 
         # A theoretical minimum of 2 bins are needed for the curve fit.
         if np.count_nonzero(non_empty_bins) < 2:
             continue
 
         # The weights are the squared inverse of the standard deviation of each bin.
-        bin_weights = bin_stds["value"].values[non_empty_bins] / \
-            np.sqrt(hypsometric_bins["count"].values[non_empty_bins])
+        bin_weights = bin_stds["value"].values[non_empty_bins] / np.sqrt(
+            hypsometric_bins["count"].values[non_empty_bins]
+        )
         bin_weights[bin_weights == 0.0] = 1e-8  # Avoid divide by zero problems.
 
         # Fit linear coefficients to scale the regional signal to the hypsometric bins properly.
         # The inverse of the pixel counts are used as weights, to properly disregard poorly constrained bins.
         with warnings.catch_warnings():
             # curve_fit will sometimes say "can't estimate covariance". This is okay.
             warnings.filterwarnings("ignore", message="covariance")
@@ -735,15 +754,17 @@
                 xdata=signal.values[non_empty_bins],  # The xdata is the normalized regional signal
                 ydata=hypsometric_bins["value"].values[non_empty_bins],  # The ydata is the actual values.
                 p0=[1, 0],  # The initial guess of a and b (doesn't matter too much)
                 sigma=bin_weights,
             )[0]
 
         # Create a linear model from the elevations and the scaled regional signal.
-        model = scipy.interpolate.interp1d(signal.index.mid, np.poly1d(coeffs)(signal.values), bounds_error=False, fill_value="extrapolate")
+        model = scipy.interpolate.interp1d(
+            signal.index.mid, np.poly1d(coeffs)(signal.values), bounds_error=False, fill_value="extrapolate"
+        )
 
         # Find which values to fill using the model (all nans within the glacier extent)
         if not idealized_ddem:
             values_to_fill = glacier_values & ddem_nans
         # If it should be idealized, replace all glacier values with the model
         else:
             values_to_fill = glacier_values
```

### Comparing `xdem-0.0.7/xdem.egg-info/PKG-INFO` & `xdem-0.0.8/xdem.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,94 @@
 Metadata-Version: 2.1
 Name: xdem
-Version: 0.0.7
+Version: 0.0.8
 Summary: Set of tools to manipulate Digital Elevation Models (DEMs) 
 Home-page: https://github.com/GlacioHack/xdem
 Author: The GlacioHack Team
 Author-email: this-is-not-an-email@a.com
 License: BSD-3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rioxarray
 Provides-Extra: richdem
 Provides-Extra: opencv
 Provides-Extra: pytransform3d
 License-File: LICENSE
 
-# xdem
-Set of tools to manipulate Digital Elevation Models (DEMs)
-
-More documentation to come!
+# xDEM: robust analysis of DEMs in Python.
 
 [![Documentation Status](https://readthedocs.org/projects/xdem/badge/?version=latest)](https://xdem.readthedocs.io/en/latest/?badge=latest)
 [![build](https://github.com/GlacioHack/xdem/actions/workflows/python-package.yml/badge.svg)](https://github.com/GlacioHack/xdem/actions/workflows/python-package.yml)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/xdem.svg)](https://anaconda.org/conda-forge/xdem)
+[![PyPI version](https://badge.fury.io/py/xdem.svg)](https://badge.fury.io/py/xdem)
 [![Coverage Status](https://coveralls.io/repos/github/GlacioHack/xdem/badge.svg?branch=main)](https://coveralls.io/github/GlacioHack/xdem?branch=main)
 
-To cite this package: [![Zenodo](https://zenodo.org/badge/doi/10.5281/zenodo.4809697.svg)](https://zenodo.org/record/4809698)
-
-## Installation
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GlacioHack/xdem/main)
+[![Pre-Commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+**xDEM** is an open source project to develop a core Python package for the analysis of digital elevation models (DEMs).
+
+It aims at **providing modular and robust tools for the most common analyses needed with DEMs**, including both geospatial
+operations specific to DEMs and a wide range of 3D alignment and correction methods from published, peer-reviewed studies.
+The core manipulation of DEMs (e.g., vertical alignment, terrain analysis) are **conveniently centered around `DEM` and `dDEM` classes** (that, notably, re-implements all tools
+of [gdalDEM](https://gdal.org/programs/gdaldem.html)). More complex pipelines (e.g., 3D rigid coregistration, bias corrections, filtering) are **built around
+modular `Coreg`, `BiasCorr` and `Filter` classes that easily interface between themselves**. Finally, xDEM includes advanced
+uncertainty analysis tools based on spatial statistics of [SciKit-GStat](https://scikit-gstat.readthedocs.io/en/latest/).
+
+Additionally, xDEM inherits many convenient functionalities from [GeoUtils](https://github.com/GlacioHack/geoutils) such as
+**implicit loading**, **numerical interfacing** and **convenient object-based geospatial methods** to easily perform
+the most common higher-level tasks needed by geospatial users (e.g., reprojection, cropping, vector masking). Through [GeoUtils](https://github.com/GlacioHack/geoutils), xDEM
+relies on [Rasterio](https://github.com/rasterio/rasterio), [GeoPandas](https://github.com/geopandas/geopandas) and [Pyproj](https://github.com/pyproj4/pyproj)
+for georeferenced calculations, and on [NumPy](https://github.com/numpy/numpy) and [Xarray](https://github.com/pydata/xarray) for numerical analysis. It allows easy access to
+the functionalities of these packages through interfacing or composition, and quick inter-operability through object conversion.
+
+If you are looking for an accessible Python package to write the Python equivalent of your [GDAL](https://gdal.org/) command lines, or of your
+[QGIS](https://www.qgis.org/en/site/) analysis pipeline **without a steep learning curve** on Python GIS syntax, xDEM is perfect for you! For more advanced
+users, xDEM also aims at being efficient and scalable by supporting lazy loading and parallel computing (ongoing).
 
-### With conda (recommended)
-```bash
-conda install -c conda-forge --strict-channel-priority xdem
-```
-The `--strict-channel-priority` flag seems essential for Windows installs to function correctly, and is recommended for UNIX-based systems as well.
-
-Solving dependencies can take a long time with `conda`. To speed up this, consider installing `mamba`:
-
-```bash
-conda install mamba -n base -c conda-forge
-```
+## Documentation
 
-Once installed, the same commands can be run by simply replacing `conda` by `mamba`. More details available through the [mamba project](https://github.com/mamba-org/mamba).
+For a quick start, full feature description or search through the API, see xDEM's documentation at: https://xdem.readthedocs.io.
 
-If running into the `sklearn` error `ImportError: dlopen: cannot load any more object with static TLS`, your system 
-needs to update its `glibc` (see details [here](https://github.com/scikit-learn/scikit-learn/issues/14485#issuecomment-822678559)).
-If you have no administrator right on the system, you might be able to circumvent this issue by installing a working 
-environment with specific downgraded versions of `scikit-learn` and `numpy`:
-```bash
-conda create -n xdem-env -c conda-forge xdem scikit-learn==0.20.3 numpy==1.19.*
-```
-On very old systems, if the above install results in segmentation faults, try setting more specifically 
-`numpy==1.19.2=py37h54aff64_0` (worked with Debian 8.11, GLIBC 2.19).
+## Installation
 
-### Installing with pip
-**NOTE**: Setting up GDAL and PROJ may need some extra steps, depending on your operating system and configuration.
 ```bash
-pip install xdem
-```
-
-### Installing for contributors
-Recommended: Use conda for depencency solving.
-```
-$ git clone https://github.com/GlacioHack/xdem.git
-$ cd ./xdem
-$ conda env create -f dev-environment.yml
-$ conda activate xdem
-$ pip install -e .
-```
-After installing, we recommend to check that everything is working by running the tests:
-
+mamba install -c conda-forge xdem
 ```
-$ pytest -rA
-```
-
-## Structure 
-
-xdem are for now composed of three libraries:
-- `coreg.py` with tools covering differet aspects of DEM coregistration
-- `spatial_tools.py` for spatial operations on DEMs
-- `dem.py` for DEM-specific operations, such as vertical datum correction.
-
-## How to contribute
-
-You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/xdem/issues) section. All contributions are welcome.
-To avoid conflicts, it is suggested to use separate branches for each implementation. All changes must then be submitted to the dev branch using pull requests. Each PR must be reviewed by at least one other person.
-
-Please see our [contribution page](CONTRIBUTING.md) for more detailed instructions.
-
-### Documentation
-See the documentation at https://xdem.readthedocs.io
-
-### Testing - again please read!
-These tools are only valuable if we can rely on them to perform exactly as we expect. So, we need testing. Please create tests for every function that you make, as much as you are able. Guidance/examples here for the moment: https://github.com/GeoUtils/georaster/blob/master/test/test_georaster.py
-https://github.com/corteva/rioxarray/blob/master/test/integration/test_integration__io.py
-
+See [mamba's documentation](https://mamba.readthedocs.io/en/latest/) to install `mamba`, which will solve your environment much faster than `conda`.
 
+## Citing methods implemented in the package
 
-### Examples
+When using a method implemented in xDEM, please **cite both the package and the related study**:
 
-**Coregister a DEM to another DEM**
-```python
-import xdem
+Citing xDEM: [![Zenodo](https://zenodo.org/badge/doi/10.5281/zenodo.4809697.svg)](https://zenodo.org/record/4809698)
 
-reference_dem = xdem.DEM("path/to/reference.tif")
-dem_to_be_aligned = xdem.DEM("path/to/dem.tif")
+Citing the related study:
 
-nuth_kaab = xdem.coreg.NuthKaab()
+- **Coregistration**:
+  - Horizontal shift from aspect/slope relationship of *[Nuth and Kääb (2011)](https://doi.org/10.5194/tc-5-271-2011)*,
+  - Iterative closest point (ICP) of *[Besl and McKay (1992)](http://dx.doi.org/10.1109/34.121791)*,
+- **Bias correction**:
+  - Along-track multi-sinusoidal noise by basin-hopping of *[Girod et al. (2017)](https://doi.org/10.3390/rs9070704)*,
+- **Uncertainty analysis**:
+  - Heteroscedasticity and multi-range correlations from stable terrain of *[Hugonnet et al. (2022)](https://doi.org/10.1109/JSTARS.2022.3188922)*,
+- **Terrain attributes**:
+  - Slope, aspect and hillshade of either *[Horn (1981)](http://dx.doi.org/10.1109/PROC.1981.11918)* or *[Zevenbergen and Thorne (1987)](http://dx.doi.org/10.1002/esp.3290120107)*,
+  - Profile, plan and maximum curvature of *[Zevenbergen and Thorne (1987)](http://dx.doi.org/10.1002/esp.3290120107)*,
+  - Topographic position index of *[Weiss (2001)](http://www.jennessent.com/downloads/TPI-poster-TNC_18x22.pdf)*,
+  - Terrain ruggedness index of either *[Riley et al. (1999)](http://download.osgeo.org/qgis/doc/reference-docs/Terrain_Ruggedness_Index.pdf)* or *[Wilson et al. (2007)](http://dx.doi.org/10.1080/01490410701295962)*,
+  - Roughness of *[Dartnell (2000)](http://dx.doi.org/10.14358/PERS.70.9.1081)*,
+  - Rugosity of *[Jenness (2004)](https://doi.org/10.2193/0091-7648(2004)032[0829:CLSAFD]2.0.CO;2)*,
+  - Fractal roughness of *[Taud et Parrot (2005)](https://doi.org/10.4000/geomorphologie.622)*.
 
-nuth_kaab.fit(reference_dem.data, dem_to_be_aligned.data, transform=reference_dem.transform)
+## Start contributing
 
+1. Fork the repository, make a feature branch and push changes.
+2. When ready, submit a pull request from the feature branch of your fork to `GlacioHack/geoutils:main`.
+3. The PR will be reviewed by at least one maintainer, discussed, then merged.
 
-aligned_dem = xdem.DEM.from_array(
-	nuth_kaab.apply(dem_to_be_aligned.data, transform=dem_to_be_aligned.transform),
-	transform=dem_to_be_aligned.transform,
-	crs=dem_to_be_aligned.crs
-)
-
-aligned_dem.save("path/to/coreg.tif")
-```
-This is an implementation of the [Nuth and Kääb (2011)](https://doi.org/10.5194/tc-5-271-2011) approach.
-[Please see the documentation](https://xdem.readthedocs.io/en/latest/coregistration.html) for more approaches.
-
-**Subtract one DEM with another**
-```python
-import xdem
-
-first_dem = xdem.DEM("path/to/first.tif")
-second_dem = xdem.DEM("path/to/second.tif")
-
-difference = first_dem - second_dem
-
-difference.save("path/to/difference.tif")
-```
-By default, `second_dem` is reprojected to fit `first_dem`.
-This can be switched with the keyword argument `reference="second"`.
-The resampling method can also be changed (e.g. `resampling_method="nearest"`) from the default `"cubic_spline"`.
-
+More info on [our contributing page](CONTRIBUTING.md).
```

