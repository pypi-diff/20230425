# Comparing `tmp/SciQLop-0.1.1.tar.gz` & `tmp/SciQLop-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciQLop-0.1.1.tar", last modified: Wed Mar 15 12:00:57 2023, max compression
+gzip compressed data, was "SciQLop-0.2.1.tar", last modified: Tue Apr 25 07:43:55 2023, max compression
```

## Comparing `SciQLop-0.1.1.tar` & `SciQLop-0.2.1.tar`

### file list

```diff
@@ -1,84 +1,90 @@
--rw-r--r--   0        0        0    35147 2023-03-15 12:00:38.523446 SciQLop-0.1.1/COPYING
--rw-r--r--   0        0        0     1859 2023-03-15 12:00:38.523446 SciQLop-0.1.1/README.md
--rw-r--r--   0        0        0       23 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/__init__.py
--rw-r--r--   0        0        0      987 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/app.py
--rw-r--r--   0        0        0     1156 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/__init__.py
--rw-r--r--   0        0        0      532 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/enums.py
--rw-r--r--   0        0        0      172 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/models.py
--rw-r--r--   0        0        0       44 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/__init__.py
--rw-r--r--   0        0        0      100 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/base/__init__.py
--rw-r--r--   0        0        0     2094 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/base/pipeline_model_item.py
--rw-r--r--   0        0        0     4950 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/base/pipelines.py
--rw-r--r--   0        0        0     3876 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/data_pipeline.py
--rw-r--r--   0        0        0      718 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/data_provider.py
--rw-r--r--   0        0        0     1605 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/graph.py
--rw-r--r--   0        0        0      212 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/plot.py
--rw-r--r--   0        0        0      278 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/pipelines_model/time_sync_panel.py
--rw-r--r--   0        0        0        0 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/products_model/__init__.py
--rw-r--r--   0        0        0     6575 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/products_model/model.py
--rw-r--r--   0        0        0     2983 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/products_model/product_node.py
--rw-r--r--   0        0        0        0 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/resampling/__init__.py
--rw-r--r--   0        0        0     1069 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/resampling/spectro_regrid.py
--rw-r--r--   0        0        0      186 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/backend/unique_names.py
--rw-r--r--   0        0        0     1645 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/mime/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/mime/types.py
--rw-r--r--   0        0        0     1993 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/plugins/__init__.py
--rw-r--r--   0        0        0     3561 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/plugins/catalogs.py
--rw-r--r--   0        0        0     3906 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/plugins/speasy.py
--rw-r--r--   0        0        0     1487 2023-03-15 12:00:38.523446 SciQLop-0.1.1/SciQLop/plugins/test_plugin.py
--rw-r--r--   0        0        0   552261 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/__init__.py
--rw-r--r--   0        0        0   118794 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/SciQLop.png
--rw-r--r--   0        0        0     3191 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/Simple_icon_time.svg
--rw-r--r--   0        0        0     1956 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/add.png
--rw-r--r--   0        0        0     2001 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/allEvents.png
--rw-r--r--   0        0        0      615 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/catalogue.png
--rw-r--r--   0        0        0     1003 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/chart.png
--rw-r--r--   0        0        0     1047 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/cursor.png
--rw-r--r--   0        0        0     2150 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/dataSourceComponent.png
--rw-r--r--   0        0        0      882 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/dataSourceNode.png
--rw-r--r--   0        0        0     1213 2023-03-15 12:00:38.527446 SciQLop-0.1.1/SciQLop/resources/icons/dataSourceProduct.png
--rw-r--r--   0        0        0     4821 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/dataSourceRoot.png
--rw-r--r--   0        0        0      788 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/database.png
--rw-r--r--   0        0        0      834 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/delete.png
--rwxr-xr-x   0        0        0     1266 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/discard.png
--rw-r--r--   0        0        0     1231 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/down.png
--rw-r--r--   0        0        0     1731 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/drag.png
--rw-r--r--   0        0        0     4413 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/next.png
--rwxr-xr-x   0        0        0     1450 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/openInspector.png
--rw-r--r--   0        0        0     2319 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/plot.png
--rw-r--r--   0        0        0     2114 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/pointer.png
--rw-r--r--   0        0        0     4377 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/previous.png
--rw-r--r--   0        0        0     4841 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/rectangle.png
--rw-r--r--   0        0        0     1916 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/remove.png
--rw-r--r--   0        0        0    10041 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/satellite.svg
--rw-r--r--   0        0        0     1334 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/save.png
--rw-r--r--   0        0        0    85300 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/sciqlop2PNG_1024.png
--rw-r--r--   0        0        0     3714 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/time.png
--rw-r--r--   0        0        0     1084 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/trash.png
--rw-r--r--   0        0        0     2234 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/unplot.png
--rw-r--r--   0        0        0     1197 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/up.png
--rw-r--r--   0        0        0     4056 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/icons/zoom.png
--rw-r--r--   0        0        0     1249 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/resources/resources.qrc
--rw-r--r--   0        0        0        0 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/__init__.py
--rw-r--r--   0        0        0     2737 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/central_widget.py
--rw-r--r--   0        0        0       31 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/common/__init__.py
--rw-r--r--   0        0        0      813 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/common/tree_view.py
--rw-r--r--   0        0        0     3007 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/console.py
--rw-r--r--   0        0        0     3102 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/datetime_range.py
--rw-r--r--   0        0        0      157 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/__init__.py
--rw-r--r--   0        0        0      282 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/drop_handler.py
--rw-r--r--   0        0        0     2450 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/helper.py
--rw-r--r--   0        0        0     3120 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py
--rw-r--r--   0        0        0     1134 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/placeholder.py
--rw-r--r--   0        0        0     3270 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/mainwindow.py
--rw-r--r--   0        0        0       39 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/pipelines/__init__.py
--rw-r--r--   0        0        0     2085 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/pipelines/pipeline_tree.py
--rw-r--r--   0        0        0        0 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/plots/__init__.py
--rw-r--r--   0        0        0     2018 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/plots/colormap_graph.py
--rw-r--r--   0        0        0     2130 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/plots/line_graph.py
--rw-r--r--   0        0        0     8108 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/plots/plot.py
--rw-r--r--   0        0        0     5772 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/plots/time_sync_panel.py
--rw-r--r--   0        0        0       39 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/products_tree/__init__.py
--rw-r--r--   0        0        0     1303 2023-03-15 12:00:38.531446 SciQLop-0.1.1/SciQLop/widgets/products_tree/products_tree.py
--rw-r--r--   0        0        0     1337 2023-03-15 12:00:38.535447 SciQLop-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 SciQLop-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-04-25 07:43:34.629640 SciQLop-0.2.1/COPYING
+-rw-r--r--   0        0        0     1859 2023-04-25 07:43:34.629640 SciQLop-0.2.1/README.md
+-rw-r--r--   0        0        0       23 2023-04-25 07:43:34.629640 SciQLop-0.2.1/SciQLop/__init__.py
+-rw-r--r--   0        0        0     1276 2023-04-25 07:43:34.629640 SciQLop-0.2.1/SciQLop/app.py
+-rw-r--r--   0        0        0     1433 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/__init__.py
+-rw-r--r--   0        0        0      532 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/enums.py
+-rw-r--r--   0        0        0      831 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/logging/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/models.py
+-rw-r--r--   0        0        0        1 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/__init__.py
+-rw-r--r--   0        0        0     5202 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/auto_register.py
+-rw-r--r--   0        0        0      128 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/__init__.py
+-rw-r--r--   0        0        0     6856 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/model.py
+-rw-r--r--   0        0        0     2925 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/pipeline_node.py
+-rw-r--r--   0        0        0     5349 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_pipeline.py
+-rw-r--r--   0        0        0      718 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_provider.py
+-rw-r--r--   0        0        0     3820 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/graph.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/__init__.py
+-rw-r--r--   0        0        0     6549 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/model.py
+-rw-r--r--   0        0        0     3195 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/product_node.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/resampling/__init__.py
+-rw-r--r--   0        0        0     1069 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/resampling/spectro_regrid.py
+-rw-r--r--   0        0        0      186 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/unique_names.py
+-rw-r--r--   0        0        0     1645 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/mime/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/mime/types.py
+-rw-r--r--   0        0        0     2279 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/__init__.py
+-rw-r--r--   0        0        0      181 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/catalogs.py
+-rw-r--r--   0        0        0     4035 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py
+-rw-r--r--   0        0        0     2379 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py
+-rw-r--r--   0        0        0     1706 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py
+-rw-r--r--   0        0        0     3906 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/speasy.py
+-rw-r--r--   0        0        0     1419 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/test_plugin.py
+-rw-r--r--   0        0        0   552261 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/__init__.py
+-rw-r--r--   0        0        0   118794 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/SciQLop.png
+-rw-r--r--   0        0        0     3191 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/Simple_icon_time.svg
+-rw-r--r--   0        0        0     1956 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/add.png
+-rw-r--r--   0        0        0     2001 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/allEvents.png
+-rw-r--r--   0        0        0      615 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/catalogue.png
+-rw-r--r--   0        0        0     1003 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/chart.png
+-rw-r--r--   0        0        0     1047 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/cursor.png
+-rw-r--r--   0        0        0     2150 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceComponent.png
+-rw-r--r--   0        0        0      882 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceNode.png
+-rw-r--r--   0        0        0     1213 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceProduct.png
+-rw-r--r--   0        0        0     4821 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceRoot.png
+-rw-r--r--   0        0        0      788 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/database.png
+-rw-r--r--   0        0        0      834 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/delete.png
+-rwxr-xr-x   0        0        0     1266 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/discard.png
+-rw-r--r--   0        0        0     1231 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/down.png
+-rw-r--r--   0        0        0     1731 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/drag.png
+-rw-r--r--   0        0        0     4413 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/next.png
+-rwxr-xr-x   0        0        0     1450 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/openInspector.png
+-rw-r--r--   0        0        0     2319 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/plot.png
+-rw-r--r--   0        0        0     2114 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/pointer.png
+-rw-r--r--   0        0        0     4377 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/previous.png
+-rw-r--r--   0        0        0     4841 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/rectangle.png
+-rw-r--r--   0        0        0     1916 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/remove.png
+-rw-r--r--   0        0        0    10041 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/satellite.svg
+-rw-r--r--   0        0        0     1334 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/save.png
+-rw-r--r--   0        0        0    85300 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/sciqlop2PNG_1024.png
+-rw-r--r--   0        0        0     3714 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/time.png
+-rw-r--r--   0        0        0     1084 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/trash.png
+-rw-r--r--   0        0        0     2234 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/unplot.png
+-rw-r--r--   0        0        0     1197 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/up.png
+-rw-r--r--   0        0        0     4056 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/zoom.png
+-rw-r--r--   0        0        0     1249 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/resources.qrc
+-rw-r--r--   0        0        0        0 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/__init__.py
+-rw-r--r--   0        0        0     3758 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/central_widget.py
+-rw-r--r--   0        0        0       31 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/common/__init__.py
+-rw-r--r--   0        0        0     1005 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/common/tree_view.py
+-rw-r--r--   0        0        0     2499 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/console.py
+-rw-r--r--   0        0        0     3102 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/datetime_range.py
+-rw-r--r--   0        0        0      157 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/__init__.py
+-rw-r--r--   0        0        0      282 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/drop_handler.py
+-rw-r--r--   0        0        0     2450 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/helper.py
+-rw-r--r--   0        0        0     3120 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py
+-rw-r--r--   0        0        0     1134 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/placeholder.py
+-rw-r--r--   0        0        0     4651 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/mainwindow.py
+-rw-r--r--   0        0        0       39 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/pipelines/__init__.py
+-rw-r--r--   0        0        0     2085 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/pipelines/pipeline_tree.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/colormap_graph.py
+-rw-r--r--   0        0        0     1719 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/line_graph.py
+-rw-r--r--   0        0        0    10327 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_series_plot.py
+-rw-r--r--   0        0        0     1556 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_span.py
+-rw-r--r--   0        0        0     1050 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_span_controller.py
+-rw-r--r--   0        0        0     7663 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_sync_panel.py
+-rw-r--r--   0        0        0       39 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/products_tree/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/products_tree/products_tree.py
+-rw-r--r--   0        0        0     1364 2023-04-25 07:43:34.645641 SciQLop-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 SciQLop-0.2.1/PKG-INFO
```

### Comparing `SciQLop-0.1.1/COPYING` & `SciQLop-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/README.md` & `SciQLop-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/backend/enums.py` & `SciQLop-0.2.1/SciQLop/backend/enums.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/backend/pipelines_model/data_provider.py` & `SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_provider.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/backend/products_model/model.py` & `SciQLop-0.2.1/SciQLop/backend/products_model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from PySide6.QtCore import QModelIndex, QMimeData, QAbstractItemModel, QStringListModel, QPersistentModelIndex, Qt
 from PySide6.QtGui import QIcon
 
 from SciQLop.mime import register_mime, encode_mime
 from SciQLop.mime.types import PRODUCT_LIST_MIME_TYPE
 from .product_node import ProductNode
-import re
 
 
 def for_all_nodes(f, node):
     f(node)
     for child in node.children:
         for_all_nodes(f, child)
 
@@ -57,15 +56,15 @@
     _filter: str = ""
 
     def __init__(self, parent=None):
         super(ProductsModel, self).__init__(parent)
         self._icons: Dict[str, QIcon] = {}
         self._mime_data = None
         self._completion_model = QStringListModel(self)
-        self._root = ProductNode(name="root", metadata={}, uid='root', provider="")
+        self._root = ProductNode(name="", metadata={}, uid='root', provider="")
         self.set_filter("")
 
     def set_filter(self, filter_regex: str):
         self._filter = filter_regex
         self.beginResetModel()
         self._filtered_root = _FilterNode(None, self._root, self._filter)
         self.endResetModel()
@@ -168,15 +167,15 @@
             return flags
         return Qt.NoItemFlags
 
 
 def _mime_encode_product_list(products: List[ProductNode]) -> QMimeData:
     mdata = QMimeData()
     mdata.setData(PRODUCT_LIST_MIME_TYPE, pickle.dumps(list(map(lambda p: p.copy(), products))))
-    mdata.setText(":".join(list(map(lambda p: f"{p.provider}/{p.uid}", products))))
+    mdata.setText(":".join(list(map(lambda p: f"{p.path}", products))))
     return mdata
 
 
 def _mime_decode_product_list(mime_data: QMimeData) -> List[ProductNode] or None:
     if PRODUCT_LIST_MIME_TYPE in mime_data.formats():
         return pickle.loads(mime_data.data(PRODUCT_LIST_MIME_TYPE))
     return None
```

### Comparing `SciQLop-0.1.1/SciQLop/backend/products_model/product_node.py` & `SciQLop-0.2.1/SciQLop/backend/products_model/product_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def set_parent(self, parent: 'ProductNode'):
         if self._parent is None:
             self._parent = parent
         else:
             raise ValueError("Can't set parent when one is already set")
 
     def __getitem__(self, item: str) -> "ProductNode" or None:
-        return next(iter(filter(lambda n: n._product.name == item, self._children)), None)
+        return next(iter(filter(lambda n: n.name == item, self._children)), None)
 
     @property
     def children(self) -> List['ProductNode']:
         return self._children
 
     @property
     def parent(self) -> 'ProductNode' or None:
@@ -95,7 +95,15 @@
     @property
     def uid(self):
         return self._uid
 
     @property
     def str(self):
         return self._str_content
+
+    @property
+    def path(self):
+        if self._parent:
+            parent_path = self._parent.path
+            if parent_path != "":
+                return self.parent.path + "/" + self.name
+        return self.name
```

### Comparing `SciQLop-0.1.1/SciQLop/backend/resampling/spectro_regrid.py` & `SciQLop-0.2.1/SciQLop/backend/resampling/spectro_regrid.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/mime/__init__.py` & `SciQLop-0.2.1/SciQLop/mime/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/plugins/__init__.py` & `SciQLop-0.2.1/SciQLop/plugins/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import importlib
 import os
 import traceback
-import importlib
+from types import SimpleNamespace
+
 from PySide6.QtCore import QRunnable, Slot, Signal, QThreadPool, QObject
 
 here = os.path.dirname(os.path.realpath(__file__))
 
 threadpool = QThreadPool()
 
+loaded_plugins = SimpleNamespace()
+
 
 class WorkerSignals(QObject):
-    result = Signal(object)
+    result = Signal(object, object)
 
 
 class Worker(QRunnable):
     '''
     Worker thread
 
     Inherits from QRunnable to handler worker thread setup, signals and wrap-up.
@@ -32,41 +36,44 @@
         self.args = args
         self.kwargs = kwargs
         self.signals = WorkerSignals()
 
     @Slot()
     def run(self):
         try:
-            self.signals.result.emit(self.fn(*self.args, **self.kwargs))
+            self.signals.result.emit(*self.fn(*self.args, **self.kwargs))
         except Exception as e:
             print(f"Oups can't load {name} , {e}")
             traceback.print_exc()
 
 
-def load_plugin(mod, main_window):
+def load_plugin(name, mod, main_window):
     if mod:
         try:
-            return mod.load(main_window)
+            r = mod.load(main_window)
+            loaded_plugins.__dict__[name] = r
+            return r
         except Exception as e:
             print(f"Oups can't load {mod} , {e}")
             traceback.print_exc()
 
 
 def load_module(name):
     try:
         mod = importlib.import_module(f"SciQLop.plugins.{name}", "*")
-        return mod
+        return name, mod
     except Exception as e:
         print(f"Oups can't load {name} , {e}")
         traceback.print_exc()
 
 
 def background_load(plugin, main_window):
     w = Worker(load_module, plugin)
-    w.signals.result.connect(lambda mod: load_plugin(mod, main_window))
+    w.signals.result.connect(lambda name, mod: load_plugin(name, mod, main_window))
     return threadpool.start(w)
 
 
 def load_all(main_window):
-    plugin_list = [f[:-3] for f in os.listdir(here) if f[-3:] == '.py' and f != '__init__.py']
+    plugin_list = [f[:-3] for f in os.listdir(here) if f[-3:] == '.py' and f != '__init__.py'] + \
+                  [f for f in os.listdir(here) if os.path.isdir(f"{here}/{f}") and not f.startswith('_')]
     print(plugin_list)
-    return [background_load(plugin, main_window) for plugin in plugin_list]
+    return {plugin: background_load(plugin, main_window) for plugin in plugin_list}
```

### Comparing `SciQLop-0.1.1/SciQLop/plugins/catalogs.py` & `SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,100 @@
-import tscat
-from tscat_gui import TSCatGUI
-from PySide6.QtWidgets import QComboBox
-from PySide6.QtGui import QAction, QIcon
-from PySide6.QtCore import QRunnable, Slot, Signal, QThreadPool, QObject
-from datetime import datetime
-from SciQLop.widgets.mainwindow import SciQLopMainWindow
-from SciQLop.widgets.plots.time_sync_panel import TimeSyncPanel, TimeRange
-
-
-def catalog_display_txt(catalog):
-    if catalog is not None:
-        return catalog.name
-    return "None"
-
-
-def index_of(catalogs, catalog):
-    index = 0
-    if catalog:
-        for c in catalogs:
-            if (c is not None) and (c.uuid == catalog.uuid):
-                return index
-            index += 1
-    return 0
-
+from typing import List, Optional
 
-def zoom_out(start: datetime, stop: datetime, factor: float):
-    delta = ((stop - start) / 2.) * factor
-    return start - delta, stop + delta
+from PySide6.QtCore import Slot, Signal, Qt
+from PySide6.QtWidgets import QWidget, QComboBox, QVBoxLayout, QSizePolicy, QCheckBox
 
+from SciQLop.backend import TimeRange
+from SciQLop.backend.logging import getLogger
+from SciQLop.widgets.mainwindow import SciQLopMainWindow
+from SciQLop.widgets.plots.time_span import TimeSpan
+from SciQLop.widgets.plots.time_span_controller import TimeSpanController
+from SciQLop.widgets.plots.time_sync_panel import TimeSyncPanel
+from .catalog_selector import CatalogItem, CatalogSelector
+from .event_selector import EventSelector
 
-def timestamps(start: datetime, stop: datetime):
-    return start.timestamp(), stop.timestamp()
-
-
-class CatalogSelector(QComboBox):
-    def __init__(self, parent=None):
-        super(CatalogSelector, self).__init__(parent)
-        self.catalogs = [None]
-        self.update_list()
-
-    def update_list(self):
-        selected = self.catalogs[self.currentIndex()]
-        self.catalogs = [None] + tscat.get_catalogues()
-        self.clear()
-        self.addItems(map(catalog_display_txt, self.catalogs))
-        self.setCurrentIndex(index_of(self.catalogs, selected))
+log = getLogger(__name__)
 
 
 class PanelSelector(QComboBox):
+    panel_selection_changed = Signal(str)
+
     def __init__(self, parent=None):
         super(PanelSelector, self).__init__(parent)
         self.addItems(["None"])
+        self.setSizeAdjustPolicy(QComboBox.SizeAdjustPolicy.AdjustToContents)
+        self.currentTextChanged.connect(self.panel_selection_changed)
 
     def update_list(self, panels):
         selected = self.currentText()
         self.clear()
         self.addItems(["None"] + panels)
         self.setCurrentText(selected)
 
 
-class CatalogGUISpawner(QAction):
-    def __init__(self, catalog_gui, parent=None):
-        super(CatalogGUISpawner, self).__init__(parent)
-        self.catalog_gui = catalog_gui
-        self.setIcon(QIcon("://icons/catalogue.png"))
-        self.triggered.connect(self.show_catalogue_gui)
-
-    def show_catalogue_gui(self):
-        self.catalog_gui.show()
-
-
-class Plugin(QObject):
-    def __init__(self, main_window: SciQLopMainWindow):
-        super(Plugin, self).__init__(main_window)
-        self.ui = TSCatGUI()
-        self.catalog_selector = CatalogSelector()
-        self.panel_selector = PanelSelector()
-        self.show_catalog = CatalogGUISpawner(self.ui)
+class LightweightManager(QWidget):
+    update_panels_list = Signal(list)
+    current_panel: Optional[TimeSyncPanel] = None
+    main_window: SciQLopMainWindow = None
+    spans: List[TimeSpan] = []
+
+    def __init__(self, main_window: SciQLopMainWindow, parent=None):
+        super().__init__(parent=parent)
+        self.setLayout(QVBoxLayout())
         self.main_window = main_window
-        self.last_event = None
+        self.catalog_selector = CatalogSelector(self)
+        self.follow_selected_event = QCheckBox("Jump on selected event", self)
+        self.allow_edition = QCheckBox("Allow edition", self)
+        self.panel_selector = PanelSelector(self)
+        self.event_selector = EventSelector(self)
+        self.layout().addWidget(self.panel_selector)
+        self.layout().addWidget(self.follow_selected_event)
+        self.layout().addWidget(self.allow_edition)
+        self.layout().addWidget(self.catalog_selector)
+        self.layout().addWidget(self.event_selector)
+
+        self.setWindowTitle("Catalogs")
+
+        self.catalog_selector.catalog_selected.connect(self.catalog_selected)
+        self.update_panels_list.connect(self.panel_selector.update_list)
+        self.panel_selector.panel_selection_changed.connect(self.panel_selected)
+        self.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+        self.event_selector.event_selected.connect(self.event_selected)
+        self.allow_edition.stateChanged.connect(self._allow_edition_state_change)
 
-        main_window.toolBar.addAction(self.show_catalog)
-        main_window.toolBar.addWidget(self.catalog_selector)
-        main_window.toolBar.addWidget(self.panel_selector)
+        self._time_span_ctrlr: Optional[TimeSpanController] = None
 
-        main_window.central_widget.panels_list_changed.connect(self.panel_selector.update_list)
-
-        self.ui.event_selected.connect(self.event_selected)
+    @Slot()
+    def catalog_selected(self, catalogs: List[CatalogItem]):
+        events = []
+        for c in catalogs:
+            events += c.events
+        self.event_selector.update_list(events)
+        self.update_spans()
 
     @Slot()
     def event_selected(self, event):
-        if self.panel_selector.currentText() != 'None':
-            if self.last_event is not None:
-                del self.last_event
-            e = tscat.get_events(tscat.filtering.UUID(event))[0]
-            print(e)
-            time_range = TimeRange(*timestamps(*zoom_out(e.start, e.stop, 0.3)))
-            print(time_range)
-            if e:
-                p: TimeSyncPanel = self.main_window.plot_panel(self.panel_selector.currentText())
-                print(p)
-                if p:
-                    p.time_range = time_range
-                    # self.last_event = EventTimeSpan(p, *timestamps(e.start, e.stop))
+        if self.follow_selected_event.isChecked() and self.current_panel is not None:
+            self.current_panel.time_range = TimeRange(event.start.timestamp(), event.stop.timestamp()) * 1.3
+
+    def update_spans(self):
+        if self.current_panel is not None:
+            self._time_span_ctrlr = TimeSpanController(parent=self, plot_panel=self.current_panel)
+            ro = not self.allow_edition.isChecked()
+            self.spans = [
+                TimeSpan(TimeRange(event.start.timestamp(), event.stop.timestamp()), plot_panel=self.current_panel,
+                         visible=False, read_only=ro) for
+                event
+                in self.event_selector.events]
+            self._time_span_ctrlr.set_ranges(self.spans)
 
+    @Slot()
+    def panel_selected(self, panel):
+        log.debug(f"New panel selected: {panel}")
+        self.current_panel = self.main_window.plot_panel(panel)
+        self.update_spans()
 
-def load(main_window: SciQLopMainWindow):
-    return Plugin(main_window)
+    @Slot()
+    def _allow_edition_state_change(self, state):
+        ro = state == Qt.Unchecked
+        for s in self.spans:
+            s.read_only = ro
```

### Comparing `SciQLop-0.1.1/SciQLop/plugins/speasy.py` & `SciQLop-0.2.1/SciQLop/plugins/speasy.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/plugins/test_plugin.py` & `SciQLop-0.2.1/SciQLop/plugins/test_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import humanize
 import numpy as np
 from speasy.products import SpeasyVariable, DataContainer, VariableTimeAxis
 
 from SciQLop.backend import Product
 from SciQLop.backend.enums import ParameterType
 from SciQLop.backend.models import products
 from SciQLop.backend.pipelines_model.data_provider import DataProvider, DataOrder
@@ -22,14 +21,13 @@
 
     def get_data(self, product, start, stop):
         x = np.arange(start.timestamp(), stop.timestamp(), 0.1) * 1.
         y = np.empty((len(x), 3))
         y[:, 0] = np.cos(x / 100.) * 10.
         y[:, 1] = np.cos((x + 100) / 100.) * 10.
         y[:, 2] = np.cos((x + 200) / 100.) * 10.
-        print(f"{humanize.intword(len(x))} points")
         return SpeasyVariable(axes=[VariableTimeAxis((x * 1e9).astype("datetime64[ns]"))], values=DataContainer(y),
                               columns=["x", "y", "z"])
 
 
 def load(main_window):
     return TestPlugin(main_window)
```

### Comparing `SciQLop-0.1.1/SciQLop/resources/__init__.py` & `SciQLop-0.2.1/SciQLop/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/SciQLop.png` & `SciQLop-0.2.1/SciQLop/resources/icons/SciQLop.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/Simple_icon_time.svg` & `SciQLop-0.2.1/SciQLop/resources/icons/Simple_icon_time.svg`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/add.png` & `SciQLop-0.2.1/SciQLop/resources/icons/add.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/allEvents.png` & `SciQLop-0.2.1/SciQLop/resources/icons/allEvents.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/catalogue.png` & `SciQLop-0.2.1/SciQLop/resources/icons/catalogue.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/chart.png` & `SciQLop-0.2.1/SciQLop/resources/icons/chart.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/cursor.png` & `SciQLop-0.2.1/SciQLop/resources/icons/cursor.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/dataSourceComponent.png` & `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceComponent.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/dataSourceNode.png` & `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceNode.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/dataSourceProduct.png` & `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceProduct.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/dataSourceRoot.png` & `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceRoot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/database.png` & `SciQLop-0.2.1/SciQLop/resources/icons/database.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/delete.png` & `SciQLop-0.2.1/SciQLop/resources/icons/delete.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/discard.png` & `SciQLop-0.2.1/SciQLop/resources/icons/discard.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/down.png` & `SciQLop-0.2.1/SciQLop/resources/icons/down.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/drag.png` & `SciQLop-0.2.1/SciQLop/resources/icons/drag.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/next.png` & `SciQLop-0.2.1/SciQLop/resources/icons/next.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/openInspector.png` & `SciQLop-0.2.1/SciQLop/resources/icons/openInspector.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/plot.png` & `SciQLop-0.2.1/SciQLop/resources/icons/plot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/pointer.png` & `SciQLop-0.2.1/SciQLop/resources/icons/pointer.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/previous.png` & `SciQLop-0.2.1/SciQLop/resources/icons/previous.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/rectangle.png` & `SciQLop-0.2.1/SciQLop/resources/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/remove.png` & `SciQLop-0.2.1/SciQLop/resources/icons/remove.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/satellite.svg` & `SciQLop-0.2.1/SciQLop/resources/icons/satellite.svg`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/save.png` & `SciQLop-0.2.1/SciQLop/resources/icons/save.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/sciqlop2PNG_1024.png` & `SciQLop-0.2.1/SciQLop/resources/icons/sciqlop2PNG_1024.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/time.png` & `SciQLop-0.2.1/SciQLop/resources/icons/time.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/trash.png` & `SciQLop-0.2.1/SciQLop/resources/icons/trash.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/unplot.png` & `SciQLop-0.2.1/SciQLop/resources/icons/unplot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/up.png` & `SciQLop-0.2.1/SciQLop/resources/icons/up.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/icons/zoom.png` & `SciQLop-0.2.1/SciQLop/resources/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/resources/resources.qrc` & `SciQLop-0.2.1/SciQLop/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/widgets/central_widget.py` & `SciQLop-0.2.1/SciQLop/widgets/central_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,99 @@
-from PySide6 import QtCore, QtWidgets, QtGui
-from PySide6.QtCore import Signal, QMimeData
-from PySide6.QtWidgets import QDockWidget, QMainWindow
+from typing import List
+
+import PySide6QtAds as QtAds
+from PySide6.QtCore import Signal, QMimeData, Qt, Slot
+from PySide6.QtGui import QCloseEvent
+from PySide6.QtWidgets import QMainWindow
+
 from .drag_and_drop import DropHandler, DropHelper
 from .plots.time_sync_panel import TimeSyncPanel
-from ..mime.types import PRODUCT_LIST_MIME_TYPE
-from ..mime import decode_mime
 from ..backend import TimeRange
 from ..backend.unique_names import make_simple_incr_name
+from ..backend.models import pipelines
+from ..mime import decode_mime
+from ..mime.types import PRODUCT_LIST_MIME_TYPE
+
+
+class TimeSyncPanelDockWidgetWrapper(QtAds.CDockWidget):
+    closed = Signal(str)
 
+    def __init__(self, name, time_range, parent=None):
+        super(TimeSyncPanelDockWidgetWrapper, self).__init__(name)
+        panel = TimeSyncPanel(parent=None, name=name,
+                              time_range=time_range)
+        panel.time_range = time_range
+        # self._panel.please_delete_me.connect(self._panel_asked_to_be_deleted)
+        self.setWidget(panel)
+        panel.delete_me.connect(self.closeDockWidget)
+        # self.viewToggled.connect(self._handle_view_toggled)
+        self.setFeature(QtAds.CDockWidget.DockWidgetDeleteOnClose, True)
+
+    @property
+    def panel(self) -> TimeSyncPanel:
+        return self.widget()
+
+    @property
+    def name(self):
+        return self.panel.name
+
+    def __del__(self):
+        with pipelines.model_update_ctx():
+            print('TimeSyncPanelDockWidgetWrapper dtor')
+            pipelines.remove_panel(self.panel)
 
-class CentralWidget(QtWidgets.QMainWindow):
+
+class CentralWidget(QMainWindow):
     panels_list_changed = Signal(list)
+    dock_widget_added = Signal(TimeSyncPanelDockWidgetWrapper)
 
     def __init__(self, parent, time_range: TimeRange):
         QMainWindow.__init__(self, parent)
-        self.setWindowFlags(QtCore.Qt.WindowType.Widget)
+        self.setWindowFlags(Qt.WindowType.Widget)
+        self.dock_manager = QtAds.CDockManager(self)
         self.setWindowTitle("Plot area")
-        self.setDockNestingEnabled(True)
         self.setMinimumSize(200, 200)
-        self._panels = {}
         self._default_time_range = time_range
         self._drop_helper = DropHelper(widget=self,
                                        handlers=[
                                            DropHandler(mime_type=PRODUCT_LIST_MIME_TYPE,
                                                        callback=self._plot)])
 
     def _plot(self, mime_data: QMimeData) -> bool:
         assert mime_data.hasFormat(PRODUCT_LIST_MIME_TYPE)
         products = decode_mime(mime_data)
         panel = self.new_plot_panel()
         panel.plot(products)
         return True
 
     def plot_panel(self, name: str) -> TimeSyncPanel or None:
-        return self._panels.get(name)
+        widget = self.dock_manager.findDockWidget(name)
+        if widget:
+            return widget.panel
 
     def new_plot_panel(self) -> TimeSyncPanel:
-        panel: TimeSyncPanel = TimeSyncPanel(name=make_simple_incr_name(base="Panel"),
-                                             time_range=self._default_time_range)
-        panel.time_range = self._default_time_range
-        dw = QDockWidget(self)
-        dw.setAttribute(QtCore.Qt.WidgetAttribute.WA_DeleteOnClose)
-        dw.setAllowedAreas(QtGui.Qt.DockWidgetArea.AllDockWidgetAreas)
-        dw.setWidget(panel)
-        panel.setParent(dw)
-        self.addDockWidget(QtGui.Qt.DockWidgetArea.TopDockWidgetArea, dw)
-        dw.setWindowTitle(panel.name)
-        self._panels[panel.name] = panel
-        panel.destroyed.connect(lambda: self.remove_panel(panel))
-        panel.delete_me.connect(dw.close)
+        dw = TimeSyncPanelDockWidgetWrapper(name=make_simple_incr_name(base="Panel"),
+                                            time_range=self._default_time_range, parent=self)
+        self.dock_manager.addDockWidget(QtAds.DockWidgetArea.TopDockWidgetArea, dw)
+        self.dock_widget_added.emit(dw)
         self.panels_list_changed.emit(self.panels())
-        return panel
+        pipelines.add_add_panel(dw.panel)
+        return dw.panel
 
     def set_default_time_range(self, time_range: TimeRange):
         self._default_time_range = time_range
 
-    def remove_panel(self, panel: TimeSyncPanel or str):
+    def remove_panel(self, panel: TimeSyncPanelDockWidgetWrapper or str):
+        print(f"remove_panel {panel}")
         if type(panel) is str:
-            name = panel
+            dw: TimeSyncPanelDockWidgetWrapper = self.dock_manager.findDockWidget(panel)
         else:
-            name = panel.name
-        if name in self._panels:
-            self._panels.pop(name)
+            dw = panel
+        dw.release_widget()
+        self.dock_manager.removeDockWidget(dw)
         self.panels_list_changed.emit(self.panels())
 
-    def panels(self):
-        return list(self._panels.keys())
+    def closeEvent(self, event: QCloseEvent):
+        event.accept()
+
+    def panels(self) -> List[str]:
+        return list(self.dock_manager.dockWidgetsMap().keys())
```

### Comparing `SciQLop-0.1.1/SciQLop/widgets/common/tree_view.py` & `SciQLop-0.2.1/SciQLop/widgets/common/tree_view.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from PySide6 import QtCore, QtWidgets, QtGui
+from PySide6 import QtCore, QtGui
+from PySide6.QtWidgets import QTreeView, QAbstractScrollArea, QSizePolicy, QAbstractItemView
 
 
-class TreeView(QtWidgets.QTreeView):
+class TreeView(QTreeView):
 
     def __init__(self, parent=None):
         super(TreeView, self).__init__(parent)
         self.header().setVisible(False)
         self.setDragEnabled(True)
-        self.setDragDropMode(QtWidgets.QAbstractItemView.DragOnly)
-        self.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
+        self.setDragDropMode(QAbstractItemView.DragOnly)
+        self.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self._expend_all_action = QtGui.QAction("Expand all")
         self._collapse_all_action = QtGui.QAction("Collapse all")
         self.addAction(self._expend_all_action)
         self.addAction(self._collapse_all_action)
         self.setContextMenuPolicy(QtCore.Qt.ActionsContextMenu)
         self._expend_all_action.triggered.connect(self.expandAll)
         self._collapse_all_action.triggered.connect(self.collapseAll)
+        self.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
+        self.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
```

### Comparing `SciQLop-0.1.1/SciQLop/widgets/console.py` & `SciQLop-0.2.1/SciQLop/widgets/console.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from typing import Dict, Any
-
 from PySide6.QtCore import QSize
-from PySide6.QtWidgets import QDockWidget
 from qtconsole.inprocess import QtInProcessKernelManager
 from qtconsole.rich_jupyter_widget import RichJupyterWidget
 
 
 class IPythonWidget(RichJupyterWidget):
     """Live IPython console widget.
 
@@ -44,15 +41,15 @@
 
         :param variable_dict: Dictionary of variables to be pushed to the
             console's interactive namespace (```{variable_name: object, …}```)
         """
         self.kernel_manager.kernel.shell.push(variable_dict)
 
 
-class Console(QDockWidget):
+class Console(IPythonWidget):
     """Dock Widget including a :class:`IPythonWidget` inside
     a vertical layout.
 
     .. image:: img/IPythonDockWidget.png
 
     :param available_vars: Dictionary of variables to be pushed to the
         console's interactive namespace: ``{"variable_name": object, …}``
@@ -61,26 +58,13 @@
     :param title: Dock widget title
     :param parent: Parent :class:`qt.QMainWindow` containing this
         :class:`qt.QDockWidget`
     """
 
     def __init__(self, parent=None, available_vars=None, custom_banner=None,
                  title="Console"):
-        super(Console, self).__init__(title, parent)
-
-        self.ipyconsole = IPythonWidget(custom_banner=custom_banner)
+        super(Console, self).__init__(parent, custom_banner=custom_banner)
 
         self.layout().setContentsMargins(0, 0, 0, 0)
-        self.setWidget(self.ipyconsole)
 
         if available_vars is not None:
-            self.ipyconsole.pushVariables(available_vars)
-
-    def pushVariables(self, variables: Dict[str, Any]):
-        self.ipyconsole.pushVariables(variables)
-
-    def showEvent(self, event):
-        """Make sure this widget is raised when it is shown
-        (when it is first created as a tab in PlotWindow or when it is shown
-        again after hiding).
-        """
-        self.raise_()
+            self.pushVariables(available_vars)
```

### Comparing `SciQLop-0.1.1/SciQLop/widgets/datetime_range.py` & `SciQLop-0.2.1/SciQLop/widgets/datetime_range.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/helper.py` & `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/helper.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py` & `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return mime_type in self._handlers and self._place_holder is None
 
     def _leave_drag(self):
         self._current_handler = None
         self._place_holder = None
 
     def leave_drag(self):
-        self._place_holder_delay.start(200)
+        self._place_holder_delay.start(500)
 
     def create_place_holder_if_needed(self, mime_type: str, child_widget: QWidget, position: QPointF) -> bool:
         if self.accepts(mime_type=mime_type):
             zone = _place_holder_zone(child_widget, position)
             if zone != PlaceHolderPosition.NONE:
                 index = self._widget.indexOf(child_widget)
                 if zone == PlaceHolderPosition.BOTTOM:
```

### Comparing `SciQLop-0.1.1/SciQLop/widgets/drag_and_drop/placeholder.py` & `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/placeholder.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/widgets/pipelines/pipeline_tree.py` & `SciQLop-0.2.1/SciQLop/widgets/pipelines/pipeline_tree.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.1.1/SciQLop/widgets/plots/plot.py` & `SciQLop-0.2.1/SciQLop/widgets/plots/time_series_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from typing import List
+from abc import abstractmethod
 
 from PySide6.QtCore import QMimeData, Qt, QMargins, Signal
 from PySide6.QtGui import QColorConstants, QColor, QMouseEvent
 from PySide6.QtWidgets import QVBoxLayout, QFrame
-from SciQLopPlots import QCustomPlot, QCP, QCPAxisTickerDateTime, QCPLegend, QCPAbstractLegendItem, QCPMarginGroup, \
-    QCPColorScale
+from SciQLopPlots import SciQLopPlot, QCustomPlot, QCP, QCPAxisTickerDateTime, QCPLegend, QCPAbstractLegendItem, \
+    QCPMarginGroup, \
+    QCPColorScale, SciQLopGraph, SciQLopColorMap
 from seaborn import color_palette
 
 from SciQLop.backend.models import products
+from SciQLop.backend.pipelines_model.auto_register import auto_register
 from SciQLop.backend.pipelines_model.data_provider import DataProvider
 from SciQLop.backend.pipelines_model.data_provider import providers
-from SciQLop.backend.pipelines_model.plot import Plot as _Plot
+from SciQLop.backend.pipelines_model.graph import Graph
 from SciQLop.backend.products_model.product_node import ProductNode
+from SciQLop.backend.pipelines_model.base import PipelineModelItem
+from SciQLop.backend.pipelines_model.base import model as pipelines_model
 from .colormap_graph import ColorMapGraph
 from .line_graph import LineGraph
 from ..drag_and_drop import DropHandler, DropHelper
 from ...backend import Product
 from ...backend import TimeRange
-from ...backend.enums import ParameterType
+from ...backend.enums import ParameterType, DataOrder
+from ...backend.unique_names import make_simple_incr_name
 from ...mime import decode_mime
 from ...mime.types import PRODUCT_LIST_MIME_TYPE, TIME_RANGE_MIME_TYPE
 
 
 def _to_qcolor(r: float, g: float, b: float):
     return QColor(int(r * 255), int(g * 255), int(b * 255))
 
 
-def _configure_plot(plot: QCustomPlot):
+def _configure_plot(plot: SciQLopPlot):
     plot.setPlottingHint(QCP.phFastPolylines, True)
     plot.setInteractions(
         QCP.iRangeDrag | QCP.iRangeZoom | QCP.iSelectPlottables | QCP.iSelectAxes | QCP.iSelectLegend | QCP.iSelectItems)
     plot.legend.setVisible(True)
     plot.legend.setSelectableParts(QCPLegend.SelectablePart.spItems)
     date_ticker = QCPAxisTickerDateTime()
     date_ticker.setDateTimeFormat("yyyy/MM/dd \nhh:mm:ss")
@@ -45,22 +51,27 @@
     layout = plot.layout()
     if layout:
         layout.setSpacing(0)
         layout.setContentsMargins(0, 0, 0, 0)
     plot.setAutoAddPlottableToLegend(False)
 
 
-class TimeSeriesPlot(QFrame, _Plot):
+class MetaTimeSeriesPlot(type(QFrame), type(PipelineModelItem)):
+    pass
+
+
+@auto_register
+class TimeSeriesPlot(QFrame, PipelineModelItem, metaclass=MetaTimeSeriesPlot):
     time_range_changed = Signal(TimeRange)
     _time_range: TimeRange = TimeRange(0., 0.)
 
     def __init__(self, parent=None):
-        super(TimeSeriesPlot, self).__init__(parent)
-        _Plot.__init__(self, f"Plot", parent)
-        self._plot = QCustomPlot(self)
+        QFrame.__init__(self, parent=parent)
+        self.setObjectName(make_simple_incr_name(base="Plot"))
+        self._plot = SciQLopPlot(self)
         self.setLayout(QVBoxLayout())
         self.layout().addWidget(self._plot)
         self.setMinimumHeight(300)
         self._drop_helper = DropHelper(widget=self,
                                        handlers=[
                                            DropHandler(mime_type=PRODUCT_LIST_MIME_TYPE,
                                                        callback=self._plot_from_mime_data),
@@ -71,14 +82,15 @@
         self._palette_index = 0
         _configure_plot(self._plot)
         self.setContentsMargins(0, 0, 0, 0)
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.xAxis.rangeChanged.connect(lambda range: self.time_range_changed.emit(TimeRange(range.lower, range.upper)))
         self._plot.selectionChangedByUser.connect(self._update_selection)
         self._plot.legendDoubleClick.connect(self._hide_graph)
+        self._parent_node = None
 
     def _hide_graph(self, legend: QCPLegend, item: QCPAbstractLegendItem, event: QMouseEvent):
         item.plottable().setVisible(not item.plottable().visible())
         if item.plottable().visible():
             item.setTextColor(QColorConstants.Black)
             item.setSelectedTextColor(QColorConstants.Black)
         else:
@@ -94,14 +106,18 @@
                 item.setSelected(True)
                 graph.setSelected(True)
 
     def set_margin_group(self, margin_group: QCPMarginGroup):
         self._plot.axisRect(0).setMarginGroup(QCP.msLeft, margin_group)
 
     @property
+    def plot_instance(self):
+        return self._plot
+
+    @property
     def xAxis(self):
         return self._plot.xAxis
 
     @property
     def xAxis2(self):
         return self._plot.xAxis2
 
@@ -112,16 +128,19 @@
     @property
     def yAxis2(self):
         return self._plot.yAxis2
 
     def replot(self, refresh_priority=QCustomPlot.rpQueuedReplot):
         return self._plot.replot(refresh_priority)
 
-    def addSciQLopGraph(self, x_axis, y_axis, labels, data_order):
-        return self._plot.addSciQLopGraph(x_axis, y_axis, labels, data_order)
+    def addSciQLopGraph(self, x_axis, y_axis, data_order, labels=None):
+        if labels is not None:
+            return SciQLopGraph(self._plot, x_axis, y_axis, labels, data_order)
+        else:
+            return SciQLopGraph(self._plot, x_axis, y_axis, data_order)
 
     def addSciQLopColorMap(self, x_axis, y_axis, label, with_color_scale=True):
         colormap = self._plot.addSciQLopColorMap(x_axis, y_axis, label)
         colormap.colorMap().setLayer(self._plot.layer("background"))
         if with_color_scale:
             color_scale = QCPColorScale(self._plot)
             self._plot.plotLayout().addElement(0, 1, color_scale)
@@ -147,50 +166,98 @@
 
     def _set_time_range(self, mime_data: QMimeData) -> bool:
         self.time_range = decode_mime(mime_data, [TIME_RANGE_MIME_TYPE])
         return True
 
     @property
     def time_range(self) -> TimeRange:
-        return TimeRange(self.xAxis.range().lower, self.xAxis.range().upper)
+        return TimeRange.from_qcprange(self.xAxis.range())
 
     @time_range.setter
     def time_range(self, time_range: TimeRange):
         if self._time_range != time_range:
-            print("Setting xAxis range")
             self.xAxis.setRange(time_range.start, time_range.stop)
             self.replot(QCustomPlot.rpQueuedReplot)
 
     def plot(self, product: Product or str):
         if type(product) is str:
             product = products.product(product)
-        if product.parameter_type in (ParameterType.VECTOR, ParameterType.MULTICOMPONENT, ParameterType.SCALAR):
-            self.add_multi_line_graph(providers[product.provider], product,
-                                      components=product.metadata.get('components') or [product.name])
-        elif product.parameter_type == ParameterType.SPECTROGRAM:
-            self.add_colormap_graph(providers[product.provider], product)
-
-    def add_multi_line_graph(self, provider: DataProvider, product: ProductNode, components: List[str]):
-        graph = LineGraph(parent=self, provider=provider, product=product)
-        self.xAxis.rangeChanged.connect(lambda r: graph.xRangeChanged.emit(TimeRange(r.lower, r.upper)))
-        return graph
-        # self._pipeline.append(PlotPipeline(graph=graph, provider=provider, product=product, time_range=self.time_range))
+        if product:
+            if product.parameter_type in (ParameterType.VECTOR, ParameterType.MULTICOMPONENT, ParameterType.SCALAR):
+                self._add_multi_line_graph(providers[product.provider], product,
+                                           components=product.metadata.get('components') or [
+                                               product.name])
+            elif product.parameter_type == ParameterType.SPECTROGRAM and not self.has_colormap:
+                self._add_colormap_graph(providers[product.provider], product)
+
+    def _register_new_graph(self, graph):
+        self.time_range_changed.connect(graph.xRangeChanged)
+
+    def _add_multi_line_graph(self, provider: DataProvider, product: ProductNode, components: List[str]):
+        graph = LineGraph(parent=self, sciqlop_graph=self.addSciQLopGraph(self.xAxis, self.yAxis,
+                                                                          SciQLopGraph.DataOrder.xFirst if provider.data_order == DataOrder.X_FIRST else SciQLopGraph.DataOrder.yFirst),
+                          provider=provider, product=product)
+        self._register_new_graph(graph)
 
-    def add_colormap_graph(self, provider: DataProvider, product: ProductNode):
+    def _add_colormap_graph(self, provider: DataProvider, product: ProductNode):
         graph = ColorMapGraph(parent=self, provider=provider, product=product)
-        self.xAxis.rangeChanged.connect(lambda r: graph.xRangeChanged.emit(TimeRange(r.lower, r.upper)))
-        return graph
-        # self._pipeline.append(PlotPipeline(graph=graph, provider=provider, product=product, time_range=self.time_range))
+        self._register_new_graph(graph)
 
     def remove_graph(self, graph):
-        self._plot.removeGraph(graph)
+        with pipelines_model.model_update_ctx():
+            if isinstance(graph, SciQLopGraph) or isinstance(graph, SciQLopColorMap):
+                for g in self._graphs:
+                    if g.graph is graph:
+                        graph = g
+            graph.deleteLater()
 
     def select(self):
         self.setStyleSheet("border: 3px dashed blue;")
 
     def unselect(self):
         self.setStyleSheet("")
 
-    def delete(self):
-        _Plot.delete(self)
+    @property
+    def has_colormap(self):
+        return len(list(filter(lambda c: isinstance(c, ColorMapGraph), self.children_nodes))) > 0
+
+    def __eq__(self, other: 'PipelineModelItem') -> bool:
+        return self is other
+
+    @property
+    def icon(self) -> str:
+        return ""
+
+    @property
+    def name(self) -> str:
+        return self.objectName()
+
+    @name.setter
+    def name(self, new_name: str):
+        with pipelines_model.model_update_ctx():
+            self.setObjectName(new_name)
+
+    @property
+    def parent_node(self) -> 'PipelineModelItem':
+        return self._parent_node
+
+    @parent_node.setter
+    def parent_node(self, parent: 'PipelineModelItem'):
+        with pipelines_model.model_update_ctx():
+            if self._parent_node is not None:
+                self._parent_node.remove_children_node(self)
+            self._parent_node = parent
+            if parent is not None:
+                parent.add_children_node(self)
+
+    @property
+    def children_nodes(self) -> List['PipelineModelItem']:
+        return list(filter(lambda n: isinstance(n, Graph), self.children()))
+
+    def remove_children_node(self, node: 'PipelineModelItem'):
+        self.remove_graph(node)
+
+    def add_children_node(self, node: 'PipelineModelItem'):
+        pass
+
+    def delete_node(self):
         self.close()
-        self.deleteLater()
```

### Comparing `SciQLop-0.1.1/SciQLop/widgets/products_tree/products_tree.py` & `SciQLop-0.2.1/SciQLop/widgets/products_tree/products_tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from PySide6 import QtCore, QtWidgets, QtGui
+from PySide6 import QtCore, QtGui
+from PySide6.QtWidgets import QSizePolicy, QWidget, QLineEdit, QCompleter, QVBoxLayout
 
 from SciQLop.backend.models import products
 from SciQLop.widgets.common import TreeView
 
 
-class ProductTree(QtWidgets.QWidget):
+class ProductTree(QWidget):
     def __init__(self, parent=None):
         super(ProductTree, self).__init__(parent)
         self._view = TreeView(self)
         self._view.setModel(products)
         self._view.setSortingEnabled(False)
-        self._filter = QtWidgets.QLineEdit(self)
+        self._filter = QLineEdit(self)
         self._filter.setClearButtonEnabled(True)
-        self._filter.addAction(QtGui.QIcon(":/icons/zoom.png"), QtWidgets.QLineEdit.LeadingPosition)
+        self._filter.addAction(QtGui.QIcon(":/icons/zoom.png"), QLineEdit.LeadingPosition)
         self._filter.setPlaceholderText("Search...")
-        self._completer = QtWidgets.QCompleter(self)
+        self._completer = QCompleter(self)
         self._completer.setModel(products.completion_model)
         self._completer.setCaseSensitivity(QtCore.Qt.CaseInsensitive)
-        self._completer.setCompletionMode(QtWidgets.QCompleter.PopupCompletion)
-        self._completer.setModelSorting(QtWidgets.QCompleter.CaseSensitivelySortedModel)
+        self._completer.setCompletionMode(QCompleter.PopupCompletion)
+        self._completer.setModelSorting(QCompleter.CaseSensitivelySortedModel)
         self._filter.setCompleter(self._completer)
-        self.setLayout(QtWidgets.QVBoxLayout())
+        self.setLayout(QVBoxLayout())
         self.layout().addWidget(self._filter)
         self.layout().addWidget(self._view)
         self._filter.textChanged.connect(lambda: products.set_filter(self._filter.text()))
         self.setWindowTitle("Products")
+        self.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
```

### Comparing `SciQLop-0.1.1/pyproject.toml` & `SciQLop-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'SciQLop'
-version = "0.1.1"
+version = "0.2.1"
 description = "An ergonomic and efficient application to browse and label in situ plasma measurements from multi-mission satellite data."
 keywords = ["machine-learning", "satellite", "plasma-physics", "nasa-data", "amda", "cdpp"]
 authors = [
     { name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
@@ -25,17 +25,17 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ['numpy', 'SciQLopPlots>=0.1.7', 'speasy', 'qtconsole', 'tscat_gui>=0.2.0', 'seaborn', "scipy"]
+dependencies = ['numpy', 'SciQLopPlots>=0.3.2', 'speasy', 'qtconsole', 'tscat_gui>=0.2.0', 'seaborn', "scipy", "PySide6-QtAds==4.0.1.2"]
 [project.urls]
 homepage = "https://github.com/SciQLop/SciQLop"
 
 [project.gui-scripts]
 sciqlop = "SciQLop.app:main"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
-qt_api = "pyside6"
+qt_api = "pyside6"
```

### Comparing `SciQLop-0.1.1/PKG-INFO` & `SciQLop-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciQLop
-Version: 0.1.1
+Version: 0.2.1
 Summary: An ergonomic and efficient application to browse and label in situ plasma measurements from multi-mission satellite data.
 Keywords: machine-learning,satellite,plasma-physics,nasa-data,amda,cdpp
 Author-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Maintainer-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,21 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy
-Requires-Dist: SciQLopPlots>=0.1.7
+Requires-Dist: SciQLopPlots>=0.3.2
 Requires-Dist: speasy
 Requires-Dist: qtconsole
 Requires-Dist: tscat_gui>=0.2.0
 Requires-Dist: seaborn
 Requires-Dist: scipy
+Requires-Dist: PySide6-QtAds==4.0.1.2
 Project-URL: homepage, https://github.com/SciQLop/SciQLop
 
 
 <div style="text-align:center">
 <img src="gui/resources/icones/sciqlop2PNG_1024.png" alt="sciqlop_logo" style="width: 200px;"/>
 <br /><br />
 <img src="pictures/sciqlop_screenshot.png" alt="sciqlop_logo" style="width: 80%;"/>
```

