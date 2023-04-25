# Comparing `tmp/sohuprompt-1.0.3.tar.gz` & `tmp/sohuprompt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sohuprompt-1.0.3.tar", last modified: Sun Apr 23 03:00:06 2023, max compression
+gzip compressed data, was "sohuprompt-1.0.4.tar", last modified: Tue Apr 25 03:49:23 2023, max compression
```

## Comparing `sohuprompt-1.0.3.tar` & `sohuprompt-1.0.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.985925 sohuprompt-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-23 03:00:06.984925 sohuprompt-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-23 02:57:04.000000 sohuprompt-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 03:00:06.985925 sohuprompt-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      682 2023-04-23 02:56:05.000000 sohuprompt-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.978925 sohuprompt-1.0.3/sohuprompt/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-23 02:55:47.000000 sohuprompt-1.0.3/sohuprompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.980925 sohuprompt-1.0.3/sohuprompt/data_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.981925 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/closed_QA.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/coreference.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/entity_typing.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/generation.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/nli.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/paraphrase.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/processor.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/reading_comprehensation.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/relation.py
--rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/summarization.py
--rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/topic_classification.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/conditional_generation_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/data_sampler.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/fewglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/huggingface_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/lama_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/nli_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/relation_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16683 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/text_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/typing_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    15591 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/default_config.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/lm_bff_trainer.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/pipeline_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.981925 sohuprompt-1.0.3/sohuprompt/plms/
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.982925 sohuprompt-1.0.3/sohuprompt/plms/glm/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/glm.py
--rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/tokenization_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/lm.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/mlm.py
--rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/seq2seq.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/utils.py
--rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompt_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.983925 sohuprompt-1.0.3/sohuprompt/prompts/
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/automatic_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/generation_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/knowledgeable_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/manual_template.py
--rw-r--r--   0 root         (0) root         (0)     9645 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/manual_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/mixed_template.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/one2one_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prefix_tuning_template.py
--rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prompt_generator.py
--rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prototypical_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/ptr_prompts.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/ptuning_prompts.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/soft_template.py
--rw-r--r--   0 root         (0) root         (0)     9069 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/soft_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/protoverb_trainer.py
--rw-r--r--   0 root         (0) root         (0)    31323 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.984925 sohuprompt-1.0.3/sohuprompt/utils/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/crossfit_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/cuda.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/logging.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/metrics.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/reproduciblity.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.979925 sohuprompt-1.0.3/sohuprompt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.946190 sohuprompt-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-25 03:49:23.945190 sohuprompt-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6324 2023-04-25 02:49:09.000000 sohuprompt-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 03:49:23.946190 sohuprompt-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      724 2023-04-25 03:47:47.000000 sohuprompt-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.939190 sohuprompt-1.0.4/sohuprompt/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-25 03:48:17.000000 sohuprompt-1.0.4/sohuprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.941190 sohuprompt-1.0.4/sohuprompt/data_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.942190 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/closed_QA.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/coreference.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/entity_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/generation.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/nli.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/paraphrase.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/processor.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/reading_comprehensation.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/relation.py
+-rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/summarization.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/data_utils/ZH/topic_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/conditional_generation_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/data_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/fewglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/huggingface_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/lama_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/nli_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/relation_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-04-25 02:48:15.000000 sohuprompt-1.0.4/sohuprompt/data_utils/text_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/typing_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/data_utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15913 2023-04-25 03:42:43.000000 sohuprompt-1.0.4/sohuprompt/default_config.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/lm_bff_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/pipeline_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.942190 sohuprompt-1.0.4/sohuprompt/plms/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.943190 sohuprompt-1.0.4/sohuprompt/plms/glm/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/glm.py
+-rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/plms/glm/tokenization_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/lm.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/mlm.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/seq2seq.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/plms/utils.py
+-rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompt_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.945190 sohuprompt-1.0.4/sohuprompt/prompts/
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/automatic_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/generation_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/knowledgeable_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/manual_template.py
+-rw-r--r--   0 root         (0) root         (0)     9645 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/manual_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/mixed_template.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/one2one_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/prefix_tuning_template.py
+-rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/prompt_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/prototypical_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/ptr_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/ptuning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/soft_template.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/prompts/soft_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/protoverb_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    31323 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.945190 sohuprompt-1.0.4/sohuprompt/utils/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/utils/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/utils/crossfit_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/utils/cuda.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.4/sohuprompt/utils/logging.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/utils/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/utils/reproduciblity.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 02:06:53.000000 sohuprompt-1.0.4/sohuprompt/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:49:23.940190 sohuprompt-1.0.4/sohuprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-25 03:49:23.000000 sohuprompt-1.0.4/sohuprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-25 03:49:23.000000 sohuprompt-1.0.4/sohuprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 03:49:23.000000 sohuprompt-1.0.4/sohuprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-25 03:49:23.000000 sohuprompt-1.0.4/sohuprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-25 03:49:23.000000 sohuprompt-1.0.4/sohuprompt.egg-info/top_level.txt
```

### Comparing `sohuprompt-1.0.3/README.md` & `sohuprompt-1.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
-# <div align="center">SohuPrompt</div>
+# <div align="center"><img src="https://s1.ax1x.com/2023/04/23/p9e0XDA.png" width="20%" ></img></div>
 
 <div align="center">
 <p align="center">
   <a href="#预览">预览</a> •
   <a href="#安装">安装</a> •
-  <a href="#如何使用">如何使用</a> 
+  <a href="#快速开始">快速开始</a> 
 </p>
 
 </div>
 
 ![version](https://img.shields.io/badge/version-v1.0.3-green)
 
 
 
 
 ## 新闻
 
  
 
-- ❗️ 2023年4月：版本更新，支持[ChatGLM](https://github.com/THUDM/ChatGLM-6B), 可以使用SohuPrompt工具对ChatGLM进行微调.
+- ❗️ 2023年4月：版本更新，支持[ChatGLM](https://github.com/THUDM/ChatGLM-6B), 可以使用SohuPrompt工具对ChatGLM进行微调。
 - 2023年4月：SohuPrompt v1.0.1版本发布，欢迎大家为SohuPrompt贡献代码。
 
 ## 预览
 
 Prompt-learning是最新的训练范式，它可以将预训练语言模型（PLMs）更好的适配下游NLP任务。SohuPrompt库提供了一个标准、灵活和可扩展的框架，用于部署prompt-learning流水线，它支持直接从[huggingface transformers](https://github.com/huggingface/transformers)加载PLMs。在未来，我们将支持[deepspeed](https://github.com/microsoft/DeepSpeed)或[colossal ai](https://github.com/hpcaitech/ColossalAI)来加快训练和预测速度。
 
 
@@ -35,60 +35,138 @@
 </div>
 
 
 
 
 ## 安装
 
-### 使用 Pip
+### 使用 pip
 
 
 ```shell
 pip install sohuprompt
 ```
 你也可以从gitlab源安装最新版本的SohuPrompt。
 
 
 
 
-## 如何使用
-### 第一步：加载数据集
+## 快速开始
+### 第一步 定义config
+详细了解config的配置，请参考[config](sohuprompt/default_config.py)
+```yaml
+environment:
+  num_gpus: 1
+  cuda_visible_devices:
+        - 1
+  local_rank: 0
+
+logging:
+    path: pretrained_model/
+    unique_string: chatglm
+
+dataset:
+  name: generate_comment
+  path: ./data/
+
+task: generation
+
+dataloader:
+  decoder_max_length: 128 
+  max_seq_length: 128
+  truncate_method: tail
+
+train:
+  num_epochs: 1
+  batch_size: 1
+  teacher_forcing: True
+  gradient_accumulation_steps: 4
+  bf16: False
+  fp16: False
+  deepspeed: False
+  label_smoothing_factor: 0
+
+dev:
+  batch_size: 1
+  shuffle_data: False
+
+test:
+  batch_size: 2
+  shuffle_data: False
+
+generation:
+  parent_config: task
+  max_new_tokens: 64
+  num_beam_groups: 5
+  num_beams: 5
+  diversity_penalty: 3.0
+  temperature: 2.0
+  repetition_penalty: 5.0
+  early_stopping: False
+  length_penalty: 3.0
+  bad_words_ids:
+  - - 3473
+    - 1837
+  - - 3473
+    - 27556
+  - - 259
+    - 3473
+
+plm:
+  model_name: chatglm 
+  model_path: pretrained_model/chatglm-6b/
+  optimize:
+    freeze_para: True
+    lr: 0.00003
+
+template: ptuning_template
+verbalizer: 
+
+ptuning_template:
+  choice: 0
+  file_path: ptuning_prompt.txt
+  placeholder_mapping:                                     
+    <text_a>: text_a
+    <text_b>: text_b
+    <text_c>: text_c
+```
+### 第二步：加载数据集
 ```python
 from sohuprompt.data_utils import load_dataset
 
 train_dataset, valid_dataset, test_dataset, Processor = load_dataset(config, test=False)
 # 数据集中的数据源通过config确定，config是一个yaml文件，我们通过config来对代码进行各种有效的配置
 ```
 
-### 第二步：加载预训练模型
+### 第三步：加载预训练模型
 ```python
 from sohuprompt.plms import load_plm_from_config
 
 plm_model, plm_tokenizer, plm_config, plm_wrapper_class = load_plm_from_config(config)
 # 模型的配置也是通过config来确定的
 ```
-### 第三步：加载prompt-template与verbalizer
+### 第四步：加载prompt-template与verbalizer
 ```python
-from SohuPrompt.prompts import load_template, load_verbalizer
+from sohuprompt.prompts import load_template, load_verbalizer
 
 template = load_template(config=config, model=plm_model, tokenizer=plm_tokenizer, plm_config=plm_config)
 verbalizer = load_verbalizer(config=config, model=plm_model, tokenizer=plm_tokenizer, plm_config=plm_config, classes=Processor.labels)
 # template和verbalizer的配置也是通过config来确定
 ```
-### 第四步：加载prompt-learning模型
+### 第五步：加载prompt-learning模型
 ```python
-from SohuPrompt.pipeline_base import PromptForClassification, PromptForGeneration
+from sohuprompt.pipeline_base import PromptForClassification, PromptForGeneration
 
 prompt_model = PromptForGeneration(plm_model, template, freeze_plm=config.plm.optimize.freeze_para, gen_config=config.generation, )
 # 这里需要注意的是，prompt_model的类型是PromptForGeneration，即生成任务，如果是分类任务，那么prompt_model的类型是PromptForClassification
 # prompt_model = PromptForClassification(plm_model, template, verbalizer, freeze_plm = config.plm.optimize.freeze_para)
 ```
-### 第五步：加载dataloader
+### 第六步：加载dataloader
 ```python
-from SohuPrompt import PromptDataLoader
+from sohuprompt import PromptDataLoader
 
 # 为了更好的适配prompt-learning，我们重新对prompt dataloader进行包装
 def build_dataloader(
         dataset, template, tokenizer, tokenizer_wrapper_class, config, split
 ):
     dataloader = PromptDataLoader(
         dataset=dataset,
@@ -105,22 +183,22 @@
     )
     return dataloader
 # 定义完build_dataloader之后，我们就可以加载dataloader了
 train_dataloader = (build_dataloader(train_dataset, template, plm_tokenizer, plm_wrapper_class, config, "train") if train_dataset else None)
 valid_dataloader = (build_dataloader(valid_dataset, template, plm_tokenizer, plm_wrapper_class, config, "dev") if valid_dataset else None)
 test_dataloader = (build_dataloader(test_dataset, template, plm_tokenizer, plm_wrapper_class, config, "test") if test_dataset else None)
 ```
-### 第六步：加载trainer
+### 第七步：加载trainer
 ```python
-from SohuPrompt.trainer import ClassificationRunner, GenerationRunner
+from sohuprompt.trainer import ClassificationRunner, GenerationRunner
 
 runner = GenerationRunner(model=prompt_model, train_dataloader=train_dataloader, valid_dataloader=valid_dataloader, test_dataloader=test_dataloader, config=config, )
 # 注意，这里的runner要与第五步中的prompt_model的类型相对应，如果是PromptForGeneration，那么runner的类型就是GenerationRunner，如果是PromptForClassification，那么runner的类型就是ClassificationRunner
 # runner = ClassificationRunner(model=prompt_model, train_dataloader=train_dataloader, valid_dataloader=valid_dataloader, test_dataloader=test_dataloader, config=config, )
 ```
-### 第七步：训练模型
+### 第八步：训练模型
 ```python
 runner.run()
 ```
 ## 代码贡献
 欢迎大家使用SohuPrompt和为SohuPrompt贡献代码
```

#### html2text {}

```diff
@@ -1,45 +1,60 @@
  #
-                                  SohuPrompt
-                      é¢è§ â¢ å®è£ â¢ å¦ä½ä½¿ç¨
+                 [https://s1.ax1x.com/2023/04/23/p9e0XDA.png]
+                      é¢è§ â¢ å®è£ â¢ å¿«éå¼å§
 ![version](https://img.shields.io/badge/version-v1.0.3-green) ## æ°é» -
 âï¸ 2023å¹´4æï¼çæ¬æ´æ°ï¼æ¯æ[ChatGLM](https://github.com/THUDM/
-ChatGLM-6B), å¯ä»¥ä½¿ç¨SohuPromptå·¥å·å¯¹ChatGLMè¿è¡å¾®è°. -
+ChatGLM-6B), å¯ä»¥ä½¿ç¨SohuPromptå·¥å·å¯¹ChatGLMè¿è¡å¾®è°ã -
 2023å¹´4æï¼SohuPrompt
 v1.0.1çæ¬åå¸ï¼æ¬¢è¿å¤§å®¶ä¸ºSohuPromptè´¡ç®ä»£ç ã ## é¢è§ Prompt-
 learningæ¯ææ°çè®­ç»èå¼ï¼å®å¯ä»¥å°é¢è®­ç»è¯­è¨æ¨¡åï¼PLMsï¼æ´å¥½çééä¸æ¸¸NLPä»»å¡ãSohuPromptåºæä¾äºä¸ä¸ªæ åãçµæ´»åå¯æ©å±çæ¡æ¶ï¼ç¨äºé¨ç½²prompt-
 learningæµæ°´çº¿ï¼å®æ¯æç´æ¥ä»[huggingface transformers](https://
 github.com/huggingface/transformers)å è½½PLMsãå¨æªæ¥ï¼æä»¬å°æ¯æ
 [deepspeed](https://github.com/microsoft/DeepSpeed)æ[colossal ai](https://
 github.com/hpcaitech/ColossalAI)æ¥å å¿«è®­ç»åé¢æµéåº¦ã
                   [https://z3.ax1x.com/2021/11/03/IAdT3D.png]
-## å®è£ ### ä½¿ç¨ Pip ```shell pip install sohuprompt ```
-ä½ ä¹å¯ä»¥ä»gitlabæºå®è£ææ°çæ¬çSohuPromptã ## å¦ä½ä½¿ç¨ ###
-ç¬¬ä¸æ­¥ï¼å è½½æ°æ®é ```python from sohuprompt.data_utils import
-load_dataset train_dataset, valid_dataset, test_dataset, Processor =
-load_dataset(config, test=False) #
+## å®è£ ### ä½¿ç¨ pip ```shell pip install sohuprompt ```
+ä½ ä¹å¯ä»¥ä»gitlabæºå®è£ææ°çæ¬çSohuPromptã ## å¿«éå¼å§ ###
+ç¬¬ä¸æ­¥ å®ä¹config è¯¦ç»äºè§£configçéç½®ï¼è¯·åè[config]
+(sohuprompt/default_config.py) ```yaml environment: num_gpus: 1
+cuda_visible_devices: - 1 local_rank: 0 logging: path: pretrained_model/
+unique_string: chatglm dataset: name: generate_comment path: ./data/ task:
+generation dataloader: decoder_max_length: 128 max_seq_length: 128
+truncate_method: tail train: num_epochs: 1 batch_size: 1 teacher_forcing: True
+gradient_accumulation_steps: 4 bf16: False fp16: False deepspeed: False
+label_smoothing_factor: 0 dev: batch_size: 1 shuffle_data: False test:
+batch_size: 2 shuffle_data: False generation: parent_config: task
+max_new_tokens: 64 num_beam_groups: 5 num_beams: 5 diversity_penalty: 3.0
+temperature: 2.0 repetition_penalty: 5.0 early_stopping: False length_penalty:
+3.0 bad_words_ids: - - 3473 - 1837 - - 3473 - 27556 - - 259 - 3473 plm:
+model_name: chatglm model_path: pretrained_model/chatglm-6b/ optimize:
+freeze_para: True lr: 0.00003 template: ptuning_template verbalizer:
+ptuning_template: choice: 0 file_path: ptuning_prompt.txt placeholder_mapping:
+: text_a : text_b : text_c ``` ### ç¬¬äºæ­¥ï¼å è½½æ°æ®é ```python from
+sohuprompt.data_utils import load_dataset train_dataset, valid_dataset,
+test_dataset, Processor = load_dataset(config, test=False) #
 æ°æ®éä¸­çæ°æ®æºéè¿configç¡®å®ï¼configæ¯ä¸ä¸ªyamlæä»¶ï¼æä»¬éè¿configæ¥å¯¹ä»£ç è¿è¡åç§ææçéç½®
-``` ### ç¬¬äºæ­¥ï¼å è½½é¢è®­ç»æ¨¡å ```python from sohuprompt.plms import
+``` ### ç¬¬ä¸æ­¥ï¼å è½½é¢è®­ç»æ¨¡å ```python from sohuprompt.plms import
 load_plm_from_config plm_model, plm_tokenizer, plm_config, plm_wrapper_class =
 load_plm_from_config(config) # æ¨¡åçéç½®ä¹æ¯éè¿configæ¥ç¡®å®ç
-``` ### ç¬¬ä¸æ­¥ï¼å è½½prompt-templateä¸verbalizer ```python from
-SohuPrompt.prompts import load_template, load_verbalizer template =
+``` ### ç¬¬åæ­¥ï¼å è½½prompt-templateä¸verbalizer ```python from
+sohuprompt.prompts import load_template, load_verbalizer template =
 load_template(config=config, model=plm_model, tokenizer=plm_tokenizer,
 plm_config=plm_config) verbalizer = load_verbalizer(config=config,
 model=plm_model, tokenizer=plm_tokenizer, plm_config=plm_config,
 classes=Processor.labels) #
 templateåverbalizerçéç½®ä¹æ¯éè¿configæ¥ç¡®å® ``` ###
-ç¬¬åæ­¥ï¼å è½½prompt-learningæ¨¡å ```python from SohuPrompt.pipeline_base
+ç¬¬äºæ­¥ï¼å è½½prompt-learningæ¨¡å ```python from sohuprompt.pipeline_base
 import PromptForClassification, PromptForGeneration prompt_model =
 PromptForGeneration(plm_model, template,
 freeze_plm=config.plm.optimize.freeze_para, gen_config=config.generation, ) #
 è¿ééè¦æ³¨æçæ¯ï¼prompt_modelçç±»åæ¯PromptForGenerationï¼å³çæä»»å¡ï¼å¦ææ¯åç±»ä»»å¡ï¼é£ä¹prompt_modelçç±»åæ¯PromptForClassification
 # prompt_model = PromptForClassification(plm_model, template, verbalizer,
 freeze_plm = config.plm.optimize.freeze_para) ``` ###
-ç¬¬äºæ­¥ï¼å è½½dataloader ```python from SohuPrompt import PromptDataLoader
+ç¬¬å­æ­¥ï¼å è½½dataloader ```python from sohuprompt import PromptDataLoader
 # ä¸ºäºæ´å¥½çééprompt-learningï¼æä»¬éæ°å¯¹prompt
 dataloaderè¿è¡åè£ def build_dataloader( dataset, template, tokenizer,
 tokenizer_wrapper_class, config, split ): dataloader = PromptDataLoader
 ( dataset=dataset, template=template, tokenizer=tokenizer,
 tokenizer_wrapper_class=tokenizer_wrapper_class, batch_size=config
 [split].batch_size, shuffle=config[split].shuffle_data, teacher_forcing=config
 [split].teacher_forcing if hasattr(config[split], "teacher_forcing") else None,
@@ -47,18 +62,18 @@
 **config.dataloader ) return dataloader #
 å®ä¹å®build_dataloaderä¹åï¼æä»¬å°±å¯ä»¥å è½½dataloaderäº
 train_dataloader = (build_dataloader(train_dataset, template, plm_tokenizer,
 plm_wrapper_class, config, "train") if train_dataset else None)
 valid_dataloader = (build_dataloader(valid_dataset, template, plm_tokenizer,
 plm_wrapper_class, config, "dev") if valid_dataset else None) test_dataloader =
 (build_dataloader(test_dataset, template, plm_tokenizer, plm_wrapper_class,
-config, "test") if test_dataset else None) ``` ### ç¬¬å­æ­¥ï¼å è½½trainer
-```python from SohuPrompt.trainer import ClassificationRunner, GenerationRunner
+config, "test") if test_dataset else None) ``` ### ç¬¬ä¸æ­¥ï¼å è½½trainer
+```python from sohuprompt.trainer import ClassificationRunner, GenerationRunner
 runner = GenerationRunner(model=prompt_model,
 train_dataloader=train_dataloader, valid_dataloader=valid_dataloader,
 test_dataloader=test_dataloader, config=config, ) #
 æ³¨æï¼è¿éçrunnerè¦ä¸ç¬¬äºæ­¥ä¸­çprompt_modelçç±»åç¸å¯¹åºï¼å¦ææ¯PromptForGenerationï¼é£ä¹runnerçç±»åå°±æ¯GenerationRunnerï¼å¦ææ¯PromptForClassificationï¼é£ä¹runnerçç±»åå°±æ¯ClassificationRunner
 # runner = ClassificationRunner(model=prompt_model,
 train_dataloader=train_dataloader, valid_dataloader=valid_dataloader,
 test_dataloader=test_dataloader, config=config, ) ``` ###
-ç¬¬ä¸æ­¥ï¼è®­ç»æ¨¡å ```python runner.run() ``` ## ä»£ç è´¡ç®
+ç¬¬å«æ­¥ï¼è®­ç»æ¨¡å ```python runner.run() ``` ## ä»£ç è´¡ç®
 æ¬¢è¿å¤§å®¶ä½¿ç¨SohuPromptåä¸ºSohuPromptè´¡ç®ä»£ç 
```

### Comparing `sohuprompt-1.0.3/setup.py` & `sohuprompt-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='sohuprompt',
-        version='1.0.3',
+        version='1.0.4',
         packages=find_packages(),  # 查找包的路径
         # package_dir={'': 'src'},  # 包的root路径映射到的实际路径
         # include_package_data=False,
         # package_data={'data': []},
         description='A python lib for sohuprompt',
         # long_description='',
         author='senhaowang,chencheng',
         author_email='senhaowang@sohu-inc.com',
         # url='http://www.xxxxx.com/',  # homepage
         license='MIT',
-        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'sklearn', 'jieba'],
+        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'sklearn', 'jieba', 'tensorboardX', 'icetk', 'yacs', 'rouge'],
         )
```

### Comparing `sohuprompt-1.0.3/sohuprompt/config.py` & `sohuprompt-1.0.4/sohuprompt/config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/closed_QA.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/closed_QA.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/coreference.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/coreference.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/entity_typing.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/entity_typing.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/generation.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/generation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/nli.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/nli.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/paraphrase.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/paraphrase.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/reading_comprehensation.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/reading_comprehensation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/relation.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/relation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/sentiment.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/sentiment.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/summarization.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/summarization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/topic_classification.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/ZH/topic_classification.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/__init__.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/conditional_generation_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/conditional_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/data_processor.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/data_sampler.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/data_sampler.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/fewglue_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/fewglue_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/huggingface_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/lama_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/lama_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/nli_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/nli_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/relation_classification_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/relation_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/text_classification_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/text_classification_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
         self.labels = [0,1]
 
     def get_examples(self, data_dir, split):
         examples = []
         if split != "test":
             path = os.path.join(data_dir, "{}.csv".format(split))
             with open(path, encoding='utf8') as f:
-                reader = csv.reader(f, delimiter=',', quoting=csv.QUOTE_NONE)
+                reader = csv.reader(f, delimiter='\t', quoting=csv.QUOTE_NONE)
                 for row in reader:
-                    text_a, text_b, label_id = row[0], row[1] ,int(row[2])
-                    example = InputExample(text_a=row[0], text_b=row[1], label=label_id)
+                    label_id = int(row[4])
+                    example = InputExample(text_a=row[2], text_b=row[3], label=label_id)
                     examples.append(example)
         else:
             path = os.path.join(data_dir, "{}.xlsx".format(split))
             df = pd.read_excel(path, engine='openpyxl')
             values = df.values
             for row in values:
                 label = row[5]
```

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/typing_dataset.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/typing_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/data_utils/utils.py` & `sohuprompt-1.0.4/sohuprompt/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/default_config.py` & `sohuprompt-1.0.4/sohuprompt/default_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,19 @@
     cfg.train.teacher_forcing = False # whether perform teacher forcing in training.
                         # if true, the desired prediction on each mask will
                         # be filled in the mask.
     cfg.train.gradient_accumulation_steps = 1 # update weight  every N step of training.
                         # set 1 to disable gradient accumulation.
     cfg.train.max_grad_norm = -1.0 # <0 for unlimited gradients norm
     cfg.train.clean = False # set to True for not saving checkpoint and no tensorboard logging
+    cfg.train.label_smoothing_factor = 0 # set label somooth factor
+    cfg.train.fp16 = False # whether to use fp16 training
+    cfg.train.bf16 = False # whether to use bf16 training
+    cfg.train.deepspeed = False # whether to use deepspeed training
+    cfg.train.colossalai = False # whether to use colossalai training
 
     cfg.dev = CfgNode(new_allowed=True)
     cfg.dev.batch_size = 2 # evaluationn batch_size, can be a bit larger than training batch_size
     cfg.dev.shuffle_data = False # whether to perform data shuffling in evaluation
 
     cfg.test = CfgNode(new_allowed=True)
     cfg.test.batch_size = 2 # evaluationn batch_size, can be a bit larger than training batch_size
```

### Comparing `sohuprompt-1.0.3/sohuprompt/lm_bff_trainer.py` & `sohuprompt-1.0.4/sohuprompt/lm_bff_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/pipeline_base.py` & `sohuprompt-1.0.4/sohuprompt/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/__init__.py` & `sohuprompt-1.0.4/sohuprompt/plms/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/glm/configuration_chatglm.py` & `sohuprompt-1.0.4/sohuprompt/plms/glm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/glm/glm.py` & `sohuprompt-1.0.4/sohuprompt/plms/glm/glm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/glm/modeling_chatglm.py` & `sohuprompt-1.0.4/sohuprompt/plms/glm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/glm/quantization.py` & `sohuprompt-1.0.4/sohuprompt/plms/glm/quantization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/glm/tokenization_chatglm.py` & `sohuprompt-1.0.4/sohuprompt/plms/glm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/lm.py` & `sohuprompt-1.0.4/sohuprompt/plms/lm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/mlm.py` & `sohuprompt-1.0.4/sohuprompt/plms/mlm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/seq2seq.py` & `sohuprompt-1.0.4/sohuprompt/plms/seq2seq.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/plms/utils.py` & `sohuprompt-1.0.4/sohuprompt/plms/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompt_base.py` & `sohuprompt-1.0.4/sohuprompt/prompt_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/__init__.py` & `sohuprompt-1.0.4/sohuprompt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/automatic_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/automatic_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/generation_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/generation_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/knowledgeable_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/knowledgeable_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/manual_template.py` & `sohuprompt-1.0.4/sohuprompt/prompts/manual_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/manual_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/manual_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/mixed_template.py` & `sohuprompt-1.0.4/sohuprompt/prompts/mixed_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/one2one_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/one2one_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/prefix_tuning_template.py` & `sohuprompt-1.0.4/sohuprompt/prompts/prefix_tuning_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/prompt_generator.py` & `sohuprompt-1.0.4/sohuprompt/prompts/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/prototypical_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/prototypical_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/ptr_prompts.py` & `sohuprompt-1.0.4/sohuprompt/prompts/ptr_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/ptuning_prompts.py` & `sohuprompt-1.0.4/sohuprompt/prompts/ptuning_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/soft_template.py` & `sohuprompt-1.0.4/sohuprompt/prompts/soft_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/prompts/soft_verbalizer.py` & `sohuprompt-1.0.4/sohuprompt/prompts/soft_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/protoverb_trainer.py` & `sohuprompt-1.0.4/sohuprompt/protoverb_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/trainer.py` & `sohuprompt-1.0.4/sohuprompt/trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/calibrate.py` & `sohuprompt-1.0.4/sohuprompt/utils/calibrate.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/crossfit_metrics.py` & `sohuprompt-1.0.4/sohuprompt/utils/crossfit_metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/cuda.py` & `sohuprompt-1.0.4/sohuprompt/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/logging.py` & `sohuprompt-1.0.4/sohuprompt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/metrics.py` & `sohuprompt-1.0.4/sohuprompt/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt/utils/utils.py` & `sohuprompt-1.0.4/sohuprompt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.3/sohuprompt.egg-info/SOURCES.txt` & `sohuprompt-1.0.4/sohuprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

