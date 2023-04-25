# Comparing `tmp/cloudify-common-6.4.2.0.tar.gz` & `tmp/cloudify-common-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-common-6.4.2.tar", last modified: Mon Feb  6 10:36:09 2023, max compression
+gzip compressed data, was "cloudify-common-7.0.0.tar", last modified: Tue Apr 25 11:53:36 2023, max compression
```

## Comparing `cloudify-common-6.4.2.0.tar` & `cloudify-common-7.0.0.tar`

### file list

```diff
@@ -1,214 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/
--rw-r--r--   0 root         (0) root         (0)    10273 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       39 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      258 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3034 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/
--rw-r--r--   0 root         (0) root         (0)     2286 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/_compat.py
--rw-r--r--   0 root         (0) root         (0)     4948 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)    24364 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/amqp_client.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/cluster_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/compute/
--rw-r--r--   0 root         (0) root         (0)     4460 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/conflict_handlers.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/constants.py
--rw-r--r--   0 root         (0) root         (0)    43031 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/context.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/cryptography_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/ctx_wrappers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8429 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/ctx_wrappers/ctx-py.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/decorators.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)    18447 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/dispatch.py
--rw-r--r--   0 root         (0) root         (0)    16788 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/endpoint.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/error_handling.py
--rw-r--r--   0 root         (0) root         (0)     4886 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/event.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    17145 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/logs.py
--rw-r--r--   0 root         (0) root         (0)    18173 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/manager.py
--rw-r--r--   0 root         (0) root         (0)     7626 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/mocks.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/models_states.py
--rw-r--r--   0 root         (0) root         (0)    19753 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/plugin_installer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/plugins/
--rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/plugins/install_utils.py
--rw-r--r--   0 root         (0) root         (0)    53975 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/plugins/lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    56057 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/plugins/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/proxy/
--rw-r--r--   0 root         (0) root         (0)      637 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3965 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/proxy/client.py
--rw-r--r--   0 root         (0) root         (0)     8182 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/proxy/server.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/rabbitmq_client.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/snapshots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.222518 cloudify-common-6.4.2/cloudify/snmp/
--rw-r--r--   0 root         (0) root         (0)     5393 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/snmp/CLOUDIFY-MIB.mib
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/snmp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4934 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/snmp/snmp_trap.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/state.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/systemddbus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.226518 cloudify-common-6.4.2/cloudify/test_utils/
--rw-r--r--   0 root         (0) root         (0)      751 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/test_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/test_utils/dispatch_helper.py
--rw-r--r--   0 root         (0) root         (0)    11243 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/test_utils/local_workflow_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/test_utils/mock_rest_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.226518 cloudify-common-6.4.2/cloudify/tests/
--rw-r--r--   0 root         (0) root         (0)     1178 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62608 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_builtin_workflows.py
--rw-r--r--   0 root         (0) root         (0)    33385 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)    15849 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_ctx_relationships.py
--rw-r--r--   0 root         (0) root         (0)    12607 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_decorators.py
--rw-r--r--   0 root         (0) root         (0)     8181 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     5315 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_event.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_install_agent_local_workflow.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_install_new_agents_workflow.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_keep_trying_http.py
--rw-r--r--   0 root         (0) root         (0)     8494 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_lifecycle_retry.py
--rw-r--r--   0 root         (0) root         (0)     4870 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_local_get_attribute.py
--rw-r--r--   0 root         (0) root         (0)    62936 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_local_workflows.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_local_workflows_init.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_logs.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_node_state.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_operation_retry.py
--rw-r--r--   0 root         (0) root         (0)    13089 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_state.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_task_retry.py
--rw-r--r--   0 root         (0) root         (0)     4251 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_task_retry_event_context.py
--rw-r--r--   0 root         (0) root         (0)     5419 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_task_serialize.py
--rw-r--r--   0 root         (0) root         (0)     7579 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_task_subgraph.py
--rw-r--r--   0 root         (0) root         (0)    25777 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_tasks_graph.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/tests/workflows.py
--rw-r--r--   0 root         (0) root         (0)    35981 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.226518 cloudify-common-6.4.2/cloudify/workflows/
--rw-r--r--   0 root         (0) root         (0)      848 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/amqp_dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/events.py
--rw-r--r--   0 root         (0) root         (0)    36765 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/local.py
--rw-r--r--   0 root         (0) root         (0)    39927 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/tasks.py
--rw-r--r--   0 root         (0) root         (0)    25643 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/tasks_graph.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/workflow_api.py
--rw-r--r--   0 root         (0) root         (0)    78197 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/workflows/workflow_context.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify/zip_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.226518 cloudify-common-6.4.2/cloudify_async_client/
--rw-r--r--   0 root         (0) root         (0)       69 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_async_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_async_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_async_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.230518 cloudify-common-6.4.2/cloudify_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6046 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      302 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-02-06 10:36:09.000000 cloudify-common-6.4.2/cloudify_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.234518 cloudify-common-6.4.2/cloudify_rest_client/
--rw-r--r--   0 root         (0) root         (0)      731 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/_compat.py
--rw-r--r--   0 root         (0) root         (0)     7532 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/agents.py
--rw-r--r--   0 root         (0) root         (0)     3411 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    21601 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/blueprints.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/bytes_stream_utils.py
--rw-r--r--   0 root         (0) root         (0)    22111 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/client.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/constants.py
--rw-r--r--   0 root         (0) root         (0)     6367 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/deployment_modifications.py
--rw-r--r--   0 root         (0) root         (0)     8772 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/deployment_updates.py
--rw-r--r--   0 root         (0) root         (0)    29806 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/deployments.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     5855 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/events.py
--rw-r--r--   0 root         (0) root         (0)    10265 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10954 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/execution_schedules.py
--rw-r--r--   0 root         (0) root         (0)    17979 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/executions.py
--rw-r--r--   0 root         (0) root         (0)     4817 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/filters.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/idp.py
--rw-r--r--   0 root         (0) root         (0)     8444 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/inter_deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/labels.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/ldap.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/license.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/maintenance.py
--rw-r--r--   0 root         (0) root         (0)    15074 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/manager.py
--rw-r--r--   0 root         (0) root         (0)    10973 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/node_instances.py
--rw-r--r--   0 root         (0) root         (0)    11333 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/nodes.py
--rw-r--r--   0 root         (0) root         (0)     6612 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/operations.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/permissions.py
--rw-r--r--   0 root         (0) root         (0)    13571 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/plugins.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/plugins_update.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/responses.py
--rw-r--r--   0 root         (0) root         (0)     7085 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/secrets.py
--rw-r--r--   0 root         (0) root         (0)     5029 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/sites.py
--rw-r--r--   0 root         (0) root         (0)     8460 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/summary.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tenants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.234518 cloudify-common-6.4.2/cloudify_rest_client/tests/
--rw-r--r--   0 root         (0) root         (0)     2158 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tests/test_authentication_headers.py
--rw-r--r--   0 root         (0) root         (0)      786 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tests/test_responses.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tests/test_tokens.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/tokens.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/users.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/utils.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/cloudify_rest_client/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.234518 cloudify-common-6.4.2/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)       71 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/ctx_wrappers/ctx-sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.234518 cloudify-common-6.4.2/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)      637 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/_compat.py
--rw-r--r--   0 root         (0) root         (0)     4502 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/constants.py
--rw-r--r--   0 root         (0) root         (0)    18028 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/dsl_parser/elements/
--rw-r--r--   0 root         (0) root         (0)      759 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5669 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/blueprint.py
--rw-r--r--   0 root         (0) root         (0)    10308 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/data_types.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/deployment_schedules.py
--rw-r--r--   0 root         (0) root         (0)    29821 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/imports.py
--rw-r--r--   0 root         (0) root         (0)     5664 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6139 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/misc.py
--rw-r--r--   0 root         (0) root         (0)    25867 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/node_templates.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/node_types.py
--rw-r--r--   0 root         (0) root         (0)    14699 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/operation.py
--rw-r--r--   0 root         (0) root         (0)     4377 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/plugins.py
--rw-r--r--   0 root         (0) root         (0)    19733 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/policies.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/relationships.py
--rw-r--r--   0 root         (0) root         (0)     6151 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/scalable.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/types.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/version.py
--rw-r--r--   0 root         (0) root         (0)     8465 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/elements/workflows.py
--rw-r--r--   0 root         (0) root         (0)     5408 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/dsl_parser/framework/
--rw-r--r--   0 root         (0) root         (0)      637 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/framework/elements.py
--rw-r--r--   0 root         (0) root         (0)    31478 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/framework/parser.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/framework/requirements.py
--rw-r--r--   0 root         (0) root         (0)    67291 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/functions.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/dsl_parser/import_resolver/
--rw-r--r--   0 root         (0) root         (0)      637 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/import_resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/import_resolver/abstract_import_resolver.py
--rw-r--r--   0 root         (0) root         (0)     7528 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/import_resolver/default_import_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/dsl_parser/interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/constants.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/interfaces_merger.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/interfaces_parser.py
--rw-r--r--   0 root         (0) root         (0)    10166 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/operation_merger.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/interfaces/utils.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/models.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/multi_instance.py
--rw-r--r--   0 root         (0) root         (0)     5772 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)    43440 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/rel_graph.py
--rw-r--r--   0 root         (0) root         (0)     9339 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/scan.py
--rw-r--r--   0 root         (0) root         (0)     7833 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/tasks.py
--rw-r--r--   0 root         (0) root         (0)    16567 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/utils.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/version.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/dsl_parser/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/script_runner/
--rw-r--r--   0 root         (0) root         (0)      637 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/script_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/script_runner/constants.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/script_runner/eval_env.py
--rw-r--r--   0 root         (0) root         (0)    14367 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/script_runner/tasks.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-06 10:36:09.242518 cloudify-common-6.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2974 2023-02-06 10:35:51.000000 cloudify-common-6.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/
+-rw-r--r--   0 root         (0) root         (0)    10273 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/
+-rw-r--r--   0 root         (0) root         (0)     2286 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)    23830 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/amqp_client.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cluster_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/compute/
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/conflict_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/constants.py
+-rw-r--r--   0 root         (0) root         (0)    47099 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/context.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cryptography_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/ctx_wrappers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/ctx_wrappers/ctx-py.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    18954 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/dispatch.py
+-rw-r--r--   0 root         (0) root         (0)    19018 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/error_handling.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/event.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/logs.py
+-rw-r--r--   0 root         (0) root         (0)    18303 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/manager.py
+-rw-r--r--   0 root         (0) root         (0)     7829 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/models_states.py
+-rw-r--r--   0 root         (0) root         (0)    20337 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugin_installer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/plugins/
+-rw-r--r--   0 root         (0) root         (0)      643 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/install_utils.py
+-rw-r--r--   0 root         (0) root         (0)    53945 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    56356 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/proxy/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/client.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/server.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/rabbitmq_client.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snapshots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/snmp/
+-rw-r--r--   0 root         (0) root         (0)     5393 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/CLOUDIFY-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/snmp_trap.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/state.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/systemddbus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/test_utils/
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/dispatch_helper.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/local_workflow_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/mock_rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    37803 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify/workflows/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/amqp_dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/events.py
+-rw-r--r--   0 root         (0) root         (0)    36444 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/local.py
+-rw-r--r--   0 root         (0) root         (0)    40724 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    26098 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/tasks_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)    80330 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/workflow_context.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/zip_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify_async_client/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4997 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.550778 cloudify-common-7.0.0/cloudify_rest_client/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/_datetime_compat.py
+-rw-r--r--   0 root         (0) root         (0)     7494 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/agents.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    23374 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/bytes_stream_utils.py
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/community_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployment_modifications.py
+-rw-r--r--   0 root         (0) root         (0)     8791 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployment_updates.py
+-rw-r--r--   0 root         (0) root         (0)    34027 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/events.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    11252 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/execution_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    18715 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/executions.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/filters.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/idp.py
+-rw-r--r--   0 root         (0) root         (0)     9024 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/inter_deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/labels.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/license.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/maintenance.py
+-rw-r--r--   0 root         (0) root         (0)    15074 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)    11333 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/nodes.py
+-rw-r--r--   0 root         (0) root         (0)     6699 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/operations.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    15934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     7141 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/plugins_update.py
+-rw-r--r--   0 root         (0) root         (0)    11395 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/responses.py
+-rw-r--r--   0 root         (0) root         (0)     8474 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/secrets_providers.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/sites.py
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/summary.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/users.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.550778 cloudify-common-7.0.0/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/ctx_wrappers/ctx-sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/constants.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/constraints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/elements/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5669 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/data_types.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/deployment_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    31837 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/imports.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/misc.py
+-rw-r--r--   0 root         (0) root         (0)    25808 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/node_templates.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/node_types.py
+-rw-r--r--   0 root         (0) root         (0)    16633 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/operation.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    19699 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/policies.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/relationships.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/scalable.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/version.py
+-rw-r--r--   0 root         (0) root         (0)     8400 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/workflows.py
+-rw-r--r--   0 root         (0) root         (0)     5578 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/framework/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/elements.py
+-rw-r--r--   0 root         (0) root         (0)    31720 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/requirements.py
+-rw-r--r--   0 root         (0) root         (0)    71265 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/import_resolver/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5209 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/abstract_import_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     7670 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/default_import_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/dsl_parser/interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_merger.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10119 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/operation_merger.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/models.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/multi_instance.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)    43420 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/rel_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/scan.py
+-rw-r--r--   0 root         (0) root         (0)    12187 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    18600 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/version.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/script_runner/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/constants.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/eval_env.py
+-rw-r--r--   0 root         (0) root         (0)    16145 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/tasks.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/setup.py
```

### Comparing `cloudify-common-6.4.2/LICENSE` & `cloudify-common-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/README.md` & `cloudify-common-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/__init__.py` & `cloudify-common-7.0.0/cloudify/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/agent_utils.py` & `cloudify-common-7.0.0/cloudify/agent_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,16 @@
     name = cloudify_agent['name']
     rabbitmq_client.delete_exchange(vhost, name)
 
 
 def _get_agent_system(cloudify_agent):
     if cloudify_agent.get('windows'):
         system = 'windows'
+    elif cloudify_agent.get('architecture'):
+        system = f"manylinux {cloudify_agent['architecture']}"
     else:
         system = cloudify_agent.get('distro')
         if cloudify_agent.get('distro_codename'):
             system = '{0} {1}'.format(system,
                                       cloudify_agent.get('distro_codename'))
     return system
```

### Comparing `cloudify-common-6.4.2/cloudify/amqp_client.py` & `cloudify-common-7.0.0/cloudify/amqp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,53 +14,43 @@
 #    * limitations under the License.
 
 from collections import deque
 import copy
 import json
 import logging
 import os
+import queue
 import random
 import ssl
-import sys
 import threading
 import time
 
 import pika
 import pika.exceptions
 
 from cloudify import broker_config, utils
 from cloudify.constants import INSPECT_TIMEOUT
-from cloudify._compat import queue
 
 # keep compat with both pika 0.11 and pika 1.1: switch the calls based
 # on this flag. We're keeping compat with 0.11 for the py2.6 agent on rhel6.
 # all pika calls that are different between 0.11 and 1.1, must be under
 # if statements on this flag.
 OLD_PIKA = not hasattr(pika, 'SSLOptions')
 
 logger = logging.getLogger(__name__)
 
-if sys.version_info >= (2, 7):
-    # requires 2.7+
-    def wait_for_event(evt, poll_interval=0.5):
-        """Wait for a threading.Event by polling, to allow handling of signals.
-        (ie. doesnt block ^C)
-        """
-        while True:
-            if evt.wait(poll_interval):
-                return
-else:
-    def wait_for_event(evt, poll_interval=None):
-        """Wait for a threading.Event. Stub for compatibility."""
-        # in python 2.6, Event.wait always returns None, so we can either:
-        #  - .wait() without a timeout and block ^C which is inconvenient
-        #  - .wait() with timeout and then check .is_set(),
-        #     which is not threadsafe
-        # We choose the inconvenient but safe method.
-        evt.wait()
+
+# requires 2.7+
+def wait_for_event(evt, poll_interval=0.5):
+    """Wait for a threading.Event by polling, to allow handling of signals.
+    (ie. does not block ^C)
+    """
+    while True:
+        if evt.wait(poll_interval):
+            return
 
 
 class AMQPParams(object):
     def __init__(self,
                  amqp_host=None,
                  amqp_user=None,
                  amqp_pass=None,
```

### Comparing `cloudify-common-6.4.2/cloudify/cluster.py` & `cloudify-common-7.0.0/cloudify/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/cluster_status.py` & `cloudify-common-7.0.0/cloudify/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/compute/__init__.py` & `cloudify-common-7.0.0/cloudify/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/conflict_handlers.py` & `cloudify-common-7.0.0/cloudify/conflict_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/constants.py` & `cloudify-common-7.0.0/cloudify/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
+REST_PROTOCOL_KEY = 'REST_PROTOCOL'
 REST_HOST_KEY = 'REST_HOST'
 REST_PORT_KEY = 'REST_PORT'
+ADMIN_API_TOKEN_KEY = 'ADMIN_API_TOKEN'
 AGENT_WORK_DIR_KEY = 'AGENT_WORK_DIR'
 MANAGER_FILE_SERVER_URL_KEY = 'MANAGER_FILE_SERVER_URL'
 MANAGER_FILE_SERVER_ROOT_KEY = 'MANAGER_FILE_SERVER_ROOT'
 MANAGER_FILE_SERVER_SCHEME = 'MANAGER_FILE_SERVER_SCHEME'
 MANAGER_NAME = 'MANAGER_NAME'
 FILE_SERVER_RESOURCES_FOLDER = 'resources'
 FILE_SERVER_BLUEPRINTS_FOLDER = 'blueprints'
@@ -57,14 +59,16 @@
 # upgraded - not none or provided)
 AGENT_INSTALL_METHODS_INSTALLED = [
     AGENT_INSTALL_METHOD_INIT_SCRIPT,
     AGENT_INSTALL_METHOD_PLUGIN,
     AGENT_INSTALL_METHOD_REMOTE,
 ]
 
+LOCAL_RESOURCES_ROOT_ENV_KEY = 'CFY_RESOURCES_ROOT'
+
 COMPUTE_NODE_TYPE = 'cloudify.nodes.Compute'
 
 BROKER_PORT_NO_SSL = 5672
 BROKER_PORT_SSL = 5671
 CELERY_TASK_RESULT_EXPIRES = 600
 LOCAL_REST_CERT_FILE_KEY = 'LOCAL_REST_CERT_FILE'
 SECURED_PROTOCOL = 'https'
```

### Comparing `cloudify-common-6.4.2/cloudify/context.py` & `cloudify-common-7.0.0/cloudify/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,105 @@
                 self._relationship_runtimes.update({
                     relationship.target.instance.id:
                     relationship.target.instance.runtime_properties
                 })
         return self._relationship_runtimes
 
 
-class CommonContext(object):
+class DeploymentWorkdirMixin:
+    def download_deployment_workdir(self):
+        """Download a copy of deployment-in-context's working directory from
+        the manager, but only if these files are not available locally.
+        """
+        if not deployment_workdirs_sync_required():
+            return
+
+        local_dir = self.local_deployment_workdir()
+        if not local_dir:
+            return
+
+        return self._endpoint.download_deployment_workdir(self.deployment.id,
+                                                          local_dir)
+
+    def upload_deployment_workdir(self):
+        """Upload a local copy of deployment-in-context's working directory to
+        the manager, but only if these files are not available locally.
+        """
+        if not deployment_workdirs_sync_required():
+            return
+
+        local_dir = self.local_deployment_workdir()
+        if not local_dir:
+            return
+
+        return self._endpoint.upload_deployment_workdir(self.deployment.id,
+                                                        local_dir)
+
+    def sync_deployment_workdir(self):
+        """Sync a local copy of deployment-in-context's working directory to
+        the manager, but only if these files are not available locally.  The
+        method returns a contextmanager, so it should be used like:
+
+        ```
+        with ctx.sync_deployment_workdir():
+            do_something()
+        ```
+        """
+        if not deployment_workdirs_sync_required():
+            return utils.nullcontext()
+
+        local_dir = self.local_deployment_workdir()
+        if not local_dir:
+            return utils.nullcontext()
+
+        return self._endpoint.sync_deployment_workdir(self.deployment.id,
+                                                      local_dir)
+
+    def local_deployment_workdir(self):
+        """Generate absolute path to deployment's local working directory.
+        The directory is a local copy of relevant directory on the manager.
+        """
+        if not self.deployment.id or not self.deployment.tenant_name:
+            return
+
+        local_resources_root = utils.get_local_resources_root()
+        if local_resources_root:
+            return os.path.join(
+                local_resources_root,
+                'deployments',
+                self.deployment.tenant_name,
+                self.deployment.id,
+            )
+
+        raise exceptions.NonRecoverableError(
+            'Local resources root directory not defined, is '
+            f'{constants.LOCAL_RESOURCES_ROOT_ENV_KEY} environment variable '
+            'set?')
+
+    def upload_deployment_file(
+        self,
+        target_file_path,
+        src_file,
+        src_file_mtime=None,
+    ):
+        return self._endpoint.upload_deployment_file(
+            deployment_id=self.deployment.id,
+            target_file_path=target_file_path,
+            src_file=src_file,
+            src_file_mtime=src_file_mtime,
+        )
+
+    def delete_deployment_file(self, file_path):
+        return self._endpoint.delete_deployment_file(
+            deployment_id=self.deployment.id,
+            file_path=file_path,
+        )
+
+
+class CommonContext(DeploymentWorkdirMixin):
 
     def __init__(self, ctx=None):
         self._context = ctx or {}
         self._local = ctx.get('local', False)
         if self._local:
             # there are times when this instance is instantiated merely for
             # accessing the attributes so we can tolerate no storage (such is
@@ -276,14 +366,19 @@
 
     @property
     def id(self):
         """The deployment id the plugin invocation belongs to."""
         return self._context.get('deployment_id')
 
     @property
+    def tenant_name(self):
+        """The deployment tenant's name."""
+        return self._context.get('tenant', {}).get('name')
+
+    @property
     def runtime_only_evaluation(self):
         return self._context.get('runtime_only_evaluation')
 
     @property
     def display_name(self):
         """The deployment's display_name used e.g. in Cloudify UI."""
         return self._context.get('deployment_display_name')
@@ -784,14 +879,19 @@
 
     @property
     def rest_host(self):
         """REST host"""
         return self._rest_host
 
     @property
+    def rest_port(self):
+        """REST port"""
+        return self._context.get('rest_port')
+
+    @property
     def rest_token(self):
         """REST service token"""
         return self._context.get('rest_token')
 
     @property
     def rest_ssl_cert(self):
         """REST SSL Certificate Content"""
@@ -1206,14 +1306,19 @@
 
     @property
     def source(self):
         """The source package of the plugin."""
         return self._plugin_context.get('source')
 
     @property
+    def properties(self):
+        """The properties of the plugin."""
+        return self._plugin_context.get('properties')
+
+    @property
     def prefix(self):
         """The plugin prefix."""
         return utils.plugin_prefix(
             name=self.package_name or self.name,
             version=self.package_version,
             deployment_id=self._deployment_id,
             tenant_name=self._tenant_name)
@@ -1267,7 +1372,20 @@
         self._raise()
 
     def pop(self, k, d=None):
         self._raise()
 
     def popitem(self):
         self._raise()
+
+
+def deployment_workdirs_sync_required():
+    """Returns `True` if mgmtworker and manager are running on different
+    hosts.  The test is just a comparison of environment variables:
+    `CFY_RESOURCES_ROOT` and `MANAGER_FILE_SERVER_ROOT`.
+    """
+    local_resources_root =\
+        os.environ.get(constants.LOCAL_RESOURCES_ROOT_ENV_KEY)
+    file_manager_root =\
+        os.environ.get(constants.MANAGER_FILE_SERVER_ROOT_KEY)
+    return (local_resources_root
+            and (local_resources_root != file_manager_root))
```

### Comparing `cloudify-common-6.4.2/cloudify/cryptography_utils.py` & `cloudify-common-7.0.0/cloudify/cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/ctx_wrappers/ctx-py.py` & `cloudify-common-7.0.0/cloudify/ctx_wrappers/ctx-py.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 #!/usr/bin/env python
 
 import sys
 import json
 import shlex
 import subprocess
-from collections import MutableMapping, Mapping
-
-PY2 = sys.version_info[0] == 2
-
-if PY2:
-    text_type = unicode  # NOQA
-else:
-    text_type = str
+from collections.abc import MutableMapping, Mapping
 
 
 def check_output(*popenargs, **kwargs):
     """Run command with arguments and return its output as a byte string.
 
     Backported from Python 2.7 as it's implemented as pure python on stdlib.
     >>> check_output(['/usr/bin/python', '--version'])
@@ -39,15 +32,15 @@
         error.stderr = stderr
         error.output = output
         raise error
     return output
 
 
 def unicode_to_string(text):
-    if isinstance(text, text_type):
+    if isinstance(text, str):
         return text
     elif isinstance(text, bytes):
         return text.decode('utf-8', 'ignore')
     if isinstance(text, list):
         return [unicode_to_string(a) for a in text]
     if isinstance(text, dict):
         return dict((unicode_to_string(key), unicode_to_string(
```

### Comparing `cloudify-common-6.4.2/cloudify/decorators.py` & `cloudify-common-7.0.0/cloudify/decorators.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/dispatch.py` & `cloudify-common-7.0.0/cloudify/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,30 @@
 This module will normally run from a plugin-specific virtualenv.
 """
 
 import copy
 import json
 import logging
 import os
+import queue
 import sys
+import textwrap
 import threading
 import traceback
+from io import StringIO
 
 from cloudify_rest_client.executions import Execution
 from cloudify_rest_client.exceptions import InvalidExecutionUpdateStatus
 
 from cloudify import logs
 from cloudify import exceptions
 from cloudify import state
 from cloudify import context
 from cloudify import utils
 from cloudify import constants
-from cloudify._compat import queue, StringIO
 from cloudify.manager import update_execution_status, get_rest_client
 from cloudify.constants import LOGGING_CONFIG_FILE
 from cloudify.error_handling import serialize_known_exception
 
 from cloudify.workflows import api
 
 
@@ -141,15 +143,15 @@
                 raise ctx.operation._operation_retry
         return result
 
     def _run_operation_func(self, ctx, kwargs):
         try:
             return self.func(*self.args, **kwargs)
         except Exception as e:
-            err = _WrappedTaskError(e, traceback.format_exc())
+            err = _WrappedTaskError(e, sys.exc_info()[2])
             raise err
         finally:
             if ctx.type == constants.NODE_INSTANCE:
                 ctx.instance.update()
             elif ctx.type == constants.RELATIONSHIP_INSTANCE:
                 ctx.source.instance.update()
                 ctx.target.instance.update()
@@ -161,33 +163,48 @@
     We'll wrap the exception and the traceback, so that we can
     preserve the original traceback. We want the original traceback
     to be around, so that we can only print that, without adding
     framework-level frames that come from dispatch.py itself.
     """
     def __init__(self, wrapped_exc, wrapped_tb, *args, **kwargs):
         super(_WrappedTaskError, self).__init__(*args, **kwargs)
+
+        # figure out how many lines to show: negative limit means only the
+        # last N lines will be shown. We show all but one, i.e. we skip
+        # the top-most line.
+        stack = traceback.extract_tb(wrapped_tb)
+        limit = -len(stack) + 1
+
+        traceback_lines = traceback.format_tb(wrapped_tb, limit=limit)
+        exception_lines = traceback.format_exception_only(
+            # compat with pythons pre-3.10; the first argument is ignored
+            # in 3.10+
+            type(wrapped_exc),
+            value=wrapped_exc,
+        )
+
         self.wrapped_exc = wrapped_exc
-        self.wrapped_tb = wrapped_tb
+        self.wrapped_tb = (
+            textwrap.dedent(''.join(traceback_lines))
+            + ''.join(exception_lines)
+        )
 
 
 class WorkflowHandler(TaskHandler):
     def __init__(self, *args, **kwargs):
         if api is None:
             raise RuntimeError('Dispatcher not installed')
         super(WorkflowHandler, self).__init__(*args, **kwargs)
 
     @property
     def ctx_cls(self):
         # import workflow_context in-function so that it doesn't need to
         # be imported when handling an operation
         # (only when handling a workflow)
         from cloudify.workflows import workflow_context
-
-        if getattr(self.func, 'workflow_system_wide', False):
-            return workflow_context.CloudifySystemWideWorkflowContext
         return workflow_context.CloudifyWorkflowContext
 
     def handle(self):
         self.kwargs['ctx'] = self.ctx
         with state.current_workflow_ctx.push(self.ctx, self.kwargs):
             self._validate_workflow_func()
             if self.ctx.local or self.ctx.dry_run:
@@ -338,15 +355,15 @@
                 if not self.ctx.internal.graph_mode:
                     for workflow_task in self.ctx.internal.task_graph.tasks:
                         workflow_task.async_result.get()
             except api.ExecutionCancelled:
                 result = {'result': api.EXECUTION_CANCELLED_RESULT}
                 return result
             except BaseException as workflow_ex:
-                err = _WrappedTaskError(workflow_ex, traceback.format_exc())
+                err = _WrappedTaskError(workflow_ex, sys.exc_info()[2])
                 result = {'error': err}
                 return result
             return result
 
     def _workflow_started(self):
         self._update_execution_status(Execution.STARTED)
         dry_run = ' (dry run)' if self.ctx.dry_run else ''
@@ -445,15 +462,15 @@
     dispatch_dir = sys.argv[1]
     with open(os.path.join(dispatch_dir, 'input.json')) as f:
         dispatch_inputs = json.load(f)
     cloudify_context = dispatch_inputs['cloudify_context']
     args = dispatch_inputs['args']
     kwargs = dispatch_inputs['kwargs']
     dispatch_type = cloudify_context['type']
-    threading.current_thread().setName('Dispatch-{0}'.format(dispatch_type))
+    threading.current_thread().name = f'Dispatch-{dispatch_type}'
     handler_cls = TASK_HANDLERS[dispatch_type]
     handler = handler_cls(
         cloudify_context=cloudify_context, args=args, kwargs=kwargs)
     try:
         _setup_logging()
         payload = handler.handle()
         payload_type = 'result'
```

### Comparing `cloudify-common-6.4.2/cloudify/endpoint.py` & `cloudify-common-7.0.0/cloudify/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,24 +163,41 @@
 
     def get_workdir(self):
         raise NotImplementedError('Implemented by subclasses')
 
     def get_execution(self, execution_id):
         raise NotImplementedError('Implemented by subclasses')
 
+    def download_deployment_workdir(self, deployment_id, local_dir):
+        raise NotImplementedError('Implemented by subclasses')
+
+    def upload_deployment_workdir(self, deployment_id, local_dir):
+        raise NotImplementedError('Implemented by subclasses')
+
+    def sync_deployment_workdir(self, deployment_id, local_dir):
+        raise NotImplementedError('Implemented by subclasses')
+
+    def upload_deployment_file(
+        self, target_file_path, src_file, src_file_mtime=None
+    ):
+        raise NotImplementedError('Implemented by subclasses')
+
+    def delete_deployment_file(self, file_path):
+        raise NotImplementedError('Implemented by subclasses')
+
 
 class ManagerEndpoint(Endpoint):
     def __init__(self, *args, **kwargs):
         super(ManagerEndpoint, self).__init__(*args, **kwargs)
         self._rest_client = None
 
     @property
     def rest_client(self):
         if self._rest_client is None:
-            self._rest_client = manager.get_rest_client()
+            self._rest_client = manager.get_rest_client(self.ctx.tenant_name)
         return self._rest_client
 
     def get_node(self, node_id):
         return self.rest_client.nodes.get(
             self.ctx.deployment.id, node_id, evaluate_functions=True)
 
     def get_node_instance(self, node_instance_id):
@@ -317,14 +334,42 @@
         self.rest_client.operations.update(
             operation_id,
             state=state,
             agent_name=utils.get_daemon_name(),
             manager_name=utils.get_manager_name(),
         )
 
+    def download_deployment_workdir(self, deployment_id, local_dir):
+        return self.rest_client.resources.download_deployment_workdir(
+            deployment_id, local_dir)
+
+    def upload_deployment_workdir(self, deployment_id, local_dir):
+        return self.rest_client.resources.upload_deployment_workdir(
+            deployment_id, local_dir)
+
+    def sync_deployment_workdir(self, deployment_id, local_dir):
+        return self.rest_client.resources.sync_deployment_workdir(
+            deployment_id, local_dir)
+
+    def upload_deployment_file(
+        self, deployment_id, target_file_path, src_file, src_file_mtime=None,
+    ):
+        return self.rest_client.resources.upload_deployment_file(
+            deployment_id=deployment_id,
+            target_file_path=target_file_path,
+            src_file=src_file,
+            src_file_mtime=src_file_mtime,
+        )
+
+    def delete_deployment_file(self, deployment_id, file_path):
+        return self.rest_client.resources.delete_deployment_file(
+            deployment_id=deployment_id,
+            file_path=file_path,
+        )
+
 
 class LocalEndpoint(Endpoint):
 
     def __init__(self, ctx, storage):
         super(LocalEndpoint, self).__init__(ctx)
         self.storage = storage
 
@@ -438,7 +483,24 @@
 
     def get_operation(self, operation_id):
         return None
 
     def get_execution(self, execution_id):
         # same issue as get_brokers
         return Execution({'id': execution_id, 'status': 'started'})
+
+    def download_deployment_workdir(self, deployment_id, local_dir):
+        pass
+
+    def upload_deployment_workdir(self, deployment_id, local_dir):
+        pass
+
+    def sync_deployment_workdir(self, deployment_id, local_dir):
+        return utils.nullcontext()
+
+    def upload_deployment_file(
+        self, target_file_path, src_file, src_file_mtime=None
+    ):
+        pass
+
+    def delete_deployment_file(self, file_path):
+        pass
```

### Comparing `cloudify-common-6.4.2/cloudify/error_handling.py` & `cloudify-common-7.0.0/cloudify/error_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import traceback
+from io import StringIO
 
-from cloudify._compat import StringIO
 from cloudify.utils import format_exception
 from cloudify import exceptions
 
 
 def serialize_known_exception(e, formatted_traceback=None):
     """
     Serialize a cloudify exception into a dict
```

### Comparing `cloudify-common-6.4.2/cloudify/event.py` & `cloudify-common-7.0.0/cloudify/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-from cloudify._compat import StringIO
+from io import StringIO
 
 HIGH_VERBOSE = 3
 MEDIUM_VERBOSE = 2
 LOW_VERBOSE = 1
 NO_VERBOSE = 0
```

### Comparing `cloudify-common-6.4.2/cloudify/exceptions.py` & `cloudify-common-7.0.0/cloudify/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/logs.py` & `cloudify-common-7.0.0/cloudify/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     ENV_AGENT_LOG_LEVEL,
     ENV_AGENT_LOG_DIR,
     ENV_AGENT_LOG_MAX_BYTES,
     ENV_AGENT_LOG_MAX_HISTORY,
     get_manager_name,
     get_daemon_name,
 )
-from cloudify._compat import text_type
 
 EVENT_CLASS = _event.Event
 EVENT_VERBOSITY_LEVEL = _event.NO_VERBOSE
 
 
 def message_context_from_cloudify_context(ctx):
     """Build a message context from a CloudifyContext instance"""
@@ -73,25 +72,14 @@
         'deployment_id': ctx.deployment.id,
         'execution_id': ctx.execution_id,
         'workflow_id': ctx.workflow_id,
         'tenant': {'name': ctx.tenant_name},
     }
 
 
-def message_context_from_sys_wide_wf_context(ctx):
-    """Build a message context from a CloudifyWorkflowContext instance"""
-    return {
-        'blueprint_id': None,
-        'deployment_id': None,
-        'execution_id': ctx.execution_id,
-        'workflow_id': ctx.workflow_id,
-        'tenant': {'name': ctx.tenant_name},
-    }
-
-
 def message_context_from_workflow_node_instance_context(ctx):
     """Build a message context from a CloudifyWorkflowNode instance"""
     message_context = message_context_from_workflow_context(ctx.ctx)
     message_context.update({
         'node_name': ctx.node_id,
         'node_id': ctx.id,
     })
@@ -132,21 +120,14 @@
 class CloudifyWorkflowLoggingHandler(CloudifyBaseLoggingHandler):
     """A Handler class for writing workflow log messages to RabbitMQ"""
     def __init__(self, ctx, out_func=None):
         CloudifyBaseLoggingHandler.__init__(
             self, ctx, out_func, message_context_from_workflow_context)
 
 
-class SystemWideWorkflowLoggingHandler(CloudifyBaseLoggingHandler):
-    """Class for writing system-wide workflow log messages to RabbitMQ"""
-    def __init__(self, ctx, out_func=None):
-        CloudifyBaseLoggingHandler.__init__(
-            self, ctx, out_func, message_context_from_sys_wide_wf_context)
-
-
 class CloudifyWorkflowNodeLoggingHandler(CloudifyBaseLoggingHandler):
     """A Handler class for writing workflow nodes log messages to RabbitMQ"""
     def __init__(self, ctx, out_func=None):
         CloudifyBaseLoggingHandler.__init__(
             self, ctx, out_func,
             message_context_from_workflow_node_instance_context)
 
@@ -206,29 +187,14 @@
     :param additional_context: additional context to be added to the context
     """
     _send_event(
         message_context_from_workflow_context(ctx),
         event_type, message, args, additional_context, out_func)
 
 
-def send_sys_wide_wf_event(ctx, event_type, message=None, args=None,
-                           additional_context=None, out_func=None):
-    """Send a workflow event
-
-    :param ctx: A CloudifySystemWideWorkflowContext instance
-    :param event_type: The event type
-    :param message: The message
-    :param args: additional arguments that may be added to the message
-    :param additional_context: additional context to be added to the context
-    """
-    _send_event(
-        message_context_from_sys_wide_wf_context(ctx),
-        event_type, message, args, additional_context, out_func)
-
-
 def send_workflow_node_event(ctx, event_type,
                              message=None,
                              args=None,
                              additional_context=None,
                              out_func=None,
                              skip_send=False):
     """Send a workflow node event
@@ -345,15 +311,15 @@
     event_obj = EVENT_CLASS(
         event,
         verbosity_level=EVENT_VERBOSITY_LEVEL,
         with_worker_names=with_worker_names,
     )
     if not event_obj.has_output:
         return None
-    return text_type(event_obj)
+    return str(event_obj)
 
 
 def _log_message(logger, message):
     level = message.get('level', 'info')
     log_func = getattr(logger, level, logger.info)
     exec_id = message.get('context', {}).get('execution_id')
     execution_creator_username = message.get('context', {}).get(
```

### Comparing `cloudify-common-6.4.2/cloudify/manager.py` & `cloudify-common-7.0.0/cloudify/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     return CloudifyClusterClient(
         headers=headers,
         host=utils.get_manager_rest_service_host(),
         port=utils.get_manager_rest_service_port(),
         tenant=tenant,
         token=token,
-        protocol=constants.SECURED_PROTOCOL,
+        protocol=utils.get_manager_rest_service_protocol(),
         cert=utils.get_local_rest_certificate(),
         kerberos_env=utils.get_kerberos_indication(
             os.environ.get(constants.KERBEROS_ENV_KEY))
     )
 
 
 def _save_resource(logger, resource, resource_path, target_path):
@@ -313,25 +313,26 @@
         yield os.path.join(
             constants.FILE_SERVER_DEPLOYMENTS_FOLDER,
             tenant_name,
             deployment_id,
             resource_path
         ).replace('\\', '/')
 
-    client = get_rest_client()
-    blueprint = client.blueprints.get(blueprint_id)
-    if blueprint['visibility'] == VisibilityState.GLOBAL:
-        tenant_name = blueprint['tenant_name']
-
-    yield os.path.join(
-        constants.FILE_SERVER_BLUEPRINTS_FOLDER,
-        tenant_name,
-        blueprint_id,
-        resource_path
-    ).replace('\\', '/')
+    if blueprint_id:
+        client = get_rest_client()
+        blueprint = client.blueprints.get(blueprint_id)
+        if blueprint['visibility'] == VisibilityState.GLOBAL:
+            tenant_name = blueprint['tenant_name']
+
+        yield os.path.join(
+            constants.FILE_SERVER_BLUEPRINTS_FOLDER,
+            tenant_name,
+            blueprint_id,
+            resource_path
+        ).replace('\\', '/')
 
     if use_global:
         yield resource_path
 
 
 def get_resource(blueprint_id, deployment_id, tenant_name, resource_path):
     """
@@ -372,15 +373,16 @@
     tried_paths = []
     resource_files = set()
     for path in _resource_paths(
             blueprint_id, deployment_id, tenant_name, resource_path,
             use_global=False):
         try:
             directory_index = get_resource_from_manager(path)
-            for f in json.loads(directory_index)['files']:
+            directory_index_dict = json.loads(directory_index)
+            for f in directory_index_dict.keys():
                 resource_files.add(f)
         except (ValueError, KeyError, NonRecoverableError):
             tried_paths.append(path)
         except HttpException as e:
             if e.code != 404:
                 raise
```

### Comparing `cloudify-common-6.4.2/cloudify/mocks.py` & `cloudify-common-7.0.0/cloudify/mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,7 +238,18 @@
         return self._config or []
 
     def get_managers(self, network=None):
         return [ManagerItem(m) for m in self._managers]
 
     def get_brokers(self, network=None):
         return [RabbitMQBrokerItem(b) for b in self._brokers]
+
+    def upload_deployment_file(
+        self,
+        target_file_path,
+        src_file,
+        src_file_mtime=None,
+    ):
+        pass
+
+    def delete_deployment_file(self, file_path):
+        pass
```

### Comparing `cloudify-common-6.4.2/cloudify/models_states.py` & `cloudify-common-7.0.0/cloudify/models_states.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/plugin_installer.py` & `cloudify-common-7.0.0/cloudify/plugin_installer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,39 @@
 import tempfile
 import platform
 import threading
 
 from os import walk
 from functools import wraps
 from contextlib import contextmanager
+from urllib.parse import urljoin
+from urllib.request import pathname2url
 
 import wagon
 import fasteners
 
 from cloudify import ctx
 from cloudify.manager import get_rest_client
 from cloudify.utils import (
     LocalCommandRunner, target_plugin_prefix, extract_archive,
-    get_python_path, get_manager_name, get_daemon_name
+    get_python_path, get_manager_name, get_daemon_name,
 )
-from cloudify._compat import reraise, urljoin, pathname2url, parse_version
 from cloudify.exceptions import (
     NonRecoverableError,
     CommandExecutionException,
     PluginInstallationError
 )
 from cloudify.models_states import PluginInstallationState
 from cloudify_rest_client.exceptions import CloudifyClientError
 
+try:
+    from packaging.version import parse as parse_version
+except ImportError:
+    from distutils.version import LooseVersion as parse_version
+
 PLUGIN_INSTALL_LOCK = threading.Lock()
 runner = LocalCommandRunner()
 
 
 def _manage_plugin_state(pre_state, post_state, allow_missing=False):
     """Update plugin state when doing a plugin operation.
 
@@ -121,36 +127,30 @@
     if source:
         _install_source_plugin(
             deployment_id=deployment_id,
             plugin=plugin,
             source=source,
             args=args)
     else:
-        platform, distro, release = _platform_and_distro()
         name = plugin.get('package_name') or plugin.get('name')
         raise NonRecoverableError(
-            'No source or managed plugin found for {0} '
-            '[current platform={1}, distro={2}, release={3}]'
-            .format(name, platform, distro, release))
+           f'No source or managed plugin found for {name} '
+           f'[current platform={platform.system()}, '
+           f'arch={platform.machine()}]')
 
 
-def _make_virtualenv(path):
+def _make_virtualenv(python_executable, path):
     """Make a venv and link the current venv to it.
 
     The new venv will have the current venv linked, ie. it will be
     able to import libraries from the current venv, but libraries
     installed directly will have precedence.
     """
-    runner.run([
-        sys.executable, '-m', 'virtualenv',
-        '--no-download',
-        '--no-pip', '--no-wheel', '--no-setuptools',
-        path
-    ])
-    _link_virtualenv(path)
+    runner.run([python_executable, '-m', 'venv', '--without-pip', path])
+    _link_virtualenv(python_executable, path)
 
 
 def is_already_installed(dst_dir, plugin_id):
     ctx.logger.debug('Checking if managed plugin installation exists '
                      'in %s', dst_dir)
     if os.path.exists(dst_dir):
         ctx.logger.debug('Plugin path exists: %s', dst_dir)
@@ -198,26 +198,26 @@
                 'Using existing installation of managed plugin: %s [%s]',
                 plugin.id, _get_plugin_description(plugin))
             return
 
         ctx.logger.info(
             'Installing managed plugin: %s [%s]',
             plugin.id, _get_plugin_description(plugin))
-        _make_virtualenv(dst_dir)
+        _make_virtualenv(_python_executable(plugin), dst_dir)
         try:
             _wagon_install(plugin, venv=dst_dir, args=args)
             with open(os.path.join(dst_dir, 'plugin.id'), 'w') as f:
                 f.write(plugin.id)
         except Exception as e:
             shutil.rmtree(dst_dir, ignore_errors=True)
             tpe, value, tb = sys.exc_info()
             exc = NonRecoverableError(
                 'Failed installing managed plugin: {0} [{1}][{2}]'
                 .format(plugin.id, plugin.package_name, e))
-            reraise(NonRecoverableError, exc, tb)
+            raise exc.with_traceback(tb)
 
 
 def _wagon_install(plugin, venv, args):
     client = get_rest_client()
     wagon_dir = tempfile.mkdtemp(prefix='{0}-'.format(plugin.id))
     wagon_path = os.path.join(wagon_dir, 'wagon.tar.gz')
     try:
@@ -248,15 +248,15 @@
     with _lock(dst_dir):
         if is_already_installed(dst_dir, 'source-{0}'.format(deployment_id)):
             ctx.logger.info(
                 'Using existing installation of source plugin: %s', name)
             return
 
         ctx.logger.info('Installing plugin from source: %s', name)
-        _make_virtualenv(dst_dir)
+        _make_virtualenv(_python_executable(plugin), dst_dir)
         try:
             _pip_install(source=source, venv=dst_dir, args=args)
         except Exception:
             shutil.rmtree(dst_dir, ignore_errors=True)
             raise
         with open(os.path.join(dst_dir, 'plugin.id'), 'w') as f:
             f.write('source-{0}'.format(deployment_id))
@@ -431,36 +431,27 @@
     This compares a plugin's .supported_platform field with the
     platform we're running on.
     """
     if not plugin.supported_platform:
         return False
     if plugin.supported_platform == 'any':
         return True
-    current_platform, current_dist, current_release = _platform_and_distro()
 
     if os.name == 'posix':
         # for linux,
         # 1) allow manylinux always,
-        # 2) disallow if the distro is specified and different than current
+        # 2) disallow if the arch is specified and different than current
         if plugin.supported_platform.startswith('manylinux'):
             return True
-        if plugin.distribution and plugin.distribution != current_dist:
-            return False
-        if plugin.distribution_release \
-                and plugin.distribution_release != current_release:
-            return False
-    # non-linux, or linux but the distribution fits
-    return plugin.supported_platform == current_platform
-
-
-def _platform_and_distro():
-    current_platform = wagon.get_platform()
-    distribution, _, distribution_release = platform.linux_distribution(
-        full_distribution_name=False)
-    return current_platform, distribution.lower(), distribution_release.lower()
+        if plugin.supported_platform.startswith('linux_'):
+            if plugin.supported_platform.split('_', 1)[1] != \
+                    platform.machine():
+                return False
+    # non-linux, or linux but the platform fits
+    return plugin.supported_platform == wagon.get_platform()
 
 
 def get_plugin_source(plugin, blueprint_id=None):
 
     source = plugin.get('source') or ''
     if not source:
         return None
@@ -500,50 +491,71 @@
     As taken from: https://github.com/pypa/pip/blob/9.0.1/pip/download.py#L459
     """
     path = os.path.normpath(os.path.abspath(path))
     url = urljoin('file:', pathname2url(path))
     return url
 
 
-def _link_virtualenv(venv):
+def _link_virtualenv(executable, venv):
     """Add current venv's libs to the target venv.
 
     Add a .pth file with a link to the current venv, to the target
     venv's site-packages.
     Also copy .pth files' contents from the current venv, so that the
     target venv also uses editable packages from the source venv.
     """
-    own_site_packages = get_pth_dir()
-    target = get_pth_dir(venv)
+    own_site_packages = get_pth_dir(executable)
+    target = get_pth_dir(get_python_path(venv))
     with open(os.path.join(target, 'agent.pth'), 'w') as agent_link:
         agent_link.write('# link to the agent virtualenv, created by '
                          'the plugin installer\n')
         agent_link.write('{0}\n'.format(own_site_packages))
 
         for filename in glob.glob(os.path.join(own_site_packages, '*.pth')):
             pth_path = os.path.join(own_site_packages, filename)
             with open(pth_path) as pth:
                 agent_link.write('\n# copied from {0}:\n'.format(pth_path))
                 agent_link.write(pth.read())
                 agent_link.write('\n')
 
 
-def get_pth_dir(venv=None):
+def get_pth_dir(executable):
     """Get the directory suitable for .pth files in this venv.
 
     This will return the site-packages directory, which is one of the
     targets that is scanned for .pth files.
     This is mostly a reimplementation of sysconfig.get_path('purelib'),
     but sysconfig is not available in 2.6.
     """
     output = runner.run([
-        get_python_path(venv) if venv else sys.executable,
+        executable,
         '-c',
-        'import json, sys; print(json.dumps([sys.prefix, sys.version[:3]]))'
+        'import json, sys; print(json.dumps([sys.prefix, sys.version_info]))'
     ]).std_out
-    prefix, version = json.loads(output)
+    prefix, version_parts = json.loads(output)
+    version = '{0}.{1}'.format(version_parts[0], version_parts[1])
     if os.name == 'nt':
         return '{0}/Lib/site-packages'.format(prefix)
     elif os.name == 'posix':
         return '{0}/lib/python{1}/site-packages'.format(prefix, version)
     else:
         raise NonRecoverableError('Unsupported OS: {0}'.format(os.name))
+
+
+def _python_executable(plugin):
+    if 'supported_py_versions' not in plugin:
+        # This is the case for source plugins
+        return sys.executable
+
+    v = sys.version_info
+    if f'py{v.major}{v.minor}' in plugin['supported_py_versions']:
+        return sys.executable
+    for v in reversed(plugin['supported_py_versions']):
+        # This won't work with Python>=10, e.g. `py101`
+        file_name = f'python{v[2:3]}.{v[3:]}'
+        for path in os.environ['PATH'].split(os.pathsep):
+            file_path = os.path.join(path, file_name)
+            if os.path.isfile(file_path) and os.access(file_path, os.X_OK):
+                return file_path
+    raise NonRecoverableError(
+        "This version of Cloudify does not support plugins build for Python "
+        f"versions: {plugin['supported_py_versions']}.")
```

### Comparing `cloudify-common-6.4.2/cloudify/plugins/__init__.py` & `cloudify-common-7.0.0/cloudify/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/plugins/install_utils.py` & `cloudify-common-7.0.0/cloudify/plugins/install_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/plugins/lifecycle.py` & `cloudify-common-7.0.0/cloudify/plugins/lifecycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,14 @@
             subgraphs[instance.id] = subgraph
 
         for instance in self.intact_nodes:
             subgraphs[instance.id] = self.graph.subgraph(
                 'stub_{0}'.format(instance.id))
 
         graph_finisher_func(self.graph, subgraphs)
-        self.graph.optimize()
         return self.graph
 
     def _finish_install(self, graph, subgraphs):
         self._finish_subgraphs(
             graph=graph,
             subgraphs=subgraphs,
             intact_op='cloudify.interfaces.relationship_lifecycle.establish',
```

### Comparing `cloudify-common-6.4.2/cloudify/plugins/workflows.py` & `cloudify-common-7.0.0/cloudify/plugins/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,21 +121,25 @@
         to be healthy (their check_status operation is defined and has run),
         are considered passing
     """
     healthy_instances = set()
     for instance in instances:
         try:
             status = instance.system_properties['status']
-            if not status['ok']:
-                continue
-            if require_task and not status['task']:
-                continue
-            healthy_instances.add(instance)
+            task = status['task']
+            ok = status['ok']
         except KeyError:
-            pass
+            task = None
+            ok = None
+
+        if (
+            ok or
+            task is None and not require_task
+        ):
+            healthy_instances.add(instance)
     return healthy_instances
 
 
 def _reinstall_disallowed_exception(to_reinstall):
     if len(to_reinstall) > 5:
         instance_ids = [inst.id for inst in to_reinstall]
         names_message = (
@@ -918,25 +922,30 @@
         'operation': operation
     }
     if allow_kwargs_override is not None:
         exec_op_params['allow_kwargs_override'] = allow_kwargs_override
 
     # registering actual tasks to sequences
     for instance in filtered_node_instances:
+        subgraph = graph.subgraph(instance.id)
+        subgraphs[instance.id] = subgraph
+
+        if not instance.node.has_operation(operation):
+            continue
+
         start_event_message = 'Starting operation {0}'.format(operation)
         if operation_kwargs:
             start_event_message += ' (Operation parameters: {0})'.format(
                 operation_kwargs)
-        subgraph = graph.subgraph(instance.id)
+
         sequence = subgraph.sequence()
         sequence.add(
             instance.send_event(start_event_message),
             instance.execute_operation(**exec_op_params),
             instance.send_event('Finished operation {0}'.format(operation)))
-        subgraphs[instance.id] = subgraph
 
     # adding tasks dependencies if required
     if run_by_dependency_order:
         for instance in ctx.node_instances:
             for rel in instance.relationships:
                 graph.add_dependency(subgraphs[instance.id],
                                      subgraphs[rel.target_id])
@@ -1043,16 +1052,17 @@
 
     # registering actual tasks to sequences
     for instance in filtered_node_instances:
         task = instance.execute_operation(
             operation='cloudify.interfaces.validation.check_status'
         )
         task.info = {'instance_id': instance.id}
-        task.on_success = check_status_on_success
-        task.on_failure = on_fail
+        if not task.is_nop():
+            task.on_success = check_status_on_success
+            task.on_failure = on_fail
         graph.add_task(task)
         tasks[instance.id] = task
 
     # adding tasks dependencies if required
     if run_by_dependency_order:
         for instance in ctx.node_instances:
             for rel in instance.relationships:
@@ -1080,15 +1090,15 @@
         **kwargs)
     graph.execute()
 
 
 @make_or_get_graph
 def _make_check_drift_graph(
     ctx,
-    run_by_dependency_order=False,
+    run_by_dependency_order=True,
     type_names=None,
     node_ids=None,
     node_instance_ids=None,
     ignore_failure=False,
 ):
     """Make the graph for the check_status workflow
 
@@ -1115,34 +1125,37 @@
 
     # registering actual tasks to sequences
     for instance in filtered_node_instances:
         task = instance.execute_operation(
             operation='cloudify.interfaces.lifecycle.check_drift'
         )
         task.info = {'instance_id': instance.id}
-        task.on_success = check_drift_on_success
-        task.on_failure = on_fail
+        if not task.is_nop():
+            task.on_success = check_drift_on_success
+            task.on_failure = on_fail
         graph.add_task(task)
         tasks[instance.id] = task
         for rel in instance.relationships:
             source_task = rel.execute_source_operation(
                 'cloudify.interfaces.relationship_lifecycle.check_drift')
             target_task = rel.execute_target_operation(
                 'cloudify.interfaces.relationship_lifecycle.check_drift')
-            source_task.on_success = check_drift_on_success
-            source_task.on_failure = on_fail
+            if not source_task.is_nop():
+                source_task.on_success = check_drift_on_success
+                source_task.on_failure = on_fail
             graph.add_task(source_task)
             graph.add_dependency(source_task, task)
             source_task.info = {
                 'instance_id': instance.id,
                 'relationship_target': rel.target_id,
             }
 
-            target_task.on_success = check_drift_on_success
-            target_task.on_failure = on_fail
+            if not target_task.is_nop():
+                target_task.on_success = check_drift_on_success
+                target_task.on_failure = on_fail
             graph.add_task(target_task)
             graph.add_dependency(target_task, task)
             target_task.info = {
                 'instance_id': rel.target_id,
                 'relationship_source': instance.id,
             }
```

### Comparing `cloudify-common-6.4.2/cloudify/proxy/__init__.py` & `cloudify-common-7.0.0/cloudify/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/proxy/client.py` & `cloudify-common-7.0.0/cloudify/proxy/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/proxy/server.py` & `cloudify-common-7.0.0/cloudify/proxy/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  * See the License for the specific language governing permissions and
 #  * limitations under the License.
 
 import traceback
 import re
-import collections
 import json
+import queue
 import threading
 import socket
+from collections.abc import MutableMapping
+from io import StringIO
 from wsgiref.simple_server import WSGIServer, WSGIRequestHandler
 from wsgiref.simple_server import make_server as make_wsgi_server
 
 import bottle
 
-from cloudify._compat import text_type, queue, StringIO
 from cloudify.proxy.client import ScriptException
 from cloudify.state import current_ctx
 
 
 class CtxProxy(object):
 
     def __init__(self, ctx, socket_url):
@@ -151,15 +152,15 @@
     num_args = len(args)
     index = 0
     while index < num_args:
         arg = args[index]
         desugared_attr = _desugar_attr(current, arg)
         if desugared_attr:
             current = getattr(current, desugared_attr)
-        elif isinstance(current, collections.MutableMapping):
+        elif isinstance(current, MutableMapping):
             key = arg
             path_dict = PathDictAccess(current)
             if index + 1 == num_args:
                 # read dict prop by path
                 value = path_dict.get(key)
                 current = value
             elif index + 2 == num_args:
@@ -168,15 +169,15 @@
                 current = path_dict.set(key, value)
             else:
                 raise RuntimeError('Illegal argument while accessing dict')
             break
         elif callable(current):
             kwargs = {}
             remaining_args = args[index:]
-            if isinstance(remaining_args[-1], collections.MutableMapping):
+            if isinstance(remaining_args[-1], MutableMapping):
                 kwargs = remaining_args[-1]
                 remaining_args = remaining_args[:-1]
             current = current(*remaining_args, **kwargs)
             break
         else:
             raise RuntimeError('{0} cannot be processed in {1}'
                                .format(arg, args))
@@ -185,15 +186,15 @@
     if callable(current):
         current = current()
 
     return current
 
 
 def _desugar_attr(obj, attr):
-    if not isinstance(attr, text_type):
+    if not isinstance(attr, str):
         return None
     try:
         if hasattr(obj, attr):
             return attr
     except UnicodeError:
         return None
     attr = attr.replace('-', '_')
```

### Comparing `cloudify-common-6.4.2/cloudify/rabbitmq_client.py` & `cloudify-common-7.0.0/cloudify/rabbitmq_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ############
 
 import os
 import random
 import requests
 import tempfile
 
-from cloudify._compat import urlquote
+from urllib.parse import quote as urlquote
 from cloudify.utils import ipv6_url_compat
 
 
 RABBITMQ_MANAGEMENT_PORT = 15671
 USERNAME_PATTERN = 'rabbitmq_user_{0}'
```

### Comparing `cloudify-common-6.4.2/cloudify/snapshots.py` & `cloudify-common-7.0.0/cloudify/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/snmp/CLOUDIFY-MIB.mib` & `cloudify-common-7.0.0/cloudify/snmp/CLOUDIFY-MIB.mib`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/snmp/snmp_trap.py` & `cloudify-common-7.0.0/cloudify/snmp/snmp_trap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/state.py` & `cloudify-common-7.0.0/cloudify/state.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/systemddbus.py` & `cloudify-common-7.0.0/cloudify/systemddbus.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/test_utils/__init__.py` & `cloudify-common-7.0.0/cloudify/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/test_utils/dispatch_helper.py` & `cloudify-common-7.0.0/cloudify/test_utils/dispatch_helper.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/test_utils/local_workflow_decorator.py` & `cloudify-common-7.0.0/cloudify/test_utils/local_workflow_decorator.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/test_utils/mock_rest_client.py` & `cloudify-common-7.0.0/cloudify/test_utils/mock_rest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         'relationships': relationships,
         'index': index or 0,
     })
 
 
 class MockRestclient(CloudifyClient):
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         pass
 
     @property
     def node_instances(self):
         return MockNodeInstancesClient()
 
     @property
```

### Comparing `cloudify-common-6.4.2/cloudify/tests/__init__.py` & `cloudify-common-7.0.0/dsl_parser/elements/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 ########
-# Copyright (c) 2013 GigaSpaces Technologies Ltd. All rights reserved
+# Copyright (c) 2015 GigaSpaces Technologies Ltd. All rights reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
+from dsl_parser import (version as _version,
+                        exceptions,
+                        models)
+from dsl_parser.framework.elements import Element, Leaf
 
-import logging
-import sys
 
+class ToscaDefinitionsVersion(Element):
 
-def get_logger(name):
-    ch = logging.StreamHandler(sys.stdout)
-    ch.setLevel(logging.DEBUG)
-    formatter = logging.Formatter(fmt='%(asctime)s [%(levelname)s] '
-                                      '[%(name)s] %(message)s',
-                                  datefmt='%H:%M:%S')
-    ch.setFormatter(formatter)
-
-    logger = logging.getLogger(name)
-    for handler in logger.handlers:
-        logger.removeHandler(handler)
-
-    logger.addHandler(ch)
-    logger.setLevel(logging.DEBUG)
-    return logger
+    schema = Leaf(type=str)
+    add_namespace_to_schema_elements = False
+    provides = ['version']
+
+    def validate(self):
+        if self.initial_value is None:
+            raise exceptions.DSLParsingLogicException(
+                27, '{0} field must appear in the main blueprint file'.format(
+                    _version.VERSION))
+
+        _version.validate_dsl_version(self.initial_value)
+
+    def parse(self):
+        return models.Version(_version.process_dsl_version(self.initial_value))
+
+    def calculate_provided(self):
+        return {
+            'version': _version.parse_dsl_version(self.initial_value)
+        }
```

### Comparing `cloudify-common-6.4.2/cloudify/tests/test_tasks_graph.py` & `cloudify-common-7.0.0/cloudify/workflows/tasks_graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,762 +1,718 @@
 ########
-# Copyright (c) 2018 Cloudify Platform Ltd. All rights reserved
+# Copyright (c) 2014 GigaSpaces Technologies Ltd. All rights reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-import mock
-import time
-import testtools
-from contextlib import contextmanager
 
-from cloudify_rest_client.operations import Operation
+import time
+import threading
+from collections import defaultdict
+from functools import wraps
 
-from cloudify.exceptions import WorkflowFailed, NonRecoverableError
+from cloudify.utils import get_func
+from cloudify.exceptions import WorkflowFailed
 from cloudify.workflows import api
 from cloudify.workflows import tasks
-from cloudify.workflows.tasks_graph import TaskDependencyGraph
+from cloudify.state import workflow_ctx
+
+
+def make_or_get_graph(f):
+    """Decorate a graph-creating function with this, to automatically
+    make it try to retrieve the graph from storage first.
+    """
+    @wraps(f)
+    def _inner(*args, **kwargs):
+        if workflow_ctx.dry_run:
+            kwargs.pop('name', None)
+            return f(*args, **kwargs)
+        name = kwargs.pop('name')
+        graph = workflow_ctx.get_tasks_graph(name)
+        if not graph:
+            graph = f(*args, **kwargs)
+            graph.store(name=name)
+        else:
+            graph = TaskDependencyGraph.restore(workflow_ctx, graph)
+        return graph
+    return _inner
+
+
+class TaskDependencyGraphError(object):
+    def __init__(self, task_name, traceback, error_causes, error_time=None):
+        self.task_name = task_name
+        self.traceback = traceback
+        self.error_causes = error_causes
+        self.error_time = error_time or time.time()
+
+
+def _task_error_causes_short(task):
+    """Examine the task, and return a summary of its errors.
+
+    If the task didn't error out, return the empty string.
+    """
+    if not hasattr(task, 'error') or not isinstance(task.error, dict):
+        return ''
+    error_parts = []
+    causes = task.error.get('known_exception_type_kwargs', {}).get('causes')
+    for c in causes:
+        error_parts.append('{0} `{1}`'.format(c['type'], c['message']))
+    if not causes:
+        # no known causes - just show the exception directly
+        error_parts.append(
+            '{0} `{1}`'.format(
+                task.error['exception_type'],
+                task.error['message']
+            )
+        )
+    return '\n'.join(error_parts)
+
+
+def _task_error_causes_traceback(task):
+    """Examine the task, and return tracebacks of its errors.
+
+    The tracebacks are concatenated into a single string.
+    If the task didn't error out, return the empty string.
+    """
+    if not hasattr(task, 'error') or not isinstance(task.error, dict):
+        return ''
+    error_parts = []
+    for c in task.error.get('known_exception_type_kwargs', {}).get('causes'):
+        traceback = c.get('traceback')
+        if traceback:
+            # this is a bit dirty - remove the first line of the traceback,
+            # which says "Traceback (most recent call last):". This is so
+            # that we can add our own line instead later, which also
+            # says the name of the erroring out task
+            header, _, traceback = traceback.strip().partition('\n')
+            error_parts.append(traceback)
+    return '\n'.join(error_parts)
 
-from cloudify.state import current_workflow_ctx
-from cloudify.plugins.lifecycle import LifecycleProcessor
-from cloudify.workflows.workflow_context import (
-    _WorkflowContextBase,
-    WorkflowNodesAndInstancesContainer
-)
-from cloudify_rest_client.node_instances import NodeInstance
-from cloudify_rest_client.nodes import Node
-
-
-@contextmanager
-def limited_sleep_mock(limit=100):
-    # using lists to allow a 'nonlocal' set in py2
-    current_time = [time.time()]
-    calls = [0]
-
-    def _fake_sleep(delta):
-        current_time[0] += delta
-        calls[0] += 1
-        if calls[0] > limit:
-            raise RuntimeError('Timeout')
-
-    def _fake_time():
-        return current_time[0]
-
-    mock_sleep = mock.patch('time.sleep', _fake_sleep)
-    mock_time = mock.patch('time.time', _fake_time)
-    with mock_sleep:
-        with mock_time:
-            yield mock_sleep, mock_time
-
-
-class MockWorkflowContext(_WorkflowContextBase):
-    wait_after_fail = 600
-    dry_run = False
-    resume = False
 
+class TaskDependencyGraphErrors(object):
     def __init__(self):
-        super(MockWorkflowContext, self).__init__({}, lambda *a: mock.Mock())
-        self.internal.handler.operation_cloudify_context = {}
+        self._errors = []
 
+    def __len__(self):
+        return len(self._errors)
 
-class FailedTask(tasks.WorkflowTask):
-    """A task that always immediately fails with a NonRecoverableError"""
-    name = 'failtask'
+    def __bool__(self):
+        return len(self._errors) > 0
 
-    def apply_async(self):
-        self.async_result.result = NonRecoverableError()
-        self.set_state(tasks.TASK_FAILED)
-        return self.async_result
+    def add_error(self, result, task):
+        summary = "Task failed: {0}".format(task.short_description)
+        short_causes_text = _task_error_causes_short(task)
+        if short_causes_text:
+            summary = '{0}: {1}'.format(summary, short_causes_text)
+        self._errors.append(TaskDependencyGraphError(
+            task_name=task.short_description,
+            error_causes=short_causes_text,
+            traceback=_task_error_causes_traceback(task),
+        ))
+
+    def first_error_time(self):
+        if not self._errors:
+            return None
+        return self._errors[0].error_time
 
+    def format_exception(self):
+        """Turn errors stored here into a single human-readable WorkflowFailed
 
-class PassedTask(tasks.WorkflowTask):
-    """A task that always immediately completes successfully"""
-    name = 'task'
+        This formats the actual message the user will see. Show information
+        about all errors that happened, and a traceback.
+        """
+        if not self._errors:
+            return None
+        if len(self._errors) > 1:
+            message = '{0} operation errors:\n{1}'.format(
+                len(self._errors),
+                '\n'.join(
+                    '{0}: {1}'.format(err.task_name, err.error_causes)
+                    for err in self._errors
+                ),
+            )
+        else:
+            message = 'Task failed: {0}: {1}'.format(
+                self._errors[0].task_name,
+                self._errors[0].error_causes,
+            )
+        if self._errors[0].traceback:
+            message = (
+                '{0}\nTraceback of {1} (most recent call last):\n{2}'
+                .format(
+                    message,
+                    self._errors[0].task_name,
+                    self._errors[0].traceback,
+                )
+            )
+        return WorkflowFailed(
+            message,
+            # a task failed, not the workflow function itself: no need to
+            # show the traceback of the workflow function
+            hide_traceback=True,
+        )
+
+
+class TaskDependencyGraph(object):
+    """A task graph.
+
+    :param workflow_context: A WorkflowContext instance (used for logging)
+    """
+
+    @classmethod
+    def restore(cls, workflow_context, retrieved_graph):
+        graph = cls(workflow_context, graph_id=retrieved_graph.id)
+        ops = workflow_context.get_operations(retrieved_graph.id)
+        graph._restore_operations(ops)
+        graph._restore_dependencies(ops)
+        graph._stored = True
+        return graph
+
+    def __init__(self, workflow_context, graph_id=None,
+                 default_subgraph_task_config=None):
+        self.ctx = workflow_context
+        default_subgraph_task_config = default_subgraph_task_config or {}
+        self._default_subgraph_task_config = default_subgraph_task_config
+        self._wake_after_fail = None
+        self._stored = False
+        self.id = graph_id
+        self._tasks = {}
+        self._dependencies = defaultdict(set)
+        self._dependents = defaultdict(set)
+        self._ready = set()
+        self._waiting_for = set()
+        self._tasks_wait = threading.Event()
+        self._finished_tasks = {}
+        self._op_types_cache = {}
+        self._errors = None
 
-    def apply_async(self):
-        self.set_state(tasks.TASK_SUCCEEDED)
-        self.async_result.result = None
-        return self.async_result
+    def optimize(self):
+        """Optimize this tasks graph, removing tasks that do nothing.
 
+        Empty subgraphs, and NOP tasks, are dropped. A subgraph is considered
+        empty if it only contains NOP tasks, and empty subgraphs.
+        """
+        removable = [
+            task for task in self._tasks.values()
+            if task.is_nop()
+        ]
+        for task in removable:
+            dependents = self._dependents[task]
+            dependencies = self._dependencies[task]
+            if task.containing_subgraph:
+                task.containing_subgraph.tasks.pop(task.id)
+            self.remove_task(task)
+            for dependent in dependents:
+                for dependency in dependencies:
+                    self.add_dependency(dependent, dependency)
+
+    def linearize(self):
+        """Traverse the graph, and return tasks in dependency order.
+
+        This makes sure that if task A depends on task B, then A is
+        going to be after B in the resulting list. Ordering of tasks
+        that are not related by dependencies is undefined.
 
-class TestTasksGraphExecute(testtools.TestCase):
-    def test_executes_single_task(self):
-        """A single NOP task is executed within a single iteration of the
-        tasks graph loop"""
-        g = TaskDependencyGraph(MockWorkflowContext())
-        task = tasks.NOPLocalWorkflowTask(mock.Mock())
-        g.add_task(task)
-        with limited_sleep_mock(limit=1):
-            g.execute()
-        self.assertTrue(task.is_terminated)
-
-    def test_executes_multiple_concurrent(self):
-        """Independent tasks will be executed concurrently within the same
-        iteration of the graph loop.
-        """
-        g = TaskDependencyGraph(MockWorkflowContext())
-        task1 = tasks.NOPLocalWorkflowTask(mock.Mock())
-        task2 = tasks.NOPLocalWorkflowTask(mock.Mock())
-        g.add_task(task1)
-        g.add_task(task2)
-        with limited_sleep_mock(limit=1):
-            g.execute()
-        self.assertTrue(task1.is_terminated)
-        self.assertTrue(task2.is_terminated)
-
-    def test_task_failed(self):
-        """Execution is stopped when a task failed. The next task is not
-        executed"""
-
-        task1 = FailedTask(mock.Mock(), total_retries=0)
-        task2 = mock.Mock(execute_after=0)
-
-        g = TaskDependencyGraph(MockWorkflowContext())
-        seq = g.sequence()
-        seq.add(task1, task2)
-
-        with limited_sleep_mock():
-            self.assertRaisesRegex(WorkflowFailed, 'failtask', g.execute)
-        self.assertTrue(task1.is_terminated)
-        self.assertFalse(task2.apply_async.called)
+        This is useful for logging, debugging, and testing.
+        """
+        dependencies_copy = {k: set(v) for k, v in self._dependencies.items()}
+        ordered = []
+        ready = [
+            task for task in self._tasks.values()
+            if not dependencies_copy.get(task)
+        ]
+        while ready:
+            new_ready = []
+            for task in ready:
+                ordered.append(task)
+                for dependent_task in self._dependents[task]:
+                    dependencies_copy[dependent_task].discard(task)
+                    if not dependencies_copy.get(dependent_task):
+                        new_ready.append(dependent_task)
+            ready = new_ready
+        return ordered
 
-    def test_task_sequence(self):
-        """Tasks in a sequence are called in order"""
+    def _restore_dependencies(self, ops):
+        """Set dependencies between this graph's tasks according to ops.
 
-        class Task(tasks.WorkflowTask):
-            name = 'task'
+        :param ops: a list of rest-client Operation objects
+        """
+        # a mapping of operations which retry previously-failed operations
+        retries_dict = dict(
+            (x.parameters['retried_task'], x.id) for x in ops if
+            x.parameters.get('retried_task'))
+
+        for op_descr in ops:
+            op = self.get_task(op_descr.id)
+            if op is None:
+                continue
+            for target_id in op_descr.dependencies:
+                target = self.get_task(target_id)
+                if target is not None:
+                    self.add_dependency(op, target)
+                else:
+                    new_target = self._retrieve_active_target(target_id,
+                                                              retries_dict)
+                    if new_target is not None:
+                        self.add_dependency(op, new_target)
+
+    def _retrieve_active_target(self, target_id, retries_dict):
+        # traverse the retried task chain to find the active task which
+        # corresponds to the defunct target
+        next_target = target_id
+        while next_target:
+            last_target = next_target
+            next_target = retries_dict.get(last_target)
+        return self.get_task(last_target)
 
-            def apply_async(self):
-                record.append(self.i)
-                self.set_state(tasks.TASK_SUCCEEDED)
-                self.async_result.result = None
-                return self.async_result
+    def _restore_operations(self, ops):
+        """Restore operations from ops into this graph.
 
-        task_count = 10
+        :param ops: a list of rest-client Operation objects
+        """
+        ops_by_id = dict((op.id, op) for op in ops)
+        restored_ops = {}
+        for op_descr in ops:
+            if op_descr.id in restored_ops:  # already restored - a subgraph
+                continue
+            if op_descr.state in tasks.TERMINATED_STATES:
+                continue
+
+            op = self._restore_operation(op_descr)
+            restored_ops[op_descr.id] = op
+
+            # restore the subgraph - even if the subgraph was already finished,
+            # we are going to be running an operation from it, so mark it as
+            # pending again.
+            # Follow the subgraph hierarchy up.
+            while op_descr.containing_subgraph:
+                subgraph_id = op_descr.containing_subgraph
+                subgraph_descr = ops_by_id[subgraph_id]
+                subgraph_descr['state'] = tasks.TASK_STARTED
+                subgraph = self._restore_operation(subgraph_descr)
+                self.add_task(subgraph)
+                restored_ops[subgraph_id] = subgraph
+
+                op.containing_subgraph = subgraph
+                subgraph.add_task(op)
+
+                op, op_descr = subgraph, subgraph_descr
 
-        # prepare the task seuqence
-        seq_tasks = []
-        for i in range(task_count):
-            t = Task(mock.Mock())
-            seq_tasks.append(t)
-            t.i = i
-        g = TaskDependencyGraph(MockWorkflowContext())
-        seq = g.sequence()
-        seq.add(*seq_tasks)
-
-        record = []
-
-        with limited_sleep_mock():
-            g.execute()
-
-        expected = list(range(task_count))
-        self.assertEqual(expected, record)
-
-    def test_cancel(self):
-        """When execution is cancelled, an error is thrown and tasks are
-        not executed.
-        """
-        g = TaskDependencyGraph(MockWorkflowContext())
-        task = mock.Mock()
-        g.add_task(task)
-        with mock.patch('cloudify.workflows.api.cancel_request', True):
-            self.assertRaises(api.ExecutionCancelled, g.execute)
-
-        self.assertFalse(task.apply_async.called)
-        self.assertFalse(task.cancel.called)
-
-    def test_task_on_success(self):
-        """If a task has a success callback, dependent tasks still run"""
-        wctx = MockWorkflowContext()
-        g = TaskDependencyGraph(wctx)
-        record = []
+            self.add_task(op)
 
-        class Task(tasks.WorkflowTask):
-            name = 'task'
+    def _restore_operation(self, op_descr):
+        """Create a Task object from a rest-client Operation object.
 
-            def apply_async(self):
-                record.append(self.i)
-                self.set_state(tasks.TASK_SUCCEEDED)
-                self.async_result.result = None
-                return self.async_result
+        If the task was already restored before, return a reference to the
+        same object.
+        """
+        restored = self.get_task(op_descr.id)
+        if restored is not None:
+            return restored
+        op_cls = self._get_operation_class(op_descr.type)
+        return op_cls.restore(
+            self.ctx._get_current_object(), self, op_descr)
+
+    def _get_operation_class(self, task_type):
+        if task_type in self._op_types_cache:
+            return self._op_types_cache[task_type]
+        if task_type == 'SubgraphTask':
+            op_cls = SubgraphTask
+        elif '.' in task_type:
+            op_cls = get_func(task_type)
+        else:
+            op_cls = getattr(tasks, task_type)
+
+        if not issubclass(op_cls, tasks.WorkflowTask):
+            raise RuntimeError('{0} is not a subclass of WorkflowTask'
+                               .format(task_type))
+        self._op_types_cache[task_type] = op_cls
+        return op_cls
+
+    def store(self, name, optimize=True):
+        if optimize:
+            self.optimize()
+        serialized_tasks = []
+        for task in self._tasks.values():
+            serialized = task.dump()
+            serialized['dependencies'] = [
+                dep.id for dep in self._dependencies.get(task, [])]
+            serialized_tasks.append(serialized)
+        stored_graph = self.ctx.store_tasks_graph(
+            name, operations=serialized_tasks)
+        if stored_graph:
+            self.id = stored_graph['id']
+            self._stored = True
+            for task in self._tasks.values():
+                task.stored = True
+
+    @property
+    def tasks(self):
+        return list(self._tasks.values())
 
-        def on_success(task):
-            record.append('success')
-            return tasks.HandlerResult.cont()
-
-        t1 = Task(wctx)
-        t1.i = 1
-        t2 = Task(wctx)
-        t1.on_success = on_success
-        t2.i = 2
-        g.add_task(t1)
-        g.add_task(t2)
-        g.add_dependency(t2, t1)
-        g.execute()
-        assert record == [1, 'success', 2]
-
-    def test_continue_after_fail(self):
-        wctx = MockWorkflowContext()
-        g = TaskDependencyGraph(wctx)
-
-        ft = FailedTask(wctx)
-        t1 = PassedTask(wctx)
-        t2 = PassedTask(wctx)
-        t3 = PassedTask(wctx)
-        t4 = PassedTask(wctx)
-        t5 = PassedTask(wctx)
-        for t in [t1, t2, t3, t4, t5, ft]:
-            g.add_task(t)
-
-        # there's two disjoint subgraphs:
-        # t1 -> ft -> t2
-        # t3 -> t4 -> t5
-        # t1 runs, ft fails, and t2 does not run
-        # t3, t4, and t5 all run
-        g.add_dependency(ft, t1)
-        g.add_dependency(t2, ft)
-        g.add_dependency(t4, t3)
-        g.add_dependency(t5, t4)
-
-        self.assertRaisesRegex(WorkflowFailed, 'failtask', g.execute)
-        for t in [t1, t3, t4, t5]:
-            assert t.get_state() == 'succeeded'
-        assert t2.get_state() == 'pending'
-
-    def test_dependency_failed(self):
-        wctx = MockWorkflowContext()
-        g = TaskDependencyGraph(wctx)
-
-        ft = FailedTask(wctx)
-        t1 = PassedTask(wctx)
-        t2 = PassedTask(wctx)
-        for t in [ft, t1, t2]:
-            g.add_task(t)
-
-        g.add_dependency(t2, t1)
-        g.add_dependency(t2, ft)
-
-        self.assertRaisesRegex(WorkflowFailed, 'failtask', g.execute)
-        assert t1.get_state() == 'succeeded'
-        assert ft.get_state() == 'failed'
-        assert t2.get_state() == 'pending'
-
-
-class _CustomRestorableTask(tasks.WorkflowTask):
-    """A custom user-provided task, that can be restored"""
-    name = '_CustomRestorableTask'
-    task_type = 'cloudify.tests.test_tasks_graph._CustomRestorableTask'
-
-
-class TestTaskGraphRestore(testtools.TestCase):
-    def _remote_task(self):
-        """Make a RemoteWorkflowTask mock for use in tests"""
-        return {
-            'type': 'RemoteWorkflowTask',
-            'dependencies': [],
-            'parameters': {
-                'info': {},
-                'current_retries': 0,
-                'send_task_events': False,
-                'containing_subgraph': None,
-                'task_kwargs': {
-                    'kwargs': {
-                        '__cloudify_context': {}
-                    }
-                }
-            }
-        }
+    def add_task(self, task):
+        """Add a WorkflowTask to this graph
 
-    def _subgraph(self):
-        """Make a SubgraphTask mock for use in tests"""
-        return {
-            'type': 'SubgraphTask',
-            'id': 0,
-            'dependencies': [],
-            'parameters': {
-                'info': {},
-                'current_retries': 0,
-                'send_task_events': False,
-                'containing_subgraph': None,
-                'task_kwargs': {}
-            }
-        }
+        :param task: The task
+        """
+        self._tasks[task.id] = task
+        self._ready.add(task)
 
-    def _restore_graph(self, operations):
-        mock_wf_ctx = mock.Mock()
-        mock_wf_ctx.get_operations.return_value = [
-            Operation(op) for op in operations]
-        mock_retrieved_graph = mock.Mock(id=0)
-        return TaskDependencyGraph.restore(mock_wf_ctx, mock_retrieved_graph)
-
-    def test_restore_empty(self):
-        """Restoring an empty list of operations results in an empty graph"""
-        assert self._restore_graph([]).tasks == []
-
-    def test_restore_single(self):
-        """A single operation is restored into the graph"""
-        graph = self._restore_graph([self._remote_task()])
-        assert len(graph.tasks) == 1
-        assert isinstance(graph.tasks[0], tasks.RemoteWorkflowTask)
-
-    def test_restore_finished(self):
-        """Finished tasks are not restored into the graph"""
-        task = self._remote_task()
-        task['state'] = tasks.TASK_SUCCEEDED
-        graph = self._restore_graph([task])
-        assert graph.tasks == []
-
-    def test_restore_with_subgraph(self):
-        """Restoring operations keeps subgraph structure"""
-        subgraph = self._subgraph()
-        task = self._remote_task()
-        subgraph['id'] = 15
-        task['parameters']['containing_subgraph'] = 15
-
-        graph = self._restore_graph([subgraph, task])
-        assert len(graph.tasks) == 2
-        subgraphs = [op for op in graph.tasks if op.is_subgraph]
-        remote_tasks = [op for op in graph.tasks if not op.is_subgraph]
-
-        assert len(subgraphs) == 1
-        assert len(remote_tasks) == 1
-
-        assert len(subgraphs[0].tasks) == 1
-        assert remote_tasks[0].containing_subgraph is subgraphs[0]
-
-    def test_restore_with_dependencies(self):
-        """Restoring operations keeps the dependency structure"""
-        task1 = self._remote_task()
-        task1['id'] = 1
-        task2 = self._remote_task()
-        task2['id'] = 2
-        task2['dependencies'] = [1]
-
-        graph = self._restore_graph([task1, task2])
-        assert len(graph.tasks) == 2
-        assert graph._dependencies[2] == set([1])
-
-    def test_restore_with_finished_subgraph(self):
-        """Restoring operations keeps subgraph structure"""
-        subgraph = self._subgraph()
-        task = self._remote_task()
-        subgraph['id'] = 15
-        task['parameters']['containing_subgraph'] = 15
-
-        subgraph['state'] = tasks.TASK_SUCCEEDED
-
-        graph = self._restore_graph([subgraph, task])
-        assert len(graph.tasks) == 2
-        subgraphs = [op for op in graph.tasks if op.is_subgraph]
-        remote_tasks = [op for op in graph.tasks if not op.is_subgraph]
-
-        assert len(subgraphs) == 1
-        assert len(remote_tasks) == 1
-
-        assert len(subgraphs[0].tasks) == 1
-        assert remote_tasks[0].containing_subgraph is subgraphs[0]
-
-    def test_restore_multiple_in_subgraph(self):
-        """Multiple tasks in the same subgraph, reference the same subgraph.
-
-        As opposed to restoring the same subgraph multiple times, it's all
-        references to one object. If it was restored multiple times, then
-        the next task in the subgraph would still run even if a previous
-        task failed.
-        """
-        subgraph = self._subgraph()
-        subgraph['id'] = 15
-        task1 = self._remote_task()
-        task1['id'] = 1
-        task2 = self._remote_task()
-        task2['id'] = 2
-        task1['parameters']['containing_subgraph'] = 15
-        task2['parameters']['containing_subgraph'] = 15
-
-        graph = self._restore_graph([subgraph, task1, task2])
-        assert len(graph.tasks) == 3
-        subgraphs = [op for op in graph.tasks if op.is_subgraph]
-        remote_tasks = [op for op in graph.tasks if not op.is_subgraph]
-
-        # those are all references to the same subgraph, the subgraph was
-        # NOT restored multiple times
-        assert remote_tasks[0].containing_subgraph \
-            is remote_tasks[1].containing_subgraph \
-            is subgraphs[0]
-
-        assert len(subgraphs[0].tasks) == 2
-
-    def test_restore_custom(self):
-        task = _CustomRestorableTask(None)
-        serialized = task.dump()
-        # dependencies are added by the graph normally, not by task.dump
-        serialized['dependencies'] = []
-
-        graph = self._restore_graph([serialized])
-        assert len(graph.tasks) == 1
-        assert isinstance(graph.tasks[0], _CustomRestorableTask)
-        # ..but we didn't just get the same object back, it was restored indeed
-        assert graph.tasks[0] is not task
+    def get_task(self, task_id):
+        """Get a task instance that was inserted to this graph by its id
 
+        :param task_id: the task id
+        :return: a WorkflowTask instance for the requested task if found.
+                 None, otherwise.
+        """
+        return self._tasks.get(task_id)
 
-class NonExecutingGraph(TaskDependencyGraph):
-    """A TaskDependencyGraph that never actually executes anything"""
-    def execute(self):
-        return
+    def remove_task(self, task):
+        """Remove the provided task from the graph
 
-    def store(self, name=None):
-        pass
+        :param task: The task
+        """
+        if task.is_subgraph:
+            for subgraph_task in task.tasks.values():
+                self.remove_task(subgraph_task)
+        if task.id in self._tasks:
+            del self._tasks[task.id]
+            self._ready.discard(task)
+            for dependent in self._dependents.pop(task, []):
+                self._dependencies[dependent].discard(task)
+                if not self._dependencies.get(dependent):
+                    self._ready.add(dependent)
+            for dependency in self._dependencies.pop(task, []):
+                self._dependents[dependency].discard(task)
+
+    def add_dependency(self, src_task, dst_task):
+        """Add a dependency between tasks: src depends on dst.
+
+        The source task will only be executed after the target task terminates.
+        A task may depend on several tasks, in which case it will only be
+        executed after all its 'destination' tasks terminate
 
+        :param src_task: The source task
+        :param dst_task: The target task
+        """
+        if src_task == dst_task:
+            return
+        if src_task.id not in self._tasks:
+            raise RuntimeError('src not in graph: {0!r}'.format(src_task))
+        if dst_task.id not in self._tasks:
+            raise RuntimeError('dst not in graph: {0!r}'.format(dst_task))
+        self._dependencies[src_task].add(dst_task)
+        self._dependents[dst_task].add(src_task)
+        self._ready.discard(src_task)
+
+    def remove_dependency(self, src_task, dst_task):
+        if src_task.id not in self._tasks:
+            raise RuntimeError('src not in graph: {0!r}'.format(src_task))
+        if dst_task.id not in self._tasks:
+            raise RuntimeError('dst not in graph: {0!r}'.format(dst_task))
+        self._dependencies[src_task].discard(dst_task)
+        self._dependents[dst_task].discard(src_task)
+        if not self._dependencies[src_task]:
+            self._ready.add(src_task)
+            self._tasks_wait.set()
 
-class TestLifecycleGraphs(testtools.TestCase):
-    def _make_ctx_and_graph(self):
-        ctx = MockWorkflowContext()
-        graph = NonExecutingGraph(ctx)
-        ctx.get_tasks_graph = mock.Mock(return_value=None)
-        ctx.get_operations = mock.Mock(return_value=[])
-        ctx.internal.graph_mode = True
-        return ctx, graph
-
-    def _make_node(self, **kwargs):
-        node = {
-            'id': 'node1',
-            'relationships': [],
-            'operations': {},
-            'id': 'node1',
-            'type_hierarchy': []
-        }
-        node.update(kwargs)
-        return Node(node)
+    def sequence(self):
+        """
+        :return: a new TaskSequence for this graph
+        """
+        return TaskSequence(self)
 
-    def _make_instance(self, **kwargs):
-        instance = {
-            'id': 'node1_1',
-            'node_id': 'node1',
-            'relationships': [],
-        }
-        instance.update(kwargs)
-        return NodeInstance(instance)
+    def subgraph(self, name):
+        task = SubgraphTask(self, info={'name': name},
+                            **self._default_subgraph_task_config)
+        self.add_task(task)
+        return task
 
-    def _make_operation(self, **kwargs):
-        operation = {
-            'operation': 'plugin1.op1',
-            'plugin': 'plugin1',
-            'has_intrinsic_functions': False,
-            'executor': 'host_agent',
-            'max_retries': 10,
-            'retry_interval': 10,
-        }
-        operation.update(kwargs)
-        return operation
+    def execute(self):
+        """Execute tasks in this graph.
 
-    def _make_lifecycle_processor(self, ctx, graph, nodes, instances):
-        container = WorkflowNodesAndInstancesContainer(
-            ctx, nodes, instances)
-        return LifecycleProcessor(
-            graph,
-            node_instances=list(container.node_instances)
-        )
+        Run ready tasks, register callbacks on their result, process
+        results from tasks that did finish.
+        Tasks whose dependencies finished, are marked as ready for
+        the next iteration.
+
+        This main loop is directed by the _tasks_wait event, which
+        is set only when there is something to be done: a task response
+        has been received, some tasks dependencies finished which makes
+        new tasks ready to be run, or the execution was cancelled.
 
-    def _make_plugin(self, name='plugin1'):
-        return {'name': name, 'package_name': name}
+        If a task failed, wait for ctx.wait_after_fail for additional
+        responses to come in anyway.
+        """
+        self._errors = TaskDependencyGraphErrors()
+        api.cancel_callbacks.add(self._tasks_wait.set)
 
-    def test_install_empty(self):
-        """No instances - no operations"""
-        ctx, graph = self._make_ctx_and_graph()
-        pr = LifecycleProcessor(graph)
-        with current_workflow_ctx.push(ctx):
-            pr.install()
-        assert graph.tasks == []
-
-    def test_install_empty_instance(self):
-        """Instance without interfaces - still set to started"""
-        ctx, graph = self._make_ctx_and_graph()
-        pr = self._make_lifecycle_processor(
-            ctx, graph,
-            nodes=[self._make_node()],
-            instances=[self._make_instance()]
-        )
-        with current_workflow_ctx.push(ctx):
-            pr.install()
-        assert any(
-            task.name == 'SetNodeInstanceStateTask'
-            and task.info == 'started'
-            for task in graph.tasks
-        )
+        while not self._is_finished():
+            self._tasks_wait.clear()
+
+            while self._ready:
+                task = self._ready.pop()
+                if task.dependency_error:
+                    # this task was "ready" because all of its dependencies
+                    # finished (at least one successfully), but one of the
+                    # dependencies finished with an error. It must not run.
+                    continue
+                self._run_task(task)
+
+            self._tasks_wait.wait(1)
+
+            while self._finished_tasks:
+                task, result = self._finished_tasks.popitem()
+                self._handle_terminated_task(result, task)
+
+        api.cancel_callbacks.discard(self._tasks_wait.set)
+        if self._wake_after_fail:
+            self._wake_after_fail.cancel()
+        if self._errors:
+            raise self._errors.format_exception()
+        if api.has_cancel_request():
+            raise api.ExecutionCancelled()
+
+    def _is_finished(self):
+        if api.has_cancel_request():
+            return True
+
+        if not self._tasks:
+            return True
+
+        if self._errors:
+            if not self._waiting_for and not self._ready:
+                return True
+            deadline = \
+                self._errors.first_error_time() + self.ctx.wait_after_fail
+            if time.time() > deadline:
+                return True
+            else:
+                self._wake_after_fail = threading.Timer(
+                    deadline - time.time(),
+                    self._tasks_wait.set)
+                self._wake_after_fail.daemon = True
+                self._wake_after_fail.start()
+        return False
+
+    def _run_task(self, task):
+        result = task.apply_async()
+        self._waiting_for.add(task)
+        result.on_result(self._task_finished, task)
+
+    def _task_finished(self, result, task):
+        self._finished_tasks[task] = result
+        self._tasks_wait.set()
+
+    def _handle_terminated_task(self, result, task):
+        self._waiting_for.discard(task)
+        handler_result = task.handle_task_terminated()
+        dependents = self._dependents[task]
+        dependencies = self._dependencies[task]
+        self.remove_task(task)
+        if handler_result.action == tasks.HandlerResult.HANDLER_FAIL:
+            if isinstance(task, SubgraphTask) and task.failed_task:
+                task = task.failed_task
+            result = self._task_error(result, task)
+            self._ready -= dependents
+            # mark all the dependent tasks as having a dependency error, so
+            # that they will not run, even if all their other dependencies
+            # finish successfully
+            for d in dependents:
+                d.dependency_error = True
+        elif handler_result.action == tasks.HandlerResult.HANDLER_RETRY:
+            new_task = handler_result.retried_task
+            if self.id is not None:
+                stored = self.ctx.store_operation(
+                    new_task,
+                    [dep.id for dep in self._dependencies[task]],
+                    self.id)
+                if stored:
+                    new_task.stored = True
+            self.add_task(new_task)
+            for dependency in dependencies:
+                self.add_dependency(new_task, self.get_task(dependency))
+            for dependent in dependents:
+                self.add_dependency(self.get_task(dependent), new_task)
+
+        self._tasks_wait.set()
+
+    def _task_error(self, result, task):
+        self._errors.add_error(result, task)
+        self._waiting_for = {
+            t for t in self._waiting_for if not t.is_subgraph
+        }
+        return result
 
-    def test_install_create_operation(self):
-        """Instance with a create interface - the operation is called"""
-        ctx, graph = self._make_ctx_and_graph()
-
-        pr = self._make_lifecycle_processor(
-            ctx, graph,
-            nodes=[self._make_node(
-                operations={
-                    'cloudify.interfaces.lifecycle.create':
-                    self._make_operation()
-                },
-                plugins=[self._make_plugin()]
-            )],
-            instances=[self._make_instance()]
-        )
-        with current_workflow_ctx.push(ctx):
-            pr.install()
-        assert any(
-            task.name == 'plugin1.op1'
-            for task in graph.tasks
-        )
-        assert any(
-            task.name == 'SetNodeInstanceStateTask'
-            and task.info == 'started'
-            for task in graph.tasks
-        )
 
-    def test_update_resumed_install(self):
-        """When resuming an interrupted install, the instance is deleted first
+class forkjoin(object):
+    """
+    A simple wrapper for tasks. Used in conjunction with TaskSequence.
+    Defined to make the code easier to read (instead of passing a list)
+    see ``TaskSequence.add`` for more details
+    """
+
+    def __init__(self, *tasks):
+        self.tasks = tasks
+
+
+class TaskSequence(object):
+    """
+    Helper class to add tasks in a sequential manner to a task dependency
+    graph
+
+    :param graph: The TaskDependencyGraph instance
+    """
+
+    def __init__(self, graph):
+        self.graph = graph
+        self.last_fork_join_tasks = None
+
+    def add(self, *tasks):
+        """Add tasks to the sequence.
+
+        :param tasks: Each task might be:
+            * A WorkflowTask instance, in which case, it will be
+              added to the graph with a dependency between it and
+              the task previously inserted into the sequence
+            * A forkjoin of tasks, in which case it will be treated
+              as a "fork-join" task in the sequence, i.e. all the
+              fork-join tasks will depend on the last task in the
+              sequence (could be fork join) and the next added task
+              will depend on all tasks in this fork-join task
         """
-        ctx, graph = self._make_ctx_and_graph()
+        for fork_join_tasks in tasks:
+            if isinstance(fork_join_tasks, forkjoin):
+                fork_join_tasks = fork_join_tasks.tasks
+            else:
+                fork_join_tasks = [fork_join_tasks]
+            for task in fork_join_tasks:
+                self.graph.add_task(task)
+                if self.last_fork_join_tasks is not None:
+                    for last_fork_join_task in self.last_fork_join_tasks:
+                        self.graph.add_dependency(task, last_fork_join_task)
+            if fork_join_tasks:
+                self.last_fork_join_tasks = fork_join_tasks
+
+
+class SubgraphTask(tasks.WorkflowTask):
+
+    def __init__(self,
+                 graph,
+                 workflow_context=None,
+                 task_id=None,
+                 total_retries=tasks.DEFAULT_SUBGRAPH_TOTAL_RETRIES,
+                 **kwargs):
+        kwargs.setdefault('info', {})
+        super(SubgraphTask, self).__init__(
+            graph.ctx,
+            task_id,
+            total_retries=total_retries,
+            **kwargs)
+        self.graph = graph
+        self.tasks = {}
+        self.failed_task = None
+        if not self.on_failure:
+            self.on_failure = _on_failure_handler_fail
+
+    @classmethod
+    def restore(cls, ctx, graph, task_descr):
+        task_descr.parameters['task_kwargs']['graph'] = graph
+        return super(SubgraphTask, cls).restore(ctx, graph, task_descr)
+
+    def _duplicate(self):
+        raise NotImplementedError('self.retried_task should be set explicitly'
+                                  ' in self.on_failure handler')
+
+    @property
+    def cloudify_context(self):
+        return {}
+
+    def is_local(self):
+        return True
+
+    @property
+    def name(self):
+        return self.info.get('name') or self.id
+
+    @property
+    def is_subgraph(self):
+        return True
+
+    def is_nop(self):
+        return not self.tasks or all(
+            t.is_nop() for t in self.tasks.values()
+        )
+
+    def sequence(self):
+        return TaskSequence(self)
+
+    def subgraph(self, name):
+        task = SubgraphTask(self.graph, info={'name': name},
+                            **self.graph._default_subgraph_task_config)
+        self.add_task(task)
+        return task
+
+    def add_task(self, task):
+        self.graph.add_task(task)
+        self.add_dependency(task, self)
+        self.tasks[task.id] = task
+        if task.containing_subgraph and task.containing_subgraph is not self:
+            raise RuntimeError('task {0}[{1}] cannot be contained in more '
+                               'than one subgraph. It is currently contained '
+                               'in {2} and it is now being added to {3}'
+                               .format(task,
+                                       task.id,
+                                       task.containing_subgraph.name,
+                                       self.name))
+        task.containing_subgraph = self
 
-        node = self._make_node(
-            operations={
-                'cloudify.interfaces.lifecycle.create':
-                self._make_operation(operation='plugin1.op1'),
-                'cloudify.interfaces.lifecycle.delete':
-                self._make_operation(operation='plugin1.op2')
-            },
-            plugins=[{'name': 'plugin1', 'package_name': 'plugin1'}]
-        )
-        instance = self._make_instance()
-        pr = self._make_lifecycle_processor(
-            ctx, graph,
-            nodes=[node],
-            instances=[instance]
-        )
-        with current_workflow_ctx.push(ctx):
-            pr.install()
+    def remove_task(self, task):
+        self.graph.remove_task(task)
 
-        # after creating the install graph, resume it - it should first
-        # delete the instance, before re-installing it
-        ctx.resume = True
-        instance['state'] = 'creating'
-        pr._update_resumed_install(graph)
-
-        delete_task_index = None
-        install_task_index = None
-        for ix, task in enumerate(graph.linearize()):
-            if task.name == 'plugin1.op1':
-                install_task_index = ix
-            elif task.name == 'plugin1.op2':
-                delete_task_index = ix
-
-        assert install_task_index is not None
-        assert delete_task_index is not None
-        assert delete_task_index < install_task_index
-
-    def test_update_resumed_install_dependency(self):
-        """Similar to test_update_resumed_install, but with a relationship too
-        """
-        ctx, graph = self._make_ctx_and_graph()
-
-        node1 = self._make_node(
-            operations={
-                'cloudify.interfaces.lifecycle.create':
-                self._make_operation(operation='plugin1.n1_create'),
-                'cloudify.interfaces.lifecycle.delete':
-                self._make_operation(operation='plugin1.n1_delete')
-            },
-            plugins=[self._make_plugin()]
-        )
-        node2 = self._make_node(
-            relationships=[{
-                'target_id': 'node1',
-                'type_hierarchy': ['cloudify.relationships.depends_on']
-            }],
-            id='node2',
-            operations={
-                'cloudify.interfaces.lifecycle.create':
-                self._make_operation(operation='plugin1.n2_create'),
-                'cloudify.interfaces.lifecycle.delete':
-                self._make_operation(operation='plugin1.n2_delete')
-            },
-            plugins=[self._make_plugin()]
-        )
-        ni1 = self._make_instance()
-        ni2 = self._make_instance(
-            relationships=[{
-                'target_id': 'node1_1',
-                'target_name': 'node1'
-            }],
-            node_id='node2',
-            id='node2_1'
-        )
-        pr = self._make_lifecycle_processor(
-            ctx, graph,
-            nodes=[node1, node2],
-            instances=[ni1, ni2]
-        )
-        with current_workflow_ctx.push(ctx):
-            pr.install()
+    def add_dependency(self, src_task, dst_task):
+        self.graph.add_dependency(src_task, dst_task)
 
-        # resume an install, with one node that was interrupted in creating
-        ni1['state'] = 'creating'
-        ctx.resume = True
-        pr._update_resumed_install(graph)
-
-        # to check that the operations happened in the desired order, examine
-        # their position in the linearized graph
-        task_indexes = {
-            'n1_create': None,
-            'n1_delete': None,
-            'n2_create': None,
-            'n2_delete': None,
-        }
-        for ix, task in enumerate(graph.linearize()):
-            name = task.name.replace('plugin1.', '')
-            if name in task_indexes:
-                task_indexes[name] = ix
-
-        # delete happened before create - reinstall
-        assert task_indexes['n1_delete'] < task_indexes['n1_create']
-        # dependency installed before the dependent
-        assert task_indexes['n1_create'] < task_indexes['n2_create']
-
-        # n2 didnt need to be deleted, because it wasn't in the creating state
-        assert task_indexes['n2_delete'] is None
-
-
-class TestGraphOptimization(testtools.TestCase):
-    """Tests for graph.optimize(), which omits empty/pointless tasks"""
-
-    def test_removes_nop(self):
-        """optimize removes NOPTasks"""
-        ctx = MockWorkflowContext()
-        g = TaskDependencyGraph(ctx)
-        nop_task = tasks.NOPLocalWorkflowTask(ctx)
-        not_nop_task = tasks.WorkflowTask(ctx)
-        g.add_task(nop_task)
-        g.add_task(not_nop_task)
-        assert set(g.tasks) == {nop_task, not_nop_task}
-        g.optimize()
-        assert set(g.tasks) == {not_nop_task}
-
-    def test_removes_dependent_nop(self):
-        """optimize removes NOPTasks even if they have dependencies"""
-        ctx = MockWorkflowContext()
-        g = TaskDependencyGraph(ctx)
-        base_nop_task = tasks.NOPLocalWorkflowTask(ctx)
-        dependent_nop_task = tasks.NOPLocalWorkflowTask(ctx)
-        task = tasks.WorkflowTask(ctx)
-        g.add_task(task)
-        g.add_task(base_nop_task)
-        g.add_task(dependent_nop_task)
-        g.add_dependency(dependent_nop_task, task)
-        g.add_dependency(task, base_nop_task)
-        assert set(g.tasks) == {base_nop_task, dependent_nop_task, task}
-        g.optimize()
-        assert set(g.tasks) == {task}
-
-    def test_moves_dependencies(self):
-        """optimize "shortcuts" dependencies
-
-        We have a dependency chain of: task2 -> nop_task -> task1.
-        After optimize, nop is removed, and the chain is just: task2 -> task1
-        """
-        ctx = MockWorkflowContext()
-        g = TaskDependencyGraph(ctx)
-        task1 = tasks.WorkflowTask(ctx)
-        nop_task = tasks.NOPLocalWorkflowTask(ctx)
-        task2 = tasks.WorkflowTask(ctx)
-        g.add_task(task1)
-        g.add_task(task2)
-        g.add_task(nop_task)
-        g.add_dependency(task2, nop_task)
-        g.add_dependency(nop_task, task1)
-        assert set(g.tasks) == {task1, task2, nop_task}
-        g.optimize()
-        assert set(g.tasks) == {task1, task2}
-        assert g._dependencies == {
-            task2: set([task1]),
-        }
-        assert g._dependents == {
-            task1: set([task2]),
-        }
+    def apply_async(self):
+        super(SubgraphTask, self).apply_async()
+        if not self.tasks:
+            self.set_state(tasks.TASK_SUCCEEDED)
+        else:
+            # subgraph started - allow its tasks to run - remove their
+            # dependency on the subgraph, so they don't wait on the
+            # subgraph anymore
+            for task_id, task in self.tasks.items():
+                self.graph.remove_dependency(task, self)
+            self.set_state(tasks.TASK_STARTED)
+        return self.async_result
 
-    def test_moves_chain_dependencies(self):
-        r"""The dependency shortcut works even with more complex graphs
+    def task_terminated(self, task, new_task=None):
+        del self.tasks[task.id]
+        if new_task:
+            self.tasks[new_task.id] = new_task
+            new_task.containing_subgraph = self
+        if self.get_state() not in tasks.TERMINATED_STATES:
+            if self.failed_task:
+                self.set_state(tasks.TASK_FAILED)
+            elif not self.tasks:
+                self.set_state(tasks.TASK_SUCCEEDED)
+
+    def set_state(self, state):
+        super(SubgraphTask, self).set_state(state)
+        if state in tasks.TERMINATED_STATES:
+            self.async_result.result = None
+
+    def __repr__(self):
+        return '<{0} {1}: {2}>'.format(self.task_type, self.id, self.name)
 
-        The setup is:
-            task1 \                                 / task3
-                   >- nop1 -> nop2 -> ... -> nop10 <
-            task2 /                                 \ task4
-
-        After optimization, all the NOPs are removed, and we're left with
-        only:
-            task1 \ / task3
-                   x
-            task2 / \ task4
-        """
-        ctx = MockWorkflowContext()
-        g = TaskDependencyGraph(ctx)
-        task1 = tasks.WorkflowTask(ctx)
-        task2 = tasks.WorkflowTask(ctx)
-        task3 = tasks.WorkflowTask(ctx)
-        task4 = tasks.WorkflowTask(ctx)
-        nops_chain = [
-            tasks.NOPLocalWorkflowTask(ctx)
-            for _ in range(10)
-        ]
-        g.add_task(task1)
-        g.add_task(task2)
-        g.add_task(task3)
-        g.add_task(task4)
-        for nop_task in nops_chain:
-            g.add_task(nop_task)
-        for nop_task, next_nop_task in zip(nops_chain, nops_chain[1:]):
-            g.add_dependency(nop_task, next_nop_task)
-        g.add_dependency(task3, nops_chain[0])
-        g.add_dependency(task4, nops_chain[0])
-        g.add_dependency(nops_chain[-1], task1)
-        g.add_dependency(nops_chain[-1], task2)
-        g.optimize()
-        assert g._dependencies == {
-            task3: set([task1, task2]),
-            task4: set([task1, task2]),
-        }
-        assert g._dependents == {
-            task1: set([task3, task4]),
-            task2: set([task3, task4]),
-        }
 
-    def test_removes_empty_subgraph(self):
-        """optimize removes all kinds of "empty" subgraphs"""
-        ctx = MockWorkflowContext()
-        g = TaskDependencyGraph(ctx)
-
-        # sg1 is just empty, no tasks inside it
-        sg1 = g.subgraph(ctx)
-        # sg2 contains only a NOPTask
-        sg2 = g.subgraph(ctx)
-        sg2.add_task(tasks.NOPLocalWorkflowTask(ctx))
-
-        # sg3 contains sg4, which is empty behcause it only contains a NOPTask
-        sg3 = g.subgraph(ctx)
-        sg4 = g.subgraph(ctx)
-        sg4.add_task(tasks.NOPLocalWorkflowTask(ctx))
-        sg3.add_task(sg4)
-
-        # sg5 is a subgraph that contains a real task! it is not removed
-        sg5 = g.subgraph(ctx)
-        real_task = tasks.WorkflowTask(ctx)
-        sg5.add_task(real_task)
-
-        assert set(g.tasks) > {sg1, sg2, sg3, sg4, sg5, real_task}
-        g.optimize()
-        assert set(g.tasks) == {sg5, real_task}
+def _on_failure_handler_fail(task):
+    return tasks.HandlerResult.fail()
```

### Comparing `cloudify-common-6.4.2/cloudify/tests/workflows.py` & `cloudify-common-7.0.0/dsl_parser/elements/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 ########
-# Copyright (c) 2015 GigaSpaces Technologies Ltd. All rights reserved
+# Copyright (c) 2018 Cloudify Platform Ltd. All rights reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-from cloudify.decorators import workflow
+import numbers
 
-
-@workflow
-def execute_operation(ctx, operation, testing, nodes, **_):
-    for node_id in nodes:
-        node = ctx.get_node(node_id)
-        instance = next(node.instances)
-        instance.execute_operation(operation, kwargs={'testing': testing})
+PRIMITIVE_TYPES = (list, bool, numbers.Number, str, dict)
```

### Comparing `cloudify-common-6.4.2/cloudify/utils.py` & `cloudify-common-7.0.0/cloudify/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,37 +30,63 @@
 import traceback
 import threading
 import subprocess
 
 from datetime import datetime, timedelta
 from contextlib import contextmanager, closing
 from functools import wraps
+from io import StringIO
 from requests.exceptions import ConnectionError, Timeout
 import socket   # replace with ipaddress when this is py3-only
 
 
 from dsl_parser.constants import PLUGIN_INSTALL_KEY, PLUGIN_NAME_KEY
 
 from cloudify import constants
 from cloudify.state import workflow_parameters, workflow_ctx, ctx, current_ctx
-from cloudify._compat import StringIO, parse_version
-from cloudify._compat import uuid4  # NOQA - import just to re-export here
 from cloudify.constants import (SUPPORTED_ARCHIVE_TYPES,
                                 KEEP_TRYING_HTTP_TOTAL_TIMEOUT_SEC,
                                 MAX_WAIT_BETWEEN_HTTP_RETRIES_SEC)
 from cloudify.exceptions import CommandExecutionException, NonRecoverableError
 
+try:
+    from packaging.version import parse as parse_version
+except ImportError:
+    from distutils.version import LooseVersion as parse_version
+
+
 ENV_CFY_EXEC_TEMPDIR = 'CFY_EXEC_TEMP'
 ENV_AGENT_LOG_LEVEL = 'AGENT_LOG_LEVEL'
 ENV_AGENT_LOG_DIR = 'AGENT_LOG_DIR'
 ENV_AGENT_LOG_MAX_BYTES = 'AGENT_LOG_MAX_BYTES'
 ENV_AGENT_LOG_MAX_HISTORY = 'AGENT_LOG_MAX_HISTORY'
 
 ADMIN_API_TOKEN_PATH = '/opt/mgmtworker/work/admin_token'
 
+try:
+    from contextlib import nullcontext
+except ImportError:
+    # python 3.6 doesn't have nullcontext, so let's pretty much copy over
+    # 3.7+'s implementation'
+    class nullcontext:
+        def __init__(self, enter_result=None):
+            self.enter_result = enter_result
+
+        def __enter__(self):
+            return self.enter_result
+
+        def __exit__(self, *excinfo):
+            pass
+
+        async def __aenter__(self):
+            return self.enter_result
+
+        async def __aexit__(self, *excinfo):
+            pass
+
 
 class ManagerVersion(object):
     """Cloudify manager version helper class."""
 
     def __init__(self, raw_version):
         """Raw version, for example: 3.4.0-m1, 3.3, 3.2.1, 3.3-rc1."""
 
@@ -189,18 +215,19 @@
     Available only on mgmtworkers, returns the hostname of the manager
     this is running on.
     """
     return os.environ.get(constants.MANAGER_NAME)
 
 
 def get_manager_file_server_scheme():
-    """
-    Returns the manager file server base url.
-    """
-    return os.environ.get(constants.MANAGER_FILE_SERVER_SCHEME, 'https')
+    """Returns the protocol to use for connecting to the fileserver"""
+    return os.environ.get(
+        constants.MANAGER_FILE_SERVER_SCHEME,
+        get_manager_rest_service_protocol(),
+    )
 
 
 def get_manager_file_server_url():
     """
     Returns the manager file server base url.
     """
     port = get_manager_rest_service_port()
@@ -214,47 +241,57 @@
 def get_manager_file_server_root():
     """
     Returns the host the manager REST service is running on.
     """
     return os.environ[constants.MANAGER_FILE_SERVER_ROOT_KEY]
 
 
+def get_manager_rest_service_protocol():
+    return os.environ.get(
+        constants.REST_PROTOCOL_KEY,
+        constants.SECURED_PROTOCOL,
+    )
+
+
 def get_manager_rest_service_host():
     """
     Returns the host the manager REST service is running on.
     """
-    host_ip = None
+    if os.environ.get(constants.REST_HOST_KEY):
+        return os.environ[constants.REST_HOST_KEY].split(',')
     try:
         # Context could be not available sometimes
-        host_ip = _get_current_context().rest_host
+        return _get_current_context().rest_host
+    except RuntimeError:
+        pass
+
+
+def get_manager_rest_service_port():
+    """
+    Returns the port the manager REST service is running on.
+    """
+    if os.environ.get(constants.REST_PORT_KEY):
+        return int(os.environ[constants.REST_PORT_KEY])
+    try:
+        return _get_current_context().rest_port
     except RuntimeError:
         pass
-    # In case host_ip was None or a RuntimeError raise, then fallback from
-    # environment variable
-    return host_ip or os.environ[constants.REST_HOST_KEY].split(',')
 
 
 def get_broker_ssl_cert_path():
     """
     Returns location of the broker certificate on the agent
     """
     return os.environ[constants.BROKER_SSL_CERT_PATH]
 
 
 # maintained for backwards compatibility
 get_manager_ip = get_manager_rest_service_host
 
 
-def get_manager_rest_service_port():
-    """
-    Returns the port the manager REST service is running on.
-    """
-    return int(os.environ[constants.REST_PORT_KEY])
-
-
 def get_local_rest_certificate():
     """
     Returns the path to the local copy of the server's public certificate
     """
     ssl_cert_path = os.path.join(
         os.path.dirname(os.environ[constants.LOCAL_REST_CERT_FILE_KEY]),
         'tmp_cloudify_internal_cert.pem'
@@ -427,18 +464,21 @@
     """Get workflow parameters (except `ctx` key) as a dict."""
     p = workflow_parameters.copy()
     if 'ctx' in p:
         del p['ctx']
     return p
 
 
+def get_local_resources_root():
+    return os.environ.get(constants.LOCAL_RESOURCES_ROOT_ENV_KEY)
+
+
 class LocalCommandRunner(object):
 
     def __init__(self, logger=None, host='localhost'):
-
         """
         :param logger: This logger will be used for
                        printing the output and the command.
         """
 
         logger = logger or setup_logger('LocalCommandRunner')
         self.logger = logger
@@ -447,15 +487,14 @@
     def run(self, command,
             exit_on_failure=True,
             stdout_pipe=True,
             stderr_pipe=True,
             cwd=None,
             execution_env=None,
             encoding='utf-8'):
-
         """
         Runs local commands.
 
         :param command: The command to execute.
         :param exit_on_failure: False to ignore failures.
         :param stdout_pipe: False to not pipe the standard output.
         :param stderr_pipe: False to not pipe the standard error.
@@ -646,16 +685,21 @@
         system_random.choice(allowed_characters)
         for _ in range(password_length)
     )
     return password
 
 
 def get_admin_api_token():
-    with open(ADMIN_API_TOKEN_PATH, 'r') as token_file:
-        token = token_file.read()
+    token = os.environ.get(constants.ADMIN_API_TOKEN_KEY)
+
+    if not token:
+        with open(ADMIN_API_TOKEN_PATH, 'r') as token_file:
+            token = token_file.read()
+            token = token.strip()
+
     return token
 
 
 internal = Internal()
 
 
 def extract_plugins_to_install(plugin_list, filter_func):
@@ -1031,14 +1075,39 @@
 def ipv6_url_compat(addr):
     """Return URL-compatible version of IPv6 address (or just an address)."""
     if _is_ipv6(addr):
         return '[{0}]'.format(addr)
     return addr
 
 
+def uuid4():
+    """Generate a random UUID, and return a string representation of it.
+
+    This is pretty much a copy of the stdlib uuid4. We inline it here,
+    because we'd like to avoid importing the stdlib uuid module on the
+    operation dispatch critical path, because importing the stdlib
+    uuid module runs some subprocesses (for detecting the uuid1-uuid3 MAC
+    address), and that causes more memory pressure than we'd like.
+    """
+    uuid_bytes = os.urandom(16)
+    uuid_as_int = int.from_bytes(uuid_bytes, byteorder='big')
+    uuid_as_int &= ~(0xc000 << 48)
+    uuid_as_int |= 0x8000 << 48
+    uuid_as_int &= ~(0xf000 << 64)
+    uuid_as_int |= 4 << 76
+    uuid_as_hex = '%032x' % uuid_as_int
+    return '%s-%s-%s-%s-%s' % (
+        uuid_as_hex[:8],
+        uuid_as_hex[8:12],
+        uuid_as_hex[12:16],
+        uuid_as_hex[16:20],
+        uuid_as_hex[20:]
+    )
+
+
 def keep_trying_http(total_timeout_sec=KEEP_TRYING_HTTP_TOTAL_TIMEOUT_SEC,
                      max_delay_sec=MAX_WAIT_BETWEEN_HTTP_RETRIES_SEC):
     """
     Keep (re)trying HTTP requests.
 
     This is a wrapper function that will keep (re)running whatever function it
     wraps until it raises a "non-repairable" exception (where "repairable"
@@ -1064,28 +1133,22 @@
             timeout_at = None if total_timeout_sec is None \
                 else datetime.utcnow() + timedelta(seconds=total_timeout_sec)
             while True:
                 try:
                     return func(*args, **kwargs)
                 except (ConnectionError, Timeout) as ex:
                     if timeout_at and datetime.utcnow() > timeout_at:
-                        logger.error(
-                            'Finished retrying {0}: total timeout of {1} '
-                            'seconds exceeded: {2}'
-                            .format(func, total_timeout_sec, ex_to_str(ex))
-                        )
+                        logger.error(f'Finished retrying {func}: '
+                                     f'total timeout of {total_timeout_sec} '
+                                     f'seconds exceeded: {ex_to_str(ex)}')
                         raise
                     delay = random.randint(0, max_delay_sec)
-                    logger.warning(
-                        'Will retry {0} in {1} seconds: {2}'
-                        .format(func, delay, ex_to_str(ex))
-                    )
+                    logger.warning(f'Will retry {func} in {delay} seconds: ' +
+                                   ex_to_str(ex))
                     time.sleep(delay)
                 except Exception as ex:
-                    logger.error(
-                        'Will not retry {0}: the encountered error cannot '
-                        'be fixed by retrying: {1}'
-                        .format(func, ex_to_str(ex))
-                    )
+                    logger.error(f'Will not retry {func}: the encountered '
+                                 'error cannot be fixed by retrying: ' +
+                                 ex_to_str(ex))
                     raise
         return wrapper
     return inner
```

### Comparing `cloudify-common-6.4.2/cloudify/workflows/__init__.py` & `cloudify-common-7.0.0/cloudify/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/workflows/amqp_dispatcher.py` & `cloudify-common-7.0.0/cloudify/workflows/amqp_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/workflows/events.py` & `cloudify-common-7.0.0/cloudify/workflows/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/workflows/local.py` & `cloudify-common-7.0.0/cloudify/workflows/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,31 @@
 import tempfile
 import copy
 import importlib
 import shutil
 import json
 import time
 import threading
-import sys
 import weakref
 
+from abc import ABC
 from datetime import datetime
 from contextlib import contextmanager
+from io import StringIO
 
 from cloudify_rest_client.nodes import Node
 from cloudify_rest_client.blueprints import Blueprint
 from cloudify_rest_client.deployments import Deployment
 from cloudify_rest_client.executions import Execution
 from cloudify_rest_client.node_instances import NodeInstance
 from cloudify_rest_client.deployment_updates import DeploymentUpdate
 
-from cloudify._compat import StringIO, ABC
 from cloudify import dispatch, utils
 from cloudify.workflows.workflow_context import (
     DEFAULT_LOCAL_TASK_THREAD_POOL_SIZE)
-from cloudify._compat import reraise, text_type
 
 try:
     from dsl_parser.constants import HOST_TYPE
     from dsl_parser import parser as dsl_parser, tasks as dsl_tasks
     from dsl_parser import functions as dsl_functions
     _import_error = None
 except ImportError as e:
@@ -117,15 +116,15 @@
         try:
             rv = dispatch.dispatch(__cloudify_context=ctx,
                                    **merged_parameters)
             self.storage.execution_ended(execution_id)
             return rv
         except Exception as e:
             self.storage.execution_ended(execution_id, e)
-            reraise(e.__class__, e, sys.exc_info()[2])
+            raise
 
 
 def init_env(blueprint_path,
              name='local',
              inputs=None,
              storage=None,
              ignored_modules=None,
@@ -243,15 +242,15 @@
         raise AttributeError("mapping error: {0} has no attribute '{1}' "
                              "[node={2}, type={3}]"
                              .format(module.__name__, method_name,
                                      node_name, tpe))
 
 
 def _try_convert_from_str(string, target_type):
-    if target_type == text_type:
+    if target_type == str:
         return string
     if target_type == bool:
         if string.lower() == 'true':
             return True
         if string.lower() == 'false':
             return False
         return string
@@ -270,25 +269,25 @@
     execution_parameters = execution_parameters or {}
 
     missing_mandatory_parameters = set()
 
     allowed_types = {
         'integer': int,
         'float': float,
-        'string': (text_type, bytes),
+        'string': (str, bytes),
         'boolean': bool
     }
     wrong_types = {}
 
     for name, param in workflow_parameters.items():
 
         if 'type' in param and name in execution_parameters:
 
             # check if need to convert from string
-            if (isinstance(execution_parameters[name], (text_type, bytes)) and
+            if (isinstance(execution_parameters[name], (str, bytes)) and
                     param['type'] in allowed_types and
                     param['type'] != 'string'):
                 execution_parameters[name] = \
                     _try_convert_from_str(
                         execution_parameters[name],
                         allowed_types[param['type']])
 
@@ -408,21 +407,16 @@
                              relationships=None,
                              force=False):
         with self._lock(node_instance_id):
             instance = self.get_node_instance(node_instance_id)
             instance_version = instance.get('version', 0)
             if not force and state is None and version != instance_version:
                 raise StorageConflictError(
-                    'version {version} does not match current version of node'
-                    'instance {node_instance_id} which is {instance_version}'
-                    .format(
-                        version=version,
-                        node_instance_id=node_instance_id,
-                        instance_version=instance_version,
-                    )
+                    f'version {version} does not match current version of node'
+                    f'instance {node_instance_id} which is {instance_version}'
                 )
             else:
                 instance['version'] = instance_version + 1
             if runtime_properties is not None:
                 instance['runtime_properties'] = runtime_properties
             if system_properties is not None:
                 instance['system_properties'] = system_properties
```

### Comparing `cloudify-common-6.4.2/cloudify/workflows/tasks.py` & `cloudify-common-7.0.0/cloudify/workflows/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-import functools
 import time
 import threading
 import types
+from functools import lru_cache, wraps
 
 from cloudify import exceptions, logs
 from cloudify.workflows import api
 from cloudify.manager import (
     get_rest_client,
     get_node_instance,
     update_execution_status,
@@ -34,28 +34,18 @@
     TASK_RESCHEDULED,
     TASK_SUCCEEDED,
     TASK_FAILED,
     TERMINATED_STATES,
 )
 from cloudify.state import workflow_ctx, current_workflow_ctx
 from cloudify.utils import get_func, uuid4
+from cloudify.error_handling import serialize_known_exception
 # imported for backwards compat:
 from cloudify.constants import TASK_RESPONSE_SENT, INSPECT_TIMEOUT  # noqa
 
-try:
-    from functools import lru_cache
-except ImportError:
-    # py2.7 doesn't have lru_cache, but this is only used mgmtworker-side,
-    # on py3 only. Still, this module needs to be importable. Make a noop
-    # function that still has the same interface.
-    def lru_cache():
-        def _inner(f):
-            return f
-        return _inner
-
 
 INFINITE_TOTAL_RETRIES = -1
 DEFAULT_TOTAL_RETRIES = INFINITE_TOTAL_RETRIES
 DEFAULT_RETRY_INTERVAL = 30
 DEFAULT_SUBGRAPH_TOTAL_RETRIES = 0
 
 DEFAULT_SEND_TASK_EVENTS = True
@@ -65,15 +55,15 @@
 
 def with_execute_after(f):
     """Wrap a task's apply_async to delay it if requested.
 
     If a task has .execute_after set, the apply_async will actually
     only run after that time has passed.
     """
-    @functools.wraps(f)
+    @wraps(f)
     def _inner(*args, **kwargs):
         task = args[0]
         if api.has_cancel_request():
             return task.async_result
         if task.execute_after and task.execute_after > time.time():
             t = threading.Timer(
                 task.execute_after - time.time(),
@@ -136,15 +126,14 @@
         """
         self.id = task_id or uuid4()
         self._state = TASK_PENDING
         self.async_result = WorkflowTaskResult(self)
         self.on_success = on_success
         self.on_failure = on_failure
         self.info = info
-        self.error = None
         self.total_retries = total_retries
         self.retry_interval = retry_interval
         self.timeout = timeout
         self.timeout_recoverable = timeout_recoverable
         self.is_terminated = False
         self.workflow_context = workflow_context
         self.send_task_events = send_task_events
@@ -156,14 +145,19 @@
         # graph during retries
         self.execute_after = None
         self.stored = False
 
         # ID of the task that is being retried by this task
         self.retried_task = None
 
+        # error is a dict as returned by serialize_known_exception:
+        # for remote tasks it is set when the AMQP dispatcher receives a
+        # task error response
+        self.error = None
+
         # this is set when a dependency errors out. Then, this task must not
         # run!
         self.dependency_error = False
 
     @classmethod
     def restore(cls, ctx, graph, task_descr):
         params = task_descr.parameters
@@ -518,14 +512,15 @@
                 self, self._task_target)
             if should_send:
                 self.set_state(TASK_SENT)
                 self.workflow_context.internal.handler.send_task(
                     self, self._task_target, self._task_queue)
         except (exceptions.NonRecoverableError,
                 exceptions.RecoverableError) as e:
+            self.error = serialize_known_exception(e)
             self.set_state(TASK_FAILED)
             self.async_result.result = e
         return self.async_result
 
     def is_local(self):
         return False
 
@@ -610,15 +605,18 @@
         else:
             host_node_instance = client.node_instances.get(host_id)
         cloudify_agent = host_node_instance.runtime_properties.get(
             'cloudify_agent', {})
 
         # we found the actual agent, just return it
         if cloudify_agent.get('queue') and cloudify_agent.get('name'):
-            return cloudify_agent, self._get_tenant_dict(tenant, client)
+            return (
+                cloudify_agent,
+                self._get_tenant_dict(host_node_instance, tenant, client)
+            )
 
         # this node instance isn't the real agent, check if it proxies to one.
         # Evaluate functions because proxy info might contain runtime
         # intrinsic functions (get_attributes/get_capabilities)
         node = client.nodes.get(
             deployment_id,
             host_node_instance.node_id,
@@ -629,48 +627,63 @@
             proxy_deployment = remote['deployment']
             proxy_node_instance = remote['node_instance']
             proxy_tenant = remote.get('tenant')
         except KeyError:
             # no queue information and no proxy - cannot continue
             missing = 'queue' if not cloudify_agent.get('queue') else 'name'
             raise exceptions.NonRecoverableError(
-                'Missing cloudify_agent.{0} runtime information. '
+                '{0}: missing cloudify_agent.{1} runtime information. '
                 'This most likely means that the Compute node was '
-                'never started successfully'.format(missing))
+                'never started successfully'
+                .format(host_node_instance.id, missing)
+            )
         else:
             # the agent does proxy to another, recursively get from that one
             # (if the proxied-to agent in turn proxies to yet another one,
             # look up that one, etc)
             return self._get_agent_settings(
                 node_instance_id=proxy_node_instance,
                 deployment_id=proxy_deployment,
                 tenant=proxy_tenant)
 
-    def _get_tenant_dict(self, tenant_name, client):
+    def _get_tenant_dict(self, node_instance, tenant_name, client):
         if tenant_name is None or \
                 tenant_name == self.cloudify_context['tenant']['name']:
             return self.cloudify_context['tenant']
         tenant = client.tenants.get(tenant_name)
         if tenant.get('rabbitmq_vhost') is None:
             raise exceptions.NonRecoverableError(
-                'Could not get RabbitMQ credentials for tenant {0}'
-                .format(tenant_name))
+                '{0}: could not get RabbitMQ credentials for tenant {1}'
+                .format(node_instance.id, tenant_name)
+            )
         return tenant
 
     def _get_queue_kwargs(self):
         """Queue, name, and tenant of the agent that will execute the task
 
         This must return the values of the actual agent, possibly
         one that is available via deployment proxying.
         """
         executor = self.cloudify_context['executor']
+        node_instance_id = self.cloudify_context['node_id']
+
+        if executor == 'auto':
+            # for executor=auto, we'll be a host_agent script if we do have
+            # a host, otherwise CDA
+            client = get_rest_client()
+            node_instance = client.node_instances.get(node_instance_id)
+            if node_instance.host_id:
+                executor = 'host_agent'
+            else:
+                executor = 'central_deployment_agent'
+
         if executor == 'host_agent':
             if self._cloudify_agent is None:
                 self._cloudify_agent, tenant = self._get_agent_settings(
-                    node_instance_id=self.cloudify_context['node_id'],
+                    node_instance_id=node_instance_id,
                     deployment_id=self.cloudify_context['deployment_id'],
                     tenant=None)
             return (self._cloudify_agent['queue'],
                     self._cloudify_agent['name'],
                     tenant,
                     self._cloudify_agent['rest_host'])
         else:
@@ -813,15 +826,18 @@
     @with_execute_after
     def apply_async(self):
         self.set_state(TASK_SUCCEEDED)
         self.async_result.result = None
         return self.async_result
 
     def is_nop(self):
-        return True
+        # If a nop has a success/failure handler, then it's not really
+        # a nop, because it does _do_ something, and can't be just dropped
+        # from the graph
+        return self.on_success is None and self.on_failure is None
 
     def is_local(self):
         return True
 
 
 class DryRunLocalWorkflowTask(LocalWorkflowTask):
     def apply_async(self):
```

### Comparing `cloudify-common-6.4.2/cloudify/workflows/workflow_api.py` & `cloudify-common-7.0.0/cloudify/workflows/workflow_api.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify/workflows/workflow_context.py` & `cloudify-common-7.0.0/cloudify/workflows/workflow_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 """
 
 from __future__ import absolute_import
 
 import functools
 import copy
 import json
+import queue
 import threading
 
 from dsl_parser import functions as dsl_functions
 from dsl_parser.utils import parse_simple_type_value
 
 
 from cloudify import context
-from cloudify._compat import queue
 from cloudify.manager import (get_bootstrap_context,
                               get_rest_client,
                               download_resource)
 from cloudify.workflows.tasks import (RemoteWorkflowTask,
                                       LocalWorkflowTask,
                                       NOPLocalWorkflowTask,
                                       DryRunLocalWorkflowTask,
@@ -53,18 +53,16 @@
 
 from cloudify import utils, logs
 from cloudify.state import current_workflow_ctx
 from cloudify.workflows import events
 from cloudify.workflows.tasks_graph import TaskDependencyGraph
 from cloudify.logs import (CloudifyWorkflowLoggingHandler,
                            CloudifyWorkflowNodeLoggingHandler,
-                           SystemWideWorkflowLoggingHandler,
                            init_cloudify_logger,
-                           send_workflow_event,
-                           send_sys_wide_wf_event)
+                           send_workflow_event)
 from cloudify.models_states import DeploymentModificationState
 
 
 try:
     from collections import OrderedDict
 except ImportError:
     from ordereddict import OrderedDict
@@ -374,14 +372,18 @@
         return self._node_instance.get('modification')
 
     @property
     def scaling_groups(self):
         return self._node_instance.get('scaling_groups', [])
 
     @property
+    def deployment_id(self):
+        return self._node_instance.get('deployment_id')
+
+    @property
     def runtime_properties(self):
         """The node instance runtime properties
 
         Note that in workflow code, it is common for runtime-properties
         to be outdated, if a prior operation changed them.
         Before using this value, consider if it is up to date. You can
         use the refresh_node_instances method to bring all node-instance
@@ -494,14 +496,19 @@
         return self.ctx.get_node(self.host_id)
 
     @property
     def number_of_instances(self):
         return self._node.number_of_instances
 
     @property
+    def planned_number_of_instances(self):
+        """Current planned amount of instances of this node"""
+        return self._node.planned_number_of_instances
+
+    @property
     def relationships(self):
         """The node relationships"""
         return iter(self._relationships.values())
 
     @property
     def operations(self):
         """The node operations"""
@@ -589,14 +596,18 @@
         return self._context.get('rest_token')
 
     @property
     def rest_host(self):
         return self._context.get('rest_host')
 
     @property
+    def rest_port(self):
+        return self._context.get('rest_port')
+
+    @property
     def execution_token(self):
         """The token of the current execution"""
         return self._context.get('execution_token')
 
     @property
     def bypass_maintenance(self):
         """If true, all requests sent bypass maintenance mode."""
@@ -703,25 +714,30 @@
             total_retries = self.internal.get_task_configuration()[
                 'total_retries']
         else:
             total_retries = operation_total_retries
 
         if plugin and plugin['package_name']:
             plugin = self.internal.handler.get_plugin(plugin)
+            plugin_properties = self.internal.handler.get_plugin_properties(
+                node_instance.deployment_id if node_instance else None, plugin)
+        else:
+            plugin_properties = {}
 
         node_context = {
             'node_id': node_instance.id,
             'node_name': node_instance.node_id,
             'plugin': {
                 'name': plugin_name,
                 'package_name': plugin.get('package_name'),
                 'package_version': plugin.get('package_version'),
                 'visibility': plugin.get('visibility'),
                 'tenant_name': plugin.get('tenant_name'),
-                'source': plugin.get('source')
+                'source': plugin.get('source'),
+                'properties': plugin_properties,
             },
             'operation': {
                 'name': operation,
                 'retry_number': 0,
                 'max_retries': total_retries
             },
             'has_intrinsic_functions': has_intrinsic_functions,
@@ -1203,22 +1219,14 @@
         return self._nodes_and_instances.get_node_instance(*args, **kwargs)
 
     def refresh_node_instances(self, *args, **kwargs):
         return self._nodes_and_instances.refresh_node_instances(
             *args, **kwargs)
 
 
-class CloudifySystemWideWorkflowContext(_WorkflowContextBase):
-    def __init__(self, ctx):
-        super(CloudifySystemWideWorkflowContext, self).__init__(
-            ctx,
-            SystemWideWfRemoteContextHandler
-        )
-
-
 class CloudifyWorkflowContextInternal(object):
 
     def __init__(self, workflow_context, handler):
         self.workflow_context = workflow_context
         self.handler = handler
         self._bootstrap_context = None
         self._graph_mode = False
@@ -1419,14 +1427,27 @@
 
     def get_node_instances(self):
         raise NotImplementedError('Implemented by subclasses')
 
     def get_plugin(self, plugin_spec):
         raise NotImplementedError('Implemented by subclasses')
 
+    def get_plugin_properties(self, deployment_id, plugin_spec):
+        raise NotImplementedError('Implemented by subclasses')
+
+    def evaluate_plugin_properties(self, deployment_id, plugin_properties):
+        payload = {k: v['value'] for k, v in plugin_properties.items()
+                   if isinstance(v, dict) and 'value' in v}
+        evaluated = self.evaluate_functions(deployment_id, {}, payload)
+        if not evaluated:
+            return plugin_properties
+        for k, v in evaluated.items():
+            plugin_properties[k]['value'] = v
+        return plugin_properties
+
     def update_node_instance(
         self,
         node_instance_id,
         version,
         state=None,
         runtime_properties=None,
         system_properties=None,
@@ -1538,21 +1559,25 @@
     def wait_for_result(self, *args, **kwargs):
         if self._dispatcher is None:
             self._prepare_dispatcher()
         return self._dispatcher.wait_for_result(*args, **kwargs)
 
     @property
     def operation_cloudify_context(self):
-        return {'local': False,
-                'bypass_maintenance': utils.get_is_bypass_maintenance(),
-                'rest_token': utils.get_rest_token(),
-                'workflow_parameters': utils.get_workflow_parameters(),
-                'execution_token': utils.get_execution_token(),
-                'execution_creator_username':
-                    utils.get_execution_creator_username()}
+        return {
+            'local': False,
+            'rest_token': self.workflow_ctx.rest_token,
+            'rest_host': self.workflow_ctx.rest_host,
+            'rest_port': self.workflow_ctx.rest_port,
+            'bypass_maintenance': utils.get_is_bypass_maintenance(),
+            'workflow_parameters': utils.get_workflow_parameters(),
+            'execution_token': utils.get_execution_token(),
+            'execution_creator_username':
+            utils.get_execution_creator_username()
+        }
 
     def download_deployment_resource(self,
                                      blueprint_id,
                                      deployment_id,
                                      tenant_name,
                                      resource_path,
                                      target_path=None):
@@ -1648,25 +1673,51 @@
         dep = self.workflow_ctx.deployment
         return self.rest_client.node_instances.list(
             deployment_id=dep.id,
             _get_all_results=True,
         )
 
     def get_plugin(self, plugin):
-        key = (plugin.get('package_name'), plugin.get('package_version'))
+        key = (
+            plugin.get('name'),
+            plugin.get('package_name'),
+            plugin.get('package_version'),
+        )
         if key not in self._plugins_cache:
             filter_plugin = {'package_name': plugin.get('package_name'),
                              'package_version': plugin.get('package_version')}
             managed_plugins = self.rest_client.plugins.list(**filter_plugin)
             if managed_plugins:
                 plugin['visibility'] = managed_plugins[0]['visibility']
                 plugin['tenant_name'] = managed_plugins[0]['tenant_name']
             self._plugins_cache[key] = plugin
         return self._plugins_cache[key]
 
+    def get_plugin_properties(self, deployment_id, plugin_spec):
+        if not deployment_id:
+            return {}
+        plugins = self._get_matching_plugins(deployment_id, plugin_spec)
+        if not plugins:
+            return {}
+        return self.evaluate_plugin_properties(
+            deployment_id, plugins[0].get('properties', {}))
+
+    def _get_matching_plugins(self, deployment_id, plugin):
+        dep = self.rest_client.deployments.get(deployment_id)
+        bp = self.rest_client.blueprints.get(dep.blueprint_id)
+        return [
+            p for p in
+            bp.plan['deployment_plugins_to_install'] +
+            bp.plan['workflow_plugins_to_install'] +
+            bp.plan['host_agent_plugins_to_install']
+            if p.get('name') == plugin.get('name')
+            and p.get('package_name') == plugin.get('package_name')
+            and p.get('package_version') == plugin.get('package_version')
+        ]
+
     def update_node_instance(self, *args, **kwargs):
         return self.rest_client.node_instances.update(*args, **kwargs)
 
     def set_deployment_attributes(self, deployment_id, **kwargs):
         self.rest_client.deployments.set_attributes(deployment_id, **kwargs)
 
     def get_deployment_update(self, update_id):
@@ -1803,30 +1854,14 @@
             deployment_id = self.workflow_ctx.deployment.id
             deployment = self.rest_client.deployments.get(
                 deployment_id, _include=['scaling_groups'])
             self._scaling_groups = deployment['scaling_groups']
         return self._scaling_groups
 
 
-class SystemWideWfRemoteContextHandler(RemoteContextHandler):
-
-    def get_context_logging_handler(self):
-        return SystemWideWorkflowLoggingHandler(self.workflow_ctx,
-                                                out_func=logs.manager_log_out)
-
-    def send_workflow_event(self, event_type, message=None, args=None,
-                            additional_context=None):
-        send_sys_wide_wf_event(self.workflow_ctx,
-                               event_type=event_type,
-                               message=message,
-                               args=args,
-                               additional_context=additional_context,
-                               out_func=logs.manager_event_out)
-
-
 class LocalCloudifyWorkflowContextHandler(CloudifyWorkflowContextHandler):
 
     def __init__(self, workflow_ctx, storage):
         super(LocalCloudifyWorkflowContextHandler, self).__init__(
             workflow_ctx)
         self.storage = storage
         self._send_task_event_func = None
@@ -1899,14 +1934,36 @@
 
     def get_node_instances(self):
         return self.storage.get_node_instances()
 
     def get_plugin(self, plugin):
         return plugin
 
+    def get_plugin_properties(self, deployment_id, plugin_spec):
+        if not deployment_id:
+            return {}
+        dep = self.storage.get_deployment(deployment_id)
+        if not dep.blueprint_id:
+            return {}
+        bp = self.storage.get_blueprint(dep.blueprint_id)
+        if not bp.plan:
+            return {}
+        plugins = [
+            p for p in
+            bp.plan['deployment_plugins_to_install'] +
+            bp.plan['workflow_plugins_to_install'] +
+            bp.plan['host_agent_plugins_to_install']
+            if p.get('package_name') == plugin_spec.get('package_name')
+            and p.get('package_version') == plugin_spec.get('package_version')
+        ]
+        if not plugins or 'properties' not in plugins[0]:
+            return {}
+        return self.evaluate_plugin_properties(
+            deployment_id, plugins[0].get('properties', {}))
+
     def update_node_instance(self, *args, **kwargs):
         return self.storage.update_node_instance(*args, **kwargs)
 
     def set_deployment_attributes(self, deployment_id, **kwargs):
         if 'workflows' in kwargs:
             workflows = []
             for name, wf in kwargs['workflows'].items():
```

### Comparing `cloudify-common-6.4.2/cloudify/zip_utils.py` & `cloudify-common-7.0.0/cloudify/zip_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_async_client/audit_log.py` & `cloudify-common-7.0.0/cloudify_async_client/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_async_client/client.py` & `cloudify-common-7.0.0/cloudify_async_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_common.egg-info/SOURCES.txt` & `cloudify-common-7.0.0/cloudify_common.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 cloudify/__init__.py
-cloudify/_compat.py
 cloudify/agent_utils.py
 cloudify/amqp_client.py
 cloudify/cluster.py
 cloudify/cluster_status.py
 cloudify/conflict_handlers.py
 cloudify/constants.py
 cloudify/context.py
@@ -43,40 +42,14 @@
 cloudify/snmp/CLOUDIFY-MIB.mib
 cloudify/snmp/__init__.py
 cloudify/snmp/snmp_trap.py
 cloudify/test_utils/__init__.py
 cloudify/test_utils/dispatch_helper.py
 cloudify/test_utils/local_workflow_decorator.py
 cloudify/test_utils/mock_rest_client.py
-cloudify/tests/__init__.py
-cloudify/tests/test_builtin_workflows.py
-cloudify/tests/test_context.py
-cloudify/tests/test_ctx_relationships.py
-cloudify/tests/test_decorators.py
-cloudify/tests/test_dispatch.py
-cloudify/tests/test_event.py
-cloudify/tests/test_install_agent_local_workflow.py
-cloudify/tests/test_install_new_agents_workflow.py
-cloudify/tests/test_keep_trying_http.py
-cloudify/tests/test_lifecycle_retry.py
-cloudify/tests/test_local_get_attribute.py
-cloudify/tests/test_local_workflows.py
-cloudify/tests/test_local_workflows_init.py
-cloudify/tests/test_logs.py
-cloudify/tests/test_node_state.py
-cloudify/tests/test_operation_retry.py
-cloudify/tests/test_proxy.py
-cloudify/tests/test_state.py
-cloudify/tests/test_task_retry.py
-cloudify/tests/test_task_retry_event_context.py
-cloudify/tests/test_task_serialize.py
-cloudify/tests/test_task_subgraph.py
-cloudify/tests/test_tasks_graph.py
-cloudify/tests/test_utils.py
-cloudify/tests/workflows.py
 cloudify/workflows/__init__.py
 cloudify/workflows/amqp_dispatcher.py
 cloudify/workflows/events.py
 cloudify/workflows/local.py
 cloudify/workflows/tasks.py
 cloudify/workflows/tasks_graph.py
 cloudify/workflows/workflow_api.py
@@ -88,21 +61,22 @@
 cloudify_common.egg-info/SOURCES.txt
 cloudify_common.egg-info/dependency_links.txt
 cloudify_common.egg-info/entry_points.txt
 cloudify_common.egg-info/not-zip-safe
 cloudify_common.egg-info/requires.txt
 cloudify_common.egg-info/top_level.txt
 cloudify_rest_client/__init__.py
-cloudify_rest_client/_compat.py
+cloudify_rest_client/_datetime_compat.py
 cloudify_rest_client/agents.py
 cloudify_rest_client/audit_log.py
 cloudify_rest_client/blueprints.py
 cloudify_rest_client/bytes_stream_utils.py
 cloudify_rest_client/client.py
 cloudify_rest_client/cluster.py
+cloudify_rest_client/community_contacts.py
 cloudify_rest_client/constants.py
 cloudify_rest_client/deployment_modifications.py
 cloudify_rest_client/deployment_updates.py
 cloudify_rest_client/deployments.py
 cloudify_rest_client/evaluate.py
 cloudify_rest_client/events.py
 cloudify_rest_client/exceptions.py
@@ -119,32 +93,29 @@
 cloudify_rest_client/manager.py
 cloudify_rest_client/node_instances.py
 cloudify_rest_client/nodes.py
 cloudify_rest_client/operations.py
 cloudify_rest_client/permissions.py
 cloudify_rest_client/plugins.py
 cloudify_rest_client/plugins_update.py
+cloudify_rest_client/resources.py
 cloudify_rest_client/responses.py
 cloudify_rest_client/secrets.py
+cloudify_rest_client/secrets_providers.py
 cloudify_rest_client/sites.py
 cloudify_rest_client/snapshots.py
 cloudify_rest_client/summary.py
 cloudify_rest_client/tenants.py
 cloudify_rest_client/tokens.py
 cloudify_rest_client/user_groups.py
 cloudify_rest_client/users.py
 cloudify_rest_client/utils.py
 cloudify_rest_client/workflows.py
-cloudify_rest_client/tests/__init__.py
-cloudify_rest_client/tests/test_authentication_headers.py
-cloudify_rest_client/tests/test_responses.py
-cloudify_rest_client/tests/test_tokens.py
 ctx_wrappers/ctx-sh
 dsl_parser/__init__.py
-dsl_parser/_compat.py
 dsl_parser/constants.py
 dsl_parser/constraints.py
 dsl_parser/exceptions.py
 dsl_parser/functions.py
 dsl_parser/holder.py
 dsl_parser/models.py
 dsl_parser/multi_instance.py
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/__init__.py` & `cloudify-common-7.0.0/cloudify_rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/agents.py` & `cloudify-common-7.0.0/cloudify_rest_client/agents.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,21 +150,14 @@
         :param kwargs: Optional filter fields. For a list of available fields
                see the REST service's models.Agent.fields
         :return: A ListResponse containing the agents' details
         """
         if sort:
             kwargs['_sort'] = '-' + sort if is_descending else sort
 
-        if _include is None:
-            # Default the _include to what was available before, to avoid
-            # defaulting to including credentials, etc
-            _include = ['id', 'host_id', 'ip', 'install_method', 'system',
-                        'version', 'node', 'deployment', 'tenant_name']
-
-        kwargs.setdefault('state', [AgentState.STARTED])
         response = self.api.get('/{self._uri_prefix}'.format(self=self),
                                 _include=_include,
                                 params=kwargs)
         return ListResponse(
             [self._wrapper_cls(item) for item in response['items']],
             response['metadata']
         )
@@ -192,24 +185,33 @@
                 'state': state,
                 'create_rabbitmq_user': create_rabbitmq_user}
         data.update(kwargs)
         response = self.api.put('/{0}/{1}'.format(self._uri_prefix, name),
                                 data=data)
         return self._wrapper_cls(response)
 
-    def update(self, name, state):
-        """Update agent with the provided state.
+    def update(self, name, state=None, **kwargs):
+        """Update agent with the provided settings.
 
         :param name: The name of the agent to update
         :param state: The updated state
+        :param kwargs: Additional agent settings to update, e.g. version
         :return: The updated agent
         """
-        data = {'state': state}
-        response = self.api.patch('/{0}/{1}'.format(self._uri_prefix, name),
-                                  data=data)
+        data = {}
+        # state is kept separate from kwargs, so that old-style (pre-7.0)
+        # invocation with positional args like `.update(name, state)`
+        # still works.
+        if state:
+            data['state'] = state
+        data.update(kwargs)
+        response = self.api.patch(
+            '/{0}/{1}'.format(self._uri_prefix, name),
+            data=data,
+        )
         return self._wrapper_cls(response)
 
     def replace_ca_certs(self,
                          bundle,
                          new_manager_ca_cert,
                          new_broker_ca_cert):
         """Replace the agents' CA certs
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/audit_log.py` & `cloudify-common-7.0.0/cloudify_rest_client/audit_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cloudify_rest_client.responses import DeletedResponse, ListResponse
 
 
 class AuditLog(dict):
     """AuditLog describes a single entry in the `audit_log` table.  The table
     is used to to log `operation`s ('create', 'update', 'delete') performed on
-    most of the database tables.  Fields `ref_table` and `ref_id` are used to
-    address referenced records."""
+    most of the database tables.  Fields `ref_table`,`ref_id` and
+    `ref_identifier` are used to address referenced records."""
 
     def __init__(self, audit_log):
         super(AuditLog, self).__init__()
         self.update(audit_log)
 
     @property
     def ref_table(self):
@@ -18,14 +18,19 @@
 
     @property
     def ref_id(self):
         """Row ID in the referenced table."""
         return self['ref_id']
 
     @property
+    def ref_identifier(self):
+        """Row identifier in the referenced table."""
+        return self['ref_identifier']
+
+    @property
     def operation(self):
         """Operation performed on the row: 'create', 'update' or 'delete'."""
         return self['operation']
 
     @property
     def creator_name(self):
         """Username of the author of the change (if any)."""
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/blueprints.py` & `cloudify-common-7.0.0/cloudify_rest_client/blueprints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import json
 import os
 import tempfile
 import shutil
 import contextlib
+from urllib.parse import quote as urlquote, urlparse
+
+from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 from cloudify_rest_client import utils
 from cloudify_rest_client import bytes_stream_utils
-from cloudify_rest_client._compat import urlquote, urlparse
 from cloudify_rest_client.constants import VisibilityState
 from cloudify_rest_client.exceptions import CloudifyClientError
-from cloudify_rest_client.executions import Execution
 from cloudify_rest_client.responses import ListResponse
 
 from .labels import Label
 
 
 class Blueprint(dict):
 
@@ -94,127 +96,182 @@
     @property
     def tenant_name(self):
         """
         :return: The name of the tenant associated with this blueprint.
         """
         return self.get('tenant_name')
 
+    @property
+    def requirements(self):
+        """Requirements for creating deployments based on this blueprint.
+
+        If set, this is a dict with key describing various requirements,
+        such as "secrets" or "parent_capabilities". It is up to the caller
+        to interpret them.
+
+        :return: A description of blueprint deploy requirements.
+        """
+        return self.get('requirements')
+
 
 class BlueprintsClient(object):
 
     def __init__(self, api):
         self.api = api
         self._uri_prefix = 'blueprints'
         self._wrapper_cls = Blueprint
 
-    def _prepare_put_request(self,
-                             archive_location,
-                             application_file_name,
-                             visibility,
-                             progress_callback,
-                             async_upload,
-                             labels=None,
-                             created_at=None,
-                             created_by=None,
-                             state=None,
-                             skip_execution=False):
-        query_params = {'visibility': visibility, 'async_upload': async_upload,
-                        'skip_execution': skip_execution}
+    def _prepare_put_request(
+        self,
+        archive_location,
+        application_file_name,
+        visibility,
+        async_upload,
+        labels=None,
+        created_at=None,
+        created_by=None,
+        state=None,
+        skip_execution=False,
+        requirements=None,
+    ):
+        params = {'visibility': visibility, 'async_upload': async_upload,
+                  'skip_execution': skip_execution}
         if application_file_name is not None:
-            query_params['application_file_name'] = \
-                urlquote(application_file_name)
+            params['application_file_name'] = urlquote(application_file_name)
         if labels is not None:
-            labels_params = []
-            for label in labels:
-                if (not isinstance(label, dict)) or len(label) != 1:
-                    raise CloudifyClientError(
+            if any(not isinstance(label, dict) or len(label) > 1
+                   for label in labels):
+                raise CloudifyClientError(
                         'Labels must be a list of 1-entry dictionaries: '
                         '[{<key1>: <value1>}, {<key2>: [<value2>, <value3>]}, '
                         '...]')
-
-                [(key, value)] = label.items()
-                value = value.replace('=', '\\=').replace(',', '\\,')
-                labels_params.append('{0}={1}'.format(key, value))
-            query_params['labels'] = ','.join(labels_params)
+            params['labels'] = [
+                {
+                    'key': list(label.keys())[0],
+                    'value': list(label.values())[0],
+                }
+                for label in labels
+            ]
         if created_at:
-            query_params['created_at'] = created_at
+            params['created_at'] = created_at
         if created_by:
-            query_params['created_by'] = created_by
+            params['created_by'] = created_by
         if state:
-            query_params['state'] = state
+            params['state'] = state
 
         # For a Windows path (e.g. "C:\aaa\bbb.zip") scheme is the
         # drive letter and therefore the 2nd condition is present
         if urlparse(archive_location).scheme and \
                 not os.path.exists(archive_location):
             # archive location is URL
-            query_params['blueprint_archive_url'] = archive_location
-            data = None
+            params['blueprint_archive_url'] = archive_location
+            blueprint_archive = None
         else:
             # archive location is a system path
-            data = bytes_stream_utils.request_data_file_stream(
-                archive_location,
-                progress_callback=progress_callback,
-                client=self.api)
+            blueprint_archive = (
+                'filename',
+                open(archive_location, 'rb'),
+                'text/plain',
+            )
+        if requirements:
+            params['requirements'] = requirements
+
+        data = {
+            'params': json.dumps(params),
+        }
+        if blueprint_archive:
+            data['blueprint_archive'] = blueprint_archive
+
+        return data
+
+    def _upload(
+        self,
+        archive_location,
+        blueprint_id,
+        application_file_name=None,
+        visibility=VisibilityState.TENANT,
+        progress_callback=None,
+        async_upload=False,
+        labels=None,
+        created_at=None,
+        created_by=None,
+        state=None,
+        skip_execution=False,
+        validate=False,
+        legacy=False,
+        requirements=None,
+    ):
+        def callback_wrapper(watcher):
+            if getattr(watcher, 'cfy_progress_complete', False):
+                # Don't print the final line twice
+                return
+            read_bytes, total_bytes = watcher.bytes_read, watcher.len
+            progress_callback(read_bytes, total_bytes)
+            if read_bytes == total_bytes:
+                watcher.cfy_progress_complete = True
 
-        return query_params, data
+        uri = '/{self._uri_prefix}/{id}'.format(self=self, id=blueprint_id)
+        if validate:
+            uri += '/validate'
+            expected_status = [201, 204]
+        else:
+            expected_status = 201
 
-    def _upload(self,
-                archive_location,
-                blueprint_id,
-                application_file_name=None,
-                visibility=VisibilityState.TENANT,
-                progress_callback=None,
-                async_upload=False,
-                labels=None,
-                created_at=None,
-                created_by=None,
-                state=None,
-                skip_execution=False):
-        query_params, data = self._prepare_put_request(
+        params = self._prepare_put_request(
             archive_location,
             application_file_name,
             visibility,
-            progress_callback,
             async_upload,
             labels,
             created_at,
             created_by,
             state,
             skip_execution,
+            requirements,
         )
-        uri = '/{self._uri_prefix}/{id}'.format(self=self, id=blueprint_id)
+
+        if legacy:
+            # Legacy mode is only intended for use with systests, so no
+            # progress callback, sorry!
+            params.pop('blueprint_archive', None)
+            params = json.loads(params.get('params', '{}'))
+            # System tests don't use url based upload
+            data = bytes_stream_utils.request_data_file_stream(
+                archive_location,
+                client=self.api)
+            return self.api.put(
+                uri,
+                params=params,
+                data=data,
+                expected_status_code=expected_status,
+            )
+
+        multipart = MultipartEncoder(fields=params)
+        if progress_callback:
+            multipart = MultipartEncoderMonitor(
+                multipart, callback_wrapper)
         return self.api.put(
             uri,
-            params=query_params,
-            data=data,
-            expected_status_code=201
+            data=multipart,
+            headers={'Content-Type': multipart.content_type},
+            expected_status_code=expected_status,
         )
 
     def _validate(self,
                   archive_location,
                   blueprint_id,
                   application_file_name=None,
                   visibility=VisibilityState.TENANT,
                   progress_callback=None):
-        query_params, data = self._prepare_put_request(
-            archive_location,
-            application_file_name,
-            visibility,
-            progress_callback,
-            async_upload=False,
-        )
-        uri = '/{self._uri_prefix}/{id}/validate'.format(self=self,
-                                                         id=blueprint_id)
-        return self.api.put(
-            uri,
-            params=query_params,
-            data=data,
-            expected_status_code=(200, 204)
-        )
+        return self._upload(archive_location, blueprint_id,
+                            application_file_name=application_file_name,
+                            visibility=visibility,
+                            progress_callback=progress_callback,
+                            async_upload=False,
+                            validate=True)
 
     def _validate_blueprint_size(self, path, tempdir, skip_size_limit):
         blueprint_directory = os.path.dirname(path) or os.getcwd()
         size, files = utils.get_folder_size_and_files(blueprint_directory)
 
         try:
             config = self.api.get('/config', params={'scope': 'rest'})
@@ -282,35 +339,39 @@
             response = self.api.get('/{self._uri_prefix}'.format(self=self),
                                     params=params)
         return ListResponse(
             [self._wrapper_cls(item) for item in response['items']],
             response['metadata']
         )
 
-    def publish_archive(self,
-                        archive_location,
-                        blueprint_id,
-                        blueprint_filename=None,
-                        visibility=VisibilityState.TENANT,
-                        progress_callback=None,
-                        async_upload=False,
-                        labels=None,
-                        created_at=None,
-                        created_by=None,
-                        skip_execution=False):
+    def publish_archive(
+        self,
+        archive_location,
+        blueprint_id,
+        blueprint_filename=None,
+        visibility=VisibilityState.TENANT,
+        progress_callback=None,
+        async_upload=False,
+        labels=None,
+        created_at=None,
+        created_by=None,
+        skip_execution=False,
+        requirements=None,
+    ):
         """Publishes a blueprint archive to the Cloudify manager.
 
         :param archive_location: Path or Url to the archive file.
         :param blueprint_id: Id of the uploaded blueprint.
         :param blueprint_filename: The archive's main blueprint yaml filename.
         :param visibility: The visibility of the blueprint, can be 'private',
                            'tenant' or 'global'.
         :param progress_callback: Progress bar callback method
         :param labels: The blueprint's labels. A list of 1-entry
             dictionaries: [{<key1>: <value1>}, {<key2>: <value2>}, ...]'
+        :requirements: A dict representing the blueprint deploy requirements
         :return: Created blueprint.
 
         Archive file should contain a single directory in which there is a
         blueprint file named `blueprint_filename` (if `blueprint_filename`
         is None, this value will be passed to the REST service where a
         default value should be used).
         Blueprint ID parameter is available for specifying the
@@ -323,52 +384,61 @@
             application_file_name=blueprint_filename,
             visibility=visibility,
             progress_callback=progress_callback,
             async_upload=async_upload,
             labels=labels,
             created_at=created_at,
             created_by=created_by,
-            skip_execution=skip_execution)
+            skip_execution=skip_execution,
+            requirements=requirements,
+        )
         if not async_upload:
             return self._wrapper_cls(response)
 
     @staticmethod
     def calc_size(blueprint_path):
         tempdir = tempfile.mkdtemp()
         try:
             tar_path = utils.tar_blueprint(blueprint_path, tempdir)
             size = os.path.getsize(tar_path)
         finally:
             shutil.rmtree(tempdir)
         return size
 
-    def upload(self,
-               path,
-               entity_id,
-               visibility=VisibilityState.TENANT,
-               progress_callback=None,
-               skip_size_limit=True,
-               async_upload=False,
-               labels=None,
-               created_at=None,
-               created_by=None,
-               state=None,
-               skip_execution=False):
+    def upload(
+        self,
+        path,
+        entity_id,
+        visibility=VisibilityState.TENANT,
+        progress_callback=None,
+        skip_size_limit=True,
+        async_upload=False,
+        labels=None,
+        created_at=None,
+        created_by=None,
+        state=None,
+        skip_execution=False,
+        legacy=False,
+        requirements=None,
+    ):
         """
         Uploads a blueprint to Cloudify's manager.
 
         :param path: Main blueprint yaml file path.
         :param entity_id: Id of the uploaded blueprint.
         :param visibility: The visibility of the blueprint, can be 'private',
                            'tenant' or 'global'.
         :param progress_callback: Progress bar callback method
         :param skip_size_limit: Indicator whether to check size limit on
                            blueprint folder
         :param labels: The blueprint's labels. A list of 1-entry
             dictionaries: [{<key1>: <value1>}, {<key2>: <value2>}, ...]'
+        :param legacy: Support some parameters for upload to older managers.
+                       Internal use only.
+        :requirements: A dict representing the blueprint deploy requirements
         :return: Created response.
 
         Blueprint path should point to the main yaml file of the response
         to be uploaded. Its containing folder will be packed to an archive
         and get uploaded to the manager.
         Blueprint ID parameter is available for specifying the
         response's unique Id.
@@ -385,15 +455,18 @@
                 visibility=visibility,
                 progress_callback=progress_callback,
                 async_upload=async_upload,
                 labels=labels,
                 created_at=created_at,
                 created_by=created_by,
                 state=state,
-                skip_execution=skip_execution)
+                skip_execution=skip_execution,
+                legacy=legacy,
+                requirements=requirements,
+            )
             if not async_upload:
                 return self._wrapper_cls(response)
         finally:
             shutil.rmtree(tempdir)
 
     def validate(self,
                  path,
@@ -435,15 +508,15 @@
                 visibility=visibility,
                 progress_callback=progress_callback)
         finally:
             shutil.rmtree(tempdir)
 
         if response:
             # on cloudify earlier than 6.4, response is None (204 no content)
-            return Execution(response)
+            return response
 
     def get(self, blueprint_id, _include=None):
         """
         Gets a blueprint by its id.
 
         :param blueprint_id: Blueprint's id to get.
         :param _include: List of fields to include in response.
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/bytes_stream_utils.py` & `cloudify-common-7.0.0/cloudify_rest_client/bytes_stream_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-########
-# Copyright (c) 2015 GigaSpaces Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
-
+import cgi
 import os
 
 CONTENT_DISPOSITION_HEADER = 'content-disposition'
 DEFAULT_BUFFER_SIZE = 8192
 
 
 def request_data_file_stream(file_path,
@@ -80,19 +66,22 @@
     Read buffer-sized chunks from a stream, and write them to file
     :param streamed_response: The binary stream
     :param output_file: Name of the output file
     :param buffer_size: Size of the buffer
     :param progress_callback: Callback function - can be used to print progress
     :return:
     """
-    output_filename = streamed_response.headers[
-        CONTENT_DISPOSITION_HEADER].split('filename=')[1]
+    header_value = streamed_response.headers.get(CONTENT_DISPOSITION_HEADER)
+    output_filename = None
+    if header_value:
+        _, content_params = cgi.parse_header(header_value)
+        output_filename = content_params.get('filename')
 
     if not output_file:
-        if CONTENT_DISPOSITION_HEADER not in streamed_response.headers:
+        if not output_filename:
             raise RuntimeError(
                 'Cannot determine attachment filename: {0} header not'
                 ' found in response headers'.format(
                     CONTENT_DISPOSITION_HEADER))
         output_file = output_filename
 
     if os.path.isdir(output_file):
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/client.py` & `cloudify-common-7.0.0/cloudify_rest_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 import requests
 from base64 import b64encode
 from requests.packages import urllib3
 
 from cloudify import constants
 from cloudify.utils import ipv6_url_compat
 
-from ._compat import PY36PLUS
-from .utils import is_kerberos_env
+from cloudify_rest_client.utils import is_kerberos_env, StreamedResponse
 from cloudify_rest_client import exceptions
 from cloudify_rest_client.idp import IdentityProviderClient
 from cloudify_rest_client.ldap import LdapClient
 from cloudify_rest_client.nodes import NodesClient
 from cloudify_rest_client.users import UsersClient
 from cloudify_rest_client.sites import SitesClient
 from cloudify_rest_client.agents import AgentsClient
 from cloudify_rest_client.events import EventsClient
 from cloudify_rest_client.license import LicenseClient
 from cloudify_rest_client.manager import ManagerClient
 from cloudify_rest_client.plugins import PluginsClient
 from cloudify_rest_client.secrets import SecretsClient
+from cloudify_rest_client.secrets_providers import SecretsProvidersClient
 from cloudify_rest_client.tenants import TenantsClient
 from cloudify_rest_client.evaluate import EvaluateClient
 from cloudify_rest_client.summary import SummariesClient
 from cloudify_rest_client.snapshots import SnapshotsClient
 from cloudify_rest_client.log_bundles import LogBundlesClient
 from cloudify_rest_client.cluster import ClusterStatusClient
 from cloudify_rest_client.blueprints import BlueprintsClient
@@ -52,28 +52,27 @@
 from cloudify_rest_client.inter_deployment_dependencies import (
     InterDeploymentDependencyClient)
 from cloudify_rest_client.labels import (DeploymentsLabelsClient,
                                          BlueprintsLabelsClient)
 from cloudify_rest_client.filters import (DeploymentsFiltersClient,
                                           BlueprintsFiltersClient)
 from cloudify_rest_client.workflows import WorkflowsClient
+from cloudify_rest_client.resources import ResourcesClient
 from cloudify_rest_client.audit_log import AuditLogClient
+from cloudify_rest_client.community_contacts import CommunityContactsClient
+from cloudify_async_client.audit_log import AuditLogAsyncClient
 
 try:
     from requests_kerberos import HTTPKerberosAuth
 except Exception:
     # requests_kerberos library require pykerberos.
     # pykerberos require krb5-devel, which isn't python lib.
     # Kerberos users will need to manually install it.
     HTTPKerberosAuth = None
 
-if PY36PLUS:
-    from cloudify_async_client.audit_log import AuditLogAsyncClient
-else:
-    AuditLogAsyncClient = None
 
 DEFAULT_PORT = 80
 SECURED_PORT = 443
 SECURED_PROTOCOL = 'https'
 DEFAULT_PROTOCOL = 'http'
 DEFAULT_API_VERSION = 'v3.1'
 BASIC_AUTH_PREFIX = 'Basic'
@@ -103,23 +102,37 @@
         self.logger = logging.getLogger('cloudify.rest_client.http')
         self.cert = cert
         self.trust_all = trust_all
         self._set_header(constants.CLOUDIFY_AUTHENTICATION_HEADER,
                          self._get_auth_header(username, password),
                          log_value=False)
         self._set_header(constants.CLOUDIFY_TOKEN_AUTHENTICATION_HEADER, token)
-        self._set_header(CLOUDIFY_TENANT_HEADER, tenant)
+        tenant_from_header = headers.get(CLOUDIFY_TENANT_HEADER) if headers\
+            else None
+        self.tenant_name = tenant or tenant_from_header
         if session is None:
             session = requests.Session()
         self._session = session
 
     @property
+    def tenant_name(self):
+        return self._tenant_name
+
+    @tenant_name.setter
+    def tenant_name(self, name):
+        self._tenant_name = name
+        self._set_header(CLOUDIFY_TENANT_HEADER, name)
+
+    @property
+    def base_url(self):
+        return f'{self.protocol}://{self.host}:{self.port}'
+
+    @property
     def url(self):
-        return '{0}://{1}:{2}/api/{3}'.format(self.protocol, self.host,
-                                              self.port, self.api_version)
+        return f'{self.base_url}/api/{self.api_version}'
 
     def has_kerberos(self):
         if self.kerberos_env is not None:
             return self.kerberos_env
         return bool(HTTPKerberosAuth) and is_kerberos_env()
 
     def has_auth_header(self):
@@ -203,22 +216,19 @@
                                    headers=headers,
                                    stream=stream,
                                    verify=verify,
                                    timeout=timeout or self.default_timeout_sec,
                                    auth=auth)
         if self.logger.isEnabledFor(logging.DEBUG):
             for hdr, hdr_content in response.request.headers.items():
-                self.logger.debug('request header:  %s: %s'
-                                  % (hdr, hdr_content))
-            self.logger.debug('reply:  "%s %s" %s'
-                              % (response.status_code,
-                                 response.reason, response.content))
+                self.logger.debug('request header:  %s: %s', hdr, hdr_content)
+            self.logger.debug('reply:  "%s %s" %s', response.status_code,
+                              response.reason, response.content)
             for hdr, hdr_content in response.headers.items():
-                self.logger.debug('response header:  %s: %s'
-                                  % (hdr, hdr_content))
+                self.logger.debug('response header:  %s: %s', hdr, hdr_content)
 
         if isinstance(expected_status_code, numbers.Number):
             expected_status_code = [expected_status_code]
         if response.status_code not in expected_status_code:
             self._raise_client_error(response, request_url)
 
         if response.status_code == 204:
@@ -248,17 +258,20 @@
                    requests_method,
                    uri,
                    data=None,
                    params=None,
                    headers=None,
                    expected_status_code=200,
                    stream=False,
+                   url_prefix=True,
                    versioned_url=True,
                    timeout=None):
-        if versioned_url:
+        if not url_prefix:
+            request_url = f'{self.base_url}{uri}'
+        elif versioned_url:
             request_url = '{0}{1}'.format(self.url, uri)
         else:
             # remove version from url ending
             url = self.url.rsplit('/', 1)[0]
             request_url = '{0}{1}'.format(url, uri)
 
         # build headers
@@ -311,107 +324,97 @@
                 'please make sure it is online and all required ports are '
                 'open.'
                 '\nThis can also happen when the manager is not working with '
                 'SSL, but the client does'.format(e)
             )
 
     def get(self, uri, data=None, params=None, headers=None, _include=None,
-            expected_status_code=200, stream=False, versioned_url=True,
-            timeout=None):
+            expected_status_code=200, stream=False, url_prefix=True,
+            versioned_url=True, timeout=None):
         if _include:
             fields = ','.join(_include)
             if not params:
                 params = {}
             params['_include'] = fields
         return self.do_request(self._session.get,
                                uri,
                                data=data,
                                params=params,
                                headers=headers,
                                expected_status_code=expected_status_code,
                                stream=stream,
+                               url_prefix=url_prefix,
                                versioned_url=versioned_url,
                                timeout=timeout)
 
     def put(self, uri, data=None, params=None, headers=None,
-            expected_status_code=200, stream=False, timeout=None):
+            expected_status_code=200, stream=False, url_prefix=True,
+            timeout=None):
         return self.do_request(self._session.put,
                                uri,
                                data=data,
                                params=params,
                                headers=headers,
                                expected_status_code=expected_status_code,
                                stream=stream,
+                               url_prefix=url_prefix,
                                timeout=timeout)
 
     def patch(self, uri, data=None, params=None, headers=None,
-              expected_status_code=200, stream=False, timeout=None):
+              expected_status_code=200, stream=False, url_prefix=True,
+              timeout=None):
         return self.do_request(self._session.patch,
                                uri,
                                data=data,
                                params=params,
                                headers=headers,
                                expected_status_code=expected_status_code,
                                stream=stream,
+                               url_prefix=url_prefix,
                                timeout=timeout)
 
     def post(self, uri, data=None, params=None, headers=None,
-             expected_status_code=200, stream=False, timeout=None):
+             expected_status_code=200, stream=False, url_prefix=True,
+             timeout=None):
         return self.do_request(self._session.post,
                                uri,
                                data=data,
                                params=params,
                                headers=headers,
                                expected_status_code=expected_status_code,
                                stream=stream,
+                               url_prefix=url_prefix,
                                timeout=timeout)
 
     def delete(self, uri, data=None, params=None, headers=None,
-               expected_status_code=(200, 204), stream=False, timeout=None):
+               expected_status_code=(200, 204), stream=False, url_prefix=True,
+               timeout=None):
         return self.do_request(self._session.delete,
                                uri,
                                data=data,
                                params=params,
                                headers=headers,
                                expected_status_code=expected_status_code,
                                stream=stream,
+                               url_prefix=url_prefix,
                                timeout=timeout)
 
     def _get_auth_header(self, username, password):
         if not username or not password:
             return None
         credentials = '{0}:{1}'.format(username, password).encode('utf-8')
         encoded_credentials = b64encode(credentials).decode('utf-8')
         return BASIC_AUTH_PREFIX + ' ' + encoded_credentials
 
     def _set_header(self, key, value, log_value=True):
         if not value:
             return
         self.headers[key] = value
         value = value if log_value else '*'
-        self.logger.debug('Setting `{0}` header: {1}'.format(key, value))
-
-
-class StreamedResponse(object):
-
-    def __init__(self, response):
-        self._response = response
-
-    @property
-    def headers(self):
-        return self._response.headers
-
-    def bytes_stream(self, chunk_size=8192):
-        return self._response.iter_content(chunk_size)
-
-    def lines_stream(self):
-        return self._response.iter_lines()
-
-    def close(self):
-        self._response.close()
+        self.logger.debug('Setting `%s` header: %s', key, value)
 
 
 class CloudifyClient(object):
     """Cloudify's management client."""
     client_class = HTTPClient
 
     def __init__(self, host='localhost', port=None, protocol=DEFAULT_PROTOCOL,
@@ -478,25 +481,28 @@
         self.maintenance_mode = MaintenanceModeClient(self._client)
         self.deployment_updates = DeploymentUpdatesClient(self._client)
         self.tenants = TenantsClient(self._client)
         self.user_groups = UserGroupsClient(self._client)
         self.users = UsersClient(self._client)
         self.ldap = LdapClient(self._client)
         self.secrets = SecretsClient(self._client)
+        self.secrets_providers = SecretsProvidersClient(self._client)
         self.agents = AgentsClient(self._client)
         self.summary = SummariesClient(self._client)
         self.operations = OperationsClient(self._client)
         self.tasks_graphs = TasksGraphClient(self._client)
         self.license = LicenseClient(self._client)
         self.sites = SitesClient(self._client)
         self.cluster_status = ClusterStatusClient(self._client)
         self.inter_deployment_dependencies = InterDeploymentDependencyClient(
             self._client)
         self.deployments_filters = DeploymentsFiltersClient(self._client)
         self.blueprints_filters = BlueprintsFiltersClient(self._client)
         self.deployments_labels = DeploymentsLabelsClient(self._client)
         self.blueprints_labels = BlueprintsLabelsClient(self._client)
         self.workflows = WorkflowsClient(self._client)
+        self.resources = ResourcesClient(self._client)
+        self.community_contacts = CommunityContactsClient(self._client)
         if AuditLogAsyncClient is None:
             self.auditlog = AuditLogClient(self._client)
         else:
             self.auditlog = AuditLogAsyncClient(self._client)
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/cluster.py` & `cloudify-common-7.0.0/cloudify_rest_client/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/constants.py` & `cloudify-common-7.0.0/cloudify_rest_client/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/deployment_modifications.py` & `cloudify-common-7.0.0/cloudify_rest_client/deployment_modifications.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/deployment_updates.py` & `cloudify-common-7.0.0/cloudify_rest_client/deployment_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import os
 import json
 import shutil
 import tempfile
+from urllib.parse import quote as urlquote, urlparse
+from urllib.request import pathname2url
 
 from mimetypes import MimeTypes
 
 from cloudify_rest_client import utils
-from cloudify_rest_client._compat import urlquote, pathname2url, urlparse
 from cloudify_rest_client.responses import ListResponse
 
 
 class DeploymentUpdate(dict):
 
     def __init__(self, update):
         self.update(update)
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/deployments.py` & `cloudify-common-7.0.0/cloudify_rest_client/deployments.py`

 * *Files 13% similar despite different names*

```diff
@@ -114,21 +114,14 @@
     def deployment_groups(self):
         """
         :return: IDs of deployment groups that this deployment belongs to
         """
         return self.get('deployment_groups')
 
     @property
-    def latest_execution_status(self):
-        """
-        :return: The deployment latest execution status
-        """
-        return self.get('latest_execution_status')
-
-    @property
     def installation_status(self):
         """
         :return: The deployment installation status
         """
         return self.get('installation_status')
 
     @property
@@ -170,14 +163,37 @@
     def environment_type(self):
         """
         :return: The environment type
         """
         return self.get('environment_type')
 
     @property
+    def latest_execution_id(self):
+        """
+        :return: The deployment latest execution ID
+        """
+        # this value was called .latest_execution (which was just the string
+        # ID indeed) in 7.0 and before
+        return self.get('latest_execution_id') or self.get('latest_execution')
+
+    @property
+    def latest_execution_workflow_id(self):
+        """
+        :return: The deployment latest execution workflow name
+        """
+        return self.get('latest_execution_workflow_id')
+
+    @property
+    def latest_execution_status(self):
+        """
+        :return: The deployment latest execution status
+        """
+        return self.get('latest_execution_status')
+
+    @property
     def latest_execution_total_operations(self):
         """
         :return: The total operations for latest execution of deployment
         """
         return self.get('latest_execution_total_operations')
 
     @property
@@ -309,19 +325,14 @@
 class DeploymentScalingGroup(dict):
 
     def __init__(self, scaling_groups):
         super(DeploymentScalingGroup, self).__init__()
         self.update(scaling_groups)
 
     @property
-    def deployment_id(self):
-        """ID of the deployment the capabilities belong to."""
-        return self['deployment_id']
-
-    @property
     def name(self):
         """Name of the scaling group."""
         return self['name']
 
     @property
     def members(self):
         """A list of members of the scaling group (nodes)."""
@@ -384,15 +395,15 @@
         response = self.api.get('/deployment-groups/{0}'.format(group_id))
         return DeploymentGroup(response)
 
     def put(self, group_id, visibility=VisibilityState.TENANT,
             description=None, blueprint_id=None, default_inputs=None,
             labels=None, filter_id=None, deployment_ids=None,
             new_deployments=None, deployments_from_group=None,
-            created_by=None, created_at=None):
+            created_by=None, created_at=None, creation_counter=None):
         """Create or update the specified deployment group.
 
         Setting group deployments using this method (via either filter_id
         or deployment_ids) will set, NOT ADD, ie. it will remove all other
         deployments from the group.
 
         :param visibility: visibility of the group
@@ -410,14 +421,16 @@
             and default_inputs
         :type new_deployments: a list of dicts, each can contain the
             keys "id", "inputs", "labels"
         :param deployments_from_group: add all deployments belonging to the
             group given by this id
         :param created_by: Override the creator. Internal use only.
         :param created_at: Override the creation timestamp. Internal use only.
+        :param creation_counter: Override the creation counter.
+            Internal use only.
         :return: the created deployment group
         """
         data = {
             'visibility': visibility,
             'description': description,
             'blueprint_id': blueprint_id,
             'default_inputs': default_inputs,
@@ -427,14 +440,16 @@
             'new_deployments': new_deployments,
             'deployments_from_group': deployments_from_group,
         }
         if created_at:
             data['created_at'] = created_at
         if created_by:
             data['created_by'] = created_by
+        if creation_counter:
+            data['creation_counter'] = creation_counter
         response = self.api.put(
             '/deployment-groups/{0}'.format(group_id), data=data,
         )
         return DeploymentGroup(response)
 
     def add_deployments(self, group_id, deployment_ids=None, count=None,
                         new_deployments=None, filter_id=None,
@@ -601,29 +616,35 @@
         )
 
 
 class DeploymentScalingGroupsClient(object):
     def __init__(self, api):
         self.api = api
 
-    def list(self, deployment_id, constraints=None, _include=None, **kwargs):
+    def list(self, blueprint_id=None, deployment_id=None,
+             constraints=None, _include=None, **kwargs):
         """
         Returns a list of deployment's scaling groups matching constraints.
 
+        :param blueprint_id: An identifier of a blueprint which scaling
+               groups are going to be searched.
         :param deployment_id: An identifier of a deployment which scaling
                groups are going to be searched.
         :param constraints: A list of DSL constraints for scaling_group
                data type to filter the scaling groups by.
         :param _include: List of fields to include in response.
         :param kwargs: Optional filter fields. for a list of available fields
                see the REST service's models.Deployment.fields
         :return: DeploymentScalingGroup list.
         """
         params = copy(kwargs) or {}
-        params['deployment_id'] = deployment_id
+        if blueprint_id is not None:
+            params['blueprint_id'] = blueprint_id
+        if deployment_id is not None:
+            params['deployment_id'] = deployment_id
         if _include:
             params['_include'] = ','.join(_include)
 
         response = self.api.post('/searches/scaling-groups', params=params,
                                  data={'constraints': constraints or {}})
         return ListResponse(
             items=[DeploymentScalingGroup(item) for item in response['items']],
@@ -716,14 +737,29 @@
                site_name=None,
                runtime_only_evaluation=False,
                labels=None,
                display_name=None,
                async_create=None,
                created_at=None,
                created_by=None,
+               workflows=None,
+               groups=None,
+               scaling_groups=None,
+               policy_triggers=None,
+               policy_types=None,
+               outputs=None,
+               capabilities=None,
+               resource_tags=None,
+               description=None,
+               deployment_status=None,
+               installation_status=None,
+               sub_services_status=None,
+               sub_environments_status=None,
+               sub_services_count=None,
+               sub_environments_count=None,
                _workdir_zip=None):
         """
         Creates a new deployment for the provided blueprint id and
         deployment id.
 
         :param blueprint_id: Blueprint id to create a deployment of.
         :param deployment_id: Deployment id of the new created deployment.
@@ -740,29 +776,81 @@
             evaluated at parse time.
         :param labels: The deployment's labels. A list of 1-entry
             dictionaries: [{<key1>: <value1>}, {<key2>: <value2>}, ...]'
         :param display_name: The deployment's display name.
         :param async_create: if True, do not wait for the deployment
             environment to finish creating
         :param _workdir_zip: Internal only.
+        :param workflows: Set the deployment workflows. Internal use only.
+        :param groups: Set groups. Internal use only.
+        :param scaling_groups: Set scaling_groups. Internal use only.
+        :param policy_triggers: Set policy_triggers. Internal use only.
+        :param policy_types: Set policy_types. Internal use only.
+        :param outputs: Set outputs. Internal use only.
+        :param capabilities: Set capabilities. Internal use only.
+        :param resource_tags: Set resource_tags. Internal use only.
+        :param description: Set description. Internal use only.
+        :param created_by: Override the creator. Internal use only.
+        :param created_at: Override the creation timestamp. Internal use only.
+        :param deployment_status: Set deployment status. Internal use only.
+        :param installation_status: Set installation status.
+                                    Internal use only.
+        :param sub_services_status: Set sub-services status. Internal use only.
+        :param sub_environments_status: Set sub-environments status.
+                                        Internal use only.
+        :param sub_services_count: Set sub-services count. Internal use only.
+        :param sub_environments_count: Set sub-environments count.
+                                       Internal use only.
         :return: The created deployment.
         """
         assert blueprint_id
         assert deployment_id
         data = {'blueprint_id': blueprint_id, 'visibility': visibility}
-        if inputs:
+        if inputs is not None:
             data['inputs'] = inputs
-        if site_name:
+        if site_name is not None:
             data['site_name'] = site_name
-        if labels:
+        if labels is not None:
             data['labels'] = labels
-        if display_name:
+        if display_name is not None:
             data['display_name'] = display_name
-        if _workdir_zip:
+        if _workdir_zip is not None:
             data['workdir_zip'] = _workdir_zip
+        if workflows is not None:
+            data['workflows'] = workflows
+        if groups is not None:
+            data['groups'] = groups
+        if scaling_groups is not None:
+            data['scaling_groups'] = scaling_groups
+        if policy_triggers is not None:
+            data['policy_triggers'] = policy_triggers
+        if policy_types is not None:
+            data['policy_types'] = policy_types
+        if outputs is not None:
+            data['outputs'] = outputs
+        if capabilities is not None:
+            data['capabilities'] = capabilities
+        if resource_tags is not None:
+            data['resource_tags'] = resource_tags
+        if outputs is not None:
+            data['outputs'] = outputs
+        if description is not None:
+            data['description'] = description
+        if deployment_status is not None:
+            data['deployment_status'] = deployment_status
+        if installation_status is not None:
+            data['installation_status'] = installation_status
+        if sub_services_status is not None:
+            data['sub_services_status'] = sub_services_status
+        if sub_environments_status is not None:
+            data['sub_environments_status'] = sub_environments_status
+        if sub_services_count is not None:
+            data['sub_services_count'] = sub_services_count
+        if sub_environments_count is not None:
+            data['sub_environments_count'] = sub_environments_count
         data['skip_plugins_validation'] = skip_plugins_validation
         data['runtime_only_evaluation'] = runtime_only_evaluation
         uri = '/deployments/{0}'.format(deployment_id)
         params = {}
         if created_at:
             data['created_at'] = created_at
         if created_by:
@@ -849,16 +937,17 @@
         if created_at:
             data['created_at'] = created_at
         updated_dep = self.api.patch(
             '/deployments/{0}'.format(deployment_id), data=data)
         return Deployment(updated_dep)
 
     def set_attributes(self, deployment_id, **kwargs):
-        """Set kwargs on the deployment.
+        """Set arbitrary properties on the deployment.
+
+        If you're not sure, you probably want to look at deployment update
+        instead.
 
-        This is used internally for first populating the deployment
-        with the attributes from the plan.
-        For updating existing deployments, use the deployment update methods.
+        For internal use only.
         """
         updated_dep = self.api.patch(
             '/deployments/{0}'.format(deployment_id), data=kwargs)
         return Deployment(updated_dep)
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/evaluate.py` & `cloudify-common-7.0.0/cloudify_rest_client/evaluate.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/events.py` & `cloudify-common-7.0.0/cloudify_rest_client/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/exceptions.py` & `cloudify-common-7.0.0/cloudify_rest_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,22 @@
         self.status_code = status_code
         self.error_code = error_code
         self.server_traceback = server_traceback
         self.response = response
         self._message = message
 
     def __str__(self):
+        message = self._message
+        if self.server_traceback:
+            _, _, last_line = self.server_traceback.strip().rpartition('\n')
+            if last_line:
+                message = '{0} ({1})'.format(self._message, last_line)
         if self.status_code != -1:
-            return '{0}: {1}'.format(self.status_code, self._message)
-        return self._message
+            return '{0}: {1}'.format(self.status_code, message)
+        return message
 
 
 class DeploymentEnvironmentCreationInProgressError(CloudifyClientError):
     """
     Raised when there's attempt to execute a deployment workflow and
     deployment environment creation workflow execution is still running.
     In such a case, workflow execution should be retried after a reasonable
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/execution_schedules.py` & `cloudify-common-7.0.0/cloudify_rest_client/execution_schedules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import datetime
+
 from cloudify_rest_client.responses import ListResponse
 
 
 class ExecutionSchedule(dict):
     """
     Cloudify execution schedule.
     """
@@ -92,15 +94,15 @@
         self.api = api
         self._uri_prefix = 'execution-schedules'
 
     def create(self, schedule_id, deployment_id, workflow_id,
                execution_arguments=None, parameters=None,
                since=None, until=None, recurrence=None, count=None,
                weekdays=None, rrule=None, slip=0, stop_on_fail=False,
-               created_by=None, created_at=None):
+               created_by=None, created_at=None, enabled=True):
         """Schedules a deployment's workflow execution whose id is provided.
 
         :param schedule_id: Name for the schedule task. Used for listing,
             updating or deleting it later.
         :param deployment_id: The deployment's id to execute a workflow for.
         :param workflow_id: The workflow to be executed id.
         :param execution_arguments: A dict of arguments passed directly to the
@@ -130,33 +132,40 @@
             and `weekdays`.
         :param slip: Maximum time window after the target time has passed,
             in which the scheduled execution can run (in minutes).
         :param stop_on_fail: If set to true, once the execution has failed,
             the scheduler won't make further attempts to run it.
         :param created_by: Override the creator. Internal use only.
         :param created_at: Override the creation timestamp. Internal use only.
+        :param enabled: Boolean indicating whether the schedule should be
+                        enabled.
         :return: The created execution schedule.
         """
         assert schedule_id
         assert deployment_id
         assert workflow_id
         assert since
+        if isinstance(since, datetime):
+            since = since.isoformat()
+        if isinstance(until, datetime):
+            until = until.isoformat()
         params = {'deployment_id': deployment_id}
         data = {
             'workflow_id': workflow_id,
             'execution_arguments': execution_arguments,
             'parameters': parameters,
-            'since': since.isoformat(),
-            'until': until.isoformat() if until else None,
+            'since': since,
+            'until': until,
             'recurrence': recurrence,
             'count': count,
             'weekdays': weekdays,
             'rrule': rrule,
             'slip': slip,
-            'stop_on_fail': stop_on_fail
+            'stop_on_fail': stop_on_fail,
+            'enabled': enabled,
         }
         if created_by:
             data['created_by'] = created_by
         if created_at:
             data['created_at'] = created_at
         uri = '/{self._uri_prefix}/{id}'.format(self=self, id=schedule_id)
         response = self.api.put(uri,
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/executions.py` & `cloudify-common-7.0.0/cloudify_rest_client/executions.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,32 @@
             data={
                 'success_group_id': success_group,
                 'failure_group_id': failed_group,
             }
         )
         return ExecutionGroup(response)
 
+    def set_concurrency(self, execution_group_id, concurrency):
+        """Change the concurrency setting of an execution-group.
+
+        This affects the de-queueing mechanism: when starting queued
+        executions, the new concurrency setting will be used.
+
+        :param execution_group_id: ID of the execution group
+        :param concurrency: the new concurrency setting, a natural number
+        :return: The updated ExecutionGroup
+        """
+        response = self.api.patch(
+            '/execution-groups/{0}'.format(execution_group_id),
+            data={
+                'concurrency': concurrency,
+            },
+        )
+        return ExecutionGroup(response)
+
 
 class ExecutionsClient(object):
 
     def __init__(self, api):
         self.api = api
         self._uri_prefix = 'executions'
         self._wrapper_cls = Execution
@@ -405,15 +423,16 @@
         """
         return self.create(*args, **kwargs)
 
     def create(self, deployment_id, workflow_id, parameters=None,
                allow_custom_parameters=False, force=False, dry_run=False,
                queue=False, schedule=None, force_status=None,
                created_by=None, created_at=None, started_at=None,
-               ended_at=None, execution_id=None, wait_after_fail=600):
+               ended_at=None, execution_id=None, wait_after_fail=600,
+               error=None):
         """Creates an execution on a deployment.
         If force_status is provided, the execution will not be started.
         Otherwise, parameters and return value are identical to 'start'.
         """
         if schedule:
             warnings.warn("The 'schedule' flag is deprecated. Please use "
                           "`cfy deployments schedule create instead`",
@@ -430,14 +449,15 @@
             'wait_after_fail': wait_after_fail,
             'force_status': force_status,
             'created_by': created_by,
             'created_at': created_at,
             'started_at': started_at,
             'ended_at': ended_at,
             'id': execution_id,
+            'error': error,
         }
         uri = '/executions'
         response = self.api.post(uri,
                                  data=data,
                                  expected_status_code=201)
         return Execution(response)
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/filters.py` & `cloudify-common-7.0.0/cloudify_rest_client/filters.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/inter_deployment_dependencies.py` & `cloudify-common-7.0.0/cloudify_rest_client/inter_deployment_dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from cloudify.deployment_dependencies import (create_deployment_dependency,
+from cloudify.deployment_dependencies import (build_deployment_dependency,
                                               DEPENDENCY_CREATOR)
 
 from cloudify_rest_client.responses import ListResponse
 
 
 class InterDeploymentDependency(dict):
 
@@ -24,14 +24,18 @@
         self.update(dependency)
 
     @property
     def id(self):
         return self['id']
 
     @property
+    def target_deployment_func(self):
+        return self['target_deployment_func']
+
+    @property
     def dependency_creator(self):
         return self[DEPENDENCY_CREATOR]
 
     @property
     def source_deployment_id(self):
         return self['source_deployment_id']
 
@@ -56,18 +60,26 @@
 
     def _wrap_list(self, response):
         return ListResponse(
             [self._wrapper_cls(item) for item in response['items']],
             response['metadata']
         )
 
-    def create(self, dependency_creator, source_deployment,
+    def create(self,
+               dependency_creator,
+               source_deployment,
                target_deployment=None,
-               external_source=None, external_target=None,
-               target_deployment_func=None):
+               external_source=None,
+               external_target=None,
+               target_deployment_func=None,
+               _id=None,
+               _visibility=None,
+               _created_at=None,
+               _created_by=None,
+               ):
         """Creates an inter-deployment dependency.
 
         :param dependency_creator: a string representing the entity that
          is responsible for this dependency (e.g. an intrinsic function
          blueprint path, 'node_instances.some_node_instance', etc.).
         :param source_deployment: source deployment that depends on the target
          deployment.
@@ -77,22 +89,32 @@
         resource as target, pass here a JSON containing the source deployment
         metadata, i.e. deployment name, tenant name, and the manager host(s).
         :param external_target: if the source deployment uses an external
         resource as target, pass here a JSON containing the target deployment
         metadata, i.e. deployment name, tenant name, and the manager host(s).
         :param target_deployment_func: a function used to determine the target
         deployment.
+        :param _id: Override the identifier. Internal use only.
+        :param _visibility: Override the visibility. Internal use only.
+        :param _created_at: Override the creation timestamp. Internal use only.
+        :param _created_by: Override the creator. Internal use only.
         :return: an InterDeploymentDependency object.
         """
-        data = create_deployment_dependency(dependency_creator,
-                                            source_deployment,
-                                            target_deployment,
-                                            target_deployment_func,
-                                            external_source,
-                                            external_target)
+        data = build_deployment_dependency(
+            dependency_creator,
+            source_deployment=source_deployment,
+            target_deployment=target_deployment,
+            target_deployment_func=target_deployment_func,
+            external_source=external_source,
+            external_target=external_target,
+            id=_id,
+            visibility=_visibility,
+            created_at=_created_at,
+            created_by=_created_by,
+        )
         response = self.api.put(
             '/{self._uri_prefix}'.format(self=self), data=data)
         return self._wrapper_cls(response)
 
     def create_many(self, source_deployment_id, inter_deployment_dependencies):
         """Creates a number of inter-deployment dependencies.
 
@@ -148,19 +170,21 @@
         resource as target, pass here a JSON containing the source deployment
         metadata, i.e. deployment name, tenant name, and the manager host(s).
         :param external_target: if the source deployment uses an external
         resource as target, pass here a JSON containing the target deployment
         metadata, i.e. deployment name, tenant name, and the manager host(s).
         :return: an InterDeploymentDependency object.
         """
-        data = create_deployment_dependency(dependency_creator,
-                                            source_deployment,
-                                            target_deployment,
-                                            external_source=external_source,
-                                            external_target=external_target)
+        data = build_deployment_dependency(
+            dependency_creator,
+            source_deployment=source_deployment,
+            target_deployment=target_deployment,
+            external_source=external_source,
+            external_target=external_target,
+        )
         data['is_component_deletion'] = is_component_deletion
         self.api.delete('/{self._uri_prefix}'.format(self=self), data=data)
 
     def list(self, _include=None, sort=None, is_descending=False, **kwargs):
         """
         Returns a list of available  inter-deployment dependencies.
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/labels.py` & `cloudify-common-7.0.0/cloudify_rest_client/labels.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/ldap.py` & `cloudify-common-7.0.0/cloudify_rest_client/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/license.py` & `cloudify-common-7.0.0/cloudify_rest_client/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/log_bundles.py` & `cloudify-common-7.0.0/cloudify_rest_client/log_bundles.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/maintenance.py` & `cloudify-common-7.0.0/cloudify_rest_client/maintenance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/manager.py` & `cloudify-common-7.0.0/cloudify_rest_client/manager.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/node_instances.py` & `cloudify-common-7.0.0/cloudify_rest_client/node_instances.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/nodes.py` & `cloudify-common-7.0.0/cloudify_rest_client/nodes.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/operations.py` & `cloudify-common-7.0.0/cloudify_rest_client/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     def containing_subgraph(self):
         return self.get('parameters', {}).get('containing_subgraph')
 
     @property
     def info(self):
         return self.get('parameters', {}).get('info')
 
+    @property
+    def tasks_graph_id(self):
+        return self.get('tasks_graph_id')
+
 
 class OperationsClient(object):
     def __init__(self, api):
         self.api = api
         self._uri_prefix = 'operations'
         self._wrapper_cls = Operation
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/permissions.py` & `cloudify-common-7.0.0/cloudify_rest_client/permissions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/plugins.py` & `cloudify-common-7.0.0/cloudify_rest_client/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import contextlib
+import re
+import tempfile
+from urllib.parse import urlparse
 
 from cloudify_rest_client import bytes_stream_utils
-from cloudify_rest_client._compat import urlparse
 from cloudify_rest_client.responses import ListResponse
 from cloudify_rest_client.constants import VisibilityState
 
 
 class Plugin(dict):
     """
     Cloudify plugin.
@@ -187,14 +189,21 @@
     @property
     def resource_tags(self):
         """
         :return: resource_tags declared for that plugin.
         """
         return self.get('resource_tags')
 
+    @property
+    def yaml_files_paths(self):
+        """
+        :return: yaml_files_paths declared for that plugin.
+        """
+        return self.get('yaml_files_paths')
+
 
 class PluginsClient(object):
     """
     Cloudify's plugin management client.
     """
     def __init__(self, api):
         self.api = api
@@ -307,24 +316,29 @@
         )
         if 'metadata' in response and 'items' in response:
             # This is a list of plugins - for caravan
             return self._wrap_list(response)
         else:
             return self._wrapper_cls(response)
 
-    def download(self, plugin_id, output_file, progress_callback=None):
+    def download(self, plugin_id, output_file, progress_callback=None,
+                 full_archive=False):
         """Downloads a previously uploaded plugin archive from the manager
 
         :param plugin_id: The plugin ID of the plugin to be downloaded.
         :param output_file: The file path of the downloaded plugin file
         :param progress_callback: Callback function - can be used to print
         a progress bar
+        :param full_archive: If set to true, download a zip containing the
+        wagon and all yaml files for this plugin.
         :return: The file path of the downloaded plugin.
         """
         uri = '/plugins/{0}/archive'.format(plugin_id)
+        if full_archive:
+            uri += '?full_archive=true'
         with contextlib.closing(self.api.get(uri, stream=True)) as response:
             output_file = bytes_stream_utils.write_response_stream_to_file(
                 response, output_file, progress_callback=progress_callback)
 
             return output_file
 
     def download_yaml(self, plugin_id, output_file, progress_callback=None):
@@ -339,14 +353,56 @@
         uri = '/plugins/{0}/yaml'.format(plugin_id)
         with contextlib.closing(self.api.get(uri, stream=True)) as response:
             output_file = bytes_stream_utils.write_response_stream_to_file(
                 response, output_file, progress_callback=progress_callback)
 
             return output_file
 
+    def get_yaml(self, plugin_id, dsl_version=None, progress_callback=None):
+        """Get plugin yaml file content, compatible with provided dsl_version
+
+        :param plugin_id: The plugin ID of the plugin yaml to be downloaded.
+        :param dsl_version: Preferred version of the plugin yaml.
+        :param progress_callback: Callback function - can be used to print
+        a progress bar
+        :return: A content of plugin yaml.
+        """
+        params = {'dsl_version': dsl_version} if dsl_version else {}
+        uri = '/plugins/{0}/yaml'.format(plugin_id)
+        with tempfile.TemporaryDirectory() as tmpdir:
+            output_file = os.path.join(tmpdir, 'plugin.yaml')
+            response = self.api.get(uri, params=params, stream=True)
+            output_file = bytes_stream_utils.write_response_stream_to_file(
+                response, output_file, progress_callback=progress_callback)
+            with open(output_file) as fh:
+                content = fh.read()
+
+        return content
+
+    def list_yaml_files(self, plugin_id, dsl_version=None):
+        """List plugin yaml files compatible with provided dsl_version
+
+        :param plugin_id: The plugin ID of the plugin yaml to be downloaded.
+        :param dsl_version: Preferred version of the plugin yaml.
+        :return: A list of plugin yaml paths.
+        """
+        plugin_dict = self.api.get(f'/plugins/{plugin_id}')
+        plugin = Plugin(plugin_dict)
+        if not plugin.yaml_files_paths or not dsl_version:
+            return plugin.yaml_files_paths or []
+
+        unknown_dsl_version_yaml_files_paths = []
+        for yaml_file_path in plugin.yaml_files_paths:
+            if yaml_file_path.endswith(f'{dsl_version}.yaml'):
+                return [yaml_file_path]
+            if not re.search(r"_\d_\d+.yaml$", yaml_file_path):
+                unknown_dsl_version_yaml_files_paths += [yaml_file_path]
+
+        return unknown_dsl_version_yaml_files_paths
+
     def set_global(self, plugin_id):
         """
         Updates the plugin's visibility to global
 
         :param plugin_id: Plugin's id to update.
         :return: The plugin.
         """
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/plugins_update.py` & `cloudify-common-7.0.0/cloudify_rest_client/plugins_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,26 +99,29 @@
                                 params=params)
         return self._wrap_list(response)
 
     def inject(self, blueprint_id, force=False,
                created_by=None, created_at=None,
                execution_id=None, state=None,
                update_id=None, affected_deployments=None,
+               deployments_per_tenant=None, all_tenants=None,
                temp_blueprint_id=None):
         return PluginsUpdate(self.api.post(
             '/{self._uri_prefix}/{}/update/initiate'.format(blueprint_id,
                                                             self=self),
             data=_data_from_kwargs(
                 force=force,
                 created_by=created_by,
                 created_at=created_at,
                 execution_id=execution_id,
                 state=state,
                 update_id=update_id,
+                all_tenants=all_tenants,
                 affected_deployments=affected_deployments,
+                deployments_per_tenant=deployments_per_tenant,
                 temp_blueprint_id=temp_blueprint_id,
             ),
         ))
 
     def update_plugins(self, blueprint_id, force=False, plugin_names=None,
                        to_latest=None, all_to_latest=True,
                        to_minor=None, all_to_minor=False,
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/responses.py` & `cloudify-common-7.0.0/cloudify_rest_client/responses.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/sites.py` & `cloudify-common-7.0.0/cloudify_rest_client/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         """
         Create a new site.
 
         :param name: The name of the site.
         :param location: The location of the site : "latitude,longitude".
         :param visibility: The visibility of the site, can be 'private',
                            'tenant' or 'global'
-        :param creator: Override the creator. Internal use only.
+        :param created_by: Override the creator. Internal use only.
         :param created_at: Override the creation timestamp. Internal use only.
         :return: The created site.
         """
         data = {'visibility': visibility}
         if location:
             data['location'] = location
         if created_by:
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/snapshots.py` & `cloudify-common-7.0.0/cloudify_rest_client/snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import os
 import contextlib
+from urllib.parse import urlparse
 
 from cloudify_rest_client import bytes_stream_utils
-from cloudify_rest_client._compat import urlparse
 from cloudify_rest_client.executions import Execution
 from cloudify_rest_client.responses import ListResponse
 
 
 class Snapshot(dict):
     """
     Cloudify snapshot.
@@ -109,31 +109,31 @@
 
     def create(self,
                snapshot_id,
                include_credentials,
                include_logs=True,
                include_events=True,
                queue=False,
-               include_metrics=None,
-               tempdir_path=None):
+               tempdir_path=None,
+               legacy=True):
         """
         Creates a new snapshot.
 
         :param snapshot_id: Snapshot id of the snapshot that will be created.
-        :param include_metrics: Deprecated parameter, should not be used.
         :return: The created snapshot.
         """
         assert snapshot_id
         uri = '/snapshots/{0}'.format(snapshot_id)
         params = {
             'include_credentials': include_credentials,
             'include_logs': include_logs,
             'include_events': include_events,
             'queue': queue,
             'tempdir_path': tempdir_path,
+            'legacy': legacy,
         }
         response = self.api.put(uri, data=params, expected_status_code=201)
         return Execution(response)
 
     def delete(self, snapshot_id):
         """
         Deletes the snapshot whose id matches the provided snapshot id.
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/summary.py` & `cloudify-common-7.0.0/cloudify_rest_client/summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     def __init__(self, api, summary_type):
         self.api = api
         self.summary_type = summary_type
 
     def get(self, _target_field, _sub_field=None, **kwargs):
         params = {
             '_target_field': _target_field,
-            '_sub_field': _sub_field,
         }
+        if _sub_field:
+            params['_sub_field'] = _sub_field
         params.update(kwargs)
         response = self.api.get(
             '/summary/{summary_type}'.format(summary_type=self.summary_type),
             params=params,
         )
         return ListResponse(response['items'], response['metadata'])
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/tenants.py` & `cloudify-common-7.0.0/cloudify_rest_client/tenants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/tokens.py` & `cloudify-common-7.0.0/cloudify_rest_client/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/user_groups.py` & `cloudify-common-7.0.0/cloudify_rest_client/user_groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/users.py` & `cloudify-common-7.0.0/cloudify_rest_client/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,21 +61,35 @@
     def active(self):
         """
         :return: Whether the user is active.
         """
         return self.get('active')
 
     @property
+    def created_at(self):
+        """
+        :return: The user creation time.
+        """
+        return self.get('created_at')
+
+    @property
     def last_login_at(self):
         """
         :return: The last time the user logged in.
         """
         return self.get('last_login_at')
 
     @property
+    def first_login_at(self):
+        """
+        :return: The first time the user logged in.
+        """
+        return self.get('first_login_at')
+
+    @property
     def is_locked(self):
         """
         :return: Whether a user is locked or not.
         """
         return self.get('is_locked')
 
 
@@ -102,20 +116,24 @@
         response = self.api.get('/users',
                                 _include=_include,
                                 params=params)
         return ListResponse([User(item) for item in response['items']],
                             response['metadata'])
 
     def create(self, username, password, role, is_prehashed=None,
-               created_at=None):
+               created_at=None, first_login_at=None, last_login_at=None):
         data = {'username': username, 'password': password, 'role': role}
         if is_prehashed is not None:
             data['is_prehashed'] = is_prehashed
         if created_at:
             data['created_at'] = created_at
+        if first_login_at:
+            data['first_login_at'] = first_login_at
+        if last_login_at:
+            data['last_login_at'] = last_login_at
         response = self.api.put('/users', data=data, expected_status_code=201)
         return User(response)
 
     def set_password(self, username, new_password):
         data = {'password': new_password}
         response = self.api.post('/users/{0}'.format(username), data=data)
         return User(response)
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/utils.py` & `cloudify-common-7.0.0/cloudify_rest_client/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -102,7 +102,26 @@
             f = os.path.join(p, executable)
             if os.path.isfile(f):
                 # the file exists, we have a shot at spawn working
                 return f
         return None
     else:
         return executable
+
+
+class StreamedResponse(object):
+
+    def __init__(self, response):
+        self._response = response
+
+    @property
+    def headers(self):
+        return self._response.headers
+
+    def bytes_stream(self, chunk_size=8192):
+        return self._response.iter_content(chunk_size)
+
+    def lines_stream(self):
+        return self._response.iter_lines()
+
+    def close(self):
+        self._response.close()
```

### Comparing `cloudify-common-6.4.2/cloudify_rest_client/workflows.py` & `cloudify-common-7.0.0/cloudify_rest_client/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/__init__.py` & `cloudify-common-7.0.0/dsl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/constants.py` & `cloudify-common-7.0.0/dsl_parser/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 PLUGINS = 'plugins'
 INTERFACES = 'interfaces'
 SOURCE_INTERFACES = 'source_interfaces'
 TARGET_INTERFACES = 'target_interfaces'
 WORKFLOWS = 'workflows'
 RELATIONSHIPS = 'relationships'
 PROPERTIES = 'properties'
+RUNTIME_PROPERTIES = 'runtime_properties'
 PARAMETERS = 'parameters'
 TYPE_HIERARCHY = 'type_hierarchy'
 POLICY_TRIGGERS = 'policy_triggers'
 POLICY_TYPES = 'policy_types'
 POLICIES = 'policies'
 GROUPS = 'groups'
 INPUTS = 'inputs'
@@ -80,37 +81,40 @@
 VERSION = 'version'
 CLOUDIFY = 'cloudify'
 
 SCRIPT_PLUGIN_NAME = 'script'
 SCRIPT_PLUGIN_RUN_TASK = 'script_runner.tasks.run'
 SCRIPT_PLUGIN_EXECUTE_WORKFLOW_TASK = 'script_runner.tasks.execute_workflow'
 SCRIPT_PATH_PROPERTY = 'script_path'
+SCRIPT_SOURCE_PROPERTY = 'script_source'
 
 FUNCTION_NAME_PATH_SEPARATOR = '__sep__'
 
 NODES = 'nodes'
 OPERATIONS = 'operations'
 NODE_INSTANCES = 'node_instances'
 
 IMPORT_RESOLVER_KEY = 'import_resolver'
 VALIDATE_DEFINITIONS_VERSION = 'validate_definitions_version'
 RESOLVER_IMPLEMENTATION_KEY = 'implementation'
 RESLOVER_PARAMETERS_KEY = 'parameters'
 
-TYPES_BASED_ON_DB_ENTITIES = [
+OBJECT_BASED_TYPES_DSL_1_4 = [
     'blueprint_id', 'deployment_id', 'capability_value', 'scaling_group',
-    'node_id', 'node_type', 'node_instance', 'secret_key'
-]
-TYPES_WHICH_REQUIRE_DEPLOYMENT_ID_CONSTRAINT = [
-    'capability_value', 'scaling_group',
-    'node_id', 'node_type', 'node_instance'
-]
+    'node_id', 'node_type', 'node_instance', 'secret_key', ]
+OBJECT_BASED_TYPES_DSL_1_5 = ['operation_name', ]
+OBJECT_BASED_TYPES = OBJECT_BASED_TYPES_DSL_1_4 + OBJECT_BASED_TYPES_DSL_1_5
+BLUEPRINT_OR_DEPLOYMENT_ID_CONSTRAINT_TYPES = \
+    ['scaling_group', 'operation_name', 'node_id', 'node_type']
+DEPLOYMENT_ID_CONSTRAINT_TYPES = \
+    ['capability_value', 'node_instance']
+ID_CONSTRAINT_TYPES = BLUEPRINT_OR_DEPLOYMENT_ID_CONSTRAINT_TYPES + \
+                      DEPLOYMENT_ID_CONSTRAINT_TYPES
 USER_PRIMITIVE_TYPES = ['string', 'integer', 'float', 'boolean', 'list',
-                        'dict', 'regex', 'textarea'] \
-                       + TYPES_BASED_ON_DB_ENTITIES
+                        'dict', 'regex', 'textarea'] + OBJECT_BASED_TYPES
 
 PLUGIN_DSL_KEYS_NOT_FROM_YAML = ['blueprint_labels', 'labels', 'resource_tags']
 PLUGIN_DSL_KEYS_READ_FROM_DB = PLUGIN_DSL_KEYS_NOT_FROM_YAML
 PLUGIN_DSL_KEYS_ADD_VALUES_NODE = ['blueprint_labels', 'labels']
 
 UNBOUNDED_LITERAL = 'UNBOUNDED'
 UNBOUNDED = -1
```

### Comparing `cloudify-common-6.4.2/dsl_parser/constraints.py` & `cloudify-common-7.0.0/dsl_parser/constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import re
 import numbers
 
-from dsl_parser._compat import text_type
 from dsl_parser import exceptions, utils
 from dsl_parser.constants import (
     INPUTS,
     DEFAULT,
     CONSTRAINTS as CONSTRAINT_CONST,
     TYPE,
     ITEM_TYPE,
-    TYPES_BASED_ON_DB_ENTITIES,
-    TYPES_WHICH_REQUIRE_DEPLOYMENT_ID_CONSTRAINT,
+    OBJECT_BASED_TYPES,
+    BLUEPRINT_OR_DEPLOYMENT_ID_CONSTRAINT_TYPES,
+    DEPLOYMENT_ID_CONSTRAINT_TYPES,
+    ID_CONSTRAINT_TYPES,
 )
 
 _NOT_COMPARABLE_ERROR_MSG = "Value is not comparable, the Constraint " \
                             "argument type  is '{0}' but value type is '{1}'."
 _NO_LENGTH_ERROR_MSG = "Value's length could not be computed. Value " \
                        "type is '{0}'."
 
@@ -95,19 +96,20 @@
 
     # The name of the operator as it appears in the YAML file.
     name = None
     # The data type of this constraint, what type of arguments it
     # accepts at it's initialization/definition.
     constraint_data_type = None
 
-    def __init__(self, args):
+    def __init__(self, args, error_message=None):
         """
         :param args: the constraint arguments.
         """
         self.args = args
+        self.error_message = error_message
 
     def predicate(self, value):
         """Value compliance hook.
 
         :param value: value to check the constraint with.
         :return: whether the value complies with this constraint.
         """
@@ -200,15 +202,16 @@
             _NOT_COMPARABLE_ERROR_MSG.format(
                 type(self.args).__name__, type(value).__name__))
 
 
 @register_constraint(name='valid_values', constraint_data_type=_SEQUENCE)
 class ValidValues(DataBasedConstraint):
     SUPPORTED_DATA_TYPES = ['capability_value', 'scaling_group',
-                            'node_id', 'node_type', 'node_instance']
+                            'node_id', 'node_type', 'node_instance',
+                            'operation_name', ]
 
     def predicate(self, value):
         return _try_predicate_func(
             lambda: value in self.args,
             "Value cannot be searched in the given "
             "valid values. Constraint argument type "
             "is '{0}' but value type is "
@@ -259,15 +262,15 @@
 
 @register_constraint(name='pattern', constraint_data_type=_REGEX)
 class Pattern(Constraint):
     # This class represents a regex constraint.
     # E.g. if self.args = 'abc' then calling `predicate` will only return True
     # when value = "abc".
     def predicate(self, value):
-        if not isinstance(value, text_type):
+        if not isinstance(value, str):
             raise exceptions.ConstraintException(
                 "Value must be of type string, got type "
                 "'{0}'".format(type(value).__name__))
         return bool(re.match(self.args, value))
 
 
 @register_constraint(name='filter_id', constraint_data_type=_STRING)
@@ -285,15 +288,16 @@
     SUPPORTED_DATA_TYPES = ['deployment_id', 'blueprint_id']
 
 
 @register_constraint(name='name_pattern', constraint_data_type=_DICT)
 class NamePattern(DataBasedConstraint):
     SUPPORTED_DATA_TYPES = ['deployment_id', 'blueprint_id', 'secret_key',
                             'capability_value', 'scaling_group',
-                            'node_id', 'node_type', 'node_instance']
+                            'node_id', 'node_type', 'node_instance',
+                            'operation_name', ]
 
     def query_param(self, data_type=None):
         if data_type == 'blueprint_id':
             return 'id_specs'
         elif data_type == 'deployment_id':
             return 'display_name_specs'
         elif data_type == 'secret_key':
@@ -304,25 +308,28 @@
             return 'type_specs'
         elif data_type == 'node_instance':
             return 'id_specs'
         elif data_type == 'capability_value':
             return 'capability_key_specs'
         elif data_type == 'scaling_group':
             return 'scaling_group_name_specs'
+        elif data_type == 'operation_name':
+            return 'operation_name_specs'
         else:
             raise NotImplementedError(
                 "'{0}' constraint is not implemented for data type '{1}'"
                 .format(self.name, data_type)
             )
 
 
 @register_constraint(name='deployment_id', constraint_data_type=_STRING)
 class DeploymentId(DataBasedConstraint):
     SUPPORTED_DATA_TYPES = ['capability_value', 'scaling_group',
-                            'node_id', 'node_type', 'node_instance']
+                            'node_id', 'node_type', 'node_instance',
+                            'operation_name', ]
 
 
 @register_validation_func(constraint_data_type=_SCALAR)
 def is_valid_scalar(arg):
     return isinstance(arg, numbers.Number) and not isinstance(arg, bool)
 
 
@@ -336,26 +343,26 @@
 @register_validation_func(constraint_data_type=_SEQUENCE)
 def is_valid_sequence(args):
     return isinstance(args, (list, tuple))
 
 
 @register_validation_func(constraint_data_type=_REGEX)
 def is_valid_regex(arg):
-    if not isinstance(arg, text_type):
+    if not isinstance(arg, str):
         return False
     try:
         re.compile(arg)
         return True
     except re.error:
         return False
 
 
 @register_validation_func(constraint_data_type=_STRING)
 def is_string(arg):
-    return isinstance(arg, text_type)
+    return isinstance(arg, str)
 
 
 @register_validation_func(constraint_data_type=_DICT)
 def is_dict(arg):
     return isinstance(arg, dict)
 
 
@@ -363,33 +370,37 @@
     """Validates the given constraint class arguments.
 
     :param constraint_cls: a Constraint class.
     :param args: the constraint operator arguments.
     :param ancestor: ancestor element of this constraint.
     :raises DSLParsingFormatException: in case of a violation.
     """
-    if utils.get_function(args) \
-            or not VALIDATION_FUNCTIONS[
-                constraint_cls.constraint_data_type](args):
+    if utils.get_function(args):
+        # allow functions to be constraint values. Those need to be
+        # evaluated before actually checking the constraints (when creating
+        # the deployment, with concrete input values).
+        return
+    if not VALIDATION_FUNCTIONS[constraint_cls.constraint_data_type](args):
         raise exceptions.DSLParsingLogicException(
             exceptions.ERROR_INVALID_CONSTRAINT_ARGUMENT,
             'Invalid constraint operator argument "{0}", for constraint '
             'operator "{1}" in '
             '"{2}".'.format(args, constraint_cls.name, ancestor))
 
 
 def parse(definition):
     """
     :param definition: a Constraint definition. A constraint is a dictionary
     with a single key-value pair, i.e. { constraint_operator_name: argument/s }
     :return: an instantiated Constraint.
     """
+    kwargs = {'error_message': definition.pop('error_message', None)}
     name, args = dict(definition).popitem()
     constraint_cls = CONSTRAINTS[name]
-    return constraint_cls(args)
+    return constraint_cls(args, **kwargs)
 
 
 def validate_input_value(input_name, input_constraints, input_value,
                          type_name, item_type_name, value_getter):
     if type_name != 'list' or not item_type_name:
         return _validate_input_value(
             input_name, input_constraints, input_value,
@@ -416,43 +427,55 @@
     if input_constraints and utils.get_function(input_value):
         raise exceptions.DSLParsingException(
             exceptions.ERROR_INPUT_WITH_FUNCS_AND_CONSTRAINTS,
             'Input value {0}, of input {1}, cannot contain an intrinsic '
             'function and also have '
             'constraints.'.format(input_value, input_name))
 
-    if type_name in TYPES_BASED_ON_DB_ENTITIES:
+    if type_name in OBJECT_BASED_TYPES:
         if not value_getter:
             raise exceptions.ConstraintException(
                 'Invalid call to validate_input_value: value_getter not set')
-        if type_name in TYPES_WHICH_REQUIRE_DEPLOYMENT_ID_CONSTRAINT \
+        if type_name in BLUEPRINT_OR_DEPLOYMENT_ID_CONSTRAINT_TYPES:
+            if value_getter.has_deployment_id() \
+                    or 'deployment_id' in {c.name for c in input_constraints}:
+                pass
+            elif value_getter.has_blueprint_id()\
+                    or 'blueprint_id' in {c.name for c in input_constraints}:
+                pass
+            else:
+                raise exceptions.ConstraintException(
+                    f"Input '{input_name}' of type '{type_name}' lacks "
+                    "'blueprint_id' or 'deployment_id' constraint.")
+        if type_name in DEPLOYMENT_ID_CONSTRAINT_TYPES \
                 and not value_getter.has_deployment_id() \
                 and 'deployment_id' not in {c.name for c in input_constraints}:
             raise exceptions.ConstraintException(
                 "Input '{0}' of type '{1}' lacks 'deployment_id' constraint."
                 .format(input_name, type_name))
-        if type_name not in TYPES_WHICH_REQUIRE_DEPLOYMENT_ID_CONSTRAINT \
+        if type_name not in ID_CONSTRAINT_TYPES \
                 or ('deployment_id' not in {c.name for c in input_constraints}
                     and value_getter.has_deployment_id()):
             matching_values = value_getter.get(type_name, input_value)
             if not any(v == input_value for v in matching_values or []):
                 raise exceptions.ConstraintException(
                     "Value '{0}' of '{1}' is not a valid value for data type "
                     "'{2}'.".format(input_value, input_name, type_name))
 
     data_based_constraints = []
     for c in input_constraints:
         if c.data_based(type_name):
             data_based_constraints.append(c)
             continue
         if not c.predicate(input_value):
+            msg = f'is invalid. {c.error_message}' if c.error_message \
+                else f'violates constraint {c}.'
             raise exceptions.ConstraintException(
-                "Value {0} of input {1} violates constraint "
-                "{2}.".format(input_value, input_name, c))
-    if ((type_name in TYPES_WHICH_REQUIRE_DEPLOYMENT_ID_CONSTRAINT
+                f"Value {input_value} of input {input_name} {msg}")
+    if ((type_name in DEPLOYMENT_ID_CONSTRAINT_TYPES
          or data_based_constraints)
         and not predicate_many(input_value,
                                type_name,
                                value_getter,
                                data_based_constraints)):
         raise exceptions.ConstraintException(
             "Value '{0}' of input '{1}' does not match any relevant entity "
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/__init__.py` & `cloudify-common-7.0.0/script_runner/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-########
-# Copyright (c) 2018 Cloudify Platform Ltd. All rights reserved
+#########
+# Copyright (c) 2014 GigaSpaces Technologies Ltd. All rights reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#        http://www.apache.org/licenses/LICENSE-2.0
+#       http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
-
-import numbers
-from dsl_parser._compat import text_type
-
-PRIMITIVE_TYPES = (list, bool, numbers.Number, text_type, dict)
+#  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  * See the License for the specific language governing permissions and
+#  * limitations under the License.
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/blueprint.py` & `cloudify-common-7.0.0/dsl_parser/elements/blueprint.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/data_types.py` & `cloudify-common-7.0.0/dsl_parser/elements/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,80 +13,76 @@
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import utils
 from dsl_parser import elements
 from dsl_parser import constants
 from dsl_parser import exceptions
-from dsl_parser._compat import text_type
 from dsl_parser.elements import types, version as _version
 from dsl_parser.framework.elements import (
     Element,
     Dict,
     DictElement,
     Leaf)
 from dsl_parser.framework.requirements import (
     Value,
     Requirement,
     sibling_predicate)
 
 
 class SchemaPropertyDescription(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class SchemaPropertyDisplayLabel(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
     requires = {
         _version.ToscaDefinitionsVersion: ['version'],
         'inputs': ['validate_version']
     }
 
     def validate(self, version, validate_version):
         if validate_version:
             self.validate_version(version, (1, 3))
 
 
 class SchemaPropertyType(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     # requires will be modified later.
     requires = {}
 
     provides = ['component_types']
 
-    def validate(self, data_type, **kwargs):
+    def validate(self, data_type, version=None, validate_version=None,
+                 **kwargs):
         if self.initial_value and self.initial_value not in \
                 constants.USER_PRIMITIVE_TYPES and not data_type:
             raise exceptions.DSLParsingLogicException(
                 exceptions.ERROR_UNKNOWN_TYPE,
                 "Illegal type name '{0}'".format(self.initial_value))
+        if not validate_version or not self.initial_value:
+            return
+        if self.initial_value in constants.OBJECT_BASED_TYPES_DSL_1_4:
+            self.validate_version(version, (1, 4))
+        elif self.initial_value in constants.OBJECT_BASED_TYPES_DSL_1_5:
+            self.validate_version(version, (1, 5))
 
     def calculate_provided(self, component_types, **kwargs):
         return {'component_types': component_types}
 
 
 class SchemaInputType(SchemaPropertyType):
-
-    def validate(self, data_type, version=None, validate_version=None,
-                 **kwargs):
-        if self.initial_value and self.initial_value not in \
-                constants.USER_PRIMITIVE_TYPES and not data_type:
-            raise exceptions.DSLParsingLogicException(
-                exceptions.ERROR_UNKNOWN_TYPE,
-                "Illegal type name '{0}'".format(self.initial_value))
-        if validate_version and self.initial_value and \
-                self.initial_value in constants.TYPES_BASED_ON_DB_ENTITIES:
-            self.validate_version(version, (1, 4))
+    pass
 
 
 class SchemaListItemType(SchemaPropertyType):
     def __init__(self, *args, **kwargs):
         super(SchemaListItemType, self).__init__(*args, **kwargs)
         self.requires.update({
             _version.ToscaDefinitionsVersion: ['version'],
@@ -204,20 +200,20 @@
 
 class SchemaWithInitialDefault(Schema):
     add_namespace_to_schema_elements = False
 
 
 class DataTypeDescription(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class DataTypeVersion(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class DataType(types.Type):
 
     schema = {
         'properties': SchemaWithInitialDefault,
         'description': DataTypeDescription,
@@ -305,11 +301,13 @@
     return source.initial_value == target.name
 
 
 SchemaPropertyType.requires[DataType] = [
     Value('data_type', predicate=_has_type, required=False),
     Requirement('component_types', predicate=_has_type, required=False)
 ]
+SchemaPropertyType.requires[_version.ToscaDefinitionsVersion] = ['version']
+SchemaPropertyType.requires['inputs'] = ['validate_version']
 SchemaInputType.requires[DataType] = [
     Value('data_type', predicate=_has_type, required=False),
     Requirement('component_types', predicate=_has_type, required=False)
 ]
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/deployment_schedules.py` & `cloudify-common-7.0.0/dsl_parser/elements/deployment_schedules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from datetime import datetime
 
-from dsl_parser._compat import text_type
 from dsl_parser import exceptions
 from dsl_parser.framework.elements import (DictElement,
                                            DictNoDefaultElement,
                                            Element,
                                            Leaf,
                                            List,
                                            Dict)
@@ -22,40 +21,40 @@
 
 class ScheduleCount(Element):
     schema = Leaf(type=int)
 
 
 class ScheduleName(Element):
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class DateTimeExpression(Element):
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class RequiredDateTimeExpression(DateTimeExpression):
     required = True
 
 
 class TimeDelta(Element):
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     def validate(self):
         if self.initial_value:
             unpack_timedelta_string(self.initial_value)
 
 
 class TimeZoneExpression(Element):
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class ScheduledWorkflowId(Element):
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class ScheduledWorkflowForce(Element):
     schema = Leaf(type=bool)
 
 
 class ScheduledWorkflowDryRun(Element):
@@ -98,15 +97,15 @@
                 if isinstance(value, dict) and 'get_attribute' in value:
                     value_msg = ' from the value of {}'.format(key)
                     raise exceptions.DSLParsingException(
                         1, err_msg.format('contain', value_msg))
 
 
 class Weekday(Element):
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     def validate(self):
         weekdays_list = ['su', 'mo', 'tu', 'we', 'th', 'fr', 'sa']
         err_msg = "{0} is not a valid weekday value. Accepted values: {1}"
         weekday_value = self.initial_value.lower()[-2:]
         if weekday_value not in weekdays_list:
             raise exceptions.DSLParsingException(
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/imports.py` & `cloudify-common-7.0.0/dsl_parser/elements/imports.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import os
+from collections import deque, OrderedDict
+from typing import Iterable, Tuple, Optional
 
-from networkx.algorithms import topological_sort
-from networkx.classes import DiGraph
+from urllib.request import pathname2url
 
 from cloudify.exceptions import InvalidBlueprintImport
 
 from dsl_parser import (exceptions,
                         constants,
                         version as _version,
                         utils)
-from dsl_parser._compat import text_type
 from dsl_parser.holder import Holder
-from dsl_parser._compat import pathname2url
 from dsl_parser.import_resolver.abstract_import_resolver import\
-    is_remote_resource
-from dsl_parser.framework.elements import (Element,
+    is_remote_resource, AbstractImportResolver
+from dsl_parser.framework.elements import (Dict,
+                                           DictElement,
+                                           Element,
                                            Leaf,
                                            List)
+from dsl_parser.utils import get_function
 
 
 MERGE_NO_OVERRIDE = set([
     constants.INTERFACES,
     constants.NODE_TYPES,
     constants.PLUGINS,
     constants.WORKFLOWS,
@@ -66,25 +68,58 @@
     constants.IMPORTS,
     _version.VERSION
 ])
 
 
 class Import(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class Imports(Element):
 
     schema = List(type=Import)
 
 
+class ImportPluginProperty(Element):
+    schema = Leaf(type=(str, int, float, bool, list, dict))
+
+    requires = {
+        'inputs': ['validate_version', 'version'],
+    }
+
+    def validate(self, version, validate_version, **kwargs):
+        if validate_version:
+            self.validate_version(version.definitions_version, (1, 5))
+        if isinstance(self.initial_value, (str, int, float, bool, list)):
+            return
+        if isinstance(self.initial_value, dict) \
+                and get_function(self.initial_value):
+            return
+        raise exceptions.DSLParsingFormatException(
+            exceptions.ERROR_INVALID_IMPORT_SPECS,
+            'Properties of imported node should either be strings, integers, '
+            'floats, booleans, lists or intrinsic functions')
+
+
+class ImportPluginProperties(DictElement):
+    schema = Dict(type=ImportPluginProperty)
+
+    requires = {
+        'inputs': ['validate_version', 'version'],
+    }
+
+    def validate(self, version, validate_version, **kwargs):
+        if validate_version:
+            self.validate_version(version.definitions_version, (1, 5))
+
+
 class ImportLoader(Element):
 
-    schema = Leaf(type=text_type)
+    schema = [Leaf(type=str), Dict(type=ImportPluginProperties)]
 
 
 class ImportsLoader(Element):
 
     schema = List(type=ImportLoader)
     provides = ['resource_base']
     requires = {
@@ -98,18 +133,28 @@
 
     resource_base = None
 
     def validate(self, **kwargs):
         imports = [i.value for i in self.children()]
         imports_set = set()
         for _import in imports:
-            if _import in imports_set:
+            if isinstance(_import, str):
+                import_key = _import
+            elif isinstance(_import, dict):
+                import_key = _validate_import_dict(_import)
+            else:
+                raise exceptions.DSLParsingFormatException(
+                    exceptions.ERROR_INVALID_IMPORT_SPECS,
+                    'The import statement should be either a string '
+                    'or a dictionary'
+                )
+            if import_key in imports_set:
                 raise exceptions.DSLParsingFormatException(
                     2, 'Duplicate imports')
-            imports_set.add(_import)
+            imports_set.add(import_key)
 
     def parse(self,
               main_blueprint_holder,
               resources_base_path,
               blueprint_location,
               version,
               resolver,
@@ -133,16 +178,16 @@
         return {
             'resource_base': self.resource_base
         }
 
 
 def _dsl_location_to_url(dsl_location, resources_base_path):
     if dsl_location is not None:
-        dsl_location = _get_resource_location(dsl_location,
-                                              resources_base_path)
+        dsl_location = next(
+            _get_resource_location(dsl_location, resources_base_path))
         if dsl_location is None:
             ex = exceptions.DSLParsingLogicException(
                 30, "Failed converting dsl "
                     "location to url: no suitable "
                     "location found "
                     "for dsl '{0}'"
                     .format(dsl_location))
@@ -152,334 +197,384 @@
 
 
 def _get_resource_location(resource_name,
                            resources_base_path,
                            current_resource_context=None,
                            dsl_version=None):
     if is_remote_resource(resource_name):
-        return resource_name
+        yield resource_name
+        return
 
     for fn in _possible_resource_locations(resource_name, dsl_version):
         if os.path.exists(fn):
-            return 'file:{0}'.format(pathname2url(os.path.abspath(fn)))
+            yield f'file:{pathname2url(os.path.abspath(fn))}'
 
     if current_resource_context:
         candidate_url = current_resource_context[
             :current_resource_context.rfind('/') + 1] + resource_name
-        if utils.url_exists(candidate_url):
-            return candidate_url
+        yield candidate_url
 
     if resources_base_path:
         full_path = os.path.join(resources_base_path, resource_name)
         for fn in _possible_resource_locations(full_path, dsl_version):
             if os.path.exists(fn):
-                return 'file:{0}'.format(pathname2url(os.path.abspath(fn)))
-        return 'file:{0}'.format(
-            pathname2url(os.path.abspath(full_path)))
+                yield f'file:{pathname2url(os.path.abspath(fn))}'
 
-    return None
+    for fn in _possible_resource_locations(resource_name, dsl_version):
+        yield f'resource:{fn}'
 
 
 def _possible_resource_locations(resource_name, dsl_version):
     if not dsl_version:
         return [resource_name]
     filename, ext = os.path.splitext(resource_name)
     return ['{0}_{1}{2}'.format(filename, dsl_version, ext), resource_name]
 
 
-def _extract_import_parts(import_url,
-                          resources_base_path,
-                          current_resource_context=None,
-                          dsl_version=None):
-    """
-    :param import_url: a string which is the import path
-    :param resources_base_path: In case of a relative file path, this
-                                is the base path.
-    :param current_resource_context: Current import statement,
-    :param dsl_version: DSL version used by the root blueprint.
-    :return: Will return a breakdown of the URL to
-            (namespace, import_url). If the import is not
-            namespaced, the returned namespace will be
-            None.
-    """
-    namespace, _, import_url = \
-        import_url.rpartition(constants.NAMESPACE_DELIMITER)
-
-    if namespace == '':
-        # The mark of no namespace is None, so we need to use that value.
-        namespace = None
-
-    return namespace, _get_resource_location(import_url,
-                                             resources_base_path,
-                                             current_resource_context,
-                                             dsl_version)
-
-
 def _insert_imported_list(blueprint_holder, blueprints_imported):
-    key_holder = Holder(constants.IMPORTED_BLUEPRINTS)
-    blueprint_holder.value[key_holder] = Holder([])
-    value_holder = blueprint_holder.value[key_holder]
-
-    for import_url in blueprints_imported:
-        value_holder.value.append(Holder(import_url))
-
-
-def _insert_namespaces_mapping(blueprint_holder, mapping):
-    key_holder = Holder(constants.NAMESPACES_MAPPING)
-    blueprint_holder.value[key_holder] = Holder({})
-    value_holder = blueprint_holder.value[key_holder]
-
-    for namespace, blueprint_id in mapping.items():
-        namespace_holder = Holder(namespace)
-        value_holder.value[namespace_holder] = Holder(blueprint_id)
+    blueprint_holder.set_item(
+        constants.IMPORTED_BLUEPRINTS,
+        list(blueprints_imported.values())
+    )
+    blueprint_holder.set_item(
+        constants.NAMESPACES_MAPPING,
+        blueprints_imported,
+    )
 
 
 def _combine_imports(parsed_dsl_holder, dsl_location,
                      resources_base_path, version, resolver,
                      validate_version):
-    ordered_imports, blueprint_imports, mapping = _build_ordered_imports(
+    ordered_imports, mapping = _build_ordered_imports(
         parsed_dsl_holder,
         dsl_location,
         resources_base_path,
         resolver)
     holder_result = parsed_dsl_holder.copy()
     version_key_holder, version_value_holder = parsed_dsl_holder.get_item(
         _version.VERSION)
     holder_result.value = {}
-    _insert_imported_list(holder_result, blueprint_imports)
-    _insert_namespaces_mapping(holder_result, mapping)
+    _insert_imported_list(holder_result, mapping)
     for imported in ordered_imports:
-        import_url, namespace = imported['import']
-        parsed_imported_dsl_holder = imported['parsed']
+        parsed_imported_dsl_holder = imported.parsed
         if validate_version:
             _validate_version(version.raw,
-                              import_url,
+                              imported.url,
                               parsed_imported_dsl_holder)
-        is_cloudify_types = imported['cloudify_types']
+        if imported.url != constants.ROOT_ELEMENT_VALUE:
+            _validate_and_set_properties(
+                parsed_imported_dsl_holder, imported.properties)
+        is_cloudify_types = imported.is_cloudify_types
         _merge_parsed_into_combined(
             holder_result, parsed_imported_dsl_holder,
-            version, namespace, is_cloudify_types)
+            version, imported.namespace, is_cloudify_types)
     holder_result.value[version_key_holder] = version_value_holder
     return holder_result
 
 
 def _dsl_version(parsed_dsl_holder):
     version = parsed_dsl_holder.get_item('tosca_definitions_version')
     if version:
         version = version[1].value
     if version.startswith('cloudify_dsl_'):
         return version.replace('cloudify_dsl_', '', 1)
 
 
-def _build_ordered_imports(parsed_dsl_holder,
-                           dsl_location,
-                           resources_base_path,
-                           resolver):
+def is_parsed_resource(item):
+    """
+    Checking if the given item is in parsed yaml type.
+    """
+    return isinstance(item, Holder)
 
-    def location(value):
-        return value or constants.ROOT_ELEMENT_VALUE
 
-    def is_parsed_resource(item):
-        """
-        Checking if the given item is in parsed yaml type.
-        """
-        return isinstance(item, Holder)
+def validate_namespace(namespace):
+    """
+    The namespace delimiter is not allowed in the namespace.
+    """
+    if namespace and constants.NAMESPACE_DELIMITER in namespace:
+        raise exceptions.DSLParsingLogicException(
+            212,
+            'Invalid {0}: import\'s namespace cannot'
+            'contain namespace delimiter'.format(namespace))
 
-    def validate_namespace(namespace):
-        """
-        The namespace delimiter is not allowed in the namespace.
-        """
-        if namespace and constants.NAMESPACE_DELIMITER in namespace:
-            raise exceptions.DSLParsingLogicException(
-                212,
-                'Invalid {0}: import\'s namespace cannot'
-                'contain namespace delimiter'.format(namespace))
 
-    def is_cloudify_basic_types(imported_holder):
-        """
-        Cloudify basic types can be recognized with the following rules
-        at high assurance:
-        - Has a metadata field named cloudify_types.
-        - Has a node type named cloudify.nodes.Root (for backward capability).
-        """
-        _, metadata = imported_holder.get_item(constants.METADATA)
-        _, node_types = imported_holder.get_item(constants.NODE_TYPES)
-        if (metadata and metadata.get_item('cloudify_types')[1]) or node_types:
-            root_type = node_types.get_item('cloudify.nodes.Root')[1]
-            if root_type and not root_type.is_cloudify_type:
-                # If it was already marked with the flag,
-                # this means that this blueprint is using Cloudify basic types
-                # and not equal to it.
-                return True
-        return False
-
-    def validate_import_namespace(namespace,
-                                  cloudify_basic_types,
-                                  context_namespace):
-        """
-        Cloudify basic types can not be imported with namespace,
-        due to that will disrupt core Cloudify types with the namespace prefix
-        which will not allow proper functioning, like: added a prefix to
-        install workflow.
-        """
-        if cloudify_basic_types and namespace:
-            if not context_namespace or namespace != context_namespace:
-                raise exceptions.DSLParsingLogicException(
-                    214,
-                    'Invalid import namespace {0}: cannot be used'
-                    ' on Cloudify basic types.'.format(namespace))
+def is_cloudify_basic_types(imported_holder):
+    """
+    Cloudify basic types can be recognized with the following rules
+    at high assurance:
+    - Has a metadata field named cloudify_types.
+    - Has a node type named cloudify.nodes.Root (for backward capability).
+    """
+    _, metadata = imported_holder.get_item(constants.METADATA)
+    _, node_types = imported_holder.get_item(constants.NODE_TYPES)
+    if (metadata and metadata.get_item('cloudify_types')[1]) or node_types:
+        root_type = node_types.get_item('cloudify.nodes.Root')[1]
+        if root_type and not root_type.is_cloudify_type:
+            # If it was already marked with the flag,
+            # this means that this blueprint is using Cloudify basic types
+            # and not equal to it.
+            return True
+    return False
 
-    def resolve_import_graph_key(import_url, namespace):
-        """
-        An import's key in the graph key is a combination with
-        it's namespace and it, but in case that the import is
-        Cloudify basic types the key is without the namespace.
-        """
-        import_key = (import_url, namespace)
-        if import_key in imports_graph:
-            return import_key
-        # In case, of Cloudify basic types
-        import_key = (import_key, None)
-        if import_key in imports_graph:
-            return import_key
-        return import_url, namespace
 
-    def validate_blueprint_import_namespace(namespace, import_url):
-        """
-        Blueprint import must be used with namespace, this is enforced for
-        enabling the use of scripts from the imported blueprint which needs
-        the namespace for maintaining the path to the scripts.
-        """
-        if not namespace:
+def validate_import_namespace(namespace,
+                              cloudify_basic_types,
+                              context_namespace):
+    """
+    Cloudify basic types can not be imported with namespace,
+    due to that will disrupt core Cloudify types with the namespace prefix
+    which will not allow proper functioning, like: added a prefix to
+    install workflow.
+    """
+    if cloudify_basic_types and namespace:
+        if not context_namespace or namespace != context_namespace:
             raise exceptions.DSLParsingLogicException(
-                213,
-                'Invalid {0}: blueprint import cannot'
-                'be used without namespace'.format(import_url))
+                214,
+                'Invalid import namespace {0}: cannot be used'
+                ' on Cloudify basic types.'.format(namespace))
 
-    def add_namespace_to_mapping(blueprint_id, namespace):
-        """
-        The mapping is saved only for namespaced blueprint import
-        in order of supporting imported scripts, so one-to-one
-        mapping (blueprint-namespace) is a must for to be able to
-        pull the scripts.
-        """
-        if namespaces_mapping.get(namespace, None):
-            raise exceptions.DSLParsingLogicException(
-                214, "Import failed {0}: can not use the same"
-                     " namespace for importing blueprints".format(namespace))
-        namespaces_mapping[namespace] = blueprint_id
-
-    def build_ordered_imports_recursive(_current_parsed_dsl_holder,
-                                        _current_import,
-                                        context_namespace=None,
-                                        dsl_version=None):
-        imports_key_holder, imports_value_holder = _current_parsed_dsl_holder.\
-            get_item(constants.IMPORTS)
+
+def validate_blueprint_import_namespace(namespace, import_url):
+    """
+    Blueprint import must be used with namespace, this is enforced for
+    enabling the use of scripts from the imported blueprint which needs
+    the namespace for maintaining the path to the scripts.
+    """
+    if not namespace:
+        raise exceptions.DSLParsingLogicException(
+            213,
+            'Invalid {0}: blueprint import cannot'
+            'be used without namespace'.format(import_url))
+
+
+def _normalize_plugin_import(plugin, imported_dsl, namespace):
+    utils.remove_dsl_keys(
+        imported_dsl,
+        constants.PLUGIN_DSL_KEYS_NOT_FROM_YAML)
+    for key in constants.PLUGIN_DSL_KEYS_READ_FROM_DB:
+        if not plugin.get(key):
+            continue
+        value = plugin[key]
+        if key in constants.PLUGIN_DSL_KEYS_ADD_VALUES_NODE:
+            value = utils.add_values_node_description(value)
+        _merge_into_dict_or_throw_on_duplicate(
+            Holder.of({key: value}),
+            imported_dsl,
+            key,
+            namespace)
+
+
+class _ImportedDSL:
+    """Represents one imported DSL file.
+
+    This is only useful when fetching the imports, in order to keep track
+    of which ones were already downloaded, and to traverse the import tree.
+    """
+    url: str
+    parsed: Optional[Holder]
+    namespace: Optional[str]
+    properties: Optional[dict]
+
+    def __init__(
+        self,
+        url,
+        parsed=None,
+        namespace=None,
+        properties=None,
+    ):
+        self.url = url
+        self.parsed = parsed
+        self.namespace = namespace
+        self.properties = properties
+
+    @property
+    def key(self) -> Tuple[str, Optional[str]]:
+        return (self.url, self.namespace)
+
+    @property
+    def dsl_version(self) -> str:
+        return _dsl_version(self.parsed)
+
+    @property
+    def is_cloudify_types(self) -> bool:
+        return is_cloudify_basic_types(self.parsed)
+
+    def get_imports(self) -> Iterable[Tuple[str, Optional[dict]]]:
+        _, imports_value_holder = self.parsed.get_item(constants.IMPORTS)
         if not imports_value_holder:
             return
-
-        for another_import in imports_value_holder.restore():
-            namespace, import_url = _extract_import_parts(another_import,
-                                                          resources_base_path,
-                                                          _current_import,
-                                                          dsl_version)
-            validate_namespace(namespace)
-            if context_namespace:
-                if namespace:
-                    namespace = utils.generate_namespaced_value(
-                        context_namespace,
-                        namespace)
-                else:
-                    # In case a namespace was added earlier in the import
-                    # chain.
-                    namespace = context_namespace
-            if import_url is None:
-                ex = exceptions.DSLParsingLogicException(
-                    13, "Import failed: no suitable location found for "
-                        "import '{0}'".format(another_import))
-                ex.failed_import = another_import
-                raise ex
-
-            if utils.is_blueprint_import(import_url):
-                validate_blueprint_import_namespace(namespace, import_url)
-                blueprint_id = utils.remove_blueprint_import_prefix(import_url)
-                blueprint_imports.add(blueprint_id)
-                add_namespace_to_mapping(blueprint_id, namespace)
-
-            import_key = resolve_import_graph_key(import_url, namespace)
-            import_context = (location(_current_import), context_namespace)
-            if import_key in imports_graph:
-                is_cloudify_types = imports_graph[import_key]['cloudify_types']
-                validate_import_namespace(namespace,
-                                          is_cloudify_types,
-                                          context_namespace)
-                imports_graph.add_graph_dependency(
-                    import_url,
-                    import_context,
-                    namespace)
+        for raw_import in imports_value_holder.restore():
+            if isinstance(raw_import, dict):
+                # This is actually guaranteed to be a dict of length 1
+                yield list(raw_import.items())[0]
             else:
-                imported_dsl = resolver.fetch_import(import_url,
-                                                     dsl_version=dsl_version)
-                if not is_parsed_resource(imported_dsl):
-                    imported_dsl = utils.load_yaml(
-                        raw_yaml=imported_dsl,
-                        error_message="Failed to parse import '{0}'"
-                                      "(via '{1}')"
-                                      .format(another_import, import_url),
-                        filename=import_url)
-                try:
-                    plugin = resolver.retrieve_plugin(import_url,
-                                                      dsl_version=dsl_version)
-                except InvalidBlueprintImport:
-                    plugin = None
-                if plugin:
-                    # If it is a plugin, then use labels and tags from the DB
-                    utils.remove_dsl_keys(
-                        imported_dsl,
-                        constants.PLUGIN_DSL_KEYS_NOT_FROM_YAML)
-                    for key in constants.PLUGIN_DSL_KEYS_READ_FROM_DB:
-                        if not plugin.get(key):
-                            continue
-                        value = plugin[key]
-                        if key in constants.PLUGIN_DSL_KEYS_ADD_VALUES_NODE:
-                            value = utils.add_values_node_description(value)
-                        _merge_into_dict_or_throw_on_duplicate(
-                            Holder.of({key: value}),
-                            imported_dsl,
-                            key,
-                            namespace)
-                cloudify_basic_types = is_cloudify_basic_types(imported_dsl)
-                validate_import_namespace(namespace,
-                                          cloudify_basic_types,
-                                          context_namespace)
-                if cloudify_basic_types:
-                    # Remove namespace data from import
-                    namespace = None
-                imports_graph.add(
-                    import_url,
-                    imported_dsl,
-                    cloudify_basic_types,
-                    import_context,
-                    namespace)
-                build_ordered_imports_recursive(imported_dsl,
-                                                import_url,
-                                                namespace,
-                                                dsl_version)
+                yield raw_import, None
 
-    imports_graph = ImportsGraph()
-    blueprint_imports = set()
-    namespaces_mapping = {}
 
-    imports_graph.add(location(dsl_location), parsed_dsl_holder)
-    build_ordered_imports_recursive(
-        parsed_dsl_holder, dsl_location,
-        dsl_version=_dsl_version(parsed_dsl_holder)
+def _prefix_namespace(parent_namespace, namespace):
+    validate_namespace(namespace)
+    if parent_namespace and namespace:
+        return utils.generate_namespaced_value(parent_namespace, namespace)
+    else:
+        return parent_namespace or namespace
+
+
+def _split_import_namespace(import_url):
+    namespace, _, resolved_url = \
+        import_url.rpartition(constants.NAMESPACE_DELIMITER)
+    if namespace:
+        validate_namespace(namespace)
+    else:
+        namespace = None
+    return namespace, resolved_url
+
+
+def _fetch_import(
+    original_import_url: str,
+    resolver: AbstractImportResolver,
+    parent: _ImportedDSL,
+    resources_base_path: str,
+    properties: dict,
+    dsl_version: str,
+    namespaces_mapping: dict,
+    already_imported: dict,
+) -> Optional[dict]:
+    """Fetch and parse a single import
+
+    Based on the import url, and all the additional required details,
+    return the parsed DSL (or None if this DSL was already imported before).
+    If the url cannot be resolved, an error is raised.
+    """
+    namespace, resolved_url = \
+        _split_import_namespace(original_import_url)
+    namespace = _prefix_namespace(parent.namespace, namespace)
+    import_urls = _get_resource_location(
+        resolved_url,
+        resources_base_path,
+        parent.url,
+        dsl_version,
     )
-    sorted_imports_graph = imports_graph.topological_sort()
-    return sorted_imports_graph, blueprint_imports, namespaces_mapping
+
+    fetch_error = None
+    for import_url in import_urls:
+        next_item = _ImportedDSL(
+            url=import_url,
+            namespace=namespace,
+            properties=properties,
+        )
+        if next_item.key in already_imported:
+            # this was already seen! let's just check the namespace
+            validate_import_namespace(
+                namespace,
+                already_imported[next_item.key].is_cloudify_types,
+                parent.namespace,
+            )
+            return None
+
+        if utils.is_blueprint_import(import_url):
+            validate_blueprint_import_namespace(namespace, import_url)
+            blueprint_id = \
+                utils.remove_blueprint_import_prefix(import_url)
+            if namespaces_mapping.get(namespace):
+                raise exceptions.DSLParsingLogicException(
+                    214,
+                    f'Import failed {namespace}: can not use the same'
+                    'namespace for importing blueprints'
+                )
+            namespaces_mapping[namespace] = blueprint_id
+
+        # here we actually fetch and parse the DSL
+        try:
+            imported_dsl = resolver.fetch_import(
+                import_url,
+                dsl_version=dsl_version,
+            )
+        except Exception as exc:
+            fetch_error = exc
+            continue
+
+        if not is_parsed_resource(imported_dsl):
+            imported_dsl = utils.load_yaml(
+                raw_yaml=imported_dsl,
+                error_message="Failed to parse import '{0}'"
+                              "(via '{1}')"
+                              .format(original_import_url, import_url),
+                filename=import_url)
+
+        # if this was a plugin import, the DSL needs to be massaged a bit...
+        try:
+            plugin = resolver.retrieve_plugin(
+                import_url,
+                dsl_version=dsl_version,
+            )
+        except InvalidBlueprintImport:
+            plugin = None
+        if plugin:
+            # If it is a plugin, then use labels and tags from the DB
+            _normalize_plugin_import(plugin, imported_dsl, namespace)
+
+        if utils.is_blueprint_import(import_url):
+            namespaces_mapping[namespace] = blueprint_id
+
+        next_item.parsed = imported_dsl
+        validate_import_namespace(next_item.namespace,
+                                  next_item.is_cloudify_types,
+                                  parent.namespace)
+        if next_item.is_cloudify_types:
+            # Remove namespace data from import
+            next_item.namespace = None
+        return next_item
+
+    if fetch_error:
+        # if we weren't able to fetch the imported dsl, and we did see an
+        # error in fetching, reraise that
+        raise fetch_error
+    ex = exceptions.DSLParsingLogicException(
+        13, "Import failed: no suitable location found for "
+            "import '{0}'".format(original_import_url))
+    ex.failed_import = original_import_url
+    raise ex
+
+
+def _build_ordered_imports(parsed_dsl_holder,
+                           dsl_location,
+                           resources_base_path,
+                           resolver):
+    namespaces_mapping = {}
+    root_dsl = _ImportedDSL(url=dsl_location, parsed=parsed_dsl_holder)
+
+    # this is an OrderedDict and not just a list,
+    ordered_imports = OrderedDict([
+        (root_dsl.key, root_dsl),
+    ])
+
+    # BFS over the imports. Necessarily, the traversal order will be such
+    # that parent imports come before child imports (i.e. if A import B,
+    # A comes before B)
+    to_visit = deque([root_dsl])
+    while to_visit:
+        parent = to_visit.popleft()
+
+        for original_import_url, properties in parent.get_imports():
+            next_item = _fetch_import(
+                original_import_url,
+                resolver,
+                parent,
+                resources_base_path,
+                properties,
+                root_dsl.dsl_version,
+                namespaces_mapping,
+                ordered_imports,
+            )
+
+            if next_item:
+                ordered_imports[next_item.key] = next_item
+                to_visit.append(next_item)
+
+    return ordered_imports.values(), namespaces_mapping
 
 
 def _validate_version(dsl_version,
                       import_url,
                       parsed_imported_dsl_holder):
     version_key_holder, version_value_holder = parsed_imported_dsl_holder\
         .get_item(_version.VERSION)
@@ -492,14 +587,78 @@
                 "version is '{0}', import with different version is "
                 "'{1}', version of problematic import is '{2}'"
                 .format(dsl_version,
                         import_url,
                         version_value_holder.value))
 
 
+def _validate_and_set_properties(parsed_imported_dsl_holder, properties):
+    _, plugins = parsed_imported_dsl_holder.get_item('plugins')
+    if not plugins:
+        return
+    for plugin_name in plugins.keys():
+        _, plugin = plugins.get_item(plugin_name)
+        if plugin:
+            _validate_and_set_plugin_properties(plugin, properties)
+
+
+def _validate_and_set_plugin_properties(plugin_dsl_holder, properties):
+    _, plugin_properties = plugin_dsl_holder.get_item('properties')
+    if not plugin_properties:
+        return
+    invalid_types = []
+    redundant_properties = list(properties.keys()) if properties else []
+    for property_name in plugin_properties.keys():
+        _, plugin_property = plugin_properties.get_item(property_name)
+        _, property_type = plugin_property.get_item('type')
+        if properties and property_name in properties:
+            redundant_properties.remove(property_name)
+            if _is_type_valid(properties[property_name], property_type.value):
+                plugin_property.set_item('value', properties[property_name])
+            elif get_function(properties[property_name]):
+                plugin_property.set_item('value', properties[property_name])
+            else:
+                invalid_types.append(
+                    f"Property {property_name}: value "
+                    f"'{properties[property_name]}' should be of type "
+                    f"{property_type.value}"
+                )
+    errors = []
+    if invalid_types:
+        errors.extend(invalid_types)
+    if redundant_properties:
+        errors.append(
+            'Properties for imported plugin are redundant: '
+            f'{redundant_properties}, consider updating import lines'
+        )
+    if errors:
+        raise exceptions.DSLParsingLogicException(
+            exceptions.ERROR_INVALID_IMPORT_PROPERTIES,
+            '.  '.join(errors)
+            )
+
+
+def _is_type_valid(obj, type_name):
+    if type_name == 'string':
+        return isinstance(obj, (str, int))
+    elif type_name == 'integer':
+        return isinstance(obj, int)
+    elif type_name == 'float':
+        return isinstance(obj, (int, float))
+    elif type_name == 'boolean':
+        return isinstance(obj, bool)
+    elif type_name == 'list':
+        return isinstance(obj, list)
+    else:
+        raise exceptions.DSLParsingFormatException(
+            exceptions.ERROR_INVALID_IMPORT_SPECS,
+            'Properties should either be strings, integers, '
+            'floats, booleans, or lists.')
+
+
 def _can_import_version(version_orig, version_imported):
     """Accept importing a file which uses equal or earlier DSL version."""
     return _version.SUPPORTED_VERSIONS.index(version_orig) >= \
         _version.SUPPORTED_VERSIONS.index(version_imported)
 
 
 def _mark_key_value_holder_items(value_holder, field_name, field_value):
@@ -577,15 +736,15 @@
             raise exceptions.DSLParsingLogicException(
                 3, msg.format(key_holder.value))
 
 
 def _prepare_namespaced_elements(key_holder, namespace, value_holder):
     if isinstance(value_holder.value, dict):
         _mark_key_value_holder_items(value_holder, 'namespace', namespace)
-    elif isinstance(value_holder.value, text_type):
+    elif isinstance(value_holder.value, str):
         # In case of primitive type we a need a different way to mark
         # the sub elements with the namespace, but leaving the option
         # for the DSL element to not receive the namespace.
         value_holder.only_children_namespace = True
 
         value_holder.namespace = namespace
     if not utils.check_if_overridable_cloudify_type(key_holder.value):
@@ -631,15 +790,15 @@
         4, "Import failed: Could not merge '{0}' due to conflict "
            "on '{1}'".format(key_name, key_holder.value))
 
 
 def _extend_node_template(from_dict_holder, to_dict_holder):
     for key_holder, value_holder in from_dict_holder.value.items():
         if (isinstance(value_holder.value, dict) or
-                isinstance(value_holder.value, text_type)):
+                isinstance(value_holder.value, str)):
             to_dict_holder.value[key_holder] = value_holder
         elif (isinstance(value_holder.value, list) and
               key_holder.value == constants.RELATIONSHIPS):
             _extend_list_with_namespaced_values(
                 value_holder.namespace,
                 value_holder,
                 to_dict_holder.value[key_holder])
@@ -692,41 +851,13 @@
             )
         else:
             raise exceptions.DSLParsingLogicException(
                 4, "Import failed: Could not merge '{0}' due to conflict "
                    "on '{1}'".format(key_name, key_holder.value))
 
 
-class ImportsGraph(object):
-
-    def __init__(self):
-        self._imports_tree = DiGraph()
-        self._imports_graph = DiGraph()
-
-    def add(self, import_url, parsed, cloudify_types=False,
-            via_import=None, namespace=None):
-        node_key = (import_url, namespace)
-        if import_url not in self._imports_tree:
-            self._imports_tree.add_node(
-                node_key, parsed=parsed, cloudify_types=cloudify_types)
-            self._imports_graph.add_node(
-                node_key, parsed=parsed, cloudify_types=cloudify_types)
-        if via_import:
-            self._imports_tree.add_edge(node_key, via_import)
-            self._imports_graph.add_edge(node_key, via_import)
-
-    def add_graph_dependency(self, import_url, via_import, namespace):
-        if via_import:
-            self._imports_graph.add_edge((import_url, namespace), via_import)
-
-    def topological_sort(self):
-        return reversed(list(
-            ({'import': i,
-             'parsed': self._imports_tree.node[i]['parsed'],
-              'cloudify_types': self._imports_tree.node[i]['cloudify_types']}
-             for i in topological_sort(self._imports_tree))))
-
-    def __contains__(self, item):
-        return item in self._imports_tree
-
-    def __getitem__(self, item):
-        return self._imports_tree.node[item]
+def _validate_import_dict(_import):
+    if len(_import) != 1:
+        raise exceptions.DSLParsingFormatException(
+            exceptions.ERROR_INVALID_IMPORT_SPECS,
+            'Import with properties should be a single-entry dictionary')
+    return list(_import.keys())[0]
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/inputs.py` & `cloudify-common-7.0.0/dsl_parser/elements/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,45 +10,61 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import exceptions, constraints, utils
+from dsl_parser.elements import version as _version
 from dsl_parser.elements.data_types import (Schema,
                                             SchemaProperty,
                                             SchemaInputType,
                                             SchemaListItemType,
                                             SchemaPropertyDefault,
                                             SchemaPropertyDescription,
                                             SchemaPropertyDisplayLabel,
                                             SchemaPropertyHidden,
                                             SchemaPropertyRequired,
                                             )
 from dsl_parser.framework.elements import Element, Leaf, List, Dict
 from dsl_parser.framework.requirements import Requirement, sibling_predicate
+from dsl_parser.version import version_description
 
 
 class Constraint(Element):
     schema = Leaf(type=dict)
 
     add_namespace_to_schema_elements = False
 
-    def validate(self, **kwargs):
+    requires = {
+        _version.ToscaDefinitionsVersion: ['version'],
+        'inputs': ['validate_version']
+    }
+
+    def validate(self, version, validate_version, **kwargs):
         constraint_op_keys = list(self.initial_value)
         if not constraint_op_keys:
             raise exceptions.DSLParsingLogicException(
                 exceptions.ERROR_UNKNOWN_TYPE,
                 "Empty constraint operator name given. Allowed operators: "
                 "{0}".format(constraints.CONSTRAINTS))
         if len(constraint_op_keys) > 1:
-            raise exceptions.DSLParsingLogicException(
-                exceptions.ERROR_UNKNOWN_TYPE,
-                "Each constraint operator dict must be in it's own list item.")
-        constraint_name = constraint_op_keys[0]
+            if validate_version:
+                self.validate_version(
+                    version, (1, 5),
+                    'Constraint\'s additional attributes are not supported '
+                    f'in version {version_description(version)}, they were '
+                    f'added in {version_description((1, 5))}')
+            else:
+                raise exceptions.DSLParsingLogicException(
+                    exceptions.ERROR_UNKNOWN_TYPE,
+                    "Each constraint operator dict must be in it's own list "
+                    "item.")
+        constraint_name = [cn for cn in constraint_op_keys
+                           if cn != 'error_message'][0]
         if constraint_name not in constraints.CONSTRAINTS:
             raise exceptions.DSLParsingLogicException(
                 exceptions.ERROR_UNKNOWN_TYPE,
                 "No such constraint operator '{0}'. Allowed operators: "
                 "{1}".format(constraint_name, constraints.CONSTRAINTS))
         ancestor = self.ancestor(SchemaProperty).name
         constraints.validate_args(
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/misc.py` & `cloudify-common-7.0.0/dsl_parser/elements/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import elements, exceptions
-from dsl_parser._compat import text_type
 from dsl_parser.elements import version as element_version
 from dsl_parser.elements.deployment_schedules import DeploymentSchedules
 from dsl_parser.framework.elements import (DictElement,
                                            DictNoDefaultElement,
                                            Element,
                                            Leaf,
                                            List,
                                            Dict)
 
 
 class OutputDescription(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class OutputValue(Element):
 
     required = True
     schema = Leaf(type=elements.PRIMITIVE_TYPES)
@@ -48,15 +47,15 @@
 class Outputs(DictElement):
 
     schema = Dict(type=Output)
 
 
 class CapabilityDescription(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class CapabilityValue(Element):
 
     required = True
     schema = Leaf(type=elements.PRIMITIVE_TYPES)
@@ -86,15 +85,15 @@
     def validate(self, version, validate_version):
         if validate_version:
             self.validate_version(version, (1, 2))
 
 
 class Description(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     requires = {
         element_version.ToscaDefinitionsVersion: ['version'],
         'inputs': ['validate_version']
     }
 
     def validate(self, version, validate_version):
@@ -105,29 +104,29 @@
 class Metadata(Element):
 
     schema = Leaf(type=dict)
 
 
 class Imported(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class ImportedBlueprints(Element):
     """
     Internal DSL element used for maintaining a list of imported blueprints,
     this is for enabling protection against their deletion when used.
     """
 
     schema = List(type=Imported)
 
 
 class NamespaceMapping(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class NamespacesMapping(DictElement):
     """
     An internal DSL element for mapping all the used blueprints import
     namespaces.
@@ -151,15 +150,15 @@
         are assigned to a blueprint while it's uploaded, and the intrinsic
         functions are not yet processed.
         """
         type_err_msg = "The blueprint label's value must be a string. " \
                        "Please modify the values of {0}"
 
         for value in self.initial_value['values']:
-            if not isinstance(value, text_type):
+            if not isinstance(value, str):
                 raise exceptions.DSLParsingException(
                     1, type_err_msg.format(self.name))
 
 
 class DeploymentLabel(DictNoDefaultElement):
     schema = {
         'values': LabelValue
@@ -173,15 +172,15 @@
         type_err_msg = "The label's value must be a string or an intrinsic " \
                        "function. Please modify the values of {0}"
         get_attr_err_msg = "The label's value cannot be a runtime property. " \
                            "Please remove the `get_attribute` function from " \
                            "the values of {0}"
 
         for value in self.initial_value['values']:
-            if not isinstance(value, (dict, text_type)):
+            if not isinstance(value, (dict, str)):
                 raise exceptions.DSLParsingException(
                     1, type_err_msg.format(self.name))
             if isinstance(value, dict) and 'get_attribute' in value:
                 raise exceptions.DSLParsingException(
                     1, get_attr_err_msg.format(self.name))
 
 
@@ -198,19 +197,19 @@
 
 
 class DeploymentGroups(Element):
     schema = Leaf(list)
 
 
 class DeploymentIDTemplate(Element):
-    schema = Leaf(text_type)
+    schema = Leaf(str)
 
 
 class DeploymentDisplayName(Element):
-    schema = Leaf(type=(text_type, dict))
+    schema = Leaf(type=(str, dict))
 
 
 class DeploymentSettings(DictNoDefaultElement):
     schema = {
         'default_schedules': DeploymentSchedules,
         'default_groups': DeploymentGroups,
         'id_template': DeploymentIDTemplate,
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/node_templates.py` & `cloudify-common-7.0.0/dsl_parser/elements/node_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #    * limitations under the License.
 
 import copy
 
 from dsl_parser import (exceptions,
                         utils,
                         constants)
-from dsl_parser._compat import text_type
 from dsl_parser.interfaces import interfaces_parser
 from dsl_parser.elements import (node_types as _node_types,
                                  plugins as _plugins,
                                  relationships as _relationships,
                                  operation as _operation,
                                  data_types as _data_types,
                                  scalable,
@@ -35,15 +34,15 @@
                                            Dict,
                                            List)
 
 
 class NodeTemplateType(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         _node_types.NodeTypes: [Value('node_types')]
     }
 
     def validate(self, node_types):
         if self.initial_value not in node_types:
             err_message = ("Could not locate node type: '{0}'; "
@@ -80,15 +79,15 @@
                 "part of its type schema"),
             node_name=self.ancestor(NodeTemplate).name)
 
 
 class NodeTemplateRelationshipType(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         _relationships.Relationships: [Value('relationships')]
     }
 
     def validate(self, relationships):
         if self.initial_value not in relationships:
             raise exceptions.DSLParsingLogicException(
@@ -97,15 +96,15 @@
                     .format(self.ancestor(NodeTemplate).name,
                             self.initial_value))
 
 
 class NodeTemplateRelationshipTarget(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     def validate(self):
         relationship_type = self.sibling(NodeTemplateRelationshipType).name
         node_name = self.ancestor(NodeTemplate).name
         node_template_names = self.ancestor(NodeTemplates).initial_value_holder
         if self.initial_value not in node_template_names:
             raise exceptions.DSLParsingLogicException(
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/node_types.py` & `cloudify-common-7.0.0/dsl_parser/elements/node_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,36 +20,60 @@
 from dsl_parser.elements import (operation,
                                  data_types as _data_types,
                                  types)
 from dsl_parser.framework import requirements
 from dsl_parser.framework.elements import Dict
 
 
+class NodeTypeProperty(_data_types.SchemaProperty):
+    pass
+
+
+class NodeTypeProperties(_data_types.SchemaWithInitialDefault):
+    schema = Dict(type=NodeTypeProperty)
+
+
+class NodeTypeRuntimeProperty(_data_types.SchemaProperty):
+    min_version = (1, 5)
+
+
+class NodeTypeRuntimeProperties(_data_types.SchemaWithInitialDefault):
+    min_version = (1, 5)
+    schema = Dict(type=NodeTypeRuntimeProperty)
+
+
 class NodeType(types.Type):
 
     schema = {
         'derived_from': types.TypeDerivedFrom,
         'interfaces': operation.NodeTypeInterfaces,
-        'properties': _data_types.SchemaWithInitialDefault,
+        'properties': NodeTypeProperties,
+        'runtime_properties': NodeTypeRuntimeProperties,
     }
     requires = {
         'self': [requirements.Value('super_type',
                                     predicate=types.derived_from_predicate,
                                     required=False)],
         _data_types.DataTypes: [requirements.Value('data_types')]
     }
 
     def parse(self, super_type, data_types):
         node_type = self.build_dict_result()
         if not node_type.get('derived_from'):
             node_type.pop('derived_from', None)
         if super_type:
             node_type[constants.PROPERTIES] = utils.merge_schemas(
-                overridden_schema=super_type.get('properties', {}),
-                overriding_schema=node_type.get('properties', {}),
+                overridden_schema=super_type.get(constants.PROPERTIES, {}),
+                overriding_schema=node_type.get(constants.PROPERTIES, {}),
+                data_types=data_types)
+            node_type[constants.RUNTIME_PROPERTIES] = utils.merge_schemas(
+                overridden_schema=super_type.get(
+                    constants.RUNTIME_PROPERTIES, {}),
+                overriding_schema=node_type.get(
+                    constants.RUNTIME_PROPERTIES, {}),
                 data_types=data_types)
             node_type[constants.INTERFACES] = interfaces_parser. \
                 merge_node_type_interfaces(
                     overridden_interfaces=super_type[constants.INTERFACES],
                     overriding_interfaces=node_type[constants.INTERFACES])
         node_type[constants.TYPE_HIERARCHY] = self.create_type_hierarchy(
             super_type)
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/operation.py` & `cloudify-common-7.0.0/dsl_parser/elements/operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,36 +15,35 @@
 
 import copy
 import numbers
 
 from dsl_parser import (constants,
                         exceptions,
                         utils)
-from dsl_parser._compat import text_type
 from dsl_parser.elements import (inputs,
                                  version as _version)
 from dsl_parser.framework.elements import (DictElement,
                                            Element,
                                            Leaf,
                                            Dict)
 from dsl_parser.interfaces.utils import (operation,
                                          no_op_operation)
 
 
 class OperationImplementation(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     def parse(self):
         return self.initial_value if self.initial_value is not None else ''
 
 
 class OperationExecutor(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     add_namespace_to_schema_elements = False
 
     def validate(self):
         if self.initial_value is None:
             return
         value = self.initial_value
@@ -131,15 +130,15 @@
 class OperationTimeoutRecoverable(Element):
     schema = Leaf(type=bool)
 
 
 class Operation(Element):
 
     def parse(self):
-        if isinstance(self.initial_value, text_type):
+        if isinstance(self.initial_value, str):
             return {
                 'implementation': self.initial_value,
                 'executor': None,
                 'inputs': {},
                 'max_retries': None,
                 'retry_interval': None,
                 'timeout': None,
@@ -148,15 +147,15 @@
         else:
             return self.build_dict_result()
 
 
 class NodeTypeOperation(Operation):
 
     schema = [
-        Leaf(type=text_type),
+        Leaf(type=str),
         {
             'implementation': OperationImplementation,
             'inputs': NodeTypeOperationInputs,
             'executor': OperationExecutor,
             'max_retries': OperationMaxRetries,
             'retry_interval': OperationRetryInterval,
             'timeout': OperationTimeout,
@@ -164,15 +163,15 @@
         }
     ]
 
 
 class NodeTemplateOperation(Operation):
 
     schema = [
-        Leaf(type=text_type),
+        Leaf(type=str),
         {
             'implementation': OperationImplementation,
             'inputs': NodeTemplateOperationInputs,
             'executor': OperationExecutor,
             'max_retries': OperationMaxRetries,
             'retry_interval': OperationRetryInterval,
             'timeout': OperationTimeout,
@@ -302,42 +301,63 @@
                                'be defined (enforced by schema validation)')
         else:
             return no_op_operation(operation_name=operation_name)
 
     candidate_plugins = [p for p in plugins
                          if operation_mapping.startswith('{0}.'.format(p))]
 
-    if (utils.is_valid_url(operation_mapping) or
-        _is_local_script_resource_exists(resource_bases, operation_mapping) or
+    is_valid_url = utils.is_valid_url(operation_mapping)
+    local_resource_exists = _is_local_script_resource_exists(
+        resource_bases, operation_mapping)
+    if is_valid_url or local_resource_exists:
+        is_script = False
+    else:
+        is_script = _is_inline_script(operation_mapping)
+
+    if (
+        is_valid_url or
+        is_script or
+        local_resource_exists or
         (not candidate_plugins and _is_remote_script_resource(
-            operation_mapping, remote_resources_namespaces))):
+            operation_mapping, remote_resources_namespaces))
+    ):
+        if (
+            constants.SCRIPT_PATH_PROPERTY in operation_payload or
+            constants.SCRIPT_SOURCE_PROPERTY in operation_payload
+        ):
+            # if `implementation` is already a script source/path,
+            # disallow also providing that argument in inputs
+            wf_or_op = 'workflow' if is_workflows else 'operation'
+            offending_property = constants.SCRIPT_PATH_PROPERTY
+            if constants.SCRIPT_SOURCE_PROPERTY in operation_payload:
+                offending_property = constants.SCRIPT_PATH_PROPERTY
+
+            raise exceptions.DSLParsingLogicException(
+                60,
+                f"Cannot define '{offending_property}' property "
+                f"in '{operation_mapping}' for {wf_or_op} '{operation_name}'"
+            )
 
-        operation_payload = copy.deepcopy(operation_payload or {})
-        if constants.SCRIPT_PATH_PROPERTY in operation_payload:
-            message = "Cannot define '{0}' property in '{1}' for {2} '{3}'" \
-                .format(constants.SCRIPT_PATH_PROPERTY,
-                        operation_mapping,
-                        'workflow' if is_workflows else 'operation',
-                        operation_name)
-            raise exceptions.DSLParsingLogicException(60, message)
         script_path = operation_mapping
+        operation_payload = copy.deepcopy(operation_payload or {})
+        operation_executor = operation_executor or 'auto'
+
+        script_property = constants.SCRIPT_PATH_PROPERTY
+        if is_script:
+            script_property = constants.SCRIPT_SOURCE_PROPERTY
+
         if is_workflows:
             operation_mapping = constants.SCRIPT_PLUGIN_EXECUTE_WORKFLOW_TASK
-            operation_payload.update({
-                constants.SCRIPT_PATH_PROPERTY: {
-                    'default': script_path,
-                    'description': 'Workflow script executed by the script'
-                                   ' plugin'
-                }
-            })
+            operation_payload[script_property] = {
+                'default': script_path,
+                'description': 'Workflow script executed by the script plugin',
+            }
         else:
             operation_mapping = constants.SCRIPT_PLUGIN_RUN_TASK
-            operation_payload.update({
-                constants.SCRIPT_PATH_PROPERTY: script_path
-            })
+            operation_payload[script_property] = script_path
 
         # There can be more then one script plugin defined in the blueprint,
         # in case of the other one's are namespaced. But they are actually
         # pointing to the same installed one.
         script_plugins = utils.find_suffix_matches_in_list(
             constants.SCRIPT_PLUGIN_NAME,
             plugins)
@@ -412,7 +432,45 @@
             "Could not extract plugin or a script resource is not found from "
             "{2} mapping/script-path '{0}', which is declared for {2} '{1}'."
             .format(operation_mapping,
                     operation_name,
                     'workflow' if is_workflows else 'operation'))
         error_message = base_error_message + partial_error_message
         raise exceptions.DSLParsingLogicException(error_code, error_message)
+
+
+def _is_inline_script(script):
+    """Check if the string `script` contains a script.
+
+    The string, which is coming from an operation mapping in the blueprint,
+    can contain either an operation dotted import path, or a script written
+    right there in the blueprint.
+    """
+    script = script.strip()
+    if script.count('\n') > 1:
+        # multiple lines? this for sure isn't a dotted path
+        return True
+
+    if utils.NAMESPACE_DELIMITER in script:
+        ns, _, _rest = script.partition(utils.NAMESPACE_DELIMITER)
+        if ns.isidentifier():
+            # a namespace delimiter, separating a single identifier? this
+            # for sure is not a script!
+            return False
+
+    if '/' in script or '\\' in script:
+        # script is one line and contains a slash/backslash - interpret
+        # this as a path (posix or windows).
+        # This means it's impossible to have 1-line scripts containing
+        # slashes, but this stays backwards-compatible
+        return False
+
+    if (
+        '.' in script and
+        all(part.isidentifier() for part in script.split('.'))
+    ):
+        # this looks like a dotted path - identifiers separated by dots
+        return False
+
+    # it doesn't look like a file path, or a dotted path - it must be a
+    # one-liner script!
+    return True
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/plugins.py` & `cloudify-common-7.0.0/dsl_parser/elements/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import (constants,
                         exceptions)
-from dsl_parser._compat import text_type
 from dsl_parser.elements import version as element_version
+from dsl_parser.elements.data_types import (SchemaPropertyDescription,
+                                            SchemaPropertyType,
+                                            SchemaPropertyDisplayLabel)
 from dsl_parser.framework.elements import (DictElement,
                                            Element,
                                            Leaf,
                                            Dict)
 
 
 class PluginExecutor(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
     def validate(self):
         if self.initial_value not in [constants.CENTRAL_DEPLOYMENT_AGENT,
                                       constants.HOST_AGENT]:
             raise exceptions.DSLParsingLogicException(
                 18, "Plugin '{0}' has an illegal "
@@ -41,15 +43,15 @@
                             self.initial_value,
                             constants.CENTRAL_DEPLOYMENT_AGENT,
                             constants.HOST_AGENT))
 
 
 class PluginSource(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class PluginInstall(Element):
 
     schema = Leaf(type=bool)
     add_namespace_to_schema_elements = False
@@ -57,15 +59,15 @@
     def parse(self):
         value = self.initial_value
         return value if value is not None else True
 
 
 class PluginVersionValidatedElement(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
     requires = {
         element_version.ToscaDefinitionsVersion: ['version'],
         'inputs': ['validate_version']
     }
     min_version = None
 
@@ -100,27 +102,59 @@
     min_version = (1, 2)
 
 
 class PluginDistributionRelease(PluginVersionValidatedElement):
     min_version = (1, 2)
 
 
+class PluginPropertiesDescription(PluginVersionValidatedElement):
+    min_version = (1, 5)
+    schema = Leaf(type=str)
+
+
+class PluginPropertyValue(Element):
+    schema = Leaf(type=(str, int, float, bool, list, dict))
+
+
+class PluginProperty(Element):
+    schema = {
+        'description': SchemaPropertyDescription,
+        'type': SchemaPropertyType,
+        'display_label': SchemaPropertyDisplayLabel,
+        'value': PluginPropertyValue,
+    }
+
+
+class PluginProperties(DictElement):
+    schema = Dict(type=PluginProperty)
+    requires = {
+        element_version.ToscaDefinitionsVersion: ['version'],
+        'inputs': ['validate_version']
+    }
+
+    def validate(self, version, validate_version):
+        if validate_version:
+            self.validate_version(version, (1, 5))
+
+
 class Plugin(DictElement):
 
     schema = {
         'source': PluginSource,
         'executor': PluginExecutor,
         'install': PluginInstall,
         'install_arguments': PluginInstallArguments,
         'package_name': PluginPackageName,
         'package_version': PluginPackageVersion,
         'supported_platform': PluginSupportedPlatform,
         'distribution': PluginDistribution,
         'distribution_version': PluginDistributionVersion,
-        'distribution_release': PluginDistributionRelease
+        'distribution_release': PluginDistributionRelease,
+        'properties_description': PluginPropertiesDescription,
+        'properties': PluginProperties,
     }
 
     def validate(self):
         if self.child(PluginInstall).value:
             if not (self.child(PluginSource).value or
                     self.child(PluginPackageName).value):
                 raise exceptions.DSLParsingLogicException(
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/policies.py` & `cloudify-common-7.0.0/dsl_parser/elements/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 #    * limitations under the License.
 
 import itertools
 
 from networkx.algorithms import (
     ancestors,
     recursive_simple_cycles,
-    topological_sort,
 )
 from networkx.classes import DiGraph
 
 from dsl_parser import (exceptions,
                         utils,
                         constants)
-from dsl_parser._compat import text_type
 from dsl_parser.elements import (node_templates as _node_templates,
                                  data_types,
                                  scalable,
                                  version as _version)
 from dsl_parser.framework.requirements import Value
 from dsl_parser.framework.elements import (DictElement,
                                            Element,
@@ -37,15 +35,15 @@
                                            List,
                                            Dict)
 
 
 class PolicyTriggerSource(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class PolicyTriggerParameters(data_types.Schema):
     add_namespace_to_schema_elements = False
 
 
@@ -56,15 +54,15 @@
         'source': PolicyTriggerSource,
     }
 
 
 class PolicyTypeSource(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class PolicyTypeProperties(data_types.Schema):
     add_namespace_to_schema_elements = False
 
 
@@ -85,15 +83,15 @@
 
     schema = Dict(type=PolicyTrigger)
 
 
 class GroupPolicyType(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         PolicyTypes: [Value(constants.POLICY_TYPES)]
     }
 
     def validate(self, policy_types):
         if self.initial_value not in policy_types:
             raise exceptions.DSLParsingLogicException(
@@ -130,15 +128,15 @@
                 self.ancestor(Group).name,
                 self.ancestor(GroupPolicy).name))
 
 
 class GroupPolicyTriggerType(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         PolicyTriggers: [Value(constants.POLICY_TRIGGERS)]
     }
 
     def validate(self, policy_triggers):
         if self.initial_value not in policy_triggers:
             raise exceptions.DSLParsingLogicException(
@@ -200,15 +198,15 @@
         'properties': GroupPolicyProperties,
         'triggers': GroupPolicyTriggers,
     }
 
 
 class GroupMember(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         _node_templates.NodeTemplates: ['node_template_names']
     }
 
     def validate(self, node_template_names):
         groups = self.ancestor(Groups).initial_value
         value = self.initial_value
@@ -264,29 +262,29 @@
 
     schema = Dict(type=Group)
 
 
 class PolicyInstanceType(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
     def validate(self):
         scaling_policy = constants.SCALING_POLICY
         if self.initial_value != scaling_policy:
             raise exceptions.DSLParsingLogicException(
                 exceptions.ERROR_UNSUPPORTED_POLICY,
                 "'{0}' policy type is not implemented. "
                 "Only '{1}' policy type is supported."
                 .format(self.initial_value, scaling_policy))
 
 
 class PolicyInstanceTarget(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     requires = {
         Groups: [Value(constants.GROUPS)]
     }
 
     def validate(self, groups):
         if self.initial_value not in groups:
             raise exceptions.DSLParsingLogicException(
@@ -409,15 +407,15 @@
                 exceptions.ERROR_GROUP_CYCLE,
                 'Illegal group cycles found: {0}'.format(group_cycles))
 
     @staticmethod
     def _validate_members_in_one_group_only(member_graph):
         # verify all group members are part of exactly one group
         for member in member_graph:
-            successors = member_graph.successors(member)
+            successors = list(member_graph.successors(member))
             if len(successors) > 1:
                 raise exceptions.DSLParsingLogicException(
                     exceptions.ERROR_MULTIPLE_GROUPS,
                     "Nodes and groups cannot be members in multiple groups, "
                     "but member '{0}' belongs to the following multiple "
                     "groups: {1}".format(member, successors))
 
@@ -448,18 +446,18 @@
         containing_nodes = {}
 
         def check_pair(pair_key):
             node_a, node_b = pair_key
             if node_a == node_b:
                 return True
             if node_a not in containing_nodes:
-                containing_nodes[node_a] = topological_sort(
+                containing_nodes[node_a] = utils.topological_sort(
                     node_graph, nbunch=[node_a])
             if node_b not in containing_nodes:
-                containing_nodes[node_b] = topological_sort(
+                containing_nodes[node_b] = utils.topological_sort(
                     node_graph, nbunch=[node_b])
             a_containing_nodes = set(containing_nodes[node_a])
             a_containing_nodes.remove(node_a)
             b_containing_nodes = set(containing_nodes[node_b])
             b_containing_nodes.remove(node_b)
             if not (a_containing_nodes or b_containing_nodes):
                 return True
@@ -514,35 +512,36 @@
         # member from the relevant group.
         # if the node and its containee are in the same group, remove the
         # containee, otherwise, remove the group closest to the containing
         # node
         for member in member_graph:
             if member not in node_graph:
                 continue
-            containing_groups = topological_sort(member_graph,
-                                                 nbunch=[member])
-            containing_nodes = topological_sort(node_graph, nbunch=[member])
+            containing_groups = utils.topological_sort(member_graph,
+                                                       nbunch=[member])
+            containing_nodes = utils.topological_sort(node_graph,
+                                                      nbunch=[member])
             for node in containing_nodes:
                 if node == member:
                     continue
                 if node not in member_graph:
                     continue
 
-                containing_node_groups = topological_sort(member_graph,
-                                                          nbunch=[node])
+                containing_node_groups = utils.topological_sort(
+                    member_graph, nbunch=[node])
                 containing_node_groups_set = set(containing_node_groups)
 
                 shared_groups = (set(containing_groups) &
                                  containing_node_groups_set)
                 if not shared_groups:
                     continue
 
-                minimal_containing_group = topological_sort(
+                minimal_containing_group = utils.topological_sort(
                     member_graph, nbunch=shared_groups)[0]
-                direct_member_group = member_graph.successors(member)[0]
+                direct_member_group = list(member_graph.successors(member))[0]
                 members = scaling_groups[minimal_containing_group]['members']
                 if direct_member_group == minimal_containing_group:
                     removed_member = member
                 else:
                     for containing_group in reversed(containing_groups):
                         if containing_group not in containing_node_groups_set:
                             removed_member = containing_group
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/relationships.py` & `cloudify-common-7.0.0/dsl_parser/elements/relationships.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/scalable.py` & `cloudify-common-7.0.0/dsl_parser/elements/scalable.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-from dsl_parser._compat import text_type
 from dsl_parser import (exceptions,
                         constants,
                         functions)
 from dsl_parser.framework.elements import (DictElement,
                                            Element,
                                            Leaf)
 
@@ -63,24 +62,24 @@
 
 class MinInstances(NonNegativeInstances):
     default_value = 0
 
 
 class MaxInstances(Instances):
 
-    schema = Leaf(type=(int, text_type, dict))
+    schema = Leaf(type=(int, str, dict))
     default_value = constants.UNBOUNDED
 
     def validate(self):
         if super(MaxInstances, self).validate():
             return
         value = self.initial_value
         if value is None:
             return
-        if isinstance(value, text_type):
+        if isinstance(value, str):
             if value != constants.UNBOUNDED_LITERAL:
                 raise exceptions.DSLParsingLogicException(
                     exceptions.ERROR_INVALID_LITERAL_INSTANCES,
                     'The only valid string for {0} is {1}.'
                     .format(self.name,
                             constants.UNBOUNDED_LITERAL))
             return
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/types.py` & `cloudify-common-7.0.0/dsl_parser/elements/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import exceptions
-from dsl_parser._compat import text_type
 from dsl_parser.framework.elements import (DictElement,
                                            Element,
                                            Leaf)
 
 
 class Types(DictElement):
     pass
@@ -38,15 +37,15 @@
     def fix_properties(value):
         for key, value in value['properties'].items():
             value.pop('initial_default', None)
 
 
 class DerivedFrom(Element):
 
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     descriptor = ''
 
     def validate(self):
         if self.initial_value is None:
             return
 
         if self.initial_value not in self.ancestor(Types).initial_value_holder:
```

### Comparing `cloudify-common-6.4.2/dsl_parser/elements/workflows.py` & `cloudify-common-7.0.0/dsl_parser/elements/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 from dsl_parser import constants, constraints, exceptions, utils
-from dsl_parser._compat import text_type
 from dsl_parser.elements import (data_types,
                                  plugins as _plugins,
                                  operation,
                                  misc,
                                  version as _version)
 from dsl_parser.framework.requirements import (Value,
                                                Requirement,
@@ -104,15 +103,15 @@
     def parse(self):
         return self.build_dict_result(with_default=False)
 
 
 class WorkflowMapping(Element):
 
     required = True
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
 
 
 class WorkflowParameters(data_types.Schema):
 
     add_namespace_to_schema_elements = False
     schema = Dict(type=ParameterSchemaProperty)
 
@@ -141,15 +140,15 @@
                 exceptions.ERROR_UNKNOWN_TYPE,
                 "Invalid definition of 'active_node_instances' availability "
                 "rule: '{0}'. Allowed values: {1}"
                 .format(self.initial_value, self.valid_values))
 
 
 class NodeTypeName(Element):
-    schema = Leaf(type=text_type)
+    schema = Leaf(type=str)
     add_namespace_to_schema_elements = False
 
 
 class WorkflowAvailabilityNodeTypesRequired(Element):
     schema = List(type=NodeTypeName)
     add_namespace_to_schema_elements = False
 
@@ -171,30 +170,30 @@
             self.validate_version(version, (1, 4))
 
 
 class Workflow(Element):
 
     required = True
     schema = [
-        Leaf(type=text_type),
+        Leaf(type=str),
         {
             'mapping': WorkflowMapping,
             'parameters': WorkflowParameters,
             'is_cascading': WorkflowIsCascading,
             'availability_rules': WorkflowAvailabilityRules,
         }
     ]
     requires = {
         'inputs': [Requirement('resource_base', required=False)],
         _plugins.Plugins: [Value('plugins')],
         misc.NamespacesMapping: [Value(constants.NAMESPACES_MAPPING)]
     }
 
     def parse(self, plugins, resource_base, namespaces_mapping):
-        if isinstance(self.initial_value, text_type):
+        if isinstance(self.initial_value, str):
             operation_content = {'mapping': self.initial_value,
                                  'parameters': {}}
             is_cascading = False
             availability_rules = None
         else:
             operation_content = self.build_dict_result()
             is_cascading = self.initial_value.get('is_cascading', False)
```

### Comparing `cloudify-common-6.4.2/dsl_parser/exceptions.py` & `cloudify-common-7.0.0/dsl_parser/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,7 +193,11 @@
 ERROR_DISPLAY_FOR_INVALID_TYPE = 216
 # A `item_type` attribute is invalid
 ERROR_INVALID_ITEM_TYPE = 217
 # A `item_type` attribute is declared for invalid type
 ERROR_ITEM_TYPE_FOR_INVALID_TYPE = 218
 # Intrinsic function not allowed for certain elements of the schema
 ERROR_INTRINSIC_FUNCTION_NOT_PERMITTED = 219
+# Node not properly imported
+ERROR_INVALID_IMPORT_SPECS = 220
+# Properties defined for imported node do not match the specification
+ERROR_INVALID_IMPORT_PROPERTIES = 221
```

### Comparing `cloudify-common-6.4.2/dsl_parser/framework/__init__.py` & `cloudify-common-7.0.0/dsl_parser/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/framework/elements.py` & `cloudify-common-7.0.0/dsl_parser/framework/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import copy
+from io import StringIO
 
 from dsl_parser import exceptions
 from dsl_parser import holder
 from dsl_parser import version as _version
 
-from dsl_parser._compat import StringIO
-
 
 class Unparsed(object):
     pass
 
 
 UNPARSED = Unparsed()
 
@@ -180,43 +179,44 @@
         return matches[0]
 
     def descendants(self, element_type):
         return [e for e in self.context.descendants(self)
                 if isinstance(e, element_type)]
 
     def child(self, element_type):
-        matches = [e for e in self.context.child_elements_iter(self)
+        matches = [e for e in self.context.child_elements(self)
                    if isinstance(e, element_type)]
         if not matches:
             raise exceptions.DSLParsingElementMatchException(
                 "No matches found for '{0}'".format(element_type))
         if len(matches) > 1:
             raise exceptions.DSLParsingElementMatchException(
                 "Multiple matches found for '{0}'".format(element_type))
         return matches[0]
 
     def build_dict_result(self, with_default=True):
         return dict((child.name, child.value)
-                    for child in self.context.child_elements_iter(self)
+                    for child in self.context.child_elements(self)
                     if with_default or child.defined)
 
     def children(self):
-        return list(self.context.child_elements_iter(self))
+        return self.context.child_elements(self)
 
     def sibling(self, element_type):
         return self.parent().child(element_type)
 
-    def validate_version(self, version, min_version):
+    def validate_version(self, version, min_version, error_msg=None):
         if self.initial_value is not None and version < min_version:
             if self.name == 'type':
                 dsl_node = "type '{0}'".format(self.initial_value)
             else:
                 dsl_node = self.name
             raise exceptions.DSLParsingLogicException(
                 exceptions.ERROR_CODE_DSL_DEFINITIONS_VERSION_MISMATCH,
+                error_msg or
                 '{0} not supported in version {1}, it was added in {2}'.format(
                     dsl_node,
                     _version.version_description(version),
                     _version.version_description(min_version)
                 )
             )
```

### Comparing `cloudify-common-6.4.2/dsl_parser/framework/parser.py` & `cloudify-common-7.0.0/dsl_parser/framework/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import numbers
 
+# a hack to allow networkx 1.11 to work with python 3.10: gcd was moved from
+# fractions to math, but networkx attempts to import from fractions. Remove
+# this  after we've either upgraded or removed networkx
+import fractions
+if not hasattr(fractions, 'gcd'):
+    import math
+    fractions.gcd = math.gcd
+
+
 from networkx.algorithms import (
     descendants,
     recursive_simple_cycles,
-    topological_sort,
 )
 from networkx.classes import DiGraph
 from networkx.exception import NetworkXUnfeasible
 
-from dsl_parser._compat import text_type
 from dsl_parser.framework import elements
 from dsl_parser import (exceptions,
                         constants,
                         functions,
                         utils,
                         holder)
 from dsl_parser.framework.requirements import Requirement, sibling_predicate
@@ -50,15 +57,15 @@
         except TypeError:
             raise exceptions.DSLParsingSchemaAPIException(1)
         self._traverse_schema(element_cls.schema)
 
     def _traverse_schema(self, schema, list_nesting=0):
         if isinstance(schema, dict):
             for key, value in schema.items():
-                if not isinstance(key, text_type):
+                if not isinstance(key, str):
                     raise exceptions.DSLParsingSchemaAPIException(1)
                 self._traverse_element_cls(value)
         elif isinstance(schema, list):
             if list_nesting > 0:
                 raise exceptions.DSLParsingSchemaAPIException(1)
             if len(schema) == 0:
                 raise exceptions.DSLParsingSchemaAPIException(1)
@@ -152,21 +159,22 @@
                     element.initial_value_holder.value)
                 delattr(element.initial_value_holder, SKIP_NAMESPACE_FLAG)
 
     @property
     def parsed_value(self):
         return self._root_element.value if self._root_element else None
 
-    def child_elements_iter(self, element):
-        return self._element_tree.successors_iter(element)
+    def child_elements(self, element):
+        return list(self._element_tree.successors(element))
 
     def ancestors_iter(self, element):
         current_element = element
         while True:
-            predecessors = self._element_tree.predecessors(current_element)
+            predecessors = list(self._element_tree.predecessors(
+                current_element))
             if not predecessors:
                 return
             if len(predecessors) > 1:
                 raise exceptions.DSLParsingFormatException(
                     1, 'More than 1 parent found for {0}'
                        .format(element))
             current_element = predecessors[0]
@@ -308,15 +316,15 @@
                 if k == 'get_input' and not isinstance(v, list):
                     namespaced_value =\
                         utils.generate_namespaced_value(namespace, v)
                     element[k] = namespaced_value
                     holder_element.value[holder_key].value = namespaced_value
                     holder_value.skip_namespace = True
                 if k == 'get_input' and isinstance(v, list):
-                    if isinstance(v[0], text_type):
+                    if isinstance(v[0], str):
                         element[k][0] =\
                             utils.generate_namespaced_value(namespace, v[0])
                 elif k == 'get_property' or k == 'get_attribute':
                     set_namespace_node_intrinsic_functions(
                         namespace,
                         v,
                         holder_element.value[holder_key].value)
@@ -324,15 +332,15 @@
                 if isinstance(v, dict) or k == 'concat':
                     handle_intrinsic_function_namespace(
                         holder_element.value[holder_key], v)
                 elif isinstance(v, list):
                     traverse_list(holder_element.value[holder_key], v)
 
         def should_add_namespace_to_string_leaf(element):
-            if not isinstance(element._initial_value, text_type):
+            if not isinstance(element._initial_value, str):
                 return False
             is_premitive_type = (element._initial_value in
                                  constants.USER_PRIMITIVE_TYPES)
             overridable_cloudify_type = \
                 utils.check_if_overridable_cloudify_type(
                     element._initial_value)
             should_skip_adding_namespace =\
@@ -423,15 +431,15 @@
 
     def _calculate_element_graph(self):
         self.element_graph = DiGraph(self._element_tree)
         for element_type, _elements in self.element_type_to_elements.items():
             requires = element_type.requires
             for requirement, requirement_values in requires.items():
                 requirement_values = [
-                    Requirement(r) if isinstance(r, text_type)
+                    Requirement(r) if isinstance(r, str)
                     else r for r in requirement_values]
                 if requirement == 'inputs':
                     continue
                 if requirement == 'self':
                     requirement = element_type
                 dependencies = self.element_type_to_elements.get(
                     requirement, [])
@@ -461,22 +469,22 @@
                 for dependency in dependencies:
                     for element in _elements:
                         add_dependency = all(
                             predicate(element, dependency)
                             for predicate in predicates)
                         if add_dependency:
                             self.element_graph.add_edge(element, dependency)
-        # we reverse the graph because only netorkx 1.9.1 has the reverse
+        # we reverse the graph because only networkx 1.9.1 has the reverse
         # flag in the topological sort function, it is only used by it
         # so this should be good
         self.element_graph.reverse(copy=False)
 
     def elements_graph_topological_sort(self):
         try:
-            return topological_sort(self.element_graph)
+            return utils.topological_sort(self.element_graph, reverse=True)
         except NetworkXUnfeasible:
             # Cycle detected
             cycle = recursive_simple_cycles(self.element_graph)[0]
             names = [str(e.name) for e in cycle]
             names.append(str(names[0]))
             ex = exceptions.DSLParsingLogicException(
                 exceptions.ERROR_CODE_CYCLE,
@@ -536,15 +544,15 @@
 
         def validate_schema(schema):
             if isinstance(schema, (dict, elements.Dict)):
                 if not isinstance(value, dict):
                     raise exceptions.DSLParsingFormatException(
                         1, _expected_type_message(value, dict))
                 for key in value:
-                    if not isinstance(key, text_type):
+                    if not isinstance(key, str):
                         raise exceptions.DSLParsingFormatException(
                             1, "Dict keys must be strings but"
                                " found '{0}' of type '{1}'"
                                .format(key, _py_type_to_user_type(type(key))))
 
             if strict and isinstance(schema, dict):
                 for key in value:
@@ -596,15 +604,15 @@
         element.provided = element.calculate_provided(**required_args)
 
     @staticmethod
     def _extract_element_requirements(element):
         context = element.context
         required_args = {}
         for required_type, requirements in element.requires.items():
-            requirements = [Requirement(r) if isinstance(r, text_type)
+            requirements = [Requirement(r) if isinstance(r, str)
                             else r for r in requirements]
             if not requirements:
                 # only set required type as a logical dependency
                 pass
             elif required_type == 'inputs':
                 for input in requirements:
                     if input.name not in context.inputs and input.required:
@@ -702,15 +710,15 @@
             .format(_py_type_to_user_type(expected_type),
                     _py_type_to_user_type(type(value))))
 
 
 def _py_type_to_user_type(_type):
     if isinstance(_type, tuple):
         return list(set(_py_type_to_user_type(t) for t in _type))
-    elif issubclass(_type, text_type):
+    elif issubclass(_type, str):
         return 'string'
     elif issubclass(_type, bool):
         return 'boolean'
     elif issubclass(_type, numbers.Integral):
         return 'integer'
     elif issubclass(_type, float):
         return 'float'
```

### Comparing `cloudify-common-6.4.2/dsl_parser/framework/requirements.py` & `cloudify-common-7.0.0/dsl_parser/framework/requirements.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/functions.py` & `cloudify-common-7.0.0/dsl_parser/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  * See the License for the specific language governing permissions and
 #  * limitations under the License.
 
 import abc
 import collections
-
-import pkg_resources
 import json
+import pkg_resources
+from typing import Dict, Union
 
 from functools import wraps
 
 from dsl_parser import exceptions, scan, constants
-from dsl_parser._compat import ABC, text_type
 from dsl_parser.constants import (OUTPUTS,
                                   CAPABILITIES,
                                   NODE_INSTANCES,
-                                  INTER_DEPLOYMENT_FUNCTIONS,
                                   EVAL_FUNCS_PATH_PREFIX_KEY,
                                   EVAL_FUNCS_PATH_DEFAULT_PREFIX)
 from dsl_parser.utils import (TEMPLATE_FUNCTIONS,
                               get_function,
                               parse_simple_type_value)
 
 
@@ -142,25 +140,25 @@
     return s
 
 
 _register_entry_point_functions()
 
 
 def _contains_legal_nested_attribute_path_items(args):
-    return all(get_function(x) or isinstance(x, (text_type, int))
+    return all(get_function(x) or isinstance(x, (str, int))
                for x in args)
 
 
 def _is_legal_nested_attribute_path(args):
     return isinstance(args, list) \
         and len(args) >= 2 \
         and _contains_legal_nested_attribute_path_items(args)
 
 
-class Function(ABC):
+class Function(abc.ABC):
     name = 'function'
     func_eval_type = None
 
     def __init__(self, args, scope=None, context=None, path=None, raw=None,
                  return_type=None):
         """Initializes the instance.
 
@@ -190,32 +188,29 @@
     def validate(self, plan):
         pass
 
     @abc.abstractmethod
     def evaluate(self, handler):
         pass
 
-    def register_function_to_plan(self, plan):
-        pass
-
 
 @register(name='get_input', func_eval_type=HYBRID_FUNC)
 class GetInput(Function):
 
     def __init__(self, args, **kwargs):
         self.input_value = None
         super(GetInput, self).__init__(args, **kwargs)
 
     def parse_args(self, args):
         def _is_valid_args_list(args_list):
             return isinstance(args_list, list) \
                 and len(args_list) >= 1 \
                 and _contains_legal_nested_attribute_path_items(args_list)
 
-        if not isinstance(args, text_type) \
+        if not isinstance(args, str) \
                 and not get_function(args) \
                 and not _is_valid_args_list(args):
             raise ValueError(
                 "Illegal argument(s) passed to {0} function. Expected either "
                 "a string, or a function, or a list [input_name\\function "
                 "[, key1\\index1\\function [,...]]] "
                 "but got {1}".format(self.name, args))
@@ -228,29 +223,28 @@
             return
         if input_value not in plan.inputs:
             raise exceptions.UnknownInputError(
                 "get_input function references an "
                 "unknown input '{0}'.".format(input_value))
 
     def evaluate(self, handler):
-        return_value = None
         if isinstance(self.input_value, list):
             if any(get_function(x) for x in self.input_value):
                 raise exceptions.FunctionEvaluationError(
                     '{0}: found an unresolved argument: {1}'
                     .format(self.name, self.input_value))
 
             return_value = self._get_input_attribute(
                 handler.get_input(self.input_value[0]))
-
-        if get_function(self.input_value):
-            raise exceptions.FunctionEvaluationError(
-                '{0}: found an unresolved argument: {1}'
-                .format(self.name, self.input_value))
-        return_value = return_value or handler.get_input(self.input_value)
+        else:
+            if get_function(self.input_value):
+                raise exceptions.FunctionEvaluationError(
+                    '{0}: found an unresolved argument: {1}'
+                    .format(self.name, self.input_value))
+            return_value = handler.get_input(self.input_value)
 
         if self.return_type:
             _, ok = parse_simple_type_value(return_value, self.return_type)
             if not ok:
                 raise exceptions.InputEvaluationError(
                     "Value '{0}' of input '{1}' does not match data type "
                     "declared for '{2}': '{3}'."
@@ -325,22 +319,22 @@
                 "property (e.g. [tenant, name] or [deployment, id]) "
                 "but got {1}".format(self.name, args))
 
     def validate(self, plan):
         known_entities = set(p[0] for p in self.VALID_PROPERTIES)
         if get_function(self.entity):
             return
-        if not isinstance(self.entity, text_type) \
+        if not isinstance(self.entity, str) \
                 or self.entity not in known_entities:
             raise exceptions.UnknownSysEntityError(
                 "{0} function unable to determine entity: {1}"
                 .format(self.name, self.entity))
         if get_function(self.property):
             return
-        if not isinstance(self.property, text_type) \
+        if not isinstance(self.property, str) \
                 or (self.entity, self.property) not in self.VALID_PROPERTIES:
             raise exceptions.UnknownSysPropertyError(
                 "{0} function unable to determine property: {1} {2}"
                 .format(self.name, self.entity, self.property))
 
     def evaluate(self, handler):
         return handler.get_sys(self.entity, self.property)
@@ -351,15 +345,15 @@
     VALID_PROPERTIES = ['ids', 'names', 'count']
 
     def __init__(self, args, **kwargs):
         self.property = None
         super(GetConsumers, self).__init__(args, **kwargs)
 
     def parse_args(self, args):
-        if isinstance(args, text_type) and args in self.VALID_PROPERTIES:
+        if isinstance(args, str) and args in self.VALID_PROPERTIES:
             self.property = args
         else:
             raise ValueError(
                 "Illegal argument passed to {name} function. Expected a "
                 "property string (one of: {props}), but got {args}".format(
                     name=self.name, props=', '.join(self.VALID_PROPERTIES),
                     args=args))
@@ -652,22 +646,22 @@
                                 attribute_path,
                                 handler,
                                 context,
                                 path,
                                 raise_if_not_found=False,
                                 func_name=fn_name)
 
-    if value is None:
-        # attribute not found in instance runtime properties
-        # special case for { get_attributes_list: [
-        #                        ..., node_instance_id] }
-        # returns the node-instance-id
-        if len(attribute_path) == 1\
-                and attribute_path[0] == 'node_instance_id':
+    if value is None and len(attribute_path) == 1:
+        # specialcase some get_attribute parameters:
+        # - node_instance_id returns the node instance ID
+        # - node_instance_index returns the node instance index
+        if attribute_path[0] == 'node_instance_id':
             value = ni['id']
+        elif attribute_path[0] == 'node_instance_index':
+            value = ni['index']
     # still nothing? look in node properties
     if value is None:
         value = _get_property_value(node['id'],
                                     node.get('properties', {}),
                                     attribute_path,
                                     handler,
                                     context,
@@ -828,15 +822,15 @@
         self.secret_id = None
         super(GetSecret, self).__init__(args, **kwargs)
 
     def parse_args(self, args):
         if (
             not (
                 (isinstance(args, list) and len(args) > 1)
-                or isinstance(args, text_type)
+                or isinstance(args, str)
                 or get_function(args)
             )
         ):
             raise exceptions.FunctionValidationError(
                 "`get_secret` function argument should be a list with at "
                 "least 2 elements, a string, or a dict (a function). Instead "
                 "it is a {0} with the value: {1}.".format(type(args), args))
@@ -945,21 +939,14 @@
         merged = {}
         for cur_dict in self.merged:
             merged.update(cur_dict)
         return merged
 
 
 class InterDeploymentDependencyCreatingFunction(Function):
-
-    def register_function_to_plan(self, plan):
-        plan.setdefault(
-            INTER_DEPLOYMENT_FUNCTIONS,
-            {}
-        )[self.function_identifier] = self.target_deployment
-
     @abc.abstractproperty
     def target_deployment(self):
         pass
 
     @property
     def function_identifier(self):
         return '{0}.{1}'.format(self.path, self.name)
@@ -980,15 +967,15 @@
             raise ValueError(
                 "`get_capability` function argument should be a list with 2 "
                 "elements at least - [ deployment ID, capability ID "
                 "[, key/index[, key/index [...]]] ]. Instead it is: [{0}]"
                 .format(','.join('{0}'.format(a) for a in args))
             )
         for arg_index, arg in enumerate(args):
-            if not isinstance(arg, (text_type, int)) and not get_function(arg):
+            if not isinstance(arg, (str, int)) and not get_function(arg):
                 raise ValueError(
                     "`get_capability` function arguments can't be complex "
                     "values; only strings/ints/functions are accepted. "
                     "Instead, the item with index {0} is {1} of type {2}"
                     .format(arg_index, arg, type(arg))
                 )
 
@@ -1025,15 +1012,15 @@
                 "with 2 elements at least - [ group ID, capability ID "
                 "[, key/index[, key/index [...]]] ]. Instead it is: [{0}]"
                 .format(','.join('{0}'.format(a) for a in args))
             )
         for arg_index, arg in enumerate(args):
             if arg_index == 1 and isinstance(arg, list):
                 continue
-            if not isinstance(arg, (text_type, int)) and not get_function(arg):
+            if not isinstance(arg, (str, int)) and not get_function(arg):
                 raise ValueError(
                     "`get_group_capability` function arguments can't be "
                     "complex values; only strings/ints/functions are "
                     "accepted. Instead, the item with index {0} is {1} "
                     "of type {2}".format(arg_index, arg, type(arg))
                 )
         self.capability_path = args
@@ -1050,15 +1037,15 @@
     def __init__(self, args, **kwargs):
         self.label_key = None
         self.values_list_index = None
         super(GetLabel, self).__init__(args, **kwargs)
 
     def parse_args(self, args):
         if isinstance(args, list) and len(args) == 2:
-            if not (isinstance(args[0], text_type) or get_function(args[0])):
+            if not (isinstance(args[0], str) or get_function(args[0])):
                 raise exceptions.FunctionValidationError(
                     '`get_label`',
                     "the <label-key> should be a string or a dict "
                     "(a function). Instead, it is a {0} with the value: "
                     "{1}.".format(type(args[0]), args[0])
                 )
             if not (isinstance(args[1], int) or args[1].isdigit()):
@@ -1066,15 +1053,15 @@
                     '`get_label`',
                     "the <label-values list index> should be a number "
                     "(in string or int form). Instead, it is a {0} with the "
                     "value: {1}.".format(type(args[1]), args[1])
                 )
             self.label_key = args[0]
             self.values_list_index = int(args[1])
-        elif isinstance(args, text_type):
+        elif isinstance(args, str):
             self.label_key = args
         elif get_function(args):
             self.label_key = args
         else:
             raise exceptions.FunctionValidationError(
                 '`get_label`',
                 "`get_label` function argument should be a list of 2 "
@@ -1093,15 +1080,15 @@
 @register(name='get_environment_capability', func_eval_type=RUNTIME_FUNC)
 class GetEnvironmentCapability(Function):
     def __init__(self, args, **kwargs):
         self.capability_path = None
         super(GetEnvironmentCapability, self).__init__(args, **kwargs)
 
     def parse_args(self, args):
-        if isinstance(args, text_type):
+        if isinstance(args, str):
             self.capability_path = [args]
         elif isinstance(args, list):
             if len(args) < 2:
                 raise exceptions.FunctionValidationError(
                     '`get_environment_capability`',
                     "`get_environment_capability` function arguments can't be"
                     " list with only one item; only string or list with"
@@ -1115,15 +1102,15 @@
                 '`get_environment_capability`',
                 "`get_environment_capability` function argument should be a "
                 "string or list with more than one item are accepted."
                 " Instead, it is a {0} with the value: {1}.".format(type(
                     args), args)
             )
         for arg_index, arg in enumerate(args):
-            if not isinstance(arg, (text_type, int)) and not get_function(arg):
+            if not isinstance(arg, (str, int)) and not get_function(arg):
                 raise ValueError(
                     "`get_environment_capability` function arguments"
                     " can't be complex values; only strings/ints/functions"
                     " are accepted. Instead, the item with index"
                     " {0} is {1} of type {2}".format(arg_index, arg, type(arg))
                 )
 
@@ -1133,15 +1120,15 @@
     def evaluate(self, handler):
         return handler.get_environment_capability(self.capability_path)
 
 
 class ValidateArgumentMixin(object):
     def _validate_argument(self,
                            argument_name,
-                           argument_type=text_type,
+                           argument_type=str,
                            validation_only=False):
         exception_cls = exceptions.FunctionValidationError if validation_only \
             else exceptions.FunctionEvaluationError
         value = getattr(self, argument_name)
         if get_function(value):
             if validation_only:
                 return
@@ -1255,15 +1242,15 @@
 @register(name='string_lower', func_eval_type=HYBRID_FUNC)
 class StringLower(Function, ValidateArgumentMixin):
     def __init__(self, *args, **kwargs):
         self.input = None
         super(StringLower, self).__init__(*args, **kwargs)
 
     def parse_args(self, args):
-        if isinstance(args, text_type) \
+        if isinstance(args, str) \
                 or (isinstance(args, dict) and len(args) == 1):
             self.input = args
         else:
             raise exceptions.FunctionValidationError(
                 self.name, 'should be called with exactly one parameter')
 
     def validate(self, plan):
@@ -1277,15 +1264,15 @@
 @register(name='string_upper', func_eval_type=HYBRID_FUNC)
 class StringUpper(Function, ValidateArgumentMixin):
     def __init__(self, *args, **kwargs):
         self.input = None
         super(StringUpper, self).__init__(*args, **kwargs)
 
     def parse_args(self, args):
-        if isinstance(args, text_type) \
+        if isinstance(args, str) \
                 or (isinstance(args, dict) and len(args) == 1):
             self.input = args
         else:
             raise exceptions.FunctionValidationError(
                 self.name, 'should be called with exactly one parameter')
 
     def validate(self, plan):
@@ -1463,50 +1450,58 @@
         storage=storage)
 
 
 def _clean_invalid_secrets(data_dict, storage):
     clean_dict = {}
     for k, v in data_dict.items():
         value = v['value']
-        if isinstance(value, dict) and 'get_secret' in value:
-            secret_key = value['get_secret']
-            if isinstance(value['get_secret'], list):
-                secret_key = secret_key[0]
-            try:
-                storage.secret_method(secret_key)
-            except Exception as e:
-                if hasattr(e, 'status_code') and e.status_code == 404:
-                    continue
-                else:
-                    raise
         clean_dict[k] = value
+        if not isinstance(value, dict) or 'get_secret' not in value:
+            continue
+        secret_key = value['get_secret']
+        if isinstance(value['get_secret'], list):
+            secret_key = secret_key[0]
+        if not isinstance(secret_key, str):
+            continue
+        try:
+            storage.secret_method(secret_key)
+        except Exception as e:
+            if hasattr(e, 'status_code') and e.status_code == 404:
+                del clean_dict[k]
+                continue
+            else:
+                raise
     return clean_dict
 
 
 def _args_to_str_func(handler, v, scope, context, path):
     """Used to display extra information when recursion limit is reached.
     This is the message-creating function used with an _EvaluationHandler,
     so it takes the same arguments as that.
     """
     return "Limit was reached with the following path - {0}".format(path)
 
 
 class _EvaluationHandler(object):
+    # if this is True, replace nested functions with their return values
+    # (if this is False, only go through the plan, and don't mutate it)
+    scan_replace = True
+
     @limit_recursion(50, args_to_str_func=_args_to_str_func)
     def __call__(self, v, scope, context, path):
         evaluated_value = v
         scanned = False
         while True:
             scan.scan_properties(
                 evaluated_value,
                 self,
                 scope=scope,
                 context=context,
                 path=path,
-                replace=True)
+                replace=self.scan_replace)
             func = parse(evaluated_value,
                          scope=scope,
                          context=context,
                          path=path)
             if not isinstance(func, Function):
                 break
             previous_evaluated_value = evaluated_value
@@ -1534,15 +1529,14 @@
         if not self._runtime_only_evaluation and \
                 func.func_eval_type in (HYBRID_FUNC, STATIC_FUNC):
             return_value = func.evaluate(self)
         else:
             if 'operation' in func.context:
                 func.context['operation']['has_intrinsic_functions'] = True
             return_value = func.raw
-        func.register_function_to_plan(self._plan)
         return return_value
 
     def get_input(self, input_name):
         try:
             return self._plan.inputs[input_name]
         except KeyError:
             raise exceptions.UnknownInputError(
@@ -1652,14 +1646,100 @@
         return self._storage.get_consumers(prop)
 
     @property
     def runtime_only_evaluation(self):
         return True
 
 
+class IDDSpec(object):
+    """Description of an inter-deployment-dependency.
+
+    Instances of IDDSpec describe a single dependency, based on an
+    IDDCreatingFunction.
+    Based on IDDSpec, we will be able to render actual instances of
+    inter-deployment-dependencies, containing links to actual node instances.
+    """
+    def __init__(
+        self,
+        scope: str,
+        context: Dict[str, str],
+        target_deployment: Union[str, Dict],
+        function_identifier: str,
+    ):
+        """Create an IDDSpec; this should only be created by IDDFindingHandler
+
+        :param scope: func.scope of the creating function ("node_template")
+        :param context: a dict containing optionally the keys:
+            - "node_name" - the node id - for node_template IDDs
+            - "target_node_name", "source_node_name" - the relationship
+              source and target node names - for relationship IDDs
+        :param target_deployment: the IDDCreatingFunction's target_deployment -
+            either a string target deployment id (if a literal was provided),
+            or a function representation (arbitrarily-nested dict)
+        :param function_identifier: the path of the IDDCreatingFunction,
+            for example "outputs.out1.value.get_capability"
+        """
+        self.scope = scope
+        self.context = context
+        self.target_deployment = target_deployment
+        self.function_identifier = function_identifier
+
+
+class IDDFindingHandler(_EvaluationHandler):
+    """An EvaluationHandler that goes through all functions, and stores IDDs.
+
+    Instead of recursively evaluating the functions, only recursively examine
+    them, and the functions that create inter-deployment-dependencies are
+    registered in the .dependencies list on this instance.
+    """
+    scan_replace = False
+
+    def __init__(self, plan):
+        self._plan = plan
+        self.dependencies = []
+
+    def evaluate_function(self, func):
+        if not isinstance(func, InterDeploymentDependencyCreatingFunction):
+            return
+        context = {}
+        if func.scope == 'node_template':
+            context['node_name'] = func.context['name']
+        elif func.scope == 'node_template_relationship':
+            context = {
+                'source_node_name': func.context['node_template']['name'],
+                'target_node_name': func.context['relationship']['target_id'],
+                'relationship_type': func.context['relationship']['type'],
+            }
+        dependency = IDDSpec(
+            func.scope,
+            context,
+            func.target_deployment,
+            func.function_identifier,
+        )
+        self.dependencies.append(dependency)
+
+
+class SecretFindingHandler(_EvaluationHandler):
+    """An EvaluationHandler that finds secret names used in the plan."""
+    scan_replace = False
+
+    def __init__(self, plan):
+        self._plan = plan
+        self.secrets = set()
+
+    def evaluate_function(self, func):
+        if not isinstance(func, GetSecret):
+            return
+        secret_name = func.secret_id
+        if isinstance(secret_name, list):
+            secret_name = secret_name[0]
+        if isinstance(secret_name, str):
+            self.secrets.add(secret_name)
+
+
 def plan_evaluation_handler(plan, runtime_only_evaluation=False):
     return _PlanEvaluationHandler(plan, runtime_only_evaluation)
 
 
 def runtime_evaluation_handler(storage):
     return _RuntimeEvaluationHandler(storage)
 
@@ -1677,20 +1757,48 @@
             path=path,
             replace=False)
         return v
 
     scan.scan_service_template(plan, handler, replace=False)
 
 
+def find_requirements(plan):
+    required_parent_capabilities = []
+    secrets = []
+
+    def handler(v, scope, context, path):
+        func = parse(v, scope=scope, context=context, path=path)
+        if isinstance(func, GetEnvironmentCapability):
+            required_parent_capabilities.append(func.capability_path)
+        elif isinstance(func, GetSecret):
+            secrets.append(func.secret_id)
+        scan.scan_properties(
+            v,
+            handler,
+            scope=scope,
+            context=context,
+            path=path,
+            replace=False)
+        return v
+
+    scan.scan_service_template(plan, handler, replace=False)
+
+    return {
+        'parent_capabilities': required_parent_capabilities,
+        'secrets': secrets,
+    }
+
+
 def get_nested_attribute_value_of_capability(root, path):
     value = root
     for index, attr in enumerate(path[2:]):
         if isinstance(value, dict):
             if attr not in value:
                 raise exceptions.FunctionEvaluationError(
+                    'get_capability',
                     "Attribute '{0}' doesn't exist in '{1}' "
                     "in deployment '{2}'.".format(
                         attr,
                         _convert_attribute_list_to_python_syntax_string(
                             path[1:index + 2]),
                         path[0]
                     )
@@ -1698,32 +1806,35 @@
 
             value = value[attr]
         elif isinstance(value, list):
             try:
                 value = value[attr]
             except TypeError:
                 raise exceptions.FunctionEvaluationError(
+                    'get_capability',
                     "Item in index {0} in the get_capability arguments "
                     "list [{1}] is expected to be an int "
                     "but got {2}.".format(
                         index + 2,
                         ', '.join('{0}'.format(item) for item in path),
                         type(attr).__name__))
             except IndexError:
                 raise exceptions.FunctionEvaluationError(
+                    'get_capability',
                     "List size of '{0}' is {1}, in "
                     "deployment '{2}', but index {3} is "
                     "retrieved.".format(
                         _convert_attribute_list_to_python_syntax_string(
                             path[1:index + 2]),
                         len(value),
                         path[0],
                         attr))
         else:
             raise exceptions.FunctionEvaluationError(
+                'get_capability',
                 "Object {0}, in capability '{1}' in deployment '{2}', "
                 "has no attribute {3}".format(
                     _convert_attribute_list_to_python_syntax_string(
                         path[2:index + 2]),
                     path[1],
                     path[0],
                     attr))
```

### Comparing `cloudify-common-6.4.2/dsl_parser/holder.py` & `cloudify-common-7.0.0/dsl_parser/holder.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,23 @@
                              'is of type {0}'
                              .format(type(self.value).__name__))
         for key_holder, value_holder in self.value.items():
             if key_holder.value == key:
                 return key_holder, value_holder
         return None, None
 
+    def set_item(self, key, value):
+        if not isinstance(self.value, dict):
+            raise ValueError('Value is expected to be a dictionary while it '
+                             'is of type {0}'
+                             .format(type(self.value).__name__))
+        self.value.update({
+            Holder.of(key): Holder.of(value)
+        })
+
     def restore(self):
         if isinstance(self.value, dict):
             return dict((key_holder.restore(), value_holder.restore())
                         for key_holder, value_holder in self.value.items())
         elif isinstance(self.value, list):
             return [value_holder.restore() for value_holder in self.value]
         elif isinstance(self.value, set):
@@ -111,7 +120,14 @@
                       start_column=self.start_column,
                       end_line=self.end_line,
                       end_column=self.end_column,
                       filename=self.filename,
                       namespace=self.namespace,
                       is_cloudify_type=self.is_cloudify_type,
                       only_children_namespace=self.only_children_namespace)
+
+    def keys(self):
+        if not isinstance(self.value, dict):
+            raise ValueError('Value is expected to be a dictionary while it '
+                             'is of type {0}'
+                             .format(type(self.value).__name__))
+        return [k.value for k in self.value.keys()]
```

### Comparing `cloudify-common-6.4.2/dsl_parser/import_resolver/__init__.py` & `cloudify-common-7.0.0/dsl_parser/import_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/import_resolver/abstract_import_resolver.py` & `cloudify-common-7.0.0/dsl_parser/import_resolver/abstract_import_resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  * See the License for the specific language governing permissions and
 #  * limitations under the License.
 
 import abc
+import time
 
 import requests
-from retrying import retry
 
 from dsl_parser import exceptions
-from dsl_parser._compat import ABC
-
+from cloudify.manager import get_resource_from_manager
 
 DEFAULT_RETRY_DELAY = 1
 MAX_NUMBER_RETRIES = 5
 DEFAULT_REQUEST_TIMEOUT = 10
 
 
 def is_remote_resource(resource_url):
     url_parts = resource_url.split(':')
     if url_parts[0] in ['http', 'https', 'file', 'ftp', 'plugin', 'blueprint']:
         return True
 
 
-class AbstractImportResolver(ABC):
+class AbstractImportResolver(abc.ABC):
     """
     This class is abstract and should be inherited by concrete
     implementations of import resolver.
     The only mandatory implementation is of resolve, which is expected
     to open the import url and return its data.
     """
 
@@ -59,32 +58,34 @@
     error_str = 'Import failed: Unable to open import url'
     if import_url.startswith('file:'):
         try:
             filename = import_url[len('file:'):]
             with open(filename) as f:
                 return f.read()
         except Exception as ex:
-            ex = exceptions.DSLParsingLogicException(
-                13, '{0} {1}; {2}'.format(error_str, import_url, ex))
-            raise ex
+            raise exceptions.DSLParsingLogicException(
+                13, f"{error_str} {import_url}; {ex}")
+    elif import_url.startswith('resource:'):
+        try:
+            filename = import_url[len('resource:'):]
+            return get_resource_from_manager(filename)
+        except Exception as ex:
+            raise exceptions.DSLParsingLogicException(
+                13, f"{error_str} {import_url}; {ex}")
     else:
         number_of_attempts = MAX_NUMBER_RETRIES + 1
 
         # Defines on which errors we should retry the import.
         def _is_recoverable_error(e):
             return isinstance(e, (requests.ConnectionError, requests.Timeout))
 
         # Defines on which return values we should retry the import.
         def _is_internal_error(result):
             return hasattr(result, 'status_code') and result.status_code >= 500
 
-        @retry(stop_max_attempt_number=number_of_attempts,
-               wait_fixed=DEFAULT_RETRY_DELAY,
-               retry_on_exception=_is_recoverable_error,
-               retry_on_result=_is_internal_error)
         def get_import():
             response = requests.get(import_url,
                                     timeout=DEFAULT_REQUEST_TIMEOUT)
             # The response is a valid one, and the content should be returned
             if 200 <= response.status_code < 300:
                 return response.text
             # If the response status code is above 500, an internal server
@@ -95,23 +96,40 @@
             # Any other response should raise an exception.
             else:
                 invalid_url_err = exceptions.DSLParsingLogicException(
                     13, '{0} {1}; status code: {2}'.format(
                         error_str, import_url, response.status_code))
                 raise invalid_url_err
 
+        def get_import_wrapper():
+            exception_caught = None
+            for attempt in range(number_of_attempts):
+                try:
+                    result = get_import()
+                    if not _is_internal_error(result):
+                        return result
+                except Exception as ex:
+                    if not _is_recoverable_error(ex):
+                        raise ex
+                    else:
+                        exception_caught = ex
+                time.sleep(DEFAULT_RETRY_DELAY)
+            if exception_caught:
+                raise exception_caught
+
         try:
-            import_result = get_import()
+            import_result = get_import_wrapper()
             # If the error is an internal error only. A custom exception should
             # be raised.
             if _is_internal_error(import_result):
-                msg = 'Import failed {0} times, due to internal server error' \
-                      '; {1}'.format(number_of_attempts, import_result.text)
-                raise exceptions.DSLParsingLogicException(13, msg)
+                raise exceptions.DSLParsingLogicException(
+                    13,
+                    f"Import failed {number_of_attempts} times, "
+                    f"due to internal server error; {import_result.text}"
+                )
             return import_result
         # If any ConnectionError, Timeout or URLRequired should rise
         # after the retrying mechanism, a custom exception will be raised.
         except (requests.ConnectionError, requests.Timeout,
-                requests.URLRequired) as err:
-
+                requests.URLRequired) as ex:
             raise exceptions.DSLParsingLogicException(
-                13, '{0} {1}; {2}'.format(error_str, import_url, err))
+                13, f"{error_str} {import_url}; {ex}")
```

### Comparing `cloudify-common-6.4.2/dsl_parser/import_resolver/default_import_resolver.py` & `cloudify-common-7.0.0/dsl_parser/import_resolver/default_import_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,9 +173,13 @@
             result = [yaml_file for yaml_file in yaml_files
                       if '{0}.yaml'.format(dsl_version) in yaml_file]
             if result:
                 return result
 
         # Return the first file that does not match *_\d_\d+\.yaml pattern
         for yaml_file in yaml_files:
-            if not re.match(r"_\d_\d+\.yaml$", yaml_file):
+            if not re.search(r"_\d_\d+\.yaml$", yaml_file):
                 return [yaml_file]
+
+        # If dsl_version is not provided, return the last yaml_file
+        if not dsl_version:
+            return [sorted(yaml_files)[-1]]
```

### Comparing `cloudify-common-6.4.2/dsl_parser/interfaces/constants.py` & `cloudify-common-7.0.0/dsl_parser/interfaces/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/interfaces/interfaces_merger.py` & `cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_merger.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/interfaces/interfaces_parser.py` & `cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/interfaces/operation_merger.py` & `cloudify-common-7.0.0/dsl_parser/interfaces/operation_merger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
-from dsl_parser._compat import text_type
 from dsl_parser.interfaces.constants import NO_OP
 from dsl_parser.interfaces.utils import (operation_mapping,
                                          merge_schema_and_instance_inputs)
 
 
 class OperationMerger(object):
 
     @staticmethod
     def _create_operation(raw_operation):
         if raw_operation is None:
             return None
-        if isinstance(raw_operation, text_type):
+        if isinstance(raw_operation, str):
             return operation_mapping(
                 implementation=raw_operation,
                 inputs={},
                 executor=None,
                 max_retries=None,
                 retry_interval=None,
                 timeout=None,
```

### Comparing `cloudify-common-6.4.2/dsl_parser/interfaces/utils.py` & `cloudify-common-7.0.0/dsl_parser/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/models.py` & `cloudify-common-7.0.0/dsl_parser/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             policy_types={},
             policy_triggers={},
             description=None,
             groups={},
             capabilities={},
             resource_tags=None,
             labels={},
+            requirements={},
         )
         self.update(plan)
 
     @property
     def version(self):
         return self['version']
```

### Comparing `cloudify-common-6.4.2/dsl_parser/multi_instance.py` & `cloudify-common-7.0.0/dsl_parser/multi_instance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/dsl_parser/parser.py` & `cloudify-common-7.0.0/dsl_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             'validate_version': validate_version
         },
         element_cls=blueprint.Blueprint)
     if validate_input_defaults:
         constraints.validate_input_defaults(plan)
     if validate_intrinsic_function:
         functions.validate_functions(plan)
+    plan['requirements'] = functions.find_requirements(plan)
     return plan, merged_blueprint_holder
 
 
 def _resolve_blueprint_imports(dsl_location,
                                dsl_string,
                                resolver,
                                resources_base_path,
```

### Comparing `cloudify-common-6.4.2/dsl_parser/rel_graph.py` & `cloudify-common-7.0.0/dsl_parser/rel_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,19 @@
 import copy
 import collections
 from random import choice
 from string import ascii_lowercase, digits
 
 from networkx.algorithms import (
     descendants,
-    topological_sort,
-    weakly_connected_component_subgraphs,
+    weakly_connected_components,
 )
 from networkx.classes import DiGraph
 
-from dsl_parser import (constants,
-                        exceptions)
+from dsl_parser import (constants, exceptions, utils)
 
 NODES = 'nodes'
 RELATIONSHIPS = 'relationships'
 DEPENDS_ON_REL_TYPE = constants.DEPENDS_ON_REL_TYPE
 CONNECTED_TO_REL_TYPE = constants.CONNECTED_TO_REL_TYPE
 CONTAINED_IN_REL_TYPE = constants.CONTAINED_IN_REL_TYPE
 GROUP_CONTAINED_IN_REL_TYPE = '__group_contained_in__'
@@ -96,15 +94,15 @@
                     node_id in contained_in_group):
                 group_name = contained_in_group[node_id]
                 relationship['target_id'] = group_name
                 relationship['replaced'] = target_id
                 graph.add_edge(node_id, group_name,
                                relationship=relationship,
                                index=index)
-                top_level_group_name = topological_sort(
+                top_level_group_name = utils.topological_sort(
                     groups_graph, nbunch=[group_name])[-1]
                 graph.add_edge(
                     top_level_group_name, target_id,
                     relationship={
                         'type': GROUP_CONTAINED_IN_REL_TYPE,
                         constants.TYPE_HIERARCHY:
                             [GROUP_CONTAINED_IN_REL_TYPE],
@@ -219,15 +217,15 @@
         modified_nodes=modified_nodes,
         existing_node_instance_ids=existing_ni_ids)
 
     _handle_contained_in(ctx)
 
     ctx.node_instance_ids = existing_ni_ids or collections.defaultdict(set)
     ctx.deployment_node_instance_ids.clear()
-    for node_instance_id, data in deployment_node_graph.nodes_iter(
+    for node_instance_id, data in deployment_node_graph.nodes(
             data=True):
         node_id = _node_id_from_node_instance(data['node'])
         ctx.node_instance_ids[node_id].add(node_instance_id)
         ctx.deployment_node_instance_ids[node_id].add(node_instance_id)
 
     _handle_connected_to_and_depends_on(ctx)
 
@@ -239,25 +237,25 @@
 def extract_node_instances(node_instances_graph,
                            ctx,
                            copy_instances=False,
                            contained_graph=None):
     contained_graph = contained_graph or ctx.deployment_contained_graph
     added_missing_node_instance_ids = set()
     node_instances = []
-    for node_instance_id, data in node_instances_graph.nodes_iter(data=True):
+    for node_instance_id, data in node_instances_graph.nodes(data=True):
         node_instance = data['node']
         if node_instance.get('group'):
             continue
         node_instance_attributes = data.get('node_instance_attributes')
         if copy_instances:
             node_instance = copy.deepcopy(node_instance)
         if node_instance_attributes:
             node_instance.update(node_instance_attributes)
         indexed_relationship_instances = []
-        for target_node_instance_id in node_instances_graph.neighbors_iter(
+        for target_node_instance_id in node_instances_graph.neighbors(
                 node_instance_id):
             edge_data = node_instances_graph[node_instance_id][
                 target_node_instance_id]
             relationship_instance = edge_data['relationship']
             relationship_index = edge_data['index']
             if copy_instances:
                 relationship_instance = copy.deepcopy(relationship_instance)
@@ -286,16 +284,16 @@
                     # In deployment modification, if an instance is contained
                     # in a node and that node is not new, it needs to be added
                     # as a "related" node. Added and removed nodes are marked
                     # as such, so all we need to do is add this node with
                     # no relationships
                     if (target_id not in node_instances_graph and
                             target_id not in added_missing_node_instance_ids):
-                        target_node_instance = contained_graph.node[target_id][
-                            'node']
+                        target_node_instance = contained_graph\
+                            .nodes[target_id]['node']
                         if copy_instances:
                             target_node_instance = copy.deepcopy(
                                 target_node_instance)
                         target_node_instance[RELATIONSHIPS] = []
                         node_instances.append(target_node_instance)
                         added_missing_node_instance_ids.add(target_id)
             if not group_rel:
@@ -363,69 +361,70 @@
         ctx=ctx,
         copy_instances=True,
         contained_graph=ctx.previous_deployment_contained_graph)
 
 
 def _graph_diff(G, H, node_instance_attributes):
     result = DiGraph()
-    for n1, data in G.nodes_iter(data=True):
+    for n1, data in G.nodes(data=True):
         if n1 in H:
             continue
-        result.add_node(n1, data,
+        result.add_node(n1, **data,
                         node_instance_attributes=node_instance_attributes)
-        for n2 in G.neighbors_iter(n1):
-            result.add_node(n2, G.node[n2])
-            result.add_edge(n1, n2, G[n1][n2])
-        for n2 in G.predecessors_iter(n1):
-            result.add_node(n2, G.node[n2])
-            result.add_edge(n2, n1, G[n2][n1])
+        for n2 in G.neighbors(n1):
+            result.add_node(n2, **G.nodes[n2])
+            result.add_edge(n1, n2, **G[n1][n2])
+        for n2 in G.predecessors(n1):
+            result.add_node(n2, **G.nodes[n2])
+            result.add_edge(n2, n1, **G[n2][n1])
     return result
 
 
 def _graph_diff_relationships(G, H, node_instance_attributes):
     """
     G represents the base and H represents the changed graph.
     :param G:
     :param H:
     :param node_instance_attributes:
     :return:
     """
     result = DiGraph()
-    for source, dest, data in G.edges_iter(data=True):
+    for source, dest, data in G.edges(data=True):
         if source in H and dest not in H[source]:
-            new_node = copy.deepcopy(G.node[source])
-            result.add_node(source, new_node,
+            new_node = copy.deepcopy(G.nodes[source])
+            result.add_node(source, **new_node,
                             node_instance_attributes=node_instance_attributes)
-            result.add_node(dest, G.node[dest])
-            result.add_edge(source, dest, G[source][dest])
+            result.add_node(dest, **G.nodes[dest])
+            result.add_edge(source, dest, **G[source][dest])
     return result
 
 
 def _handle_contained_in(ctx):
     # for each 'contained' tree, recursively build new trees based on
     # scaling groups with generated ids
-    for contained_tree in weakly_connected_component_subgraphs(
-            ctx.plan_contained_graph.reverse(copy=True)):
+    g = ctx.plan_contained_graph.reverse(copy=True)
+    for contained_tree in [g.subgraph(c)
+                           for c in weakly_connected_components(g)]:
         # extract tree root node id
-        node_id = topological_sort(contained_tree)[0]
+        node_id = utils.topological_sort(contained_tree)[0]
         _build_multi_instance_node_tree_rec(
             node_id=node_id,
             contained_tree=contained_tree,
             ctx=ctx)
     ctx.deployment_contained_graph = ctx.deployment_node_graph.copy()
 
 
 def _build_multi_instance_node_tree_rec(node_id,
                                         contained_tree,
                                         ctx,
                                         parent_relationship=None,
                                         parent_relationship_index=None,
                                         parent_node_instance_id=None,
                                         current_host_instance_id=None):
-    node = contained_tree.node[node_id]['node']
+    node = contained_tree.nodes[node_id]['node']
     containers = _build_and_update_node_instances(
         ctx=ctx,
         node=node,
         parent_node_instance_id=parent_node_instance_id,
         parent_relationship=parent_relationship,
         current_host_instance_id=current_host_instance_id)
     for container in containers:
@@ -436,15 +435,15 @@
         ctx.deployment_node_graph.add_node(node_instance_id,
                                            node=node_instance)
         if parent_node_instance_id is not None:
             ctx.deployment_node_graph.add_edge(
                 node_instance_id, parent_node_instance_id,
                 relationship=relationship_instance,
                 index=parent_relationship_index)
-        for child_node_id in contained_tree.neighbors_iter(node_id):
+        for child_node_id in contained_tree.neighbors(node_id):
             _descendants = descendants(contained_tree, child_node_id)
             _descendants.add(child_node_id)
             child_contained_tree = contained_tree.subgraph(_descendants)
             _build_multi_instance_node_tree_rec(
                 node_id=child_node_id,
                 contained_tree=child_contained_tree,
                 ctx=ctx,
@@ -458,15 +457,15 @@
 
 def _build_and_update_node_instances(ctx,
                                      node,
                                      parent_node_instance_id,
                                      parent_relationship,
                                      current_host_instance_id):
     node_id = node['id']
-    current_instances_num = ctx.plan_node_graph.node[node_id][
+    current_instances_num = ctx.plan_node_graph.nodes[node_id][
         'scale_properties']['current_instances']
     new_instances_num = 0
     previous_containers = []
     if ctx.is_modification:
         all_previous_node_instance_ids = ctx.deployment_node_instance_ids[
             node_id]
         previous_node_instance_ids = [
@@ -492,15 +491,15 @@
                                           total_instances_num,
                                           modified_node,
                                           ctx)
         else:
             new_instances_num = (current_instances_num -
                                  previous_instances_num)
         previous_node_instances = [
-            ctx.previous_deployment_node_graph.node[node_instance_id]['node']
+            ctx.previous_deployment_node_graph.nodes[node_instance_id]['node']
             for node_instance_id in previous_node_instance_ids]
         previous_containers = [Container(node_instance,
                                          _extract_contained(node,
                                                             node_instance),
                                          node_instance.get('host_id'))
                                for node_instance in previous_node_instances]
     else:
@@ -658,18 +657,18 @@
             connection_type=connection_type,
             relationship_target_ids=relationship_target_ids)
 
 
 def _build_previous_target_ids_for_all_to_one(ctx):
     relationship_target_ids = {}
     if ctx.is_modification:
-        for s, t, e_data in ctx.previous_deployment_node_graph.edges_iter(
+        for s, t, e_data in ctx.previous_deployment_node_graph.edges(
                 data=True):
-            s_node = ctx.previous_deployment_node_graph.node[s]['node']
-            t_node = ctx.previous_deployment_node_graph.node[t]['node']
+            s_node = ctx.previous_deployment_node_graph.nodes[s]['node']
+            t_node = ctx.previous_deployment_node_graph.nodes[t]['node']
             rel = e_data['relationship']
             key = (_node_id_from_node_instance(s_node),
                    _node_id_from_node_instance(t_node),
                    rel['type'])
             if key not in relationship_target_ids:
                 relationship_target_ids[key] = set()
             target_ids = relationship_target_ids[key]
@@ -775,15 +774,15 @@
     for key, value in source_scaling_groups_map.items():
         partitioned_node_instance_ids.append((value,
                                               target_scaling_groups_map[key]))
     return partitioned_node_instance_ids
 
 
 def _build_scaling_groups_map(ctx, node_instance_ids, group):
-    node_instances = [ctx.deployment_node_graph.node[n]['node']
+    node_instances = [ctx.deployment_node_graph.nodes[n]['node']
                       for n in node_instance_ids]
     scaling_groups_map = collections.defaultdict(list)
     for node_instance in node_instances:
         node_instance_id = node_instance['id']
         group_id = ctx.containing_group_id(
             node_instance_id=node_instance_id,
             group_name=group)
@@ -832,15 +831,15 @@
     return result
 
 
 # currently we have decided not to support such relationships
 # until we better understand what semantics are required for such
 # relationships
 def _verify_no_unsupported_relationships(graph):
-    for s, t, edge in graph.edges_iter(data=True):
+    for s, t, edge in graph.edges(data=True):
         if not _relationship_type_hierarchy_includes_one_of(
                 edge['relationship'], [
                     DEPENDS_ON_REL_TYPE,
                     CONTAINED_IN_REL_TYPE,
                     CONNECTED_TO_REL_TYPE,
                     GROUP_CONTAINED_IN_REL_TYPE]):
             raise exceptions.UnsupportedRelationship()
@@ -888,23 +887,23 @@
             previous_deployment_contained_graph)
         self.modified_nodes = modified_nodes
         self.node_instance_ids = \
             existing_node_instance_ids or collections.defaultdict(set)
         self.deployment_node_instance_ids = collections.defaultdict(set)
         if self.is_modification:
             for node_instance_id, data in \
-                    self.previous_deployment_node_graph.nodes_iter(data=True):
+                    self.previous_deployment_node_graph.nodes(data=True):
                 self.deployment_node_instance_ids[
                     _node_id_from_node_instance(data['node'])].add(
                     node_instance_id)
 
     def get_group_member_mapping(self):
         group_member_mapping = {}
         for instance_id, details in (
-            self.previous_deployment_node_graph.nodes_iter(data=True)
+            self.previous_deployment_node_graph.nodes(data=True)
         ):
             for scaling_group in details.get('node',
                                              {}).get('scaling_groups', []):
                 scaling_group_id = scaling_group['id']
                 if scaling_group_id not in group_member_mapping:
                     group_member_mapping[scaling_group_id] = []
                 group_member_mapping[scaling_group_id].append(
@@ -918,40 +917,40 @@
 
     def minimal_containing_group(self, node_a, node_b):
         a_groups = self._containing_groups(node_a)
         b_groups = self._containing_groups(node_b)
         shared_groups = set(a_groups) & set(b_groups)
         if not shared_groups:
             return None
-        return topological_sort(self.plan_contained_graph,
-                                nbunch=shared_groups)[0]
+        return utils.topological_sort(self.plan_contained_graph,
+                                      nbunch=shared_groups)[0]
 
     def _containing_groups(self, node_id):
         graph = self.plan_contained_graph
         result = []
         while True:
             succ = graph.succ[node_id]
             if succ:
                 assert len(succ) == 1
                 node_id = list(succ.keys())[0]
-                if not graph.node[node_id]['node'].get('group'):
+                if not graph.nodes[node_id]['node'].get('group'):
                     continue
                 result.append(node_id)
             else:
                 break
         return result
 
     def containing_group_id(self, node_instance_id, group_name):
         graph = self.deployment_contained_graph
         while True:
             succ = graph.succ[node_instance_id]
             if succ:
                 assert len(succ) == 1
                 node_instance_id = list(succ.keys())[0]
-                node = graph.node[node_instance_id]['node']
+                node = graph.nodes[node_instance_id]['node']
                 if not node.get('group'):
                     continue
                 if _node_id_from_node_instance(node) == group_name:
                     return node['id']
             else:
                 return None
 
@@ -960,27 +959,27 @@
                                    contained_graph):
         result = []
         while True:
             succ = contained_graph.succ[instance_id]
             if succ:
                 assert len(succ) == 1
                 node_instance_id = list(succ.keys())[0]
-                node = contained_graph.node[node_instance_id]['node']
+                node = contained_graph.nodes[node_instance_id]['node']
                 instance_id = node['id']
                 result.append({
                     'name': _node_id_from_node_instance(node),
                     'id': instance_id
                 })
                 if not node.get('group'):
                     return result[:-1], result[-1]
             else:
                 return result, None
 
     def restore_plan_node_graph(self):
-        for _, data in self.plan_node_graph.nodes_iter(data=True):
+        for _, data in self.plan_node_graph.nodes(data=True):
             node = data['node']
             for relationship in node.get('relationships', []):
                 replaced = relationship.pop('replaced', None)
                 if replaced:
                     relationship['target_id'] = replaced
 
     def _build_connected_to_and_depends_on_graph(self, graph):
@@ -995,32 +994,32 @@
         result = self._build_graph_by_relationship_types(
             graph,
             build_from_types=[CONTAINED_IN_REL_TYPE,
                               GROUP_CONTAINED_IN_REL_TYPE],
             exclude_types=[])
         # don't forget to include nodes in this graph that no one is contained
         # in them (these will be considered 1 node trees)
-        result.add_nodes_from(graph.nodes_iter(data=True))
+        result.add_nodes_from(graph.nodes(data=True))
         return result
 
     @staticmethod
     def _build_graph_by_relationship_types(graph,
                                            build_from_types,
                                            exclude_types):
         relationship_base_graph = DiGraph()
-        for source, target, edge_data in graph.edges_iter(data=True):
+        for source, target, edge_data in graph.edges(data=True):
             include_edge = (
                 _relationship_type_hierarchy_includes_one_of(
                     edge_data['relationship'], build_from_types) and not
                 _relationship_type_hierarchy_includes_one_of(
                     edge_data['relationship'], exclude_types))
             if include_edge:
-                relationship_base_graph.add_node(source, graph.node[source])
-                relationship_base_graph.add_node(target, graph.node[target])
-                relationship_base_graph.add_edge(source, target, edge_data)
+                relationship_base_graph.add_node(source, **graph.nodes[source])
+                relationship_base_graph.add_node(target, **graph.nodes[target])
+                relationship_base_graph.add_edge(source, target, **edge_data)
         return relationship_base_graph
 
 
 class Container(object):
 
     def __init__(self,
                  node_instance,
```

### Comparing `cloudify-common-6.4.2/dsl_parser/scan.py` & `cloudify-common-7.0.0/dsl_parser/scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,19 +29,14 @@
 OUTPUTS_SCOPE = 'outputs'
 POLICIES_SCOPE = 'policies'
 SCALING_GROUPS_SCOPE = 'scaling_groups'
 CAPABILITIES_SCOPE = 'capabilities'
 LABELS_SCOPE = 'labels'
 DEPLOYMENT_SETTINGS_SCOPE = 'deployment_settings'
 
-# Searching for secrets in the blueprint only one time of the few times
-# that scan_service_template is called
-collect_secrets = False
-secrets = set()
-
 
 def scan_properties(value,
                     handler,
                     scope=None,
                     context=None,
                     path='',
                     replace=False):
@@ -66,34 +61,24 @@
     :param path: The properties base path.
     :param replace: whether to do an in-place replacement or not.
     """
     if isinstance(value, dict):
         for k, v in value.items():
             current_path = '{0}.{1}'.format(path, k)
             result = handler(v, scope, context, current_path)
-            _collect_secret(result)
             if replace and result != v:
                 value[k] = result
     elif isinstance(value, list):
         for index, item in enumerate(value):
             current_path = '{0}[{1}]'.format(path, index)
             result = handler(item, scope, context, current_path)
-            _collect_secret(result)
             if replace and result != item:
                 value[index] = result
 
 
-def _collect_secret(value):
-    if collect_secrets and isinstance(value, dict) and 'get_secret' in value:
-        secret_name = value['get_secret']
-        if isinstance(value['get_secret'], list):
-            secret_name = secret_name[0]
-        secrets.add(secret_name)
-
-
 def _scan_operations(operations,
                      handler,
                      scope=None,
                      context=None,
                      path='',
                      replace=False):
     for name, definition in operations.items():
@@ -133,18 +118,15 @@
                          context=context,
                          path='{0}.{1}.{2}'.format(NODES,
                                                    node_template['name'],
                                                    r['type']),
                          replace=replace)
 
 
-def scan_service_template(plan, handler, replace=False, search_secrets=False):
-    global collect_secrets
-    collect_secrets = search_secrets
-
+def scan_service_template(plan, handler, replace=False):
     for node_template in plan.node_templates:
         scan_node_template(node_template, handler, replace=replace)
         scan_node_operation_properties(node_template, handler, replace=replace)
     for output_name, output in plan.outputs.items():
         scan_properties(output,
                         handler,
                         scope=OUTPUTS_SCOPE,
@@ -191,18 +173,14 @@
     scan_properties(plan.get('deployment_settings'),
                     handler,
                     scope=DEPLOYMENT_SETTINGS_SCOPE,
                     context=plan,
                     path=DEPLOYMENT_SETTINGS,
                     replace=replace)
 
-    if collect_secrets and len(secrets) > 0:
-        plan['secrets'] = list(secrets)
-        secrets.clear()
-
 
 def scan_node_template(node_template, handler, replace=False):
     scan_properties(node_template[PROPERTIES],
                     handler,
                     scope=NODE_TEMPLATE_SCOPE,
                     context=node_template,
                     path='{0}.{1}.{2}'.format(
```

### Comparing `cloudify-common-6.4.2/dsl_parser/tasks.py` & `cloudify-common-7.0.0/dsl_parser/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import copy
 import json
+from typing import List
 
 from dsl_parser import (scan,
                         utils,
                         models,
                         parser,
                         functions,
                         exceptions,
                         constraints,
                         multi_instance)
-from dsl_parser.constants import INPUTS, DEFAULT, DATA_TYPES, TYPE, ITEM_TYPE
+from dsl_parser.constants import (
+    INPUTS, DEFAULT, DATA_TYPES, TYPE, ITEM_TYPE, INTER_DEPLOYMENT_FUNCTIONS,
+)
 from dsl_parser.multi_instance import modify_deployment
 
 
 __all__ = [
     'modify_deployment'
 ]
 
@@ -140,39 +143,148 @@
                                           list(plan[INPUTS])))
 
     plan[INPUTS] = inputs
 
 
 def _process_functions(plan, runtime_only_evaluation=False):
     handler = functions.plan_evaluation_handler(plan, runtime_only_evaluation)
-    scan.scan_service_template(
-        plan, handler, replace=True, search_secrets=True)
+    scan.scan_service_template(plan, handler, replace=True)
 
 
-def _validate_secrets(plan, get_secret_method):
-    if 'secrets' not in plan:
-        return
+def _find_idd_creating_functions(plan) -> List[functions.IDDSpec]:
+    handler = functions.IDDFindingHandler(plan)
+    scan.scan_service_template(plan, handler, replace=False)
+    return handler.dependencies
+
+
+def _find_rel_target_by_iddspec(relationships, idd_spec):
+    """Find the target instance that matches the relationship in IDDSpec
+
+    The node-instance can have many relationships, so we need to find one
+    that matches the target node name & type.
+    If there's multiple relationships of the same type to the same node,
+    then we will just select the first instance, because we have no way
+    to distinguish them.
+    (that case shouldn't be possible anyway)
+    """
+    assert idd_spec.scope == 'node_template_relationship'
+
+    target_name = idd_spec.context['target_node_name']
+    rel_type = idd_spec.context['relationship_type']
+
+    for relationship in relationships:
+        if (
+            target_name == relationship['target_name']
+            and rel_type == relationship['type']
+        ):
+            return relationship['target_id']
+
+    node_name = idd_spec.context['node']
+    raise ValueError(
+        'IDDs: relationship not found: {0} {1} {2}'
+        .format(node_name, rel_type, target_name),
+    )
+
+
+def _format_idds(plan, dep_specs):
+    """Format IDDSpecs into actual dependencies by choosing the node-instances.
+
+    IDDSpecs will contain just node name, but there can be many node instances
+    for a given node name, so we need to expand every such IDDSpec into
+    multiple actual IDD dicts.
+
+    This returns a list of dicts containing the keys:
+        - function_identifier - the IDDCreatingFunction path
+        - target_deployment - the deployment id, or a dict representing
+          a function call
+        - context - a dict containing possibly the keys SELF, TARGET, SOURCE -
+          this is the context that can be passed into function evaluation,
+          when evaluating the target_deployment (if it is a function)
+    """
+    idds = []
+    nis_by_node = {}
+    for ni in plan.get('node_instances', []):
+        node_name = ni['node_id']
+        nis_by_node.setdefault(node_name, []).append(ni)
+
+    for idd_spec in dep_specs:
+        idd_base = {
+            'function_identifier': idd_spec.function_identifier,
+            'target_deployment': idd_spec.target_deployment,
+        }
+
+        if idd_spec.scope == 'node_template':
+            # the IDDSpec is a node one (e.g. in node properties):
+            # create an instance of IDD, for every node-instance of the node
+            node_name = idd_spec.context['node_name']
+            for ni in nis_by_node[node_name]:
+                idd = idd_base.copy()
+                idd['context'] = {
+                    'self': ni['id'],
+                }
+                idds.append(idd)
+
+        elif idd_spec.scope == 'node_template_relationship':
+            # the IDDSpec is a relationship one (e.g. in relationship operation
+            # inputs) - create an instance of IDD for every node-instance of
+            # the source node
+            node_name = idd_spec.context['source_node_name']
+
+            for ni in nis_by_node[node_name]:
+                target_id = _find_rel_target_by_iddspec(
+                    ni.get('relationships', []),
+                    idd_spec,
+                )
+                idd = idd_base.copy()
+                idd['context'] = {
+                    'self': ni['id'],
+                    'source': ni['id'],
+                    'target': target_id,
+                }
+                idds.append(idd)
+        else:
+            # other IDDSpec - e.g. outputs, capabilities, etc. Those can be
+            # evaluated without any additional context.
+            idd = idd_base.copy()
+            idd['context'] = {}
+            idds.append(idd)
+    return idds
+
+
+def _find_secrets(plan):
+    """Find secret names used in the plan.
+
+    Secret names that are non-evaluated (e.g. based on get_attribute calls)
+    are not returned, only secret names known at plan creation time
+    """
+    handler = functions.SecretFindingHandler(plan)
+    scan.scan_service_template(plan, handler, replace=False)
+    return handler.secrets
+
 
+def _validate_secrets(secrets, get_secret_method):
     # Mainly for local workflow that doesn't support secrets
+    if not secrets:
+        return
+
     if get_secret_method is None:
         raise exceptions.UnsupportedGetSecretError(
             "The get_secret intrinsic function is not supported"
         )
 
     invalid_secrets = []
-    for secret_key in plan['secrets']:
+    for secret_key in secrets:
         try:
             get_secret_method(secret_key)
         except Exception as exception:
             if hasattr(exception, 'status_code')\
                     and exception.status_code == 404:
                 invalid_secrets.append(secret_key)
             else:
                 raise
-    plan.pop('secrets')
 
     if invalid_secrets:
         raise exceptions.UnknownSecretError(
             "Required secrets: [{0}] don't exist in this tenant"
             .format(', '.join(s for s in invalid_secrets))
         )
 
@@ -185,9 +297,13 @@
                             **_):
     """
     Prepare a plan for deployment
     """
     plan = models.Plan(copy.deepcopy(plan))
     _set_plan_inputs(plan, inputs, auto_correct_types, values_getter)
     _process_functions(plan, runtime_only_evaluation)
-    _validate_secrets(plan, get_secret_method)
-    return multi_instance.create_deployment_plan(plan, existing_ni_ids)
+    secrets = _find_secrets(plan)
+    _validate_secrets(secrets, get_secret_method)
+    dep_specs = _find_idd_creating_functions(plan)
+    dep_plan = multi_instance.create_deployment_plan(plan, existing_ni_ids)
+    dep_plan[INTER_DEPLOYMENT_FUNCTIONS] = _format_idds(dep_plan, dep_specs)
+    return dep_plan
```

### Comparing `cloudify-common-6.4.2/dsl_parser/utils.py` & `cloudify-common-7.0.0/dsl_parser/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 import copy
 import contextlib
 import importlib
 import numbers
 import sys
 import re
 
+from networkx import NetworkXError, NetworkXUnfeasible
+
 import yaml.parser
 
-from dsl_parser._compat import (
-    urlparse, text_type, reraise, Request, urlopen, URLError)
+from urllib.error import URLError
+from urllib.parse import urlparse
+from urllib.request import Request, urlopen
+
 from dsl_parser.constants import (
     RESOLVER_IMPLEMENTATION_KEY,
     RESLOVER_PARAMETERS_KEY,
     NAMESPACE_DELIMITER
 )
 from dsl_parser.import_resolver.default_import_resolver import (
     DefaultImportResolver
@@ -194,18 +198,19 @@
                 value, bool):
             return value, True
     elif type_name == 'boolean':
         if isinstance(value, bool):
             return value, True
     elif type_name in ('string', 'textarea', 'deployment_id', 'blueprint_id',
                        'node_id', 'node_type', 'node_instance',
-                       'capability_value', 'scaling_group', 'secret_key'):
+                       'capability_value', 'scaling_group', 'secret_key',
+                       'operation_name', ):
         return value, True
     elif type_name == 'regex':
-        if isinstance(value, text_type):
+        if isinstance(value, str):
             try:
                 re.compile(value)
                 return value, True
             except re.error:
                 return None, False
     elif type_name == 'list':
         if isinstance(value, (list, tuple)):
@@ -275,15 +280,15 @@
     raise exceptions.DSLParsingLogicException(
         exceptions.ERROR_VALUE_DOES_NOT_MATCH_TYPE, err_msg)
 
 
 def cast_to_type(value, type_name):
     """Try converting value to the specified type_name if possible."""
 
-    if not isinstance(value, text_type):
+    if not isinstance(value, str):
         return value
 
     try:
         if type_name == 'integer':
             return int(value)
         if type_name == 'float':
             return float(value)
@@ -304,19 +309,19 @@
     except yaml.parser.ParserError as ex:
         raise exceptions.DSLParsingFormatException(-1,
                                                    '{0}: Illegal yaml; {1}'
                                                    .format(error_message, ex))
 
 
 def url_exists(url):
-    request = Request(url)
     try:
+        request = Request(url)
         with contextlib.closing(urlopen(request)):
             return True
-    except URLError:
+    except (ValueError, URLError):
         return False
 
 
 def is_valid_url(url):
     # Checks whether a given string represents a valid
     # URL (syntax-wise).
     return urlparse(url).scheme != ''
@@ -354,29 +359,26 @@
     if not properties:
         properties = {}
     try:
         cls = get_class(class_path)
         instance = cls(**properties)
     except Exception as e:
         exc_type, exc, traceback = sys.exc_info()
-        reraise(
-            RuntimeError,
-            RuntimeError('Failed to instantiate {0}, error: {1}'
-                         .format(class_path, e)),
-            traceback)
+        raise RuntimeError(f'Failed to instantiate {class_path}, error: {e}')\
+            .with_traceback(traceback)
 
     return instance
 
 
 def get_class(class_path):
     """Returns a class from a string formatted as module:class"""
     if not class_path:
         raise ValueError('class path is missing or empty')
 
-    if not isinstance(class_path, text_type):
+    if not isinstance(class_path, str):
         raise ValueError('class path is not a string')
 
     class_path = class_path.strip()
     if ':' not in class_path or class_path.count(':') > 1:
         raise ValueError('Invalid class path, expected format: '
                          'module:class')
 
@@ -463,7 +465,59 @@
         if k == 'type':
             continue
         elif k in TEMPLATE_FUNCTIONS:
             result = (TEMPLATE_FUNCTIONS[k], v)
         else:
             return None
     return result
+
+
+def topological_sort(G, nbunch=None, reverse=False):
+    """Return a list of nodes in topological sort order (networkx==1.x algo)
+
+    This is a copy of topological_sort function from networkx 1.11.  The new
+    implementation (networkx==2.x.y) is not backward compatible:
+      - it does not support nbunch parameter (esp. not in case len(nbunch) > 1)
+      - the results are slightly different and not always deterministic, hence
+        taking the first of the sorted elements does not behave as we would
+        expect it to
+
+    https://github.com/networkx/networkx/blob/cabefb75b1e116fc57d5b30e5d93b217d68b3a2e/networkx/algorithms/dag.py#L88-L168
+    """
+    if not G.is_directed():
+        raise NetworkXError(
+            "Topological sort not defined on undirected graphs.")
+
+    # nonrecursive version
+    seen = set()
+    order = []
+    explored = set()
+
+    if nbunch is None:
+        nbunch = G.nodes
+    for v in nbunch:     # process all vertices in G
+        if v in explored:
+            continue
+        fringe = [v]   # nodes yet to look at
+        while fringe:
+            w = fringe[-1]  # depth first search
+            if w in explored:  # already looked down this branch
+                fringe.pop()
+                continue
+            seen.add(w)     # mark as seen
+            # Check successors for cycles and for new nodes
+            new_nodes = []
+            for n in G[w]:
+                if n not in explored:
+                    if n in seen:  # CYCLE !!
+                        raise NetworkXUnfeasible("Graph contains a cycle.")
+                    new_nodes.append(n)
+            if new_nodes:   # Add new_nodes to fringe
+                fringe.extend(new_nodes)
+            else:           # No new nodes so w is fully explored
+                explored.add(w)
+                order.append(w)
+                fringe.pop()    # done considering this node
+    if reverse:
+        return order
+    else:
+        return list(reversed(order))
```

### Comparing `cloudify-common-6.4.2/dsl_parser/version.py` & `cloudify-common-7.0.0/dsl_parser/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import collections
 
-from dsl_parser._compat import text_type
 from dsl_parser.exceptions import DSLParsingLogicException
 
 VERSION = 'tosca_definitions_version'
 DSL_VERSION_PREFIX = 'cloudify_dsl_'
 DSL_VERSION_1_0 = DSL_VERSION_PREFIX + '1_0'
 DSL_VERSION_1_1 = DSL_VERSION_PREFIX + '1_1'
 DSL_VERSION_1_2 = DSL_VERSION_PREFIX + '1_2'
 DSL_VERSION_1_3 = DSL_VERSION_PREFIX + '1_3'
 DSL_VERSION_1_4 = DSL_VERSION_PREFIX + '1_4'
+DSL_VERSION_1_5 = DSL_VERSION_PREFIX + '1_5'
 SUPPORTED_VERSIONS = [
     DSL_VERSION_1_0,
     DSL_VERSION_1_1,
     DSL_VERSION_1_2,
     DSL_VERSION_1_3,
-    DSL_VERSION_1_4
+    DSL_VERSION_1_4,
+    DSL_VERSION_1_5,
 ]
 
 
 def validate_dsl_version(dsl_version):
     if dsl_version not in SUPPORTED_VERSIONS:
         raise DSLParsingLogicException(
             29, 'Unexpected tosca_definitions_version {0}; Currently '
@@ -29,15 +30,15 @@
 
 def parse_dsl_version(dsl_version):
 
     if not dsl_version:
         raise DSLParsingLogicException(71, '{0} is missing or empty'
                                        .format(VERSION))
 
-    if not isinstance(dsl_version, text_type):
+    if not isinstance(dsl_version, str):
         raise DSLParsingLogicException(72, 'Invalid {0}: {1} is not a string'
                                        .format(VERSION, dsl_version))
 
     # handle the 'dsl_version_' prefix
     if dsl_version.startswith(DSL_VERSION_PREFIX):
         short_dsl_version = dsl_version[len(DSL_VERSION_PREFIX):]
     else:
```

### Comparing `cloudify-common-6.4.2/dsl_parser/yaml_loader.py` & `cloudify-common-7.0.0/dsl_parser/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/script_runner/eval_env.py` & `cloudify-common-7.0.0/script_runner/eval_env.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-6.4.2/script_runner/tasks.py` & `cloudify-common-7.0.0/script_runner/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
+import ast
 import codecs
 import os
 import re
 import shutil
 import sys
 import time
 import json
 import tempfile
+import textwrap
 import subprocess
 from contextlib import contextmanager
 
 import requests
 
 from cloudify import ctx as operation_ctx
 from cloudify.utils import (create_temp_folder,
@@ -55,37 +57,72 @@
 POLL_LOOP_INTERVAL = 0.1
 POLL_LOOP_LOG_ITERATIONS = 200
 
 DEFAULT_TASK_LOG_DIR = os.path.join(tempfile.gettempdir(), 'cloudify')
 
 
 @operation
-def run(script_path, process=None, ssl_cert_content=None, **kwargs):
+def run(
+    script_path=None,
+    script_source=None,
+    process=None,
+    ssl_cert_content=None,
+    **kwargs,
+):
     ctx = operation_ctx._get_current_object()
-    if script_path is None:
-        raise NonRecoverableError('Script path parameter not defined')
+    if script_path is None and script_source is None:
+        raise NonRecoverableError(
+            'Either script_path or script_source must be provided')
+    if script_source and script_path:
+        raise NonRecoverableError(
+            'Only provide script_path or script_source, not both')
     process = create_process_config(process or {}, kwargs)
-    script_path = download_resource(ctx.download_resource, script_path,
-                                    ssl_cert_content)
+    if script_source:
+        script_path = _script_source_to_file(script_source, process)
+    else:
+        script_path = download_resource(
+            ctx.download_resource,
+            script_path,
+            ssl_cert_content
+        )
     os.chmod(script_path, 0o755)
     script_func = get_run_script_func(script_path, process)
     try:
         script_result = process_execution(script_func, script_path, ctx,
                                           process)
     finally:
         os.remove(script_path)
     return script_result
 
 
 @workflow
-def execute_workflow(script_path, ssl_cert_content=None, **kwargs):
+def execute_workflow(
+    script_path=None,
+    script_source=None,
+    ssl_cert_content=None,
+    **kwargs,
+):
+    if script_path is None and script_source is None:
+        raise NonRecoverableError(
+            'Either script_path or script_source must be provided')
+    if script_source and script_path:
+        raise NonRecoverableError(
+            'Only provide script_path or script_source, not both')
     ctx = workflows_ctx._get_current_object()
-    script_path = download_resource(
-        ctx.internal.handler.download_deployment_resource, script_path,
-        ssl_cert_content)
+    if script_source:
+        script_path = _script_source_to_file(
+            script_source,
+            {'eval_python': True},
+        )
+    else:
+        script_path = download_resource(
+            ctx.internal.handler.download_deployment_resource,
+            script_path,
+            ssl_cert_content,
+        )
     try:
         script_result = process_execution(eval_script, script_path, ctx)
     finally:
         os.remove(script_path)
     return script_result
 
 
@@ -157,14 +194,47 @@
             return script_result
         else:
             raise NonRecoverableError(str(script_result))
     else:
         return script_result
 
 
+def _script_source_to_file(script_source, process):
+    """Write script_source to a file, with an auto-detected file extension.
+
+    If the script is valid python syntax, we'll consider it a python
+    script, otherwise it's a shell script.
+
+    eval_python still overrides this auto-detection.
+
+    Return a filename in the tempdir.
+    """
+    is_python = False
+    script_source = textwrap.dedent(script_source)
+    if process.get('eval_python'):
+        is_python = True
+    else:
+        try:
+            ast.parse(script_source)
+        except SyntaxError:
+            pass
+        else:
+            is_python = True
+
+    if is_python:
+        filename = 'script.py'
+    else:
+        filename = 'script.sh'
+
+    script_path = os.path.join(create_temp_folder(), filename)
+    with open(script_path, 'w') as f:
+        f.write(script_source)
+    return script_path
+
+
 def treat_script_as_python_script(script_path, process):
     eval_python = process.get('eval_python')
     script_extension = os.path.splitext(script_path)[1].lower()
     return eval_python is True or \
         (script_extension == constants.PYTHON_SCRIPT_FILE_EXTENSION and
          eval_python is not False)
 
@@ -352,16 +422,19 @@
             env['PATH'] = os.pathsep.join([env_path, bin_dir])
     else:
         env['PATH'] = bin_dir
 
     return env
 
 
-def download_resource(download_resource_func, script_path,
-                      ssl_cert_content=None):
+def download_resource(
+    download_resource_func,
+    script_path,
+    ssl_cert_content=None,
+):
     split = script_path.split('://')
     schema = split[0]
     target_path = _get_target_path(script_path)
     if schema in ['http', 'https']:
         with _prepare_ssl_cert(ssl_cert_content) as cert_file:
             response = requests.get(script_path, verify=cert_file)
         # We only accept HTTP 200. Any other code (including other 2xx codes)
```

