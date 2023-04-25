# Comparing `tmp/pyrecdp-1.0.1b202304142.tar.gz` & `tmp/pyrecdp-1.0.1b20230425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.0.1b202304142.tar", last modified: Fri Apr 14 22:49:35 2023, max compression
+gzip compressed data, was "dist/pyrecdp-1.0.1b20230425.tar", last modified: Tue Apr 25 07:56:59 2023, max compression
```

## Comparing `pyrecdp-1.0.1b202304142.tar` & `pyrecdp-1.0.1b20230425.tar`

### file list

```diff
@@ -1,113 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8860 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1001 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     2813 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    12498 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/DataEstimator.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     5253 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/engines/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2878 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1881 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4055 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/statics.py
--rw-r--r--   0 root         (0) root         (0)     7142 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5712 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54029 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7111 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-14 21:12:55.000000 pyrecdp-1.0.1b202304142/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 22:49:35.945148 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8860 2023-04-14 22:49:35.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3368 2023-04-14 22:49:35.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 22:49:35.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-14 22:49:35.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-14 22:49:35.000000 pyrecdp-1.0.1b202304142/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 22:49:35.949148 pyrecdp-1.0.1b202304142/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1394 2023-04-14 22:49:31.000000 pyrecdp-1.0.1b202304142/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.604280 pyrecdp-1.0.1b20230425/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-04-25 02:53:10.000000 pyrecdp-1.0.1b20230425/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-04-25 07:56:59.603279 pyrecdp-1.0.1b20230425/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.584280 pyrecdp-1.0.1b20230425/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-25 02:53:10.000000 pyrecdp-1.0.1b20230425/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.584280 pyrecdp-1.0.1b20230425/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.585280 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-25 04:39:12.000000 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.586279 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-25 04:39:12.000000 pyrecdp-1.0.1b20230425/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.587279 pyrecdp-1.0.1b20230425/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     2813 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    12498 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/DataEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.588280 pyrecdp-1.0.1b20230425/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.590279 pyrecdp-1.0.1b20230425/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.590279 pyrecdp-1.0.1b20230425/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.591280 pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.594280 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     4055 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/statics.py
+-rw-r--r--   0 root         (0) root         (0)     7142 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.598280 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5712 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.600279 pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54029 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.601280 pyrecdp-1.0.1b20230425/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.602280 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.585280 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-25 07:56:59.000000 pyrecdp-1.0.1b20230425/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 07:56:59.604280 pyrecdp-1.0.1b20230425/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-25 07:56:29.000000 pyrecdp-1.0.1b20230425/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:56:59.603279 pyrecdp-1.0.1b20230425/tests/
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/tests/test_data_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-04-25 03:08:58.000000 pyrecdp-1.0.1b20230425/tests/test_spark_dataprocessor.py
```

### Comparing `pyrecdp-1.0.1b202304142/LICENSE` & `pyrecdp-1.0.1b20230425/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/PKG-INFO` & `pyrecdp-1.0.1b20230425/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202304142
+Version: 1.0.1b20230425
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
-License: UNKNOWN
+Author-email: chendi.xue@intel.com
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -214,9 +213,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202304142/README.md` & `pyrecdp-1.0.1b20230425/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b20230425/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/__init__.py` & `pyrecdp-1.0.1b20230425/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/BasePipeline.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/DataEstimator.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/DataEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b20230425/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/core/dataframe.py` & `pyrecdp-1.0.1b20230425/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b20230425/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b20230425/pyrecdp/core/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from woodwork.column_schema import ColumnSchema
 from pandas import StringDtype
-from pyrecdp.core.utils import is_text_series, is_tuple, is_encoded
+from pyrecdp.core.utils import is_text_series, is_tuple, is_encoded, is_integer_convertable
 class TextDtype(StringDtype):
     pass
 
 class SeriesSchema:
     def __init__(self, *args):
         if len(args) == 1:
             s = args[0]
             self.name = s.name
             in_type = s.dtype
             self.config = {}
             self.config['is_text'] = is_text_series(s)
             if self.config['is_text']:
                 self.config['is_encoded'] = is_encoded(s)
             self.config['is_tuple'] = is_tuple(s)
+            self.config['is_integer'] = is_integer_convertable(s)
         elif len(args) >= 2:
             # s_dtype is possible to be pandas.dtype or woodwork.dtype       
             self.name = args[0]
             # TODO: convert featuretools return_type to recdp return type
             in_type = args[1]
             if len(args) > 2:
                 self.config = args[2]
             else:
                 self.config = {}
+            self.config['is_integer'] = False
         else:
             raise ValueError(f"SeriesSchema unsupport input as {args}")
 
         if in_type:
             # check all types
             from pandas.api.types import is_bool_dtype
             from pandas.api.types import is_string_dtype
@@ -36,16 +38,16 @@
             from pandas.api.types import is_integer_dtype
             from pandas.api.types import is_datetime64_any_dtype
             from pandas.api.types import is_categorical_dtype
             from pandas.api.types import is_object_dtype, is_list_like
             self.config['is_boolean'] = is_bool_dtype(in_type)
             self.config['is_string'] = is_string_dtype(in_type)
             self.config['is_numeric'] = is_numeric_dtype(in_type)
-            self.config['is_float'] = is_float_dtype(in_type)
-            self.config['is_integer'] = is_integer_dtype(in_type)
+            self.config['is_integer'] = is_integer_dtype(in_type) or self.config['is_integer']
+            self.config['is_float'] = is_float_dtype(in_type) if not self.config['is_integer'] else False
             self.config['is_datetime'] = is_datetime64_any_dtype(in_type)
             self.config['is_categorical'] = is_categorical_dtype(in_type)
             self.config['is_list'] = is_object_dtype(in_type) and is_list_like(in_type)
 
             if isinstance(in_type, ColumnSchema):
                 self.config['is_categorical'] = in_type.is_categorical
                 self.config['is_numeric'] = in_type.is_numeric or 'numeric' in str(in_type)
```

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b20230425/pyrecdp/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,24 @@
         return False
     
     return try_text(s)
 
 def is_tuple(s):
     t = type(s.loc[s.first_valid_index()]) if s.first_valid_index() >= 0 else None
     return isinstance(t, tuple)
-           
+       
+def is_integer_convertable(s):
+    from pandas.api.types import is_numeric_dtype
+    if not is_numeric_dtype(s.dtype):
+        return False
+    s = s.fillna(0)
+    if np.array_equal(s, s.astype(int)):
+        return True
+    return False
+        
 def is_encoded(s):
     line_id = s.first_valid_index()
     if line_id < 0:
         return False
     sample_data = s.loc[line_id:(line_id+1000)]
     from pyrecdp.primitives.generators.nlp import BertTokenizerDecode
     proc_ = BertTokenizerDecode().get_function()
```

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b20230425/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/datetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             Year,
             Hour,
             #PartOfDay()
         ]
         self.op_name = 'datetime_feature'            
 
     def fit_prepare(self, pipeline, children, max_idx):
+        cur_idx = max_idx
         pa_schema = pipeline[children[0]].output
         for pa_field in pa_schema:
             if pa_field.is_datetime:
                 self.feature_in.append(pa_field.name)
         feature_in_out_map = {}     
         for in_feat_name in self.feature_in:
             feature_in_out_map[in_feat_name] = []
```

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/statics.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b20230425/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b20230425/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b20230425/pyrecdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202304142
+Version: 1.0.1b20230425
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
-License: UNKNOWN
+Author-email: chendi.xue@intel.com
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -214,9 +213,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202304142/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b20230425/pyrecdp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 pyrecdp/datasets/download.py
 pyrecdp/datasets/ibm_fraud_detect.py
 pyrecdp/datasets/nyc_taxi.py
 pyrecdp/datasets/outbrain.py
 pyrecdp/datasets/pretrained.py
 pyrecdp/datasets/twitter_recsys.py
 pyrecdp/primitives/__init__.py
-pyrecdp/primitives/engines/__init__.py
-pyrecdp/primitives/engines/runner.py
 pyrecdp/primitives/estimators/__init__.py
 pyrecdp/primitives/estimators/base.py
 pyrecdp/primitives/estimators/lightgbm.py
 pyrecdp/primitives/generators/__init__.py
 pyrecdp/primitives/generators/base.py
 pyrecdp/primitives/generators/binned.py
 pyrecdp/primitives/generators/category.py
@@ -87,8 +85,13 @@
 pyrecdp/widgets/utils.py
 pyrecdp/widgets/templates/base.html
 pyrecdp/widgets/templates/error.html
 pyrecdp/widgets/templates/interactions.html
 pyrecdp/widgets/templates/overview.html
 pyrecdp/widgets/templates/scripts.html
 pyrecdp/widgets/templates/styles.html
-pyrecdp/widgets/templates/variables.html
+pyrecdp/widgets/templates/variables.html
+tests/test_data_estimator.py
+tests/test_feature_wrangler.py
+tests/test_pipeline_json.py
+tests/test_relational_builder.py
+tests/test_spark_dataprocessor.py
```

### Comparing `pyrecdp-1.0.1b202304142/setup.py` & `pyrecdp-1.0.1b20230425/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="pyrecdp",
-    version="1.0.1b202304142",
+    version="1.0.1b20230425",
     author="INTEL AIA",
+    author_email="chendi.xue@intel.com",
     description=
     "A data processing bundle for spark based recommender system operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/intel/e2eAIOK/",
     project_urls={
         "Bug Tracker": "https://github.com/intel/e2eAIOK/",
@@ -40,12 +41,16 @@
         "pandas_flavor",
         "featuretools",
         "bokeh>=2.4.2",
         "transformers",
         "ipywidgets",
         "plotly",
         "shapely",
+        "graphviz",
         "requests",
         "distro",
         "pyspark==3.3.1",
         "lightgbm",
+        "jupyter",
+        "docx2txt",
+        "openpyxl"
         ])
```

