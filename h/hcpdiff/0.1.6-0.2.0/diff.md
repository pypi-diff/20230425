# Comparing `tmp/hcpdiff-0.1.6.tar.gz` & `tmp/hcpdiff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.1.6.tar", last modified: Thu Apr 13 13:48:22 2023, max compression
+gzip compressed data, was "hcpdiff-0.2.0.tar", last modified: Tue Apr 25 10:12:54 2023, max compression
```

## Comparing `hcpdiff-0.1.6.tar` & `hcpdiff-0.2.0.tar`

### file list

```diff
@@ -1,83 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.736085 hcpdiff-0.1.6/
--rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4856 2023-04-13 13:48:22.735091 hcpdiff-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4119 2023-04-12 09:50:49.000000 hcpdiff-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.611278 hcpdiff-0.1.6/cfgs/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.616777 hcpdiff-0.1.6/cfgs/infer/
--rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.1.6/cfgs/infer/change_vae.yaml
--rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.1.6/cfgs/infer/euler_a.yaml
--rw-rw-rw-   0        0        0     1441 2023-04-12 10:04:24.000000 hcpdiff-0.1.6/cfgs/infer/v1.yaml
--rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.1.6/cfgs/te_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.621591 hcpdiff-0.1.6/cfgs/train/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.634567 hcpdiff-0.1.6/cfgs/train/examples/
--rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/CustomDiffusion.yaml
--rw-rw-rw-   0        0        0     2807 2023-04-13 13:47:11.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamArtist++.yaml
--rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamArtist.yaml
--rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamBooth.yaml
--rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/TextualInversion.yaml
--rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/fine-tuning.yaml
--rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/locon.yaml
--rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/lora_conventional.yaml
--rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/train_base.yaml
--rw-rw-rw-   0        0        0      987 2023-04-11 08:41:31.000000 hcpdiff-0.1.6/cfgs/train/tuning_base.yaml
--rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.1.6/cfgs/unet_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.643674 hcpdiff-0.1.6/hcpdiff/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.662458 hcpdiff-0.1.6/hcpdiff/data/
--rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/data/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/data/bucket.py
--rw-rw-rw-   0        0        0     5678 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/data/pair_dataset.py
--rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.681221 hcpdiff-0.1.6/hcpdiff/models/
--rw-rw-rw-   0        0        0      290 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/models/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/models/cfg_context.py
--rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/layers.py
--rw-rw-rw-   0        0        0     7732 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/lora.py
--rw-rw-rw-   0        0        0     7067 2023-04-13 07:55:06.000000 hcpdiff-0.1.6/hcpdiff/models/lora_layers.py
--rw-rw-rw-   0        0        0     5721 2023-04-13 07:55:06.000000 hcpdiff-0.1.6/hcpdiff/models/plugin.py
--rw-rw-rw-   0        0        0     3582 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/text_emb_ex.py
--rw-rw-rw-   0        0        0     5507 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/textencoder_ex.py
--rw-rw-rw-   0        0        0     2360 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/tokenizer_ex.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.694428 hcpdiff-0.1.6/hcpdiff/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/tools/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.1.6/hcpdiff/tools/convert_caption_txt2json.py
--rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/create_embedding.py
--rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/gen_from_ptlist.py
--rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.1.6/hcpdiff/tools/init_proj.py
--rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/merge_model_part.py
--rw-rw-rw-   0        0        0     7233 2023-04-12 09:50:49.000000 hcpdiff-0.1.6/hcpdiff/tools/sd2diffusers.py
--rw-rw-rw-   0        0        0    23465 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/train_ac.py
--rw-rw-rw-   0        0        0     1827 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/train_ac_single.py
--rw-rw-rw-   0        0        0     9171 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/train_colo.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.712161 hcpdiff-0.1.6/hcpdiff/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/utils/caption_tools.py
--rw-rw-rw-   0        0        0     7789 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/utils/cfg_net_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.720183 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/
--rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
--rw-rw-rw-   0        0        0     1833 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
--rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/colo_utils.py
--rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ema.py
--rw-rw-rw-   0        0        0      448 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/emb_utils.py
--rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/img_size_tool.py
--rw-rw-rw-   0        0        0     6623 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/utils.py
--rw-rw-rw-   0        0        0     4215 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.655783 hcpdiff-0.1.6/hcpdiff.egg-info/
--rw-rw-rw-   0        0        0     4856 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1961 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      225 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.733097 hcpdiff-0.1.6/prompt_tuning_template/
--rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.1.6/prompt_tuning_template/caption.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.1.6/prompt_tuning_template/name.txt
--rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.1.6/prompt_tuning_template/name_2pt_caption.txt
--rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.1.6/prompt_tuning_template/name_caption.txt
--rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.1.6/prompt_tuning_template/object.txt
--rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.1.6/prompt_tuning_template/style.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 13:48:22.736085 hcpdiff-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-13 13:48:19.000000 hcpdiff-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.734085 hcpdiff-0.1.6/test/
--rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.1.6/test/test_plugin_param.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.134604 hcpdiff-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5477 2023-04-25 10:12:54.133605 hcpdiff-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4740 2023-04-24 07:27:38.000000 hcpdiff-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.077252 hcpdiff-0.2.0/cfgs/
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.080242 hcpdiff-0.2.0/cfgs/infer/
+-rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.2.0/cfgs/infer/change_vae.yaml
+-rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.2.0/cfgs/infer/euler_a.yaml
+-rw-rw-rw-   0        0        0     1659 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/img2img.yaml
+-rw-rw-rw-   0        0        0     1804 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/img2img_controlnet.yaml
+-rw-rw-rw-   0        0        0     1554 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/text2img.yaml
+-rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.2.0/cfgs/te_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.083243 hcpdiff-0.2.0/cfgs/train/
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.089254 hcpdiff-0.2.0/cfgs/train/examples/
+-rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/CustomDiffusion.yaml
+-rw-rw-rw-   0        0        0     2815 2023-04-15 14:19:44.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamArtist++.yaml
+-rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamArtist.yaml
+-rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamBooth.yaml
+-rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/TextualInversion.yaml
+-rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/fine-tuning.yaml
+-rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/locon.yaml
+-rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/lora_conventional.yaml
+-rw-rw-rw-   0        0        0      343 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/train/plugin_control.yaml
+-rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/train_base.yaml
+-rw-rw-rw-   0        0        0     1241 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/train/tuning_base.yaml
+-rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.2.0/cfgs/unet_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.093458 hcpdiff-0.2.0/hcpdiff/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.101451 hcpdiff-0.2.0/hcpdiff/data/
+-rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/data/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.2.0/hcpdiff/data/bucket.py
+-rw-rw-rw-   0        0        0     5732 2023-04-17 09:36:22.000000 hcpdiff-0.2.0/hcpdiff/data/pair_dataset.py
+-rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.109275 hcpdiff-0.2.0/hcpdiff/models/
+-rw-rw-rw-   0        0        0      295 2023-04-15 14:19:44.000000 hcpdiff-0.2.0/hcpdiff/models/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/models/cfg_context.py
+-rw-rw-rw-   0        0        0     7719 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/models/controlnet.py
+-rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.2.0/hcpdiff/models/layers.py
+-rw-rw-rw-   0        0        0     7949 2023-04-17 08:00:11.000000 hcpdiff-0.2.0/hcpdiff/models/lora_base.py
+-rw-rw-rw-   0        0        0     7735 2023-04-17 08:00:11.000000 hcpdiff-0.2.0/hcpdiff/models/lora_layers.py
+-rw-rw-rw-   0        0        0     6045 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/models/plugin.py
+-rw-rw-rw-   0        0        0     3957 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/models/text_emb_ex.py
+-rw-rw-rw-   0        0        0     5784 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/models/textencoder_ex.py
+-rw-rw-rw-   0        0        0     2440 2023-04-14 04:04:05.000000 hcpdiff-0.2.0/hcpdiff/models/tokenizer_ex.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.115275 hcpdiff-0.2.0/hcpdiff/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/hcpdiff/tools/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.2.0/hcpdiff/tools/convert_caption_txt2json.py
+-rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/create_embedding.py
+-rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/gen_from_ptlist.py
+-rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.2.0/hcpdiff/tools/init_proj.py
+-rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/merge_model_part.py
+-rw-rw-rw-   0        0        0     8536 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/tools/sd2diffusers.py
+-rw-rw-rw-   0        0        0    25035 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_ac.py
+-rw-rw-rw-   0        0        0     3683 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_ac_single.py
+-rw-rw-rw-   0        0        0     8448 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_colo.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.121606 hcpdiff-0.2.0/hcpdiff/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/hcpdiff/utils/caption_tools.py
+-rw-rw-rw-   0        0        0    11320 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/cfg_net_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.123604 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/
+-rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/__init__.py
+-rw-rw-rw-   0        0        0     3197 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
+-rw-rw-rw-   0        0        0     1884 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
+-rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/colo_utils.py
+-rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/ema.py
+-rw-rw-rw-   0        0        0      468 2023-04-17 09:36:22.000000 hcpdiff-0.2.0/hcpdiff/utils/emb_utils.py
+-rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/img_size_tool.py
+-rw-rw-rw-   0        0        0     5713 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/net_utils.py
+-rw-rw-rw-   0        0        0     2835 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/utils/utils.py
+-rw-rw-rw-   0        0        0     7299 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.098452 hcpdiff-0.2.0/hcpdiff.egg-info/
+-rw-rw-rw-   0        0        0     5477 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2263 2023-04-25 10:12:54.000000 hcpdiff-0.2.0/hcpdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      225 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.130606 hcpdiff-0.2.0/prompt_tuning_template/
+-rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.2.0/prompt_tuning_template/caption.txt
+-rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.2.0/prompt_tuning_template/name.txt
+-rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.2.0/prompt_tuning_template/name_2pt_caption.txt
+-rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.2.0/prompt_tuning_template/name_caption.txt
+-rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.2.0/prompt_tuning_template/object.txt
+-rw-rw-rw-   0        0        0     1212 2023-04-17 05:27:11.000000 hcpdiff-0.2.0/prompt_tuning_template/object_caption.txt
+-rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.2.0/prompt_tuning_template/style.txt
+-rw-rw-rw-   0        0        0     1099 2023-04-17 05:27:11.000000 hcpdiff-0.2.0/prompt_tuning_template/style_caption.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:12:54.135606 hcpdiff-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-04-25 10:12:52.000000 hcpdiff-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.133605 hcpdiff-0.2.0/test/
+-rw-rw-rw-   0        0        0     1062 2023-04-19 08:08:17.000000 hcpdiff-0.2.0/test/test_combine.py
+-rw-rw-rw-   0        0        0      717 2023-04-25 06:44:29.000000 hcpdiff-0.2.0/test/test_ctnet.py
+-rw-rw-rw-   0        0        0      918 2023-04-20 07:07:20.000000 hcpdiff-0.2.0/test/test_paradict.py
+-rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.2.0/test/test_plugin_param.py
```

### Comparing `hcpdiff-0.1.6/LICENSE` & `hcpdiff-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/PKG-INFO` & `hcpdiff-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.6
+Version: 0.2.0
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HCP-Diffusion
 
+[![PyPI](https://img.shields.io/pypi/v/hcpdiff)](https://pypi.org/project/hcpdiff/)
+[![GitHub stars](https://img.shields.io/github/stars/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/stargazers)
+[![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
+[![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
+
 [📘中文说明](./README_cn.md)
 
 ## Introduction
 HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
 It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
 
 This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
@@ -62,15 +68,15 @@
 
 Install from source:
 ```bash
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
-hcpinit
+## hcpinit
 ```
 
 ## User guidance
 
 Training:
 ```yaml
 # with accelerate
```

### Comparing `hcpdiff-0.1.6/README.md` & `hcpdiff-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # HCP-Diffusion
 
+[![PyPI](https://img.shields.io/pypi/v/hcpdiff)](https://pypi.org/project/hcpdiff/)
+[![GitHub stars](https://img.shields.io/github/stars/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/stargazers)
+[![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
+[![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
+
 [📘中文说明](./README_cn.md)
 
 ## Introduction
 HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
 It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
 
 This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
@@ -43,15 +49,15 @@
 
 Install from source:
 ```bash
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
-hcpinit
+## hcpinit
 ```
 
 ## User guidance
 
 Training:
 ```yaml
 # with accelerate
```

### Comparing `hcpdiff-0.1.6/cfgs/infer/euler_a.yaml` & `hcpdiff-0.2.0/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/infer/v1.yaml` & `hcpdiff-0.2.0/cfgs/infer/text2img.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
 out_dir: 'output/'
 emb_dir: 'embs/'
 N_repeats: 1
 bs: 4
 num: 1
 seed: null
-save_cfg: True
+fp16: True
+
+condition: null
+
+save:
+  save_cfg: True
+  image_type: png
+  quality: 95
+#  image_type: webp
+#  quality: 75
 
 infer_args:
   width: 512
   height: 512
   guidance_scale: 7.5
 
 new_components: {}
```

### Comparing `hcpdiff-0.1.6/cfgs/te_struct.txt` & `hcpdiff-0.2.0/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/DreamArtist++.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 _base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
 
 unet: null
 
 lora_unet:
   - lr: 1e-4
     rank: 0.01875
-    type: p
+    branch: p
     layers:
       - 're:.*\.attn.?$'
       #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
   - lr: 4e-5 # Low negative unet lr prevents image collapse
     rank: 0.01875
-    type: n
+    branch: n
     layers:
       - 're:.*\.attn.?$'
       #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
   #  - lr: 1e-4
   #    rank: 0.01875
   #    type: p
   #    layers:
@@ -25,21 +25,21 @@
   #    type: n
   #    layers:
   #      - 're:.*\.resnets$' # Increases fitness, but potentially reduces controllability and change style
 
 lora_text_encoder:
   - lr: 1e-5
     rank: 0.01
-    type: p
+    branch: p
     layers:
       - 're:.*self_attn$'
       - 're:.*mlp$'
   - lr: 1e-5
     rank: 0.01
-    type: n
+    branch: n
     layers:
       - 're:.*self_attn$'
       - 're:.*mlp$'
 
 tokenizer_pt:
   train: # prompt tuning embeddings
     - { name: 'pt-botdog1', lr: 0.003 }
```

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/locon.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.2.0/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/train/train_base.yaml` & `hcpdiff-0.2.0/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/cfgs/unet_struct.txt` & `hcpdiff-0.2.0/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/data/bucket.py` & `hcpdiff-0.2.0/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.2.0/hcpdiff/data/pair_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,26 +79,26 @@
             return dict()
 
     def load_template(self, template_file):
         with open(template_file, 'r', encoding='utf-8') as f:
             return f.read().strip().split('\n')
 
     @torch.no_grad()
-    def cache_latents(self, vae, weight_dtype):
+    def cache_latents(self, vae, weight_dtype, device, show_prog=True):
         self.latents = {}
         self.bucket.rest(0)
 
-        for path, size in tqdm(self.bucket):
+        for path, size in tqdm(self.bucket, disable=not show_prog):
             img_name = os.path.basename(path)
             if img_name not in self.latents:
                 image = self.load_image(path)
                 att_mask = self.get_att_map(get_file_name(img_name))
                 image, att_mask = self.process_data(image, att_mask, size)
 
-                image = image.unsqueeze(0).cuda().to(weight_dtype)
+                image = image.unsqueeze(0).to(device, dtype=weight_dtype)
                 latents = vae.encode(image).latent_dist.sample().squeeze(0)
                 self.latents[img_name] = [(latents * 0.18215).cpu(), att_mask]
 
     def get_att_map(self, img_name):
         if img_name not in self.att_mask_path:
             return None
         att_mask = Image.open(self.att_mask_path[img_name]).convert("L")
```

### Comparing `hcpdiff-0.1.6/hcpdiff/data/utils.py` & `hcpdiff-0.2.0/hcpdiff/data/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/models/cfg_context.py` & `hcpdiff-0.2.0/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/models/layers.py` & `hcpdiff-0.2.0/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/models/lora_layers.py` & `hcpdiff-0.2.0/hcpdiff/models/lora_layers.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,162 +7,137 @@
     :Created:     09/04/2023
     :Licence:     Apache-2.0
 """
 
 from typing import Union
 
 import torch
-from einops import repeat, rearrange
+from einops import repeat, rearrange, einsum
 from torch import nn
 
-from hcpdiff.utils.utils import low_rank_approximate
+from .lora_base import LoraBlock
 from .layers import GroupLinear
 
+class LoraLayer(LoraBlock):
+    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, **kwargs):
+        super().__init__(host, rank, dropout, scale, bias, inplace)
+
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.lora_down = nn.Linear(host.in_features, self.rank, bias=False)
+            self.lora_up = nn.Linear(self.rank, host.out_features, bias=bias)
+
+        def get_collapsed_param(self):
+            w = self.lora_up.weight.data @ self.lora_down.weight.data
+            b = self.lora_up.bias.data if self.bias else None
+            return w, b
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.lora_down = nn.Conv2d(host.in_channels, self.rank, kernel_size=host.kernel_size, stride=host.stride,
+                                       padding=host.padding, dilation=host.dilation, groups=host.groups, bias=False)
+            self.lora_up = nn.Conv2d(self.rank, host.out_channels, kernel_size=1, stride=1, padding=0,
+                                     groups=host.groups, bias=bias)
+
+        def get_collapsed_param(self):
+            w = einsum(self.lora_up.weight.data, self.lora_down.weight.data, 'o r ..., r i ... -> o i ...')
+            b = self.lora_up.bias.data if self.bias else None
+            return w, b
 
-class LoraLayerBase(nn.Module):
-    def __init__(self, host: Union[nn.Linear, nn.Conv2d], rank, dropout=0.1, bias=False):
-        super().__init__()
-        self.host = host
-        self.rank = rank
-        self.dropout = nn.Dropout(dropout)
-        self.host_type = None
-        self.bias = bias
-
-        if isinstance(self.rank, float):
-            self.rank = max(round(host().out_features * self.rank), 1)
-
-        self.build_layers()
-
-    def build_layers(self):
-        pass
-
-    def feed_sdv(self, U, V, weight):
-        self.lora_up.weight.data = U.to(device=weight.device, dtype=weight.dtype)
-        self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
-
-    def init_weights(self, svd_init=False):
-        host = self.host()
-        if svd_init:
-            U, V = low_rank_approximate(host.weight, self.rank)
-            self.feed_sdv(U, V, host.weight)
-        else:
-            self.lora_down.reset_parameters()
-            nn.init.zeros_(self.lora_up.weight)
-
-    def forward(self, x):
-        x = self.dropout(self.lora_up(self.lora_down(x)))
-        return x
-
-    def get_collapsed_param(self):
-        w = collapse_lora_weight(self.lora_up.weight.data, self.lora_up.weight.data, self.host_type)
-        b = self.lora_up.bias.data
-        return w, b
+class LoraLayerGroup(LoraBlock):
+    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=1, **kwargs):
+        self.rank_groups_raw = rank_groups
+        super().__init__(host, rank, dropout, scale, bias, inplace)
 
     def collapse_to_host(self, alpha=None, base_alpha=1.0):
-        if alpha is None:
-            alpha = self.scale
+        raise NotImplementedError('LoraLayerGroup not support reparameterization.')
 
-        host = self.host()
-        re_w, re_b = self.get_collapsed_param()
-        host.weight = nn.Parameter(
-            host.weight.data * base_alpha + alpha * re_w.to(host.weight.device, dtype=host.weight.dtype)
-        )
-
-        if self.lora_up.bias is not None:
-            if host.bias is None:
-                host.bias = nn.Parameter(re_b.to(host.weight.device, dtype=host.weight.dtype))
-            else:
-                host.bias = nn.Parameter(
-                    host.bias.data * base_alpha + alpha * re_b.to(host.weight.device, dtype=host.weight.dtype))
-
-
-class LoraLayerLinear(LoraLayerBase):
-    def __init__(self, host, rank, dropout=0.1, bias=False):
-        super().__init__(host, rank, dropout, bias)
-        self.host_type = 'linear'
-
-    def build_layers(self):
-        host = self.host()
-        self.lora_down = nn.Linear(host.in_features, self.rank, bias=False)
-        self.lora_up = nn.Linear(self.rank, host.out_features, bias=self.bias)
-
-
-class LoraLayerConv2d(LoraLayerBase):
-    def __init__(self, host, rank, dropout=0.1, bias=False):
-        super().__init__(host, rank, dropout, bias)
-        self.host_type = 'conv'
-
-    def build_layers(self):
-        host = self.host()
-        self.lora_down = nn.Conv2d(host.in_channels, self.rank, kernel_size=host.kernel_size, stride=host.stride,
-                                   padding=host.padding, dilation=host.dilation, groups=host.groups, bias=False)
-        self.lora_up = nn.Conv2d(self.rank, host.out_channels, kernel_size=1, stride=1, padding=0, groups=host.groups, bias=self.bias)
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw, dtype=torch.int))
+            self.lora_down = GroupLinear(host.in_features*self.rank_groups, self.rank, groups=self.rank_groups, bias=False)
+            self.lora_up = GroupLinear(self.rank, host.out_features*self.rank_groups, groups=self.rank_groups, bias=bias)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            x = repeat(x, 'b l c -> b l (g c)', g=self.rank_groups)
+            x = rearrange(x, 'b l (g c) -> b g l c', g=self.rank_groups)
+            x = self.dropout(self.lora_up(self.lora_down(x)))
+            x = torch.prod(x, dim=1, dtype=torch.float16)**(1/self.rank_groups).to(dtype=x.dtype)
+            return x
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
+            self.lora_down = nn.Conv2d(host.in_channels * self.rank_groups, self.rank, kernel_size=host.kernel_size, stride=host.stride,
+                                       padding=host.padding, dilation=host.dilation, groups=self.rank_groups, bias=False)
+            self.lora_up = nn.Conv2d(self.rank, host.out_channels * self.rank_groups, kernel_size=1, stride=1,
+                                     padding=0, groups=self.rank_groups, bias=bias)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            x = self.dropout(self.lora_up(self.lora_down(x)))
+            x = torch.prod(rearrange(x, 'b (g c) h w -> b g c h w'), dim=1, dtype=torch.float16) ** (1 / self.rank_groups).to(dtype=x.dtype)
+            return x
 
-class LoraLayerLinearGroup(LoraLayerLinear):
-    def __init__(self, host, rank, dropout=0.1, bias=False, rank_groups=1):
+class LohaLayer(LoraBlock):
+    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=2, **kwargs):
         self.rank_groups_raw = rank_groups
-        super().__init__(host, rank, dropout, bias)
-
-    def build_layers(self):
-        host = self.host()
-        self.register_buffer('rank_groups', torch.tensor(self.rank_groups_raw, dtype=torch.int))
-        self.lora_down = GroupLinear(host.in_features*self.rank_groups, self.rank, groups=self.rank_groups, bias=False)
-        self.lora_up = GroupLinear(self.rank, host.out_features*self.rank_groups, groups=self.rank_groups, bias=self.bias)
-
-    def feed_sdv(self, U, V, weight):
-        self.lora_up.weight.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-        self.lora_down.weight.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-
-    def forward(self, x):
-        x = repeat(x, 'b l c -> b l (g c)', g=self.rank_groups)
-        x = rearrange(x, 'b l (g c) -> b g l c', g=self.rank_groups)
-        x = self.dropout(self.lora_up(self.lora_down(x)))
-        x = torch.prod(x, dim=1, dtype=torch.float16)**(1/self.rank_groups).to(dtype=x.dtype)
-        return x
-
-    def get_collapsed_param(self):
-        raise NotImplementedError('LoraLayerLinearGroup not support reparameterization.')
+        super().__init__(host, rank, dropout, scale, bias, inplace, hook_param='weight')
 
+    def forward(self, host_param: nn.Parameter):
+        return host_param + self.layer(host_param) * self.scale
 
-class LoraLayerConv2dGroup(LoraLayerLinear):
-    def __init__(self, host, rank, dropout=0.1, bias=False, rank_groups=1):
-        self.rank_groups_raw = rank_groups
-        super().__init__(host, rank, dropout, bias)
-
-    def build_layers(self):
-        host = self.host()
-        self.register_buffer('rank_groups', torch.tensor(self.rank_groups_raw))
-        self.lora_down = nn.Conv2d(host.in_channels*self.rank_groups, self.rank, kernel_size=host.kernel_size, stride=host.stride,
-                                   padding=host.padding, dilation=host.dilation, groups=self.rank_groups, bias=False)
-        self.lora_up = nn.Conv2d(self.rank, host.out_channels * self.rank_groups, kernel_size=1, stride=1, padding=0,
-                                 groups=self.rank_groups, bias=self.bias)
-
-    def feed_sdv(self, U, V, weight):
-        self.lora_up.weight.data = rearrange(U, 'o (g ri) -> (g o) ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-        self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
-
-    def forward(self, x):
-        x = self.dropout(self.lora_up(self.lora_down(x)))
-        x = torch.prod(rearrange(x, 'b (g c) h w -> b g c h w'), dim=1, dtype=torch.float16)**(1/self.rank_groups).to(dtype=x.dtype)
-        return x
-
-    def get_collapsed_param(self):
-        raise NotImplementedError('LoraLayerConv2dGroup not support reparameterization.')
-
-
-def collapse_lora_weight(lora_up, lora_down, host_type):
-    if host_type == 'linear':
-        return lora_up @ lora_down
-    elif host_type == 'conv':
-        return lora_up.flatten(1) @ lora_down.flatten(1)
-
-def build_layer(host, host_type, rank, dropout=0.1, bias=False, rank_groups=1):
-    if rank_groups > 1:
-        if host_type == 'linear':
-            return LoraLayerLinearGroup(host, rank, dropout, bias, rank_groups)
-        elif host_type == 'conv':
-            return LoraLayerLinearGroup(host, rank, dropout, bias, rank_groups)
-    else:
-        if host_type == 'linear':
-            return LoraLayerLinear(host, rank, dropout, bias)
-        elif host_type == 'conv':
-            return LoraLayerConv2d(host, rank, dropout, bias)
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
+            self.W_down = nn.Parameter(torch.empty((block.rank_groups_raw, self.rank//block.rank_groups_raw, host.in_features)))
+            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features, self.rank//block.rank_groups_raw)))
+
+        def forward(self, x):
+            return torch.prod(self.W_up @ self.W_down, dim=0)
+
+        def feed_svd(self, U, V, weight):
+            self.W_up.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.W_down.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def get_collapsed_param(self):
+            w = torch.prod(self.W_up.data @ self.W_down.data, dim=0)
+            b = None
+            return w, b
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.W_down = nn.Parameter( torch.empty((block.rank_groups_raw, self.rank // block.rank_groups_raw,
+                                                     host.in_features, *host.kernel_size)))
+            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features,
+                                                    self.rank//block.rank_groups_raw, *([1]*len(host.kernel_size)))))
+
+        def forward(self, x):
+            return torch.prod(einsum(self.W_up, self.W_down, 'g o r ..., g r i ... -> g o i ...'), dim=0)
+
+        def feed_svd(self, U, V, weight):
+            self.W_up.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.W_down.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def get_collapsed_param(self):
+            w = torch.prod(einsum(self.W_up.data, self.W_down.data, 'g o r ..., g r i ... -> g o i ...'), dim=0)
+            b = None
+            return w, b
+
+layer_map={
+    'lora': LoraLayer,
+    'loha_group': LoraLayerGroup,
+    'loha': LohaLayer,
+}
```

### Comparing `hcpdiff-0.1.6/hcpdiff/models/plugin.py` & `hcpdiff-0.2.0/hcpdiff/models/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,112 +12,118 @@
 
 import torch
 from torch import nn
 import weakref
 
 class BasePluginBlock(nn.Module):
 
-    def forward(self, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+    def forward(self, host:nn.Module, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
         return fea_out
 
     def remove(self):
         pass
 
+    def feed_input_data(self, data):
+        self.input_data = data
+
+    def register_input_feeder_to(self, host_model):
+        if not hasattr(host_model, 'input_feeder'):
+            host_model.input_feeder = []
+        host_model.input_feeder.append(self.feed_input_data)
+
+    def set_hyper_params(self, **kwargs):
+        for k,v in kwargs.items():
+            setattr(self, k, v)
+
 class SinglePluginBlock(BasePluginBlock):
-    def __init__(self, layer:nn.Module):
+    def __init__(self, host:nn.Module, hook_param=None, host_model=None):
         super().__init__()
-        self.host = weakref.ref(layer)
+        self.host = weakref.ref(host)
 
-        self.hook_handle = layer.register_forward_hook(self.layer_hook)
+        if hook_param is None:
+            self.hook_handle = host.register_forward_hook(self.layer_hook)
+        else: # hook for model parameters
+            self.backup = getattr(host, hook_param)
+            self.target = hook_param
+            self.handle_pre = host.register_forward_pre_hook(self.pre_hook)
+            self.handle_post = host.register_forward_hook(self.post_hook)
 
     def layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
         return self(fea_in, fea_out)
 
-    def remove(self):
-        self.hook_handle.remove()
-
-class SinglePluginParameter(BasePluginBlock):
-    def __init__(self, layer:nn.Module, hook_target='weight'):
-        super().__init__()
-        self.host = weakref.ref(layer)
-        self.backup = getattr(layer, hook_target)
-        self.target = hook_target
-        self.handle_pre = layer.register_forward_pre_hook(self.pre_hook)
-        self.handle_post = layer.register_forward_hook(self.post_hook)
-
-    def forward(self, host_param: nn.Parameter):
-        return host_param
-
     def pre_hook(self, host, fea_in:torch.Tensor):
         host.weight_restored = False
         host_param = getattr(host, self.target)
         delattr(host, self.target)
         setattr(host, self.target, self(host_param))
         return fea_in
 
     def post_hook(self, host, fea_int, fea_out):
         if not getattr(host, 'weight_restored', False):
             setattr(host, self.target, self.backup)
             host.weight_restored = True
 
     def remove(self):
-        self.handle_pre.remove()
-        self.handle_post.remove()
+        if hasattr(self, 'hook_handle'):
+            self.hook_handle.remove()
+        else:
+            self.handle_pre.remove()
+            self.handle_post.remove()
 
 class PluginBlock(BasePluginBlock):
-    def __init__(self, from_layer:nn.Module, to_layer:nn.Module, pre_hook_to=False):
+    def __init__(self, from_layer:nn.Module, to_layer:nn.Module, pre_hook_to=False, host_model=None):
         super().__init__()
         self.host_from = weakref.ref(from_layer)
         self.host_to = weakref.ref(to_layer)
         #self.pre_hook_to = pre_hook_to
 
-        self.hook_handle_from = from_layer.register_forward_hook(self.from_layer_hook)
+        self.hook_handle_from = from_layer.register_forward_pre_hook(self.from_layer_hook)
         if pre_hook_to:
             self.hook_handle_to = to_layer.register_forward_pre_hook(self.to_layer_pre_hook)
         else:
             self.hook_handle_to = to_layer.register_forward_hook(self.to_layer_hook)
 
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        self.feat_from = fea_out
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor]):
+        self.feat_from = fea_in
 
     def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
         return self(self.feat_from, fea_out)
 
-    def to_layer_pre_hook(self, host, fea_in:torch.Tensor):
+    def to_layer_pre_hook(self, host, fea_in:Tuple[torch.Tensor]):
         return self(self.feat_from, fea_in)
 
     def remove(self):
         self.hook_handle_from.remove()
         self.hook_handle_to.remove()
 
 class MultiPluginBlock(BasePluginBlock):
-    def __init__(self, from_layers:List[nn.Module], to_layers:List[nn.Module], pre_hook_to=False):
+    def __init__(self, from_layers:List[nn.Module], to_layers:List[nn.Module], pre_hook_to=False, host_model=None):
         super().__init__()
         self.host_from = [weakref.ref(x) for x in from_layers]
         self.host_to = [weakref.ref(x) for x in to_layers]
 
         self.feat_from=[None for _ in range(len(from_layers))]
 
         self.hook_handle_from = []
         self.hook_handle_to = []
 
         for idx, layer in enumerate(from_layers):
-            handle_from = layer.register_forward_hook(lambda host, fea_in, fea_out:self.from_layer_hook(host, fea_in, fea_out, idx))
+            handle_from = layer.register_forward_pre_hook(lambda host, fea_in, idx=idx:self.from_layer_hook(host, fea_in, idx))
             self.hook_handle_from.append(handle_from)
         for idx, layer in enumerate(to_layers):
             if pre_hook_to:
-                handle_to = layer.register_forward_pre_hook(lambda host, fea_in:self.to_layer_pre_hook(host, fea_in, idx))
+                handle_to = layer.register_forward_pre_hook(lambda host, fea_in, idx=idx:self.to_layer_pre_hook(host, fea_in, idx))
             else:
-                handle_to = layer.register_forward_hook(lambda host, fea_in, fea_out:self.to_layer_hook(host, fea_in, fea_out, idx))
+                handle_to = layer.register_forward_hook(lambda host, fea_in, fea_out, idx=idx:self.to_layer_hook(host, fea_in, fea_out, idx))
             self.hook_handle_to.append(handle_to)
 
         self.record_count=0
 
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        self.feat_from[idx] = fea_out
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], idx: int):
+        self.feat_from[idx] = fea_in
         self.record_count+=1
         if self.record_count==len(self.feat_from): # call forward when all feat is record
             self.record_count = 0
             self.feat_to = self(self.feat_from)
 
     def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
         return self.feat_to[idx] + fea_out
```

### Comparing `hcpdiff-0.1.6/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.2.0/hcpdiff/models/text_emb_ex.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,55 @@
 ====================
     :Name:        hook for embedding
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
+from typing import Tuple
 
 import torch
 from torch import nn
 import os
 from loguru import logger
 from einops import rearrange, repeat
 
 from hcpdiff.utils.emb_utils import load_emb
+from .plugin import SinglePluginBlock
 
-class EmbeddingPTHook:
-    def __init__(self, token_embedding, N_word=75, N_repeats=3):
-        super().__init__()
-        self.token_embedding=token_embedding
-        token_embedding.forward_raw = token_embedding.forward
-        token_embedding.forward = self.forward
+class EmbeddingPTHook(SinglePluginBlock):
+    def __init__(self, token_embedding:nn.Module, N_word=75, N_repeats=3):
+        super().__init__(token_embedding)
+        token_embedding.emb_ex = self
+        self.handle_pre = token_embedding.register_forward_pre_hook(self.pre_hook)
 
         self.N_word=N_word
         self.N_repeats=N_repeats
+        self.num_embeddings=token_embedding.num_embeddings
         self.emb={}
+        self.emb_train=nn.ParameterList()
 
-    def add_emb(self, emb, token_id):
+    def add_emb(self, emb:nn.Parameter, token_id:int):
         self.emb[token_id]=emb
 
-    def forward(self, input_ids):
+    def pre_hook(self, host, input_ids: Tuple[torch.Tensor]):
+        self.input_ids = rearrange(input_ids[0], '(b r) w -> b (r w)', r=self.N_repeats)  # 兼容Attention mask
+        return self.input_ids.clip(0, self.num_embeddings-1)
+
+    def forward(self, fea_in:Tuple[torch.Tensor], inputs_embeds:torch.Tensor): # inputs_embeds:[B, N_word+2, N_emb]
         '''
         :param input_ids: [B, N_ids]
         :return: [B, N_repeat, N_word+2, N_emb]
         '''
-        input_ids=rearrange(input_ids, '(b r) w -> b (r w)', r=self.N_repeats) # 兼容Attention mask
-
-        rep_idxs_B = input_ids>=self.token_embedding.num_embeddings
-        inputs_embeds = self.token_embedding.forward_raw(input_ids.clip(0, self.token_embedding.num_embeddings-1)) # [B, N_word+2, N_emb]
-
+        rep_idxs_B = self.input_ids >= self.num_embeddings
         BOS = repeat(inputs_embeds[0,0,:], 'e -> r 1 e', r=self.N_repeats)
         EOS = repeat(inputs_embeds[0,-1,:], 'e -> r 1 e', r=self.N_repeats)
 
         replaced_embeds = []
-        for item, rep_idxs, ids_raw in zip(inputs_embeds, rep_idxs_B, input_ids):
+        for item, rep_idxs, ids_raw in zip(inputs_embeds, rep_idxs_B, self.input_ids):
             # insert pt to embeddings
             rep_idxs=torch.where(rep_idxs)[0]
             item_new=[]
             rep_idx_last=0
             for rep_idx in rep_idxs:
                 rep_idx=rep_idx.item()
                 item_new.append(item[rep_idx_last:rep_idx, :])
@@ -60,14 +63,18 @@
             replaced_item = torch.cat(item_new, dim=0)[1:self.N_word*self.N_repeats+1, :]
             replaced_item = rearrange(replaced_item, '(r w) e -> r w e', r=self.N_repeats, w=self.N_word)
             replaced_item = torch.cat([BOS, replaced_item, EOS], dim=1) # [N_repeat, N_word+2, N_emb]
 
             replaced_embeds.append(replaced_item)
         return torch.cat(replaced_embeds, dim=0) # [B*N_repeat, N_word+2, N_emb]
 
+    def remove(self):
+        super(EmbeddingPTHook, self).remove()
+        self.handle_pre.remove()
+
     @classmethod
     def hook(cls, ex_words_emb, tokenizer, text_encoder, log=False, **kwargs):
         word_list = list(ex_words_emb.keys())
         tokenizer.add_tokens(word_list)
         token_ids = tokenizer(' '.join(word_list)).input_ids[1:-1]
 
         embedding_hook = cls(text_encoder.text_model.embeddings.token_embedding, **kwargs)
@@ -76,10 +83,10 @@
             embedding_hook.add_emb(ex_words_emb[word], tid)
             if log:
                 logger.info(f'hook: {word}, len: {ex_words_emb[word].shape[0]}, id: {tid}')
         return embedding_hook
 
     @classmethod
     def hook_from_dir(cls, emb_dir, tokenizer, text_encoder, log=True, device='cuda:0', **kwargs):
-        ex_words_emb = {file[:-3]: nn.Parameter(load_emb(os.path.join(emb_dir, file)).to(device), requires_grad=True)
+        ex_words_emb = {file[:-3]: nn.Parameter(load_emb(os.path.join(emb_dir, file)).to(device), requires_grad=False)
                         for file in os.listdir(emb_dir) if file.endswith('.pt')}
         return cls.hook(ex_words_emb, tokenizer, text_encoder, log, **kwargs), ex_words_emb
```

### Comparing `hcpdiff-0.1.6/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.2.0/hcpdiff/models/textencoder_ex.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,42 +43,45 @@
             attention_mask = text_inputs.attention_mask.to(self.device)
         else:
             attention_mask = None
 
         prompt_embeds = self.text_enc(
             text_input_ids.to(self.device),
             attention_mask=attention_mask,
+            output_hidden_states=True,
         )
         return prompt_embeds
 
     def forward_hook_input(self, host, feat_in):
         feat_re = rearrange(feat_in[0], 'b (r w) -> (b r) w', r=self.N_repeats) # 使Attention mask的尺寸为N_word+2
         return (feat_re,) if len(feat_in)==1 else (feat_re, *feat_in[1:])
 
     def forward_hook(self, host, feat_in:Tuple[torch.Tensor], feat_out):
         if self.clip_skip>0:
-            encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip]
+            encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip-1]
             encoder_hidden_states = self.text_enc.text_model.final_layer_norm(encoder_hidden_states)
+            encoder_hidden_states += 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
         else:
-            encoder_hidden_states = feat_out[0]  # Get the text embedding for conditioning
+            encoder_hidden_states = feat_out['last_hidden_state']  # Get the text embedding for conditioning
 
         encoder_hidden_states = rearrange(encoder_hidden_states, '(b r) ... -> b r ...', r=self.N_repeats)  # [B, N_repeat, N_word+2, N_emb]
         BOS, EOS = encoder_hidden_states[:, 0, :1, :], encoder_hidden_states[:, -1, -1:, :]
         encoder_hidden_states = torch.cat([BOS, encoder_hidden_states[:, :, 1:-1, :].flatten(1, 2), EOS], dim=1)  # [B, N_repeat*N_word+2, N_emb]
 
         return encoder_hidden_states
 
     @staticmethod
     def mult_attn(prompt_embeds, attn_mult):
         if attn_mult!=None:
             for i, item in enumerate(attn_mult):
-                original_mean = prompt_embeds[i, :, :].mean()
-                prompt_embeds[i, 1:len(item) + 1, :] *= item.view(-1, 1).to(prompt_embeds.device)
-                new_mean = prompt_embeds[i, :, :].mean()
-                prompt_embeds[i] *= original_mean / new_mean
+                if len(item)>0:
+                    original_mean = prompt_embeds[i, ...].mean()
+                    prompt_embeds[i, 1:len(item) + 1, :] *= item.view(-1, 1).to(prompt_embeds.device)
+                    new_mean = prompt_embeds[i, ...].mean()
+                    prompt_embeds[i, ...] *= original_mean / new_mean
         return prompt_embeds
 
     def enable_xformers(self):
         try:
             from xformers.components import build_attention
             my_config = {
                 "name": 'scaled_dot_product',
@@ -123,9 +126,9 @@
 
             attn_output = layer.out_proj(attn_output)
 
             return attn_output, None
         layer.forward = forward
 
     @classmethod
-    def hook_pipe(cls, pipe, N_repeats=3):
-        return cls(pipe.text_encoder, pipe.tokenizer, N_repeats=N_repeats, device=pipe._execution_device)
+    def hook_pipe(cls, pipe, N_repeats=3, clip_skip=0):
+        return cls(pipe.text_encoder, pipe.tokenizer, N_repeats=N_repeats, device=pipe._execution_device, clip_skip=clip_skip)
```

### Comparing `hcpdiff-0.1.6/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.2.0/hcpdiff/models/tokenizer_ex.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         mult = 1.0
         mult_seq = []
         for token in token_seq:
             if token[0] == '{' or token[0] == '}':
                 mult *= next(mult_iter)
             else:
                 mult_seq.append(mult)
-        return torch.tensor(mult_seq)
+        return torch.tensor(mult_seq), clean_str
 
     def parse_attn_mult(self, text):
         if isinstance(text, str):
-            return [self.parse_attn_mult_one(text)]
+            mult_seq, clean_str = self.parse_attn_mult_one(text)
+            return [mult_seq], [clean_str]
         else:
-            return [self.parse_attn_mult_one(item) for item in text]
+            return list(zip(*[self.parse_attn_mult_one(item) for item in text]))
```

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.2.0/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.2.0/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.2.0/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/init_proj.py` & `hcpdiff-0.2.0/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/merge_model_part.py` & `hcpdiff-0.2.0/hcpdiff/tools/merge_model_part.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.2.0/hcpdiff/tools/sd2diffusers.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Conversion script for the LDM checkpoints. """
 
 import argparse
+import os.path
+
 import torch
 from transformers import CLIPTextModel
+from hcpdiff.utils.ckpt_manager import CkptManagerSafe, CkptManagerPKL
 
 import diffusers.pipelines.stable_diffusion.convert_from_ckpt as convert_from_ckpt
 try:
     from diffusers.pipelines.stable_diffusion.convert_from_ckpt import download_from_original_stable_diffusion_ckpt as load_sd_ckpt
 except:
     from diffusers.pipelines.stable_diffusion.convert_from_ckpt import load_pipeline_from_original_stable_diffusion_ckpt as load_sd_ckpt
 
@@ -170,12 +173,33 @@
         clip_stats_path=args.clip_stats_path,
         controlnet=args.controlnet,
     )
 
     if args.half:
         pipe.to(torch_dtype=torch.float16)
 
+    def replace(k_from, k_to, sd):
+        new_sd = {}
+        for k,v in sd.items():
+            if k.startswith(k_from):
+                new_sd[k_to+k[len(k_from):]]=v
+            else:
+                new_sd[k]=v
+        return new_sd
+
     if args.controlnet:
-        # only save the controlnet model
-        pipe.controlnet.save_pretrained(args.dump_path, safe_serialization=args.to_safetensors)
+        ckpt_manager = CkptManagerSafe() if args.to_safetensors else CkptManagerPKL()
+
+        sd_control = pipe.controlnet.state_dict()
+        sd_control = replace('controlnet_cond_embedding.conv_in', 'cond_head.0', sd_control)
+        for i in range(3):
+            sd_control = replace(f'controlnet_cond_embedding.blocks.{i*2}', f'cond_head.{2+i*4}', sd_control)
+            sd_control = replace(f'controlnet_cond_embedding.blocks.{i*2+1}', f'cond_head.{4+i*4}', sd_control)
+        sd_control = replace('controlnet_cond_embedding.conv_out', 'cond_head.14', sd_control)
+        sd_control = {f'___.{k}':v for k,v in sd_control.items()} # Add placeholder for plugin
+        os.makedirs(args.dump_path, exist_ok=True)
+        ckpt_manager._save_ckpt(sd_control, None, None, save_path=os.path.join(args.dump_path,
+                                    f'controlnet.{"safetensors" if args.to_safetensors else "ckpt"}'))
     else:
-        pipe.save_pretrained(args.dump_path, safe_serialization=args.to_safetensors)
+        pipe.save_pretrained(args.dump_path, safe_serialization=args.to_safetensors)
+
+    #python -m hcpdiff.tools.sd2diffusers --checkpoint_path test/control_sd15_canny.pth --original_config_file test/config.yaml --dump_path test/ckpt/control --controlnet
```

### Comparing `hcpdiff-0.1.6/hcpdiff/train_ac.py` & `hcpdiff-0.2.0/hcpdiff/train_ac.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 import itertools
 import os
 import sys
 
 import torch
 import torch.utils.checkpoint
 import transformers
-from accelerate import Accelerator
+from accelerate import Accelerator, DistributedDataParallelKwargs
 from accelerate.utils import set_seed
 from transformers import AutoTokenizer
 from omegaconf import OmegaConf
 import hydra
 from loguru import logger
 import time
 
 import diffusers
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 
 from hcpdiff.data import TextImagePairDataset, RatioBucket
-from hcpdiff.utils.utils import get_scheduler, import_model_class_from_model_name_or_path, cycle_data,\
-    load_config_with_cli, get_cfg_range, var_get
+from hcpdiff.utils.utils import cycle_data, load_config_with_cli, get_cfg_range
+from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
 from hcpdiff.utils.ema import ModelEMA
 from hcpdiff.utils.cfg_net_tools import make_hcpdiff
 from hcpdiff.utils.emb_utils import load_emb
 from hcpdiff.data import collate_fn_ft
 from hcpdiff.visualizer import Visualizer
 from hcpdiff.utils.ckpt_manager import CkptManagerPKL, CkptManagerSafe
@@ -49,19 +49,19 @@
 
         if self.is_local_main_process:
             self.exp_dir = os.path.join(self.cfgs.exp_dir, f'{time.strftime("%Y-%m-%d-%H-%M-%S")}')
             os.makedirs(os.path.join(self.exp_dir, 'ckpts/'), exist_ok=True)
             logger.add(os.path.join(self.exp_dir, 'train.log'))
             with open(os.path.join(self.exp_dir, 'cfg.yaml'), 'w', encoding='utf-8') as f:
                 f.write(OmegaConf.to_yaml(cfgs_raw))
+        else:
+            logger.disable("__main__")
 
-        logger.info(f'rank: {self.local_rank}')
-        if self.is_local_main_process:
-            logger.info(f'world_size: {self.world_size}')
-            logger.info(f'accumulation: {self.cfgs.train.gradient_accumulation_steps}')
+        logger.info(f'world_size: {self.world_size}')
+        logger.info(f'accumulation: {self.cfgs.train.gradient_accumulation_steps}')
 
         if self.is_local_main_process:
             transformers.utils.logging.set_verbosity_warning()
             diffusers.utils.logging.set_verbosity_warning()
         else:
             transformers.utils.logging.set_verbosity_error()
             diffusers.utils.logging.set_verbosity_error()
@@ -69,14 +69,15 @@
         self.lr=1e-5 # no usage, place set lr in cfgs
         self.train_TE = (cfgs.text_encoder is not None) or (cfgs.lora_text_encoder is not None)
 
         self.build_ckpt_manager()
         self.build_model()
         self.make_hooks()
         self.config_model()
+        self.cache_latents=False
         self.train_loader, self.arb_ist=self.build_data(cfgs.data)
         if cfgs.data_class is None:
             self.train_loader_class=None # without DreamBooth
         else:
             self.train_loader_class, self.arb_class=self.build_data(cfgs.data_class)
         if self.cache_latents:
             self.vae = self.vae.to('cpu')
@@ -104,35 +105,38 @@
         return self.accelerator.device
 
     @property
     def is_local_main_process(self):
         return self.accelerator.is_local_main_process
 
     def init_context(self, cfgs_raw):
+        ddp_kwargs = DistributedDataParallelKwargs(broadcast_buffers=False)
         self.accelerator = Accelerator(
             gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
             mixed_precision=self.cfgs.mixed_precision,
             step_scheduler_with_optimizer=False,
+            kwargs_handlers=[ddp_kwargs], # fix inplace bug in DDP while use data_class
         )
 
         self.local_rank = int(os.environ.get("LOCAL_RANK", -1))
         self.world_size = self.accelerator.num_processes
 
         set_seed(self.cfgs.seed + self.local_rank)
 
     def prepare(self):
         # Prepare everything with accelerator.
-        prepare_obj_list = [self.unet, self.train_loader]
-        prepare_name_list = ['unet', 'train_loader']
+        if self.train_TE:
+            prepare_obj_list = [self.TE_unet, self.train_loader]
+            prepare_name_list = ['TE_unet', 'train_loader']
+        else:
+            prepare_obj_list = [self.unet, self.train_loader]
+            prepare_name_list = ['unet', 'train_loader']
         if hasattr(self, 'optimizer'):
             prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
             prepare_name_list.extend(['optimizer', 'lr_scheduler'])
-        if self.train_TE:
-            prepare_obj_list.append(self.text_encoder)
-            prepare_name_list.append('text_encoder')
         if hasattr(self, 'optimizer_pt'):
             prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
             prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
 
         prepared_obj = self.accelerator.prepare(*prepare_obj_list)
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
@@ -164,41 +168,45 @@
         self.build_unet_and_TE()
 
     def build_unet_and_TE(self): # for easy to use colossalAI
         self.unet = UNet2DConditionModel.from_pretrained(
             self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision
         )
         # import correct text encoder class
-        text_encoder_cls = import_model_class_from_model_name_or_path(self.cfgs.model.pretrained_model_name_or_path,
-                                                                      self.cfgs.model.revision)
+        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path, self.cfgs.model.revision)
         self.text_encoder = text_encoder_cls.from_pretrained(
             self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
         )
 
+        if self.train_TE:
+            # Wrap unet and text_encoder to make DDP happy. Multiple DDP has soooooo many fxxking bugs!
+            self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
+
 
     def build_ema(self):
         if self.cfgs.model.ema_unet>0:
             self.ema_unet = ModelEMA(self.unet.named_parameters(), self.cfgs.model.ema_unet)
         if self.train_TE and self.cfgs.model.ema_text_encoder>0:
             self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
 
     def build_ckpt_manager(self):
         if self.cfgs.ckpt_type=='torch':
             self.ckpt_manager = CkptManagerPKL()
         elif self.cfgs.ckpt_type=='safetensors':
             self.ckpt_manager = CkptManagerSafe()
         else:
             raise NotImplementedError(f'Not support ckpt type: {self.cfgs.ckpt_type}')
-        self.ckpt_manager.set_save_dir(os.path.join(self.exp_dir, 'ckpts'), emb_dir=self.cfgs.tokenizer_pt.emb_dir)
+        if self.is_local_main_process:
+            self.ckpt_manager.set_save_dir(os.path.join(self.exp_dir, 'ckpts'), emb_dir=self.cfgs.tokenizer_pt.emb_dir)
 
     def get_unet_raw(self):
-        return self.unet.module
+        return self.TE_unet.module.unet if self.train_TE else self.unet.module
 
     def get_text_encoder_raw(self):
-        return self.text_encoder.module if self.train_TE else self.text_encoder
+        return self.TE_unet.module.TE if self.train_TE else self.text_encoder
 
     def config_model(self):
         if self.cfgs.model.enable_xformers:
             if is_xformers_available():
                 self.unet.enable_xformers_memory_efficient_attention()
                 #self.text_enc_hook.enable_xformers()
             else:
@@ -220,32 +228,33 @@
         if self.cfgs.mixed_precision == "fp16":
             weight_dtype = torch.float16
         elif self.cfgs.mixed_precision == "bf16":
             weight_dtype = torch.bfloat16
         self.weight_dtype = weight_dtype
 
         # Move vae and text_encoder to device and cast to weight_dtype
-        self.vae.to(self.device, dtype=weight_dtype)
+        self.vae = self.vae.to(self.device, dtype=weight_dtype)
         if not self.train_TE:
-            self.text_encoder.to(self.device, dtype=weight_dtype)
+            self.text_encoder = self.text_encoder.to(self.device, dtype=weight_dtype)
 
     @torch.no_grad()
     def load_resume(self):
         if self.cfgs.train.resume is not None:
             for ckpt in self.cfgs.train.resume.ckpt_path.unet:
-                self.ckpt_manager.load_ckpt_to_model(self.unet, ckpt, model_ema=var_get(self, 'ema_unet', None))
+                self.ckpt_manager.load_ckpt_to_model(self.unet, ckpt, model_ema=getattr(self, 'ema_unet', None))
             for ckpt in self.cfgs.train.resume.ckpt_path.TE:
-                self.ckpt_manager.load_ckpt_to_model(self.text_encoder, ckpt, model_ema=var_get(self, 'ema_text_encoder', None))
+                self.ckpt_manager.load_ckpt_to_model(self.text_encoder, ckpt, model_ema=getattr(self, 'ema_text_encoder', None))
             for name, ckpt in self.cfgs.train.resume.ckpt_path.words:
                 self.ex_words_emb[name].data = load_emb(ckpt)
 
     def make_hooks(self):
         # Hook tokenizer and embedding to support pt
         self.embedding_hook, self.ex_words_emb = EmbeddingPTHook.hook_from_dir(
-                        self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
+                        self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, log=self.is_local_main_process,
+                        N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
 
         self.text_enc_hook = TEEXHook(self.text_encoder, self.tokenizer, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device,
                                       clip_skip=self.cfgs.model.clip_skip)
 
     def build_data(self, cfg_data):
         train_dataset = TextImagePairDataset(cfg_data, self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
         if isinstance(train_dataset.bucket, RatioBucket):
@@ -253,15 +262,15 @@
             train_dataset.bucket.make_arb(cfg_data.batch_size*self.world_size)
         else:
             arb=False
         logger.info(f"len(train_dataset): {len(train_dataset)}")
 
         if cfg_data.cache_latents:
             self.cache_latents = True
-            train_dataset.cache_latents(self.vae, self.weight_dtype)
+            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
 
         # Pytorch Data loader
         train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
                                                                         rank=self.local_rank, shuffle=not arb)
         train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=cfg_data.batch_size,
             num_workers=self.cfgs.train.workers, sampler=train_sampler, collate_fn=collate_fn_ft)
         return train_loader, arb
@@ -285,14 +294,15 @@
         # params for embedding
         train_params_emb = []
         self.train_pts = {}
         if self.cfgs.tokenizer_pt.train is not None:
             for v in self.cfgs.tokenizer_pt.train:
                 self.train_pts[v.name]=self.ex_words_emb[v.name]
                 self.ex_words_emb[v.name].requires_grad=True
+                self.embedding_hook.emb_train.append(self.ex_words_emb[v.name])
                 train_params_emb.append({'params':self.ex_words_emb[v.name], 'lr':v.lr})
 
         return train_params_unet + train_params_text_encoder, train_params_emb
 
     def build_optimizer_scheduler(self):
         # set optimizer
         parameters, parameters_pt = self.get_param_group_train()
@@ -344,24 +354,27 @@
             loss_sum+=loss
 
             self.global_step += 1
             if self.is_local_main_process:
                 if self.global_step % self.cfgs.train.save_step == 0:
                     self.save_model()
                 if self.global_step % self.cfgs.train.log_step == 0:
-                    logger.info('Step [{}/{}], LR {:.2e}, Loss: {:.5f}'
+                    lr_model = self.lr_scheduler.get_last_lr()[0] if hasattr(self, 'lr_scheduler') else 0.
+                    lr_word = self.lr_scheduler_pt.get_last_lr()[0] if hasattr(self, 'lr_scheduler_pt') else 0.
+                    logger.info('Step [{}/{}], LR_model: {:.2e}, LR_word: {:.2e}, Loss: {:.5f}'
                                 .format(self.global_step, self.cfgs.train.scheduler.num_training_steps,
-                                        self.lr_scheduler.get_last_lr()[0], loss_sum / self.cfgs.train.log_step))
+                                        lr_model, lr_word, loss_sum / self.cfgs.train.log_step))
                     loss_sum = 0
 
             if self.global_step >= self.cfgs.train.scheduler.num_training_steps:
                 break
 
         self.wait_for_everyone()
-        self.save_model()
+        if self.is_local_main_process:
+            self.save_model()
 
     def wait_for_everyone(self):
         self.accelerator.wait_for_everyone()
 
     @torch.no_grad()
     def get_latents(self, image, dataset):
         if dataset.latents is None:
@@ -380,17 +393,20 @@
         timesteps = timesteps.long()
 
         # Add noise to the latents according to the noise magnitude at each timestep
         # (this is the forward diffusion process)
         return self.noise_scheduler.add_noise(latents, noise, timesteps), noise, timesteps
 
     def encode_decode(self, prompt_ids, noisy_latents, timesteps):
-        # for colossalAI support
-        encoder_hidden_states = self.text_encoder(prompt_ids)  # Get the text embedding for conditioning
-        model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
+        # for DDP support
+        if self.train_TE:
+            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps)
+        else:
+            encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
+            model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
         return model_pred
 
     def forward(self, latents, prompt_ids):
         noisy_latents, noise, timesteps = self.make_noise(latents)
 
         # CFG context for DreamArtist
         noisy_latents, timesteps = self.cfg_context.pre(noisy_latents, timesteps)
@@ -412,29 +428,31 @@
         att_mask = att_mask.to(self.device)
         prompt_ids=prompt_ids.to(self.device)
         with self.accelerator.accumulate(self.unet):
             latents = self.get_latents(image, self.train_loader.dataset)
             model_pred, target = self.forward(latents, prompt_ids)
 
             if self.train_loader_class is not None:
+                loss = self.get_loss(model_pred, target, att_mask) # Compute instance loss
+                self.accelerator.backward(loss)
+
                 #DreamBooth prior forward
                 image_cls, att_mask_cls, prompt_ids_cls = next(self.data_iter_class)
                 image_cls = image_cls.to(self.device, dtype=self.weight_dtype)
                 att_mask_cls = att_mask_cls.to(self.device)
                 prompt_ids_cls = prompt_ids_cls.to(self.device)
                 latents_cls = self.get_latents(image_cls, self.train_loader_class.dataset)
                 model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls)
 
-                loss = self.get_loss(model_pred, target, att_mask) # Compute instance loss
                 prior_loss = self.get_loss(model_pred_prior, target_prior, att_mask_cls) # Compute prior loss
-                loss = loss + self.cfgs.train.loss.prior_loss_weight * prior_loss
+                loss = self.cfgs.train.loss.prior_loss_weight * prior_loss
+                self.accelerator.backward(loss)
             else:
                 loss = self.get_loss(model_pred, target, att_mask)
-
-            self.accelerator.backward(loss)
+                self.accelerator.backward(loss)
 
             if hasattr(self, 'optimizer'):
                 if self.accelerator.sync_gradients: # fine-tuning
                     params_to_clip = (
                         itertools.chain(self.unet.parameters(), self.text_encoder.parameters())
                         if self.train_TE else self.unet.parameters()
                     )
@@ -448,30 +466,35 @@
                 self.lr_scheduler_pt.step()
                 self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
 
             self.update_ema()
         return loss.item()
 
     def get_loss(self, model_pred, target, att_mask):
-        return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
+        if len(self.embedding_hook.emb_train)>0:
+            return (self.criterion(model_pred.float(), target.float()) * att_mask).mean() \
+               + 0*sum(self.embedding_hook.emb_train).mean() # avoid unused parameters, make gradient checkpointing happy
+        else:
+            return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
             self.ema_unet.step(self.get_unet_raw().named_parameters())
         if hasattr(self, 'ema_text_encoder'):
             self.ema_text_encoder.step(self.get_text_encoder_raw().named_parameters())
 
     def save_model(self, from_raw=False):
         unet_raw=self.get_unet_raw()
-        self.ckpt_manager.save_model_with_lora(unet_raw, self.lora_unet, model_ema=var_get(self, 'ema_unet', None),
+        self.ckpt_manager.save_model_with_lora(unet_raw, self.lora_unet, model_ema=getattr(self, 'ema_unet', None),
                                                name='unet', step=self.global_step)
         if self.train_TE:
             TE_raw = self.get_text_encoder_raw()
-            self.ckpt_manager.save_model_with_lora(TE_raw, self.lora_TE, model_ema=var_get(self, 'ema_text_encoder', None),
-                                                   name='text_encoder', step=self.global_step)
+            # exclude_key: embeddings should not save with text-encoder
+            self.ckpt_manager.save_model_with_lora(TE_raw, self.lora_TE, model_ema=getattr(self, 'ema_text_encoder', None),
+                                                   name='text_encoder', step=self.global_step, exclude_key='emb_ex.')
 
         if self.DA_lora:
             self.ckpt_manager.save_model_with_lora(None, self.lora_unet_neg, name='unet-neg', step=self.global_step)
             if self.train_TE:
                 self.ckpt_manager.save_model_with_lora(None, self.lora_TE_neg, name='text_encoder-neg', step=self.global_step)
 
         self.ckpt_manager.save_embedding(self.train_pts, self.global_step, self.cfgs.tokenizer_pt.replace)
```

### Comparing `hcpdiff-0.1.6/hcpdiff/train_colo.py` & `hcpdiff-0.2.0/hcpdiff/train_colo.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,16 @@
 from colossalai.nn.parallel.utils import get_static_torch_model
 from colossalai.utils import get_current_device
 from colossalai.utils.model.colo_init_context import ColoInitContext
 
 from hcpdiff.train_ac import Trainer, get_scheduler, ModelEMA
 from diffusers import UNet2DConditionModel
 from hcpdiff.utils.colo_utils import gemini_zero_dpp, GeminiAdamOptimizerP
-from hcpdiff.utils.utils import import_model_class_from_model_name_or_path, load_config_with_cli
-
-class TEUnetWapper(nn.Module):
-    def __init__(self, unet, TE):
-        super().__init__()
-        self.unet = unet
-        self.TE = TE
-
-    def forward(self, prompt_ids, noisy_latents, timesteps):
-        encoder_hidden_states = self.TE(prompt_ids)  # Get the text embedding for conditioning
-        model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
-        return model_pred
+from hcpdiff.utils.utils import load_config_with_cli
+from hcpdiff.utils.net_utils import import_text_encoder_class, TEUnetWrapper
 
 class TrainerColo(Trainer):
     def init_context(self, cfgs_raw):
         # If passed along, set the training seed now.
         if self.cfgs.seed is None:
             colossalai.launch_from_torch(config='./config.py')
         else:
@@ -61,25 +51,26 @@
         pass
 
     def wait_for_everyone(self):
         torch.cuda.synchronize()
 
     def build_unet_and_TE(self):
         # import correct text encoder class
-        text_encoder_cls = import_model_class_from_model_name_or_path(self.cfgs.model.pretrained_model_name_or_path,
-                                                                      self.cfgs.model.revision)
+        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path,
+                                                     self.cfgs.model.revision)
         with ColoInitContext(device=self.device):
             self.unet = UNet2DConditionModel.from_pretrained(
                 self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision,
                 low_cpu_mem_usage=False
             )
             if self.train_TE:
                 self.text_encoder = text_encoder_cls.from_pretrained(
                     self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
                 )
+                self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
         if not self.train_TE:
             self.text_encoder = text_encoder_cls.from_pretrained(
                 self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
             )
 
     def build_ema(self):
         if self.cfgs.model.ema_unet>0:
@@ -94,15 +85,15 @@
         self.lora_unet.set_inplace(False)
         if self.DA_lora:
             self.lora_unet_neg.set_inplace(False)
         if self.train_TE:
             self.lora_TE.set_inplace(False)
             if self.DA_lora:
                 self.lora_TE_neg.set_inplace(False)
-            self.TE_unet = gemini_zero_dpp(TEUnetWapper(self.unet, self.text_encoder))
+            self.TE_unet = gemini_zero_dpp(self.TE_unet)
         else:
             self.unet = gemini_zero_dpp(self.unet)
         return params
 
     def build_optimizer_scheduler(self):
         # set optimizer
         parameters, parameters_pt = self.get_param_group_train()
@@ -119,21 +110,14 @@
         if len(parameters_pt)>0: # do prompt-tuning
             if self.cfgs.train.scale_lr_pt:
                 self.scale_lr(parameters_pt)
 
             self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
             self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
 
-    def encode_decode(self, prompt_ids, noisy_latents, timesteps):
-        if self.train_TE:
-            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps)
-        else:
-            model_pred = super(TrainerColo, self).encode_decode(prompt_ids, noisy_latents, timesteps)
-        return model_pred
-
     def train_one_step(self, image, att_mask, prompt_ids):
         torch.cuda.reset_peak_memory_stats()
         image = image.to(self.device, dtype=self.weight_dtype, non_blocking=True)
         att_mask = att_mask.to(self.device, non_blocking=True)
         prompt_ids = prompt_ids.to(self.device, non_blocking=True)
 
         latents = self.get_latents(image, self.train_loader.dataset)
```

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.2.0/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_pkl.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,43 +7,60 @@
     :Created:     8/04/2023
     :Licence:     MIT
 """
 
 import torch
 from torch import nn
 import os
-from hcpdiff.models.lora import LoraBlock, LoraGroup, split_state
+from hcpdiff.models.lora_base import LoraBlock, LoraGroup, split_state
 from hcpdiff.utils.emb_utils import save_emb
 
 class CkptManagerPKL:
     def __init__(self, lora_from_raw=False):
         self.lora_from_raw = lora_from_raw
 
     def set_save_dir(self, save_dir, emb_dir=None):
         os.makedirs(save_dir, exist_ok=True)
         self.save_dir = save_dir
         self.emb_dir = emb_dir
 
-    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name, step, model_ema=None):
+    def exclude_state(self, state, key):
+        if key is None:
+            return state
+        else:
+            return {k:v for k,v in state.items() if key in k}
+
+    def save_model(self, model: nn.Module, name, step, model_ema=None, exclude_key=None):
+        sd_model = {
+            'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
+        }
+        if model_ema is not None:
+            sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
+            sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
+        self._save_ckpt(sd_model, name, step)
+
+    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name, step, model_ema=None,
+                             exclude_key=None):
         sd_model = {
-            'base': LoraBlock.extract_trainable_state_without_lora(model),
+            'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
         } if model is not None else {}
         if not lora_blocks.empty():
             sd_model['lora']=lora_blocks.state_dict(model if self.lora_from_raw else None)
 
         if model_ema is not None:
             sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
-            sd_model['base_ema'] = sd_ema
+            sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
             if not lora_blocks.empty():
                 sd_model['lora_ema'] = {sd_ema_lora[k] for k in sd_model['lora'].keys()}
 
         self._save_ckpt(sd_model, name, step)
 
-    def _save_ckpt(self, sd_model, name, step):
-        save_path = os.path.join(self.save_dir, f"{name}-{step}.ckpt")
+    def _save_ckpt(self, sd_model, name, step, save_path=None):
+        if save_path is None:
+            save_path = os.path.join(self.save_dir, f"{name}-{step}.ckpt")
         torch.save(sd_model, save_path)
 
     def load_ckpt(self, ckpt_path, map_location='cpu'):
         return torch.load(ckpt_path, map_location=map_location)
 
     def load_ckpt_to_model(self, model:nn.Module, ckpt_path, model_ema=None):
         sd = self.load_ckpt(ckpt_path)
```

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from safetensors import safe_open
 from safetensors.torch import save_file
 
 from .ckpt_pkl import CkptManagerPKL
 
 class CkptManagerSafe(CkptManagerPKL):
 
-    def _save_ckpt(self, sd_model, name, step):
-        save_path = os.path.join(self.save_dir, f"{name}-{step}.safetensors")
+    def _save_ckpt(self, sd_model, name, step, save_path=None):
+        if save_path is None:
+            save_path = os.path.join(self.save_dir, f"{name}-{step}.safetensors")
         sd_unfold = self.unfold_dict(sd_model)
         save_file(sd_unfold, save_path)
 
     def load_ckpt(self, ckpt_path, map_location='cpu'):
         with safe_open(ckpt_path, framework="pt", device=map_location) as f:
             sd_fold = self.fold_dict(f)
         return sd_fold
```

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.2.0/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/ema.py` & `hcpdiff-0.2.0/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.2.0/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/hcpdiff/utils/utils.py` & `hcpdiff-0.2.0/hcpdiff/utils/net_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,34 @@
-import os.path
-from typing import Optional, Union
+from typing import Optional, Union, Tuple, Dict, Callable
 
-import re
-import torch
 from torch import nn
 from torch.optim import lr_scheduler
 from diffusers.optimization import SchedulerType, TYPE_TO_SCHEDULER_FUNCTION, Optimizer
-from omegaconf import OmegaConf
 from transformers import PretrainedConfig
+from collections import OrderedDict
 
-def str2bool(v):
-    return v.lower() in ("yes", "true", "t", "1")
+class TEUnetWrapper(nn.Module):
+    def __init__(self, unet, TE):
+        super().__init__()
+        self.unet = unet
+        self.TE = TE
+
+    def forward(self, prompt_ids, noisy_latents, timesteps, **kwargs):
+        input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
+
+        if hasattr(self.TE, 'input_feeder'):
+            for feeder in self.TE.input_feeder:
+                feeder(input_all)
+        if hasattr(self.unet, 'input_feeder'):
+            for feeder in self.unet.input_feeder:
+                feeder(input_all)
+
+        encoder_hidden_states = self.TE(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
+        model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
+        return model_pred
 
 def get_scheduler(
     name: Union[str, SchedulerType],
     optimizer: Optimizer,
     num_warmup_steps: Optional[int] = None,
     num_training_steps: Optional[int] = None,
     scheduler_kwargs = {},
@@ -71,64 +85,15 @@
     if name == SchedulerType.POLYNOMIAL:
         return schedule_func(
             optimizer, num_warmup_steps=num_warmup_steps, num_training_steps=num_training_steps, **scheduler_kwargs
         )
 
     return schedule_func(optimizer, num_warmup_steps=num_warmup_steps, num_training_steps=num_training_steps, **scheduler_kwargs)
 
-def low_rank_approximate(weight, rank, clamp_quantile=0.99):
-    if len(weight.shape)==4: # conv
-        weight=weight.flatten(1)
-        out_ch, in_ch, k1, k2 = weight.shape
-
-    U, S, Vh = torch.linalg.svd(weight)
-    U = U[:, :rank]
-    S = S[:rank]
-    U = U @ torch.diag(S)
-
-    Vh = Vh[:rank, :]
-
-    dist = torch.cat([U.flatten(), Vh.flatten()])
-    hi_val = torch.quantile(dist, clamp_quantile)
-    low_val = -hi_val
-
-    U = U.clamp(low_val, hi_val)
-    Vh = Vh.clamp(low_val, hi_val)
-
-    if len(weight.shape) == 4:
-        # U is (out_channels, rank) with 1x1 conv.
-        U = U.reshape(U.shape[0], U.shape[1], 1, 1)
-        # V is (rank, in_channels * kernel_size1 * kernel_size2)
-        Vh = Vh.reshape(Vh.shape[0], in_ch, k1, k2)
-    return U, Vh
-
-def load_config(path):
-    cfg = OmegaConf.load(path)
-    if '_base_' in cfg:
-        for base in cfg['_base_']:
-            cfg = OmegaConf.merge(load_config(base), cfg)
-        del cfg['_base_']
-    return cfg
-
-def load_config_with_cli(path, args_list=None):
-    cfg = load_config(path)
-    cfg_cli = OmegaConf.from_cli(args_list)
-    cfg = OmegaConf.merge(cfg, cfg_cli)
-    return cfg
-
-def _default(v, default):
-    return default if v is None else v
-
-def dict_get(data, key, default):
-    return data[key] if key in data else default
-
-def var_get(data, key, default):
-    return getattr(data, key) if hasattr(data, key) else default
-
-def import_model_class_from_model_name_or_path(pretrained_model_name_or_path: str, revision: str):
+def import_text_encoder_class(pretrained_model_name_or_path: str, revision: str):
     text_encoder_config = PretrainedConfig.from_pretrained(
         pretrained_model_name_or_path,
         subfolder="text_encoder",
         revision=revision,
     )
     model_class = text_encoder_config.architectures[0]
 
@@ -139,42 +104,23 @@
     elif model_class == "RobertaSeriesModelWithTransformation":
         from diffusers.pipelines.alt_diffusion.modeling_roberta_series import RobertaSeriesModelWithTransformation
 
         return RobertaSeriesModelWithTransformation
     else:
         raise ValueError(f"{model_class} is not supported.")
 
-def cycle_data(data_loader, arb=False):
-    epoch=0
-    while True:
-        if arb:
-            data_loader.dataset.bucket.rest(epoch)
-        for data in data_loader:
-            yield data
-        epoch+=1
-
-def get_cfg_range(cfg_text:str):
-    dy_cfg_f='ln'
-    if cfg_text.find(':')!=-1:
-        cfg_text, dy_cfg_f = cfg_text.split(':')
-
-    if cfg_text.find('-')!=-1:
-        l, h = cfg_text.split('-')
-        return float(l), float(h), dy_cfg_f
-    else:
-        return float(cfg_text), float(cfg_text), dy_cfg_f
-
-def to_validate_file(name):
-    rstr = r"[\/\\\:\*\?\"\<\>\|]"  # '/ \ : * ? " < > |'
-    new_title = re.sub(rstr, "_", name)  # 替换为下划线
-    return new_title
-
-def make_mask(start, end, length):
-    mask=torch.zeros(length)
-    mask[int(length*start):int(length*end)]=1
-    return mask.bool()
-
-def get_file_name(file: str):
-    return file.rsplit('.',1)[0]
-
-def get_file_ext(file: str):
-    return file.rsplit('.',1)[1].lower()
+def remove_all_hooks(model: nn.Module) -> None:
+    for name, child in model.named_modules():
+        if hasattr(child, "_forward_hooks"):
+            child._forward_hooks: Dict[int, Callable] = OrderedDict()
+        elif hasattr(child, "_forward_pre_hooks"):
+            child._forward_pre_hooks: Dict[int, Callable] = OrderedDict()
+        elif hasattr(child, "_backward_hooks"):
+            child._backward_hooks: Dict[int, Callable] = OrderedDict()
+
+def remove_layers(model: nn.Module, layer_class):
+    named_modules = {k: v for k, v in model.named_modules()}
+    for k,v in named_modules.items():
+        if isinstance(v, layer_class):
+            parent, name = named_modules[k.rsplit('.', 1)]
+            delattr(parent, name)
+            del v
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hcpdiff-0.1.6/hcpdiff/visualizer.py` & `hcpdiff-0.2.0/hcpdiff/visualizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,136 @@
 import argparse
 import os
 import sys
 
 import hydra
 import torch
-from diffusers import StableDiffusionPipeline
+from diffusers import StableDiffusionPipeline, StableDiffusionImg2ImgPipeline, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
+from diffusers.utils import PIL_INTERPOLATION
 from matplotlib import pyplot as plt
 from omegaconf import OmegaConf
 
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook
-from hcpdiff.utils.cfg_net_tools import load_hcpdiff
-from hcpdiff.utils.utils import to_validate_file, load_config_with_cli
+from hcpdiff.utils.cfg_net_tools import load_hcpdiff, make_plugin
+from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config
+from hcpdiff.utils.img_size_tool import types_support
+from torch.cuda.amp import autocast
+from PIL import Image
+import numpy as np
+
+class UnetHook(): # for controlnet
+    def __init__(self, unet):
+        self.unet = unet
+        self.call_raw = UNet2DConditionModel.__call__
+        UNet2DConditionModel.__call__ = self.unet_call
 
+    def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
+        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states, **kwargs)
 
 class Visualizer:
     def __init__(self, cfgs):
         self.cfgs_raw = cfgs
         self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
-        self.cfg_merge = cfgs.merge
+        self.cfg_merge = self.cfgs.merge
 
-        comp = StableDiffusionPipeline.from_pretrained(cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False).components
-        comp.update(cfgs.new_components)
-        self.pipe = StableDiffusionPipeline(**comp)
+        pipeline = self.get_pipeline()
+        comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False).components
+        comp.update(self.cfgs.new_components)
+        self.pipe = pipeline(**comp)
 
         if self.cfg_merge:
             self.merge_model()
 
         self.pipe = self.pipe.to("cuda")
-        emb, _ = EmbeddingPTHook.hook_from_dir(cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=cfgs.N_repeats)
-        self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=cfgs.N_repeats)
+        emb, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=self.cfgs.N_repeats)
+        self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=self.cfgs.N_repeats, clip_skip=self.cfgs.clip_skip)
         self.token_ex = TokenizerHook(self.pipe.tokenizer)
+        UnetHook(self.pipe.unet)
 
         if is_xformers_available():
             self.pipe.unet.enable_xformers_memory_efficient_attention()
             # self.te_hook.enable_xformers()
 
+    def get_pipeline(self):
+        if self.cfgs.condition is None:
+            return StableDiffusionPipeline
+        else:
+            if self.cfgs.condition.type=='i2i':
+                return StableDiffusionImg2ImgPipeline
+            elif self.cfgs.condition.type=='controlnet':
+                return StableDiffusionPipeline
+            else:
+                raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
+
     def merge_model(self):
+        if 'plugin_cfg' in self.cfg_merge: # Build plugins
+            plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
+            make_plugin(self.pipe.unet, plugin_cfg.plugin)
+
         for cfg_group in self.cfg_merge.values():
             if hasattr(cfg_group, 'type'):
                 if cfg_group.type == 'unet':
                     load_hcpdiff(self.pipe.unet, cfg_group)
                 elif cfg_group.type == 'TE':
                     load_hcpdiff(self.pipe.text_encoder, cfg_group)
 
     def set_scheduler(self, scheduler):
         self.pipe.scheduler = scheduler
 
+    def prepare_cond_image(self, image, width, height, batch_size, device):
+        if not isinstance(image, torch.Tensor):
+            if isinstance(image, Image.Image):
+                image = [image]
+
+            if isinstance(image[0], Image.Image):
+                image = [
+                    np.array(i.resize((width, height), resample=PIL_INTERPOLATION["lanczos"]))[None, :] for i in image
+                ]
+                image = np.concatenate(image, axis=0)
+                image = np.array(image).astype(np.float32) / 255.0
+                image = image.transpose(0, 3, 1, 2)
+                image = torch.from_numpy(image)
+            elif isinstance(image[0], torch.Tensor):
+                image = torch.cat(image, dim=0)
+
+        image = image.repeat_interleave(batch_size, dim=0)
+        image = image.to(device=device)
+
+        return image
+
+    def get_ex_input(self):
+        ex_input_dict = {}
+        if self.cfgs.condition is not None:
+            img = Image.open(self.cfgs.condition.image).convert('RGB')
+            ex_input_dict['cond'] = self.prepare_cond_image(img, self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda')
+        return ex_input_dict
+
     @torch.no_grad()
     def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
         os.makedirs(root, exist_ok=True)
-        num_img_exist = len([x for x in os.listdir(root) if x.endswith('.png')])
+        num_img_exist = len([x for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])
 
-        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt + prompt).chunk(2)
-        emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
-        emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
-        images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
+        ex_input_dict = self.get_ex_input()
+
+        mult_p, clean_text_p = self.token_ex.parse_attn_mult(prompt)
+        mult_n, clean_text_n = self.token_ex.parse_attn_mult(negative_prompt)
+        with autocast(enabled=self.cfgs.fp16):
+            emb_n, emb_p = self.te_hook.encode_prompt_to_emb(clean_text_n + clean_text_p).chunk(2)
+            emb_p = self.te_hook.mult_attn(emb_p, mult_p)
+            emb_n = self.te_hook.mult_attn(emb_n, mult_n)
+
+            if hasattr(self.pipe.unet, 'input_feeder'):
+                for feeder in self.pipe.unet.input_feeder:
+                    feeder(ex_input_dict)
+
+            images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
 
         for p, pn, img in zip(prompt, negative_prompt, images):
-            img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.png"))
+            img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
 
             if save_cfg:
                 with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
                     f.write(OmegaConf.to_yaml(self.cfgs_raw))
             num_img_exist += 1
 
     def show_latent(self, prompt, negative_prompt='', **kwargs):
@@ -91,8 +159,8 @@
         G.manual_seed(cfgs.seed)
     else:
         G = None
 
     viser = Visualizer(cfgs)
     for i in range(cfgs.num):
         viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt] * cfgs.bs, negative_prompt=[cfgs.neg_prompt] * cfgs.bs,
-                         generator=G, save_cfg=cfgs.save_cfg, **cfgs.infer_args)
+                         generator=G, save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
```

### Comparing `hcpdiff-0.1.6/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.2.0/hcpdiff.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.6
+Version: 0.2.0
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HCP-Diffusion
 
+[![PyPI](https://img.shields.io/pypi/v/hcpdiff)](https://pypi.org/project/hcpdiff/)
+[![GitHub stars](https://img.shields.io/github/stars/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/stargazers)
+[![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
+[![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
+
 [📘中文说明](./README_cn.md)
 
 ## Introduction
 HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
 It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
 
 This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
@@ -62,15 +68,15 @@
 
 Install from source:
 ```bash
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
-hcpinit
+## hcpinit
 ```
 
 ## User guidance
 
 Training:
 ```yaml
 # with accelerate
```

### Comparing `hcpdiff-0.1.6/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.2.0/hcpdiff.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 README.md
 setup.py
 cfgs/te_struct.txt
 cfgs/unet_struct.txt
 cfgs/infer/change_vae.yaml
 cfgs/infer/euler_a.yaml
-cfgs/infer/v1.yaml
+cfgs/infer/img2img.yaml
+cfgs/infer/img2img_controlnet.yaml
+cfgs/infer/text2img.yaml
+cfgs/train/plugin_control.yaml
 cfgs/train/train_base.yaml
 cfgs/train/tuning_base.yaml
 cfgs/train/examples/CustomDiffusion.yaml
 cfgs/train/examples/DreamArtist++.yaml
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
 cfgs/train/examples/TextualInversion.yaml
@@ -29,16 +32,17 @@
 hcpdiff.egg-info/top_level.txt
 hcpdiff/data/__init__.py
 hcpdiff/data/bucket.py
 hcpdiff/data/pair_dataset.py
 hcpdiff/data/utils.py
 hcpdiff/models/__init__.py
 hcpdiff/models/cfg_context.py
+hcpdiff/models/controlnet.py
 hcpdiff/models/layers.py
-hcpdiff/models/lora.py
+hcpdiff/models/lora_base.py
 hcpdiff/models/lora_layers.py
 hcpdiff/models/plugin.py
 hcpdiff/models/text_emb_ex.py
 hcpdiff/models/textencoder_ex.py
 hcpdiff/models/tokenizer_ex.py
 hcpdiff/tools/__init__.py
 hcpdiff/tools/convert_caption_txt2json.py
@@ -50,18 +54,24 @@
 hcpdiff/utils/__init__.py
 hcpdiff/utils/caption_tools.py
 hcpdiff/utils/cfg_net_tools.py
 hcpdiff/utils/colo_utils.py
 hcpdiff/utils/ema.py
 hcpdiff/utils/emb_utils.py
 hcpdiff/utils/img_size_tool.py
+hcpdiff/utils/net_utils.py
 hcpdiff/utils/utils.py
 hcpdiff/utils/ckpt_manager/__init__.py
 hcpdiff/utils/ckpt_manager/ckpt_pkl.py
 hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
 prompt_tuning_template/caption.txt
 prompt_tuning_template/name.txt
 prompt_tuning_template/name_2pt_caption.txt
 prompt_tuning_template/name_caption.txt
 prompt_tuning_template/object.txt
+prompt_tuning_template/object_caption.txt
 prompt_tuning_template/style.txt
+prompt_tuning_template/style_caption.txt
+test/test_combine.py
+test/test_ctnet.py
+test/test_paradict.py
 test/test_plugin_param.py
```

### Comparing `hcpdiff-0.1.6/prompt_tuning_template/object.txt` & `hcpdiff-0.2.0/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/prompt_tuning_template/style.txt` & `hcpdiff-0.2.0/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.6/setup.py` & `hcpdiff-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.1.6",
+    version="0.2.0",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

### Comparing `hcpdiff-0.1.6/test/test_plugin_param.py` & `hcpdiff-0.2.0/test/test_plugin_param.py`

 * *Files identical despite different names*

