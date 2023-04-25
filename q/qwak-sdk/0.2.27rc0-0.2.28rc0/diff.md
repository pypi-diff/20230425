# Comparing `tmp/qwak_sdk-0.2.27rc0.tar.gz` & `tmp/qwak_sdk-0.2.28rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_sdk-0.2.27rc0.tar", max compression
+gzip compressed data, was "qwak_sdk-0.2.28rc0.tar", max compression
```

## Comparing `qwak_sdk-0.2.27rc0.tar` & `qwak_sdk-0.2.28rc0.tar`

### file list

```diff
@@ -1,302 +1,302 @@
--rw-r--r--   0        0        0      183 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/README.md
--rw-r--r--   0        0        0     2617 2023-04-24 09:02:59.412293 qwak_sdk-0.2.27rc0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-04-24 09:02:59.392293 qwak_sdk-0.2.27rc0/qwak_sdk/__init__.py
--rw-r--r--   0        0        0     2039 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/cli.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/__init__.py
--rw-r--r--   0        0        0      327 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/admin_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/__init__.py
--rw-r--r--   0        0        0      477 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/generate/__init__.py
--rw-r--r--   0        0        0      677 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py
--rw-r--r--   0        0        0     1403 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
--rw-r--r--   0        0        0      796 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
--rw-r--r--   0        0        0      952 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/__init__.py
--rw-r--r--   0        0        0      367 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/config_base.py
--rw-r--r--   0        0        0      885 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
--rw-r--r--   0        0        0      886 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
--rw-r--r--   0        0        0     1626 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
--rw-r--r--   0        0        0      817 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
--rw-r--r--   0        0        0      340 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
--rw-r--r--   0        0        0      277 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/spec.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/__init__.py
--rw-r--r--   0        0        0       49 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
--rw-r--r--   0        0        0     3098 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py
--rw-r--r--   0        0        0      646 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/attach/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py
--rw-r--r--   0        0        0      949 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/attach/ui.py
--rw-r--r--   0        0        0      277 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/__init__.py
--rw-r--r--   0        0        0      857 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/automations_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/delete/__init__.py
--rw-r--r--   0        0        0      235 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/delete/_logic.py
--rw-r--r--   0        0        0      604 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/__init__.py
--rw-r--r--   0        0        0      346 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/executions_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/list/__init__.py
--rw-r--r--   0        0        0      330 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/list/_logic.py
--rw-r--r--   0        0        0      669 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/list/__init__.py
--rw-r--r--   0        0        0      252 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/list/_logic.py
--rw-r--r--   0        0        0      546 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/register/__init__.py
--rw-r--r--   0        0        0     1624 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/register/_logic.py
--rw-r--r--   0        0        0     1331 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/register/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/delete/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/delete/_logic.py
--rw-r--r--   0        0        0     1039 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/delete/ui.py
--rw-r--r--   0        0        0     1002 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/list/__init__.py
--rw-r--r--   0        0        0     4145 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/pause/__init__.py
--rw-r--r--   0        0        0      695 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/pause/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/register/__init__.py
--rw-r--r--   0        0        0    10893 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/register/_logic.py
--rw-r--r--   0        0        0     2822 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/register/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/resume/__init__.py
--rw-r--r--   0        0        0      700 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/resume/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/trigger/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/trigger/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/_logic/__init__.py
--rw-r--r--   0        0        0     2050 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/__init__.py
--rw-r--r--   0        0        0     2005 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/build_steps.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
--rw-r--r--   0        0        0     6129 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
--rw-r--r--   0        0        0     4383 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
--rw-r--r--   0        0        0     2908 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
--rw-r--r--   0        0        0     1369 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
--rw-r--r--   0        0        0     1435 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
--rw-r--r--   0        0        0      359 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
--rw-r--r--   0        0        0      975 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
--rw-r--r--   0        0        0      311 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
--rw-r--r--   0        0        0     9876 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py
--rw-r--r--   0        0        0      131 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
--rw-r--r--   0        0        0      881 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py
--rw-r--r--   0        0        0       73 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
--rw-r--r--   0        0        0      189 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
--rw-r--r--   0        0        0     1872 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/context.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/interface/__init__.py
--rw-r--r--   0        0        0      568 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
--rw-r--r--   0        0        0      745 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/__init__.py
--rw-r--r--   0        0        0      421 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
--rw-r--r--   0        0        0     1929 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      957 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     1917 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     2589 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     2025 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2232 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     4459 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
--rw-r--r--   0        0        0     5385 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
--rw-r--r--   0        0        0      274 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      611 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1605 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0    11882 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0      183 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
--rw-r--r--   0        0        0     1644 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/__init__.py
--rw-r--r--   0        0        0     1686 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
--rw-r--r--   0        0        0     1181 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
--rw-r--r--   0        0        0      188 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/text.py
--rw-r--r--   0        0        0     7125 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/__init__.py
--rw-r--r--   0        0        0      491 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/builds_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/cancel/__init__.py
--rw-r--r--   0        0        0      181 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/cancel/_logic.py
--rw-r--r--   0        0        0      528 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/cancel/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/logs/__init__.py
--rw-r--r--   0        0        0     1054 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/logs/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/status/__init__.py
--rw-r--r--   0        0        0      256 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/status/_logic.py
--rw-r--r--   0        0        0      983 2023-04-24 09:02:21.060322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/status/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/create/__init__.py
--rw-r--r--   0        0        0     1335 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/create/_logic.py
--rw-r--r--   0        0        0     1016 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/create/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/delete/__init__.py
--rw-r--r--   0        0        0      186 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/delete/_logic.py
--rw-r--r--   0        0        0      638 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
--rw-r--r--   0        0        0     1251 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
--rw-r--r--   0        0        0     2494 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
--rw-r--r--   0        0        0     8227 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
--rw-r--r--   0        0        0    13221 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
--rw-r--r--   0        0        0     3900 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
--rw-r--r--   0        0        0     5809 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
--rw-r--r--   0        0        0      770 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
--rw-r--r--   0        0        0     1067 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
--rw-r--r--   0        0        0     3166 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
--rw-r--r--   0        0        0      495 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      903 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3025 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
--rw-r--r--   0        0        0      500 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
--rw-r--r--   0        0        0      902 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      907 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3621 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     4926 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
--rw-r--r--   0        0        0      905 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
--rw-r--r--   0        0        0     1500 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     5391 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
--rw-r--r--   0        0        0     5783 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
--rw-r--r--   0        0        0     3036 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
--rw-r--r--   0        0        0     2093 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/cancel/__init__.py
--rw-r--r--   0        0        0      409 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/cancel/_logic.py
--rw-r--r--   0        0        0      838 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/cancel/ui.py
--rw-r--r--   0        0        0      799 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/execution_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/report/__init__.py
--rw-r--r--   0        0        0      533 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/report/_logic.py
--rw-r--r--   0        0        0     1445 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/report/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/start/__init__.py
--rw-r--r--   0        0        0      605 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/start/_logic.py
--rw-r--r--   0        0        0     5168 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/start/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/status/__init__.py
--rw-r--r--   0        0        0      480 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/status/_logic.py
--rw-r--r--   0        0        0      830 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/status/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
--rw-r--r--   0        0        0       35 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       84 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      164 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0   129370 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3606 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
--rw-r--r--   0        0        0       41 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       74 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      161 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0    53393 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3963 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
--rw-r--r--   0        0        0      139 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      120 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
--rw-r--r--   0        0        0      140 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
--rw-r--r--   0        0        0     2165 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
--rw-r--r--   0        0        0      117 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
--rw-r--r--   0        0        0       61 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      182 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0     3349 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      751 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
--rw-r--r--   0        0        0       68 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0     3349 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0      448 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      752 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0     1916 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/list/__init__.py
--rw-r--r--   0        0        0      166 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/list/_logic.py
--rw-r--r--   0        0        0     1135 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/list/ui.py
--rw-r--r--   0        0        0     1241 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/models_command_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/feedback/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py
--rw-r--r--   0        0        0     1378 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/feedback/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/logs/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/logs/ui.py
--rw-r--r--   0        0        0      693 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
--rw-r--r--   0        0        0     1821 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
--rw-r--r--   0        0        0     3160 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
--rw-r--r--   0        0        0     1222 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/update/__init__.py
--rw-r--r--   0        0        0      393 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/update/_logic.py
--rw-r--r--   0        0        0      622 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/update/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/create/__init__.py
--rw-r--r--   0        0        0      259 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/create/_logic.py
--rw-r--r--   0        0        0      691 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/create/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/delete/__init__.py
--rw-r--r--   0        0        0      203 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/delete/_logic.py
--rw-r--r--   0        0        0      557 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/list/__init__.py
--rw-r--r--   0        0        0      182 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/list/_logic.py
--rw-r--r--   0        0        0     1124 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/list/ui.py
--rw-r--r--   0        0        0      589 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/projects_command_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/delete/__init__.py
--rw-r--r--   0        0        0      141 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/delete/_logic.py
--rw-r--r--   0        0        0      741 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/get/__init__.py
--rw-r--r--   0        0        0      142 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/get/_logic.py
--rw-r--r--   0        0        0      574 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/get/ui.py
--rw-r--r--   0        0        0      502 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/secrets_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/set/__init__.py
--rw-r--r--   0        0        0      149 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/set/_logic.py
--rw-r--r--   0        0        0      615 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/set/ui.py
--rw-r--r--   0        0        0      430 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/commands/ui_tools.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/common/__init__.py
--rw-r--r--   0        0        0      437 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/common/run_config/__init__.py
--rw-r--r--   0        0        0     3166 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/common/run_config/base.py
--rw-r--r--   0        0        0     6087 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/common/run_config/utils.py
--rw-r--r--   0        0        0      381 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_command_exception.py
--rw-r--r--   0        0        0      133 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
--rw-r--r--   0        0        0      424 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      130 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0       48 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_resource_not_found.py
--rw-r--r--   0        0        0      746 2023-04-24 09:02:21.064322 qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/__init__.py
--rw-r--r--   0        0        0     3164 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/file_registry.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/__init__.py
--rw-r--r--   0        0        0     4541 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/cli_tools.py
--rw-r--r--   0        0        0      488 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/config_handler.py
--rw-r--r--   0        0        0       71 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/logger/__init__.py
--rw-r--r--   0        0        0     8869 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/logger/logging.yml
--rw-r--r--   0        0        0     1013 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/tracking.py
--rw-r--r--   0        0        0      136 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/main.py
--rw-r--r--   0        0        0        0 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/tools/__init__.py
--rw-r--r--   0        0        0      287 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/tools/colors.py
--rw-r--r--   0        0        0      174 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/tools/files.py
--rw-r--r--   0        0        0     5616 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/tools/log_handling.py
--rw-r--r--   0        0        0     1192 2023-04-24 09:02:21.068322 qwak_sdk-0.2.27rc0/qwak_sdk/tools/utils.py
--rw-r--r--   0        0        0     8334 1970-01-01 00:00:00.000000 qwak_sdk-0.2.27rc0/setup.py
--rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 qwak_sdk-0.2.27rc0/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/README.md
+-rw-r--r--   0        0        0     2617 2023-04-25 09:07:53.970791 qwak_sdk-0.2.28rc0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-04-25 09:07:53.970791 qwak_sdk-0.2.28rc0/qwak_sdk/__init__.py
+-rw-r--r--   0        0        0     2039 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/cli.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/admin_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/generate/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py
+-rw-r--r--   0        0        0     1403 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
+-rw-r--r--   0        0        0      796 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
+-rw-r--r--   0        0        0      952 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/config_base.py
+-rw-r--r--   0        0        0      885 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
+-rw-r--r--   0        0        0     1626 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
+-rw-r--r--   0        0        0      817 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
+-rw-r--r--   0        0        0      340 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
+-rw-r--r--   0        0        0      277 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/spec.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
+-rw-r--r--   0        0        0     3098 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py
+-rw-r--r--   0        0        0      646 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/attach/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py
+-rw-r--r--   0        0        0      949 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/attach/ui.py
+-rw-r--r--   0        0        0      277 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/__init__.py
+-rw-r--r--   0        0        0      857 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/automations_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/delete/__init__.py
+-rw-r--r--   0        0        0      235 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/delete/_logic.py
+-rw-r--r--   0        0        0      604 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/__init__.py
+-rw-r--r--   0        0        0      346 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/executions_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/list/__init__.py
+-rw-r--r--   0        0        0      330 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/list/_logic.py
+-rw-r--r--   0        0        0      669 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/list/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/list/__init__.py
+-rw-r--r--   0        0        0      252 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/list/_logic.py
+-rw-r--r--   0        0        0      546 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/list/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/register/__init__.py
+-rw-r--r--   0        0        0     1624 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/register/_logic.py
+-rw-r--r--   0        0        0     1331 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/register/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/delete/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/delete/_logic.py
+-rw-r--r--   0        0        0     1039 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/delete/ui.py
+-rw-r--r--   0        0        0     1002 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/list/__init__.py
+-rw-r--r--   0        0        0     4145 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/list/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/pause/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/pause/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/register/__init__.py
+-rw-r--r--   0        0        0    10893 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/register/_logic.py
+-rw-r--r--   0        0        0     2822 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/register/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/resume/__init__.py
+-rw-r--r--   0        0        0      700 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/resume/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/trigger/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/trigger/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/_logic/__init__.py
+-rw-r--r--   0        0        0     2050 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/__init__.py
+-rw-r--r--   0        0        0     2005 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/build_steps.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.350681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
+-rw-r--r--   0        0        0     6129 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
+-rw-r--r--   0        0        0     4383 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
+-rw-r--r--   0        0        0     2908 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
+-rw-r--r--   0        0        0     1369 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
+-rw-r--r--   0        0        0     1435 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
+-rw-r--r--   0        0        0      359 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
+-rw-r--r--   0        0        0      975 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
+-rw-r--r--   0        0        0      311 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
+-rw-r--r--   0        0        0     9876 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py
+-rw-r--r--   0        0        0      131 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
+-rw-r--r--   0        0        0      881 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py
+-rw-r--r--   0        0        0       73 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
+-rw-r--r--   0        0        0      189 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
+-rw-r--r--   0        0        0     1872 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/context.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/interface/__init__.py
+-rw-r--r--   0        0        0      568 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
+-rw-r--r--   0        0        0      745 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
+-rw-r--r--   0        0        0     1929 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     1917 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     2589 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     2025 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2232 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     4459 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
+-rw-r--r--   0        0        0     5385 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0      274 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      611 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1605 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0    11882 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0      183 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
+-rw-r--r--   0        0        0     1644 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/__init__.py
+-rw-r--r--   0        0        0     1686 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
+-rw-r--r--   0        0        0     1181 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
+-rw-r--r--   0        0        0      188 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/text.py
+-rw-r--r--   0        0        0     7125 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/builds_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/cancel/__init__.py
+-rw-r--r--   0        0        0      181 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/cancel/_logic.py
+-rw-r--r--   0        0        0      528 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/cancel/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/logs/__init__.py
+-rw-r--r--   0        0        0     1054 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/logs/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/status/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/status/_logic.py
+-rw-r--r--   0        0        0      983 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/status/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/create/__init__.py
+-rw-r--r--   0        0        0     1335 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/create/_logic.py
+-rw-r--r--   0        0        0     1016 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/create/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/delete/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/delete/_logic.py
+-rw-r--r--   0        0        0      638 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
+-rw-r--r--   0        0        0     1251 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
+-rw-r--r--   0        0        0     2494 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
+-rw-r--r--   0        0        0     8227 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
+-rw-r--r--   0        0        0    13221 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
+-rw-r--r--   0        0        0     3900 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
+-rw-r--r--   0        0        0     5809 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
+-rw-r--r--   0        0        0      770 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
+-rw-r--r--   0        0        0     1067 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
+-rw-r--r--   0        0        0     3166 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      903 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3025 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
+-rw-r--r--   0        0        0      500 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
+-rw-r--r--   0        0        0      902 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      907 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3621 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     4926 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
+-rw-r--r--   0        0        0      905 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     1500 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     5391 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
+-rw-r--r--   0        0        0     5783 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
+-rw-r--r--   0        0        0     3036 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
+-rw-r--r--   0        0        0     2093 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/cancel/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/cancel/_logic.py
+-rw-r--r--   0        0        0      838 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/cancel/ui.py
+-rw-r--r--   0        0        0      799 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/execution_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/report/__init__.py
+-rw-r--r--   0        0        0      533 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/report/_logic.py
+-rw-r--r--   0        0        0     1445 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/report/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/start/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/start/_logic.py
+-rw-r--r--   0        0        0     5168 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/start/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/status/__init__.py
+-rw-r--r--   0        0        0      480 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/status/_logic.py
+-rw-r--r--   0        0        0      830 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/status/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-25 09:07:06.354681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0   129370 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3610 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0     1030 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0    53393 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3967 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
+-rw-r--r--   0        0        0      139 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
+-rw-r--r--   0        0        0     2169 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0     3353 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      751 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0     3353 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0      448 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      752 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0     1916 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/list/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/list/_logic.py
+-rw-r--r--   0        0        0     1135 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/list/ui.py
+-rw-r--r--   0        0        0     1241 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/models_command_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/feedback/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py
+-rw-r--r--   0        0        0     1378 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/feedback/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/logs/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/logs/ui.py
+-rw-r--r--   0        0        0      693 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
+-rw-r--r--   0        0        0     1821 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
+-rw-r--r--   0        0        0     3160 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
+-rw-r--r--   0        0        0     1222 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/update/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/update/_logic.py
+-rw-r--r--   0        0        0      622 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/update/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/create/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/create/_logic.py
+-rw-r--r--   0        0        0      691 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/create/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/delete/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/delete/_logic.py
+-rw-r--r--   0        0        0      557 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/list/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/list/_logic.py
+-rw-r--r--   0        0        0     1124 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/list/ui.py
+-rw-r--r--   0        0        0      589 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/projects_command_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/delete/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/delete/_logic.py
+-rw-r--r--   0        0        0      741 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/get/__init__.py
+-rw-r--r--   0        0        0      142 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/get/_logic.py
+-rw-r--r--   0        0        0      574 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/get/ui.py
+-rw-r--r--   0        0        0      502 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/secrets_commands_group.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/set/__init__.py
+-rw-r--r--   0        0        0      149 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/set/_logic.py
+-rw-r--r--   0        0        0      615 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/set/ui.py
+-rw-r--r--   0        0        0      430 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/commands/ui_tools.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/common/__init__.py
+-rw-r--r--   0        0        0      437 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/common/run_config/__init__.py
+-rw-r--r--   0        0        0     3166 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/common/run_config/base.py
+-rw-r--r--   0        0        0     6087 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/common/run_config/utils.py
+-rw-r--r--   0        0        0      381 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_command_exception.py
+-rw-r--r--   0        0        0      133 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
+-rw-r--r--   0        0        0      424 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      130 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0       48 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_resource_not_found.py
+-rw-r--r--   0        0        0      746 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/__init__.py
+-rw-r--r--   0        0        0     3164 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/file_registry.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/__init__.py
+-rw-r--r--   0        0        0     4541 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/cli_tools.py
+-rw-r--r--   0        0        0      488 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/config_handler.py
+-rw-r--r--   0        0        0       71 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/logger/__init__.py
+-rw-r--r--   0        0        0     8869 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/logger/logging.yml
+-rw-r--r--   0        0        0     1013 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/tracking.py
+-rw-r--r--   0        0        0      136 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/tools/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/tools/colors.py
+-rw-r--r--   0        0        0      174 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/tools/files.py
+-rw-r--r--   0        0        0     5616 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/tools/log_handling.py
+-rw-r--r--   0        0        0     1192 2023-04-25 09:07:06.358681 qwak_sdk-0.2.28rc0/qwak_sdk/tools/utils.py
+-rw-r--r--   0        0        0     8334 1970-01-01 00:00:00.000000 qwak_sdk-0.2.28rc0/setup.py
+-rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 qwak_sdk-0.2.28rc0/PKG-INFO
```

### Comparing `qwak_sdk-0.2.27rc0/pyproject.toml` & `qwak_sdk-0.2.28rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-sdk"
-version = "0.2.27.rc0"
+version = "0.2.28.rc0"
 description = "Qwak SDK and CLI for qwak models"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak_sdk"},
 ]
@@ -23,15 +23,15 @@
 "Home page" = "https://www.qwak.com/"
 
 [tool.poetry.scripts]
 qwak = "qwak_sdk.main:qwak_cli"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-qwak-core = "==0.0.29"
+qwak-core = "==0.0.35"
 qwak-inference = "==0.0.10.rc0"
 tabulate = ">=0.8.0"
 python-json-logger = ">=2.0.2"
 pydantic = "*"
 yaspin = ">=2.0.0"
 assertpy = "^1.1"
 cookiecutter = "*"
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/cli.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/parser.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/auto_scalling/attach/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/auto_scalling/attach/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/automations_commands_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/automations_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/delete/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/executions/list/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/executions/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/list/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/register/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/automations/register/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/automations/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/delete/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/delete/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/delete/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/list/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/pause/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/pause/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/register/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/register/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/resume/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/resume/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/feature_store/trigger/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/feature_store/trigger/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/_logic/variations.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/build_steps.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/build_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/context.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/context.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/build/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/build/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/cancel/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/logs/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/builds/status/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/builds/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/create/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/create/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/create/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/delete/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/cancel/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/execution_commands_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/execution_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/report/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/report/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/report/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/report/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/start/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/start/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/start/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/start/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/executions/status/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/executions/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,18 +57,18 @@
 
         y_predicted = self.catboost.predict(X_validation)
         f1 = f1_score(y_validation, y_predicted)
 
         qwak.log_metric({"f1_score": f1})
 
     def schema(self):
-        from qwak.model.schema import ExplicitFeature, ModelSchema, Prediction
+        from qwak.model.schema import ExplicitFeature, InferenceOutput, ModelSchema
 
         model_schema = ModelSchema(
-            features=[
+            inputs=[
                 ExplicitFeature(name="User_Id", type=str),
                 ExplicitFeature(name="State", type=str),
                 ExplicitFeature(name="Account_Length", type=int),
                 ExplicitFeature(name="Area_Code", type=int),
                 ExplicitFeature(name="Intl_Plan", type=int),
                 ExplicitFeature(name="VMail_Plan", type=int),
                 ExplicitFeature(name="VMail_Message", type=int),
@@ -79,15 +79,15 @@
                 ExplicitFeature(name="Night_Mins", type=float),
                 ExplicitFeature(name="Night_Calls", type=int),
                 ExplicitFeature(name="Intl_Mins", type=float),
                 ExplicitFeature(name="Intl_Calls", type=int),
                 ExplicitFeature(name="CustServ_Calls", type=int),
                 ExplicitFeature(name="Agitation_Level", type=int),
             ],
-            predictions=[Prediction(name="Churn_Probability", type=float)],
+            outputs=[InferenceOutput(name="Churn_Probability", type=float)],
         )
         return model_schema
 
     @qwak.api()
     def predict(self, df):
         df = df.drop(["User_Id"], axis=1)
         return pd.DataFrame(
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import numpy as np
 import pandas as pd
 import qwak
 from catboost import CatBoostClassifier, Pool, cv
 from qwak.model.base import QwakModel
-from qwak.model.schema import ExplicitFeature, ModelSchema, Prediction
+from qwak.model.schema import ExplicitFeature, InferenceOutput, ModelSchema
 from sklearn.model_selection import train_test_split
 
 RUNNING_FILE_ABSOLUTE_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 class CreditRisk(QwakModel):
     """The Model class inherit QwakModel base class"""
@@ -80,28 +80,28 @@
                 np.max(cv_data["test-Accuracy-mean"])
             )
         )
         qwak.log_metric({"val_accuracy": np.max(cv_data["test-Accuracy-mean"])})
 
     def schema(self):
         return ModelSchema(
-            features=[
+            inputs=[
                 ExplicitFeature(name="UserId", type=str),
                 ExplicitFeature(name="Age", type=int),
                 ExplicitFeature(name="Sex", type=str),
                 ExplicitFeature(name="Job", type=int),
                 ExplicitFeature(name="Housing", type=str),
                 ExplicitFeature(name="Saving accounts", type=str),
                 ExplicitFeature(name="Checking account", type=str),
                 ExplicitFeature(name="Credit amount", type=float),
                 ExplicitFeature(name="Duration", type=int),
                 ExplicitFeature(name="Purpose", type=str),
                 ExplicitFeature(name="Age_cat", type=str),
             ],
-            predictions=[Prediction(name="Default_Probability", type=float)],
+            outputs=[InferenceOutput(name="Default_Probability", type=float)],
         )
 
     @qwak.api()
     def predict(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.drop(["UserId"], axis=1)
         return pd.DataFrame(
             self.model.predict_proba(df)[:, 1], columns=["Default_Probability"]
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,23 +22,23 @@
            """
         pass
 
     def schema(self):
         """ Specification of the model inputs and outputs. Optional method
 
         Example:
-        >>> from qwak.model.schema import ModelSchema, Prediction, ExplicitFeature
+        >>> from qwak.model.schema import ModelSchema, InferenceOutput, ExplicitFeature
         >>>
         >>> def schema(self) -> ModelSchema:
         >>>     model_schema = ModelSchema(
-        >>>     features=[
+        >>>     inputs=[
         >>>         ExplicitFeature(name="State", type=str),
         >>>     ],
-        >>>     predictions=[
-        >>>         Prediction(name="score", type=float)
+        >>>     outputs=[
+        >>>         InferenceOutput(name="score", type=float)
         >>>     ])
         >>>     return model_schema
 
        Returns: a model schema specification
        """
         pass
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 import qwak
 from catboost import CatBoostClassifier, Pool, cv
 from catboost.datasets import titanic
 from qwak.model.base import QwakModel
-from qwak.model.schema import ExplicitFeature, ModelSchema, Prediction
+from qwak.model.schema import ExplicitFeature, InferenceOutput, ModelSchema
 from sklearn.model_selection import train_test_split
 
 
 class TitanicSurvivalPrediction(QwakModel):
     def __init__(self):
         loss_function = os.getenv("loss_fn", "Logloss")
         learning_rate = os.getenv("learning_rate", None)
@@ -70,28 +70,28 @@
                 np.max(cv_data["test-Accuracy-mean"])
             )
         )
         qwak.log_metric({"val_accuracy": np.max(cv_data["test-Accuracy-mean"])})
 
     def schema(self):
         return ModelSchema(
-            features=[
+            inputs=[
                 ExplicitFeature(name="PassengerId", type=int),
                 ExplicitFeature(name="Pclass", type=int),
                 ExplicitFeature(name="Name", type=str),
                 ExplicitFeature(name="Sex", type=str),
                 ExplicitFeature(name="Age", type=int),
                 ExplicitFeature(name="SibSp", type=int),
                 ExplicitFeature(name="Parch", type=int),
                 ExplicitFeature(name="Ticket", type=str),
                 ExplicitFeature(name="Fare", type=float),
                 ExplicitFeature(name="Cabin", type=str),
                 ExplicitFeature(name="Embarked", type=str),
             ],
-            predictions=[Prediction(name="Survived_Probability", type=float)],
+            outputs=[InferenceOutput(name="Survived_Probability", type=float)],
         )
 
     @qwak.api()
     def predict(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.drop(["PassengerId"], axis=1)
         return pd.DataFrame(
             self.model.predict_proba(df)[:, 1], columns=["Survived_Probability"]
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 import qwak
 from catboost import CatBoostClassifier, Pool, cv
 from catboost.datasets import titanic
 from qwak.model.base import QwakModel
-from qwak.model.schema import ExplicitFeature, ModelSchema, Prediction
+from qwak.model.schema import ExplicitFeature, InferenceOutput, ModelSchema
 from sklearn.model_selection import train_test_split
 
 
 class TitanicSurvivalPrediction(QwakModel):
     def __init__(self):
         loss_function = os.getenv("loss_fn", "Logloss")
         learning_rate = os.getenv("learning_rate", None)
@@ -70,28 +70,28 @@
                 np.max(cv_data["test-Accuracy-mean"])
             )
         )
         qwak.log_metric({"val_accuracy": np.max(cv_data["test-Accuracy-mean"])})
 
     def schema(self):
         return ModelSchema(
-            features=[
+            inputs=[
                 ExplicitFeature(name="PassengerId", type=int),
                 ExplicitFeature(name="Pclass", type=int),
                 ExplicitFeature(name="Name", type=str),
                 ExplicitFeature(name="Sex", type=str),
                 ExplicitFeature(name="Age", type=int),
                 ExplicitFeature(name="SibSp", type=int),
                 ExplicitFeature(name="Parch", type=int),
                 ExplicitFeature(name="Ticket", type=str),
                 ExplicitFeature(name="Fare", type=float),
                 ExplicitFeature(name="Cabin", type=str),
                 ExplicitFeature(name="Embarked", type=str),
             ],
-            predictions=[Prediction(name="Survived_Probability", type=float)],
+            outputs=[InferenceOutput(name="Survived_Probability", type=float)],
         )
 
     @qwak.api()
     def predict(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.drop(["PassengerId"], axis=1)
         return pd.DataFrame(
             self.model.predict_proba(df)[:, 1], columns=["Survived_Probability"]
```

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/init/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/init/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/list/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/models_command_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/models_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/feedback/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/feedback/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/logs/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/models/runtime/update/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/models/runtime/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/create/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/delete/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/list/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/projects/projects_command_group.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/projects/projects_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/delete/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/get/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/commands/secrets/set/ui.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/commands/secrets/set/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/common/run_config/base.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/common/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/common/run_config/utils.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/common/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/inner/file_registry.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/inner/file_registry.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/cli_tools.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/logger/logger.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/logger/logging.yml` & `qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/inner/tools/tracking.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/inner/tools/tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/tools/log_handling.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/tools/log_handling.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/qwak_sdk/tools/utils.py` & `qwak_sdk-0.2.28rc0/qwak_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.27rc0/setup.py` & `qwak_sdk-0.2.28rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 install_requires = \
 ['assertpy>=1.1,<2.0',
  'cookiecutter',
  'gitpython>=2.1.0',
  'pydantic',
  'python-json-logger>=2.0.2',
- 'qwak-core==0.0.29',
+ 'qwak-core==0.0.35',
  'qwak-inference==0.0.10.rc0',
  'tabulate>=0.8.0',
  'yaspin>=2.0.0']
 
 extras_require = \
 {'batch': ['boto3>=1.24.89,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
@@ -147,15 +147,15 @@
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['qwak = qwak_sdk.main:qwak_cli']}
 
 setup_kwargs = {
     'name': 'qwak-sdk',
-    'version': '0.2.27rc0',
+    'version': '0.2.28rc0',
     'description': 'Qwak SDK and CLI for qwak models',
     'long_description': '# Qwak SDK\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_sdk-0.2.27rc0/PKG-INFO` & `qwak_sdk-0.2.28rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sdk
-Version: 0.2.27rc0
+Version: 0.2.28rc0
 Summary: Qwak SDK and CLI for qwak models
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,15 +25,15 @@
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
 Requires-Dist: pydantic
 Requires-Dist: python-json-logger (>=2.0.2)
-Requires-Dist: qwak-core (==0.0.29)
+Requires-Dist: qwak-core (==0.0.35)
 Requires-Dist: qwak-inference (==0.0.10.rc0)
 Requires-Dist: tabulate (>=0.8.0)
 Requires-Dist: yaspin (>=2.0.0)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
 
 # Qwak SDK
```

