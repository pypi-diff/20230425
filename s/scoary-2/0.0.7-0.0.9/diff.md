# Comparing `tmp/scoary-2-0.0.7.tar.gz` & `tmp/scoary-2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoary-2-0.0.7.tar", max compression
+gzip compressed data, was "scoary-2-0.0.9.tar", max compression
```

## Comparing `scoary-2-0.0.7.tar` & `scoary-2-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      703 2022-07-06 16:03:49.983158 scoary-2-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1966 2022-05-11 12:05:34.227855 scoary-2-0.0.7/scoary/KeyValueStore.py
--rw-r--r--   0        0        0     8991 2022-05-17 11:04:53.732433 scoary-2-0.0.7/scoary/ScoaryTree.py
--rw-r--r--   0        0        0      172 2022-05-16 13:34:58.710034 scoary-2-0.0.7/scoary/__init__.py
--rw-r--r--   0        0        0    12523 2022-07-05 10:52:21.895782 scoary-2-0.0.7/scoary/analyze_trait.py
--rw-r--r--   0        0        0     7075 2022-06-30 06:21:54.084177 scoary-2-0.0.7/scoary/final_overview.py
--rw-r--r--   0        0        0      209 2022-05-18 12:01:07.252515 scoary-2-0.0.7/scoary/init_multiprocessing.py
--rw-r--r--   0        0        0     5245 2022-07-06 15:59:38.563926 scoary-2-0.0.7/scoary/load_genes.py
--rw-r--r--   0        0        0    16467 2022-07-06 15:55:20.707657 scoary-2-0.0.7/scoary/load_traits.py
--rw-r--r--   0        0        0     3150 2022-01-28 10:49:39.798770 scoary-2-0.0.7/scoary/newick.py
--rw-r--r--   0        0        0     3627 2022-06-30 06:21:54.085177 scoary-2-0.0.7/scoary/permutations.py
--rw-r--r--   0        0        0    10929 2022-07-06 16:02:54.956670 scoary-2-0.0.7/scoary/picking.py
--rw-r--r--   0        0        0     2079 2022-05-19 15:51:56.608248 scoary-2-0.0.7/scoary/progressbar.py
--rw-r--r--   0        0        0    12045 2022-07-05 09:26:28.693578 scoary-2-0.0.7/scoary/scoary.py
--rw-r--r--   0        0        0    17258 2022-05-17 14:04:15.239665 scoary-2-0.0.7/scoary/scoary_1_picking.py
--rw-r--r--   0        0        0     1344 2022-06-30 06:21:54.086177 scoary-2-0.0.7/scoary/templates/config.json
--rw-r--r--   0        0        0     1406 2022-03-18 14:45:44.178049 scoary-2-0.0.7/scoary/templates/favicon.ico
--rw-r--r--   0        0        0      966 2022-05-03 12:46:21.149074 scoary-2-0.0.7/scoary/templates/overview.css
--rw-r--r--   0        0        0     1896 2022-05-19 12:44:39.803241 scoary-2-0.0.7/scoary/templates/overview.html
--rw-r--r--   0        0        0     7142 2022-05-19 12:49:30.033855 scoary-2-0.0.7/scoary/templates/overview.js
--rw-r--r--   0        0        0     1741 2022-06-30 06:21:54.058177 scoary-2-0.0.7/scoary/templates/trait.css
--rw-r--r--   0        0        0     3836 2022-05-19 12:42:46.518804 scoary-2-0.0.7/scoary/templates/trait.html
--rw-r--r--   0        0        0    32887 2022-05-19 15:05:56.281180 scoary-2-0.0.7/scoary/templates/trait.js
--rw-r--r--   0        0        0     3003 2022-04-04 09:39:33.342139 scoary-2-0.0.7/scoary/upgma.py
--rw-r--r--   0        0        0     9369 2022-07-05 09:26:28.670578 scoary-2-0.0.7/scoary/utils.py
--rw-r--r--   0        0        0      949 2022-07-06 16:04:03.688609 scoary-2-0.0.7/setup.py
--rw-r--r--   0        0        0      678 2022-07-06 16:04:03.688907 scoary-2-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      703 2022-09-30 09:36:06.688489 scoary-2-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1966 2022-05-11 12:05:34.227855 scoary-2-0.0.9/scoary/KeyValueStore.py
+-rw-r--r--   0        0        0     8991 2022-05-17 11:04:53.732433 scoary-2-0.0.9/scoary/ScoaryTree.py
+-rw-r--r--   0        0        0      172 2022-05-16 13:34:58.710034 scoary-2-0.0.9/scoary/__init__.py
+-rw-r--r--   0        0        0    12523 2022-07-05 10:52:21.895782 scoary-2-0.0.9/scoary/analyze_trait.py
+-rw-r--r--   0        0        0     7117 2022-09-30 08:38:59.338790 scoary-2-0.0.9/scoary/final_overview.py
+-rw-r--r--   0        0        0      209 2022-05-18 12:01:07.252515 scoary-2-0.0.9/scoary/init_multiprocessing.py
+-rw-r--r--   0        0        0     5160 2022-09-30 08:43:49.437429 scoary-2-0.0.9/scoary/load_genes.py
+-rw-r--r--   0        0        0    16259 2022-09-30 08:31:28.772737 scoary-2-0.0.9/scoary/load_traits.py
+-rw-r--r--   0        0        0     3150 2022-01-28 10:49:39.798770 scoary-2-0.0.9/scoary/newick.py
+-rw-r--r--   0        0        0     3627 2022-06-30 06:21:54.085177 scoary-2-0.0.9/scoary/permutations.py
+-rw-r--r--   0        0        0    10929 2022-07-06 16:02:54.956670 scoary-2-0.0.9/scoary/picking.py
+-rw-r--r--   0        0        0     2079 2022-05-19 15:51:56.608248 scoary-2-0.0.9/scoary/progressbar.py
+-rw-r--r--   0        0        0    12133 2022-08-29 11:01:50.335254 scoary-2-0.0.9/scoary/scoary.py
+-rw-r--r--   0        0        0    17258 2022-05-17 14:04:15.239665 scoary-2-0.0.9/scoary/scoary_1_picking.py
+-rw-r--r--   0        0        0     1344 2022-06-30 06:21:54.086177 scoary-2-0.0.9/scoary/templates/config.json
+-rwxr-xr-x   0        0        0     3287 2022-07-06 17:32:33.601776 scoary-2-0.0.9/scoary/templates/favicon.svg
+-rw-r--r--   0        0        0      966 2022-05-03 12:46:21.149074 scoary-2-0.0.9/scoary/templates/overview.css
+-rw-r--r--   0        0        0     1896 2022-07-06 18:37:33.935231 scoary-2-0.0.9/scoary/templates/overview.html
+-rw-r--r--   0        0        0     7142 2022-05-19 12:49:30.033855 scoary-2-0.0.9/scoary/templates/overview.js
+-rw-r--r--   0        0        0     1741 2022-06-30 06:21:54.058177 scoary-2-0.0.9/scoary/templates/trait.css
+-rw-r--r--   0        0        0     3836 2022-07-06 18:37:33.927231 scoary-2-0.0.9/scoary/templates/trait.html
+-rw-r--r--   0        0        0    32887 2022-05-19 15:05:56.281180 scoary-2-0.0.9/scoary/templates/trait.js
+-rw-r--r--   0        0        0     3003 2022-04-04 09:39:33.342139 scoary-2-0.0.9/scoary/upgma.py
+-rw-r--r--   0        0        0     9369 2022-07-05 09:26:28.670578 scoary-2-0.0.9/scoary/utils.py
+-rw-r--r--   0        0        0      949 2022-09-30 09:36:37.429132 scoary-2-0.0.9/setup.py
+-rw-r--r--   0        0        0      678 2022-09-30 09:36:37.429308 scoary-2-0.0.9/PKG-INFO
```

### Comparing `scoary-2-0.0.7/pyproject.toml` & `scoary-2-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scoary-2"
-version = "0.0.7"
+version = "0.0.9"
 description = "Scoary 2: Associate genes with traits!"
 authors = ["MrTomRod <roder.thomas@gmail.com>"]
 license = "GPL3"
 packages = [
     { include = "scoary" }
 ]
 include = [
```

### Comparing `scoary-2-0.0.7/scoary/KeyValueStore.py` & `scoary-2-0.0.9/scoary/KeyValueStore.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/ScoaryTree.py` & `scoary-2-0.0.9/scoary/ScoaryTree.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/analyze_trait.py` & `scoary-2-0.0.9/scoary/analyze_trait.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/final_overview.py` & `scoary-2-0.0.9/scoary/final_overview.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import logging
 from shutil import copy
 import numpy as np
 import pandas as pd
 from scipy.cluster import hierarchy
 from scipy.spatial.distance import cdist, squareform
+import matplotlib as mpl
+
+mpl.use('SVG')
+# The SVG backend avoids this error message:
+# ValueError: Image size of 700x165660 pixels is too large. It must be less than 2^16 in each direction.
+# This allows for dendrograms with at least 20'000 traits
 
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.collections import PatchCollection, QuadMesh
 from matplotlib.patches import Rectangle
 
@@ -102,49 +108,48 @@
 
     logger.info('Adding isolate info...')
     if isolate_info_df is not None:
         isolate_info_df.to_csv(f'{ns.outdir}/isolate_info.tsv', sep='\t')
 
     logger.info('Copying files...')
     # copy files
-    files = ['overview.html', 'trait.html', 'overview.css', 'trait.css', 'overview.js', 'trait.js']
-    copy(src=f'{ROOT_DIR}/templates/overview.html', dst=f'{ns.outdir}/overview.html')
-    copy(src=f'{ROOT_DIR}/templates/trait.html', dst=f'{ns.outdir}/trait.html')
-    for file in ['config.json', 'trait.js', 'trait.css', 'overview.js', 'overview.css', 'favicon.ico']:
+    for file in ['overview.html', 'trait.html']:
+        copy(src=f'{ROOT_DIR}/templates/{file}', dst=f'{ns.outdir}/{file}')
+    for file in ['config.json', 'trait.js', 'trait.css', 'overview.js', 'overview.css', 'favicon.svg']:
         copy(src=f'{ROOT_DIR}/templates/{file}', dst=f'{ns.outdir}/app/{file}')
 
     summary_df_index = list(summary_df.index)
     if len(summary_df) > 1:
         logger.info('Calculating dendrogram linkage matrix...')
         # prepare data, create linkage_matrix
         pre_jaccard = ns.traits_df[summary_df.index].astype('float').T
         pre_jaccard = ((pre_jaccard.fillna(0.5) * 2) - 1).astype('int')  # False -> -1, NAN -> 0, True -> 1
 
-        # whether class=0 and class=1 are arbitrary. Calculate both possibilities, take minimum
+        # whether class=0 or class=1 is arbitrary. Calculate both possibilities, take minimum
         d1 = cdist(pre_jaccard, pre_jaccard, metric='jaccard')
         d2 = cdist(pre_jaccard, 0 - pre_jaccard, metric='jaccard')
-        jaccard_distance = np.minimum(d1, d2)
+        jaccard_distance = np.minimum(d1, d2) * 2  # multiply by 2 to make maximal distance 1 again
 
-        jaccard_df = pd.DataFrame(
-            jaccard_distance, columns=pre_jaccard.index, index=pre_jaccard.index
+        jaccard_df = pd.DataFrame(jaccard_distance, columns=pre_jaccard.index, index=pre_jaccard.index)
+        del d1, d2, jaccard_distance
+        linkage_matrix = hierarchy.linkage(
+            squareform(jaccard_df, checks=True),
+            method='average',
+            optimal_ordering=True
         )
-        linkage_matrix = hierarchy.linkage(squareform(jaccard_df), 'single')
 
         # calculate plot proportions
         content_height = max(3., len(jaccard_df) / 6)  # height dependent on number of compounds
         whitespace_abs = 0.6  # absolute amount of whitespace
         total_height = content_height + whitespace_abs  # total plot height
         whitespace_rel = whitespace_abs / 3 / total_height  # relative amount of whitespace
 
         # create matplotlib figure
         plt.close()
-        fig = plt.figure(figsize=(8, total_height), dpi=4)
-        # dpi=4 avoids this error message:
-        # ValueError: Image size of 700x165660 pixels is too large. It must be less than 2^16 in each direction.
-        # This allows for dendrograms with at least 20'000 traits
+        fig = plt.figure(figsize=(8, total_height))  # , dpi=4)
         gs = fig.add_gridspec(
             nrows=1, ncols=2, width_ratios=(2, 1),
             left=0.05, right=0.6, bottom=whitespace_rel * 2, top=1 - whitespace_rel,
             wspace=0, hspace=0
         )
 
         # get axes objects with shared y-axis
@@ -152,15 +157,15 @@
         ax_colorbar = fig.add_subplot(gs[0, 1], sharey=ax_dendrogram)
 
         logger.info('Plotting dendrogram...')
         # plot dendrogram
         dendrogram_params = plot_dendrogram(linkage_matrix, labels=jaccard_df.columns.values, ax=ax_dendrogram)
 
         # reindex summary_df according to order in dendrogram
-        summary_df_index = dendrogram_params['ivl'][::-1]
+        summary_df_index = dendrogram_params['ivl']
         summary_df = summary_df.reindex(summary_df_index)
 
         column_defs = {
             'best_fisher_q': {'marker': '$f$', 'color': 'tab:green'},
             'best_empirical_p': {'marker': '$e$', 'color': 'tab:purple'},
             'best_fq*ep': {'marker': '*', 'color': 'tab:red'}
         }
```

### Comparing `scoary-2-0.0.7/scoary/load_genes.py` & `scoary-2-0.0.9/scoary/load_genes.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,15 @@
     Load Roary-style gene count file with columns=strains and rows=genes
 
     :param path: Path to file
     :param delimiter: delimiter
     :param start_col: how many columns to skip
     :return: genes_df (DataFrame, dtype: bool); columns: strains; index: genes
     """
-    dtypes = defaultdict(lambda: int)
-    dtypes["index_column"] = str
-    count_df = pd.read_csv(path, delimiter=delimiter, index_col=0, dtype=dtypes)
+    count_df = pd.read_csv(path, delimiter=delimiter, index_col=0)
 
     # remove columns that are not in traits_df
     if restrict_to is not None or ignore is not None:
         count_df = filter_df(count_df, restrict_to, ignore)
 
     # sanity checks
     assert count_df.columns.is_unique, f'{path=}: columns not unique'
```

### Comparing `scoary-2-0.0.7/scoary/load_traits.py` & `scoary-2-0.0.9/scoary/load_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import queue
-from collections import defaultdict
 from datetime import datetime
 from typing import Callable
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import KMeans
 from pandas._libs.parsers import STR_NA_VALUES
@@ -42,17 +41,15 @@
     else:
         return ~classes
 
 
 def load_binary(traits: str, delimiter: str, restrict_to: str = None, ignore: str = None,
                 limit_traits: (int, int) = None):
     logger.debug(f'Loading binary traits: {traits=} {delimiter=}')
-    dtypes = defaultdict(lambda: int)
-    dtypes["index_column"] = str
-    traits_df = pd.read_csv(traits, delimiter=delimiter, index_col=0, dtype=dtypes, na_values=STR_NA_VALUES)
+    traits_df = pd.read_csv(traits, delimiter=delimiter, index_col=0, na_values=STR_NA_VALUES)
 
     if limit_traits is not None:
         assert len(limit_traits) == 2, f'{limit_traits=} is poorly formatted: must be (int, int).'
         l1, l2 = limit_traits
         assert type(l1) is type(l2) is int, f'{limit_traits=} is poorly formatted: must be (int, int).'
         traits_df = traits_df[traits_df.columns[l1:l2]]
 
@@ -76,17 +73,15 @@
 
     return traits_df
 
 
 def load_numeric(traits: str, delimiter: str, restrict_to: str = None, ignore: str = None,
                  limit_traits: (int, int) = None):
     logger.debug(f'Loading numeric traits: {traits=} {delimiter=}')
-    dtypes = defaultdict(lambda: float)
-    dtypes["index_column"] = str
-    numeric_df = pd.read_csv(traits, delimiter=delimiter, index_col=0, dtype=dtypes, na_values=STR_NA_VALUES)
+    numeric_df = pd.read_csv(traits, delimiter=delimiter, index_col=0, na_values=STR_NA_VALUES)
 
     if limit_traits is not None:
         assert len(limit_traits) == 2, f'{limit_traits=} is poorly formatted: must be (int, int).'
         l1, l2 = limit_traits
         assert type(l1) is type(l2) is int, f'{limit_traits=} is poorly formatted: must be (int, int).'
         numeric_df = numeric_df[numeric_df.columns[l1:l2]]
```

### Comparing `scoary-2-0.0.7/scoary/newick.py` & `scoary-2-0.0.9/scoary/newick.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/permutations.py` & `scoary-2-0.0.9/scoary/permutations.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/picking.py` & `scoary-2-0.0.9/scoary/picking.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/progressbar.py` & `scoary-2-0.0.9/scoary/progressbar.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/scoary.py` & `scoary-2-0.0.9/scoary/scoary.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     :param multiple_testing: "method:cutoff" for filtering genes after Fisher's test, where cutoff is a number that
     specifies the FWER and method is one of [bonferroni, sidak, holm-sidak, holm, simes-hochberg, hommel, fdr_bh,
     fdr_by,  fdr_tsbh, fdr_tsbky]. Alternatively, the method can be 'native': then, the cutoff targets the uncorrected
     pvalue from Fisher's test.
     :param worst_cutoff: Drop traits if no gene with "worst" pvalue lower than threshold. Recommended if
     dataset contains multiple species
     :param max_genes: Keep only n highest-scoring genes in Fisher's test. Recommended if dataset is big and contains
-     multiple species
+     multiple species; avoids waisting computational resources on traits that simply correlate with phylogeny
     :param gene_info: Path to file that describes genes: columns=arbitrary properties, rows=genes
     :param trait_info: Path to file that describes traits: columns=arbitrary properties, rows=traits
     :param isolate_info: Path to file that describes isolates: columns=arbitrary properties, rows=isolates
     :param newicktree: Path to a custom tree in Newick format
     :param pairwise: If False, only perform Fisher's test. If True, also perform pairwise comparisons
      algorithm.
     :param n_permut: Post-hoc label-switching test: perform N permutations of the phenotype by random label switching.
```

### Comparing `scoary-2-0.0.7/scoary/scoary_1_picking.py` & `scoary-2-0.0.9/scoary/scoary_1_picking.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/templates/config.json` & `scoary-2-0.0.9/scoary/templates/config.json`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/templates/overview.css` & `scoary-2-0.0.9/scoary/templates/overview.css`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/templates/overview.html` & `scoary-2-0.0.9/scoary/templates/overview.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <title>Traits overview (Scoary 2)</title>
-    <link rel="icon" type="image/x-icon" href="app/favicon.ico">
+    <link rel="icon" type="image/x-icon" href="app/favicon.svg">
 
     <script src="https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.3.2/papaparse.min.js"
             crossorigin="anonymous"></script>
 
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
           integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
```

### Comparing `scoary-2-0.0.7/scoary/templates/overview.js` & `scoary-2-0.0.9/scoary/templates/overview.js`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/templates/trait.css` & `scoary-2-0.0.9/scoary/templates/trait.css`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/templates/trait.html` & `scoary-2-0.0.9/scoary/templates/trait.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <title>Scoary2 Trait</title>
-    <link rel="icon" type="image/x-icon" href="app/favicon.ico">
+    <link rel="icon" type="image/x-icon" href="app/favicon.svg">
 
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css"
           rel="stylesheet" crossorigin="anonymous">
     <link href="//cdn.datatables.net/1.11.5/css/jquery.dataTables.min.css"
           rel="stylesheet" crossorigin="anonymous">
     <script src="https://code.jquery.com/jquery-3.6.0.slim.min.js"
             crossorigin="anonymous"></script>
```

### Comparing `scoary-2-0.0.7/scoary/templates/trait.js` & `scoary-2-0.0.9/scoary/templates/trait.js`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/upgma.py` & `scoary-2-0.0.9/scoary/upgma.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/scoary/utils.py` & `scoary-2-0.0.9/scoary/utils.py`

 * *Files identical despite different names*

### Comparing `scoary-2-0.0.7/setup.py` & `scoary-2-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'statsmodels>=0.13.2,<0.14.0']
 
 entry_points = \
 {'console_scripts': ['scoary = scoary.scoary:main']}
 
 setup_kwargs = {
     'name': 'scoary-2',
-    'version': '0.0.7',
+    'version': '0.0.9',
     'description': 'Scoary 2: Associate genes with traits!',
     'long_description': None,
     'author': 'MrTomRod',
     'author_email': 'roder.thomas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `scoary-2-0.0.7/PKG-INFO` & `scoary-2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoary-2
-Version: 0.0.7
+Version: 0.0.9
 Summary: Scoary 2: Associate genes with traits!
 License: GPL3
 Author: MrTomRod
 Author-email: roder.thomas@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

