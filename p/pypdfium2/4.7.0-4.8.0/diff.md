# Comparing `tmp/pypdfium2-4.7.0.tar.gz` & `tmp/pypdfium2-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfium2-4.7.0.tar", last modified: Tue Apr 18 04:01:49 2023, max compression
+gzip compressed data, was "pypdfium2-4.8.0.tar", last modified: Tue Apr 25 04:02:15 2023, max compression
```

## Comparing `pypdfium2-4.7.0.tar` & `pypdfium2-4.8.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.832905 pypdfium2-4.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/.reuse/dep5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:01:49.832905 pypdfium2-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/setupsrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/autorelease.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11023 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/build_pdfium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/craft_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/packaging_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/setup_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/update_pdfium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/sourcebuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/sourcebuild/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/public_headers.patch
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/shared_library.patch
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/syslibs_sourcebuild.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/sourcebuild/patches/win/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/build.patch
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/pdfium.patch
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/resources.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.824905 pypdfium2-4.7.0/src/pypdfium2/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/arrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/extract_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/imgtopdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/pdfinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/toc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    27011 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/textpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 04:01:24.000000 pypdfium2-4.7.0/src/pypdfium2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.824905 pypdfium2-4.7.0/src/pypdfium2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/.reuse/dep5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/setupsrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/autorelease.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10887 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/build_pdfium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/craft_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/packaging_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/setup_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/update_pdfium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/sourcebuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/sourcebuild/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/public_headers.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/shared_library.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/sourcebuild/patches/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/build.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/pdfium.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/resources.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.767060 pypdfium2-4.8.0/src/pypdfium2/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.771060 pypdfium2-4.8.0/src/pypdfium2/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/arrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/extract_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/imgtopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/pdfinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.771060 pypdfium2-4.8.0/src/pypdfium2/_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26905 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/textpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 04:01:33.000000 pypdfium2-4.8.0/src/pypdfium2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.767060 pypdfium2-4.8.0/src/pypdfium2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/top_level.txt
```

### Comparing `pypdfium2-4.7.0/.reuse/dep5` & `pypdfium2-4.8.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/LICENSES/Apache-2.0.txt` & `pypdfium2-4.8.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/LICENSES/BSD-3-Clause.txt` & `pypdfium2-4.8.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/LICENSES/CC-BY-4.0.txt` & `pypdfium2-4.8.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/LICENSES/LicenseRef-PdfiumThirdParty.txt` & `pypdfium2-4.8.0/LICENSES/LicenseRef-PdfiumThirdParty.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/MANIFEST.in` & `pypdfium2-4.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/PKG-INFO` & `pypdfium2-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.7.0
+Version: 4.8.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
@@ -204,20 +204,20 @@
 
 * Include a JPEG image in a PDF
   ```python
   pdf = pdfium.PdfDocument.new()
   
   image = pdfium.PdfImage.new(pdf)
   image.load_jpeg("./tests/resources/mona_lisa.jpg")
-  metadata = image.get_metadata()
+  width, height = image.get_size()
   
-  matrix = pdfium.PdfMatrix().scale(metadata.width, metadata.height)
+  matrix = pdfium.PdfMatrix().scale(width, height)
   image.set_matrix(matrix)
   
-  page = pdf.new_page(metadata.width, metadata.height)
+  page = pdf.new_page(width, height)
   page.insert_obj(image)
   page.gen_content()
   ```
 
 * Save the document
   ```python
   # PDF 1.7 standard
@@ -265,16 +265,16 @@
 
 * While some functions are quite easy to use, things soon get more complex.
   First of all, function parameters are not only used for input, but also for output:
   ```python
   # Initialise an integer object (defaults to 0)
   c_version = ctypes.c_int()
   # Let the function assign a value to the c_int object, and capture its return code (True for success, False for failure)
-  success = pdfium.FPDF_GetFileVersion(pdf, c_version)
-  if success:
+  ok = pdfium.FPDF_GetFileVersion(pdf, c_version)
+  if ok:
       # If successful, get the Python int by accessing the `value` attribute of the c_int object
       version = c_version.value
   else:
       # Otherwise, set the variable to None (in other cases, it may be desired to raise an exception instead)
       version = None
   ```
```

### Comparing `pypdfium2-4.7.0/README.md` & `pypdfium2-4.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -177,20 +177,20 @@
 
 * Include a JPEG image in a PDF
   ```python
   pdf = pdfium.PdfDocument.new()
   
   image = pdfium.PdfImage.new(pdf)
   image.load_jpeg("./tests/resources/mona_lisa.jpg")
-  metadata = image.get_metadata()
+  width, height = image.get_size()
   
-  matrix = pdfium.PdfMatrix().scale(metadata.width, metadata.height)
+  matrix = pdfium.PdfMatrix().scale(width, height)
   image.set_matrix(matrix)
   
-  page = pdf.new_page(metadata.width, metadata.height)
+  page = pdf.new_page(width, height)
   page.insert_obj(image)
   page.gen_content()
   ```
 
 * Save the document
   ```python
   # PDF 1.7 standard
@@ -238,16 +238,16 @@
 
 * While some functions are quite easy to use, things soon get more complex.
   First of all, function parameters are not only used for input, but also for output:
   ```python
   # Initialise an integer object (defaults to 0)
   c_version = ctypes.c_int()
   # Let the function assign a value to the c_int object, and capture its return code (True for success, False for failure)
-  success = pdfium.FPDF_GetFileVersion(pdf, c_version)
-  if success:
+  ok = pdfium.FPDF_GetFileVersion(pdf, c_version)
+  if ok:
       # If successful, get the Python int by accessing the `value` attribute of the c_int object
       version = c_version.value
   else:
       # Otherwise, set the variable to None (in other cases, it may be desired to raise an exception instead)
       version = None
   ```
```

### Comparing `pypdfium2-4.7.0/pyproject.toml` & `pypdfium2-4.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/setup.py` & `pypdfium2-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/autorelease.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/autorelease.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/build_pdfium.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/build_pdfium.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     (PatchDir/"shared_library.patch", PDFiumDir),
     (PatchDir/"public_headers.patch", PDFiumDir),
 ]
 PatchesWindows = [
     (PatchDir/"win"/"pdfium.patch", PDFiumDir),
     (PatchDir/"win"/"build.patch", PDFiumDir/"build"),
 ]
-PatchesSyslibs = [
-    (PatchDir/"syslibs_sourcebuild.patch", PDFiumDir/"build")
-]
 
 DefaultConfig = {
     "is_debug": False,
     "treat_warnings_as_errors": False,
     # "clang_use_chrome_plugins": False,
     "pdf_is_standalone": True,
     "pdf_enable_v8": False,
@@ -58,20 +55,20 @@
     "use_system_freetype": True,
     "use_system_lcms2": True,
     "use_system_libjpeg": True,
     "use_system_libopenjpeg2": True,
     "use_system_libpng": True,
     "use_system_zlib": True,
     "use_system_libtiff": True,
-    "sysroot": "/",
 }
 
 
 if sys.platform.startswith("linux"):
     SyslibsConfig["use_custom_libcxx"] = False
+    SyslibsConfig["use_sysroot"] = False
 elif sys.platform.startswith("darwin"):
     DefaultConfig["mac_deployment_target"] = "10.13.0"
     SyslibsConfig["use_system_xcode"] = True
 
 
 def dl_depottools(do_update):
     
@@ -291,16 +288,15 @@
     Ninja   = get_tool("ninja")
     
     pdfium_dl_done = dl_pdfium(GClient, b_update, b_revision)
     v_libpdfium = get_pdfium_version()
     
     if pdfium_dl_done:
         patch_pdfium(v_libpdfium)
-    if b_use_syslibs:  # FIXME needs reset
-        _apply_patchset(PatchesSyslibs, check=False)
+    if b_use_syslibs:
         _dl_unbundler()
 
     if b_use_syslibs:
         run_cmd(["python3", "build/linux/unbundle/replace_gn_files.py", "--system-libraries", "icu"], cwd=PDFiumDir)
     
     config_dict = DefaultConfig.copy()
     if b_use_syslibs:
```

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/craft_packages.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/craft_packages.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/packaging_base.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/packaging_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     if pl_name == PlatformNames.darwin_x64:
         # pdfium-binaries/steps/05-configure.sh defines `mac_deployment_target = "10.13.0"`
         return "macosx_10_13_x86_64"
     elif pl_name == PlatformNames.darwin_arm64:
         # macOS 11 is the first version available on arm64
         return "macosx_11_0_arm64"
     # As of Jan 2023, pdfium requires glibc >= 2.26 (see https://crrev.com/1084974 and https://groups.google.com/a/chromium.org/g/chromium-dev/c/SdCs9k3celo/m/bnnBzU1FCgAJ)
-    # TODO lower requirements for older PDFium binaries?
+    # TODO? lower requirements for older PDFium binaries
     elif pl_name == PlatformNames.linux_x64:
         return "manylinux_2_26_x86_64"
     elif pl_name == PlatformNames.linux_x86:
         return "manylinux_2_26_i686"
     elif pl_name == PlatformNames.linux_arm64:
         return "manylinux_2_26_aarch64"
     elif pl_name == PlatformNames.linux_arm32:
```

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/setup_base.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/setup_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/update_pdfium.py` & `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/update_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/sourcebuild/patches/public_headers.patch` & `pypdfium2-4.8.0/sourcebuild/patches/public_headers.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/sourcebuild/patches/win/build.patch` & `pypdfium2-4.8.0/sourcebuild/patches/win/build.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/sourcebuild/patches/win/resources.rc` & `pypdfium2-4.8.0/sourcebuild/patches/win/resources.rc`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/__main__.py` & `pypdfium2-4.8.0/src/pypdfium2/__main__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/_parsers.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/_parsers.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/arrange.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/arrange.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/attachments.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/attachments.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/extract_images.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/extract_images.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/extract_text.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/extract_text.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/imgtopdf.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/imgtopdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,20 +52,17 @@
         else:
             pil_image = PIL.Image.open(fp)
             bitmap = pdfium.PdfBitmap.from_pil(pil_image)
             pil_image.close()
             image_obj.set_bitmap(bitmap)
             bitmap.close()
         
-        metadata = image_obj.get_metadata()
-        width, height = metadata.width, metadata.height
-        
-        image_obj.set_matrix( pdfium.PdfMatrix().scale(width, height) )
-        
-        page = pdf.new_page(width, height)
+        w, h = image_obj.get_size()
+        image_obj.set_matrix( pdfium.PdfMatrix().scale(w, h) )
+        page = pdf.new_page(w, h)
         page.insert_obj(image_obj)
         page.gen_content()
         
         image_obj.close()  # no-op
         page.close()
     
     if args.output.exists():
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/pageobjects.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/pageobjects.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
             pad_1 = pad_0 + "    "
             print(preamble + pad_0 + consts.ObjectTypeToStr.get(obj.type))
             
             if show_pos:
                 pos = round_list(obj.get_pos(), args.n_digits)
                 print(pad_1 + f"Position: {pos}")
             
+            # TODO? also call get_size() for coverage
             if show_imageinfo and isinstance(obj, pdfium.PdfImage):
                 print(pad_1 + f"Filters: {obj.get_filters()}")
                 metadata = obj.get_metadata()
                 print_img_metadata(metadata, pad=pad_1)
             
             count += 1
             preamble = ""
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/pdfinfo.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/pdfinfo.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/render.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/render.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/tile.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/tile.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_cli/toc.py` & `pypdfium2-4.8.0/src/pypdfium2/_cli/toc.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/__init__.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/bases.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/bases.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/consts.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     pdfium_c.FPDF_ERR_PAGE:     "Page not found or content error",
 })
 
 #: Convert a PDFium unsupported constant (:attr:`FPDF_UNSP_*`) to string.
 UnsupportedInfoToStr = _fallback_dict({
     pdfium_c.FPDF_UNSP_DOC_XFAFORM:               "XFA form",
     pdfium_c.FPDF_UNSP_DOC_PORTABLECOLLECTION:    "Portable collection",
-    pdfium_c.FPDF_UNSP_DOC_ATTACHMENT:            "Attachment",
+    pdfium_c.FPDF_UNSP_DOC_ATTACHMENT:            "Attachment (incomplete support)",  # https://crbug.com/pdfium/1945
     pdfium_c.FPDF_UNSP_DOC_SECURITY:              "Security",
     pdfium_c.FPDF_UNSP_DOC_SHAREDREVIEW:          "Shared review",
     pdfium_c.FPDF_UNSP_DOC_SHAREDFORM_ACROBAT:    "Shared form (acrobat)",
     pdfium_c.FPDF_UNSP_DOC_SHAREDFORM_FILESYSTEM: "Shared form (filesystem)",
     pdfium_c.FPDF_UNSP_DOC_SHAREDFORM_EMAIL:      "Shared form (email)",
     pdfium_c.FPDF_UNSP_ANNOT_3DANNOT:             "3D annotation",
     pdfium_c.FPDF_UNSP_ANNOT_MOVIE:               "Movie annotation",
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/utils.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/attachment.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/attachment.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         pdfium_c.FPDFAttachment_GetFile(self, None, 0, n_bytes)
         n_bytes = n_bytes.value
         if n_bytes == 0:
             raise PdfiumError(f"Failed to extract attachment (buffer length {n_bytes}).")
         
         buffer = ctypes.create_string_buffer(n_bytes)
         out_buflen = ctypes.c_ulong()
-        success = pdfium_c.FPDFAttachment_GetFile(self, buffer, n_bytes, out_buflen)
+        ok = pdfium_c.FPDFAttachment_GetFile(self, buffer, n_bytes, out_buflen)
         out_buflen = out_buflen.value
-        if not success:
+        if not ok:
             raise PdfiumError("Failed to extract attachment (error status).")
         if n_bytes < out_buflen:
             raise PdfiumError(f"Failed to extract attachment (expected {n_bytes} bytes, but got {out_buflen}).")
         
         return buffer
     
     
@@ -82,16 +82,16 @@
         If this function is called on an existing attachment, it will be changed to point at the new data,
         but the previous data will not be removed from the file (as of PDFium 5418).
         
         Parameters:
             data (bytes | ctypes.Array):
                 New file data for the attachment. May be any data type that can be implicitly converted to :class:`~ctypes.c_void_p`.
         """
-        success = pdfium_c.FPDFAttachment_SetFile(self, self.pdf, data, len(data))
-        if not success:
+        ok = pdfium_c.FPDFAttachment_SetFile(self, self.pdf, data, len(data))
+        if not ok:
             raise PdfiumError("Failed to set attachment data.")
     
     
     def has_key(self, key):
         """
         Parameters:
             key (str):
@@ -134,10 +134,10 @@
         Set the attribute specified by *key* to the string *value*.
         
         Parameters:
             value (str): New string value for the attribute.
         """
         enc_value = (value + "\x00").encode("utf-16-le")
         enc_value_ptr = ctypes.cast(enc_value, pdfium_c.FPDF_WIDESTRING)
-        success = pdfium_c.FPDFAttachment_SetStringValue(self, _encode_key(key), enc_value_ptr)
-        if not success:
+        ok = pdfium_c.FPDFAttachment_SetStringValue(self, _encode_key(key), enc_value_ptr)
+        if not ok:
             raise PdfiumError(f"Failed to set attachment param '{key}' to '{value}'.")
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/bitmap.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/bitmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,15 @@
     @classmethod
     def new_foreign(cls, width, height, format, rev_byteorder=False, force_packed=False):
         """
         Create a new bitmap using :func:`FPDFBitmap_CreateEx`, with a buffer allocated by PDFium.
         
         Using this method is discouraged. Prefer :meth:`.new_native` instead.
         """
-        
-        if force_packed:
-            stride = width * consts.BitmapTypeToNChannels[format]
-        else:
-            stride = 0
-        
+        stride = width * consts.BitmapTypeToNChannels[format] if force_packed else 0
         raw = pdfium_c.FPDFBitmap_CreateEx(width, height, format, None, stride)
         return cls.from_raw(raw, rev_byteorder)
     
     
     @classmethod
     def new_foreign_simple(cls, width, height, use_alpha, rev_byteorder=False):
         """
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/document.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,53 +159,53 @@
             config = pdfium_c.FPDF_FORMFILLINFO(version=2)
         raw = pdfium_c.FPDFDOC_InitFormFillEnvironment(self, config)
         if not raw:
             raise PdfiumError(f"Initializing form env failed for document {self}.")
         self.formenv = PdfFormEnv(raw, config, self)
     
     
-    # ?TODO(v5) consider cached property
+    # TODO?(v5) consider cached property
     def get_formtype(self):
         """
         Returns:
             int: PDFium form type that applies to the document (:attr:`FORMTYPE_*`).
             :attr:`FORMTYPE_NONE` if the document has no forms.
         """
         return pdfium_c.FPDF_GetFormType(self)
     
     
-    # ?TODO(v5) consider cached property
+    # TODO?(v5) consider cached property
     def get_pagemode(self):
         """
         Returns:
             int: Page displaying mode (:attr:`PAGEMODE_*`).
         """
         return pdfium_c.FPDFDoc_GetPageMode(self)
     
     
-    # ?TODO(v5) consider cached property
+    # TODO?(v5) consider cached property
     def is_tagged(self):
         """
         Returns:
             bool: Whether the document is tagged (cf. PDF 1.7, 10.7 "Tagged PDF").
         """
         return bool( pdfium_c.FPDFCatalog_IsTagged(self) )
     
     
     def _save_to(self, buffer, version=None, flags=pdfium_c.FPDF_NO_INCREMENTAL):
         
         c_writer = utils.get_bufwriter(buffer)
         saveargs = (self, c_writer, flags)
         
         if version is None:
-            success = pdfium_c.FPDF_SaveAsCopy(*saveargs)
+            ok = pdfium_c.FPDF_SaveAsCopy(*saveargs)
         else:
-            success = pdfium_c.FPDF_SaveWithVersion(*saveargs, version)
+            ok = pdfium_c.FPDF_SaveWithVersion(*saveargs, version)
         
-        if not success:
+        if not ok:
             raise PdfiumError("Failed to save document.")
     
     
     def save(self, dest, *args, **kwargs):
         """
         Save the document at its current state.
         
@@ -247,16 +247,16 @@
     def get_version(self):
         """
         Returns:
             int | None: The PDF version of the document (14 for 1.4, 15 for 1.5, ...),
             or None if the document is new or its version could not be determined.
         """
         version = ctypes.c_int()
-        success = pdfium_c.FPDF_GetFileVersion(self, version)
-        if not success:
+        ok = pdfium_c.FPDF_GetFileVersion(self, version)
+        if not ok:
             return None
         return version.value
     
     
     def get_metadata_value(self, key):
         """
         Returns:
@@ -331,16 +331,16 @@
         Unlink the attachment at *index* (zero-based).
         It will be hidden from the viewer, but is still present in the file (as of PDFium 5418).
         Following attachments shift one slot to the left in the array representation used by PDFium's API.
         
         Handles to the attachment in question received from :meth:`.get_attachment`
         must not be accessed anymore after this method has been called.
         """
-        success = pdfium_c.FPDFDoc_DeleteAttachment(self, index)
-        if not success:
+        ok = pdfium_c.FPDFDoc_DeleteAttachment(self, index)
+        if not ok:
             raise PdfiumError(f"Failed to delete attachment at index {index}.")
     
     
     # TODO deprecate in favour of index access?
     def get_page(self, index):
         """
         Returns:
@@ -405,35 +405,35 @@
                 Zero-based index at which to insert the given pages. If None, they are appended to the end of the document.
         """
         
         if index is None:
             index = len(self)
         
         if isinstance(pages, str):
-            success = pdfium_c.FPDF_ImportPages(self, pdf, pages.encode("ascii"), index)
+            ok = pdfium_c.FPDF_ImportPages(self, pdf, pages.encode("ascii"), index)
         else:
             page_count = 0
             c_pages = None
             if pages:
                 page_count = len(pages)
                 c_pages = (ctypes.c_int * page_count)(*pages)
-            success = pdfium_c.FPDF_ImportPagesByIndex(self, pdf, c_pages, page_count, index)
+            ok = pdfium_c.FPDF_ImportPagesByIndex(self, pdf, c_pages, page_count, index)
         
-        if not success:
+        if not ok:
             raise PdfiumError("Failed to import pages.")
     
     
     def get_page_size(self, index):
         """
         Returns:
             (float, float): Width and height in PDF canvas units of the page at *index* (zero-based).
         """
         size = pdfium_c.FS_SIZEF()
-        success = pdfium_c.FPDF_GetPageSizeByIndexF(self, index, size)
-        if not success:
+        ok = pdfium_c.FPDF_GetPageSizeByIndexF(self, index, size)
+        if not ok:
             raise PdfiumError("Failed to get page size by index.")
         return (size.width, size.height)
     
     
     def get_page_label(self, index):
         """
         Returns:
@@ -465,15 +465,16 @@
         
         return PdfXObject(
             raw = raw_xobject,
             pdf = dest_pdf,
         )
     
     
-    # TODO(v5) consider switching to a wrapper around the raw bookmark with on-demand cached properties
+    # TODO(v5) consider switching to a wrapper class around the raw bookmark
+    # (either with getter methods, or possibly cached properties)
     def _get_bookmark(self, bookmark, level):
         
         n_bytes = pdfium_c.FPDFBookmark_GetTitle(bookmark, None, 0)
         buffer = ctypes.create_string_buffer(n_bytes)
         pdfium_c.FPDFBookmark_GetTitle(bookmark, buffer, n_bytes)
         title = buffer.raw[:n_bytes-2].decode('utf-16-le')
         
@@ -551,31 +552,25 @@
     def _process_page(cls, index, input_data, password, renderer, converter, pass_info, need_formenv, mk_formconfig, **kwargs):
         
         pdf = cls(
             input_data,
             password = password,
         )
         if need_formenv:
-            if mk_formconfig:
-                pdf.init_forms(config=mk_formconfig())
-            else:
-                pdf.init_forms()
-        page = pdf[index]
+            pdf.init_forms(config=mk_formconfig()) if mk_formconfig else pdf.init_forms()
         
+        page = pdf[index]
         bitmap = renderer(page, **kwargs)
         info = bitmap.get_info()
         result = converter(bitmap)
         
         for g in (bitmap, page, pdf):
             g.close()
         
-        if pass_info:
-            return result, info
-        else:
-            return result
+        return (result, info) if pass_info else result
     
     
     def render(
             self,
             converter,
             renderer = PdfPage.render,
             page_indices = None,
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/matrix.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/matrix.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/page.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         Define the absolute, clockwise page rotation (0, 90, 180, or 270 degrees).
         """
         pdfium_c.FPDFPage_SetRotation(self, consts.RotationToConst[rotation])
     
     
     def _get_box(self, box_func, fallback_func, fallback_ok):
         left, bottom, right, top = c_float(), c_float(), c_float(), c_float()
-        success = box_func(self, left, bottom, right, top)
-        if not success:
+        ok = box_func(self, left, bottom, right, top)
+        if not ok:
             return (fallback_func() if fallback_ok else None)
         return (left.value, bottom.value, right.value, top.value)
     
     # NOTE in case further arguments are needed (besides fallback_ok), then use *args, **kwargs in callers
     
     def get_mediabox(self, fallback_ok=True):
         """
@@ -166,16 +166,16 @@
     
     def get_bbox(self):
         """
         Returns:
             The bounding box of the page (the intersection between its media box and crop box).
         """
         rect = pdfium_c.FS_RECTF()
-        success = pdfium_c.FPDF_GetPageBoundingBox(self, rect)
-        if not success:
+        ok = pdfium_c.FPDF_GetPageBoundingBox(self, rect)
+        if not ok:
             raise PdfiumError("Failed to get page bounding box.")
         return (rect.left, rect.bottom, rect.right, rect.top)
     
     
     # TODO add bindings to FPDFPage_TransFormWithClip()
     
     
@@ -234,16 +234,16 @@
     
     def gen_content(self):
         """
         Generate page content to apply additions, removals or modifications of page objects.
         
         If page content was changed, this function should be called once before saving the document or re-loading the page.
         """
-        success = pdfium_c.FPDFPage_GenerateContent(self)
-        if not success:
+        ok = pdfium_c.FPDFPage_GenerateContent(self)
+        if not ok:
             raise PdfiumError("Failed to generate page content.")
     
     
     def get_objects(self, filter=None, max_depth=2, form=None, level=0):
         """
         Iterate through the page objects on this page.
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/pageobjects.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/pageobjects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # SPDX-FileCopyrightText: 2023 geisserml <geisserml@gmail.com>
 # SPDX-License-Identifier: Apache-2.0 OR BSD-3-Clause
 
 __all__ = ["PdfObject", "PdfImage"]
 
 import ctypes
+from ctypes import c_uint, c_float
 from pathlib import Path
 from collections import namedtuple
 import pypdfium2.raw as pdfium_c
 from pypdfium2._helpers.misc import PdfiumError
 from pypdfium2._helpers.matrix import PdfMatrix
 from pypdfium2._helpers.bitmap import PdfBitmap
 from pypdfium2._helpers._internal import consts, utils
 from pypdfium2._helpers._internal.bases import AutoCloseable
 
 try:
     import PIL.Image
 except ImportError:
     PIL = None
 
-c_float = ctypes.c_float
-
 
 class PdfObject (AutoCloseable):
     """
     Page object helper class.
     
     When constructing a :class:`.PdfObject`, an instance of a more specific subclass may be returned instead,
     depending on the object's :attr:`.type` (e. g. :class:`.PdfImage`).
@@ -86,41 +85,41 @@
         
         Returns:
             A tuple of four :class:`float` coordinates for left, bottom, right, and top.
         """
         if self.page is None:
             raise RuntimeError("Must not call get_pos() on a loose pageobject.")
         
-        left, bottom, right, top = c_float(), c_float(), c_float(), c_float()
-        success = pdfium_c.FPDFPageObj_GetBounds(self, left, bottom, right, top)
-        if not success:
+        l, b, r, t = c_float(), c_float(), c_float(), c_float()
+        ok = pdfium_c.FPDFPageObj_GetBounds(self, l, b, r, t)
+        if not ok:
             raise PdfiumError("Failed to locate pageobject.")
         
-        return (left.value, bottom.value, right.value, top.value)
+        return (l.value, b.value, r.value, t.value)
     
     
     def get_matrix(self):
         """
         Returns:
             PdfMatrix: The pageobject's current transform matrix.
         """
         fs_matrix = pdfium_c.FS_MATRIX()
-        success = pdfium_c.FPDFPageObj_GetMatrix(self, fs_matrix)
-        if not success:
+        ok = pdfium_c.FPDFPageObj_GetMatrix(self, fs_matrix)
+        if not ok:
             raise PdfiumError("Failed to get matrix of pageobject.")
         return PdfMatrix.from_raw(fs_matrix)
     
     
     def set_matrix(self, matrix):
         """
         Parameters:
             matrix (PdfMatrix): Set this matrix as the pageobject's transform matrix.
         """
-        success = pdfium_c.FPDFPageObj_SetMatrix(self, matrix)
-        if not success:
+        ok = pdfium_c.FPDFPageObj_SetMatrix(self, matrix)
+        if not ok:
             raise PdfiumError("Failed to set matrix of pageobject.")
     
     
     def transform(self, matrix):
         """
         Parameters:
             matrix (PdfMatrix): Multiply the page object's current transform matrix by this matrix.
@@ -155,35 +154,47 @@
             page = None,
             pdf = pdf,
         )
     
     
     def get_metadata(self):
         """
-        Retrieve image metadata, including dimensions, DPI, bits per pixel, and color space.
+        Retrieve image metadata including DPI, bits per pixel, color space, and size.
         If the image does not belong to a page yet, bits per pixel and color space will be unset (0).
         
         Note:
             * The DPI values signify the resolution of the image on the PDF page, not the DPI metadata embedded in the image file.
-            * Due to issues in PDFium, this function can be inefficient.
+            * Due to issues in PDFium, this function can be slow. If you only need image size, prefer the faster :meth:`.get_size` instead.
         
         Returns:
             FPDF_IMAGEOBJ_METADATA: Image metadata structure
         """
-        
         # https://crbug.com/pdfium/1928
-        
         metadata = pdfium_c.FPDF_IMAGEOBJ_METADATA()
-        success = pdfium_c.FPDFImageObj_GetImageMetadata(self, self.page, metadata)
-        if not success:
+        ok = pdfium_c.FPDFImageObj_GetImageMetadata(self, self.page, metadata)
+        if not ok:
             raise PdfiumError("Failed to get image metadata.")
-        
         return metadata
     
     
+    def get_size(self):
+        """
+        .. versionadded:: 4.8/5731
+        
+        Returns:
+            (int, int): Image dimensions as a tuple of (width, height).
+        """
+        # https://pdfium-review.googlesource.com/c/pdfium/+/106290
+        w, h = c_uint(), c_uint()
+        ok = pdfium_c.FPDFImageObj_GetImagePixelSize(self, w, h)
+        if not ok:
+            raise PdfiumError("Failed to get image size.")
+        return w.value, h.value
+    
+    
     def load_jpeg(self, source, pages=None, inline=False, autoclose=True):
         """
         Set a JPEG as the image object's content.
         
         Parameters:
             source (str | pathlib.Path | typing.BinaryIO):
                 Input JPEG, given as file path or readable byte buffer.
@@ -203,23 +214,19 @@
             autoclose = True
         elif utils.is_buffer(source, "r"):
             buffer = source
         else:
             raise ValueError(f"Cannot load JPEG from {source} - not a file path or byte buffer.")
         
         bufaccess, ld_data = utils.get_bufreader(buffer)
-        
-        if inline:
-            loader = pdfium_c.FPDFImageObj_LoadJpegFileInline
-        else:
-            loader = pdfium_c.FPDFImageObj_LoadJpegFile
+        loader = pdfium_c.FPDFImageObj_LoadJpegFileInline if inline else pdfium_c.FPDFImageObj_LoadJpegFile
         
         c_pages, page_count = utils.pages_c_array(pages)
-        success = loader(c_pages, page_count, self, bufaccess)
-        if not success:
+        ok = loader(c_pages, page_count, self, bufaccess)
+        if not ok:
             raise PdfiumError("Failed to load JPEG into image object.")
         
         if inline:
             for data in ld_data:
                 id(data)
             if autoclose:
                 buffer.close()
@@ -237,16 +244,16 @@
         Parameters:
             bitmap (PdfBitmap):
                 The bitmap to inject into the image object.
             pages (list[PdfPage] | None):
                 A list of loaded pages that might contain the image object. See :meth:`.load_jpeg`.
         """
         c_pages, page_count = utils.pages_c_array(pages)
-        success = pdfium_c.FPDFImageObj_SetBitmap(c_pages, page_count, self, bitmap)
-        if not success:
+        ok = pdfium_c.FPDFImageObj_SetBitmap(c_pages, page_count, self, bitmap)
+        if not ok:
             raise PdfiumError("Failed to set image to bitmap.")
     
     
     def get_bitmap(self, render=False):
         """
         Get a bitmap rasterization of the image.
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/textpage.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/textpage.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Returns:
             str: The text in the range in question, or an empty string if no text was found.
         """
         
         if count == -1:
             count = self.count_chars() - index
         
-        # FIXME does not take possible unicode surrogation into account
+        # FIXME not sure if we may calculate buffer size like that - what about unicode surrogation, for one thing?
         n_bytes = count * 2
         buffer = ctypes.create_string_buffer(n_bytes+2)
         buffer_ptr = ctypes.cast(buffer, ctypes.POINTER(ctypes.c_ushort))
         
         pdfium_c.FPDFText_GetText(self, index, count, buffer_ptr)
         return buffer.raw[:n_bytes].decode("utf-16-le", errors=errors)
     
@@ -147,36 +147,40 @@
                 TODO
         Returns:
             Float values for left, bottom, right and top in PDF canvas units.
         """
         
         if loose:
             rect = pdfium_c.FS_RECTF()
-            success = pdfium_c.FPDFText_GetLooseCharBox(self, index, rect)
+            ok = pdfium_c.FPDFText_GetLooseCharBox(self, index, rect)
             l, b, r, t = rect.left, rect.bottom, rect.right, rect.top
         else:
             l, b, r, t = c_double(), c_double(), c_double(), c_double()
-            success = pdfium_c.FPDFText_GetCharBox(self, index, l, r, b, t)  # yes, lrbt!
+            ok = pdfium_c.FPDFText_GetCharBox(self, index, l, r, b, t)  # yes, lrbt!
             l, b, r, t = l.value, b.value, r.value, t.value
         
-        if not success:
+        if not ok:
             raise PdfiumError("Failed to get charbox.")
         
         return l, b, r, t
     
     
     def get_rect(self, index):
         """
         Get the bounding box of a text rectangle at the given index.
+        Note that :meth:`.count_rects` must be called once with default parameters
+        before subsequent :meth:`.get_rect` calls for this function to work (due to PDFium's API).
         
         Returns:
             Float values for left, bottom, right and top in PDF canvas units.
         """
         l, b, r, t = c_double(), c_double(), c_double(), c_double()
-        pdfium_c.FPDFText_GetRect(self, index, l, t, r, b)  # yes, ltrb!
+        ok = pdfium_c.FPDFText_GetRect(self, index, l, t, r, b)  # yes, ltrb!
+        if not ok:
+            raise PdfiumError("Failed to get rectangle. (Make sure count_rects() was called with default params once before subsequent get_rect() calls.)")
         return (l.value, b.value, r.value, t.value)
     
     
     def search(self, text, index=0, match_case=False, match_whole_word=False, consecutive=False):
         """
         Locate text on the page.
         
@@ -228,16 +232,16 @@
     
     @property
     def parent(self):  # AutoCloseable hook
         return self.textpage
     
     
     def _get_occurrence(self, find_func):
-        success = find_func(self)
-        if not success:
+        ok = find_func(self)
+        if not ok:
             return None
         index = pdfium_c.FPDFText_GetSchResultIndex(self)
         count = pdfium_c.FPDFText_GetSchCount(self)
         return index, count
     
     
     def get_next(self):
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/_helpers/unsupported.py` & `pypdfium2-4.8.0/src/pypdfium2/_helpers/unsupported.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,11 +52,8 @@
     def _keep(self):
         id(self.handlers)
         id(self._config)
     
     
     @staticmethod
     def _default(type):
-        # https://crbug.com/pdfium/1945
-        if type in (pdfium_c.FPDF_UNSP_DOC_ATTACHMENT, ):
-            return
         lib_logger.warning(f"Unsupported PDF feature: {consts.UnsupportedInfoToStr.get(type)}")
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2/version.py` & `pypdfium2-4.8.0/src/pypdfium2/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-FileCopyrightText: 2023 geisserml <geisserml@gmail.com>
 # SPDX-License-Identifier: Apache-2.0 OR BSD-3-Clause
 
 __all__ = ["V_PYPDFIUM2", "V_LIBPDFIUM", "V_BUILDNAME", "V_PDFIUM_IS_V8"]
 
 V_MAJOR = 4
-V_MINOR = 7
+V_MINOR = 8
 V_PATCH = 0
 V_BETA = None
 
 #: pypdfium2 version string
 V_PYPDFIUM2 = f"{V_MAJOR}.{V_MINOR}.{V_PATCH}"
 if V_BETA is not None:
     V_PYPDFIUM2 += f"b{V_BETA}"
 
 #: PDFium library version string (git tag or commit hash)
-V_LIBPDFIUM = "5715"
+V_LIBPDFIUM = "5731"
 
 #: String describing the included PDFium binary's origin (pdfium-binaries, source)
 V_BUILDNAME = "pdfium-binaries"
 
 #: Whether the included PDFium binary was built with V8 support or not
 V_PDFIUM_IS_V8 = False
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2.egg-info/PKG-INFO` & `pypdfium2-4.8.0/src/pypdfium2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.7.0
+Version: 4.8.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
@@ -204,20 +204,20 @@
 
 * Include a JPEG image in a PDF
   ```python
   pdf = pdfium.PdfDocument.new()
   
   image = pdfium.PdfImage.new(pdf)
   image.load_jpeg("./tests/resources/mona_lisa.jpg")
-  metadata = image.get_metadata()
+  width, height = image.get_size()
   
-  matrix = pdfium.PdfMatrix().scale(metadata.width, metadata.height)
+  matrix = pdfium.PdfMatrix().scale(width, height)
   image.set_matrix(matrix)
   
-  page = pdf.new_page(metadata.width, metadata.height)
+  page = pdf.new_page(width, height)
   page.insert_obj(image)
   page.gen_content()
   ```
 
 * Save the document
   ```python
   # PDF 1.7 standard
@@ -265,16 +265,16 @@
 
 * While some functions are quite easy to use, things soon get more complex.
   First of all, function parameters are not only used for input, but also for output:
   ```python
   # Initialise an integer object (defaults to 0)
   c_version = ctypes.c_int()
   # Let the function assign a value to the c_int object, and capture its return code (True for success, False for failure)
-  success = pdfium.FPDF_GetFileVersion(pdf, c_version)
-  if success:
+  ok = pdfium.FPDF_GetFileVersion(pdf, c_version)
+  if ok:
       # If successful, get the Python int by accessing the `value` attribute of the c_int object
       version = c_version.value
   else:
       # Otherwise, set the variable to None (in other cases, it may be desired to raise an exception instead)
       version = None
   ```
```

### Comparing `pypdfium2-4.7.0/src/pypdfium2.egg-info/SOURCES.txt` & `pypdfium2-4.8.0/src/pypdfium2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 setupsrc/pypdfium2_setup/build_pdfium.py
 setupsrc/pypdfium2_setup/craft_packages.py
 setupsrc/pypdfium2_setup/packaging_base.py
 setupsrc/pypdfium2_setup/setup_base.py
 setupsrc/pypdfium2_setup/update_pdfium.py
 sourcebuild/patches/public_headers.patch
 sourcebuild/patches/shared_library.patch
-sourcebuild/patches/syslibs_sourcebuild.patch
 sourcebuild/patches/win/build.patch
 sourcebuild/patches/win/pdfium.patch
 sourcebuild/patches/win/resources.rc
 src/pypdfium2/__init__.py
 src/pypdfium2/__main__.py
 src/pypdfium2/internal.py
 src/pypdfium2/version.py
```

