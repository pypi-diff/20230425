# Comparing `tmp/pulumi_fastly-7.3.0a1682029970.tar.gz` & `tmp/pulumi_fastly-7.4.0a1682376810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-7.3.0a1682029970.tar", last modified: Thu Apr 20 22:37:35 2023, max compression
+gzip compressed data, was "pulumi_fastly-7.4.0a1682376810.tar", last modified: Mon Apr 24 23:00:30 2023, max compression
```

## Comparing `pulumi_fastly-7.3.0a1682029970.tar` & `pulumi_fastly-7.4.0a1682376810.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   504881 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)   449591 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   504881 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)   449591 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:00:30.714122 pulumi_fastly-7.4.0a1682376810/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-24 23:00:30.000000 pulumi_fastly-7.4.0a1682376810/setup.py
```

### Comparing `pulumi_fastly-7.3.0a1682029970/PKG-INFO` & `pulumi_fastly-7.4.0a1682376810/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 7.3.0a1682029970
+Version: 7.4.0a1682376810
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.3.0a1682029970/README.md` & `pulumi_fastly-7.4.0a1682376810/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/__init__.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_inputs.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_utilities.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/vars.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_services.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/outputs.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/provider.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_authorization.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_compute.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_vcl.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_activation.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/user.py` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 7.3.0a1682029970
+Version: 7.4.0a1682376810
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-7.4.0a1682376810/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1682029970/setup.py` & `pulumi_fastly-7.4.0a1682376810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "7.3.0a1682029970"
-PLUGIN_VERSION = "7.3.0-alpha.1682029970+a58f0717"
+VERSION = "7.4.0a1682376810"
+PLUGIN_VERSION = "7.4.0-alpha.1682376810+704fb577"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

