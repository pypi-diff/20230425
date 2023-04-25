# Comparing `tmp/edc-rx-0.1.4.tar.gz` & `tmp/edc-rx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.4.tar", last modified: Tue Apr 18 01:41:33 2023, max compression
+gzip compressed data, was "edc-rx-0.1.5.tar", last modified: Tue Apr 25 02:49:30 2023, max compression
```

## Comparing `edc-rx-0.1.4.tar` & `edc-rx-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467733 edc-rx-0.1.4/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.459466 edc-rx-0.1.4/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.462997 edc-rx-0.1.4/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-04-18 01:41:25.000000 edc-rx-0.1.4/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-04-18 01:41:25.000000 edc-rx-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.4/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.4/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-18 01:41:33.467826 edc-rx-0.1.4/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.4/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.463885 edc-rx-0.1.4/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.464930 edc-rx-0.1.4/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.4/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.465579 edc-rx-0.1.4/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1558 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466018 edc-rx-0.1.4/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466283 edc-rx-0.1.4/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1914 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466406 edc-rx-0.1.4/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467513 edc-rx-0.1.4/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467651 edc-rx-0.1.4/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      900 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.464680 edc-rx-0.1.4/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.4/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-04-18 01:41:25.000000 edc-rx-0.1.4/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.4/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-04-18 01:41:33.468159 edc-rx-0.1.4/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440753 edc-rx-0.1.5/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.432135 edc-rx-0.1.5/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.435691 edc-rx-0.1.5/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-04-18 01:41:25.000000 edc-rx-0.1.5/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-04-18 01:41:25.000000 edc-rx-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.5/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.5/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-25 02:49:30.440841 edc-rx-0.1.5/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.5/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.436755 edc-rx-0.1.5/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.437730 edc-rx-0.1.5/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.5/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.438404 edc-rx-0.1.5/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1698 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.438902 edc-rx-0.1.5/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.439189 edc-rx-0.1.5/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.439305 edc-rx-0.1.5/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.5/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440416 edc-rx-0.1.5/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440654 edc-rx-0.1.5/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.5/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4232 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/tests/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      799 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.437414 edc-rx-0.1.5/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.5/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-04-18 01:41:25.000000 edc-rx-0.1.5/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.5/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-04-25 02:49:30.441177 edc-rx-0.1.5/setup.cfg
```

### Comparing `edc-rx-0.1.4/.github/workflows/build.yml` & `edc-rx-0.1.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/.gitignore` & `edc-rx-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/.pre-commit-config.yaml` & `edc-rx-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/LICENSE` & `edc-rx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/PKG-INFO` & `edc-rx-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Microcopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.4/README.rst` & `edc-rx-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.5/edc_rx/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.5/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.conf import settings
+from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from edc_constants.choices import YES_NO
 
 
 class DrugRefillModelMixin(models.Model):
     rx_other = models.CharField(
         verbose_name="If other, please specify ...",
@@ -47,12 +48,13 @@
         blank=True,
     )
 
     return_in_days = models.IntegerField(
         verbose_name=(
             "In how many days has the patient been asked "
             "to return to clinic for a drug refill?"
-        )
+        ),
+        validators=[MinValueValidator(0), MaxValueValidator(180)],
     )
 
     class Meta:
         abstract = True
```

### Comparing `edc-rx-0.1.4/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.5/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.5/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.5/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     def clean(self):
         cleaned_data = super().clean()
         data = dict(self.data.lists())
         rx = self.list_model_cls.objects.filter(id__in=data.get("rx") or [])
         rx_names = [obj.display_name for obj in rx]
         inline_drug_names = self.raise_on_duplicates()
 
-        try:
-            validate_total_days(self)
-        except TotalDaysMismatch as e:
-            raise forms.ValidationError(e)
+        if data.get("return_in_days")[0] is not None and data.get("return_in_days")[0] != "":
+            try:
+                validate_total_days(self, return_in_days=int(data.get("return_in_days")[0]))
+            except TotalDaysMismatch as e:
+                raise forms.ValidationError(e)
 
         if (
             self.cleaned_data.get("drug")
             and self.cleaned_data.get("drug").display_name not in rx_names
         ):
             treatment = " + ".join(rx_names)
             raise forms.ValidationError(
```

### Comparing `edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/edc_rx/utils.py` & `edc-rx-0.1.5/edc_rx/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,19 @@
 
 
 class TotalDaysMismatch(Exception):
     pass
 
 
 def validate_total_days(form: Any, return_in_days: int | None = None) -> None:
-    return_in_days = return_in_days or form.cleaned_data.get("return_in_days")
-    if (
-        form.cleaned_data.get("clinic_days")
-        and form.cleaned_data.get("club_days")
-        and form.cleaned_data.get("purchased_days")
-        and int(return_in_days or 0)
-    ):
-        total = (
-            form.cleaned_data.get("clinic_days")
-            or 0 + form.cleaned_data.get("club_days")
-            or 0 + form.cleaned_data.get("purchased_days")
-            or 0
+    return_in_days = return_in_days or form.cleaned_data.get("return_in_days") or 0
+    clinic_days = form.cleaned_data.get("clinic_days") or 0
+    club_days = form.cleaned_data.get("club_days") or 0
+    purchased_days = form.cleaned_data.get("purchased_days") or 0
+
+    total_days = clinic_days + club_days + purchased_days
+    if total_days != return_in_days:
+        raise TotalDaysMismatch(
+            f"Patient to return for a drug refill in {return_in_days} days. "
+            f"Check that the total days supplied "
+            f"({clinic_days} + {club_days} + {purchased_days}) matches this."
         )
-        if total != int(return_in_days or 0):
-            raise TotalDaysMismatch(
-                f"Patient to return for a drug refill in {return_in_days} days. "
-                "Check that the total days match."
-            )
```

### Comparing `edc-rx-0.1.4/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.5/edc_rx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Microcopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.4/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.5/edc_rx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 edc_rx/tests/etc/user-aes-restricted.key
 edc_rx/tests/etc/user-rsa-local-private.pem
 edc_rx/tests/etc/user-rsa-local-public.pem
 edc_rx/tests/etc/user-rsa-restricted-private.pem
 edc_rx/tests/etc/user-rsa-restricted-public.pem
 edc_rx/tests/etc/user-salt-local.key
 edc_rx/tests/etc/user-salt-restricted.key
-edc_rx/tests/tests/__init__.py
+edc_rx/tests/tests/__init__.py
+edc_rx/tests/tests/test_utils.py
```

### Comparing `edc-rx-0.1.4/pyproject.toml` & `edc-rx-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/runtests.py` & `edc-rx-0.1.5/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.4/setup.cfg` & `edc-rx-0.1.5/setup.cfg`

 * *Files identical despite different names*

