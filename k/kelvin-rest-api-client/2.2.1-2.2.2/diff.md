# Comparing `tmp/kelvin-rest-api-client-2.2.1.tar.gz` & `tmp/kelvin-rest-api-client-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelvin-rest-api-client-2.2.1.tar", last modified: Mon Dec 19 07:40:09 2022, max compression
+gzip compressed data, was "kelvin-rest-api-client-2.2.2.tar", last modified: Tue Apr 25 10:39:04 2023, max compression
```

## Comparing `kelvin-rest-api-client-2.2.1.tar` & `kelvin-rest-api-client-2.2.2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     4156 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     2861 2022-12-19 07:18:12.000000 kelvin-rest-api-client-2.2.1/HISTORY.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1147 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/LICENSE
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      238 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/MANIFEST.in
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    15020 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/PKG-INFO
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     8484 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/README.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)        6 2022-12-19 07:18:12.000000 kelvin-rest-api-client-2.2.1/VERSION.txt
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/docs/
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      625 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/Makefile
--rwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)     5171 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/conf.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       33 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/contributing.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       28 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/history.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      374 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/index.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1525 2021-09-24 06:33:32.000000 kelvin-rest-api-client-2.2.1/docs/installation.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      808 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/make.bat
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       60 2022-10-18 13:13:02.000000 kelvin-rest-api-client-2.2.1/docs/modules.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       27 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/readme.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      172 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.base.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      190 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.exceptions.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      172 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.role.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      526 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      178 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.school.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      198 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.school_class.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      181 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.session.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      172 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.user.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      187 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.workgroup.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      137 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       40 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/docs/ucsschool.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1491 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/docs/usage-auth.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      627 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/docs/usage-correlation.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1504 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-language.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     3519 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-role.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    10059 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-school-class.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     7640 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-school.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    10477 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-users.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    10244 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage-workgroups.rst
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1225 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/docs/usage.rst
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    15020 2022-12-19 07:40:09.000000 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1750 2022-12-19 07:40:09.000000 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)        1 2022-12-19 07:40:09.000000 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      493 2022-12-19 07:40:09.000000 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)       10 2022-12-19 07:40:09.000000 kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      102 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/requirements.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      103 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/requirements_dev.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      185 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/requirements_test.txt
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      267 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/setup.cfg
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     2031 2022-12-14 12:33:42.000000 kelvin-rest-api-client-2.2.1/setup.py
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/tests/
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    40941 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/tests/conftest.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      196 2020-06-04 14:05:21.000000 kelvin-rest-api-client-2.2.1/tests/test_init.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1627 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/tests/test_kelvin_object_init.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     2663 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/tests/test_logger.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     3213 2021-09-17 06:57:09.000000 kelvin-rest-api-client-2.2.1/tests/test_role.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     9281 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/tests/test_school.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    13274 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/tests/test_school_class.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      194 2022-12-15 08:47:39.000000 kelvin-rest-api-client-2.2.1/tests/test_server.yaml
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)      187 2021-09-20 09:24:56.000000 kelvin-rest-api-client-2.2.1/tests/test_server_example.yaml
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     8246 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/tests/test_session.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     2599 2021-09-17 06:57:09.000000 kelvin-rest-api-client-2.2.1/tests/test_test.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    19965 2022-12-19 07:18:12.000000 kelvin-rest-api-client-2.2.1/tests/test_user.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    11521 2022-10-18 14:05:13.000000 kelvin-rest-api-client-2.2.1/tests/test_workgroup.py
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.799126 kelvin-rest-api-client-2.2.1/ucsschool/
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.799126 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/
-drwxr-xr-x   0 twenzel   (2942) Domain Users  (5001)        0 2022-12-19 07:40:09.803126 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1407 2022-10-18 13:51:32.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/__init__.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)    10003 2022-12-19 07:18:12.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/base.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     1641 2021-09-17 06:57:09.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/exceptions.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     3055 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/role.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     4142 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/school.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     3774 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/school_class.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     9243 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/session.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     7978 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/user.py
--rw-r--r--   0 twenzel   (2942) Domain Users  (5001)     4091 2022-11-28 11:28:57.000000 kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/workgroup.py
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.403910 kelvin-rest-api-client-2.2.2/
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     4156 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     2976 2023-04-25 08:39:54.000000 kelvin-rest-api-client-2.2.2/HISTORY.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1147 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/LICENSE
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      238 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/MANIFEST.in
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    12518 2023-04-25 10:39:04.403910 kelvin-rest-api-client-2.2.2/PKG-INFO
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     8484 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/README.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)        6 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/VERSION.txt
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.399910 kelvin-rest-api-client-2.2.2/docs/
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      625 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/Makefile
+-rwxr-xr-x   0 m0u       (1000) m0u       (1000)     5171 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/conf.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       33 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/contributing.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       28 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/history.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      374 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/index.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1525 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/installation.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      808 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/make.bat
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       60 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/modules.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       27 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/docs/readme.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      172 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.base.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      190 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.exceptions.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      172 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.role.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      526 2022-06-30 13:13:08.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      178 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.school.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      198 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.school_class.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      181 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.session.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      172 2022-06-28 09:44:52.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.user.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      187 2022-06-30 13:13:08.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.workgroup.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      137 2022-06-30 13:13:08.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       40 2022-06-30 13:13:08.000000 kelvin-rest-api-client-2.2.2/docs/ucsschool.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1491 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/docs/usage-auth.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      627 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/docs/usage-correlation.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1504 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/docs/usage-language.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     3893 2023-04-25 08:39:54.000000 kelvin-rest-api-client-2.2.2/docs/usage-role.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    10411 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/docs/usage-school-class.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     7640 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/docs/usage-school.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    10766 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/docs/usage-users.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    10587 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/docs/usage-workgroups.rst
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1225 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/docs/usage.rst
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.399910 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    12518 2023-04-25 10:39:04.000000 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1783 2023-04-25 10:39:04.000000 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)        1 2023-04-25 10:39:04.000000 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      493 2023-04-25 10:39:04.000000 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)       10 2023-04-25 10:39:04.000000 kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      102 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/requirements.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      103 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/requirements_dev.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      185 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/requirements_test.txt
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      267 2023-04-25 10:39:04.403910 kelvin-rest-api-client-2.2.2/setup.cfg
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     2031 2022-12-19 09:35:21.000000 kelvin-rest-api-client-2.2.2/setup.py
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.403910 kelvin-rest-api-client-2.2.2/tests/
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    40941 2022-10-03 14:38:01.000000 kelvin-rest-api-client-2.2.2/tests/conftest.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      196 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/tests/test_init.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1627 2022-07-01 04:46:04.000000 kelvin-rest-api-client-2.2.2/tests/test_kelvin_object_init.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     2663 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/tests/test_logger.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     4052 2023-04-25 08:39:54.000000 kelvin-rest-api-client-2.2.2/tests/test_role.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     9203 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/tests/test_school.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    14146 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/tests/test_school_class.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      193 2023-04-20 13:43:53.000000 kelvin-rest-api-client-2.2.2/tests/test_server.yaml
+-rw-r--r--   0 m0u       (1000) m0u       (1000)      187 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/tests/test_server_example.yaml
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     8246 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/tests/test_session.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     2599 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/tests/test_test.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    20633 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/tests/test_user.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    12352 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/tests/test_workgroup.py
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.395910 kelvin-rest-api-client-2.2.2/ucsschool/
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.395910 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/
+drwxr-xr-x   0 m0u       (1000) m0u       (1000)        0 2023-04-25 10:39:04.403910 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1407 2022-06-30 13:13:07.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/__init__.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)    10003 2022-12-19 09:35:21.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/base.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     1641 2022-04-11 15:11:22.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/exceptions.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)        0 2022-12-19 09:35:21.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/py.typed
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     3110 2023-04-25 08:39:54.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/role.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     4142 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/school.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     3829 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/school_class.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     9243 2022-11-21 11:46:23.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/session.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     8033 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/user.py
+-rw-r--r--   0 m0u       (1000) m0u       (1000)     4146 2023-04-20 13:21:13.000000 kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/workgroup.py
```

### Comparing `kelvin-rest-api-client-2.2.1/CONTRIBUTING.rst` & `kelvin-rest-api-client-2.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/HISTORY.rst` & `kelvin-rest-api-client-2.2.2/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.2.2 (2023-04-14)
+------------------
+
+* Support HEAD for ``SchoolClass``, ``User``, ``WorkGroup``, and ``Role``.
+
 2.2.1 (2022-12-15)
 ------------------
 
 * Use deepcopy in ``to_dict`` method to prevent values of ``udm_properties`` from being updated in objects which are copied.
 
 2.2.0 (2022-10-13)
 --------------------
```

### Comparing `kelvin-rest-api-client-2.2.1/LICENSE` & `kelvin-rest-api-client-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/PKG-INFO` & `kelvin-rest-api-client-2.2.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,351 +1,356 @@
 Metadata-Version: 2.1
 Name: kelvin-rest-api-client
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python library to interact with the UCS@school Kelvin REST API.
 Home-page: https://github.com/univention/kelvin-rest-api-client
 Author: Daniel Troeder
 Author-email: troeder@univention.de
 License: GNU Affero General Public License v3
-Description: =========================================
-        Python UCS\@school Kelvin REST API Client
-        =========================================
-        
-        |python| |license| |code style| |bandit| |codecov| |docspassing| |gh Code Linting| |gh Integration tests|
-        
-        Python library to interact with the `UCS\@school Kelvin REST API`_.
-        
-        * Free software: GNU Affero General Public License version 3
-        * Documentation: https://kelvin-rest-api-client.readthedocs.io
-        
-        
-        Features
-        --------
-        
-        * Asynchronous
-        * Automatic handling of HTTP(S) sessions
-        * Type annotations
-        * ~95% test coverage (unittests + integration tests)
-        * Python 3.7, 3.8, 3.9, 3.10
-        
-        Compatibility
-        -------------
-        
-        A list of UCS\@school Kelvin REST API server versions which introduce breaking changes can be found in the [UCS\@school Kelvin REST API Documentation](https://docs.software-univention.de/ucsschool-kelvin-rest-api/kelvin-client-compatibility.html).
-        
-        
-        Usage
-        -----
-        
-        The ``Session`` context manager opens and closes a HTTP session:
-        
-        .. code-block:: python
-        
-            >>> import asyncio
-            >>> from ucsschool.kelvin.client import Session, User, UserResource
-            >>>
-            >>> async def get_user(username: str) -> User:
-            ...     async with Session(
-            ...         "USERNAME",
-            ...         "PASSWORD",
-            ...         "master.ucs.local",
-            ...         verify="ucs-root-ca.crt"
-            ...     ) as session:
-            ...         return await UserResource(session=session).get(name=username)
-            ...
-            >>> obj = asyncio.run(get_user("demo_student"))
-            >>>
-            >>> print(obj)
-            User('name'='test_user', dn='uid=test_user,cn=schueler,cn=users,ou=DEMOSCHOOL,dc=example,dc=com')
-            >>> print(obj.firstname, obj.lastname)
-            Test User
-        
-        There are more examples in the `docs`_ *usage* section.
-        
-        For HTTPS to work, the SSL CA of the target system (UCS Master) must either be publicly signed, installed on the client system or available as file (as in the example above).
-        If the SSL CA certificate is not available ``verify=False``.
-        Obviously that is *not safe*! The CA of any UCS server can always be downloaded from ``http://FQDN.OF.UCS/ucs-root-ca.crt``.
-        
-        
-        Installation
-        ------------
-        
-        Install *UCS\@school Kelvin REST API Client* via pip from `PyPI`_:
-        
-        .. code-block:: console
-        
-            $ pip install kelvin-rest-api-client
-        
-        
-        Tests
-        -----
-        
-        There are some isolated unittests, but most tests run against a real *UCS\@school Kelvin REST API*.
-        A UCS Docker container has been prepared for this (additionally to the Kelvin API Docker container).
-        The ``Makefile`` automates downloading and starting the Docker containers (3.2 GB GB) and running the tests.
-        It is also possible to use an existing UCS DC Master with UCS\@school and the Kelvin API installed.
-        
-        The tests expect the existence of two schools (``OUs``) on the target system (the Kelvin API does not support creation of schools yet).
-        The schools are ``DEMOSCHOOL`` and ``DEMOSCHOOL2``.
-        The first one usually already exists, but trying to create it again is safe.
-        To create the schools run *on the UCS DC Master*:
-        
-        .. code-block:: console
-        
-            $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL
-            $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL2
-        
-        Furthermore an email domain must exist:
-        
-        .. code-block:: console
-        
-            $ udm mail/domain create \
-                --ignore_exists \
-                --position "cn=domain,cn=mail,$(ucr get ldap/base)" \
-                --set name="$(ucr get domainname)"
-        
-        Since version ``1.5.0`` the Kelvin REST API supports UDM properties in all resources. A configuration is required for the tests for this feature:
-        
-        .. code-block:: console
-        
-            $ cat > /etc/ucsschool/kelvin/mapped_udm_properties.json <<__EOF__
-            {
-                "user": ["title"],
-                "school_class": ["mailAddress"],
-                "school": ["description"]
-            }
-            __EOF__
-        
-        The provided UCS Docker containers already contain both OUs.
-        They can be started using the Makefile:
-        
-        .. code-block:: console
-        
-            $ make start-docker-containers
-        
-            Downloading Docker image '..-ucsschool-udm-rest-api-only:stable-4.4-8'...
-            Downloading Docker image '../ucsschool-kelvin-rest-api:1.5.5'...
-            Starting UCS docker container...
-            Waiting for UCS docker container to start...
-            Waiting for IP address of UCS container...
-            Waiting for UDM REST API...........
-            Creating Kelvin REST API container...
-            Configuring Kelvin REST API container...
-            Rebuilding the OpenAPI client library in the Kelvin API Container...
-            Starting Kelvin REST API server...
-            Waiting for Kelvin docker container to start...
-            Waiting for IP address of Kelvin container...
-            Waiting for Kelvin API...
-            Fixing log file permissions...
-            Setting up reverse proxy...
-            ==> UDM REST API log file: /tmp/udm-rest-api-log/directory-manager-rest.log
-            ==> UDM REST API: http://172.17.0.2/univention/udm/
-            ==> Kelvin API configs: /tmp/kelvin-api/configs/
-            ==> Kelvin API hooks: /tmp/kelvin-api/kelvin-hooks/
-            ==> Kelvin API log file: /tmp/kelvin-api/log/http.log
-            ==> Kelvin API: http://172.17.0.3:8911/ucsschool/kelvin/v1/docs
-            ==> Kelvin API: https://172.17.0.2/ucsschool/kelvin/v1/docs
-        
-        The Docker containers can be stopped and removed by running:
-        
-        .. code-block:: console
-        
-            $ make stop-and-remove-docker-containers
-        
-        The Docker images will not be removed, only the running containers.
-        
-        Run tests with current Python interpreter:
-        
-        .. code-block:: console
-        
-            $ make test
-        
-        Using `tox`_ the tests can be executed with all supported Python versions:
-        
-        .. code-block:: console
-        
-            $ make test-all
-        
-        To use an existing UCS server for the tests, copy the file ``tests/test_server_example.yaml`` to ``tests/test_server.yaml`` and adapt the settings before starting the tests:
-        
-        .. code-block:: console
-        
-            $ cp tests/test_server_example.yaml tests/test_server.yaml
-            $ $EDITOR tests/test_server.yaml
-            # check settings with a single test:
-            $ python -m pytest tests/test_user.py::test_get
-            # if OK, run all tests:
-            $ make test
-        
-        
-        Logging
-        -------
-        
-        Standard logging is used for tracking the libraries activity.
-        To capture the log messages for this project, subscribe to a logger named ``ucsschool.kelvin.client``.
-        *Attention:* Passwords and session tokens will be logged at log level ``DEBUG``!
-        
-        The *UCS\@school Kelvin REST API* on the UCS server logs into the file ``/var/log/univention/ucsschool-kelvin-rest-api/http.log``.
-        The *UDM REST API* on the UCS server logs into the file ``/var/log/univention/directory-manager-rest.log``.
-        
-        Repo permissions
-        ----------------
-        * Github: @dansan and @JuergenBS
-        * Gitlab: @JuergenBS
-        * PyPI: @dansan and @SamuelYaron
-        * RTD: @dansan and @SamuelYaron
-        
-        Credits
-        -------
-        
-        .. _`UCS\@school Kelvin REST API`: https://docs.software-univention.de/ucsschool-kelvin-rest-api/
-        .. _`tox`: http://tox.readthedocs.org/
-        .. _`docs`: https://kelvin-rest-api-client.readthedocs.io
-        .. _`PyPI`: https://pypi.org/project/kelvin-rest-api-client/
-        .. |license| image:: https://img.shields.io/badge/License-AGPL%20v3-orange.svg
-            :alt: GNU AGPL V3 license
-            :target: https://www.gnu.org/licenses/agpl-3.0
-        .. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
-            :alt: Python 3.7+
-            :target: https://www.python.org/
-        .. |code style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :alt: Code style: black
-            :target: https://github.com/psf/black
-        .. |codecov| image:: https://codecov.io/gh/univention/kelvin-rest-api-client/branch/master/graph/badge.svg
-            :alt: Code coverage
-            :target: https://codecov.io/gh/univention/kelvin-rest-api-client
-        .. |docspassing| image:: https://readthedocs.org/projects/kelvin-rest-api-client/badge/?version=latest
-            :alt: Documentation Status
-            :target: https://kelvin-rest-api-client.readthedocs.io/en/latest/?badge=latest
-        .. |travisci| image:: https://travis-ci.com/univention/kelvin-rest-api-client.svg?branch=master
-            :target: https://app.travis-ci.com/github/univention/kelvin-rest-api-client
-        .. |bandit| image:: https://img.shields.io/badge/security-bandit-yellow.svg
-            :alt: Security: bandit
-            :target: https://github.com/PyCQA/bandit
-        .. |gh Code Linting| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Code%20Linting/badge.svg
-            :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Code+Linting%22
-        .. |gh Integration tests| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Integration%20tests/badge.svg
-            :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
-        
-        
-        =======
-        History
-        =======
-        
-        2.2.1 (2022-12-15)
-        ------------------
-        
-        * Use deepcopy in ``to_dict`` method to prevent values of ``udm_properties`` from being updated in objects which are copied.
-        
-        2.2.0 (2022-10-13)
-        --------------------
-        
-        * Support Http ``Accept-Language`` Header.
-        
-        2.1.0 (2022-10-07)
-        --------------------
-        
-        * Support HEAD for ``School``.
-        
-        2.0.1 (2022-10-05)
-        --------------------
-        
-        * Use detailed upstream error message in ``InvalidRequest`` exception messages.
-        
-        2.0.0 (2022-09-10)
-        --------------------
-        
-        * **API Change**: The required argument ``school`` in the ``User`` constructor has now the default argument ``None``. The argument ``name`` is not required anymore. Optional values, which are set to ``None``, are not passed to the Kelvin server anymore. This enables automatic value generation on the Kelvin REST API server. To make use of this, the attributes can be either set to ``None``, the empty string ``""`` or left out completely. Additionally, you have to create a schema for the corresponding attribute on the Kelvin REST API server.
-        * Send a correlation ID with each request.
-        
-        1.7.1 (2022-08-30)
-        --------------------
-        
-        * Loosen dependency constraints.
-        
-        1.7.0 (2022-07-07)
-        --------------------
-        
-        * Support user ``workgroups`` attribute.
-        
-        1.6.1 (2022-06-30)
-        --------------------
-        
-        * Ignore unknown attributes in KelvinObject child classes.
-        
-        1.6.0 (2022-06-27)
-        --------------------
-        
-        * Add support for workgroup resource.
-        
-        1.5.2.1 (2022-04-05)
-        --------------------
-        
-        * Fixed: Logger does replace values of credentials with placeholders.
-        
-        1.5.2 (2022-02-22)
-        ------------------
-        
-        * Automatic tests now run with Python 3.7 - 3.10.
-        * Fixed: The timeout attribute from a session instance is now used for requests.
-        
-        1.5.1 (2021-11-30)
-        ------------------
-        
-        * Add attribute ``expiration_date`` to the ``User`` class. The attribute was added to the Kelvin REST API app in version ``1.5.1``.
-        
-        1.5.0 (2021-09-21)
-        ------------------
-        
-        * Add attribute ``udm_properties`` to classes ``School`` and ``SchoolClass``.  The attributes were added to the Kelvin REST API app in version ``1.5.0``.
-        
-        0.3.0 (2021-05-04)
-        ------------------
-        
-        * Add support for the creation of school (OU) objects.
-        
-        0.2.2 (2020-11-09)
-        ------------------
-        
-        * Add support for the ``kelvin_password_hashes`` attribute of the ``User`` class.
-        
-        0.2.1 (2020-08-07)
-        ------------------
-        
-        * fix JWT token validity calculation: timestamp uses UTC
-        * documentation fixes
-        * dependency updates
-        * tests also run on Python 3.9-dev
-        
-        0.2.0 (2020-04-17)
-        ------------------
-        
-        * move tox to test requirements
-        * fix user object creation with default parameters
-        * change ``as_dict`` to be a method instead of a property
-        * fix flaky tests
-        * improve test coverage
-        * pass more env args to tox
-        * fix AttributeError with repr(role)
-        * add complete usage documentation
-        
-        0.1.0 (2020-04-16)
-        ------------------
-        
-        * First release.
-        
 Keywords: Univention UCS UCS@school REST
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: development
+License-File: LICENSE
+
+=========================================
+Python UCS\@school Kelvin REST API Client
+=========================================
+
+|python| |license| |code style| |bandit| |codecov| |docspassing| |gh Code Linting| |gh Integration tests|
+
+Python library to interact with the `UCS\@school Kelvin REST API`_.
+
+* Free software: GNU Affero General Public License version 3
+* Documentation: https://kelvin-rest-api-client.readthedocs.io
+
+
+Features
+--------
+
+* Asynchronous
+* Automatic handling of HTTP(S) sessions
+* Type annotations
+* ~95% test coverage (unittests + integration tests)
+* Python 3.7, 3.8, 3.9, 3.10
+
+Compatibility
+-------------
+
+A list of UCS\@school Kelvin REST API server versions which introduce breaking changes can be found in the [UCS\@school Kelvin REST API Documentation](https://docs.software-univention.de/ucsschool-kelvin-rest-api/kelvin-client-compatibility.html).
+
+
+Usage
+-----
+
+The ``Session`` context manager opens and closes a HTTP session:
+
+.. code-block:: python
+
+    >>> import asyncio
+    >>> from ucsschool.kelvin.client import Session, User, UserResource
+    >>>
+    >>> async def get_user(username: str) -> User:
+    ...     async with Session(
+    ...         "USERNAME",
+    ...         "PASSWORD",
+    ...         "master.ucs.local",
+    ...         verify="ucs-root-ca.crt"
+    ...     ) as session:
+    ...         return await UserResource(session=session).get(name=username)
+    ...
+    >>> obj = asyncio.run(get_user("demo_student"))
+    >>>
+    >>> print(obj)
+    User('name'='test_user', dn='uid=test_user,cn=schueler,cn=users,ou=DEMOSCHOOL,dc=example,dc=com')
+    >>> print(obj.firstname, obj.lastname)
+    Test User
+
+There are more examples in the `docs`_ *usage* section.
+
+For HTTPS to work, the SSL CA of the target system (UCS Master) must either be publicly signed, installed on the client system or available as file (as in the example above).
+If the SSL CA certificate is not available ``verify=False``.
+Obviously that is *not safe*! The CA of any UCS server can always be downloaded from ``http://FQDN.OF.UCS/ucs-root-ca.crt``.
+
+
+Installation
+------------
+
+Install *UCS\@school Kelvin REST API Client* via pip from `PyPI`_:
+
+.. code-block:: console
+
+    $ pip install kelvin-rest-api-client
+
+
+Tests
+-----
+
+There are some isolated unittests, but most tests run against a real *UCS\@school Kelvin REST API*.
+A UCS Docker container has been prepared for this (additionally to the Kelvin API Docker container).
+The ``Makefile`` automates downloading and starting the Docker containers (3.2 GB GB) and running the tests.
+It is also possible to use an existing UCS DC Master with UCS\@school and the Kelvin API installed.
+
+The tests expect the existence of two schools (``OUs``) on the target system (the Kelvin API does not support creation of schools yet).
+The schools are ``DEMOSCHOOL`` and ``DEMOSCHOOL2``.
+The first one usually already exists, but trying to create it again is safe.
+To create the schools run *on the UCS DC Master*:
+
+.. code-block:: console
+
+    $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL
+    $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL2
+
+Furthermore an email domain must exist:
+
+.. code-block:: console
+
+    $ udm mail/domain create \
+        --ignore_exists \
+        --position "cn=domain,cn=mail,$(ucr get ldap/base)" \
+        --set name="$(ucr get domainname)"
+
+Since version ``1.5.0`` the Kelvin REST API supports UDM properties in all resources. A configuration is required for the tests for this feature:
+
+.. code-block:: console
+
+    $ cat > /etc/ucsschool/kelvin/mapped_udm_properties.json <<__EOF__
+    {
+        "user": ["title"],
+        "school_class": ["mailAddress"],
+        "school": ["description"]
+    }
+    __EOF__
+
+The provided UCS Docker containers already contain both OUs.
+They can be started using the Makefile:
+
+.. code-block:: console
+
+    $ make start-docker-containers
+
+    Downloading Docker image '..-ucsschool-udm-rest-api-only:stable-4.4-8'...
+    Downloading Docker image '../ucsschool-kelvin-rest-api:1.5.5'...
+    Starting UCS docker container...
+    Waiting for UCS docker container to start...
+    Waiting for IP address of UCS container...
+    Waiting for UDM REST API...........
+    Creating Kelvin REST API container...
+    Configuring Kelvin REST API container...
+    Rebuilding the OpenAPI client library in the Kelvin API Container...
+    Starting Kelvin REST API server...
+    Waiting for Kelvin docker container to start...
+    Waiting for IP address of Kelvin container...
+    Waiting for Kelvin API...
+    Fixing log file permissions...
+    Setting up reverse proxy...
+    ==> UDM REST API log file: /tmp/udm-rest-api-log/directory-manager-rest.log
+    ==> UDM REST API: http://172.17.0.2/univention/udm/
+    ==> Kelvin API configs: /tmp/kelvin-api/configs/
+    ==> Kelvin API hooks: /tmp/kelvin-api/kelvin-hooks/
+    ==> Kelvin API log file: /tmp/kelvin-api/log/http.log
+    ==> Kelvin API: http://172.17.0.3:8911/ucsschool/kelvin/v1/docs
+    ==> Kelvin API: https://172.17.0.2/ucsschool/kelvin/v1/docs
+
+The Docker containers can be stopped and removed by running:
+
+.. code-block:: console
+
+    $ make stop-and-remove-docker-containers
+
+The Docker images will not be removed, only the running containers.
+
+Run tests with current Python interpreter:
+
+.. code-block:: console
+
+    $ make test
+
+Using `tox`_ the tests can be executed with all supported Python versions:
+
+.. code-block:: console
+
+    $ make test-all
+
+To use an existing UCS server for the tests, copy the file ``tests/test_server_example.yaml`` to ``tests/test_server.yaml`` and adapt the settings before starting the tests:
+
+.. code-block:: console
+
+    $ cp tests/test_server_example.yaml tests/test_server.yaml
+    $ $EDITOR tests/test_server.yaml
+    # check settings with a single test:
+    $ python -m pytest tests/test_user.py::test_get
+    # if OK, run all tests:
+    $ make test
+
+
+Logging
+-------
+
+Standard logging is used for tracking the libraries activity.
+To capture the log messages for this project, subscribe to a logger named ``ucsschool.kelvin.client``.
+*Attention:* Passwords and session tokens will be logged at log level ``DEBUG``!
+
+The *UCS\@school Kelvin REST API* on the UCS server logs into the file ``/var/log/univention/ucsschool-kelvin-rest-api/http.log``.
+The *UDM REST API* on the UCS server logs into the file ``/var/log/univention/directory-manager-rest.log``.
+
+Repo permissions
+----------------
+* Github: @dansan and @JuergenBS
+* Gitlab: @JuergenBS
+* PyPI: @dansan and @SamuelYaron
+* RTD: @dansan and @SamuelYaron
+
+Credits
+-------
+
+.. _`UCS\@school Kelvin REST API`: https://docs.software-univention.de/ucsschool-kelvin-rest-api/
+.. _`tox`: http://tox.readthedocs.org/
+.. _`docs`: https://kelvin-rest-api-client.readthedocs.io
+.. _`PyPI`: https://pypi.org/project/kelvin-rest-api-client/
+.. |license| image:: https://img.shields.io/badge/License-AGPL%20v3-orange.svg
+    :alt: GNU AGPL V3 license
+    :target: https://www.gnu.org/licenses/agpl-3.0
+.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+    :alt: Python 3.7+
+    :target: https://www.python.org/
+.. |code style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :alt: Code style: black
+    :target: https://github.com/psf/black
+.. |codecov| image:: https://codecov.io/gh/univention/kelvin-rest-api-client/branch/master/graph/badge.svg
+    :alt: Code coverage
+    :target: https://codecov.io/gh/univention/kelvin-rest-api-client
+.. |docspassing| image:: https://readthedocs.org/projects/kelvin-rest-api-client/badge/?version=latest
+    :alt: Documentation Status
+    :target: https://kelvin-rest-api-client.readthedocs.io/en/latest/?badge=latest
+.. |travisci| image:: https://travis-ci.com/univention/kelvin-rest-api-client.svg?branch=master
+    :target: https://app.travis-ci.com/github/univention/kelvin-rest-api-client
+.. |bandit| image:: https://img.shields.io/badge/security-bandit-yellow.svg
+    :alt: Security: bandit
+    :target: https://github.com/PyCQA/bandit
+.. |gh Code Linting| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Code%20Linting/badge.svg
+    :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Code+Linting%22
+.. |gh Integration tests| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Integration%20tests/badge.svg
+    :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
+
+
+=======
+History
+=======
+
+2.2.2 (2023-04-14)
+------------------
+
+* Support HEAD for ``SchoolClass``, ``User``, ``WorkGroup``, and ``Role``.
+
+2.2.1 (2022-12-15)
+------------------
+
+* Use deepcopy in ``to_dict`` method to prevent values of ``udm_properties`` from being updated in objects which are copied.
+
+2.2.0 (2022-10-13)
+--------------------
+
+* Support Http ``Accept-Language`` Header.
+
+2.1.0 (2022-10-07)
+--------------------
+
+* Support HEAD for ``School``.
+
+2.0.1 (2022-10-05)
+--------------------
+
+* Use detailed upstream error message in ``InvalidRequest`` exception messages.
+
+2.0.0 (2022-09-10)
+--------------------
+
+* **API Change**: The required argument ``school`` in the ``User`` constructor has now the default argument ``None``. The argument ``name`` is not required anymore. Optional values, which are set to ``None``, are not passed to the Kelvin server anymore. This enables automatic value generation on the Kelvin REST API server. To make use of this, the attributes can be either set to ``None``, the empty string ``""`` or left out completely. Additionally, you have to create a schema for the corresponding attribute on the Kelvin REST API server.
+* Send a correlation ID with each request.
+
+1.7.1 (2022-08-30)
+--------------------
+
+* Loosen dependency constraints.
+
+1.7.0 (2022-07-07)
+--------------------
+
+* Support user ``workgroups`` attribute.
+
+1.6.1 (2022-06-30)
+--------------------
+
+* Ignore unknown attributes in KelvinObject child classes.
+
+1.6.0 (2022-06-27)
+--------------------
+
+* Add support for workgroup resource.
+
+1.5.2.1 (2022-04-05)
+--------------------
+
+* Fixed: Logger does replace values of credentials with placeholders.
+
+1.5.2 (2022-02-22)
+------------------
+
+* Automatic tests now run with Python 3.7 - 3.10.
+* Fixed: The timeout attribute from a session instance is now used for requests.
+
+1.5.1 (2021-11-30)
+------------------
+
+* Add attribute ``expiration_date`` to the ``User`` class. The attribute was added to the Kelvin REST API app in version ``1.5.1``.
+
+1.5.0 (2021-09-21)
+------------------
+
+* Add attribute ``udm_properties`` to classes ``School`` and ``SchoolClass``.  The attributes were added to the Kelvin REST API app in version ``1.5.0``.
+
+0.3.0 (2021-05-04)
+------------------
+
+* Add support for the creation of school (OU) objects.
+
+0.2.2 (2020-11-09)
+------------------
+
+* Add support for the ``kelvin_password_hashes`` attribute of the ``User`` class.
+
+0.2.1 (2020-08-07)
+------------------
+
+* fix JWT token validity calculation: timestamp uses UTC
+* documentation fixes
+* dependency updates
+* tests also run on Python 3.9-dev
+
+0.2.0 (2020-04-17)
+------------------
+
+* move tox to test requirements
+* fix user object creation with default parameters
+* change ``as_dict`` to be a method instead of a property
+* fix flaky tests
+* improve test coverage
+* pass more env args to tox
+* fix AttributeError with repr(role)
+* add complete usage documentation
+
+0.1.0 (2020-04-16)
+------------------
+
+* First release.
```

### Comparing `kelvin-rest-api-client-2.2.1/README.rst` & `kelvin-rest-api-client-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/Makefile` & `kelvin-rest-api-client-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/conf.py` & `kelvin-rest-api-client-2.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/installation.rst` & `kelvin-rest-api-client-2.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/make.bat` & `kelvin-rest-api-client-2.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/ucsschool.kelvin.client.rst` & `kelvin-rest-api-client-2.2.2/docs/ucsschool.kelvin.client.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-auth.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-auth.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-correlation.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-correlation.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-language.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-language.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-role.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-role.rst`

 * *Files 7% similar despite different names*

```diff
@@ -91,14 +91,28 @@
 
     role.as_dict()
     {'name': 'student',
      'display_name': 'student',
      'url': 'https://master.ucs.local/ucsschool/kelvin/v1/roles/student'}
 
 
+Check if role exists
+--------------------
+
+.. code-block:: python
+
+    from ucsschool.kelvin.client import Session, RoleResource
+
+    async with Session(**credentials) as session:
+        if await RoleResource(session=session).exists(name="student"):
+            print("The role 'student' exists!")
+
+Note: This method only works with Kelvin server version 1.8.8 or newer.
+
+
 Search roles
 ------------
 
 The :py:meth:`search()` method allows searching for roles.
 No filter argument are supported.
 
 .. code-block:: python
```

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-school-class.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-school-class.rst`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,26 @@
      'description': 'A test class',
      'users': ['demo_student', 'demo_teacher'],
      'create_share': True,
      'dn': 'cn=DEMOSCHOOL-testclass,cn=klassen,cn=schueler,cn=groups,ou=DEMOSCHOOL,dc=example,dc=com',
      'url': 'https://10.200.3.70/ucsschool/kelvin/v1/classes/DEMOSCHOOL/testclass'}
 
 
+Check if school class exists
+----------------------------
+
+.. code-block:: python
+
+    from ucsschool.kelvin.client import Session, SchoolClassResource
+
+    async with Session(**credentials) as session:
+        if await SchoolClassResource(session=session).exists(name="testclass", school="DEMOSCHOOL"):
+            print("The school class exists!")
+
+
 Search school classes
 ---------------------
 
 The :py:meth:`search()` method allows searching for school classes, filtering by ``school`` (mandatory) and ``name`` (optional).
 
 The mandatory ``school`` argument must be exact while the optional ``name`` argument support an inexact search using ``*`` as a placeholder.
```

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-school.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-school.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-users.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-users.rst`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,26 @@
      'workgroups': {},
      'source_uid': 'TESTID',
      'udm_properties': {},
      'dn': 'uid=test1,cn=schueler,cn=users,ou=DEMOSCHOOL,dc=example,dc=com',
      'url': 'https://master.ucs.local/ucsschool/kelvin/v1/users/test1'}
 
 
+Check if user exists
+--------------------
+
+.. code-block:: python
+
+    from ucsschool.kelvin.client import Session, UserResource
+
+    async with Session(**credentials) as session:
+        if await UserResource(session=session).exists(name="test1"):
+            print("The user exists!")
+
+
 Search users
 ------------
 
 The :py:meth:`search()` method allows searching for users, using a number of filters.
 Most (but now all) attributes support searching inexact, using an asterisk (``*``) as placeholder.
 
 In the following examples the search is always limited to users of the school ``DEMOSCHOOL``.
```

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage-workgroups.rst` & `kelvin-rest-api-client-2.2.2/docs/usage-workgroups.rst`

 * *Files 7% similar despite different names*

```diff
@@ -201,14 +201,26 @@
      'description': 'A test workgroup',
      'users': ['demo_student', 'demo_teacher'],
      'create_share': True,
      'dn': 'cn=DEMOSCHOOL-testworkgroup,cn=schueler,cn=groups,ou=DEMOSCHOOL,dc=example,dc=com',
      'url': 'https://10.200.3.70/ucsschool/kelvin/v1/workgroups/DEMOSCHOOL/testworkgroup'}
 
 
+Check if workgroup exists
+-------------------------
+
+.. code-block:: python
+
+    from ucsschool.kelvin.client import Session, WorkGroupResource
+
+    async with Session(**credentials) as session:
+        if await WorkGroupResource(session=session).exists(school="DEMOSCHOOL", name="testworkgroup"):
+            print("The workgroup exists!")
+
+
 Search workgroups
 ---------------------
 
 The :py:meth:`search()` method allows searching for workgroups, filtering by ``school`` (mandatory) and ``name`` (optional).
 
 The mandatory ``school`` argument must be exact while the optional ``name`` argument support an inexact search using ``*`` as a placeholder.
```

### Comparing `kelvin-rest-api-client-2.2.1/docs/usage.rst` & `kelvin-rest-api-client-2.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/PKG-INFO` & `kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,351 +1,356 @@
 Metadata-Version: 2.1
 Name: kelvin-rest-api-client
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python library to interact with the UCS@school Kelvin REST API.
 Home-page: https://github.com/univention/kelvin-rest-api-client
 Author: Daniel Troeder
 Author-email: troeder@univention.de
 License: GNU Affero General Public License v3
-Description: =========================================
-        Python UCS\@school Kelvin REST API Client
-        =========================================
-        
-        |python| |license| |code style| |bandit| |codecov| |docspassing| |gh Code Linting| |gh Integration tests|
-        
-        Python library to interact with the `UCS\@school Kelvin REST API`_.
-        
-        * Free software: GNU Affero General Public License version 3
-        * Documentation: https://kelvin-rest-api-client.readthedocs.io
-        
-        
-        Features
-        --------
-        
-        * Asynchronous
-        * Automatic handling of HTTP(S) sessions
-        * Type annotations
-        * ~95% test coverage (unittests + integration tests)
-        * Python 3.7, 3.8, 3.9, 3.10
-        
-        Compatibility
-        -------------
-        
-        A list of UCS\@school Kelvin REST API server versions which introduce breaking changes can be found in the [UCS\@school Kelvin REST API Documentation](https://docs.software-univention.de/ucsschool-kelvin-rest-api/kelvin-client-compatibility.html).
-        
-        
-        Usage
-        -----
-        
-        The ``Session`` context manager opens and closes a HTTP session:
-        
-        .. code-block:: python
-        
-            >>> import asyncio
-            >>> from ucsschool.kelvin.client import Session, User, UserResource
-            >>>
-            >>> async def get_user(username: str) -> User:
-            ...     async with Session(
-            ...         "USERNAME",
-            ...         "PASSWORD",
-            ...         "master.ucs.local",
-            ...         verify="ucs-root-ca.crt"
-            ...     ) as session:
-            ...         return await UserResource(session=session).get(name=username)
-            ...
-            >>> obj = asyncio.run(get_user("demo_student"))
-            >>>
-            >>> print(obj)
-            User('name'='test_user', dn='uid=test_user,cn=schueler,cn=users,ou=DEMOSCHOOL,dc=example,dc=com')
-            >>> print(obj.firstname, obj.lastname)
-            Test User
-        
-        There are more examples in the `docs`_ *usage* section.
-        
-        For HTTPS to work, the SSL CA of the target system (UCS Master) must either be publicly signed, installed on the client system or available as file (as in the example above).
-        If the SSL CA certificate is not available ``verify=False``.
-        Obviously that is *not safe*! The CA of any UCS server can always be downloaded from ``http://FQDN.OF.UCS/ucs-root-ca.crt``.
-        
-        
-        Installation
-        ------------
-        
-        Install *UCS\@school Kelvin REST API Client* via pip from `PyPI`_:
-        
-        .. code-block:: console
-        
-            $ pip install kelvin-rest-api-client
-        
-        
-        Tests
-        -----
-        
-        There are some isolated unittests, but most tests run against a real *UCS\@school Kelvin REST API*.
-        A UCS Docker container has been prepared for this (additionally to the Kelvin API Docker container).
-        The ``Makefile`` automates downloading and starting the Docker containers (3.2 GB GB) and running the tests.
-        It is also possible to use an existing UCS DC Master with UCS\@school and the Kelvin API installed.
-        
-        The tests expect the existence of two schools (``OUs``) on the target system (the Kelvin API does not support creation of schools yet).
-        The schools are ``DEMOSCHOOL`` and ``DEMOSCHOOL2``.
-        The first one usually already exists, but trying to create it again is safe.
-        To create the schools run *on the UCS DC Master*:
-        
-        .. code-block:: console
-        
-            $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL
-            $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL2
-        
-        Furthermore an email domain must exist:
-        
-        .. code-block:: console
-        
-            $ udm mail/domain create \
-                --ignore_exists \
-                --position "cn=domain,cn=mail,$(ucr get ldap/base)" \
-                --set name="$(ucr get domainname)"
-        
-        Since version ``1.5.0`` the Kelvin REST API supports UDM properties in all resources. A configuration is required for the tests for this feature:
-        
-        .. code-block:: console
-        
-            $ cat > /etc/ucsschool/kelvin/mapped_udm_properties.json <<__EOF__
-            {
-                "user": ["title"],
-                "school_class": ["mailAddress"],
-                "school": ["description"]
-            }
-            __EOF__
-        
-        The provided UCS Docker containers already contain both OUs.
-        They can be started using the Makefile:
-        
-        .. code-block:: console
-        
-            $ make start-docker-containers
-        
-            Downloading Docker image '..-ucsschool-udm-rest-api-only:stable-4.4-8'...
-            Downloading Docker image '../ucsschool-kelvin-rest-api:1.5.5'...
-            Starting UCS docker container...
-            Waiting for UCS docker container to start...
-            Waiting for IP address of UCS container...
-            Waiting for UDM REST API...........
-            Creating Kelvin REST API container...
-            Configuring Kelvin REST API container...
-            Rebuilding the OpenAPI client library in the Kelvin API Container...
-            Starting Kelvin REST API server...
-            Waiting for Kelvin docker container to start...
-            Waiting for IP address of Kelvin container...
-            Waiting for Kelvin API...
-            Fixing log file permissions...
-            Setting up reverse proxy...
-            ==> UDM REST API log file: /tmp/udm-rest-api-log/directory-manager-rest.log
-            ==> UDM REST API: http://172.17.0.2/univention/udm/
-            ==> Kelvin API configs: /tmp/kelvin-api/configs/
-            ==> Kelvin API hooks: /tmp/kelvin-api/kelvin-hooks/
-            ==> Kelvin API log file: /tmp/kelvin-api/log/http.log
-            ==> Kelvin API: http://172.17.0.3:8911/ucsschool/kelvin/v1/docs
-            ==> Kelvin API: https://172.17.0.2/ucsschool/kelvin/v1/docs
-        
-        The Docker containers can be stopped and removed by running:
-        
-        .. code-block:: console
-        
-            $ make stop-and-remove-docker-containers
-        
-        The Docker images will not be removed, only the running containers.
-        
-        Run tests with current Python interpreter:
-        
-        .. code-block:: console
-        
-            $ make test
-        
-        Using `tox`_ the tests can be executed with all supported Python versions:
-        
-        .. code-block:: console
-        
-            $ make test-all
-        
-        To use an existing UCS server for the tests, copy the file ``tests/test_server_example.yaml`` to ``tests/test_server.yaml`` and adapt the settings before starting the tests:
-        
-        .. code-block:: console
-        
-            $ cp tests/test_server_example.yaml tests/test_server.yaml
-            $ $EDITOR tests/test_server.yaml
-            # check settings with a single test:
-            $ python -m pytest tests/test_user.py::test_get
-            # if OK, run all tests:
-            $ make test
-        
-        
-        Logging
-        -------
-        
-        Standard logging is used for tracking the libraries activity.
-        To capture the log messages for this project, subscribe to a logger named ``ucsschool.kelvin.client``.
-        *Attention:* Passwords and session tokens will be logged at log level ``DEBUG``!
-        
-        The *UCS\@school Kelvin REST API* on the UCS server logs into the file ``/var/log/univention/ucsschool-kelvin-rest-api/http.log``.
-        The *UDM REST API* on the UCS server logs into the file ``/var/log/univention/directory-manager-rest.log``.
-        
-        Repo permissions
-        ----------------
-        * Github: @dansan and @JuergenBS
-        * Gitlab: @JuergenBS
-        * PyPI: @dansan and @SamuelYaron
-        * RTD: @dansan and @SamuelYaron
-        
-        Credits
-        -------
-        
-        .. _`UCS\@school Kelvin REST API`: https://docs.software-univention.de/ucsschool-kelvin-rest-api/
-        .. _`tox`: http://tox.readthedocs.org/
-        .. _`docs`: https://kelvin-rest-api-client.readthedocs.io
-        .. _`PyPI`: https://pypi.org/project/kelvin-rest-api-client/
-        .. |license| image:: https://img.shields.io/badge/License-AGPL%20v3-orange.svg
-            :alt: GNU AGPL V3 license
-            :target: https://www.gnu.org/licenses/agpl-3.0
-        .. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
-            :alt: Python 3.7+
-            :target: https://www.python.org/
-        .. |code style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :alt: Code style: black
-            :target: https://github.com/psf/black
-        .. |codecov| image:: https://codecov.io/gh/univention/kelvin-rest-api-client/branch/master/graph/badge.svg
-            :alt: Code coverage
-            :target: https://codecov.io/gh/univention/kelvin-rest-api-client
-        .. |docspassing| image:: https://readthedocs.org/projects/kelvin-rest-api-client/badge/?version=latest
-            :alt: Documentation Status
-            :target: https://kelvin-rest-api-client.readthedocs.io/en/latest/?badge=latest
-        .. |travisci| image:: https://travis-ci.com/univention/kelvin-rest-api-client.svg?branch=master
-            :target: https://app.travis-ci.com/github/univention/kelvin-rest-api-client
-        .. |bandit| image:: https://img.shields.io/badge/security-bandit-yellow.svg
-            :alt: Security: bandit
-            :target: https://github.com/PyCQA/bandit
-        .. |gh Code Linting| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Code%20Linting/badge.svg
-            :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Code+Linting%22
-        .. |gh Integration tests| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Integration%20tests/badge.svg
-            :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
-        
-        
-        =======
-        History
-        =======
-        
-        2.2.1 (2022-12-15)
-        ------------------
-        
-        * Use deepcopy in ``to_dict`` method to prevent values of ``udm_properties`` from being updated in objects which are copied.
-        
-        2.2.0 (2022-10-13)
-        --------------------
-        
-        * Support Http ``Accept-Language`` Header.
-        
-        2.1.0 (2022-10-07)
-        --------------------
-        
-        * Support HEAD for ``School``.
-        
-        2.0.1 (2022-10-05)
-        --------------------
-        
-        * Use detailed upstream error message in ``InvalidRequest`` exception messages.
-        
-        2.0.0 (2022-09-10)
-        --------------------
-        
-        * **API Change**: The required argument ``school`` in the ``User`` constructor has now the default argument ``None``. The argument ``name`` is not required anymore. Optional values, which are set to ``None``, are not passed to the Kelvin server anymore. This enables automatic value generation on the Kelvin REST API server. To make use of this, the attributes can be either set to ``None``, the empty string ``""`` or left out completely. Additionally, you have to create a schema for the corresponding attribute on the Kelvin REST API server.
-        * Send a correlation ID with each request.
-        
-        1.7.1 (2022-08-30)
-        --------------------
-        
-        * Loosen dependency constraints.
-        
-        1.7.0 (2022-07-07)
-        --------------------
-        
-        * Support user ``workgroups`` attribute.
-        
-        1.6.1 (2022-06-30)
-        --------------------
-        
-        * Ignore unknown attributes in KelvinObject child classes.
-        
-        1.6.0 (2022-06-27)
-        --------------------
-        
-        * Add support for workgroup resource.
-        
-        1.5.2.1 (2022-04-05)
-        --------------------
-        
-        * Fixed: Logger does replace values of credentials with placeholders.
-        
-        1.5.2 (2022-02-22)
-        ------------------
-        
-        * Automatic tests now run with Python 3.7 - 3.10.
-        * Fixed: The timeout attribute from a session instance is now used for requests.
-        
-        1.5.1 (2021-11-30)
-        ------------------
-        
-        * Add attribute ``expiration_date`` to the ``User`` class. The attribute was added to the Kelvin REST API app in version ``1.5.1``.
-        
-        1.5.0 (2021-09-21)
-        ------------------
-        
-        * Add attribute ``udm_properties`` to classes ``School`` and ``SchoolClass``.  The attributes were added to the Kelvin REST API app in version ``1.5.0``.
-        
-        0.3.0 (2021-05-04)
-        ------------------
-        
-        * Add support for the creation of school (OU) objects.
-        
-        0.2.2 (2020-11-09)
-        ------------------
-        
-        * Add support for the ``kelvin_password_hashes`` attribute of the ``User`` class.
-        
-        0.2.1 (2020-08-07)
-        ------------------
-        
-        * fix JWT token validity calculation: timestamp uses UTC
-        * documentation fixes
-        * dependency updates
-        * tests also run on Python 3.9-dev
-        
-        0.2.0 (2020-04-17)
-        ------------------
-        
-        * move tox to test requirements
-        * fix user object creation with default parameters
-        * change ``as_dict`` to be a method instead of a property
-        * fix flaky tests
-        * improve test coverage
-        * pass more env args to tox
-        * fix AttributeError with repr(role)
-        * add complete usage documentation
-        
-        0.1.0 (2020-04-16)
-        ------------------
-        
-        * First release.
-        
 Keywords: Univention UCS UCS@school REST
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: development
+License-File: LICENSE
+
+=========================================
+Python UCS\@school Kelvin REST API Client
+=========================================
+
+|python| |license| |code style| |bandit| |codecov| |docspassing| |gh Code Linting| |gh Integration tests|
+
+Python library to interact with the `UCS\@school Kelvin REST API`_.
+
+* Free software: GNU Affero General Public License version 3
+* Documentation: https://kelvin-rest-api-client.readthedocs.io
+
+
+Features
+--------
+
+* Asynchronous
+* Automatic handling of HTTP(S) sessions
+* Type annotations
+* ~95% test coverage (unittests + integration tests)
+* Python 3.7, 3.8, 3.9, 3.10
+
+Compatibility
+-------------
+
+A list of UCS\@school Kelvin REST API server versions which introduce breaking changes can be found in the [UCS\@school Kelvin REST API Documentation](https://docs.software-univention.de/ucsschool-kelvin-rest-api/kelvin-client-compatibility.html).
+
+
+Usage
+-----
+
+The ``Session`` context manager opens and closes a HTTP session:
+
+.. code-block:: python
+
+    >>> import asyncio
+    >>> from ucsschool.kelvin.client import Session, User, UserResource
+    >>>
+    >>> async def get_user(username: str) -> User:
+    ...     async with Session(
+    ...         "USERNAME",
+    ...         "PASSWORD",
+    ...         "master.ucs.local",
+    ...         verify="ucs-root-ca.crt"
+    ...     ) as session:
+    ...         return await UserResource(session=session).get(name=username)
+    ...
+    >>> obj = asyncio.run(get_user("demo_student"))
+    >>>
+    >>> print(obj)
+    User('name'='test_user', dn='uid=test_user,cn=schueler,cn=users,ou=DEMOSCHOOL,dc=example,dc=com')
+    >>> print(obj.firstname, obj.lastname)
+    Test User
+
+There are more examples in the `docs`_ *usage* section.
+
+For HTTPS to work, the SSL CA of the target system (UCS Master) must either be publicly signed, installed on the client system or available as file (as in the example above).
+If the SSL CA certificate is not available ``verify=False``.
+Obviously that is *not safe*! The CA of any UCS server can always be downloaded from ``http://FQDN.OF.UCS/ucs-root-ca.crt``.
+
+
+Installation
+------------
+
+Install *UCS\@school Kelvin REST API Client* via pip from `PyPI`_:
+
+.. code-block:: console
+
+    $ pip install kelvin-rest-api-client
+
+
+Tests
+-----
+
+There are some isolated unittests, but most tests run against a real *UCS\@school Kelvin REST API*.
+A UCS Docker container has been prepared for this (additionally to the Kelvin API Docker container).
+The ``Makefile`` automates downloading and starting the Docker containers (3.2 GB GB) and running the tests.
+It is also possible to use an existing UCS DC Master with UCS\@school and the Kelvin API installed.
+
+The tests expect the existence of two schools (``OUs``) on the target system (the Kelvin API does not support creation of schools yet).
+The schools are ``DEMOSCHOOL`` and ``DEMOSCHOOL2``.
+The first one usually already exists, but trying to create it again is safe.
+To create the schools run *on the UCS DC Master*:
+
+.. code-block:: console
+
+    $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL
+    $ /usr/share/ucs-school-import/scripts/create_ou DEMOSCHOOL2
+
+Furthermore an email domain must exist:
+
+.. code-block:: console
+
+    $ udm mail/domain create \
+        --ignore_exists \
+        --position "cn=domain,cn=mail,$(ucr get ldap/base)" \
+        --set name="$(ucr get domainname)"
+
+Since version ``1.5.0`` the Kelvin REST API supports UDM properties in all resources. A configuration is required for the tests for this feature:
+
+.. code-block:: console
+
+    $ cat > /etc/ucsschool/kelvin/mapped_udm_properties.json <<__EOF__
+    {
+        "user": ["title"],
+        "school_class": ["mailAddress"],
+        "school": ["description"]
+    }
+    __EOF__
+
+The provided UCS Docker containers already contain both OUs.
+They can be started using the Makefile:
+
+.. code-block:: console
+
+    $ make start-docker-containers
+
+    Downloading Docker image '..-ucsschool-udm-rest-api-only:stable-4.4-8'...
+    Downloading Docker image '../ucsschool-kelvin-rest-api:1.5.5'...
+    Starting UCS docker container...
+    Waiting for UCS docker container to start...
+    Waiting for IP address of UCS container...
+    Waiting for UDM REST API...........
+    Creating Kelvin REST API container...
+    Configuring Kelvin REST API container...
+    Rebuilding the OpenAPI client library in the Kelvin API Container...
+    Starting Kelvin REST API server...
+    Waiting for Kelvin docker container to start...
+    Waiting for IP address of Kelvin container...
+    Waiting for Kelvin API...
+    Fixing log file permissions...
+    Setting up reverse proxy...
+    ==> UDM REST API log file: /tmp/udm-rest-api-log/directory-manager-rest.log
+    ==> UDM REST API: http://172.17.0.2/univention/udm/
+    ==> Kelvin API configs: /tmp/kelvin-api/configs/
+    ==> Kelvin API hooks: /tmp/kelvin-api/kelvin-hooks/
+    ==> Kelvin API log file: /tmp/kelvin-api/log/http.log
+    ==> Kelvin API: http://172.17.0.3:8911/ucsschool/kelvin/v1/docs
+    ==> Kelvin API: https://172.17.0.2/ucsschool/kelvin/v1/docs
+
+The Docker containers can be stopped and removed by running:
+
+.. code-block:: console
+
+    $ make stop-and-remove-docker-containers
+
+The Docker images will not be removed, only the running containers.
+
+Run tests with current Python interpreter:
+
+.. code-block:: console
+
+    $ make test
+
+Using `tox`_ the tests can be executed with all supported Python versions:
+
+.. code-block:: console
+
+    $ make test-all
+
+To use an existing UCS server for the tests, copy the file ``tests/test_server_example.yaml`` to ``tests/test_server.yaml`` and adapt the settings before starting the tests:
+
+.. code-block:: console
+
+    $ cp tests/test_server_example.yaml tests/test_server.yaml
+    $ $EDITOR tests/test_server.yaml
+    # check settings with a single test:
+    $ python -m pytest tests/test_user.py::test_get
+    # if OK, run all tests:
+    $ make test
+
+
+Logging
+-------
+
+Standard logging is used for tracking the libraries activity.
+To capture the log messages for this project, subscribe to a logger named ``ucsschool.kelvin.client``.
+*Attention:* Passwords and session tokens will be logged at log level ``DEBUG``!
+
+The *UCS\@school Kelvin REST API* on the UCS server logs into the file ``/var/log/univention/ucsschool-kelvin-rest-api/http.log``.
+The *UDM REST API* on the UCS server logs into the file ``/var/log/univention/directory-manager-rest.log``.
+
+Repo permissions
+----------------
+* Github: @dansan and @JuergenBS
+* Gitlab: @JuergenBS
+* PyPI: @dansan and @SamuelYaron
+* RTD: @dansan and @SamuelYaron
+
+Credits
+-------
+
+.. _`UCS\@school Kelvin REST API`: https://docs.software-univention.de/ucsschool-kelvin-rest-api/
+.. _`tox`: http://tox.readthedocs.org/
+.. _`docs`: https://kelvin-rest-api-client.readthedocs.io
+.. _`PyPI`: https://pypi.org/project/kelvin-rest-api-client/
+.. |license| image:: https://img.shields.io/badge/License-AGPL%20v3-orange.svg
+    :alt: GNU AGPL V3 license
+    :target: https://www.gnu.org/licenses/agpl-3.0
+.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+    :alt: Python 3.7+
+    :target: https://www.python.org/
+.. |code style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :alt: Code style: black
+    :target: https://github.com/psf/black
+.. |codecov| image:: https://codecov.io/gh/univention/kelvin-rest-api-client/branch/master/graph/badge.svg
+    :alt: Code coverage
+    :target: https://codecov.io/gh/univention/kelvin-rest-api-client
+.. |docspassing| image:: https://readthedocs.org/projects/kelvin-rest-api-client/badge/?version=latest
+    :alt: Documentation Status
+    :target: https://kelvin-rest-api-client.readthedocs.io/en/latest/?badge=latest
+.. |travisci| image:: https://travis-ci.com/univention/kelvin-rest-api-client.svg?branch=master
+    :target: https://app.travis-ci.com/github/univention/kelvin-rest-api-client
+.. |bandit| image:: https://img.shields.io/badge/security-bandit-yellow.svg
+    :alt: Security: bandit
+    :target: https://github.com/PyCQA/bandit
+.. |gh Code Linting| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Code%20Linting/badge.svg
+    :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Code+Linting%22
+.. |gh Integration tests| image:: https://github.com/univention/kelvin-rest-api-client/workflows/Integration%20tests/badge.svg
+    :target: https://github.com/univention/kelvin-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
+
+
+=======
+History
+=======
+
+2.2.2 (2023-04-14)
+------------------
+
+* Support HEAD for ``SchoolClass``, ``User``, ``WorkGroup``, and ``Role``.
+
+2.2.1 (2022-12-15)
+------------------
+
+* Use deepcopy in ``to_dict`` method to prevent values of ``udm_properties`` from being updated in objects which are copied.
+
+2.2.0 (2022-10-13)
+--------------------
+
+* Support Http ``Accept-Language`` Header.
+
+2.1.0 (2022-10-07)
+--------------------
+
+* Support HEAD for ``School``.
+
+2.0.1 (2022-10-05)
+--------------------
+
+* Use detailed upstream error message in ``InvalidRequest`` exception messages.
+
+2.0.0 (2022-09-10)
+--------------------
+
+* **API Change**: The required argument ``school`` in the ``User`` constructor has now the default argument ``None``. The argument ``name`` is not required anymore. Optional values, which are set to ``None``, are not passed to the Kelvin server anymore. This enables automatic value generation on the Kelvin REST API server. To make use of this, the attributes can be either set to ``None``, the empty string ``""`` or left out completely. Additionally, you have to create a schema for the corresponding attribute on the Kelvin REST API server.
+* Send a correlation ID with each request.
+
+1.7.1 (2022-08-30)
+--------------------
+
+* Loosen dependency constraints.
+
+1.7.0 (2022-07-07)
+--------------------
+
+* Support user ``workgroups`` attribute.
+
+1.6.1 (2022-06-30)
+--------------------
+
+* Ignore unknown attributes in KelvinObject child classes.
+
+1.6.0 (2022-06-27)
+--------------------
+
+* Add support for workgroup resource.
+
+1.5.2.1 (2022-04-05)
+--------------------
+
+* Fixed: Logger does replace values of credentials with placeholders.
+
+1.5.2 (2022-02-22)
+------------------
+
+* Automatic tests now run with Python 3.7 - 3.10.
+* Fixed: The timeout attribute from a session instance is now used for requests.
+
+1.5.1 (2021-11-30)
+------------------
+
+* Add attribute ``expiration_date`` to the ``User`` class. The attribute was added to the Kelvin REST API app in version ``1.5.1``.
+
+1.5.0 (2021-09-21)
+------------------
+
+* Add attribute ``udm_properties`` to classes ``School`` and ``SchoolClass``.  The attributes were added to the Kelvin REST API app in version ``1.5.0``.
+
+0.3.0 (2021-05-04)
+------------------
+
+* Add support for the creation of school (OU) objects.
+
+0.2.2 (2020-11-09)
+------------------
+
+* Add support for the ``kelvin_password_hashes`` attribute of the ``User`` class.
+
+0.2.1 (2020-08-07)
+------------------
+
+* fix JWT token validity calculation: timestamp uses UTC
+* documentation fixes
+* dependency updates
+* tests also run on Python 3.9-dev
+
+0.2.0 (2020-04-17)
+------------------
+
+* move tox to test requirements
+* fix user object creation with default parameters
+* change ``as_dict`` to be a method instead of a property
+* fix flaky tests
+* improve test coverage
+* pass more env args to tox
+* fix AttributeError with repr(role)
+* add complete usage documentation
+
+0.1.0 (2020-04-16)
+------------------
+
+* First release.
```

### Comparing `kelvin-rest-api-client-2.2.1/kelvin_rest_api_client.egg-info/SOURCES.txt` & `kelvin-rest-api-client-2.2.2/kelvin_rest_api_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -55,13 +55,14 @@
 tests/test_session.py
 tests/test_test.py
 tests/test_user.py
 tests/test_workgroup.py
 ucsschool/kelvin/client/__init__.py
 ucsschool/kelvin/client/base.py
 ucsschool/kelvin/client/exceptions.py
+ucsschool/kelvin/client/py.typed
 ucsschool/kelvin/client/role.py
 ucsschool/kelvin/client/school.py
 ucsschool/kelvin/client/school_class.py
 ucsschool/kelvin/client/session.py
 ucsschool/kelvin/client/user.py
 ucsschool/kelvin/client/workgroup.py
```

### Comparing `kelvin-rest-api-client-2.2.1/setup.py` & `kelvin-rest-api-client-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/conftest.py` & `kelvin-rest-api-client-2.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_kelvin_object_init.py` & `kelvin-rest-api-client-2.2.2/tests/test_kelvin_object_init.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_logger.py` & `kelvin-rest-api-client-2.2.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_role.py` & `kelvin-rest-api-client-2.2.2/tests/test_role.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License with the Debian GNU/Linux or Univention distribution in file
 # /usr/share/common-licenses/AGPL-3; if not, see
 # <http://www.gnu.org/licenses/>.
 
+import asyncio
 import random
+from unittest.mock import patch
 
 import pytest
 from faker import Faker
 
 from ucsschool.kelvin.client import RoleResource, Session
 
 fake = Faker()
@@ -77,7 +79,29 @@
 async def test_role_attrs(compare_kelvin_obj_with_test_data, kelvin_session_kwargs):
     role = random.choice(("staff", "student", "teacher"))
     async with Session(**kelvin_session_kwargs) as session:
         obj = await RoleResource(session=session).get(name=role)
     assert obj.name == role
     assert set(obj._kelvin_attrs) == {"name", "display_name"}
     assert set(obj.as_dict().keys()) == {"name", "display_name", "url"}
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("role", ["staff", "student", "teacher"])
+async def test_exists(kelvin_session_kwargs, role):
+    async with Session(**kelvin_session_kwargs) as session:
+        await RoleResource(session=session).exists(name=role)
+        with patch("ucsschool.kelvin.client.session.Session.head") as mock:
+            f = asyncio.Future()
+            f.set_result(True)
+            mock.return_value = f
+            await RoleResource(session=session).exists(name=role)
+
+            mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_exists_non_existing(kelvin_session_kwargs):
+    async with Session(**kelvin_session_kwargs) as session:
+        assert not await RoleResource(session=session).exists(
+            name=fake.user_name(),
+        )
```

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_school.py` & `kelvin-rest-api-client-2.2.2/tests/test_school.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,16 @@
         await ldap_access.modify(obj.dn, {"displayName": [(ldap3.MODIFY_REPLACE, [display_name_new])]})
         await obj.reload()
         assert obj.display_name == display_name_new
         await ldap_access.modify(obj.dn, {"displayName": [(ldap3.MODIFY_REPLACE, [display_name_old])]})
 
 
 @pytest.mark.asyncio
-async def test_exists(kelvin_session_kwargs, new_school, schedule_delete_ou_using_ssh):
+async def test_exists(kelvin_session_kwargs, new_school):
     school = new_school(1)[0]
-    # schedule_delete_ou_using_ssh(school.name)
     async with Session(**kelvin_session_kwargs) as session:
         assert await SchoolResource(session=session).exists(name=school.name)
         assert not await SchoolResource(session=session).exists(name="DOESNOTEXIST")
         with patch("ucsschool.kelvin.client.session.Session.head") as mock:
             f = asyncio.Future()
             f.set_result(True)
             mock.return_value = f
```

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_school_class.py` & `kelvin-rest-api-client-2.2.2/tests/test_school_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License with the Debian GNU/Linux or Univention distribution in file
 # /usr/share/common-licenses/AGPL-3; if not, see
 # <http://www.gnu.org/licenses/>.
 
+import asyncio
 from dataclasses import asdict
+from unittest.mock import patch
 
 import ldap3
 import pytest
 from faker import Faker
 
 from ucsschool.kelvin.client import InvalidRequest, NoObject, SchoolClass, SchoolClassResource, Session
 
@@ -343,7 +345,27 @@
         obj: SchoolClass = await SchoolClassResource(session=session).get(school=school, name=name)
         assert obj.description == description_old
         await obj.reload()
         assert obj.description == description_old
         await ldap_access.modify(obj.dn, {"description": [(ldap3.MODIFY_REPLACE, [description_new])]})
         await obj.reload()
         assert obj.description == description_new
+
+
+@pytest.mark.asyncio
+async def test_exists(kelvin_session_kwargs, new_school_class):
+    sc1_dn, sc1_attr = await new_school_class()
+    async with Session(**kelvin_session_kwargs) as session:
+        assert await SchoolClassResource(session=session).exists(
+            name=sc1_attr["name"], school=sc1_attr["school"]
+        )
+        assert not await SchoolClassResource(session=session).exists(
+            name="DOESNOTEXIST", school=sc1_attr["school"]
+        )
+        with patch("ucsschool.kelvin.client.session.Session.head") as mock:
+            f = asyncio.Future()
+            f.set_result(True)
+            mock.return_value = f
+            await SchoolClassResource(session=session).exists(
+                name=sc1_attr["name"], school=sc1_attr["school"]
+            )
+            mock.assert_called_once()
```

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_session.py` & `kelvin-rest-api-client-2.2.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_test.py` & `kelvin-rest-api-client-2.2.2/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_user.py` & `kelvin-rest-api-client-2.2.2/tests/test_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License with the Debian GNU/Linux or Univention distribution in file
 # /usr/share/common-licenses/AGPL-3; if not, see
 # <http://www.gnu.org/licenses/>.
 
+import asyncio
 import time
 from dataclasses import asdict
+from unittest.mock import patch
 
 import ldap3
 import pytest
 from faker import Faker
 
 from ucsschool.kelvin.client import (
     InvalidRequest,
@@ -532,7 +534,21 @@
     async with Session(**kelvin_session_kwargs) as session:
         old_obj: User = await UserResource(session=session).get(school=user.school, name=user.name)
         old_obj.udm_properties["title"] = "before"
 
         new_user = User(**old_obj.as_dict(), session=session)
         new_user.udm_properties["title"] = "after"
         assert old_obj.udm_properties["title"] != new_user.udm_properties["title"]
+
+
+@pytest.mark.asyncio
+async def test_exists(kelvin_session_kwargs, new_school_user):
+    user = await new_school_user()
+    async with Session(**kelvin_session_kwargs) as session:
+        assert await UserResource(session=session).exists(name=user.name)
+        assert not await UserResource(session=session).exists(name="DOESNOTEXIST")
+        with patch("ucsschool.kelvin.client.session.Session.head") as mock:
+            f = asyncio.Future()
+            f.set_result(True)
+            mock.return_value = f
+            await UserResource(session=session).exists(name=user.name)
+            mock.assert_called_once()
```

### Comparing `kelvin-rest-api-client-2.2.1/tests/test_workgroup.py` & `kelvin-rest-api-client-2.2.2/tests/test_workgroup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License with the Debian GNU/Linux or Univention distribution in file
 # /usr/share/common-licenses/AGPL-3; if not, see
 # <http://www.gnu.org/licenses/>.
 
+import asyncio
 from dataclasses import asdict
+from unittest.mock import patch
 
 import ldap3
 import pytest
 from faker import Faker
 
 from ucsschool.kelvin.client import InvalidRequest, NoObject, Session, WorkGroup, WorkGroupResource
 
@@ -300,7 +302,25 @@
         obj: WorkGroup = await WorkGroupResource(session=session).get(school=school, name=name)
         assert obj.description == description_old
         await obj.reload()
         assert obj.description == description_old
         await ldap_access.modify(obj.dn, {"description": [(ldap3.MODIFY_REPLACE, [description_new])]})
         await obj.reload()
         assert obj.description == description_new
+
+
+@pytest.mark.asyncio
+async def test_exists(kelvin_session_kwargs, new_workgroup):
+    wg1_dn, wg1_attr = await new_workgroup()
+    async with Session(**kelvin_session_kwargs) as session:
+        await WorkGroupResource(session=session).exists(name=wg1_attr["name"], school=wg1_attr["school"])
+        assert not await WorkGroupResource(session=session).exists(
+            name="DOESNOTEXIST", school=wg1_attr["school"]
+        )
+        with patch("ucsschool.kelvin.client.session.Session.head") as mock:
+            f = asyncio.Future()
+            f.set_result(True)
+            mock.return_value = f
+            await WorkGroupResource(session=session).exists(
+                name=wg1_attr["name"], school=wg1_attr["school"]
+            )
+            mock.assert_called_once()
```

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/__init__.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/base.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/base.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/exceptions.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/role.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/role.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,13 +81,14 @@
         return dict((attr, getattr(self, attr)) for attr in attrs)
 
 
 class RoleResource(KelvinResource):
     class Meta:
         kelvin_object: Type[KelvinObject] = Role
         required_get_attrs: Iterable[str] = ("name",)
+        required_head_attrs: Iterable[str] = ("name",)
         required_search_attrs: Iterable[str] = ()
 
     def __init__(self, session: Session, language: str = None):
         super().__init__(session=session, language=language)
         self.collection_url = self.session.urls["role"]
         self.object_url = f"{self.session.urls['role']}{{name}}"
```

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/school.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/school.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/school_class.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/school_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 
 class SchoolClassResource(KelvinResource):
     class Meta:
         kelvin_object: Type[KelvinObject] = SchoolClass
         required_get_attrs: Iterable[str] = ("name", "school")
         required_save_attrs: Iterable[str] = ("name", "school")
+        required_head_attrs: Iterable[str] = ("name",)
         required_search_attrs: Iterable[str] = ("school",)
 
     def __init__(self, session: Session, language: str = None):
         super().__init__(session=session, language=language)
         self.collection_url = self.session.urls["class"]
         self.object_url = f"{self.session.urls['class']}{{school}}/{{name}}"
```

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/session.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/session.py`

 * *Files identical despite different names*

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/user.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 
 
 class UserResource(KelvinResource):
     class Meta:
         kelvin_object: Type[KelvinObject] = User
         required_get_attrs: Iterable[str] = ("name",)
         required_save_attrs: Iterable[str] = ("school", "roles")
+        required_head_attrs: Iterable[str] = ("name",)
         required_search_attrs: Iterable[str] = ()
 
     def __init__(self, session: Session, language: str = None):
         super().__init__(session=session, language=language)
         self.collection_url = self.session.urls["user"]
         self.object_url = f"{self.session.urls['user']}{{name}}"
```

### Comparing `kelvin-rest-api-client-2.2.1/ucsschool/kelvin/client/workgroup.py` & `kelvin-rest-api-client-2.2.2/ucsschool/kelvin/client/workgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 
 class WorkGroupResource(KelvinResource):
     class Meta:
         kelvin_object: Type[KelvinObject] = WorkGroup
         required_get_attrs: Iterable[str] = ("name", "school")
         required_save_attrs: Iterable[str] = ("name", "school")
+        required_head_attrs: Iterable[str] = ("name",)
         required_search_attrs: Iterable[str] = ("school",)
 
     def __init__(self, session: Session, language: str = None):
         super().__init__(session=session, language=language)
         self.collection_url = self.session.urls["workgroup"]
         self.object_url = f"{self.session.urls['workgroup']}{{school}}/{{name}}"
```

