# Comparing `tmp/noloadj-1.2.5.tar.gz` & `tmp/noloadj-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\noloadj-1.2.5.tar", last modified: Sun Mar 19 16:58:26 2023, max compression
+gzip compressed data, was "dist\noloadj-1.2.6.tar", last modified: Tue Apr 25 13:33:14 2023, max compression
```

## Comparing `noloadj-1.2.5.tar` & `noloadj-1.2.6.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/
--rw-rw-rw-   0        0        0      257 2022-12-18 18:14:06.000000 noloadj-1.2.5/AUTHORS.md
--rw-rw-rw-   0        0        0     2749 2022-12-18 18:14:06.000000 noloadj-1.2.5/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11550 2022-12-18 18:14:06.000000 noloadj-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      166 2022-12-18 18:14:06.000000 noloadj-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5324 2023-03-19 16:58:26.000000 noloadj-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4773 2023-01-31 12:52:24.000000 noloadj-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:25.000000 noloadj-1.2.5/docs/
--rw-rw-rw-   0        0        0      203 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/NoLOAD_Jax_description.rst
--rw-rw-rw-   0        0        0      379 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/about_NoLOAD_Jax.rst
--rw-rw-rw-   0        0        0    30996 2023-01-31 12:52:24.000000 noloadj-1.2.5/docs/how_to_NoLOAD_Jax.rst
--rw-rw-rw-   0        0        0     1639 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/index.rst
--rw-rw-rw-   0        0        0     9321 2023-01-31 12:52:24.000000 noloadj-1.2.5/docs/installation_requirements.rst
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:25.000000 noloadj-1.2.5/docs/new_features/
--rw-rw-rw-   0        0        0      814 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.0.1.rst
--rw-rw-rw-   0        0        0      250 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.0.2.rst
--rw-rw-rw-   0        0        0      469 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.0.rst
--rw-rw-rw-   0        0        0      296 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.1.rst
--rw-rw-rw-   0        0        0      271 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.2.rst
--rw-rw-rw-   0        0        0      359 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.3.rst
--rw-rw-rw-   0        0        0      435 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.41.rst
--rw-rw-rw-   0        0        0      879 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.5.rst
--rw-rw-rw-   0        0        0      233 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.6.rst
--rw-rw-rw-   0        0        0      469 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.7.rst
--rw-rw-rw-   0        0        0      411 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.8.rst
--rw-rw-rw-   0        0        0      369 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.1.9.rst
--rw-rw-rw-   0        0        0      615 2022-12-18 18:14:06.000000 noloadj-1.2.5/docs/new_features/v1.2.0.rst
--rw-rw-rw-   0        0        0      415 2023-01-02 22:40:32.000000 noloadj-1.2.5/docs/new_features/v1.2.1.rst
--rw-rw-rw-   0        0        0      257 2023-01-31 12:52:24.000000 noloadj-1.2.5/docs/new_features/v1.2.15.rst
--rw-rw-rw-   0        0        0      267 2023-01-31 12:52:24.000000 noloadj-1.2.5/docs/new_features/v1.2.2.rst
--rw-rw-rw-   0        0        0      349 2023-01-31 12:52:24.000000 noloadj-1.2.5/docs/new_features/v1.2.3.rst
--rw-rw-rw-   0        0        0      379 2023-03-10 22:25:29.000000 noloadj-1.2.5/docs/new_features/v1.2.4.rst
--rw-rw-rw-   0        0        0      380 2023-03-19 16:53:06.000000 noloadj-1.2.5/docs/new_features/v1.2.5.rst
--rw-rw-rw-   0        0        0      781 2023-03-19 16:53:06.000000 noloadj-1.2.5/docs/new_functionnalities.rst
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj/
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj/ODE/
--rw-rw-rw-   0        0        0     9102 2023-03-19 16:53:06.000000 noloadj-1.2.5/noloadj/ODE/ode45.py
--rw-rw-rw-   0        0        0    14583 2023-03-19 16:53:06.000000 noloadj-1.2.5/noloadj/ODE/ode45_extract.py
--rw-rw-rw-   0        0        0     9058 2023-03-19 16:53:06.000000 noloadj-1.2.5/noloadj/ODE/ode45_extract_fft.py
--rw-rw-rw-   0        0        0     4007 2023-03-19 16:53:06.000000 noloadj-1.2.5/noloadj/ODE/ode45_fft.py
--rw-rw-rw-   0        0        0     2612 2023-03-10 22:25:29.000000 noloadj-1.2.5/noloadj/ODE/ode_tools.py
--rw-rw-rw-   0        0        0       88 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj/analyse/
--rw-rw-rw-   0        0        0     4829 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/analyse/simulation.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj/gui/
--rw-rw-rw-   0        0        0     8873 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/gui/plotIterations.py
--rw-rw-rw-   0        0        0     6664 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/gui/plotPareto.py
--rw-rw-rw-   0        0        0     1671 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/gui/testOverLabels.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj/optimization/
--rw-rw-rw-   0        0        0     3042 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/optimization/ExportToXML.py
--rw-rw-rw-   0        0        0     6001 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/optimization/Tools.py
--rw-rw-rw-   0        0        0       88 2022-12-19 16:40:36.000000 noloadj-1.2.5/noloadj/optimization/__init__.py
--rw-rw-rw-   0        0        0     3278 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/optimization/iterationHandler.py
--rw-rw-rw-   0        0        0    12053 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/optimization/multiobjective.py
--rw-rw-rw-   0        0        0    12830 2023-03-10 22:25:29.000000 noloadj-1.2.5/noloadj/optimization/optimProblem.py
--rw-rw-rw-   0        0        0     5005 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/optimization/paretoTools.py
--rw-rw-rw-   0        0        0     7437 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/optimization/specifications.py
--rw-rw-rw-   0        0        0    36269 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/optimization/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj/tutorial/
--rw-rw-rw-   0        0        0     2043 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/tutorial/01-UnconstrainedMonoObjective.py
--rw-rw-rw-   0        0        0     2015 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/tutorial/02-ConstrainedMonoObjective.py
--rw-rw-rw-   0        0        0     2404 2023-01-31 12:52:24.000000 noloadj-1.2.5/noloadj/tutorial/03-ConstrainedMultiObjective.py
--rw-rw-rw-   0        0        0     3885 2023-03-10 22:28:52.000000 noloadj-1.2.5/noloadj/tutorial/04-ConstrainedMonoObjective2.py
--rw-rw-rw-   0        0        0     1097 2022-12-18 18:14:06.000000 noloadj-1.2.5/noloadj/tutorial/plotTools.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:58:26.000000 noloadj-1.2.5/noloadj.egg-info/
--rw-rw-rw-   0        0        0     5324 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-19 16:58:25.000000 noloadj-1.2.5/noloadj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 16:58:26.000000 noloadj-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1625 2023-03-19 16:53:06.000000 noloadj-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.529621 noloadj-1.2.6/
+-rw-rw-rw-   0        0        0      257 2021-12-02 13:17:49.000000 noloadj-1.2.6/AUTHORS.md
+-rw-rw-rw-   0        0        0     2749 2021-12-02 13:17:49.000000 noloadj-1.2.6/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11550 2021-12-02 13:17:49.000000 noloadj-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      166 2021-12-02 13:17:49.000000 noloadj-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5324 2023-04-25 13:33:14.529621 noloadj-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4773 2023-01-18 15:18:00.000000 noloadj-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.398140 noloadj-1.2.6/docs/
+-rw-rw-rw-   0        0        0      203 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/NoLOAD_Jax_description.rst
+-rw-rw-rw-   0        0        0      379 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/about_NoLOAD_Jax.rst
+-rw-rw-rw-   0        0        0    30996 2023-01-19 15:23:24.000000 noloadj-1.2.6/docs/how_to_NoLOAD_Jax.rst
+-rw-rw-rw-   0        0        0     1639 2022-09-26 12:06:06.000000 noloadj-1.2.6/docs/index.rst
+-rw-rw-rw-   0        0        0     9321 2023-01-18 15:19:37.000000 noloadj-1.2.6/docs/installation_requirements.rst
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/docs/new_features/
+-rw-rw-rw-   0        0        0      814 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/new_features/v1.0.1.rst
+-rw-rw-rw-   0        0        0      250 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/new_features/v1.0.2.rst
+-rw-rw-rw-   0        0        0      469 2021-12-07 14:23:29.000000 noloadj-1.2.6/docs/new_features/v1.1.0.rst
+-rw-rw-rw-   0        0        0      296 2022-03-28 19:16:25.000000 noloadj-1.2.6/docs/new_features/v1.1.1.rst
+-rw-rw-rw-   0        0        0      271 2022-06-22 12:46:39.000000 noloadj-1.2.6/docs/new_features/v1.1.2.rst
+-rw-rw-rw-   0        0        0      359 2022-07-04 14:52:17.000000 noloadj-1.2.6/docs/new_features/v1.1.3.rst
+-rw-rw-rw-   0        0        0      435 2022-07-31 13:27:41.000000 noloadj-1.2.6/docs/new_features/v1.1.41.rst
+-rw-rw-rw-   0        0        0      879 2022-09-15 14:23:43.000000 noloadj-1.2.6/docs/new_features/v1.1.5.rst
+-rw-rw-rw-   0        0        0      233 2022-09-16 13:40:40.000000 noloadj-1.2.6/docs/new_features/v1.1.6.rst
+-rw-rw-rw-   0        0        0      469 2022-09-26 12:42:53.000000 noloadj-1.2.6/docs/new_features/v1.1.7.rst
+-rw-rw-rw-   0        0        0      411 2022-10-10 13:59:06.000000 noloadj-1.2.6/docs/new_features/v1.1.8.rst
+-rw-rw-rw-   0        0        0      369 2022-11-10 08:54:10.000000 noloadj-1.2.6/docs/new_features/v1.1.9.rst
+-rw-rw-rw-   0        0        0      615 2022-11-28 16:05:49.000000 noloadj-1.2.6/docs/new_features/v1.2.0.rst
+-rw-rw-rw-   0        0        0      415 2023-01-06 10:14:29.000000 noloadj-1.2.6/docs/new_features/v1.2.1.rst
+-rw-rw-rw-   0        0        0      257 2023-01-10 10:26:06.000000 noloadj-1.2.6/docs/new_features/v1.2.15.rst
+-rw-rw-rw-   0        0        0      267 2023-01-11 14:31:56.000000 noloadj-1.2.6/docs/new_features/v1.2.2.rst
+-rw-rw-rw-   0        0        0      349 2023-01-26 15:46:21.000000 noloadj-1.2.6/docs/new_features/v1.2.3.rst
+-rw-rw-rw-   0        0        0      379 2023-03-03 15:08:46.000000 noloadj-1.2.6/docs/new_features/v1.2.4.rst
+-rw-rw-rw-   0        0        0      380 2023-03-17 15:42:28.000000 noloadj-1.2.6/docs/new_features/v1.2.5.rst
+-rw-rw-rw-   0        0        0      581 2023-04-25 12:44:12.000000 noloadj-1.2.6/docs/new_features/v1.2.6.rst
+-rw-rw-rw-   0        0        0      805 2023-04-25 12:44:12.000000 noloadj-1.2.6/docs/new_functionnalities.rst
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/noloadj/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/ODE/
+-rw-rw-rw-   0        0        0    10618 2023-04-25 12:36:26.000000 noloadj-1.2.6/noloadj/ODE/ode45.py
+-rw-rw-rw-   0        0        0    15882 2023-04-21 14:33:22.000000 noloadj-1.2.6/noloadj/ODE/ode45_extract.py
+-rw-rw-rw-   0        0        0     4896 2023-04-25 12:42:14.000000 noloadj-1.2.6/noloadj/ODE/ode45_extract_fft.py
+-rw-rw-rw-   0        0        0     1889 2023-04-25 12:38:23.000000 noloadj-1.2.6/noloadj/ODE/ode45_fft.py
+-rw-rw-rw-   0        0        0     2794 2023-04-17 08:44:05.000000 noloadj-1.2.6/noloadj/ODE/ode_tools.py
+-rw-rw-rw-   0        0        0       88 2022-11-14 15:31:43.000000 noloadj-1.2.6/noloadj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/analyse/
+-rw-rw-rw-   0        0        0     4829 2023-01-19 13:47:35.000000 noloadj-1.2.6/noloadj/analyse/simulation.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/gui/
+-rw-rw-rw-   0        0        0     8873 2022-09-26 10:08:50.000000 noloadj-1.2.6/noloadj/gui/plotIterations.py
+-rw-rw-rw-   0        0        0     6664 2022-09-15 13:49:58.000000 noloadj-1.2.6/noloadj/gui/plotPareto.py
+-rw-rw-rw-   0        0        0     1671 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/gui/testOverLabels.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.514000 noloadj-1.2.6/noloadj/optimization/
+-rw-rw-rw-   0        0        0     3042 2021-12-07 13:44:04.000000 noloadj-1.2.6/noloadj/optimization/ExportToXML.py
+-rw-rw-rw-   0        0        0     6001 2023-01-13 10:49:31.000000 noloadj-1.2.6/noloadj/optimization/Tools.py
+-rw-rw-rw-   0        0        0       88 2023-02-20 11:35:20.000000 noloadj-1.2.6/noloadj/optimization/__init__.py
+-rw-rw-rw-   0        0        0     3278 2022-07-29 13:59:40.000000 noloadj-1.2.6/noloadj/optimization/iterationHandler.py
+-rw-rw-rw-   0        0        0    12053 2023-01-26 15:54:37.000000 noloadj-1.2.6/noloadj/optimization/multiobjective.py
+-rw-rw-rw-   0        0        0    12830 2023-02-24 13:24:55.000000 noloadj-1.2.6/noloadj/optimization/optimProblem.py
+-rw-rw-rw-   0        0        0     5005 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/optimization/paretoTools.py
+-rw-rw-rw-   0        0        0     7437 2023-01-19 13:13:53.000000 noloadj-1.2.6/noloadj/optimization/specifications.py
+-rw-rw-rw-   0        0        0    36269 2023-01-26 15:34:33.000000 noloadj-1.2.6/noloadj/optimization/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.514000 noloadj-1.2.6/noloadj/tutorial/
+-rw-rw-rw-   0        0        0     2043 2023-01-19 13:08:31.000000 noloadj-1.2.6/noloadj/tutorial/01-UnconstrainedMonoObjective.py
+-rw-rw-rw-   0        0        0     2015 2023-01-19 13:14:21.000000 noloadj-1.2.6/noloadj/tutorial/02-ConstrainedMonoObjective.py
+-rw-rw-rw-   0        0        0     2404 2023-01-19 13:10:12.000000 noloadj-1.2.6/noloadj/tutorial/03-ConstrainedMultiObjective.py
+-rw-rw-rw-   0        0        0     3885 2023-01-18 15:05:58.000000 noloadj-1.2.6/noloadj/tutorial/04-ConstrainedMonoObjective2.py
+-rw-rw-rw-   0        0        0     1097 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/tutorial/plotTools.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/noloadj.egg-info/
+-rw-rw-rw-   0        0        0     5324 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1784 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:33:14.529621 noloadj-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-04-17 14:46:08.000000 noloadj-1.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `noloadj-1.2.5/CONTRIBUTING.md` & `noloadj-1.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/LICENSE` & `noloadj-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/PKG-INFO` & `noloadj-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noloadj
-Version: 1.2.5
+Version: 1.2.6
 Summary: solving constrained optimization problem for the design of engineering systems
 Author: B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT
 Author-email: benoit.delinchant@G2ELab.grenoble-inp.fr
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `noloadj-1.2.5/README.md` & `noloadj-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/how_to_NoLOAD_Jax.rst` & `noloadj-1.2.6/docs/how_to_NoLOAD_Jax.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/index.rst` & `noloadj-1.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/installation_requirements.rst` & `noloadj-1.2.6/docs/installation_requirements.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/new_features/v1.0.1.rst` & `noloadj-1.2.6/docs/new_features/v1.0.1.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/new_features/v1.1.5.rst` & `noloadj-1.2.6/docs/new_features/v1.1.5.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/new_features/v1.2.0.rst` & `noloadj-1.2.6/docs/new_features/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/docs/new_functionnalities.rst` & `noloadj-1.2.6/docs/new_functionnalities.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 What's new in the latest versions
 =================================
 
-The new version of NoLOAD_Jax v1.2.5 is available!
-The release is from 19th of March 2023.
+The new version of NoLOAD_Jax v1.2.6 is available!
+The release is from 25th of April 2023.
 
 .. toctree::
    :maxdepth: 2
 
-   new_features/v1.2.5
+   new_features/v1.2.6
 
 
 Information about the latest versions
 -------------------------------------
 
 .. toctree::
    :maxdepth: 1
 
    new_features/v1.2.4
+   new_features/v1.2.4
    new_features/v1.2.3
    new_features/v1.2.2
    new_features/v1.2.15
    new_features/v1.2.1
    new_features/v1.2.0
    new_features/v1.1.9
    new_features/v1.1.8
```

### Comparing `noloadj-1.2.5/noloadj/ODE/ode45.py` & `noloadj-1.2.6/noloadj/ODE/ode45.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,226 +1,251 @@
 import jax.numpy as np
 from jax.lax import *
 from jax import custom_jvp,jvp,interpreters
 from functools import partial
 
-def odeint45(f,y0,t,*args,T=0.,h0=1e-5,tol=1.48e-8):
-    return _odeint45(f,h0,tol,y0,t,T,*args)
+def odeint45(f,x0,t,*P,T=0.,h0=1e-5,tol=1.48e-8):
+    return _odeint45(f,h0,tol,x0,t,T,*P)
 
 
-def rk_step(y_prev, t_prev, h,f,*args):
-    k1=f(y_prev, t_prev,*args)
-    k2 = f(y_prev + h*0.2 * k1, t_prev + 0.2 * h,*args)
-    k3 = f(y_prev + h*(3 * k1 + 9 * k2) / 40,t_prev + 3 * h / 10,*args)
-    k4 = f(y_prev + h*(44 * k1 / 45 - 56 * k2 / 15 + 32 * k3 / 9),t_prev +
-           4 * h / 5,*args)
-    k5 = f(y_prev + h*(19372 * k1 / 6561 - 25360 * k2 / 2187 +
+def rk_step(x_prev, t_prev, h,f,*P):
+    k1=f(x_prev, t_prev,*P)
+    k2 = f(x_prev + h*0.2 * k1, t_prev + 0.2 * h,*P)
+    k3 = f(x_prev + h*(3 * k1 + 9 * k2) / 40,t_prev + 3 * h / 10,*P)
+    k4 = f(x_prev + h*(44 * k1 / 45 - 56 * k2 / 15 + 32 * k3 / 9),t_prev +
+           4 * h / 5,*P)
+    k5 = f(x_prev + h*(19372 * k1 / 6561 - 25360 * k2 / 2187 +
             64448 * k3 / 6561- 212 * k4 / 729),
-           t_prev + 8 * h / 9,*args)
-    k6 = f(y_prev + h*(9017 * k1 / 3168 - 355 * k2 / 33 + 46732 * k3 / 5247+
-            49 * k4 / 176 - 5103 * k5 / 18656),t_prev + h,*args)
-    k7 = f(y_prev + h*(35 * k1 / 384 + 500 * k3 / 1113 +
-            125 * k4 / 192 -2187 * k5 / 6784 + 11 * k6 / 84),t_prev + h,*args)
+           t_prev + 8 * h / 9,*P)
+    k6 = f(x_prev + h*(9017 * k1 / 3168 - 355 * k2 / 33 + 46732 * k3 / 5247+
+            49 * k4 / 176 - 5103 * k5 / 18656),t_prev + h,*P)
+    k7 = f(x_prev + h*(35 * k1 / 384 + 500 * k3 / 1113 +
+            125 * k4 / 192 -2187 * k5 / 6784 + 11 * k6 / 84),t_prev + h,*P)
 
-    y = y_prev + h *(35 * k1 / 384 + 500 * k3 / 1113 + 125 * k4 / 192
+    x = x_prev + h *(35 * k1 / 384 + 500 * k3 / 1113 + 125 * k4 / 192
              -2187 * k5 / 6784 + 11 * k6 / 84)
-    yest = y_prev + h *(5179 * k1 / 57600 + 7571* k3 / 16695 + 393 * k4 /640
+    xest = x_prev + h *(5179 * k1 / 57600 + 7571* k3 / 16695 + 393 * k4 /640
             - 92097 * k5 / 339200 + 187 * k6 / 2100 + k7 / 40)
     t_now = t_prev + h
-    return y, yest, t_now
+    return x, xest, t_now
 
 
-def optimal_step(y,yest,h,tol,errcon=1.89e-4):
-    est=np.linalg.norm(y-yest)
+def optimal_step(x,xest,h,tol,errcon=1.89e-4):
+    est=np.linalg.norm(x-xest)
     R = (est+1e-16) / h
     err_ratio = R / tol
     delta = (2*err_ratio)**(-0.2)
     h=np.where(est>=errcon,h*delta,1.0*h)
     return h
 
-def prediction(t,tprev,val_seuil,output,outputprev):
-    return t+(t-tprev)*(val_seuil-output)/(output-outputprev)
 
 def interpolation(state):
-    y,h,y_prev,t_prev,t_now,output,outputprev=state
-    tchoc=(-t_prev*output+t_now*outputprev)/(outputprev-output)
+    x,h,x_prev,t_prev,t_now,y_prev,y,var_seuil,var_seuil_prev=state
+    tchoc=(-t_prev*var_seuil+t_now*var_seuil_prev)/(var_seuil_prev-var_seuil)
     h=tchoc-t_prev
+    xchoc=(x_prev-x)*tchoc/(t_prev-t_now)+(t_prev*x-t_now*x_prev)/(t_prev-t_now)
     ychoc=(y_prev-y)*tchoc/(t_prev-t_now)+(t_prev*y-t_now*y_prev)/(t_prev-t_now)
-    return ychoc,h,y_prev,t_prev,tchoc,output,outputprev
-
-def GetTimeofNextVarHit(t,tprev,f,y,y_prev,tevent):
-    for element in f.zero_crossing:
-        state,var_name,seuil=element
-        ind=f.names.index(var_name)
-        if isinstance(seuil,float):
-            val_seuil=seuil
-        elif seuil[0]=='-':
-            val_seuil = -y[f.names.index(seuil[1::])]
-        else:
-            val_seuil=y[f.names.index(seuil)]
-        temp=prediction(t,tprev,val_seuil,y[ind],y_prev[ind])
-        tevent=cond(temp>t,lambda tevent:np.minimum(tevent,temp),
-                    lambda tevent:tevent,tevent)
-    return tevent+1e-12
-
-def init_etat(f,y,inew):
-    for element in f.zero_crossing:
-        new_state,var_name,seuil=element
-        ind=f.names.index(var_name)
-        if isinstance(seuil,float):
-            y=y.at[ind].set(np.where(inew==new_state,seuil,y[ind]))
-        elif seuil[0]=='-':
-            y=y.at[ind].set(np.where(inew==new_state,
-                        -y[f.names.index(seuil[1::])],y[ind]))
-        else:
-            y=y.at[ind].set(np.where(inew==new_state,y[f.names.index(seuil)],
-                                   y[ind]))
-    return y
+    return xchoc,h,x_prev,t_prev,tchoc,y_prev,ychoc,var_seuil,var_seuil_prev
 
+def interp_state_chgt(x_prev,y_prev,yb,t_prev,x,y,t_now,f,i,h,cnew):
+    ind=np.where(np.array_equiv(y,yb),-1,np.argmax(np.abs(y-yb)))
+    val_seuil=yb[ind]
+    condition = np.bitwise_and(np.sign(x[ind]-val_seuil)!=np.sign(
+            x_prev[ind]-val_seuil),np.not_equal(ind,-1))
+    condition=np.bitwise_and(condition,np.bitwise_not(np.allclose(
+            x_prev[ind]-val_seuil,0.)))
+    x,h,_,_,t_now,_,y,_,_=cond(condition,interpolation,
+                lambda state:state,(x,h,x_prev,t_prev,t_now,y_prev,y,
+                                    x[ind]-val_seuil,x_prev[ind]-val_seuil))
+    if hasattr(f,'commande'):
+        _,x,y=f.update(x,y,t_now,i,cnew)
+    else:
+        _,x,y=f.update(x,y,t_now,i)
+    return x,y,h,t_now
 
-def next_step_simulation(y_prev,t_prev,i,h,f,tol,h0,T,*args):
-    if hasattr(f,'etat_actuel'):
-        f.etat_actuel=i
-    y,yest,t_now=rk_step(y_prev,t_prev,h,f.derivative,*args)
-    hopt=0.
-    if hasattr(f,'etat_actuel'):
+def next_step_simulation(x_prev,t_prev,y_prev,i,c,h,f,tol,h0,T,*P):
+    if hasattr(f,'etat'):
+        f.etat=i
+    x,xest,t_now=rk_step(x_prev,t_prev,h,f.derivative,*P)
+    if hasattr(f,'computeotherX'):
+        x=f.computeotherX(x,t_now,*P)
+        xest=f.computeotherX(xest,t_now,*P)
+    y=f.output(x,t_now,*P)
+    hopt,cnew,tpdi=0.,0,0.
+    if hasattr(f,'etat'):
         if hasattr(f,'commande'):
-            tpdi=f.commande(t_now,T)
+            tpdi,cnew=f.commande(t_now,T)
+            inew,_,yb=f.update(x,y,t_now,i,cnew)
+            x,y,h,t_now=cond(inew!=i,lambda state:interp_state_chgt(x_prev,y_prev,
+              yb,t_prev,x,y,t_now,f,i,h,cnew),lambda state:state,(x,y,h,t_now))
         else:
-            tpdi=100.
-        inew=np.argmax(np.array(f.cond_etat(y,t_now)))
-        y=cond(inew!=i,lambda y:init_etat(f,y,inew),lambda y:y,y)
-        tevent=GetTimeofNextVarHit(t_now,t_prev,f,y,y_prev,tpdi)
-        hopt = optimal_step(y,yest, h, tol)
-        hopt=np.minimum(tevent-t_now,hopt)
+            inew,_,yb=f.update(x,y,t_now,i)
+            x,y,h,t_now=cond(inew!=i,lambda state:interp_state_chgt(x_prev,y_prev,
+             yb,t_prev,x,y,t_now,f,i,h,0),lambda state:state,(x,y,h,t_now))
+
+        y=f.output(x,t_now,*P)
+        hopt = optimal_step(x,xest, h, tol)
+        if hasattr(f,'commande'):
+            hopt=np.minimum(tpdi-t_now,hopt)
         hopt=np.where(inew!=i,h0,hopt) # pour accelerer code
-        hopt=np.where(hopt==0.,h0,hopt)
     else:
         inew=i
+        cnew=c
     if hasattr(f,'event'):
         for e in f.event:
             name,signe_str,seuil,name2,chgt_etat=e
-            output,outputprev=get_indice(f.names,y,[name]),\
-                            get_indice(f.names,y_prev,[name])
+            var_seuil,var_seuil_prev=get_indice(f.xnames,x,[name]),\
+                            get_indice(f.xnames,x_prev,[name])
             signe=np.where(signe_str=='<',-1,1)
-            condition = np.bitwise_and(np.sign(output-seuil)==signe,
-                       np.bitwise_not(np.allclose(outputprev-seuil,0.)))
-            hopt = optimal_step(y, yest, h, tol)
-            y,h,_,_,t_now,_,_=cond(condition,interpolation,
-                lambda state:state,(y,h,y_prev,t_prev,t_now,
-                                    output-seuil,outputprev-seuil))
-            yevent=cond(condition,chgt_etat,lambda state:state,
-                                        get_indice(f.names,y,[name2]))
-            y=y.at[f.names.index(name2)].set(yevent)
-    elif not hasattr(f,'event') and not hasattr(f,'etat_actuel'):
-        hopt = optimal_step(y, yest, h, tol)
-    return y,t_now,hopt,inew
+            condition = np.bitwise_and(np.sign(var_seuil-seuil)==signe,
+                       np.bitwise_not(np.allclose(var_seuil_prev-seuil,0.)))
+            hopt = optimal_step(x, xest, h, tol)
+            x,h,_,_,t_now,_,y,_,_=cond(condition,interpolation,
+                lambda state:state,(x,h,x_prev,t_prev,t_now,y_prev,y,
+                                    var_seuil-seuil,var_seuil_prev-seuil))
+            xevent=cond(condition,chgt_etat,lambda state:state,
+                                        get_indice(f.xnames,x,[name2]))
+            x=x.at[f.xnames.index(name2)].set(xevent)
+            y=f.output(x,t_now,*P)
+    elif not hasattr(f,'event') and not hasattr(f,'etat'):
+        hopt = optimal_step(x, xest, h, tol)
+    return x,t_now,y,hopt,inew,cnew
 
 @partial(custom_jvp,nondiff_argnums=(0,1,2))
-def _odeint45(f,h0,tol,y0,t,T,*args):
+def _odeint45(f,h0,tol,x0,t,T,*P):
 
     def scan_fun(state,t):
 
         def cond_fn(state):
-            _,_,y_prev,t_prev,h,_=state
+            _,_,_,x_prev,t_prev,_,h,_,_=state
             return (t_prev<t) & (h>0)
 
         def body_fn(state):
-            _,_,y_prev,t_prev,h,i=state
+            _,_,_,x_prev,t_prev,y_prev,h,i,c=state
 
-            y,t_now,hopt,inew=next_step_simulation(y_prev,t_prev,i,h,f,tol,h0,
-                                                   T,*args)
+            x,t_now,y,hopt,inew,cnew=next_step_simulation(x_prev,t_prev,y_prev,
+                                                    i,c,h,f,tol,h0,T,*P)
 
-            return y_prev,t_prev,y,t_now,hopt,inew
+            return x_prev,t_prev,y_prev,x,t_now,y,hopt,inew,cnew
 
-        y_prev,t_prev,y_now,t_now,h,i = while_loop(cond_fn, body_fn, state)
+        x_prev,t_prev,y_prev,x_now,t_now,y_now,h,i,c = while_loop(cond_fn,
+                                                                  body_fn,state)
         #interpolation lineaire
+        x=((x_prev-x_now)*t+t_prev*x_now-t_now*x_prev)/(t_prev-t_now)
         y=((y_prev-y_now)*t+t_prev*y_now-t_now*y_prev)/(t_prev-t_now)
-        return (y_prev,t_prev,y,t,h,i),y
+        return (x_prev,t_prev,y_prev,x,t,y,h,i,c),(x,y)
 
-    if hasattr(f,'etat_actuel'):
-        i0=f.etat_actuel
+    if hasattr(f,'etat'):
+        i0=f.etat
+        if hasattr(f,'commande'):
+            _,c0=f.commande(0.,T)
+        else:
+            c0=0
     else:
         i0=0
-    _,ys=scan(scan_fun,(y0,t[0],y0,t[0],h0,i0),t[1:])
+        c0=0
+    y0=f.output(x0,0.,*P)
+    vect,(xs,ys)=scan(scan_fun,(x0,t[0],y0,x0,t[0],y0,h0,i0,c0),t[1:])
+    if hasattr(f,'etat'):
+        f.etat=vect[7]
+    xs=np.transpose(np.concatenate((x0[None], xs)))
     ys=np.transpose(np.concatenate((y0[None], ys)))
-    return ys
+    return xs,ys
 
 
 @_odeint45.defjvp
 def _odeint45_jvp(f,h0,tol, primals, tangents):
-    y0, t,T, *args = primals
-    delta_y0, _,_, *delta_args = tangents
-    nargs = len(args)
-
-    def f_aug(y,delta_y, t, *args_and_delta_args):
-        args, delta_args = args_and_delta_args[:nargs], args_and_delta_args[nargs:]
-        primal_dot, tangent_dot = jvp(f.derivative, (y, t, *args), (delta_y,
-                                                    0., *delta_args))
+    x0, t,T, *P = primals
+    delta_x0, _,_, *dP = tangents
+    nPdP = len(P)
+
+    def f_aug(x,delta_x, t, *P_and_dP):
+        P, dP = P_and_dP[:nPdP], P_and_dP[nPdP:]
+        primal_dot, tangent_dot = jvp(f.derivative, (x, t, *P), (delta_x,
+                                                    0., *dP))
         return tangent_dot
 
-    ys,ys_dot = odeint45_etendu(f,f_aug,nargs,h0,tol, y0,delta_y0,
-                                        t,T, *args, *delta_args)
-    return ys,ys_dot
-
-def rk_step_der(y_prev, t_prev, delta_y_prev,h,f_aug,*args):
-    k1 = f_aug(y_prev, delta_y_prev, t_prev, *args)
-    k2 = f_aug(y_prev, delta_y_prev + h * 0.2 * k1,t_prev + 0.2 * h , *args)
-    k3 = f_aug(y_prev, delta_y_prev + h * (3 * k1 + 9 * k2) / 40,t_prev
-               +3 * h / 10, *args)
-    k4 = f_aug(y_prev,delta_y_prev + h*(44 * k1 / 45 - 56 * k2 /15+32*k3/9),
-               t_prev + 4 * h / 5,*args)
-    k5 = f_aug(y_prev, delta_y_prev + h * (19372 * k1 / 6561 - 25360*k2/2187
-                + 64448 * k3 / 6561 - 212 * k4 / 729),t_prev + 8 * h / 9, *args)
-    k6 = f_aug(y_prev,delta_y_prev+h*(9017 * k1 / 3168 -355 *k2/33 +46732*k3
-            / 5247 + 49 * k4 / 176 - 5103 * k5 / 18656),t_prev + h, *args)
-    delta_y = delta_y_prev + h *(35 * k1 / 384 + 500 * k3 / 1113 +
+    xs,xs_dot,ys,ys_dot = odeint45_etendu(f,f_aug,nPdP,h0,tol, x0,delta_x0,
+                                        t,T, *P, *dP)
+    return (xs,ys),(xs_dot,ys_dot)
+
+def rk_step_der(x_prev, t_prev, delta_x_prev,h,f_aug,*dP):
+    k1 = f_aug(x_prev, delta_x_prev, t_prev, *dP)
+    k2 = f_aug(x_prev, delta_x_prev + h * 0.2 * k1,t_prev + 0.2 * h , *dP)
+    k3 = f_aug(x_prev, delta_x_prev + h * (3 * k1 + 9 * k2) / 40,t_prev
+               +3 * h / 10, *dP)
+    k4 = f_aug(x_prev,delta_x_prev + h*(44 * k1 / 45 - 56 * k2 /15+32*k3/9),
+               t_prev + 4 * h / 5,*dP)
+    k5 = f_aug(x_prev, delta_x_prev + h * (19372 * k1 / 6561 - 25360*k2/2187
+                + 64448 * k3 / 6561 - 212 * k4 / 729),t_prev + 8 * h / 9, *dP)
+    k6 = f_aug(x_prev,delta_x_prev+h*(9017 * k1 / 3168 -355 *k2/33 +46732*k3
+            / 5247 + 49 * k4 / 176 - 5103 * k5 / 18656),t_prev + h, *dP)
+    delta_x = delta_x_prev + h *(35 * k1 / 384 + 500 * k3 / 1113 +
             125 * k4 / 192 - 2187 * k5 / 6784 + 11 * k6 / 84)
-    return delta_y
+    return delta_x
 
 
-def odeint45_etendu(f,f_aug,nargs,h0,tol,y0,delta_y0,t,T,*args):
-    args_red = args[:nargs]
+def odeint45_etendu(f,f_aug,nPdP,h0,tol,x0,delta_x0,t,T,*P_and_dP):
+    P,dP = P_and_dP[:nPdP],P_and_dP[nPdP:]
 
     def scan_fun(state, t):
 
         def cond_fn(state):
-            _,_,_,y_prev,delta_y_prev, t_prev, h,_ = state
+            _,_,_,_,_,x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,h,_,_=state
             return (t_prev < t) & (h > 0)
 
         def body_fn(state):
-            _,_,_,y_prev,delta_y_prev, t_prev, h,i = state
+            _,_,_,_,_,x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,h,i,c=state
 
-            y,t_now,hopt,inew=next_step_simulation(y_prev,t_prev,i,h,f,tol,h0,
-                                                   T,*args_red)
+            x,t_now,y,hopt,inew,cnew=next_step_simulation(x_prev,t_prev,y_prev,
+                                                        i,c,h,f,tol,h0,T,*P)
 
-            delta_y=rk_step_der(y_prev,t_prev,delta_y_prev,h,f_aug,*args)
+            delta_x=rk_step_der(x_prev,t_prev,delta_x_prev,h,f_aug,*P_and_dP)
+            if hasattr(f,'computeotherX'):
+                delta_x=jvp(f.computeotherX,(x,t_now,*P),(delta_x,0.,*dP))[1]
+            delta_y=jvp(f.output,(x,t_now,*P),(delta_x,0.,*dP))[1]
 
-            return y_prev,delta_y_prev,t_prev,y,delta_y,t_now,hopt,inew
+            return x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,x,delta_x,\
+                   y,delta_y,t_now,hopt,inew,cnew
 
-        y_prev,delta_y_prev,t_prev,y_now,delta_y_now,t_now,h,i = \
-              while_loop(cond_fn, body_fn, state)
+        x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,x_now,delta_x_now,y_now,\
+          delta_y_now,t_now,h,i,c = while_loop(cond_fn, body_fn, state)
         # interpolation lineaire
+        x = ((x_prev- x_now)*t+t_prev*x_now-t_now*x_prev)/(t_prev - t_now)
+        delta_x = ((delta_x_prev-delta_x_now)*t+t_prev*delta_x_now-t_now*
+                   delta_x_prev) / (t_prev - t_now)
         y = ((y_prev- y_now)*t+t_prev*y_now-t_now*y_prev)/(t_prev - t_now)
         delta_y = ((delta_y_prev-delta_y_now)*t+t_prev*delta_y_now-t_now*
                    delta_y_prev) / (t_prev - t_now)
-        return (y_prev,delta_y_prev,t_prev,y,delta_y, t, h,i), (y,delta_y)
+        return (x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,x,delta_x,y,
+                delta_y,t, h,i,c), (x,delta_x,y,delta_y)
 
     for element in f.__dict__.keys(): # pour eviter erreurs de code
         if isinstance(f.__dict__[element],interpreters.ad.JVPTracer):
             f.__dict__[element]=f.__dict__[element].primal
-    if hasattr(f,'etat_actuel'):
-        i0=f.etat_actuel
+    if hasattr(f,'etat'):
+        i0=f.etat
+        if hasattr(f,'commande'):
+            _,c0=f.commande(0.,T)
+        else:
+            c0=0
     else:
         i0=0
-    _,(ys,delta_ys)=scan(scan_fun,(y0,delta_y0,t[0],y0,delta_y0,t[0],h0,i0),
-                         t[1:])
+        c0=0
+    y0=f.output(x0,0.,*P)
+    delta_y0=jvp(f.output,(x0,0.,*P),(delta_x0,0.,*dP))[1]
+    vect,(xs,delta_xs,ys,delta_ys)=scan(scan_fun,(x0,delta_x0,y0,delta_y0,t[0],
+                            x0,delta_x0,y0,delta_y0,t[0],h0,i0,c0),t[1:])
+    if hasattr(f,'etat'):
+        f.etat=vect[11]
+    xs=np.transpose(np.concatenate((x0[None], xs)))
     ys=np.transpose(np.concatenate((y0[None], ys)))
-    delta_ys=np.transpose(np.concatenate((delta_y0[None], delta_ys)))
-    return ys,delta_ys
+    delta_xs=np.transpose(np.concatenate((delta_x0[None], delta_xs)))
+    delta_ys = np.transpose(np.concatenate((delta_y0[None], delta_ys)))
+    return xs,delta_xs,ys,delta_ys
 
 
 def get_indice(names,valeur,output):
     if len(output)==1:
         return valeur[names.index(output[0])]
     else:
         return (valeur[names.index(i)] for i in output)
```

### Comparing `noloadj-1.2.5/noloadj/ODE/ode45_extract.py` & `noloadj-1.2.6/noloadj/ODE/ode45_extract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,303 +1,369 @@
 import jax.numpy as np
 from jax.lax import *
 from jax import custom_jvp,jvp,interpreters
 from functools import partial
 from noloadj.ODE.ode45 import rk_step_der,interpolation,next_step_simulation
 
-def odeint45_extract(f,y0,*args,T=0.,h0=1e-5,tol=1.48e-8):
-    return _odeint45(f,h0,tol,y0,T,*args)
+def odeint45_extract(f,x0,*P,T=0.,h0=1e-5,tol=1.48e-8):
+    return _odeint45(f,h0,tol,x0,T,*P)
 
 
 @partial(custom_jvp,nondiff_argnums=(0,1,2))
-def _odeint45(f,h0,tol,y0,T,*args):
+def _odeint45(f,h0,tol,x0,T,*P):
     type,cond_stop=f.stop
 
     def cond_fn(state):
-        y_prev2,_,y_prev,t_prev,h,cstr,_=state
+        x_prev2,_,_,x_prev,t_prev,_,h,cstr,_,_=state
         if type=='seuil':
-            val,seuil=cond_stop(y_prev,f.names)
-            valp,_=cond_stop(y_prev2,f.names)
+            val,seuil=cond_stop(x_prev,f.xnames)
+            valp,_=cond_stop(x_prev2,f.xnames)
             return (h>0) & (np.sign(val-seuil)==np.sign(valp-seuil))
         else:
             return (h > 0) & cond_stop(t_prev,t_prev+h,cstr)
 
 
     def body_fn(state):
-        _,_,y_prev,t_prev,h,cstr,i=state
+        _,_,_,x_prev,t_prev,y_prev,h,cstr,i,c=state
 
-        y,t_now,hopt,inew=next_step_simulation(y_prev,t_prev,i,h,f,tol,h0,
-                                                   T,*args)
+        x,t_now,y,hopt,inew,cnew=next_step_simulation(x_prev,t_prev,y_prev,
+                                                    i,c,h,f,tol,h0,T,*P)
 
         if type=='seuil':
-            output,seuil=cond_stop(y,f.names)
-            outputprev,_=cond_stop(y_prev,f.names)
-            y,hopt,_,_,t_now,_,_=cond(
+            output,seuil=cond_stop(x,f.xnames)
+            outputprev,_=cond_stop(x_prev,f.xnames)
+            x,hopt,_,_,t_now,_,y,_,_=cond(
                 np.sign(output-seuil)!=np.sign(outputprev-seuil),interpolation,
-                lambda state:state,(y,hopt,y_prev,t_prev,t_now,output-seuil,
-                                    outputprev-seuil))
+                lambda state:state,(x,hopt,x_prev,t_prev,t_now,y_prev,y,
+                                    output-seuil,outputprev-seuil))
         elif isinstance(type,float):
+            x=np.where(t_now>type,((x_prev-x)*type+t_prev*x-t_now*x_prev)
+                       /(t_prev-t_now),x)
             y=np.where(t_now>type,((y_prev-y)*type+t_prev*y-t_now*y_prev)
                        /(t_prev-t_now),y)
             t_now,hopt=np.where(t_now>type,type,t_now),\
                        np.where(t_now>type,type-t_prev,hopt)
 
         if f.constraints!={}:
             for i in f.constraints.keys():
                 if isinstance(f.constraints[i][1],tuple):
-                    test_exp,(_,expression,_,_,_,_)=f.constraints[i]
+                    test_exp,(_,expression,_,_,_,_,name)=f.constraints[i]
                 else:
-                    (_,expression,_,_,_,_)=f.constraints[i]
+                    (_,expression,_,_,_,_,name)=f.constraints[i]
                     test_exp = lambda t: True
-                cstr[i]=np.where(test_exp(t_now),expression(t_prev,
-                            y_prev, t_now, y,cstr[i],h,T,f.names),cstr[i])
+                ind=f.xnames.index(name)
+                cstr[i]=np.where(test_exp(t_now),expression(t_prev,x_prev[ind],
+                            t_now,x[ind],cstr[i],h,T),cstr[i])
 
-        return y_prev,t_prev,y,t_now,hopt,cstr,inew
+        return x_prev,t_prev,y_prev,x,t_now,y,hopt,cstr,inew,cnew
 
     cstr=dict(zip(list(f.constraints.keys()),[0.]*len(f.constraints)))# INITIALISATION
     if f.constraints!={}:
         for i in f.constraints.keys():
             if isinstance(f.constraints[i][1],tuple):
-                test_exp,(init,_,_,_,_,_)=f.constraints[i]
+                test_exp,(init,_,_,_,_,_,name)=f.constraints[i]
             else:
-                (init,_,_,_,_,_)=f.constraints[i]
+                (init,_,_,_,_,_,name)=f.constraints[i]
                 test_exp=lambda t:True
-            cstr[i]=np.where(test_exp(0.),init(y0,0.,h0,f.names),cstr[i])
+            ind=f.xnames.index(name)
+            cstr[i]=np.where(test_exp(0.),init(x0[ind],0.,h0),cstr[i])
 
-    if hasattr(f,'etat_actuel'):
-        i0=f.etat_actuel
+    if hasattr(f,'etat'):
+        i0=f.etat
+        if hasattr(f,'commande'):
+            _,c0=f.commande(0.,T)
+        else:
+            c0=0
     else:
         i0=0
-    _,_,yf,ts,h,cstr,_=while_loop(cond_fn,body_fn,(y0,0.,y0,0.,h0,cstr,i0))
+        c0=0
+    y0=f.output(x0,0.,*P)
+    _,_,_,xf,ts,yf,h,cstr,ifinal,_=while_loop(cond_fn,body_fn,
+                                         (x0,0.,y0,x0,0.,y0,h0,cstr,i0,c0))
+    if hasattr(f,'etat'):
+        f.etat=ifinal
     if f.constraints!={}:
         for i in f.constraints.keys():
             if isinstance(f.constraints[i][1],tuple):
-                _,(_,_,fin,_,_,_)=f.constraints[i]
+                _,(_,_,fin,_,_,_,_)=f.constraints[i]
             else:
-                (_,_,fin,_,_,_)=f.constraints[i]
+                (_,_,fin,_,_,_,_)=f.constraints[i]
             cstr[i]=fin(ts,cstr[i],T)
 
-    return (ts,yf,cstr)
+    return (ts,xf,yf,cstr)
 
 
 @_odeint45.defjvp
 def _odeint45_jvp(f,h0,tol, primals, tangents):
-    y0,T, *args = primals
-    delta_y0,dT, *delta_args = tangents
-    nargs = len(args)
-
-    def f_aug(y,delta_y, t, *args_and_delta_args):
-        args, delta_args=args_and_delta_args[:nargs],args_and_delta_args[nargs:]
-        primal_dot, tangent_dot = jvp(f.derivative, (y, t, *args), (delta_y,
-                                                            0., *delta_args))
+    x0,T, *P = primals
+    delta_x0,dT, *dP = tangents
+    nPdP = len(P)
+
+    def f_aug(x,delta_x, t, *P_and_dP):
+        P, dP=P_and_dP[:nPdP],P_and_dP[nPdP:]
+        primal_dot, tangent_dot = jvp(f.derivative, (x, t, *P), (delta_x,
+                                                            0., *dP))
         return tangent_dot
 
-    yf,cstr,ts,dts,yf_dot,cstr_dot=odeint45_etendu(f,f_aug,nargs,h0,
-                tol, y0,delta_y0,T,dT, *args, *delta_args)
-    return (ts,yf,cstr),(dts,yf_dot,cstr_dot)
+    xf,yf,cstr,ts,dts,xf_dot,yf_dot,cstr_dot=odeint45_etendu(f,f_aug,nPdP,h0,
+                tol, x0,delta_x0,T,dT, *P, *dP)
+    return (ts,xf,yf,cstr),(dts,xf_dot,yf_dot,cstr_dot)
 
 
-def odeint45_etendu(f,f_aug,nargs,h0,tol,y0,delta_y0,T,dT,*args):
-    args_red = args[:nargs]
+def odeint45_etendu(f,f_aug,nPdP,h0,tol,x0,delta_x0,T,dT,*P_and_dP):
+    P,dP = P_and_dP[:nPdP],P_and_dP[nPdP:]
     type,cond_stop=f.stop
 
     def cond_fn(state):
-        y_prev2,_,_,y_prev,delta_y_prev, t_prev, h,cstr,_,_ = state
+        x_prev2,_,_,_,_,x_prev,delta_x_prev,_,_,t_prev, h,cstr,_,_,_ = state
         if type=='seuil':
-            val,seuil=cond_stop(y_prev,f.names)
-            valp,_ = cond_stop(y_prev2,f.names)
+            val,seuil=cond_stop(x_prev,f.xnames)
+            valp,_ = cond_stop(x_prev2,f.xnames)
             return (h>0) & (np.sign(val-seuil)==np.sign(valp-seuil))
         else:
             return (h > 0) & cond_stop(t_prev,t_prev+h,cstr)
 
 
     def body_fn(state):
-        _,_,_,y_prev,delta_y_prev, t_prev, h,cstr,delta_cstr,i = state
+        _,_,_,_,_,x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev, h,cstr,\
+                delta_cstr,i,c = state
 
-        y,t_now,hopt,inew=next_step_simulation(y_prev,t_prev,i,h,f,tol,h0,
-                                                   T,*args_red)
+        x,t_now,y,hopt,inew,cnew=next_step_simulation(x_prev,t_prev,y_prev,
+                                                        i,c,h,f,tol,h0,T,*P)
 
         if type=='seuil':
-            output,seuil=cond_stop(y,f.names)
-            outputprev,_=cond_stop(y_prev,f.names)
-            y,hopt,_,_,t_now,_,_=cond(
+            output,seuil=cond_stop(x,f.xnames)
+            outputprev,_=cond_stop(x_prev,f.xnames)
+            x,hopt,_,_,t_now,_,y,_,_=cond(
                 np.sign(output-seuil)!=np.sign(outputprev-seuil),interpolation,
-                        lambda state:state,(y,hopt,y_prev,t_prev,t_now,
+                        lambda state:state,(x,hopt,x_prev,t_prev,t_now,y_prev,y,
                                             output-seuil,outputprev-seuil))
         elif isinstance(type,float):
+            x=np.where(t_now>type,((x_prev-x)*type+t_prev*x-t_now*x_prev)
+                       /(t_prev-t_now),x)
             y=np.where(t_now>type,((y_prev-y)*type+t_prev*y-t_now*y_prev)
                        /(t_prev-t_now),y)
             t_now,hopt=np.where(t_now>type,type,t_now),\
                        np.where(t_now>type,type-t_prev,hopt)
 
-        delta_y=rk_step_der(y_prev,t_prev,delta_y_prev,h,f_aug,*args)
+        delta_x=rk_step_der(x_prev,t_prev,delta_x_prev,h,f_aug,*P_and_dP)
+        if hasattr(f,'computeotherX'):
+            delta_x=jvp(f.computeotherX,(x,t_now,*P),(delta_x,0.,*dP))[1]
+        delta_y=jvp(f.output,(x,t_now,*P),(delta_x,0.,*dP))[1]
 
         if f.constraints!={}:
             for i in f.constraints.keys():
                 if isinstance(f.constraints[i][1], tuple):
-                    test_exp,(_,expression,_,_,der_expression,_)=f.constraints[i]
+                    test_exp,(_,expression,_,_,der_expression,_,name)=\
+                        f.constraints[i]
                 else:
-                    (_,expression,_,_,der_expression,_)=f.constraints[i]
+                    (_,expression,_,_,der_expression,_,name)=f.constraints[i]
                     test_exp = lambda t: True
-                cstr[i] = np.where(test_exp(t_now),expression(t_prev, y_prev,
-                            t_now,y, cstr[i],h,T,f.names),cstr[i])
+                ind=f.xnames.index(name)
+                cstr[i] = np.where(test_exp(t_now),expression(t_prev,x_prev[ind],
+                            t_now,x[ind], cstr[i],h,T),cstr[i])
                 delta_cstr[i]= np.where(test_exp(t_now),der_expression(t_prev,
-                    y_prev,delta_y_prev, t_now, y,delta_y,cstr[i],delta_cstr[i],
-                    h,T,f.names),delta_cstr[i])
+                    x_prev[ind],delta_x_prev[ind], t_now, x[ind],delta_x[ind],
+                                    cstr[i],delta_cstr[i],h,T),delta_cstr[i])
 
-        return y_prev,delta_y_prev,t_prev,y, delta_y,t_now, hopt,cstr,\
-               delta_cstr,inew
+        return x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,x,delta_x,y,\
+               delta_y,t_now, hopt,cstr,delta_cstr,inew,cnew
 
     cstr=dict(zip(list(f.constraints.keys()),[0.]*len(f.constraints)))#INITIALISATION
     delta_cstr=dict(zip(list(f.constraints.keys()),[0.]*len(f.constraints)))
     if f.constraints!={}:
         for i in f.constraints.keys():
             if isinstance(f.constraints[i][1], tuple):
-                test_exp,(init,_,_,dinit,_,_) = f.constraints[i]
+                test_exp,(init,_,_,dinit,_,_,name) = f.constraints[i]
             else:
-                (init,_,_,dinit,_,_) = f.constraints[i]
+                (init,_,_,dinit,_,_,name) = f.constraints[i]
                 test_exp = lambda t: True
-            cstr[i] = np.where(test_exp(0.),init(y0,0.,h0,f.names),cstr[i])
-            delta_cstr[i]=np.where(test_exp(0.),dinit(y0,delta_y0,0.,h0,f.names),
-                                     delta_cstr[i])
+            ind=f.xnames.index(name)
+            cstr[i]=np.where(test_exp(0.),init(x0[ind],0.,h0),
+                             cstr[i])
+            delta_cstr[i]=np.where(test_exp(0.),dinit(x0[ind],delta_x0[ind],0.,
+                                    h0),delta_cstr[i])
 
     for element in f.__dict__.keys(): # pour eviter erreurs de code
         if isinstance(f.__dict__[element],interpreters.ad.JVPTracer):
             f.__dict__[element]=f.__dict__[element].primal
-    if hasattr(f,'etat_actuel'):
-        i0=f.etat_actuel
+    if hasattr(f,'etat'):
+        i0=f.etat
+        if hasattr(f,'commande'):
+            _,c0=f.commande(0.,T)
+        else:
+            c0=0
     else:
         i0=0
-    yfm1,_,_,yf,delta_yf,ts,h,cstr,delta_cstr,ifinal=while_loop(cond_fn,
-        body_fn,(y0,delta_y0,0.,y0,delta_y0,0.,h0,cstr,delta_cstr,i0))
-
+        c0=0
+    y0=f.output(x0,0.,*P)
+    delta_y0=jvp(f.output,(x0,0.,*P),(delta_x0,0.,*dP))[1]
+    xfm1,_,_,_,_,xf,delta_xf,yf,delta_yf,ts,h,cstr,delta_cstr,ifinal,_=\
+        while_loop(cond_fn,body_fn,(x0,delta_x0,y0,delta_y0,0.,x0,delta_x0,y0,
+                                    delta_y0,0.,h0,cstr,delta_cstr,i0,c0))
+    if hasattr(f,'etat'):
+        f.etat=ifinal
     if f.constraints!={}:
         for i in f.constraints.keys():
             if isinstance(f.constraints[i][1],tuple):
-                _,(_,_,fin,_,_,der_fin)=f.constraints[i]
+                _,(_,_,fin,_,_,der_fin,name)=f.constraints[i]
             else:
-                (_,_,fin,_,_,der_fin)=f.constraints[i]
+                (_,_,fin,_,_,der_fin,name)=f.constraints[i]
+            ind=f.xnames.index(name)
             cstr[i]=fin(ts,cstr[i],T)
-            delta_cstr[i]=der_fin(ts,cstr[i],T,delta_cstr[i],dT,yf,f.names)
+            delta_cstr[i]=der_fin(ts,cstr[i],T,delta_cstr[i],dT,xf[ind])
 
     if type=='seuil': # partial derivatives of ts
-        dout,_=cond_stop(delta_yf,f.names)
-        yseuil,_=cond_stop(f.derivative(yf,ts,*args_red),f.names)
-        dts=-(1/yseuil)*dout
+        dout,_=cond_stop(delta_xf,f.xnames)
+        xseuil,_=cond_stop(f.derivative(xf,ts,*P),f.xnames)
+        dts=-(1/xseuil)*dout
     elif type=='rp':
-        f.etat_actuel=ifinal
-        ind_rp=f.names.index(f.last_var_bf_rp)
-        yseuil=f.derivative(yf,ts,*args_red)[ind_rp]
-        dts=-(1/yseuil)*delta_yf[ind_rp]
+        #f.etat=ifinal
+        ind_rp=f.xnames.index(f.last_var_bf_rp)
+        xseuil=f.derivative(xf,ts,*P)[ind_rp]
+        dts=-(1/xseuil)*delta_xf[ind_rp]
     else:
         dts=0.
-    return yf,cstr,ts,dts,delta_yf,delta_cstr
+    return xf,yf,cstr,ts,dts,delta_xf,delta_yf,delta_cstr
 
 
 ################################################################################
 def T_pair(T):
     return lambda t:(t//T)%2==0
 
 def T_impair(T):
     return lambda t:(t//T)%2!=0
 
 def T_numero(T,n,i):
     return lambda t:(t//T)%n!=i
 
-def Min(ind):
-    return lambda y0,t0,h0,names:y0[names.index(ind)],\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names:np.minimum(
-               y[names.index(ind)],cstr), \
-        lambda tchoc,cstr,_:cstr,\
-        lambda y0,dy0,t0,h0,names:dy0[names.index(ind)],\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names:\
-               np.where(np.minimum(cstr,y[names.index(ind)])==
-                        y[names.index(ind)],dy[names.index(ind)],dcstr),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr
-
-def Max(ind):
-    return lambda y0,t0,h0,names:y0[names.index(ind)],\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names:np.maximum\
-               (y[names.index(ind)],cstr), \
-        lambda tchoc,cstr,_:cstr,\
-        lambda y0,dy0,t0,h0,names:dy0[names.index(ind)],\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names:\
-               np.where(np.maximum(cstr,y[names.index(ind)])==
-                        y[names.index(ind)],dy[names.index(ind)],dcstr),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr
-
-def moy(ind):
-    return lambda y0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names:cstr+0.5*h*\
-          (y_prev[names.index(ind)]+y[names.index(ind)]),\
-        lambda tchoc,cstr,_:cstr/tchoc,\
-        lambda y0,dy0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names: \
-            dcstr+0.5*h*(dprev[names.index(ind)]+ dy[names.index(ind)]),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr/tchoc
-
-def eff(ind):
-    return lambda y0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names: cstr+0.5*h*\
-            (y_prev[names.index(ind)]**2+y[names.index(ind)]**2),\
-        lambda tchoc,cstr,_:np.sqrt(cstr/tchoc),\
-        lambda y0,dy0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names: \
-        dcstr+0.5*h*(2*y_prev[names.index(ind)]*dprev[names.index(ind)]+
-                     2*y[names.index(ind)]* dy[names.index(ind)]),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr/(2*tchoc*cstr)
-
-def min_T(T,ind):
-    return lambda y0,t0,h0,names:y0[names.index(ind)],\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names:np.where((t_prev//T)==(t//T),
-            np.minimum(y[names.index(ind)],cstr),y[names.index(ind)]), \
-        lambda tchoc,cstr,_:cstr, \
-        lambda y0,dy0,t0,h0,names:dy0[names.index(ind)],\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names:\
-            np.where((t_prev//T)==(t//T),np.where(np.minimum(cstr,
-                y[names.index(ind)])==y[names.index(ind)],dy[names.index(ind)],
-                                                  dcstr),dy[names.index(ind)]),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr
-
-def max_T(T,ind):
-    return lambda y0,t0,h0,names:y0[names.index(ind)],\
-        lambda t_prev,y_prev,t,y,cstr,h,_,names:np.where((t_prev//T)==(t//T),
-            np.maximum(y[names.index(ind)],cstr),y[names.index(ind)]),\
-        lambda tchoc,cstr,_:cstr,\
-        lambda y0,dy0,t0,h0,names:dy0[names.index(ind)],\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,_,names:\
-            np.where((t_prev//T)==(t//T),np.where(np.maximum(cstr,
-                y[names.index(ind)])==y[names.index(ind)],dy[names.index(ind)],
-                                                  dcstr),dy[names.index(ind)]),\
-        lambda tchoc,cstr,_,dcstr,dT,yf,names:dcstr
-
-def moy_T(ind):
-    return lambda y0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,t,y,cstr,h,T,names:np.where((t_prev//T)==(t//T),
-        cstr+0.5*h*(y_prev[names.index(ind)]+y[names.index(ind)]), 0.),\
-        lambda tchoc,cstr,T:cstr/T,\
-        lambda y0,dy0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,T,names: \
-        np.where((t_prev//T)==(t//T),dcstr+0.5*h*(dprev[names.index(ind)]+
-            dy[names.index(ind)]),0.),\
-        lambda tchoc,cstr,T,dcstr,dT,yf,names:dcstr/T+((yf[names.index(ind)]-
-                                                        cstr)/T)*dT
-
-def eff_T(ind):
-    return lambda y0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,t,y,cstr,h,T,names: np.where((t_prev//T)==(t//T),
-        cstr+0.5*h*(y_prev[names.index(ind)]**2+y[names.index(ind)]**2),0.),\
-        lambda tchoc,cstr,T:np.sqrt(cstr/T),\
-        lambda y0,dy0,t0,h0,names:0.,\
-        lambda t_prev,y_prev,dprev,t,y,dy,cstr,dcstr,h,T,names: \
-        np.where((t_prev//T)==(t//T),dcstr+0.5*h*(2*y_prev[names.index(ind)]*
-            dprev[names.index(ind)]+2*y[names.index(ind)]*
-            dy[names.index(ind)]),0.),\
-        lambda tchoc,cstr,T,dcstr,dT,yf,names:dcstr/(2*T*cstr)+(yf[names.index
-                                    (ind)]**2-cstr**2)/(2*cstr*T)*dT
+def Min(name):
+    def init(x0,t0,h0):
+        return x0
+    def expression(t_prev,x_prev,t,x,cstr,h,_):
+        return np.minimum(x,cstr)
+    def fin(tchoc,cstr,_):
+        return cstr
+    def dinit(x0,dx0,t0,h0):
+        return dx0
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,_):
+        return np.where(np.minimum(cstr,x)==x,dx,dcstr)
+    def dfin(tchoc,cstr,_,dcstr,dT,xf):
+        return dcstr
+    return init,expression,fin,dinit,dexpression,dfin,name
+
+def Max(name):
+    def init(x0,t0,h0):
+        return x0
+    def expression(t_prev,x_prev,t,x,cstr,h,_):
+        return np.maximum(x,cstr)
+    def fin(tchoc, cstr, _):
+        return cstr
+    def dinit(x0, dx0, t0, h0):
+        return dx0
+    def dexpression(t_prev, x_prev, dprev, t, x, dx, cstr, dcstr, h, _):
+        return np.where(np.maximum(cstr,x)==x,dx,dcstr)
+    def dfin(tchoc, cstr, _, dcstr, dT, xf):
+        return dcstr
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def moy(name):
+    def init(x0,t0,h0):
+        return 0.
+    def expression(t_prev, x_prev, t, x, cstr, h, _):
+        return cstr+0.5*h*(x_prev+x)
+    def fin(tchoc,cstr,_):
+        return cstr/tchoc
+    def dinit(x0,dx0,t0,h0):
+        return 0.
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,_):
+        return dcstr+0.5*h*(dprev+ dx)
+    def dfin(tchoc,cstr,_,dcstr,dT,xf):
+        return dcstr/tchoc
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def eff(name):
+    def init(x0,t0,h0):
+        return 0.
+    def expression(t_prev,x_prev,t,x,cstr,h,_):
+        return cstr+0.5*h*(x_prev**2+x**2)
+    def fin(tchoc,cstr,_):
+        return np.sqrt(cstr/tchoc)
+    def dinit(x0,dx0,t0,h0):
+        return 0.
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,_):
+        return dcstr+0.5*h*(2*x_prev*dprev+2*x* dx)
+    def dfin(tchoc,cstr,_,dcstr,dT,xf):
+        return dcstr/(2*tchoc*cstr)
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def min_T(T,name):
+    def init(x0,t0,h0):
+        return x0
+    def expression(t_prev,x_prev,t,x,cstr,h,_):
+        return np.where((t_prev//T)==(t//T),np.minimum(x,cstr),x)
+    def fin(tchoc,cstr,_):
+        return cstr
+    def dinit(x0,dx0,t0,h0):
+        return dx0
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,_):
+        return jvp(expression,(t_prev,x_prev,t,x,cstr,h,_),
+                   (0.,dprev,0.,dx,dcstr,0.,0.))[1]#np.where((t_prev//T)==(t//T),np.where(np.minimum(cstr,
+                #x)==x,dx,dcstr),dx)#
+    def dfin(tchoc,cstr,_,dcstr,dT,xf):
+        return dcstr
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def max_T(T,name):
+    def init(x0,t0,h0):
+        return x0
+    def expression(t_prev,x_prev,t,x,cstr,h,_):
+        return np.where((t_prev//T)==(t//T),np.maximum(x,cstr),x)
+    def fin(tchoc,cstr,_):
+        return cstr
+    def dinit(x0,dx0,t0,h0):
+        return dx0
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,_):
+        return jvp(expression,(t_prev,x_prev,t,x,cstr,h,_),
+                   (0.,dprev,0.,dx,dcstr,0.,0.))[1]#np.where((t_prev//T)==(t//T),np.where(np.maximum(cstr,
+                #x)==x,dx,dcstr),dx)#
+    def dfin(tchoc,cstr,_,dcstr,dT,xf):
+        return dcstr
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def moy_T(name):
+    def init(x0,t0,h0):
+        return 0.
+    def expression(t_prev,x_prev,t,x,cstr,h,T):
+        return np.where((t_prev//T)==(t//T),cstr+0.5*h*(x_prev+x), 0.)
+    def fin(tchoc,cstr,T):
+        return cstr/T
+    def dinit(x0,dx0,t0,h0):
+        return 0.
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,T):
+        return np.where((t_prev//T)==(t//T),dcstr+0.5*h*(dprev+dx),0.)
+    def dfin(tchoc,cstr,T,dcstr,dT,xf):
+        return dcstr/T+((xf-cstr)/T)*dT
+    return init, expression, fin, dinit, dexpression, dfin,name
+
+def eff_T(name):
+    def init(x0,t0,h0):
+        return 0.
+    def expression(t_prev,x_prev,t,x,cstr,h,T):
+        return np.where((t_prev//T)==(t//T),cstr+0.5*h*(x_prev**2+x**2),0.)
+    def fin(tchoc,cstr,T):
+        return np.sqrt(cstr/T)
+    def dinit(x0,dx0,t0,h0):
+        return 0.
+    def dexpression(t_prev,x_prev,dprev,t,x,dx,cstr,dcstr,h,T):
+        return np.where((t_prev//T)==(t//T),dcstr+0.5*h*(2*x_prev*
+                                    dprev+2*x*dx),0.)
+    def dfin(tchoc,cstr,T,dcstr,dT,xf):
+        return dcstr/(2*T*cstr)+(xf**2-cstr**2)/(2*cstr*T)*dT
+    return init, expression, fin, dinit, dexpression, dfin,name
 
 
 def reg_perm(T,nbT,names_var,a=1e-5):
     constr = {}
     for i in range(len(names_var)):
         constr[names_var[i]+'_min']=(T_pair(nbT * T),
                                      min_T(nbT * T, names_var[i]))
@@ -315,15 +381,15 @@
             vectimp=vectimp.at[i].set(cstr[names_var[i]+'_minimp'])
             vectimp=vectimp.at[2*i+1].set(cstr[names_var[i]+'_maximp'])
         return np.bitwise_not(np.bitwise_and(np.allclose(vectp,vectimp,atol=a),
                     np.not_equal(t_prev//T,t//T)))
     return ('rp',regime_perm),constr
 
 def seuil(ind,seuil=0.):
-    return ('seuil', lambda y,names: (y[names.index(ind)], seuil))
+    return ('seuil', lambda x,names: (x[names.index(ind)], seuil))
 
 def temps_final(tf):
     return (tf,lambda t_prev,t,cstr:t_prev<tf)
 
 def get_indice(names,valeur,output):
     if len(output)==1:
         return valeur[names.index(output[0])]
```

### Comparing `noloadj-1.2.5/noloadj/ODE/ode_tools.py` & `noloadj-1.2.6/noloadj/ODE/ode_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import jax.numpy as np
-from jax.lax import switch
+from jax.lax import switch,cond
 from jax import custom_jvp,jvp
 import jax
 from functools import partial
 
-def fonction(res):
-    return lambda _: res()
+def fonction(func):
+    return lambda _: func()
 
 def vect_temporel(debut,fin,pas):
     return np.linspace(debut,fin,int((fin-debut)/pas))
 
 def indice_t(t,pas,debut=0.):
     return ((t-debut)/pas).astype(int)
 
 def Switch(etat,funcs):
     return switch(etat,[fonction(func) for func in funcs],None)
 
+def Condition(conditions,functions,state):
+    for i in range(len(conditions)):
+        state=cond(conditions[i],functions[i],lambda state:state,state)
+    return state
+
 ###################################################### external functions
 @partial(custom_jvp,nondiff_argnums=(1,2))
 def compute_external(inputs,len_output,Extfunc):
     output_type=jax.ShapeDtypeStruct((len_output,),'float64')
     def compute_intermediary_function(inputs):
         outputs=Extfunc.compute(inputs)
         return np.array(outputs)
```

### Comparing `noloadj-1.2.5/noloadj/analyse/simulation.py` & `noloadj-1.2.6/noloadj/analyse/simulation.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/gui/plotIterations.py` & `noloadj-1.2.6/noloadj/gui/plotIterations.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/gui/plotPareto.py` & `noloadj-1.2.6/noloadj/gui/plotPareto.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/gui/testOverLabels.py` & `noloadj-1.2.6/noloadj/gui/testOverLabels.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/ExportToXML.py` & `noloadj-1.2.6/noloadj/optimization/ExportToXML.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/Tools.py` & `noloadj-1.2.6/noloadj/optimization/Tools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/iterationHandler.py` & `noloadj-1.2.6/noloadj/optimization/iterationHandler.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/multiobjective.py` & `noloadj-1.2.6/noloadj/optimization/multiobjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/optimProblem.py` & `noloadj-1.2.6/noloadj/optimization/optimProblem.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/paretoTools.py` & `noloadj-1.2.6/noloadj/optimization/paretoTools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/specifications.py` & `noloadj-1.2.6/noloadj/optimization/specifications.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/optimization/wrapper.py` & `noloadj-1.2.6/noloadj/optimization/wrapper.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/tutorial/01-UnconstrainedMonoObjective.py` & `noloadj-1.2.6/noloadj/tutorial/01-UnconstrainedMonoObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/tutorial/02-ConstrainedMonoObjective.py` & `noloadj-1.2.6/noloadj/tutorial/02-ConstrainedMonoObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/tutorial/03-ConstrainedMultiObjective.py` & `noloadj-1.2.6/noloadj/tutorial/03-ConstrainedMultiObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/tutorial/04-ConstrainedMonoObjective2.py` & `noloadj-1.2.6/noloadj/tutorial/04-ConstrainedMonoObjective2.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj/tutorial/plotTools.py` & `noloadj-1.2.6/noloadj/tutorial/plotTools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.5/noloadj.egg-info/PKG-INFO` & `noloadj-1.2.6/noloadj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noloadj
-Version: 1.2.5
+Version: 1.2.6
 Summary: solving constrained optimization problem for the design of engineering systems
 Author: B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT
 Author-email: benoit.delinchant@G2ELab.grenoble-inp.fr
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `noloadj-1.2.5/noloadj.egg-info/SOURCES.txt` & `noloadj-1.2.6/noloadj.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 docs/new_features/v1.2.0.rst
 docs/new_features/v1.2.1.rst
 docs/new_features/v1.2.15.rst
 docs/new_features/v1.2.2.rst
 docs/new_features/v1.2.3.rst
 docs/new_features/v1.2.4.rst
 docs/new_features/v1.2.5.rst
+docs/new_features/v1.2.6.rst
 noloadj/__init__.py
 noloadj.egg-info/PKG-INFO
 noloadj.egg-info/SOURCES.txt
 noloadj.egg-info/dependency_links.txt
 noloadj.egg-info/requires.txt
 noloadj.egg-info/top_level.txt
 noloadj/ODE/ode45.py
```

### Comparing `noloadj-1.2.5/setup.py` & `noloadj-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 # SPDX-FileCopyrightText: 2021 G2Elab / MAGE
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 NoLOAD_Jax installation script
-:version: 1.2.5
+:version: 1.2.6
 """
 
 from setuptools import setup, find_packages
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (1, 2, 5)
+__version_info__ = (1, 2, 6)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 #__docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

