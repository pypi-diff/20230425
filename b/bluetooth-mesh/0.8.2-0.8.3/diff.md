# Comparing `tmp/bluetooth-mesh-0.8.2.tar.gz` & `tmp/bluetooth-mesh-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bluetooth-mesh-0.8.2.tar", last modified: Tue Apr 25 11:27:37 2023, max compression
+gzip compressed data, was "dist/bluetooth-mesh-0.8.3.tar", last modified: Tue Apr 25 11:58:56 2023, max compression
```

## Comparing `bluetooth-mesh-0.8.2.tar` & `bluetooth-mesh-0.8.3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1234 2020-03-20 10:52:47.000000 bluetooth-mesh-0.8.2/.gitignore
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13702 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/.pylintrc
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      252 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/.readthedocs.yml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1238 2022-04-12 11:29:02.000000 bluetooth-mesh-0.8.2/.travis.yml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      285 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/AUTHORS
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    18006 2018-11-22 08:06:11.000000 bluetooth-mesh-0.8.2/LICENSE
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/PKG-INFO
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1931 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.2/README.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       74 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    36147 2022-02-02 12:42:42.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/application.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/apps/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      332 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/apps/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      113 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/apps/hookspecs.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    54089 2022-04-12 07:30:22.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/apps/meshcli.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      390 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/apps/mixins.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3348 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/crypto.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    21860 2021-03-11 08:56:00.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/interfaces.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    18575 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/mesh.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4028 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      589 2022-04-12 11:01:40.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/capnproto.py
--rwxrwxr-x   0 khorne    (1000) khorne    (1000)     8853 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/capnproto_generator.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    37203 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/config.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      432 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3144 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/battery.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3605 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/level.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      281 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5615 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/ctl.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4944 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/lightness.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2588 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/onoff.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2237 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generics.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3676 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/health.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    23969 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/properties.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3727 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/scene.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    11769 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/sensor.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      672 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6838 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/debug.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4219 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/debugV2.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     7081 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/gateway_config_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3695 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/light_extended_controller.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5145 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/network_diagnostic_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     7449 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/rrule_scheduler.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     8703 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_debug.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    10468 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6482 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2285 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_access.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2925 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_battery.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    39789 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_config.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4162 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_generics.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5255 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_health.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6199 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_level.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13545 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_light.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5300 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_scene.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    31797 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_sensor.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1332 2021-04-26 14:31:14.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_strings.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4669 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_time.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     9414 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/time.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13716 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/messages/util.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/models/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       67 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/models/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    17537 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/models/base.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    82908 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/models/models.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     9695 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/provisioning.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-03-19 13:27:43.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1478 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/fixtures.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     8072 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_application.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1979 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_construct_match.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3934 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_element.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1764 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_gatherer.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1965 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_key_derivation.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4772 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_light_lightness_client.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    12070 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_mesh.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    12410 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_model.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    14459 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_provisioning.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3227 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_scene_client.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1925 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_security.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1984 2021-04-15 08:26:46.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_signal.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2743 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_tasklet.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2660 2021-01-29 08:55:12.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/tokenring.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6875 2022-04-12 10:15:30.000000 bluetooth-mesh-0.8.2/bluetooth_mesh/utils.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/PKG-INFO
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3620 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/SOURCES.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        1 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/dependency_links.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      132 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/entry_points.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      257 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/requires.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       15 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/top_level.txt
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        7 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/.gitignore
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      634 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/Makefile
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/_ext/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6620 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.2/docs/_ext/autoconstruct.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/_static/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/_static/.keep
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/api/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      901 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/api/application.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2576 2022-06-06 08:21:17.000000 bluetooth-mesh-0.8.2/docs/api/messages.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      843 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/api/models.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      114 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/api.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2394 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.2/docs/conf.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1045 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/index.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      454 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/installation.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/mod/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       69 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/application.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/docs/mod/examples/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      895 2020-12-02 08:20:28.000000 bluetooth-mesh-0.8.2/docs/mod/examples/bulk_query.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      957 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.2/docs/mod/examples/callbacks.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      979 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/examples/delay.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      779 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/examples/expect.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      577 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/examples/model.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1110 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/examples/query.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      575 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/examples/repeat.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       59 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/messages.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3653 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod/models.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       80 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/mod.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      119 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/docs/quickstart.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2666 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.2/docs/skeleton.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      513 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.2/pyproject.toml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       63 2023-04-25 11:27:37.000000 bluetooth-mesh-0.8.2/setup.cfg
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2945 2023-04-25 11:27:25.000000 bluetooth-mesh-0.8.2/setup.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      652 2022-06-06 08:22:51.000000 bluetooth-mesh-0.8.2/tox.ini
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1234 2020-03-20 10:52:47.000000 bluetooth-mesh-0.8.3/.gitignore
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    13702 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/.pylintrc
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      252 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/.readthedocs.yml
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1238 2022-04-12 11:29:02.000000 bluetooth-mesh-0.8.3/.travis.yml
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      285 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/AUTHORS
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    18006 2018-11-22 08:06:11.000000 bluetooth-mesh-0.8.3/LICENSE
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/PKG-INFO
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1931 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.3/README.rst
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       74 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    36147 2022-02-02 12:42:42.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/application.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      332 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      113 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/hookspecs.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    54089 2022-04-12 07:30:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/meshcli.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      390 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/mixins.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3348 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/crypto.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    21860 2021-03-11 08:56:00.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/interfaces.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    18575 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/mesh.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4028 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      589 2022-04-12 11:01:40.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto.py
+-rwxrwxr-x   0 khorne    (1000) khorne    (1000)     8853 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto_generator.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    37836 2023-04-25 11:58:34.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/config.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      432 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3144 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/battery.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3605 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/level.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      281 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     5615 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/ctl.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4944 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/lightness.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2588 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/onoff.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2237 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generics.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3676 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/health.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    23969 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/properties.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3727 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/scene.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    11769 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/sensor.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      672 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     6838 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debug.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4219 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debugV2.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     7081 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/gateway_config_server.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3695 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/light_extended_controller.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     5145 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/network_diagnostic_server.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     7449 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/rrule_scheduler.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     8703 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_debug.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    10468 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     6482 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2285 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_access.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2925 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_battery.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    41195 2023-04-25 11:58:34.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_config.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4162 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_generics.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     5255 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_health.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     6199 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_level.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    13545 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_light.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     5300 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_scene.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    31797 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_sensor.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1332 2021-04-26 14:31:14.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_strings.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4669 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_time.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     9414 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/time.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    13716 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/util.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       67 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    17537 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/base.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    82908 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/models.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     9695 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/provisioning.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-03-19 13:27:43.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/__init__.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1478 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/fixtures.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     8072 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_application.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1979 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_construct_match.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3934 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_element.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1764 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_gatherer.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1965 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_key_derivation.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     4772 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_light_lightness_client.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    12070 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_mesh.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    12410 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_model.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)    14459 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_provisioning.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3227 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_scene_client.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1925 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_security.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1984 2021-04-15 08:26:46.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_signal.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2743 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_tasklet.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2660 2021-01-29 08:55:12.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/tokenring.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     6875 2022-04-12 10:15:30.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/utils.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/PKG-INFO
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3620 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/SOURCES.txt
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)        1 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/dependency_links.txt
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      132 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/entry_points.txt
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      257 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/requires.txt
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       15 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/top_level.txt
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)        7 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/.gitignore
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      634 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/Makefile
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/_ext/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     6620 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/_ext/autoconstruct.py
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/_static/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/_static/.keep
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/api/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      901 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api/application.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2576 2022-06-06 08:21:17.000000 bluetooth-mesh-0.8.3/docs/api/messages.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      843 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api/models.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      114 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2394 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/conf.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1045 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/index.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      454 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/installation.rst
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/mod/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       69 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/application.rst
+drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/mod/examples/
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      895 2020-12-02 08:20:28.000000 bluetooth-mesh-0.8.3/docs/mod/examples/bulk_query.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      957 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/mod/examples/callbacks.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      979 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/delay.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      779 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/expect.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      577 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/model.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     1110 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/query.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      575 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/repeat.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       59 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/messages.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     3653 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/models.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       80 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      119 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/quickstart.rst
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2666 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/skeleton.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      513 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/pyproject.toml
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)       63 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/setup.cfg
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)     2945 2023-04-25 11:58:43.000000 bluetooth-mesh-0.8.3/setup.py
+-rw-rw-r--   0 khorne    (1000) khorne    (1000)      652 2022-06-06 08:22:51.000000 bluetooth-mesh-0.8.3/tox.ini
```

### Comparing `bluetooth-mesh-0.8.2/.gitignore` & `bluetooth-mesh-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/.pylintrc` & `bluetooth-mesh-0.8.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/.travis.yml` & `bluetooth-mesh-0.8.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/LICENSE` & `bluetooth-mesh-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/PKG-INFO` & `bluetooth-mesh-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-mesh
-Version: 0.8.2
+Version: 0.8.3
 Summary: Bluetooth mesh for Python
 Home-page: http://github.com/silvairgit/python-bluetooth-mesh
 Author-email: michal.lowas-rzechonek@silvair.com
 License: UNKNOWN
 Description: =====================
         python-bluetooth-mesh
         =====================
```

### Comparing `bluetooth-mesh-0.8.2/README.rst` & `bluetooth-mesh-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/application.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/application.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/apps/meshcli.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/apps/meshcli.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/crypto.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/crypto.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/interfaces.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/interfaces.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/mesh.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/__init__.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/capnproto.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/capnproto_generator.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto_generator.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/config.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,41 +25,48 @@
 from datetime import timedelta
 
 from construct import (
     Adapter,
     BitsInteger,
     BitStruct,
     Bytes,
+    Bytewise,
     Embedded,
     ExprValidator,
     Flag,
     GreedyBytes,
     GreedyRange,
+    If,
+    IfThenElse,
     Int8ul,
     Int16ul,
     Int24ul,
+    Int8sl,
+    Mapping,
     Padding,
     Rebuild,
     Select,
     Struct,
     len_,
     obj_,
-    this, Int8sl, If, Mapping, IfThenElse, Bytewise,
+    this, Byte
 )
 
-from bluetooth_mesh.messages.util import BitList, EmbeddedBitStruct, EnumAdapter
-from bluetooth_mesh.messages.util import EnumSwitch as Switch
 from bluetooth_mesh.messages.util import (
+    BitList,
+    EmbeddedBitStruct,
+    EnumAdapter,
     LogAdapter,
     NamedSelect,
     Opcode,
     RangeValidator,
     Reversed,
     SwitchStruct,
 )
+from bluetooth_mesh.messages.util import EnumSwitch as Switch
 
 
 class SecureNetworkBeacon(enum.IntEnum):
     OFF = 0x00
     ON = 0x01
 
 
@@ -604,14 +611,33 @@
     "vendor_models" / ModelRelationItem[this["number_v"]],
 )
 
 CompositionDataPage1 = Struct(
     'element' / GreedyRange(CompositionDataPage1Element)
 )
 
+Version = Struct(
+    'version_x' / Int8ul,
+    'version_y' / Int8ul,
+    'version_z' / Int8ul,
+)
+
+MeshProfileEntry = Struct(
+    "mesh_profile_identifier" / Int16ul,
+    "version" / Version,
+    "num_element_offsets" / Rebuild(Int8ul, len_(this["element_offset_list"])),
+    "element_offset_list" / Int8ul[this["num_element_offsets"]],
+    "additional_data_len" / Rebuild(Int16ul, len_(this["additional_data"])),
+    "additional_data" / Int8ul[this["additional_data_len"]],
+)
+
+CompositionDataPage2 = Struct(
+    'record_list' / GreedyRange(MeshProfileEntry)
+)
+
 Retransmit = BitStruct(
     # sssssccc
     "interval_steps" / BitsInteger(5),
     "count" / BitsInteger(3),
 )
 # fmt: on
 
@@ -769,36 +795,36 @@
 
 ConfigBeaconStatus = ConfigBeaconSet
 
 
 class CompositionDataPage(enum.IntEnum):
     ZERO = 0
     FIRST = 1
+    SECOND = 2
     TWO_HUNDRED_AND_FIFTY_FIFTH = 255
 
 
 CompositionDataPageAdapter = EnumAdapter(Int8ul, CompositionDataPage)
 
 ConfigCompositionDataGet = Struct(
     "page" / CompositionDataPageAdapter,
 )
 
 ConfigCompositionData = Switch(
     this.page,
     {
         CompositionDataPage.ZERO: CompositionDataPage0,
         CompositionDataPage.FIRST: CompositionDataPage1,
+        CompositionDataPage.SECOND: CompositionDataPage2,
         CompositionDataPage.TWO_HUNDRED_AND_FIFTY_FIFTH: GreedyBytes,
     },
-    default=GreedyBytes
-
 )
 
-ConfigCompositionDataStatus = Struct(
-    "page" / Int8ul,
+ConfigCompositionDataStatus = SwitchStruct(
+    "page" / CompositionDataPageAdapter,
     "data" / ConfigCompositionData,
 )
 
 ConfigDefaultTTLGet = Struct()
 
 ConfigDefaultTTLSet = Struct(
     "ttl" / TTL,
```

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/battery.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/battery.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/level.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/level.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/ctl.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/ctl.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/light/lightness.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/lightness.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generic/onoff.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/onoff.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/generics.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generics.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/health.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/health.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/properties.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/properties.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/scene.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/scene.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/sensor.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/sensor.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/__init__.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/debug.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debug.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/debugV2.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debugV2.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/gateway_config_server.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/gateway_config_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/light_extended_controller.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/light_extended_controller.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/network_diagnostic_server.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/network_diagnostic_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/rrule_scheduler.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/rrule_scheduler.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_debug.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_access.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_access.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_battery.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_battery.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_config.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,182 +185,14 @@
     pytest.param(
         VirtualLabel,
         bytes.fromhex('0080'),
         0x8000,
         id="VirtualAddress - Min"
     ),
     pytest.param(
-        CompositionDataPage0Element,
-        bytes.fromhex('00000101ADDEEFBEADDE'),
-        {
-            "location": GATTNamespaceDescriptor.UNKNOWN,
-            "sig_number": 0x01,
-            "vendor_number": 0x01,
-            "sig_models": [{"model_id": 0xDEAD}],
-            "vendor_models": [{"model_id": 0xDEAD, "vendor_id": 0xBEEF}]
-        },
-        id="CompositionDataPage0Element", ),
-    pytest.param(
-        CompositionDataPage0Element,
-        bytes.fromhex('00000001EFBEADDE'),
-        {
-            "location": GATTNamespaceDescriptor.UNKNOWN,
-            "sig_number": 0x00,
-            "vendor_number": 0x01,
-            "sig_models": [],
-            "vendor_models": [{"model_id": 0xDEAD, "vendor_id": 0xBEEF}]
-        },
-        id="CompositionDataPage0Element - No SIG", ),
-    pytest.param(
-        CompositionDataPage0Element,
-        bytes.fromhex('00000100ADDE'),
-        {
-            "location": GATTNamespaceDescriptor.UNKNOWN,
-            "sig_number": 0x01,
-            "vendor_number": 0x00,
-            "sig_models": [{"model_id": 0xDEAD}],
-            "vendor_models": []
-        },
-        id="CompositionDataPage0Element - No vendor"
-    ),
-    pytest.param(
-        CompositionDataPage0,
-        bytes.fromhex('3601CE00FECAEFBE0BB000000000'),
-        {
-            "cid": 0x0136,
-            "pid": 0x00CE,
-            "vid": 0xCAFE,
-            "crpl": 0xBEEF,
-            "features": 0xB00B,
-            "elements": [
-                {
-                    "location": GATTNamespaceDescriptor.UNKNOWN,
-                    "sig_number": 0x00,
-                    "vendor_number": 0x00,
-                    "sig_models": [],
-                    "vendor_models": []
-                }
-            ]
-        },
-        id="CompositionData - One element", ),
-    pytest.param(
-        CompositionDataPage0,
-        bytes.fromhex('3601CE00FECAEFBE0BB00000000000000000'),
-        {
-            "cid": 0x0136,
-            "pid": 0x00CE,
-            "vid": 0xCAFE,
-            "crpl": 0xBEEF,
-            "features": 0xB00B,
-            "elements": [
-                {
-                    "location": GATTNamespaceDescriptor.UNKNOWN,
-                    "sig_number": 0x00,
-                    "vendor_number": 0x00,
-                    "sig_models": [],
-                    "vendor_models": []
-                },
-                {
-                    "location": GATTNamespaceDescriptor.UNKNOWN,
-                    "sig_number": 0x00,
-                    "vendor_number": 0x00,
-                    "sig_models": [],
-                    "vendor_models": []
-                }
-            ]
-        },
-        id="CompositionData - Two elements"
-    ),
-    pytest.param(
-        CompositionDataPage1,
-        bytes.fromhex('02010005000000010201000501170101'),
-        {"element": [
-            {
-                "number_s": 2,
-                "number_v": 1,
-                "sig_models": [
-                    {
-                        "extended_items_count": 0,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": False,
-                        "corresponding_id": None,
-                        "extended_models_items": []
-                    },
-                    {
-                        "extended_items_count": 1,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": True,
-                        "corresponding_id": 0,
-                        "extended_models_items": [
-                            {
-                                "model_item_index": 0,
-                                "element_offset": 0
-                            }
-                        ]
-                    },
-                ],
-                "vendor_models": [
-                    {
-                        "extended_items_count": 0,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": False,
-                        "corresponding_id": None,
-                        "extended_models_items": []
-                    },
-                ]
-            },
-            {
-                "number_s": 1,
-                "number_v": 2,
-                "sig_models": [
-                    {
-                        "extended_items_count": 0,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": True,
-                        "corresponding_id": 0,
-                        "extended_models_items": []
-                    },
-                ],
-                "vendor_models": [
-                    {
-                        "extended_items_count": 1,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": True,
-                        "corresponding_id": 1,
-                        "extended_models_items": [
-                            {
-                                "model_item_index": 2,
-                                "element_offset": -1
-                            }
-                        ]
-                    },
-                    {
-                        "extended_items_count": 0,
-                        "format": ExtendedModelsItemFormat.SHORT,
-                        "corresponding_present": True,
-                        "corresponding_id": 1,
-                        "extended_models_items": []
-                    }
-
-                ]
-            }
-        ]
-        },
-        id="CompositionData Page 1"
-    ),
-    pytest.param(
-        ConfigCompositionDataStatus,
-        bytes.fromhex('03CAFE'),
-        {
-            "page": 0x03,
-            "data": bytes.fromhex('CAFE'),
-        },
-        id="ConfigCompositionDataStatus - not page 0 or 1"
-    ),
-    pytest.param(
         Retransmit,
         bytes.fromhex('07'),
         {
             "count": 0x07,
             "interval_steps": 0x00
         },
         id="Retransmit - Max count"
@@ -601,14 +433,206 @@
                     }
                 ]
                 }
         },
         id="ConfigCompositionDataStatus - page 1"
     ),
     pytest.param(
+        ConfigCompositionDataStatus,
+        bytes.fromhex('02001601000001010000'),
+        {
+            "page": 0x02,
+            "second":
+                {"record_list": [
+                    {
+                        "mesh_profile_identifier": 0x1600,
+                        "version": {
+                            "version_x": 1,
+                            "version_y": 0,
+                            "version_z": 0
+                        },
+                        "num_element_offsets": 1,
+                        "element_offset_list": [1],
+                        "additional_data_len": 0,
+                        "additional_data": []
+                    }
+                ]}
+        },
+        id="ConfigCompositionDataStatus - page 2"
+    ),
+    pytest.param(
+        ConfigCompositionDataStatus,
+        bytes.fromhex('FFCAFE'),
+        {
+            "page": 0xFF,
+            "two_hundred_and_fifty_fifth": bytes.fromhex('CAFE'),
+        },
+        id="ConfigCompositionDataStatus - not page 0 or 1 or 3"
+    ),
+    pytest.param(
+        CompositionDataPage0,
+        bytes.fromhex('3601CE00FECAEFBE0BB000000000'),
+        {
+            "cid": 0x0136,
+            "pid": 0x00CE,
+            "vid": 0xCAFE,
+            "crpl": 0xBEEF,
+            "features": 0xB00B,
+            "elements": [
+                {
+                    "location": GATTNamespaceDescriptor.UNKNOWN,
+                    "sig_number": 0x00,
+                    "vendor_number": 0x00,
+                    "sig_models": [],
+                    "vendor_models": []
+                }
+            ]
+        },
+        id="CompositionData - One element", ),
+    pytest.param(
+        CompositionDataPage0,
+        bytes.fromhex('3601CE00FECAEFBE0BB00000000000000000'),
+        {
+            "cid": 0x0136,
+            "pid": 0x00CE,
+            "vid": 0xCAFE,
+            "crpl": 0xBEEF,
+            "features": 0xB00B,
+            "elements": [
+                {
+                    "location": GATTNamespaceDescriptor.UNKNOWN,
+                    "sig_number": 0x00,
+                    "vendor_number": 0x00,
+                    "sig_models": [],
+                    "vendor_models": []
+                },
+                {
+                    "location": GATTNamespaceDescriptor.UNKNOWN,
+                    "sig_number": 0x00,
+                    "vendor_number": 0x00,
+                    "sig_models": [],
+                    "vendor_models": []
+                }
+            ]
+        },
+        id="CompositionData - Two elements"
+    ),
+    pytest.param(
+        CompositionDataPage0Element,
+        bytes.fromhex('00000101ADDEEFBEADDE'),
+        {
+            "location": GATTNamespaceDescriptor.UNKNOWN,
+            "sig_number": 0x01,
+            "vendor_number": 0x01,
+            "sig_models": [{"model_id": 0xDEAD}],
+            "vendor_models": [{"model_id": 0xDEAD, "vendor_id": 0xBEEF}]
+        },
+        id="CompositionDataPage0Element", ),
+    pytest.param(
+        CompositionDataPage0Element,
+        bytes.fromhex('00000001EFBEADDE'),
+        {
+            "location": GATTNamespaceDescriptor.UNKNOWN,
+            "sig_number": 0x00,
+            "vendor_number": 0x01,
+            "sig_models": [],
+            "vendor_models": [{"model_id": 0xDEAD, "vendor_id": 0xBEEF}]
+        },
+        id="CompositionDataPage0Element - No SIG", ),
+    pytest.param(
+        CompositionDataPage0Element,
+        bytes.fromhex('00000100ADDE'),
+        {
+            "location": GATTNamespaceDescriptor.UNKNOWN,
+            "sig_number": 0x01,
+            "vendor_number": 0x00,
+            "sig_models": [{"model_id": 0xDEAD}],
+            "vendor_models": []
+        },
+        id="CompositionDataPage0Element - No vendor"
+    ),
+
+    pytest.param(
+        CompositionDataPage1,
+        bytes.fromhex('02010005000000010201000501170101'),
+        {"element": [
+            {
+                "number_s": 2,
+                "number_v": 1,
+                "sig_models": [
+                    {
+                        "extended_items_count": 0,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": False,
+                        "corresponding_id": None,
+                        "extended_models_items": []
+                    },
+                    {
+                        "extended_items_count": 1,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": True,
+                        "corresponding_id": 0,
+                        "extended_models_items": [
+                            {
+                                "model_item_index": 0,
+                                "element_offset": 0
+                            }
+                        ]
+                    },
+                ],
+                "vendor_models": [
+                    {
+                        "extended_items_count": 0,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": False,
+                        "corresponding_id": None,
+                        "extended_models_items": []
+                    },
+                ]
+            },
+            {
+                "number_s": 1,
+                "number_v": 2,
+                "sig_models": [
+                    {
+                        "extended_items_count": 0,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": True,
+                        "corresponding_id": 0,
+                        "extended_models_items": []
+                    },
+                ],
+                "vendor_models": [
+                    {
+                        "extended_items_count": 1,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": True,
+                        "corresponding_id": 1,
+                        "extended_models_items": [
+                            {
+                                "model_item_index": 2,
+                                "element_offset": -1
+                            }
+                        ]
+                    },
+                    {
+                        "extended_items_count": 0,
+                        "format": ExtendedModelsItemFormat.SHORT,
+                        "corresponding_present": True,
+                        "corresponding_id": 1,
+                        "extended_models_items": []
+                    }
+
+                ]
+            }
+        ]
+        },
+        id="CompositionData Page 1"
+    ),
+    pytest.param(
         CompositionDataPage1Element,
         bytes.fromhex('050307011AFD0901383001080508480000050A00050AD0'),
         {
             "number_s": 5,
             "number_v": 3,
             "sig_models": [
                 {
@@ -699,14 +723,34 @@
                             ]
                         },
                     ]
         },
         id="Config Composition Data Page 1 - single element"
     ),
     pytest.param(
+        CompositionDataPage2,
+        bytes.fromhex('021601020303010203020011FF'),
+        {"record_list": [
+            {
+                "mesh_profile_identifier": 0x1602,
+                "version": {
+                    "version_x": 1,
+                    "version_y": 2,
+                    "version_z": 3
+                },
+                "num_element_offsets": 3,
+                "element_offset_list": [1, 2, 3],
+                "additional_data_len": 2,
+                "additional_data":  [0x11, 0xFF]
+
+            }]
+        },
+        id="CompositionData Page 2"
+    ),
+    pytest.param(
         ModelRelationItem,
         bytes.fromhex('010A'),
         {
             "extended_items_count": 0,
             "format": ExtendedModelsItemFormat.SHORT,
             "corresponding_present": True,
             "corresponding_id": 10,
```

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_generics.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_generics.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_health.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_health.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_level.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_level.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_light.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_light.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_scene.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_sensor.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_strings.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_strings.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/test/test_time.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_time.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/time.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/time.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/messages/util.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/util.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/models/base.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/models/base.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/models/models.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/models/models.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/provisioning.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/provisioning.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/fixtures.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_application.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_application.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_construct_match.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_construct_match.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_element.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_element.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_gatherer.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_gatherer.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_key_derivation.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_key_derivation.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_light_lightness_client.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_light_lightness_client.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_mesh.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_model.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_model.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_provisioning.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_scene_client.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_scene_client.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_security.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_security.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_signal.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/test/test_tasklet.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_tasklet.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/tokenring.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/tokenring.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh/utils.py` & `bluetooth-mesh-0.8.3/bluetooth_mesh/utils.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/PKG-INFO` & `bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-mesh
-Version: 0.8.2
+Version: 0.8.3
 Summary: Bluetooth mesh for Python
 Home-page: http://github.com/silvairgit/python-bluetooth-mesh
 Author-email: michal.lowas-rzechonek@silvair.com
 License: UNKNOWN
 Description: =====================
         python-bluetooth-mesh
         =====================
```

### Comparing `bluetooth-mesh-0.8.2/bluetooth_mesh.egg-info/SOURCES.txt` & `bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/Makefile` & `bluetooth-mesh-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/_ext/autoconstruct.py` & `bluetooth-mesh-0.8.3/docs/_ext/autoconstruct.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/api/application.rst` & `bluetooth-mesh-0.8.3/docs/api/application.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/api/messages.rst` & `bluetooth-mesh-0.8.3/docs/api/messages.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/api/models.rst` & `bluetooth-mesh-0.8.3/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/conf.py` & `bluetooth-mesh-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/index.rst` & `bluetooth-mesh-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/bulk_query.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/bulk_query.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/callbacks.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/callbacks.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/delay.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/delay.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/expect.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/expect.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/model.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/model.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/query.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/query.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/examples/repeat.py` & `bluetooth-mesh-0.8.3/docs/mod/examples/repeat.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/mod/models.rst` & `bluetooth-mesh-0.8.3/docs/mod/models.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/docs/skeleton.py` & `bluetooth-mesh-0.8.3/docs/skeleton.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/pyproject.toml` & `bluetooth-mesh-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.2/setup.py` & `bluetooth-mesh-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 # fmt: off
 setup(
     name='bluetooth-mesh',
-    version='0.8.2',
+    version='0.8.3',
     author_email='michal.lowas-rzechonek@silvair.com',
     description=(
         'Bluetooth mesh for Python'
     ),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='http://github.com/silvairgit/python-bluetooth-mesh',
```

### Comparing `bluetooth-mesh-0.8.2/tox.ini` & `bluetooth-mesh-0.8.3/tox.ini`

 * *Files identical despite different names*

