# Comparing `tmp/mosaicml-cli-0.4.0a1.tar.gz` & `tmp/mosaicml-cli-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a1.tar", last modified: Thu Apr 20 21:11:00 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a2.tar", last modified: Mon Apr 24 23:16:08 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a1.tar` & `mosaicml-cli-0.4.0a2.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.250504 mosaicml-cli-0.4.0a1/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 21:11:00.250344 mosaicml-cli-0.4.0a1/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.216455 mosaicml-cli-0.4.0a1/mcli/
--rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.217087 mosaicml-cli-0.4.0a1/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.217780 mosaicml-cli-0.4.0a1/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.218250 mosaicml-cli-0.4.0a1/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.220217 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3292 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.221087 mosaicml-cli-0.4.0a1/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.222173 mosaicml-cli-0.4.0a1/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-20 21:07:59.000000 mosaicml-cli-0.4.0a1/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.224495 mosaicml-cli-0.4.0a1/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)     1102 2023-04-18 18:36:19.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.224865 mosaicml-cli-0.4.0a1/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.225722 mosaicml-cli-0.4.0a1/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226128 mosaicml-cli-0.4.0a1/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226429 mosaicml-cli-0.4.0a1/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226881 mosaicml-cli-0.4.0a1/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.227161 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.227571 mosaicml-cli-0.4.0a1/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.228254 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.228729 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.229832 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)    10343 2023-04-20 21:08:39.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.231613 mosaicml-cli-0.4.0a1/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.232186 mosaicml-cli-0.4.0a1/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init.py
--rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.233281 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-20 21:09:05.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.233786 mosaicml-cli-0.4.0a1/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.234169 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.234709 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.235078 mosaicml-cli-0.4.0a1/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.235481 mosaicml-cli-0.4.0a1/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     7550 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.236737 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.237046 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.237541 mosaicml-cli-0.4.0a1/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.239123 mosaicml-cli-0.4.0a1/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)     8426 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.239477 mosaicml-cli-0.4.0a1/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.241265 mosaicml-cli-0.4.0a1/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.242677 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.243023 mosaicml-cli-0.4.0a1/mcli/proto/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a1/mcli/proto/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-20 00:22:55.000000 mosaicml-cli-0.4.0a1/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.243365 mosaicml-cli-0.4.0a1/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)     1045 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.247716 mosaicml-cli-0.4.0a1/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-20 00:22:47.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-20 21:10:31.000000 mosaicml-cli-0.4.0a1/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.248966 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     4609 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-20 21:11:00.250547 mosaicml-cli-0.4.0a1/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.250029 mosaicml-cli-0.4.0a1/tests/
--rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/tests/test_upgrade.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.653933 mosaicml-cli-0.4.0a2/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-24 23:16:08.653770 mosaicml-cli-0.4.0a2/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/README.md
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.625951 mosaicml-cli-0.4.0a2/mcli/
+-rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.626533 mosaicml-cli-0.4.0a2/mcli/api/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.626996 mosaicml-cli-0.4.0a2/mcli/api/cluster/
+-rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/cluster/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.627500 mosaicml-cli-0.4.0a2/mcli/api/engine/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/engine/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/engine/engine.py
+-rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/exceptions.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.628931 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/
+-rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     3311 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.629506 mosaicml-cli-0.4.0a2/mcli/api/mint/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/shell.py
+-rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/tty.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.630251 mosaicml-cli-0.4.0a2/mcli/api/model/
+-rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/cluster_details.py
+-rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.632468 mosaicml-cli-0.4.0a2/mcli/api/runs/
+-rw-r--r--   0 anna       (501) staff       (20)     1199 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     4910 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.632766 mosaicml-cli-0.4.0a2/mcli/api/schema/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/schema/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.633403 mosaicml-cli-0.4.0a2/mcli/api/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-24 22:56:35.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/typing_future.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.633804 mosaicml-cli-0.4.0a2/mcli/api/users/
+-rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/users/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634105 mosaicml-cli-0.4.0a2/mcli/cli/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/__init__.py
+-rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/cli.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634577 mosaicml-cli-0.4.0a2/mcli/cli/common/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634865 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.635320 mosaicml-cli-0.4.0a2/mcli/cli/m_create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.635814 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.636064 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.636702 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)    10343 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.638046 mosaicml-cli-0.4.0a2/mcli/cli/m_get/
+-rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/display.py
+-rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.638484 mosaicml-cli-0.4.0a2/mcli/cli/m_init/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639126 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639456 mosaicml-cli-0.4.0a2/mcli/cli/m_log/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639727 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640137 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640541 mosaicml-cli-0.4.0a2/mcli/cli/m_root/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640909 mosaicml-cli-0.4.0a2/mcli/cli/m_run/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     8099 2023-04-24 23:14:14.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.642300 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.642715 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.643326 mosaicml-cli-0.4.0a2/mcli/cli/m_util/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/util.py
+-rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.644768 mosaicml-cli-0.4.0a2/mcli/models/
+-rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/gpu_type.py
+-rw-r--r--   0 anna       (501) staff       (20)    11810 2023-04-24 23:13:07.000000 mosaicml-cli-0.4.0a2/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_cluster.py
+-rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_envvar.py
+-rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/run_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.645030 mosaicml-cli-0.4.0a2/mcli/objects/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.646652 mosaicml-cli-0.4.0a2/mcli/objects/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648016 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648317 mosaicml-cli-0.4.0a2/mcli/proto/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/proto/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648560 mosaicml-cli-0.4.0a2/mcli/sdk/
+-rw-r--r--   0 anna       (501) staff       (20)     1068 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/sdk/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.651968 mosaicml-cli-0.4.0a2/mcli/utils/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_cli.py
+-rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_date.py
+-rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_docker.py
+-rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_epilog.py
+-rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_logging.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_pypi.py
+-rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_rich.py
+-rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_run_status.py
+-rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_spinner.py
+-rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_types.py
+-rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_yaml.py
+-rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-24 23:14:24.000000 mosaicml-cli-0.4.0a2/mcli/version.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.652874 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     4640 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/pyproject.toml
+-rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-24 23:16:08.653981 mosaicml-cli-0.4.0a2/setup.cfg
+-rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/setup.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.653488 mosaicml-cli-0.4.0a2/tests/
+-rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/tests/test_config.py
+-rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/tests/test_simple.py
+-rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a1/PKG-INFO` & `mosaicml-cli-0.4.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a1/README.md` & `mosaicml-cli-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a2/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a2/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a2/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
     publicDNS
+    createdByEmail
   }}
 }}"""
 
 __all__ = ['delete_inference_deployments']
 
 
 @overload
```

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a2/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a2/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a2/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a2/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a2/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """API calls for run management"""
 # pylint: disable=useless-import-alias
 from mcli.api.model.run import Run
 from mcli.api.runs.api_create_run import create_run
 from mcli.api.runs.api_delete_runs import delete_run, delete_runs
 from mcli.api.runs.api_get_run_logs import follow_run_logs, get_run_logs
 from mcli.api.runs.api_get_runs import get_run, get_runs
+from mcli.api.runs.api_start_run import start_run, start_runs
 from mcli.api.runs.api_stop_runs import stop_run, stop_runs
 from mcli.api.runs.api_update_run_metadata import update_run_metadata
 from mcli.api.runs.api_watch_run import wait_for_run_status, watch_run_status
 from mcli.models import ComputeConfig, FinalRunConfig, RunConfig, SchedulingConfig
 from mcli.utils.utils_run_status import RunStatus
 
 __all__ = [
@@ -23,13 +24,15 @@
     'delete_run',
     'delete_runs',
     'follow_run_logs',
     'get_run_logs',
     'get_run',
     'get_runs',
     'get_run',
+    'start_run',
+    'start_runs',
     'stop_run',
     'stop_runs',
     'update_run_metadata',
     'wait_for_run_status',
     'watch_run_status',
 ]
```

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a2/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a2/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a2/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a2/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a2/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a2/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a2/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_run/m_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 
 from mcli.api.exceptions import MAPIException, cli_error_handler
 from mcli.api.runs import create_run, delete_runs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.config import MCLIConfig
 from mcli.models.run_config import VALID_OPTIMIZATION_LEVELS
-from mcli.sdk import Run, RunConfig, follow_run_logs, get_run, wait_for_run_status
+from mcli.sdk import Run, RunConfig, follow_run_logs, get_run, start_run, wait_for_run_status
 from mcli.utils.utils_epilog import CommonLog
 from mcli.utils.utils_logging import INFO, OK
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
 
@@ -63,18 +63,39 @@
         print('')
 
     wait_for_run_status(run, status=RunStatus.COMPLETED, timeout=10)
 
     return 0
 
 
+def finish_run(run: Run, follow: bool, restarted: bool = False) -> int:
+    if not follow:
+        log_cmd = f'mcli logs {run.name}'
+        message = f"""
+        {OK} Run [cyan]{run.name}[/] {'re' if restarted else ''}submitted.
+
+        To see the run\'s status, use:
+
+        [bold]mcli get runs[/]
+
+        To see the run\'s logs, use:
+
+        [bold]{log_cmd}[/]
+        """
+        logger.info(textwrap.dedent(message).strip())
+        return 0
+    else:
+        return follow_run(run)
+
+
 # pylint: disable-next=too-many-statements
 @cli_error_handler('mcli run')
 def run_entrypoint(
     file: Optional[str] = None,
+    restart_run: Optional[str] = None,
     clone: Optional[str] = None,
     follow: bool = True,
     override_cluster: Optional[str] = None,
     override_gpu_type: Optional[str] = None,
     override_gpu_num: Optional[int] = None,
     override_image: Optional[str] = None,
     override_name: Optional[str] = None,
@@ -89,27 +110,33 @@
     if file:
         run_config = RunConfig.from_file(path=file)
     elif clone:
         run = get_run(clone)
         if run.submitted_config is None:
             raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {clone}")
         run_config = run.submitted_config
+    elif restart_run:
+        with console_status('Restarting run...'):
+            run = start_run(restart_run, timeout=None)
+
+        return finish_run(run, follow, restarted=True)
+
     else:
         return print_help()
 
     # command line overrides
     # only supports basic format for now and not structured params
     if override_cluster is not None:
-        run_config.cluster = override_cluster
+        run_config.compute['cluster'] = override_cluster
 
     if override_gpu_type is not None:
-        run_config.gpu_type = override_gpu_type
+        run_config.compute['gpu_type'] = override_gpu_type
 
     if override_gpu_num is not None:
-        run_config.gpu_num = override_gpu_num
+        run_config.compute['gpus'] = override_gpu_num
 
     if override_image is not None:
         run_config.image = override_image
 
     if override_name is not None:
         run_config.name = override_name
 
@@ -124,31 +151,15 @@
 
     if override_nodes is not None:
         run_config.compute['nodes'] = override_nodes
 
     with console_status('Submitting run...'):
         run = create_run(run=run_config, timeout=None)
 
-    if not follow:
-        log_cmd = f'mcli logs {run.name}'
-        message = f"""
-        {OK} Run [cyan]{run.name}[/] submitted.
-
-        To see the run\'s status, use:
-
-        [bold]mcli get runs[/]
-
-        To see the run\'s logs, use:
-
-        [bold]{log_cmd}[/]
-        """
-        logger.info(textwrap.dedent(message).strip())
-        return 0
-    else:
-        return follow_run(run)
+    return finish_run(run, follow)
 
 
 def add_run_argparser(subparser: argparse._SubParsersAction) -> None:
     run_parser: argparse.ArgumentParser = subparser.add_parser(
         'run',
         aliases=['r'],
         help='Launch a run in the MosaicML platform',
@@ -162,14 +173,21 @@
         '-f',
         '--file',
         dest='file',
         help='File from which to load arguments.',
     )
 
     parser.add_argument(
+        '-r',
+        '--restart',
+        dest='restart_run',
+        help='Previously stopped run to start again',
+    )
+
+    parser.add_argument(
         '--clone',
         dest='clone',
         help='Copy the run config from an existing run',
     )
 
     parser.add_argument(
         '--priority',
```

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a2/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/config.py` & `mosaicml-cli-0.4.0a2/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a2/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a2/mcli/models/inference_deployment_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,47 @@
 
 import logging
 from dataclasses import asdict, dataclass, field
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional
 
 import yaml
+from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import _clean_run_name
-from mcli.utils.utils_config import BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, uuid_generator
-from mcli.utils.utils_string_functions import validate_image
+from mcli.utils.utils_config import (BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, Translation,
+                                     uuid_generator)
+from mcli.utils.utils_string_functions import camel_case_to_snake_case, snake_case_to_camel_case, validate_image
 
 logger = logging.getLogger(__name__)
 
 DEPLOYMENT_CONFIG_UID_LENGTH = 6
 
 
+class HFModelConfig(TypedDict, total=False):
+    """Typed dictionary for nested hugging face model configs"""
+    task: str
+    model_dtype: Optional[str]
+    autocast_dtype: Optional[str]
+
+
+class CustomModelConfig(TypedDict, total=False):
+    """Typed dictionary for nested custom model configs"""
+    model_handler: str
+
+
+class ModelConfig(TypedDict, total=False):
+    """Typed dictionary for model configs"""
+    checkpoint_path: str
+    hf_model: Optional[HFModelConfig]
+    custom_mdoel: Optional[CustomModelConfig]
+
+
 @dataclass
 class FinalInferenceDeploymentConfig(DeserializableModel):
     """A finalized deployment configuration
     This configuration must be complete, with enough details to submit a new deployment to the
     MosaicML Cloud.
     """
 
@@ -32,14 +53,17 @@
     image: str
     replicas: int
     env_variables: List[Dict[str, str]]
     integrations: List[Dict[str, Any]]
 
     metadata: Dict[str, Any] = field(default_factory=dict)
 
+    # Model config - optional for backwards-compatibility
+    model: ModelConfig = field(default_factory=ModelConfig)
+
     gpu_type: str = ''
     command: str = ''
 
     cluster: str = ''
 
     _property_translations = {
         'deployment_id': 'deployment_id',
@@ -49,14 +73,15 @@
         'cluster': 'cluster',
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
         'envVariables': 'env_variables',
         'integrations': 'integrations',
+        'model': 'model',
     }
 
     def __str__(self) -> str:
         return yaml.safe_dump(asdict(self))
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> FinalInferenceDeploymentConfig:
@@ -67,28 +92,35 @@
 
         if 'envVariables' not in response:
             response['envVariables'] = []
 
         if 'integrations' not in response:
             response['integrations'] = []
 
+        if 'model' not in response:
+            response['model'] = {
+                'checkpointPath': '',
+            }
+
         missing = set(cls._property_translations) - set(response)
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
                 message=('Missing required key(s) in response to deserialize '
                          f'FinalDeploymentConfig object: {", ".join(missing)}'),
             )
         data = {}
         for k, v in cls._property_translations.items():
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
+            elif v == 'model':
+                value = InferenceModelTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
 
     @classmethod
     def finalize_config(cls, deployment_config: InferenceDeploymentConfig) -> FinalInferenceDeploymentConfig:
         """Create a :class:`~mcli.models.deployment_config.FinalDeploymentConfig` from the provided
@@ -148,14 +180,16 @@
         translated_input = {}
         for field_name, value in asdict(self).items():
             translated_name = translations.get(field_name, field_name)
             if field_name == 'env_variables':
                 value = EnvVarTranslation.to_mapi(value)
             elif field_name == 'integrations':
                 value = IntegrationTranslation.to_mapi(value)
+            elif field_name == 'model':
+                value = InferenceModelTranslation.to_mapi(value)
             elif field_name == "gpu_type" and not value:
                 continue
             elif field_name == "cluster" and not value:
                 continue
             translated_input[translated_name] = value
         return {
             'inferenceDeploymentInput': translated_input,
@@ -183,25 +217,27 @@
     cluster: Optional[str] = None
     image: Optional[str] = None
     replicas: Optional[int] = None
     command: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     env_variables: List[Dict[str, str]] = field(default_factory=list)
     integrations: List[Dict[str, Any]] = field(default_factory=list)
+    model: ModelConfig = field(default_factory=ModelConfig)
 
     _property_translations = {
         'deploymentName': 'name',
         'gpuNum': 'gpu_num',
         'cluster': 'cluster',
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
         'envVariables': 'env_variables',
         'integrations': 'integrations',
+        'model': 'model',
     }
 
     _required_display_properties = {'name', 'image', 'command', 'replicas'}
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InferenceDeploymentConfig:
         data = {}
@@ -210,10 +246,61 @@
                 # This must be an optional property, so skip
                 continue
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
+            elif v == 'model':
+                value = InferenceModelTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
+
+
+class InferenceModelTranslation(Translation[ModelConfig, Dict[str, Any]]):
+    """Translate model configs to and from MAPI"""
+
+    CHECKPOINT_PATH = 'checkpoint_path'
+    HF_MODEL = 'hf_model'
+    CUSTOM_MODEL = 'custom_model'
+
+    @classmethod
+    def from_mapi(cls, value: Dict[str, Any]) -> ModelConfig:
+        checkpoint_path = value.pop(snake_case_to_camel_case(cls.CHECKPOINT_PATH))
+
+        translated_config = {}
+        for model_type, nested_model_config in value.items():
+            translated_model_type = camel_case_to_snake_case(model_type)
+            translated_config[translated_model_type] = {}
+
+            for key, val in nested_model_config.items():
+                # Translate keys to camel case for MAPI parameters
+                translated_key = camel_case_to_snake_case(key)
+                translated_config[translated_model_type][translated_key] = val
+
+        translated_config[cls.CHECKPOINT_PATH] = checkpoint_path
+        return ModelConfig(**translated_config)
+
+    @classmethod
+    def to_mapi(cls, value: ModelConfig) -> Dict[str, Any]:
+        checkpoint_path = value.pop(cls.CHECKPOINT_PATH)
+
+        translated_config = {}
+        for model_type, nested_model_config in value.items():
+            translated_model_type = snake_case_to_camel_case(model_type)
+            translated_config[translated_model_type] = {}
+
+            nested_model_config = None
+            if model_type == cls.HF_MODEL:
+                nested_model_config = value.get(cls.HF_MODEL)
+            elif model_type == cls.CUSTOM_MODEL:
+                nested_model_config = value.get(cls.CUSTOM_MODEL)
+
+            if nested_model_config:
+                for key, val in nested_model_config.items():
+                    # Translate keys to camel case for MAPI parameters
+                    translated_key = snake_case_to_camel_case(key)
+                    translated_config[translated_model_type][translated_key] = val
+
+        translated_config[snake_case_to_camel_case(cls.CHECKPOINT_PATH)] = checkpoint_path
+        return translated_config
```

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a2/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a2/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a2/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a2/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a2/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a2/mcli/sdk/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
                                             delete_inference_deployments, get_inference_deployments,
                                             ping_inference_deployment, predict)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
-                           follow_run_logs, get_run, get_run_logs, get_runs, stop_run, stop_runs, update_run_metadata,
-                           wait_for_run_status, watch_run_status)
+                           follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
+                           update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
```

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a2/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/mcli/version.py` & `mosaicml-cli-0.4.0a2/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a1"
+__version__ = "0.4.0a2"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 mcli/api/model/inference_deployment.py
 mcli/api/model/run.py
 mcli/api/runs/__init__.py
 mcli/api/runs/api_create_run.py
 mcli/api/runs/api_delete_runs.py
 mcli/api/runs/api_get_run_logs.py
 mcli/api/runs/api_get_runs.py
+mcli/api/runs/api_start_run.py
 mcli/api/runs/api_stop_runs.py
 mcli/api/runs/api_update_run_metadata.py
 mcli/api/runs/api_watch_run.py
 mcli/api/schema/__init__.py
 mcli/api/schema/generic_model.py
 mcli/api/secrets/__init__.py
 mcli/api/secrets/api_create_secret.py
```

### Comparing `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 
 [all]
-pytest-mock>=3.7.0
-pyright>=1.1.256
-sphinxcontrib-serializinghtml>=1.1.5
-yapf>=0.33.0
-pytest-cov>=4.0.0
-sphinx-panels>=0.6.0
-furo>=2022.3.4
-pylint>=2.12.2
-sphinxcontrib-devhelp>=1.0.2
-sphinxcontrib-katex>=0.8.6
-sphinx-copybutton>=0.5.0
-sphinx-design
-sphinx_external_toc>=0.3.0
 pytest>=6.2.5
-sphinx>=4.4.0
-sphinx-rtd-theme>=1.0.0
+sphinx_external_toc>=0.3.0
+pylint>=2.12.2
+pyright>=1.1.256
+toml>=0.10.2
 myst-parser>=0.16.1
+sphinx-design
+sphinxcontrib-applehelp>=1.0.2
+pytest-cov>=4.0.0
+sphinxcontrib-jsmath>=1.0.1
+sphinxemoji>=0.2.0
+sphinxcontrib-htmlhelp>=2.0.0
+sphinxcontrib-images>=0.9.4
+sphinx-markdown-tables>=0.0.15
 sphinxext-opengraph>=0.6.1
-sphinx-argparse>=0.3.1
+pytest-mock>=3.7.0
 isort>=5.9.3
+sphinx>=4.4.0
+furo>=2022.3.4
+sphinx-rtd-theme>=1.0.0
+sphinxcontrib-serializinghtml>=1.1.5
+yapf>=0.33.0
+sphinx-panels>=0.6.0
+sphinxcontrib-qthelp>=1.0.3
 radon>=5.1.0
+sphinx-copybutton>=0.5.0
 pre-commit>=2.17.0
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-jsmath>=1.0.1
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-applehelp>=1.0.2
-sphinxcontrib-qthelp>=1.0.3
-sphinx-markdown-tables>=0.0.15
-sphinxemoji>=0.2.0
-toml>=0.10.2
+sphinxcontrib-katex>=0.8.6
+sphinx-argparse>=0.3.1
+sphinxcontrib-devhelp>=1.0.2
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest-cov>=4.0.0
```

### Comparing `mosaicml-cli-0.4.0a1/pyproject.toml` & `mosaicml-cli-0.4.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/setup.py` & `mosaicml-cli-0.4.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/tests/test_config.py` & `mosaicml-cli-0.4.0a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a1/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a2/tests/test_upgrade.py`

 * *Files identical despite different names*

