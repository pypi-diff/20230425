# Comparing `tmp/cloudify-6.4.2.tar.gz` & `tmp/cloudify-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-6.4.2.tar", last modified: Thu Feb  2 10:47:45 2023, max compression
+gzip compressed data, was "cloudify-7.0.0.tar", last modified: Tue Apr 25 11:56:05 2023, max compression
```

## Comparing `cloudify-6.4.2.tar` & `cloudify-7.0.0.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.855991 cloudify-6.4.2/
--rw-r--r--   0 root         (0) root         (0)    11325 2023-02-02 10:47:27.000000 cloudify-6.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-02-02 10:47:45.855991 cloudify-6.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      591 2023-02-02 10:47:27.000000 cloudify-6.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.843991 cloudify-6.4.2/cloudify.egg-info/
--rw-r--r--   0 root         (0) root         (0)      189 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2186 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      301 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-02 10:47:45.000000 cloudify-6.4.2/cloudify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.847991 cloudify-6.4.2/cloudify_cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.847991 cloudify-6.4.2/cloudify_cli/async_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/async_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/async_commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     6764 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/blueprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.847991 cloudify-6.4.2/cloudify_cli/cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74539 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/cli/cfy.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/cli/completion_utils.py
--rw-r--r--   0 root         (0) root         (0)    30874 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/cli/helptexts.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/colorful_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.851991 cloudify-6.4.2/cloudify_cli/commands/
--rw-r--r--   0 root         (0) root         (0)      641 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16028 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/agents.py
--rw-r--r--   0 root         (0) root         (0)    10374 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/apply.py
--rw-r--r--   0 root         (0) root         (0)     4715 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    31496 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/blueprints.py
--rw-r--r--   0 root         (0) root         (0)    14297 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/certificates.py
--rw-r--r--   0 root         (0) root         (0)    16683 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/cluster.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)    70701 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/deployments.py
--rw-r--r--   0 root         (0) root         (0)    12266 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/events.py
--rw-r--r--   0 root         (0) root         (0)    32283 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/executions.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/groups.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/idp.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/init.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/ldap.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/license.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     6804 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/logs.py
--rw-r--r--   0 root         (0) root         (0)     5465 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/maintenance_mode.py
--rw-r--r--   0 root         (0) root         (0)    10293 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/node_instances.py
--rw-r--r--   0 root         (0) root         (0)     8555 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/nodes.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/permissions.py
--rw-r--r--   0 root         (0) root         (0)    41038 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/plugins.py
--rw-r--r--   0 root         (0) root         (0)    27830 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/profiles.py
--rw-r--r--   0 root         (0) root         (0)    13858 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/secrets.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/sites.py
--rw-r--r--   0 root         (0) root         (0)     9945 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/ssh.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/status.py
--rw-r--r--   0 root         (0) root         (0)     2264 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/summary.py
--rw-r--r--   0 root         (0) root         (0)    10822 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/tenants.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/tokens.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/uninstall.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     9355 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/users.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/commands/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 10:47:45.851991 cloudify-6.4.2/cloudify_cli/config/
--rw-r--r--   0 root         (0) root         (0)      641 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/config/config.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/constants.py
--rw-r--r--   0 root         (0) root         (0)    24371 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/env.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/execution_events_fetcher.py
--rw-r--r--   0 root         (0) root         (0)    13747 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/filters_utils.py
--rw-r--r--   0 root         (0) root         (0)     6052 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5989 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/labels_utils.py
--rw-r--r--   0 root         (0) root         (0)     8492 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/local.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/logger.py
--rw-r--r--   0 root         (0) root         (0)    13362 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/main.py
--rw-r--r--   0 root         (0) root         (0)    54445 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/prettytable.py
--rw-r--r--   0 root         (0) root         (0)    10905 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/replace_certificates_config.py
--rw-r--r--   0 root         (0) root         (0)     6743 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/table.py
--rw-r--r--   0 root         (0) root         (0)    16284 2023-02-02 10:47:27.000000 cloudify-6.4.2/cloudify_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-02 10:47:45.855991 cloudify-6.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2100 2023-02-02 10:47:27.000000 cloudify-6.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11325 2023-04-25 11:55:41.000000 cloudify-7.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-25 11:56:05.291888 cloudify-7.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2023-04-25 11:55:41.000000 cloudify-7.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.279890 cloudify-7.0.0/cloudify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/async_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/async_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/async_commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     6759 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/blueprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78764 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/cfy.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/completion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    31831 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/helptexts.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/colorful_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/cloudify_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/agents.py
+-rw-r--r--   0 root         (0) root         (0)    10374 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/apply.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)    14297 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/certificates.py
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/community.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    71965 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/deployments.py
+-rw-r--r--   0 root         (0) root         (0)    12209 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/events.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/executions.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/groups.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/idp.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/init.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/license.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     5465 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/maintenance_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    41310 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    27830 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    21581 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/sites.py
+-rw-r--r--   0 root         (0) root         (0)    10099 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/status.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10822 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/uninstall.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     9355 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/users.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/cloudify_cli/config/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/constants.py
+-rw-r--r--   0 root         (0) root         (0)    22806 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/env.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/execution_events_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)    13653 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/filters_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6006 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/labels_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8492 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/local.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/logger.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/main.py
+-rw-r--r--   0 root         (0) root         (0)    54445 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/prettytable.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/replace_certificates_config.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/table.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:56:05.291888 cloudify-7.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-04-25 11:55:41.000000 cloudify-7.0.0/setup.py
```

### Comparing `cloudify-6.4.2/LICENSE` & `cloudify-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/README.md` & `cloudify-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify.egg-info/SOURCES.txt` & `cloudify-7.0.0/cloudify.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,36 +33,35 @@
 cloudify_cli/commands/__init__.py
 cloudify_cli/commands/agents.py
 cloudify_cli/commands/apply.py
 cloudify_cli/commands/audit_log.py
 cloudify_cli/commands/blueprints.py
 cloudify_cli/commands/certificates.py
 cloudify_cli/commands/cluster.py
+cloudify_cli/commands/community.py
 cloudify_cli/commands/config.py
 cloudify_cli/commands/deployments.py
 cloudify_cli/commands/events.py
 cloudify_cli/commands/executions.py
 cloudify_cli/commands/groups.py
 cloudify_cli/commands/idp.py
 cloudify_cli/commands/init.py
 cloudify_cli/commands/install.py
 cloudify_cli/commands/ldap.py
 cloudify_cli/commands/license.py
 cloudify_cli/commands/log_bundles.py
-cloudify_cli/commands/logs.py
 cloudify_cli/commands/maintenance_mode.py
 cloudify_cli/commands/node_instances.py
 cloudify_cli/commands/nodes.py
 cloudify_cli/commands/permissions.py
 cloudify_cli/commands/plugins.py
 cloudify_cli/commands/profiles.py
 cloudify_cli/commands/secrets.py
 cloudify_cli/commands/sites.py
 cloudify_cli/commands/snapshots.py
-cloudify_cli/commands/ssh.py
 cloudify_cli/commands/status.py
 cloudify_cli/commands/summary.py
 cloudify_cli/commands/tenants.py
 cloudify_cli/commands/tokens.py
 cloudify_cli/commands/uninstall.py
 cloudify_cli/commands/user_groups.py
 cloudify_cli/commands/users.py
```

### Comparing `cloudify-6.4.2/cloudify_cli/__init__.py` & `cloudify-7.0.0/cloudify_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/async_commands/audit_log.py` & `cloudify-7.0.0/cloudify_cli/async_commands/audit_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import json
 
+import aiohttp.client_exceptions
+
 from cloudify_cli.exceptions import CloudifyCliError
 from cloudify_cli.logger import get_global_json_output
 
 
 def stream_logs(creator_name,
                 execution_id,
                 since,
@@ -30,20 +32,23 @@
     if not hasattr(client.auditlog, 'stream'):
         raise CloudifyCliError('Streaming requires Python>=3.6.')
     logger.info('Streaming audit log entries...')
     response = await client.auditlog.stream(timeout=timeout,
                                             creator_name=creator_name,
                                             execution_id=execution_id,
                                             since=since)
-    async for data in response.content:
-        for audit_log in _streamed_audit_log(data):
-            if get_global_json_output():
-                print(audit_log)
-            else:
-                print(_format_audit_log(audit_log))
+    try:
+        async for data in response.content:
+            for audit_log in _streamed_audit_log(data):
+                if get_global_json_output():
+                    print(audit_log)
+                else:
+                    print(_format_audit_log(audit_log))
+    except aiohttp.client_exceptions.ClientError as e:
+        raise CloudifyCliError(f'Error getting audit log stream: {e}') from e
 
 
 def _streamed_audit_log(data):
     line = data.strip().decode(errors='ignore')
     if line:
         yield json.loads(line)
```

### Comparing `cloudify-6.4.2/cloudify_cli/blueprint.py` & `cloudify-7.0.0/cloudify_cli/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ############
 
 import os
 import tempfile
 from shutil import copy, copytree
-
-from cloudify._compat import urlparse
+from urllib.parse import urlparse
 
 from cloudify_cli import utils
 from cloudify_cli.exceptions import CloudifyCliError
 from cloudify_cli.constants import DEFAULT_BLUEPRINT_PATH
 
 
 ICON_FILENAME = 'icon.png'
```

### Comparing `cloudify-6.4.2/cloudify_cli/cli/__init__.py` & `cloudify-7.0.0/cloudify_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/cli/cfy.py` & `cloudify-7.0.0/cloudify_cli/cli/cfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import traceback
 import pkg_resources
 import datetime
 import re
 import subprocess
 import locale
 import codecs
-from functools import wraps
 import unicodedata
+from functools import wraps
+from io import StringIO
+from urllib.parse import quote as urlquote
 
 import click
 
-from cloudify._compat import StringIO, urlquote
+from cloudify.models_states import AgentState
 from cloudify_rest_client.constants import VisibilityState
 from cloudify_rest_client.exceptions import NotModifiedError
 from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.exceptions import MaintenanceModeActiveError
 from cloudify_rest_client.exceptions import MaintenanceModeActivatingError
 
 from cloudify_cli import env, logger
@@ -41,15 +43,15 @@
     set_global_json_output,
     set_global_extended_view)
 from cloudify_cli.utils import generate_random_string
 
 
 CLICK_CONTEXT_SETTINGS = dict(
     help_option_names=['-h', '--help'],
-    token_normalize_func=lambda param: param.lower())
+)
 
 AGENT_FILTER_NODE_IDS = 'node_ids'
 AGENT_FILTER_NODE_INSTANCE_IDS = 'node_instance_ids'
 AGENT_FILTER_DEPLOYMENT_ID = 'deployment_id'
 AGENT_FILTER_INSTALL_METHODS = 'install_methods'
 
 
@@ -442,15 +444,15 @@
         logger.info('Possible solutions:')
         for solution in possible_solutions:
             logger.info('  - {0}'.format(solution))
 
     def new_excepthook(tpe, value, tb):
         with open(DEFAULT_LOG_FILE, 'a') as log_file:
             traceback.print_exception(
-                etype=tpe,
+                tpe,
                 value=value,
                 tb=tb,
                 file=log_file)
 
         logger = get_logger()
 
         prefix = None
@@ -471,15 +473,15 @@
             output_message = False
         if issubclass(tpe, CloudifyBootstrapError):
             output_message = False
         if global_verbosity_level:
             # print traceback if verbose
             s_traceback = StringIO()
             traceback.print_exception(
-                etype=tpe,
+                tpe,
                 value=value,
                 tb=tb,
                 file=s_traceback)
             logger.error(s_traceback.getvalue())
             if server_traceback:
                 logger.error('Server Traceback (most recent call last):')
 
@@ -1278,14 +1280,41 @@
 
         self.secret_string = click.option(
             '-s',
             '--secret-string',
             required=False,
             help=helptexts.SECRET_STRING)
 
+        self.secret_schema = click.option(
+            '--schema',
+            'secret_schema',
+            required=False,
+            default=None,
+            cls=MutuallyExclusiveOption,
+            mutually_exclusive=['dict', 'list'],
+            help=helptexts.SECRET_SCHEMA)
+
+        self.secret_flag_dict = click.option(
+            '--dict',
+            'secret_flag_dict',
+            is_flag=True,
+            default=False,
+            cls=MutuallyExclusiveOption,
+            mutually_exclusive=['schema', 'list'],
+            help=helptexts.SECRET_FLAG_DICT)
+
+        self.secret_flag_list = click.option(
+            '--list',
+            'secret_flag_list',
+            is_flag=True,
+            default=False,
+            cls=MutuallyExclusiveOption,
+            mutually_exclusive=['schema', 'dict'],
+            help=helptexts.SECRET_FLAG_LIST)
+
         self.secret_update_if_exists = click.option(
             '-u',
             '--update-if-exists',
             is_flag=True,
             cls=MutuallyExclusiveOption,
             mutually_exclusive=['hidden_value', 'visibility'],
             help=helptexts.SECRET_UPDATE_IF_EXISTS,
@@ -1398,14 +1427,21 @@
         )
 
         self.tempdir_path = click.option(
             '--tempdir-path',
             help=helptexts.TEMPDIR_PATH
         )
 
+        self.legacy = click.option(
+            '--legacy/--no-legacy',
+            is_flag=True,
+            default=True,
+            help=helptexts.LEGACY_SNAPSHOT
+        )
+
         self.wait_for_status = click.option(
             '-w',
             '--wait-for-status',
             is_flag=True,
             default=False,
             help=helptexts.WAIT_FOR_STATUS
         )
@@ -1858,14 +1894,39 @@
             is_flag=True,
             help=helptexts.DRIFT_ONLY,
             default=False,
             cls=MutuallyExclusiveOption,
             mutually_exclusive=['blueprint_id', 'blueprint_path', 'inputs'],
         )
 
+        self.secrets_provider_name = click.option(
+            '--name',
+            'secrets_provider_name',
+            required=True,
+            callback=validate_value_not_empty,
+            help=helptexts.SECRETS_PROVIDER_NAME,
+        )
+
+        self.provider_name = click.option(
+            '-p',
+            '--provider',
+            'provider_name',
+            required=False,
+            callback=validate_value_not_empty,
+            help=helptexts.SECRETS_PROVIDER_NAME,
+        )
+
+        self.evaluate_functions = click.option(
+            '--evaluate-functions',
+            is_flag=True,
+            default=False,
+            required=False,
+            help=helptexts.EVALUATE_FUNCTIONS,
+        )
+
     def common_options(self, f):
         """A shorthand for applying commonly used arguments.
 
         To be used for arguments that are going to be applied for all or
         almost all commands.
         """
         for arg in [self.manager, self.json, self.format,
@@ -1893,26 +1954,44 @@
         return sum((part.split(',') for part in value), [])
 
     def agent_filters(self, f):
         """Set of filter arguments for commands working with a list of agents
 
         Applies deployment id, node id and node instance id filters.
         """
-        node_instance_id = click.option('--node-instance-id', multiple=True,
-                                        help=helptexts.AGENT_NODE_INSTANCE_ID,
-                                        callback=self.parse_comma_separated)
-        node_id = click.option('--node-id', multiple=True,
-                               help=helptexts.AGENT_NODE_ID,
-                               callback=self.parse_comma_separated)
-        install_method = click.option('--install-method', multiple=True,
-                                      help=helptexts.AGENT_INSTALL_METHOD,
-                                      callback=self.parse_comma_separated)
-        deployment_id = click.option('--deployment-id', multiple=True,
-                                     help=helptexts.AGENT_DEPLOYMENT_ID,
-                                     callback=self.parse_comma_separated)
+        node_instance_id = click.option(
+            '--node-instance-id',
+            multiple=True,
+            help=helptexts.AGENT_NODE_INSTANCE_ID,
+            callback=self.parse_comma_separated,
+        )
+        node_id = click.option(
+            '--node-id',
+            multiple=True,
+            help=helptexts.AGENT_NODE_ID,
+            callback=self.parse_comma_separated,
+        )
+        install_method = click.option(
+            '--install-method',
+            multiple=True,
+            help=helptexts.AGENT_INSTALL_METHOD,
+            callback=self.parse_comma_separated,
+        )
+        deployment_id = click.option(
+            '--deployment-id',
+            multiple=True,
+            help=helptexts.AGENT_DEPLOYMENT_ID,
+            callback=self.parse_comma_separated,
+        )
+        all_states = click.option(
+            '--all-states',
+            default=False,
+            is_flag=True,
+            help=helptexts.AGENT_ALL_STATES,
+        )
 
         # we add separate --node-instance-id, --node-id and --deployment-id
         # arguments, but only expose a agents_filter = {'node_id': ..} dict
         # to the decorated function
         def _filters_deco(f):
             @wraps(f)
             def _inner(*args, **kwargs):
@@ -1920,20 +1999,22 @@
                 for arg_name, filter_name in [
                         ('node_id', AGENT_FILTER_NODE_IDS),
                         ('node_instance_id', AGENT_FILTER_NODE_INSTANCE_IDS),
                         ('deployment_id', AGENT_FILTER_DEPLOYMENT_ID),
                         ('install_method', AGENT_FILTER_INSTALL_METHODS)]:
                     filters[filter_name] = kwargs.pop(arg_name, None)
 
+                if not kwargs.pop('all_states', False):
+                    filters['state'] = [AgentState.STARTED]
                 kwargs['agent_filters'] = filters
                 return f(*args, **kwargs)
             return _inner
 
         for arg in [install_method, node_instance_id, node_id,
-                    deployment_id, _filters_deco]:
+                    deployment_id, all_states, _filters_deco]:
             f = arg(f)
         return f
 
     @staticmethod
     def secret_file():
         return click.option(
             '-f',
@@ -2111,20 +2192,24 @@
             '-e',
             '--execution-id',
             dest,
             required=required,
             help=helptexts.EXECUTION_ID)
 
     @staticmethod
-    def blueprint_id(required=False, validate=False):
+    def blueprint_id(
+        required=False,
+        validate=False,
+        help=helptexts.BLUEPRINT_ID,
+    ):
         return click.option(
             '-b',
             '--blueprint-id',
             required=required,
-            help=helptexts.BLUEPRINT_ID,
+            help=help,
             callback=_get_validate_callback(validate))
 
     @staticmethod
     def blueprint_path(required=False,
                        extra_message='',
                        exists=True):
         return click.option(
@@ -2421,14 +2506,96 @@
 
     def blueprint_filter_rules(self, f):
         return self._filter_rules(f, 'blueprint')
 
     def deployment_filter_rules(self, f):
         return self._filter_rules(f, 'deployment')
 
+    @staticmethod
+    def secrets_provider_type(
+            required=True,
+            _help=None,
+            default=None,
+            callback=validate_value_not_empty,
+    ):
+        args = [
+            '-y',
+            '--type',
+            'secrets_provider_type',
+        ]
+        kwargs = {
+            'required': required,
+            'help': _help or helptexts.SECRETS_PROVIDER_TYPE,
+            'callback': callback,
+        }
+
+        if default is not None:
+            kwargs['default'] = default
+
+        return click.option(*args, **kwargs)
+
+    @staticmethod
+    def secrets_provider_skip_check():
+        return click.option(
+            '-s',
+            '--skip-check',
+            is_flag=True,
+            default=False,
+            required=False,
+            help=helptexts.SECRETS_PROVIDER_SKIP_CHECK,
+        )
+
+    @staticmethod
+    def connection_parameters(required=True, _help=None, default=None):
+        args = [
+            '-c',
+            '--connection-parameters',
+        ]
+        kwargs = {
+            'required': required,
+            'help': _help or helptexts.SECRETS_PROVIDER_CONNECTION_PARAMETERS,
+            'callback': inputs_callback,
+            'multiple': True,
+            'default': default,
+        }
+
+        return click.option(*args, **kwargs)
+
+    @staticmethod
+    def provider_options(required=True, _help=None, default=None):
+        args = [
+            '-o',
+            '--provider-options',
+        ]
+        kwargs = {
+            'required': required,
+            'help': _help or helptexts.SECRETS_PROVIDER_OPTIONS,
+            'callback': inputs_callback,
+            'multiple': True,
+            'default': default,
+        }
+
+        return click.option(*args, **kwargs)
+
+    @staticmethod
+    def provider_multiple(required=False, _help=None, default=None):
+        args = [
+            '-p',
+            '--provider',
+            'provider',
+        ]
+        kwargs = {
+            'required': required,
+            'help': _help or helptexts.SECRETS_PROVIDER_NAME_MULTIPLE,
+            'multiple': True,
+            'default': default,
+        }
+
+        return click.option(*args, **kwargs)
+
 
 options = Options()
 
 
 class SummaryArgs(click.Choice):
     """
     Used for correctly displaying usage of summary commands (e.g. `cfy
```

### Comparing `cloudify-6.4.2/cloudify_cli/cli/completion_utils.py` & `cloudify-7.0.0/cloudify_cli/cli/completion_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/cli/helptexts.py` & `cloudify-7.0.0/cloudify_cli/cli/helptexts.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,14 +331,18 @@
 GET_DATA = 'When set to True, displays the full list of connected resources ' \
            '(users/tenants/user-groups), for each listed resource. When set ' \
            'to False displays the total number of connected resources. ' \
            '(default:False)'
 PROFILE_NAME = 'Name of the profile to use'
 SECRET_VALUE = "The secret's value to be set"
 SECRET_STRING = "The string to use as the secret's value"
+SECRET_FLAG_DICT = "Whether the secret is to be treated as a dict"
+SECRET_FLAG_LIST = "Whether the secret is to be treated as a lists"
+SECRET_SCHEMA = "A JSON schema against which the secret will be validated [" \
+                "default: '{\"type\": \"string\"}']"
 SECRET_FILE = "The file with the contents of the secret"
 SECRET_UPDATE_IF_EXISTS = 'Update secret value if secret key already ' \
                           'exists. [This option is deprecated; use cfy ' \
                           'secrets update command instead]'
 HIDDEN_VALUE = 'The secret value is only shown to the user that created the ' \
                'secret and to admins. Use of the secret is allowed ' \
                'according to user roles and the visibility of the secret'
@@ -425,14 +429,15 @@
 AGENT_NODE_INSTANCE_ID = 'The node instance id to be used for filtering ' \
                          + _MULTIPLE_TIMES_FRAGMENT
 AGENT_NODE_ID = 'The node id to be used for filtering' \
                 + _MULTIPLE_TIMES_FRAGMENT
 AGENT_INSTALL_METHOD = 'Only show agents installed with this install_method' \
                        + _MULTIPLE_TIMES_FRAGMENT
 AGENT_DEPLOYMENT_ID = DEPLOYMENT_ID + _MULTIPLE_TIMES_FRAGMENT
+AGENT_ALL_STATES = 'Show agents in all states, not only started ones'
 
 AGENTS_WAIT = "Wait for agents operations to end, and show execution logs"
 INSTALL_AGENT_TIMEOUT = "Agent installation timeout"
 WAIT_AFTER_FAIL = 'When a task fails, wait this many seconds for ' \
                   'already-running tasks to return'
 RESET_OPERATIONS = 'Reset operations in started state, so that they are '\
                    'run again unconditionally'
@@ -591,18 +596,30 @@
 SET_USERNAME = 'The name of the user who will be the new owner '\
                'of the resource.'
 WORKER_NAMES = 'Show the worker name for each event'
 DRIFT_ONLY = 'Run update without changing anything. This will still check ' \
              'drift and run update operations as necessary'
 TEMPDIR_PATH = "Temporary location to be used for snapshot creation. If not " \
                "specified, /tmp will be used."
+LEGACY_SNAPSHOT = "Create legacy version of the snapshot (as opposed to 'new')"
 WAIT_FOR_STATUS = "Whether to wait for snapshot status [default: False]."
 SUMMARY_HELP = """
     Retrieve summary of {type}, e.g. a count of each {example}.
 
     `TARGET_FIELD` is the field to summarize {type} on. `SUB_FIELD` is an
     optional second field to summarize {type} on. Both can be chosen from
     [{fields}].
 
     E.g. `cfy {type} summary tenant_name visibility` will summarize
     {type} by tenant_name with a secondary grouping by visibility.
     """
+SECRETS_PROVIDER_NAME = "Secrets Provider's name"
+SECRETS_PROVIDER_NAME_MULTIPLE = "Secrets Provider's name list"
+SECRETS_PROVIDER_SKIP_CHECK = "Do not check connectivity to secrets provider."
+SECRETS_PROVIDER_TYPE = "Secrets Provider's type"
+SECRETS_PROVIDER_CONNECTION_PARAMETERS = """
+    Secrets Provider's connection parameters in stringify JSON format
+    """
+SECRETS_PROVIDER_OPTIONS = """
+    Secrets Provider's options in stringify JSON format
+    """
+EVALUATE_FUNCTIONS = "Evaluate functions in returned nodes and node instances"
```

### Comparing `cloudify-6.4.2/cloudify_cli/colorful_event.py` & `cloudify-7.0.0/cloudify_cli/colorful_event.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/__init__.py` & `cloudify-7.0.0/cloudify_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/agents.py` & `cloudify-7.0.0/cloudify_cli/commands/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from cloudify_cli.execution_events_fetcher import (
     wait_for_execution,
     WAIT_FOR_EXECUTION_SLEEP_INTERVAL)
 from cloudify_cli.table import print_data
 
 
 _NODE_INSTANCE_STATE_STARTED = 'started'
-AGENT_COLUMNS = ['id', 'ip', 'deployment', 'node', 'system', 'version',
-                 'install_method', 'tenant_name']
+AGENT_COLUMNS = ['id', 'ip', 'deployment', 'state', 'node', 'system',
+                 'version', 'install_method', 'tenant_name']
 
 MAX_TRACKER_THREADS = 20
 
 
 @cfy.group(name='agents')
 @cfy.options.common_options
 @cfy.assert_manager_active()
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/apply.py` & `cloudify-7.0.0/cloudify_cli/commands/apply.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/audit_log.py` & `cloudify-7.0.0/cloudify_cli/commands/audit_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import re
 from datetime import datetime, timedelta
 
 import click
 
-from cloudify._compat import PY2
-
 from cloudify_cli.cli import cfy, helptexts
 from cloudify_cli.exceptions import CloudifyCliError
+from cloudify_cli.logger import get_global_json_output
 from cloudify_cli.table import print_data
 
-AUDITLOG_COLUMNS = ['ref_table', 'ref_id', 'operation', 'creator_name',
-                    'execution_id', 'created_at']
+REF_OBJECT = 'ref_object'
+LIST_COLUMNS = ['operation', REF_OBJECT, 'creator_name', 'execution_id',
+                'created_at']
+JSON_COLUMNS = ['id', 'ref_table', 'ref_id', 'ref_identifier', 'operation',
+                'creator_name', 'execution_id', 'created_at']
 
 
-def _parse_before(ctx, spec):
+def _parse_before(ctx, _, spec):
     """Parse the --before/--since parameter"""
     if not spec:
         return spec
     if spec == "now":
         return datetime.utcnow()
     r = re.match(r'^([.\d]+)([hdw])$', spec, re.IGNORECASE)
     if r:
@@ -40,15 +42,14 @@
         return spec
 
 
 @cfy.group(name='auditlog')
 @cfy.assert_manager_active()
 def auditlog():
     """Manage the audit log"""
-    pass
 
 
 @auditlog.command(name='list',
                   short_help='List audit log entries')
 @click.option('-c', '--creator-name',
               help=helptexts.AUDIT_CREATOR_NAME)
 @click.option('-e', '--execution-id',
@@ -76,16 +77,14 @@
               descending,
               pagination_offset,
               pagination_size,
               logger,
               client,
               ):
     if follow:
-        if PY2:
-            raise CloudifyCliError('Streaming requires Python>=3.6.')
         from cloudify_cli.async_commands.audit_log import stream_logs
         stream_logs(creator_name,
                     execution_id,
                     since,
                     timeout,
                     logger,
                     client)
@@ -117,19 +116,35 @@
         execution_id=execution_id,
         since=since,
         order_by=sort_by,
         desc=descending,
         offset=pagination_offset,
         size=pagination_size,
     )
-    print_data(AUDITLOG_COLUMNS, logs, 'AuditLogs:')
+    columns = JSON_COLUMNS if get_global_json_output() else LIST_COLUMNS
+    print_data(columns, _update_refs(logs), 'AuditLogs:')
     logger.info('Showing %d of %d audit log entries',
                 len(logs), logs.metadata.pagination.total)
 
 
+def _update_refs(logs_response):
+    for log in logs_response:
+        if ref_identifier := log.get('ref_identifier'):
+            if tenant_name := ref_identifier.get("tenant_name"):
+                prefix = f'{tenant_name}:'
+            else:
+                prefix = ''
+            for col in ['id', 'manager_id', 'username', 'storage_id']:
+                if val := ref_identifier.get(col):
+                    log[REF_OBJECT] = f'{prefix}{log.get("ref_table")}:{val}'
+            if not log.get(REF_OBJECT):
+                log[REF_OBJECT] = f'{log.get("ref_table")}:{log.get("ref_id")}'
+        yield log
+
+
 @auditlog.command(name='truncate',
                   short_help='Truncate audit log')
 @click.option('-b', '--before',
               required=True,
               help=helptexts.AUDIT_TRUNCATE_BEFORE,
               callback=_parse_before)
 @click.option('-c', '--creator-name',
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/blueprints.py` & `cloudify-7.0.0/cloudify_cli/commands/blueprints.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ############
 
 import os
 import json
 import shutil
+from urllib.parse import urlparse
 
 import click
 
 from dsl_parser.parser import parse_from_path
 from dsl_parser.exceptions import DSLParsingException
-from cloudify._compat import urlparse
 from cloudify_rest_client.constants import VISIBILITY_EXCEPT_PRIVATE
 
 from cloudify_cli import (
     blueprint,
     env,
     exceptions,
     filters_utils,
@@ -100,15 +100,16 @@
 
     `BLUEPRINT_PATH` can be either a local blueprint yaml file or
     blueprint archive; a url to a blueprint archive or an
     `organization/blueprint_repo[:tag/branch]` (to be
     retrieved from GitHub).
     Supported archive types are: zip, tar, tar.gz and tar.bz2
     """
-    client.license.check()
+    if client.manager.get_version().get('edition') == 'premium':
+        client.license.check()
     utils.explicit_tenant_name_message(tenant_name, logger)
     processed_blueprint_path = blueprint.get(
         blueprint_path, blueprint_filename, icon_path)
 
     # Take into account that `blueprint.get` might not return a URL
     # instead of a blueprint file (archive files are not locally downloaded)
     parsed_path = urlparse(processed_blueprint_path)
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/certificates.py` & `cloudify-7.0.0/cloudify_cli/commands/certificates.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/cluster.py` & `cloudify-7.0.0/cloudify_cli/commands/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     stored_nodes_names = ({_get_node_host(node) for node in stored_nodes}
                           if stored_nodes else {})
     received_nodes_names = {_get_node_host(node) for node in nodes}
     for node in nodes:
         _update_node(node, nodes_type, logger, stored_nodes_names)
     # filter out removed nodes
     env.profile.cluster[nodes_type] = [
-        node for node in env.profile.cluster[nodes_type]
+        node for node in env.profile.cluster.get(nodes_type, {})
         if _get_node_host(node) in received_nodes_names]
     env.profile.save()
 
 
 def _update_node(node, node_type, logger, stored_nodes_names):
     if _get_node_host(node) not in stored_nodes_names:
         if node_type == CloudifyNodeType.MANAGER:
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/config.py` & `cloudify-7.0.0/cloudify_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/deployments.py` & `cloudify-7.0.0/cloudify_cli/commands/deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # limitations under the License.
 ############
 
 import os
 import uuid
 import json
 from datetime import datetime
+from io import StringIO
 
 import click
 
-from cloudify._compat import StringIO
 from cloudify_rest_client.constants import VISIBILITY_EXCEPT_PRIVATE
 from cloudify_rest_client.exceptions import (
     DeploymentPluginNotFound,
     UnknownDeploymentInputError,
     UnknownDeploymentSecretError,
     MissingRequiredDeploymentInputError,
     UnsupportedDeploymentGetSecretError,
@@ -271,19 +271,22 @@
         logger.info('Showing %d of %d deployments (%d hidden by filter)',
                     len(deployments), total, filtered)
     else:
         logger.info('Showing %d of %d deployments', len(deployments), total)
 
 
 # to have identical behaviour for both list and status-list, apply the same
-# decorators to both. We'll have two "stub" functions repressenting those
+# decorators to both. We'll have two "stub" functions representing those
 # commands, and both delegate to the same base.
 deployments_list_decorators = [
-    cfy.options.blueprint_id(),
-    click.option('--group-id', '-g'),
+    cfy.options.blueprint_id(
+        help='Show deployments created from this blueprint'),
+    click.option(
+        '--group-id', '-g',
+        help='Show deployments belonging to this group'),
     cfy.options.filter_id,
     cfy.options.deployment_filter_rules,
     cfy.options.sort_by(),
     cfy.options.descending,
     cfy.options.tenant_name_for_list(
         required=False, resource_name_for_help='deployment'),
     cfy.options.all_tenants,
@@ -1153,27 +1156,33 @@
 
 
 @groups.command('list', short_help='List all deployment groups')
 @cfy.pass_client()
 @cfy.pass_logger
 @cfy.options.extended_view
 def groups_list(client, logger):
+    """List all deployment groups"""
     groups = [_format_group(g) for g in client.deployment_groups.list()]
     print_data(DEP_GROUP_COLUMNS, groups, 'Deployment groups:')
 
 
 @groups.command('create', short_help='Create a new deployment group')
 @click.argument('deployment-group-name')
 @cfy.options.inputs
 @cfy.options.group_default_blueprint
 @cfy.options.group_description
 @cfy.pass_client()
 @cfy.pass_logger
 def groups_create(deployment_group_name, inputs, default_blueprint,
                   description, client, logger):
+    """Create a deployment group
+
+    The provided inputs will be used as default inputs for new deployments
+    created using `cfy deployments groups extend --count`.
+    """
     client.deployment_groups.put(
         deployment_group_name,
         default_inputs=inputs,
         blueprint_id=default_blueprint,
         description=description
     )
     logger.info('Group %s created', deployment_group_name)
@@ -1184,14 +1193,20 @@
 @cfy.options.delete_deployments
 @cfy.options.with_logs
 @cfy.options.force(help=helptexts.FORCE_DELETE_DEPLOYMENT)
 @cfy.pass_client()
 @cfy.pass_logger
 def groups_delete(deployment_group_name, delete_deployments, force, with_logs,
                   client, logger):
+    """Delete a deployment group
+
+    This deletes a deployment group, which by default only removes the
+    grouping, the deployments in the group are still left intact.
+    To delete all deployments, pass `--delete-deployments`.
+    """
     client.deployment_groups.delete(
         deployment_group_name,
         delete_deployments=delete_deployments,
         force=force,
         with_logs=with_logs,
     )
     logger.info('Group %s deleted', deployment_group_name)
@@ -1202,14 +1217,19 @@
 @cfy.options.inputs
 @cfy.options.group_default_blueprint
 @cfy.options.group_description
 @cfy.pass_client()
 @cfy.pass_logger
 def groups_update(deployment_group_name, inputs, default_blueprint,
                   description, client, logger):
+    """Update a deployment group
+
+    This changes the group's attributes; for updating deployments belonging
+    to this group, see `update-deployments`.
+    """
     client.deployment_groups.put(
         deployment_group_name,
         default_inputs=inputs,
         blueprint_id=default_blueprint,
         description=description
     )
     logger.info('Group %s updated', deployment_group_name)
@@ -1224,14 +1244,19 @@
 @cfy.options.deployment_group_deployments_from_group
 @cfy.options.into_environments_group
 @cfy.pass_client()
 @cfy.pass_logger
 def groups_extend(deployment_group_name, deployment_id, count, filter_id,
                   filter_rules, from_group, environments_group,
                   client, logger):
+    """Add deployments to an existing group
+
+    This adds deployments from a filter, or from another group, or creates
+    new deployments, using this group's default blueprint and inputs.
+    """
     new_deployments = []
     if environments_group:
         for deployment in client.deployments.list(
                 deployment_group_id=environments_group):
             if deployment.is_environment():
                 new_deployments.append({
                     'id': '{uuid}',
@@ -1259,14 +1284,15 @@
 @cfy.options.deployment_group_filter_id
 @cfy.options.deployment_filter_rules
 @cfy.options.deployment_group_deployments_from_group
 @cfy.pass_client()
 @cfy.pass_logger
 def groups_shrink(deployment_group_name, deployment_id, filter_id,
                   filter_rules, from_group, client, logger):
+    """Shrink a group, removing deployments from it"""
     group = client.deployment_groups.remove_deployments(
         deployment_group_name,
         deployment_id,
         filter_id=filter_id,
         filter_rules=filter_rules,
         deployments_from_group=from_group,
     )
@@ -1296,44 +1322,53 @@
 @click.argument('deployment-group-name')
 @cfy.options.tenant_name(required=False, resource_name_for_help='group')
 @cfy.options.common_options
 @cfy.assert_manager_active()
 @cfy.pass_client()
 @cfy.pass_logger
 def list_group_labels(deployment_group_name, logger, client, tenant_name):
+    """List labels of a group"""
     list_labels(deployment_group_name, 'deployment group',
                 client.deployment_groups, logger, tenant_name)
 
 
 @group_labels.command(name='add', short_help="Add labels to a group")
 @cfy.argument('labels-list', callback=cfy.parse_and_validate_labels)
 @click.argument('deployment-group-name')
 @cfy.options.tenant_name(required=False, resource_name_for_help='group')
 @cfy.options.common_options
 @cfy.assert_manager_active()
 @cfy.pass_client()
 @cfy.pass_logger
 def add_group_labels(labels_list, deployment_group_name,
                      logger, client, tenant_name):
-    """LABELS_LIST: <key>:<value>,<key>:<value>"""
+    """Add labels to the deployment group.
+
+    Dpeloyments added to this group will have the group labels added to them.
+    LABELS_LIST: <key>:<value>,<key>:<value>
+    """
     add_labels(deployment_group_name, 'deployment group',
                client.deployment_groups, labels_list, logger, tenant_name)
 
 
 @group_labels.command(name='delete', short_help="Delete labels from a group")
 @cfy.argument('label', callback=cfy.parse_and_validate_label_to_delete)
 @click.argument('deployment-group-name')
 @cfy.options.tenant_name(required=False, resource_name_for_help='group')
 @cfy.options.common_options
 @cfy.assert_manager_active()
 @cfy.pass_client()
 @cfy.pass_logger
 def delete_group_labels(label, deployment_group_name,
                         logger, client, tenant_name):
-    """
+    """Remove a label from the deployment group.
+
+    Deployments added to this group will no longer have the label
+    added to them.
+
     LABEL: Can be either <key>:<value> or <key>. If <key> is provided,
     all labels associated with this key will be deleted from the group.
     """
     delete_labels(deployment_group_name, 'deployment group',
                   client.deployment_groups, label, logger, tenant_name)
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/events.py` & `cloudify-7.0.0/cloudify_cli/commands/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,38 +37,52 @@
 @cfy.assert_manager_active()
 def events():
     """Show events from workflow executions
     """
     pass
 
 
-@events.command(name='list',
-                short_help='List deployments events [manager only]')
+@events.command(
+    name='list',
+    short_help='List deployments events [manager only]',
+)
 @cfy.argument('execution-id', required=False)
 @cfy.options.execution_id(required=False, dest='execution_id_opt')
-@click.option('--execution-group', '-g',
-              help='The execution group ID to list the events for',
-              cls=cfy.MutuallyExclusiveOption,
-              mutually_exclusive=['execution_id_opt'])
+@click.option(
+    '--execution-group', '-g',
+    help='The execution group ID to list the events for',
+    cls=cfy.MutuallyExclusiveOption,
+    mutually_exclusive=['execution_id_opt'],
+)
 @cfy.options.worker_names
 @cfy.options.include_logs
 @cfy.options.json_output
 @cfy.options.tail
 @cfy.options.common_options
 @cfy.options.tenant_name(required=False, resource_name_for_help='execution')
-@cfy.options.from_datetime(required=False,
-                           help="List events that occurred at this timestamp"
-                                " or after")
-@cfy.options.to_datetime(required=False,
-                         mutually_exclusive_with=['tail', 'before'],
-                         help="List events that occurred at this timestamp"
-                              " or before", )
-@cfy.options.before(required=False,
-                    mutually_exclusive_with=['tail', 'to_datetime'],
-                    help="List events that occurred this long ago or earlier")
+@cfy.options.from_datetime(
+    required=False,
+    help="List events that occurred at this timestamp or after"
+)
+@cfy.options.to_datetime(
+    required=False,
+    mutually_exclusive_with=['tail', 'before'],
+    help="List events that occurred at this timestamp or before",
+)
+@cfy.options.before(
+    required=False,
+    mutually_exclusive_with=['tail', 'to_datetime'],
+    help="List events that occurred this long ago or earlier",
+)
+@click.option('--node', help='List events for this node')
+@click.option(
+    '--operation',
+    help='List events for this interface operation '
+         '(eg. cloudify.interfaces.lifecycle.create)',
+)
 @cfy.options.pagination_offset
 @cfy.options.pagination_size
 @cfy.pass_client()
 @cfy.pass_logger
 def list(execution_id,
          execution_id_opt,
          execution_group,
@@ -78,14 +92,16 @@
          tenant_name,
          from_datetime,
          to_datetime,
          before,
          pagination_offset,
          pagination_size,
          with_worker_names,
+         node,
+         operation,
          client,
          logger):
     """Display events for an execution"""
     if execution_id and execution_id_opt:
         raise click.UsageError(
             "Execution ID provided both as a positional "
             "argument ('{}') and as an option ('{}'). "
@@ -109,81 +125,93 @@
         raise click.UsageError('Provide either Execution ID or Execution '
                                'Group ID, not both')
 
     if before:
         to_datetime = before
 
     if execution_id:
-        logger.info('Listing events for execution id {0} [{1}]'.format(
+        logger.info(
+            'Listing events for execution id %s [%s]',
             execution_id,
-            _filter_description(include_logs, from_datetime, to_datetime)))
+            _filter_description(include_logs, from_datetime, to_datetime),
+        )
         execution_selection = {
             'execution_id': execution_id
         }
         wait_for_method = wait_for_execution
         wait_for_record = client.executions.get(execution_id)
     else:
-        logger.info('Listing events for execution group {0} [{1}]'.format(
+        logger.info(
+            'Listing events for execution group %s [%s]',
             execution_group,
-            _filter_description(include_logs, from_datetime, to_datetime)))
+            _filter_description(include_logs, from_datetime, to_datetime),
+        )
         execution_selection = {
             'execution_group_id': execution_group
         }
         wait_for_method = wait_for_execution_group
         wait_for_record = client.execution_groups.get(execution_group)
 
     utils.explicit_tenant_name_message(tenant_name, logger)
     try:
         execution_events = ExecutionEventsFetcher(
             client,
             include_logs=include_logs,
             from_datetime=from_datetime,
             to_datetime=to_datetime,
+            node_id=node,
+            operation=operation,
             **execution_selection
         )
 
         events_logger = get_events_logger(json_output, with_worker_names)
 
         if tail:
-            execution = wait_for_method(client,
-                                        wait_for_record,
-                                        events_handler=events_logger,
-                                        include_logs=include_logs,
-                                        timeout=None,  # don't timeout ever
-                                        from_datetime=from_datetime)
+            execution = wait_for_method(
+                client,
+                wait_for_record,
+                events_handler=events_logger,
+                include_logs=include_logs,
+                timeout=None,  # don't timeout ever
+                from_datetime=from_datetime,
+            )
             if hasattr(execution, 'error') and execution.error:
-                logger.info('Execution of workflow {0} for deployment '
-                            '{1} failed. [error={2}]'.format(
-                                execution.workflow_id,
-                                execution.deployment_id,
-                                execution.error))
+                logger.info(
+                    'Execution of workflow %s for deployment %s failed. '
+                    '[error=%s]',
+                    execution.workflow_id,
+                    execution.deployment_id,
+                    execution.error,
+                )
                 raise SuppressedCloudifyCliError()
             if hasattr(execution, 'workflow_id'):
                 if hasattr(execution, 'deployment_id'):
-                    logger.info('Finished executing workflow {0} on '
-                                'deployment {1}'.format(
-                                    execution.workflow_id,
-                                    execution.deployment_id))
+                    logger.info(
+                        'Finished executing workflow %s on deployment %s',
+                        execution.workflow_id,
+                        execution.deployment_id,
+                    )
                 elif hasattr(execution, 'deployment_group_id'):
-                    logger.info('Finished executing workflow {0} on '
-                                'deployment group {1}'.format(
-                                    execution.workflow_id,
-                                    execution.deployment_group_id))
+                    logger.info(
+                        'Finished executing workflow %s '
+                        'on deployment group %s',
+                        execution.workflow_id,
+                        execution.deployment_group_id,
+                    )
             else:
-                logger.info('Finished executing {0}'.format(
-                    wait_for_record.id))
+                logger.info('Finished executing %s', wait_for_record.id)
 
         else:
             # don't tail, get only the events created until now and return
             current_events, total_events = execution_events. \
                 fetch_and_process_events_batch(events_handler=events_logger,
                                                offset=pagination_offset,
                                                size=pagination_size)
-            logger.info('\nShowing {0} of {1} events'.format(current_events,
-                                                             total_events))
+            logger.info(
+                '\nShowing %s of %s events', current_events, total_events)
             if not json_output:
                 logger.info('Debug messages are only shown when you use very '
                             'verbose mode (-vv)')
     except CloudifyClientError as e:
         if e.status_code != 404:
             raise
         raise CloudifyCliError('Execution {0} not found'.format(execution_id))
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/executions.py` & `cloudify-7.0.0/cloudify_cli/commands/executions.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,15 +516,15 @@
 @cfy.options.common_options
 @cfy.argument('execution-id', required=False)
 @click.option('--graph-id', required=False,
               help='List operations of this graph '
                    '(exclusive with execution-id)')
 @click.option('--show-internal', type=bool, is_flag=True, default=False,
               help='Also list internal operations')
-@click.option('--state', default=False, help='List operations in this state')
+@click.option('--state', required=False, help='List operations in this state')
 @cfy.pass_logger
 @cfy.pass_client()
 def operations_list(execution_id, graph_id, state, show_internal,
                     client, logger):
     """List operations for an execution or a graph"""
     ops = client.operations.list(
         graph_id=graph_id,
@@ -549,14 +549,19 @@
                 short_help='Retrieve execution group information')
 @cfy.argument('execution_group_id')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 @cfy.options.extended_view
 def execution_groups_get(execution_group_id, client, logger):
+    """Display execution group information
+
+    This includes the source deployment group, and the workflow name.
+    """
+
     group = client.execution_groups.get(execution_group_id)
     print_single(
         ['id', 'workflow_id', 'deployment_group_id'],
         group,
         'Execution group {0}:'.format(execution_group_id)
     )
 
@@ -572,14 +577,15 @@
 @groups.command('list',
                 short_help='List all execution groups')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 @cfy.options.extended_view
 def execution_groups_list(client, logger):
+    """List all execution groups"""
     groups = [_format_group(g) for g in client.execution_groups.list()]
     print_data(
         ['id', 'workflow_id', 'deployment_group'],
         groups,
         'Execution groups:'
     )
 
@@ -588,14 +594,15 @@
                 short_help='Details of an execution group [manager only]')
 @cfy.argument('execution_group_id')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 @cfy.options.extended_view
 def execution_groups_details(execution_group_id, client, logger):
+    """Show execution group details"""
     group = client.execution_groups.get(execution_group_id)
     group.update({'#executions': len(group.get('execution_ids'))})
     print_single(['workflow_id', 'deployment_group_id', '#executions',
                   'created_at', 'status'],
                  group,
                  'Execution group {0}:'.format(execution_group_id))
 
@@ -639,14 +646,19 @@
 @cfy.options.force(help=helptexts.FORCE_CONCURRENT_EXECUTION)
 @cfy.options.timeout()
 @cfy.pass_client()
 @cfy.pass_logger
 def execution_groups_start(deployment_group, workflow_id, parameters,
                            json_output, force, timeout, concurrency,
                            with_worker_names, client, logger):
+    """Start an execution group
+
+    This starts an execution on every deployment in the given deployment
+    group.
+    """
     events_logger = get_events_logger(json_output, with_worker_names)
     group = client.execution_groups.start(
         deployment_group_id=deployment_group,
         workflow_id=workflow_id,
         default_parameters=parameters,
         force=force,
         concurrency=concurrency,
@@ -689,14 +701,19 @@
 @cfy.options.tenant_name(
     required=False, resource_name_for_help='execution group')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 def execution_groups_cancel(group_id, force, kill,
                             client, logger, tenant_name):
+    """Cancel an execution group
+
+    This cancels all running executions in the group. Executions that already
+    finished are unaffected.
+    """
     utils.explicit_tenant_name_message(tenant_name, logger)
     if kill:
         message = 'Killing'
     elif force:
         message = 'Force-cancelling'
     else:
         message = 'Cancelling'
@@ -711,14 +728,19 @@
 @cfy.options.tenant_name(
     required=False, resource_name_for_help='execution group')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 def execution_groups_resume(group_id, reset_operations,
                             client, logger, tenant_name):
+    """Resume an execution group
+
+    This resumes all failed executions in the group. Executions that already
+    finished are unaffected.
+    """
     utils.explicit_tenant_name_message(tenant_name, logger)
     logger.info('Resuming execution group %s', group_id)
     client.execution_groups.resume(group_id, force=reset_operations)
     logger.info("A resume request for group %s has been sent", group_id)
 
 
 @groups.command('set-success-group',
@@ -751,26 +773,49 @@
 @cfy.options.tenant_name(
     required=False, resource_name_for_help='execution group')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
 def execution_groups_set_failure(group_id, failure_group_id,
                                  client, logger, tenant_name):
-    """Set success target group for this execution-group.
+    """Set failure target group for this execution-group.
 
-    Deployments for which the execution succeeds, will be added to the
+    Deployments for which the execution fails, will be added to the
     success target deployments group.
     """
     utils.explicit_tenant_name_message(tenant_name, logger)
     client.execution_groups.set_target_group(
         group_id, failed_group=failure_group_id)
-    logger.info('Execution group %s: success target group set to %s',
+    logger.info('Execution group %s: failure target group set to %s',
                 group_id, failure_group_id)
 
 
+@groups.command('set-concurrency',
+                short_help='Change the concurrency for a group')
+@cfy.argument('group-id')
+@cfy.argument('concurrency', type=int)
+@cfy.options.tenant_name(
+    required=False, resource_name_for_help='execution group')
+@cfy.options.common_options
+@cfy.pass_client()
+@cfy.pass_logger
+def execution_groups_set_concurrency(
+    group_id, concurrency, client, logger, tenant_name,
+):
+    """Change the concurrency setting of an execution group.
+
+    When starting executions belonging to this group, the new concurrency
+    setting will be used. Already-running executions are unaffected.
+    """
+    utils.explicit_tenant_name_message(tenant_name, logger)
+    client.execution_groups.set_concurrency(group_id, concurrency)
+    logger.info('Execution group %s: concurrency set to %s',
+                group_id, concurrency)
+
+
 @cfy.group(name='executions')
 @cfy.options.common_options
 def local_executions():
     """Handle workflow executions"""
 
 
 @local_executions.command(name='start', short_help='Execute a workflow')
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/groups.py` & `cloudify-7.0.0/cloudify_cli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/init.py` & `cloudify-7.0.0/cloudify_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/install.py` & `cloudify-7.0.0/cloudify_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/ldap.py` & `cloudify-7.0.0/cloudify_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/license.py` & `cloudify-7.0.0/cloudify_cli/commands/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/log_bundles.py` & `cloudify-7.0.0/cloudify_cli/commands/log_bundles.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/maintenance_mode.py` & `cloudify-7.0.0/cloudify_cli/commands/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/node_instances.py` & `cloudify-7.0.0/cloudify_cli/commands/node_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,30 @@
 @node_instances.command(name='get',
                         short_help='Retrieve node-instance information '
                                    '[manager only]')
 @cfy.argument('node_instance_id')
 @cfy.options.common_options
 @cfy.options.tenant_name(
     required=False, resource_name_for_help='node-instance')
+@cfy.options.evaluate_functions
 @cfy.pass_logger
 @cfy.pass_client()
 @cfy.options.extended_view
-def get(node_instance_id, logger, client, tenant_name):
+def get(node_instance_id, evaluate_functions, logger, client, tenant_name):
     """Retrieve information for a specific node-instance
 
     `NODE_INSTANCE_ID` is the id of the node-instance to get information on.
     """
     utils.explicit_tenant_name_message(tenant_name, logger)
-    logger.info('Retrieving node instance {0}'.format(node_instance_id))
+    logger.info('Retrieving node instance %s', node_instance_id)
     try:
-        node_instance = client.node_instances.get(node_instance_id)
+        node_instance = client.node_instances.get(
+            node_instance_id,
+            evaluate_functions=evaluate_functions,
+        )
     except CloudifyClientError as e:
         if e.status_code != 404:
             raise
         raise CloudifyCliError('Node instance {0} not found'.format(
             node_instance_id))
 
     _print_node_instance(node_instance)
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/nodes.py` & `cloudify-7.0.0/cloudify_cli/commands/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,27 +56,39 @@
 
 @nodes.command(name='get',
                short_help='Retrieve node information [manager only]')
 @cfy.argument('node-id')
 @cfy.options.deployment_id(required=True)
 @cfy.options.common_options
 @cfy.options.tenant_name(required=False, resource_name_for_help='node')
+@cfy.options.evaluate_functions
 @cfy.pass_logger
 @cfy.pass_client()
 @cfy.options.extended_view
-def get(node_id, deployment_id, logger, client, tenant_name):
+def get(
+    node_id,
+    deployment_id,
+    evaluate_functions,
+    client,
+    logger,
+    tenant_name,
+):
     """Retrieve information for a specific node of a specific deployment
 
     `NODE_ID` is the node id to get information on.
     """
     utils.explicit_tenant_name_message(tenant_name, logger)
     logger.info('Retrieving node {0} for deployment {1}'.format(
         node_id, deployment_id))
     try:
-        node = client.nodes.get(deployment_id, node_id)
+        node = client.nodes.get(
+            deployment_id,
+            node_id,
+            evaluate_functions=evaluate_functions,
+        )
     except CloudifyClientError as e:
         if e.status_code != 404:
             raise
         raise CloudifyCliError('Node {0} was not found'.format(node_id))
 
     logger.debug('Getting node instances for node with ID \'{0}\''
                  .format(node_id))
@@ -153,27 +165,29 @@
     is_flag=True,
 )
 @cfy.options.all_tenants
 @cfy.options.search
 @cfy.options.pagination_offset
 @cfy.options.pagination_size
 @cfy.options.common_options
+@cfy.options.evaluate_functions
 @cfy.pass_logger
 @cfy.pass_client()
 @cfy.options.extended_view
 def nodes_list(
     deployment_id,
     sort_by,
     descending,
     tenant_name,
     all_tenants,
     run_checks,
     search,
     pagination_offset,
     pagination_size,
+    evaluate_functions,
     logger,
     client
 ):
     """List nodes
 
     If `DEPLOYMENT_ID` is provided, list nodes for that deployment.
     Otherwise, list nodes for all deployments.
@@ -191,14 +205,15 @@
         else:
             logger.info('Listing all nodes...')
             instance_counts = False
         nodes = client.nodes.list(
             deployment_id=deployment_id,
             sort=sort_by,
             is_descending=descending,
+            evaluate_functions=evaluate_functions,
             _all_tenants=all_tenants,
             _search=search,
             _offset=pagination_offset,
             _size=pagination_size,
             _instance_counts=instance_counts,
         )
     except CloudifyClientError as e:
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/permissions.py` & `cloudify-7.0.0/cloudify_cli/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/plugins.py` & `cloudify-7.0.0/cloudify_cli/commands/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,16 @@
            logger,
            client,
            tenant_name):
     """Upload a plugin to the manager
 
     `PLUGIN_PATH` is the path to wagon archive to upload.
     """
-    client.license.check()
+    if client.manager.get_version().get('edition') == 'premium':
+        client.license.check()
     # Test whether the path is a valid URL. If it is, no point in doing local
     # validations - it will be validated on the server side anyway
     utils.explicit_tenant_name_message(tenant_name, logger)
     logger.info('Creating plugin zip archive..')
     wagon_path = utils.get_local_path(plugin_path, create_temp=True)
     zip_files = [wagon_path] + \
                 [utils.get_local_path(p, create_temp=True) for p in yaml_path]
@@ -157,25 +158,29 @@
                                        plugin_title=title,
                                        visibility=visibility,
                                        progress_callback=progress_handler)
         logger.info("Plugin uploaded. Plugin's id is %s", plugin.id)
     finally:
         for f in zip_files:
             os.remove(f)
+            f_dir = os.path.dirname(f)
+            if os.path.exists(f_dir) and os.path.isdir(f_dir):
+                os.rmdir(f_dir)
         os.remove(zip_path)
 
 
 @plugins.command(name='bundle-upload',
                  short_help='Upload a bundle of plugins [manager only]')
 @cfy.options.plugins_bundle_path
 @cfy.pass_client()
 @cfy.pass_logger
 @cfy.options.extended_view
 def upload_caravan(client, logger, path):
-    client.license.check()
+    if client.manager.get_version().get('edition') == 'premium':
+        client.license.check()
     if not path:
         logger.info("Starting upload of plugins bundle, "
                     "this may take few minutes to complete.")
         path = 'http://repository.cloudifysource.org/' \
                'cloudify/wagons/cloudify-plugins-bundle.tgz'
     progress = utils.generate_progress_handler(path, '')
     plugins_ = client.plugins.upload(path, progress_callback=progress)
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/profiles.py` & `cloudify-7.0.0/cloudify_cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/sites.py` & `cloudify-7.0.0/cloudify_cli/commands/sites.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/snapshots.py` & `cloudify-7.0.0/cloudify_cli/commands/snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 @cfy.group(name='snapshots')
 @cfy.options.common_options
 @cfy.assert_manager_active()
 def snapshots():
     """Handle manager snapshots
     """
-    pass
 
 
 @snapshots.command(name='restore',
                    short_help='Restore a manager from a snapshot '
                    '[manager only]')
 @cfy.argument('snapshot-id')
 @cfy.options.force(help=helptexts.FORCE_RESTORE_ON_DIRTY_MANAGER)
@@ -93,23 +92,25 @@
 @cfy.argument('snapshot-id', required=False, callback=cfy.validate_name)
 @cfy.options.exclude_credentials
 @cfy.options.exclude_logs
 @cfy.options.exclude_events
 @cfy.options.common_options
 @cfy.options.queue_snapshot
 @cfy.options.tempdir_path
+@cfy.options.legacy
 @cfy.options.wait_for_status
 @cfy.pass_client()
 @cfy.pass_logger
 def create(snapshot_id,
            exclude_credentials,
            exclude_logs,
            exclude_events,
            queue,
            tempdir_path,
+           legacy,
            wait_for_status,
            logger,
            client):
     """Create a snapshot on the manager
 
     The snapshot will contain the relevant data to restore a manager to
     its previous state.
@@ -120,15 +121,16 @@
     logger.info('Creating snapshot {0}...'.format(snapshot_id))
 
     execution = client.snapshots.create(snapshot_id,
                                         not exclude_credentials,
                                         not exclude_logs,
                                         not exclude_events,
                                         queue,
-                                        tempdir_path=tempdir_path)
+                                        tempdir_path=tempdir_path,
+                                        legacy=legacy)
     started_log_msg = "Started workflow execution. The execution's id is" \
                       " {0}.".format(execution.id)
     queued_log_msg = '`queue` flag was passed, snapshot creation will start' \
                      ' automatically when possible. Execution id:' \
                      ' {0}'.format(execution.id)
     queued = True if execution.status == 'queued' else False
     logger.info(queued_log_msg) if queued else logger.info(started_log_msg)
@@ -176,15 +178,16 @@
            logger,
            client,
            tenant_name):
     """Upload a snapshot to the manager
 
     `SNAPSHOT_PATH` is the path to the snapshot to upload.
     """
-    client.license.check()
+    if client.manager.get_version().get('edition') == 'premium':
+        client.license.check()
     utils.explicit_tenant_name_message(tenant_name, logger)
     snapshot_id = snapshot_id or utils.generate_suffixed_id('snapshot')
 
     logger.info('Uploading snapshot {0}...'.format(snapshot_path))
     progress_handler = utils.generate_progress_handler(snapshot_path, '')
     snapshot = client.snapshots.upload(snapshot_path,
                                        snapshot_id,
```

### Comparing `cloudify-6.4.2/cloudify_cli/commands/status.py` & `cloudify-7.0.0/cloudify_cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/summary.py` & `cloudify-7.0.0/cloudify_cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/tenants.py` & `cloudify-7.0.0/cloudify_cli/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/tokens.py` & `cloudify-7.0.0/cloudify_cli/commands/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/uninstall.py` & `cloudify-7.0.0/cloudify_cli/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/user_groups.py` & `cloudify-7.0.0/cloudify_cli/commands/user_groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/users.py` & `cloudify-7.0.0/cloudify_cli/commands/users.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/commands/workflows.py` & `cloudify-7.0.0/cloudify_cli/commands/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/config/__init__.py` & `cloudify-7.0.0/cloudify_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/config/config.py` & `cloudify-7.0.0/cloudify_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/constants.py` & `cloudify-7.0.0/cloudify_cli/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/env.py` & `cloudify-7.0.0/cloudify_cli/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,27 @@
 import errno
 import types
 import shutil
 import getpass
 import tempfile
 import itertools
 from base64 import b64encode
-from contextlib import contextmanager
 
 import yaml
 import requests
 
 from cloudify_rest_client import CloudifyClient
 from cloudify_rest_client.client import HTTPClient
 from cloudify.cluster_status import CloudifyNodeType
 from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify.utils import ipv6_url_compat
 
 from cloudify_cli import constants
 from cloudify_cli.exceptions import CloudifyCliError
 
-try:
-    from fabric import Connection
-    from paramiko import AuthenticationException
-except ImportError:
-    Connection = None
-
 
 _ENV_NAME = 'manager'
 DEFAULT_LOG_FILE = os.path.expanduser(
     '{0}/cloudify-{1}/cloudify-cli.log'.format(
         tempfile.gettempdir(), getpass.getuser()))
 
 CLOUDIFY_WORKDIR = os.path.join(
@@ -670,60 +663,9 @@
         super(CloudifyClusterClient, self).__init__(*args, **kwargs)
 
     def client_class(self, *args, **kwargs):
         kwargs.setdefault('profile', self._profile)
         return ClusterHTTPClient(*args, **kwargs)
 
 
-@contextmanager
-def ssh_connection(host=None, user=None, key=None):
-    if Connection is None:
-        raise CloudifyCliError(
-            "SSH not available - fabric not installed")
-    if host is None:
-        host = profile.manager_ip
-    if user is None:
-        user = profile.ssh_user
-    if key is None:
-        key = profile.ssh_key
-    connect_kwargs = {}
-    if key:
-        connect_kwargs['key_filename'] = [key]
-    conn = Connection(
-        host=host,
-        user=user,
-        port=profile.ssh_port or 22,
-        connect_kwargs=connect_kwargs or None
-    )
-    try:
-        conn.open()
-        yield conn
-    except AuthenticationException as e:
-        if user:
-            user_message = user
-        else:
-            user_message = '{0} (from ssh config)'.format(conn.user)
-
-        if key:
-            key_message = key
-        elif conn.ssh_config.get('identityfile'):
-            key_message = '{0} (from ssh config)'.format(
-                ', '.join(conn.ssh_config['identityfile']))
-        else:
-            key_message = 'default'
-
-        raise CloudifyCliError(
-            "SSH: could not connect to {host} "
-            "(username: {user}, key: {key}): {exc}"
-            .format(
-                host=conn.host,
-                user=user_message,
-                key=key_message,
-                exc=e
-            )
-        )
-    finally:
-        conn.close()
-
-
 profile = get_profile_context(suppress_error=True)
 target_manager = None
```

### Comparing `cloudify-6.4.2/cloudify_cli/exceptions.py` & `cloudify-7.0.0/cloudify_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/execution_events_fetcher.py` & `cloudify-7.0.0/cloudify_cli/execution_events_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/filters_utils.py` & `cloudify-7.0.0/cloudify_cli/filters_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 
 from cloudify_cli import utils
 from cloudify_cli.exceptions import CloudifyCliError
 from cloudify_cli.table import print_data, print_details
 from cloudify_cli.utils import validate_visibility, handle_client_error
 
-from cloudify._compat import PY2
 from cloudify_rest_client.exceptions import InvalidFilterRule
 
 FILTERS_COLUMNS = ['id', 'labels_filter_rules', 'attrs_filter_rules',
                    'created_at', 'updated_at', 'visibility',
                    'tenant_name', 'created_by']
 
 NOT_FOUND_MSG = 'Requested {0} filter with ID `{1}` was not found in ' \
@@ -77,17 +76,14 @@
 
         return [value.replace('\x00', ',').replace('\\:', ':')
                 for value in raw_values_list]
 
     def __str__(self, cli_operator):
         values = (self['values'][0] if len(self['values']) == 1 else
                   u'[{0}]'.format(','.join(self['values'])))
-        if PY2:
-            values = values.encode('utf-8')
-
         return '"{key}{operator}{values}"'.format(key=self['key'],
                                                   operator=cli_operator,
                                                   values=values)
 
 
 class LabelsFilterRule(FilterRule):
     def __init__(self, key, values, operator):
```

### Comparing `cloudify-6.4.2/cloudify_cli/inputs.py` & `cloudify-7.0.0/cloudify_cli/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from __future__ import absolute_import
 
 import os
 import glob
 import yaml
 import json
 
-from cloudify._compat import text_type
-
 from cloudify_cli.exceptions import CloudifyCliError
 from cloudify_cli.logger import get_logger
 from cloudify_cli.utils import deep_update_dict, insert_dotted_key_to_dict
 
 
 # TODO: Add test for inputs as JSON/YAML string
 def inputs_to_dict(resources, **kwargs):
@@ -44,15 +42,15 @@
         return dict()
 
     parsed_dict = {}
 
     for resource in resources:
         logger.debug('Processing inputs source: {0}'.format(resource))
         # Workflow parameters always pass an empty dictionary. We ignore it
-        if isinstance(resource, (text_type, bytes)):
+        if isinstance(resource, (str, bytes)):
             try:
                 if kwargs.get('dot_hierarchy'):
                     deep_update_dict(parsed_dict,
                                      _parse_single_input(resource, **kwargs))
                 else:
                     parsed_dict.update(_parse_single_input(resource))
             except CloudifyCliError as ex:
```

### Comparing `cloudify-6.4.2/cloudify_cli/labels_utils.py` & `cloudify-7.0.0/cloudify_cli/labels_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/local.py` & `cloudify-7.0.0/cloudify_cli/local.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/logger.py` & `cloudify-7.0.0/cloudify_cli/logger.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/main.py` & `cloudify-7.0.0/cloudify_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,45 +109,25 @@
     import_spec=('cloudify_cli.commands.profiles', 'profiles'),
     short_help='Handle Cloudify CLI profiles'
 )
 def profiles():
     pass
 
 
-@click.command(
-    name='ssh',
-    cls=LazyLoadedCommand,
-    short_help='Connect using SSH [manager only]',
-    import_spec=('cloudify_cli.commands.ssh', 'ssh'),
-)
-def ssh():
-    pass
-
-
 @click.group(
     name='idp',
     cls=LazyLoadedGroup,
     import_spec=('cloudify_cli.commands.idp', 'idp'),
     short_help='Identity provider commands'
 )
 def idp():
     pass
 
 
 @click.group(
-    name='logs',
-    cls=LazyLoadedGroup,
-    import_spec=('cloudify_cli.commands.logs', 'logs'),
-    short_help='Handle manager service logs'
-)
-def logs():
-    pass
-
-
-@click.group(
     name='ldap',
     cls=LazyLoadedGroup,
     import_spec=('cloudify_cli.commands.ldap', 'ldap'),
     short_help='Set LDAP authenticator'
 )
 def ldap():
     pass
@@ -450,14 +430,24 @@
     import_spec=('cloudify_cli.commands.permissions', 'permissions'),
     short_help="Handle manager user permissions"
 )
 def permissions():
     pass
 
 
+@click.group(
+    name='community',
+    cls=LazyLoadedGroup,
+    import_spec=('cloudify_cli.commands.community', 'community'),
+    short_help="Commands specific for the Community edition"
+)
+def community():
+    pass
+
+
 @click.command(
     name='install',
     cls=LazyLoadedCommand,
     import_spec=('cloudify_cli.commands.install', 'manager'),
     short_help='Install an application blueprint [manager only]'
 )
 def manager_install():
@@ -520,17 +510,15 @@
         """
         cfy.set_cli_except_hook(verbose)
 
     _cfy.add_command(init)
     _cfy.add_command(status)
     _cfy.add_command(profiles)
 
-    _cfy.add_command(ssh)
     _cfy.add_command(idp)
-    _cfy.add_command(logs)
     _cfy.add_command(ldap)
     _cfy.add_command(users)
     _cfy.add_command(agents)
     _cfy.add_command(events)
     _cfy.add_command(cluster)
     _cfy.add_command(cluster_managers)
     _cfy.add_command(cluster_db_nodes)
@@ -546,14 +534,15 @@
     _cfy.add_command(groups)
     _cfy.add_command(workflows)
     _cfy.add_command(license)
     _cfy.add_command(sites)
     _cfy.add_command(certificates)
     _cfy.add_command(apply)
     _cfy.add_command(auditlog)
+    _cfy.add_command(community)
 
     if env.is_manager_active():
         _cfy.add_command(manager_blueprints)
         _cfy.add_command(manager_deployments)
         _cfy.add_command(manager_executions)
         _cfy.add_command(manager_node_instances)
         _cfy.add_command(config)
```

### Comparing `cloudify-6.4.2/cloudify_cli/prettytable.py` & `cloudify-7.0.0/cloudify_cli/prettytable.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/replace_certificates_config.py` & `cloudify-7.0.0/cloudify_cli/replace_certificates_config.py`

 * *Files identical despite different names*

### Comparing `cloudify-6.4.2/cloudify_cli/table.py` & `cloudify-7.0.0/cloudify_cli/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from cloudify_cli.logger import (
     get_global_json_output,
     get_global_extended_view,
     CloudifyJSONEncoder,
     output)
 from cloudify_cli.prettytable import PrettyTable
 
-from cloudify._compat import text_type
-
 
 def generate(cols, data, defaults=None, labels=None):
     """
     Return a new PrettyTable instance representing the list.
 
     Arguments:
 
@@ -77,15 +75,15 @@
         display_value = get_values_per_column(c, data, defaults)
         pt.add_row([labels.get(c, c), display_value])
     return pt
 
 
 def get_values_per_column(column, row_data, defaults):
     if column in row_data:
-        if row_data[column] and isinstance(row_data[column], text_type):
+        if row_data[column] and isinstance(row_data[column], str):
             row_data[column] = get_timestamp(row_data[column]) \
                 or row_data[column]
         elif row_data[column] and isinstance(row_data[column], list):
             row_data[column] = ','.join(row_data[column])
         elif isinstance(row_data[column], bool):
             pass  # Taking care of False (otherwise would be changed to '')
         elif isinstance(row_data[column], int):
```

### Comparing `cloudify-6.4.2/cloudify_cli/utils.py` & `cloudify-7.0.0/cloudify_cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,21 @@
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 import yaml
 import requests
 from retrying import retry
+from urllib.parse import urlparse
 
 from cloudify_cli.constants import SUPPORTED_ARCHIVE_TYPES, DEFAULT_TIMEOUT
 from cloudify_cli.exceptions import CloudifyCliError, CloudifyTimeoutError
 from cloudify_cli.execution_events_fetcher import ExecutionEventsFetcher
 from cloudify_cli.logger import get_logger, get_events_logger
 
-from cloudify._compat import urlparse
 from cloudify.models_states import BlueprintUploadState
 from cloudify_rest_client.constants import VisibilityState
 from cloudify_rest_client.exceptions import CloudifyClientError
 
 WAIT_FOR_BLUEPRINT_UPLOAD_SLEEP_INTERVAL = 1
```

### Comparing `cloudify-6.4.2/setup.py` & `cloudify-7.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,48 +13,35 @@
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 import sys
 
 from setuptools import setup
 
 install_requires = [
-        'click>7,<8',
-        'wagon[venv]>=0.10.1',
+        'click>8,<9',
+        'wagon[venv]>=0.11.2',
         'retrying==1.3.3',
         'colorama==0.4.4',
         'requests>=2.7.0,<3.0.0',
-        'click_didyoumean==0.0.3',
-        'cloudify-common[dispatcher]==6.4.2',
+        'click_didyoumean==0.3.0',
+        'cloudify-common[dispatcher]==7.0.0',
         'backports.shutil_get_terminal_size==1.0.0',
-        'ipaddress==1.0.23',
-        'setuptools<=40.7.3',
-        'cryptography==3.3.2',
-        'cffi>=1.14,<1.15',
-        'pynacl==1.4.0',
-        # Fabric depend on paramiko that depends on cryptography so we need
-        # to install the correct version of cryptography before installing
-        # the fabric so that fabric can be installed correctly in both py2 +
-        # py3
-        'fabric==2.5.0',
+        'cryptography>=37,<40',
+        'fabric==2.7.1',
 ]
-if sys.version_info[:2] < (3, 6):
-    install_requires.append('pyyaml==5.4.1')
-else:
-    install_requires.append('pyyaml==6.0')
 
 packages = ['cloudify_cli',
             'cloudify_cli.cli',
             'cloudify_cli.commands',
-            'cloudify_cli.config']
-if sys.version_info[:2] >= (3, 6):
-    packages += ['cloudify_cli.async_commands']
+            'cloudify_cli.config',
+            'cloudify_cli.async_commands']
 
 setup(
     name='cloudify',
-    version='6.4.2',
+    version='7.0.0',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=packages,
     license='LICENSE',
     description="Cloudify's Command Line Interface",
     entry_points={
         'console_scripts': [
```

