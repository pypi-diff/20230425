# Comparing `tmp/pulumi_proxmoxve-3.1.0.tar.gz` & `tmp/pulumi_proxmoxve-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-3.1.0.tar", last modified: Tue Apr  4 09:38:51 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-4.0.0.tar", last modified: Tue Apr 25 11:53:38 2023, max compression
```

## Comparing `pulumi_proxmoxve-3.1.0.tar` & `pulumi_proxmoxve-4.0.0.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.279748 pulumi_proxmoxve-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-04 09:38:51.279748 pulumi_proxmoxve-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.271748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.271748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/cluster_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/cluster_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_cluster_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_cluster_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.271748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.275748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.275748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.275748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.275748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34037 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80659 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:38:51.271748 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:38:51.279748 pulumi_proxmoxve-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-04 09:38:51.000000 pulumi_proxmoxve-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.666999 pulumi_proxmoxve-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-25 11:53:38.666999 pulumi_proxmoxve-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.658999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.658999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.662999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.662999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.662999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.662999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.662999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.666999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83159 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:53:38.658999 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:53:38.666999 pulumi_proxmoxve-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-25 11:53:38.000000 pulumi_proxmoxve-4.0.0/setup.py
```

### Comparing `pulumi_proxmoxve-3.1.0/PKG-INFO` & `pulumi_proxmoxve-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 3.1.0
+Version: 4.0.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Proxmox VE Resource Provider
 
 [![](https://img.shields.io/github/license/muhlba91/pulumi-proxmoxve?style=for-the-badge)](LICENSE)
 [![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/release.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions)
 [![](https://img.shields.io/github/release-date/muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/releases)
```

### Comparing `pulumi_proxmoxve-3.1.0/README.md` & `pulumi_proxmoxve-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 if typing.TYPE_CHECKING:
     import pulumi_proxmoxve.cluster as __cluster
     cluster = __cluster
     import pulumi_proxmoxve.config as __config
     config = __config
     import pulumi_proxmoxve.ct as __ct
     ct = __ct
+    import pulumi_proxmoxve.network as __network
+    network = __network
     import pulumi_proxmoxve.permission as __permission
     permission = __permission
     import pulumi_proxmoxve.storage as __storage
     storage = __storage
     import pulumi_proxmoxve.vm as __vm
     vm = __vm
 else:
     cluster = _utilities.lazy_import('pulumi_proxmoxve.cluster')
     config = _utilities.lazy_import('pulumi_proxmoxve.config')
     ct = _utilities.lazy_import('pulumi_proxmoxve.ct')
+    network = _utilities.lazy_import('pulumi_proxmoxve.network')
     permission = _utilities.lazy_import('pulumi_proxmoxve.permission')
     storage = _utilities.lazy_import('pulumi_proxmoxve.storage')
     vm = _utilities.lazy_import('pulumi_proxmoxve.vm')
 
 _utilities.register(
     resource_modules="""
 [
@@ -48,26 +51,58 @@
   "fqn": "pulumi_proxmoxve.ct",
   "classes": {
    "proxmoxve:CT/container:Container": "Container"
   }
  },
  {
   "pkg": "proxmoxve",
-  "mod": "Cluster/clusterAlias",
-  "fqn": "pulumi_proxmoxve.cluster",
+  "mod": "Network/firewall",
+  "fqn": "pulumi_proxmoxve.network",
   "classes": {
-   "proxmoxve:Cluster/clusterAlias:ClusterAlias": "ClusterAlias"
+   "proxmoxve:Network/firewall:Firewall": "Firewall"
   }
  },
  {
   "pkg": "proxmoxve",
-  "mod": "Cluster/clusterIPSet",
-  "fqn": "pulumi_proxmoxve.cluster",
+  "mod": "Network/firewallAlias",
+  "fqn": "pulumi_proxmoxve.network",
   "classes": {
-   "proxmoxve:Cluster/clusterIPSet:ClusterIPSet": "ClusterIPSet"
+   "proxmoxve:Network/firewallAlias:FirewallAlias": "FirewallAlias"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "Network/firewallIPSet",
+  "fqn": "pulumi_proxmoxve.network",
+  "classes": {
+   "proxmoxve:Network/firewallIPSet:FirewallIPSet": "FirewallIPSet"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "Network/firewallOptions",
+  "fqn": "pulumi_proxmoxve.network",
+  "classes": {
+   "proxmoxve:Network/firewallOptions:FirewallOptions": "FirewallOptions"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "Network/firewallRules",
+  "fqn": "pulumi_proxmoxve.network",
+  "classes": {
+   "proxmoxve:Network/firewallRules:FirewallRules": "FirewallRules"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "Network/firewallSecurityGroup",
+  "fqn": "pulumi_proxmoxve.network",
+  "classes": {
+   "proxmoxve:Network/firewallSecurityGroup:FirewallSecurityGroup": "FirewallSecurityGroup"
   }
  },
  {
   "pkg": "proxmoxve",
   "mod": "Permission/group",
   "fqn": "pulumi_proxmoxve.permission",
   "classes": {
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/outputs.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,50 +6,55 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'ClusterIPSetCidrArgs',
+    'VirtualEnvironment',
 ]
 
-@pulumi.input_type
-class ClusterIPSetCidrArgs:
+@pulumi.output_type
+class VirtualEnvironment(dict):
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 comment: Optional[pulumi.Input[str]] = None,
-                 nomatch: Optional[pulumi.Input[bool]] = None):
-        pulumi.set(__self__, "name", name)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if nomatch is not None:
-            pulumi.set(__self__, "nomatch", nomatch)
+                 endpoint: Optional[str] = None,
+                 insecure: Optional[bool] = None,
+                 otp: Optional[str] = None,
+                 password: Optional[str] = None,
+                 username: Optional[str] = None):
+        if endpoint is not None:
+            pulumi.set(__self__, "endpoint", endpoint)
+        if insecure is not None:
+            pulumi.set(__self__, "insecure", insecure)
+        if otp is not None:
+            pulumi.set(__self__, "otp", otp)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    def endpoint(self) -> Optional[str]:
+        return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "comment")
+    def insecure(self) -> Optional[bool]:
+        return pulumi.get(self, "insecure")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @property
+    @pulumi.getter
+    def otp(self) -> Optional[str]:
+        return pulumi.get(self, "otp")
 
     @property
     @pulumi.getter
-    def nomatch(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "nomatch")
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
 
-    @nomatch.setter
-    def nomatch(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "nomatch", value)
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/cluster_alias.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,235 +4,218 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['ClusterAliasArgs', 'ClusterAlias']
+__all__ = ['PoolArgs', 'Pool']
 
 @pulumi.input_type
-class ClusterAliasArgs:
+class PoolArgs:
     def __init__(__self__, *,
-                 cidr: pulumi.Input[str],
-                 comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 pool_id: pulumi.Input[str],
+                 comment: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ClusterAlias resource.
-        :param pulumi.Input[str] cidr: IP/CIDR block
-        :param pulumi.Input[str] comment: Alias comment
-        :param pulumi.Input[str] name: Alias name
+        The set of arguments for constructing a Pool resource.
+        :param pulumi.Input[str] pool_id: The pool id
+        :param pulumi.Input[str] comment: The pool comment
         """
-        pulumi.set(__self__, "cidr", cidr)
+        pulumi.set(__self__, "pool_id", pool_id)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
 
     @property
-    @pulumi.getter
-    def cidr(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="poolId")
+    def pool_id(self) -> pulumi.Input[str]:
         """
-        IP/CIDR block
+        The pool id
         """
-        return pulumi.get(self, "cidr")
+        return pulumi.get(self, "pool_id")
 
-    @cidr.setter
-    def cidr(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cidr", value)
+    @pool_id.setter
+    def pool_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "pool_id", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Alias comment
+        The pool comment
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Alias name
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
 
 @pulumi.input_type
-class _ClusterAliasState:
+class _PoolState:
     def __init__(__self__, *,
-                 cidr: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 members: Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]] = None,
+                 pool_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ClusterAlias resources.
-        :param pulumi.Input[str] cidr: IP/CIDR block
-        :param pulumi.Input[str] comment: Alias comment
-        :param pulumi.Input[str] name: Alias name
+        Input properties used for looking up and filtering Pool resources.
+        :param pulumi.Input[str] comment: The pool comment
+        :param pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]] members: The pool members
+        :param pulumi.Input[str] pool_id: The pool id
         """
-        if cidr is not None:
-            pulumi.set(__self__, "cidr", cidr)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def cidr(self) -> Optional[pulumi.Input[str]]:
-        """
-        IP/CIDR block
-        """
-        return pulumi.get(self, "cidr")
-
-    @cidr.setter
-    def cidr(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cidr", value)
+        if members is not None:
+            pulumi.set(__self__, "members", members)
+        if pool_id is not None:
+            pulumi.set(__self__, "pool_id", pool_id)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Alias comment
+        The pool comment
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def members(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]]:
+        """
+        The pool members
+        """
+        return pulumi.get(self, "members")
+
+    @members.setter
+    def members(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]]):
+        pulumi.set(self, "members", value)
+
+    @property
+    @pulumi.getter(name="poolId")
+    def pool_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Alias name
+        The pool id
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "pool_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @pool_id.setter
+    def pool_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pool_id", value)
 
 
-class ClusterAlias(pulumi.CustomResource):
+class Pool(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidr: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 pool_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a ClusterAlias resource with the given unique name, props, and options.
+        Create a Pool resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: IP/CIDR block
-        :param pulumi.Input[str] comment: Alias comment
-        :param pulumi.Input[str] name: Alias name
+        :param pulumi.Input[str] comment: The pool comment
+        :param pulumi.Input[str] pool_id: The pool id
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ClusterAliasArgs,
+                 args: PoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a ClusterAlias resource with the given unique name, props, and options.
+        Create a Pool resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ClusterAliasArgs args: The arguments to use to populate this resource's properties.
+        :param PoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ClusterAliasArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PoolArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidr: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 pool_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ClusterAliasArgs.__new__(ClusterAliasArgs)
+            __props__ = PoolArgs.__new__(PoolArgs)
 
-            if cidr is None and not opts.urn:
-                raise TypeError("Missing required property 'cidr'")
-            __props__.__dict__["cidr"] = cidr
             __props__.__dict__["comment"] = comment
-            __props__.__dict__["name"] = name
-        super(ClusterAlias, __self__).__init__(
-            'proxmoxve:Cluster/clusterAlias:ClusterAlias',
+            if pool_id is None and not opts.urn:
+                raise TypeError("Missing required property 'pool_id'")
+            __props__.__dict__["pool_id"] = pool_id
+            __props__.__dict__["members"] = None
+        super(Pool, __self__).__init__(
+            'proxmoxve:Permission/pool:Pool',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            cidr: Optional[pulumi.Input[str]] = None,
             comment: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None) -> 'ClusterAlias':
+            members: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PoolMemberArgs']]]]] = None,
+            pool_id: Optional[pulumi.Input[str]] = None) -> 'Pool':
         """
-        Get an existing ClusterAlias resource's state with the given name, id, and optional extra
+        Get an existing Pool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: IP/CIDR block
-        :param pulumi.Input[str] comment: Alias comment
-        :param pulumi.Input[str] name: Alias name
+        :param pulumi.Input[str] comment: The pool comment
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PoolMemberArgs']]]] members: The pool members
+        :param pulumi.Input[str] pool_id: The pool id
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ClusterAliasState.__new__(_ClusterAliasState)
+        __props__ = _PoolState.__new__(_PoolState)
 
-        __props__.__dict__["cidr"] = cidr
         __props__.__dict__["comment"] = comment
-        __props__.__dict__["name"] = name
-        return ClusterAlias(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["members"] = members
+        __props__.__dict__["pool_id"] = pool_id
+        return Pool(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def cidr(self) -> pulumi.Output[str]:
+    def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        IP/CIDR block
+        The pool comment
         """
-        return pulumi.get(self, "cidr")
+        return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
+    def members(self) -> pulumi.Output[Sequence['outputs.PoolMember']]:
         """
-        Alias comment
+        The pool members
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "members")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="poolId")
+    def pool_id(self) -> pulumi.Output[str]:
         """
-        Alias name
+        The pool id
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "pool_id")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/cluster_ip_set.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/dns.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,237 +3,237 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
-from . import outputs
-from ._inputs import *
+from . import _utilities
 
-__all__ = ['ClusterIPSetArgs', 'ClusterIPSet']
+__all__ = ['DNSArgs', 'DNS']
 
 @pulumi.input_type
-class ClusterIPSetArgs:
+class DNSArgs:
     def __init__(__self__, *,
-                 cidrs: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 domain: pulumi.Input[str],
+                 node_name: pulumi.Input[str],
+                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a ClusterIPSet resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]] cidrs: List of IP or Networks
-        :param pulumi.Input[str] comment: IPSet comment
-        :param pulumi.Input[str] name: IPSet name
+        The set of arguments for constructing a DNS resource.
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
         """
-        if cidrs is not None:
-            pulumi.set(__self__, "cidrs", cidrs)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "domain", domain)
+        pulumi.set(__self__, "node_name", node_name)
+        if servers is not None:
+            pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
-    def cidrs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]]:
+    def domain(self) -> pulumi.Input[str]:
         """
-        List of IP or Networks
+        The DNS search domain
         """
-        return pulumi.get(self, "cidrs")
+        return pulumi.get(self, "domain")
 
-    @cidrs.setter
-    def cidrs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]]):
-        pulumi.set(self, "cidrs", value)
+    @domain.setter
+    def domain(self, value: pulumi.Input[str]):
+        pulumi.set(self, "domain", value)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Input[str]:
         """
-        IPSet comment
+        The node name
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "node_name")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @node_name.setter
+    def node_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "node_name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        IPSet name
+        The DNS servers
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "servers")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @servers.setter
+    def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "servers", value)
 
 
 @pulumi.input_type
-class _ClusterIPSetState:
+class _DNSState:
     def __init__(__self__, *,
-                 cidrs: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 domain: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering ClusterIPSet resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]] cidrs: List of IP or Networks
-        :param pulumi.Input[str] comment: IPSet comment
-        :param pulumi.Input[str] name: IPSet name
+        Input properties used for looking up and filtering DNS resources.
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
         """
-        if cidrs is not None:
-            pulumi.set(__self__, "cidrs", cidrs)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        if domain is not None:
+            pulumi.set(__self__, "domain", domain)
+        if node_name is not None:
+            pulumi.set(__self__, "node_name", node_name)
+        if servers is not None:
+            pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
-    def cidrs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]]:
+    def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        List of IP or Networks
+        The DNS search domain
         """
-        return pulumi.get(self, "cidrs")
+        return pulumi.get(self, "domain")
 
-    @cidrs.setter
-    def cidrs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterIPSetCidrArgs']]]]):
-        pulumi.set(self, "cidrs", value)
+    @domain.setter
+    def domain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "domain", value)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        IPSet comment
+        The node name
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "node_name")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @node_name.setter
+    def node_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "node_name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        IPSet name
+        The DNS servers
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "servers")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @servers.setter
+    def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "servers", value)
 
 
-class ClusterIPSet(pulumi.CustomResource):
+class DNS(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterIPSetCidrArgs']]]]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Create a ClusterIPSet resource with the given unique name, props, and options.
+        Create a DNS resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterIPSetCidrArgs']]]] cidrs: List of IP or Networks
-        :param pulumi.Input[str] comment: IPSet comment
-        :param pulumi.Input[str] name: IPSet name
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ClusterIPSetArgs] = None,
+                 args: DNSArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a ClusterIPSet resource with the given unique name, props, and options.
+        Create a DNS resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ClusterIPSetArgs args: The arguments to use to populate this resource's properties.
+        :param DNSArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ClusterIPSetArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DNSArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterIPSetCidrArgs']]]]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ClusterIPSetArgs.__new__(ClusterIPSetArgs)
+            __props__ = DNSArgs.__new__(DNSArgs)
 
-            __props__.__dict__["cidrs"] = cidrs
-            __props__.__dict__["comment"] = comment
-            __props__.__dict__["name"] = name
-        super(ClusterIPSet, __self__).__init__(
-            'proxmoxve:Cluster/clusterIPSet:ClusterIPSet',
+            if domain is None and not opts.urn:
+                raise TypeError("Missing required property 'domain'")
+            __props__.__dict__["domain"] = domain
+            if node_name is None and not opts.urn:
+                raise TypeError("Missing required property 'node_name'")
+            __props__.__dict__["node_name"] = node_name
+            __props__.__dict__["servers"] = servers
+        super(DNS, __self__).__init__(
+            'proxmoxve:index/dNS:DNS',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            cidrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterIPSetCidrArgs']]]]] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None) -> 'ClusterIPSet':
+            domain: Optional[pulumi.Input[str]] = None,
+            node_name: Optional[pulumi.Input[str]] = None,
+            servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'DNS':
         """
-        Get an existing ClusterIPSet resource's state with the given name, id, and optional extra
+        Get an existing DNS resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterIPSetCidrArgs']]]] cidrs: List of IP or Networks
-        :param pulumi.Input[str] comment: IPSet comment
-        :param pulumi.Input[str] name: IPSet name
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ClusterIPSetState.__new__(_ClusterIPSetState)
+        __props__ = _DNSState.__new__(_DNSState)
 
-        __props__.__dict__["cidrs"] = cidrs
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["name"] = name
-        return ClusterIPSet(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["domain"] = domain
+        __props__.__dict__["node_name"] = node_name
+        __props__.__dict__["servers"] = servers
+        return DNS(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def cidrs(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterIPSetCidr']]]:
+    def domain(self) -> pulumi.Output[str]:
         """
-        List of IP or Networks
+        The DNS search domain
         """
-        return pulumi.get(self, "cidrs")
+        return pulumi.get(self, "domain")
 
     @property
-    @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Output[str]:
         """
-        IPSet comment
+        The node name
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "node_name")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def servers(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        IPSet name
+        The DNS servers
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "servers")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_cluster_alias.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,92 +6,70 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetClusterAliasResult',
-    'AwaitableGetClusterAliasResult',
-    'get_cluster_alias',
-    'get_cluster_alias_output',
+    'GetGroupsResult',
+    'AwaitableGetGroupsResult',
+    'get_groups',
 ]
 
 @pulumi.output_type
-class GetClusterAliasResult:
+class GetGroupsResult:
     """
-    A collection of values returned by getClusterAlias.
+    A collection of values returned by getGroups.
     """
-    def __init__(__self__, cidr=None, comment=None, id=None, name=None):
-        if cidr and not isinstance(cidr, str):
-            raise TypeError("Expected argument 'cidr' to be a str")
-        pulumi.set(__self__, "cidr", cidr)
-        if comment and not isinstance(comment, str):
-            raise TypeError("Expected argument 'comment' to be a str")
-        pulumi.set(__self__, "comment", comment)
+    def __init__(__self__, comments=None, group_ids=None, id=None):
+        if comments and not isinstance(comments, list):
+            raise TypeError("Expected argument 'comments' to be a list")
+        pulumi.set(__self__, "comments", comments)
+        if group_ids and not isinstance(group_ids, list):
+            raise TypeError("Expected argument 'group_ids' to be a list")
+        pulumi.set(__self__, "group_ids", group_ids)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def cidr(self) -> str:
-        return pulumi.get(self, "cidr")
+    def comments(self) -> Sequence[str]:
+        return pulumi.get(self, "comments")
 
     @property
-    @pulumi.getter
-    def comment(self) -> str:
-        return pulumi.get(self, "comment")
+    @pulumi.getter(name="groupIds")
+    def group_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "group_ids")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
 
-
-class AwaitableGetClusterAliasResult(GetClusterAliasResult):
+class AwaitableGetGroupsResult(GetGroupsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetClusterAliasResult(
-            cidr=self.cidr,
-            comment=self.comment,
-            id=self.id,
-            name=self.name)
+        return GetGroupsResult(
+            comments=self.comments,
+            group_ids=self.group_ids,
+            id=self.id)
 
 
-def get_cluster_alias(name: Optional[str] = None,
-                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClusterAliasResult:
+def get_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:Cluster/getClusterAlias:getClusterAlias', __args__, opts=opts, typ=GetClusterAliasResult).value
-
-    return AwaitableGetClusterAliasResult(
-        cidr=__ret__.cidr,
-        comment=__ret__.comment,
-        id=__ret__.id,
-        name=__ret__.name)
+    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
-
-@_utilities.lift_output_func(get_cluster_alias)
-def get_cluster_alias_output(name: Optional[pulumi.Input[str]] = None,
-                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterAliasResult]:
-    """
-    Use this data source to access information about an existing resource.
-    """
-    ...
+    return AwaitableGetGroupsResult(
+        comments=__ret__.comments,
+        group_ids=__ret__.group_ids,
+        id=__ret__.id)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_cluster_aliases.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_dns.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,63 +3,95 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
 __all__ = [
-    'GetClusterAliasesResult',
-    'AwaitableGetClusterAliasesResult',
-    'get_cluster_aliases',
+    'GetDNSResult',
+    'AwaitableGetDNSResult',
+    'get_dns',
+    'get_dns_output',
 ]
 
 @pulumi.output_type
-class GetClusterAliasesResult:
+class GetDNSResult:
     """
-    A collection of values returned by getClusterAliases.
+    A collection of values returned by getDNS.
     """
-    def __init__(__self__, alias_ids=None, id=None):
-        if alias_ids and not isinstance(alias_ids, list):
-            raise TypeError("Expected argument 'alias_ids' to be a list")
-        pulumi.set(__self__, "alias_ids", alias_ids)
+    def __init__(__self__, domain=None, id=None, node_name=None, servers=None):
+        if domain and not isinstance(domain, str):
+            raise TypeError("Expected argument 'domain' to be a str")
+        pulumi.set(__self__, "domain", domain)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if node_name and not isinstance(node_name, str):
+            raise TypeError("Expected argument 'node_name' to be a str")
+        pulumi.set(__self__, "node_name", node_name)
+        if servers and not isinstance(servers, list):
+            raise TypeError("Expected argument 'servers' to be a list")
+        pulumi.set(__self__, "servers", servers)
 
     @property
-    @pulumi.getter(name="aliasIds")
-    def alias_ids(self) -> Sequence[str]:
-        return pulumi.get(self, "alias_ids")
+    @pulumi.getter
+    def domain(self) -> str:
+        return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
+    @property
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> str:
+        return pulumi.get(self, "node_name")
+
+    @property
+    @pulumi.getter
+    def servers(self) -> Sequence[str]:
+        return pulumi.get(self, "servers")
+
 
-class AwaitableGetClusterAliasesResult(GetClusterAliasesResult):
+class AwaitableGetDNSResult(GetDNSResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetClusterAliasesResult(
-            alias_ids=self.alias_ids,
-            id=self.id)
+        return GetDNSResult(
+            domain=self.domain,
+            id=self.id,
+            node_name=self.node_name,
+            servers=self.servers)
 
 
-def get_cluster_aliases(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClusterAliasesResult:
+def get_dns(node_name: Optional[str] = None,
+            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDNSResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
+    __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:Cluster/getClusterAliases:getClusterAliases', __args__, opts=opts, typ=GetClusterAliasesResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:index/getDNS:getDNS', __args__, opts=opts, typ=GetDNSResult).value
 
-    return AwaitableGetClusterAliasesResult(
-        alias_ids=__ret__.alias_ids,
-        id=__ret__.id)
+    return AwaitableGetDNSResult(
+        domain=__ret__.domain,
+        id=__ret__.id,
+        node_name=__ret__.node_name,
+        servers=__ret__.servers)
+
+
+@_utilities.lift_output_func(get_dns)
+def get_dns_output(node_name: Optional[pulumi.Input[str]] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSResult]:
+    """
+    Use this data source to access information about an existing resource.
+    """
+    ...
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/config/vars.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,57 +4,54 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 
-__all__ = [
-    'VirtualEnvironment',
-]
-
-@pulumi.output_type
-class VirtualEnvironment(dict):
-    def __init__(__self__, *,
-                 endpoint: Optional[str] = None,
-                 insecure: Optional[bool] = None,
-                 otp: Optional[str] = None,
-                 password: Optional[str] = None,
-                 username: Optional[str] = None):
-        if endpoint is not None:
-            pulumi.set(__self__, "endpoint", endpoint)
-        if insecure is not None:
-            pulumi.set(__self__, "insecure", insecure)
-        if otp is not None:
-            pulumi.set(__self__, "otp", otp)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+import types
 
+__config__ = pulumi.Config('proxmoxve')
+
+
+class _ExportableConfig(types.ModuleType):
     @property
-    @pulumi.getter
     def endpoint(self) -> Optional[str]:
-        return pulumi.get(self, "endpoint")
+        """
+        The endpoint for the Proxmox Virtual Environment API
+        """
+        return __config__.get('endpoint')
 
     @property
-    @pulumi.getter
     def insecure(self) -> Optional[bool]:
-        return pulumi.get(self, "insecure")
+        """
+        Whether to skip the TLS verification step
+        """
+        return __config__.get_bool('insecure')
 
     @property
-    @pulumi.getter
     def otp(self) -> Optional[str]:
-        return pulumi.get(self, "otp")
+        """
+        The one-time password for the Proxmox Virtual Environment API
+        """
+        return __config__.get('otp')
 
     @property
-    @pulumi.getter
     def password(self) -> Optional[str]:
-        return pulumi.get(self, "password")
+        """
+        The password for the Proxmox Virtual Environment API
+        """
+        return __config__.get('password')
 
     @property
-    @pulumi.getter
     def username(self) -> Optional[str]:
-        return pulumi.get(self, "username")
+        """
+        The username for the Proxmox Virtual Environment API
+        """
+        return __config__.get('username')
 
+    @property
+    def virtual_environment(self) -> Optional[str]:
+        return __config__.get('virtualEnvironment')
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,23 +423,26 @@
 
 @pulumi.input_type
 class ContainerNetworkInterfaceArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  bridge: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 firewall: Optional[pulumi.Input[bool]] = None,
                  mac_address: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  rate_limit: Optional[pulumi.Input[float]] = None,
                  vlan_id: Optional[pulumi.Input[int]] = None):
         pulumi.set(__self__, "name", name)
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if firewall is not None:
+            pulumi.set(__self__, "firewall", firewall)
         if mac_address is not None:
             pulumi.set(__self__, "mac_address", mac_address)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if rate_limit is not None:
             pulumi.set(__self__, "rate_limit", rate_limit)
         if vlan_id is not None:
@@ -469,14 +472,23 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
+    @pulumi.getter
+    def firewall(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "firewall")
+
+    @firewall.setter
+    def firewall(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "firewall", value)
+
+    @property
     @pulumi.getter(name="macAddress")
     def mac_address(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "mac_address")
 
     @mac_address.setter
     def mac_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mac_address", value)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,23 +407,26 @@
         ContainerNetworkInterface.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  bridge: Optional[str] = None,
                  enabled: Optional[bool] = None,
+                 firewall: Optional[bool] = None,
                  mac_address: Optional[str] = None,
                  mtu: Optional[int] = None,
                  rate_limit: Optional[float] = None,
                  vlan_id: Optional[int] = None):
         pulumi.set(__self__, "name", name)
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if firewall is not None:
+            pulumi.set(__self__, "firewall", firewall)
         if mac_address is not None:
             pulumi.set(__self__, "mac_address", mac_address)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if rate_limit is not None:
             pulumi.set(__self__, "rate_limit", rate_limit)
         if vlan_id is not None:
@@ -441,14 +444,19 @@
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         return pulumi.get(self, "enabled")
 
     @property
+    @pulumi.getter
+    def firewall(self) -> Optional[bool]:
+        return pulumi.get(self, "firewall")
+
+    @property
     @pulumi.getter(name="macAddress")
     def mac_address(self) -> Optional[str]:
         return pulumi.get(self, "mac_address")
 
     @property
     @pulumi.getter
     def mtu(self) -> Optional[int]:
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/role.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,237 +3,190 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
-__all__ = ['DNSArgs', 'DNS']
+__all__ = ['RoleArgs', 'Role']
 
 @pulumi.input_type
-class DNSArgs:
+class RoleArgs:
     def __init__(__self__, *,
-                 domain: pulumi.Input[str],
-                 node_name: pulumi.Input[str],
-                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        The set of arguments for constructing a DNS resource.
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] node_name: The node name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
-        """
-        pulumi.set(__self__, "domain", domain)
-        pulumi.set(__self__, "node_name", node_name)
-        if servers is not None:
-            pulumi.set(__self__, "servers", servers)
-
-    @property
-    @pulumi.getter
-    def domain(self) -> pulumi.Input[str]:
+                 privileges: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 role_id: pulumi.Input[str]):
         """
-        The DNS search domain
+        The set of arguments for constructing a Role resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] privileges: The role privileges
+        :param pulumi.Input[str] role_id: The role id
         """
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: pulumi.Input[str]):
-        pulumi.set(self, "domain", value)
+        pulumi.set(__self__, "privileges", privileges)
+        pulumi.set(__self__, "role_id", role_id)
 
     @property
-    @pulumi.getter(name="nodeName")
-    def node_name(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def privileges(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        The node name
+        The role privileges
         """
-        return pulumi.get(self, "node_name")
+        return pulumi.get(self, "privileges")
 
-    @node_name.setter
-    def node_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "node_name", value)
+    @privileges.setter
+    def privileges(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "privileges", value)
 
     @property
-    @pulumi.getter
-    def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> pulumi.Input[str]:
         """
-        The DNS servers
+        The role id
         """
-        return pulumi.get(self, "servers")
+        return pulumi.get(self, "role_id")
 
-    @servers.setter
-    def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "servers", value)
+    @role_id.setter
+    def role_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "role_id", value)
 
 
 @pulumi.input_type
-class _DNSState:
+class _RoleState:
     def __init__(__self__, *,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 node_name: Optional[pulumi.Input[str]] = None,
-                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        Input properties used for looking up and filtering DNS resources.
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] node_name: The node name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
-        """
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if node_name is not None:
-            pulumi.set(__self__, "node_name", node_name)
-        if servers is not None:
-            pulumi.set(__self__, "servers", servers)
-
-    @property
-    @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
+                 privileges: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 role_id: Optional[pulumi.Input[str]] = None):
         """
-        The DNS search domain
+        Input properties used for looking up and filtering Role resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] privileges: The role privileges
+        :param pulumi.Input[str] role_id: The role id
         """
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
+        if privileges is not None:
+            pulumi.set(__self__, "privileges", privileges)
+        if role_id is not None:
+            pulumi.set(__self__, "role_id", role_id)
 
     @property
-    @pulumi.getter(name="nodeName")
-    def node_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def privileges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The node name
+        The role privileges
         """
-        return pulumi.get(self, "node_name")
+        return pulumi.get(self, "privileges")
 
-    @node_name.setter
-    def node_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "node_name", value)
+    @privileges.setter
+    def privileges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "privileges", value)
 
     @property
-    @pulumi.getter
-    def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS servers
+        The role id
         """
-        return pulumi.get(self, "servers")
+        return pulumi.get(self, "role_id")
 
-    @servers.setter
-    def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "servers", value)
+    @role_id.setter
+    def role_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role_id", value)
 
 
-class DNS(pulumi.CustomResource):
+class Role(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 node_name: Optional[pulumi.Input[str]] = None,
-                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 privileges: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a DNS resource with the given unique name, props, and options.
+        Create a Role resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] node_name: The node name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] privileges: The role privileges
+        :param pulumi.Input[str] role_id: The role id
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DNSArgs,
+                 args: RoleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DNS resource with the given unique name, props, and options.
+        Create a Role resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param DNSArgs args: The arguments to use to populate this resource's properties.
+        :param RoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DNSArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RoleArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 node_name: Optional[pulumi.Input[str]] = None,
-                 servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 privileges: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DNSArgs.__new__(DNSArgs)
+            __props__ = RoleArgs.__new__(RoleArgs)
 
-            if domain is None and not opts.urn:
-                raise TypeError("Missing required property 'domain'")
-            __props__.__dict__["domain"] = domain
-            if node_name is None and not opts.urn:
-                raise TypeError("Missing required property 'node_name'")
-            __props__.__dict__["node_name"] = node_name
-            __props__.__dict__["servers"] = servers
-        super(DNS, __self__).__init__(
-            'proxmoxve:index/dNS:DNS',
+            if privileges is None and not opts.urn:
+                raise TypeError("Missing required property 'privileges'")
+            __props__.__dict__["privileges"] = privileges
+            if role_id is None and not opts.urn:
+                raise TypeError("Missing required property 'role_id'")
+            __props__.__dict__["role_id"] = role_id
+        super(Role, __self__).__init__(
+            'proxmoxve:Permission/role:Role',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            domain: Optional[pulumi.Input[str]] = None,
-            node_name: Optional[pulumi.Input[str]] = None,
-            servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'DNS':
+            privileges: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            role_id: Optional[pulumi.Input[str]] = None) -> 'Role':
         """
-        Get an existing DNS resource's state with the given name, id, and optional extra
+        Get an existing Role resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] node_name: The node name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The DNS servers
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] privileges: The role privileges
+        :param pulumi.Input[str] role_id: The role id
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DNSState.__new__(_DNSState)
+        __props__ = _RoleState.__new__(_RoleState)
 
-        __props__.__dict__["domain"] = domain
-        __props__.__dict__["node_name"] = node_name
-        __props__.__dict__["servers"] = servers
-        return DNS(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["privileges"] = privileges
+        __props__.__dict__["role_id"] = role_id
+        return Role(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def domain(self) -> pulumi.Output[str]:
-        """
-        The DNS search domain
+    def privileges(self) -> pulumi.Output[Sequence[str]]:
         """
-        return pulumi.get(self, "domain")
-
-    @property
-    @pulumi.getter(name="nodeName")
-    def node_name(self) -> pulumi.Output[str]:
+        The role privileges
         """
-        The node name
-        """
-        return pulumi.get(self, "node_name")
+        return pulumi.get(self, "privileges")
 
     @property
-    @pulumi.getter
-    def servers(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> pulumi.Output[str]:
         """
-        The DNS servers
+        The role id
         """
-        return pulumi.get(self, "servers")
+        return pulumi.get(self, "role_id")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,95 +3,96 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
+from . import outputs
 
 __all__ = [
-    'GetDNSResult',
-    'AwaitableGetDNSResult',
-    'get_dns',
-    'get_dns_output',
+    'GetPoolResult',
+    'AwaitableGetPoolResult',
+    'get_pool',
+    'get_pool_output',
 ]
 
 @pulumi.output_type
-class GetDNSResult:
+class GetPoolResult:
     """
-    A collection of values returned by getDNS.
+    A collection of values returned by getPool.
     """
-    def __init__(__self__, domain=None, id=None, node_name=None, servers=None):
-        if domain and not isinstance(domain, str):
-            raise TypeError("Expected argument 'domain' to be a str")
-        pulumi.set(__self__, "domain", domain)
+    def __init__(__self__, comment=None, id=None, members=None, pool_id=None):
+        if comment and not isinstance(comment, str):
+            raise TypeError("Expected argument 'comment' to be a str")
+        pulumi.set(__self__, "comment", comment)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if node_name and not isinstance(node_name, str):
-            raise TypeError("Expected argument 'node_name' to be a str")
-        pulumi.set(__self__, "node_name", node_name)
-        if servers and not isinstance(servers, list):
-            raise TypeError("Expected argument 'servers' to be a list")
-        pulumi.set(__self__, "servers", servers)
+        if members and not isinstance(members, list):
+            raise TypeError("Expected argument 'members' to be a list")
+        pulumi.set(__self__, "members", members)
+        if pool_id and not isinstance(pool_id, str):
+            raise TypeError("Expected argument 'pool_id' to be a str")
+        pulumi.set(__self__, "pool_id", pool_id)
 
     @property
     @pulumi.getter
-    def domain(self) -> str:
-        return pulumi.get(self, "domain")
+    def comment(self) -> str:
+        return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="nodeName")
-    def node_name(self) -> str:
-        return pulumi.get(self, "node_name")
+    @pulumi.getter
+    def members(self) -> Sequence['outputs.GetPoolMemberResult']:
+        return pulumi.get(self, "members")
 
     @property
-    @pulumi.getter
-    def servers(self) -> Sequence[str]:
-        return pulumi.get(self, "servers")
+    @pulumi.getter(name="poolId")
+    def pool_id(self) -> str:
+        return pulumi.get(self, "pool_id")
 
 
-class AwaitableGetDNSResult(GetDNSResult):
+class AwaitableGetPoolResult(GetPoolResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetDNSResult(
-            domain=self.domain,
+        return GetPoolResult(
+            comment=self.comment,
             id=self.id,
-            node_name=self.node_name,
-            servers=self.servers)
+            members=self.members,
+            pool_id=self.pool_id)
 
 
-def get_dns(node_name: Optional[str] = None,
-            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDNSResult:
+def get_pool(pool_id: Optional[str] = None,
+             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['nodeName'] = node_name
+    __args__['poolId'] = pool_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:index/getDNS:getDNS', __args__, opts=opts, typ=GetDNSResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPool:getPool', __args__, opts=opts, typ=GetPoolResult).value
 
-    return AwaitableGetDNSResult(
-        domain=__ret__.domain,
+    return AwaitableGetPoolResult(
+        comment=__ret__.comment,
         id=__ret__.id,
-        node_name=__ret__.node_name,
-        servers=__ret__.servers)
+        members=__ret__.members,
+        pool_id=__ret__.pool_id)
 
 
-@_utilities.lift_output_func(get_dns)
-def get_dns_output(node_name: Optional[pulumi.Input[str]] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSResult]:
+@_utilities.lift_output_func(get_pool)
+def get_pool_output(pool_id: Optional[pulumi.Input[str]] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,70 +6,60 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetGroupsResult',
-    'AwaitableGetGroupsResult',
-    'get_groups',
+    'GetPoolsResult',
+    'AwaitableGetPoolsResult',
+    'get_pools',
 ]
 
 @pulumi.output_type
-class GetGroupsResult:
+class GetPoolsResult:
     """
-    A collection of values returned by getGroups.
+    A collection of values returned by getPools.
     """
-    def __init__(__self__, comments=None, group_ids=None, id=None):
-        if comments and not isinstance(comments, list):
-            raise TypeError("Expected argument 'comments' to be a list")
-        pulumi.set(__self__, "comments", comments)
-        if group_ids and not isinstance(group_ids, list):
-            raise TypeError("Expected argument 'group_ids' to be a list")
-        pulumi.set(__self__, "group_ids", group_ids)
+    def __init__(__self__, id=None, pool_ids=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-
-    @property
-    @pulumi.getter
-    def comments(self) -> Sequence[str]:
-        return pulumi.get(self, "comments")
-
-    @property
-    @pulumi.getter(name="groupIds")
-    def group_ids(self) -> Sequence[str]:
-        return pulumi.get(self, "group_ids")
+        if pool_ids and not isinstance(pool_ids, list):
+            raise TypeError("Expected argument 'pool_ids' to be a list")
+        pulumi.set(__self__, "pool_ids", pool_ids)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
+    @property
+    @pulumi.getter(name="poolIds")
+    def pool_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "pool_ids")
+
 
-class AwaitableGetGroupsResult(GetGroupsResult):
+class AwaitableGetPoolsResult(GetPoolsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetGroupsResult(
-            comments=self.comments,
-            group_ids=self.group_ids,
-            id=self.id)
+        return GetPoolsResult(
+            id=self.id,
+            pool_ids=self.pool_ids)
 
 
-def get_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
+def get_pools(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPools:getPools', __args__, opts=opts, typ=GetPoolsResult).value
 
-    return AwaitableGetGroupsResult(
-        comments=__ret__.comments,
-        group_ids=__ret__.group_ids,
-        id=__ret__.id)
+    return AwaitableGetPoolsResult(
+        id=__ret__.id,
+        pool_ids=__ret__.pool_ids)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,95 +4,107 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 
 __all__ = [
-    'GetPoolResult',
-    'AwaitableGetPoolResult',
-    'get_pool',
-    'get_pool_output',
+    'GetVirtualMachineResult',
+    'AwaitableGetVirtualMachineResult',
+    'get_virtual_machine',
+    'get_virtual_machine_output',
 ]
 
 @pulumi.output_type
-class GetPoolResult:
+class GetVirtualMachineResult:
     """
-    A collection of values returned by getPool.
+    A collection of values returned by getVirtualMachine.
     """
-    def __init__(__self__, comment=None, id=None, members=None, pool_id=None):
-        if comment and not isinstance(comment, str):
-            raise TypeError("Expected argument 'comment' to be a str")
-        pulumi.set(__self__, "comment", comment)
+    def __init__(__self__, id=None, name=None, node_name=None, tags=None, vm_id=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if members and not isinstance(members, list):
-            raise TypeError("Expected argument 'members' to be a list")
-        pulumi.set(__self__, "members", members)
-        if pool_id and not isinstance(pool_id, str):
-            raise TypeError("Expected argument 'pool_id' to be a str")
-        pulumi.set(__self__, "pool_id", pool_id)
-
-    @property
-    @pulumi.getter
-    def comment(self) -> str:
-        return pulumi.get(self, "comment")
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if node_name and not isinstance(node_name, str):
+            raise TypeError("Expected argument 'node_name' to be a str")
+        pulumi.set(__self__, "node_name", node_name)
+        if tags and not isinstance(tags, list):
+            raise TypeError("Expected argument 'tags' to be a list")
+        pulumi.set(__self__, "tags", tags)
+        if vm_id and not isinstance(vm_id, int):
+            raise TypeError("Expected argument 'vm_id' to be a int")
+        pulumi.set(__self__, "vm_id", vm_id)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def members(self) -> Sequence['outputs.GetPoolMemberResult']:
-        return pulumi.get(self, "members")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> str:
+        return pulumi.get(self, "node_name")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Sequence[str]:
+        return pulumi.get(self, "tags")
 
     @property
-    @pulumi.getter(name="poolId")
-    def pool_id(self) -> str:
-        return pulumi.get(self, "pool_id")
+    @pulumi.getter(name="vmId")
+    def vm_id(self) -> int:
+        return pulumi.get(self, "vm_id")
 
 
-class AwaitableGetPoolResult(GetPoolResult):
+class AwaitableGetVirtualMachineResult(GetVirtualMachineResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPoolResult(
-            comment=self.comment,
+        return GetVirtualMachineResult(
             id=self.id,
-            members=self.members,
-            pool_id=self.pool_id)
+            name=self.name,
+            node_name=self.node_name,
+            tags=self.tags,
+            vm_id=self.vm_id)
 
 
-def get_pool(pool_id: Optional[str] = None,
-             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolResult:
+def get_virtual_machine(node_name: Optional[str] = None,
+                        vm_id: Optional[int] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualMachineResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['poolId'] = pool_id
+    __args__['nodeName'] = node_name
+    __args__['vmId'] = vm_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPool:getPool', __args__, opts=opts, typ=GetPoolResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:VM/getVirtualMachine:getVirtualMachine', __args__, opts=opts, typ=GetVirtualMachineResult).value
 
-    return AwaitableGetPoolResult(
-        comment=__ret__.comment,
+    return AwaitableGetVirtualMachineResult(
         id=__ret__.id,
-        members=__ret__.members,
-        pool_id=__ret__.pool_id)
+        name=__ret__.name,
+        node_name=__ret__.node_name,
+        tags=__ret__.tags,
+        vm_id=__ret__.vm_id)
 
 
-@_utilities.lift_output_func(get_pool)
-def get_pool_output(pool_id: Optional[pulumi.Input[str]] = None,
-                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolResult]:
+@_utilities.lift_output_func(get_virtual_machine)
+def get_virtual_machine_output(node_name: Optional[pulumi.Input[str]] = None,
+                               vm_id: Optional[pulumi.Input[int]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachineResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,60 +6,80 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetPoolsResult',
-    'AwaitableGetPoolsResult',
-    'get_pools',
+    'GetRolesResult',
+    'AwaitableGetRolesResult',
+    'get_roles',
 ]
 
 @pulumi.output_type
-class GetPoolsResult:
+class GetRolesResult:
     """
-    A collection of values returned by getPools.
+    A collection of values returned by getRoles.
     """
-    def __init__(__self__, id=None, pool_ids=None):
+    def __init__(__self__, id=None, privileges=None, role_ids=None, specials=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if pool_ids and not isinstance(pool_ids, list):
-            raise TypeError("Expected argument 'pool_ids' to be a list")
-        pulumi.set(__self__, "pool_ids", pool_ids)
+        if privileges and not isinstance(privileges, list):
+            raise TypeError("Expected argument 'privileges' to be a list")
+        pulumi.set(__self__, "privileges", privileges)
+        if role_ids and not isinstance(role_ids, list):
+            raise TypeError("Expected argument 'role_ids' to be a list")
+        pulumi.set(__self__, "role_ids", role_ids)
+        if specials and not isinstance(specials, list):
+            raise TypeError("Expected argument 'specials' to be a list")
+        pulumi.set(__self__, "specials", specials)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="poolIds")
-    def pool_ids(self) -> Sequence[str]:
-        return pulumi.get(self, "pool_ids")
+    @pulumi.getter
+    def privileges(self) -> Sequence[Sequence[str]]:
+        return pulumi.get(self, "privileges")
+
+    @property
+    @pulumi.getter(name="roleIds")
+    def role_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "role_ids")
+
+    @property
+    @pulumi.getter
+    def specials(self) -> Sequence[bool]:
+        return pulumi.get(self, "specials")
 
 
-class AwaitableGetPoolsResult(GetPoolsResult):
+class AwaitableGetRolesResult(GetRolesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPoolsResult(
+        return GetRolesResult(
             id=self.id,
-            pool_ids=self.pool_ids)
+            privileges=self.privileges,
+            role_ids=self.role_ids,
+            specials=self.specials)
 
 
-def get_pools(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolsResult:
+def get_roles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRolesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPools:getPools', __args__, opts=opts, typ=GetPoolsResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
 
-    return AwaitableGetPoolsResult(
+    return AwaitableGetRolesResult(
         id=__ret__.id,
-        pool_ids=__ret__.pool_ids)
+        privileges=__ret__.privileges,
+        role_ids=__ret__.role_ids,
+        specials=__ret__.specials)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,219 +3,246 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
-from . import outputs
-from ._inputs import *
+from . import _utilities
 
-__all__ = ['PoolArgs', 'Pool']
+__all__ = ['TimeArgs', 'Time']
 
 @pulumi.input_type
-class PoolArgs:
+class TimeArgs:
     def __init__(__self__, *,
-                 pool_id: pulumi.Input[str],
-                 comment: Optional[pulumi.Input[str]] = None):
+                 node_name: pulumi.Input[str],
+                 time_zone: pulumi.Input[str]):
         """
-        The set of arguments for constructing a Pool resource.
-        :param pulumi.Input[str] pool_id: The pool id
-        :param pulumi.Input[str] comment: The pool comment
+        The set of arguments for constructing a Time resource.
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[str] time_zone: The time zone
         """
-        pulumi.set(__self__, "pool_id", pool_id)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
+        pulumi.set(__self__, "node_name", node_name)
+        pulumi.set(__self__, "time_zone", time_zone)
 
     @property
-    @pulumi.getter(name="poolId")
-    def pool_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Input[str]:
         """
-        The pool id
+        The node name
         """
-        return pulumi.get(self, "pool_id")
+        return pulumi.get(self, "node_name")
 
-    @pool_id.setter
-    def pool_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "pool_id", value)
+    @node_name.setter
+    def node_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "node_name", value)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="timeZone")
+    def time_zone(self) -> pulumi.Input[str]:
         """
-        The pool comment
+        The time zone
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "time_zone")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @time_zone.setter
+    def time_zone(self, value: pulumi.Input[str]):
+        pulumi.set(self, "time_zone", value)
 
 
 @pulumi.input_type
-class _PoolState:
+class _TimeState:
     def __init__(__self__, *,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 members: Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]] = None,
-                 pool_id: Optional[pulumi.Input[str]] = None):
+                 local_time: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 time_zone: Optional[pulumi.Input[str]] = None,
+                 utc_time: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Pool resources.
-        :param pulumi.Input[str] comment: The pool comment
-        :param pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]] members: The pool members
-        :param pulumi.Input[str] pool_id: The pool id
+        Input properties used for looking up and filtering Time resources.
+        :param pulumi.Input[str] local_time: The local timestamp
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[str] time_zone: The time zone
+        :param pulumi.Input[str] utc_time: The UTC timestamp
         """
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if members is not None:
-            pulumi.set(__self__, "members", members)
-        if pool_id is not None:
-            pulumi.set(__self__, "pool_id", pool_id)
+        if local_time is not None:
+            pulumi.set(__self__, "local_time", local_time)
+        if node_name is not None:
+            pulumi.set(__self__, "node_name", node_name)
+        if time_zone is not None:
+            pulumi.set(__self__, "time_zone", time_zone)
+        if utc_time is not None:
+            pulumi.set(__self__, "utc_time", utc_time)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="localTime")
+    def local_time(self) -> Optional[pulumi.Input[str]]:
         """
-        The pool comment
+        The local timestamp
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "local_time")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @local_time.setter
+    def local_time(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "local_time", value)
 
     @property
-    @pulumi.getter
-    def members(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The pool members
+        The node name
         """
-        return pulumi.get(self, "members")
+        return pulumi.get(self, "node_name")
 
-    @members.setter
-    def members(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PoolMemberArgs']]]]):
-        pulumi.set(self, "members", value)
+    @node_name.setter
+    def node_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "node_name", value)
 
     @property
-    @pulumi.getter(name="poolId")
-    def pool_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="timeZone")
+    def time_zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The pool id
+        The time zone
         """
-        return pulumi.get(self, "pool_id")
+        return pulumi.get(self, "time_zone")
 
-    @pool_id.setter
-    def pool_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pool_id", value)
+    @time_zone.setter
+    def time_zone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "time_zone", value)
+
+    @property
+    @pulumi.getter(name="utcTime")
+    def utc_time(self) -> Optional[pulumi.Input[str]]:
+        """
+        The UTC timestamp
+        """
+        return pulumi.get(self, "utc_time")
+
+    @utc_time.setter
+    def utc_time(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "utc_time", value)
 
 
-class Pool(pulumi.CustomResource):
+class Time(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 pool_id: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 time_zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Pool resource with the given unique name, props, and options.
+        Create a Time resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The pool comment
-        :param pulumi.Input[str] pool_id: The pool id
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[str] time_zone: The time zone
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PoolArgs,
+                 args: TimeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Pool resource with the given unique name, props, and options.
+        Create a Time resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param PoolArgs args: The arguments to use to populate this resource's properties.
+        :param TimeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(PoolArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TimeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 pool_id: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 time_zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = PoolArgs.__new__(PoolArgs)
+            __props__ = TimeArgs.__new__(TimeArgs)
 
-            __props__.__dict__["comment"] = comment
-            if pool_id is None and not opts.urn:
-                raise TypeError("Missing required property 'pool_id'")
-            __props__.__dict__["pool_id"] = pool_id
-            __props__.__dict__["members"] = None
-        super(Pool, __self__).__init__(
-            'proxmoxve:Permission/pool:Pool',
+            if node_name is None and not opts.urn:
+                raise TypeError("Missing required property 'node_name'")
+            __props__.__dict__["node_name"] = node_name
+            if time_zone is None and not opts.urn:
+                raise TypeError("Missing required property 'time_zone'")
+            __props__.__dict__["time_zone"] = time_zone
+            __props__.__dict__["local_time"] = None
+            __props__.__dict__["utc_time"] = None
+        super(Time, __self__).__init__(
+            'proxmoxve:index/time:Time',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            members: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PoolMemberArgs']]]]] = None,
-            pool_id: Optional[pulumi.Input[str]] = None) -> 'Pool':
+            local_time: Optional[pulumi.Input[str]] = None,
+            node_name: Optional[pulumi.Input[str]] = None,
+            time_zone: Optional[pulumi.Input[str]] = None,
+            utc_time: Optional[pulumi.Input[str]] = None) -> 'Time':
         """
-        Get an existing Pool resource's state with the given name, id, and optional extra
+        Get an existing Time resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The pool comment
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PoolMemberArgs']]]] members: The pool members
-        :param pulumi.Input[str] pool_id: The pool id
+        :param pulumi.Input[str] local_time: The local timestamp
+        :param pulumi.Input[str] node_name: The node name
+        :param pulumi.Input[str] time_zone: The time zone
+        :param pulumi.Input[str] utc_time: The UTC timestamp
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _PoolState.__new__(_PoolState)
+        __props__ = _TimeState.__new__(_TimeState)
 
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["members"] = members
-        __props__.__dict__["pool_id"] = pool_id
-        return Pool(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["local_time"] = local_time
+        __props__.__dict__["node_name"] = node_name
+        __props__.__dict__["time_zone"] = time_zone
+        __props__.__dict__["utc_time"] = utc_time
+        return Time(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="localTime")
+    def local_time(self) -> pulumi.Output[str]:
+        """
+        The local timestamp
+        """
+        return pulumi.get(self, "local_time")
 
     @property
-    @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Output[str]:
         """
-        The pool comment
+        The node name
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "node_name")
 
     @property
-    @pulumi.getter
-    def members(self) -> pulumi.Output[Sequence['outputs.PoolMember']]:
+    @pulumi.getter(name="timeZone")
+    def time_zone(self) -> pulumi.Output[str]:
         """
-        The pool members
+        The time zone
         """
-        return pulumi.get(self, "members")
+        return pulumi.get(self, "time_zone")
 
     @property
-    @pulumi.getter(name="poolId")
-    def pool_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="utcTime")
+    def utc_time(self) -> pulumi.Output[str]:
         """
-        The pool id
+        The UTC timestamp
         """
-        return pulumi.get(self, "pool_id")
+        return pulumi.get(self, "utc_time")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,23 +859,26 @@
 
 
 @pulumi.input_type
 class VirtualMachineNetworkDeviceArgs:
     def __init__(__self__, *,
                  bridge: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 firewall: Optional[pulumi.Input[bool]] = None,
                  mac_address: Optional[pulumi.Input[str]] = None,
                  model: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  rate_limit: Optional[pulumi.Input[float]] = None,
                  vlan_id: Optional[pulumi.Input[int]] = None):
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if firewall is not None:
+            pulumi.set(__self__, "firewall", firewall)
         if mac_address is not None:
             pulumi.set(__self__, "mac_address", mac_address)
         if model is not None:
             pulumi.set(__self__, "model", model)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if rate_limit is not None:
@@ -898,14 +901,23 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
+    @pulumi.getter
+    def firewall(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "firewall")
+
+    @firewall.setter
+    def firewall(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "firewall", value)
+
+    @property
     @pulumi.getter(name="macAddress")
     def mac_address(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "mac_address")
 
     @mac_address.setter
     def mac_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mac_address", value)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,107 +4,98 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 
 __all__ = [
-    'GetVirtualMachineResult',
-    'AwaitableGetVirtualMachineResult',
-    'get_virtual_machine',
-    'get_virtual_machine_output',
+    'GetVirtualMachinesResult',
+    'AwaitableGetVirtualMachinesResult',
+    'get_virtual_machines',
+    'get_virtual_machines_output',
 ]
 
 @pulumi.output_type
-class GetVirtualMachineResult:
+class GetVirtualMachinesResult:
     """
-    A collection of values returned by getVirtualMachine.
+    A collection of values returned by getVirtualMachines.
     """
-    def __init__(__self__, id=None, name=None, node_name=None, tags=None, vm_id=None):
+    def __init__(__self__, id=None, node_name=None, tags=None, vms=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
         if node_name and not isinstance(node_name, str):
             raise TypeError("Expected argument 'node_name' to be a str")
         pulumi.set(__self__, "node_name", node_name)
         if tags and not isinstance(tags, list):
             raise TypeError("Expected argument 'tags' to be a list")
         pulumi.set(__self__, "tags", tags)
-        if vm_id and not isinstance(vm_id, int):
-            raise TypeError("Expected argument 'vm_id' to be a int")
-        pulumi.set(__self__, "vm_id", vm_id)
+        if vms and not isinstance(vms, list):
+            raise TypeError("Expected argument 'vms' to be a list")
+        pulumi.set(__self__, "vms", vms)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
     @pulumi.getter(name="nodeName")
-    def node_name(self) -> str:
+    def node_name(self) -> Optional[str]:
         return pulumi.get(self, "node_name")
 
     @property
     @pulumi.getter
-    def tags(self) -> Sequence[str]:
+    def tags(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "tags")
 
     @property
-    @pulumi.getter(name="vmId")
-    def vm_id(self) -> int:
-        return pulumi.get(self, "vm_id")
+    @pulumi.getter
+    def vms(self) -> Sequence['outputs.GetVirtualMachinesVmResult']:
+        return pulumi.get(self, "vms")
 
 
-class AwaitableGetVirtualMachineResult(GetVirtualMachineResult):
+class AwaitableGetVirtualMachinesResult(GetVirtualMachinesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetVirtualMachineResult(
+        return GetVirtualMachinesResult(
             id=self.id,
-            name=self.name,
             node_name=self.node_name,
             tags=self.tags,
-            vm_id=self.vm_id)
+            vms=self.vms)
 
 
-def get_virtual_machine(node_name: Optional[str] = None,
-                        vm_id: Optional[int] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualMachineResult:
+def get_virtual_machines(node_name: Optional[str] = None,
+                         tags: Optional[Sequence[str]] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualMachinesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
-    __args__['vmId'] = vm_id
+    __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:VM/getVirtualMachine:getVirtualMachine', __args__, opts=opts, typ=GetVirtualMachineResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:VM/getVirtualMachines:getVirtualMachines', __args__, opts=opts, typ=GetVirtualMachinesResult).value
 
-    return AwaitableGetVirtualMachineResult(
+    return AwaitableGetVirtualMachinesResult(
         id=__ret__.id,
-        name=__ret__.name,
         node_name=__ret__.node_name,
         tags=__ret__.tags,
-        vm_id=__ret__.vm_id)
+        vms=__ret__.vms)
 
 
-@_utilities.lift_output_func(get_virtual_machine)
-def get_virtual_machine_output(node_name: Optional[pulumi.Input[str]] = None,
-                               vm_id: Optional[pulumi.Input[int]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachineResult]:
+@_utilities.lift_output_func(get_virtual_machines)
+def get_virtual_machines_output(node_name: Optional[pulumi.Input[Optional[str]]] = None,
+                                tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
+                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachinesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -752,23 +752,26 @@
     def get(self, key: str, default = None) -> Any:
         VirtualMachineNetworkDevice.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bridge: Optional[str] = None,
                  enabled: Optional[bool] = None,
+                 firewall: Optional[bool] = None,
                  mac_address: Optional[str] = None,
                  model: Optional[str] = None,
                  mtu: Optional[int] = None,
                  rate_limit: Optional[float] = None,
                  vlan_id: Optional[int] = None):
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if firewall is not None:
+            pulumi.set(__self__, "firewall", firewall)
         if mac_address is not None:
             pulumi.set(__self__, "mac_address", mac_address)
         if model is not None:
             pulumi.set(__self__, "model", model)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if rate_limit is not None:
@@ -783,14 +786,19 @@
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         return pulumi.get(self, "enabled")
 
     @property
+    @pulumi.getter
+    def firewall(self) -> Optional[bool]:
+        return pulumi.get(self, "firewall")
+
+    @property
     @pulumi.getter(name="macAddress")
     def mac_address(self) -> Optional[str]:
         return pulumi.get(self, "mac_address")
 
     @property
     @pulumi.getter
     def model(self) -> Optional[str]:
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 class VirtualMachineArgs:
     def __init__(__self__, *,
                  node_name: pulumi.Input[str],
                  acpi: Optional[pulumi.Input[bool]] = None,
                  agent: Optional[pulumi.Input['VirtualMachineAgentArgs']] = None,
                  audio_device: Optional[pulumi.Input['VirtualMachineAudioDeviceArgs']] = None,
                  bios: Optional[pulumi.Input[str]] = None,
+                 boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input['VirtualMachineCdromArgs']] = None,
                  clone: Optional[pulumi.Input['VirtualMachineCloneArgs']] = None,
                  cpu: Optional[pulumi.Input['VirtualMachineCpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]] = None,
                  initialization: Optional[pulumi.Input['VirtualMachineInitializationArgs']] = None,
@@ -55,14 +56,15 @@
         """
         The set of arguments for constructing a VirtualMachine resource.
         :param pulumi.Input[str] node_name: The node name
         :param pulumi.Input[bool] acpi: Whether to enable ACPI
         :param pulumi.Input['VirtualMachineAgentArgs'] agent: The QEMU agent configuration
         :param pulumi.Input['VirtualMachineAudioDeviceArgs'] audio_device: The audio devices
         :param pulumi.Input[str] bios: The BIOS implementation
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input['VirtualMachineCdromArgs'] cdrom: The CDROM drive
         :param pulumi.Input['VirtualMachineCloneArgs'] clone: The cloning configuration
         :param pulumi.Input['VirtualMachineCpuArgs'] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: The disk devices
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input['VirtualMachineInitializationArgs'] initialization: The cloud-init configuration
@@ -96,14 +98,16 @@
             pulumi.set(__self__, "acpi", acpi)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if audio_device is not None:
             pulumi.set(__self__, "audio_device", audio_device)
         if bios is not None:
             pulumi.set(__self__, "bios", bios)
+        if boot_orders is not None:
+            pulumi.set(__self__, "boot_orders", boot_orders)
         if cdrom is not None:
             pulumi.set(__self__, "cdrom", cdrom)
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
@@ -220,14 +224,26 @@
         return pulumi.get(self, "bios")
 
     @bios.setter
     def bios(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bios", value)
 
     @property
+    @pulumi.getter(name="bootOrders")
+    def boot_orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The guest will attempt to boot from devices in the order they appear here
+        """
+        return pulumi.get(self, "boot_orders")
+
+    @boot_orders.setter
+    def boot_orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "boot_orders", value)
+
+    @property
     @pulumi.getter
     def cdrom(self) -> Optional[pulumi.Input['VirtualMachineCdromArgs']]:
         """
         The CDROM drive
         """
         return pulumi.get(self, "cdrom")
 
@@ -599,14 +615,15 @@
 @pulumi.input_type
 class _VirtualMachineState:
     def __init__(__self__, *,
                  acpi: Optional[pulumi.Input[bool]] = None,
                  agent: Optional[pulumi.Input['VirtualMachineAgentArgs']] = None,
                  audio_device: Optional[pulumi.Input['VirtualMachineAudioDeviceArgs']] = None,
                  bios: Optional[pulumi.Input[str]] = None,
+                 boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input['VirtualMachineCdromArgs']] = None,
                  clone: Optional[pulumi.Input['VirtualMachineCloneArgs']] = None,
                  cpu: Optional[pulumi.Input['VirtualMachineCpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]] = None,
                  initialization: Optional[pulumi.Input['VirtualMachineInitializationArgs']] = None,
@@ -641,14 +658,15 @@
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering VirtualMachine resources.
         :param pulumi.Input[bool] acpi: Whether to enable ACPI
         :param pulumi.Input['VirtualMachineAgentArgs'] agent: The QEMU agent configuration
         :param pulumi.Input['VirtualMachineAudioDeviceArgs'] audio_device: The audio devices
         :param pulumi.Input[str] bios: The BIOS implementation
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input['VirtualMachineCdromArgs'] cdrom: The CDROM drive
         :param pulumi.Input['VirtualMachineCloneArgs'] clone: The cloning configuration
         :param pulumi.Input['VirtualMachineCpuArgs'] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: The disk devices
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input['VirtualMachineInitializationArgs'] initialization: The cloud-init configuration
@@ -686,14 +704,16 @@
             pulumi.set(__self__, "acpi", acpi)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if audio_device is not None:
             pulumi.set(__self__, "audio_device", audio_device)
         if bios is not None:
             pulumi.set(__self__, "bios", bios)
+        if boot_orders is not None:
+            pulumi.set(__self__, "boot_orders", boot_orders)
         if cdrom is not None:
             pulumi.set(__self__, "cdrom", cdrom)
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
@@ -808,14 +828,26 @@
         return pulumi.get(self, "bios")
 
     @bios.setter
     def bios(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bios", value)
 
     @property
+    @pulumi.getter(name="bootOrders")
+    def boot_orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The guest will attempt to boot from devices in the order they appear here
+        """
+        return pulumi.get(self, "boot_orders")
+
+    @boot_orders.setter
+    def boot_orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "boot_orders", value)
+
+    @property
     @pulumi.getter
     def cdrom(self) -> Optional[pulumi.Input['VirtualMachineCdromArgs']]:
         """
         The CDROM drive
         """
         return pulumi.get(self, "cdrom")
 
@@ -1249,14 +1281,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acpi: Optional[pulumi.Input[bool]] = None,
                  agent: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAgentArgs']]] = None,
                  audio_device: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAudioDeviceArgs']]] = None,
                  bios: Optional[pulumi.Input[str]] = None,
+                 boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
                  clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
                  cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
                  initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
@@ -1290,14 +1323,15 @@
         Create a VirtualMachine resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acpi: Whether to enable ACPI
         :param pulumi.Input[pulumi.InputType['VirtualMachineAgentArgs']] agent: The QEMU agent configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineAudioDeviceArgs']] audio_device: The audio devices
         :param pulumi.Input[str] bios: The BIOS implementation
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']] cdrom: The CDROM drive
         :param pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']] clone: The cloning configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: The disk devices
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']] initialization: The cloud-init configuration
@@ -1350,14 +1384,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acpi: Optional[pulumi.Input[bool]] = None,
                  agent: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAgentArgs']]] = None,
                  audio_device: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAudioDeviceArgs']]] = None,
                  bios: Optional[pulumi.Input[str]] = None,
+                 boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
                  clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
                  cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
                  initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
@@ -1395,14 +1430,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VirtualMachineArgs.__new__(VirtualMachineArgs)
 
             __props__.__dict__["acpi"] = acpi
             __props__.__dict__["agent"] = agent
             __props__.__dict__["audio_device"] = audio_device
             __props__.__dict__["bios"] = bios
+            __props__.__dict__["boot_orders"] = boot_orders
             __props__.__dict__["cdrom"] = cdrom
             __props__.__dict__["clone"] = clone
             __props__.__dict__["cpu"] = cpu
             __props__.__dict__["description"] = description
             __props__.__dict__["disks"] = disks
             __props__.__dict__["hostpcis"] = hostpcis
             __props__.__dict__["initialization"] = initialization
@@ -1447,14 +1483,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             acpi: Optional[pulumi.Input[bool]] = None,
             agent: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAgentArgs']]] = None,
             audio_device: Optional[pulumi.Input[pulumi.InputType['VirtualMachineAudioDeviceArgs']]] = None,
             bios: Optional[pulumi.Input[str]] = None,
+            boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
             clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
             cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
             description: Optional[pulumi.Input[str]] = None,
             disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
             hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
             initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
@@ -1494,14 +1531,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acpi: Whether to enable ACPI
         :param pulumi.Input[pulumi.InputType['VirtualMachineAgentArgs']] agent: The QEMU agent configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineAudioDeviceArgs']] audio_device: The audio devices
         :param pulumi.Input[str] bios: The BIOS implementation
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']] cdrom: The CDROM drive
         :param pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']] clone: The cloning configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: The disk devices
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']] initialization: The cloud-init configuration
@@ -1539,14 +1577,15 @@
 
         __props__ = _VirtualMachineState.__new__(_VirtualMachineState)
 
         __props__.__dict__["acpi"] = acpi
         __props__.__dict__["agent"] = agent
         __props__.__dict__["audio_device"] = audio_device
         __props__.__dict__["bios"] = bios
+        __props__.__dict__["boot_orders"] = boot_orders
         __props__.__dict__["cdrom"] = cdrom
         __props__.__dict__["clone"] = clone
         __props__.__dict__["cpu"] = cpu
         __props__.__dict__["description"] = description
         __props__.__dict__["disks"] = disks
         __props__.__dict__["hostpcis"] = hostpcis
         __props__.__dict__["initialization"] = initialization
@@ -1610,14 +1649,22 @@
     def bios(self) -> pulumi.Output[Optional[str]]:
         """
         The BIOS implementation
         """
         return pulumi.get(self, "bios")
 
     @property
+    @pulumi.getter(name="bootOrders")
+    def boot_orders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        The guest will attempt to boot from devices in the order they appear here
+        """
+        return pulumi.get(self, "boot_orders")
+
+    @property
     @pulumi.getter
     def cdrom(self) -> pulumi.Output[Optional['outputs.VirtualMachineCdrom']]:
         """
         The CDROM drive
         """
         return pulumi.get(self, "cdrom")
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 3.1.0
+Version: 4.0.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Proxmox VE Resource Provider
 
 [![](https://img.shields.io/github/license/muhlba91/pulumi-proxmoxve?style=for-the-badge)](LICENSE)
 [![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/release.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions)
 [![](https://img.shields.io/github/release-date/muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/releases)
```

### Comparing `pulumi_proxmoxve-3.1.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-4.0.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 pulumi_proxmoxve.egg-info/PKG-INFO
 pulumi_proxmoxve.egg-info/SOURCES.txt
 pulumi_proxmoxve.egg-info/dependency_links.txt
 pulumi_proxmoxve.egg-info/not-zip-safe
 pulumi_proxmoxve.egg-info/requires.txt
 pulumi_proxmoxve.egg-info/top_level.txt
 pulumi_proxmoxve/cluster/__init__.py
-pulumi_proxmoxve/cluster/_inputs.py
-pulumi_proxmoxve/cluster/cluster_alias.py
-pulumi_proxmoxve/cluster/cluster_ip_set.py
-pulumi_proxmoxve/cluster/get_cluster_alias.py
-pulumi_proxmoxve/cluster/get_cluster_aliases.py
 pulumi_proxmoxve/cluster/get_nodes.py
-pulumi_proxmoxve/cluster/outputs.py
 pulumi_proxmoxve/config/__init__.py
 pulumi_proxmoxve/config/outputs.py
 pulumi_proxmoxve/config/vars.py
 pulumi_proxmoxve/ct/__init__.py
 pulumi_proxmoxve/ct/_inputs.py
 pulumi_proxmoxve/ct/container.py
 pulumi_proxmoxve/ct/outputs.py
+pulumi_proxmoxve/network/__init__.py
+pulumi_proxmoxve/network/_inputs.py
+pulumi_proxmoxve/network/firewall.py
+pulumi_proxmoxve/network/firewall_alias.py
+pulumi_proxmoxve/network/firewall_ip_set.py
+pulumi_proxmoxve/network/firewall_options.py
+pulumi_proxmoxve/network/firewall_rules.py
+pulumi_proxmoxve/network/firewall_security_group.py
+pulumi_proxmoxve/network/outputs.py
 pulumi_proxmoxve/permission/__init__.py
 pulumi_proxmoxve/permission/_inputs.py
 pulumi_proxmoxve/permission/get_group.py
 pulumi_proxmoxve/permission/get_groups.py
 pulumi_proxmoxve/permission/get_pool.py
 pulumi_proxmoxve/permission/get_pools.py
 pulumi_proxmoxve/permission/get_role.py
```

### Comparing `pulumi_proxmoxve-3.1.0/setup.py` & `pulumi_proxmoxve-4.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.1.0"
-PLUGIN_VERSION = "3.1.0"
+VERSION = "4.0.0"
+PLUGIN_VERSION = "4.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
 
 
 setup(name='pulumi_proxmoxve',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

