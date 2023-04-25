# Comparing `tmp/stamox-0.1.3.tar.gz` & `tmp/stamox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stamox-0.1.3.tar", last modified: Fri Apr 14 06:57:37 2023, max compression
+gzip compressed data, was "stamox-0.1.4.tar", last modified: Tue Apr 25 06:23:38 2023, max compression
```

## Comparing `stamox-0.1.3.tar` & `stamox-0.1.4.tar`

### file list

```diff
@@ -1,96 +1,91 @@
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.277423 stamox-0.1.3/
--rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.3/LICENCE
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:57:37.277289 stamox-0.1.3/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     3921 2023-04-10 09:03:02.000000 stamox-0.1.3/README.md
--rw-r--r--   0 jiayaobo   (501) staff       (20)      413 2023-03-28 10:26:52.000000 stamox-0.1.3/pyproject.toml
--rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-14 06:57:37.277465 stamox-0.1.3/setup.cfg
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1121 2023-04-14 06:56:34.000000 stamox-0.1.3/setup.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.266378 stamox-0.1.3/stamox/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      610 2023-04-10 07:38:29.000000 stamox-0.1.3/stamox/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267207 stamox-0.1.3/stamox/anova/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       70 2023-03-28 10:30:02.000000 stamox-0.1.3/stamox/anova/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267508 stamox-0.1.3/stamox/anova/one_way/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.3/stamox/anova/one_way/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4298 2023-04-10 07:41:59.000000 stamox-0.1.3/stamox/anova/one_way/_aov.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-11 10:08:22.000000 stamox-0.1.3/stamox/basic.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267790 stamox-0.1.3/stamox/cluster/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-10 07:00:50.000000 stamox-0.1.3/stamox/cluster/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5151 2023-04-14 05:37:17.000000 stamox-0.1.3/stamox/cluster/_kmeans.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.268741 stamox-0.1.3/stamox/core/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      630 2023-04-10 07:21:03.000000 stamox-0.1.3/stamox/core/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      231 2023-04-13 16:45:38.000000 stamox-0.1.3/stamox/core/_func_state.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-14 05:56:50.000000 stamox-0.1.3/stamox/core/_utils.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2921 2023-04-14 06:25:15.000000 stamox-0.1.3/stamox/core/base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2324 2023-04-14 06:17:30.000000 stamox-0.1.3/stamox/core/jit.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6336 2023-04-14 06:56:15.000000 stamox-0.1.3/stamox/core/maps.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-14 06:43:29.000000 stamox-0.1.3/stamox/core/pipe.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272202 stamox-0.1.3/stamox/distribution/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1680 2023-04-13 15:54:20.000000 stamox-0.1.3/stamox/distribution/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6173 2023-04-14 05:36:26.000000 stamox-0.1.3/stamox/distribution/_beta.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5559 2023-04-13 15:59:27.000000 stamox-0.1.3/stamox/distribution/_binomial.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6371 2023-04-13 14:31:34.000000 stamox-0.1.3/stamox/distribution/_cauchy.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5117 2023-04-08 16:53:06.000000 stamox-0.1.3/stamox/distribution/_chisq.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2220 2023-04-08 17:08:44.000000 stamox-0.1.3/stamox/distribution/_ecdf.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5675 2023-04-08 16:55:44.000000 stamox-0.1.3/stamox/distribution/_exp.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5942 2023-04-08 16:57:42.000000 stamox-0.1.3/stamox/distribution/_f.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6307 2023-04-08 16:59:05.000000 stamox-0.1.3/stamox/distribution/_gamma.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      787 2023-03-29 10:43:04.000000 stamox-0.1.3/stamox/distribution/_geom.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6467 2023-04-08 17:01:47.000000 stamox-0.1.3/stamox/distribution/_laplace.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7228 2023-04-08 17:00:17.000000 stamox-0.1.3/stamox/distribution/_normal.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6385 2023-04-08 17:03:09.000000 stamox-0.1.3/stamox/distribution/_pareto.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5449 2023-04-13 15:59:19.000000 stamox-0.1.3/stamox/distribution/_poisson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1067 2023-04-05 14:34:37.000000 stamox-0.1.3/stamox/distribution/_q_discrete_search.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1873 2023-03-29 10:43:29.000000 stamox-0.1.3/stamox/distribution/_rademacher.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6920 2023-04-08 17:04:47.000000 stamox-0.1.3/stamox/distribution/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1144 2023-03-29 10:43:56.000000 stamox-0.1.3/stamox/distribution/_triangular.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6220 2023-04-08 17:06:06.000000 stamox-0.1.3/stamox/distribution/_uniform.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5556 2023-04-08 16:42:13.000000 stamox-0.1.3/stamox/distribution/_weibull.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272503 stamox-0.1.3/stamox/experimental/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-13 16:31:36.000000 stamox-0.1.3/stamox/experimental/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1351 2023-04-13 16:31:43.000000 stamox-0.1.3/stamox/experimental/better_partial.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272823 stamox-0.1.3/stamox/experimental/decomposition/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-11 10:10:40.000000 stamox-0.1.3/stamox/experimental/decomposition/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-10 07:40:46.000000 stamox-0.1.3/stamox/experimental/decomposition/_pca.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273249 stamox-0.1.3/stamox/experimental/maps/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-11 10:10:44.000000 stamox-0.1.3/stamox/experimental/maps/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-03-27 09:56:00.000000 stamox-0.1.3/stamox/experimental/maps/auto_map.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-03-28 10:31:15.000000 stamox-0.1.3/stamox/experimental/maps/cube_map.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273381 stamox-0.1.3/stamox/experimental/nn/
--rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-12 13:43:28.000000 stamox-0.1.3/stamox/experimental/nn/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273620 stamox-0.1.3/stamox/formula/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-08 13:01:51.000000 stamox-0.1.3/stamox/formula/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1415 2023-04-11 10:10:07.000000 stamox-0.1.3/stamox/formula/_formula.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.275451 stamox-0.1.3/stamox/hypothesis/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      814 2023-04-14 06:42:01.000000 stamox-0.1.3/stamox/hypothesis/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2540 2023-04-14 06:37:22.000000 stamox-0.1.3/stamox/hypothesis/_bartlett.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      734 2023-03-29 10:40:56.000000 stamox-0.1.3/stamox/hypothesis/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2283 2023-04-06 14:56:52.000000 stamox-0.1.3/stamox/hypothesis/_durbin_watson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2740 2023-04-14 06:41:22.000000 stamox-0.1.3/stamox/hypothesis/_friedman.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      806 2023-03-29 10:41:12.000000 stamox-0.1.3/stamox/hypothesis/_p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      837 2023-03-29 10:41:19.000000 stamox-0.1.3/stamox/hypothesis/_pearsonr.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5033 2023-04-14 06:41:48.000000 stamox-0.1.3/stamox/hypothesis/_shapiro_wilk.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      954 2023-03-29 10:41:28.000000 stamox-0.1.3/stamox/hypothesis/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1179 2023-03-21 16:44:14.000000 stamox-0.1.3/stamox/hypothesis/cor2ci.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      485 2023-03-21 16:44:03.000000 stamox-0.1.3/stamox/hypothesis/cor2p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1029 2023-03-16 09:09:37.000000 stamox-0.1.3/stamox/hypothesis/corr.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276003 stamox-0.1.3/stamox/math/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-10 03:27:30.000000 stamox-0.1.3/stamox/math/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1255 2023-04-10 03:26:51.000000 stamox-0.1.3/stamox/math/combination.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      670 2023-04-05 11:46:28.000000 stamox-0.1.3/stamox/math/special.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276503 stamox-0.1.3/stamox/regression/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-13 07:01:57.000000 stamox-0.1.3/stamox/regression/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-12 13:26:06.000000 stamox-0.1.3/stamox/regression/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7062 2023-04-10 10:29:07.000000 stamox-0.1.3/stamox/regression/_lm.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276908 stamox-0.1.3/stamox/sample/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      343 2023-04-14 06:48:40.000000 stamox-0.1.3/stamox/sample/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2835 2023-04-09 14:28:45.000000 stamox-0.1.3/stamox/sample/_bootstrap.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1821 2023-04-14 06:48:11.000000 stamox-0.1.3/stamox/sample/_jackknife.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      888 2023-04-10 09:45:17.000000 stamox-0.1.3/stamox/transformation.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267053 stamox-0.1.3/stamox.egg-info/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2133 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/SOURCES.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/dependency_links.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)      385 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/requires.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/top_level.txt
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.277044 stamox-0.1.3/tests/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1747 2023-04-08 15:17:53.000000 stamox-0.1.3/tests/test_basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.370901 stamox-0.1.4/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.4/LICENCE
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4837 2023-04-25 06:23:38.370709 stamox-0.1.4/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4513 2023-04-25 03:32:49.000000 stamox-0.1.4/README.md
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      328 2023-04-20 16:25:17.000000 stamox-0.1.4/pyproject.toml
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-25 06:23:38.370946 stamox-0.1.4/setup.cfg
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1132 2023-04-23 12:15:32.000000 stamox-0.1.4/setup.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.361268 stamox-0.1.4/stamox/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1224 2023-04-24 15:12:30.000000 stamox-0.1.4/stamox/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362090 stamox-0.1.4/stamox/anova/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       58 2023-04-20 08:53:58.000000 stamox-0.1.4/stamox/anova/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362359 stamox-0.1.4/stamox/anova/one_way/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.4/stamox/anova/one_way/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4549 2023-04-25 06:17:29.000000 stamox-0.1.4/stamox/anova/one_way/_aov.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      933 2023-04-25 06:11:55.000000 stamox-0.1.4/stamox/basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362632 stamox-0.1.4/stamox/cluster/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/cluster/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5146 2023-04-25 06:15:24.000000 stamox-0.1.4/stamox/cluster/_kmeans.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.363578 stamox-0.1.4/stamox/core/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      640 2023-04-20 08:51:36.000000 stamox-0.1.4/stamox/core/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      154 2023-04-24 15:15:40.000000 stamox-0.1.4/stamox/core/_func_state.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2958 2023-04-24 03:39:07.000000 stamox-0.1.4/stamox/core/base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1670 2023-04-23 12:16:09.000000 stamox-0.1.4/stamox/core/better_partial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2805 2023-04-24 15:14:50.000000 stamox-0.1.4/stamox/core/jit.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7183 2023-04-25 03:29:46.000000 stamox-0.1.4/stamox/core/maps.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6442 2023-04-25 03:29:11.000000 stamox-0.1.4/stamox/core/pipe.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.364151 stamox-0.1.4/stamox/correlation/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      131 2023-04-17 09:53:48.000000 stamox-0.1.4/stamox/correlation/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1234 2023-04-24 15:32:33.000000 stamox-0.1.4/stamox/correlation/_cor.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1947 2023-04-24 15:32:24.000000 stamox-0.1.4/stamox/correlation/_pearson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2175 2023-04-24 15:32:18.000000 stamox-0.1.4/stamox/correlation/_spearman.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366520 stamox-0.1.4/stamox/distribution/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1824 2023-04-16 10:53:49.000000 stamox-0.1.4/stamox/distribution/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6296 2023-04-24 15:24:08.000000 stamox-0.1.4/stamox/distribution/_beta.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6218 2023-04-24 15:23:53.000000 stamox-0.1.4/stamox/distribution/_binomial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6675 2023-04-24 15:24:23.000000 stamox-0.1.4/stamox/distribution/_cauchy.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5069 2023-04-24 15:24:56.000000 stamox-0.1.4/stamox/distribution/_chisq.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2176 2023-04-21 13:54:17.000000 stamox-0.1.4/stamox/distribution/_ecdf.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5827 2023-04-21 13:57:31.000000 stamox-0.1.4/stamox/distribution/_exp.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6211 2023-04-21 14:02:56.000000 stamox-0.1.4/stamox/distribution/_f.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6522 2023-04-24 15:25:41.000000 stamox-0.1.4/stamox/distribution/_gamma.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7011 2023-04-24 15:25:50.000000 stamox-0.1.4/stamox/distribution/_laplace.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7373 2023-04-24 15:26:12.000000 stamox-0.1.4/stamox/distribution/_normal.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6365 2023-04-22 03:02:59.000000 stamox-0.1.4/stamox/distribution/_pareto.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5787 2023-04-24 15:28:25.000000 stamox-0.1.4/stamox/distribution/_poisson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7219 2023-04-22 03:11:38.000000 stamox-0.1.4/stamox/distribution/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-22 03:15:15.000000 stamox-0.1.4/stamox/distribution/_uniform.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1511 2023-04-22 03:21:20.000000 stamox-0.1.4/stamox/distribution/_utils.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6922 2023-04-24 15:29:30.000000 stamox-0.1.4/stamox/distribution/_weibull.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366677 stamox-0.1.4/stamox/experimental/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-20 08:52:04.000000 stamox-0.1.4/stamox/experimental/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366989 stamox-0.1.4/stamox/experimental/decomposition/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/decomposition/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/decomposition/_pca.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.367425 stamox-0.1.4/stamox/experimental/maps/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/auto_map.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/cube_map.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.367726 stamox-0.1.4/stamox/formula/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/formula/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1556 2023-04-21 12:35:01.000000 stamox-0.1.4/stamox/formula/_formula.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2490 2023-04-25 06:12:34.000000 stamox-0.1.4/stamox/functions.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.368458 stamox-0.1.4/stamox/hypothesis/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      427 2023-04-21 10:11:31.000000 stamox-0.1.4/stamox/hypothesis/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2535 2023-04-24 15:30:51.000000 stamox-0.1.4/stamox/hypothesis/_bartlett.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      923 2023-04-19 05:36:05.000000 stamox-0.1.4/stamox/hypothesis/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2282 2023-04-24 15:31:15.000000 stamox-0.1.4/stamox/hypothesis/_durbin_watson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2736 2023-04-24 15:31:44.000000 stamox-0.1.4/stamox/hypothesis/_friedman.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.368874 stamox-0.1.4/stamox/math/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/math/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1243 2023-04-21 12:41:38.000000 stamox-0.1.4/stamox/math/combination.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1497 2023-04-21 06:19:17.000000 stamox-0.1.4/stamox/math/special.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6771 2023-04-25 03:43:41.000000 stamox-0.1.4/stamox/pipe_functions.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.369457 stamox-0.1.4/stamox/regression/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/regression/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/regression/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7260 2023-04-24 15:30:13.000000 stamox-0.1.4/stamox/regression/_lm.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.369933 stamox-0.1.4/stamox/sample/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      228 2023-04-19 05:08:41.000000 stamox-0.1.4/stamox/sample/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2719 2023-04-25 06:18:28.000000 stamox-0.1.4/stamox/sample/_bootstrap.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1741 2023-04-25 06:18:12.000000 stamox-0.1.4/stamox/sample/_jackknife.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1803 2023-04-25 06:18:39.000000 stamox-0.1.4/stamox/transformation.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.361944 stamox-0.1.4/stamox.egg-info/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4837 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1957 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      399 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/requires.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/top_level.txt
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.370462 stamox-0.1.4/tests/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1463 2023-04-25 06:13:09.000000 stamox-0.1.4/tests/test_basic.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      871 2023-04-24 15:10:59.000000 stamox-0.1.4/tests/test_transformation.py
```

### Comparing `stamox-0.1.3/LICENCE` & `stamox-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `stamox-0.1.3/PKG-INFO` & `stamox-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: stamox
-Version: 0.1.3
-Summary: Accelerate Your Statistical Analysis with JAX.
-Home-page: https://github.com/jiayaobo/stamox
-Author: Jia Yaobo
-License: Apache 2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: complete
-License-File: LICENCE
-
 <h1 align='center'>Stamox</h1>
 
 [![PyPI version](https://badge.fury.io/py/stamox.svg)](https://badge.fury.io/py/stamox)
 [![PyPI - License](https://img.shields.io/pypi/l/stamox)](https://pypi.org/project/stamox/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stamox)](https://pypi.org/project/stamox/)
 [![GitHub stars](https://img.shields.io/github/stars/jiayaobo/stamox)]()
 
@@ -42,121 +29,143 @@
 *calculate cdf*
 
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
-pip install stamox
+pip install -U stamox
+# or
+pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
 
 ### Similar but faster distribution functions to `R`
 
+You can simply import all functions from `stamox.functions`
+
 ```python
-from stamox.distribution import *
+from stamox.functions import dnorm, pnorm, qnorm, rnorm
 import jax.random as jrandom
 
 key = jrandom.PRNGKey(20010813)
 
 # random
 x = rnorm(key, sample_shape=(1000, ))
 # cdf
-pnorm(x)
+prob = pnorm(x)
 # ppf
-qnorm(x)
+qntl = qnorm(prob)
 # pdf
 dnorm(x)
 ```
 
 ### Fearless Pipeable
 
 `>>` is the pipe operator, which is the similar to `|>` in `F#` and `Elixir` or `%>%` in `R`.
 
-* Internal Functions Pipeable
+* You can simply import all pipeable functions from `pipe_functions`
 
 ```python
 import jax.random as jrandom
-from stamox.basic import scale
-from stamox.core import pipe_jit
-from stamox.distribution import rnorm
-from stamox.regression import lm
+import stamox.pipe_functions as PF
+from stamox import pipe_jit
 
 key = jrandom.PRNGKey(20010813)
 
 @pipe_jit
 def f(x):
     return [3 * x[:, 0] + 2 * x[:, 1] - x[:, 2], x] # [y, X]
-pipe = rnorm(sample_shape=(1000, 3)) >> f >> lm
+pipe = PF.rnorm(sample_shape=(1000, 3)) >> f >> PF.lm
 state = pipe(key)
 print(state.params)
 ```
 
+### Linear Regression with Formula
+
+```python
+import pandas as pd
+import numpy as np
+from stamox.functions import lm # or from stamox.pipe_functions import lm
+
+
+x = np.random.uniform(size=(1000, 3))
+y = 2 * x[:,0] + 3 * x[:,1] + 4 * x[:,2] + np.random.normal(size=1000)
+df = pd.DataFrame(x, columns=['x1', 'x2', 'x3'])
+df['y'] = y
+
+lm(df, 'y~x1+x2+x3').params
+```
+
 * Custom Functions Pipeable
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
+from stamox import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
 import jax.random as jrandom
 
 x = jnp.ones((1000, ))
 # single input, simply add make pipe
 @make_pipe
 def f(x):
     return x ** 2
 
-# multiple input, add make partial pipe
+# multiple input, decorate with make partial pipe
 @make_partial_pipe
 def g(x, y):
     return x + y
 
-# Notice Only One Positional Argument Can Be Received Along the pipe
+# x -> f -> g(y=2.) -> f -> g(y=3.) -> f
 h = Pipeable(x) >> f >> g(y=2.) >> f >> g(y=3.) >> f
+# h is a Pipeable object, you can call it to get the result
 print(h())
 ```
 
 * Compatible With `JAX` and `Equinox`
 
 You can use autograd features from `JAX` and `Equinox` with `Stamox` easily.
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
+from stamox import make_partial_pipe
 from equinox import filter_jit, filter_vmap, filter_grad
 
 @make_partial_pipe
 @filter_jit
 @filter_vmap
 @filter_grad
 def f(x, y):
     return y * x ** 3
-       
-f(y=3.)(jnp.array([1., 2., 3.]))
+
+# df/dx = 3y * x^2
+g = f(y=3.) # derive with respect to x given y=3
+g(jnp.array([1., 2., 3.]))
 ```
 
 Or vmap, pmap, jit features integrated with `Stamox`:
 
 ```python
-from stamox.core import pipe_vmap, pipe_jit
+from stamox import pipe_vmap, pipe_jit
 
 @pipe_vmap
 @pipe_jit
 def f(x):
     return x ** 2
 
-f(jnp.array([1., 2., 3.]))
+g = f >> f >> f
+print(g(jnp.array([1, 2, 3])))
 ```
 
 ## Acceleration Support
 
 `JAX` can be accelerated by `GPU` and `TPU`. So, `Stamox` is compatible with them.
 
 ## See More
 
 [JAX](https://github.com/google/jax)
 
-[Equinox](https://github.com/patrick-kidger/equinox#readme)
+[Equinox](https://github.com/patrick-kidger/equinox#readme)
```

### Comparing `stamox-0.1.3/README.md` & `stamox-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: stamox
+Version: 0.1.4
+Summary: Accelerate Your Statistical Analysis with JAX.
+Home-page: https://github.com/jiayaobo/stamox
+Author: Jia Yaobo
+License: Apache 2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: complete
+License-File: LICENCE
+
 <h1 align='center'>Stamox</h1>
 
 [![PyPI version](https://badge.fury.io/py/stamox.svg)](https://badge.fury.io/py/stamox)
 [![PyPI - License](https://img.shields.io/pypi/l/stamox)](https://pypi.org/project/stamox/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stamox)](https://pypi.org/project/stamox/)
 [![GitHub stars](https://img.shields.io/github/stars/jiayaobo/stamox)]()
 
@@ -29,121 +42,143 @@
 *calculate cdf*
 
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
-pip install stamox
+pip install -U stamox
+# or
+pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
 
 ### Similar but faster distribution functions to `R`
 
+You can simply import all functions from `stamox.functions`
+
 ```python
-from stamox.distribution import *
+from stamox.functions import dnorm, pnorm, qnorm, rnorm
 import jax.random as jrandom
 
 key = jrandom.PRNGKey(20010813)
 
 # random
 x = rnorm(key, sample_shape=(1000, ))
 # cdf
-pnorm(x)
+prob = pnorm(x)
 # ppf
-qnorm(x)
+qntl = qnorm(prob)
 # pdf
 dnorm(x)
 ```
 
 ### Fearless Pipeable
 
 `>>` is the pipe operator, which is the similar to `|>` in `F#` and `Elixir` or `%>%` in `R`.
 
-* Internal Functions Pipeable
+* You can simply import all pipeable functions from `pipe_functions`
 
 ```python
 import jax.random as jrandom
-from stamox.basic import scale
-from stamox.core import pipe_jit
-from stamox.distribution import rnorm
-from stamox.regression import lm
+import stamox.pipe_functions as PF
+from stamox import pipe_jit
 
 key = jrandom.PRNGKey(20010813)
 
 @pipe_jit
 def f(x):
     return [3 * x[:, 0] + 2 * x[:, 1] - x[:, 2], x] # [y, X]
-pipe = rnorm(sample_shape=(1000, 3)) >> f >> lm
+pipe = PF.rnorm(sample_shape=(1000, 3)) >> f >> PF.lm
 state = pipe(key)
 print(state.params)
 ```
 
+### Linear Regression with Formula
+
+```python
+import pandas as pd
+import numpy as np
+from stamox.functions import lm # or from stamox.pipe_functions import lm
+
+
+x = np.random.uniform(size=(1000, 3))
+y = 2 * x[:,0] + 3 * x[:,1] + 4 * x[:,2] + np.random.normal(size=1000)
+df = pd.DataFrame(x, columns=['x1', 'x2', 'x3'])
+df['y'] = y
+
+lm(df, 'y~x1+x2+x3').params
+```
+
 * Custom Functions Pipeable
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
+from stamox import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
 import jax.random as jrandom
 
 x = jnp.ones((1000, ))
 # single input, simply add make pipe
 @make_pipe
 def f(x):
     return x ** 2
 
-# multiple input, add make partial pipe
+# multiple input, decorate with make partial pipe
 @make_partial_pipe
 def g(x, y):
     return x + y
 
-# Notice Only One Positional Argument Can Be Received Along the pipe
+# x -> f -> g(y=2.) -> f -> g(y=3.) -> f
 h = Pipeable(x) >> f >> g(y=2.) >> f >> g(y=3.) >> f
+# h is a Pipeable object, you can call it to get the result
 print(h())
 ```
 
 * Compatible With `JAX` and `Equinox`
 
 You can use autograd features from `JAX` and `Equinox` with `Stamox` easily.
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
+from stamox import make_partial_pipe
 from equinox import filter_jit, filter_vmap, filter_grad
 
 @make_partial_pipe
 @filter_jit
 @filter_vmap
 @filter_grad
 def f(x, y):
     return y * x ** 3
-       
-f(y=3.)(jnp.array([1., 2., 3.]))
+
+# df/dx = 3y * x^2
+g = f(y=3.) # derive with respect to x given y=3
+g(jnp.array([1., 2., 3.]))
 ```
 
 Or vmap, pmap, jit features integrated with `Stamox`:
 
 ```python
-from stamox.core import pipe_vmap, pipe_jit
+from stamox import pipe_vmap, pipe_jit
 
 @pipe_vmap
 @pipe_jit
 def f(x):
     return x ** 2
 
-f(jnp.array([1., 2., 3.]))
+g = f >> f >> f
+print(g(jnp.array([1, 2, 3])))
 ```
 
 ## Acceleration Support
 
 `JAX` can be accelerated by `GPU` and `TPU`. So, `Stamox` is compatible with them.
 
 ## See More
 
 [JAX](https://github.com/google/jax)
 
-[Equinox](https://github.com/patrick-kidger/equinox#readme)
+[Equinox](https://github.com/patrick-kidger/equinox#readme)
```

### Comparing `stamox-0.1.3/setup.py` & `stamox-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 PACKAGE_NAME = "stamox"
 AUTHOR = "Jia Yaobo"
 URL = "https://github.com/jiayaobo/stamox"
 
 LICENSE = "Apache 2.0"
 DESCRIPTION = "Accelerate Your Statistical Analysis with JAX."
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
@@ -20,17 +20,17 @@
     "jaxtyping>=0.2.14",
     "typing_extensions>=4.5.0",
     "equinox>=0.10.1",
     "jaxopt>=0.6",
     "pandas>=1.5.3",
     "patsy>=0.5.3",
     "tensorflow-probability>=0.19.0",
-    "scipy"
+    "scipy",
 ]
-TESTS_REQUIRES = ["pytest", "scipy", "numpy", "sklearn", "statsmodels"]
+TESTS_REQUIRES = ["pytest", "scipy", "numpy", "sklearn", "statsmodels", "pandas"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

### Comparing `stamox-0.1.3/stamox/anova/one_way/_aov.py` & `stamox-0.1.4/stamox/anova/one_way/_aov.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import partial
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox import filter_jit
 from jax import Array, jit
 
-from ...core import make_partial_pipe
 from ...distribution import pF
 from ...hypothesis import HypoTest
 
 
 class OneWayAnovaTest(HypoTest):
     df_between: int
     df_within: int
@@ -87,24 +86,33 @@
 
 
 @partial(jit, static_argnames=("axis"))
 def _sum_of_squares(a, axis=0) -> Array:
     return jnp.sum(a * a, axis=axis, keepdims=True)
 
 
-@make_partial_pipe
 def one_way(*samples, axis=0) -> OneWayAnovaTest:
     """Performs a one-way ANOVA test.
 
     Args:
         *samples: A sequence of samples to compare.
         axis (int): The axis along which the samples are compared.
 
     Returns:
         OneWayAnovaTest: The result of the one-way ANOVA test.
+
+    Example:
+        >>> import jax.numpy as jnp
+        >>> from stamox.functions import one_way
+        >>>  # 3 samples with 5 observations each
+        >>> a = jnp.array([1, 2, 3, 4, 5])
+        >>> b = jnp.array([2, 3, 4, 5, 6])
+        >>> c = jnp.array([3, 4, 5, 6, 7])
+        >>> one_way(a, b, c)
+
     """
     samples = [jnp.asarray(sample) for sample in samples]
     ngroups = len(samples)
     return _one_way(samples, ngroups, axis=axis)
 
 
 @filter_jit
```

### Comparing `stamox-0.1.3/stamox/cluster/_kmeans.py` & `stamox-0.1.4/stamox/cluster/_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import jax.random as jrandom
 from equinox import filter_jit
 from jax import lax, vmap
 from jax._src.random import KeyArray
 from jax.scipy.cluster.vq import vq
 from jaxtyping import ArrayLike
 
-from ..core import make_partial_pipe, StateFunc
+from ..core import StateFunc
 
 
 class KMeansState(StateFunc):
     """KMeansState class for K-means clustering.
 
     Attributes:
         n_clusters (int): Number of clusters.
@@ -46,15 +46,14 @@
         self.tot_withinss = tot_withinss
 
     def _predict(self, x: ArrayLike):
         # predict the cluster for new data
         return vq(x, self.centers)[0]
 
 
-@make_partial_pipe(name="kmeans")
 def kmeans(
     x: ArrayLike,
     n_cluster: int,
     restarts: int = 10,
     max_iters: int = 100,
     dtype: jnp.dtype = jnp.float32,
     *,
@@ -71,14 +70,15 @@
         key (KeyArray, optional): A key array used for encryption. Defaults to None.
 
     Returns:
         KMeansState: An object containing the results of the clustering algorithm.
 
     Example:
         >>> from jax import random
+        >>> from stamox.functions import kmeans
         >>> key = random.PRNGKey(0)
         >>> x = random.normal(key, shape=(100, 2))
         >>> state = kmeans(x, n_cluster=3, restarts=5, max_iters=50, key=key)
         >>> state.centers
         Array([[ 0.8450022 , -1.0791471 ],
                      [-0.7179966 ,  0.6372063 ],
                      [ 0.09818084, -0.25906876]], dtype=float32)
```

### Comparing `stamox-0.1.3/stamox/core/base.py` & `stamox-0.1.4/stamox/core/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-from typing import Callable, Optional, ParamSpec, TypeVar
+from typing import Callable, Optional, TypeVar
 
 import equinox as eqx
 
 
-P = ParamSpec("P")
 T = TypeVar("T")
 
 
 class Functional(eqx.Module):
     """General Function"""
+
     _name: str
-    _fn: Callable[P, T]
-    _is_partial: bool
-    _is_fully_partial: bool
+    _fn: Callable[..., T]
+    _pipe_type: str
 
     def __init__(
         self,
-        fn: Optional[Callable[P, T]] = None,
+        fn: Optional[Callable[..., T]] = None,
+        pipe_type: str = "normal",
         name: str = "Func",
-        is_partial: bool = False,
-        is_fully_partial: bool = False,
     ):
         """Make a General Function.
 
         Args:
             name (str, optional): Name of the function. Defaults to "Func".
+            pipe_type: Type of the function.(vmap or pmap or jit or normal) Defaults to "normal".
             fn (Optional[Callable|None], optional): Callable object.
         """
         super().__init__()
         self._name = name
         self._fn = fn
-        self._is_partial = is_partial
-        self._is_fully_partial = is_fully_partial
-    
-    
+        self._pipe_type = pipe_type
+
     @property
     def name(self):
         """Get the name of the function."""
         return self._name
 
     @property
     def func(self):
         """Get the function."""
         return self._fn
 
+    @property
+    def piep_type(self):
+        """Get the type of the function."""
+        return self._pipe_type
+
     def desc(self):
         """Description for the function."""
         return self.__repr__()
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs):
+    def __call__(self, *args, **kwargs):
         """Call the function with given arguments."""
         if self._fn is None:
             raise ValueError("No Callable Function to Call")
         return self._fn(*args, **kwargs)
 
     def __rshift__(self, _next: Callable):
         """Make Pipe.
@@ -82,15 +84,15 @@
     Args:
         name (str): Name of the state function.
         fn (Optional[Callable]): Function to be called.
     """
 
     def __init__(
         self,
-        fn: Optional[Callable[P, T]] = None,
+        fn: Optional[Callable[..., T]] = None,
         name: str = "State",
     ):
         """Initialize the state function."""
         super().__init__(fn=fn, name=name)
 
     def __repr__(self):
         """Return a string representation of the state function."""
@@ -99,15 +101,15 @@
     def _tree_flatten(self):
         """Flatten the tree structure of the state function."""
         return super()._tree_flatten()
 
     def _summary(self):
         """Print a summary of the state function."""
         pass
-    
+
     def _predict(self, *args, **kwargs):
-        """Predict """
+        """Predict"""
         pass
 
     def __call__(self, *args, **kwargs):
         """Call the state function."""
         return self.func(*args, **kwargs)
```

### Comparing `stamox-0.1.3/stamox/core/jit.py` & `stamox-0.1.4/stamox/core/jit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 from functools import partial, wraps
-from typing import Callable, ParamSpec, TypeVar
+from typing import Callable, TypeVar
 
 from equinox import filter_jit
 
 from .base import Functional
 
 
-P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def pipe_jit(
-    func: Callable[P, T] = None, *, donate: str = "none", name: str = None
-) -> Callable[P, T]:
+    func: Callable[..., T] = None, *, donate: str = "none", name: str = None
+) -> Callable[..., T]:
     """Creates a pipeable jitted functional from a given function.
 
     Args:
         func: The function to create the functional from.
         donate: Optional donation string.
         name: Optional name for the functional.
 
     Returns:
         A callable that creates a functional from the given function.
 
     Example:
-        >>> from stamox.core import pipe_jit
+        >>> from stamox import pipe_jit
         >>> f = lambda x: x + 1
         >>> f = pipe_jit(f)
         >>> g = f >> f >> f
         >>> g(1)
         4
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         fn = filter_jit(func, donate=donate)
 
         return Functional(name=name, fn=fn)
 
     return wrap if func is None else wrap(func)
 
 
 def partial_pipe_jit(
-    func: Callable[P, T] = None, *, name: str = None
-) -> Callable[P, T]:
+    func: Callable[..., T] = None, *, name: str = None
+) -> Callable[..., T]:
     """Creates a partial pipeable jitted functional from a given function.
 
     Args:
         func (Callable[P, T]): _description_
         name (str, optional): _description_. Defaults to None.
 
     Returns:
@@ -65,23 +66,33 @@
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(1)
         7
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
+        if isinstance(func, Functional):
+            if func.func is not None:
+                if func.pipe_type == "pmap" or func.pipe_type == "vmap":
+                    raise ValueError(
+                        "You can not use pmap or vmap with partial_pipe_*, use make_pipe or pipe_* instead."
+                    )
+                func = func.func
+
         @wraps(func)
         def partial_fn(*args, donate: str = "none", **kwargs):
             fn = filter_jit(func, donate=donate)
             fn = partial(fn, **kwargs)
             if len(args) != 0:
                 return fn(*args, **kwargs)
-            return Functional(name=name, fn=fn)
+            return Functional(name=name, fn=fn, pipe_type="jit")
 
         return partial_fn
 
     return wrap if func is None else wrap(func)
```

### Comparing `stamox-0.1.3/stamox/core/maps.py` & `stamox-0.1.4/stamox/core/maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from functools import partial, wraps
-from typing import Callable, Hashable, ParamSpec, TypeVar
+from typing import Callable, Hashable, TypeVar
 
 from equinox import filter_pmap, filter_vmap
 
 from .base import Functional
 
 
-P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def pipe_vmap(
-    func: Callable[P, T] = None,
+    func: Callable[..., T] = None,
     *,
     in_axes=0,
     out_axes=0,
     axis_name: Hashable = None,
-    axis_size: int | None = None,
+    axis_size: int = None,
     name: str = None
-) -> Callable[P, T]:
+) -> Callable[..., T]:
     """Creates a functional from a function with vmap.
 
     Args:
         func: The function to be wrapped.
         in_axes: The number of input axes.
         out_axes: The number of output axes.
         axis_name: The name of the axis.
@@ -30,201 +29,219 @@
         name: The name of the functional. If not provided, the name of the
         function is used.
 
     Returns:
         A callable that creates a functional from the given function.
 
     Example:
-        >>> from stamox.core import pipe_vmap
+        >>> from stamox import pipe_vmap
         >>> f = lambda x: x + 1
         >>> f = pipe_vmap(f)
         >>> g = f >> f >> f
         >>> g(jnp.array([1, 2, 3]))
         Array([4, 5, 6], dtype=int32)
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                func = func.func
         fn = filter_vmap(
             func,
             in_axes=in_axes,
             out_axes=out_axes,
             axis_name=axis_name,
             axis_size=axis_size,
         )
         return Functional(name=name, fn=fn)
 
     return wrap if func is None else wrap(func)
 
 
 def partial_pipe_vmap(
-    func: Callable[P, T] = None, *, name: str = None
-) -> Callable[P, T]:
+    func: Callable[..., T] = None, *, name: str = None
+) -> Callable[..., T]:
     """Partially apply a function to a vmap.
 
     Args:
         func (Callable[P, T]): The function to partially apply.
         name (str, optional): The name of the function. Defaults to None.
 
     Returns:
         Callable[P, T]: A partially applied function.
 
     Example:
-        >>> from stamox.core import partial_pipe_vmap
+        >>> from stamox import partial_pipe_vmap
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_vmap(f)
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(jnp.array([1, 2, 3]))
         Array([7, 8, 9], dtype=int32)
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
         else:
             name = func.__name__
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                if func.pipe_type == "pmap" or func.pipe_type == "vmap":
+                    raise ValueError(
+                        "You can not use pipe_pmap or pipe_vmap with partial_pipe_*, use make_pipe or pipe_* instead."
+                    )
+                func = func.func
 
         @wraps(func)
         def partial_fn(
             *args,
             in_axes=0,
             out_axes=0,
             axis_name: Hashable = None,
-            axis_size: int | None = None,
+            axis_size: int = None,
             **kwargs
         ):
             fn = partial(func, **kwargs)
             fn = filter_vmap(
                 fn,
                 in_axes=in_axes,
                 out_axes=out_axes,
                 axis_name=axis_name,
                 axis_size=axis_size,
             )
             if len(args) != 0:
                 return fn(*args)
-            return Functional(name=name, fn=fn)
+            return Functional(name=name, fn=fn, pipe_type="vmap")
 
         return partial_fn
 
     return wrap if func is None else wrap(func)
 
 
 def pipe_pmap(
-    func: Callable[P, T] = None,
+    func: Callable[..., T] = None,
     *,
     in_axes=0,
     out_axes=0,
     axis_name: Hashable = None,
-    axis_size: int | None = None,
+    axis_size: int = None,
     name: str = None
-) -> Callable[P, T]:
+) -> Callable[..., T]:
     """Creates a functional object from a given function.
 
     Args:
         func (Callable[P, T]): The function to be wrapped.
         in_axes (int): The number of input axes for the function.
         out_axes (int): The number of output axes for the function.
         axis_name (Hashable): The name of the axis.
-        axis_size (int | None): The size of the axis.
+        axis_size (int ): The size of the axis.
         name (str): The name of the functional object.
 
     Returns:
         Callable[P, T]: A callable object that wraps the given function.
 
     Example:
-        >>> from stamox.core import pipe_pmap
+        >>> from stamox import pipe_pmap
         >>> f = lambda x: x + 1
         >>> f = pipe_pmap(f)
         >>> g = f >> f >> f
         >>> g(jnp.array([1, 2, 3]))
         Array([4, 5, 6], dtype=int32)
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                if func.pipe_type == "pmap" or func.pipe_type == "vmap":
+                    raise ValueError(
+                        "You can not use pipe_pmap or pipe_vmap with partial_pipe_*, use make_pipe or pipe_* instead."
+                    )
+                func = func.func
         fn = filter_pmap(
             func,
             in_axes=in_axes,
             out_axes=out_axes,
             axis_name=axis_name,
             axis_size=axis_size,
         )
 
-        return Functional(name=name, fn=fn)
+        return Functional(name=name, fn=fn, pipe_type="pmap")
 
     return wrap if func is None else wrap(func)
 
 
 def partial_pipe_pmap(
-    func: Callable[P, T] = None, *, name: str = None
-) -> Callable[P, T]:
+    func: Callable[..., T] = None, *, name: str = None
+) -> Callable[..., T]:
     """Partially apply a function to a pipe.
 
     Args:
         func (Callable[P, T]): The function to partially apply.
         name (str, optional): The name of the function. Defaults to None.
 
     Returns:
         Callable[P, T]: A partially applied function.
 
     Example:
-        >>> from stamox.core import partial_pipe_pmap
+        >>> from stamox import partial_pipe_pmap
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_pmap(f)
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(jnp.array([1, 2, 3]))
         Array([7, 8, 9], dtype=int32)
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                func = func.func
 
         @wraps(func)
         def partial_fn(
             *args,
             in_axes=0,
             out_axes=0,
             axis_name: Hashable = None,
-            axis_size: int | None = None,
+            axis_size: int = None,
             **kwargs
         ):
             fn = partial(func, **kwargs)
             fn = filter_pmap(
                 fn,
                 in_axes=in_axes,
                 out_axes=out_axes,
                 axis_name=axis_name,
                 axis_size=axis_size,
             )
             if len(args) != 0:
                 return fn(*args, **kwargs)
-            return Functional(name=name, fn=fn, is_partial=True)
+            return Functional(name=name, fn=fn, pipe_type="pmap")
 
         return partial_fn
 
     return wrap if func is None else wrap(func)
```

### Comparing `stamox-0.1.3/stamox/core/pipe.py` & `stamox-0.1.4/stamox/core/pipe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from functools import partial, wraps
 from typing import (
     Any,
     Callable,
     Optional,
-    ParamSpec,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
 import equinox as eqx
 
 from .base import Functional
 
 
-P = ParamSpec("P")
 T = TypeVar("T")
 
 
 class Pipe(eqx.Module):
     """A class for creating a pipe of functions.
 
     Attributes:
@@ -32,24 +30,14 @@
         """Initialize the Pipe object.
 
         Args:
             funcs (Sequence[Functional]): A sequence of Functional objects.
         """
         self.funcs = tuple(funcs)
 
-    def _debug_call(self, x: Any = None, *args, **kwargs):
-        for fn in self.funcs:
-            if fn._is_fully_partial:
-                print(f"{fn.name} called, function info: {fn.desc()}")
-                x = fn()
-                continue
-            print(f"{fn.name} called, function info: {fn.desc()}")
-            x = fn(x, *args, **kwargs)
-        return x
-
     def __call__(self, x: Any = None, *args, **kwargs):
         """Call the Pipe object.
 
         Args:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
 
@@ -154,83 +142,95 @@
         Returns:
             Any: The piped value.
         """
         return self.value
 
 
 def make_pipe(
-    func: Optional[Callable[P, T]] = None, name: str = None
-) -> Callable[P, T]:
+    func: Optional[Callable[..., T]] = None, name: str = None
+) -> Callable[..., T]:
     """Makes a Function Pipeable.
 
     Args:
         func (Callable): Function or Callable Class.
         name (str, optional): Name of the Function. Defaults to "PipeableFunc".
         kwargs (optional): Additional keyword arguments.
 
     Returns:
         Callable: The wrapped function.
 
     Examples:
+        >>> from stamox import make_pipe
         >>> @make_pipe
         ... def add(x):
         ...     return x + 1
         >>> h = add >> add >> add
         >>> h(1)
         4
     """
 
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable[P, T]:
+    def wrap(func: Callable[..., T]) -> Callable[..., T]:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                func = func.func
 
         functional = Functional(name=name, fn=func)
         return functional
 
     return wrap if func is None else wrap(func)
 
 
 def make_partial_pipe(
-    func: Optional[Callable[P, T]] = None, name: str = None
-) -> Callable[P, T]:
+    func: Optional[Callable[..., T]] = None, name: str = None
+) -> Callable[..., T]:
     """Makes a Partial Function Pipe.
 
     Args:
         func (Callable): Function or Callable Class.
         name (str, optional): Name of the Function. Defaults to "PipeableFunc".
         kwargs (dict): Keyword arguments for the function.
 
     Returns:
         Callable: A partial function pipe.
 
     Examples:
+        >>> from stamox import make_partial_pipe
         >>> @make_partial_pipe
         ... def add(x, y):
         ...     return x + y
         >>> h = add(y=1) >> add(y=2) >> add(y=3)
         >>> h(1)
         7
     """
     if name is None and func is not None:
         if hasattr(func, "name"):
             name = func.name
-        else:
+        elif hasattr(func, "__name__"):
             name = func.__name__
+        else:
+            name = "none"
 
     @wraps(func)
-    def wrap(func: Callable[P, T]) -> Callable:
+    def wrap(func: Callable[..., T]) -> Callable:
         if isinstance(func, Functional):
-            func = func.func
+            if func.func is not None:
+                if func.pipe_type == "pmap" or func.pipe_type == "vmap":
+                    raise ValueError(
+                        "You can not use pipe_pmap or piep_vmap with make_partial_pipe, use make_pipe or pipe_* instead."
+                    )
+                func = func.func
 
         @wraps(func)
         def partial_fn(*args, **kwargs):
             if len(args) != 0:
                 return func(*args, **kwargs)
             fn = partial(func, **kwargs)
             return Functional(name=name, fn=fn)
```

### Comparing `stamox-0.1.3/stamox/distribution/__init__.py` & `stamox-0.1.4/stamox/distribution/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from stamox.distribution._gamma import dgamma, pgamma, qgamma, rgamma
 from stamox.distribution._laplace import dlaplace, plaplace, qlaplace, rlaplace
 from stamox.distribution._normal import dnorm, pnorm, qnorm, rnorm
 from stamox.distribution._pareto import dpareto, ppareto, qpareto, rpareto
 from stamox.distribution._poisson import dpoisson, ppoisson, qpoisson, rpoisson
 from stamox.distribution._t import dt, pt, qt, rt
 from stamox.distribution._uniform import dunif, punif, qunif, runif
+from stamox.distribution._weibull import dweibull, pweibull, qweibull, rweibull
 
 
 __all__ = [
     "pt",
     "qt",
     "rt",
     "dt",
@@ -65,8 +66,12 @@
     "dexp",
     "plaplace",
     "qlaplace",
     "dlaplace",
     "rlaplace",
     "ecdf",
     "step_fun",
+    "pweibull",
+    "qweibull",
+    "dweibull",
+    "rweibull",
 ]
```

### Comparing `stamox-0.1.3/stamox/distribution/_beta.py` & `stamox-0.1.4/stamox/distribution/_beta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,156 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import KeyArray, Shape
-from jax.scipy.special import betainc
 from jaxtyping import ArrayLike, Float
 from tensorflow_probability.substrates.jax.math import special as tfp_special
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pbeta(
     x: Union[Float, ArrayLike], a: Union[Float, ArrayLike], b: Union[Float, ArrayLike]
 ):
-    return betainc(a, b, x)
+    dtype = lax.dtype(x)
+    a = jnp.asarray(a, dtype=dtype)
+    b = jnp.asarray(b, dtype=dtype)
+    return tfp_special.betainc(a, b, x)
 
 
-@make_partial_pipe
 def pbeta(
     q: Union[Float, ArrayLike],
     a: Union[Float, ArrayLike],
     b: Union[Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the cumulative distribution function of the beta distribution.
 
     Args:
         q (Union[Float, ArrayLike]): Quantiles.
         a (Union[Float, ArrayLike]): Shape parameter.
         b (Union[Float, ArrayLike]): Shape parameter.
         lower_tail (bool, optional): If True (default), probabilities are P[X ≤ x], otherwise, P[X > x].
         log_prob (bool, optional): If True, probabilities are given as log(P).
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to None.
 
     Returns:
         ArrayLike: The probability or log of the probability for each quantile.
 
     Example:
         >>> q = jnp.array([0.1, 0.5, 0.9])
         >>> a = 2.0
         >>> b = 3.0
         >>> pbeta(q, a, b)
         Array([0.05230004, 0.68749976, 0.9963    ], dtype=float32)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q, 0.0, 1.0)
     p = filter_vmap(_pbeta)(q, a, b)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dbeta = filter_jit(filter_grad(_pbeta))
 
 
-@make_partial_pipe
 def dbeta(
     x: Union[Float, ArrayLike],
     a: Union[Float, ArrayLike],
     b: Union[Float, ArrayLike],
-    lower_tail=True,
-    log_prob=False,
-    dtype = jnp.float32,
+    lower_tail: bool = True,
+    log_prob: bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the probability density function of the beta distribution.
 
     Args:
       x: A float or array-like object representing the value(s) at which to evaluate the PDF.
       a: A float or array-like object representing the shape parameter of the beta distribution.
       b: A float or array-like object representing the scale parameter of the beta distribution.
       lower_tail: A boolean indicating whether to calculate the lower tail (default True).
       log_prob: A boolean indicating whether to return the logarithm of the PDF (default False).
-      dtype: The dtype of the output. Defaults to jnp.float32.
+      dtype: The dtype of the output. Defaults to None.
 
     Returns:
       ArrayLike: The probability density function of the beta distribution evaluated at x.
 
     Example:
         >>> dbeta(0.5, 2, 3, lower_tail=True, log_prob=False)
         Array([1.4999996], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, dtype = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
-    p = filter_vmap(_dbeta)(x, a, b)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
-    return p
+    x = _check_clip_distribution_domain(x, 0.0, 1.0)
+    d = filter_vmap(_dbeta)(x, a, b)
+    d = _post_process(d, lower_tail, log_prob)
+    return d
 
 
 @filter_jit
 def _qbeta(
     p: Union[Float, ArrayLike], a: Union[Float, ArrayLike], b: Union[Float, ArrayLike]
 ):
     return tfp_special.betaincinv(a, b, p)
 
 
-@make_partial_pipe
 def qbeta(
     p: Union[Float, ArrayLike],
     a: Union[Float, ArrayLike],
     b: Union[Float, ArrayLike],
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the quantile of beta distribution function.
 
     Args:
         p: A float or array-like object representing the quantile.
         a: A float or array-like object representing the alpha parameter.
         b: A float or array-like object representing the beta parameter.
         lower_tail: A boolean indicating whether to compute the lower tail of the
         distribution (defaults to True).
         log_prob: A boolean indicating whether to compute the log probability
         (defaults to False).
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to None.
 
     Returns:
         ArrayLike: The value of the beta distribution at the given quantile.
 
     Example:
-        >>> qbeta(0.5, 2, 3, lower_tail=True, log_prob=False)
+        >>> qbeta(0.5, 2, 3)
         Array([0.38572744], dtype=float32)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, dtype = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail=lower_tail, log_prob=log_prob)
     x = filter_vmap(_qbeta)(p, a, b)
     return x
 
 
-@make_partial_pipe
 def rbeta(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     a: Union[Float, ArrayLike] = None,
     b: Union[Float, ArrayLike] = None,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random numbers from the Beta distribution.
 
     Args:
         key: A PRNGKey used for random number generation.
         sample_shape: An optional shape for the output samples.
         a: The shape parameter of the Beta distribution. Can be either a float or an array-like object.
@@ -166,28 +163,25 @@
         ArrayLike: Random numbers from the Beta distribution.
 
     Example:
         >>> key = jax.random.PRNGKey(0)
         >>> rbeta(key, sample_shape=(3,), a=2, b=3)
         Array([0.02809353, 0.13760717, 0.49360353], dtype=float32)
     """
-    rvs = _rbeta(key, a, b, sample_shape)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _rbeta(key, a, b, sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
 
 
 @filter_jit
 def _rbeta(
     key: KeyArray,
     a: Union[Float, ArrayLike],
     b: Union[Float, ArrayLike],
     sample_shape: Optional[Shape] = None,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(a), jnp.shape(b))
     a = jnp.broadcast_to(a, sample_shape)
     b = jnp.broadcast_to(b, sample_shape)
     return jrand.beta(key, a, b, sample_shape, dtype=dtype)
```

### Comparing `stamox-0.1.3/stamox/distribution/_binomial.py` & `stamox-0.1.4/stamox/distribution/_binomial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,186 @@
 from typing import Optional
 
 import jax.numpy as jnp
-import numpy as np
 from equinox import filter_jit, filter_vmap
 from jax import pure_callback, ShapeDtypeStruct
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Bool
 from scipy.stats import binom
 from tensorflow_probability.substrates.jax.distributions import Binomial as tfp_Binomial
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pbinom(q, size, prob) -> ArrayLike:
+    size = jnp.asarray(size, dtype=q.dtype)
+    prob = jnp.asarray(prob, dtype=q.dtype)
     bino = tfp_Binomial(total_count=size, probs=prob)
     return bino.cdf(q)
 
 
-@make_partial_pipe
 def pbinom(
     q: ArrayLike,
     size: ArrayLike,
     prob: ArrayLike,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the cumulative probability of a binomial distribution.
 
     Args:
         q (ArrayLike): The quantiles to compute.
         size (ArrayLike): The number of trials.
         prob (ArrayLike): The probability of success in each trial.
         lower_tail (Bool, optional): If True (default), the lower tail probability is returned.
         log_prob (Bool, optional): If True, the logarithm of the probability is returned.
-        dtype (optional): The data type of the output array. Defaults to jnp.float32.
+        dtype (optional): The data type of the output array. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cumulative probability of the binomial distribution.
 
     Example:
         >>> q = jnp.array([0.1, 0.5, 0.9])
         >>> size = 10
         >>> prob = 0.5
         >>> pbinom(q, size, prob)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q, 0, size)
     p = filter_vmap(_pbinom)(q, size, prob)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 @filter_jit
 def _dbinom(q, size, prob) -> ArrayLike:
+    size = jnp.asarray(size, dtype=q.dtype)
+    prob = jnp.asarray(prob, dtype=q.dtype)
     bino = tfp_Binomial(total_count=size, probs=prob)
     return bino.prob(q)
 
 
-@make_partial_pipe
 def dbinom(
     q: ArrayLike,
     size: ArrayLike,
     prob: ArrayLike,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the probability of a binomial distribution.
 
     Args:
         q (ArrayLike): The value to compute the probability for.
         size (ArrayLike): The number of trials in the binomial distribution.
         prob (ArrayLike): The probability of success in each trial.
         lower_tail (Bool, optional): Whether to compute the lower tail probability. Defaults to True.
         log_prob (Bool, optional): Whether to return the logarithm of the probability. Defaults to False.
-        dtype (jnp.float32, optional): The data type of the output array. Defaults to jnp.float32.
+        dtype (jnp.float_, optional): The data type of the output array. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability of the binomial distribution.
+
+    Example:
+        >>> q = jnp.array([0.1, 0.5, 0.9])
+        >>> size = 10
+        >>> prob = 0.5
+        >>> dbinom(q, size, prob)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_dbinom)(q, size, prob)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
-    return p
+    d = filter_vmap(_dbinom)(q, size, prob)
+    d = _post_process(d, lower_tail, log_prob)
+    return d
 
 
 @filter_jit
 def _qbinom(p, size, prob, dtype) -> ArrayLike:
     result_shape_type = ShapeDtypeStruct(jnp.shape(p), dtype)
-    _scp_binom_ppf = lambda x: binom(size, prob).ppf(x).astype(np.int32)
+    _scp_binom_ppf = lambda x: binom(size, prob).ppf(x).astype(dtype)
     q = pure_callback(_scp_binom_ppf, result_shape_type, p)
     return q
 
 
-@make_partial_pipe
 def qbinom(
     p: ArrayLike,
     size: ArrayLike,
     prob: ArrayLike,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.int32,
+    dtype=jnp.int_,
 ) -> ArrayLike:
     """Computes the quantile of a binomial distribution.
 
     Args:
         p (ArrayLike): The probability of success.
         size (ArrayLike): The number of trials.
         prob (ArrayLike): The probability of success in each trial.
         lower_tail (Bool, optional): Whether to compute the lower tail or not. Defaults to True.
         log_prob (Bool, optional): Whether to compute the log probability or not. Defaults to False.
-        dtype (jnp.int32, optional): The data type of the output array. Defaults to jnp.int32.
+        dtype (jnp.int_, optional): The data type of the output array. Defaults to jnp.int_.
 
     Returns:
         ArrayLike: The quantile of the binomial distribution.
+
+    Example:
+        >>> p = jnp.array([0.1, 0.5, 0.9])
+        >>> size = 10
+        >>> prob = 0.5
+        >>> qbinom(p, size, prob)
     """
-    p = jnp.asarray(p)
+    if dtype is None:
+        dtype = jnp.int_
+    p = jnp.asarray(p, dtype=jnp.float_)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-
+    p = _check_clip_probability(p, lower_tail, log_prob)
     q = filter_vmap(_qbinom)(p, size, prob, dtype)
     return q
 
 
 @filter_jit
-def _rbinom(key, n, prob, sample_shape, dtype) -> ArrayLike:
-    bino = tfp_Binomial(total_count=n, probs=prob)
+def _rbinom(key, size, prob, sample_shape, dtype) -> ArrayLike:
+    bino = tfp_Binomial(total_count=size, probs=prob)
     return bino.sample(sample_shape=sample_shape, seed=key).astype(dtype)
 
 
-@make_partial_pipe
 def rbinom(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    n: ArrayLike = None,
+    size: ArrayLike = None,
     prob: ArrayLike = None,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.int_,
 ) -> ArrayLike:
     """Generates random binomial samples from a given probability distribution.
 
     Args:
         key (KeyArray): A random number generator key.
         sample_shape (Optional[Shape], optional): The shape of the output array. Defaults to None.
-        n (ArrayLike, optional): The number of trials. Defaults to None.
+        size (ArrayLike, optional): The number of trials. Defaults to None.
         prob (ArrayLike, optional): The probability of success for each trial. Defaults to None.
         lower_tail (Bool, optional): Whether to return the lower tail of the distribution. Defaults to True.
         log_prob (Bool, optional): Whether to return the logarithm of the probability. Defaults to False.
         dtype (jnp.float32, optional): The data type of the output array. Defaults to jnp.float32.
 
     Returns:
         ArrayLike: An array containing the random binomial samples.
+
+    Example:
+        >>> key = jax.random.PRNGKey(0)
+        >>> sample_shape = (3, 3)
+        >>> size = 10
+        >>> prob = 0.5
+        >>> rbinom(key, sample_shape, size, prob)
     """
-    rvs = _rbinom(key, n, prob, sample_shape, dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _rbinom(key, size, prob, sample_shape, dtype)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/distribution/_cauchy.py` & `stamox-0.1.4/stamox/distribution/_cauchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,171 +1,175 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jaxtyping import ArrayLike, Bool, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pcauchy(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ) -> ArrayLike:
+    dtype = lax.dtype(x)
+    loc = jnp.asarray(loc, dtype=dtype)
+    scale = jnp.asarray(scale, dtype=dtype)
     scaled = (x - loc) / scale
     return jnp.arctan(scaled) / jnp.pi + 0.5
 
 
-@make_partial_pipe
 def pcauchy(
     q: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the cumulative denisty probability c function of the Cauchy distribution.
 
     Args:
         q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
         loc (Union[Float, ArrayLike], optional): The location parameter of the Cauchy distribution. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): The scale parameter of the Cauchy distribution. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to return the lower tail probability. Defaults to True.
         log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cumulative density function of the Cauchy distribution.
 
     Example:
         >>> pcauchy(1.0, loc=0.0, scale=1.0, lower_tail=True, log_prob=False)
         Array([0.75], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q)
     p = filter_vmap(_pcauchy)(q, loc, scale)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dcauchy = filter_grad(filter_jit(_pcauchy))
 
 
-@make_partial_pipe
 def dcauchy(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the pdf of the Cauchy distribution.
 
     Args:
         x (Union[Float, ArrayLike]): The input values.
         loc (Union[Float, ArrayLike], optional): The location parameter. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): The scale parameter. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to compute the lower tail. Defaults to True.
         log_prob (Bool, optional): Whether to compute the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The pdf of the Cauchy distribution.
 
     Example:
-        >>> dcauchy(1.0, loc=0.0, scale=1.0, lower_tail=True, log_prob=False)
+        >>> dcauchy(1.0, loc=0.0, scale=1.0)
         Array([0.15915494], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, dtype = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x)
     grads = filter_vmap(_dcauchy)(x, loc, scale)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qcauchy(
     q: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ):
-    return loc + scale * jnp.tan(jnp.pi * (q - 0.5))
+    dtype = lax.dtype(q)
+    loc = jnp.asarray(loc, dtype=dtype)
+    scale = jnp.asarray(scale, dtype=dtype)
+    return lax.add(loc, lax.mul(scale, lax.tan(lax.mul(jnp.pi, lax.sub(q, 0.5)))))
 
 
-@make_partial_pipe
 def qcauchy(
     q: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the quantile of the Cauchy distribution.
 
     Args:
         q (Union[float, array-like]): Quantiles to compute.
         loc (Union[float, array-like], optional): Location parameter. Defaults to 0.0.
         scale (Union[float, array-like], optional): Scale parameter. Defaults to 1.0.
         lower_tail (bool, optional): Whether to compute the lower tail. Defaults to True.
         log_prob (bool, optional): Whether to compute the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantiles of the Cauchy distribution.
 
     Example:
-        >>> qcauchy(0.5, loc=1.0, scale=2.0, lower_tail=True, log_prob=False)
+        >>> qcauchy(0.5, loc=1.0, scale=2.0)
         Array([1.], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    if not lower_tail:
-        q = 1 - q
-    if log_prob:
-        q = jnp.exp(q)
+    q = _check_clip_probability(q, lower_tail, log_prob)
     return filter_vmap(_qcauchy)(q, loc, scale)
 
 
+@filter_jit
 def _rcauchy(
     key: KeyArray,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
     loc = jnp.broadcast_to(loc, sample_shape)
     scale = jnp.broadcast_to(scale, sample_shape)
+    loc = jnp.asarray(loc, dtype=dtype)
+    scale = jnp.asarray(scale, dtype=dtype)
     return jrand.cauchy(key, sample_shape, dtype=dtype) * scale + loc
 
 
-@make_partial_pipe
 def rcauchy(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random samples from the Cauchy distribution.
 
     Args:
         key: A PRNGKey to use for generating the samples.
         sample_shape: The shape of the output array.
         loc: The location parameter of the Cauchy distribution.
@@ -180,12 +184,9 @@
     Example:
         >>> key = jax.random.PRNGKey(0)
         >>> rcauchy(key, sample_shape=(2, 3), loc=0.0, scale=1.0)
         Array([[ 0.23841971, -3.0880406 ,  0.9507532 ],
                 [ 2.8963416 ,  0.31303588, -0.14792857]], dtype=float32)
     """
     rvs = _rcauchy(key, loc, scale, sample_shape, dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/distribution/_chisq.py` & `stamox-0.1.4/stamox/distribution/_poisson.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,169 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_jit, filter_vmap
-from jax._src.random import KeyArray, Shape
-from jaxtyping import ArrayLike, Float, Int
+from jax import pure_callback, ShapeDtypeStruct
+from jax._src.random import Shape
+from jax.random import KeyArray
+from jax.scipy.special import gammainc, gammaln
+from jaxtyping import Array, ArrayLike, Bool, Float
+from scipy.stats import poisson
+
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
-from ..core import make_partial_pipe
-from ._gamma import _dgamma, _pgamma, _qgamma
 
-
-@make_partial_pipe
-def dchisq(
-    x: Union[Float, ArrayLike],
-    df: Union[Int, Float, ArrayLike],
-    lower_tail=True,
-    log_prob=False,
-    dtype=jnp.float32,
-) -> ArrayLike:
-    """Computes the chi-squared distribution.
-
-    Args:
-        x: A float or array-like object representing the values at which to evaluate the chi-squared distribution.
-        df: The degrees of freedom for the chi-squared distribution.
-        lower_tail: A boolean indicating whether to compute the lower tail of the chi-squared distribution (defaults to True).
-        log_prob: A boolean indicating whether to return the log probability (defaults to False).
-        dtype: The dtype of the output (defaults to float32).
-
-    Returns:
-        ArrayLike: The chi-squared distribution evaluated at `x`.
-
-    Example:
-        >>> dchisq(2.0, 3, lower_tail=True, log_prob=False)
-        Array([0.20755368], dtype=float32, weak_type=True)
-    """
-    x = jnp.asarray(x, dtype=dtype)
-    x = jnp.atleast_1d(x)
-    grads = filter_vmap(_dgamma)(x, df / 2, 1 / 2)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
-    return grads
+@filter_jit
+def _ppoisson(x: Union[Float, ArrayLike], rate: Union[Float, ArrayLike]) -> Array:
+    k = jnp.floor(x) + 1.0
+    return 1 - gammainc(k, rate)
 
 
-@make_partial_pipe
-def pchisq(
+def ppoisson(
     q: Union[Float, ArrayLike],
-    df: Union[Int, Float, ArrayLike],
+    rate: Union[Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Calculates the chi-squared probability density function.
+    """Computes the cumulative distribution function of the Poisson distribution.
 
     Args:
-        q (Union[float, array-like]): The value of the chi-squared variable.
-        df (Union[int, float, array-like]): The degrees of freedom.
-        lower_tail (bool): Whether to calculate the lower tail (default True).
-        log_prob (bool): Whether to return the log probability (default False).
-        dtype (dtype): The dtype of the output (default float32).
+        q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
+        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The chi-squared probability density function.
+        ArrayLike: The cumulative distribution function of the Poisson distribution evaluated at `q`.
 
     Example:
-        >>> pchisq(2.0, 3, lower_tail=True, log_prob=False)
-        Array([0.42759317], dtype=float32, weak_type=True)
+        >>> ppoisson(1.0, rate=1.0)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, dtype = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_pgamma)(q, df / 2, 1 / 2)
-    if not lower_tail:
-        p = 1.0 - p
-    if log_prob:
-        p = jnp.log(p)
+    q = _check_clip_distribution_domain(q, lower=0.0)
+    p = filter_vmap(_ppoisson)(q, rate)
+    p = _post_process(p, lower_tail=lower_tail, log_prob=log_prob)
     return p
 
 
-@make_partial_pipe
-def qchisq(
-    p: Union[Float, ArrayLike],
-    df: Union[Int, Float, ArrayLike],
+@filter_jit
+def _dpoisson(x, rate):
+    e = jnp.exp(-rate)
+    numerator = rate**x
+    denominator = jnp.exp(gammaln(x + 1))
+    return (numerator / denominator) * e
+
+
+def dpoisson(
+    x: Union[Float, ArrayLike],
+    rate: Union[Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the inverse of the chi-squared cumulative distribution function.
+    """Computes the probability density function of the Poisson distribution.
 
     Args:
-        p (Union[Float, ArrayLike]): Probability value or array of probability values.
-        df (Union[Int, Float, ArrayLike]): Degrees of freedom.
-        lower_tail (bool, optional): If True (default), probabilities are P[X ≤ x], otherwise, P[X > x].
-        log_prob (bool, optional): If True, probabilities are given as log(p).
-        dtype (dtype, optional): The dtype of the output (default float32).
+        x (Union[Float, ArrayLike]): The value at which to evaluate the PDF.
+        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail of the PDF. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The quantiles corresponding to the given probabilities.
+        ArrayLike: The probability density function of the Poisson distribution evaluated at `x`.
 
-    Example:
-        >>> qchisq(0.95, 10)
-        Array([18.307034], dtype=float32)
+    Examples:
+        >>> dpoisson(1.0, rate=1.0)
     """
-    p = jnp.asarray(p, dtype=dtype)
-    p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-    q = filter_vmap(_qgamma)(p, df / 2, 1 / 2)
-    return q
+    x, _ = _promote_dtype_to_floating(x, dtype)
+    x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x, lower=0.0)
+    grads = filter_vmap(_dpoisson)(x, rate)
+    grads = _post_process(grads, lower_tail=lower_tail, log_prob=log_prob)
+    return grads
 
 
 @filter_jit
-def _rchisq(
+def _rpoisson(
     key: KeyArray,
-    df: Union[Int, Float, ArrayLike],
+    rate: Union[Float, ArrayLike],
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.int_,
 ):
-    if sample_shape is None:
-        sample_shape = jnp.shape(df)
-    df = jnp.broadcast_to(df, sample_shape)
-    return jrand.chisquare(key, df, shape=sample_shape, dtype=dtype)
+    return jrand.poisson(key, rate, shape=sample_shape, dtype=dtype)
 
 
-@make_partial_pipe
-def rchisq(
+def rpoisson(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    df: Union[Int, Float, ArrayLike] = None,
+    rate: Union[Float, ArrayLike] = None,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.int_,
 ) -> ArrayLike:
-    """
-    Generates random variates from the chi-squared distribution.
+    """Generates samples from the Poisson distribution.
 
     Args:
-        key (KeyArray): Random key to generate the random numbers.
+        key (KeyArray): Random number generator state used for random sampling.
+        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
         sample_shape (Optional[Shape], optional): Shape of the output array. Defaults to None.
-        df (Union[Int, Float, ArrayLike], optional): Degrees of freedom. Defaults to None.
         lower_tail (bool, optional): Whether to return the lower tail probability. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (dtype, optional): The dtype of the output (default float32).
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int_.
 
     Returns:
-        ArrayLike: Random variates from the chi-squared distribution.
+        ArrayLike: Samples from the Poisson distribution.
 
-    Example:
-        >>> key = jax.random.PRNGKey(0)
-        >>> rchisq(key, df=2)
-        Array(1.982825, dtype=float32)
+    Examples:
+        >>> key = jrand.PRNGKey(0)
+        >>> rpoisson(key, rate=1.0)
     """
-    rvs = _rchisq(key, df, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _rpoisson(key, rate, sample_shape=sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail=lower_tail, log_prob=log_prob)
     return rvs
+
+
+@filter_jit
+def _qpoisson(q, rate, dtype):
+    result_shape_type = ShapeDtypeStruct(jnp.shape(q), dtype)
+    _scp_poisson_ppf = lambda q, rate: poisson(rate).ppf(q).astype(dtype)
+    p = pure_callback(_scp_poisson_ppf, result_shape_type, q, rate)
+    return p
+
+
+def qpoisson(
+    p: Union[Float, ArrayLike],
+    rate: Union[Float, ArrayLike],
+    lower_tail: Bool = True,
+    log_prob: Bool = False,
+    dtype=jnp.int_,
+) -> ArrayLike:
+    """Computes the quantile function of the Poisson distribution.
+
+    Args:
+        p (Union[Float, ArrayLike]): The probability at which to evaluate the quantile function.
+        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail of the quantile function. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int_.
+
+    Returns:
+        ArrayLike: The quantile function of the Poisson distribution evaluated at `p`.
+
+    Example:
+        >>> qpoisson(0.5, rate=1.0)
+    """
+    p, _ = _promote_dtype_to_floating(p, None)
+    p = jnp.atleast_1d(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
+    q = filter_vmap(_qpoisson)(p, rate, dtype)
+    return q
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stamox-0.1.3/stamox/distribution/_ecdf.py` & `stamox-0.1.4/stamox/distribution/_ecdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from typing import Callable
 
 import jax.numpy as jnp
 from jax import jit
 from jaxtyping import ArrayLike
 
-from ..core import make_partial_pipe
 
-
-def step_fun(x, y, ival=0.0, sorted=False, side="left", dtype=jnp.float32):
+def step_fun(x, y, ival=0.0, sorted=False, side="left", dtype=jnp.float_):
     """Returns a function that evaluates a step function at given points.
 
     Args:
         x (array-like): The x-coordinates of the step points.
         y (array-like): The y-coordinates of the step points.
         ival (float, optional): The initial value of the step function. Defaults to 0.
         sorted (bool, optional): Whether the x-coordinates are already sorted. Defaults to False.
         side (str, optional): The side of the interval to take when evaluating the step function. Must be either 'left' or 'right'. Defaults to 'left'.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         Callable[..., ArrayLike]: A function that evaluates the step function at given points.
     """
     if side.lower() not in ["right", "left"]:
         raise ValueError("side must be left or right")
 
@@ -33,31 +31,30 @@
     if not sorted:
         asort = jnp.argsort(_x)
         _x = jnp.take(_x, asort, 0)
         _y = jnp.take(_y, asort, 0)
 
     @jit
     def _call(time):
-        time = jnp.asarray(time)
+        time = jnp.asarray(time, dtype=dtype)
         tind = jnp.searchsorted(_x, time, side) - 1
         return _y[tind]
 
     return _call
 
 
-@make_partial_pipe
-def ecdf(x: ArrayLike, side="right", dtype=jnp.float32) -> Callable[..., ArrayLike]:
+def ecdf(x: ArrayLike, side="right", dtype=jnp.float_) -> Callable[..., ArrayLike]:
     """Calculates the empirical cumulative distribution function (ECDF) of a given array.
 
     Args:
         x (array): The array to calculate the ECDF for.
         side (str, optional): Specifies which side of the step function to use. Defaults to 'right'.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         Callable[..., ArrayLike]: A function that evaluates the ECDF at given points.
     """
-    x = jnp.array(x, copy=True, dtype=dtype)
+    x = jnp.asarray(x, dtype=dtype)
     x = jnp.sort(x)
     nobs = x.size
-    y = jnp.linspace(1.0 / nobs, 1, nobs)
+    y = jnp.linspace(1.0 / nobs, 1, nobs, dtype=dtype)
     return step_fun(x, y, side=side, sorted=True)
```

### Comparing `stamox-0.1.3/stamox/distribution/_exp.py` & `stamox-0.1.4/stamox/distribution/_exp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,161 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pexp(x: Union[float, ArrayLike], rate: float) -> Float:
     return -jnp.expm1(-rate * x)
 
 
-@make_partial_pipe
 def pexp(
     q: Union[Float, ArrayLike],
     rate: Union[Float, ArrayLike],
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the probability of a given value or array of values for an exponential distribution.
 
     Args:
         q: Union[Float, ArrayLike]. The value or array of values to calculate the probability of.
         rate: Union[Float, ArrayLike]. The rate parameter of the exponential distribution.
         lower_tail: bool, optional. Whether to return the lower tail probability (default is True).
         log_prob: bool, optional. Whether to return the log probability (default is False).
-        dtype: jnp.dtype, optional. The dtype of the output (default is float32).
+        dtype: jnp.dtype, optional. The dtype of the output (default is float_).
 
     Returns:
         ArrayLike: The probability of the given value or array of values.
 
     Example:
         >>> pexp(1.0, 0.5)
         Array([0.39346933], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q, 0)
     p = filter_vmap(_pexp)(q, rate)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 @filter_jit
 def _qexp(q: Union[float, ArrayLike], rate: float) -> Float:
-    return -jnp.log1p(-q) / rate
+    dtype = lax.dtype(q)
+    rate = lax.convert_element_type(rate, dtype)
+    return -lax.div(lax.log1p(-q), rate)
 
 
-@make_partial_pipe
 def qexp(
     p: Union[float, ArrayLike],
     rate: Union[float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the quantile of an exponential distribution.
 
     Args:
         p (Union[float, ArrayLike]): Probability or log probability.
         rate (Union[float, ArrayLike]): Rate parameter of the exponential distribution.
         lower_tail (bool, optional): Whether to compute the lower tail. Defaults to True.
         log_prob (bool, optional): Whether `p` is a log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantile of the exponential distribution.
 
     Example:
         >>> qexp(0.5, 1.0)
         Array([0.6931472], dtype=float32, weak_type=True)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
     x = filter_vmap(_qexp)(p, rate)
     return x
 
 
 _dexp = filter_jit(filter_grad(_pexp))
 
 
-@make_partial_pipe
 def dexp(
     x: Union[Float, ArrayLike],
     rate: Union[Float, ArrayLike],
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the derivative of the exponential distribution.
 
     Args:
         x (Union[Float, ArrayLike]): The value at which to evaluate the derivative.
         rate (Union[Float, ArrayLike]): The rate parameter of the exponential distribution.
         lower_tail (bool, optional): Whether to calculate the lower tail probability. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The derivative of the exponential distribution evaluated at x.
 
     Example:
         >>> dexp(1.0, 0.5, lower_tail=True, log_prob=False)
         Array([0.30326533], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x, 0)
     grads = filter_vmap(_dexp)(x, rate)
-    if not lower_tail:
-        grads = -grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _rexp(
     key: KeyArray,
     rate: Union[Float, ArrayLike],
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
         sample_shape = jnp.shape(rate)
     rate = jnp.broadcast_to(rate, sample_shape)
     return jrand.exponential(key, shape=sample_shape, dtype=dtype) / rate
 
 
-@make_partial_pipe
 def rexp(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     rate: Union[Float, ArrayLike] = None,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random samples from the exponential distribution.
 
     Args:
         key (KeyArray): A PRNGKey to use for generating random numbers.
         sample_shape (Optional[Shape], optional): The shape of the output array. Defaults to None.
         rate (Union[Float, ArrayLike], optional): The rate parameter of the exponential distribution. Defaults to None.
         lower_tail (bool, optional): Whether to return the lower tail of the distribution. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability of the samples. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: An array of random samples from the exponential distribution.
 
     Example:
         >>> key = jax.random.PRNGKey(0)
         >>> rexp(key, sample_shape=(2, 3), rate=1.0, lower_tail=False, log_prob=True)
```

### Comparing `stamox-0.1.3/stamox/distribution/_f.py` & `stamox-0.1.4/stamox/distribution/_pareto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,180 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
-from jax._src.random import KeyArray, Shape
-from jaxtyping import ArrayLike, Float
-
-from ..core import make_partial_pipe
-from ..math.special import fdtr, fdtri
+from jax._src.random import Shape
+from jax.random import KeyArray
+from jaxtyping import ArrayLike, Bool, Float
+
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
-def _pf(
+def _ppareto(
     x: Union[Float, ArrayLike],
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
 ):
-    return fdtr(dfn, dfd, x)
+    return 1 - jnp.power(scale / x, alpha)
 
 
-@make_partial_pipe
-def pF(
+def ppareto(
     q: Union[Float, ArrayLike],
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Calculates the cumulative distribution function of the F-distribution.
+    """Computes the cumulative distribution function of the Pareto distribution.
 
     Args:
-        q (Union[Float, ArrayLike]): The value at which to evaluate the cdf.
-        dfn (Union[Float, ArrayLike]): The numerator degrees of freedom.
-        dfd (Union[Float, ArrayLike]): The denominator degrees of freedom.
-        lower_tail (bool, optional): If True (default), the lower tail probability is returned.
-        log_prob (bool, optional): If True, the logarithm of the probability is returned.
-        dtype (jnp.dtype, optional): The dtype of the output (default is float32).
+        q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
+        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
+        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The cumulative distribution function evaluated at `q`.
+        ArrayLike: The cumulative distribution function of the Pareto distribution evaluated at `q`.
 
     Example:
-        >>> pF(1.0, 1.0, 1.0)
-        Array([0.5000001], dtype=float32, weak_type=True)
+        >>> ppareto(0.2, 0.1, 2.0)
+        Array([0.75], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_pf)(q, dfn, dfd)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    q = filter_vmap(_check_clip_distribution_domain)(q, scale)
+    p = filter_vmap(_ppareto)(q, scale, alpha)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
-_df = filter_jit(filter_grad(_pf))
+_dpareto = filter_grad(filter_jit(_ppareto))
 
 
-@make_partial_pipe
-def dF(
+def dpareto(
     x: Union[Float, ArrayLike],
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
-    lower_tail: bool = True,
-    log_prob: bool = False,
-    dtype=jnp.float32,
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
+    lower_tail=True,
+    log_prob=False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Calculates the gradient of the cumulative distribution function for a given x, dfn and dfd.
+    """Computes the density of the Pareto distribution.
 
     Args:
-        x (Union[Float, ArrayLike]): The value at which to calculate the gradient of the cumulative distribution function.
-        dfn (Union[Float, ArrayLike]): The numerator degrees of freedom.
-        dfd (Union[Float, ArrayLike]): The denominator degrees of freedom.
-        lower_tail (bool, optional): Whether to calculate the lower tail of the cumulative distribution function. Defaults to True.
+        x (Union[Float, ArrayLike]): The value at which to evaluate the density.
+        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
+        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail probability. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The gradient of the cumulative distribution function.
+        ArrayLike: The density of the Pareto distribution evaluated at `x`.
 
     Example:
-        >>> dF(1.0, 1.0, 1.0)
-        Array([0.1591549], dtype=float32, weak_type=True)
+        >>> dpareto(0.2, 0.1, 2.0)
+        Array([2.4999998], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
-    grads = filter_vmap(_df)(x, dfn, dfd)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = filter_vmap(_dpareto)(x, scale, alpha)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
-def _qf(
+def _qpareto(
     q: Union[Float, ArrayLike],
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
 ):
-    return fdtri(dfn, dfd, q)
+    return scale / jnp.power(1 - q, 1 / alpha)
 
 
-@make_partial_pipe
-def qF(
+def qpareto(
     p: Union[Float, ArrayLike],
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
-    lower_tail: bool = True,
-    log_prob: bool = False,
-    dtype=jnp.float32,
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
+    lower_tail: Bool = True,
+    log_prob: Bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Calculates the quantile function of a given distribution.
+    """Computes the quantile function of the Pareto distribution.
 
     Args:
-        p (Union[Float, ArrayLike]): The quantile to calculate.
-        dfn (Union[Float, ArrayLike]): The degrees of freedom for the numerator.
-        dfd (Union[Float, ArrayLike]): The degrees of freedom for the denominator.
-        lower_tail (bool, optional): Whether to calculate the lower tail or not. Defaults to True.
-        log_prob (bool, optional): Whether to calculate the log probability or not. Defaults to False.
+        p (Union[Float, ArrayLike]): Quantiles to compute.
+        scale (Union[Float, ArrayLike]): Scale parameter of the Pareto distribution.
+        alpha (Union[Float, ArrayLike]): Shape parameter of the Pareto distribution.
+        lower_tail (Bool, optional): Whether to compute the lower tail probability. Defaults to True.
+        log_prob (Bool, optional): Whether to compute the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The calculated quantile.
+        ArrayLike: The quantiles of the Pareto distribution.
 
     Example:
-        >>> qF(0.5, 1.0, 1.0)
-        Array([0.99999714], dtype=float32)
+        >>> qpareto(0.2, 0.1, 2.0)
+        Array([0.1118034], dtype=float32, weak_type=True)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-    return filter_vmap(_qf)(p, dfn, dfd)
+    p = _check_clip_probability(p, lower_tail, log_prob)
+    return filter_vmap(_qpareto)(p, scale, alpha)
 
 
 @filter_jit
-def _rf(
+def _rpareto(
     key: KeyArray,
-    dfn: Union[Float, ArrayLike],
-    dfd: Union[Float, ArrayLike],
+    scale: Union[Float, ArrayLike],
+    alpha: Union[Float, ArrayLike],
     sample_shape: Optional[Shape] = None,
-    dtype = jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
-        sample_shape = jnp.broadcast_shapes(jnp.shape(dfn), jnp.shape(dfd))
-    dfn = jnp.broadcast_to(dfn, sample_shape)
-    dfd = jnp.broadcast_to(dfd, sample_shape)
-    return jrand.f(key, dfn, dfd, shape=sample_shape, dtype=dtype)
+        sample_shape = jnp.broadcast_shapes(jnp.shape(scale), jnp.shape(alpha))
+    scale = jnp.broadcast_to(scale, sample_shape)
+    alpha = jnp.broadcast_to(alpha, sample_shape)
+    return jrand.pareto(key, alpha, shape=sample_shape, dtype=dtype) * scale
 
 
-@make_partial_pipe
-def rF(
+def rpareto(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    dfn: Union[Float, ArrayLike] = None,
-    dfd: Union[Float, ArrayLike] = None,
-    lower_tail: bool = True,
-    log_prob: bool = False,
-    dtype = jnp.float32,
-):
-    """Generate random variates from F-distribution.
+    scale: Union[Float, ArrayLike] = None,
+    alpha: Union[Float, ArrayLike] = None,
+    lower_tail: Bool = True,
+    log_prob: Bool = False,
+    dtype=jnp.float_,
+) -> ArrayLike:
+    """Generate random variable following a Pareto distribution.
 
     Args:
-        key (KeyArray): Random key used for PRNG.
-        sample_shape (Optional[Shape], optional): Shape of the samples to be drawn. Defaults to None.
-        dfn (Union[Float, ArrayLike]): Degrees of freedom in numerator.
-        dfd (Union[Float, ArrayLike]): Degrees of freedom in denominator.
-        lower_tail (bool, optional): Whether to calculate the lower tail probability. Defaults to True.
-        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to float32.
+        key (KeyArray): A random number generator key.
+        sample_shape (Optional[Shape], optional): The shape of the samples to be drawn. Defaults to None.
+        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
+        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
+        lower_tail (Bool, optional): Whether to calculate the lower tail probability. Defaults to True.
+        log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike : Random variates from F-distribution.
+        ArrayLike: random variable following a Pareto distribution.
 
     Example:
-        >>> rF(jax.random.PRNGKey(0), dfn=1.0, dfd=1.0)
-        Array(40.787617, dtype=float32)
-
+        >>> rpareto(jax.random.PRNGKey(0), sample_shape=(2, 3), scale=0.1, alpha=2.0)
+        Array([[0.15330292, 0.10539087, 0.19686179],
+                [0.30740616, 0.15743963, 0.13524036]], dtype=float32)
     """
-    rvs = _rf(key, dfn, dfd, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _rpareto(key, scale, alpha, sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/distribution/_gamma.py` & `stamox-0.1.4/stamox/distribution/_gamma.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 import tensorflow_probability.substrates.jax.math as tfp_math
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import KeyArray, Shape
 from jax.scipy.special import gammainc
 from jaxtyping import ArrayLike, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pgamma(
     q, shape: Union[Float, ArrayLike] = 1.0, rate: Union[Float, ArrayLike] = 1.0
 ):
     return gammainc(shape, q * rate)
 
 
-@make_partial_pipe
 def pgamma(
     q: Union[Float, ArrayLike],
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the cumulative distribution function of the gamma distribution.
 
     Args:
         q: A float or array-like object representing the input to the gamma function.
         shape: A float or array-like object representing the shape parameter of the gamma function.
         rate: A float or array-like object representing the rate parameter of the gamma function.
         lower_tail: A boolean indicating whether to compute the lower tail of the gamma function.
         log_prob: A boolean indicating whether to compute the logarithm of the probability density function.
-        dtype: The dtype of the output. Defaults to float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The CDF value of the given value or array of values.
 
     Example:
         >>> pgamma(1.0, 0.5, 0.5)
         Array([0.6826893], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q, 0.0, jnp.inf)
     p = filter_vmap(_pgamma)(q, shape, rate)
-    if not lower_tail:
-        p = 1.0 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dgamma = filter_jit(filter_grad(_pgamma))
 
 
-@make_partial_pipe
 def dgamma(
     x: Union[Float, ArrayLike],
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Compute density of gamma distribution.
 
     Args:
         x (Union[Float, ArrayLike]): The value at which to evaluate the gamma
             distribution.
         shape (Union[Float, ArrayLike], optional): The shape parameter of the
@@ -85,89 +87,85 @@
         ArrayLike: The density of the gamma distribution evaluated
             at `x`. If `log_prob` is True, returns the log probability.
 
     Example:
         >>> dgamma(1.0, 0.5, 0.5)
         Array([0.24197064], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x, 0.0, jnp.inf)
     grads = filter_vmap(_dgamma)(x, shape, rate)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qgamma(
     q: Union[Float, ArrayLike],
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
 ):
-    return tfp_math.igammainv(shape, q) / rate
+    dtype = lax.dtype(q)
+    shape = jnp.asarray(shape, dtype=dtype)
+    rate = jnp.asarray(rate, dtype=dtype)
+    return lax.div(tfp_math.igammainv(shape, q), rate)
 
 
-@make_partial_pipe
 def qgamma(
     p: Union[Float, ArrayLike],
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the quantile of the gamma distribution.
 
     Args:
         p: A float or array-like object representing the quantile.
         shape: A float or array-like object representing the shape parameter of the gamma distribution.
         rate: A float or array-like object representing the rate parameter of the gamma distribution.
         lower_tail: A boolean indicating whether to compute the lower tail (default) or upper tail.
         log_prob: A boolean indicating whether to compute the log probability (default False).
-        dtype: The dtype of the output. Defaults to float32.
+        dtype: The dtype of the output. Defaults to float_.
 
     Returns:
         ArrayLike: The quantile of the gamma distribution.
 
     Example:
         >>> qgamma(0.5, 0.5, 0.5)
         Array([0.45493677], dtype=float32)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
     x = filter_vmap(_qgamma)(p, shape, rate)
     return x
 
 
-@make_partial_pipe
 def rgamma(
     key,
     sample_shape: Optional[Shape] = None,
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random gamma values.
 
     Args:
         key: A PRNGKey to use for the random number generation.
         sample_shape: An optional shape for the output array.
         shape: The shape parameter of the gamma distribution.
         rate: The rate parameter of the gamma distribution.
         lower_tail: Whether to return the lower tail of the distribution.
         log_prob: Whether to return the log probability of the result.
-        dtype: The dtype of the output. Defaults to float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: A random gamma value or an array of random gamma values.
 
     Example:
         >>> rgamma(key, shape=0.5, rate=0.5)
         Array(0.3384059, dtype=float32)
@@ -182,14 +180,14 @@
 
 @filter_jit
 def _rgamma(
     key: KeyArray,
     shape: Union[Float, ArrayLike] = 1.0,
     rate: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(shape), jnp.shape(rate))
     shape = jnp.broadcast_to(shape, sample_shape)
     rate = jnp.broadcast_to(rate, sample_shape)
     return jrand.gamma(key, shape, sample_shape, dtype) / rate
```

### Comparing `stamox-0.1.3/stamox/distribution/_laplace.py` & `stamox-0.1.4/stamox/distribution/_laplace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,183 +1,188 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jaxtyping import ArrayLike, Bool, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _plaplace(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ):
-    scaled = (x - loc) / scale
-    return 0.5 - 0.5 * jnp.sign(scaled) * jnp.expm1(-jnp.abs(scaled))
+    dtype = lax.dtype(x)
+    loc = jnp.asarray(loc, dtype=dtype)
+    scale = jnp.asarray(scale, dtype=dtype)
+    half = jnp.asarray(0.5, dtype=dtype)
+    scaled = lax.div(lax.sub(x, loc), scale)
+    subtrahend = half * lax.mul(jnp.sign(scaled), lax.expm1(-lax.abs(scaled)))
+    return lax.sub(half, subtrahend)
 
 
-@make_partial_pipe
 def plaplace(
     q: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the Laplace cumulative density function.
 
     Args:
         q (Union[Float, ArrayLike]): The value at which to evaluate the Plaplace PDF.
         loc (Union[Float, ArrayLike], optional): The location parameter of the Plaplace PDF. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): The scale parameter of the Plaplace PDF. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to return the lower tail of the Plaplace PDF. Defaults to True.
         log_prob (Bool, optional): Whether to return the logarithm of the Plaplace PDF. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The Laplace CDF evaluated at `q`.
 
     Example:
         >>> plaplace(1.0, 1.0, 1.0)
         Array([0.5], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q)
     p = filter_vmap(_plaplace)(q, loc, scale)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dlaplace = filter_grad(filter_jit(_plaplace))
 
 
-@make_partial_pipe
 def dlaplace(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the Laplace probability density function for a given x, location and scale.
 
     Args:
         x (Union[Float, ArrayLike]): The value at which to calculate the probability density.
         loc (Union[Float, ArrayLike], optional): The location parameter. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): The scale parameter. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to return the lower tail of the distribution. Defaults to True.
         log_prob (Bool, optional): Whether to return the logarithm of the probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability density at the given x.
 
     Example:
         >>> dlaplace(1.0, 1.0, 1.0)
         Array([0.], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
-    p = filter_vmap(_dlaplace)(x, loc, scale)
-    if not lower_tail:
-        p = -p
-    if log_prob:
-        p = jnp.log(p)
-    return p
+    x = _check_clip_distribution_domain(x)
+    grads = filter_vmap(_dlaplace)(x, loc, scale)
+    grads = _post_process(grads, lower_tail, log_prob)
+    return grads
 
 
 @filter_jit
 def _qlaplace(
     q: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ):
-    a = q - 0.5
-    return loc - scale * jnp.sign(a) * jnp.log1p(-2 * jnp.abs(a))
+    dtype = lax.dtype(q)
+    loc = jnp.asarray(loc, dtype=dtype)
+    scale = jnp.asarray(scale, dtype=dtype)
+    half = jnp.asarray(0.5, dtype=dtype)
+    a = lax.sub(half, q)
+    return scale * jnp.sign(a) * jnp.log1p(-2 * jnp.abs(a)) - loc
 
 
-@make_partial_pipe
 def qlaplace(
     p: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Computes the quantile of the Laplace distribution.
 
     Args:
         p (Union[Float, ArrayLike]): Quantiles to compute.
         loc (Union[Float, ArrayLike], optional): Location parameter. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): Scale parameter. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to compute the lower tail. Defaults to True.
         log_prob (Bool, optional): Whether to compute the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantiles of the Laplace distribution.
 
     Example:
         >>> qlaplace(0.5, 1.0, 1.0)
         Array([1.], dtype=float32, weak_type=True)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
     return filter_vmap(_qlaplace)(p, loc, scale)
 
 
 @filter_jit
 def _rlaplace(
     key: KeyArray,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
     loc = jnp.broadcast_to(loc, sample_shape)
     scale = jnp.broadcast_to(scale, sample_shape)
     return jrand.laplace(key, sample_shape, dtype=dtype) * scale + loc
 
 
-@make_partial_pipe
 def rlaplace(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random Laplace samples from a given key.
 
     Args:
         key (KeyArray): The PRNG key to use for generating the samples.
         sample_shape (Optional[Shape], optional): The shape of the output array. Defaults to None.
         loc (Union[Float, ArrayLike], optional): The location parameter of the Laplace distribution. Defaults to 0.0.
         scale (Union[Float, ArrayLike], optional): The scale parameter of the Laplace distribution. Defaults to 1.0.
         lower_tail (Bool, optional): Whether to return the lower tail probability. Defaults to True.
         log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: An array containing the random Laplace samples.
 
     Example:
         >>> rlaplace(key, (2, 3))
         Array([[-0.16134426,  1.6125823 , -0.6615164 ],
```

### Comparing `stamox-0.1.3/stamox/distribution/_normal.py` & `stamox-0.1.4/stamox/distribution/_normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,203 +1,200 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jax.scipy.special import ndtr, ndtri
 from jaxtyping import ArrayLike, Bool, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pnorm(
     x: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
 ):
-    scaled = (x - mean) / sd
+    mean = jnp.asarray(mean, dtype=x.dtype)
+    sd = jnp.asarray(sd, dtype=x.dtype)
+    scaled = lax.div(lax.sub(x, mean), sd)
     return ndtr(scaled)
 
 
-@make_partial_pipe(name="pnorm")
 def pnorm(
     q: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculate the cumulative distribution function (CDF) of the normal distribution.
 
     Args:
         q (Union[Float, ArrayLike]): The quantiles to calculate the CDF at.
         mean (Union[Float, ArrayLike], optional): The mean of the normal distribution. Defaults to 0.0.
         sd (Union[Float, ArrayLike], optional): The standard deviation of the normal distribution.
             Defaults to 1.0.
         lower_tail (bool, optional): If True, calculate the probability that x is less than or equal to the
             given quantile(s). If False, calculate the probability that x is greater than the given quantile(s).
             Defaults to True.
         log_prob (bool, optional): If True, return the log of the CDF instead of the actual value.
             Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The CDF of the normal distribution evaluated at x.
 
 
     Examples:
         >>> pnorm(2.0)
         Array([0.97724986], dtype=float32)
 
         >>> pnorm([1.5, 2.0, 2.5], mean=2.0, sd=0.5, lower_tail=False)
         Array([0.8413447 , 0.5       , 0.15865529], dtype=float32)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
+    q = _check_clip_distribution_domain(q)
     p = filter_vmap(_pnorm)(q, mean, sd)
-    if not lower_tail:
-        p = 1.0 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dnorm = filter_jit(filter_grad(_pnorm))
 
 
-@make_partial_pipe(name="dnorm")
 def dnorm(
     x: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """
     Probability density function (PDF) for Normal distribution.
 
     Args:
         x (Union[Float, ArrayLike]): The input value(s) at which to evaluate the PDF.
         mean (Union[Float, ArrayLike], optional): The mean of the normal distribution. Defaults to 0.0.
         sd (Union[Float, ArrayLike], optional): The standard deviation of the normal distribution. Defaults to 1.0.
         lower_tail (bool, optional): If True (default), returns the cumulative distribution function (CDF) from negative infinity up to x. Otherwise, returns the CDF from x to positive infinity.
         log_prob (bool, optional): If True, returns the log-probability instead of the probability.
-        dtype (jnp.dtype, optional): The dtype of the output. Default is `jnp.float32`.
+        dtype (jnp.dtype, optional): The dtype of the output. Default is `jnp.float_`.
 
     Returns:
         ArrayLike: The probability density function evaluated at point(s) x.
 
     Example:
         >>> import jax.numpy as jnp
         >>> x = jnp.array([0.5, 1.0, -1.5])
         >>> dnorm(x)
         Array([0.35206532, 0.24197075, 0.12951761], dtype=float32)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x)
     grads = filter_vmap(_dnorm)(x, mean, sd)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qnorm(
     p: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
 ):
     x = ndtri(p)
-    return x * sd + mean
+    sd = lax.convert_element_type(sd, x.dtype)
+    mean = lax.convert_element_type(mean, x.dtype)
+    return lax.add(lax.mul(x, sd), mean)
 
 
-@make_partial_pipe(name="qnorm")
 def qnorm(
     p: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """
     Calculates the quantile function of the normal distribution for a given probability.
 
     Args:
         p (float or jnp.ndarray): Probability values.
         mean (float or jnp.ndarray, optional): Mean of the normal distribution. Default is 0.0.
         sd (float or jnp.ndarray, optional): Standard deviation of the normal distribution. Default is 1.0.
         lower_tail (bool, optional): If `True`, returns P(X ≤ x). If `False`, returns P(X > x). Default is `True`.
         log_prob (bool, optional): If `True`, returns the logarithm of the quantile function. Default is `False`.
-        dtype (jnp.dtype, optional): The dtype of the output. Default is `jnp.float32`.
+        dtype (jnp.dtype, optional): The dtype of the output. Default is `jnp.float_`.
 
     Returns:
         ArrayLike: The inverse cumulative density function of the normal distribution evaluated at `q`.
 
 
     Examples:
         >>> qnorm(0.5)
         Array([0.], dtype=float32)
         >>> qnorm([0.25, 0.75], mean=3, sd=2)
         Array([1.6510204, 4.3489795], dtype=float32)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
     x = filter_vmap(_qnorm)(p, mean, sd)
     return x
 
 
 @filter_jit
 def _rnorm(key, mean, sd, sample_shape, dtype):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(mean), jnp.shape(sd))
     mean = jnp.broadcast_to(mean, sample_shape)
     sd = jnp.broadcast_to(sd, sample_shape)
     return jrand.normal(key, sample_shape, dtype=dtype) * sd + mean
 
 
-@make_partial_pipe(name="rnorm")
 def rnorm(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     mean: Union[Float, ArrayLike] = 0.0,
     sd: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random variables from a normal distribution.
 
     Args:
         key: A KeyArray object used to generate the random numbers.
         sample_shape: An optional tuple of integers specifying the shape of the
         output array. Defaults to an empty tuple.
         mean: The mean of the normal distribution. Defaults to 0.0.
         sd: The standard deviation of the normal distribution. Defaults to 1.0.
         lower_tail: If True (default), returns the cumulative distribution function (CDF) from negative infinity up to x. Otherwise, returns the CDF from x to positive infinity.
         log_prob: If True, returns the log-probability instead of the probability.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: Random samples from a normal distribution.
 
     Example:
-        >>> import jax.numpy as jnp
-        >>> from jax import random
         >>> key = random.PRNGKey(0)
         >>> rnorm(key, sample_shape=(3, 2))
         Array([[ 0.18784384, -1.2833426 ],
                 [ 0.6494181 ,  1.2490594 ],
                 [ 0.24447003, -0.11744965]], dtype=float32)
 
     """
```

### Comparing `stamox-0.1.3/stamox/distribution/_pareto.py` & `stamox-0.1.4/stamox/distribution/_uniform.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,186 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
-from jax._src.random import Shape
-from jax.random import KeyArray
+from jax import lax
+from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Bool, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
-def _ppareto(
+def _punif(
     x: Union[Float, ArrayLike],
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
 ):
-    return 1 - jnp.power(scale / x, alpha)
+    mini = lax.convert_element_type(mini, x.dtype)
+    maxi = lax.convert_element_type(maxi, x.dtype)
+    p = lax.div(lax.sub(x, mini), lax.sub(maxi, mini))
+    p = jnp.clip(p, a_min=mini, a_max=maxi)
+    return p
 
 
-@make_partial_pipe
-def ppareto(
+def punif(
     q: Union[Float, ArrayLike],
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
-    lower_tail: bool = True,
-    log_prob: bool = False,
-    dtype=jnp.float32,
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
+    lower_tail: Bool = True,
+    log_prob: Bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the cumulative distribution function of the Pareto distribution.
+    """Computes the cumulative distribution function of the uniform distribution.
 
     Args:
         q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
-        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
-        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
+        mini (Union[Float, ArrayLike], optional): The minimum value of the uniform distribution. Defaults to 0.0.
+        maxi (Union[Float, ArrayLike], optional): The maximum value of the uniform distribution. Defaults to 1.0.
         lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The cumulative distribution function of the Pareto distribution evaluated at `q`.
+        ArrayLike: The cumulative distribution function of the uniform distribution evaluated at `q`.
 
     Example:
-        >>> ppareto(0.2, 0.1, 2.0)
-        Array([0.75], dtype=float32, weak_type=True)
+        >>> punif(0.5)
+        Array([0.5], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_ppareto)(q, scale, alpha)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = filter_vmap(_punif)(q, mini, maxi)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
-_dpareto = filter_grad(filter_jit(_ppareto))
+_dunif = filter_grad(filter_jit(_punif))
 
 
-@make_partial_pipe
-def dpareto(
+def dunif(
     x: Union[Float, ArrayLike],
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
-    lower_tail=True,
-    log_prob=False,
-    dtype=jnp.float32,
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
+    lower_tail: Bool = True,
+    log_prob: Bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the density of the Pareto distribution.
+    """Calculates the probability density function of a uniform distribution.
 
     Args:
-        x (Union[Float, ArrayLike]): The value at which to evaluate the density.
-        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
-        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
-        lower_tail (bool, optional): Whether to compute the lower tail probability. Defaults to True.
-        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        x (Union[Float, ArrayLike]): The value or array of values for which to calculate the probability density.
+        mini (Union[Float, Array], optional): The lower bound of the uniform distribution. Defaults to 0.0.
+        maxi (Union[Float, Array], optional): The upper bound of the uniform distribution. Defaults to 1.0.
+        lower_tail (Bool, optional): Whether to calculate the lower tail probability. Defaults to True.
+        log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The density of the Pareto distribution evaluated at `x`.
+        ArrayLike: The probability density of the given value(s).
 
     Example:
-        >>> dpareto(0.2, 0.1, 2.0)
-        Array([2.4999998], dtype=float32, weak_type=True)
+        >>> dunif(0.5)
+        Array([1.], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
-    grads = filter_vmap(_dpareto)(x, scale, alpha)
+    p = filter_vmap(_dunif)(x, mini, maxi)
     if not lower_tail:
-        grads = 1 - grads
+        p = 1 - p
     if log_prob:
-        grads = jnp.log(grads)
-    return grads
+        p = jnp.log(p)
+    return p
 
 
 @filter_jit
-def _qpareto(
+def _qunif(
     q: Union[Float, ArrayLike],
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
 ):
-    return scale / jnp.power(1 - q, 1 / alpha)
+    x = q * (maxi - mini) + mini
+    x = jnp.clip(x, a_min=mini, a_max=maxi)
+    return x
 
 
-@make_partial_pipe
-def qpareto(
+def qunif(
     p: Union[Float, ArrayLike],
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the quantile function of the Pareto distribution.
+    """
+    Computes the quantile function of a uniform distribution.
 
     Args:
         p (Union[Float, ArrayLike]): Quantiles to compute.
-        scale (Union[Float, ArrayLike]): Scale parameter of the Pareto distribution.
-        alpha (Union[Float, ArrayLike]): Shape parameter of the Pareto distribution.
-        lower_tail (Bool, optional): Whether to compute the lower tail probability. Defaults to True.
-        log_prob (Bool, optional): Whether to compute the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        mini (Union[Float, Array], optional): Lower bound of the uniform distribution. Defaults to 0.0.
+        maxi (Union[Float, Array], optional): Upper bound of the uniform distribution. Defaults to 1.0.
+        lower_tail (Bool, optional): Whether to compute the lower tail or not. Defaults to True.
+        log_prob (Bool, optional): Whether to compute the log probability or not. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The quantiles of the Pareto distribution.
+       ArrayLike: The quantiles of the uniform distribution.
 
     Example:
-        >>> qpareto(0.2, 0.1, 2.0)
-        Array([0.1118034], dtype=float32, weak_type=True)
+        >>> qunif(0.5)
+        Array([0.5], dtype=float32, weak_type=True)
     """
     p = jnp.asarray(p, dtype=dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-    return filter_vmap(_qpareto)(p, scale, alpha)
+    p = _check_clip_probability(p, lower_tail, log_prob)
+    q = filter_vmap(_qunif)(p, mini, maxi)
+    return q
 
 
 @filter_jit
-def _rpareto(
+def _runif(
     key: KeyArray,
-    scale: Union[Float, ArrayLike],
-    alpha: Union[Float, ArrayLike],
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
-    if sample_shape is None:
-        sample_shape = jnp.broadcast_shapes(jnp.shape(scale), jnp.shape(alpha))
-    scale = jnp.broadcast_to(scale, sample_shape)
-    alpha = jnp.broadcast_to(alpha, sample_shape)
-    return jrand.pareto(key, alpha, shape=sample_shape, dtype=dtype) * scale
+    return jrand.uniform(key, sample_shape, minval=mini, maxval=maxi, dtype=dtype)
 
 
-@make_partial_pipe
-def rpareto(
+def runif(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    scale: Union[Float, ArrayLike] = None,
-    alpha: Union[Float, ArrayLike] = None,
+    mini: Union[Float, ArrayLike] = 0.0,
+    maxi: Union[Float, ArrayLike] = 1.0,
     lower_tail: Bool = True,
     log_prob: Bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Generate random variable following a Pareto distribution.
+    """Generates random numbers from a uniform distribution.
 
     Args:
-        key (KeyArray): A random number generator key.
-        sample_shape (Optional[Shape], optional): The shape of the samples to be drawn. Defaults to None.
-        scale (Union[Float, ArrayLike]): The scale parameter of the Pareto distribution.
-        alpha (Union[Float, ArrayLike]): The shape parameter of the Pareto distribution.
-        lower_tail (Bool, optional): Whether to calculate the lower tail probability. Defaults to True.
-        log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        key: A PRNGKey to use for generating the random numbers.
+        sample_shape: The shape of the output array.
+        mini: The minimum value of the uniform distribution.
+        maxi: The maximum value of the uniform distribution.
+        lower_tail: Whether to generate values from the lower tail of the distribution.
+        log_prob: Whether to return the log probability of the generated values.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: random variable following a Pareto distribution.
+        ArrayLike: An array of random numbers from a uniform distribution.
 
     Example:
-        >>> rpareto(jax.random.PRNGKey(0), sample_shape=(2, 3), scale=0.1, alpha=2.0)
-        Array([[0.15330292, 0.10539087, 0.19686179],
-                [0.30740616, 0.15743963, 0.13524036]], dtype=float32)
+        >>> runif(key, sample_shape=(2, 3))
+        Array([[0.57450044, 0.09968603, 0.7419659 ],
+                [0.8941783 , 0.59656656, 0.45325184]], dtype=float32)
+
     """
-    rvs = _rpareto(key, scale, alpha, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _runif(key, mini, maxi, sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/distribution/_poisson.py` & `stamox-0.1.4/stamox/distribution/_chisq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,165 +1,152 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_jit, filter_vmap
-from jax import pure_callback, ShapeDtypeStruct
-from jax._src.random import Shape
-from jax.random import KeyArray
-from jax.scipy.special import gammainc, gammaln
-from jaxtyping import Array, ArrayLike, Bool, Float
-from scipy.stats import poisson
+from jax._src.random import KeyArray, Shape
+from jaxtyping import ArrayLike, Float, Int
 
-from ..core import make_partial_pipe
+from ._gamma import _dgamma, _pgamma, _qgamma
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
-@filter_jit
-def _ppoisson(x: Union[Float, ArrayLike], rate: Union[Float, ArrayLike]) -> Array:
-    k = jnp.floor(x) + 1.0
-    return 1 - gammainc(k, rate)
+def dchisq(
+    x: Union[Float, ArrayLike],
+    df: Union[Int, Float, ArrayLike],
+    lower_tail=True,
+    log_prob=False,
+    dtype=jnp.float_,
+) -> ArrayLike:
+    """Computes the chi-squared distribution.
+
+    Args:
+        x: A float or array-like object representing the values at which to evaluate the chi-squared distribution.
+        df: The degrees of freedom for the chi-squared distribution.
+        lower_tail: A boolean indicating whether to compute the lower tail of the chi-squared distribution (defaults to True).
+        log_prob: A boolean indicating whether to return the log probability (defaults to False).
+        dtype: The dtype of the output (defaults to float32).
+
+    Returns:
+        ArrayLike: The chi-squared distribution evaluated at `x`.
+
+    Example:
+        >>> dchisq(2.0, 3)
+        Array([0.20755368], dtype=float32, weak_type=True)
+    """
+    x, dtype = _promote_dtype_to_floating(x, dtype)
+    x = jnp.atleast_1d(x)
+    x = _check_clip_distribution_domain(x, 0.0, jnp.inf)
+    grads = filter_vmap(_dgamma)(x, df / 2, 1 / 2)
+    grads = _post_process(grads, lower_tail, log_prob)
+    return grads
 
 
-@make_partial_pipe
-def ppoisson(
+def pchisq(
     q: Union[Float, ArrayLike],
-    rate: Union[Float, ArrayLike],
+    df: Union[Int, Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the cumulative distribution function of the Poisson distribution.
+    """Calculates the chi-squared probability density function.
 
     Args:
-        q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
-        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
-        lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
-        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        q (Union[float, array-like]): The value of the chi-squared variable.
+        df (Union[int, float, array-like]): The degrees of freedom.
+        lower_tail (bool): Whether to calculate the lower tail (default True).
+        log_prob (bool): Whether to return the log probability (default False).
+        dtype (dtype): The dtype of the output (default jnp.float_).
 
     Returns:
-        ArrayLike: The cumulative distribution function of the Poisson distribution evaluated at `q`.
+        ArrayLike: The chi-squared probability density function.
+
+    Example:
+        >>> pchisq(2.0, 3)
+        Array([0.42759317], dtype=float32, weak_type=True)
     """
     q = jnp.asarray(q, dtype=dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_ppoisson)(q, rate)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    q = _check_clip_distribution_domain(q, 0.0, jnp.inf)
+    p = filter_vmap(_pgamma)(q, df / 2, 1 / 2)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
-@filter_jit
-def _dpoisson(x, rate):
-    e = jnp.exp(-rate)
-    numerator = rate**x
-    denominator = jnp.exp(gammaln(x + 1))
-    return (numerator / denominator) * e
-
-
-@make_partial_pipe
-def dpoisson(
-    x: Union[Float, ArrayLike],
-    rate: Union[Float, ArrayLike],
+def qchisq(
+    p: Union[Float, ArrayLike],
+    df: Union[Int, Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the probability density function of the Poisson distribution.
+    """Computes the inverse of the chi-squared cumulative distribution function.
 
     Args:
-        x (Union[Float, ArrayLike]): The value at which to evaluate the PDF.
-        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
-        lower_tail (bool, optional): Whether to compute the lower tail of the PDF. Defaults to True.
-        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        p (Union[Float, ArrayLike]): Probability value or array of probability values.
+        df (Union[Int, Float, ArrayLike]): Degrees of freedom.
+        lower_tail (bool, optional): If True (default), probabilities are P[X ≤ x], otherwise, P[X > x].
+        log_prob (bool, optional): If True, probabilities are given as log(p).
+        dtype (dtype, optional): The dtype of the output (default jnp.float_).
 
     Returns:
-        ArrayLike: The probability density function of the Poisson distribution evaluated at `x`.
+        ArrayLike: The quantiles corresponding to the given probabilities.
+
+    Example:
+        >>> qchisq(0.95, 10)
+        Array([18.307034], dtype=float32)
     """
-    x = jnp.asarray(x, dtype=dtype)
-    x = jnp.atleast_1d(x)
-    grads = filter_vmap(_dpoisson)(x, rate)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
-    return grads
+    p = jnp.asarray(p, dtype=dtype)
+    p = jnp.atleast_1d(p)
+    p = _check_clip_probability(p, lower_tail, log_prob)
+    q = filter_vmap(_qgamma)(p, df / 2, 1 / 2)
+    return q
 
 
 @filter_jit
-def _rpoisson(
+def _rchisq(
     key: KeyArray,
-    rate: Union[Float, ArrayLike],
+    df: Union[Int, Float, ArrayLike],
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.int32,
+    dtype=jnp.float_,
 ):
-    return jrand.poisson(key, rate, shape=sample_shape, dtype=dtype)
+    if sample_shape is None:
+        sample_shape = jnp.shape(df)
+    df = jnp.broadcast_to(df, sample_shape)
+    return jrand.chisquare(key, df, shape=sample_shape, dtype=dtype)
 
 
-@make_partial_pipe
-def rpoisson(
+def rchisq(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    rate: Union[Float, ArrayLike] = None,
+    df: Union[Int, Float, ArrayLike] = None,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.int32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Generates samples from the Poisson distribution.
+    """
+    Generates random variates from the chi-squared distribution.
 
     Args:
-        key (KeyArray): Random number generator state used for random sampling.
-        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
+        key (KeyArray): Random key to generate the random numbers.
         sample_shape (Optional[Shape], optional): Shape of the output array. Defaults to None.
+        df (Union[Int, Float, ArrayLike], optional): Degrees of freedom. Defaults to None.
         lower_tail (bool, optional): Whether to return the lower tail probability. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int32.
+        dtype (dtype, optional): The dtype of the output (default float_).
 
     Returns:
-        ArrayLike: Samples from the Poisson distribution.
-    """
-    rvs = _rpoisson(key, rate, sample_shape=sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
-    return rvs
-
-
-@filter_jit
-def _qpoisson(q, rate, dtype):
-    result_shape_type = ShapeDtypeStruct(jnp.shape(q), dtype)
-    _scp_poisson_ppf = lambda q, rate: poisson(rate).ppf(q).astype(dtype)
-    p = pure_callback(_scp_poisson_ppf, result_shape_type, q, rate)
-    return p
+        ArrayLike: Random variates from the chi-squared distribution.
 
-
-@make_partial_pipe
-def qpoisson(
-    p: Union[Float, ArrayLike],
-    rate: Union[Float, ArrayLike],
-    lower_tail: Bool = True,
-    log_prob: Bool = False,
-    dtype=jnp.int32,
-) -> ArrayLike:
-    """Computes the quantile function of the Poisson distribution.
-
-    Args:
-        p (Union[Float, ArrayLike]): The probability at which to evaluate the quantile function.
-        rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
-        lower_tail (bool, optional): Whether to compute the lower tail of the quantile function. Defaults to True.
-        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int32.
-
-    Returns:
-        ArrayLike: The quantile function of the Poisson distribution evaluated at `p`.
+    Example:
+        >>> key = jax.random.PRNGKey(0)
+        >>> rchisq(key, df=2)
+        Array(1.982825, dtype=float32)
     """
-    p = jnp.asarray(p)
-    p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-    q = filter_vmap(_qpoisson)(p, rate, dtype)
-    return q
+    rvs = _rchisq(key, df, sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail, log_prob)
+    return rvs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stamox-0.1.3/stamox/distribution/_t.py` & `stamox-0.1.4/stamox/distribution/_t.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,216 +1,212 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
-from jax.scipy.special import betainc
 from jaxtyping import ArrayLike, Float, Int
 from tensorflow_probability.substrates.jax.math import special as tfp_special
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
 def _pt(
     x: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ):
-    scaled = (x - loc) / scale
-    scaled_squared = scaled * scaled
-    beta_value = df / (df + scaled_squared)
+    df = lax.convert_element_type(df, x.dtype)
+    loc = lax.convert_element_type(loc, x.dtype)
+    scale = lax.convert_element_type(scale, x.dtype)
+    scaled = lax.div(lax.sub(x, loc), scale)
+    scaled_squared = lax.integer_pow(scaled, 2)
+    beta_value = lax.div(df, lax.add(df, scaled_squared))
     return 0.5 * (
-        1 + jnp.sign(scaled) - jnp.sign(scaled) * betainc(0.5 * df, 0.5, beta_value)
+        1.0
+        + jnp.sign(scaled)
+        - jnp.sign(scaled) * tfp_special.betainc(0.5 * df, 0.5, beta_value)
     )
 
 
-@make_partial_pipe
 def pt(
     q: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the probability of a given value for Student T distribution.
 
     Args:
         q: The value to calculate the probability of.
         df: The degrees of freedom of the distribution.
         loc: The location parameter of the distribution.
         scale: The scale parameter of the distribution.
         lower_tail: Whether to calculate the lower tail probability or not.
         log_prob: Whether to return the log probability or not.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cdf value of the given value for Student T distribution.
 
     Example:
         >>> pt(1.0, 1.0)
         Array([0.74999994], dtype=float32, weak_type=True)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
     p = filter_vmap(_pt)(q, df, loc, scale)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
-
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dt = filter_jit(filter_grad(_pt))
 
 
-@make_partial_pipe
 def dt(
     x: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the probability density function of a Student's t-distribution.
 
     Args:
         x: A float or array-like object representing the values at which to evaluate
         the probability density function.
         df: Degrees of freedom for the Student's t-distribution.
         loc: Location parameter for the Student's t-distribution. Defaults to 0.0.
         scale: Scale parameter for the Student's t-distribution. Defaults to 1.0.
         lower_tail: Whether to return the lower tail probability. Defaults to True.
         log_prob: Whether to return the log probability. Defaults to False.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability density function evaluated at `x`.
 
     Example:
         >>> dt(1.0, 1.0)
         Array([0.1591549], dtype=float32, weak_type=True)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
     grads = filter_vmap(_dt)(x, df, loc, scale)
-    if not lower_tail:
-        grads = 1 - grads
-    if log_prob:
-        grads = jnp.log(grads)
+    grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qt(
     q: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
 ):
+    df = lax.convert_element_type(df, q.dtype)
+    loc = lax.convert_element_type(loc, q.dtype)
+    scale = lax.convert_element_type(scale, q.dtype)
+    one = lax.convert_element_type(1, q.dtype)
     beta_value = tfp_special.betaincinv(0.5 * df, 0.5, 1 - jnp.abs(1 - 2 * q))
-    scaled_squared = df * (1 / beta_value - 1)
+    scaled_squared = df * (one / beta_value - one)
     scaled = jnp.sign(q - 0.5) * jnp.sqrt(scaled_squared)
     return scaled * scale + loc
 
 
-@make_partial_pipe
 def qt(
     p: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail=True,
     log_prob=False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Calculates the quantile of Student T distribution.
 
     Args:
         p: A float or array-like object representing the quantile to be calculated.
         df: An int, float, or array-like object representing the degrees of freedom.
         loc: An optional float or array-like object representing the location parameter. Defaults to 0.0.
         scale: An optional float or array-like object representing the scale parameter. Defaults to 1.0.
         lower_tail: A boolean indicating whether the lower tail should be used. Defaults to True.
         log_prob: A boolean indicating whether the probability should be logged. Defaults to False.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantile of the Student T distribution.
 
     Example:
         >>> qt(0.5, 1.0)
         Array([0.], dtype=float32, weak_type=True)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
+    p = _check_clip_probability(p, lower_tail=lower_tail, log_prob=log_prob)
     q = filter_vmap(_qt)(p, df, loc, scale)
     return q
 
 
 @filter_jit
 def _rt(
     key: KeyArray,
     df: Union[Int, Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(
             jnp.shape(df), jnp.shape(loc), jnp.shape(scale)
         )
     scale = jnp.broadcast_to(scale, sample_shape)
     loc = jnp.broadcast_to(loc, sample_shape)
     return jrand.t(key, df, sample_shape, dtype=dtype) * scale + loc
 
 
-@make_partial_pipe
 def rt(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     df: Union[Int, Float, ArrayLike] = None,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
     lower_tail: bool = True,
     log_prob: bool = False,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ) -> ArrayLike:
     """Generates random numbers from a t-distribution.
 
     Args:
         key: Type of the random number generator.
         sample_shape: Shape of the output array.
         df: Degrees of freedom.
         loc: Location parameter.
         scale: Scale parameter.
         lower_tail: Whether to return the lower tail probability. Defaults to True.
         log_prob: Whether to return the log probability. Defaults to False.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: Random numbers from a t-distribution.
 
     Example:
         >>> rt(key, (2, 3), 1.0)
         Array([[1.9982358e+02, 2.3699088e-01, 6.6509140e-01],
                 [5.3681795e-02, 3.3967651e+01, 6.8611817e+00]], dtype=float32)
     """
     rvs = _rt(key, df, loc, scale, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/distribution/_uniform.py` & `stamox-0.1.4/stamox/distribution/_weibull.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,183 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_grad, filter_jit, filter_vmap
+from jax import lax
 from jax._src.random import KeyArray, Shape
-from jaxtyping import ArrayLike, Bool, Float
+from jaxtyping import ArrayLike, Float
 
-from ..core import make_partial_pipe
+from ._utils import (
+    _check_clip_distribution_domain,
+    _check_clip_probability,
+    _post_process,
+    _promote_dtype_to_floating,
+)
 
 
 @filter_jit
-def _punif(
+def _pweibull(
     x: Union[Float, ArrayLike],
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
 ):
-    p = (x - mini) / (maxi - mini)
-    p = jnp.clip(p, a_min=mini, a_max=maxi)
-    return p
+    concentration = lax.convert_element_type(concentration, x.dtype)
+    scale = lax.convert_element_type(scale, x.dtype)
+    scaled_x = lax.div(x, scale)
+    powered = jnp.float_power(scaled_x, concentration)
+    return 1 - jnp.exp(-powered)
 
 
-@make_partial_pipe
-def punif(
+def pweibull(
     q: Union[Float, ArrayLike],
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
-    lower_tail: Bool = True,
-    log_prob: Bool = False,
-    dtype=jnp.float32,
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
+    lower_tail: bool = True,
+    log_prob: bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Computes the cumulative distribution function of the uniform distribution.
+    """Computes the cumulative distribution function of the Weibull distribution.
 
     Args:
         q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
-        mini (Union[Float, ArrayLike], optional): The minimum value of the uniform distribution. Defaults to 0.0.
-        maxi (Union[Float, ArrayLike], optional): The maximum value of the uniform distribution. Defaults to 1.0.
+        concentration (Union[Float, ArrayLike], optional): The concentration parameter of the Weibull distribution. Defaults to 0.0.
+        scale (Union[Float, ArrayLike], optional): The scale parameter of the Weibull distribution. Defaults to 1.0.
         lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
-        ArrayLike: The cumulative distribution function of the uniform distribution evaluated at `q`.
+        Array: The cumulative distribution function of the Weibull distribution evaluated at `q`.
 
     Example:
-        >>> punif(0.5)
-        Array([0.5], dtype=float32, weak_type=True)
+        >>> pweibull(1.0, concentration=1.0, scale=1.0)
     """
-    q = jnp.asarray(q, dtype=dtype)
+    q, _ = _promote_dtype_to_floating(q, dtype)
     q = jnp.atleast_1d(q)
-    p = filter_vmap(_punif)(q, mini, maxi)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    q = _check_clip_distribution_domain(q, lower=0.0)
+    p = filter_vmap(_pweibull)(q, concentration, scale)
+    p = _post_process(p, lower_tail=lower_tail, log_prob=log_prob)
     return p
 
 
-_dunif = filter_grad(filter_jit(_punif))
+_dweibull = filter_grad(filter_jit(_pweibull))
 
 
-@make_partial_pipe
-def dunif(
-    x: Union[Float, ArrayLike],
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
-    lower_tail: Bool = True,
-    log_prob: Bool = False,
-    dtype=jnp.float32,
+def dweibull(
+    x, concentration=0.0, scale=1.0, lower_tail=True, log_prob=False, dtype=None
 ) -> ArrayLike:
-    """Calculates the probability density function of a uniform distribution.
+    """Computes the probability density function of the Weibull distribution.
 
     Args:
-        x (Union[Float, ArrayLike]): The value or array of values for which to calculate the probability density.
-        mini (Union[Float, Array], optional): The lower bound of the uniform distribution. Defaults to 0.0.
-        maxi (Union[Float, Array], optional): The upper bound of the uniform distribution. Defaults to 1.0.
-        lower_tail (Bool, optional): Whether to calculate the lower tail probability. Defaults to True.
-        log_prob (Bool, optional): Whether to return the log probability. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        x (Union[Float, ArrayLike]): The value at which to evaluate the PDF.
+        concentration (Union[Float, ArrayLike], optional): The concentration parameter of the Weibull distribution. Defaults to 0.0.
+        scale (Union[Float, ArrayLike], optional): The scale parameter of the Weibull distribution. Defaults to 1.0.
+        lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (Optional[jnp.dtype], optional): The dtype of the output. Defaults to None.
+
 
     Returns:
-        ArrayLike: The probability density of the given value(s).
+        Array: The probability density function of the Weibull distribution evaluated at `x`.
 
     Example:
-        >>> dunif(0.5)
-        Array([1.], dtype=float32, weak_type=True)
+        >>> dweibull(0.5, 1.0, 1.0)
     """
-    x = jnp.asarray(x, dtype=dtype)
+    x, _ = _promote_dtype_to_floating(x, dtype)
     x = jnp.atleast_1d(x)
-    p = filter_vmap(_dunif)(x, mini, maxi)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
-    return p
+    x = _check_clip_distribution_domain(x, lower=0.0)
+    grads = filter_vmap(_dweibull)(x, concentration, scale)
+    grads = _post_process(grads, lower_tail=lower_tail, log_prob=log_prob)
+    return grads
 
 
 @filter_jit
-def _qunif(
+def _qweibull(
     q: Union[Float, ArrayLike],
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
-):
-    x = q * (maxi - mini) + mini
-    x = jnp.clip(x, a_min=mini, a_max=maxi)
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
+) -> ArrayLike:
+    concentration = lax.convert_element_type(concentration, q.dtype)
+    scale = lax.convert_element_type(scale, q.dtype)
+    one = lax.convert_element_type(1, q.dtype)
+    nlog_q = -lax.log(lax.sub(one, q))
+    inv_concentration = lax.div(one, concentration)
+    powerd = jnp.float_power(nlog_q, inv_concentration)
+    x = lax.mul(powerd, scale)
     return x
 
 
-@make_partial_pipe
-def qunif(
+def qweibull(
     p: Union[Float, ArrayLike],
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
-    lower_tail: Bool = True,
-    log_prob: Bool = False,
-    dtype=jnp.float32,
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
+    lower_tail: bool = True,
+    log_prob: bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """
-    Computes the quantile function of a uniform distribution.
+    """Computes the quantile function of the Weibull distribution.
 
     Args:
-        p (Union[Float, ArrayLike]): Quantiles to compute.
-        mini (Union[Float, Array], optional): Lower bound of the uniform distribution. Defaults to 0.0.
-        maxi (Union[Float, Array], optional): Upper bound of the uniform distribution. Defaults to 1.0.
-        lower_tail (Bool, optional): Whether to compute the lower tail or not. Defaults to True.
-        log_prob (Bool, optional): Whether to compute the log probability or not. Defaults to False.
-        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
+        p (Union[Float, ArrayLike]): The quantiles to compute.
+        concentration (Union[Float, ArrayLike], optional): The concentration parameter of the Weibull distribution. Defaults to 0.0.
+        scale (Union[Float, ArrayLike], optional): The scale parameter of the Weibull distribution. Defaults to 1.0.
+        lower_tail (bool, optional): Whether to compute the lower tail of the distribution. Defaults to True.
+        log_prob (bool, optional): Whether to compute the log probability of the distribution. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
+
 
     Returns:
-       ArrayLike: The quantiles of the uniform distribution.
+        Array: The computed quantiles.
 
     Example:
-        >>> qunif(0.5)
-        Array([0.5], dtype=float32, weak_type=True)
+        >>> qweibull(0.5, 1.0, 1.0)
     """
-    p = jnp.asarray(p, dtype=dtype)
+    p, _ = _promote_dtype_to_floating(p, dtype)
     p = jnp.atleast_1d(p)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.exp(p)
-    q = filter_vmap(_qunif)(p, mini, maxi)
+    p = _check_clip_probability(p, lower_tail, log_prob)
+    q = filter_vmap(_qweibull)(p, concentration, scale)
     return q
 
 
 @filter_jit
-def _runif(
+def _rweibull(
     key: KeyArray,
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
     sample_shape: Optional[Shape] = None,
-    dtype=jnp.float32,
+    dtype=jnp.float_,
 ):
-    return jrand.uniform(key, sample_shape, minval=mini, maxval=maxi, dtype=dtype)
+    return jrand.weibull_min(key, scale, concentration, sample_shape, dtype=dtype)
 
 
-@make_partial_pipe
-def runif(
+def rweibull(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
-    mini: Union[Float, ArrayLike] = 0.0,
-    maxi: Union[Float, ArrayLike] = 1.0,
-    lower_tail: Bool = True,
-    log_prob: Bool = False,
-    dtype=jnp.float32,
+    concentration: Union[Float, ArrayLike] = 0.0,
+    scale: Union[Float, ArrayLike] = 1.0,
+    lower_tail: bool = True,
+    log_prob: bool = False,
+    dtype=jnp.float_,
 ) -> ArrayLike:
-    """Generates random numbers from a uniform distribution.
+    """Generates samples from the Weibull distribution.
 
     Args:
-        key: A PRNGKey to use for generating the random numbers.
-        sample_shape: The shape of the output array.
-        mini: The minimum value of the uniform distribution.
-        maxi: The maximum value of the uniform distribution.
-        lower_tail: Whether to generate values from the lower tail of the distribution.
-        log_prob: Whether to return the log probability of the generated values.
-        dtype: The dtype of the output. Defaults to jnp.float32.
+        key (KeyArray): Random key used for generating random numbers.
+        sample_shape (Optional[Shape], optional): Shape of the output sample. Defaults to None.
+        concentration (Union[Float, ArrayLike], optional): Concentration parameter of the Weibull distribution. Defaults to 0.0.
+        scale (Union[Float, ArrayLike], optional): Scale parameter of the Weibull distribution. Defaults to 1.0.
+        lower_tail (bool, optional): Whether to return the lower tail probability. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (Optional[jnp.dtype], optional): The dtype of the output. Defaults to jnp.float_.
+
 
     Returns:
-        ArrayLike: An array of random numbers from a uniform distribution.
+        rvs (ArrayLike): Probability of the Weibull distribution.
 
     Example:
-        >>> runif(key, sample_shape=(2, 3))
-        Array([[0.57450044, 0.09968603, 0.7419659 ],
-                [0.8941783 , 0.59656656, 0.45325184]], dtype=float32)
-
+        >>> key = jax.random.PRNGKey(0)
+        >>> rweibull(key, 1.0, 1.0)
     """
-    rvs = _runif(key, mini, maxi, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _rweibull(key, concentration, scale, sample_shape, dtype=dtype)
+    rvs = _post_process(rvs, lower_tail=lower_tail, log_prob=log_prob)
     return rvs
```

### Comparing `stamox-0.1.3/stamox/experimental/better_partial.py` & `stamox-0.1.4/stamox/core/better_partial.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,31 +13,38 @@
     def __new__(cls, func, /, *args, **keywords) -> Self:
         if not callable(func):
             raise TypeError("the first argument must be callable")
 
         if hasattr(func, "func"):
             keywords = {**func.keywords, **keywords}
             func = func.func
-
         self = super(better_partial, cls).__new__(cls)
         # get all args name
         args_name = inspect.getfullargspec(func).args
+        keywords_default = {}
         self.args_name = args_name
         self.func = func
         unassign_argsname = [arg for arg in args_name if arg not in keywords]
+        # get default argnames and value
+        sig = inspect.signature(func)
+        for param in sig.parameters.values():
+            if param.default != inspect.Parameter.empty:
+                keywords_default[param.name] = param.default
         for i, arg in enumerate(unassign_argsname):
             if i < len(args):
                 keywords[arg] = args[i]
-        self.keywords = keywords
+        self.keywords = keywords_default
+        self.keywords.update(keywords)
 
         return self
 
     def __call__(self, *args, **keywords) -> _T:
         keywords = {**self.keywords, **keywords}
-        unassign_argsname = [arg for arg in self.args_name if arg not in keywords]
-        for i, arg in enumerate(unassign_argsname):
+        unassign_or_none_argsname = [
+            arg
+            for arg in self.args_name
+            if arg not in keywords or keywords[arg] is None
+        ]
+        for i, arg in enumerate(unassign_or_none_argsname):
             if i < len(args):
                 keywords[arg] = args[i]
-            else:
-                raise TypeError(f"missing required argument {arg}")
-
         return self.func(**keywords)
```

### Comparing `stamox-0.1.3/stamox/experimental/decomposition/_pca.py` & `stamox-0.1.4/stamox/experimental/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.3/stamox/experimental/maps/auto_map.py` & `stamox-0.1.4/stamox/experimental/maps/auto_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.3/stamox/experimental/maps/cube_map.py` & `stamox-0.1.4/stamox/experimental/maps/cube_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.3/stamox/formula/_formula.py` & `stamox-0.1.4/stamox/formula/_formula.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 @make_partial_pipe
 def get_design_matrices(
     data: pd.DataFrame,
     formula: str,
     eval_env=0,
     NA_action="drop",
     return_type="matrix",
-    dtype=jnp.float32,
+    dtype: jnp.dtype = None,
 ) -> Matrices:
     """Get design matrices from a formula and data.
 
     Args:
         data: A pandas DataFrame containing the data.
         formula: A string representation of a formula.
         eval_env: An environment mapping column names to arrays which patsy can use when evaluating a formula.
         NA_action: A string specifying how to handle missing values. One of "drop", "raise", or "na_action".
         return_type: A string specifying the return type. One of "matrix", "dataframe", or "design_info".
+        dtype: The data type to use for the design matrices.
 
     Returns:
         Matrices: A named tuple containing the design matrices for the response and predictors, as well as the names of the columns in each matrix.
 
     """
     y, X = patsy.dmatrices(
         formula, data, eval_env=eval_env, NA_action=NA_action, return_type=return_type
     )
+    if dtype is None:
+        dtype = jnp.promote_types(y.dtype, X.dtype)
     return Matrices(
         jnp.asarray(y, dtype=dtype),
         jnp.asarray(X, dtype=dtype),
         y.design_info.column_names,
         X.design_info.column_names,
     )
```

### Comparing `stamox-0.1.3/stamox/hypothesis/_bartlett.py` & `stamox-0.1.4/stamox/hypothesis/_bartlett.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# ::: stamox/hypothesis/_bartlett.py ::: 1 of 1 (100%)
-
 from functools import partial
 from typing import Sequence
 
 import jax.numpy as jnp
 from equinox import filter_jit
 from jax import vmap
 from jaxtyping import ArrayLike
@@ -46,25 +44,26 @@
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
     @property
     def df(self):
         return self.parameters
 
 
-def bartlett_test_fun(*samples: Sequence[ArrayLike]) -> BartlettTest:
+def bartlett_test(*samples: Sequence[ArrayLike]) -> BartlettTest:
     """Calculates the Bartlett test statistic for multiple samples.
 
     Args:
         *samples Sequence[ArrayLike]): A sequence of 1-D arrays, each containing
             a sample of scores. All samples must have the same length.
 
     Returns:
         BartlettTest: The Bartlett Test object.
 
     Example:
+        >>> from stamox.functions import bartlett_test
         >>> bartlett_test([1, 2, 3], [1, 2, 3])
         BartlettTest(statistic=0.0, parameters=1, p_value=1.0)
     """
     samples = jnp.vstack(samples)
     return _bartlett(samples)
```

### Comparing `stamox-0.1.3/stamox/hypothesis/_durbin_watson.py` & `stamox-0.1.4/stamox/hypothesis/_durbin_watson.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         axis (int, optional): The axis along which to compute the statistic. Defaults to 0.
 
     Returns:
         DurbinWatsonTest: The Durbin-Watson Test object.
 
     Example:
         >>> import jax.numpy as jnp
-        >>> from stamox.hypothesis import durbin_watson_test
+        >>> from stamox.functions import durbin_watson_test
         >>> resids = jnp.array([1, 2, 3, 4, 5])
         >>> durbin_watson_test(resids)
         Durbin-Waston Test(statistic=0.0, parameters=None, p_value=None)
     """
     resids = jnp.atleast_1d(resids)
     return _durbin_watson(resids, axis)
```

### Comparing `stamox-0.1.3/stamox/hypothesis/_friedman.py` & `stamox-0.1.4/stamox/hypothesis/_friedman.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             statistic, parameters, p_value, estimate, null_value, alternative, name
         )
     
     def __repr__(self):
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
 
-def friedman_test_fun(*samples: Sequence[ArrayLike]) -> FriedmanTest:
+def friedman_test(*samples: Sequence[ArrayLike]) -> FriedmanTest:
     """Computes the Friedman statistic for a set of samples.
 
     Args:
         *samples: A sequence of samples, each sample being a sequence of
             observations.
 
     Returns:
```

### Comparing `stamox-0.1.3/stamox/math/combination.py` & `stamox-0.1.4/stamox/math/combination.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from jax import lax
 from jax.scipy.special import gammaln
 
 from ..core import make_partial_pipe
 
 
 @make_partial_pipe
-def combination(k, n, dtype=jnp.int32):
+def combination(k, n):
     """Calculates the number of combinations of k elements from a set of n elements.
 
     Args:
         k (int or array): Number of elements to choose from the set.
         n (int): Size of the set.
 
     Returns:
         int or array: The number of combinations of k elements from a set of n elements.
 
     Example:
         >>> combination(2, 5)
         10
     """
-    k = jnp.asarray(k, dtype=dtype)
+    k = jnp.asarray(k, dtype=jnp.float_)
     k = jnp.atleast_1d(k)
     return filter_vmap(_comb)(k, n)
 
 
 @filter_jit
 def _cal_comb(k, n):
     log_kfrac = gammaln(k + 1)
```

### Comparing `stamox-0.1.3/stamox/regression/_base.py` & `stamox-0.1.4/stamox/regression/_base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.3/stamox/regression/_lm.py` & `stamox-0.1.4/stamox/regression/_lm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Tuple, Union
 
 import equinox as eqx
 import jax.numpy as jnp
+import numpy as np
 from jaxtyping import ArrayLike
 from pandas import DataFrame
 
-from ..core import make_partial_pipe
 from ..distribution import pF, pt
 from ..formula import get_design_matrices
 from ._base import RegState
 
 
 class OLSState(RegState):
     _X_names: List[str]
@@ -120,40 +120,39 @@
         )
 
     @property
     def resid_stderr(self):
         return jnp.sqrt(self.SSE / self.df_resid)
 
 
-@make_partial_pipe
 def lm(
     data: Union[List, Tuple, DataFrame, ArrayLike],
     formula=None,
     subset=None,
     weights=None,
     NA_action="drop",
     method="qr",
-    dtype=jnp.float32,
+    dtype: jnp.dtype = jnp.float_,
 ) -> OLSState:
     """Fits a linear model using the given data and parameters.
 
     Args:
         data (Union[List, Tuple, DataFrame, ArrayLike]): The data to fit the linear model with.
         formula (str, optional): A formula for the linear model. Defaults to None.
         subset (list, optional): A list of indices to use as a subset of the data. Defaults to None.
         weights (array-like, optional): An array of weights to apply to the data. Defaults to None.
         NA_action (str, optional): The action to take when encountering missing values. Defaults to "drop".
         method (str, optional): The method to use for fitting the linear model. Defaults to "qr".
-        dtype (jnp.float32, optional): The data type to use for the linear model. Defaults to jnp.float32.
+        dtype (jnp.float32, optional): The data type to use for the linear model. Defaults to jnp.float_.
 
     Returns:
         OLSState: The state of the fitted linear model.
 
     Example:
-        >>> from stamox.regression import lm
+        >>> from stamox.functions import lm
         >>> import pandas as pd
         >>> import numpy as np
         >>> np.random.seed(42)
         >>> X = np.random.uniform(size=(1000, 3))
         >>> y = (
                 3 * X[:, 0]
                 + 2 * X[:, 1]
@@ -174,32 +173,37 @@
             raise ValueError("formula is required when data is DataFrame")
         elif isinstance(data, list):
             y = data[0]
             X = data[1]
         elif isinstance(data, tuple):
             y = data[0]
             X = data[1]
-        elif isinstance(data, ArrayLike):
+        elif isinstance(data, jnp.ndarray) or isinstance(data, np.ndarray):
             y = data[:, 0]
             X = data[:, 1:]
         else:
             raise ValueError("data is not supported")
+
+        if dtype is None:
+            dtype = jnp.promote_types(y.dtype, X.dtype)
+        y = jnp.asarray(y, dtype=dtype)
+        X = jnp.asarray(X, dtype=dtype)
         X_names = None
         y_names = None
     else:
         matrices = get_design_matrices(data, formula, NA_action=NA_action, dtype=dtype)
         y = matrices.y
         X = matrices.X
         X_names = matrices.X_names
         y_names = matrices.y_names
     if subset is not None:
         y = y[subset, :]
         X = X[subset, :]
     if weights is not None:
-        weights = jnp.asarray(weights).reshape(-1, 1)
+        weights = jnp.asarray(weights, dtype=dtype).reshape(-1, 1)
         W = jnp.diag(weights.reshape(-1))
         y = jnp.multiply(y, weights)
         X = jnp.matmul(X.T, W).T
     return _fit_lm(X, y, method, X_names=X_names, y_names=y_names)
 
 
 @eqx.filter_jit
@@ -218,15 +222,15 @@
         X_pinv = jnp.linalg.inv(X.T @ X) @ X.T
     elif method == "qr":
         Q, R = jnp.linalg.qr(X)
         R_inv = jnp.linalg.inv(R)
         X_pinv = R_inv @ Q.T
     elif method == "svd":
         U, S, Vt = jnp.linalg.svd(X)
-        D = jnp.zeros((num_samples, in_features))
+        D = jnp.zeros((num_samples, in_features), dtype=X.dtype)
         D = D.at[:in_features, :in_features].set(jnp.diag(1 / S))
         X_pinv = Vt.T @ D.T @ U.T
     else:
         raise NotImplementedError("Not Implemented")
     coefs = X_pinv @ y
     _coefs_std = jnp.sqrt(jnp.diag(X_pinv @ X_pinv.T)).reshape(-1, 1)
     _fitted_values = X @ coefs
```

### Comparing `stamox-0.1.3/stamox/sample/_bootstrap.py` & `stamox-0.1.4/stamox/sample/_bootstrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from typing import Callable, TypeVar
 
 import jax.random as jrandom
 from equinox import filter_jit, filter_vmap
 from jaxtyping import ArrayLike, PyTree
 
-from ..core import make_partial_pipe
-
 
 ReturnValue = TypeVar("ReturnValue")
 
 
-@make_partial_pipe(name="bootstrap_sample")
 def bootstrap_sample(
     data: ArrayLike, num_samples: int, *, key: jrandom.KeyArray = None
 ) -> ArrayLike:
     """Generates `num_samples` bootstrap samples from `data` with replacement.
 
     Args:
         data (array-like): The original data.
@@ -23,15 +20,15 @@
 
     Returns:
         ArrayLike: An array of size `(num_samples, len(data))` containing the bootstrap samples.
 
     Example:
         >>> import jax.numpy as jnp
         >>> import jax.random as jrandom
-        >>> from stamox.sample import bootstrap_sample
+        >>> from stamox.functions import bootstrap_sample
         >>> data = jnp.arange(10)
         >>> key = jrandom.PRNGKey(0)
         >>> bootstrap_sample(data, num_samples=3, key=key)
         Array([[9, 1, 6, 2, 9, 3, 9, 9, 4, 5],
                 [4, 0, 4, 4, 6, 2, 5, 6, 5, 3],
                 [7, 6, 9, 0, 0, 7, 0, 5, 8, 4]], dtype=int32)
     """
@@ -47,15 +44,14 @@
         sample = data[sample_indices, ...]
         return sample
 
     samples = filter_vmap(sample_fn)(keys)
     return samples
 
 
-@make_partial_pipe(name="bootstrap")
 def bootstrap(
     data: ArrayLike,
     call: Callable[..., ReturnValue],
     num_samples: int,
     *,
     key: jrandom.KeyArray = None
 ) -> PyTree:
```

### Comparing `stamox-0.1.3/stamox/sample/_jackknife.py` & `stamox-0.1.4/stamox/sample/_jackknife.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import Callable, TypeVar
 
 import jax.numpy as jnp
 from equinox import filter_jit, filter_vmap
 from jaxtyping import ArrayLike, PyTree
 
-from ..core import make_partial_pipe
-
 
 ReturnValue = TypeVar("ReturnValue")
 
 
-def jackknife_sample_fun(data: ArrayLike) -> ArrayLike:
+def jackknife_sample(data: ArrayLike) -> ArrayLike:
     """Generates `num_samples` jackknife samples from `data` with replacement.
 
     Args:
         data (array-like): The original data.
 
     Returns:
         ArrayLike: An array of size (len(data)-1, len(data)) containing the jackknife samples.
 
     Example:
         >>> import jax.numpy as jnp
-        >>> from stamox.sample import jackknife_sample
+        >>> from stamox.functions import jackknife_sample
         >>> data = jnp.arange(3)
         >>> jackknife_sample(data)
         Array([[1, 2],
                 [0, 2],
                 [0, 1]], dtype=int32)
 
     """
@@ -38,15 +36,14 @@
         return x[idx]
 
     samples = filter_vmap(apply_except_one, in_axes=(None, 0))(data, jnp.arange(n))
 
     return samples
 
 
-@make_partial_pipe(name="jackknife")
 def jackknife(data: ArrayLike, call: Callable[..., ReturnValue]) -> PyTree:
     """Computes the jackknife estimate of a given data set.
 
     Args:
         data (ArrayLike): The data set to be analyzed.
         call (Callable[..., ReturnValue]): A function to be applied to each sample.
 
@@ -56,9 +53,9 @@
     Example:
         >>> import jax.numpy as jnp
         >>> from stamox.sample import jackknife
         >>> data = jnp.arange(3)
         >>> jackknife(data, lambda x: jnp.mean(x))
         Array([1.5, 1. , 0.5], dtype=float32)
     """
-    samples = jackknife_sample_fun(data)
+    samples = jackknife_sample(data)
     return filter_jit(filter_vmap(lambda x: call(x)))(samples)
```

### Comparing `stamox-0.1.3/stamox.egg-info/PKG-INFO` & `stamox-0.1.4/stamox.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -42,117 +42,139 @@
 *calculate cdf*
 
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
-pip install stamox
+pip install -U stamox
+# or
+pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
 
 ### Similar but faster distribution functions to `R`
 
+You can simply import all functions from `stamox.functions`
+
 ```python
-from stamox.distribution import *
+from stamox.functions import dnorm, pnorm, qnorm, rnorm
 import jax.random as jrandom
 
 key = jrandom.PRNGKey(20010813)
 
 # random
 x = rnorm(key, sample_shape=(1000, ))
 # cdf
-pnorm(x)
+prob = pnorm(x)
 # ppf
-qnorm(x)
+qntl = qnorm(prob)
 # pdf
 dnorm(x)
 ```
 
 ### Fearless Pipeable
 
 `>>` is the pipe operator, which is the similar to `|>` in `F#` and `Elixir` or `%>%` in `R`.
 
-* Internal Functions Pipeable
+* You can simply import all pipeable functions from `pipe_functions`
 
 ```python
 import jax.random as jrandom
-from stamox.basic import scale
-from stamox.core import pipe_jit
-from stamox.distribution import rnorm
-from stamox.regression import lm
+import stamox.pipe_functions as PF
+from stamox import pipe_jit
 
 key = jrandom.PRNGKey(20010813)
 
 @pipe_jit
 def f(x):
     return [3 * x[:, 0] + 2 * x[:, 1] - x[:, 2], x] # [y, X]
-pipe = rnorm(sample_shape=(1000, 3)) >> f >> lm
+pipe = PF.rnorm(sample_shape=(1000, 3)) >> f >> PF.lm
 state = pipe(key)
 print(state.params)
 ```
 
+### Linear Regression with Formula
+
+```python
+import pandas as pd
+import numpy as np
+from stamox.functions import lm # or from stamox.pipe_functions import lm
+
+
+x = np.random.uniform(size=(1000, 3))
+y = 2 * x[:,0] + 3 * x[:,1] + 4 * x[:,2] + np.random.normal(size=1000)
+df = pd.DataFrame(x, columns=['x1', 'x2', 'x3'])
+df['y'] = y
+
+lm(df, 'y~x1+x2+x3').params
+```
+
 * Custom Functions Pipeable
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
+from stamox import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
 import jax.random as jrandom
 
 x = jnp.ones((1000, ))
 # single input, simply add make pipe
 @make_pipe
 def f(x):
     return x ** 2
 
-# multiple input, add make partial pipe
+# multiple input, decorate with make partial pipe
 @make_partial_pipe
 def g(x, y):
     return x + y
 
-# Notice Only One Positional Argument Can Be Received Along the pipe
+# x -> f -> g(y=2.) -> f -> g(y=3.) -> f
 h = Pipeable(x) >> f >> g(y=2.) >> f >> g(y=3.) >> f
+# h is a Pipeable object, you can call it to get the result
 print(h())
 ```
 
 * Compatible With `JAX` and `Equinox`
 
 You can use autograd features from `JAX` and `Equinox` with `Stamox` easily.
 
 ```python
-from stamox.core import make_pipe, make_partial_pipe, Pipeable
 import jax.numpy as jnp
+from stamox import make_partial_pipe
 from equinox import filter_jit, filter_vmap, filter_grad
 
 @make_partial_pipe
 @filter_jit
 @filter_vmap
 @filter_grad
 def f(x, y):
     return y * x ** 3
-       
-f(y=3.)(jnp.array([1., 2., 3.]))
+
+# df/dx = 3y * x^2
+g = f(y=3.) # derive with respect to x given y=3
+g(jnp.array([1., 2., 3.]))
 ```
 
 Or vmap, pmap, jit features integrated with `Stamox`:
 
 ```python
-from stamox.core import pipe_vmap, pipe_jit
+from stamox import pipe_vmap, pipe_jit
 
 @pipe_vmap
 @pipe_jit
 def f(x):
     return x ** 2
 
-f(jnp.array([1., 2., 3.]))
+g = f >> f >> f
+print(g(jnp.array([1, 2, 3])))
 ```
 
 ## Acceleration Support
 
 `JAX` can be accelerated by `GPU` and `TPU`. So, `Stamox` is compatible with them.
 
 ## See More
```

### Comparing `stamox-0.1.3/stamox.egg-info/SOURCES.txt` & `stamox-0.1.4/stamox.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 LICENCE
 README.md
 pyproject.toml
 setup.py
 stamox/__init__.py
 stamox/basic.py
+stamox/functions.py
+stamox/pipe_functions.py
 stamox/transformation.py
 stamox.egg-info/PKG-INFO
 stamox.egg-info/SOURCES.txt
 stamox.egg-info/dependency_links.txt
 stamox.egg-info/requires.txt
 stamox.egg-info/top_level.txt
 stamox/anova/__init__.py
 stamox/anova/one_way/__init__.py
 stamox/anova/one_way/_aov.py
 stamox/cluster/__init__.py
 stamox/cluster/_kmeans.py
 stamox/core/__init__.py
 stamox/core/_func_state.py
-stamox/core/_utils.py
 stamox/core/base.py
+stamox/core/better_partial.py
 stamox/core/jit.py
 stamox/core/maps.py
 stamox/core/pipe.py
+stamox/correlation/__init__.py
+stamox/correlation/_cor.py
+stamox/correlation/_pearson.py
+stamox/correlation/_spearman.py
 stamox/distribution/__init__.py
 stamox/distribution/_beta.py
 stamox/distribution/_binomial.py
 stamox/distribution/_cauchy.py
 stamox/distribution/_chisq.py
 stamox/distribution/_ecdf.py
 stamox/distribution/_exp.py
 stamox/distribution/_f.py
 stamox/distribution/_gamma.py
-stamox/distribution/_geom.py
 stamox/distribution/_laplace.py
 stamox/distribution/_normal.py
 stamox/distribution/_pareto.py
 stamox/distribution/_poisson.py
-stamox/distribution/_q_discrete_search.py
-stamox/distribution/_rademacher.py
 stamox/distribution/_t.py
-stamox/distribution/_triangular.py
 stamox/distribution/_uniform.py
+stamox/distribution/_utils.py
 stamox/distribution/_weibull.py
 stamox/experimental/__init__.py
-stamox/experimental/better_partial.py
 stamox/experimental/decomposition/__init__.py
 stamox/experimental/decomposition/_pca.py
 stamox/experimental/maps/__init__.py
 stamox/experimental/maps/auto_map.py
 stamox/experimental/maps/cube_map.py
-stamox/experimental/nn/__init__.py
 stamox/formula/__init__.py
 stamox/formula/_formula.py
 stamox/hypothesis/__init__.py
 stamox/hypothesis/_bartlett.py
 stamox/hypothesis/_base.py
 stamox/hypothesis/_durbin_watson.py
 stamox/hypothesis/_friedman.py
-stamox/hypothesis/_p.py
-stamox/hypothesis/_pearsonr.py
-stamox/hypothesis/_shapiro_wilk.py
-stamox/hypothesis/_t.py
-stamox/hypothesis/cor2ci.py
-stamox/hypothesis/cor2p.py
-stamox/hypothesis/corr.py
 stamox/math/__init__.py
 stamox/math/combination.py
 stamox/math/special.py
 stamox/regression/__init__.py
 stamox/regression/_base.py
 stamox/regression/_lm.py
 stamox/sample/__init__.py
 stamox/sample/_bootstrap.py
 stamox/sample/_jackknife.py
-tests/test_basic.py
+tests/test_basic.py
+tests/test_transformation.py
```

### Comparing `stamox-0.1.3/tests/test_basic.py` & `stamox-0.1.4/tests/test_basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 """Test Basic Functions"""
 import numpy as np
-from absl.testing import absltest
-from jax._src import test_util as jtest
 
-from stamox.basic import mean, median, scale, sd, var
-from stamox.core import Pipeable
+from stamox import Pipeable
+from stamox.pipe_functions import mean, median, scale, sd, var
 
 
-class BasicTest(jtest.JaxTestCase):
-    def test_mean(self):
-        a = np.random.normal(size=(10000, 3))
-        self.assertAllClose(mean(a, axis=1), np.mean(a, axis=1))
-
-    def test_pipe_mean(self):
-        a = np.random.normal(size=(10000, 3))
-        p = Pipeable(a) >> mean(axis=1)
-        self.assertAllClose(p(a), np.mean(a, axis=1))
-
-    def test_median(self):
-        a = np.random.normal(size=(10000, 3))
-        self.assertAllClose(median(a, axis=1), np.median(a, axis=1))
-
-    def test_pipe_median(self):
-        a = np.random.normal(size=(10000, 3))
-        p = Pipeable(a) >> median(axis=1)
-        self.assertAllClose(p(a), np.median(a, axis=1))
-
-    def test_std(self):
-        a = np.random.normal(size=(10000, 3))
-        self.assertAllClose(sd(a, axis=1), np.std(a, axis=1))
-
-    def test_pipe_std(self):
-        a = np.random.normal(size=(10000, 3))
-        p = Pipeable(a) >> sd(axis=1)
-        self.assertAllClose(p(a), np.std(a, axis=1))
-
-    def test_var(self):
-        a = np.random.normal(size=(10000, 3))
-        self.assertAllClose(var(a, axis=1), np.var(a, axis=1))
-
-    def test_pipe_var(self):
-        a = np.random.normal(size=(10000, 3))
-        p = Pipeable(a) >> var(axis=1)
-        self.assertAllClose(p(a), np.var(a, axis=1))
-
-    def test_scale(self):
-        a = np.random.normal(size=(10000, 3)) * 2
-        self.assertAllClose(
-            scale(a), (a - np.mean(a, axis=0)) / np.std(a, axis=0, ddof=1)
-        )
+def test_mean():
+    a = np.random.normal(size=(10000, 3))
+    np.testing.assert_allclose(mean(a, axis=1), np.mean(a, axis=1))
 
 
-if __name__ == "__main__":
-    absltest.main(testLoader=jtest.JaxTestLoader())
+def test_pipe_mean():
+    a = np.random.normal(size=(10000, 3))
+    p = Pipeable(a) >> mean(axis=1)
+    np.testing.assert_allclose(p(a), np.mean(a, axis=1))
+
+
+def test_median():
+    a = np.random.normal(size=(10000, 3))
+    np.testing.assert_allclose(median(a, axis=1), np.median(a, axis=1))
+
+
+def test_pipe_median():
+    a = np.random.normal(size=(10000, 3))
+    p = Pipeable(a) >> median(axis=1)
+    np.testing.assert_allclose(p(a), np.median(a, axis=1))
+
+
+def test_std():
+    a = np.random.normal(size=(10000, 3))
+    np.testing.assert_allclose(sd(a, axis=1), np.std(a, axis=1))
+
+
+def test_pipe_std():
+    a = np.random.normal(size=(10000, 3))
+    p = Pipeable(a) >> sd(axis=1)
+    np.testing.assert_allclose(p(a), np.std(a, axis=1))
+
+
+def test_var():
+    a = np.random.normal(size=(10000, 3))
+    np.testing.assert_allclose(var(a, axis=1), np.var(a, axis=1))
+
+
+def test_pipe_var():
+    a = np.random.normal(size=(10000, 3))
+    p = Pipeable(a) >> var(axis=1)
+    np.testing.assert_allclose(p(a), np.var(a, axis=1))
+
+
+def test_scale():
+    a = np.random.normal(size=(10000, 3)) * 2
+    np.testing.assert_allclose(
+        scale(a), (a - np.mean(a, axis=0)) / np.std(a, axis=0, ddof=1)
+    )
```

