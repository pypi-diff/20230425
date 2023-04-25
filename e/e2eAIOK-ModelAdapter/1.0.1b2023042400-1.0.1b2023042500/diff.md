# Comparing `tmp/e2eAIOK-ModelAdapter-1.0.1b2023042400.tar.gz` & `tmp/e2eAIOK-ModelAdapter-1.0.1b2023042500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e2eAIOK-ModelAdapter-1.0.1b2023042400.tar", last modified: Mon Apr 24 00:21:58 2023, max compression
+gzip compressed data, was "dist/e2eAIOK-ModelAdapter-1.0.1b2023042500.tar", last modified: Tue Apr 25 00:48:09 2023, max compression
```

## Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400.tar` & `e2eAIOK-ModelAdapter-1.0.1b2023042500.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/office31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/default_ma.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/image_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/torch_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/extend_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-24 00:21:51.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 00:21:57.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:21:58.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-24 00:21:57.000000 e2eAIOK-ModelAdapter-1.0.1b2023042400/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-04-25 00:48:05.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/office31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/default_ma.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/torch_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/extend_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-25 00:48:06.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 00:48:08.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:48:09.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-25 00:48:08.000000 e2eAIOK-ModelAdapter-1.0.1b2023042500/setup.py
```

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/PKG-INFO` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK-ModelAdapter
-Version: 1.0.1b2023042400
+Version: 1.0.1b2023042500
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
         
@@ -74,21 +74,21 @@
         git submodule update --init --recursive
         python scripts/start_e2eaiok_docker.py --backend [tensorflow, pytorch, pytorch112] --dataset_path ../ --workers host1, host2, host3, host4 --proxy "http://addr:ip"
         ```
         
         ## Demos
         
         * Built-in Models
-          * [DLRM](modelzoo/dlrm/README.md) - RecSys, PyTorch
-          * [DIEN](modelzoo/dien/README.md) - RecSys, TensorFlow
-          * [WND](modelzoo/WnD/README.md) - RecSys, TensorFlow
-          * [RNNT](modelzoo/rnnt/README.md) - Speech Recognition, PyTorch
-          * [RESNET](modelzoo/resnet/README.md) - Computer vision, TensorFlow
-          * [BERT](modelzoo/bert/README.md) - Natual Language Processing, TensorFlow
-          * [MiniGo](modelzoo/minigo/README.md) - minimalist engine modeled after AlphaGo Zero, TensorFlow
+          * [DLRM](demo/builtin/dlrm/DLRM_DEMO.ipynb) - RecSys, PyTorch
+          * [DIEN](demo/builtin/dien/DIEN_DEMO.ipynb) - RecSys, TensorFlow
+          * [WND](demo/builtin/wnd/WND_DEMO.ipynb) - RecSys, TensorFlow
+          * [RNNT](demo/builtin/rnnt/RNNT_DEMO.ipynb) - Speech Recognition, PyTorch
+          * [RESNET](demo/builtin/resnet/RESNET_DEMO.ipynb) - Computer vision, TensorFlow
+          * [BERT](demo/builtin/bert/BERT_DEMO.ipynb) - Natual Language Processing, TensorFlow
+          * [MiniGo](demo/builtin/minigo/MiniGo_DEMO.ipynb) - minimalist engine modeled after AlphaGo Zero, TensorFlow
         
         * Neural network constructor 
         
           * DE-NAS demos:
             * [DE-NAS Overview](demo/denas/DENAS_SUMMARY.ipynb) 
               * [CNN](demo/denas/computer_vision/DENAS_CNN_DEMO.ipynb) - Computer Vision, PyTorch
               * [ViT](demo/denas/computer_vision/DENAS_ViT_DEMO.ipynb) - Computer Vision, PyTorch
@@ -100,31 +100,17 @@
              * [Model Adapter Overview](demo/ma/Model_Adapter_Summary.ipynb) 
                * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
                * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
                * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
         
         ## Performance
         
-        Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-        For [DeNAS](e2eAIOK/DeNas/README.md) CNN and ViT, Intel® End-to-End AI Optimization Kit delivered 40.73x and 35.63x search time speedup, 82.57x and 4.44x training time speedup over [ZenNAS](https://github.com/idstcv/ZenNAS) and [AutoFormer](https://github.com/microsoft/Cream/tree/main/AutoFormer) respectively. For DeNAS searched CNN, ViT, BERT and ASR model, Intel® End-to-End AI Optimization Kit delivered 9.86x, 4.44x, 7.68x and 59.12x training time speedup with 0.03x, 1.20x, 0.62x and 0.81x model size respectively. Please refer to DeNAS link for detailed test dataset and test method.
-        > Noted: Optimized lighter models' accuracy are slightly lower: CNN -3% accuracy, ViT -5% accuracy, BERT -4% F1 score.
-        
-        ![Performance](./docs/source/e2eaiok_v10_performance_nas.png "Intel® End-to-End AI Optimization Kit Performance")
-        ![Performance](./docs/source/e2eaiok_v10_performance_stock.png "Intel® End-to-End AI Optimization Kit Performance")
-        
-        Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-        For [MiniGO](modelzoo/minigo/README.md), [BERT](modelzoo/bert/README.md), [ResNet](modelzoo/resnet/README.md), [RNN-T](modelzoo/rnnt/README.md), Intel® End-to-End AI Optimization Kit delivered 13.06x, 10.10x, 8.77x and 14.19x training time speedup respecitvely through E2E optimizations. Please refer to corresponding model link for detailed test dataset and test method. 
-        > Noted: Optimized lighter models' accuracy are slightly lower: ResNet -5% accuracy, BERT -1% F1 score.
-        
-        ![Performance](./docs/source/e2eaiok_v02_performance.png "Intel® End-to-End AI Optimization Kit Performance")
-        
-        Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-        For [WnD](modelzoo/WnD/README.md), [DIEN](modelzoo/dien/README.md) and [DLRM](modelzoo/dlrm/README.md), Intel® End-to-End AI Optimization Kit delivered 51.01x(5.02x ELT & 113.03x training), 12.67x(14.86x ELT & 11.91x training) and 71.16x(86.40x ELT & 42.31x training) E2E time speedup, 21.18x, 14.11x and 124.98x inference throughput speedup respectively. Please refer to corresponding model link for detailed test dataset and test method.
-        
-        ![Performance](./docs/source/e2eaiok_v01_performance.png "Intel® End-to-End AI Optimization Kit Performance")
+        * [E2E RecSys Performance](docs/source/e2e_recsys_performance.md) - DLRM, DIEN, WnD
+        * [SDA Model Performance](docs/source/sda_model_performance.md) - ResNet, BERT, RNN-T, MiniGo
+        * [DE-NAS Performance](docs/source/denas_performance.md) - CNN, ViT, BERT, ASR
         
         
         ## Getting Support
         
         * [Github Issues](https://github.com/intel/e2eAIOK/issues)
         
 Platform: UNKNOWN
```

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/README.md` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,121 @@
-# [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
-
-# INTRODUCTION
-
-## Problem Statement
-
-Modern End to End AI pipeline life cycle is quite complicate with a complex pipeline including data processing, feature engineering, model development, and model deployment & maintenance. The iterative nature for feature engineering, model testing and hyper-parameter optimization makes the process more time-consuming. This complexity creates an entry-barrier for novice and citizen data scientists who might not have such expertise or skills.  Meanwhile, people tend to develop larger and larger models to get better performance, which are quite often over-parameterized.  Those overparameterized models not only poses significant challenges on AI hardware infrastructure as they require expensive computation power for training, but also posed a challenge when try to deploy in resource constraint environment which is a common need.
-
-## Solution with Intel® End-to-End AI Optimization Kit
-
-Intel® End-to-End AI Optimization Kit is a composable toolkits for E2E AI optimization to deliver high performance lightweight networks/models efficiently on commodity HW like CPU, intending to make E2E AI pipelines faster, easier and more accessible.
-
-Making AI Faster: It reduces E2E time on CPU to an acceptable range throughput full pipeline optimization and improved scale-up/out capability on Intel platforms with Intel optimized framework and toolkits, delivers popular lighter DL Models with close enough performance and significantly higher inference throughput.
-
-Making AI Easier: It automates provides simplified toolkits for data processing, distributed training, and compact neural network construction, automates E2E AI pipeline with click to run workflows and can be easily plugged to third party ML solutions/platforms as an independent composable component.
-
-Making AI more accessible:  Through built-in optimized, parameterized models generated by smart democratization advisor and domain-specific, neural architected search (NAS) based network constructure, it brings complex DL to commodity HW, everyone can easily access AI on existing CPU clusters without the need to be an expert on data engineering and data science.
-
-## This solution is intended for
-
-This solution is intended for citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-
-## Papers and Blogs
-
-* [ICYMI – SigOpt Summit Recap Democratizing End-to-End Recommendation Systems](https://sigopt.com/blog/icymi-sigopt-summit-recap-democratizing-end-to-end-recommendation-systems-with-jian-zhang/)
-* [The SigOpt Intelligent Experimentation Platform](https://www.intel.com/content/www/us/en/developer/articles/technical/sigopt-intelligent-experimentation-platform.html#gs.gz2ls6)
-* [SDC2022 - Data Platform for End-to-end AI Democratization](https://storagedeveloper.org/events/sdc-2022/agenda/session/326)
-* [SIHG4SR: Side Information Heterogeneous Graph for Session Recommender](https://dl.acm.org/doi/abs/10.1145/3556702.3556852)
-
-# ARCHITECTURE
-
-## Intel® End-to-End AI Optimization Kit
-
-Intel® End-to-End AI Optimization Kit is a composable toolkits for E2E AI optimization to deliver high performance lightweight networks/models efficiently on commodity HW. It is a pipeline framework that streamlines AI optimization technologies in each stage of E2E AI pipeline, including data processing, feature engineering, training, hyper-parameter tunning, and inference. Intel® End-to-End AI Optimization Kit delivers high performance, lightweight models efficiently on commodity hardware.
-
-## The key components are
-
-* [RecDP](RecDP/README.md):  A parallel data processing and feature engineering lib on top of Spark, and extensible to other data processing tools. It provides abstraction API to hide Spark programming complexity, delivers optimized performance through adaptive query plan & strategy, supports critical feature engineering functions on Tabular dataset, and can be easily integrated to third party solutions.  
-
-* [Smart Democratization Advisor (SDA)](e2eAIOK/SDA/README.md): A user-guided tool to facilitate automation of built-in model democratization via parameterized models, it generates yaml files based on user choice, provided build-in intelligence through parameterized models and leverage SigOpt for HPO. SDA converts the manual model tuning and optimization to assisted autoML and autoHPO. SDA provides a list of build-in optimized models ranging from RecSys, CV, NLP, ASR and RL.
-
-* Neural Network Constructor: A neural architecture search technology and transfer learning based component to build compact neural network models for specific domains directly. It includes two componments, [DE-NAS](e2eAIOK/DeNas/README.md) and [Model Adapter](e2eAIOK/ModelAdapter/README.md). DE-NAS is a multi-model, hardware aware, train-free neural architecture search approach to build models for CV, NLP, ASR directly. Model Adapter leverages transfer learning model adaptor to deploy the models in user’s production environment.
-
-For more information, you may [read the docs](https://github.com/intel/e2eAIOK).
-![Architecture](./docs/source/aiok_workflow.png)
-
-# Getting Started
-
-## Installing
-
-### Install with Baremetal Environment
-
- - To install all components:
-   - To install e2eAIOK in baremetal environment, use `pip install e2eAIOK`
-   - To install latest nightly build, use `pip install e2eAIOK --pre`
-
- - To install each individual component:
-   - To install SDA, use `pip install e2eAIOK-sda`
-   - To install DE-NAS, use `pip install e2eAIOK-denas`
-   - To install Model Adapter, use `pip install e2eAIOK-ModelAdapter`
-
-### Install with Docker Environment
-``` bash
-git clone https://github.com/intel/e2eAIOK.git
-cd e2eAIOK
-git submodule update --init --recursive
-python scripts/start_e2eaiok_docker.py --backend [tensorflow, pytorch, pytorch112] --dataset_path ../ --workers host1, host2, host3, host4 --proxy "http://addr:ip"
-```
-
-## Demos
-
-* Built-in Models
-  * [DLRM](modelzoo/dlrm/README.md) - RecSys, PyTorch
-  * [DIEN](modelzoo/dien/README.md) - RecSys, TensorFlow
-  * [WND](modelzoo/WnD/README.md) - RecSys, TensorFlow
-  * [RNNT](modelzoo/rnnt/README.md) - Speech Recognition, PyTorch
-  * [RESNET](modelzoo/resnet/README.md) - Computer vision, TensorFlow
-  * [BERT](modelzoo/bert/README.md) - Natual Language Processing, TensorFlow
-  * [MiniGo](modelzoo/minigo/README.md) - minimalist engine modeled after AlphaGo Zero, TensorFlow
-
-* Neural network constructor 
-
-  * DE-NAS demos:
-    * [DE-NAS Overview](demo/denas/DENAS_SUMMARY.ipynb) 
-      * [CNN](demo/denas/computer_vision/DENAS_CNN_DEMO.ipynb) - Computer Vision, PyTorch
-      * [ViT](demo/denas/computer_vision/DENAS_ViT_DEMO.ipynb) - Computer Vision, PyTorch
-      * [BERT](demo/denas/bert/DENAS_BERT_DEMO.ipynb) - NLP, PyTorch
-      * [ASR](demo/denas/asr/DENAS_ASR_DEMO.ipynb) - Speech Recognition, PyTorch
-      * [BERT](demo/denas/hf/DENAS_HF_DEMO.ipynb) - Hugging Face models, PyTorch
-  
-  * Model Aadapter demos
-     * [Model Adapter Overview](demo/ma/Model_Adapter_Summary.ipynb) 
-       * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
-       * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
-       * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
-
-## Performance
-
-Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-For [DeNAS](e2eAIOK/DeNas/README.md) CNN and ViT, Intel® End-to-End AI Optimization Kit delivered 40.73x and 35.63x search time speedup, 82.57x and 4.44x training time speedup over [ZenNAS](https://github.com/idstcv/ZenNAS) and [AutoFormer](https://github.com/microsoft/Cream/tree/main/AutoFormer) respectively. For DeNAS searched CNN, ViT, BERT and ASR model, Intel® End-to-End AI Optimization Kit delivered 9.86x, 4.44x, 7.68x and 59.12x training time speedup with 0.03x, 1.20x, 0.62x and 0.81x model size respectively. Please refer to DeNAS link for detailed test dataset and test method.
-> Noted: Optimized lighter models' accuracy are slightly lower: CNN -3% accuracy, ViT -5% accuracy, BERT -4% F1 score.
-
-![Performance](./docs/source/e2eaiok_v10_performance_nas.png "Intel® End-to-End AI Optimization Kit Performance")
-![Performance](./docs/source/e2eaiok_v10_performance_stock.png "Intel® End-to-End AI Optimization Kit Performance")
-
-Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-For [MiniGO](modelzoo/minigo/README.md), [BERT](modelzoo/bert/README.md), [ResNet](modelzoo/resnet/README.md), [RNN-T](modelzoo/rnnt/README.md), Intel® End-to-End AI Optimization Kit delivered 13.06x, 10.10x, 8.77x and 14.19x training time speedup respecitvely through E2E optimizations. Please refer to corresponding model link for detailed test dataset and test method. 
-> Noted: Optimized lighter models' accuracy are slightly lower: ResNet -5% accuracy, BERT -1% F1 score.
-
-![Performance](./docs/source/e2eaiok_v02_performance.png "Intel® End-to-End AI Optimization Kit Performance")
-
-Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
-For [WnD](modelzoo/WnD/README.md), [DIEN](modelzoo/dien/README.md) and [DLRM](modelzoo/dlrm/README.md), Intel® End-to-End AI Optimization Kit delivered 51.01x(5.02x ELT & 113.03x training), 12.67x(14.86x ELT & 11.91x training) and 71.16x(86.40x ELT & 42.31x training) E2E time speedup, 21.18x, 14.11x and 124.98x inference throughput speedup respectively. Please refer to corresponding model link for detailed test dataset and test method.
-
-![Performance](./docs/source/e2eaiok_v01_performance.png "Intel® End-to-End AI Optimization Kit Performance")
-
-
-## Getting Support
-
-* [Github Issues](https://github.com/intel/e2eAIOK/issues)
+Metadata-Version: 2.1
+Name: e2eAIOK-ModelAdapter
+Version: 1.0.1b2023042500
+Summary: Intel® End-to-End AI Optimization Kit
+Home-page: https://github.com/intel/e2eAIOK
+Author: INTEL
+License: Apache License
+Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
+Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
+        
+        # INTRODUCTION
+        
+        ## Problem Statement
+        
+        Modern End to End AI pipeline life cycle is quite complicate with a complex pipeline including data processing, feature engineering, model development, and model deployment & maintenance. The iterative nature for feature engineering, model testing and hyper-parameter optimization makes the process more time-consuming. This complexity creates an entry-barrier for novice and citizen data scientists who might not have such expertise or skills.  Meanwhile, people tend to develop larger and larger models to get better performance, which are quite often over-parameterized.  Those overparameterized models not only poses significant challenges on AI hardware infrastructure as they require expensive computation power for training, but also posed a challenge when try to deploy in resource constraint environment which is a common need.
+        
+        ## Solution with Intel® End-to-End AI Optimization Kit
+        
+        Intel® End-to-End AI Optimization Kit is a composable toolkits for E2E AI optimization to deliver high performance lightweight networks/models efficiently on commodity HW like CPU, intending to make E2E AI pipelines faster, easier and more accessible.
+        
+        Making AI Faster: It reduces E2E time on CPU to an acceptable range throughput full pipeline optimization and improved scale-up/out capability on Intel platforms with Intel optimized framework and toolkits, delivers popular lighter DL Models with close enough performance and significantly higher inference throughput.
+        
+        Making AI Easier: It automates provides simplified toolkits for data processing, distributed training, and compact neural network construction, automates E2E AI pipeline with click to run workflows and can be easily plugged to third party ML solutions/platforms as an independent composable component.
+        
+        Making AI more accessible:  Through built-in optimized, parameterized models generated by smart democratization advisor and domain-specific, neural architected search (NAS) based network constructure, it brings complex DL to commodity HW, everyone can easily access AI on existing CPU clusters without the need to be an expert on data engineering and data science.
+        
+        ## This solution is intended for
+        
+        This solution is intended for citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+        
+        ## Papers and Blogs
+        
+        * [ICYMI – SigOpt Summit Recap Democratizing End-to-End Recommendation Systems](https://sigopt.com/blog/icymi-sigopt-summit-recap-democratizing-end-to-end-recommendation-systems-with-jian-zhang/)
+        * [The SigOpt Intelligent Experimentation Platform](https://www.intel.com/content/www/us/en/developer/articles/technical/sigopt-intelligent-experimentation-platform.html#gs.gz2ls6)
+        * [SDC2022 - Data Platform for End-to-end AI Democratization](https://storagedeveloper.org/events/sdc-2022/agenda/session/326)
+        * [SIHG4SR: Side Information Heterogeneous Graph for Session Recommender](https://dl.acm.org/doi/abs/10.1145/3556702.3556852)
+        
+        # ARCHITECTURE
+        
+        ## Intel® End-to-End AI Optimization Kit
+        
+        Intel® End-to-End AI Optimization Kit is a composable toolkits for E2E AI optimization to deliver high performance lightweight networks/models efficiently on commodity HW. It is a pipeline framework that streamlines AI optimization technologies in each stage of E2E AI pipeline, including data processing, feature engineering, training, hyper-parameter tunning, and inference. Intel® End-to-End AI Optimization Kit delivers high performance, lightweight models efficiently on commodity hardware.
+        
+        ## The key components are
+        
+        * [RecDP](RecDP/README.md):  A parallel data processing and feature engineering lib on top of Spark, and extensible to other data processing tools. It provides abstraction API to hide Spark programming complexity, delivers optimized performance through adaptive query plan & strategy, supports critical feature engineering functions on Tabular dataset, and can be easily integrated to third party solutions.  
+        
+        * [Smart Democratization Advisor (SDA)](e2eAIOK/SDA/README.md): A user-guided tool to facilitate automation of built-in model democratization via parameterized models, it generates yaml files based on user choice, provided build-in intelligence through parameterized models and leverage SigOpt for HPO. SDA converts the manual model tuning and optimization to assisted autoML and autoHPO. SDA provides a list of build-in optimized models ranging from RecSys, CV, NLP, ASR and RL.
+        
+        * Neural Network Constructor: A neural architecture search technology and transfer learning based component to build compact neural network models for specific domains directly. It includes two componments, [DE-NAS](e2eAIOK/DeNas/README.md) and [Model Adapter](e2eAIOK/ModelAdapter/README.md). DE-NAS is a multi-model, hardware aware, train-free neural architecture search approach to build models for CV, NLP, ASR directly. Model Adapter leverages transfer learning model adaptor to deploy the models in user’s production environment.
+        
+        For more information, you may [read the docs](https://github.com/intel/e2eAIOK).
+        ![Architecture](./docs/source/aiok_workflow.png)
+        
+        # Getting Started
+        
+        ## Installing
+        
+        ### Install with Baremetal Environment
+        
+         - To install all components:
+           - To install e2eAIOK in baremetal environment, use `pip install e2eAIOK`
+           - To install latest nightly build, use `pip install e2eAIOK --pre`
+        
+         - To install each individual component:
+           - To install SDA, use `pip install e2eAIOK-sda`
+           - To install DE-NAS, use `pip install e2eAIOK-denas`
+           - To install Model Adapter, use `pip install e2eAIOK-ModelAdapter`
+        
+        ### Install with Docker Environment
+        ``` bash
+        git clone https://github.com/intel/e2eAIOK.git
+        cd e2eAIOK
+        git submodule update --init --recursive
+        python scripts/start_e2eaiok_docker.py --backend [tensorflow, pytorch, pytorch112] --dataset_path ../ --workers host1, host2, host3, host4 --proxy "http://addr:ip"
+        ```
+        
+        ## Demos
+        
+        * Built-in Models
+          * [DLRM](demo/builtin/dlrm/DLRM_DEMO.ipynb) - RecSys, PyTorch
+          * [DIEN](demo/builtin/dien/DIEN_DEMO.ipynb) - RecSys, TensorFlow
+          * [WND](demo/builtin/wnd/WND_DEMO.ipynb) - RecSys, TensorFlow
+          * [RNNT](demo/builtin/rnnt/RNNT_DEMO.ipynb) - Speech Recognition, PyTorch
+          * [RESNET](demo/builtin/resnet/RESNET_DEMO.ipynb) - Computer vision, TensorFlow
+          * [BERT](demo/builtin/bert/BERT_DEMO.ipynb) - Natual Language Processing, TensorFlow
+          * [MiniGo](demo/builtin/minigo/MiniGo_DEMO.ipynb) - minimalist engine modeled after AlphaGo Zero, TensorFlow
+        
+        * Neural network constructor 
+        
+          * DE-NAS demos:
+            * [DE-NAS Overview](demo/denas/DENAS_SUMMARY.ipynb) 
+              * [CNN](demo/denas/computer_vision/DENAS_CNN_DEMO.ipynb) - Computer Vision, PyTorch
+              * [ViT](demo/denas/computer_vision/DENAS_ViT_DEMO.ipynb) - Computer Vision, PyTorch
+              * [BERT](demo/denas/bert/DENAS_BERT_DEMO.ipynb) - NLP, PyTorch
+              * [ASR](demo/denas/asr/DENAS_ASR_DEMO.ipynb) - Speech Recognition, PyTorch
+              * [BERT](demo/denas/hf/DENAS_HF_DEMO.ipynb) - Hugging Face models, PyTorch
+          
+          * Model Aadapter demos
+             * [Model Adapter Overview](demo/ma/Model_Adapter_Summary.ipynb) 
+               * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
+               * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
+               * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
+        
+        ## Performance
+        
+        * [E2E RecSys Performance](docs/source/e2e_recsys_performance.md) - DLRM, DIEN, WnD
+        * [SDA Model Performance](docs/source/sda_model_performance.md) - ResNet, BERT, RNN-T, MiniGo
+        * [DE-NAS Performance](docs/source/denas_performance.md) - CNN, ViT, BERT, ASR
+        
+        
+        ## Getting Support
+        
+        * [Github Issues](https://github.com/intel/e2eAIOK/issues)
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/factory.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/__init__.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/cifar.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/composed_dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/office31.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/office31.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/default_ma.conf` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/default_ma.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/main.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/main.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/task.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/task.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/train.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/default.conf` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/default.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_asr.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_cv.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_nlp.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/data_utils.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/image_list.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/image_list.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/data_builder.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/data_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/lenet.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/lenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/model_utils.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/model_builder.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/torch_trainer.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/extend_distributed.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/extend_distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/trainer/utils/utils.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/trainer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK/common/utils.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK/common/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.0.1b2023042400/setup.py` & `e2eAIOK-ModelAdapter-1.0.1b2023042500/setup.py`

 * *Files identical despite different names*

