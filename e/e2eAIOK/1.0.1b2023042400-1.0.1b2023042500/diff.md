# Comparing `tmp/e2eAIOK-1.0.1b2023042400.tar.gz` & `tmp/e2eAIOK-1.0.1b2023042500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e2eAIOK-1.0.1b2023042400.tar", last modified: Mon Apr 24 00:02:46 2023, max compression
+gzip compressed data, was "dist/e2eAIOK-1.0.1b2023042500.tar", last modified: Tue Apr 25 00:05:58 2023, max compression
```

## Comparing `e2eAIOK-1.0.1b2023042400.tar` & `e2eAIOK-1.0.1b2023042500.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/TransformerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/TransformerLM.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/asr_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/asr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/augment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/wer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/init_asr_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/supernet_asr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/Accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/asr_nas.py
--rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/metric_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/DeNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/benchmark_network_latency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/cv_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/supernet_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/ZenNet.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/Linear_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/attention_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/multihead_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/qkv_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/embedding_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/layernorm_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/bert_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/supernet_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/utils_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/compute_de_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/transformer_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/BaseSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/RandomSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/SearchEngineFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/SigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/supernet_hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/office31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/default_ma.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/SDA.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/image_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/torch_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/extend_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/dataloader/hydrodataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroautolearner.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroconnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydromodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydromodelzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroweblistener.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 00:02:44.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:02:46.000000 e2eAIOK-1.0.1b2023042400/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-24 00:02:38.000000 e2eAIOK-1.0.1b2023042400/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/TransformerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/TransformerLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/asr_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/asr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/augment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/wer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/init_asr_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/supernet_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/Accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/asr_nas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/metric_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/DeNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/benchmark_network_latency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/cv_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/supernet_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/ZenNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/Linear_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/attention_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/multihead_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/qkv_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/embedding_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/layernorm_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/bert_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/supernet_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/utils_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/compute_de_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/transformer_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/BaseSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/RandomSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/SearchEngineFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/SigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/supernet_hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/office31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/default_ma.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/SDA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/torch_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/extend_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/dataloader/hydrodataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroautolearner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroconnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydromodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydromodelzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroweblistener.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 00:05:56.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-25 00:05:57.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:05:57.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:05:57.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 00:05:57.000000 e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:05:58.000000 e2eAIOK-1.0.1b2023042500/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-25 00:05:48.000000 e2eAIOK-1.0.1b2023042500/setup.py
```

### Comparing `e2eAIOK-1.0.1b2023042400/PKG-INFO` & `e2eAIOK-1.0.1b2023042500/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK
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

### Comparing `e2eAIOK-1.0.1b2023042400/README.md` & `e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/PKG-INFO`

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
+Name: e2eAIOK
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

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/TransformerBase.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/TransformerBase.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/TransformerLM.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/TransformerLM.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/asr_model_builder.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/asr_model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/asr_trainer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/asr_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/augment.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/augment.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/batch.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/batch.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataio.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataio.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataloader.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/dataset.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/sampler.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/sampler.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/dataio/wer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/dataio/wer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/features.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/librispeech_prepare.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/librispeech_prepare.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/features.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/signal_processing.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/signal_processing.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/ctc.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/ctc.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/decoders/seq2seq.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/decoders/seq2seq.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/init_asr_parser.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/init_asr_parser.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/CNN.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/CNN.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/containers.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/containers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/lib/convolution.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/lib/convolution.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/model_builder_denas_asr.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/model_builder_denas_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/supernet_asr.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/supernet_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/losses.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/losses.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/trainer/schedulers.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/trainer/schedulers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/Accuracy.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/Accuracy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/asr_nas.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/asr_nas.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/checkpoints.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/data_pipeline.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/data_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/depgraph.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/depgraph.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/distributed.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/edit_distance.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/edit_distance.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/metric_stats.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/metric_stats.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/parameter_transfer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/parameter_transfer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/asr/utils/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/asr/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/benchmark_network_latency.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/benchmark_network_latency.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/cv_trainer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/cv_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/model_builder_denas_cv.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/model_builder_denas_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/supernet_transformer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/supernet_transformer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/third_party/ZenNet.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/third_party/ZenNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/cnn.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/cv/utils/vit.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/cv/utils/vit.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/attention.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/attention.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/decoder.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/decoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/encoder.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/encoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/normalization.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/normalization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/asr/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/asr/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/Linear_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/embedding_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/layernorm_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/multihead_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/multihead_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/qkv_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/qkv_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/cv/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/cv/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/Linear_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_attention_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_attention_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/layernorm_super.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/optimization.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/optimization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/module/nlp/tokenization.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/module/nlp/tokenization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/bert_trainer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/bert_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/supernet_bert.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/supernet_bert.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/nlp/utils_eval.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/nlp/utils_eval.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/basic_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/basic_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/compute_de_score.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/compute_de_score.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/scores/transformer_proxy.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/scores/transformer_proxy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/BaseSearchEngine.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/BaseSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/RandomSearchEngine.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/RandomSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/SearchEngineFactory.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/SearchEngineFactory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/SigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/SigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/search.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/search.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/supernet_hf.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/supernet_hf.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/thirdparty/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/thirdparty/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/train.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/DeNas/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/DeNas/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/factory.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/__init__.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/cifar.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/composed_dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/dataset/office31.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/dataset/office31.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/default_ma.conf` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/default_ma.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/main.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/main.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/task.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/task.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/ModelAdapter/training/train.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/ModelAdapter/training/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/SDA.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/SDA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/TestAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/TestAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/default.conf` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/default.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_asr.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_cv.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_builder_nlp.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_builder_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/data_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/data_utils/image_list.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/data_utils/image_list.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/data_builder.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/data_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/lenet.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/lenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model/model_utils/model_utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model/model_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/model_builder.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/torch_trainer.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/extend_distributed.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/extend_distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/trainer/utils/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/trainer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/common/utils.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/common/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/dataloader/hydrodataloader.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/dataloader/hydrodataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroDB.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroDB.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroautolearner.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroautolearner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroconfig.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroconfig.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydromodel.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydromodel.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK/utils/hydroserver.py` & `e2eAIOK-1.0.1b2023042500/e2eAIOK/utils/hydroserver.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/e2eAIOK.egg-info/SOURCES.txt` & `e2eAIOK-1.0.1b2023042500/e2eAIOK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042400/setup.py` & `e2eAIOK-1.0.1b2023042500/setup.py`

 * *Files identical despite different names*

