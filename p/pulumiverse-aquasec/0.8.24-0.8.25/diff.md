# Comparing `tmp/pulumiverse_aquasec-0.8.24.tar.gz` & `tmp/pulumiverse_aquasec-0.8.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_aquasec-0.8.24.tar", last modified: Tue Apr  4 16:30:46 2023, max compression
+gzip compressed data, was "pulumiverse_aquasec-0.8.25.tar", last modified: Tue Apr 25 11:36:03 2023, max compression
```

## Comparing `pulumiverse_aquasec-0.8.24.tar` & `pulumiverse_aquasec-0.8.25.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   245766 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/acknowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/application_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/aqua_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   149029 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/container_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   155371 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/enforcer_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/firewall_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   153018 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/function_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/function_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_acknowledges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_application_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_aqua_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_container_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    42589 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_enforcer_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_firewall_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    43775 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_function_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_function_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    44693 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_assurance_polic.py
--rw-r--r--   0 runner    (1001) docker     (123)    43663 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    43691 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_image_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_integration_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_integration_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    44517 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_kubernetes_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_permissions_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles_mapping_saas.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_users_saas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/group.py
--rw-r--r--   0 runner    (1001) docker     (123)   152546 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/host_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    91347 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/host_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    71537 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/image.py
--rw-r--r--   0 runner    (1001) docker     (123)   152664 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/image_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    50533 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/integration_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   165870 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/kubernetes_assurance_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/notification_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)   313233 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16769 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/permissions_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role_mapping_saas.py
--rw-r--r--   0 runner    (1001) docker     (123)    43677 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/user_saas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 16:30:46.579382 pulumiverse_aquasec-0.8.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-04 16:30:46.000000 pulumiverse_aquasec-0.8.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245766 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/acknowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/application_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/aqua_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149029 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/container_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155371 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/enforcer_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/firewall_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153018 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/function_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/function_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_acknowledges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_application_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_aqua_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_container_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42589 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_enforcer_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_firewall_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43775 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_function_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_function_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44693 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_assurance_polic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43663 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43691 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_image_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_integration_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_integration_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44517 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_kubernetes_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_permissions_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles_mapping_saas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_users_saas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152546 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/host_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91347 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/host_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71537 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152664 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/image_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50533 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/integration_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165870 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/kubernetes_assurance_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/notification_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)   313233 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16769 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/permissions_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role_mapping_saas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43677 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/user_saas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:36:03.745252 pulumiverse_aquasec-0.8.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 11:36:03.000000 pulumiverse_aquasec-0.8.25/setup.py
```

### Comparing `pulumiverse_aquasec-0.8.24/PKG-INFO` & `pulumiverse_aquasec-0.8.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_aquasec
-Version: 0.8.24
+Version: 0.8.25
 Summary: A Pulumi package for creating and managing Aquasec cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-aquasec
 Keywords: pulumi aquasec category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_aquasec-0.8.24/README.md` & `pulumiverse_aquasec-0.8.25/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/__init__.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/_inputs.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/_utilities.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/acknowledge.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/acknowledge.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/application_scope.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/application_scope.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/aqua_label.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/aqua_label.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/config/vars.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/container_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/container_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/enforcer_groups.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/enforcer_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/firewall_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/function_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/function_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/function_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/function_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_acknowledges.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_acknowledges.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_application_scope.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_application_scope.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_aqua_labels.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_aqua_labels.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_container_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_container_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_enforcer_groups.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_enforcer_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_firewall_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_function_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_function_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_function_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_function_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_gateways.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_gateways.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_groups.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_assurance_polic.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_assurance_polic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_host_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_host_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_image.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_image_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_image_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_integration_registry.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_integration_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_integration_state.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_integration_state.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_kubernetes_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_kubernetes_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_notifications.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_permissions_sets.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_permissions_sets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles_mapping.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_roles_mapping_saas.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_roles_mapping_saas.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_service.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_users.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/get_users_saas.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/get_users_saas.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/group.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/host_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/host_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/host_runtime_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/host_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/image.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/image.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/image_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/image_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/integration_registry.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/integration_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/kubernetes_assurance_policy.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/kubernetes_assurance_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/notification.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/notification_slack.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/notification_slack.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/outputs.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/permissions_sets.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/permissions_sets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/provider.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role_mapping.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/role_mapping_saas.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/role_mapping_saas.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/service.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/user.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec/user_saas.py` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec/user_saas.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/PKG-INFO` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-aquasec
-Version: 0.8.24
+Version: 0.8.25
 Summary: A Pulumi package for creating and managing Aquasec cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-aquasec
 Keywords: pulumi aquasec category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_aquasec-0.8.24/pulumiverse_aquasec.egg-info/SOURCES.txt` & `pulumiverse_aquasec-0.8.25/pulumiverse_aquasec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_aquasec-0.8.24/setup.py` & `pulumiverse_aquasec-0.8.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.8.24"
-PLUGIN_VERSION = "0.8.24"
+VERSION = "0.8.25"
+PLUGIN_VERSION = "0.8.25"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aquasec', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-aquasec'])
         except OSError as error:
```

