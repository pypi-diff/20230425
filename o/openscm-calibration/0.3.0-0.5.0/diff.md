# Comparing `tmp/openscm_calibration-0.3.0.tar.gz` & `tmp/openscm_calibration-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openscm_calibration-0.3.0.tar", max compression
+gzip compressed data, was "openscm_calibration-0.5.0.tar", max compression
```

## Comparing `openscm_calibration-0.3.0.tar` & `openscm_calibration-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1494 2023-03-28 06:22:50.306791 openscm_calibration-0.3.0/LICENSE
--rw-r--r--   0        0        0     1785 2023-04-21 03:24:50.664404 openscm_calibration-0.3.0/README.rst
--rw-r--r--   0        0        0     3622 2023-04-21 03:52:28.595137 openscm_calibration-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      170 2023-04-21 03:24:50.718664 openscm_calibration-0.3.0/src/openscm_calibration/__init__.py
--rw-r--r--   0        0        0     6260 2023-04-21 03:24:50.719466 openscm_calibration-0.3.0/src/openscm_calibration/cost.py
--rw-r--r--   0        0        0    11764 2023-04-21 03:24:50.720379 openscm_calibration-0.3.0/src/openscm_calibration/emcee_plotting.py
--rw-r--r--   0        0        0     4191 2023-04-21 03:24:50.721233 openscm_calibration-0.3.0/src/openscm_calibration/emcee_utils.py
--rw-r--r--   0        0        0      652 2023-04-21 03:24:50.722026 openscm_calibration-0.3.0/src/openscm_calibration/iter_utils.py
--rw-r--r--   0        0        0     2675 2023-04-21 03:24:50.722970 openscm_calibration-0.3.0/src/openscm_calibration/minimize.py
--rw-r--r--   0        0        0     6499 2023-04-21 03:24:50.724048 openscm_calibration-0.3.0/src/openscm_calibration/model_runner.py
--rw-r--r--   0        0        0        0 2023-04-21 03:24:50.724623 openscm_calibration-0.3.0/src/openscm_calibration/py.typed
--rw-r--r--   0        0        0    25457 2023-04-21 03:24:50.726750 openscm_calibration-0.3.0/src/openscm_calibration/scipy_plotting.py
--rw-r--r--   0        0        0      827 2023-04-21 03:24:50.727865 openscm_calibration-0.3.0/src/openscm_calibration/scmdata_utils.py
--rw-r--r--   0        0        0    10244 2023-04-21 03:24:50.728975 openscm_calibration-0.3.0/src/openscm_calibration/store.py
--rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 openscm_calibration-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1494 2023-04-25 04:44:58.071324 openscm_calibration-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2424 2023-04-25 04:44:58.071324 openscm_calibration-0.5.0/README.rst
+-rw-r--r--   0        0        0     3620 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/__init__.py
+-rw-r--r--   0        0        0     6260 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/cost.py
+-rw-r--r--   0        0        0    11764 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/emcee_plotting.py
+-rw-r--r--   0        0        0     4191 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/emcee_utils.py
+-rw-r--r--   0        0        0     1583 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/matplotlib_utils.py
+-rw-r--r--   0        0        0     2675 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/minimize.py
+-rw-r--r--   0        0        0     6499 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/model_runner.py
+-rw-r--r--   0        0        0        0 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/py.typed
+-rw-r--r--   0        0        0    30078 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/scipy_plotting.py
+-rw-r--r--   0        0        0      827 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/scmdata_utils.py
+-rw-r--r--   0        0        0    10244 2023-04-25 04:44:58.083324 openscm_calibration-0.5.0/src/openscm_calibration/store.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 openscm_calibration-0.5.0/PKG-INFO
```

### Comparing `openscm_calibration-0.3.0/LICENSE` & `openscm_calibration-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/README.rst` & `openscm_calibration-0.5.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 .. sec-begin-description
 
 OpenSCM-Calibration
 ===================
 
++-------------------+------+--------+
+| Repository health | |CI| | |Docs| |
++-------------------+------+--------+
+
+.. sec-begin-links
+
+.. |CI| image:: https://github.com/openscm/OpenSCM-Calibration/workflows/CI/badge.svg
+    :target: https://github.com/openscm/OpenSCM-Calibration/actions?query=workflow%3A%22CI%22
+    :alt: CI status
+.. |Docs| image:: https://readthedocs.org/projects/openscm-calibration/badge/?version=latest
+    :target: https://openscm-calibration.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation status
+
+.. sec-end-links
+
 Calibration tools for simple climate models (and other things perhaps,
 surprise us with your applications).
 
+Full documentation can be found at https://openscm-calibration.readthedocs.io/.
+
 .. sec-end-description
 
 .. sec-begin-installation
 
 Installation
 ------------
```

### Comparing `openscm_calibration-0.3.0/pyproject.toml` & `openscm_calibration-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "0.3.0"
+version = "0.5.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 major_version_zero = true
 
 [tool.jupytext]
 formats = "ipynb,myst"
 
 [tool.poetry]
 name = "openscm-calibration"
-version = "0.3.0"
+version = "0.5.0"
 description = ""
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-energy-college.org>"]
 readme = "README.rst"
 packages = [{include = "openscm_calibration", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -21,21 +21,19 @@
 scmdata = "0.15.0"
 openscm-units = "^0.5.0"
 
 notebook = { version = "^6.5.3", optional = true }
 emcwrap = { version = "^0.2.4", optional = true }
 multiprocess = { version = "^0.70.14", optional = true }
 tqdm = { version = "^4.65.0", optional = true }
-# While waiting for a new release, see
-# https://github.com/dnanhkhoa/nb_black/issues/38
-nb-black = { version = "^1.0.7",  optional = true }
 corner = { version = "^2.2.1", optional = true }
 seaborn = { version = "^0.12.2", optional = true }
 h5py = { version = "^3.8.0", optional = true }
 ipywidgets = { version = "^8.0.6", optional = true }
+more-itertools = "^9.1.0"
 
 [tool.poetry.extras]
 notebooks = ["notebook", "emcwrap", "multiprocess", "tqdm", "corner", "seaborn", "nb-black", "h5py", "ipywidgets"]
 plots = ["corner", "seaborn"]
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.2.2"
@@ -56,14 +54,16 @@
 isort = "^5.12.0"
 mypy = "^1.1.1"
 pydocstyle = {extras = ["toml"], version = "^6.3.0"}
 pylint = "^2.17.1"
 bandit = "^1.7.5"
 pytest-cov = "^4.0.0"
 commitizen = "^2.42.1"
+blacken-docs = { git = "https://github.com/znicholls/blacken-docs.git", rev = "3e62e39" }
+tokenize-rt = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 known_first_party = "openscm_calibration"
```

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/cost.py` & `openscm_calibration-0.5.0/src/openscm_calibration/cost.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/emcee_plotting.py` & `openscm_calibration-0.5.0/src/openscm_calibration/emcee_plotting.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/emcee_utils.py` & `openscm_calibration-0.5.0/src/openscm_calibration/emcee_utils.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/minimize.py` & `openscm_calibration-0.5.0/src/openscm_calibration/minimize.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/model_runner.py` & `openscm_calibration-0.5.0/src/openscm_calibration/model_runner.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/scipy_plotting.py` & `openscm_calibration-0.5.0/src/openscm_calibration/scipy_plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,33 +7,37 @@
 import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
+    List,
     Optional,
     Protocol,
     Tuple,
     Union,
 )
 
+import more_itertools
 import numpy as np
 import scmdata
 from attrs import define, field
 
+from openscm_calibration.matplotlib_utils import get_fig_axes_holder_from_mosaic
+
 if TYPE_CHECKING:
     import attr
     import matplotlib
     import numpy.typing as nptype
     import pandas as pd
     import scmdata.run
     import tqdm
 
-    import openscm_calibration.store
+    from openscm_calibration.store import OptResStore
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 """Logger for this module"""
 
 
 class SupportsScipyOptCallback(Protocol):
@@ -83,23 +87,31 @@
     Class that supports updating figures
 
     For example, :class:`IPython.core.display_functions.DisplayHandle`
     """
 
     def update(
         self,
-        fig: matplotlib.figure.Figure,
-    ) -> None:
+        obj: Any,
+        **kwargs: Any,
+    ) -> Any:
         """
         Update the figure
 
         Parameters
         ----------
-        fig
+        obj
             Figure to update
+
+        **kwargs
+            Other arguments used by the updater
+
+        Returns
+        -------
+            Anything (not used)
         """
 
 
 ScmRunToDictConverter = Callable[
     [scmdata.run.BaseScmRun], Dict[str, scmdata.run.BaseScmRun]
 ]
 """
@@ -218,24 +230,24 @@
     ``timeseries_axes``. See docstring of ``timeseries_axes`` for rules about
     its values.
     """
 
     cost_key: str
     """Key for the axes on which the cost function should be plotted"""
 
-    parameters: Tuple[str] = field(validator=[_all_in_axes])
+    parameters: Tuple[str, ...] = field(validator=[_all_in_axes])
     """
     Parameters to be optimised
 
     This must match the order in which the parameters are handled by the
     optimiser i.e. it is used to translate the unlabeled array of parameter
     values onto the desired axes.
     """
 
-    timeseries_axes: Tuple[str] = field(
+    timeseries_axes: Tuple[str, ...] = field(
         validator=[_all_in_axes, _compatible_with_convert_and_target]
     )
     """
     Axes on which to plot timeseries
 
     The timeseries in ``target`` and ``store.res`` are
     converted into dictionaries using ``convert_scmrun_to_plot_dict``. The
@@ -248,15 +260,15 @@
     Callable which converts :obj:`scmdata.run.BaseScmRun` into a dictionary in
     which the keys are a subset of the values in ``timeseries_axes``
     """
 
     target: scmdata.run.BaseScmRun
     """Target to which we are optimising"""
 
-    store: openscm_calibration.store.OptResStore
+    store: OptResStore
     """Optimisation result store"""
 
     thin_ts_to_plot: int = 20
     """
     Thinning to apply to the timeseries to plot
 
     In other words, only plot every ``thin_ts_to_plot`` runs on the timeseries
@@ -319,14 +331,97 @@
         convergence
             Received from :func:`scipy.optimize.differential_evolution`
             on callback. We are not sure what this does is or what it is used
             for.
         """
         self.update_plots()
 
+    @classmethod
+    def from_autogenerated_figure(  # pylint:disable=too-many-arguments
+        cls,
+        cost_key: str,
+        params: Tuple[str],
+        convert_scmrun_to_plot_dict: ScmRunToDictConverter,
+        target: scmdata.run.BaseScmRun,
+        store: OptResStore,
+        kwargs_create_mosaic: Optional[Dict[str, Any]] = None,
+        kwargs_get_fig_axes_holder: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
+    ) -> OptPlotter:
+        """
+        Create plotter with automatic figure generation
+
+        Parameters
+        ----------
+        cost_key
+            Name to use for the cost axis
+
+        params
+            Parameters that are being optimised
+
+            This is used to generate the plotting axes. It must also match the
+            order in which the parameters are handled by the optimiser i.e. it
+            is used to translate the unlabeled array of parameter values onto
+            the desired axes.
+
+        convert_scmrun_to_plot_dict
+            Callable which converts :obj:`scmdata.run.BaseScmRun` into a
+            dictionary
+
+        target
+            Target to which we are optimising
+
+        store
+            Optimisation result store
+
+        kwargs_create_mosaic
+            Passed to :func:`get_optimisation_mosaic`
+
+        kwargs_get_fig_axes_holder
+            Passed to :func:`get_fig_axes_holder_from_mosaic`
+
+        **kwargs
+            Passed to the initialiser of :obj:`OptPlotter`
+
+        Returns
+        -------
+            :obj:`OptPlotter` initialised with generated figure, axes and
+            holder
+        """
+        if kwargs_create_mosaic is None:
+            kwargs_create_mosaic = {}
+
+        if kwargs_get_fig_axes_holder is None:
+            kwargs_get_fig_axes_holder = {}
+
+        timeseries_axes = tuple(convert_scmrun_to_plot_dict(target).keys())
+        mosaic = get_optimisation_mosaic(
+            cost_key=cost_key,
+            params=params,
+            timeseries=timeseries_axes,
+            **kwargs_create_mosaic,
+        )
+
+        fig, axes, holder = get_fig_axes_holder_from_mosaic(
+            mosaic, **kwargs_get_fig_axes_holder
+        )
+
+        return cls(
+            holder=holder,
+            fig=fig,
+            axes=axes,
+            cost_key=cost_key,
+            parameters=params,
+            timeseries_axes=timeseries_axes,
+            convert_scmrun_to_plot_dict=convert_scmrun_to_plot_dict,
+            target=target,
+            store=store,
+            **kwargs,
+        )
+
     def update_plots(self) -> None:
         """
         Update all the plots
         """
         costs, para_vals, res = self.store.get_costs_labelled_xsamples_res()
 
         # check if anything to plot
@@ -777,15 +872,15 @@
     actually be called. If provided, it also keeps track of the number of
     model calls via a progress bar.
     """
 
     real_callback: SupportsScipyOptCallback
     """Callback to be called if a sufficient number of runs have been done"""
 
-    store: openscm_calibration.store.OptResStore
+    store: OptResStore
     """Optimisation result store"""
 
     last_callback_val: int = 0
     """Number of model calls at last callback"""
 
     update_every: int = 50
     """Update the plots every X calls to the model"""
@@ -911,7 +1006,74 @@
         run_converted = run.convert_unit(model_unit)
 
         tmp.append(run_converted)
 
     out = scmdata.run_append(tmp)
 
     return out
+
+
+def get_optimisation_mosaic(  # pylint:disable=too-many-arguments
+    cost_key: str,
+    params: Tuple[str, ...],
+    timeseries: Tuple[str, ...],
+    cost_col_relwidth: int = 1,
+    n_parameters_per_row: int = 1,
+    n_timeseries_per_row: int = 1,
+) -> List[List[str]]:
+    """
+    Get optimisation mosaic
+
+    This gives back the grid of axes to use for plotting. It can be understood
+    by matplotlib but in theory could be used with any tool that understands
+    such mosaics/grids.
+
+    Parameters
+    ----------
+    cost_key
+        Name to use for the cost axis
+
+    params
+        Parameters axes to generate
+
+    timeseries
+        Timeseries axes to generate
+
+    cost_col_relwidth
+        Width of the cost axis, relative to the width of each parameter axis
+
+    n_parameters_per_row
+        Number of parameters to plot per row (as many rows as are needed to
+        plot all the parameters are created)
+
+    n_timeseries_per_row
+        Number of timeseries to plot per row (as many rows as are needed to
+        plot all the timeseries are created)
+
+    Returns
+    -------
+        Mosaic
+    """
+    parameters_wrapped = more_itertools.grouper(
+        params, n_parameters_per_row, fillvalue="."
+    )
+    timeseries_axes_wrapped = more_itertools.grouper(
+        timeseries, n_timeseries_per_row, fillvalue="."
+    )
+
+    n_top_half_cols = cost_col_relwidth + n_parameters_per_row
+    n_bottom_half_cols = n_timeseries_per_row
+
+    top_half_row_repeats = [
+        ([cost_key] * cost_col_relwidth + list(parameter_row), n_bottom_half_cols)
+        for parameter_row in parameters_wrapped
+    ]
+    bottom_half_row_repeats = [
+        (row, n_top_half_cols) for row in timeseries_axes_wrapped
+    ]
+
+    mosaic = [
+        list(more_itertools.repeat_each(row, n_repeats))
+        for row, n_repeats in top_half_row_repeats + bottom_half_row_repeats
+    ]
+
+    return mosaic
```

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/scmdata_utils.py` & `openscm_calibration-0.5.0/src/openscm_calibration/scmdata_utils.py`

 * *Files identical despite different names*

### Comparing `openscm_calibration-0.3.0/src/openscm_calibration/store.py` & `openscm_calibration-0.5.0/src/openscm_calibration/store.py`

 * *Files identical despite different names*

