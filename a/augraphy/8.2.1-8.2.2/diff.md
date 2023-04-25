# Comparing `tmp/augraphy-8.2.1.tar.gz` & `tmp/augraphy-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augraphy-8.2.1.tar", last modified: Thu Apr  6 13:14:06 2023, max compression
+gzip compressed data, was "augraphy-8.2.2.tar", last modified: Tue Apr 25 01:49:40 2023, max compression
```

## Comparing `augraphy-8.2.1.tar` & `augraphy-8.2.2.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.160456 augraphy-8.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-06 13:13:58.000000 augraphy-8.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-06 13:14:06.160456 augraphy-8.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-06 13:13:58.000000 augraphy-8.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.152457 augraphy-8.2.1/augraphy/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.156456 augraphy-8.2.1/augraphy/augmentations/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/badphotocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/bindingsandfasteners.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/bleedthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/bookbinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/brightnesstexturize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/colorpaper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/dirtydrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/dirtyrollers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/dithering.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/faxify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/inkbleed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/jpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/letterpress.py
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/lightinggradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/lowinkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/lowinkperiodiclines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/lowinkrandomlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/noisetexturize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/pageborder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/pencilscribbles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/subtlenoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/augmentations/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.156456 augraphy-8.2.1/augraphy/base/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/augmentationpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/augmentationresult.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/augmentationsequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/oneof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/base/paperfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.160456 augraphy-8.2.1/augraphy/default/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/default/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.160456 augraphy-8.2.1/augraphy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/composepipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/figsharedownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/imageoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/noisegenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-04-06 13:13:58.000000 augraphy-8.2.1/augraphy/utilities/overlaybuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:14:06.156456 augraphy-8.2.1/augraphy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-06 13:14:06.000000 augraphy-8.2.1/augraphy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-06 13:14:06.000000 augraphy-8.2.1/augraphy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:14:06.000000 augraphy-8.2.1/augraphy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 13:14:06.000000 augraphy-8.2.1/augraphy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 13:14:06.000000 augraphy-8.2.1/augraphy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 13:13:58.000000 augraphy-8.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:14:06.160456 augraphy-8.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-06 13:13:58.000000 augraphy-8.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.202194 augraphy-8.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 01:49:22.000000 augraphy-8.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-25 01:49:40.202194 augraphy-8.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-04-25 01:49:22.000000 augraphy-8.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.194194 augraphy-8.2.2/augraphy/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/badphotocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bindingsandfasteners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bleedthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bookbinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/brightnesstexturize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/colorpaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dirtydrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dirtyrollers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dithering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/faxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/inkbleed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/letterpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lightinggradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/linesdegradation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkperiodiclines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkrandomlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/noisetexturize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/pageborder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/quasicrystal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/scribbles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/subtlenoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/oneof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/paperfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32656 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/default/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.202194 augraphy-8.2.2/augraphy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/composepipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/figsharedownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/imageoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/meshgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/noisegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/overlaybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/slidingwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.194194 augraphy-8.2.2/augraphy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-25 01:49:40.000000 augraphy-8.2.2/augraphy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 01:49:23.000000 augraphy-8.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:49:40.202194 augraphy-8.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-25 01:49:23.000000 augraphy-8.2.2/setup.py
```

### Comparing `augraphy-8.2.1/LICENSE` & `augraphy-8.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/PKG-INFO` & `augraphy-8.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: augraphy
-Version: 8.2.1
+Version: 8.2.2
 Summary: Augmentation pipeline for rendering synthetic paper printing and scanning processes
 Home-page: https://github.com/sparkfish/augraphy
 Author: Sparkfish LLC
 Author-email: packages@sparkfish.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sparkfish/augraphy/issues
 Description: <p align="center">
-            <img src="images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
         </p>
         
         Augraphy is a Python library that creates multiple copies of original documents though an augmentation pipeline that randomly distorts each copy -- degrading the clean version into dirty and realistic copies rendered through synthetic paper printing, faxing, scanning and copy machine processes.
         
         Highly-configurable pipelines apply adjustments to the originals to create realistic old or noisy documents by acting as a factory, producing almost an infinite number of variations from their source.  This simulation of realistic paper-oriented process distortions can create large amounts of training data for AI/ML processes to learn how to remove those distortions.
         
         Treatments applied by Augraphy fabricate realistic documents that appear to have been printed on dirty laser or inkjet printers, scanned by dirty office scanners, faxed by low-resolution fax machines and otherwise mistreated by real-world paper handling office equipment.
@@ -32,19 +32,19 @@
         A paper factory provides either a white page or a randomly-selected paper texture base.  Like the ink layer, the paper can also be processed through a pipeline to further provide random realistic paper textures.
         
         After both the ink and paper phases are completed, processing continues by applying the ink, with its desired effects, to the paper.  This merged document image is then augmented further with distortions such as adding folds or other physical deformations or distortions that rely on simultaneous interactions of paper and ink layers.
         
         The end result is an image that mimics real documents.
         
         <p align="center" width="100%">
-            <img src="images/Pipeline.png">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
         </p>
         
         ## Example Before / After Images
-        ![examples](https://user-images.githubusercontent.com/74747193/135170284-8249fbab-2748-4230-821c-e56815e797cf.png)
+        ![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
         
         
         # Example Usage
         To use the default pipeline which contains all available augmentations and sensible defaults:
         
         ```python
         from augraphy import *
@@ -88,14 +88,17 @@
         |LowInkRandomLines   |            71.05|            12.74|
         |Markup              |             0.71|           533.16|
         |NoiseTexturize      |             0.53|           249.36|
         |PageBorder          |             0.52|           465.19|
         |PencilScribbles     |             1.15|           138.13|
         |SubtleNoise         |             1.03|           202.87|
         |WaterMark           |             1.19|           373.41|
+        |VoronoiTessellation |             0.47|            15.90|
+        |DelaunayTessellation|             0.76|            36.33|
+        |Quasi Crystals      |             0.25|              7.5|
         
         # Alternative Augmentation Libraries
         There are plenty of choices when it comes to [augmentation libraries](https://github.com/AgaMiko/data-augmentation-review).  However, only Augraphy is designed to address everyday office automation needs associated with paper-oriented process distortions that come from printing, faxing, scanning and copy machines.  Most other libraries focus on video and images pertinent to camera-oriented data sources and problem domains.  Augraphy is focused on supporting problems related to automation of document images such as OCR, form recognition, form data extraction, document classification, barcode decoding, denoising, document restoration, identity document data extraction, document cropping, etc.  Eventually, Augraphy will be able to support photo OCR problems with augmentations designed to emulate camera phone distortions.
         
         # Contributing
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
@@ -104,15 +107,15 @@
         
         BibTeX:
         ```
         @software{augraphy_library,
             author = {The Augraphy Project},
             title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
             url = {https://github.com/sparkfish/augraphy},
-            version = {8.2.1}
+            version = {8.2.2}
         }
         ```
         
         # License
         Copyright 2023 Sparkfish LLC
         
         Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.1/README.md` & `augraphy-8.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
+    <img src="https://github.com/sparkfish/augraphy/blob/dev/images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
 </p>
 
 Augraphy is a Python library that creates multiple copies of original documents though an augmentation pipeline that randomly distorts each copy -- degrading the clean version into dirty and realistic copies rendered through synthetic paper printing, faxing, scanning and copy machine processes.
 
 Highly-configurable pipelines apply adjustments to the originals to create realistic old or noisy documents by acting as a factory, producing almost an infinite number of variations from their source.  This simulation of realistic paper-oriented process distortions can create large amounts of training data for AI/ML processes to learn how to remove those distortions.
 
 Treatments applied by Augraphy fabricate realistic documents that appear to have been printed on dirty laser or inkjet printers, scanned by dirty office scanners, faxed by low-resolution fax machines and otherwise mistreated by real-world paper handling office equipment.
@@ -23,19 +23,19 @@
 A paper factory provides either a white page or a randomly-selected paper texture base.  Like the ink layer, the paper can also be processed through a pipeline to further provide random realistic paper textures.
 
 After both the ink and paper phases are completed, processing continues by applying the ink, with its desired effects, to the paper.  This merged document image is then augmented further with distortions such as adding folds or other physical deformations or distortions that rely on simultaneous interactions of paper and ink layers.
 
 The end result is an image that mimics real documents.
 
 <p align="center" width="100%">
-    <img src="images/Pipeline.png">
+    <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
 </p>
 
 ## Example Before / After Images
-![examples](https://user-images.githubusercontent.com/74747193/135170284-8249fbab-2748-4230-821c-e56815e797cf.png)
+![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
 
 
 # Example Usage
 To use the default pipeline which contains all available augmentations and sensible defaults:
 
 ```python
 from augraphy import *
@@ -79,14 +79,17 @@
 |LowInkRandomLines   |            71.05|            12.74|
 |Markup              |             0.71|           533.16|
 |NoiseTexturize      |             0.53|           249.36|
 |PageBorder          |             0.52|           465.19|
 |PencilScribbles     |             1.15|           138.13|
 |SubtleNoise         |             1.03|           202.87|
 |WaterMark           |             1.19|           373.41|
+|VoronoiTessellation |             0.47|            15.90|
+|DelaunayTessellation|             0.76|            36.33|
+|Quasi Crystals      |             0.25|              7.5|
 
 # Alternative Augmentation Libraries
 There are plenty of choices when it comes to [augmentation libraries](https://github.com/AgaMiko/data-augmentation-review).  However, only Augraphy is designed to address everyday office automation needs associated with paper-oriented process distortions that come from printing, faxing, scanning and copy machines.  Most other libraries focus on video and images pertinent to camera-oriented data sources and problem domains.  Augraphy is focused on supporting problems related to automation of document images such as OCR, form recognition, form data extraction, document classification, barcode decoding, denoising, document restoration, identity document data extraction, document cropping, etc.  Eventually, Augraphy will be able to support photo OCR problems with augmentations designed to emulate camera phone distortions.
 
 # Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
@@ -95,15 +98,15 @@
 
 BibTeX:
 ```
 @software{augraphy_library,
     author = {The Augraphy Project},
     title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
     url = {https://github.com/sparkfish/augraphy},
-    version = {8.2.1}
+    version = {8.2.2}
 }
 ```
 
 # License
 Copyright 2023 Sparkfish LLC
 
 Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.1/augraphy/augmentations/__init__.py` & `augraphy-8.2.2/augraphy/augmentations/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 from augraphy.augmentations.badphotocopy import BadPhotoCopy
 from augraphy.augmentations.bindingsandfasteners import BindingsAndFasteners
 from augraphy.augmentations.bleedthrough import BleedThrough
 from augraphy.augmentations.bookbinding import BookBinding
 from augraphy.augmentations.brightness import Brightness
 from augraphy.augmentations.brightnesstexturize import BrightnessTexturize
 from augraphy.augmentations.colorpaper import ColorPaper
+from augraphy.augmentations.delaunay import DelaunayTessellation
 from augraphy.augmentations.dirtydrum import DirtyDrum
 from augraphy.augmentations.dirtyrollers import DirtyRollers
 from augraphy.augmentations.dithering import Dithering
 from augraphy.augmentations.faxify import Faxify
 from augraphy.augmentations.folding import Folding
 from augraphy.augmentations.gamma import Gamma
 from augraphy.augmentations.geometric import Geometric
 from augraphy.augmentations.inkbleed import InkBleed
 from augraphy.augmentations.jpeg import Jpeg
 from augraphy.augmentations.letterpress import Letterpress
 from augraphy.augmentations.lightinggradient import LightingGradient
+from augraphy.augmentations.linesdegradation import LinesDegradation
 from augraphy.augmentations.lowinkperiodiclines import LowInkPeriodicLines
 from augraphy.augmentations.lowinkrandomlines import LowInkRandomLines
 from augraphy.augmentations.markup import Markup
 from augraphy.augmentations.noisetexturize import NoiseTexturize
 from augraphy.augmentations.pageborder import PageBorder
-from augraphy.augmentations.pencilscribbles import PencilScribbles
+from augraphy.augmentations.quasicrystal import PatternGenerator
+from augraphy.augmentations.scribbles import Scribbles
 from augraphy.augmentations.subtlenoise import SubtleNoise
+from augraphy.augmentations.voronoi import VoronoiTessellation
 from augraphy.augmentations.watermark import WaterMark
 
+
 __all__ = [
     "BadPhotoCopy",
     "BindingsAndFasteners",
     "BleedThrough",
     "BookBinding",
     "Brightness",
     "BrightnessTexturize",
     "ColorPaper",
+    "DelaunayTessellation",
     "DirtyDrum",
     "DirtyRollers",
     "Dithering",
     "Faxify",
     "Folding",
     "Gamma",
     "Geometric",
     "InkBleed",
     "Jpeg",
     "Letterpress",
     "LightingGradient",
+    "LinesDegradation",
     "LowInkPeriodicLines",
     "LowInkRandomLines",
     "Markup",
     "NoiseTexturize",
     "PageBorder",
-    "PencilScribbles",
+    "PatternGenerator",
+    "Scribbles",
     "SubtleNoise",
+    "VoronoiTessellation",
     "WaterMark",
 ]
```

### Comparing `augraphy-8.2.1/augraphy/augmentations/badphotocopy.py` & `augraphy-8.2.2/augraphy/augmentations/badphotocopy.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/bindingsandfasteners.py` & `augraphy-8.2.2/augraphy/augmentations/bindingsandfasteners.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/bleedthrough.py` & `augraphy-8.2.2/augraphy/augmentations/bleedthrough.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/bookbinding.py` & `augraphy-8.2.2/augraphy/augmentations/bookbinding.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/brightness.py` & `augraphy-8.2.2/augraphy/augmentations/brightness.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/brightnesstexturize.py` & `augraphy-8.2.2/augraphy/augmentations/brightnesstexturize.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/colorpaper.py` & `augraphy-8.2.2/augraphy/augmentations/colorpaper.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/dirtydrum.py` & `augraphy-8.2.2/augraphy/augmentations/dirtydrum.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/dirtyrollers.py` & `augraphy-8.2.2/augraphy/augmentations/dirtyrollers.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/dithering.py` & `augraphy-8.2.2/augraphy/augmentations/dithering.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/faxify.py` & `augraphy-8.2.2/augraphy/augmentations/faxify.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/folding.py` & `augraphy-8.2.2/augraphy/augmentations/folding.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/gamma.py` & `augraphy-8.2.2/augraphy/augmentations/gamma.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/geometric.py` & `augraphy-8.2.2/augraphy/augmentations/geometric.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 
 class Geometric(Augmentation):
     """Applies basic geometric transformations such as resizing, flips and rotation.
 
     :param scale: Pair of floats determining new scale of image.
     :type scale: tuple, optional
     :param translation: Pair of values determining x and y translation value.
-            The translation value will be in percentage of the image size if the value is in between 0 - 1:
-            x (int) = image width  * x (float and 0 - 1)
-            y (int) = image height * y (float and 0 - 1)
+            The translation value will be in percentage of the image size if the value is float and in between 0.0 - 1.0:
+            x (int) = image width  * x (float and 0.0 - 1.0);
+            y (int) = image height * y (float and 0.0 - 1.0)
     :type translation: tuple, optional
     :param fliplr: Flag to flip image in left right direction.
     :type fliplr: int, optional
     :param flipud: Flag to flip image in up down direction.
     :type flipud: int, optional
     :param crop: Tuple of 4 (x0, y0, xn, yn) to crop section of image.
-             The value will be in percentage of the image size if the value is in between 0 - 1:
-             x0 (int) = image width  * x0 (float and 0 - 1)
-             y0 (int) = image height * y0 (float and 0 - 1)
-             xn (int) = image width  * xn (float and 0 - 1)
-             yn (int) = image height * yn (float and 0 - 1)
+             The value will be in percentage of the image size if the value is float and in between 0.0 - 1.0:
+             x0 (int) = image width  * x0 (float and 0.0 - 1.0);
+             y0 (int) = image height * y0 (float and 0.0 - 1.0);
+             xn (int) = image width  * xn (float and 0.0 - 1.0);
+             yn (int) = image height * yn (float and 0.0 - 1.0)
     :type crop: tuple, optional
     :param rotate_range: Pair of ints determining the range from which to sample
            the image rotation.
     :type rotate_range: tuple, optional
     :param randomize: Flag to apply random geometric transformations.
     :type randomize: int, optional
     :param padding: Padding amount on each (left, right, top, bottom) side.
-            The padding amount will be in percentage of the image size if the value is in between 0 - 1:
-            left   (int) = image width  * left   (float and 0 - 1)
-            right  (int) = image height * right  (float and 0 - 1)
-            top    (int) = image width  * top    (float and 0 - 1)
-            bottom (int) = image height * bottom (float and 0 - 1)
-    :type padding: tuple, optional
+            The padding amount will be in percentage of the image size if the value is float and in between 0.0 - 1.0:
+            left   (int) = image width  * left   (float and 0.0 - 1.0);
+            right  (int) = image height * right  (float and 0.0 - 1.0);
+            top    (int) = image width  * top    (float and 0.0 - 1.0);
+            bottom (int) = image height * bottom (float and 0.0 - 1.0)
+    :type padding: list, optional
     :param padding_type: Padding methods, select from fill,duplicate and mirror.
     :type paddng_type: string, optional
     :param padding_value: Padding value (in BGR) for fill padding method.
     :type paddng_value: tuple, optional
     :param p: The probability that this Augmentation will be applied.
     :type p: float, optional
     """
@@ -52,15 +52,15 @@
         self,
         scale=(1, 1),
         translation=(0, 0),
         fliplr=0,
         flipud=0,
         crop=(),
         rotate_range=(0, 0),
-        padding=(0, 0, 0, 0),
+        padding=[0, 0, 0, 0],
         padding_type="fill",
         padding_value=(255, 255, 255),
         randomize=1,
         p=1,
     ):
         """Constructor method"""
         super().__init__(p=p)
@@ -119,18 +119,22 @@
             # crop image
             if self.crop:
                 # make sure there's only 4 inputs, x0, y0, xn, yn
                 if len(self.crop) == 4:
                     ysize, xsize = image.shape[:2]
                     xstart, ystart, xend, yend = self.crop
 
-                    if xstart < 1 and ystart < 1 and (xend <= 1 and xend > 0) and (yend <= 1 and yend > 0):
+                    # when value is float and in between 0-1, scale it with image size
+                    if xstart >= 0 and xstart <= 1 and isinstance(xstart, float):
                         xstart = int(xstart * xsize)
+                    if ystart >= 0 and ystart <= 1 and isinstance(ystart, float):
                         ystart = int(ystart * ysize)
+                    if xend >= 0 and xend <= 1 and isinstance(xend, float):
                         xend = int(xend * xsize)
+                    if yend >= 0 and yend <= 1 and isinstance(yend, float):
                         yend = int(yend * ysize)
 
                     # when value is set to -1, it takes image size
                     if yend == -1:
                         yend = ysize
                     if xend == -1:
                         xend = xsize
@@ -148,16 +152,15 @@
                     self.padding_value = np.mean(self.padding_value)
 
                 # padding on left side
                 if self.padding[0] > 0:
                     # get image size
                     ysize, xsize = image.shape[:2]
                     # convert percentage into pixel amount
-                    if self.padding[0] < 1:
-                        self.padding = list(self.padding)
+                    if self.padding[0] <= 1 and isinstance(self.padding[0], float):
                         self.padding[0] = int(self.padding[0] * xsize)
 
                     # different padding shape for grayscale and colored image
                     if len(image.shape) > 2:
                         padding_shape = (ysize, self.padding[0], image.shape[2])
                     else:
                         padding_shape = (ysize, self.padding[0])
@@ -172,16 +175,15 @@
                     image = np.concatenate([image_padding, image], axis=1)
 
                 # padding on right side
                 if self.padding[1] > 0:
                     # get image size
                     ysize, xsize = image.shape[:2]
                     # convert percentage into pixel amount
-                    if self.padding[1] < 1:
-                        self.padding = list(self.padding)
+                    if self.padding[1] <= 1 and isinstance(self.padding[1], float):
                         self.padding[1] = int(self.padding[1] * xsize)
 
                     # different padding shape for grayscale and colored image
                     if len(image.shape) > 2:
                         padding_shape = (ysize, self.padding[1], image.shape[2])
                     else:
                         padding_shape = (ysize, self.padding[1])
@@ -196,16 +198,15 @@
                     image = np.concatenate([image, image_padding], axis=1)
 
                 # padding on top side
                 if self.padding[2] > 0:
                     # get image size
                     ysize, xsize = image.shape[:2]
                     # convert percentage into pixel amount
-                    if self.padding[2] < 1:
-                        self.padding = list(self.padding)
+                    if self.padding[2] <= 1 and isinstance(self.padding[2], float):
                         self.padding[2] = int(self.padding[2] * ysize)
 
                     # different padding shape for grayscale and colored image
                     if len(image.shape) > 2:
                         padding_shape = (self.padding[2], xsize, image.shape[2])
                     else:
                         padding_shape = (self.padding[2], xsize)
@@ -220,16 +221,15 @@
                     image = np.concatenate([image_padding, image], axis=0)
 
                 # padding on bottom side
                 if self.padding[3] > 0:
                     # get image size
                     ysize, xsize = image.shape[:2]
                     # convert percentage into pixel amount
-                    if self.padding[3] < 1:
-                        self.padding = list(self.padding)
+                    if self.padding[3] <= 1 and isinstance(self.padding[3], float):
                         self.padding[3] = int(self.padding[3] * ysize)
 
                     # different padding shape for grayscale and colored image
                     if len(image.shape) > 2:
                         padding_shape = (self.padding[3], xsize, image.shape[2])
                     else:
                         padding_shape = (self.padding[3], xsize)
@@ -240,30 +240,34 @@
                         image_padding = np.flipud(image[-self.padding[3] :, :].copy())
                     else:
                         image_padding = np.full(padding_shape, fill_value=self.padding_value, dtype="uint8")
                     # combine padding image and original image
                     image = np.concatenate([image, image_padding], axis=0)
 
             # resize based on scale
+            # remove negative value (if any)
+            self.scale = list(self.scale)
+            self.scale[0] = abs(self.scale[0])
+            self.scale[1] = abs(self.scale[1])
             if self.scale[1] != 1 and self.scale[0] != 1:
                 scale = random.uniform(self.scale[0], self.scale[1])
                 if scale > 0:
                     new_width = int(image.shape[1] * scale)
                     new_height = int(image.shape[0] * scale)
                     new_size = (new_width, new_height)
                     image = cv2.resize(image, new_size, interpolation=cv2.INTER_AREA)
 
             # translate image based on translation value
             if self.translation[0] != 0 or self.translation[1] != 0:
 
                 ysize, xsize = image.shape[:2]
-                if self.translation[0] < 1 and self.translation[0] > -1:
+                if self.translation[0] <= 1 and self.translation[0] >= -1 and isinstance(self.translation[0], float):
                     self.translation = list(self.translation)
                     self.translation[0] = int(self.translation[0] * xsize)
-                if self.translation[1] < 1 and self.translation[1] > -1:
+                if self.translation[1] <= 1 and self.translation[1] >= -1 and isinstance(self.translation[1], float):
                     self.translation = list(self.translation)
                     self.translation[1] = int(self.translation[1] * ysize)
 
                 image_new = np.full_like(image, fill_value=255).astype("uint8")
                 offset_x = self.translation[0]
                 offset_y = self.translation[1]
```

### Comparing `augraphy-8.2.1/augraphy/augmentations/inkbleed.py` & `augraphy-8.2.2/augraphy/augmentations/inkbleed.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/jpeg.py` & `augraphy-8.2.2/augraphy/augmentations/jpeg.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/letterpress.py` & `augraphy-8.2.2/augraphy/augmentations/letterpress.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/lib.py` & `augraphy-8.2.2/augraphy/augmentations/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
         grayscale = image
 
     # if return grayscale image if threshold method is grayscale
     if threshold_method == "grayscale":
         return grayscale
 
     if threshold_arguments:
-        # get input arguments for threhold function
+        # get input arguments for threshold function
         input_arguments = ""
         for input_argument in threshold_arguments:
             # for string argument value
             if isinstance(threshold_arguments[input_argument], str):
                 input_value = threshold_arguments[input_argument]
             # for non-string argument value
             else:
```

### Comparing `augraphy-8.2.1/augraphy/augmentations/lightinggradient.py` & `augraphy-8.2.2/augraphy/augmentations/lightinggradient.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/lowinkline.py` & `augraphy-8.2.2/augraphy/augmentations/lowinkline.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/lowinkperiodiclines.py` & `augraphy-8.2.2/augraphy/augmentations/lowinkperiodiclines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/lowinkrandomlines.py` & `augraphy-8.2.2/augraphy/augmentations/lowinkrandomlines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/markup.py` & `augraphy-8.2.2/augraphy/augmentations/markup.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/noisetexturize.py` & `augraphy-8.2.2/augraphy/augmentations/noisetexturize.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/pageborder.py` & `augraphy-8.2.2/augraphy/augmentations/pageborder.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             height, width = image.shape[:2]
 
             noise_intensity = random.uniform(
                 self.noise_intensity_range[0],
                 self.noise_intensity_range[1],
             )
 
-            if self.width_range[0] < 1:
+            if self.width_range[0] > 0 and self.width_range[0] <= 1 and isinstance(self.width_range[0], float):
                 self.width_range = list(self.width_range)
                 self.width_range[0] = np.ceil(self.width_range[0] * min(height, width))
                 self.width_range[1] = np.ceil(self.width_range[1] * min(height, width))
             border_width = random.randint(self.width_range[0], self.width_range[1])
 
             if len(image.shape) > 2:
                 channel = image.shape[2]
@@ -348,28 +348,26 @@
                 border_image = np.full_like(image, fill_value=255)
 
             if side == "left":
                 if self.flip_border:
                     border = np.flipud(border)
                 if self.same_page_border:
                     border_y, border_x = border.shape[:2]
-                    border_image = np.full_like(image, fill_value=255)
                     border_image[:, :border_x] = border
                 else:
                     image_output = np.hstack((border, image))
 
             elif side == "right":
                 border = np.fliplr(border)
                 if self.flip_border:
                     border = np.flipud(border)
 
                 if self.same_page_border:
-
                     border_y, border_x = border.shape[:2]
-                    border_image[-border_y:, -border_x:] = border
+                    border_image[:, -border_x:] = border
                 else:
                     image_output = np.hstack((image, border))
 
             elif side == "top":
                 border = cv2.rotate(border, cv2.ROTATE_90_CLOCKWISE)
                 if self.flip_border:
                     border = np.fliplr(border)
```

### Comparing `augraphy-8.2.1/augraphy/augmentations/subtlenoise.py` & `augraphy-8.2.2/augraphy/augmentations/subtlenoise.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/augmentations/watermark.py` & `augraphy-8.2.2/augraphy/augmentations/watermark.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/augmentation.py` & `augraphy-8.2.2/augraphy/base/augmentation.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/augmentationpipeline.py` & `augraphy-8.2.2/augraphy/base/augmentationpipeline.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/augmentationresult.py` & `augraphy-8.2.2/augraphy/base/augmentationresult.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/augmentationsequence.py` & `augraphy-8.2.2/augraphy/base/augmentationsequence.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/oneof.py` & `augraphy-8.2.2/augraphy/base/oneof.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/base/paperfactory.py` & `augraphy-8.2.2/augraphy/base/paperfactory.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/default/pipeline.py` & `augraphy-8.2.2/augraphy/default/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -187,20 +187,25 @@
             markup_thickness_range=(1, 2),
             markup_type=random.choice(["strikethrough", "crossed", "highlight", "underline"]),
             markup_color="random",
             single_word_mode=False,
             repetitions=1,
             p=0.33,
         ),
-        PencilScribbles(
-            size_range=(100, 800),
-            count_range=(1, 6),
-            stroke_count_range=(1, 2),
-            thickness_range=(2, 6),
-            brightness_change=random.randint(64, 224),
+        Scribbles(
+            scribbles_type="random",
+            scribbles_location="random",
+            scribbles_size_range=(250, 600),
+            scribbles_count_range=(1, 6),
+            scribbles_thickness_range=(1, 3),
+            scribbles_brightness_change=[32, 64, 128],
+            scribbles_text="random",
+            scribbles_text_font="random",
+            scribbles_text_rotate_range=(0, 360),
+            scribbles_lines_stroke_count_range=(1, 6),
             p=0.33,
         ),
         BadPhotoCopy(
             mask=None,
             noise_type=-1,
             noise_side="random",
             noise_iteration=(1, 2),
@@ -271,15 +276,15 @@
     return default_pipeline.augment(img)
 
 
 def pipeline_archetype1():
 
     ink_phase = [
         Geometric(
-            padding=(0, 0, 0.05, 0),
+            padding=[0, 0, 0.05, 0],
             randomize=0,
         ),
         BindingsAndFasteners(
             overlay_types="darken",
             effect_type="punch_holes",
             ntimes=(3, 3),
             nscales=(1.0, 1.0),
@@ -298,14 +303,27 @@
         PageBorder(
             side="right",
             border_background_value=(0, 0),
             pages=1,
             width_range=(2, 3),
             same_page_border=0,
         ),
+        Scribbles(
+            scribbles_type="text",
+            scribbles_ink="pen",
+            scribbles_location=(0.9, 0.75),
+            scribbles_size_range=(700, 700),
+            scribbles_count_range=(1, 1),
+            scribbles_thickness_range=(1, 1),
+            scribbles_brightness_change=[96],
+            scribbles_color=(0, 0, 0),
+            scribbles_text="600",
+            scribbles_text_font="random",
+            scribbles_text_rotate_range=(30, 30),
+        ),
         Geometric(
             translation=(-0.1, 0.2),
             randomize=0,
         ),
         Geometric(
             translation=(0, -0.05),
             randomize=0,
@@ -334,14 +352,28 @@
             n_samples=(1000, 1000),
             n_clusters=(500, 500),
             std_range=(400, 400),
             value_range=(200, 255),
             value_threshold_range=(255, 255),
             blur=0,
         ),
+        Scribbles(
+            scribbles_type="text",
+            scribbles_ink="pencil",
+            scribbles_location=(0.5, 0.95),
+            scribbles_size_range=(700, 700),
+            scribbles_count_range=(1, 1),
+            scribbles_thickness_range=(1, 1),
+            scribbles_brightness_change=[0],
+            scribbles_color=(0, 0, 0),
+            scribbles_text="P·142",
+            scribbles_text_font="random",
+            scribbles_text_rotate_range=(3, 3),
+            scribbles_pencil_skeletonize=0,
+        ),
         BadPhotoCopy(
             noise_type=1,
             noise_side="bottom",
             noise_iteration=(1, 1),
             noise_size=(5, 7),
             noise_value=(0, 64),
             noise_sparsity=(0.01, 0.01),
@@ -440,30 +472,34 @@
             noise_value=(0, 15),
             noise_sparsity=(0.025, 0.025),
             noise_concentration=(0.015, 0.015),
             wave_pattern=0,
             edge_effect=0,
         ),
         Geometric(rotate_range=(2, 2), randomize=0),
-        Geometric(padding=(0.1, 0.2, 0.2, 0.05), randomize=0),
+        Geometric(padding=[0.1, 0.2, 0.2, 0.05], randomize=0),
         BadPhotoCopy(
             noise_type=2,
             noise_side="left",
             noise_value=(0, 15),
             noise_sparsity=(0.025, 0.025),
             noise_concentration=(0.025, 0.025),
             wave_pattern=0,
             edge_effect=0,
         ),
-        PencilScribbles(
-            size_range=(200, 300),
-            count_range=(2, 2),
-            stroke_count_range=(1, 1),
-            thickness_range=(2, 6),
-            brightness_change=128,
+        Scribbles(
+            scribbles_type="lines",
+            scribbles_ink="pencil",
+            scribbles_location="random",
+            scribbles_size_range=(200, 300),
+            scribbles_count_range=(2, 2),
+            scribbles_thickness_range=(2, 6),
+            scribbles_brightness_change=[64, 128],
+            scribbles_color=(0, 0, 0),
+            scribbles_lines_stroke_count_range=(1, 1),
         ),
         BindingsAndFasteners(
             foreground=None,
             overlay_types="darken",
             effect_type="clips",
             ntimes=(3, 3),
             nscales=(1, 1),
@@ -503,15 +539,15 @@
             noise_side="right",
             noise_value=(0, 15),
             noise_sparsity=(0.025, 0.025),
             noise_concentration=(0.015, 0.015),
             wave_pattern=0,
             edge_effect=0,
         ),
-        Geometric(padding=(0.01, 0.01, 0.01, 0), randomize=0),
+        Geometric(padding=[0.01, 0.01, 0.01, 0], randomize=0),
     ]
 
     pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
 
     return pipeline
 
 
@@ -646,19 +682,19 @@
         Faxify(
             monochrome=1,
             monochrome_method="threshold_otsu",
             halftone=0,
         ),
         Geometric(
             rotate_range=(-1, -1),
-            padding=(0, 0.05, 0, 0),
+            padding=[0, 0.05, 0, 0],
             randomize=0,
         ),
         Geometric(
-            crop=(0, 0.02, 1, 0.99),
+            crop=(0.0, 0.02, 1.0, 0.99),
             randomize=0,
         ),
         BadPhotoCopy(
             noise_type=4,
             noise_side="random",
             noise_iteration=(2, 3),
             noise_size=(5, 7),
@@ -700,14 +736,27 @@
         ),
         InkBleed(
             intensity_range=(0.3, 0.4),
             color_range=(0, 0),
             kernel_size=(3, 3),
             severity=(1.0, 1.0),
         ),
+        Scribbles(
+            scribbles_type="text",
+            scribbles_ink="pen",
+            scribbles_location=(0.8, 0.8),
+            scribbles_size_range=(650, 650),
+            scribbles_count_range=(1, 1),
+            scribbles_thickness_range=(2, 2),
+            scribbles_brightness_change=[0],
+            scribbles_color=(0, 0, 0),
+            scribbles_text="Dr Architg \n \n  Dr Lynn added that \n me to Dereene etan \n with you . He feel that \n we should stay away \n from the mystery that could \n help to .FTC on  \n In attend the president \n of the committee \n       Cloude ",
+            scribbles_text_font="https://www.fontsquirrel.com/fonts/download/Windsong",
+            scribbles_text_rotate_range=(15, 15),
+        ),
         BadPhotoCopy(
             noise_type=2,
             noise_side="right",
             noise_iteration=(30, 30),
             noise_size=(1, 4),
             noise_value=(0, 1),
             noise_sparsity=(0.7, 0.7),
@@ -726,15 +775,15 @@
             noise_sparsity=(0.1, 0.1),
             noise_concentration=(0.01, 0.01),
             blur_noise=0,
             blur_noise_kernel=(5, 5),
             wave_pattern=0,
             edge_effect=1,
         ),
-        Geometric(randomize=0, padding=(0, 0.02, 0, 0)),
+        Geometric(randomize=0, padding=[0, 0.02, 0, 0]),
     ]
 
     paper_phase = [
         PageBorder(
             side="right",
             noise_intensity_range=(0.5, 0.8),
             width_range=(4, 5),
@@ -772,14 +821,235 @@
     ]
 
     pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
 
     return pipeline
 
 
+def pipeline_archetype6():
+
+    ink_phase = [
+        Markup(
+            num_lines_range=(2, 2),
+            markup_length_range=(0.4, 0.4),
+            markup_thickness_range=(2, 3),
+            markup_type="strikethrough",
+            markup_color=(0, 0, 0),
+            single_word_mode=False,
+            large_word_mode=False,
+        ),
+    ]
+    paper_phase = [
+        PageBorder(
+            side="bottom",
+            width_range=(2, 2),
+            pages=1,
+            noise_intensity_range=(0.0, 0.0),
+        ),
+        Letterpress(
+            n_samples=(200, 300),
+            n_clusters=(500, 680),
+            std_range=(500, 500),
+            value_range=(245, 255),
+            value_threshold_range=(128, 128),
+            blur=0,
+        ),
+        Geometric(translation=(0, -0.05), randomize=0),
+    ]
+    post_phase = [
+        Dithering(dither="ordered", order=(4, 4)),
+        InkBleed(
+            intensity_range=(0.1, 0.2),
+            color_range=(0, 0),
+            kernel_size=(3, 3),
+            severity=(0.2, 0.2),
+        ),
+        Geometric(rotate_range=(-1, -1), randomize=0),
+        Faxify(
+            monochrome=1,
+            monochrome_method="threshold_otsu",
+            halftone=0,
+        ),
+        BadPhotoCopy(
+            noise_type=4,
+            noise_side="random",
+            noise_iteration=(4, 5),
+            noise_size=(1, 4),
+            noise_value=(0, 0),
+            noise_sparsity=(0.5, 0.6),
+            noise_concentration=(0.5, 0.5),
+            blur_noise=0,
+            wave_pattern=0,
+            edge_effect=0,
+        ),
+    ]
+
+    pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
+
+    return pipeline
+
+
+def pipeline_archetype7():
+
+    ink_phase = [
+        InkBleed(
+            intensity_range=(0.6, 0.6),
+            color_range=(0, 0),
+            kernel_size=(3, 3),
+            severity=(0.8, 0.8),
+        ),
+        BadPhotoCopy(
+            noise_type=3,
+            noise_side="top",
+            noise_iteration=(4, 5),
+            noise_size=(2, 4),
+            noise_value=(0, 5),
+            noise_sparsity=(0.025, 0.025),
+            noise_concentration=(0.05, 0.05),
+            blur_noise=0,
+            edge_effect=0,
+            wave_pattern=0,
+        ),
+        Geometric(padding=[0, 0, 0, 0.025], randomize=0),
+    ]
+    paper_phase = [
+        BadPhotoCopy(
+            noise_type=1,
+            noise_side="top",
+            noise_iteration=(4, 5),
+            noise_size=(4, 8),
+            noise_value=(0, 5),
+            noise_sparsity=(0.015, 0.015),
+            noise_concentration=(0.05, 0.05),
+            blur_noise=0,
+            edge_effect=0,
+            wave_pattern=0,
+        ),
+        Geometric(translation=(0, 0.97), randomize=0),
+    ]
+    post_phase = [
+        BadPhotoCopy(
+            noise_type=4,
+            noise_side="random",
+            noise_iteration=(6, 8),
+            noise_size=(1, 7),
+            noise_value=(0, 0),
+            noise_sparsity=(0.5, 0.6),
+            noise_concentration=(0.5, 0.5),
+            blur_noise=0,
+            wave_pattern=0,
+            edge_effect=0,
+        ),
+        Geometric(rotate_range=(1, 1), randomize=0),
+        Faxify(
+            monochrome=1,
+            monochrome_method="threshold_otsu",
+            halftone=0,
+        ),
+    ]
+
+    pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
+
+    return pipeline
+
+
+def pipeline_archetype8():
+
+    ink_phase = [
+        Scribbles(
+            scribbles_type="text",
+            scribbles_ink="pen",
+            scribbles_location=(0.7, 0.01),
+            scribbles_size_range=(300, 300),
+            scribbles_count_range=(1, 1),
+            scribbles_thickness_range=(1, 1),
+            scribbles_brightness_change=[32],
+            scribbles_color=(0, 0, 0),
+            scribbles_text="-~ ETS  Literature",
+            scribbles_text_font="random",
+            scribbles_text_rotate_range=(0, 0),
+        ),
+        BadPhotoCopy(
+            noise_type=1,
+            noise_side="left",
+            noise_iteration=(4, 5),
+            noise_size=(1, 8),
+            noise_value=(0, 5),
+            noise_sparsity=(0.005, 0.005),
+            noise_concentration=(0.1, 0.1),
+            blur_noise=0,
+            edge_effect=0,
+            wave_pattern=0,
+        ),
+        BookBinding(
+            radius_range=(10, 10),
+            curve_range=(100, 100),
+            mirror_range=(0.2, 0.2),
+            curling_direction=0,
+        ),
+        Geometric(crop=(0.0, 0.0, 1.0, 0.85), randomize=0),
+    ]
+
+    paper_phase = [
+        BadPhotoCopy(
+            noise_type=1,
+            noise_side="right",
+            noise_iteration=(4, 5),
+            noise_size=(1, 2),
+            noise_value=(0, 5),
+            noise_sparsity=(0.005, 0.005),
+            noise_concentration=(0.1, 0.1),
+            blur_noise=0,
+            edge_effect=0,
+            wave_pattern=0,
+        ),
+        Geometric(translation=(-0.05, 0), randomize=0),
+        BadPhotoCopy(
+            noise_type=1,
+            noise_side="right",
+            noise_iteration=(4, 5),
+            noise_size=(1, 2),
+            noise_value=(0, 5),
+            noise_sparsity=(0.005, 0.005),
+            noise_concentration=(0.1, 0.1),
+            blur_noise=0,
+            edge_effect=0,
+            wave_pattern=0,
+        ),
+        Geometric(translation=(-0.9, 0), randomize=0),
+    ]
+
+    post_phase = [
+        PageBorder(
+            side="right",
+            border_background_value=(230, 255),
+            flip_border=random.choice([0, 1]),
+            width_range=(1, 2),
+            pages=None,
+            noise_intensity_range=(0.3, 0.8),
+            curve_frequency=(2, 8),
+            curve_height=(2, 4),
+            curve_length_one_side=(50, 100),
+            value=(250, 255),
+            same_page_border=random.choice([0, 1]),
+        ),
+        Geometric(padding=[0, 0, 0.05, 0], padding_value=0, randomize=0),
+        Geometric(padding=[0, 0.1, 0, 0.1], padding_value=255, randomize=0),
+        Faxify(
+            monochrome=1,
+            monochrome_method="threshold_otsu",
+            halftone=0,
+        ),
+    ]
+
+    pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
+
+    return pipeline
+
+
 def pipeline_archetype9():
 
     ink_phase = [
         Letterpress(
             n_samples=(200, 300),
             n_clusters=(500, 680),
             std_range=(2500, 2500),
@@ -837,7 +1107,45 @@
     post_phase = [
         Geometric(rotate_range=(-1, -1), randomize=0),
     ]
 
     pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
 
     return pipeline
+
+
+def pipeline_archetype10():
+
+    ink_phase = [
+        BadPhotoCopy(
+            noise_type=4,
+            noise_side="random",
+            noise_iteration=(6, 8),
+            noise_size=(1, 7),
+            noise_value=(0, 0),
+            noise_sparsity=(0.5, 0.6),
+            noise_concentration=(0.2, 0.2),
+            blur_noise=0,
+            wave_pattern=0,
+            edge_effect=0,
+        ),
+        Letterpress(
+            n_samples=(200, 300),
+            n_clusters=(500, 680),
+            std_range=(2500, 2500),
+            value_range=(245, 255),
+            value_threshold_range=(128, 128),
+            blur=1,
+        ),
+    ]
+    paper_phase = []
+    post_phase = [
+        Faxify(
+            monochrome=1,
+            monochrome_method="threshold_otsu",
+            halftone=0,
+        ),
+    ]
+
+    pipeline = AugraphyPipeline(ink_phase, paper_phase, post_phase)
+
+    return pipeline
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `augraphy-8.2.1/augraphy/utilities/composepipelines.py` & `augraphy-8.2.2/augraphy/utilities/composepipelines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/figsharedownloader.py` & `augraphy-8.2.2/augraphy/utilities/figsharedownloader.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/function.py` & `augraphy-8.2.2/augraphy/utilities/function.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/imageoverlay.py` & `augraphy-8.2.2/augraphy/utilities/imageoverlay.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/interop.py` & `augraphy-8.2.2/augraphy/utilities/interop.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/noisegenerator.py` & `augraphy-8.2.2/augraphy/utilities/noisegenerator.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy/utilities/overlaybuilder.py` & `augraphy-8.2.2/augraphy/utilities/overlaybuilder.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.1/augraphy.egg-info/PKG-INFO` & `augraphy-8.2.2/augraphy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: augraphy
-Version: 8.2.1
+Version: 8.2.2
 Summary: Augmentation pipeline for rendering synthetic paper printing and scanning processes
 Home-page: https://github.com/sparkfish/augraphy
 Author: Sparkfish LLC
 Author-email: packages@sparkfish.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sparkfish/augraphy/issues
 Description: <p align="center">
-            <img src="images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/logo/augraphy.png?raw=true" width="600" title="Augraphy Logo">
         </p>
         
         Augraphy is a Python library that creates multiple copies of original documents though an augmentation pipeline that randomly distorts each copy -- degrading the clean version into dirty and realistic copies rendered through synthetic paper printing, faxing, scanning and copy machine processes.
         
         Highly-configurable pipelines apply adjustments to the originals to create realistic old or noisy documents by acting as a factory, producing almost an infinite number of variations from their source.  This simulation of realistic paper-oriented process distortions can create large amounts of training data for AI/ML processes to learn how to remove those distortions.
         
         Treatments applied by Augraphy fabricate realistic documents that appear to have been printed on dirty laser or inkjet printers, scanned by dirty office scanners, faxed by low-resolution fax machines and otherwise mistreated by real-world paper handling office equipment.
@@ -32,19 +32,19 @@
         A paper factory provides either a white page or a randomly-selected paper texture base.  Like the ink layer, the paper can also be processed through a pipeline to further provide random realistic paper textures.
         
         After both the ink and paper phases are completed, processing continues by applying the ink, with its desired effects, to the paper.  This merged document image is then augmented further with distortions such as adding folds or other physical deformations or distortions that rely on simultaneous interactions of paper and ink layers.
         
         The end result is an image that mimics real documents.
         
         <p align="center" width="100%">
-            <img src="images/Pipeline.png">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
         </p>
         
         ## Example Before / After Images
-        ![examples](https://user-images.githubusercontent.com/74747193/135170284-8249fbab-2748-4230-821c-e56815e797cf.png)
+        ![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
         
         
         # Example Usage
         To use the default pipeline which contains all available augmentations and sensible defaults:
         
         ```python
         from augraphy import *
@@ -88,14 +88,17 @@
         |LowInkRandomLines   |            71.05|            12.74|
         |Markup              |             0.71|           533.16|
         |NoiseTexturize      |             0.53|           249.36|
         |PageBorder          |             0.52|           465.19|
         |PencilScribbles     |             1.15|           138.13|
         |SubtleNoise         |             1.03|           202.87|
         |WaterMark           |             1.19|           373.41|
+        |VoronoiTessellation |             0.47|            15.90|
+        |DelaunayTessellation|             0.76|            36.33|
+        |Quasi Crystals      |             0.25|              7.5|
         
         # Alternative Augmentation Libraries
         There are plenty of choices when it comes to [augmentation libraries](https://github.com/AgaMiko/data-augmentation-review).  However, only Augraphy is designed to address everyday office automation needs associated with paper-oriented process distortions that come from printing, faxing, scanning and copy machines.  Most other libraries focus on video and images pertinent to camera-oriented data sources and problem domains.  Augraphy is focused on supporting problems related to automation of document images such as OCR, form recognition, form data extraction, document classification, barcode decoding, denoising, document restoration, identity document data extraction, document cropping, etc.  Eventually, Augraphy will be able to support photo OCR problems with augmentations designed to emulate camera phone distortions.
         
         # Contributing
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
@@ -104,15 +107,15 @@
         
         BibTeX:
         ```
         @software{augraphy_library,
             author = {The Augraphy Project},
             title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
             url = {https://github.com/sparkfish/augraphy},
-            version = {8.2.1}
+            version = {8.2.2}
         }
         ```
         
         # License
         Copyright 2023 Sparkfish LLC
         
         Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.1/augraphy.egg-info/SOURCES.txt` & `augraphy-8.2.2/augraphy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,38 @@
 augraphy/augmentations/badphotocopy.py
 augraphy/augmentations/bindingsandfasteners.py
 augraphy/augmentations/bleedthrough.py
 augraphy/augmentations/bookbinding.py
 augraphy/augmentations/brightness.py
 augraphy/augmentations/brightnesstexturize.py
 augraphy/augmentations/colorpaper.py
+augraphy/augmentations/delaunay.py
 augraphy/augmentations/dirtydrum.py
 augraphy/augmentations/dirtyrollers.py
 augraphy/augmentations/dithering.py
 augraphy/augmentations/faxify.py
 augraphy/augmentations/folding.py
 augraphy/augmentations/gamma.py
 augraphy/augmentations/geometric.py
 augraphy/augmentations/inkbleed.py
 augraphy/augmentations/jpeg.py
 augraphy/augmentations/letterpress.py
 augraphy/augmentations/lib.py
 augraphy/augmentations/lightinggradient.py
+augraphy/augmentations/linesdegradation.py
 augraphy/augmentations/lowinkline.py
 augraphy/augmentations/lowinkperiodiclines.py
 augraphy/augmentations/lowinkrandomlines.py
 augraphy/augmentations/markup.py
 augraphy/augmentations/noisetexturize.py
 augraphy/augmentations/pageborder.py
-augraphy/augmentations/pencilscribbles.py
+augraphy/augmentations/quasicrystal.py
+augraphy/augmentations/scribbles.py
 augraphy/augmentations/subtlenoise.py
+augraphy/augmentations/voronoi.py
 augraphy/augmentations/watermark.py
 augraphy/base/__init__.py
 augraphy/base/augmentation.py
 augraphy/base/augmentationpipeline.py
 augraphy/base/augmentationresult.py
 augraphy/base/augmentationsequence.py
 augraphy/base/oneof.py
@@ -48,9 +52,11 @@
 augraphy/default/pipeline.py
 augraphy/utilities/__init__.py
 augraphy/utilities/composepipelines.py
 augraphy/utilities/figsharedownloader.py
 augraphy/utilities/function.py
 augraphy/utilities/imageoverlay.py
 augraphy/utilities/interop.py
+augraphy/utilities/meshgenerator.py
 augraphy/utilities/noisegenerator.py
-augraphy/utilities/overlaybuilder.py
+augraphy/utilities/overlaybuilder.py
+augraphy/utilities/slidingwindow.py
```

### Comparing `augraphy-8.2.1/setup.py` & `augraphy-8.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     install_requires=[
-        "numba",
+        "matplotlib >= 3.4.3",
+        "numba >= 0.54.1",
         "numpy >= 1.20.1",
         "opencv-python >= 4.5.1.48",
-        "scikit-learn >= 0.0",
+        "Pillow >= 8.0.0",
+        "requests >= 2.25.1",
+        "scikit-image >= 0.18.1",
+        "scikit-learn >= 0.23.2",
         "scipy >= 1.6.3",
     ],
 )
```

