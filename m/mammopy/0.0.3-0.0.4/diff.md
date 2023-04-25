# Comparing `tmp/mammopy-0.0.3.tar.gz` & `tmp/mammopy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammopy-0.0.3.tar", max compression
+gzip compressed data, was "mammopy-0.0.4.tar", max compression
```

## Comparing `mammopy-0.0.3.tar` & `mammopy-0.0.4.tar`

### file list

```diff
@@ -1,197 +1,198 @@
--rw-r--r--   0        0        0       47 2023-04-24 11:29:48.761366 mammopy-0.0.3/MammoPy/__init__.py
--rw-r--r--   0        0        0     9407 2023-04-24 11:27:42.702682 mammopy-0.0.3/MammoPy/mammopy.py
--rw-r--r--   0        0        0      267 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__init__.py
--rw-r--r--   0        0        0      298 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      284 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      347 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      300 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      296 2023-03-22 11:45:31.970280 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0        0        0      239 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__version__.cpython-36.pyc
--rw-r--r--   0        0        0      232 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__version__.cpython-37.pyc
--rw-r--r--   0        0        0      252 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__version__.cpython-38.pyc
--rw-r--r--   0        0        0      248 2023-03-22 11:45:33.085944 mammopy-0.0.3/MammoPy/segmentation_models/__pycache__/__version__.cpython-39.pyc
--rw-r--r--   0        0        0       66 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/__version__.py
--rw-r--r--   0        0        0      148 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__init__.py
--rw-r--r--   0        0        0      330 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      304 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      312 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      332 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      328 2023-03-22 11:45:31.983165 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      881 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-310.pyc
--rw-r--r--   0        0        0      845 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-36.pyc
--rw-r--r--   0        0        0      855 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-37.pyc
--rw-r--r--   0        0        0      881 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-38.pyc
--rw-r--r--   0        0        0      877 2023-03-22 11:45:31.997169 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-39.pyc
--rw-r--r--   0        0        0      940 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc
--rw-r--r--   0        0        0      909 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc
--rw-r--r--   0        0        0      919 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc
--rw-r--r--   0        0        0      932 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc
--rw-r--r--   0        0        0      928 2023-03-22 11:45:31.990419 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc
--rw-r--r--   0        0        0     1630 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     1558 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-36.pyc
--rw-r--r--   0        0        0     1566 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-37.pyc
--rw-r--r--   0        0        0     1601 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-38.pyc
--rw-r--r--   0        0        0     1618 2023-03-22 11:45:31.987385 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     3963 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-310.pyc
--rw-r--r--   0        0        0     4162 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-36.pyc
--rw-r--r--   0        0        0     4024 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-37.pyc
--rw-r--r--   0        0        0     3981 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-38.pyc
--rw-r--r--   0        0        0     4003 2023-03-22 11:45:31.993781 mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-39.pyc
--rw-r--r--   0        0        0      532 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/heads.py
--rw-r--r--   0        0        0      848 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/initialization.py
--rw-r--r--   0        0        0     1294 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/model.py
--rw-r--r--   0        0        0     3561 2023-03-15 07:44:18.000000 mammopy-0.0.3/MammoPy/segmentation_models/base/modules.py
--rw-r--r--   0        0        0     2341 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__init__.py
--rw-r--r--   0        0        0     2219 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2165 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0     2179 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2215 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2219 2023-03-22 11:45:32.000169 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1813 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0     1768 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc
--rw-r--r--   0        0        0     1778 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc
--rw-r--r--   0        0        0     1816 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc
--rw-r--r--   0        0        0     1812 2023-03-22 11:45:32.684714 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc
--rw-r--r--   0        0        0      572 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc
--rw-r--r--   0        0        0      546 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc
--rw-r--r--   0        0        0      578 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc
--rw-r--r--   0        0        0      568 2023-03-22 11:45:33.060100 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc
--rw-r--r--   0        0        0     1399 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1374 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc
--rw-r--r--   0        0        0     1361 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc
--rw-r--r--   0        0        0     1387 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1385 2023-03-22 11:45:32.686716 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc
--rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc
--rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc
--rw-r--r--   0        0        0     4766 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc
--rw-r--r--   0        0        0     4830 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc
--rw-r--r--   0        0        0     4830 2023-03-22 11:45:32.699122 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc
--rw-r--r--   0        0        0     4420 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc
--rw-r--r--   0        0        0     4606 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc
--rw-r--r--   0        0        0     4347 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc
--rw-r--r--   0        0        0     4407 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc
--rw-r--r--   0        0        0     4411 2023-03-22 11:45:32.691122 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc
--rw-r--r--   0        0        0     4660 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc
--rw-r--r--   0        0        0     4924 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc
--rw-r--r--   0        0        0     4670 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc
--rw-r--r--   0        0        0     4648 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc
--rw-r--r--   0        0        0     4656 2023-03-22 11:45:32.707477 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc
--rw-r--r--   0        0        0     3782 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc
--rw-r--r--   0        0        0     3770 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc
--rw-r--r--   0        0        0     3733 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc
--rw-r--r--   0        0        0     3771 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc
--rw-r--r--   0        0        0     3775 2023-03-22 11:45:32.701816 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc
--rw-r--r--   0        0        0     3662 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc
--rw-r--r--   0        0        0     3663 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc
--rw-r--r--   0        0        0     3611 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc
--rw-r--r--   0        0        0     3651 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc
--rw-r--r--   0        0        0     3655 2023-03-22 11:45:32.704271 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc
--rw-r--r--   0        0        0     3227 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc
--rw-r--r--   0        0        0     3190 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc
--rw-r--r--   0        0        0     3170 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc
--rw-r--r--   0        0        0     3216 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc
--rw-r--r--   0        0        0     3218 2023-03-22 11:45:32.713478 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc
--rw-r--r--   0        0        0     6363 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc
--rw-r--r--   0        0        0     6535 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc
--rw-r--r--   0        0        0     6227 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc
--rw-r--r--   0        0        0     6323 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0     6352 2023-03-22 11:45:32.004166 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc
--rw-r--r--   0        0        0     3893 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc
--rw-r--r--   0        0        0     3961 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc
--rw-r--r--   0        0        0     3808 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc
--rw-r--r--   0        0        0     3868 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc
--rw-r--r--   0        0        0     3884 2023-03-22 11:45:32.696123 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc
--rw-r--r--   0        0        0     5720 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc
--rw-r--r--   0        0        0     5949 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc
--rw-r--r--   0        0        0     5609 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc
--rw-r--r--   0        0        0     5709 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc
--rw-r--r--   0        0        0     5711 2023-03-22 11:45:32.719478 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc
--rw-r--r--   0        0        0     4260 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc
--rw-r--r--   0        0        0     4204 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc
--rw-r--r--   0        0        0     3990 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc
--rw-r--r--   0        0        0     4054 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc
--rw-r--r--   0        0        0     4258 2023-03-22 11:45:32.693124 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc
--rw-r--r--   0        0        0     2200 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc
--rw-r--r--   0        0        0     2191 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc
--rw-r--r--   0        0        0     2154 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc
--rw-r--r--   0        0        0     2208 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-03-22 11:45:32.715477 mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc
--rw-r--r--   0        0        0     1372 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/_base.py
--rw-r--r--   0        0        0      476 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/_preprocessing.py
--rw-r--r--   0        0        0     1565 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/_utils.py
--rw-r--r--   0        0        0     5317 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/densenet.py
--rw-r--r--   0        0        0     6009 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/dpn.py
--rw-r--r--   0        0        0     6470 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/efficientnet.py
--rw-r--r--   0        0        0     3551 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/inceptionresnetv2.py
--rw-r--r--   0        0        0     3544 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/inceptionv4.py
--rw-r--r--   0        0        0     2933 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/mobilenet.py
--rw-r--r--   0        0        0     9265 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/resnet.py
--rw-r--r--   0        0        0     5849 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/senet.py
--rw-r--r--   0        0        0     9053 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/timm_efficientnet.py
--rw-r--r--   0        0        0     5637 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/vgg.py
--rw-r--r--   0        0        0     1979 2023-03-15 07:44:20.000000 mammopy-0.0.3/MammoPy/segmentation_models/encoders/xception.py
--rw-r--r--   0        0        0       23 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__init__.py
--rw-r--r--   0        0        0      209 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      183 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      191 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      211 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      207 2023-03-22 11:45:31.973166 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3090 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc
--rw-r--r--   0        0        0     3032 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc
--rw-r--r--   0        0        0     3043 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc
--rw-r--r--   0        0        0     3072 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc
--rw-r--r--   0        0        0     3066 2023-03-22 11:45:31.980558 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc
--rw-r--r--   0        0        0     3874 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     3787 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-36.pyc
--rw-r--r--   0        0        0     3760 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-37.pyc
--rw-r--r--   0        0        0     3820 2023-03-15 07:53:26.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-38.pyc
--rw-r--r--   0        0        0     3816 2023-03-22 11:45:31.976868 mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     3862 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/decoder.py
--rw-r--r--   0        0        0     4306 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/unet/model.py
--rw-r--r--   0        0        0       64 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      239 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      247 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      267 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      263 2023-03-22 11:45:33.063104 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3523 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3565 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-36.pyc
--rw-r--r--   0        0        0     3575 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-37.pyc
--rw-r--r--   0        0        0     3615 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     3611 2023-03-22 11:45:33.076361 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     4638 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc
--rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc
--rw-r--r--   0        0        0     5047 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc
--rw-r--r--   0        0        0     4682 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc
--rw-r--r--   0        0        0     4668 2023-03-22 11:45:33.080398 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc
--rw-r--r--   0        0        0     4132 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc
--rw-r--r--   0        0        0     4323 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc
--rw-r--r--   0        0        0     4320 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc
--rw-r--r--   0        0        0     4201 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc
--rw-r--r--   0        0        0     4207 2023-03-22 11:45:33.073360 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc
--rw-r--r--   0        0        0     2280 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc
--rw-r--r--   0        0        0     2234 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc
--rw-r--r--   0        0        0     2242 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc
--rw-r--r--   0        0        0     2284 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc
--rw-r--r--   0        0        0     2280 2023-03-22 11:45:33.070365 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc
--rw-r--r--   0        0        0     2874 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc
--rw-r--r--   0        0        0     3367 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc
--rw-r--r--   0        0        0     3375 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc
--rw-r--r--   0        0        0     3133 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc
--rw-r--r--   0        0        0     3139 2023-03-22 11:45:33.083399 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc
--rw-r--r--   0        0        0     5903 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-310.pyc
--rw-r--r--   0        0        0     5989 2023-03-15 07:44:24.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-36.pyc
--rw-r--r--   0        0        0     5988 2023-03-15 07:44:24.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-37.pyc
--rw-r--r--   0        0        0     5962 2023-03-15 07:53:28.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-38.pyc
--rw-r--r--   0        0        0     5984 2023-03-22 11:45:33.067362 mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-39.pyc
--rw-r--r--   0        0        0     2513 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/base.py
--rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/functional.py
--rw-r--r--   0        0        0     3475 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/losses.py
--rw-r--r--   0        0        0     1719 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/meter.py
--rw-r--r--   0        0        0     3026 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/metrics.py
--rw-r--r--   0        0        0     6382 2023-03-15 07:44:22.000000 mammopy-0.0.3/MammoPy/segmentation_models/utils/train.py
--rw-r--r--   0        0        0      590 2023-04-24 11:50:10.544937 mammopy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3974 2023-04-24 11:47:25.451011 mammopy-0.0.3/README.md
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 mammopy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-04-24 18:21:11.823077 mammopy-0.0.4/LICENSE
+-rw-r--r--   0        0        0       47 2023-04-24 11:29:48.761366 mammopy-0.0.4/MammoPy/__init__.py
+-rw-r--r--   0        0        0     9407 2023-04-24 11:27:42.702682 mammopy-0.0.4/MammoPy/mammopy.py
+-rw-r--r--   0        0        0      267 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__init__.py
+-rw-r--r--   0        0        0      298 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      284 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      347 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      300 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      296 2023-03-22 11:45:31.970280 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__version__.cpython-36.pyc
+-rw-r--r--   0        0        0      232 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__version__.cpython-37.pyc
+-rw-r--r--   0        0        0      252 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__version__.cpython-38.pyc
+-rw-r--r--   0        0        0      248 2023-03-22 11:45:33.085944 mammopy-0.0.4/MammoPy/segmentation_models/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0        0        0       66 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/__version__.py
+-rw-r--r--   0        0        0      148 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__init__.py
+-rw-r--r--   0        0        0      330 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      304 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      312 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      332 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      328 2023-03-22 11:45:31.983165 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      881 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-310.pyc
+-rw-r--r--   0        0        0      845 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-36.pyc
+-rw-r--r--   0        0        0      855 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-37.pyc
+-rw-r--r--   0        0        0      881 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-38.pyc
+-rw-r--r--   0        0        0      877 2023-03-22 11:45:31.997169 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-39.pyc
+-rw-r--r--   0        0        0      940 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc
+-rw-r--r--   0        0        0      919 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc
+-rw-r--r--   0        0        0      932 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc
+-rw-r--r--   0        0        0      928 2023-03-22 11:45:31.990419 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc
+-rw-r--r--   0        0        0     1630 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     1558 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     1566 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     1601 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     1618 2023-03-22 11:45:31.987385 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3963 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-310.pyc
+-rw-r--r--   0        0        0     4162 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-36.pyc
+-rw-r--r--   0        0        0     4024 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-37.pyc
+-rw-r--r--   0        0        0     3981 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-38.pyc
+-rw-r--r--   0        0        0     4003 2023-03-22 11:45:31.993781 mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-39.pyc
+-rw-r--r--   0        0        0      532 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/heads.py
+-rw-r--r--   0        0        0      848 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/initialization.py
+-rw-r--r--   0        0        0     1294 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/model.py
+-rw-r--r--   0        0        0     3561 2023-03-15 07:44:18.000000 mammopy-0.0.4/MammoPy/segmentation_models/base/modules.py
+-rw-r--r--   0        0        0     2341 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__init__.py
+-rw-r--r--   0        0        0     2219 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2165 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     2179 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2215 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2219 2023-03-22 11:45:32.000169 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1813 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1768 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc
+-rw-r--r--   0        0        0     1778 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc
+-rw-r--r--   0        0        0     1816 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc
+-rw-r--r--   0        0        0     1812 2023-03-22 11:45:32.684714 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc
+-rw-r--r--   0        0        0      546 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc
+-rw-r--r--   0        0        0      578 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc
+-rw-r--r--   0        0        0      568 2023-03-22 11:45:33.060100 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc
+-rw-r--r--   0        0        0     1399 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1374 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc
+-rw-r--r--   0        0        0     1361 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc
+-rw-r--r--   0        0        0     1387 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1385 2023-03-22 11:45:32.686716 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc
+-rw-r--r--   0        0        0     4766 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc
+-rw-r--r--   0        0        0     4830 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc
+-rw-r--r--   0        0        0     4830 2023-03-22 11:45:32.699122 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc
+-rw-r--r--   0        0        0     4420 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc
+-rw-r--r--   0        0        0     4606 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc
+-rw-r--r--   0        0        0     4347 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc
+-rw-r--r--   0        0        0     4407 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc
+-rw-r--r--   0        0        0     4411 2023-03-22 11:45:32.691122 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc
+-rw-r--r--   0        0        0     4660 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     4924 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     4670 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     4648 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4656 2023-03-22 11:45:32.707477 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3782 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc
+-rw-r--r--   0        0        0     3733 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc
+-rw-r--r--   0        0        0     3771 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc
+-rw-r--r--   0        0        0     3775 2023-03-22 11:45:32.701816 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc
+-rw-r--r--   0        0        0     3662 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc
+-rw-r--r--   0        0        0     3663 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc
+-rw-r--r--   0        0        0     3611 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc
+-rw-r--r--   0        0        0     3651 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc
+-rw-r--r--   0        0        0     3655 2023-03-22 11:45:32.704271 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc
+-rw-r--r--   0        0        0     3227 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc
+-rw-r--r--   0        0        0     3190 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc
+-rw-r--r--   0        0        0     3170 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc
+-rw-r--r--   0        0        0     3216 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc
+-rw-r--r--   0        0        0     3218 2023-03-22 11:45:32.713478 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc
+-rw-r--r--   0        0        0     6363 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc
+-rw-r--r--   0        0        0     6535 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc
+-rw-r--r--   0        0        0     6227 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc
+-rw-r--r--   0        0        0     6323 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     6352 2023-03-22 11:45:32.004166 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3893 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc
+-rw-r--r--   0        0        0     3961 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc
+-rw-r--r--   0        0        0     3808 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc
+-rw-r--r--   0        0        0     3868 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc
+-rw-r--r--   0        0        0     3884 2023-03-22 11:45:32.696123 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     5949 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     5609 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     5709 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     5711 2023-03-22 11:45:32.719478 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     4260 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc
+-rw-r--r--   0        0        0     4204 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc
+-rw-r--r--   0        0        0     3990 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc
+-rw-r--r--   0        0        0     4054 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc
+-rw-r--r--   0        0        0     4258 2023-03-22 11:45:32.693124 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc
+-rw-r--r--   0        0        0     2200 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc
+-rw-r--r--   0        0        0     2191 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc
+-rw-r--r--   0        0        0     2154 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc
+-rw-r--r--   0        0        0     2208 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-03-22 11:45:32.715477 mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc
+-rw-r--r--   0        0        0     1372 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/_base.py
+-rw-r--r--   0        0        0      476 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/_preprocessing.py
+-rw-r--r--   0        0        0     1565 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/_utils.py
+-rw-r--r--   0        0        0     5317 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/densenet.py
+-rw-r--r--   0        0        0     6009 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/dpn.py
+-rw-r--r--   0        0        0     6470 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/efficientnet.py
+-rw-r--r--   0        0        0     3551 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/inceptionresnetv2.py
+-rw-r--r--   0        0        0     3544 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/inceptionv4.py
+-rw-r--r--   0        0        0     2933 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/mobilenet.py
+-rw-r--r--   0        0        0     9265 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/resnet.py
+-rw-r--r--   0        0        0     5849 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/senet.py
+-rw-r--r--   0        0        0     9053 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/timm_efficientnet.py
+-rw-r--r--   0        0        0     5637 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/vgg.py
+-rw-r--r--   0        0        0     1979 2023-03-15 07:44:20.000000 mammopy-0.0.4/MammoPy/segmentation_models/encoders/xception.py
+-rw-r--r--   0        0        0       23 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__init__.py
+-rw-r--r--   0        0        0      209 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      191 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      211 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      207 2023-03-22 11:45:31.973166 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3090 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc
+-rw-r--r--   0        0        0     3032 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc
+-rw-r--r--   0        0        0     3043 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc
+-rw-r--r--   0        0        0     3072 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc
+-rw-r--r--   0        0        0     3066 2023-03-22 11:45:31.980558 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc
+-rw-r--r--   0        0        0     3874 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     3787 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     3760 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     3820 2023-03-15 07:53:26.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     3816 2023-03-22 11:45:31.976868 mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3862 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/decoder.py
+-rw-r--r--   0        0        0     4306 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/unet/model.py
+-rw-r--r--   0        0        0       64 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      247 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      267 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      263 2023-03-22 11:45:33.063104 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3523 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3565 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0        0        0     3575 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0        0        0     3615 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     3611 2023-03-22 11:45:33.076361 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     4638 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc
+-rw-r--r--   0        0        0     5047 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc
+-rw-r--r--   0        0        0     4682 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc
+-rw-r--r--   0        0        0     4668 2023-03-22 11:45:33.080398 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc
+-rw-r--r--   0        0        0     4132 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc
+-rw-r--r--   0        0        0     4323 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc
+-rw-r--r--   0        0        0     4320 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc
+-rw-r--r--   0        0        0     4201 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc
+-rw-r--r--   0        0        0     4207 2023-03-22 11:45:33.073360 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc
+-rw-r--r--   0        0        0     2280 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc
+-rw-r--r--   0        0        0     2234 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc
+-rw-r--r--   0        0        0     2242 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc
+-rw-r--r--   0        0        0     2284 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc
+-rw-r--r--   0        0        0     2280 2023-03-22 11:45:33.070365 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     3367 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc
+-rw-r--r--   0        0        0     3375 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc
+-rw-r--r--   0        0        0     3133 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     3139 2023-03-22 11:45:33.083399 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0        0        0     5903 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-310.pyc
+-rw-r--r--   0        0        0     5989 2023-03-15 07:44:24.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-36.pyc
+-rw-r--r--   0        0        0     5988 2023-03-15 07:44:24.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-37.pyc
+-rw-r--r--   0        0        0     5962 2023-03-15 07:53:28.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-38.pyc
+-rw-r--r--   0        0        0     5984 2023-03-22 11:45:33.067362 mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-39.pyc
+-rw-r--r--   0        0        0     2513 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/base.py
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/functional.py
+-rw-r--r--   0        0        0     3475 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/losses.py
+-rw-r--r--   0        0        0     1719 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/meter.py
+-rw-r--r--   0        0        0     3026 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/metrics.py
+-rw-r--r--   0        0        0     6382 2023-03-15 07:44:22.000000 mammopy-0.0.4/MammoPy/segmentation_models/utils/train.py
+-rw-r--r--   0        0        0      589 2023-04-25 06:47:37.532344 mammopy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3888 2023-04-24 18:21:11.825094 mammopy-0.0.4/README.md
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mammopy-0.0.4/PKG-INFO
```

### Comparing `mammopy-0.0.3/MammoPy/mammopy.py` & `mammopy-0.0.4/MammoPy/mammopy.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/heads.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/heads.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/model.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/__pycache__/modules.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/base/__pycache__/modules.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/heads.py` & `mammopy-0.0.4/MammoPy/segmentation_models/base/heads.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/initialization.py` & `mammopy-0.0.4/MammoPy/segmentation_models/base/initialization.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/model.py` & `mammopy-0.0.4/MammoPy/segmentation_models/base/model.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/base/modules.py` & `mammopy-0.0.4/MammoPy/segmentation_models/base/modules.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__init__.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/_base.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/_base.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/_utils.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/_utils.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/densenet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/densenet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/dpn.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/dpn.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/efficientnet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/efficientnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/inceptionresnetv2.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/inceptionv4.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/mobilenet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/mobilenet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/resnet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/senet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/senet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/timm_efficientnet.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/timm_efficientnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/vgg.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/vgg.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/encoders/xception.py` & `mammopy-0.0.4/MammoPy/segmentation_models/encoders/xception.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/__pycache__/model.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/decoder.py` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/decoder.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/unet/model.py` & `mammopy-0.0.4/MammoPy/segmentation_models/unet/model.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/base.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-310.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-36.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-37.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-38.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/__pycache__/train.cpython-39.pyc` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/__pycache__/train.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/base.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/base.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/functional.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/functional.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/losses.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/meter.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/meter.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/metrics.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/MammoPy/segmentation_models/utils/train.py` & `mammopy-0.0.4/MammoPy/segmentation_models/utils/train.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.3/pyproject.toml` & `mammopy-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "mammopy"
-version = "0.0.3"
+version = "0.0.4"
 description = "A unified solution for mammogram image analysis and interpretation"
 authors = ["UEF Cancer <uef.cancergroup@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "2.0.0"
 torchvision = "0.15.1"
 tqdm = "4.65.0"
 efficientnet_pytorch = "0.7.1"
-numpy = "1.24.2"
+numpy = "^1.18"
 Pillow = "9.5.0"
 pretrainedmodels = "0.7.4"
 pydicom = "2.3.1"
 requests = "2.28.2"
 timm = "0.6.12"
 scikit-image = "0.20.0"
```

### Comparing `mammopy-0.0.3/README.md` & `mammopy-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
   <img src="https://cdn.imgbin.com/10/3/23/imgbin-breast-cancer-senology-mammography-diego-JcEW147fdbivCyrvC5vykSPj3.jpg" height="200">
 </p>
 
 # MammoPy
 ### A Comprehensive Deep Learning Library for Mammogram Assessment
 [![PyPI version](https://badge.fury.io/py/mammopy.svg)](https://badge.fury.io/py/mammopy)
 ![GitHub](https://img.shields.io/github/license/mammopy/mammopy)
-[![Downloads](https://static.pepy.tech/badge/mammopy)](https://pepy.tech/project/mammopy)
 
 **[[Documentation]](https://github.com/uefcancer/mammopy/)**
 | **[[Paper]]()** 
 | **[[Notebook examples]]()** 
 | **[[Web applications]]()** 
 
 **Welcome to `MammoPy` Repository!** `MammoPy` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
@@ -77,22 +76,23 @@
 result['non_dense_area'] = 
 result['dense_area'] = 
 result['density']
 ```
 
 ## License
 
-The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
+The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/uefcancer/MammoPy/blob/main/LICENSE) for further details.
 
 If you use this library, please consider citing:
 ```
 @article{gudhe2022area,
   title={Area-based breast percentage density estimation in mammograms using weight-adaptive multitask learning},
   author={Gudhe, Naga Raju and Behravan, Hamid and Sudah, Mazen and Okuma, Hidemi and Vanninen, Ritva and Kosma, Veli-Matti and Mannermaa, Arto},
   journal={Scientific reports},
   volume={12},
   number={1},
   pages={12060},
   year={2022},
   publisher={Nature Publishing Group UK London}
 }
 ```
+
```

### Comparing `mammopy-0.0.3/PKG-INFO` & `mammopy-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mammopy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unified solution for mammogram image analysis and interpretation
 Author: UEF Cancer
 Author-email: uef.cancergroup@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (==9.5.0)
 Requires-Dist: efficientnet_pytorch (==0.7.1)
-Requires-Dist: numpy (==1.24.2)
+Requires-Dist: numpy (>=1.18,<2.0)
 Requires-Dist: pretrainedmodels (==0.7.4)
 Requires-Dist: pydicom (==2.3.1)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: scikit-image (==0.20.0)
 Requires-Dist: timm (==0.6.12)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: torchvision (==0.15.1)
@@ -27,15 +27,14 @@
   <img src="https://cdn.imgbin.com/10/3/23/imgbin-breast-cancer-senology-mammography-diego-JcEW147fdbivCyrvC5vykSPj3.jpg" height="200">
 </p>
 
 # MammoPy
 ### A Comprehensive Deep Learning Library for Mammogram Assessment
 [![PyPI version](https://badge.fury.io/py/mammopy.svg)](https://badge.fury.io/py/mammopy)
 ![GitHub](https://img.shields.io/github/license/mammopy/mammopy)
-[![Downloads](https://static.pepy.tech/badge/mammopy)](https://pepy.tech/project/mammopy)
 
 **[[Documentation]](https://github.com/uefcancer/mammopy/)**
 | **[[Paper]]()** 
 | **[[Notebook examples]]()** 
 | **[[Web applications]]()** 
 
 **Welcome to `MammoPy` Repository!** `MammoPy` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
@@ -102,15 +101,15 @@
 result['non_dense_area'] = 
 result['dense_area'] = 
 result['density']
 ```
 
 ## License
 
-The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
+The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/uefcancer/MammoPy/blob/main/LICENSE) for further details.
 
 If you use this library, please consider citing:
 ```
 @article{gudhe2022area,
   title={Area-based breast percentage density estimation in mammograms using weight-adaptive multitask learning},
   author={Gudhe, Naga Raju and Behravan, Hamid and Sudah, Mazen and Okuma, Hidemi and Vanninen, Ritva and Kosma, Veli-Matti and Mannermaa, Arto},
   journal={Scientific reports},
@@ -118,7 +117,8 @@
   number={1},
   pages={12060},
   year={2022},
   publisher={Nature Publishing Group UK London}
 }
 ```
 
+
```

