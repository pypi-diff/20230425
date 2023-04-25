# Comparing `tmp/mammopy-0.0.5.tar.gz` & `tmp/mammopy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammopy-0.0.5.tar", max compression
+gzip compressed data, was "mammopy-0.0.6.tar", max compression
```

## Comparing `mammopy-0.0.5.tar` & `mammopy-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,197 @@
--rw-r--r--   0        0        0       47 2023-04-25 07:36:09.842549 mammopy-0.0.5/mammopy/__init__.py
--rw-r--r--   0        0        0     9407 2023-04-25 07:35:58.442312 mammopy-0.0.5/mammopy/mammopy.py
--rw-r--r--   0        0        0      589 2023-04-25 07:38:05.781009 mammopy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1540 2023-04-25 07:38:47.273277 mammopy-0.0.5/README.md
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 mammopy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-04-25 08:46:42.222903 mammopy-0.0.6/mammopy/__init__.py
+-rw-r--r--   0        0        0     9407 2023-04-25 08:57:54.514381 mammopy-0.0.6/mammopy/mammopy.py
+-rw-r--r--   0        0        0      267 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__init__.py
+-rw-r--r--   0        0        0      298 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      284 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      347 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      298 2023-04-25 08:12:43.909066 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      296 2023-03-22 11:45:31.970280 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__version__.cpython-36.pyc
+-rw-r--r--   0        0        0      232 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__version__.cpython-37.pyc
+-rw-r--r--   0        0        0      250 2023-04-25 08:12:45.279552 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__version__.cpython-38.pyc
+-rw-r--r--   0        0        0      248 2023-03-22 11:45:33.085944 mammopy-0.0.6/mammopy/segmentation_models/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0        0        0       66 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/__version__.py
+-rw-r--r--   0        0        0      148 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__init__.py
+-rw-r--r--   0        0        0      330 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      304 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      312 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      330 2023-04-25 08:12:43.927739 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      328 2023-03-22 11:45:31.983165 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      881 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/heads.cpython-310.pyc
+-rw-r--r--   0        0        0      845 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/heads.cpython-36.pyc
+-rw-r--r--   0        0        0      855 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/heads.cpython-37.pyc
+-rw-r--r--   0        0        0      879 2023-04-25 08:12:43.958739 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/heads.cpython-38.pyc
+-rw-r--r--   0        0        0      877 2023-03-22 11:45:31.997169 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/heads.cpython-39.pyc
+-rw-r--r--   0        0        0      940 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc
+-rw-r--r--   0        0        0      919 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc
+-rw-r--r--   0        0        0      930 2023-04-25 08:12:43.939737 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc
+-rw-r--r--   0        0        0      928 2023-03-22 11:45:31.990419 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc
+-rw-r--r--   0        0        0     1630 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     1558 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     1566 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     1599 2023-04-25 08:12:43.931739 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     1618 2023-03-22 11:45:31.987385 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3963 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/modules.cpython-310.pyc
+-rw-r--r--   0        0        0     4162 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/modules.cpython-36.pyc
+-rw-r--r--   0        0        0     4024 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/modules.cpython-37.pyc
+-rw-r--r--   0        0        0     3979 2023-04-25 08:12:43.949740 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/modules.cpython-38.pyc
+-rw-r--r--   0        0        0     4003 2023-03-22 11:45:31.993781 mammopy-0.0.6/mammopy/segmentation_models/base/__pycache__/modules.cpython-39.pyc
+-rw-r--r--   0        0        0      532 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/heads.py
+-rw-r--r--   0        0        0      848 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/initialization.py
+-rw-r--r--   0        0        0     1294 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/model.py
+-rw-r--r--   0        0        0     3561 2023-03-15 07:44:18.000000 mammopy-0.0.6/mammopy/segmentation_models/base/modules.py
+-rw-r--r--   0        0        0     2341 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__init__.py
+-rw-r--r--   0        0        0     2219 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2165 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     2179 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2213 2023-04-25 08:12:43.961742 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2219 2023-03-22 11:45:32.000169 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1813 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1768 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc
+-rw-r--r--   0        0        0     1778 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc
+-rw-r--r--   0        0        0     1814 2023-04-25 08:12:44.602047 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc
+-rw-r--r--   0        0        0     1812 2023-03-22 11:45:32.684714 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc
+-rw-r--r--   0        0        0      546 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc
+-rw-r--r--   0        0        0      576 2023-04-25 08:12:45.212550 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc
+-rw-r--r--   0        0        0      568 2023-03-22 11:45:33.060100 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc
+-rw-r--r--   0        0        0     1399 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1374 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc
+-rw-r--r--   0        0        0     1361 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc
+-rw-r--r--   0        0        0     1385 2023-04-25 08:12:44.613052 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1385 2023-03-22 11:45:32.686716 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc
+-rw-r--r--   0        0        0     4766 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc
+-rw-r--r--   0        0        0     4828 2023-04-25 08:12:44.655048 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc
+-rw-r--r--   0        0        0     4830 2023-03-22 11:45:32.699122 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc
+-rw-r--r--   0        0        0     4420 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc
+-rw-r--r--   0        0        0     4606 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc
+-rw-r--r--   0        0        0     4347 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc
+-rw-r--r--   0        0        0     4405 2023-04-25 08:12:44.624100 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc
+-rw-r--r--   0        0        0     4411 2023-03-22 11:45:32.691122 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc
+-rw-r--r--   0        0        0     4660 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     4924 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     4670 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     4646 2023-04-25 08:12:44.685048 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4656 2023-03-22 11:45:32.707477 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3782 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc
+-rw-r--r--   0        0        0     3733 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc
+-rw-r--r--   0        0        0     3769 2023-04-25 08:12:44.664048 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc
+-rw-r--r--   0        0        0     3775 2023-03-22 11:45:32.701816 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc
+-rw-r--r--   0        0        0     3662 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc
+-rw-r--r--   0        0        0     3663 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc
+-rw-r--r--   0        0        0     3611 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc
+-rw-r--r--   0        0        0     3649 2023-04-25 08:12:44.675049 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc
+-rw-r--r--   0        0        0     3655 2023-03-22 11:45:32.704271 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc
+-rw-r--r--   0        0        0     3227 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc
+-rw-r--r--   0        0        0     3190 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc
+-rw-r--r--   0        0        0     3170 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc
+-rw-r--r--   0        0        0     3214 2023-04-25 08:12:44.698094 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc
+-rw-r--r--   0        0        0     3218 2023-03-22 11:45:32.713478 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc
+-rw-r--r--   0        0        0     6363 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc
+-rw-r--r--   0        0        0     6535 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc
+-rw-r--r--   0        0        0     6227 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc
+-rw-r--r--   0        0        0     6321 2023-04-25 08:12:43.973129 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     6352 2023-03-22 11:45:32.004166 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3893 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc
+-rw-r--r--   0        0        0     3961 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc
+-rw-r--r--   0        0        0     3808 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc
+-rw-r--r--   0        0        0     3866 2023-04-25 08:12:44.644048 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc
+-rw-r--r--   0        0        0     3884 2023-03-22 11:45:32.696123 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     5949 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     5609 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     5707 2023-04-25 08:12:44.719133 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     5711 2023-03-22 11:45:32.719478 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     4260 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc
+-rw-r--r--   0        0        0     4204 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc
+-rw-r--r--   0        0        0     3990 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc
+-rw-r--r--   0        0        0     4052 2023-04-25 08:12:44.634047 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc
+-rw-r--r--   0        0        0     4258 2023-03-22 11:45:32.693124 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc
+-rw-r--r--   0        0        0     2200 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc
+-rw-r--r--   0        0        0     2191 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc
+-rw-r--r--   0        0        0     2154 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc
+-rw-r--r--   0        0        0     2206 2023-04-25 08:12:44.708776 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-03-22 11:45:32.715477 mammopy-0.0.6/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc
+-rw-r--r--   0        0        0     1372 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/_base.py
+-rw-r--r--   0        0        0      476 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/_preprocessing.py
+-rw-r--r--   0        0        0     1565 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/_utils.py
+-rw-r--r--   0        0        0     5317 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/densenet.py
+-rw-r--r--   0        0        0     6009 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/dpn.py
+-rw-r--r--   0        0        0     6470 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/efficientnet.py
+-rw-r--r--   0        0        0     3551 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/inceptionresnetv2.py
+-rw-r--r--   0        0        0     3544 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/inceptionv4.py
+-rw-r--r--   0        0        0     2933 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/mobilenet.py
+-rw-r--r--   0        0        0     9265 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/resnet.py
+-rw-r--r--   0        0        0     5849 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/senet.py
+-rw-r--r--   0        0        0     9053 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/timm_efficientnet.py
+-rw-r--r--   0        0        0     5637 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/vgg.py
+-rw-r--r--   0        0        0     1979 2023-03-15 07:44:20.000000 mammopy-0.0.6/mammopy/segmentation_models/encoders/xception.py
+-rw-r--r--   0        0        0       23 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__init__.py
+-rw-r--r--   0        0        0      209 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      191 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      209 2023-04-25 08:12:43.911859 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      207 2023-03-22 11:45:31.973166 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3090 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc
+-rw-r--r--   0        0        0     3032 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc
+-rw-r--r--   0        0        0     3043 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc
+-rw-r--r--   0        0        0     3070 2023-04-25 08:12:43.925737 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc
+-rw-r--r--   0        0        0     3066 2023-03-22 11:45:31.980558 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc
+-rw-r--r--   0        0        0     3874 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     3787 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     3760 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     3818 2023-04-25 08:12:43.914740 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     3816 2023-03-22 11:45:31.976868 mammopy-0.0.6/mammopy/segmentation_models/unet/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3862 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/decoder.py
+-rw-r--r--   0        0        0     4306 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/unet/model.py
+-rw-r--r--   0        0        0       64 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      247 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      265 2023-04-25 08:12:45.215555 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      263 2023-03-22 11:45:33.063104 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3523 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3565 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0        0        0     3575 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0        0        0     3613 2023-04-25 08:12:45.253548 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     3611 2023-03-22 11:45:33.076361 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     4638 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc
+-rw-r--r--   0        0        0     5047 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc
+-rw-r--r--   0        0        0     4680 2023-04-25 08:12:45.264554 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc
+-rw-r--r--   0        0        0     4668 2023-03-22 11:45:33.080398 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc
+-rw-r--r--   0        0        0     4132 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc
+-rw-r--r--   0        0        0     4323 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc
+-rw-r--r--   0        0        0     4320 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc
+-rw-r--r--   0        0        0     4199 2023-04-25 08:12:45.244551 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc
+-rw-r--r--   0        0        0     4207 2023-03-22 11:45:33.073360 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc
+-rw-r--r--   0        0        0     2280 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc
+-rw-r--r--   0        0        0     2234 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc
+-rw-r--r--   0        0        0     2242 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc
+-rw-r--r--   0        0        0     2282 2023-04-25 08:12:45.234549 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc
+-rw-r--r--   0        0        0     2280 2023-03-22 11:45:33.070365 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     3367 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc
+-rw-r--r--   0        0        0     3375 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc
+-rw-r--r--   0        0        0     3131 2023-04-25 08:12:45.276549 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     3139 2023-03-22 11:45:33.083399 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0        0        0     5903 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/train.cpython-310.pyc
+-rw-r--r--   0        0        0     5989 2023-03-15 07:44:24.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/train.cpython-36.pyc
+-rw-r--r--   0        0        0     5988 2023-03-15 07:44:24.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/train.cpython-37.pyc
+-rw-r--r--   0        0        0     5960 2023-04-25 08:12:45.225902 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/train.cpython-38.pyc
+-rw-r--r--   0        0        0     5984 2023-03-22 11:45:33.067362 mammopy-0.0.6/mammopy/segmentation_models/utils/__pycache__/train.cpython-39.pyc
+-rw-r--r--   0        0        0     2513 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/base.py
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/functional.py
+-rw-r--r--   0        0        0     3475 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/losses.py
+-rw-r--r--   0        0        0     1719 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/meter.py
+-rw-r--r--   0        0        0     3026 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/metrics.py
+-rw-r--r--   0        0        0     6382 2023-03-15 07:44:22.000000 mammopy-0.0.6/mammopy/segmentation_models/utils/train.py
+-rw-r--r--   0        0        0      589 2023-04-25 08:58:46.462135 mammopy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1540 2023-04-25 07:38:47.273277 mammopy-0.0.6/README.md
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 mammopy-0.0.6/PKG-INFO
```

### Comparing `mammopy-0.0.5/mammopy/mammopy.py` & `mammopy-0.0.6/mammopy/mammopy.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.5/pyproject.toml` & `mammopy-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mammopy"
-version = "0.0.5"
+version = "0.0.6"
 description = "A unified solution for mammogram image analysis and interpretation"
 authors = ["UEF Cancer <uef.cancergroup@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `mammopy-0.0.5/README.md` & `mammopy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.5/PKG-INFO` & `mammopy-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mammopy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A unified solution for mammogram image analysis and interpretation
 Author: UEF Cancer
 Author-email: uef.cancergroup@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

