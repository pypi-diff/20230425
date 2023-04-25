# Comparing `tmp/phdu-1.7b9.tar.gz` & `tmp/phdu-1.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.7b9.tar", last modified: Tue Apr 18 11:22:58 2023, max compression
+gzip compressed data, was "phdu-1.8b1.tar", last modified: Tue Apr 25 09:26:28 2023, max compression
```

## Comparing `phdu-1.7b9.tar` & `phdu-1.8b1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.990646 phdu-1.7b9/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.7b9/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:22:57.990646 phdu-1.7b9/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.7b9/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.898642 phdu-1.7b9/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.7b9/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.7b9/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.7b9/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.7b9/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.7b9/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.7b9/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.938644 phdu-1.7b9/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.7b9/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.7b9/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.7b9/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    13090 2023-04-18 11:06:30.000000 phdu-1.7b9/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.7b9/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.966645 phdu-1.7b9/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.7b9/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.7b9/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      853 2022-11-08 18:00:22.000000 phdu-1.7b9/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.7b9/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    27790 2023-04-18 11:22:26.000000 phdu-1.7b9/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.7b9/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.7b9/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.974646 phdu-1.7b9/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.7b9/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.7b9/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.7b9/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.986646 phdu-1.7b9/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.7b9/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.7b9/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.7b9/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3581 2023-02-08 11:11:43.000000 phdu-1.7b9/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.926643 phdu-1.7b9/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-18 11:22:57.998647 phdu-1.7b9/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-18 11:22:37.000000 phdu-1.7b9/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.919133 phdu-1.8b1/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.8b1/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-25 09:26:28.919133 phdu-1.8b1/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.8b1/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.835129 phdu-1.8b1/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.8b1/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.8b1/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.8b1/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.8b1/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.8b1/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.8b1/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.871131 phdu-1.8b1/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.8b1/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.8b1/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.8b1/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    13684 2023-04-25 09:22:33.000000 phdu-1.8b1/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.8b1/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.895132 phdu-1.8b1/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.8b1/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.8b1/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.8b1/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.8b1/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    27792 2023-04-25 08:51:16.000000 phdu-1.8b1/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.8b1/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.8b1/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.903132 phdu-1.8b1/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.8b1/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.8b1/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.8b1/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.915133 phdu-1.8b1/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.8b1/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.8b1/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.8b1/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4127 2023-04-25 08:51:16.000000 phdu-1.8b1/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 09:26:28.859130 phdu-1.8b1/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-25 09:26:28.000000 phdu-1.8b1/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-25 09:26:28.000000 phdu-1.8b1/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-25 09:26:28.000000 phdu-1.8b1/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-25 09:26:28.000000 phdu-1.8b1/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-25 09:26:28.000000 phdu-1.8b1/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-25 09:26:28.923133 phdu-1.8b1/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-25 09:26:17.000000 phdu-1.8b1/setup.py
```

### Comparing `phdu-1.7b9/LICENSE.md` & `phdu-1.8b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/PKG-INFO` & `phdu-1.8b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b9
+Version: 1.8b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b9/README.md` & `phdu-1.8b1/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/_helper.py` & `phdu-1.8b1/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/clustering.py` & `phdu-1.8b1/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/decomposition.py` & `phdu-1.8b1/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/np_utils.py` & `phdu-1.8b1/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/pd_utils.py` & `phdu-1.8b1/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/plots/base.py` & `phdu-1.8b1/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/plots/plotly_utils.py` & `phdu-1.8b1/phdu/plots/plotly_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,51 +142,59 @@
     if label is not None:
         yrange = [*get_common_range(fig, axes=["y"]).values()][0]
         fig.add_trace(go.Scatter(x=[1000], y=[1000], mode="markers", name=label, showlegend=True,
                                  marker=dict(symbol="square", color=color, size=22), line=dict(color="gray", width=2)))
         fig.update_layout(**mod_range(fig, ([-0.25, len(x)-0.75], yrange)))
     return fig
 
-def CI_ss_plot(df, label=None, width=0.05, ms=10, ns_color='#323232', ss_color=next(plotly_default_colors()), **CI_plot_kwargs):
+def CI_ss_plot(df, label=False, width=0.05, ms=10, ns_color='#323232', ss_lower_color='#1f77b4', ss_upper_color='#ff7f0e', **CI_plot_kwargs):
     """
     df: Dataframe containing the x coordinate in the index
         and columns:
             - 'sample stat': sample statistic
             - 'CI':          confidence interval
             - 'lb':          lower bound
             - 'ub':          upper bound
     """
     def map_to_nan(x, bool_arr):
         y = x.copy()
         y[bool_arr] = np.NaN
         return y
-    significant = np.sign(df['lb']) == np.sign(df['ub'])
-    df_ns, df_ss = df.copy(), df.copy()
+    lb_sign = np.sign(df['lb'])
+    ss = lb_sign == np.sign(df['ub'])
+    ss_upper = ss & (lb_sign == 1)
+    ss_lower = ss & (lb_sign == -1)
+    df_ns, df_ss_upper, df_ss_lower = df.copy(), df.copy(), df.copy()
     cis = np.vstack(df.CI.values)
-    df_ns['CI'] = map_to_nan(cis, significant).tolist()
-    df_ss['CI'] = map_to_nan(cis, ~significant).tolist()
+    df_ns['CI'] = map_to_nan(cis, ss).tolist()
+    df_ss_upper['CI'] = map_to_nan(cis, ~ss_upper).tolist()
+    df_ss_lower['CI'] = map_to_nan(cis, ~ss_lower).tolist()
     # NS intervals
-    fig = CI_plot(df_ns.index, df_ns['sample stat'].values, np.vstack(df_ns['CI'].values), width=width, ms=ms, color=color_std(ns_color, opacity=0.55),
+    fig = CI_plot(df_ns.index, df_ns['sample stat'].values, np.vstack(df_ns['CI'].values), width=width, ms=ms, color=color_std(ns_color, opacity=0.55), label='Not SS' if label else None,
                   **CI_plot_kwargs)
     # Adding significant intervals
-    fig = CI_plot(df_ss.index, df_ss['sample stat'].values, np.vstack(df_ss['CI'].values), width=width, ms=ms, fig=fig, color=color_std(ss_color, opacity=0.2))
+    figdata = {'SS (>0)': (df_ss_upper, ss_upper_color), 'SS (<0)': (df_ss_lower, ss_lower_color)}
+    for label_ss, (df_ss, ss_color) in figdata.items():
+        fig = CI_plot(df_ss.index, df_ss['sample stat'].values, np.vstack(df_ss['CI'].values), width=width, ms=ms, fig=fig, color=color_std(ss_color, opacity=0.2), label=label_ss if label else None)
     # colorizing the index
-    def colorize(index):
+    def colorize(index_upper, index_lower):
         """
         index: pd.Series where index is the feature name and value is of type bool.
         """
         ticktext = []
-        for f, is_ss in index.items():
-            if is_ss:
-                ticktext.append(f"<span style='color:{str(ss_color)}'> {str(f)} </span>")
+        for f, is_ss_upper in index_upper.items():
+            if is_ss_upper:
+                ticktext.append(f"<span style='color:{str(ss_upper_color)}'> {str(f)} </span>")
+            elif index_lower[f]: # is_ss_lower
+                ticktext.append(f"<span style='color:{str(ss_lower_color)}'> {str(f)} </span>")
             else:
                 ticktext.append(f"<span style='color:{str(ns_color)}'> {str(f)} </span>")
         return ticktext
-    ticktext = colorize(significant)
-    fig.update_layout(xaxis=dict(tickmode='array', ticktext=ticktext, tickvals=np.arange(significant.size)))
+    ticktext = colorize(ss_upper, ss_lower)
+    fig.update_layout(xaxis=dict(tickmode='array', ticktext=ticktext, tickvals=np.arange(ss.size)))
     return fig
 
 def permtest_plot(df, H1="", colorscale="Inferno", log=True, height=800, width=1000, font_size=40, bar_len=0.9, bar_x=0.95, bar_thickness=100):
     """H1 should not contain latex code. Use unicode and HTML for super/sub-indices."""
     if log:
         df = np.log10(df)
         zmin, zmax = np.log10(0.05), 0
```

### Comparing `phdu-1.7b9/phdu/script_fmt.py` & `phdu-1.8b1/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/_integration.py` & `phdu-1.8b1/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/_plots.py` & `phdu-1.8b1/phdu/stats/_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..plots.plotly_utils import get_figure
 
 def qqplot(x, alpha=0.3, ms=20):
         pp = sm.ProbPlot(x, fit=True)
         qq = pp.qqplot(marker='.', markerfacecolor='k', markeredgecolor='k', alpha=alpha, markersize=ms)
         sm.qqline(qq.axes[0], line='45', fmt='k--')
         return plt.gcf()
-    
+
 def density_kernel(*X, cov_factor=0.1, n_points=300, **kwargs):
     fig = get_figure(yaxis_title="Probability density", **kwargs)
     for x in X:
         xs, density = _preprocess.density_kernel(x, cov_factor=cov_factor, n_points=n_points)
-        
+
         fig.add_trace(go.Scatter(x=xs, y=density, mode="lines", showlegend=False, line_width=4))
-    return fig
+    return fig
```

### Comparing `phdu-1.7b9/phdu/stats/bootstrap.py` & `phdu-1.8b1/phdu/stats/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         boot_sample[i] = func(r)
     return boot_sample
 
 @njit
 def resample_twosamples_nb(X1, X2, func, output_len=1, R=int(1e5), seed=0, smooth=False, N=0):
     """Xi: array of shape (N_samples, n_vars)."""
     data_resampled_1 = resample_nb_X(X1, R=R, seed=seed, smooth=smooth, N=N)
-    data_resampled_2 = resample_nb_X(X2, R=R, seed=seed, smooth=smooth, N=N)
+    data_resampled_2 = resample_nb_X(X2, R=R, seed=seed+1, smooth=smooth, N=N)
 
     boot_sample = np.empty((R, output_len))
     for i, (r1, r2) in enumerate(zip(data_resampled_1, data_resampled_2)):
         boot_sample[i] = func(r1, r2)
     return boot_sample
 
 def resample_twosamples(X1, X2, func, output_len=1, R=int(1e5), seed=0, smooth=False, N=0):
```

### Comparing `phdu-1.7b9/phdu/stats/conf_interval.py` & `phdu-1.8b1/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/corr.py` & `phdu-1.8b1/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/rtopy/_helper.py` & `phdu-1.8b1/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/rtopy/resample.py` & `phdu-1.8b1/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/stats/test/permutation.py` & `phdu-1.8b1/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/phdu/storage.py` & `phdu-1.8b1/phdu/storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 import re
 
 parent_dir =  'data'
 
 def move_files(keyword, folder=None, parent_dir=parent_dir, verbose=1):
     """
     Moves all files in the parent directory starting with a keyword to a folder.
-    
-    Attributes:    
+
+    Attributes:
         - keyword: keyword to look for during file matching-
         - folder: Created folder to store all files matched by the keyword
         - parend_dir: Initial directory in which the files are contained.
     """
     folder = folder if folder is not None else keyword
     Path(os.path.join(parent_dir, folder)).mkdir(exist_ok=True, parents=True)
     processed = 0
     for path in os.listdir(parent_dir):
         if path == folder:
             continue
         else:
             if re.findall(key, path):
-                os.rename(os.path.join(parent_dir, path), 
+                os.rename(os.path.join(parent_dir, path),
                           os.path.join(parent_dir, folder, path))
                 processed += 1
     if verbose:
-        print(f"Moved {processed} files from '{parent_dir}' to '{folder}' subdirectory.")        
+        print(f"Moved {processed} files from '{parent_dir}' to '{folder}' subdirectory.")
     return
 
 def delete_files_by_ext(parent_dir, extensions, verbose=1):
     """
     Removes files in parent_dir with extensions starting by (or being equal to) a certain character.
     """
     deleted = 0
     for path in os.listdir(parent_dir):
         for extension in extensions:
             if os.path.splitext(path)[1].startswith(extension):
                 os.remove(os.path.join(parent_dir, path))
                 deleted += 1
     if verbose:
-        print(f"Deleted {deleted} files.")        
+        print(f"Deleted {deleted} files.")
     return
 
 def delete_stdin_files(parent_dir="nuredduna_programmes/stdin_files", verbose=1, completed_only=True, key="Done", key_search="any"):
     """
     Removes nuredduna standard input (stdin) files, of the form python.exxxx (s. error) and python.oxxxx (s. output).
     key_search:  sets how the key is looked in a file line:    - any:   key in any position
                                                                - start.
@@ -57,38 +57,53 @@
             find_key = lambda l: key in l
         elif key_search == "start":
             find_key = lambda l: l.startswith(key)
         elif key_search == 'end':
             find_key = lambda l: l.endswith(key)
         else:
             raise ValueError(f"key_search '{key_search}' not valid. Available: 'any', 'start', 'end'.")
-        
+
         deleted_programs = 0
         deleted_files = 0
         for f in os.listdir(parent_dir):
             if f.endswith("out"):
                 ff = os.path.join(parent_dir, f)
                 if any(find_key(l) for l in open(ff).readlines()):
                     os.remove(ff)
                     deleted_programs += 1
                     deleted_files += 1
                     ff_err = "{}.err".format(os.path.splitext(ff)[0])
                     if Path(ff_err).exists():
                         os.remove(ff_err)
                         deleted_files += 1
         if verbose:
-            print(f"Deleted {deleted_files} files ({deleted_programs} completed programmes).")   
+            print(f"Deleted {deleted_files} files ({deleted_programs} completed programmes).")
     else:
         delete_files_by_ext(parent_dir, [".e", ".o"], verbose)
     return
 
 def empty_trash(verbose=1):
     home = os.path.expanduser("~")
     binDir = f"{home}/.local/share/Trash"
     deleted = 0
     for root, dirs, files in os.walk(binDir, topdown=False):
         for name in files:
             os.remove(os.path.join(root, name))
             deleted += 1
     if verbose:
         print(f"Deleted {deleted} files.")
-    return
+    return
+
+
+def delete_files_by_key(root, keys):
+    """Delete all files in root and following subdirectories containing at least one of the keys."""
+    # tree walk starting in directory 'data':
+    root = 'data'
+    count = 0
+    for dirpath, dirnames, filenames in os.walk(root):
+        # delete files containing 'DBS' or 'control'
+        for filename in filenames:
+            if any(key in filename for key in keys):
+                os.remove(os.path.join(dirpath, filename))
+                count += 1
+    print(f"Deleted {count} files containing at least one of {keys}")
+    return
```

### Comparing `phdu-1.7b9/phdu.egg-info/PKG-INFO` & `phdu-1.8b1/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b9
+Version: 1.8b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b9/phdu.egg-info/SOURCES.txt` & `phdu-1.8b1/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.7b9/setup.py` & `phdu-1.8b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.7.b9',
+    version='1.8.b1',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

