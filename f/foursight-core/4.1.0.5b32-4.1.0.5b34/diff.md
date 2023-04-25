# Comparing `tmp/foursight_core-4.1.0.5b32.tar.gz` & `tmp/foursight_core-4.1.0.5b34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b32.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b34.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b32.tar` & `foursight_core-4.1.0.5b34.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-04-24 21:25:46.781767 foursight_core-4.1.0.5b32/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/app.py
--rw-r--r--   0        0        0   105730 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-04-24 21:25:46.789767 foursight_core-4.1.0.5b32/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/package.py
--rw-r--r--   0        0        0    17014 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7709 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3459 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5745 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4878 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     4021 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    77887 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11353 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    32302 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-24 21:25:46.793768 foursight_core-4.1.0.5b32/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1926328 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-04-24 21:25:46.805769 foursight_core-4.1.0.5b32/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1549 2023-04-24 21:25:46.809769 foursight_core-4.1.0.5b32/pyproject.toml
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b32/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-25 12:19:45.041842 foursight_core-4.1.0.5b34/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-25 12:19:45.045842 foursight_core-4.1.0.5b34/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-25 12:19:45.045842 foursight_core-4.1.0.5b34/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-04-25 12:19:45.045842 foursight_core-4.1.0.5b34/foursight_core/app.py
+-rw-r--r--   0        0        0   105730 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/package.py
+-rw-r--r--   0        0        0    17014 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7709 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    23203 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20652 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3459 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     5745 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4878 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3257 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     4583 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    77887 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11353 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    32676 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4861 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-25 12:19:45.049842 foursight_core-4.1.0.5b34/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1927378 2023-04-25 12:19:45.061843 foursight_core-4.1.0.5b34/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-04-25 12:19:45.061843 foursight_core-4.1.0.5b34/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1549 2023-04-25 12:19:45.065843 foursight_core-4.1.0.5b34/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b34/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b32/LICENSE.txt` & `foursight_core-4.1.0.5b34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b34/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/buckets.py` & `foursight_core-4.1.0.5b34/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b34/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b34/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/decorators.py` & `foursight_core-4.1.0.5b34/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/deploy.py` & `foursight_core-4.1.0.5b34/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/environment.py` & `foursight_core-4.1.0.5b34/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b34/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b34/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b34/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/identity.py` & `foursight_core-4.1.0.5b34/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/mapping.json` & `foursight_core-4.1.0.5b34/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/package.py` & `foursight_core-4.1.0.5b34/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/portal_access_key_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from dcicutils import ff_utils
 from typing import Optional, Tuple
 from ...app import app
 
 
 _PORTAL_ACCESS_KEY_NAME = "access_key_foursight"
 _PORTAL_ACCESS_KEY_USER_EMAIL = "foursight.app@gmail.com"
-_PORTAL_ACCESS_KEY_EXPIRATION_DAYS = 90
 _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS = 7
 
 
 def get_portal_access_key_info(env: str,
                                obfuscate: bool = False,
                                test_mode_access_key_simulate_error: bool = False,
                                test_mode_access_key_expiration_warning_days: int = 0) -> dict:
@@ -23,55 +22,65 @@
         if key and obfuscate:
             key = key[0] + "*******"
         secret = connection_keys.get("secret")
         if secret:
             secret = "********" if obfuscate else secret[1] + "*******"
         server = connection_keys.get("server")
         access_key_info = {"key": key, "secret": secret, "server": server}
-        access_key_expires_date, access_key_expires_exception = _get_portal_access_key_expires_date(connection_keys)
+        access_key_create_date, access_key_expires_date, access_key_expires_exception = \
+            _get_portal_access_key_expires_date(connection_keys)
         if access_key_expires_date:
-            access_key_info["expires_at"] = access_key_expires_date.strftime("%Y-%m-%d %H:%M:%S")
-            access_key_info["expired"] = now >= access_key_expires_date
-            access_key_info["invalid"] = access_key_info["expired"]
-            if test_mode_access_key_expiration_warning_days > 0:
-                expires_soon_days = test_mode_access_key_expiration_warning_days
+            access_key_info["created_at"] = access_key_create_date.strftime("%Y-%m-%d %H:%M:%S")
+            if access_key_expires_date == datetime.max:
+                access_key_info["expires_at"] = None
+                access_key_info["expired"] = False
+                access_key_info["invalid"] = False
+                access_key_info["expires_soon"] = False
             else:
-                expires_soon_days = _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS
-            access_key_info["expires_soon"] = _is_datetime_within_future_ndays(access_key_expires_date,
-                                                                               ndays=expires_soon_days,
-                                                                               now=now)
+                access_key_info["expires_at"] = access_key_expires_date.strftime("%Y-%m-%d %H:%M:%S")
+                access_key_info["expired"] = now >= access_key_expires_date
+                access_key_info["invalid"] = access_key_info["expired"]
+                if test_mode_access_key_expiration_warning_days > 0:
+                    expires_soon_days = test_mode_access_key_expiration_warning_days
+                else:
+                    expires_soon_days = _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS
+                access_key_info["expires_soon"] = _is_datetime_within_future_ndays(access_key_expires_date,
+                                                                                   ndays=expires_soon_days,
+                                                                                   now=now)
             if test_mode_access_key_simulate_error:
                 access_key_info["exception"] = "test_mode_access_key_simulate_error"
                 access_key_info["invalid"] = True
         else:
-            # If we don't get an expires date at all,
-            # from _get_portal_access_key_expires_date,
-            # then we assume there is a problem.
+            # If we don't get an expires date at all, then assume there is a problem.
             access_key_info["exception"] = str(access_key_expires_exception)
             e = str(access_key_info["exception"]).lower()
             if "credenti" in e or "expir" in e:
                 access_key_info["probably_expired"] = True
             access_key_info["invalid"] = True
         access_key_info["timestamp"] = now.strftime("%Y-%m-%d %H:%M:%S")
         return access_key_info
     except Exception as e:
         return {}
 
 
-def _get_portal_access_key_expires_date(keys: dict) -> Tuple[Optional[datetime], Optional[Exception]]:
+def _get_portal_access_key_expires_date(keys: dict) -> Tuple[datetime, Optional[datetime], Optional[Exception]]:
     try:
-        #if test_mode_access_key_simulate_error:
-        #    raise Exception("test_mode_access_key_simulate_error")
         query = f"/search/?type=AccessKey&description={_PORTAL_ACCESS_KEY_NAME}&sort=-date_created"
         access_key = ff_utils.search_metadata(query, key=keys)[0]
         access_key_create_date = datetime.fromisoformat(access_key["date_created"])
-        access_key_expires_date = access_key_create_date + timedelta(days=_PORTAL_ACCESS_KEY_EXPIRATION_DAYS)
-        return (access_key_expires_date, None)
+        access_key_expires_date = access_key.get("expiration_date")
+        if access_key_expires_date:
+            access_key_expires_date = datetime.fromisoformat(access_key_expires_date)
+        else:
+            # There may or may not be an expiration date (e.g. for fourfront);
+            # if not then make it the max date which is 9999-12-31.
+            access_key_expires_date = datetime.max
+        return (access_key_create_date, access_key_expires_date, None)
     except Exception as e:
-        return (None, e)
+        return (None, None, e)
 
 
 def _is_datetime_within_future_ndays(d: datetime, ndays: int, now: Optional[datetime] = None) -> bool:
     """
     Returns True iff the given datatime is within ndays IN THE FUTURE of the CURRENT
     datetime. I.e. if the current datetime plus ndays is greater-than-or-equal to
     the given datetime the returns True; otherwise returns False.
```

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/react_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,25 @@
     def __init__(self):
         super(ReactRoutes, self).__init__()
 
     # ----------------------------------------------------------------------------------------------
     # Foursight React API routes UNPROTECTED by authorization/authentication.
     # ----------------------------------------------------------------------------------------------
 
+    @route("/{env}/auth0_config", authorize=False)
+    def reactapi_route_auth0_config(env: str) -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Returns Auth0 configuration for authentication (from Portal).
+        Note that this in an UNPROTECTED route.
+        """
+        ignored(env)
+        return reactapi_route_auth0_config_noenv()
+
     @route("/auth0_config", authorize=False)
-    def reactapi_route_auth0_config() -> Response:  # noqa: implicit @staticmethod via @route
+    def reactapi_route_auth0_config_noenv() -> Response:  # noqa: implicit @staticmethod via @route
         """
         Returns Auth0 configuration for authentication (from Portal).
         Note that this in an UNPROTECTED route.
         """
         return app.core.reactapi_auth0_config(app.current_request.to_dict())
 
     @route("/cognito_config", authorize=False)
```

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b34/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b34/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b34/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.a3264e5e.js.LICENSE.txt */
+/*! For license information please see main.a2a8cf6f.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -49320,14 +49320,24 @@
                                 }), (0, Kr.jsx)("td", {
                                     style: i,
                                     children: r.secret
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
+                                    children: "Creation Date:"
+                                }), (0, Kr.jsxs)("td", {
+                                    style: i,
+                                    children: [r.created_at, "\xa0\xa0", Fr.RightArrow, "\xa0 \xa0", (0, Kr.jsx)("small", {
+                                        children: Pr.Ago(r.created_at, !0, !1)
+                                    })]
+                                })]
+                            }), (0, Kr.jsxs)("tr", {
+                                children: [(0, Kr.jsx)("td", {
+                                    style: s,
                                     children: "Expiration Date:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: i,
                                     children: [r.expires_at, r.expires_at ? (0, Kr.jsx)(Kr.Fragment, {
                                         children: r.expired ? (0, Kr.jsxs)(Kr.Fragment, {
                                             children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("b", {
                                                 children: (0, Kr.jsx)("u", {
@@ -49338,15 +49348,15 @@
                                             })]
                                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                                             children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
                                                 children: Pr.FromNow(r.expires_at, !0, !1)
                                             })]
                                         })
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                                        children: "Unknown"
+                                        children: "None"
                                     })]
                                 })]
                             }), r.exception && (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Details:"
                                 }), (0, Kr.jsx)("td", {
@@ -49577,15 +49587,15 @@
                                             })
                                         })
                                     })]
                                 })]
                             }), n.owner && (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: i,
-                                    children: "Owner:"
+                                    children: "Issuee:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: o,
                                     children: [n.owner, n.owner_entity && n.owner_entity != n.owner && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0(", n.owner_entity, ")"]
                                     })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
@@ -49600,23 +49610,27 @@
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: i,
                                     children: "Activation Date:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: o,
-                                    children: [n.active_at, n.inactive && (0, Kr.jsxs)("b", {
+                                    children: [n.active_at, n.inactive ? (0, Kr.jsxs)("b", {
                                         style: {
                                             color: r
                                         },
                                         children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("b", {
                                             children: (0, Kr.jsx)("u", {
                                                 children: "Inactive"
                                             })
                                         }), "\xa0\xa0", Fr.LeftArrow]
+                                    }) : (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
+                                            children: Pr.Ago(n.active_at, !0, !1)
+                                        })]
                                     })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: i,
                                     children: "Expiration Date:"
                                 }), (0, Kr.jsxs)("td", {
@@ -49664,15 +49678,15 @@
                                             children: [(0, Kr.jsx)("u", {
                                                 children: "Show"
                                             }), " ", Fr.UpArrow]
                                         })
                                     })
                                 })]
                             }), u && (0, Kr.jsxs)(Kr.Fragment, {
-                                children: [(0, Kr.jsxs)("tr", {
+                                children: [n.exception && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
                                         style: i,
                                         children: "Error:"
                                     }), (0, Kr.jsx)("td", {
                                         style: o,
                                         children: n.exception
                                     })]
@@ -59009,62 +59023,66 @@
                     g = e.python,
                     y = void 0 !== g && g,
                     m = (e.chalice, e.check),
                     v = void 0 !== m && m,
                     M = e.link,
                     b = void 0 === M ? null : M,
                     w = e.optional,
-                    j = void 0 !== w && w;
-                var x = {
+                    j = void 0 !== w && w,
+                    x = e.portalCertificate,
+                    N = void 0 === x ? null : x,
+                    I = e.portalAccessKey,
+                    D = void 0 === I ? null : I;
+                var S = {
                         fontSize: "11pt",
                         fontFamily: o ? "monospace" : "inherit",
                         fontWeight: "bold",
                         wordWrap: "break-word",
                         cursor: a ? "copy" : "inherit",
                         align: "left"
                     },
-                    N = a ? {
+                    L = a ? {
                         onClick: function() {
                             return Yr.Copy(t)
                         }
                     } : {},
-                    I = v ? (0, Kr.jsxs)("span", {
+                    k = v ? (0, Kr.jsxs)("span", {
                         children: ["\xa0", (0, Kr.jsx)("b", {
                             style: {
                                 fontSize: "13pt",
                                 color: "green"
                             },
                             children: Fr.Check
                         })]
                     }) : (0, Kr.jsx)("span", {}),
-                    D = c ? (0, Kr.jsxs)("span", {
+                    C = c ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://pypi.org/project/" + t + "/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "pypi",
                                 src: Ut.PyPi(),
                                 height: "21"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    S = f ? (0, Kr.jsxs)("span", {
+                    E = f ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://github.com/" + f + "/" + ("dcicutils" === t ? "utils" : t) + "/releases/tag/" + ("chalice" !== t ? "v" : "") + n,
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.GitHub(),
                                 height: "15"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    L = h ? (0, Kr.jsxs)("span", {
+                    _ = h ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://www.elastic.co/guide/en/elasticsearch/reference/".concat(function(e) {
                                 var t = null === e || void 0 === e ? void 0 : e.split(".");
                                 return (null === t || void 0 === t ? void 0 : t.length) >= 2 ? t[0] + "." + t[1] : e
                             }(n), "/release-notes-").concat(n, ".html"),
@@ -59074,27 +59092,27 @@
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.ElasticsearchLogo(),
                                 height: "18"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    k = y ? (0, Kr.jsxs)("span", {
+                    T = y ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://docs.python.org/release/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "python",
                                 src: Ut.Python(),
                                 height: "19"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    C = (0, Kr.jsx)("span", {});
+                    A = (0, Kr.jsx)("span", {});
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         style: {
                             marginTop: "1px"
                         },
                         children: !j || n ? (0, Kr.jsxs)("div", {
                             className: "row",
@@ -59109,31 +59127,41 @@
                                         align: "left"
                                     },
                                     children: [t, ":"]
                                 })
                             }), (0, Kr.jsxs)("div", Ye(Ye({
                                 id: t,
                                 className: "col-sm-8",
-                                style: x,
+                                style: S,
                                 align: "left"
-                            }, N), {}, {
-                                children: [D, S, L, k, C, b && n ? (0, Kr.jsx)("span", {
+                            }, L), {}, {
+                                children: [C, E, _, T, A, b && n ? (0, Kr.jsx)("span", {
                                     children: (0, Kr.jsx)(Oe, {
                                         to: b,
                                         children: n
                                     })
-                                }) : (0, Kr.jsx)("span", {
-                                    children: st.IsNonEmptyObject(n) ? (0, Kr.jsx)(Kr.Fragment, {
+                                }) : (0, Kr.jsxs)("span", {
+                                    children: [st.IsNonEmptyObject(n) ? (0, Kr.jsx)(Kr.Fragment, {
                                         children: n
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
                                         children: n || (0, Kr.jsx)("span", {
                                             children: Fr.EmptySet
                                         })
-                                    })
-                                }), I]
+                                    }), D && (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
+                                            to: kr.Path("/portal_access_key"),
+                                            children: "View Details"
+                                        })]
+                                    }), N && (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
+                                            to: kr.Path("/certificates"),
+                                            children: "View Certificate"
+                                        })]
+                                    })]
+                                }), k]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
             Ms = function() {
                 var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = ta(),
@@ -59143,15 +59171,16 @@
                     Q = F[1],
                     G = a((0, t.useState)(!1), 2),
                     W = G[0],
                     H = G[1],
                     Z = a((0, t.useState)(!1), 2),
                     V = Z[0],
                     q = Z[1],
-                    J = fa();
+                    J = Xi("/portal_access_key"),
+                    K = fa();
                 return B.error ? (0, Kr.jsx)(xi, {
                     error: B.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
                     children: [(0, Kr.jsxs)(ms, {
                         info: B,
@@ -59238,32 +59267,45 @@
                         children: [(0, Kr.jsx)(vs, {
                             name: "AWS Account Number",
                             value: B.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(vs, {
+                            name: "AWS Region Name",
+                            value: B.get("app.credentials.aws_region"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Kr.jsx)(vs, {
                             name: "AWS User ARN",
                             value: B.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(vs, {
                             name: "AWS Access Key ID",
                             value: B.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(vs, {
-                            name: "AWS Region Name",
-                            value: B.get("app.credentials.aws_region"),
+                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(vs, {
+                            name: "AWS S3 Access Key ID",
+                            value: B.get("environ.S3_AWS_ACCESS_KEY_ID"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(vs, {
+                            name: "Portal Access Key",
+                            value: J.get("key"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            portalAccessKey: !0
+                        }), (0, Kr.jsx)(vs, {
                             name: "Auth0 Client ID",
                             value: B.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(ms, {
@@ -59276,15 +59318,16 @@
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(vs, {
                             name: "Portal Server",
                             value: B.get("server.portal"),
                             monospace: !0,
                             copy: !0,
-                            size: "2"
+                            size: "2",
+                            portalCertificate: !0
                         }), (0, Kr.jsx)(vs, {
                             name: "ElasticSearch Server",
                             value: B.get("server.es"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(vs, {
@@ -59601,15 +59644,15 @@
                                 position: "bottom",
                                 size: "small",
                                 text: "Reloading the Foursight app."
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
-                                    return q(!0), void J("/__reloadlambda__", {
+                                    return q(!0), void K("/__reloadlambda__", {
                                         onDone: function() {
                                             return q(!1)
                                         }
                                     })
                                 },
                                 id: "tooltip-info-reload",
                                 style: {
@@ -59632,15 +59675,15 @@
                                 cursor: "pointer"
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("img", {
                                 alt: "Clear Cache",
                                 src: Ut.ClearCache(),
                                 height: "19",
                                 onClick: function() {
-                                    J(zt.Url("/__clearcache__", !1))
+                                    K(zt.Url("/__clearcache__", !1))
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
```

### Comparing `foursight_core-4.1.0.5b32/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b34/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/routes.py` & `foursight_core-4.1.0.5b34/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/run_result.py` & `foursight_core-4.1.0.5b34/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b34/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b34/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b34/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b34/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b34/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/stage.py` & `foursight_core-4.1.0.5b34/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b34/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b32/pyproject.toml` & `foursight_core-4.1.0.5b34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b32"
+version = "4.1.0.5b34"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.1.0.5b32/PKG-INFO` & `foursight_core-4.1.0.5b34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b32
+Version: 4.1.0.5b34
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

