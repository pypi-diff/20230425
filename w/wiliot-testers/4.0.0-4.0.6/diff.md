# Comparing `tmp/wiliot-testers-4.0.0.tar.gz` & `tmp/wiliot-testers-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-testers-4.0.0.tar", last modified: Wed Mar  1 10:13:34 2023, max compression
+gzip compressed data, was "wiliot-testers-4.0.6.tar", last modified: Tue Apr 25 08:52:33 2023, max compression
```

## Comparing `wiliot-testers-4.0.0.tar` & `wiliot-testers-4.0.6.tar`

### file list

```diff
@@ -1,113 +1,108 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7247 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1993 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.429404 wiliot-testers-4.0.0/wiliot_testers/
--rw-rw-rw-   0 root         (0) root         (0)    10668 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/API_README.md
--rw-rw-rw-   0 root         (0) root         (0)     4005 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.429404 wiliot-testers-4.0.0/wiliot_testers/calibration_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/calibration_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20959 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/calibration_test/calibration_test.py
--rw-rw-rw-   0 root         (0) root         (0)    25345 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/calibration_test/calibration_test_by_tbp.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.429404 wiliot-testers-4.0.0/wiliot_testers/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/config/equipment_config.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.433404 wiliot-testers-4.0.0/wiliot_testers/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72970 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/docs/tester_api_flow.pdf
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/docs/wiliot_logo.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.433404 wiliot-testers-4.0.0/wiliot_testers/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/examples/wiliot_tester_example.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.433404 wiliot-testers-4.0.0/wiliot_testers/offline/
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.433404 wiliot-testers-4.0.0/wiliot_testers/offline/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/configs/gui_inputs_autotests.json
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/configs/gui_printer_inputs_4_Test_do_not_delete.json
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/configs/test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)     2152 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/configs/tests_suites.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.437404 wiliot-testers-4.0.0/wiliot_testers/offline/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37001 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     9764 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    44358 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_run_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    20401 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_start_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    81030 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     4386 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/docs/wiliot_logo.png
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/env_install.bat
--rw-rw-rw-   0 root         (0) root         (0)     9005 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/env_install.py
--rw-rw-rw-   0 root         (0) root         (0)   153102 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/offline_tester.py
--rw-rw-rw-   0 root         (0) root         (0)    59436 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/offline_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/run_offline_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)     7388 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/tadbik_r2r_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    20782 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/upload_and_serialize_csv_manually.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/offline/upload_and_serialize_offlne_logs.bat
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.437404 wiliot-testers-4.0.0/wiliot_testers/sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42032 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/com_connect.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.437404 wiliot-testers-4.0.0/wiliot_testers/sample/configs/
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/configs/.default_configs.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/configs/.default_surfaces.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13075 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/configs_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/get_temperature_sensor_name.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/sample_test _calib.bat
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/sample_test _offline.bat
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/sample_test.bat
--rw-rw-rw-   0 root         (0) root         (0)    73383 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/sample_test.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/sample_test_calib_offline.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/sample/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22413 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/com_connect.ui
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/comm.gif
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    24482 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/configs.ui
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/edit.gif
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/refresh.gif
--rw-rw-rw-   0 root         (0) root         (0)     3213 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/reset.png
--rw-rw-rw-   0 root         (0) root         (0)    25362 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/sample_test.ui
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/save.png
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/sample/utils/wiliot3.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/system_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/system_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42506 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/system_test/harvester_test.py
--rw-rw-rw-   0 root         (0) root         (0)    73298 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/system_test/system_test_example.py
--rw-rw-rw-   0 root         (0) root         (0)    24192 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/test_equipment.py
--rw-rw-rw-   0 root         (0) root         (0)    75914 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/tester_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6048 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers/version.py
--rw-rw-rw-   0 root         (0) root         (0)     8865 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_log.py
--rw-rw-rw-   0 root         (0) root         (0)    16525 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_tag_result.py
--rw-rw-rw-   0 root         (0) root         (0)    58357 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_tag_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/yield/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/yield/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/arduino_counter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/arduino_counter/arduino_counter.ino
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.441405 wiliot-testers-4.0.0/wiliot_testers/yield/configs/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/configs/.default_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/configs/inlay_data.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/run_yield_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)    21557 2023-03-01 10:13:16.000000 wiliot-testers-4.0.0/wiliot_testers/yield/yield_tester.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-01 10:13:34.429404 wiliot-testers-4.0.0/wiliot_testers.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-03-01 10:13:34.000000 wiliot-testers-4.0.0/wiliot_testers.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.100857 wiliot-testers-4.0.6/wiliot_testers/
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/API_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/calibration_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20959 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    25345 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/equipment_config.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72970 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/offline/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37001 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9764 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    44358 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    20401 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    81030 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4386 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.bat
+-rw-rw-rw-   0 root         (0) root         (0)     9005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py
+-rw-rw-rw-   0 root         (0) root         (0)   155011 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py
+-rw-rw-rw-   0 root         (0) root         (0)    63768 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/run_offline_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41938 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_surfaces.json
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12551 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.bat
+-rw-rw-rw-   0 root         (0) root         (0)    74858 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22413 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    24482 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/edit.gif
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/refresh.gif
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png
+-rw-rw-rw-   0 root         (0) root         (0)    26613 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/save.png
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/system_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42625 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    73298 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    31248 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/test_equipment.py
+-rw-rw-rw-   0 root         (0) root         (0)    75770 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/tester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data.bat
+-rw-rw-rw-   0 root         (0) root         (0)    14651 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data_to_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py
+-rw-rw-rw-   0 root         (0) root         (0)    16346 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    61986 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/.default_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/run_yield_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)    22306 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/yield_tester.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3451 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/top_level.txt
```

### Comparing `wiliot-testers-4.0.0/LICENSE` & `wiliot-testers-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/bitbucket-pipelines.yml` & `wiliot-testers-4.0.6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/setup.py` & `wiliot-testers-4.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,13 +37,15 @@
                      'pyqtgraph',
                      'PySimpleGUI',
                      'matplotlib',
                      'PyQt5',
                      'pygubu==0.16',
                      'appdirs',
                      'pillow',
-                     'wiliot-core'
+                     'wiliot-api==4.1.0',
+                     'wiliot-core==4.0.8',
+                     'wiliot-tools==4.0.4'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/API_README.md` & `wiliot-testers-4.0.6/wiliot_testers/API_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 ```
 
 Class **run** Initialization:
 
 -- Table 3
 
 ```python
-WiliotResult = WiliotTagTester.run(wait_for_gw_trigger = 5, max_ttfp = 5)
+WiliotResult = WiliotTagTester.run(wait_for_gw_trigger = 5)
 ```
 
 The WiliotResult is a list that contains all the data from the tag under test- for example if we had 2 stages to the
 test (2 different GW configuration or energizing patterns) we will receive list of 2 results (If the tag passed both of
 the stages)
 
 We can also add devices to the black list from this class with given advertising address:
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/__init__.py` & `wiliot-testers-4.0.6/wiliot_testers/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/calibration_test/calibration_test.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/calibration_test/calibration_test_by_tbp.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/docs/tester_api_flow.pdf` & `wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/examples/wiliot_tester_example.py` & `wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/README.md` & `wiliot-testers-4.0.6/wiliot_testers/offline/README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/configs/tests_suites.json` & `wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992283950617283%*

 * *Differences: {"'Ble_Test_Only'": "{'tests': {0: {'quality_param': {replace: OrderedDict()}}}}"}*

```diff
@@ -8,20 +8,15 @@
         "tests": [
             {
                 "absGwTxPowerIndex": -1,
                 "delayBeforeNextTest": 0,
                 "energizingPattern": 18,
                 "maxTime": 5,
                 "name": "first_packets_ble_band",
-                "quality_param": {
-                    "ttfp": [
-                        0,
-                        3
-                    ]
-                },
+                "quality_param": {},
                 "rxChannel": 37,
                 "stop_criteria": {
                     "num_packets": [
                         3,
                         99
                     ]
                 },
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/example_of_timing_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_run_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/offline_tester_start_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/r2r_communication_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/env_install.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/offline_tester.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,31 +54,36 @@
    (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
    (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
    CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
    (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
    (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 """
 import csv
+import os.path
 from datetime import datetime
 import argparse
 from PyQt5.QtWidgets import *
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 import pyqtgraph as pg
 from wiliot_testers.test_equipment import BarcodeScanner
-
 from numpy import mean
 from wiliot_testers.wiliot_tester_tag_test import *
+from wiliot_testers.wiliot_tester_log import *
 from wiliot_testers.tester_utils import *
 from wiliot_testers.offline.offline_utils import *
-from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict
+from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict, InlayTypes, DualGWMode
 from wiliot_testers.utils.get_version import get_version
+from wiliot_core import WiliotGateway, DualGWMode
+from appdirs import user_data_dir
+from queue import Queue
+import socket
 
 # a global variable which will be in the log_file name that says the R2R code version
-n_tag_counter_position = 4 # 4 characters on the esternal id indicate tag counter in the reel
+n_tag_counter_position = 4  # 4 characters on the esternal id indicate tag counter in the reel
 R2R_code_version = '13'
 # running parameters
 tested = 0
 passed = 0
 under_threshold = 0
 missing_labels = 0
 black_list_size = 0
@@ -95,14 +100,16 @@
 run_start_time_ = datetime.datetime.now()
 qr_que_list = []
 external_id_for_printer = 999999999
 yield_over_time = 0
 calculate_interval = 10
 calculate_on = 50
 
+MIN_TEST_TIME = 0.3  # seconds
+
 lock_print = threading.Lock()
 
 
 class QRThread(threading.Thread):
     def __init__(self, events, ports_and_guis):
         threading.Thread.__init__(self)
         self.events = events
@@ -124,15 +131,15 @@
             self.success = True
             self.wrong_readout_in_row = 0
 
         die = False
 
         while not die:
             time.sleep(0)
-            self.events.start_compare.wait(timeout=4)
+            self.events.start_compare.wait(timeout=10)
             if not self.events.start_compare.is_set():
                 if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
                     die = True
                     break
                 continue
 
             if not self.events.qr_queue.empty():
@@ -161,18 +168,18 @@
                     self.ports_and_guis.my_logger.logger.info(
                         "Scanning failed, trying again attempt {}/{}".format(i, self.read_out_attempts))
 
                 if not self.success:
                     self.ports_and_guis.my_logger.logger.warning('Scan failed for tag {}'.format(self.tag_comparted))
                     self.wrong_readout += 1
                     self.wrong_readout_in_row += 1
-                    if self.wrong_readout < self.qr_max_bad_tags and self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
+                    if self.wrong_readout < self.qr_max_bad_tags and \
+                            self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
                         self.events.qr_read_success.set()
 
-
             if self.wrong_readout >= self.qr_max_bad_tags:
                 die = True
                 self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing reached')
                 break
 
             if self.wrong_readout_in_row >= self.max_wrong_readouts_in_row:
                 self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing in row reached')
@@ -221,15 +228,14 @@
             'The printer printed Fail to the previous tag',
             'The printer have not printed on the last tag'
 
     Events:
         listen/ waits on:
             events.r2r_ready_or_done2tag    => user pressed Stop (end the program)
             events.done_to_printer_thread             => user pressed Stop (end the program) - to avoid deadlock
-            events.cont_to_printer_thread             => continue was pressed by user
             events.r2r_ready                => printing was made
             events.was_pass_to_printer      => the last printing was pass
         sets:
             events.printer_error            => the last print was not successful, will cause pause to this run
                                                 (and will trigger exception according to the situation)
             events.printer_success          => the last print was successful
 
@@ -254,21 +260,24 @@
             self.fail_counter = 0
             self.printer_response_timeout = 1.5  # time in seconds for printer to answer with updated printing value
             self.timer_is_done = False
             self.exception_queue = Queue()
             self.printing_format = self.ports_and_guis.Tag_Value['printingFormat']
             self.qr_enable = self.ports_and_guis.Tag_Value['QRRead']
             self.roll_sgtin = self.ports_and_guis.Tag_Printing_Value['stringBeforeCounter']
+            self.enable_line_selection = self.ports_and_guis.Tag_Printing_Value['enableLineSelection'].lower() == 'yes'
             self.events = events
             self.r2r_ready_or_done2tag_or_done_to_printer_thread = or_event_set(events.r2r_ready_or_done2tag,
                                                                                 events.done_to_printer_thread)
             self.start_value = start_value
             self.cur_value = 0
             self.pass_job_name = pass_job_name
             self.fail_job_name = self.ports_and_guis.Tag_Printing_Value['failJobName']
+            self.pass_job_num = self.ports_and_guis.Tag_Printing_Value['passJobNum']
+            self.fail_job_num = 1
 
             # open the socket & config the printer
             self.initialization()
 
         except Exception:
             exception_details = sys.exc_info()
             self.exception_queue.put(exception_details)
@@ -286,50 +295,40 @@
             # after printer crash - make sure the continue will be from a the old counter
             if use_current_value:
                 global external_id_for_printer
                 config_start_value = external_id_for_printer
             else:
                 config_start_value = self.start_value
             # initialization protocol
-            if self.printing_format == 'Test':
-                cmds = ['CAF\r\n', 'CQI\r\n', 'CLN|1|\r\n', 'CLN|2|\r\n',
-                        'LAS|' + str(self.pass_job_name) + '|2|' + str(self.sgtin) + '=' +
-                        str(self.roll_sgtin[:18]) + '|' + str(self.reel_num) + '=' + str(self.roll_sgtin[18:26]) +
-                        'T' + '|' + str(self.first_tag_counter) + '=' + str(config_start_value) + '|\r\n']
-                if self.fail_job_name == self.pass_job_name:
-                    cmds.append('LAS|' + str(self.fail_job_name) + '|1|' + str(self.sgtin) + '=' +
-                                str(self.roll_sgtin[:18]) + '|' + str(self.reel_num) + '=' +
-                                str(self.roll_sgtin[18:26]) + 'T' + '|' + str(self.first_tag_counter) + '=' +
-                                str(config_start_value) + '|\r\n')
-                else:
-                    cmds.append('LAS|' + self.fail_job_name + '|1|\r\n')
-            elif self.printing_format == 'SGTIN':
-                # SGTIN_QR has field for reel_num + 'T' and field for sgtin,
-                # SGTIN_only acts the same (the QR will not be in the sticker itself)
-                if self.pass_job_name == 'SGTIN_QR' or self.pass_job_name == 'SGTIN_only' or \
-                        self.pass_job_name == 'devkit_TEO' or self.pass_job_name == 'devkit_TIKI' \
-                        or self.pass_job_name == 'empty':
-                    cmds = ['CAF\r\n', 'CQI\r\n', 'CLN|1|\r\n', 'CLN|2|\r\n',
-                            'LAS|' + str(self.pass_job_name) + '|2|' + str(self.sgtin) + '=' + str(
-                                self.roll_sgtin[:18]) + '|'
-                            + str(self.reel_num) + '=' + str(self.roll_sgtin[18:26]) + 'T' + '|'
-                            + str(self.first_tag_counter) + '=' + str(config_start_value) + '|\r\n']
-                    if self.fail_job_name == self.pass_job_name:
-                        cmds.append('LAS|' + str(self.fail_job_name) + '|1|' + str(self.sgtin) + '=' +
-                                    str(self.roll_sgtin[:18]) + '|' + str(self.reel_num) + '=' +
-                                    str(self.roll_sgtin[18:26]) + 'T' + '|' + str(self.first_tag_counter) + '=' +
-                                    str(config_start_value) + '|\r\n')
-                    else:
-                        cmds.append('LAS|' + self.fail_job_name + '|1|\r\n')
-
+            if 'BARCODE' in self.pass_job_name.upper():
+                job_fields = [f'reel_num={self.roll_sgtin}T']
+            elif 'SGTIN' in self.pass_job_name.upper():
+                job_fields = [f'sgtin={self.roll_sgtin[:18]}', f'reel_num={self.roll_sgtin[18:26]}T']
             else:
                 printing_func('The print Job Name inserted is not supported at the moment, You will need to press Stop',
                               'PrinterThread', lock_print, logger_type='debug',
                               logger_name=self.ports_and_guis.my_logger.logger.name)
+                raise Exception('The print Job Name inserted is not supported at the moment')
 
+            job_fields.append(f'tag_number={config_start_value}')
+            job_fields.append('\r\n')
+            job_fields_str = '|'.join(job_fields)
+
+            cmds = ['CAF\r\n',
+                    'CQI\r\n',
+                    f'CLN|{self.fail_job_num}|\r\n',
+                    f'CLN|{self.pass_job_num}|\r\n',
+                    f'LAS|{self.pass_job_name}|{self.pass_job_num}|' + job_fields_str]
+            if self.fail_job_name == self.pass_job_name:
+                cmds.append(f'LAS|{self.pass_job_name}|{self.pass_job_num}|' + job_fields_str)
+            else:
+                cmds.append(f'LAS|{self.fail_job_name}|{self.fail_job_num}|\r\n')
+
+            if self.enable_line_selection:
+                cmds.append(self.get_line_selection_cmd(self.fail_job_name))  # select line
             for cmd in cmds:
                 value = self.query(cmd)
                 time.sleep(0.1)
                 # check if the return value is good, if not retry again for 10 times
                 counter = 0
                 while counter < 10:
                     # 'CQI' fails if the queue is empty
@@ -371,15 +370,15 @@
            2 -> 0 (automatically)      shutting-down
            3 -> 2, 4                   running
            4 -> 2, 3                   offline
         @except: PrinterNeedsResetException('Printer failed to switch to running mode')
         @return: None
         """
         res = self.query(self.get_state_request())
-        parts = [p for p in res.split("|")]
+        parts = res.split("|")
         if parts[1] == '0':  # (Shut down)
             res = self.query(self.set_state_command('1'))
             if res == 'ACK':
                 counter = 0
                 while counter < 10:
                     time.sleep(1)
                     res = self.query(self.set_state_command('3'))
@@ -397,70 +396,63 @@
         raise PrinterNeedsResetException('Printer failed to switch to running mode')
 
     def run(self):
         """
         runs the thread
         """
         global passed
-        first_printing_tag = True
         # this flag will tell the printer to restart its run() (for a case of connectionError)
         do_the_thread_again = True
         while do_the_thread_again:
+            do_the_thread_again = False
             time.sleep(0)
             self.ports_and_guis.my_logger.logger.debug('Starting printer inner loop')
             while not self.events.done_to_printer_thread.isSet():
                 time.sleep(0)
                 try:
                     self.r2r_ready_or_done2tag_or_done_to_printer_thread.wait()
                     if self.events.done_to_printer_thread.isSet() or self.events.done_to_r2r_thread.is_set() or \
                             self.events.done_to_tag_thread.is_set():
                         do_the_thread_again = False
                         break
 
-                    # for a case of pause - the printing test should not happen (printing should not happen)
-                    if self.events.pause_to_tag_thread.isSet():
-                        self.events.cont_to_printer_thread.wait()
-
-                    # to avoid wrong counter in edge cases of printer crash
-                    if self.events.cont_to_printer_thread.isSet():
-                        self.events.cont_to_printer_thread.clear()
-                        # get the current counter value
-                        value = self.query(self.get_state_request())
-                        if value == 'ERR':
-                            self.events.printer_error.set()
-                            raise PrinterNeedsResetException(
-                                'The printer initialization process has failed in command: ' + self.get_state_request())
-                        else:
-                            parts = [p for p in value.split("|")]
-                            self.cur_value = int(parts[5])
-
                     if self.qr_enable != 'Yes':
                         self.ports_and_guis.my_logger.logger.info('Waiting for start compare')
-                        self.events.start_compare.wait(timeout=4)  # Wait for QR scan flag
+                        self.events.start_compare.wait(timeout=10)  # Wait for QR scan flag
                         if not self.events.start_compare.is_set():
                             if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
                                 do_the_thread_again = False
                                 break
                             else:
                                 continue
                         else:
-                            self.events.start_compare.clear()
-                            self.printer_status(first_printing_tag)
-                            first_printing_tag = False
                             self.cur_value += 1
+                            self.events.start_compare.clear()
+                            t_i = datetime.datetime.now()
+                            dt = 0.0
+                            while dt < MIN_TEST_TIME:
+                                try:
+                                    self.printer_status()
+                                    break
+                                except Exception as e:
+                                    self.ports_and_guis.my_logger.logger.info(f'got exception from printer, '
+                                                                              f'try again ({e})')
+                                    dt = (datetime.datetime.now() - t_i).total_seconds()
+                                    time.sleep(0.010)
+                            if self.enable_line_selection:
+                                self.set_printing_type()  # set the printing type for the next tag #TODO need to enable it for QR as well
 
                 except Exception:
                     do_the_thread_again = False
                     exception_details = sys.exc_info()
                     self.exception_queue.put(exception_details)
                     exc_type, exc_obj, exc_trace = exception_details
                     self.events.printer_error.set()  # to avoid deadlocks
                     if isinstance(exc_obj, PrinterNeedsResetException):
                         self.events.stop_to_r2r_thread.set()
-                        self.events.pause_to_tag_thread.set()
                         self.r2r_ready_or_done2tag_or_done_to_printer_thread.wait()
                         break
                     elif isinstance(exc_obj, ConnectionResetError):
                         self.r2r_ready_or_done2tag_or_done_to_printer_thread.wait()
                         try:
                             self.reopen_sock()
                             do_the_thread_again = True
@@ -477,22 +469,72 @@
                             exc_type, exc_obj, exc_trace = exception_details
                             self.events.printer_error.set()  # to avoid deadlocks
                             if isinstance(exc_obj, PrinterNeedsResetException):
                                 self.r2r_ready_or_done2tag_or_done_to_printer_thread.wait()
                                 break
                     else:
                         self.events.stop_to_r2r_thread.set()  # to avoid from the run to continue printing in this case
-                        self.events.pause_to_tag_thread.set()
 
         self.closure()
         printing_func("Exited the while loop of printer thread", 'PrinterThread', lock_print, logger_type='debug',
                       logger_name=self.ports_and_guis.my_logger.logger.name)
         return
 
-    def printer_status(self, is_first):
+    def tag_status_to_job_type(self, tag_status):
+        if tag_status.lower() == 'fail':
+            job_type = self.fail_job_name
+        elif tag_status.lower() == 'pass':
+            job_type = self.pass_job_name
+        else:
+            self.ports_and_guis.my_logger.logger.warning(
+                'printing status should be fail or pass, but received "{}" satuts, '
+                'please restart the run'.format(tag_status))
+            raise PrinterNeedsResetException(
+                'printing status should be fail or pass, please check printer and rerun')
+        return job_type
+
+    def get_line_selection_cmd(self, job_name):
+        if job_name == self.fail_job_name:
+            line = self.fail_job_num
+        elif job_name == self.pass_job_name:
+            line = self.pass_job_num
+        else:
+            raise Exception(f'for line selection job name must be {self.fail_job_name} or {self.pass_job_name}')
+
+        return 'LSL|' + str(line) + '|\r\n'
+
+    def set_printing_type(self):
+        """
+        line selection
+        @return:
+        @rtype:
+        """
+        try:
+            tag_status = self.events.tag_status_queue.get(block=False, timeout=0.2)
+            printing_type = self.tag_status_to_job_type(tag_status)
+            line_selection_msg = self.get_line_selection_cmd(printing_type)
+            rsp = ''
+            t_0 = datetime.datetime.now()
+            dt = 0
+            timeout_ack = 1
+            while rsp != 'ACK' and dt < timeout_ack:
+                rsp = self.query(line_selection_msg)
+                if rsp == 'ACK':
+                    return
+                dt = (datetime.datetime.now() - t_0).total_seconds()
+            self.ports_and_guis.my_logger.logger.warning('Did not get ACK for Line Selection')
+            raise PrinterNeedsResetException('Did not get ACK for Line Selection')
+        except Empty:
+            self.ports_and_guis.my_logger.logger.warning('during printer line selection got exception for empty queue')
+            raise PrinterNeedsResetException('Did not get ACK for Line Selection')
+        except Exception as e:
+            self.ports_and_guis.my_logger.logger.warning('during printer line selection an error occurs: {}'.format(e))
+            raise PrinterNeedsResetException('Did not get ACK for Line Selection')
+
+    def printer_status(self):
         """
         checks if the printing value matches the values registered to the logs
         should be called only after self.events.r2r_ready was set
         Exceptions:
             @except Exception('The printer printed Pass to the previous tag'):
                     printer printed pass while it should have been print fail
             @except Exception('The printer printed Fail to the previous tag')
@@ -505,33 +547,25 @@
         parts = [p for p in res.split("|")]
         self.ports_and_guis.my_logger.logger.info(
             'Starting comparing value {} with {}'.format(str(self.cur_value), str(parts[5])))
         if parts[1] == '3':
             if parts[2] == '0':
                 self.ports_and_guis.my_logger.logger.debug('Printer status is online')
                 if int(parts[5]) == self.cur_value:
-                    if not self.ports_and_guis.print_test and self.qr_enable != 'Yes' and not is_first:
+                    if not self.ports_and_guis.print_test and self.qr_enable != 'Yes':
                         try:
                             expected_printing_type = self.events.qr_queue.get(block=False, timeout=0.2)
                             expected_printing_type = expected_printing_type['status'].lower()
                         except Exception as e:
                             self.ports_and_guis.my_logger.logger.warning(
                                 'printing type queue problem, please restart the run ({})'.format(e))
                             expected_printing_type = ''
-                        if expected_printing_type == 'fail':
-                            job_type = self.fail_job_name
-                        elif expected_printing_type == 'pass':
-                            job_type = self.pass_job_name
-                        else:
-                            self.ports_and_guis.my_logger.logger.warning(
-                                'printing status should be fail or pass, but received "{}" satuts, '
-                                'please restart the run'.format(expected_printing_type))
-                            raise PrinterNeedsResetException(
-                                'printing status should be fail or pass, please check printer and rerun')
-                            job_type = self.fail_job_name
+
+                        job_type = self.tag_status_to_job_type(expected_printing_type)
+
                         if parts[3] == job_type:
                             self.events.printer_validation_success.set()
                             self.ports_and_guis.my_logger.logger.debug(
                                 'Compare success with type {}'.format(job_type))
                         else:
                             self.events.printer_error.set()
                             raise PrinterNeedsResetException(
@@ -721,23 +755,19 @@
                 Run won't pause in that case. If tag reaches timeout, it will marked as fail
 
     Events:
         listen/ waits on:
             events.r2r_ready_or_done2tag => user pressed Stop (end the program) or r2r has finished to write the command
             events.done_or_printer_event => waits for printer event or for done_to_tag_thread (closes TagThread)
             events.done_to_tag_thread => closes TagThread at the end of the run
-            events.cont_to_tag_thread => wait for continue from MainWindow thread
-            events.pause_to_tag_thread => pauses thread if exception happened of user pressed Pause
             events.printer_error => the last print was not successful, will cause pause to this run
                                                 (and will trigger exception according to the situation)
 
         sets:
-            events.cont_to_main_thread => send continue from TagThread to MainWindow thread
             events.tag_thread_is_ready_to_main => notifies MainWindow thread TagThread is ready
-            events.pause_to_tag_thread => pauses thread if exception happened of user pressed Pause
             events.was_pass_to_printer => tag has passed. report "Pass" to printer
             events.was_fail_to_printer => tag has failed. report "Fail" to printer
             events.disable_missing_label_to_r2r_thread => if set, the run will pause if missing label is detected
             events.enable_missing_label_to_r2r_thread => if set, the run will not pause if missing label is detected
                                                         (up to maxMissingLabels set by user)
             events.start_to_r2r_thread => enable/disable R2R movement. Sends pulse on "Start/Stop machine" GPIO line
             events.stop_to_r2r_thread => stops the R2R from running in case of end of run or exception
@@ -758,47 +788,53 @@
         self.ports_and_guis = ports_and_guis
         self.events = events
         # self.test_times_up = False
         self.r2r_response_times_up = False
         self.test_suite_times_up = False
         self.duplication_handling_timer_is_done = False
         self.ttfgp_list = []
-        self.black_list =[]
+        self.black_list = []
         self.adv_addr = ''
         self.ttfp_num = 0
         self.ttfp_sum = 0
         self.rssi = 0
         self.tbp = -1
         self.ttfp = -1
         self.time_for_duplication_handling = 20  # time in seconds for duplication handling procedure
         self.management_client = management_client
         self.fatal_gw_error = False
+        self.pass_response_diff_offset = None
+        self.pass_response_diff = None
 
         self.pass_job_name = ''  # will be set inside config
         self.to_print = False
         self.printing_value = {'passJobName': None, 'stringBeforeCounter': None, 'digitsInCounter': 4,
                                'firstPrintingValue': '0'}  # will be set in config()
         self.done_or_printer_event = or_event_set(self.events.done_to_tag_thread, self.events.printer_event)
         self.fetal_error = False
         self.exception_queue = Queue()
         self.qr_enable = self.ports_and_guis.Tag_Value['QRRead']
         self.qr_offset = self.ports_and_guis.Tag_Value['QRoffset']
         self.printing_offset = self.ports_and_guis.Tag_Value['printOffset']
         self.qr_max_bad_tags = int(self.ports_and_guis.Tag_Value['maxQRWrongTags'])
         self.maxblackappear = int(self.ports_and_guis.Tag_Value['blackListAfter'])
+        self.events.tag_status_queue.maxsize = int(self.printing_offset) + 1
         if self.qr_enable == 'Yes':
             self.events.qr_queue.maxsize = int(self.qr_offset) + 1
         else:
             self.events.qr_queue.maxsize = int(self.printing_offset) + 1
-            for i in range(self.printing_offset):
+            for i in range(self.printing_offset + 1):
                 self.events.qr_queue.put({'status': 'Fail'})
+        for i in range(self.printing_offset):  # first printed tag is checked upon init
+            self.events.tag_status_queue.put('fail')
         self.did_closure_fn_run = False
 
         self.packet_headers_default = \
-            ['common_run_name', 'tag_run_location', 'test_num', 'external_id', 'time_from_start', 'raw_packet', 'rssi',
+            ['common_run_name', 'tag_run_location', 'tag_reel_location', 'test_num', 'external_id', 'time_from_start',
+             'raw_packet', 'rssi',
              'packet_status', 'adv_address', 'selected_tag', 'is_test_pass', 'status_offline', 'fail_bin',
              'fail_bin_str',
              'test_status', 'num_packets', 'num_cycles', 'sprinkler_counter_mean', 'sprinkler_counter_std',
              'sprinkler_counter_min', 'sprinkler_counter_max', 'tbp_mean', 'tbp_std', 'tbp_min', 'tbp_max',
              'tbp_num_vals',
              'per_mean', 'per_std', 'rssi_mean', 'rssi_std', 'rssi_min', 'rssi_max', 'ttfp', 'rx_rate_normalized',
              'rx_rate', 'total_test_duration', 'total_location_duration', 'test_start_time', 'trigger_time',
@@ -838,18 +874,48 @@
         self.r2r_timer = None
         self.test_suites_timer = None
         self.timer_for_curr_test = ''
         # self.printed_external_id = ''
         self.next_printed_external_id = ''
         self.timer_for_duplication_handling = None
         self.fail_tags_with_same_packet_within_secs = False
+        self.enable_line_selection = self.ports_and_guis.Tag_Printing_Value['enableLineSelection'].lower() == 'yes' \
+            if self.to_print else False
 
         self.tag_location = 0
         self.events.tag_thread_is_ready_to_main.set()
 
+    def call_printer_validation(self):
+        if self.to_print and not self.ports_and_guis.print_test:
+            self.events.printer_validation_success.clear()
+            self.events.qr_read_success.clear()
+            if self.qr_enable == 'Yes':
+                if self.events.qr_queue.full():
+                    self.events.start_compare.set()  # start qr readout
+                    self.ports_and_guis.my_logger.logger.info('Sent start to test QR')
+                else:
+                    self.events.qr_read_success.set()
+                    self.ports_and_guis.my_logger.logger.info('Queue not full yet')
+
+            else:
+                self.events.start_compare.set()
+
+    def check_printer_validation(self):
+        if self.to_print and not self.ports_and_guis.print_test:
+            self.events.validation_success.wait(timeout=5)
+            if not self.events.validation_success.isSet():
+                self.ports_and_guis.my_logger.logger.warning(
+                    "QR Validation didn't succeed or Printer counter is not right")
+                self.events.stop_to_r2r_thread.set()
+                self.events.done_to_tag_thread.set()
+            else:
+                self.ports_and_guis.my_logger.logger.info('Validation is ok')
+            self.events.printer_validation_success.clear()
+            self.events.qr_read_success.clear()
+
     @pyqtSlot()
     def run(self):
         """
         runs the thread
         """
         global problem_in_locations_hist, fail_bin_list
         problem_in_locations_hist = {'NO_RESPONSE': 0, 'NO_PACKETS_UNDER_RSSI_THR': 0, 'MISSING_LABEL': 0,
@@ -893,68 +959,80 @@
                     # will wait 10 seconds after the tag timer should have ended
                     # and then will enforce a start_r2r & fail_r2r
 
                     # self.r2r_timer = threading.Timer(self.time_out_to_missing_label, self.end_of_time,
                     #                                  ['r2r is stuck'])
                     # self.r2r_timer.start()
                     self.start_time = datetime.datetime.now()
-                    if self.to_print and not self.ports_and_guis.print_test:
-                        self.events.printer_validation_success.clear()
-                        self.events.qr_read_success.clear()
-                        if self.qr_enable == 'Yes':
-                            if self.events.qr_queue.full():
-                                self.events.start_compare.set()  # start qr readout
-                                self.ports_and_guis.my_logger.logger.info('Sent start to test QR')
-                            else:
-                                self.events.qr_read_success.set()
-                                self.ports_and_guis.my_logger.logger.info('Que not full yet')
 
-                        else:
-                            self.events.start_compare.set()
                     if self.events.done_to_tag_thread.is_set():
                         break
                     self.ports_and_guis.my_logger.results_logger.info(
                         '******************** New tag test starts at location: {}, excpected externalID is: {} ******'
                         '**************'.format(
                             str(self.tag_location), str(self.next_printed_external_id)))
 
                     if self.ports_and_guis.energizerGW:
-                        if self.ports_and_guis.additional_gw_mode == DualGWMode.DYNAMIC:
-                            self.stop_energizer()
-                        elif self.ports_and_guis.additional_gw_mode == DualGWMode.MIRROR:
-                            self.start_energizer()
                         if 'DelayBeforeTest' in self.ports_and_guis.tests_suite['additionalGW']:
                             time.sleep(int(self.ports_and_guis.tests_suite['additionalGW']['DelayBeforeTest']))
 
                     if self.extended_test:
                         self.ports_and_guis.my_logger.logger.info('Waiting for pulse')
                         self.pulse_received = self.WiliotTester.wait_for_trigger(wait_for_gw_trigger)
                         if self.pulse_received:
                             self.ports_and_guis.my_logger.logger.info('Pulse received')
                             self.events.stop_to_test_r2r_thread.set()
                             while self.events.stop_to_test_r2r_thread.is_set():
                                 time.sleep(0.01)
                                 pass
-                            self.tester_res = self.WiliotTester.run(wait_for_gw_trigger=None)
+                            self.tester_res = self.WiliotTester.run(wait_for_gw_trigger=None,
+                                                                    need_to_manual_trigger=False)
                             self.events.start_to_test_r2r_thread.set()
                             while self.events.start_to_test_r2r_thread.is_set():
                                 time.sleep(0.01)
                                 pass
                         else:
                             self.ports_and_guis.my_logger.logger.info("Pulse didn't received")
                             self.tester_res = WiliotTesterTagResultList()  # Empty list
 
                     else:
-                        self.tester_res = self.WiliotTester.run(wait_for_gw_trigger=wait_for_gw_trigger)
+                        # get trigger:
+                        self.ports_and_guis.my_logger.logger.info('Waiting for pulse')
+                        self.pulse_received = self.WiliotTester.wait_for_trigger(wait_for_gw_trigger)
+                        self.call_printer_validation()
+                        if self.pulse_received:
+                            self.ports_and_guis.my_logger.logger.info('Pulse received')
+                            if self.ports_and_guis.energizerGW:
+                                if self.ports_and_guis.additional_gw_mode == DualGWMode.DYNAMIC:
+                                    self.stop_energizer()
+                                elif self.ports_and_guis.additional_gw_mode == DualGWMode.MIRROR:
+                                    self.start_energizer()
+                                elif self.ports_and_guis.additional_gw_mode == DualGWMode.STATIC and 'lite_power' in \
+                                        self.tests_suite['additionalGW']:
+                                    self.ports_and_guis.energizerGW.config_gw(
+                                        output_power_val=self.tests_suite['additionalGW']['lite_power'])
+
+                            # start tag test
+                            self.tester_res = self.WiliotTester.run(wait_for_gw_trigger=None,
+                                                                    need_to_manual_trigger=False)
+                        else:
+                            self.ports_and_guis.my_logger.logger.info("Pulse didn't received")
+                            self.tester_res = WiliotTesterTagResultList()  # Empty list
+                    # end tag test
 
                     if self.ports_and_guis.energizerGW:
                         if self.ports_and_guis.additional_gw_mode == DualGWMode.DYNAMIC:
                             self.start_energizer()
                         elif self.ports_and_guis.additional_gw_mode == DualGWMode.MIRROR:
                             self.stop_energizer()
+                        elif self.ports_and_guis.additional_gw_mode == DualGWMode.STATIC and 'lite_power' in \
+                                self.tests_suite['additionalGW']:
+                            self.ports_and_guis.energizerGW.config_gw(
+                                output_power_val=self.tests_suite['additionalGW']['gw_output_power'])
+
                         if 'DelayAfterTest' in self.ports_and_guis.tests_suite['additionalGW']:
                             time.sleep(self.ports_and_guis.tests_suite['additionalGW']['DelayAfterTest'])
 
                     if self.ports_and_guis.temperature_enabled:
                         # self.ports_and_guis.my_logger.logger.debug('Receiving tempreture data from sensor')
                         try:
                             temperature_sensor = get_temperature()
@@ -963,31 +1041,23 @@
                             self.ports_and_guis.my_logger.logger.warning('Problem with temperature sensor detection')
                             pass
                         self.ports_and_guis.my_logger.logger.debug('Temperature is: {}'.format(str(temperature_sensor)))
                     else:
                         temperature_sensor = float(-1)
 
                     self.test_data['tag_run_location'] = self.tag_location
+                    self.test_data['tag_reel_location'] = int(self.tag_reel_location) + int(self.tag_location)
                     self.test_data['temperature_sensor'] = temperature_sensor
                     if self.events.done_to_tag_thread.is_set():
                         break
-
+                    # printing processes:
                     if self.to_print and not self.ports_and_guis.print_test:
                         self.test_data['external_id'] = self.printed_external_id
                         self.ports_and_guis.my_logger.logger.info('Making sure printer or QR doesnt have failures')
-                        self.events.validation_success.wait(timeout=5)
-                        if not self.events.validation_success.isSet():
-                            self.ports_and_guis.my_logger.logger.warning(
-                                "QR Validation didn't succeed or Printer counter is not right")
-                            self.events.stop_to_r2r_thread.set()
-                            self.events.done_to_tag_thread.set()
-                        else:
-                            self.ports_and_guis.my_logger.logger.info('Validation is ok')
-                        self.events.printer_validation_success.clear()
-                        self.events.qr_read_success.clear()
+                        self.check_printer_validation()
 
 
                     try:
                         if self.events.done_to_tag_thread.is_set():
                             break
                         tested += 1
                         if self.tester_res.is_results_empty():
@@ -1009,14 +1079,16 @@
                             self.update_packet_data(packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data)
                             if self.to_print and not self.ports_and_guis.print_test:
                                 self.events.qr_queue.put({'externalID': 'Missing Label', 'status': 'Fail'})
+                                if self.enable_line_selection:
+                                    self.events.tag_status_queue.put('fail')
                                 self.ports_and_guis.my_logger.logger.debug('Added missing label to que as fail')
                             # self.events.enable_missing_label_to_r2r_thread.set()
                             if self.missing_labels_in_a_row >= int(self.value['maxMissingLabels']):
                                 self.ports_and_guis.my_logger.logger.warning('Max missing labels were detected')
                                 self.events.done_to_r2r_thread.set()
                                 self.events.done_to_tag_thread.set()
                                 if self.to_print:
@@ -1037,25 +1109,26 @@
 
                             if self.ttfp_num:
                                 self.run_data['ttfp_avg'] = self.ttfp_sum / self.ttfp_num
 
                             selected_tag = self.tester_res.check_and_get_selected_tag_id()
                             if selected_tag == '':
                                 # Didnt understand who is talking in different stages or the case no tag was selected
-                                # self.ports_and_guis.my_logger.logger.warning(
-                                #     'Tag location: {} failed - TIMEOUT OR TAG_NOT_SELECTED'.format(str(self.tag_location)))
+
                                 try:
                                     self.ports_and_guis.my_logger.logger.warning(
                                         'Tag location: {} failed - {}'.format(self.tag_location,
                                                                               self.tester_res.get_total_fail_bin(
                                                                                   as_name=True)))
                                 except Exception:
                                     pass
                                 if self.to_print and not self.ports_and_guis.print_test:
                                     self.events.qr_queue.put({'externalID': '', 'status': 'Fail'})
+                                    if self.enable_line_selection:
+                                        self.events.tag_status_queue.put('fail')
                                     self.ports_and_guis.my_logger.logger.debug(
                                         'Tag added as fail')
                                 self.events.fail_to_r2r_thread.set()
 
                             else:
                                 if selected_tag in self.all_selected_tags:
                                     # Duplication
@@ -1065,18 +1138,22 @@
                                     self.black_list.append(selected_tag)
                                     self.ports_and_guis.my_logger.logger.warning(
                                         'Tag location: {} has been already seen in the run before'.format(str(self.tag_location)))
                                     self.tester_res.set_packet_status(adv_address=selected_tag,
                                                                       status='duplication')
                                     if self.to_print and not self.ports_and_guis.print_test:
                                         self.events.qr_queue.put({'externalID': selected_tag, 'status': 'Fail'})
+                                        if self.enable_line_selection:
+                                            self.events.tag_status_queue.put('fail')
 
-                                    if int(self.black_list.count(selected_tag)) >=  self.maxblackappear:
+                                    if int(self.black_list.count(selected_tag)) >= self.maxblackappear:
                                         self.WiliotTester.add_to_blacklist(selected_tag)
-                                        self.ports_and_guis.my_logger.logger.warning('Tag {} in location {} has reached max appearance in black list'.format(selected_tag, self.tag_location))
+                                        self.ports_and_guis.my_logger.logger.warning(
+                                            'Tag {} in location {} has reached max appearance in black list'.format(
+                                                selected_tag, self.tag_location))
                                     self.events.fail_to_r2r_thread.set()
 
                                 else:
                                     # Tag pass or fail but with respond
                                     self.missing_labels_in_a_row = 0
                                     self.all_selected_tags.append(selected_tag)
                                     if self.tester_res.is_all_tests_passed():
@@ -1097,27 +1174,32 @@
                                             self.test_data['external_id'] = self.printed_external_id
 
                                             last_pass_string = f'advAddress: {str(selected_tag)} , Tag Location:  ' \
                                                                f'{str(self.tag_location)} , External ID: {self.printed_external_id} '
                                             # f', RSSI: 'f'{self.rssi}, TBP: {self.tbp}, TTFP: {self.ttfp}'
                                             self.events.qr_queue.put(
                                                 {'externalID': self.printed_external_id, 'status': 'Pass'})
+                                            if self.enable_line_selection:
+                                                self.events.tag_status_queue.put('pass')
                                             self.ports_and_guis.my_logger.logger.info(
                                                 'Added tag {} to que as pass'.format(self.printed_external_id))
                                             self.externalId += 1
                                         else:
                                             last_pass_string = f'Tag Location:  {str(self.tag_location)}'
                                         self.events.pass_to_r2r_thread.set()
                                     else:
                                         # Tag failed statistics
                                         self.ports_and_guis.my_logger.logger.warning(
                                             'Tag location: {} failed - {}'.format(str(self.tag_location), str(
                                                 self.tester_res.get_total_fail_bin(as_name=True))))
                                         if self.to_print and not self.ports_and_guis.print_test:
                                             self.events.qr_queue.put({'externalID': '', 'status': 'Fail'})
+                                            if self.enable_line_selection:
+                                                self.events.tag_status_queue.put('pass')
+
                                             self.ports_and_guis.my_logger.logger.debug(
                                                 'Tag added as fail, failed during test')
                                         self.events.fail_to_r2r_thread.set()
                             self.all_tags += self.tester_res.get_test_unique_adva()
                             self.all_tags = list(set(self.all_tags))
                             self.run_data['total_run_responding_tags'] = len(self.all_tags)
                             total_loc_time = datetime.datetime.now() - self.start_time
@@ -1126,14 +1208,25 @@
                             self.update_packet_data(res=self.tester_res,
                                                     packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data, res=self.tester_res)
                         self.tag_location += 1
+                        # Check the diff critiria
+                        if self.pass_response_diff is not None:
+                            if len(self.all_tags) > self.pass_response_diff_offset:
+                                if (passed*100)/len(self.all_tags) < 100-int(self.pass_response_diff):
+                                    self.ports_and_guis.my_logger.logger.warning(
+                                        'Problem with setup, stop criteria for responsive tags and pass tags diff is '
+                                        'lower then threshold please check setup or change the value')
+                                    self.events.done_to_r2r_thread.set()
+                                    self.events.done_to_tag_thread.set()
+                                    if self.to_print:
+                                        self.events.done_to_printer_thread.set()
                         # update extended results:
                         if self.tester_res.is_results_empty():
                             fail_bin_list.append(FailureCodes.MISSING_LABEL.name)
                         else:
                             fail_bin_list.append(self.tester_res.get_total_fail_bin(as_name=True))
 
                         # end of tags loop ###############################
@@ -1163,20 +1256,14 @@
                     die = True
                 exception_details = sys.exc_info()
                 self.exception_queue.put(exception_details)
                 # wait until user press Continue
                 if self.r2r_timer is not None:
                     self.r2r_timer.cancel()
 
-                if not die:
-                    self.events.cont_to_tag_thread.wait()
-                self.events.cont_to_tag_thread.clear()
-                self.events.pause_to_tag_thread.clear()
-                self.events.cont_to_main_thread.set()
-
         self.closure_fn()
 
     def end_of_time(self, kind):
         """
         sets the correct flag to True when a timer is done
         @param kind: the kind of the timer
         """
@@ -1256,20 +1343,35 @@
 
         self.internal_value = {"energizingPattern": "-1", "timeProfile": "-1", "txPower": "-1", "rssiThresholdHW":
             str(self.tests_suite['rssiThresholdHW']), "rssiThresholdSW": str(self.tests_suite['rssiThresholdSW']),
                                "plDelay": str(self.tests_suite['plDelay'])}
         # for the case we do not print
         self.externalId = 0
         self.pass_job_name = ''
+        self.tag_reel_location = 0
         if self.value['toPrint'] == 'Yes':
             self.to_print = True
             self.printing_value, is_OK = self.ports_and_guis.Tag_Printing_Value, self.ports_and_guis.Tag_is_OK
             self.externalId = int(self.printing_value['firstPrintingValue'])
             self.pass_job_name = self.printing_value['passJobName']
-            self.tag_location = int(self.printing_value['tagLocation'])
+            self.tag_reel_location = int(self.printing_value['tag_reel_location'])
+
+        if 'pass_response_diff' in self.ports_and_guis.Tag_Value:
+            try:
+                self.pass_response_diff = int(self.ports_and_guis.Tag_Value['pass_response_diff'])
+            except Exception as e:
+                self.ports_and_guis.my_logger.logger.warning(f'Could not convert the pass_response_diff to number, '
+                                                             f'the defualt value would be 10: {e}')
+                self.pass_response_diff = 10
+            if 'pass_response_diff_offset' in self.ports_and_guis.Tag_Value:
+                self.pass_response_diff_offset = int(self.ports_and_guis.Tag_Value['pass_response_diff_offset'])
+            else:
+                self.pass_response_diff_offset = 100
+        else:
+            self.pass_response_diff = None
 
         # setting up the global variables ###################################################
         global desired_pass_num
         global desired_tags_num
         desired_tags_num = int(self.value['desiredTags'])
         desired_pass_num = int(self.value['desiredPass'])
 
@@ -1369,14 +1471,15 @@
             default_data = {'raw_packet': None, 'adv_address': None, 'decrypted_packet_type': None,
                             'group_id': None, 'flow_ver': None,
                             'test_mode': None, 'en': None, 'type': None, 'data_uid': None, 'nonce': None,
                             'enc_uid': None, 'mic': None, 'enc_payload': None, 'gw_packet': None, 'rssi': None,
                             'stat_param': None, 'time_from_start': None, 'counter_tag': None,
                             'is_valid_tag_packet': None, 'common_run_name': test_data['common_run_name'],
                             'tag_run_location': test_data['tag_run_location'],
+                            'tag_reel_location': test_data['tag_reel_location'],
                             'total_test_duration': test_data['total_test_duration'],
                             'total_location_duration': test_data['total_location_duration'],
                             'status_offline': test_data['status_offline'],
                             'fail_bin': test_data['fail_bin'], 'fail_bin_str': test_data['fail_bin_str'],
                             'external_id': None,
                             'qr_validated': test_data['qr_validated'], 'test_num': test_data['test_num'],
                             'trigger_time': test_data['trigger_time'], 'packet_status': None,
@@ -1430,26 +1533,28 @@
 
     def run_data_init(self):
         global run_start_time, common_run_name, tested
         if self.value['toPrint'] == 'Yes':
 
             self.init_external_id = self.printing_value['firstPrintingValue']
             self.string_before_counter = self.printing_value['stringBeforeCounter']
-            printing_format = self.printing_value['passJobName']
+            printing_format = self.printing_value['printingFormat']
+            print_pass_job_name = self.printing_value['passJobName']
             self.printed_external_id, is_ok = get_printed_value(string_before_the_counter=self.string_before_counter,
                                                                 digits_in_counter=4,
                                                                 first_counter=self.init_external_id,
                                                                 printing_format=printing_format)
 
         else:
             self.init_external_id = '0000'
             self.init_counter = '0000'
             self.string_before_counter = ''
             self.printed_external_id = ''
             printing_format = 'TEST'
+            print_pass_job_name = ''
         # self.printed_external_id = self.first_externalID
 
         self.run_data = {'common_run_name': common_run_name,
                          'tester_station_name': self.ports_and_guis.tag_tester_station_name,
                          'operator': self.ports_and_guis.Tag_Value['operator'], 'reel_run_start_time': run_start_time_,
                          'reel_run_end_time': None,
                          'batch_name': self.ports_and_guis.Tag_Value['batchName'],
@@ -1462,29 +1567,29 @@
                          'conversion_type': ConversionTypes(self.ports_and_guis.Tag_Value['conversion']).name,
                          'inlay': InlayTypes(self.ports_and_guis.Tag_Value['inlay']).name,
                          'test_suite': self.ports_and_guis.Tag_Value['inlayType'],
                          'test_suite_dict': self.ports_and_guis.tests_suite,
                          'surface': SurfaceTypes(self.ports_and_guis.Tag_Value['surface']).name,
                          'to_print': self.ports_and_guis.Tag_Value['toPrint'],
                          'qr_validation': self.ports_and_guis.Tag_Value['QRRead'],
-                         'print_pass_job_name': 'SGTIN_QR', 'printing_format': printing_format,
+                         'print_pass_job_name': print_pass_job_name, 'printing_format': printing_format,
                          'external_id_prefix': self.string_before_counter,
                          'external_id_suffix_init_value': self.init_external_id,
                          'coupler_partnumber': '',
                          'gw_version': self.ports_and_guis.ver, 'py_wiliot_version': get_version(), 'upload_date': None,
                          'owner_id': 'wiliot-ops', 'temperature_sensor_enable': self.ports_and_guis.temperature_enabled,
                          'ttfp_avg': float('nan')}
 
         self.test_data = {'common_run_name': common_run_name, 'tag_run_location': tested,
                           'total_location_duration': None, 'total_test_duration': None,
                           'status_offline': False, 'fail_bin': FailureCodes.NONE.value,
                           'fail_bin_str': FailureCodes.NONE.name,
                           'external_id': self.printed_external_id,
                           'qr_validated': self.qr_enable, 'trigger_time': None,
-                          'test_num': 0, 'temperature_sensor': float(-1)}
+                          'test_num': 0, 'temperature_sensor': float(-1), 'tag_reel_location': self.tag_reel_location}
 
 
 class R2RThread(threading.Thread):
     """
     Thread that controls R2R machine
 
     Parameters:
@@ -1628,15 +1733,14 @@
                     self.my_gpio.gpio_state(4, "OFF")
                     self.events.disable_missing_label_to_r2r_thread.clear()
                     self.en_missing_label = False
             except Exception:
                 exception_details = sys.exc_info()
                 self.exception_queue.put(exception_details)
                 self.events.stop_to_r2r_thread.set()  # to avoid from the run to continue printing in this case
-                self.events.cont_to_tag_thread.wait()
 
 
 class MainEvents:
     """
     Contains events that connect between all threads
     Events are set or cleared by threads
     Events are divided to four primary groups:
@@ -1660,33 +1764,30 @@
         self.pass_to_r2r_thread = threading.Event()
         self.fail_to_r2r_thread = threading.Event()
         self.stop_to_test_r2r_thread = threading.Event()
         self.start_to_test_r2r_thread = threading.Event()
         # set by main
         self.start_to_r2r_thread = threading.Event()
         self.stop_to_r2r_thread = threading.Event()
-        self.cont_to_tag_thread = threading.Event()
         self.stop_main_trigger = threading.Event()
         # only to be sure we initialize the counters to the printer counter
-        self.cont_to_printer_thread = threading.Event()
-        self.cont_to_main_thread = threading.Event()
-        self.pause_to_tag_thread = threading.Event()
         self.enable_missing_label_to_r2r_thread = threading.Event()
         self.disable_missing_label_to_r2r_thread = threading.Event()
         self.done_to_tag_thread = threading.Event()
         self.done_to_printer_thread = threading.Event()
         self.done2r2r_ready = threading.Event()
         self.done_to_r2r_thread = threading.Event()
         self.tag_thread_is_ready_to_main = threading.Event()
 
         # set by r2r
         # both printer and tag thread will wait on it. only printer will .clear() it (in printing mode)
         self.r2r_ready = threading.Event()
         # start qr read_out
         self.qr_queue = Queue()
+        self.tag_status_queue = Queue()
         self.start_compare = threading.Event()
         self.qr_read_success = threading.Event()
         # printer events
         self.was_pass_to_printer = threading.Event()
         self.was_fail_to_printer = threading.Event()
         self.printer_success = threading.Event()
         self.printer_error = threading.Event()
@@ -1739,14 +1840,18 @@
         # Getting the config values
         self.init_config_values()
         self.tests_suite = self.all_tests_suites[self.Tag_Value['inlayType']]
         self.total_time = 0
         for stage in self.tests_suite['tests']:
             if 'maxTime' in stage.keys():
                 self.total_time += stage['maxTime']
+            if 'delayBeforeNextTest' in stage.keys():
+                self.total_time += stage['delayBeforeNextTest']
+            if 'DelayAfterTest' in stage.keys():
+                self.total_time += stage['DelayAfterTest']
         # for Tag thread ###########
         # check if production mode or test mode to set environment for cloud_api
         env = self.Tag_Value['Environment']
         owner_id = self.Tag_Value['OwnerId']
         if 'prod' in env:
             self.env = ''
         elif 'test' in env:
@@ -1757,23 +1862,24 @@
         print('Starting run in {} mode'.format(str(self.env)))
         # printing values (2nd GUI)
         self.print_test = False
         if self.Tag_Value['toPrint'] == 'Yes':
             self.to_print = True
             if self.Tag_Value['printingFormat'] == 'Test':
                 self.print_test = True
-                self.Tag_Printing_Value, self.Tag_is_OK = printing_test_window(self.env)
+                self.Tag_Printing_Value, self.Tag_is_OK = printing_test_window()
                 if not self.Tag_is_OK:
                     msg = 'Impossible printing values entered by the user, the program will exit now'
                     printing_func(msg, 'PortsAndGuis', lock_print, logger_type='debug',
                                   logger_name=self.my_logger.logger.name)
                     sys.exit(0)
 
-            elif self.Tag_Value['printingFormat'] == 'SGTIN':
-                self.Tag_Printing_Value, self.Tag_is_OK = printing_sgtin_window(self.env, owner_id)
+            elif self.Tag_Value['printingFormat'] == 'SGTIN' or self.Tag_Value['printingFormat'] == 'Barcode':
+                self.Tag_Printing_Value, self.Tag_is_OK = printing_sgtin_window(self.env, owner_id,
+                                                                                self.Tag_Value['printingFormat'])
                 if not self.Tag_is_OK:
                     msg = 'user exited the program'
                     printing_func(msg, 'PortsAndGuis', lock_print, logger_type='debug',
                                   logger_name=self.my_logger.logger.name)
                     sys.exit(0)
             else:
                 msg = 'user chose unsupported printing format!!!'
@@ -1816,29 +1922,27 @@
         # check if the system variable exist
         assert ('testerStationName' in os.environ), 'testerStationName is missing from PC environment variables, ' \
                                                     'please add it in the following convention:' \
                                                     ' <company name>_<tester number>'
         self.tag_tester_station_name = os.environ['testerStationName']
         # serial for GW
         self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.my_logger.gw_logger.name,
-                                   is_multi_processes=True)
+                                   is_multi_processes=True, log_dir_for_multi_processes=os.path.join(self.new_path,
+                                                                                                     common_run_name))
         self.ver, _ = self.GwObj.get_gw_version()
 
         if 'additionalGW' in self.tests_suite:
             self.energizerGW = WiliotGateway(logger_name=self.my_logger.gw_logger.name, port=self.tests_suite['additionalGW']['port'])
             if self.energizerGW.connected:
                 self.energizerGW.reset_gw()
                 sleep(1)
-                self.energizerGW.write('!enable_brg_mgmt 0', with_ack=True)
                 self.energizerGW.write('!listen_to_tag_only 1', with_ack=True)
-                self.energizerGW.write('!energizing_prob_set 100', with_ack=True)
-                self.energizerGW.write('!set_pacer_interval 0', with_ack=True)
-                self.energizerGW.write('!set_packet_filter_off', with_ack=True)
                 self.energizerGW.write('!set_tester_mode 1', with_ack=True)
                 self.energizerGW.write('!pl_gw_config 0', with_ack=True)
+                self.energizerGW.write('!sub1g_sync 1', with_ack=True)
 
                 try:
                     self.additional_gw_mode = DualGWMode(self.tests_suite['additionalGW']['mode'])
                 except Exception as e:
                     raise Exception('no mode in additionalGW dict in test suite or invalid mode: {}'.format(e))
 
                 self.energizerGW.config_gw(energy_pattern_val=self.tests_suite['additionalGW']['energizingPattern'],
@@ -1862,15 +1966,15 @@
 
 
 
         # for Printer thread ###########
         self.Printer_socket = ''  # will only be opened by the thread
         if self.Tag_Value['printingFormat'] == 'Test':
             self.filename = 'gui_printer_inputs_4_Test_do_not_delete.json'
-        elif self.Tag_Value['printingFormat'] == 'SGTIN':
+        elif self.Tag_Value['printingFormat'] == 'SGTIN' or self.Tag_Value['printingFormat'] == 'Barcode':
             self.filename = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
 
         else:
             msg = 'The print Job Name inserted is not supported at the moment, You will need to press Stop'
             printing_func(msg, 'PortsAndGuis', lock_print, logger_type='debug', logger_name=self.my_logger.logger.name)
 
         # check printing configs and save it locally
@@ -2103,27 +2207,23 @@
             look_for_exceptions() will call handle_r2r_exception() which prints and handles the exception if possible
 
     Events:
         listen/ waits on:
             events.tag_thread_is_ready_to_main => event from TagThread. if set, TagThread is ready
             events.printer_event => wait for response from printer (printer_success or printer_error)
             events.printer_success => the last print was successful
-            events.cont_to_main_thread => continue response received from TagThread
             events.r2r_ready => notify if R2R in ready for movement
 
         sets:
             events.start_to_r2r_thread => enable/disable R2R movement. Sends pulse on "Start/Stop machine" GPIO line
             events.stop_to_r2r_thread => stops the R2R from running in case of end of run or exception
-            events.pause_to_tag_thread => pauses TagThread if exception happened of user pressed Pause
             events.done_to_tag_thread => closes TagThread at the end of the run
-            events.cont_to_tag_thread => send continue to paused TagThread after user pressed continue
             events.done2r2r_ready => closes R2RThread
             events.done_to_r2r_thread => kills R2R thread main loop if set
             events.done_to_printer_thread => user pressed Stop (end the program) - to avoid deadlock
-            events.cont_to_printer_thread => send continue to PrinterThread after Continue pressed by user
 
 
     Logging:
         logging to logging.debug() and logging.info()
     """
     sig = pyqtSignal(str)
 
@@ -2179,26 +2279,27 @@
             if self.no_gui:
                 if os.path.isfile(path=self.test_config_path):
                     with open(self.test_config_path, 'r') as f:
                         gui_configs = json.load(f)
                         if 'upload_to_cloud' in gui_configs and gui_configs['upload_to_cloud'].lower() == 'no':
                             self.cloud_connection = False
             if self.cloud_connection:
-                file_path, api_key, is_successful = check_user_config_is_ok(env=self.ports_and_guis.env)
+                file_path, api_key, is_successful = check_user_config_is_ok(env=self.ports_and_guis.env,
+                                                                            owner_id=self.ports_and_guis.Tag_Value[
+                                                                                'OwnerId'])
                 self.client = ManufacturingClient(api_key=api_key, env=self.ports_and_guis.env,
                                                   logger_=self.ports_and_guis.my_logger.logger.name,
                                                   log_file=self.ports_and_guis.my_logger.log_path)
 
             self.r2r_thread = R2RThread(self.events, self.ports_and_guis, no_gui=self.no_gui)
             self.tag_checker_thread = TagThread(self.events, self.ports_and_guis)
 
             if (self.printer is not None and not self.printer.exception_queue.empty()) or \
                     not self.tag_checker_thread.exception_queue.empty() or not self.r2r_thread.exception_queue.empty():
                 self.events.stop_to_r2r_thread.set()
-                self.events.pause_to_tag_thread.set()
                 self.handle_r2r_exception()
                 self.init_ok = False
 
             if self.to_scan == 'Yes':
                 self.tag_comparing_qr = QRThread(self.events, self.ports_and_guis)
 
             self.events.tag_thread_is_ready_to_main.wait()
@@ -2251,40 +2352,26 @@
 
     def open_ui(self):
         """
         opens the run main GUI that will present the run data and gives to the user ability to Stop/Continue/Pause
         """
         self.stop_label = QLabel("If you want to stop this run, press stop")
         self.stop_label.setFont(QFont('SansSerif', 10))
-        self.cont_label = QLabel("If you want to skip and fail at this location, press Continue")
-        self.cont_label.setFont(QFont('SansSerif', 10))
         self.reel_label = QLabel("Reel Name: ")
         self.reel_label.setFont(QFont('SansSerif', 10))
         self.reel_label.setStyleSheet('.QLabel {padding-top: 10px; font-weight: bold; font-size: 25px; color:#ff5e5e;}')
         self.reel_label.setFont(QFont('SansSerif', 10))
         self.tested = QLabel("Tested = 0, Passed = 0, Yield = -1%")
         self.tested.setFont(QFont('SansSerif', 10))
         self.last_tag_str = QLabel("Last Tag Passed: ")
         self.last_tag_str.setFont(QFont('SansSerif', 10, weight=QFont.Bold))
         self.last_pass = QLabel("No tag has passed yet :(")
         self.last_pass.setFont(QFont('SansSerif', 10))
         layout = QVBoxLayout()
 
-        self.continue_ = QPushButton("Continue")
-        self.continue_.setStyleSheet("background-color: grey")
-        self.continue_.setFont(QFont('SansSerif', 10))
-        self.continue_.setFixedSize(QSize(300, 22))
-        self.continue_.pressed.connect(self.continue_fn)
-        self.continue_.setEnabled(False)
-        self.pause = QPushButton("Pause")
-        self.pause.setStyleSheet("background-color: grey")
-        self.pause.setFont(QFont('SansSerif', 10))
-        self.pause.setFixedSize(QSize(300, 22))
-        self.pause.pressed.connect(self.pause_fn)
-        self.pause.setEnabled(False)
         self.stop = QPushButton("Stop")
         self.stop.setStyleSheet("background-color: #FD4B4B")
         self.stop.setFont(QFont('SansSerif', 10))
         self.stop.setFixedSize(QSize(300, 22))
         self.stop.pressed.connect(self.close)
 
         self.c = ConsolePanelHandler_GUI(self.sig)
@@ -2314,17 +2401,14 @@
                                   str(self.calculate_on) + "]", **styles)
         pen = pg.mkPen(color=(255, 0, 0))
         self.data_line = self.graphWidget.plot(self.x, self.y, pen=pen)
         self.versions = QLabel("PyWiliot Version: {}\nGW Version: {}".format(self.wiliot_ver, self.gw_version))
         self.versions.setFont(QFont('SansSerif', 10, weight=QFont.Bold))
 
         layout.addWidget(self.reel_label)
-        # layout.addWidget(self.cont_label)
-        # layout.addWidget(self.continue_)
-        # layout.addWidget(self.pause)
         layout.addWidget(self.stop_label)
         layout.addWidget(self.stop)
         layout.addWidget(self.last_tag_str)
         layout.addWidget(self.last_pass)
         layout.addWidget(self.tested)
         # layout.addWidget(self.debug)
         layout.addWidget(self.text_box)
@@ -2379,15 +2463,15 @@
                 #     tested = tested - 1
                 yield_ = passed / tested * 100
             else:
                 if passed == 0:
                     yield_ = 0
                 else:
                     yield_ = 100
-        self.events.pause_to_tag_thread.set()
+
         if self.ports_and_guis.GwObj.connected:
             self.update_timer.stop()
         # self.close()
         ttfgp_avg = None
         if len(self.tag_checker_thread.ttfgp_list) > 0:
             ttfgp_avg = mean(self.tag_checker_thread.ttfgp_list)
         self.events.done_to_tag_thread.set()
@@ -2395,15 +2479,14 @@
             time.sleep(0.5)
         # check logging due to printing offset:
         if self.ports_and_guis.Tag_Value['toPrint'] == 'Yes':
             self.check_logging_due_to_printing_offset()
 
         self.events.done_to_printer_thread.set()
         self.events.done2r2r_ready.set()
-        self.events.cont_to_tag_thread.set()  # to avoid deadlock
         self.events.done_to_r2r_thread.set()
         self.events.start_compare.clear()
 
         if self.ports_and_guis.energizerGW:
             self.ports_and_guis.energizerGW.write('cancel')
             self.ports_and_guis.energizerGW.exit_gw_api()
         if self.r2r_thread.is_alive():
@@ -2443,29 +2526,29 @@
         env_dirs = WiliotDir()
         WILIOT_DIR = env_dirs.get_wiliot_root_app_dir()
         machine_dir = join(WILIOT_DIR, 'offline')
         local_config_dir = join(machine_dir, 'configs')
 
         if self.to_print:
             self.events.done_to_printer_thread.set()
-            if self.tag_checker_thread.value['printingFormat'] == 'SGTIN':
-                filename = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
-                printing_format = 'SGTIN'
-            else:
+            printing_format = self.tag_checker_thread.value['printingFormat']
+            if printing_format == 'Test':
                 filename = 'gui_printer_inputs_4_Test_do_not_delete.json'
-                printing_format = 'Test'
+            else:
+                filename = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
 
             app_dir = os.path.abspath(os.path.dirname(__file__))
             self.folder_path = join(app_dir, 'configs')
             data = open_json(folder_path=self.folder_path, file_path=os.path.join(self.folder_path, filename),
                              default_values=DefaultGUIValues(printing_format).default_gui_values)
             last_printing_value = last_pass_string.split()
             if passed > 0:
                 data['firstPrintingValue'] = str(int(self.tag_checker_thread.externalId))
                 data['tagLocation'] = str(int(self.tag_checker_thread.tag_location))
+                data['tag_reel_location'] = str(int(self.tag_checker_thread.test_data['tag_reel_location']))
             f = open(os.path.join(self.folder_path, filename), "w")
             json.dump(data, f)
             f.close()
 
             if self.to_print:
                 if self.ports_and_guis.Tag_Value['QRRead'] != 'Yes':
                     self.printer.closure()
@@ -2525,43 +2608,14 @@
 
         self.ports_and_guis.my_logger.results_logger.info('Run finished')
         # window.close()
         self.ports_and_guis.R2R_myGPIO.__del__()
         time.sleep(1)
         sys.exit(0)
 
-    def continue_fn(self):
-        """
-        will be triggered by the Continue button and will resume the run after Pause/ run got stuck if possible.
-        """
-        if not self.events.cont_to_tag_thread.isSet() and not self.waiting_for_user_to_press_stop_because_printer \
-                and not self.tag_checker_thread.fetal_error:
-            msg = "User pressed continue, the R2R will advance now (the last spot will be fail)"
-            printing_func(msg, 'MainWindow', lock_print, logger_type='warning',
-                          logger_name=self.ports_and_guis.my_logger.logger.name)
-            self.look_for_exceptions()
-            self.events.cont_to_tag_thread.set()
-            self.events.cont_to_printer_thread.set()
-            self.events.cont_to_main_thread.wait()
-            self.events.cont_to_main_thread.clear()
-            self.events.start_to_r2r_thread.set()
-
-    def pause_fn(self):
-        """
-        will be triggered by the Pause button and will pause the run if possible.
-        """
-        if not self.events.pause_to_tag_thread.isSet() and not self.waiting_for_user_to_press_stop_because_printer \
-                and not self.tag_checker_thread.fetal_error:
-            msg = "Run paused, the R2R will pause now (the current spot will be fail)"
-            printing_func(msg, 'MainWindow', lock_print, logger_type='warning',
-                          logger_name=self.ports_and_guis.my_logger.logger.name)
-            self.events.stop_to_r2r_thread.set()
-            self.events.pause_to_tag_thread.set()
-            self.events.start_compare.clear()
-
     def recurring_timer(self):
         """
         update the runs main GUI, checks that the other threads are OK (no exceptions)
         """
         global tested, passed, missing_labels, black_list_size
         global last_pass_string, reel_name
 
@@ -2611,17 +2665,15 @@
                     self.yield_drop_happened = True
                     self.yield_was_high_lately = False
                     if not self.ignore_stop_conditions:
                         self.events.done_to_tag_thread.set()
                         self.events.done_to_r2r_thread.set()
                     else:
                         pass
-                    if not self.events.pause_to_tag_thread.isSet():
-                        self.events.stop_to_r2r_thread.set()
-                        self.events.pause_to_tag_thread.set()
+                    self.events.stop_to_r2r_thread.set()
                 elif self.y[-1] < int(self.minyield) and len(
                         self.y) > 15:  # under 40% yield-over-time for 200 tags => Pause the run
                     self.yield_drop_happened = True
                     for ii in range(1, 15):
                         if self.y[-ii] < int(self.minyield):
                             continue
                         else:
@@ -2673,29 +2725,25 @@
     def look_for_exceptions(self):
         """
         search for exceptions in the threads Exceptions Queues.
         """
         if self.to_print:
             if not self.printer.exception_queue.empty() or not self.tag_checker_thread.exception_queue.empty() or \
                     not self.r2r_thread.exception_queue.empty():
-                if not self.events.pause_to_tag_thread.isSet():
-                    msg = "Paused because an exception happened, the R2R will pause now " \
-                          "(the current spot will be fail)"
-                    printing_func(msg, 'MainWindow', lock_print, logger_type='debug',
-                                  logger_name=self.ports_and_guis.my_logger.logger.name)
-                    self.events.stop_to_r2r_thread.set()
-                    self.events.pause_to_tag_thread.set()
-                self.handle_r2r_exception()
-        elif not self.tag_checker_thread.exception_queue.empty() or not self.r2r_thread.exception_queue.empty():
-            if not self.events.pause_to_tag_thread.isSet():
-                msg = "Stopped because an exception happened, the R2R will pause now (the current spot will be fail)"
+                msg = "Paused because an exception happened, the R2R will pause now " \
+                      "(the current spot will be fail)"
                 printing_func(msg, 'MainWindow', lock_print, logger_type='debug',
                               logger_name=self.ports_and_guis.my_logger.logger.name)
                 self.events.stop_to_r2r_thread.set()
-                self.events.pause_to_tag_thread.set()
+                self.handle_r2r_exception()
+        elif not self.tag_checker_thread.exception_queue.empty() or not self.r2r_thread.exception_queue.empty():
+            msg = "Stopped because an exception happened, the R2R will pause now (the current spot will be fail)"
+            printing_func(msg, 'MainWindow', lock_print, logger_type='debug',
+                          logger_name=self.ports_and_guis.my_logger.logger.name)
+            self.events.stop_to_r2r_thread.set()
             self.handle_r2r_exception()
 
     def handle_r2r_exception(self):
         """
         handle the exception if possible. prints the exception to screen and log
         """
         if self.to_print:
@@ -2756,54 +2804,55 @@
     def check_logging_due_to_printing_offset(self):
         # check logging due to printing offset:
         if self.ports_and_guis.Tag_Value['printOffset'] != 0:
             if self.tag_checker_thread.missing_labels_in_a_row < self.ports_and_guis.Tag_Value['printOffset']:
                 packet_dict = csv_to_dict(path=self.ports_and_guis.my_logger.packets_data_path)
                 n_not_printed = self.ports_and_guis.Tag_Value[
                                     'printOffset'] - self.tag_checker_thread.missing_labels_in_a_row
-                last_tested_location = packet_dict['tag_run_location'][-1]
-                location_to_delete = []
-                for i in range(n_not_printed):
-                    try:
-                        location_to_delete.append(str(int(last_tested_location) + i))
-                    except Exception as e:
-                        self.ports_and_guis.my_logger.logger.warning(
-                            'invalid last_tested_location {} could not clean all external id that were not printed due '
-                            'to printing offset ({})'.format(last_tested_location, e))
-                failed_due_to_no_print = []
-                for i in range(len(packet_dict['tag_run_location'])):
-                    if packet_dict['tag_run_location'][i] in location_to_delete:
-                        packet_dict['external_id'][i] = ''
-                        packet_dict['status_offline'][i] = '0'
-                        if packet_dict['fail_bin_str'][i] == str(FailureCodes.PASS.name):
-                            packet_dict['fail_bin'][i] = str(FailureCodes.NOT_PRINTED.value)
-                            packet_dict['fail_bin_str'][i] = str(FailureCodes.NOT_PRINTED.name)
-                            failed_due_to_no_print.append(packet_dict['tag_run_location'][i])
-
-                packet_dict_list = []
-                for i in range(len(packet_dict['common_run_name'])):
-                    packet_dict_list.append({k: v[i] for k, v in packet_dict.items()})
-                with open(self.ports_and_guis.my_logger.packets_data_path, 'w', newline='') as f:
-                    csv_writer = csv.DictWriter(f, packet_dict.keys())
-                    csv_writer.writeheader()
-                    csv_writer.writerows(packet_dict_list)
-                    f.close()
-
-                # update run data:
-                run_dict = csv_to_dict(path=self.ports_and_guis.my_logger.run_data_path)
-                run_dict['total_run_passed_offline'][0] = \
-                    str(int(run_dict['total_run_passed_offline'][0]) - len(list(set(failed_due_to_no_print))))
-                run_dict['run_offline_yield'][0] = \
-                    str((int(run_dict['total_run_passed_offline'][0]) / int(run_dict['total_run_tested'][0])) * 100)
-                run_dict_list = [{k: v[0] for k, v in run_dict.items()}]
-                with open(self.ports_and_guis.my_logger.run_data_path, 'w', newline='') as f:
-                    csv_writer = csv.DictWriter(f, run_dict.keys())
-                    csv_writer.writeheader()
-                    csv_writer.writerows(run_dict_list)
-                    f.close()
+                if len(packet_dict['tag_run_location']):
+                    last_tested_location = packet_dict['tag_run_location'][-1]
+                    location_to_delete = []
+                    for i in range(n_not_printed):
+                        try:
+                            location_to_delete.append(str(int(last_tested_location) + i))
+                        except Exception as e:
+                            self.ports_and_guis.my_logger.logger.warning(
+                                'invalid last_tested_location {} could not clean all external id that were not printed due '
+                                'to printing offset ({})'.format(last_tested_location, e))
+                    failed_due_to_no_print = []
+                    for i in range(len(packet_dict['tag_run_location'])):
+                        if packet_dict['tag_run_location'][i] in location_to_delete:
+                            packet_dict['external_id'][i] = ''
+                            packet_dict['status_offline'][i] = '0'
+                            if packet_dict['fail_bin_str'][i] == str(FailureCodes.PASS.name):
+                                packet_dict['fail_bin'][i] = str(FailureCodes.NOT_PRINTED.value)
+                                packet_dict['fail_bin_str'][i] = str(FailureCodes.NOT_PRINTED.name)
+                                failed_due_to_no_print.append(packet_dict['tag_run_location'][i])
+
+                    packet_dict_list = []
+                    for i in range(len(packet_dict['common_run_name'])):
+                        packet_dict_list.append({k: v[i] for k, v in packet_dict.items()})
+                    with open(self.ports_and_guis.my_logger.packets_data_path, 'w', newline='') as f:
+                        csv_writer = csv.DictWriter(f, packet_dict.keys())
+                        csv_writer.writeheader()
+                        csv_writer.writerows(packet_dict_list)
+                        f.close()
+
+                    # update run data:
+                    run_dict = csv_to_dict(path=self.ports_and_guis.my_logger.run_data_path)
+                    run_dict['total_run_passed_offline'][0] = \
+                        str(int(run_dict['total_run_passed_offline'][0]) - len(list(set(failed_due_to_no_print))))
+                    run_dict['run_offline_yield'][0] = \
+                        str((int(run_dict['total_run_passed_offline'][0]) / int(run_dict['total_run_tested'][0])) * 100)
+                    run_dict_list = [{k: v[0] for k, v in run_dict.items()}]
+                    with open(self.ports_and_guis.my_logger.run_data_path, 'w', newline='') as f:
+                        csv_writer = csv.DictWriter(f, run_dict.keys())
+                        csv_writer.writeheader()
+                        csv_writer.writerows(run_dict_list)
+                        f.close()
 
 
 
 
 def set_attn_power_offline(attn_obj, attn_power, simulation=False):
     """
     configure Attenuator to a specific value
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/offline_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,24 +55,26 @@
    (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
    CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
    (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
    (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 """
 import http.client
 import serial.tools.list_ports
-from wiliot_api.manufacturing.manufacturing import ManufacturingClient
-from wiliot_core import WiliotDir, check_user_config_is_ok
+import PySimpleGUI as SimGUI
+from wiliot_api import ManufacturingClient
+from wiliot_core import check_user_config_is_ok, InlayTypes
 from wiliot_testers.utils.get_version import get_version
 from wiliot_testers.calibration_test.calibration_test_by_tbp import *
 from wiliot_testers.tester_utils import open_json, open_json_cache
 from wiliot_testers.wiliot_tester_tag_result import *
 from PIL import Image
 import re
 import pathlib
 import ast
+import time
 
 
 class ConfigDefaults(object):
     """
     contains the default values for the configuration json
     """
 
@@ -98,29 +100,39 @@
     def __init__(self, gui_type):
         if gui_type == 'Main':
             self.default_gui_values = {'missingLabel': 'No',
                                        'maxMissingLabels': '6',
                                        'toPrint': 'No', 'printOffset': '1', 'printingFormat': 'SGTIN',
                                        'batchName': 'test_reel',
                                        'tagGen': 'N/A',
-                                       'inlayType': 'Dual Band', 'inlay': InlayTypes.TEO_086.value,
+                                       'inlayType': 'Ble_Test_Only', 'inlay': InlayTypes.TEO_086.value,
                                        'desiredTags': '9999999', 'desiredPass': '9999999',
                                        'surface': SurfaceTypes.AIR.value,
                                        'conversion': ConversionTypes.STANDARD.value, 'blackListAfter': '2',
                                        'Environment': 'production', 'OwnerId': 'wiliot-ops', 'operator': '',
                                        'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2', 'maxQRWrongTags': '2',
                                        'comments': '', 'maxFailStop': '50', 'maxYieldStop': '40'}
         elif gui_type == 'Test':
-            self.default_gui_values = {'passJobName': 'SGTIN_QR', 'sgtin': 'test_test_test_test_X_',
+            self.default_gui_values = {'passJobName': 'SGTIN_QR', 'passJobNum': 2, 'sgtin': 'test_test_test_test_X_',
                                        'stringBeforeCounter': 'test',
-                                       'reelNumManually': 'test', 'firstPrintingValue': '0', 'tagLocation': '0'}
+                                       'reelNumManually': 'test', 'firstPrintingValue': '0', 'tagLocation': '0',
+                                       'tag_reel_location': '0',
+                                       'enableLineSelection': 'No'}
         elif gui_type == 'SGTIN':
-            self.default_gui_values = {'passJobName': 'SGTIN_QR', 'sgtin': '(01)00850027865010(21)',
+            self.default_gui_values = {'passJobName': 'SGTIN_QR', 'passJobNum': 2, 'sgtin': '(01)00850027865010(21)',
                                        'stringBeforeCounter': '',
-                                       'reelNumManually': '', 'firstPrintingValue': '0', 'tagLocation': '0'}
+                                       'reelNumManually': '', 'firstPrintingValue': '0', 'tagLocation': '0',
+                                       'tag_reel_location': '0',
+                                       'enableLineSelection': 'No'}
+        elif gui_type == 'Barcode':
+            self.default_gui_values = {'passJobName': 'BARCODE_8', 'passJobNum': 3, 'sgtin': '',
+                                       'stringBeforeCounter': '',
+                                       'reelNumManually': '', 'firstPrintingValue': '0', 'tagLocation': '0',
+                                       'tag_reel_location': '0',
+                                       'enableLineSelection': 'No'}
         else:
             self.default_gui_values = {}
 
 
 def simple_calibration_gui():
     """
     open pop up window
@@ -296,20 +308,19 @@
                  SimGUI.Spin(values=['Auto',1,2,3,4,5,6,7,8,10,11,12,13,14,15,16,17,18], initial_value=('Auto'),
                              size=(6, 1), key='attnComport')],
                 [SimGUI.Text('Attenuation value:', size=(40, 1)),
                  SimGUI.Spin(values=[i for i in range(5, 20)], key='attnval',
                              initial_value=5,
                              size=(6, 1))]]
 
-
     print_tab = [[SimGUI.Text('To print?', size=(40, 1)),
                   SimGUI.InputCombo(('Yes', 'No'), default_value=gui_inputs_values['toPrint'], key='toPrint')],
                  [SimGUI.Text('What is the printing job format?', size=(40, 1)),
-                  SimGUI.InputCombo(('Test', 'SGTIN'), default_value='SGTIN',
-                                    key='printingFormat')],
+                  SimGUI.InputCombo(('Test', 'SGTIN', 'Barcode'), default_value=gui_inputs_values['printingFormat']
+                  if gui_inputs_values['printingFormat'] != 'Test' else 'SGTIN', key='printingFormat')],
                  [SimGUI.Text('printing offset', size=(40, 1)),
                   SimGUI.Spin(values=[i for i in range(0, 5)], initial_value=int(gui_inputs_values['printOffset']),
                               size=(6, 1), key='printOffset')],
                  [SimGUI.Text('QR Validation:', size=(40, 1)),
                   SimGUI.InputCombo(('Yes', 'No'), visible=True, default_value=gui_inputs_values["QRRead"],
                                     key='QRRead')],
                  [SimGUI.Text('Max QR wrong readouts in row:', size=(40, 1)),
@@ -471,15 +482,15 @@
     :param digits_in_counter: amount of digits in the tag counter field (usually 4)
     :type first_counter: string
     :param first_counter: counter of the run first tag
     :type printing_format: string
     :param printing_format: this run printing format (SGTIN, string)
     """
     first_print = str(string_before_the_counter)
-    if 'SGTIN' in printing_format or 'Test' in printing_format:
+    if 'SGTIN' in printing_format or 'Test' in printing_format or 'Barcode' in printing_format:
         first_print += 'T'
     if digits_in_counter < len(first_counter):
         is_ok = False
     else:
         dif_len = (digits_in_counter - len(first_counter))
         for i in range(digits_in_counter):
             # add zeros to where the counter is not needed
@@ -489,15 +500,15 @@
                 # add the first counter number by order to the string
                 first_print += str(first_counter)
                 break
         is_ok = True
     return first_print, is_ok
 
 
-def printing_test_window(env=''):
+def printing_test_window():
     """
     opens the GUI for user input for test print
     :return: dictionary of user inputs
     """
     printing_format = 'Test'
     folder_name = 'configs'
     file_name = 'gui_printer_inputs_4_Test_do_not_delete.json'
@@ -507,19 +518,22 @@
     # If the JSON file is empty, get those values from the default
     if gui_inputs_values['reelNumManually'] == "":
         reel_num = 'test_test_test_test_X_test'
         gui_inputs_values['sgtin'] = reel_num[:22]
         gui_inputs_values['reelNumManually'] = reel_num[22:]
         gui_inputs_values['firstPrintingValue'] = '0'
         gui_inputs_values['tagLocation'] = '0'
+        gui_inputs_values['tag_reel_location'] = '0'
 
     # Define the window's contents
     layout = [[SimGUI.Text('Job to print for pass and fail:'),
-               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'devkit_TEO', 'devkit_TIKI', 'empty'),
-                                 default_value="SGTIN_QR", key='passJobName')],
+               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'BARCODE_8', 'devkit_TEO', 'devkit_TIKI', 'empty'),
+                                 default_value=gui_inputs_values['passJobName'], key='passJobName')],
+              [SimGUI.Text('pass line number:'),
+               SimGUI.Input(gui_inputs_values['passJobNum'], key='passJobNum')],
               [SimGUI.Text("What is the first counter number?")],
               [SimGUI.Input(gui_inputs_values['firstPrintingValue'], key='firstPrintingValue')],
               [SimGUI.Checkbox('Insert reel number manually?', default=False, key='isManually')],
               [SimGUI.Text("For manual mode only - what is the sgtin number?", key='sgtinNumManuallyText'),
                SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually')],
               [SimGUI.Text("For manual mode only - what is the reel number?", key='reelNumManuallyText'),
                SimGUI.Input(gui_inputs_values['reelNumManually'], key='reelNumManually')],
@@ -566,26 +580,31 @@
                 elif values['isManually']:
                     if len(str(values['firstPrintingValue'])) > tag_digits_num:
                         window['-OUTPUT-'].update(
                             'First counter number is too big for counter digits number!!\n'
                             'Please enter a new first counter number')
                         should_submit = False
 
-                    elif not len(str(values['sgtinNumManually'])) == 22:
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['sgtinNumManually'])) == 22:
                         window['-OUTPUT-'].update(
                             'SGTIN number is not equal to 22 chars!!\n'
                             'Please enter correct SGTIN, length: ' + str(len(str(values['sgtinNumManually']))))
                         should_submit = False
 
-                    elif not len(str(values['reelNumManually'])) == 4:
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['reelNumManually'])) == 4:
                         window['-OUTPUT-'].update(
                             'Reel number is not equal to 4 chars!!\n'
                             'Please enter correct Reel number')
                         should_submit = False
 
+                    elif 'Barcode' in values['passJobName'] and len(values['reelNumManually']) != 3:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 3 chars!!\n'
+                            'Please enter correct Reel number')
+
                     else:
                         pass_job_name = values['passJobName']
                         reel_number = values['sgtinNumManually'] + values['reelNumManually']
                         first_counter = values['firstPrintingValue']
                         first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
                                                                first_counter, printing_format)
                         # Output a message to the window
@@ -623,83 +642,103 @@
 
                 # manual input
                 elif values['isManually']:
                     if len(str(values['firstPrintingValue'])) > tag_digits_num:
                         window['-OUTPUT-'].update('First counter number is too big for counter digits number!!\n'
                                                   'Please enter a new first counter number')
 
-                    elif not len(str(values['sgtinNumManually'])) == 22:
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['sgtinNumManually'])) == 22:
                         window['-OUTPUT-'].update(
                             'SGTIN number is not equal to 22 chars!!\n'
                             'Please enter correct SGTIN, its length is: ' + str(len(str(values['sgtinNumManually']))))
 
-                    elif not len(str(values['reelNumManually'])) == 4:
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['reelNumManually'])) == 4:
                         window['-OUTPUT-'].update(
                             'Reel number is not equal to 4 chars!!\n'
                             'Please enter correct Reel number')
 
+                    elif 'Barcode' in values['passJobName'] and len(values['reelNumManually']) != 3:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 3 chars!!\n'
+                            'Please enter correct Reel number')
+
                     else:
                         pass_job_name = values['passJobName']
                         reel_number = values['sgtinNumManually'] + values['reelNumManually']
                         first_counter = values['firstPrintingValue']
                         first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
                                                                first_counter, printing_format)
                         # Output a message to the window
                         window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
             except Exception:
                 window['-OUTPUT-'].update(
                     'First counter is not a number!!\nPlease enter a new first counter number')
 
     # Finish up by removing from the screen
     window.close()
-    v = {'passJobName': pass_job_name, 'stringBeforeCounter': values['sgtinNumManually']+values['reelNumManually'], 'digitsInCounter': tag_digits_num,
-         'firstPrintingValue': values['firstPrintingValue'], 'failJobName': pass_job_name, 'tagLocation': values['firstPrintingValue']}
-
-    data_to_save = {'passJobName': pass_job_name, 'sgtin': values['sgtinNumManually'], 'reelNumManually': values['reelNumManually'],
-                    'firstPrintingValue': values['firstPrintingValue'], 'tagLocation': values['firstPrintingValue']}
+    v = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+         'stringBeforeCounter': values['sgtinNumManually']+values['reelNumManually'],
+         'digitsInCounter': tag_digits_num, 'enableLineSelection': gui_inputs_values['enableLineSelection'],
+         'firstPrintingValue': values['firstPrintingValue'], 'failJobName': pass_job_name,
+         'tagLocation': values['firstPrintingValue'], 'tag_reel_location': gui_inputs_values['tag_reel_location']}
+
+    data_to_save = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+                    'sgtin': values['sgtinNumManually'], 'reelNumManually': values['reelNumManually'],
+                    'enableLineSelection': gui_inputs_values['enableLineSelection'],
+                    'firstPrintingValue': values['firstPrintingValue'], 'tagLocation': values['firstPrintingValue'],
+                    'tag_reel_location': gui_inputs_values['tag_reel_location']}
     f = open(os.path.join(folder_name, file_name), "w")
     json.dump(data_to_save, f)
     f.close()
     return v, is_ok
 
 
-def printing_sgtin_window(env='', owner_id='wiliot-ops'):
+def printing_sgtin_window(env='', owner_id='wiliot-ops', printing_format='SGTIN'):
     """
     opens the GUI for user input for SGTIN print
     :return: dictionary of user inputs
     """
     read_only = False
-    printing_format = 'SGTIN'
     folder_name = 'configs'
     file_name = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
     gui_inputs_values = open_json_cache(folder_path=folder_name, file_path=os.path.join(folder_name, file_name),
                                         default_values=DefaultGUIValues(printing_format).default_gui_values)
     new_run = SimGUI.popup_yes_no('    New Reel?    \n', keep_on_top=True, font=('normal', 20))
     if new_run == 'Yes':
+        gui_inputs_values['tagLocation'] = '0'
+        gui_inputs_values['tag_reel_location'] = '0'
         try:
             logging.info('Receiving data from the cloud, please wait')
-            reel_num = get_reel_name_from_cloud_api(env, owner_id)
+            reel_num = get_reel_name_from_cloud_api(env, owner_id, printing_format)
         except Exception:
             logging.warning('Problem with receiving data from cloud')
             raise Exception
         gui_inputs_values['firstPrintingValue'] = '0000'
-        gui_inputs_values['tagLocation'] = '0'
         if 'data' in reel_num:
             reel_number = reel_num['data']
-            gui_inputs_values['sgtin'] = reel_number[:22]
-            gui_inputs_values['reelNumManually'] = reel_number[22:26]
+            if printing_format == 'SGTIN':
+                gui_inputs_values['sgtin'] = reel_number[:22]
+                gui_inputs_values['reelNumManually'] = reel_number[22:26]
+            elif printing_format == 'Barcode':
+                gui_inputs_values['sgtin'] = ''
+                gui_inputs_values['reelNumManually'] = reel_number
+            else:
+                raise Exception(f'printing_format is not supported: {printing_format}')
             read_only = True
         else:
             gui_inputs_values['sgtin'] = ''
             gui_inputs_values['reelNumManually'] = ''
             read_only = False
 
     layout = [[SimGUI.Text('Job to print for pass:'),
-               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'devkit_TEO', 'devkit_TIKI', 'empty'),
-                                 default_value="SGTIN_QR", key='passJobName')],
+               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'BARCODE_8', 'devkit_TEO', 'devkit_TIKI', 'empty'),
+                                 default_value='BARCODE_8' if printing_format == 'Barcode' else 'SGTIN_QR',
+                                 key='passJobName')],
+              [SimGUI.Text('fail line number: 1, pass line number:'),
+               SimGUI.Input(gui_inputs_values['passJobNum'], key='passJobNum')],
               [SimGUI.Text("First counter number")],
               [SimGUI.Input(0000 if read_only else gui_inputs_values['firstPrintingValue'], key='firstPrintingValue',
                             readonly=read_only)],
               [SimGUI.Checkbox('Insert reel number manually?', default=not read_only, key='isNewReel',
                                disabled=read_only, visible=False)],
               [SimGUI.Text("SGTIN number", key='sgtinNumManuallyText'),
                SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually', readonly=read_only)],
@@ -753,26 +792,32 @@
                             'First counter number is too big for counter digits number!!\n'
                             'Please enter a new first counter number you entered: ' + str(
                                 values['firstPrintingValue'] + ' in length of: ' + len(
                                     str(values['firstPrintingValue']))))
 
                         should_submit = False
 
-                    elif not len(values['sgtinNumManually']) == 22:
+                    elif printing_format == 'SGTIN' and not len(values['sgtinNumManually']) == 22:
                         window['-OUTPUT-'].update(
                             'SGTIN number is not equal to 22 chars!!\n'
                             'Please enter correct SGTIN, its length is: ' + str(len(str(values['sgtinNumManually']))))
                         should_submit = False
 
-                    elif not len(values['reelNumManually']) == 4:
+                    elif printing_format == 'SGTIN' and len(values['reelNumManually']) != 4:
                         window['-OUTPUT-'].update(
                             'Reel number is not equal to 4 chars!!\n'
                             'Please enter correct Reel number')
                         should_submit = False
 
+                    elif printing_format == 'Barcode' and len(values['reelNumManually']) != 3:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 3 chars!!\n'
+                            'Please enter correct Reel number')
+                        should_submit = False
+
                     else:
                         pass_job_name = values['passJobName']
                         reel_number = str(values['sgtinNumManually']) + str(values['reelNumManually'])
                         first_counter = values['firstPrintingValue']
                         first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
                                                                first_counter, printing_format)
                         # Output a message to the window
@@ -785,20 +830,27 @@
 
             if should_submit:
                 break
 
     # Finish up by removing from the screen
     window.close()
     if is_ok:
-        v = {'passJobName': pass_job_name, 'stringBeforeCounter': reel_number, 'digitsInCounter': tag_digits_num,
-             'firstPrintingValue': values['firstPrintingValue'], 'failJobName': 'line_',
-             'tagLocation': gui_inputs_values['tagLocation']}
-        data_to_save = {'passJobName': pass_job_name, 'sgtin': reel_number[:22], 'reelNumManually': reel_number[22:26],
+        v = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'], 'stringBeforeCounter': reel_number,
+             'digitsInCounter': tag_digits_num, 'firstPrintingValue': values['firstPrintingValue'],
+             'failJobName': 'line_', 'tagLocation': values['firstPrintingValue'],
+             'tag_reel_location': gui_inputs_values['tag_reel_location'],
+             'enableLineSelection': gui_inputs_values['enableLineSelection'],
+             'printingFormat': printing_format}
+        data_to_save = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+                        'sgtin': values['sgtinNumManually'], 'reelNumManually': values['reelNumManually'],
                         'firstPrintingValue': values['firstPrintingValue'], 'stringBeforeCounter': reel_number,
-                        'tagLocation': gui_inputs_values['tagLocation']}
+                        'tagLocation': values['firstPrintingValue'],
+                        'printingFormat': printing_format,
+                        'enableLineSelection': gui_inputs_values['enableLineSelection'],
+                        'tag_reel_location': gui_inputs_values['tag_reel_location']}
 
         f = open(os.path.join(folder_name, file_name), "w")
         json.dump(data_to_save, f)
         f.close()
         return v, is_ok
     else:
         return gui_inputs_values, is_ok
@@ -969,39 +1021,40 @@
         if event == SimGUI.WINDOW_CLOSED or event == 'Done':
             break
 
     window.close()
     return
 
 
-def get_reel_name_from_cloud_api(env, owner_id):
+def get_reel_name_from_cloud_api(env, owner_id, printing_format='SGTIN'):
     """
     api to receive reel number from cloud (should use it to avoid duplications)
     :return: the reel number (in 0x)
     """
     assert ('R2R_station_name' in os.environ), 'R2R_station_name is missing from PC environment variables'
     tester_station_name = os.environ['R2R_station_name']
     try:
 
-        file_path, api_key, is_successful = check_user_config_is_ok(env=env)
+        file_path, api_key, is_successful = check_user_config_is_ok(env=env, owner_id=owner_id)
         client = ManufacturingClient(api_key=api_key, logger_=logging.getLogger().name, env=env)
         token = client.auth_obj.get_token()
     except Exception as e:
         raise Exception('Failed to get token. Check previous errors.\n{}'.format(str(e)))
 
     try:
         conn = http.client.HTTPSConnection("api.wiliot.com")
         headers = {
             'accept': "*/*",
             'authorization': "Bearer " + token + "",
             'content-type': "application/json"
         }
         body = json.dumps({"printerId": tester_station_name})
         payload = body
-        conn.request("POST", env + "/v1/owner/" + owner_id + "/tag/roll/print", payload, headers)
+        reel_id_type = '?reelIdType=threeCharacters' if printing_format == "Barcode" else ''
+        conn.request("POST", env + "/v1/owner/" + owner_id + "/tag/roll/print" + reel_id_type, payload, headers)
         res = conn.getresponse()
         data = res.read()
         # print("get_reel_name_from_cloud_API answer is:")
         # print(data.decode("utf-8"))
         return ast.literal_eval(data.decode("utf-8"))
 
     except Exception as e:
@@ -1018,37 +1071,41 @@
     """
 
     def __init__(self):
         """
         initialize params and port
         """
         self.baud_rate = 1000000
+        self.connected = False
         ports_list = [s.device for s in serial.tools.list_ports.comports()]
         if len(ports_list) == 0:
             ports_list = [s.name for s in serial.tools.list_ports.comports()]
             if len(ports_list) == 0:
                 print("no serial ports were found. please check your connections", "init")
                 return
 
         for port in ports_list:
             try:
                 self.comport = port
                 self.s = serial.Serial(self.comport, self.baud_rate, timeout=0, write_timeout=0)
                 response = self.query("*IDN?")
 
                 if ("Williot R2R GPIO" in response):
+                    self.connected = True
                     print('Found ' + response + " Serial Number " + self.query("SER?"))
                     self.s.flushInput()
                     break
                 else:
                     self.s.close()
             except (OSError, serial.SerialException):
                 pass
             except Exception as e:
                 print(e)
+        if not self.connected:
+            raise Exception('Could NOT connect to the Arduino, please check connections')
 
     def __del__(self):
         if self.s is not None:
             self.s.close()
 
     def write(self, cmd):
         """
@@ -1173,15 +1230,19 @@
         if reconnect_success:
             response = self.query("*IDN?")
             if ("Williot R2R GPIO" in response):
                 logging.info('Connection was restablished on COM{} with version {}'.format(response,self.query("SER?")))
                 self.s.flushInput()
             else:
                 self.s.close()
-                logging.warning(f"Failed to close connection to {self.comport} {e} - Please restart connection")
-
-
+                logging.warning(f"Failed to close connection to {self.comport} - Please restart connection")
 
 
 if __name__ == '__main__':
     open_session(['Single Band', 'Dual Band'])
+    printing_test_window()
+    printing_sgtin_window(env='test', printing_format='Barcode')
+    printing_sgtin_window(env='test', printing_format='SGTIN')
+
+    r = R2rGpio()
+    open_session(['Single Band', 'Dual Band'])
     pass
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/offline/tadbik_r2r_controller.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,18 @@
 from wiliot_core import WiliotGateway
 
 
 class tadbikR2rController():
     def __init__(self):
         self.my_gpio = R2rGpio()
         self.GwObj = WiliotGateway(auto_connect=True, logger_name='root')
-        self.GwObj.config_gw(energy_pattern_val=18, pl_delay_val=0, start_gw_app=False, with_ack=True)
-        self.GwObj.write('!store_to_flash')
         self.GwObj.reset_gw()
+        time.sleep(5)
+        self.GwObj.config_gw(energy_pattern_val=18, pl_delay_val=0, start_gw_app=False, with_ack=True)
+        self.GwObj.write('!pl_gw_config 1')  # to enable production line trigger
     
     def stop(self):
         self.my_gpio.gpio_state(3, "OFF")
     
     def start(self):
         self.my_gpio.gpio_state(3, "ON")
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/com_connect.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             self.builder.get_object(f'connect_atten').configure(text='Disconnect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'disabled'
             self.builder.get_object(f'attenComBle')['state'] = 'disabled'
         else:
             self.builder.get_object(f'connect_atten').configure(text='Connect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'normal'
             self.builder.get_object(f'attenComBle')['state'] = 'normal'
-    
+
     def choose_com_ports(self, default_dict):
         com_ports = [s.device for s in tools.list_ports.comports()]
         if len(com_ports) == 0:
             com_ports = [s.name for s in tools.list_ports.comports()]
         
         if 'gw' in default_dict.keys() and default_dict['gw'] in com_ports:
             self.gw_com_port = [default_dict['gw']]
@@ -819,15 +819,14 @@
                         except:
                             logger.error(f"{atten['type']} Attenuator error: try reconnect the attenuator.")
                             return False
         
         self.start_time = time()
         try:
             str_rsp.append(self.gateway.write('!listen_to_tag_only 1', with_ack=True))
-            str_rsp.append(self.gateway.write('!energizing_prob_set 100', with_ack=True))
             str_rsp.append(self.gateway.write('!set_tester_mode 1', with_ack=True))
             if 'EmulateSurfaceValue' in params.keys():
                 str_rsp.append(self.gateway.write('!set_sub_1_ghz_energizing_frequency {}'.format(
                     params['EmulateSurfaceValue']), with_ack=True))
             _, gw_ans = self.gateway.config_gw(effective_output_power_val=22, sub1g_output_power_val=29,
                                                energy_pattern_val=params['pattern'], received_channel=params['channel'],
                                                time_profile_val=[params['tOn'], params['tTotal']], start_gw_app=True,
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/configs_gui.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,64 +61,67 @@
 from os import makedirs
 import logging
 import pygubu
 from os.path import join, abspath, dirname, isfile, isdir
 from json import dump, load
 from copy import deepcopy
 from wiliot_core import WiliotDir
+from wiliot_testers.utils.get_version import get_version
 
+VER = get_version()
 MEASURED = {'button': 'Measured', 'label': '[meter]'}
 MANUAL = {'button': 'Manual', 'label': '[db]'}
-DEFAULT_CONFIGS = ['TEO', 'TIKI']
 DEFAULT_EMULATED_SURFACE = 'no simulation'
 logger = logging.getLogger('sample')
 
 wiliot_env = WiliotDir()
 sample_test_dir = join(wiliot_env.get_common_dir(), 'sample_test')
 OUTPUT_DIR = join(sample_test_dir, 'logs')
 CONFIGS_DIR = join(sample_test_dir, 'configs')
 if not isdir(join(OUTPUT_DIR)):
     makedirs(join(OUTPUT_DIR))
 if not isdir(join(CONFIGS_DIR)):
     makedirs(join(CONFIGS_DIR))
-copyfile(join(dirname(__file__), 'configs', '.default_configs.json'), join(CONFIGS_DIR, '.default_configs.json'))
-copyfile(join(dirname(__file__), 'configs', '.default_surfaces.json'), join(CONFIGS_DIR, '.default_surfaces.json'))
 
 
 class ConfigsGui(object):
     '''
     classdocs
     '''
     isGui = False
     atten_cur_mode = MANUAL
     test_config = ''
     config = ''
     configsDict = {}
     paramDict = {}
-    userConfigsDict = {}
     defaultConfigsDict = {}
     defaultSurfacesDict = {}
+    all_configs_fields = []
     
     def __init__(self, top_builder=None):
         '''
         Constructor
         '''
         self.top_builder = top_builder
-        if isfile(join(CONFIGS_DIR, '.user_configs.json')):
-            with open(join(CONFIGS_DIR, '.user_configs.json'), 'r') as jsonFile:
-                self.configsDict = self.userConfigsDict = load(jsonFile)
-            self.userConfigsDict = self.fix_antenna_type(self.userConfigsDict)
-        with open(join(CONFIGS_DIR, '.default_configs.json'), 'r') as jsonFile:
-            self.defaultConfigsDict = load(jsonFile)
-            self.defaultConfigsDict = self.fix_antenna_type(self.defaultConfigsDict)
-            def_dict = deepcopy(self.defaultConfigsDict)
-            self.configsDict.update(def_dict)
-        with open(join(CONFIGS_DIR, '.default_surfaces.json'), 'r') as jsonFile:
+        self.config_path = join(dirname(__file__), 'configs', '.default_test_configs.json')
+        if isfile(self.config_path):
+            with open(self.config_path, 'r') as jsonFile:
+                self.configsDict = load(jsonFile)
+                if len(self.configsDict):
+                    self.all_configs_fields = list(self.configsDict[next(iter(self.configsDict))].keys())
+            self.fix_antenna_type()
+
+        with open(join(dirname(__file__), 'configs', '.default_surfaces.json'), 'r') as jsonFile:
             self.defaultSurfacesDict = load(jsonFile)
-    
+
+        self.copy_config_file()
+
+    def copy_config_file(self):
+        copyfile(self.config_path, join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json'))
+
     def gui(self, ttk_frame=None):
         self.builder = builder = pygubu.Builder()
         ui_file = join(abspath(dirname(__file__)), 'utils', 'configs.ui')
         self.builder.add_from_file(ui_file)
         
         img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
@@ -141,125 +144,120 @@
         self.set_gui_defaults()
         
         self.isGui = True
         self.ttk.mainloop()
     
     def set_gui_defaults(self):
         temp_dict = deepcopy(self.configsDict)
-        # temp_dict.update(self.userConfigsDict)
         self.builder.get_object('configsList')['values'] = [key for key, item in temp_dict.items()
                                                             if isinstance(item, dict)]
         if temp_dict.get(self.config):
             self.builder.get_object('configsList').set(self.config)
             self.top_builder.tkvariables.get('testTime').set(temp_dict[self.config]['testTime'])
             self.builder.get_object('EmulateSurface')['values'] = tuple(
                 self.defaultSurfacesDict['EmulateSurface'].keys())
             self.builder.get_object('EmulateSurface').set(DEFAULT_EMULATED_SURFACE)
             self.builder.get_object('antennaType')['values'] = ['TEO', 'TIKI']
             for param, value in temp_dict[self.config].items():
                 if self.builder.tkvariables.get(param) is not None:
                     self.builder.tkvariables.get(param).set(value)
                 else:
                     pass
-        
-        if self.config in DEFAULT_CONFIGS:
-            self.builder.get_object('save')['state'] = 'disabled'
-        else:
-            self.builder.get_object('save')['state'] = 'normal'
+        self.builder.get_object('save')['state'] = 'normal'
     
-    def fix_antenna_type(self, orig_dict):
-        tempDict = deepcopy(orig_dict)
+    def fix_antenna_type(self):
+        tempDict = deepcopy(self.configsDict)
         for config, params in tempDict.items():
             if 'antennaType' in params.keys() and params['antennaType']:
                 fixedAntenna = 'TIKI' if params['antennaType'].lower() in ['dual', 'tiki'] else 'TEO'
-                orig_dict[config]['antennaType'] = fixedAntenna
-        return orig_dict
+                self.configsDict[config]['antennaType'] = fixedAntenna
     
     def atten_mode(self):
         self.atten_cur_mode = MEASURED if self.atten_cur_mode == MANUAL else MANUAL
         self.builder.tkvariables.get('atten_mode').set(self.atten_cur_mode['button'])
         ble_label = self.builder.tkvariables.get('attenBleLabel')
         ble_label.set(ble_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
         lora_label = self.builder.tkvariables.get('attenLoRaLabel')
         lora_label.set(lora_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
     
     def close(self):
         self.isGui = False
-        for param in self.configsDict[DEFAULT_CONFIGS[0]].keys():
+        for param in self.all_configs_fields:
             if self.builder.tkvariables.get(param) is not None:
                 value = self.builder.tkvariables.get(param).get()
                 self.paramDict[param] = value
                 self.configsDict[self.config][param] = value
                 if param == 'EmulateSurface':
                     self.paramDict['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][value]
-                    self.configsDict[self.config]['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][
-                        value]
         self.ttk.destroy()
     
     def is_gui_opened(self):
         return self.isGui
     
     def get_params(self):
         return self.paramDict
     
     def get_configs(self):
         temp_dict = deepcopy(self.configsDict)
-        temp_dict.update(self.userConfigsDict)
         return temp_dict
     
     def set_params(self, test_config):
-        self.paramDict = self.configsDict[test_config]
+        if test_config not in self.configsDict.keys():
+            config_options = list(self.configsDict.keys())
+            test_config = config_options[0]
+        self.paramDict = self.configsDict[test_config].copy()
+        if 'EmulateSurface' in self.configsDict[test_config].keys():
+            surface = self.configsDict[test_config]['EmulateSurface']
+            self.paramDict['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][surface]
         self.top_builder.tkvariables.get('testTime').set(self.paramDict['testTime'])
     
     def set_default_config(self, test_config):
         self.test_config = test_config
         self.config = test_config
     
     def config_select(self, *args):
         self.config = config = self.builder.get_object('configsList').get()
-        if config in DEFAULT_CONFIGS:
-            self.builder.get_object('save')['state'] = 'disabled'
-        else:
-            self.builder.get_object('save')['state'] = 'normal'
+        self.builder.get_object('save')['state'] = 'normal'
         self.top_builder.get_object('test_config').set(config)
         self.reset()
     
     def config_set(self, config):
         self.config = config
         self.set_params(config)
         if self.isGui:
             self.builder.get_object('configsList').set(config)
             self.set_gui_defaults()
         # except BaseException:
         #     pass
     
     def save(self):
         self.config = config = self.builder.get_object('configsList').get()
-        if config not in DEFAULT_CONFIGS:
-            self.userConfigsDict[config] = {}
-            for param in self.configsDict[DEFAULT_CONFIGS[0]].keys():
-                value = self.builder.tkvariables.get(param)
-                if value is not None:
-                    self.userConfigsDict[config][param] = value.get()
-            if config not in self.configsDict.keys():
-                self.configsDict[config] = {}
-            self.configsDict[config].update(self.userConfigsDict[config])
+
+        if config not in self.configsDict.keys():
+            self.configsDict[config] = {}
+
+        for param in self.all_configs_fields:
+            value = self.builder.tkvariables.get(param)
+            if value is not None:
+                self.configsDict[config][param] = value.get()
+            else:
+                self.configsDict[config][param] = ''
         self.builder.get_object('configsList')['values'] = [key for key, item in self.configsDict.items()
                                                             if isinstance(item, dict)]
         self.top_builder.get_object('test_config')['values'] = [key for key, item in self.configsDict.items()
                                                                 if isinstance(item, dict)]
         self.top_builder.get_object('test_config').set(config)
         
-        with open(join(CONFIGS_DIR, '.user_configs.json'), 'w+') as jsonFile:
-            dump(self.userConfigsDict, jsonFile, indent=4)
+        with open(self.config_path, 'w+') as jsonFile:
+            dump(self.configsDict, jsonFile, indent=4)
+        self.copy_config_file()
         
         logger.info(f'{config} configuration saved successfully.')
     
     def reset(self):
-        self.configsDict = deepcopy(self.userConfigsDict)
         def_dict = deepcopy(self.defaultConfigsDict)
         self.configsDict.update(def_dict)
         self.set_gui_defaults()
     
     def test_time_update(self, *args):
         self.top_builder.tkvariables.get('testTime').set(self.builder.tkvariables.get('testTime').get())
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/get_temperature_sensor_name.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/sample_test.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,29 +66,29 @@
 from tkinter import messagebox
 import pygubu
 from threading import Thread, Lock
 from time import sleep
 import time
 import csv
 import datetime
-from wiliot_testers.sample.configs_gui import ConfigsGui, DEFAULT_CONFIGS, OUTPUT_DIR, CONFIGS_DIR
+from wiliot_testers.sample.configs_gui import ConfigsGui, OUTPUT_DIR, CONFIGS_DIR
 from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND, \
     popup_message
 from traceback import print_exc
 from json import load, dump
 import argparse
 import sys
 from os.path import isfile, abspath, dirname, join, isdir, exists
 from wiliot_testers.utils.get_version import get_version
 # sys.path.append(abspath(dirname(join('..', '..', '..', '..', 'pywiliot_internal'))))
 from wiliot_testers.tester_utils \
     import setLogger, changeFileHandler, removeFileHandler, CsvLog, HeaderType, TesterName, StreamToLogger
 from wiliot_core import TagCollection, PacketList
-from wiliot_core import check_user_config_is_ok
-from wiliot_api.manufacturing.manufacturing import ManufacturingClient
+from wiliot_core import check_user_config_is_ok, InlayTypes
+from wiliot_api import ManufacturingClient
 from wiliot_testers.tester_utils import upload_to_cloud_api
 
 LOG_LEVEL = 'INFO'
 
 # default_log_file = join(abspath(dirname(__file__)), 'SampleTest.log')
 default_log_file = join(OUTPUT_DIR, 'SampleTest.log')
 logger = setLogger('sample', LOG_LEVEL, outputFile=default_log_file, file_mode='a+')
@@ -108,14 +108,15 @@
 TIME = 'time'
 
 DEF_NUM_OF_TAGS = 2
 
 CLOUD_TIMEOUT_POST = 10
 CLOUD_TIMEOUT_RESOLVE = 2
 
+SGTIN_PREFIX_DEFAULT = '(01)00850027865010(21)'
 
 class SampleException(Exception):
     pass
 
 
 class SampleTest(object):
     goButtonState = CONNECT_HW
@@ -132,15 +133,14 @@
     gatewayDataThread = None
     timerThread = None
     testFinished = True
     post_data = True
     wiliotTags = False
     forceCloseRequested = False
     closeRequested = False
-    debug_mode = False
     testGo = False
     stopTimer = False
     closeListener = False
     testConfig = ''
     reel_id = ''
     gtin = ''
     testDir = ''
@@ -148,14 +148,15 @@
     station_name = ''
     pywiliot_version = ''
     testTime = 0
     # tagsCount = 0
     testStartTime = 0
     sleep = 0
     cur_atten = 0
+    test_num = 0
     defaultDict = {}
     dataBaseDict = {}
     runDataDict = {}
     params = {}
     test_barcodes = {}
     barcodes_read = {}
     tagsFinished = {}
@@ -165,19 +166,20 @@
     total_bad_advas = []
     add_to_dict_threads = []
     unknown_packets = PacketList()
     antenna = ''
     low = 0
     high = 0
     step = 1
+    n_repetitions = 1
     
     # numOfTags = ''
     multiTag = TagCollection()
     
-    def __init__(self, debug_mode=False, calib=None, environment='', post_data=True, offline=False):
+    def __init__(self, calib=None, environment='', post_data=True, offline=False):
         
         self.calib = calib
         self.offline = offline
         self.offline_tag_index = 0
         self.environment = environment
         self.post_data = post_data
         if self.offline:
@@ -189,15 +191,14 @@
         if isfile(join(CONFIGS_DIR, '.defaults.json')):
             with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
                 self.defaultDict = load(defaultComs)
 
         self.popup_login()
         
         self.builder = builder = pygubu.Builder()
-        self.debug_mode = debug_mode
         
         self.comConnect = ComConnect(top_builder=builder, new_tag_func=self.add_tag_to_test,
                                      update_go=self.update_go_state, default_dict=self.defaultDict)
         self.update_data()
         if not self.offline:
             _, api_key, is_success = check_user_config_is_ok(env='prod', owner_id=self.owner)
             if not is_success:
@@ -219,15 +220,16 @@
         self.builder.add_resource_path(img_path)
         img_path = join(abspath(dirname(__file__)), 'utils')
         self.builder.add_resource_path(img_path)
         
         missing_com_port = self.comConnect.choose_com_ports(self.defaultDict)
         
         if missing_com_port:
-            popup_message('Default com ports not available, check connections.', title='Warning', log='warning')
+            popup_message('All or some of the default com ports are not available, '
+                          'please check connections.', title='Warning', log='warning')
         
         self.ttk = Tk()
 
         self.ttk.title("Wiliot Sample Test")
         self.mainWindow = self.builder.get_object('mainwindow', self.ttk)
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.builder.connect_callbacks(self)
@@ -248,29 +250,14 @@
             value = self.builder.get_object(var).get()
             if var not in self.defaultDict.keys():
                 self.defaultDict[var] = []
             if value in self.defaultDict[var]:
                 self.defaultDict[var].pop(self.defaultDict[var].index(value))
             self.defaultDict[var].insert(0, value)
 
-    def on_edit_hw_tester(self):
-        self.builder.get_object('tester_hw_desc')['state'] = 'enabled'
-        self.builder.get_object('tester_hw_ver')['state'] = 'enabled'
-
-    def on_save_tester_hw(self):
-        self.builder.get_object('tester_hw_desc')['state'] = 'disabled'
-        self.builder.get_object('tester_hw_ver')['state'] = 'disabled'
-        tester_hw_ver = self.builder.get_object('tester_hw_ver').get()
-        tester_hw_desc = self.builder.get_object('tester_hw_desc').get()
-        # save
-        self.defaultDict['tester_hw'] = {'version': tester_hw_ver,
-                                         'description': tester_hw_desc}
-        self.runDataDict['hwVersion'] = self.dataBaseDict['hwVersion'] = tester_hw_ver
-        self.update_data()
-
     def go(self):
         if self.finishThread is not None and self.finishThread.is_alive():
             self.finishThread.join()
         self.goButtonState = goButtonState = self.builder.tkvariables.get('go').get()
         self.builder.get_object('stop')['state'] = 'disabled'
         self.update_params_state(state='disabled', group=GO)
         self.builder.get_variable('forceGo').set('0')
@@ -365,15 +352,15 @@
             # self.test_barcodes[cur_id] = scanner_index
             self.builder.get_object('scanned').insert(END, f'{cur_id}, {scanner_index}')
             mutex.release()
         else:
             mutex.release()
             popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning', log='warning')
             return False
-        
+
         if self.reel_id != '' and self.reel_id != reel_id and self.wiliotTags:
             popup_message('Tag reel different from test reel.', title='Warning', log='error')
         
         return True
     
     def update_go_state(self, force_go=False):
         if (self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go) and \
@@ -419,35 +406,41 @@
         self.builder.get_object('forceGo')['state'] = 'normal'
         self.builder.get_object('stop')['state'] = 'normal'
         self.builder.get_object('go')['state'] = 'normal'
     
     def calib_mode(self):
         self.testFinished = False
         attenuations = numpy.arange(float(self.low), float(self.high) + float(self.step), float(self.step))
+        n_rep = int(self.n_repetitions)
         for i in attenuations:
-            calibMutex.acquire()
-            self.total_num_of_unique = 0
-            self.offline_tag_index = 0
-            self.avg_unique = 1
-            self.cur_atten = i
-            self.advas_dict = {}
-            self.tagsFinished = {}
-            self.testGo = True
-            if self.antenna.lower() == 'ble':
-                self.params['attenBle'] = self.cur_atten
-                self.dataBaseDict['attenBle[db]'] = self.cur_atten
-            elif self.antenna.lower() == 'lora':
-                self.dataBaseDict['attenLoRa[db]'] = self.cur_atten
-                self.params['attenLoRa'] = self.cur_atten
-            self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
-            self.sendCommandThread.start()
-            self.sendCommandThread.join()
-            sleep(5)
-            if self.forceCloseRequested:
-                break
+            for j in range(n_rep):
+                calibMutex.acquire()
+                self.total_num_of_unique = 0
+                self.offline_tag_index = 0
+                self.avg_unique = 1
+                self.cur_atten = i
+                self.test_num = j
+                self.advas_dict = {}
+                self.tagsFinished = {}
+                self.testGo = True
+                if self.antenna.lower() == 'ble':
+                    self.params['attenBle'] = self.cur_atten
+                    self.dataBaseDict['attenBle[db]'] = self.cur_atten
+                elif self.antenna.lower() == 'lora':
+                    self.dataBaseDict['attenLoRa[db]'] = self.cur_atten
+                    self.params['attenLoRa'] = self.cur_atten
+                self.dataBaseDict['testNum'] = self.test_num
+                self.params['testNum'] = self.test_num
+
+                self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
+                self.sendCommandThread.start()
+                self.sendCommandThread.join()
+                sleep(5)
+                if self.forceCloseRequested:
+                    break
         
         calibMutex.acquire()
         self.calib_mode_post_process()
         self.comConnect.open_chambers()
         # self.builder.tkvariables.get('numTags').set(0)
         # self.builder.tkvariables.get('go').set(READ)
         # self.test_barcodes = {}
@@ -463,29 +456,31 @@
         full_test_dir = join(OUTPUT_DIR, self.testName, self.testDir)
         is_first = True
         for atten, runData in self.packets_dict.items():
             for extId, data in runData.items():
                 if data['packetList'].size() > 0:
                     packet_df = data['packetList'].get_df(add_sprinkler_info=True)
                     packet_df.insert(loc=len(packet_df.columns), column='status', value='PASSED')
-                    packet_df.insert(loc=len(packet_df.columns), column='attenuation', value=atten)
+                    packet_df.insert(loc=len(packet_df.columns), column='attenuation', value=float(atten.split('_')[0]))
+                    packet_df.insert(loc=len(packet_df.columns), column='test_num', value=int(atten.split('_')[1]))
                     packet_df.insert(loc=len(packet_df.columns), column='external_id', value=extId)
                     packet_df.insert(loc=len(packet_df.columns), column='chamber', value=data['chamber'])
                     data['packetList'].export_packet_df(
                         packet_df=packet_df, path=join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv'),
                         append=not is_first)
                     is_first = False
                 
                 unique_valid.append({
                     'adv_address': data['adv_address'],
                     'tbp': data['tbp'],
                     'ttfp': data['ttfp'],
                     'ext ID': data['ext ID'],
                     'reel': data['reel'],
-                    'attenuation': atten,
+                    'attenuation': float(atten.split('_')[0]),
+                    'test_num': int(atten.split('_')[1]),
                     'chamber': data['chamber']
                 })
         
         if len(unique_valid):
             with open(join(full_test_dir, f'{common_run_name}@unique_data.csv'), 'w+', newline='') as new_tagsCsv:
                 writer = csv.DictWriter(new_tagsCsv, fieldnames=list(unique_valid[0].keys()))
                 writer.writeheader()
@@ -568,30 +563,30 @@
             chambers = self.comConnect.get_chambers()
             if len(chambers) > scan_index and chambers[scan_index] is not None:
                 chambers[scan_index].close_chamber()
             self.update_go_state()
         else:
             self.builder.get_object('scanned').insert(END, new_tag)
             self.builder.tkvariables.get('addTag').set('')
-    
+
     def remove(self):
         """
         remove tag read from the list
         """
         tag = self.builder.get_object('scanned').get(ACTIVE)
         tags = list(self.builder.get_object('scanned').get(0, END))
         tag_index = tags.index(tag)
         self.builder.get_object('scanned').delete(tag_index, tag_index)
         tags.pop(tag_index)
         self.builder.tkvariables.get('addTag').set(tag)
         if self.stopButtonState != SEND:
             self.barcodes_read.pop(tag.split(',')[0].strip())
             self.comConnect.open_chambers(indexes=[int(tag.split(',')[1].strip())])
             self.update_go_state()
-    
+
     def update_params_state(self, state='disabled', group=GO):
         if state == 'disabled' or group == READ:
             self.builder.get_object('connect')['state'] = state
             
             if len(self.test_barcodes.keys()) == 0:
                 self.builder.get_object('read_qr')['state'] = state
                 self.builder.get_object('reelId')['state'] = state
@@ -637,17 +632,17 @@
         if 'testName' in self.defaultDict.keys():
             self.builder.get_object('testName')['values'] = self.defaultDict['testName']
             self.builder.get_object('testName').set(self.defaultDict['testName'][0])
         
         if 'operator' in self.defaultDict.keys():
             self.builder.get_object('operator')['values'] = self.defaultDict['operator']
             self.builder.get_object('operator').set(self.defaultDict['operator'][0])
-        
+
+        self.builder.get_object('inlay')['values'] = tuple(InlayTypes._member_names_)
         if 'inlay' in self.defaultDict.keys():
-            self.builder.get_object('inlay')['values'] = self.defaultDict['inlay']
             self.builder.get_object('inlay').set(self.defaultDict['inlay'][0])
         
         if 'surface' in self.defaultDict.keys():
             self.builder.get_object('surface')['values'] = self.defaultDict['surface']
             self.builder.get_object('surface').set(self.defaultDict['surface'][0])
         if 'tester_hw' in self.defaultDict.keys():
             self.builder.get_object('tester_hw_ver')['state'] = 'enabled'
@@ -659,24 +654,24 @@
             self.builder.get_object('tester_hw_desc').insert(0, self.defaultDict['tester_hw']['description'])
             self.builder.get_object('tester_hw_desc')['state'] = 'disabled'
         # if 'numOfTags' in self.defaultDict.keys():
         # self.builder.tkvariables.get('numTags').set(self.defaultDict['numOfTags'])
         # else:
         # self.builder.tkvariables.get('numTags').set(DEF_NUM_OF_TAGS)
         self.builder.tkvariables.get('numTags').set(0)
-        
-        if self.post_data:
-            self.builder.get_variable('sendToCloud').set('1')
-        else:
-            self.builder.get_variable('sendToCloud').set('0')
+
+        self.builder.get_variable('sendToCloud').set(str(int(self.post_data)))
+        self.builder.get_variable('isCalib').set(str(int(self.calib)))
+        self.builder.get_variable('isOffline').set(str(int(self.offline)))
+        self.builder.get_variable('isTestEnv').set(str(int(self.environment == 'test')))
         
         if 'config' in self.defaultDict.keys():
             self.testConfig = self.defaultDict['config']
         else:
-            self.testConfig = DEFAULT_CONFIGS[0]
+            self.testConfig = []
         self.builder.get_object('test_config').set(self.testConfig)
         self.configsGui.set_default_config(self.testConfig)
         self.configsGui.set_params(self.testConfig)
     
     def open_configs(self):
         """
         open Configs GUI
@@ -715,15 +710,15 @@
             reel_id = self.builder.tkvariables.get('reelId')
             reel_id.set(reel)
             self.reel_id = reel
         
         if 'config' in self.defaultDict.keys():
             self.testConfig = self.defaultDict['config']
         else:
-            self.testConfig = DEFAULT_CONFIGS[0]
+            self.testConfig = []
         
         self.builder.get_object('reelId').unbind("<Key>")
         self.update_params_state(state='normal', group=GO)
         self.builder.get_object('forceGo')['state'] = 'normal'
     
     def get_reel_id(self, *args):
         reel = self.builder.tkvariables.get('reelId').get()
@@ -773,15 +768,16 @@
         self.runDataDict['controlLimits'] = 'tagTbpRange: [{},{}], testTbpRange: [{},{}], respondingThr[%]: {}, ' \
                                             'validTbpThr[%]: {}'.format(params['tag_tbp_min'], params['tag_tbp_max'],
                                                                         params['test_tbp_min'], params['test_tbp_max'],
                                                                         params['test_responding_min'],
                                                                         params['test_valid_tbp'])
         self.runDataDict['hwVersion'] = self.defaultDict['tester_hw']['version'] \
             if 'tester_hw' in self.defaultDict.keys() else ''
-    
+        self.runDataDict['sub1gFrequency'] = params['EmulateSurfaceValue']
+
     def send_gw_commands(self):
         """
         send commands to the GW and start the packet listener
         """
         if self.sleep > 0:
             for i in range(self.sleep):
                 sleep(1)
@@ -856,16 +852,16 @@
             self.finishIterThread = Thread(target=self.iteration_finished, args=())
             self.finishIterThread.start()
         elif self.calib:
             self.handle_unknown_packets()
             self.unknown_packets = PacketList()
             self.post_process_iteration()
             
-            self.packets_dict[self.cur_atten] = {}
-            self.packets_dict[self.cur_atten].update(self.barcodes_read)
+            self.packets_dict[f'{self.cur_atten}_{self.test_num}'] = {}
+            self.packets_dict[f'{self.cur_atten}_{self.test_num}'].update(self.barcodes_read)
             self.calib_mode_clean_barcodes()
             calibMutex.release()
     
     def threads_sync(self):
         while not self.closeRequested and not self.forceCloseRequested and time.time() < self.targetTime:
             if len(self.add_to_dict_threads) > 0:
                 addToDictMutex.acquire()
@@ -934,16 +930,15 @@
                         logger.error(
                             f'Could not get external ID for adv_address {adv_address} '
                             f'from the cloud - dumping packet')
                     continue
 
                 ext_id = full_data['barcode'] if full_data['barcode'] in self.barcodes_read.keys() else full_data[
                     'cur_id']
-                if (ext_id is not None or self.debug_mode is not None) \
-                        and ext_id not in self.barcodes_read.keys():
+                if ext_id is not None and ext_id not in self.barcodes_read.keys():
                     logger.info(
                         f'Tag with adv_address {adv_address} and external ID {full_data["cur_id"]} '
                         f'detected but not belong to the test.')
                     self.bad_advas.append(adv_address)
                     continue
 
                 self.advas_dict[adv_address] = ext_id
@@ -1213,28 +1208,33 @@
         
         if post_data and self.post_data:
             post_success = self.post_to_cloud(run_data_path, tags_data_path, environment=self.environment)
             if not post_success:
                 popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
                               f'{self.common_run_name}@run_data.csv\n' +
                               f'{self.common_run_name}@packets_data.csv', log='warning')
-    
+
     def get_packet_ext_id(self, packet):
         """
         get external ID of a tag by sending an example packet to the cloud.
         :type packet: Packet
         :param packet: contains the raw and time of the packet.
         :return: external ID of the tag, and the external ID parsed when it's wiliot tag.
         """
         full_data = {'barcode': None, 'cur_id': None, 'reel_id': None, 'gtin': None}
         if self.offline:
             success = True
             full_data['cur_id'] = list(self.barcodes_read.keys())[self.offline_tag_index]
             full_data['reel_id'] = self.reel_id
-            full_data['gtin'] = '(01)00850027865010(21)'
+            if len(self.reel_id) < 4:
+                print('reel id smaller than 4 char assuming barcode format')
+                full_data['gtin'] = ''
+            else:
+                print('according to reel id length, assuming sgtin format')
+                full_data['gtin'] = SGTIN_PREFIX_DEFAULT
             full_data['barcode'] = full_data['gtin'] + full_data['reel_id'] + 'T' + full_data['cur_id']
             self.offline_tag_index += 1
             return full_data, success
 
         packet_payload = packet.packet_data['raw_packet'][16::]
 
         res = self.client.resolve_payload(payload=packet_payload, owner_id=self.owner)
@@ -1243,17 +1243,20 @@
             if res['externalId'] != 'unknown':
                 full_data['barcode'] = res['externalId']
                 full_data['cur_id'] = full_data['reel_id'] = full_data['gtin'] = full_data['barcode']
                 try:
                     if ')' in full_data['barcode']:
                         tag_data = full_data['barcode'].split(')')[2]
                         full_data['gtin'] = ')'.join(full_data['barcode'].split(')')[:2]) + ')'
-                    else:  # gtin without parenthesis
+                    elif len(full_data['barcode']) >= len(SGTIN_PREFIX_DEFAULT):  # gtin without parenthesis
                         full_data['gtin'] = full_data['barcode'][0:18]
                         tag_data = full_data['barcode'][18:]
+                    else:  # barcode or an other type with no prefix
+                        full_data['gtin'] = ''
+                        tag_data = full_data['barcode']
 
                     full_data['cur_id'] = tag_data.split('T')[1].strip("' ")
                     full_data['reel_id'] = tag_data.split('T')[0].strip("' ")
                     success = True
                 except Exception as e:
                     success = False
                     print('got invalid external id: {} with exception: {}'.format(res, e))
@@ -1317,32 +1320,31 @@
         num_of_answered = len(ttfp_arr)
         num_of_pass = len(pass_barcodes)
         self.dataBaseDict['packets'] = self.numOfPackets
         self.dataBaseDict['tested'] = self.runDataDict['tested'] = tested_barcodes
         self.dataBaseDict['responded'] = self.runDataDict['responded'] = num_of_answered
         self.dataBaseDict['passed'] = self.runDataDict['passed'] = num_of_pass
         self.dataBaseDict['responding[%]'] = self.runDataDict['responding[%]'] = self.runDataDict['yield'] = \
-            f'{int((num_of_answered / tested_barcodes) * 100)}%'
+            f'{int((num_of_answered / tested_barcodes) * 100) if tested_barcodes > 0 else 0}%'
         self.dataBaseDict['passed[%]'] = self.runDataDict[
-            'passed[%]'] = f'{int((num_of_pass / tested_barcodes) * 100)}%'
-
-        
+            'passed[%]'] = f'{int((num_of_pass / tested_barcodes) * 100 if tested_barcodes > 0 else 0)}%'
+        # calc ttfp
         avg_ttfp = sum(ttfp_arr) / len(ttfp_arr) if len(ttfp_arr) > 0 else -1
         ttfp_arr = ttfp_arr if len(ttfp_arr) > 0 else [-1]
         
         self.dataBaseDict['ttfpStd'] = f'{numpy.std(ttfp_arr):.3f}'
         self.runDataDict['ttfpAvg'] = self.dataBaseDict['ttfpAvg'] = f'{avg_ttfp:.3f}'
         self.dataBaseDict['ttfpMin'] = f'{min(ttfp_arr):.3f}'
         self.runDataDict['maxTtfp'] = self.dataBaseDict['ttfpMax'] = f'{max(ttfp_arr):.3f}'
-        # self.dataBaseDict['ttfpMax'] = f'{max(ttfp_arr):.3f}'
-        
+
+        # calc tbp
         avg_tbp = sum(tbp_arr) / len(tbp_arr) if len(tbp_arr) > 0 else -1
         tbp_arr = tbp_arr if len(tbp_arr) > 0 else [-1]
         
-        self.dataBaseDict['tbpStd'] = f'{numpy.std(tbp_arr):.3f}'
+        self.runDataDict['tbpStd'] = self.dataBaseDict['tbpStd'] = f'{numpy.std(tbp_arr):.3f}'
         self.runDataDict['tbpAvg'] = self.dataBaseDict['tbpAvg'] = f'{avg_tbp:.3f}'
         self.dataBaseDict['tbpMin'] = f'{min(tbp_arr):.3f}'
         self.dataBaseDict['tbpMax'] = f'{max(tbp_arr):.3f}'
         
         avg_rssi = sum(rssi_arr) / len(rssi_arr) if len(rssi_arr) > 0 else -1
         rssi_arr = rssi_arr if len(rssi_arr) > 0 else [-1]
         
@@ -1473,26 +1475,29 @@
         popup.protocol("WM_DELETE_WINDOW", quit_calib)
         
         def ok():
             # global low, high, step
             self.low = e2.get()
             self.high = e3.get()
             self.step = e4.get()
+            self.n_repetitions = e5.get()
             popup.destroy()
         
         def update_antenna_params(*args):
             self.antenna = antenna = c2.get().lower()
             if f'{antenna}_calib' in self.defaultDict.keys():
                 antennaDict = self.defaultDict[f'{antenna}_calib']
                 e2.delete(0, END)
                 e3.delete(0, END)
                 e4.delete(0, END)
+                e5.delete(0, END)
                 e2.insert(0, antennaDict['low'])
                 e3.insert(0, antennaDict['high'])
                 e4.insert(0, antennaDict['step'])
+                e5.insert(0, 1)
         
         l1 = Label(popup, text='Enter calibration parameters:', font=default_font)
         l1.grid(row=1, column=0, padx=10, pady=10, columnspan=3)
         l2 = Label(popup, text='Antenna Type:', font=default_font)
         l2.grid(row=2, column=0, padx=10, pady=10)
         c2 = ttk.Combobox(popup, values=['BLE', 'LoRa'])
         c2.grid(row=2, column=1, padx=10, pady=10)
@@ -1506,23 +1511,44 @@
         l4.grid(row=4, column=0, padx=10, pady=10)
         e3 = Entry(popup)
         e3.grid(row=4, column=1, padx=10, pady=5)
         l5 = Label(popup, text='Step:', font=default_font)
         l5.grid(row=5, column=0, padx=10, pady=10)
         e4 = Entry(popup)
         e4.grid(row=5, column=1, padx=10, pady=5)
+        l6 = Label(popup, text='Number of Repetitions per step:', font=default_font)
+        l6.grid(row=6, column=0, padx=10, pady=10)
+        e5 = Entry(popup)
+        e5.grid(row=6, column=1, padx=10, pady=5)
         b1 = Button(popup, text="Quit", command=quit_calib, height=1, width=10)
-        b1.grid(row=6, column=0, padx=10, pady=10)
+        b1.grid(row=7, column=0, padx=10, pady=10)
         b2 = Button(popup, text="Ok", command=ok, height=1, width=10)
-        b2.grid(row=6, column=2, padx=10, pady=10)
+        b2.grid(row=7, column=1, padx=10, pady=10)
         
         popup.mainloop()
         
         # return antenna, low, high, step
 
+    def on_send_to_cloud(self):
+        self.post_data = bool(int(self.builder.get_variable('sendToCloud').get()))
+        logger.info(f'send to cloud was changed to {self.post_data}')
+
+    def on_power_calib(self):
+        self.calib = bool(int(self.builder.get_variable('isCalib').get()))
+        logger.info(f'calibration mode was changed to {self.calib}')
+
+    def on_offline(self):
+        self.offline = bool(int(self.builder.get_variable('isOffline').get()))
+        logger.info(f'offline mode was changed to {self.offline}')
+
+    def on_test_env(self):
+        self.environment = 'test' if bool(int(self.builder.get_variable('isTestEnv').get())) else ''
+        env_for_printing = self.environment if self.environment != '' else 'production'
+        logger.info(f'sending data to {env_for_printing} environment')
+
 
 def popup_yes_no(question):
     root = Tk()
     root.wm_withdraw()
     result = messagebox.askquestion("Sample Test", question, icon='warning')
     root.destroy()
     if result == 'yes':
@@ -1542,15 +1568,14 @@
         eval_str = '{:.0f}'
     return float(eval_str.format(num))
 
 
 if __name__ == '__main__':
     
     parser = argparse.ArgumentParser(description='Run PixieParser')
-    parser.add_argument('-d', '--debug', help='Debug mode', default=False, action='store_true')
     parser.add_argument('-c', '--calib', help='Calibration mode', default=False, action='store_true')
     parser.add_argument('-e', '--environment', help='Environment: test or not', default='')
     parser.add_argument('-p', '--post_data', help='Post data to the cloud', default=True)
     parser.add_argument('-o', '--offline', help='Offline mode', default=False, action='store_true')
     args = parser.parse_args()
     calib = args.calib
     post_data = args.post_data
@@ -1561,13 +1586,13 @@
     # offline = True
     if calib:
         logger.warning(f'Sample Test - calibration mode active.')
     if offline:
         logger.warning(f'Sample Test - offline mode active.')
     app_folder = abspath(join(dirname(__file__), '../wiliot_testers'))
     try:
-        sampleTest = SampleTest(debug_mode=args.debug, calib=calib, environment=args.environment, post_data=post_data,
+        sampleTest = SampleTest(calib=calib, environment=args.environment, post_data=post_data,
                                 offline=offline)
         sampleTest.gui()
     except BaseException:
         print_exc()
         exit(0)
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/com_connect.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/comm.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/configs.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/configs.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/reset.png` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui`

 * *Files 2% similar despite different names*

#### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui`

```diff
@@ -252,25 +252,27 @@
           <property name="propagate">True</property>
           <property name="row">12</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Checkbutton" id="sendToCloud">
+        <property cbtype="simple" name="command" type="command">on_send_to_cloud</property>
         <property name="offvalue">0</property>
         <property name="onvalue">1</property>
-        <property name="state">disabled</property>
+        <property name="state">normal</property>
         <property name="text" translatable="yes">Send to cloud</property>
         <property name="variable">string:sendToCloud</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">12</property>
+          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="operatorLabel">
         <property name="text" translatable="yes">Operator:</property>
         <layout manager="grid">
@@ -549,15 +551,15 @@
       </object>
     </child>
     <child>
       <object class="ttk.Separator" id="separator5">
         <property name="orient">horizontal</property>
         <layout manager="grid">
           <property name="column">0</property>
-          <property name="columnspan">3</property>
+          <property name="columnspan">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">14</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
@@ -605,33 +607,57 @@
           <property name="propagate">True</property>
           <property name="row">28</property>
           <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
-      <object class="ttk.Button" id="edit_hw_tester">
-        <property cbtype="simple" name="command" type="command">on_edit_hw_tester</property>
-        <property name="image">edit.gif</property>
-        <property name="width">2</property>
+      <object class="ttk.Checkbutton" id="is_calib">
+        <property cbtype="simple" name="command" type="command">on_power_calib</property>
+        <property name="offvalue">0</property>
+        <property name="onvalue">1</property>
+        <property name="state">normal</property>
+        <property name="text" translatable="yes">test calibration</property>
+        <property name="variable">string:isCalib</property>
         <layout manager="grid">
           <property name="column">2</property>
+          <property name="padx">5</property>
+          <property name="pady">5</property>
           <property name="propagate">True</property>
-          <property name="row">27</property>
+          <property name="row">13</property>
+          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
-      <object class="ttk.Button" id="save_tester_hw">
-        <property cbtype="simple" name="command" type="command">on_save_tester_hw</property>
-        <property name="image">save.png</property>
-        <property name="text" translatable="yes">button1</property>
+      <object class="ttk.Checkbutton" id="offline">
+        <property cbtype="simple" name="command" type="command">on_offline</property>
+        <property name="offvalue">0</property>
+        <property name="onvalue">1</property>
+        <property name="text" translatable="yes">offline mode</property>
+        <property name="variable">string:isOffline</property>
         <layout manager="grid">
           <property name="column">2</property>
+          <property name="padx">5</property>
+          <property name="pady">5</property>
           <property name="propagate">True</property>
-          <property name="row">27</property>
-          <property name="sticky">e</property>
+          <property name="row">14</property>
+          <property name="sticky">w</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Checkbutton" id="is_test_env">
+        <property cbtype="simple" name="command" type="command">on_test_env</property>
+        <property name="offvalue">0</property>
+        <property name="onvalue">1</property>
+        <property name="text" translatable="yes">develop mode</property>
+        <property name="variable">string:isTestEnv</property>
+        <layout manager="grid">
+          <property name="column">2</property>
+          <property name="propagate">True</property>
+          <property name="row">15</property>
         </layout>
       </object>
     </child>
   </object>
 </interface>
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/sample/utils/wiliot3.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/system_test/harvester_test.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,23 +57,31 @@
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 '''
 Eduard Tatievski
 '''
 
+
 import matplotlib.pyplot as plt
-from wiliot_testers.test_equipment import Attenuator, EquipmentError
-from wiliot_testers.wiliot_tester_log import *
 import PySimpleGUI as SimGUI
 import os
 import pathlib
 import datetime
 import csv
 import collections
+import sys
+import threading
+import pandas as pd
+from wiliot_testers.test_equipment import Attenuator, EquipmentError
+from wiliot_testers.wiliot_tester_log import *
+from wiliot_core import WiliotGateway, ActionType, DataType
+from wiliot_core import PacketList, TagCollection
+from wiliot_testers.wiliot_tester_tag_test import *
+from wiliot_core import DecryptedPacketList, DecryptedTagCollection
 
 
 class Harvester(object):
 
     def __init__(self):
         # Getting all wanted values
         self.num_of_chambers = 1  # Number of chambers connected
@@ -796,8 +804,7 @@
 
 
 if __name__ == '__main__':
     harvest = Harvester()
     results = harvest.get_result()
     pass
 
-# TODO Add time out function, add success flag after analyzeing, duplicated packets handling, reset clock after starting analyzing, output array is still empty
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/system_test/system_test_example.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/test_equipment.py` & `wiliot-testers-4.0.6/wiliot_testers/test_equipment.py`

 * *Files 18% similar despite different names*

```diff
@@ -246,1267 +246,1708 @@
 00000f50: 6d70 6f72 7420 7365 7269 616c 0a69 6d70  mport serial.imp
 00000f60: 6f72 7420 7365 7269 616c 2e74 6f6f 6c73  ort serial.tools
 00000f70: 2e6c 6973 745f 706f 7274 730a 6672 6f6d  .list_ports.from
 00000f80: 2079 6f63 746f 7075 6365 2e79 6f63 746f   yoctopuce.yocto
 00000f90: 5f74 656d 7065 7261 7475 7265 2069 6d70  _temperature imp
 00000fa0: 6f72 7420 5941 5049 2c20 5952 6566 5061  ort YAPI, YRefPa
 00000fb0: 7261 6d2c 2059 5465 6d70 6572 6174 7572  ram, YTemperatur
-00000fc0: 650a 0a0a 636c 6173 7320 4571 7569 706d  e...class Equipm
-00000fd0: 656e 7445 7272 6f72 2845 7863 6570 7469  entError(Excepti
-00000fe0: 6f6e 293a 0a20 2020 200a 2020 2020 6465  on):.    .    de
-00000ff0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00001000: 202a 6172 6773 293a 0a20 2020 2020 2020   *args):.       
-00001010: 2069 6620 6172 6773 3a0a 2020 2020 2020   if args:.      
-00001020: 2020 2020 2020 7365 6c66 2e6d 6573 7361        self.messa
-00001030: 6765 203d 2061 7267 735b 305d 0a20 2020  ge = args[0].   
-00001040: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00001050: 2020 2020 2020 2073 656c 662e 6d65 7373         self.mess
-00001060: 6167 6520 3d20 4e6f 6e65 0a20 2020 200a  age = None.    .
-00001070: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
-00001080: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-00001090: 2070 7269 6e74 2827 6361 6c6c 696e 6720   print('calling 
-000010a0: 7374 7227 290a 2020 2020 2020 2020 6966  str').        if
-000010b0: 2073 656c 662e 6d65 7373 6167 653a 0a20   self.message:. 
-000010c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000010d0: 6e20 2745 7175 6970 6d65 6e74 4572 726f  n 'EquipmentErro
-000010e0: 723a 207b 6d73 677d 272e 666f 726d 6174  r: {msg}'.format
-000010f0: 286d 7367 3d73 656c 662e 6d65 7373 6167  (msg=self.messag
-00001100: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-00001110: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001120: 7572 6e20 2745 7175 6970 6d65 6e74 4572  urn 'EquipmentEr
-00001130: 726f 7220 6861 7320 6265 656e 2072 6169  ror has been rai
-00001140: 7365 6427 0a0a 0a64 6566 2073 6572 6961  sed'...def seria
-00001150: 6c5f 706f 7274 7328 293a 0a20 2020 2022  l_ports():.    "
-00001160: 2222 204c 6973 7473 2073 6572 6961 6c20  "" Lists serial 
-00001170: 706f 7274 206e 616d 6573 0a0a 2020 2020  port names..    
-00001180: 2020 2020 3a72 6169 7365 7320 456e 7669      :raises Envi
-00001190: 726f 6e6d 656e 7445 7272 6f72 3a0a 2020  ronmentError:.  
-000011a0: 2020 2020 2020 2020 2020 4f6e 2075 6e73            On uns
-000011b0: 7570 706f 7274 6564 206f 7220 756e 6b6e  upported or unkn
-000011c0: 6f77 6e20 706c 6174 666f 726d 730a 2020  own platforms.  
-000011d0: 2020 2020 2020 3a72 6574 7572 6e73 3a0a        :returns:.
-000011e0: 2020 2020 2020 2020 2020 2020 4120 6c69              A li
-000011f0: 7374 206f 6620 7468 6520 7365 7269 616c  st of the serial
-00001200: 2070 6f72 7473 2061 7661 696c 6162 6c65   ports available
-00001210: 206f 6e20 7468 6520 7379 7374 656d 0a20   on the system. 
-00001220: 2020 2022 2222 0a20 2020 2061 7661 696c     """.    avail
-00001230: 6162 6c65 5f70 6f72 7473 203d 205b 732e  able_ports = [s.
-00001240: 6465 7669 6365 2066 6f72 2073 2069 6e20  device for s in 
-00001250: 7365 7269 616c 2e74 6f6f 6c73 2e6c 6973  serial.tools.lis
-00001260: 745f 706f 7274 732e 636f 6d70 6f72 7473  t_ports.comports
-00001270: 2829 5d0a 2020 2020 6966 206c 656e 2861  ()].    if len(a
-00001280: 7661 696c 6162 6c65 5f70 6f72 7473 2920  vailable_ports) 
-00001290: 3d3d 2030 3a0a 2020 2020 2020 2020 6176  == 0:.        av
-000012a0: 6169 6c61 626c 655f 706f 7274 7320 3d20  ailable_ports = 
-000012b0: 5b73 2e6e 616d 6520 666f 7220 7320 696e  [s.name for s in
-000012c0: 2073 6572 6961 6c2e 746f 6f6c 732e 6c69   serial.tools.li
-000012d0: 7374 5f70 6f72 7473 2e63 6f6d 706f 7274  st_ports.comport
-000012e0: 7328 295d 0a20 2020 2020 2020 2069 6620  s()].        if 
-000012f0: 6c65 6e28 6176 6169 6c61 626c 655f 706f  len(available_po
-00001300: 7274 7329 203d 3d20 303a 0a20 2020 2020  rts) == 0:.     
-00001310: 2020 2020 2020 2070 7269 6e74 2822 6e6f         print("no
-00001320: 2073 6572 6961 6c20 706f 7274 7320 7765   serial ports we
-00001330: 7265 2066 6f75 6e64 2e20 706c 6561 7365  re found. please
-00001340: 2063 6865 636b 2079 6f75 7220 636f 6e6e   check your conn
-00001350: 6563 7469 6f6e 7322 290a 2020 2020 7265  ections").    re
-00001360: 7475 726e 2061 7661 696c 6162 6c65 5f70  turn available_p
-00001370: 6f72 7473 0a0a 0a63 6c61 7373 2041 7474  orts...class Att
-00001380: 656e 7561 746f 7228 6f62 6a65 6374 293a  enuator(object):
-00001390: 0a20 2020 2027 2727 0a20 2020 2053 7570  .    '''.    Sup
-000013a0: 706f 7274 2063 6c61 7373 2066 6f72 3a0a  port class for:.
-000013b0: 2020 2020 4150 4954 6563 6820 4165 726f      APITech Aero
-000013c0: 666c 6578 2057 6569 6e73 6368 656c 2c20  flex Weinschel, 
-000013d0: 3432 3035 2c20 302c 2056 312e 3330 0a20  4205, 0, V1.30. 
-000013e0: 2020 2027 2727 0a20 2020 200a 2020 2020     '''.    .    
-000013f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001400: 662c 2041 5454 4e5f 7479 7065 2c20 636f  f, ATTN_type, co
-00001410: 6d70 6f72 743d 2741 5554 4f27 293a 0a20  mport='AUTO'):. 
-00001420: 2020 2020 2020 2069 6620 2741 5049 2720         if 'API' 
-00001430: 696e 2041 5454 4e5f 7479 7065 3a0a 2020  in ATTN_type:.  
-00001440: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00001450: 6163 7469 7665 5f54 4520 3d20 4174 7465  active_TE = Atte
-00001460: 6e75 6174 6f72 2e41 5049 2863 6f6d 706f  nuator.API(compo
-00001470: 7274 290a 2020 2020 2020 2020 656c 7365  rt).        else
-00001480: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00001490: 7373 0a20 2020 200a 2020 2020 6465 6620  ss.    .    def 
-000014a0: 4765 7441 6374 6976 6554 4528 7365 6c66  GetActiveTE(self
-000014b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-000014c0: 6e20 7365 6c66 2e5f 6163 7469 7665 5f54  n self._active_T
-000014d0: 450a 2020 2020 0a20 2020 2063 6c61 7373  E.    .    class
-000014e0: 2041 5049 286f 626a 6563 7429 3a0a 2020   API(object):.  
-000014f0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
-00001500: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001510: 2c20 636f 6d70 6f72 743d 2241 5554 4f22  , comport="AUTO"
-00001520: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00001530: 656c 662e 6261 7564 7261 7465 203d 2039  elf.baudrate = 9
-00001540: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
-00001550: 6966 2063 6f6d 706f 7274 203d 3d20 2241  if comport == "A
-00001560: 5554 4f22 3a0a 2020 2020 2020 2020 2020  UTO":.          
-00001570: 2020 2020 2020 706f 7274 735f 6c69 7374        ports_list
-00001580: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
-00001590: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000015a0: 2020 666f 7220 706f 7274 2069 6e20 706f    for port in po
-000015b0: 7274 735f 6c69 7374 3a0a 2020 2020 2020  rts_list:.      
-000015c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000015d0: 6c66 2e63 6f6d 706f 7274 203d 2070 6f72  lf.comport = por
-000015e0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000015f0: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
-00001600: 6572 6961 6c2e 5365 7269 616c 2873 656c  erial.Serial(sel
-00001610: 662e 636f 6d70 6f72 742c 2073 656c 662e  f.comport, self.
-00001620: 6261 7564 7261 7465 2c20 7469 6d65 6f75  baudrate, timeou
-00001630: 743d 302e 3529 0a20 2020 2020 2020 2020  t=0.5).         
-00001640: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00001650: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
-00001660: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
-00001670: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
-000016a0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-000016b0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
-000016c0: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
-000016d0: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
-000016e0: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
-00001710: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
-00001720: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
-00001750: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
-00001760: 2020 2020 2020 2020 2020 2020 736c 6565              slee
-00001770: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00001780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001790: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
-000017a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000017b0: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
-000017c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000017d0: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
-000017e0: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001800: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
-00001810: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
-00001820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001830: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00001840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001850: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
-00001860: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
-00001890: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
-000018a0: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018e0: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
-000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001900: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
-00001910: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00001920: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
-00001930: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
-00001960: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
-00001970: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
-00001980: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
-00001990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000019a0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
-000019d0: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
-000019e0: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
-00001a10: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
-00001a20: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
-00001a30: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
-00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
-00001a80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00001a90: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
-00001aa0: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
-00001ab0: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
-00001ac0: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
-00001ad0: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
-00001ae0: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
-00001af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001b00: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
-00001b10: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
-00001b20: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
-00001b30: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
-00001b40: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
-00001b50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001b60: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
-00001b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001b80: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
-00001bb0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-00001bc0: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
-00001bd0: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
-00001be0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00001bf0: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
-00001c00: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
-00001c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001c20: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001c40: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
-00001c50: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
-00001c60: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001c80: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
-00001c90: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
-00001ca0: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
-00001cb0: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
-00001cc0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00001cd0: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
-00001ce0: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
-00001cf0: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
-00001d00: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
-00001d10: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
-00001d20: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
-00001d30: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
-00001d40: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
-00001d50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
-00001d80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001d90: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
-00001da0: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
-00001db0: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
-00001dc0: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
-00001dd0: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
-00001de0: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
-00001df0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001e00: 2020 6465 6620 5772 6974 6528 7365 6c66    def Write(self
-00001e10: 2c20 636d 642c 2077 6169 743d 4661 6c73  , cmd, wait=Fals
-00001e20: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00001e30: 2222 2253 656e 6420 7468 6520 696e 7075  """Send the inpu
-00001e40: 7420 636d 6420 7374 7269 6e67 2076 6961  t cmd string via
-00001e50: 2043 4f4d 2053 6f63 6b65 7422 2222 0a20   COM Socket""". 
-00001e60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00001e70: 6c66 2e73 2e69 734f 7065 6e28 293a 0a20  lf.s.isOpen():. 
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001e90: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00001ea0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00001eb0: 2020 2020 2020 7365 6c66 2e73 2e6f 7065        self.s.ope
-00001ec0: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00001ed0: 7365 6c66 2e73 2e66 6c75 7368 496e 7075  self.s.flushInpu
-00001ee0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00001ef0: 736c 6565 7028 3129 0a20 2020 2020 2020  sleep(1).       
-00001f00: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00001f10: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00001f20: 2e77 7269 7465 2873 7472 2e65 6e63 6f64  .write(str.encod
-00001f30: 6528 636d 6429 290a 2020 2020 2020 2020  e(cmd)).        
-00001f40: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00001f50: 3129 2020 2320 436f 6d6d 616e 6473 206d  1)  # Commands m
-00001f60: 6179 2062 6520 6c6f 7374 2077 6865 6e20  ay be lost when 
-00001f70: 7772 6974 696e 6720 746f 6f20 6661 7374  writing too fast
-00001f80: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00001f90: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00001fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001fb0: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-00001fc0: 2020 2023 2073 656c 662e 732e 636c 6f73     # self.s.clos
-00001fd0: 6528 290a 2020 2020 2020 2020 0a20 2020  e().        .   
-00001fe0: 2020 2020 2064 6566 2051 7565 7279 2873       def Query(s
-00001ff0: 656c 662c 2063 6d64 293a 0a20 2020 2020  elf, cmd):.     
-00002000: 2020 2020 2020 2022 2222 5365 6e64 2074         """Send t
-00002010: 6865 2069 6e70 7574 2063 6d64 2073 7472  he input cmd str
-00002020: 696e 6720 7669 6120 434f 4d20 536f 636b  ing via COM Sock
-00002030: 6574 2061 6e64 2072 6574 7572 6e20 7468  et and return th
-00002040: 6520 7265 706c 7920 7374 7269 6e67 2222  e reply string""
-00002050: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
-00002060: 2073 656c 662e 732e 6973 4f70 656e 2829   self.s.isOpen()
-00002070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002080: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-00002090: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000020a0: 2020 2020 2020 2020 2073 656c 662e 732e           self.s.
-000020b0: 6f70 656e 2829 0a20 2020 2020 2020 2020  open().         
-000020c0: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
-000020d0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-000020e0: 7365 6c66 2e73 2e66 6c75 7368 496e 7075  self.s.flushInpu
-000020f0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00002100: 736c 6565 7028 3129 0a20 2020 2020 2020  sleep(1).       
-00002110: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00002120: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00002130: 2e77 7269 7465 2863 6d64 2e65 6e63 6f64  .write(cmd.encod
-00002140: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
-00002150: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 6966 2073 656c 662e 732e 696e 5f77 6169  if self.s.in_wai
-00002180: 7469 6e67 203e 2030 3a0a 2020 2020 2020  ting > 0:.      
-00002190: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000021a0: 7461 203d 2073 656c 662e 732e 7265 6164  ta = self.s.read
-000021b0: 6c69 6e65 2829 2e64 6563 6f64 6528 2275  line().decode("u
-000021c0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
-000021d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2064 6174 6120 3d20 2727 0a20 2020 2020   data = ''.     
-00002200: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-00002210: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00002220: 6174 6120 3d20 2727 0a20 2020 2020 2020  ata = ''.       
-00002230: 2020 2020 2023 2073 656c 662e 732e 636c       # self.s.cl
-00002240: 6f73 6528 290a 2020 2020 2020 2020 2020  ose().          
-00002250: 2020 7265 7475 726e 2064 6174 610a 2020    return data.  
-00002260: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
-00002270: 6566 2063 6c6f 7365 5f70 6f72 7428 7365  ef close_port(se
-00002280: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
-00002290: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
-000022a0: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
-000022b0: 732e 6973 4f70 656e 2829 3a0a 2020 2020  s.isOpen():.    
-000022c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000022d0: 2e73 2e63 6c6f 7365 2829 0a20 2020 2020  .s.close().     
-000022e0: 2020 200a 2020 2020 2020 2020 6465 6620     .        def 
-000022f0: 6973 5f6f 7065 6e28 7365 6c66 2c20 6368  is_open(self, ch
-00002300: 6563 6b5f 706f 7274 3d46 616c 7365 293a  eck_port=False):
-00002310: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002320: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
-00002330: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002340: 2020 2020 6966 2063 6865 636b 5f70 6f72      if check_por
-00002350: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00002360: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 7365 6c66 2e51 7565 7279 2822      self.Query("
-00002390: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 7265 7370 203d 2073 656c 662e      resp = self.
-000023c0: 5175 6572 7928 222a 4944 4e3f 5c72 5c6e  Query("*IDN?\r\n
-000023d0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000023e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000023f0: 6d6f 6465 6c20 3d20 7265 7370 0a20 2020  model = resp.   
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 2069 6620 2822 4165 726f 666c       if ("Aerofl
-00002420: 6578 2220 696e 2072 6573 7029 3a0a 2020  ex" in resp):.  
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002450: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00002460: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00002470: 6966 2027 3833 3131 2720 696e 2072 6573  if '8311' in res
-00002480: 7020 6f72 2027 3833 3331 2720 696e 2072  p or '8331' in r
-00002490: 6573 703a 0a20 2020 2020 2020 2020 2020  esp:.           
-000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024b0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2073 656c 662e 636c 6f73 655f 706f 7274   self.close_port
-00002500: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00002510: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00002520: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002530: 7572 6e20 7365 6c66 2e73 2e69 734f 7065  urn self.s.isOpe
-00002540: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00002550: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00002560: 2020 2020 200a 2020 2020 2020 2020 6465       .        de
-00002570: 6620 5365 7461 7474 6e28 7365 6c66 2c20  f Setattn(self, 
-00002580: 6174 746e 293a 0a20 2020 2020 2020 2020  attn):.         
-00002590: 2020 2063 6d64 203d 2022 4154 544e 207b     cmd = "ATTN {
-000025a0: 3a2e 3266 7d5c 725c 6e22 2e66 6f72 6d61  :.2f}\r\n".forma
-000025b0: 7428 6174 746e 290a 2020 2020 2020 2020  t(attn).        
-000025c0: 2020 2020 7365 6c66 2e57 7269 7465 2863      self.Write(c
-000025d0: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-000025e0: 7661 6c75 6520 3d20 7365 6c66 2e47 6574  value = self.Get
-000025f0: 6174 746e 2829 0a20 2020 2020 2020 2020  attn().         
-00002600: 2020 2076 616c 7565 203d 2066 6c6f 6174     value = float
-00002610: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
-00002620: 2020 2020 6966 2076 616c 7565 2021 3d20      if value != 
-00002630: 6174 746e 3a0a 2020 2020 2020 2020 2020  attn:.          
-00002640: 2020 2020 2020 7072 696e 7428 6627 4572        print(f'Er
-00002650: 726f 7220 7365 7474 696e 6720 6174 7465  ror setting atte
-00002660: 6e75 6174 696f 6e3a 206e 6577 203a 207b  nuation: new : {
-00002670: 6174 746e 7d20 6375 7272 656e 743a 207b  attn} current: {
-00002680: 7661 6c75 657d 2729 0a20 2020 2020 2020  value}').       
-00002690: 2020 2020 2072 6574 7572 6e20 7661 6c75       return valu
-000026a0: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-000026b0: 2020 2064 6566 2047 6574 6174 746e 2873     def Getattn(s
-000026c0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-000026d0: 2020 636d 6420 3d20 2241 5454 4e3f 5c72    cmd = "ATTN?\r
-000026e0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-000026f0: 7661 6c75 6520 3d20 7365 6c66 2e51 7565  value = self.Que
-00002700: 7279 2863 6d64 290a 2020 2020 2020 2020  ry(cmd).        
-00002710: 2020 2020 7265 7475 726e 2076 616c 7565      return value
-00002720: 0a0a 0a63 6c61 7373 2054 6573 636f 6d3a  ...class Tescom:
-00002730: 0a20 2020 2022 2222 0a20 2020 2043 6f6e  .    """.    Con
-00002740: 7472 6f6c 2054 4553 434f 4d20 7465 7374  trol TESCOM test
-00002750: 696e 6720 6368 616d 6265 7273 0a20 2020  ing chambers.   
-00002760: 2022 2222 0a20 2020 206f 7065 6e5f 636d   """.    open_cm
-00002770: 6420 3d20 6227 4f50 454e 5c72 270a 2020  d = b'OPEN\r'.  
-00002780: 2020 636c 6f73 655f 636d 6420 3d20 6227    close_cmd = b'
-00002790: 434c 4f53 455c 7227 0a20 2020 2063 6f6d  CLOSE\r'.    com
-000027a0: 5f70 6f72 745f 6f62 6a20 3d20 4e6f 6e65  _port_obj = None
-000027b0: 0a20 2020 206d 6f64 656c 735f 6c69 7374  .    models_list
-000027c0: 203d 205b 2754 432d 3530 3634 4327 2c20   = ['TC-5064C', 
-000027d0: 2754 412d 3730 3131 4150 272c 2027 5443  'TA-7011AP', 'TC
-000027e0: 2d35 3036 3341 272c 2027 5443 2d35 3937  -5063A', 'TC-597
-000027f0: 3043 5027 5d0a 2020 2020 0a20 2020 2064  0CP'].    .    d
-00002800: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00002810: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
-00002820: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
-00002830: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
-00002840: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00002850: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
-00002860: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002870: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
-00002880: 7428 706f 7274 290a 2020 2020 2020 2020  t(port).        
-00002890: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000028a0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-000028b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000028c0: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
-000028d0: 2070 7269 6e74 2822 5465 7363 6f6d 202d   print("Tescom -
-000028e0: 2043 6f6e 6e65 6374 696f 6e20 6661 696c   Connection fail
-000028f0: 6564 2229 0a20 2020 200a 2020 2020 6465  ed").    .    de
-00002900: 6620 636f 6e6e 6563 7428 7365 6c66 2c20  f connect(self, 
-00002910: 706f 7274 293a 0a20 2020 2020 2020 2022  port):.        "
-00002920: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00002930: 6d20 706f 7274 3a20 636f 6d20 706f 7274  m port: com port
-00002940: 2074 6f20 636f 6e6e 6563 740a 2020 2020   to connect.    
-00002950: 2020 2020 3a72 6574 7572 6e3a 2063 6f6d      :return: com
-00002960: 2070 6f72 7420 6f62 6a0a 2020 2020 2020   port obj.      
-00002970: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00002980: 793a 0a20 2020 2020 2020 2020 2020 2063  y:.            c
-00002990: 6f6d 5f70 6f72 745f 6f62 6a20 3d20 7365  om_port_obj = se
-000029a0: 6c66 2e63 6f6d 5f70 6f72 745f 6f62 6a20  lf.com_port_obj 
-000029b0: 3d20 7365 7269 616c 2e53 6572 6961 6c28  = serial.Serial(
-000029c0: 706f 7274 3d70 6f72 742c 2062 6175 6472  port=port, baudr
-000029d0: 6174 653d 3936 3030 2c20 7469 6d65 6f75  ate=9600, timeou
-000029e0: 743d 3129 0a20 2020 2020 2020 2020 2020  t=1).           
-000029f0: 2069 6620 636f 6d5f 706f 7274 5f6f 626a   if com_port_obj
-00002a00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002a20: 6c66 2e64 6f6f 725f 636d 6420 3d20 4e6f  lf.door_cmd = No
-00002a30: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00002a40: 2020 2073 656c 662e 636f 6d5f 706f 7274     self.com_port
-00002a50: 5f6f 626a 2e77 7269 7465 2862 274d 4f44  _obj.write(b'MOD
-00002a60: 454c 3f5c 7227 290a 2020 2020 2020 2020  EL?\r').        
-00002a70: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00002a80: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00002a90: 2020 206d 6f64 656c 203d 2073 7472 2873     model = str(s
-00002aa0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00002ab0: 2e72 6561 6428 3134 2929 0a20 2020 2020  .read(14)).     
-00002ac0: 2020 2020 2020 2020 2020 2070 6172 7473             parts
-00002ad0: 203d 205b 7020 666f 7220 7020 696e 206d   = [p for p in m
-00002ae0: 6f64 656c 2e73 706c 6974 2822 2722 295d  odel.split("'")]
-00002af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b00: 2070 6172 7473 203d 205b 7020 666f 7220   parts = [p for 
-00002b10: 7020 696e 2070 6172 7473 5b31 5d2e 7370  p in parts[1].sp
-00002b20: 6c69 7428 2220 2229 5d0a 2020 2020 2020  lit(" ")].      
-00002b30: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00002b40: 6f64 656c 203d 2070 6172 7473 5b30 5d0a  odel = parts[0].
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 6966 206c 656e 2873 656c 662e 6d6f 6465  if len(self.mode
-00002b70: 6c29 203e 2030 3a0a 2020 2020 2020 2020  l) > 0:.        
-00002b80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002b90: 7428 2252 4620 6368 616d 6265 7220 636f  t("RF chamber co
-00002ba0: 6e6e 6563 7465 6420 746f 2070 6f72 7420  nnected to port 
-00002bb0: 2220 2b20 7374 7228 706f 7274 2929 0a20  " + str(port)). 
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2070 7269 6e74 2822 5465 7363 6f6d     print("Tescom
-00002be0: 202d 2043 6861 6d62 6572 206d 6f64 656c   - Chamber model
-00002bf0: 3a22 2c20 7365 6c66 2e6d 6f64 656c 290a  :", self.model).
+00000fc0: 650a 696d 706f 7274 206f 730a 0a0a 636c  e.import os...cl
+00000fd0: 6173 7320 4571 7569 706d 656e 7445 7272  ass EquipmentErr
+00000fe0: 6f72 2845 7863 6570 7469 6f6e 293a 0a0a  or(Exception):..
+00000ff0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001000: 2873 656c 662c 202a 6172 6773 293a 0a20  (self, *args):. 
+00001010: 2020 2020 2020 2069 6620 6172 6773 3a0a         if args:.
+00001020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001030: 2e6d 6573 7361 6765 203d 2061 7267 735b  .message = args[
+00001040: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
+00001050: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001060: 662e 6d65 7373 6167 6520 3d20 4e6f 6e65  f.message = None
+00001070: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00001080: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00001090: 2023 2070 7269 6e74 2827 6361 6c6c 696e   # print('callin
+000010a0: 6720 7374 7227 290a 2020 2020 2020 2020  g str').        
+000010b0: 6966 2073 656c 662e 6d65 7373 6167 653a  if self.message:
+000010c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000010d0: 7572 6e20 2745 7175 6970 6d65 6e74 4572  urn 'EquipmentEr
+000010e0: 726f 723a 207b 6d73 677d 272e 666f 726d  ror: {msg}'.form
+000010f0: 6174 286d 7367 3d73 656c 662e 6d65 7373  at(msg=self.mess
+00001100: 6167 6529 0a20 2020 2020 2020 2065 6c73  age).        els
+00001110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00001120: 6574 7572 6e20 2745 7175 6970 6d65 6e74  eturn 'Equipment
+00001130: 4572 726f 7220 6861 7320 6265 656e 2072  Error has been r
+00001140: 6169 7365 6427 0a0a 0a64 6566 2073 6572  aised'...def ser
+00001150: 6961 6c5f 706f 7274 7328 293a 0a20 2020  ial_ports():.   
+00001160: 2022 2222 204c 6973 7473 2073 6572 6961   """ Lists seria
+00001170: 6c20 706f 7274 206e 616d 6573 0a0a 2020  l port names..  
+00001180: 2020 2020 2020 3a72 6169 7365 7320 456e        :raises En
+00001190: 7669 726f 6e6d 656e 7445 7272 6f72 3a0a  vironmentError:.
+000011a0: 2020 2020 2020 2020 2020 2020 4f6e 2075              On u
+000011b0: 6e73 7570 706f 7274 6564 206f 7220 756e  nsupported or un
+000011c0: 6b6e 6f77 6e20 706c 6174 666f 726d 730a  known platforms.
+000011d0: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+000011e0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
+000011f0: 6c69 7374 206f 6620 7468 6520 7365 7269  list of the seri
+00001200: 616c 2070 6f72 7473 2061 7661 696c 6162  al ports availab
+00001210: 6c65 206f 6e20 7468 6520 7379 7374 656d  le on the system
+00001220: 0a20 2020 2022 2222 0a20 2020 2061 7661  .    """.    ava
+00001230: 696c 6162 6c65 5f70 6f72 7473 203d 205b  ilable_ports = [
+00001240: 732e 6465 7669 6365 2066 6f72 2073 2069  s.device for s i
+00001250: 6e20 7365 7269 616c 2e74 6f6f 6c73 2e6c  n serial.tools.l
+00001260: 6973 745f 706f 7274 732e 636f 6d70 6f72  ist_ports.compor
+00001270: 7473 2829 5d0a 2020 2020 6966 206c 656e  ts()].    if len
+00001280: 2861 7661 696c 6162 6c65 5f70 6f72 7473  (available_ports
+00001290: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+000012a0: 6176 6169 6c61 626c 655f 706f 7274 7320  available_ports 
+000012b0: 3d20 5b73 2e6e 616d 6520 666f 7220 7320  = [s.name for s 
+000012c0: 696e 2073 6572 6961 6c2e 746f 6f6c 732e  in serial.tools.
+000012d0: 6c69 7374 5f70 6f72 7473 2e63 6f6d 706f  list_ports.compo
+000012e0: 7274 7328 295d 0a20 2020 2020 2020 2069  rts()].        i
+000012f0: 6620 6c65 6e28 6176 6169 6c61 626c 655f  f len(available_
+00001300: 706f 7274 7329 203d 3d20 303a 0a20 2020  ports) == 0:.   
+00001310: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00001320: 6e6f 2073 6572 6961 6c20 706f 7274 7320  no serial ports 
+00001330: 7765 7265 2066 6f75 6e64 2e20 706c 6561  were found. plea
+00001340: 7365 2063 6865 636b 2079 6f75 7220 636f  se check your co
+00001350: 6e6e 6563 7469 6f6e 7322 290a 2020 2020  nnections").    
+00001360: 7265 7475 726e 2061 7661 696c 6162 6c65  return available
+00001370: 5f70 6f72 7473 0a0a 0a63 6c61 7373 2041  _ports...class A
+00001380: 7474 656e 7561 746f 7228 6f62 6a65 6374  ttenuator(object
+00001390: 293a 0a20 2020 2027 2727 0a20 2020 2053  ):.    '''.    S
+000013a0: 7570 706f 7274 2061 6c6c 2061 7474 6e20  upport all attn 
+000013b0: 636c 6173 7365 7320 666f 723a 0a20 2020  classes for:.   
+000013c0: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
+000013d0: 696e 6974 5f5f 2873 656c 662c 2041 5454  init__(self, ATT
+000013e0: 4e5f 7479 7065 2c20 636f 6d70 6f72 743d  N_type, comport=
+000013f0: 2741 5554 4f27 293a 0a20 2020 2020 2020  'AUTO'):.       
+00001400: 2069 6620 274d 4344 492d 5553 4227 2069   if 'MCDI-USB' i
+00001410: 6e20 4154 544e 5f74 7970 653a 0a20 2020  n ATTN_type:.   
+00001420: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00001430: 6374 6976 655f 5445 203d 2041 7474 656e  ctive_TE = Atten
+00001440: 7561 746f 722e 4d43 4449 5f55 5342 2829  uator.MCDI_USB()
+00001450: 0a20 2020 2020 2020 2065 6c69 6620 274d  .        elif 'M
+00001460: 4344 4927 2069 6e20 4154 544e 5f74 7970  CDI' in ATTN_typ
+00001470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001480: 656c 662e 5f61 6374 6976 655f 5445 203d  elf._active_TE =
+00001490: 2041 7474 656e 7561 746f 722e 4d43 4449   Attenuator.MCDI
+000014a0: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+000014b0: 2741 5049 2720 696e 2041 5454 4e5f 7479  'API' in ATTN_ty
+000014c0: 7065 206f 7220 2757 6569 6e73 6368 656c  pe or 'Weinschel
+000014d0: 2720 696e 2041 5454 4e5f 7479 7065 3a0a  ' in ATTN_type:.
+000014e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000014f0: 2e5f 6163 7469 7665 5f54 4520 3d20 4174  ._active_TE = At
+00001500: 7465 6e75 6174 6f72 2e41 5049 2863 6f6d  tenuator.API(com
+00001510: 706f 7274 290a 0a20 2020 2020 2020 2065  port)..        e
+00001520: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001530: 2070 6173 730a 0a20 2020 2064 6566 2047   pass..    def G
+00001540: 6574 4163 7469 7665 5445 2873 656c 6629  etActiveTE(self)
+00001550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001560: 2073 656c 662e 5f61 6374 6976 655f 5445   self._active_TE
+00001570: 0a0a 2020 2020 636c 6173 7320 4d43 4449  ..    class MCDI
+00001580: 286f 626a 6563 7429 3a0a 0a20 2020 2020  (object):..     
+00001590: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000015a0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+000015b0: 2020 2064 6f74 6e65 7420 3d20 4661 6c73     dotnet = Fals
+000015c0: 650a 2020 2020 2020 2020 2020 2020 7574  e.            ut
+000015d0: 696c 735f 6469 7220 3d20 6f73 2e70 6174  ils_dir = os.pat
+000015e0: 682e 6a6f 696e 286f 732e 7061 7468 2e64  h.join(os.path.d
+000015f0: 6972 6e61 6d65 285f 5f66 696c 655f 5f29  irname(__file__)
+00001600: 2c20 2775 7469 6c73 2729 0a20 2020 2020  , 'utils').     
+00001610: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
+00001620: 6170 7065 6e64 2875 7469 6c73 5f64 6972  append(utils_dir
+00001630: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001640: 2064 6f74 6e65 7420 3d3d 2054 7275 653a   dotnet == True:
+00001650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001660: 2069 6d70 6f72 7420 636c 7220 2023 2070   import clr  # p
+00001670: 7974 686f 6e6e 6574 2c20 6d61 6e75 616c  ythonnet, manual
+00001680: 6c79 2069 6e73 7461 6c6c 6564 2077 6974  ly installed wit
+00001690: 6820 6120 646f 776e 6c6f 6164 6564 2077  h a downloaded w
+000016a0: 6865 656c 2061 6e64 2070 6970 0a20 2020  heel and pip.   
+000016b0: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
+000016c0: 6f72 7420 6374 7970 6573 2020 2320 6d6f  ort ctypes  # mo
+000016d0: 6475 6c65 2074 6f20 6f70 656e 2075 7469  dule to open uti
+000016e0: 6c73 2066 696c 6573 0a20 2020 2020 2020  ls files.       
+000016f0: 2020 2020 2020 2020 2063 6c72 2e41 6464           clr.Add
+00001700: 5265 6665 7265 6e63 6528 2253 7973 7465  Reference("Syste
+00001710: 6d2e 494f 2229 0a20 2020 2020 2020 2020  m.IO").         
+00001720: 2020 2020 2020 2069 6d70 6f72 7420 5379         import Sy
+00001730: 7374 656d 2e49 4f0a 2020 2020 2020 2020  stem.IO.        
+00001740: 2020 2020 2020 2020 5379 7374 656d 2e49          System.I
+00001750: 4f2e 4469 7265 6374 6f72 792e 5365 7443  O.Directory.SetC
+00001760: 7572 7265 6e74 4469 7265 6374 6f72 7928  urrentDirectory(
+00001770: 7574 696c 735f 6469 7229 0a20 2020 2020  utils_dir).     
+00001780: 2020 2020 2020 2020 2020 2063 6c72 2e41             clr.A
+00001790: 6464 5265 6665 7265 6e63 6528 276d 636c  ddReference('mcl
+000017a0: 5f52 5544 4154 5f4e 4554 3435 2729 0a20  _RUDAT_NET45'). 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000017c0: 726f 6d20 6d63 6c5f 5255 4441 545f 4e45  rom mcl_RUDAT_NE
+000017d0: 5434 3520 696d 706f 7274 2055 5342 5f52  T45 import USB_R
+000017e0: 5544 4154 0a20 2020 2020 2020 2020 2020  UDAT.           
+000017f0: 2020 2020 2073 656c 662e 4465 7669 6365       self.Device
+00001800: 203d 2055 5342 5f52 5544 4154 2829 0a20   = USB_RUDAT(). 
+00001810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001820: 656c 662e 4465 7669 6365 2e43 6f6e 6e65  elf.Device.Conne
+00001830: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00001840: 2020 2020 2069 6e66 6f20 3d20 7365 6c66       info = self
+00001850: 2e44 6576 6963 6549 6e66 6f28 290a 2020  .DeviceInfo().  
+00001860: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001870: 696e 7428 2746 6f75 6e64 2041 7474 656e  int('Found Atten
+00001880: 7561 746f 723a 204d 6f64 656c 207b 7d2c  uator: Model {},
+00001890: 207b 7d20 2c7b 7d20 272e 666f 726d 6174   {} ,{} '.format
+000018a0: 2869 6e66 6f5b 305d 2c20 696e 666f 5b31  (info[0], info[1
+000018b0: 5d2c 2069 6e66 6f5b 325d 2929 0a20 2020  ], info[2])).   
+000018c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000018e0: 726f 6d20 5553 425f 5255 4441 5420 696d  rom USB_RUDAT im
+000018f0: 706f 7274 2055 5342 4441 540a 2020 2020  port USBDAT.    
+00001900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001910: 2e44 6576 6963 6520 3d20 5553 4244 4154  .Device = USBDAT
+00001920: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00001930: 2020 2069 6e66 6f20 3d20 7365 6c66 2e44     info = self.D
+00001940: 6576 6963 6549 6e66 6f28 290a 2020 2020  eviceInfo().    
+00001950: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001960: 7428 2746 6f75 6e64 2041 7474 656e 7561  t('Found Attenua
+00001970: 746f 723a 204d 6f64 656c 207b 7d2c 207b  tor: Model {}, {
+00001980: 7d20 2c7b 7d20 272e 666f 726d 6174 2869  } ,{} '.format(i
+00001990: 6e66 6f5b 305d 2c20 696e 666f 5b31 5d2c  nfo[0], info[1],
+000019a0: 2069 6e66 6f5b 325d 2929 0a0a 2020 2020   info[2]))..    
+000019b0: 2020 2020 6465 6620 4465 7669 6365 496e      def DeviceIn
+000019c0: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
+000019d0: 2020 2020 2020 636d 6420 3d20 223a 4d4e        cmd = ":MN
+000019e0: 3f22 0a20 2020 2020 2020 2020 2020 206d  ?".            m
+000019f0: 6f64 656c 5f6e 616d 6520 3d20 7365 6c66  odel_name = self
+00001a00: 2e44 6576 6963 652e 5365 6e64 5f53 4350  .Device.Send_SCP
+00001a10: 4928 636d 642c 2022 2229 0a20 2020 2020  I(cmd, "").     
+00001a20: 2020 2020 2020 2063 6d64 203d 2022 3a53         cmd = ":S
+00001a30: 4e3f 220a 2020 2020 2020 2020 2020 2020  N?".            
+00001a40: 7365 7269 616c 203d 2073 656c 662e 4465  serial = self.De
+00001a50: 7669 6365 2e53 656e 645f 5343 5049 2863  vice.Send_SCPI(c
+00001a60: 6d64 2c20 2222 290a 2020 2020 2020 2020  md, "").        
+00001a70: 2020 2020 636d 6420 3d20 223a 4649 524d      cmd = ":FIRM
+00001a80: 5741 5245 3f22 0a20 2020 2020 2020 2020  WARE?".         
+00001a90: 2020 2066 7720 3d20 7365 6c66 2e44 6576     fw = self.Dev
+00001aa0: 6963 652e 5365 6e64 5f53 4350 4928 636d  ice.Send_SCPI(cm
+00001ab0: 642c 2022 2229 0a20 2020 2020 2020 2020  d, "").         
+00001ac0: 2020 2023 2072 6574 7572 6e20 5b6d 6f64     # return [mod
+00001ad0: 656c 5f6e 616d 655b 315d 2c20 7365 7269  el_name[1], seri
+00001ae0: 616c 5b31 5d2c 2066 775b 315d 5d20 2023  al[1], fw[1]]  #
+00001af0: 646f 746e 6574 0a20 2020 2020 2020 2020  dotnet.         
+00001b00: 2020 2072 6574 7572 6e20 5b6d 6f64 656c     return [model
+00001b10: 5f6e 616d 652c 2073 6572 6961 6c2c 2066  _name, serial, f
+00001b20: 775d 0a0a 2020 2020 2020 2020 6465 6620  w]..        def 
+00001b30: 5365 7461 7474 6e28 7365 6c66 2c20 6174  Setattn(self, at
+00001b40: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00001b50: 2063 6d64 203d 2022 3a53 4554 4154 543a   cmd = ":SETATT:
+00001b60: 2220 2b20 7374 7228 6174 746e 290a 2020  " + str(attn).  
+00001b70: 2020 2020 2020 2020 2020 7374 6174 7573            status
+00001b80: 203d 2069 6e74 2873 656c 662e 4465 7669   = int(self.Devi
+00001b90: 6365 2e53 656e 645f 5343 5049 2863 6d64  ce.Send_SCPI(cmd
+00001ba0: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
+00001bb0: 2020 2069 6620 7374 6174 7573 203d 3d20     if status == 
+00001bc0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00001bd0: 2020 2070 7269 6e74 2827 436f 6d6d 616e     print('Comman
+00001be0: 6420 6661 696c 6564 206f 7220 696e 7661  d failed or inva
+00001bf0: 6c69 6420 6174 7465 6e75 6174 696f 6e20  lid attenuation 
+00001c00: 7365 7427 290a 2020 2020 2020 2020 2020  set').          
+00001c10: 2020 656c 6966 2073 7461 7475 7320 3d3d    elif status ==
+00001c20: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00001c30: 2020 2020 2320 7072 696e 7428 2743 6f6d      # print('Com
+00001c40: 6d61 6e64 2063 6f6d 706c 6574 6564 2073  mand completed s
+00001c50: 7563 6365 7373 6675 6c6c 7927 290a 2020  uccessfully').  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001c70: 696e 7428 2741 7474 656e 7561 7469 6f6e  int('Attenuation
+00001c80: 2073 6574 2074 6f20 207b 7d5b 6442 5d27   set to  {}[dB]'
+00001c90: 2e66 6f72 6d61 7428 666c 6f61 7428 7365  .format(float(se
+00001ca0: 6c66 2e47 6574 6174 746e 2829 2929 290a  lf.Getattn()))).
+00001cb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00001cc0: 2073 7461 7475 7320 3d3d 2032 3a0a 2020   status == 2:.  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001ce0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+00001cf0: 2020 2020 2020 2020 2027 5265 7175 6573           'Reques
+00001d00: 7465 6420 6174 7465 6e75 6174 696f 6e20  ted attenuation 
+00001d10: 7761 7320 6869 6768 6572 2074 6861 6e20  was higher than 
+00001d20: 7468 6520 616c 6c6f 7765 6420 7261 6e67  the allowed rang
+00001d30: 652c 2074 6865 2061 7474 656e 7561 7469  e, the attenuati
+00001d40: 6f6e 2077 6173 2073 6574 2074 6f20 7468  on was set to th
+00001d50: 6520 6465 7669 6365 efbf bd73 206d 6178  e device...s max
+00001d60: 696d 756d 2061 6c6c 6f77 6564 2076 616c  imum allowed val
+00001d70: 7565 2729 0a20 2020 2020 2020 2020 2020  ue').           
+00001d80: 2023 2070 7269 6e74 2873 7461 7475 7329   # print(status)
+00001d90: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00001da0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00001db0: 2020 2020 2020 2020 2063 6d64 203d 2022           cmd = "
+00001dc0: 3a41 5454 3f22 0a20 2020 2020 2020 2020  :ATT?".         
+00001dd0: 2020 2052 6573 7020 3d20 666c 6f61 7428     Resp = float(
+00001de0: 7365 6c66 2e44 6576 6963 652e 5365 6e64  self.Device.Send
+00001df0: 5f53 4350 4928 636d 642c 2022 2229 290a  _SCPI(cmd, "")).
+00001e00: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00001e10: 696e 7428 5265 7370 290a 2020 2020 2020  int(Resp).      
+00001e20: 2020 2020 2020 2320 6966 2073 7461 7475        # if statu
+00001e30: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
+00001e40: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
+00001e50: 2743 6f6d 6d61 6e64 2066 6169 6c65 6420  'Command failed 
+00001e60: 6f72 2069 6e76 616c 6964 2061 7474 656e  or invalid atten
+00001e70: 7561 7469 6f6e 2073 6574 2729 0a20 2020  uation set').   
+00001e80: 2020 2020 2020 2020 2023 2065 6c69 6620           # elif 
+00001e90: 7374 6174 7573 203d 3d20 313a 0a20 2020  status == 1:.   
+00001ea0: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
+00001eb0: 7269 6e74 2827 436f 6d6d 616e 6420 636f  rint('Command co
+00001ec0: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
+00001ed0: 756c 6c79 2729 0a20 2020 2020 2020 2020  ully').         
+00001ee0: 2020 2072 6574 7572 6e20 5265 7370 0a0a     return Resp..
+00001ef0: 2020 2020 636c 6173 7320 4d43 4449 5f55      class MCDI_U
+00001f00: 5342 286f 626a 6563 7429 3a0a 2020 2020  SB(object):.    
+00001f10: 2020 2020 2320 3634 2062 6974 2061 7272      # 64 bit arr
+00001f20: 6179 2074 6f20 7365 6e64 2074 6f20 5553  ay to send to US
+00001f30: 420a 2020 2020 2020 2020 636d 6431 203d  B.        cmd1 =
+00001f40: 205b 302c 2030 2c20 302c 2030 2c20 302c   [0, 0, 0, 0, 0,
+00001f50: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f60: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001f70: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001f80: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f90: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fa0: 2c20 302c 2030 2c20 302c 0a20 2020 2020  , 0, 0, 0,.     
+00001fb0: 2020 2020 2020 2020 2020 2030 2c20 302c             0, 0,
+00001fc0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001fd0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fe0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001ff0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00002000: 302c 2030 2c20 302c 2030 2c20 302c 0a20  0, 0, 0, 0, 0,. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00002020: 5d20 2023 2036 3420 6269 7420 6172 7261  ]  # 64 bit arra
+00002030: 7920 746f 2073 656e 6420 746f 2055 5342  y to send to USB
+00002040: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+00002050: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00002060: 2020 2020 2020 2020 2020 2320 6669 6e64            # find
+00002070: 2074 6865 2064 6576 6963 650a 2020 2020   the device.    
+00002080: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
+00002090: 203d 2075 7362 2e63 6f72 652e 6669 6e64   = usb.core.find
+000020a0: 2869 6456 656e 646f 723d 3078 3230 6365  (idVendor=0x20ce
+000020b0: 2c20 6964 5072 6f64 7563 743d 3078 3030  , idProduct=0x00
+000020c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+000020d0: 2320 7761 7320 6974 2066 6f75 6e64 3f0a  # was it found?.
+000020e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000020f0: 656c 662e 6465 7620 6973 204e 6f6e 653a  elf.dev is None:
+00002100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002110: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002120: 7228 2744 6576 6963 6520 6e6f 7420 666f  r('Device not fo
+00002130: 756e 6427 290a 2020 2020 2020 2020 2020  und').          
+00002140: 2020 2320 7365 7420 7468 6520 6163 7469    # set the acti
+00002150: 7665 2063 6f6e 6669 6775 7261 7469 6f6e  ve configuration
+00002160: 2e20 7769 7468 206e 6f20 6172 6773 2077  . with no args w
+00002170: 6520 7573 6520 6669 7273 7420 636f 6e66  e use first conf
+00002180: 6967 2e0a 2020 2020 2020 2020 2020 2020  ig..            
+00002190: 2320 2066 6f72 204c 696e 7578 206f 6e6c  #  for Linux onl
+000021a0: 790a 2020 2020 2020 2020 2020 2020 6966  y.            if
+000021b0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+000021c0: 2027 6c69 6e75 7827 3a0a 0a20 2020 2020   'linux':..     
+000021d0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+000021e0: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
+000021f0: 7365 6c66 2e64 6576 3a0a 2020 2020 2020  self.dev:.      
+00002200: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002210: 7220 696e 7465 7266 6163 6520 696e 2063  r interface in c
+00002220: 6f6e 6669 6775 7261 7469 6f6e 3a0a 2020  onfiguration:.  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2020 2020 6966 6e75 6d20 3d20 696e        ifnum = in
+00002250: 7465 7266 6163 652e 6249 6e74 6572 6661  terface.bInterfa
+00002260: 6365 4e75 6d62 6572 0a20 2020 2020 2020  ceNumber.       
+00002270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002280: 6e6f 7420 7365 6c66 2e64 6576 2e69 735f  not self.dev.is_
+00002290: 6b65 726e 656c 5f64 7269 7665 725f 6163  kernel_driver_ac
+000022a0: 7469 7665 2869 666e 756d 293a 0a20 2020  tive(ifnum):.   
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002300: 2070 7269 6e74 2022 6465 7461 6368 206b   print "detach k
+00002310: 6572 6e65 6c20 6472 6976 6572 2066 726f  ernel driver fro
+00002320: 6d20 6465 7669 6365 2025 733a 2069 6e74  m device %s: int
+00002330: 6572 6661 6365 2025 7322 2025 2028 6465  erface %s" % (de
+00002340: 762c 2069 666e 756d 290a 2020 2020 2020  v, ifnum).      
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 7365 6c66 2e64 6576 2e64 6574 6163    self.dev.detac
+00002370: 685f 6b65 726e 656c 5f64 7269 7665 7228  h_kernel_driver(
+00002380: 6966 6e75 6d29 0a20 2020 2020 2020 2020  ifnum).         
+00002390: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000023a0: 7420 7573 622e 636f 7265 2e55 5342 4572  t usb.core.USBEr
+000023b0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000023c0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000023d0: 730a 0a20 2020 2020 2020 2020 2020 2073  s..            s
+000023e0: 656c 662e 6465 762e 7365 745f 636f 6e66  elf.dev.set_conf
+000023f0: 6967 7572 6174 696f 6e28 290a 2020 2020  iguration().    
+00002400: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
+00002410: 315b 305d 203d 2034 310a 2020 2020 2020  1[0] = 41.      
+00002420: 2020 2020 2020 7365 6c66 2e64 6576 2e77        self.dev.w
+00002430: 7269 7465 2830 7830 312c 2073 656c 662e  rite(0x01, self.
+00002440: 636d 6431 2920 2023 2053 4e0a 2020 2020  cmd1)  # SN.    
+00002450: 2020 2020 2020 2020 7320 3d20 7365 6c66          s = self
+00002460: 2e64 6576 2e72 6561 6428 3078 3831 2c20  .dev.read(0x81, 
+00002470: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
+00002480: 7365 6c66 2e53 6572 6961 6c4e 756d 6265  self.SerialNumbe
+00002490: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
+000024a0: 2020 2069 203d 2031 0a20 2020 2020 2020     i = 1.       
+000024b0: 2020 2020 2077 6869 6c65 2028 735b 695d       while (s[i]
+000024c0: 203e 2030 293a 0a20 2020 2020 2020 2020   > 0):.         
+000024d0: 2020 2020 2020 2073 656c 662e 5365 7269         self.Seri
+000024e0: 616c 4e75 6d62 6572 203d 2073 656c 662e  alNumber = self.
+000024f0: 5365 7269 616c 4e75 6d62 6572 202b 2063  SerialNumber + c
+00002500: 6872 2873 5b69 5d29 0a20 2020 2020 2020  hr(s[i]).       
+00002510: 2020 2020 2020 2020 2069 203d 2069 202b           i = i +
+00002520: 2031 0a20 2020 2020 2020 2020 2020 2073   1.            s
+00002530: 656c 662e 636d 6431 5b30 5d20 3d20 3430  elf.cmd1[0] = 40
+00002540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002550: 662e 6465 762e 7772 6974 6528 3078 3031  f.dev.write(0x01
+00002560: 2c20 7365 6c66 2e63 6d64 3129 2020 2320  , self.cmd1)  # 
+00002570: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
+00002580: 2020 7320 3d20 7365 6c66 2e64 6576 2e72    s = self.dev.r
+00002590: 6561 6428 3078 3831 2c20 3634 290a 2020  ead(0x81, 64).  
+000025a0: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
+000025b0: 6f64 656c 4e61 6d65 203d 2022 220a 2020  odelName = "".  
+000025c0: 2020 2020 2020 2020 2020 6920 3d20 310a            i = 1.
+000025d0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000025e0: 6520 2873 5b69 5d20 3e20 3029 3a0a 2020  e (s[i] > 0):.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002600: 6c66 2e4d 6f64 656c 4e61 6d65 203d 2073  lf.ModelName = s
+00002610: 656c 662e 4d6f 6465 6c4e 616d 6520 2b20  elf.ModelName + 
+00002620: 6368 7228 735b 695d 290a 2020 2020 2020  chr(s[i]).      
+00002630: 2020 2020 2020 2020 2020 6920 3d20 6920            i = i 
+00002640: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
+00002650: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002660: 746e 203d 2066 6c6f 6174 2873 656c 662e  tn = float(self.
+00002670: 4d6f 6465 6c4e 616d 655b 3131 3a5d 290a  ModelName[11:]).
+00002680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002690: 2e63 6d64 315b 305d 203d 2039 390a 2020  .cmd1[0] = 99.  
+000026a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000026b0: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+000026c0: 656c 662e 636d 6431 2920 2023 2046 570a  elf.cmd1)  # FW.
+000026d0: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
+000026e0: 7365 6c66 2e64 6576 2e72 6561 6428 3078  self.dev.read(0x
+000026f0: 3831 2c20 3634 290a 2020 2020 2020 2020  81, 64).        
+00002700: 2020 2020 7365 6c66 2e46 5720 3d20 2222      self.FW = ""
+00002710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002720: 662e 4657 203d 2063 6872 2873 5b35 5d29  f.FW = chr(s[5])
+00002730: 202b 2063 6872 2873 5b36 5d29 0a20 2020   + chr(s[6]).   
+00002740: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00002750: 6174 7573 5f6d 6573 7361 6765 203d 2027  atus_message = '
+00002760: 466f 756e 6420 4174 7465 6e75 6174 6f72  Found Attenuator
+00002770: 3a20 4d6f 6465 6c20 7b7d 2c20 534e 3a20  : Model {}, SN: 
+00002780: 7b7d 202c 2046 573a 207b 7d2c 204d 6178  {} , FW: {}, Max
+00002790: 696d 756d 2061 7474 656e 7561 7469 6f6e  imum attenuation
+000027a0: 3a20 7b7d 6442 2027 2e66 6f72 6d61 7428  : {}dB '.format(
+000027b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027c0: 2073 7472 2873 656c 662e 4d6f 6465 6c4e   str(self.ModelN
+000027d0: 616d 6529 2c20 7374 7228 7365 6c66 2e53  ame), str(self.S
+000027e0: 6572 6961 6c4e 756d 6265 7229 2c20 7374  erialNumber), st
+000027f0: 7228 7365 6c66 2e46 5729 2c20 7374 7228  r(self.FW), str(
+00002800: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
+00002810: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+00002820: 7072 696e 7428 7365 6c66 2e73 7461 7475  print(self.statu
+00002830: 735f 6d65 7373 6167 6529 0a0a 2020 2020  s_message)..    
+00002840: 2020 2020 6465 6620 5265 6164 534e 2873      def ReadSN(s
+00002850: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00002860: 2020 7265 7475 726e 2073 7472 2873 656c    return str(sel
+00002870: 662e 5365 7269 616c 4e75 6d62 6572 290a  f.SerialNumber).
+00002880: 0a20 2020 2020 2020 2064 6566 2052 6561  .        def Rea
+00002890: 644d 4e28 7365 6c66 293a 0a20 2020 2020  dMN(self):.     
+000028a0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000028b0: 7228 7365 6c66 2e4d 6f64 656c 4e61 6d65  r(self.ModelName
+000028c0: 290a 0a20 2020 2020 2020 2064 6566 2052  )..        def R
+000028d0: 6561 6446 5728 7365 6c66 293a 0a20 2020  eadFW(self):.   
+000028e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000028f0: 7374 7228 7365 6c66 2e46 5729 0a0a 2020  str(self.FW)..  
+00002900: 2020 2020 2020 6465 6620 5265 6164 4d61        def ReadMa
+00002910: 7852 616e 6765 2873 656c 6629 3a0a 2020  xRange(self):.  
+00002920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002930: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002940: 746e 0a0a 2020 2020 2020 2020 6465 6620  tn..        def 
+00002950: 5365 7461 7474 6e28 7365 6c66 2c20 4174  Setattn(self, At
+00002960: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00002970: 2073 656c 662e 636d 6431 5b30 5d20 3d20   self.cmd1[0] = 
+00002980: 3139 0a20 2020 2020 2020 2020 2020 2073  19.            s
+00002990: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+000029a0: 7428 4174 746e 290a 2020 2020 2020 2020  t(Attn).        
+000029b0: 2020 2020 7365 6c66 2e63 6d64 315b 325d      self.cmd1[2]
+000029c0: 203d 2069 6e74 2828 4174 746e 202d 2069   = int((Attn - i
+000029d0: 6e74 2841 7474 6e29 2920 2a20 3429 0a20  nt(Attn)) * 4). 
+000029e0: 2020 2020 2020 2020 2020 2069 6620 4174             if At
+000029f0: 746e 203e 2073 656c 662e 4d61 7869 6d75  tn > self.Maximu
+00002a00: 6d5f 4174 746e 3a0a 2020 2020 2020 2020  m_Attn:.        
+00002a10: 2020 2020 2020 2020 7072 696e 7428 2741          print('A
+00002a20: 7474 656e 7561 7469 6f6e 206e 6f74 2069  ttenuation not i
+00002a30: 6e20 5261 6e67 652c 7365 7474 696e 6720  n Range,setting 
+00002a40: 6d61 7869 6d75 6d20 3d20 7b7d 2027 2e66  maximum = {} '.f
+00002a50: 6f72 6d61 7428 7374 7228 7365 6c66 2e4d  ormat(str(self.M
+00002a60: 6178 696d 756d 5f41 7474 6e29 2929 0a20  aximum_Attn))). 
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002a80: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+00002a90: 7428 7365 6c66 2e4d 6178 696d 756d 5f41  t(self.Maximum_A
+00002aa0: 7474 6e29 0a20 2020 2020 2020 2020 2020  ttn).           
+00002ab0: 2020 2020 2073 656c 662e 636d 6431 5b32       self.cmd1[2
+00002ac0: 5d20 3d20 696e 7428 2873 656c 662e 4d61  ] = int((self.Ma
+00002ad0: 7869 6d75 6d5f 4174 746e 202d 2069 6e74  ximum_Attn - int
+00002ae0: 2873 656c 662e 4d61 7869 6d75 6d5f 4174  (self.Maximum_At
+00002af0: 746e 2929 202a 2034 290a 2020 2020 2020  tn)) * 4).      
+00002b00: 2020 2020 2020 2320 7365 6c66 2e64 6576        # self.dev
+00002b10: 2e73 6574 5f63 6f6e 6669 6775 7261 7469  .set_configurati
+00002b20: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
+00002b30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002b40: 2020 2020 2020 2073 656c 662e 6465 762e         self.dev.
+00002b50: 7772 6974 6528 3078 3031 2c20 7365 6c66  write(0x01, self
+00002b60: 2e63 6d64 3129 2020 2320 5365 7420 6174  .cmd1)  # Set at
+00002b70: 7465 6e75 6174 696f 6e0a 2020 2020 2020  tenuation.      
+00002b80: 2020 2020 2020 2020 2020 7320 3d20 7365            s = se
+00002b90: 6c66 2e64 6576 2e72 6561 6428 3078 3831  lf.dev.read(0x81
+00002ba0: 2c20 3634 290a 2020 2020 2020 2020 2020  , 64).          
+00002bb0: 2020 2020 2020 7365 6c66 2e6e 6577 5f61        self.new_a
+00002bc0: 7474 203d 2027 5365 7474 696e 6720 4174  tt = 'Setting At
+00002bd0: 7465 6e75 6174 696f 6e20 3d20 7b7d 6442  tenuation = {}dB
+00002be0: 2027 2e66 6f72 6d61 7428 7374 7228 735b   '.format(str(s[
+00002bf0: 315d 202b 2073 5b32 5d20 2f20 3429 290a  1] + s[2] / 4)).
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00002c20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00002c30: 2254 6573 636f 6d20 2d20 4572 726f 7221  "Tescom - Error!
-00002c40: 204e 6f20 6368 616d 6265 7220 666f 756e   No chamber foun
-00002c50: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-00002c60: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002c80: 6620 7365 6c66 2e6d 6f64 656c 2069 6e20  f self.model in 
-00002c90: 7365 6c66 2e6d 6f64 656c 735f 6c69 7374  self.models_list
-00002ca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002cb0: 2020 2020 2020 7365 6c66 2e64 6f6f 725f        self.door_
-00002cc0: 636d 6420 3d20 6227 444f 4f52 3f5c 7227  cmd = b'DOOR?\r'
-00002cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ce0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002d00: 646f 6f72 5f63 6d64 203d 2062 274c 4944  door_cmd = b'LID
-00002d10: 3f5c 7227 0a20 2020 2020 2020 2020 2020  ?\r'.           
-00002d20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002d30: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-00002d40: 6570 7469 6f6e 0a20 2020 2020 2020 2065  eption.        e
-00002d50: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00002d60: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00002d70: 2020 2320 7072 696e 7428 6529 0a20 2020    # print(e).   
-00002d80: 2020 2020 2020 2020 2070 7269 6e74 2828           print((
-00002d90: 2254 6573 636f 6d20 2d20 436f 756c 6420  "Tescom - Could 
-00002da0: 6e6f 7420 636f 6e6e 6563 7420 746f 2070  not connect to p
-00002db0: 6f72 7420 2220 2b20 706f 7274 2929 0a20  ort " + port)). 
-00002dc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002dd0: 6e20 4e6f 6e65 0a20 2020 200a 2020 2020  n None.    .    
-00002de0: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
-00002df0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00002e00: 220a 2020 2020 2020 2020 636c 6f73 6573  ".        closes
-00002e10: 2063 6f6d 2070 6f72 740a 2020 2020 2020   com port.      
-00002e20: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00002e30: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00002e40: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00002e50: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00002e60: 2020 2020 2070 7269 6e74 2822 5246 2063       print("RF c
-00002e70: 6861 6d62 6572 2064 6973 636f 6e6e 6563  hamber disconnec
-00002e80: 7465 6420 6672 6f6d 2070 6f72 743a 2022  ted from port: "
-00002e90: 202b 2073 7472 2873 656c 662e 706f 7274   + str(self.port
-00002ea0: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
-00002eb0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00002ec0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00002ed0: 696e 7428 2243 6f75 6c64 206e 6f74 2064  int("Could not d
-00002ee0: 6973 636f 6e6e 6563 7422 290a 2020 2020  isconnect").    
-00002ef0: 0a20 2020 2064 6566 206f 7065 6e5f 6368  .    def open_ch
-00002f00: 616d 6265 7228 7365 6c66 293a 0a20 2020  amber(self):.   
-00002f10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002f20: 206f 7065 6e73 2063 6861 6d62 6572 0a20   opens chamber. 
-00002f30: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00002f40: 224f 4b22 2069 6620 636f 6d6d 616e 6420  "OK" if command 
-00002f50: 7761 7320 7375 6363 6573 7366 756c 0a20  was successful. 
-00002f60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002f70: 2020 2069 6620 7365 6c66 2e69 735f 646f     if self.is_do
-00002f80: 6f72 5f6f 7065 6e28 293a 0a20 2020 2020  or_open():.     
-00002f90: 2020 2020 2020 2070 7269 6e74 2822 4368         print("Ch
-00002fa0: 616d 6265 7220 6973 206f 7065 6e22 290a  amber is open").
-00002fb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002fc0: 726e 2027 4f4b 270a 2020 2020 2020 2020  rn 'OK'.        
-00002fd0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00002fe0: 2070 7269 6e74 2866 2243 6861 6d62 6572   print(f"Chamber
-00002ff0: 207b 7365 6c66 2e70 6f72 747d 2069 7320   {self.port} is 
-00003000: 6f70 656e 696e 6722 290a 2020 2020 2020  opening").      
-00003010: 2020 2020 2020 7365 6c66 2e63 6f6d 5f70        self.com_p
-00003020: 6f72 745f 6f62 6a2e 7265 7365 745f 696e  ort_obj.reset_in
-00003030: 7075 745f 6275 6666 6572 2829 0a20 2020  put_buffer().   
-00003040: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00003050: 6d5f 706f 7274 5f6f 626a 2e72 6573 6574  m_port_obj.reset
-00003060: 5f6f 7574 7075 745f 6275 6666 6572 2829  _output_buffer()
-00003070: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003080: 662e 636f 6d5f 706f 7274 5f6f 626a 2e77  f.com_port_obj.w
-00003090: 7269 7465 2873 656c 662e 6f70 656e 5f63  rite(self.open_c
-000030a0: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-000030b0: 7265 7320 3d20 2727 0a20 2020 2020 2020  res = ''.       
-000030c0: 2020 2020 2077 6169 745f 636f 756e 7465       wait_counte
-000030d0: 7220 3d20 300a 2020 2020 2020 2020 2020  r = 0.          
-000030e0: 2020 7768 696c 6520 274f 4b27 206e 6f74    while 'OK' not
-000030f0: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
-00003100: 2020 2020 2020 2020 2069 6620 7761 6974           if wait
-00003110: 5f63 6f75 6e74 6572 203e 3d20 3135 3a0a  _counter >= 15:.
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-00003140: 696f 6e28 6622 4572 726f 7220 696e 206f  ion(f"Error in o
-00003150: 7065 6e69 6e67 2063 6861 6d62 6572 207b  pening chamber {
-00003160: 7365 6c66 2e70 6f72 747d 2229 0a20 2020  self.port}").   
-00003170: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00003180: 203d 2073 656c 662e 636f 6d5f 706f 7274   = self.com_port
-00003190: 5f6f 626a 2e72 6561 6428 3134 292e 6465  _obj.read(14).de
-000031a0: 636f 6465 280a 2020 2020 2020 2020 2020  code(.          
-000031b0: 2020 2020 2020 2020 2020 2775 7466 2d38            'utf-8
-000031c0: 2729 2e75 7070 6572 2829 2e72 7374 7269  ').upper().rstri
-000031d0: 7028 275c 7227 290a 2020 2020 2020 2020  p('\r').        
-000031e0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-000031f0: 7472 2872 6573 2929 203e 2030 3a0a 2020  tr(res)) > 0:.  
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 7072 696e 7428 6627 4368 616d 6265    print(f'Chambe
-00003220: 7220 7b73 656c 662e 706f 7274 7d20 7374  r {self.port} st
-00003230: 6174 7573 3a20 2720 2b20 7374 7228 7265  atus: ' + str(re
-00003240: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
-00003250: 2020 2020 7761 6974 5f63 6f75 6e74 6572      wait_counter
-00003260: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00003270: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00003280: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003290: 6e6f 7420 7365 6c66 2e69 735f 646f 6f72  not self.is_door
-000032a0: 5f6f 7065 6e28 293a 0a20 2020 2020 2020  _open():.       
-000032b0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-000032c0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
-000032d0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000032e0: 7b73 656c 662e 706f 7274 7d20 446f 6f72  {self.port} Door
-000032f0: 2073 7461 7475 7320 646f 6573 6e27 7420   status doesn't 
-00003300: 6d61 7463 6820 636f 6d6d 616e 6420 7365  match command se
-00003310: 6e74 2122 290a 2020 2020 2020 2020 2020  nt!").          
-00003320: 2020 7072 696e 7428 6622 4368 616d 6265    print(f"Chambe
-00003330: 7220 7b73 656c 662e 706f 7274 7d20 6973  r {self.port} is
-00003340: 206f 7065 6e22 290a 2020 2020 2020 2020   open").        
-00003350: 2020 2020 7265 7475 726e 2027 4f4b 270a      return 'OK'.
-00003360: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00003370: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
-00003380: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003390: 2865 290a 2020 2020 2020 2020 2020 2020  (e).            
-000033a0: 7265 7475 726e 2022 4641 494c 220a 2020  return "FAIL".  
-000033b0: 2020 0a20 2020 2064 6566 2063 6c6f 7365    .    def close
-000033c0: 5f63 6861 6d62 6572 2873 656c 6629 3a0a  _chamber(self):.
-000033d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000033e0: 2020 2020 636c 6f73 6573 2063 6861 6d62      closes chamb
-000033f0: 6572 0a20 2020 2020 2020 203a 7265 7475  er.        :retu
-00003400: 726e 3a20 224f 4b22 2069 6620 636f 6d6d  rn: "OK" if comm
-00003410: 616e 6420 7761 7320 7375 6363 6573 7366  and was successf
-00003420: 756c 0a20 2020 2020 2020 2022 2222 0a20  ul.        """. 
-00003430: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00003440: 735f 646f 6f72 5f63 6c6f 7365 6428 293a  s_door_closed():
-00003450: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00003460: 6e74 2822 4368 616d 6265 7220 636c 6f73  nt("Chamber clos
-00003470: 6564 2229 0a20 2020 2020 2020 2020 2020  ed").           
-00003480: 2072 6574 7572 6e20 274f 4b27 0a20 2020   return 'OK'.   
-00003490: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000034a0: 2020 2020 2020 7072 696e 7428 6622 4348        print(f"CH
-000034b0: 414d 4245 5220 7b73 656c 662e 706f 7274  AMBER {self.port
-000034c0: 7d20 4953 2043 4c4f 5349 4e47 2c20 434c  } IS CLOSING, CL
-000034d0: 4541 5220 4841 4e44 5321 2121 2229 0a20  EAR HANDS!!!"). 
-000034e0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-000034f0: 2832 290a 2020 2020 2020 2020 2020 2020  (2).            
-00003500: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
-00003510: 6a2e 7772 6974 6528 7365 6c66 2e63 6c6f  j.write(self.clo
-00003520: 7365 5f63 6d64 290a 2020 2020 2020 2020  se_cmd).        
-00003530: 2020 2020 7265 7320 3d20 2727 0a20 2020      res = ''.   
-00003540: 2020 2020 2020 2020 2077 6169 745f 636f           wait_co
-00003550: 756e 7465 7220 3d20 300a 2020 2020 2020  unter = 0.      
-00003560: 2020 2020 2020 7768 696c 6520 2752 4541        while 'REA
-00003570: 4459 2720 6e6f 7420 696e 2072 6573 3a0a  DY' not in res:.
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 6966 2077 6169 745f 636f 756e 7465 7220  if wait_counter 
-000035a0: 3e3d 2032 303a 0a20 2020 2020 2020 2020  >= 20:.         
-000035b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000035c0: 2045 7863 6570 7469 6f6e 2866 2245 7272   Exception(f"Err
-000035d0: 6f72 2069 6e20 636c 6f73 696e 6720 6368  or in closing ch
-000035e0: 616d 6265 7220 7b73 656c 662e 706f 7274  amber {self.port
-000035f0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00003600: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
-00003610: 6f6d 5f70 6f72 745f 6f62 6a2e 7265 6164  om_port_obj.read
-00003620: 2831 3429 2e64 6563 6f64 6528 0a20 2020  (14).decode(.   
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2027 7574 662d 3827 292e 7570 7065 7228   'utf-8').upper(
-00003650: 292e 7273 7472 6970 2827 5c72 2729 0a20  ).rstrip('\r'). 
-00003660: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003670: 6620 2745 5252 2720 696e 2072 6573 206f  f 'ERR' in res o
-00003680: 7220 2752 4541 4459 2720 696e 2072 6573  r 'READY' in res
-00003690: 206f 7220 274f 4b27 2069 6e20 7265 733a   or 'OK' in res:
-000036a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000036b0: 2020 2020 2070 7269 6e74 2866 2743 6861       print(f'Cha
-000036c0: 6d62 6572 207b 7365 6c66 2e70 6f72 747d  mber {self.port}
-000036d0: 2073 7461 7475 733a 2027 202b 2073 7472   status: ' + str
-000036e0: 2872 6573 2929 0a20 2020 2020 2020 2020  (res)).         
-000036f0: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
-00003700: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
-00003710: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003720: 726e 2022 4641 494c 220a 2020 2020 2020  rn "FAIL".      
-00003730: 2020 2020 2020 2020 2020 7761 6974 5f63            wait_c
-00003740: 6f75 6e74 6572 202b 3d20 310a 2020 2020  ounter += 1.    
-00003750: 2020 2020 2020 2020 2020 2020 736c 6565              slee
-00003760: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00003770: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
-00003780: 735f 646f 6f72 5f63 6c6f 7365 6428 293a  s_door_closed():
-00003790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037a0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-000037b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000037c0: 2020 2020 2020 6622 7b73 656c 662e 706f        f"{self.po
-000037d0: 7274 7d20 446f 6f72 2073 7461 7475 7320  rt} Door status 
-000037e0: 646f 6573 6e27 7420 6d61 7463 6820 636f  doesn't match co
-000037f0: 6d6d 616e 6420 7365 6e74 2122 290a 2020  mmand sent!").  
-00003800: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003810: 6622 4368 616d 6265 7220 7b73 656c 662e  f"Chamber {self.
-00003820: 706f 7274 7d20 636c 6f73 6564 2229 0a20  port} closed"). 
-00003830: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003840: 6e20 274f 4b27 0a20 2020 2020 2020 2065  n 'OK'.        e
-00003850: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00003860: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00003870: 2020 7072 696e 7428 6622 4572 726f 7220    print(f"Error 
-00003880: 696e 2063 6c6f 7369 6e67 2063 6861 6d62  in closing chamb
-00003890: 6572 207b 7365 6c66 2e70 6f72 747d 2229  er {self.port}")
-000038a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000038b0: 6e74 2865 290a 2020 2020 2020 2020 2020  nt(e).          
-000038c0: 2020 7265 7475 726e 2022 4641 494c 220a    return "FAIL".
-000038d0: 2020 2020 0a20 2020 2064 6566 2069 735f      .    def is_
-000038e0: 636f 6e6e 6563 7465 6428 7365 6c66 293a  connected(self):
-000038f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003900: 2e63 6f6d 5f70 6f72 745f 6f62 6a20 6973  .com_port_obj is
-00003910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00003920: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00003930: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003940: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00003950: 2e69 734f 7065 6e28 290a 2020 2020 0a20  .isOpen().    . 
-00003960: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
-00003970: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003980: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
-00003990: 6a2e 7265 7365 745f 696e 7075 745f 6275  j.reset_input_bu
-000039a0: 6666 6572 2829 0a20 2020 2020 2020 2073  ffer().        s
-000039b0: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
-000039c0: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
-000039d0: 6f62 6a2e 7772 6974 6528 7365 6c66 2e64  obj.write(self.d
-000039e0: 6f6f 725f 636d 6429 0a20 2020 2020 2020  oor_cmd).       
-000039f0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00003a00: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
-00003a10: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
-00003a20: 6164 2831 3429 2e64 6563 6f64 6528 2775  ad(14).decode('u
-00003a30: 7466 2d38 2729 2e75 7070 6572 2829 2e72  tf-8').upper().r
-00003a40: 7374 7269 7028 275c 7227 290a 2020 2020  strip('\r').    
-00003a50: 2020 2020 7265 7475 726e 2073 7461 7465      return state
-00003a60: 0a20 2020 200a 2020 2020 6465 6620 6973  .    .    def is
-00003a70: 5f64 6f6f 725f 6f70 656e 2873 656c 6629  _door_open(self)
-00003a80: 3a0a 2020 2020 2020 2020 7374 6174 6520  :.        state 
-00003a90: 3d20 7365 6c66 2e67 6574 5f73 7461 7465  = self.get_state
-00003aa0: 2829 0a20 2020 2020 2020 2069 6620 274f  ().        if 'O
-00003ab0: 5045 4e27 2069 6e20 7374 6174 653a 0a20  PEN' in state:. 
-00003ac0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003ad0: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
-00003ae0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00003af0: 0a20 2020 2064 6566 2069 735f 646f 6f72  .    def is_door
-00003b00: 5f63 6c6f 7365 6428 7365 6c66 293a 0a20  _closed(self):. 
-00003b10: 2020 2020 2020 2073 7461 7465 203d 2073         state = s
-00003b20: 656c 662e 6765 745f 7374 6174 6528 290a  elf.get_state().
-00003b30: 2020 2020 2020 2020 6966 2027 434c 4f53          if 'CLOS
-00003b40: 4527 2069 6e20 7374 6174 653a 0a20 2020  E' in state:.   
-00003b50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003b60: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-00003b70: 7572 6e20 4661 6c73 650a 0a0a 636c 6173  urn False...clas
-00003b80: 7320 4261 7263 6f64 6553 6361 6e6e 6572  s BarcodeScanner
-00003b90: 286f 626a 6563 7429 3a0a 2020 2020 7072  (object):.    pr
-00003ba0: 6566 6978 203d 2027 7e01 3030 3030 4027  efix = '~.0000@'
-00003bb0: 0a20 2020 2073 7566 6669 7820 3d20 273b  .    suffix = ';
-00003bc0: 0327 0a20 2020 2063 6f6d 203d 2027 270a  .'.    com = ''.
-00003bd0: 2020 2020 7365 7269 616c 203d 204e 6f6e      serial = Non
-00003be0: 650a 2020 2020 0a20 2020 2064 6566 205f  e.    .    def _
-00003bf0: 5f69 6e69 745f 5f28 7365 6c66 2c20 636f  _init__(self, co
-00003c00: 6d3d 4e6f 6e65 2c20 6261 7564 3d31 3135  m=None, baud=115
-00003c10: 3230 302c 2063 6f6e 6669 673d 5472 7565  200, config=True
-00003c20: 2c20 6c6f 675f 7479 7065 3d27 4e4f 5f4c  , log_type='NO_L
-00003c30: 4f47 2729 3a0a 2020 2020 2020 2020 7365  OG'):.        se
-00003c40: 6c66 2e6c 6f67 5f74 7970 6520 3d20 6c6f  lf.log_type = lo
-00003c50: 675f 7479 7065 0a20 2020 2020 2020 2069  g_type.        i
-00003c60: 6620 636f 6d20 213d 204e 6f6e 653a 0a20  f com != None:. 
-00003c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003c80: 6f70 656e 5f70 6f72 7428 636f 6d2c 2062  open_port(com, b
-00003c90: 6175 643d 6261 7564 2c20 636f 6e66 6967  aud=baud, config
-00003ca0: 3d63 6f6e 6669 6729 0a20 2020 2020 2020  =config).       
-00003cb0: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
-00003cc0: 2023 2020 2020 2073 656c 662e 7365 7269   #     self.seri
-00003cd0: 616c 203d 2073 6572 203d 2053 6572 6961  al = ser = Seria
-00003ce0: 6c28 290a 2020 2020 0a20 2020 2064 6566  l().    .    def
-00003cf0: 206f 7065 6e5f 706f 7274 2873 656c 662c   open_port(self,
-00003d00: 2063 6f6d 2c20 6261 7564 3d31 3135 3230   com, baud=11520
-00003d10: 302c 2063 6f6e 6669 673d 5472 7565 293a  0, config=True):
-00003d20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003d30: 2e73 6572 6961 6c20 213d 204e 6f6e 6520  .serial != None 
-00003d40: 616e 6420 7365 6c66 2e73 6572 6961 6c2e  and self.serial.
-00003d50: 6973 5f6f 7065 6e28 293a 0a20 2020 2020  is_open():.     
-00003d60: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
-00003d70: 616c 2e63 6c6f 7365 506f 7274 2829 0a20  al.closePort(). 
-00003d80: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
-00003d90: 616c 203d 2073 6572 203d 2073 6572 6961  al = ser = seria
-00003da0: 6c2e 5365 7269 616c 2863 6f6d 2c20 6261  l.Serial(com, ba
-00003db0: 7564 2c20 7469 6d65 6f75 743d 302e 3529  ud, timeout=0.5)
-00003dc0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00003dd0: 7365 6c66 2e63 6865 636b 5f63 6f6d 5f70  self.check_com_p
-00003de0: 6f72 7428 293a 0a20 2020 2020 2020 2020  ort():.         
-00003df0: 2020 2070 7269 6e74 2866 277b 636f 6d7d     print(f'{com}
-00003e00: 2069 7320 6e6f 7420 6261 7263 6f64 6520   is not barcode 
-00003e10: 7363 616e 6e65 7227 290a 2020 2020 2020  scanner').      
-00003e20: 2020 6966 2073 6572 2021 3d20 4e6f 6e65    if ser != None
-00003e30: 2061 6e64 2073 656c 662e 6c6f 675f 7479   and self.log_ty
-00003e40: 7065 2021 3d20 274e 4f5f 4c4f 4727 3a0a  pe != 'NO_LOG':.
-00003e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003e60: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
-00003e70: 6e65 7220 287b 636f 6d7d 2920 636f 6e6e  ner ({com}) conn
-00003e80: 6563 7465 642e 2729 0a20 2020 2020 2020  ected.').       
-00003e90: 2065 6c69 6620 7365 7220 3d3d 204e 6f6e   elif ser == Non
-00003ea0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00003eb0: 7269 6e74 2866 2742 6172 636f 6465 2073  rint(f'Barcode s
-00003ec0: 6361 6e6e 6572 202d 2050 726f 626c 656d  canner - Problem
-00003ed0: 2063 6f6e 6e65 6374 696e 6720 7b63 6f6d   connecting {com
-00003ee0: 7d27 290a 2020 2020 2020 2020 7365 6c66  }').        self
-00003ef0: 2e63 6f6d 203d 2063 6f6d 0a20 2020 2020  .com = com.     
-00003f00: 2020 2073 6572 2e74 696d 6572 6f75 7420     ser.timerout 
-00003f10: 3d20 3120 2023 2072 6561 6420 7469 6d65  = 1  # read time
-00003f20: 206f 7574 0a20 2020 2020 2020 2073 6572   out.        ser
-00003f30: 2e77 7269 7465 5469 6d65 6f75 7420 3d20  .writeTimeout = 
-00003f40: 302e 3520 2023 2077 7269 7465 2074 696d  0.5  # write tim
-00003f50: 6520 6f75 742e 0a20 2020 2020 2020 2069  e out..        i
-00003f60: 6620 636f 6e66 6967 3a0a 2020 2020 2020  f config:.      
-00003f70: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
-00003f80: 6775 7265 2829 0a20 2020 200a 2020 2020  gure().    .    
-00003f90: 6465 6620 6669 6e64 5f61 6e64 5f6f 7065  def find_and_ope
-00003fa0: 6e5f 706f 7274 2873 656c 662c 2062 6175  n_port(self, bau
-00003fb0: 643d 3131 3532 3030 2c20 636f 6e66 6967  d=115200, config
-00003fc0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00003fd0: 636f 6d20 3d20 7365 6c66 2e66 696e 645f  com = self.find_
-00003fe0: 636f 6d5f 706f 7274 2862 6175 6429 0a20  com_port(baud). 
-00003ff0: 2020 2020 2020 2069 6620 636f 6d20 6973         if com is
-00004000: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004010: 2020 2020 2020 2073 656c 662e 6f70 656e         self.open
-00004020: 5f70 6f72 7428 636f 6d2c 2062 6175 642c  _port(com, baud,
-00004030: 2063 6f6e 6669 6729 0a20 2020 2020 2020   config).       
-00004040: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00004050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004060: 4661 6c73 650a 2020 2020 0a20 2020 2064  False.    .    d
-00004070: 6566 2066 696e 645f 636f 6d5f 706f 7274  ef find_com_port
-00004080: 2873 656c 662c 2062 6175 643d 3131 3532  (self, baud=1152
-00004090: 3030 293a 0a20 2020 2020 2020 2063 6f6d  00):.        com
-000040a0: 506f 7274 7320 3d20 7365 7269 616c 5f70  Ports = serial_p
-000040b0: 6f72 7473 2829 0a20 2020 2020 2020 2063  orts().        c
-000040c0: 6f6d 7320 3d20 5b5d 0a20 2020 2020 2020  oms = [].       
-000040d0: 2066 6f72 2063 6f6d 2069 6e20 636f 6d50   for com in comP
-000040e0: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
-000040f0: 2020 6966 2073 656c 662e 6368 6563 6b5f    if self.check_
-00004100: 636f 6d5f 706f 7274 2863 6f6d 2c20 6261  com_port(com, ba
-00004110: 7564 293a 0a20 2020 2020 2020 2020 2020  ud):.           
-00004120: 2020 2020 2063 6f6d 732e 6170 7065 6e64       coms.append
-00004130: 2863 6f6d 290a 2020 2020 2020 2020 2020  (com).          
-00004140: 2020 2020 2020 6966 206c 656e 2863 6f6d        if len(com
-00004150: 7329 203e 2031 3a0a 2020 2020 2020 2020  s) > 1:.        
-00004160: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004170: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00004180: 2020 2020 2020 2020 2020 2027 5761 726e             'Warn
-00004190: 696e 6720 2d20 6d6f 7265 2074 6861 6e20  ing - more than 
-000041a0: 6f6e 6520 6261 7263 6f64 6520 7363 616e  one barcode scan
-000041b0: 6e65 7220 666f 756e 642c 2075 7369 6e67  ner found, using
-000041c0: 2074 6865 2066 6972 7374 2062 6172 636f   the first barco
-000041d0: 6465 2073 6361 6e6e 6572 2e27 290a 2020  de scanner.').  
-000041e0: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
-000041f0: 6620 6c65 6e28 636f 6d73 2920 3e20 303a  f len(coms) > 0:
-00004200: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004210: 7572 6e20 636f 6d73 5b30 5d0a 2020 2020  urn coms[0].    
-00004220: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004230: 2020 2020 2020 7072 696e 7428 2745 7272        print('Err
-00004240: 6f72 202d 2063 6f75 6c64 206e 6f74 2066  or - could not f
-00004250: 696e 6420 6261 7263 6f64 6520 7363 616e  ind barcode scan
-00004260: 6e65 722e 2729 0a20 2020 2020 2020 2020  ner.').         
-00004270: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00004280: 2020 200a 2020 2020 6465 6620 6368 6563     .    def chec
-00004290: 6b5f 636f 6d5f 706f 7274 2873 656c 662c  k_com_port(self,
-000042a0: 2063 6f6d 3d4e 6f6e 652c 2062 6175 643d   com=None, baud=
-000042b0: 3131 3532 3030 293a 0a20 2020 2020 2020  115200):.       
-000042c0: 2069 735f 6261 725f 7363 616e 203d 2054   is_bar_scan = T
-000042d0: 7275 650a 2020 2020 2020 2020 636c 6f73  rue.        clos
-000042e0: 655f 706f 7274 203d 2046 616c 7365 0a20  e_port = False. 
-000042f0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00004300: 6c66 2e69 735f 6f70 656e 2829 2061 6e64  lf.is_open() and
-00004310: 2063 6f6d 2069 7320 6e6f 7420 4e6f 6e65   com is not None
-00004320: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00004330: 6f73 655f 706f 7274 203d 2054 7275 650a  ose_port = True.
-00004340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004350: 2e73 6572 6961 6c20 3d20 7365 7269 616c  .serial = serial
-00004360: 2e53 6572 6961 6c28 636f 6d2c 2062 6175  .Serial(com, bau
-00004370: 642c 2074 696d 656f 7574 3d30 2e35 290a  d, timeout=0.5).
-00004380: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
-00004390: 2073 656c 662e 6973 5f6f 7065 6e28 293a   self.is_open():
-000043a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000043b0: 6e74 2827 4261 7263 6f64 6553 6361 6e6e  nt('BarcodeScann
-000043c0: 6572 202d 2063 6865 636b 5f63 6f6d 5f70  er - check_com_p
-000043d0: 6f72 743a 204d 6973 7369 6e67 2063 6f6d  ort: Missing com
-000043e0: 2070 6f72 7427 290a 2020 2020 2020 2020   port').        
-000043f0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00004400: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00004410: 656c 662e 6d61 6e75 616c 5f63 6f6e 6669  elf.manual_confi
-00004420: 6775 7265 285b 2751 5259 5044 4e27 5d29  gure(['QRYPDN'])
-00004430: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00004440: 274e 4c53 2d4e 3127 2069 6e20 7374 7228  'NLS-N1' in str(
-00004450: 7265 7329 3a0a 2020 2020 2020 2020 2020  res):.          
-00004460: 2020 6973 5f62 6172 5f73 6361 6e20 3d20    is_bar_scan = 
-00004470: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00004480: 2063 6c6f 7365 5f70 6f72 743a 0a20 2020   close_port:.   
-00004490: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000044a0: 7269 616c 2e63 6c6f 7365 2829 0a20 2020  rial.close().   
-000044b0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000044c0: 7269 616c 203d 204e 6f6e 650a 2020 2020  rial = None.    
-000044d0: 2020 2020 0a20 2020 2020 2020 2072 6574      .        ret
-000044e0: 7572 6e20 6973 5f62 6172 5f73 6361 6e0a  urn is_bar_scan.
-000044f0: 2020 2020 0a20 2020 2064 6566 2063 6c6f      .    def clo
-00004500: 7365 5f70 6f72 7428 7365 6c66 293a 0a20  se_port(self):. 
-00004510: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00004520: 6572 6961 6c2e 6973 4f70 656e 2829 3a0a  erial.isOpen():.
-00004530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004540: 2e73 6572 6961 6c2e 636c 6f73 6528 290a  .serial.close().
-00004550: 2020 2020 0a20 2020 2064 6566 2069 735f      .    def is_
-00004560: 6f70 656e 2873 656c 6629 3a0a 2020 2020  open(self):.    
-00004570: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004580: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-00004590: 6d61 6e75 616c 5f63 6f6e 6669 6775 7265  manual_configure
-000045a0: 285b 2751 5259 5044 4e27 5d29 0a20 2020  (['QRYPDN']).   
-000045b0: 2020 2020 2020 2020 2069 6620 274e 4c53           if 'NLS
-000045c0: 2d4e 3127 2069 6e20 7374 7228 7265 7329  -N1' in str(res)
-000045d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000045e0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-000045f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004600: 2046 616c 7365 0a20 2020 2020 2020 2065   False.        e
-00004610: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-00004620: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00004630: 2020 2020 0a20 2020 2064 6566 2063 6f6e      .    def con
-00004640: 6669 6775 7265 2873 656c 662c 2069 6c6c  figure(self, ill
-00004650: 5363 6e3d 2731 272c 2061 6d6c 456e 613d  Scn='1', amlEna=
-00004660: 2730 272c 2067 7262 456e 613d 2730 272c  '0', grbEna='0',
-00004670: 2067 7262 566c 6c3d 2732 272c 2061 7473   grbVll='2', ats
-00004680: 456e 613d 2730 272c 2061 7473 4475 723d  Ena='0', atsDur=
-00004690: 2733 3630 3030 272c 2073 636e 4d6f 643d  '36000', scnMod=
-000046a0: 2730 272c 0a20 2020 2020 2020 2020 2020  '0',.           
-000046b0: 2020 2020 2020 2070 7762 456e 613d 2730         pwbEna='0
-000046c0: 2729 3a0a 2020 2020 2020 2020 2727 270a  '):.        '''.
-000046d0: 2020 2020 2020 2020 696c 6c53 636e 202d          illScn -
-000046e0: 2069 6c6c 756d 696e 6174 696f 6e3a 2020   illumination:  
-000046f0: 2020 302d 6f66 662c 2031 2d6e 6f72 6d61    0-off, 1-norma
-00004700: 6c2c 2032 2d61 6c77 6179 7320 6f6e 0a20  l, 2-always on. 
-00004710: 2020 2020 2020 2061 6d6c 456e 6120 2d20         amlEna - 
-00004720: 6169 6d69 6e67 3a20 2020 2020 2020 2020  aiming:         
-00004730: 2030 2d6f 6666 2c20 312d 6e6f 726d 616c   0-off, 1-normal
-00004740: 2c20 322d 616c 7761 7973 206f 6e0a 2020  , 2-always on.  
-00004750: 2020 2020 2020 7077 6245 6e61 202d 2070        pwbEna - p
-00004760: 6f77 6572 206f 6e20 6265 6570 2020 2020  ower on beep    
-00004770: 302d 6f66 662c 2031 2d6f 6e0a 2020 2020  0-off, 1-on.    
-00004780: 2020 2020 6772 6245 6e61 202d 2067 6f6f      grbEna - goo
-00004790: 6420 7265 6164 2062 6565 7020 2020 302d  d read beep   0-
-000047a0: 6f66 662c 2031 2d6f 6e0a 2020 2020 2020  off, 1-on.      
-000047b0: 2020 6174 7345 6e61 202d 2061 7574 6f20    atsEna - auto 
-000047c0: 736c 6565 7020 2020 2020 2020 302d 6469  sleep       0-di
-000047d0: 7361 626c 652c 2031 2d65 6e61 626c 650a  sable, 1-enable.
-000047e0: 2020 2020 2020 2020 6174 7344 7572 202d          atsDur -
-000047f0: 2073 6c65 6570 2064 7572 6174 696f 6e20   sleep duration 
-00004800: 2020 312d 3336 3030 3020 5b73 6563 5d0a    1-36000 [sec].
-00004810: 2020 2020 2020 2020 7363 6e4d 6f64 202d          scnMod -
-00004820: 2073 6361 6e20 6d6f 6465 2020 2020 2020   scan mode      
-00004830: 2020 302d 6c65 7665 6c20 6d6f 6465 2c20    0-level mode, 
-00004840: 322d 7365 6e73 6520 6d6f 6465 2c20 332d  2-sense mode, 3-
-00004850: 636f 6e74 696e 756f 7573 206d 6f64 652c  continuous mode,
-00004860: 2037 2d62 6174 6368 206d 6f64 650a 2020   7-batch mode.  
-00004870: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00004880: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00004890: 2020 2020 2070 6172 616d 7320 3d20 7b27       params = {'
-000048a0: 494c 4c53 434e 273a 2069 6c6c 5363 6e2c  ILLSCN': illScn,
-000048b0: 2027 414d 4c45 4e41 273a 2061 6d6c 456e   'AMLENA': amlEn
-000048c0: 612c 2027 4752 4245 4e41 273a 2067 7262  a, 'GRBENA': grb
-000048d0: 456e 612c 2027 4154 5345 4e41 273a 2061  Ena, 'ATSENA': a
-000048e0: 7473 456e 612c 0a20 2020 2020 2020 2020  tsEna,.         
-000048f0: 2020 2020 2020 2020 2027 4752 4256 4c4c           'GRBVLL
-00004900: 273a 2067 7262 566c 6c2c 2027 4154 5344  ': grbVll, 'ATSD
-00004910: 5552 273a 2061 7473 4475 722c 2027 5343  UR': atsDur, 'SC
-00004920: 4e4d 4f44 273a 2073 636e 4d6f 642c 2027  NMOD': scnMod, '
-00004930: 5057 4245 4e41 273a 2070 7762 456e 617d  PWBENA': pwbEna}
-00004940: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00004950: 3d20 5b6b 6579 202b 2076 616c 7565 2066  = [key + value f
-00004960: 6f72 206b 6579 2c20 7661 6c75 6520 696e  or key, value in
-00004970: 2070 6172 616d 732e 6974 656d 7328 295d   params.items()]
-00004980: 0a20 2020 2020 2020 2074 2c20 6973 5375  .        t, isSu
-00004990: 6363 6573 7320 3d20 7365 6c66 2e6d 616e  ccess = self.man
-000049a0: 7561 6c5f 636f 6e66 6967 7572 6528 7061  ual_configure(pa
-000049b0: 7261 6d73 290a 2020 2020 2020 2020 6966  rams).        if
-000049c0: 2069 7353 7563 6365 7373 2061 6e64 2073   isSuccess and s
-000049d0: 656c 662e 6c6f 675f 7479 7065 2021 3d20  elf.log_type != 
-000049e0: 274e 4f5f 4c4f 4727 3a0a 2020 2020 2020  'NO_LOG':.      
-000049f0: 2020 2020 2020 7072 696e 7428 6627 4261        print(f'Ba
-00004a00: 7263 6f64 6520 7363 616e 6e65 7220 287b  rcode scanner ({
-00004a10: 7365 6c66 2e63 6f6d 7d29 2063 6f6e 6669  self.com}) confi
-00004a20: 6775 7265 6420 7375 6363 6573 7366 756c  gured successful
-00004a30: 6c79 2e27 290a 2020 2020 2020 2020 656c  ly.').        el
-00004a40: 6966 206e 6f74 2069 7353 7563 6365 7373  if not isSuccess
-00004a50: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00004a60: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
-00004a70: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
-00004a80: 7d29 2063 6f6e 6669 6775 7261 7469 6f6e  }) configuration
-00004a90: 2066 6169 6c65 642e 2729 0a20 2020 200a   failed.').    .
-00004aa0: 2020 2020 6465 6620 7265 7374 6f72 655f      def restore_
-00004ab0: 616c 6c5f 6661 6374 6f72 795f 6465 6661  all_factory_defa
-00004ac0: 756c 7473 2873 656c 6629 3a0a 2020 2020  ults(self):.    
-00004ad0: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
-00004ae0: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00004af0: 7b27 4641 4344 4546 273a 2027 277d 0a20  {'FACDEF': ''}. 
-00004b00: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00004b10: 5b6b 6579 202b 2076 616c 7565 2066 6f72  [key + value for
-00004b20: 206b 6579 2c20 7661 6c75 6520 696e 2070   key, value in p
-00004b30: 6172 616d 732e 6974 656d 7328 295d 0a20  arams.items()]. 
-00004b40: 2020 2020 2020 2074 2c20 6973 5375 6363         t, isSucc
-00004b50: 6573 7320 3d20 7365 6c66 2e6d 616e 7561  ess = self.manua
-00004b60: 6c5f 636f 6e66 6967 7572 6528 7061 7261  l_configure(para
-00004b70: 6d73 290a 2020 2020 2020 2020 6966 2069  ms).        if i
-00004b80: 7353 7563 6365 7373 2061 6e64 2073 656c  sSuccess and sel
-00004b90: 662e 6c6f 675f 7479 7065 2021 3d20 274e  f.log_type != 'N
-00004ba0: 4f5f 4c4f 4727 3a0a 2020 2020 2020 2020  O_LOG':.        
-00004bb0: 2020 2020 7072 696e 7428 6627 4261 7263      print(f'Barc
-00004bc0: 6f64 6520 7363 616e 6e65 7220 287b 7365  ode scanner ({se
-00004bd0: 6c66 2e63 6f6d 7d29 2072 6573 746f 7265  lf.com}) restore
-00004be0: 6420 6661 6374 6f72 7920 6465 6661 756c  d factory defaul
-00004bf0: 7420 7375 6363 6573 7366 756c 6c79 2e27  t successfully.'
-00004c00: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
-00004c10: 6f74 2069 7353 7563 6365 7373 3a0a 2020  ot isSuccess:.  
-00004c20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00004c30: 6627 4261 7263 6f64 6520 7363 616e 6e65  f'Barcode scanne
-00004c40: 7220 287b 7365 6c66 2e63 6f6d 7d29 2072  r ({self.com}) r
-00004c50: 6573 746f 7265 6420 6661 6374 6f72 7920  estored factory 
-00004c60: 6465 6661 756c 7420 6661 696c 6564 2e27  default failed.'
-00004c70: 290a 2020 2020 0a20 2020 2064 6566 206d  ).    .    def m
-00004c80: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
-00004c90: 7365 6c66 2c20 7061 7261 6d73 293a 0a20  self, params):. 
-00004ca0: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
-00004cb0: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
-00004cc0: 7320 3d20 7365 6c66 2e70 7265 6669 7820  s = self.prefix 
-00004cd0: 2b20 273b 272e 6a6f 696e 2870 6172 616d  + ';'.join(param
-00004ce0: 7329 202b 2073 656c 662e 7375 6666 6978  s) + self.suffix
-00004cf0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00004d00: 7269 616c 2e66 6c75 7368 496e 7075 7428  rial.flushInput(
-00004d10: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00004d20: 6572 6961 6c2e 666c 7573 684f 7574 7075  erial.flushOutpu
-00004d30: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00004d40: 2e73 6572 6961 6c2e 7772 6974 6528 7374  .serial.write(st
-00004d50: 722e 656e 636f 6465 2863 6f6e 6669 6773  r.encode(configs
-00004d60: 2929 0a20 2020 2020 2020 2073 6c65 6570  )).        sleep
-00004d70: 2830 2e31 290a 2020 2020 2020 2020 742c  (0.1).        t,
-00004d80: 2069 7353 7563 6365 7373 203d 2073 656c   isSuccess = sel
-00004d90: 662e 7472 6967 6765 725f 7374 6f70 5f73  f.trigger_stop_s
-00004da0: 6574 7469 6e67 7328 290a 2020 2020 2020  ettings().      
-00004db0: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
-00004dc0: 2020 2020 2072 6574 7572 6e20 742c 2069       return t, i
-00004dd0: 7353 7563 6365 7373 0a20 2020 200a 2020  sSuccess.    .  
-00004de0: 2020 6465 6620 7363 616e 2873 656c 6629    def scan(self)
-00004df0: 3a0a 2020 2020 2020 2020 2320 7072 696e  :.        # prin
-00004e00: 7428 2261 6e61 6c6f 675f 7472 6967 6765  t("analog_trigge
-00004e10: 725f 7365 7474 696e 6722 290a 2020 2020  r_setting").    
-00004e20: 2020 2020 7365 6c66 2e73 6572 6961 6c2e      self.serial.
-00004e30: 7772 6974 6528 6222 5c78 3162 5c78 3331  write(b"\x1b\x31
-00004e40: 2229 0a20 2020 2020 2020 2073 6c65 6570  ").        sleep
-00004e50: 2830 2e31 290a 2020 2020 2020 2020 2320  (0.1).        # 
-00004e60: 7420 3d20 7365 722e 7265 6164 2873 6572  t = ser.read(ser
-00004e70: 2e69 6e5f 7761 6974 696e 6729 0a20 2020  .in_waiting).   
-00004e80: 2020 2020 2074 203d 2073 656c 662e 7365       t = self.se
-00004e90: 7269 616c 2e72 6561 645f 616c 6c28 290a  rial.read_all().
-00004ea0: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00004eb0: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
-00004ec0: 6e20 740a 2020 2020 0a20 2020 2064 6566  n t.    .    def
-00004ed0: 2073 6361 6e5f 616e 645f 666c 7573 6828   scan_and_flush(
-00004ee0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00004ef0: 656c 662e 7365 7269 616c 2e66 6c75 7368  elf.serial.flush
-00004f00: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00004f10: 7365 6c66 2e73 6572 6961 6c2e 666c 7573  self.serial.flus
-00004f20: 684f 7574 7075 7428 290a 2020 2020 2020  hOutput().      
-00004f30: 2020 7420 3d20 7365 6c66 2e73 6361 6e28    t = self.scan(
-00004f40: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00004f50: 6572 6961 6c2e 666c 7573 6849 6e70 7574  erial.flushInput
-00004f60: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00004f70: 7365 7269 616c 2e66 6c75 7368 4f75 7470  serial.flushOutp
-00004f80: 7574 2829 0a20 2020 2020 2020 2074 436c  ut().        tCl
-00004f90: 6561 6e20 3d20 7374 7228 7429 2e73 706c  ean = str(t).spl
-00004fa0: 6974 2827 5c5c 7827 295b 2d31 5d0a 2020  it('\\x')[-1].  
-00004fb0: 2020 2020 2020 6966 2074 436c 6561 6e2e        if tClean.
-00004fc0: 7374 6172 7473 7769 7468 2827 3036 2729  startswith('06')
-00004fd0: 3a0a 2020 2020 2020 2020 2020 2020 7443  :.            tC
-00004fe0: 6c65 616e 203d 2074 436c 6561 6e5b 323a  lean = tClean[2:
-00004ff0: 5d0a 2020 2020 2020 2020 2020 2020 7443  ].            tC
-00005000: 6c65 616e 203d 2074 436c 6561 6e2e 7374  lean = tClean.st
-00005010: 7269 7028 2227 5c5c 6e5c 5c72 2229 0a20  rip("'\\n\\r"). 
-00005020: 2020 2020 2020 2020 2020 2074 436c 6561             tClea
-00005030: 6e20 3d20 7443 6c65 616e 2e73 706c 6974  n = tClean.split
-00005040: 2827 5c5c 6e27 295b 2d31 5d0a 2020 2020  ('\\n')[-1].    
-00005050: 2020 2020 2020 2020 7443 6c65 616e 203d          tClean =
-00005060: 2074 436c 6561 6e2e 7370 6c69 7428 275c   tClean.split('\
-00005070: 5c72 2729 5b2d 315d 0a20 2020 2020 2020  \r')[-1].       
-00005080: 2020 2020 2072 6574 7572 6e20 7443 6c65       return tCle
-00005090: 616e 0a20 2020 2020 2020 2065 6c73 653a  an.        else:
-000050a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000050b0: 6e74 2827 5761 726e 696e 6720 2d20 6e6f  nt('Warning - no
-000050c0: 7420 7265 6365 6976 6564 2041 434b 2066  t received ACK f
-000050d0: 726f 6d20 6261 7263 6f64 6520 7363 616e  rom barcode scan
-000050e0: 6e65 722e 2729 0a20 2020 2020 2020 2020  ner.').         
-000050f0: 2020 2072 6574 7572 6e20 7374 7228 7429     return str(t)
-00005100: 2e73 706c 6974 2827 5c5c 7827 295b 2d31  .split('\\x')[-1
-00005110: 5d0a 2020 2020 0a20 2020 2064 6566 2073  ].    .    def s
-00005120: 6361 6e5f 6578 745f 6964 2873 656c 662c  can_ext_id(self,
-00005130: 2073 6361 6e44 7572 3d30 2e35 2c20 5661   scanDur=0.5, Va
-00005140: 6c69 6461 7465 436e 743d 3329 3a0a 2020  lidateCnt=3):.  
-00005150: 2020 2020 2020 6261 7263 6f64 6552 6561        barcodeRea
-00005160: 6420 3d20 2727 0a20 2020 2020 2020 2062  d = ''.        b
-00005170: 6172 636f 6465 7320 3d20 5b5d 0a20 2020  arcodes = [].   
-00005180: 2020 2020 2073 7461 7274 5469 6d65 203d       startTime =
-00005190: 2074 696d 6528 290a 2020 2020 2020 2020   time().        
-000051a0: 7768 696c 6520 2828 7469 6d65 2829 202d  while ((time() -
-000051b0: 2073 7461 7274 5469 6d65 2920 3c20 7363   startTime) < sc
-000051c0: 616e 4475 7229 3a0a 2020 2020 2020 2020  anDur):.        
-000051d0: 2020 2020 6261 7263 6f64 6552 6561 6420      barcodeRead 
-000051e0: 3d20 7365 6c66 2e73 6361 6e5f 616e 645f  = self.scan_and_
-000051f0: 666c 7573 6828 290a 2020 2020 2020 2020  flush().        
-00005200: 2020 2020 2320 6261 7263 6f64 6552 6561      # barcodeRea
-00005210: 6420 3d20 7374 7228 7429 0a20 2020 2020  d = str(t).     
-00005220: 2020 2020 2020 2069 6620 6c65 6e28 6261         if len(ba
-00005230: 7263 6f64 6552 6561 6429 203c 2038 3a0a  rcodeRead) < 8:.
-00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005250: 6261 7263 6f64 6552 6561 6420 3d20 2727  barcodeRead = ''
-00005260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005270: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00005280: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005290: 2020 2069 6620 6c65 6e28 6261 7263 6f64     if len(barcod
-000052a0: 6573 2920 3c20 5661 6c69 6461 7465 436e  es) < ValidateCn
-000052b0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000052c0: 2020 2062 6172 636f 6465 732e 6170 7065     barcodes.appe
-000052d0: 6e64 2862 6172 636f 6465 5265 6164 290a  nd(barcodeRead).
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00005300: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00005310: 2020 6261 7263 6f64 6552 6561 6420 3d20    barcodeRead = 
-00005320: 6d6f 6465 2862 6172 636f 6465 7329 0a20  mode(barcodes). 
-00005330: 2020 2020 2020 2020 2020 2066 756c 6c44             fullD
-00005340: 6174 6120 3d20 6375 7249 6420 3d20 7265  ata = curId = re
-00005350: 656c 4964 203d 2067 7469 6e20 3d20 6261  elId = gtin = ba
-00005360: 7263 6f64 6552 6561 640a 2020 2020 2020  rcodeRead.      
-00005370: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00005380: 2020 2020 2020 2020 2020 2069 6620 2729             if ')
-00005390: 2720 696e 2066 756c 6c44 6174 613a 0a20  ' in fullData:. 
-000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053b0: 2020 2067 7469 6e20 3d20 2729 272e 6a6f     gtin = ')'.jo
-000053c0: 696e 2866 756c 6c44 6174 612e 7370 6c69  in(fullData.spli
-000053d0: 7428 2729 2729 5b3a 325d 2920 2b20 2729  t(')')[:2]) + ')
-000053e0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000053f0: 2020 2020 2020 7461 6744 6174 6120 3d20        tagData = 
-00005400: 6675 6c6c 4461 7461 2e73 706c 6974 2827  fullData.split('
-00005410: 2927 295b 325d 0a20 2020 2020 2020 2020  )')[2].         
-00005420: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
-00005430: 6774 696e 2077 6974 686f 7574 2070 6172  gtin without par
-00005440: 656e 7468 6573 6973 0a20 2020 2020 2020  enthesis.       
-00005450: 2020 2020 2020 2020 2020 2020 2067 7469               gti
-00005460: 6e20 3d20 6675 6c6c 4461 7461 5b30 3a31  n = fullData[0:1
-00005470: 385d 0a20 2020 2020 2020 2020 2020 2020  8].             
-00005480: 2020 2020 2020 2074 6167 4461 7461 203d         tagData =
-00005490: 2066 756c 6c44 6174 615b 3138 3a5d 0a20   fullData[18:]. 
-000054a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000054b0: 7572 4964 203d 2074 6167 4461 7461 2e73  urId = tagData.s
-000054c0: 706c 6974 2827 5427 295b 315d 2e73 7472  plit('T')[1].str
-000054d0: 6970 2822 2720 2229 2e73 706c 6974 2827  ip("' ").split('
-000054e0: 2827 295b 305d 0a20 2020 2020 2020 2020  (')[0].         
-000054f0: 2020 2020 2020 2072 6565 6c49 6420 3d20         reelId = 
-00005500: 7461 6744 6174 612e 7370 6c69 7428 2754  tagData.split('T
-00005510: 2729 5b30 5d2e 7374 7269 7028 2227 2022  ')[0].strip("' "
-00005520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005530: 2020 7265 7475 726e 2066 756c 6c44 6174    return fullDat
-00005540: 612c 2063 7572 4964 2c20 7265 656c 4964  a, curId, reelId
-00005550: 2c20 6774 696e 0a20 2020 2020 2020 2020  , gtin.         
-00005560: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-00005570: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00005580: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00005590: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000055a0: 6675 6c6c 4461 7461 2c20 6375 7249 642c  fullData, curId,
-000055b0: 2072 6565 6c49 642c 2067 7469 6e0a 2020   reelId, gtin.  
-000055c0: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
-000055d0: 6574 7572 6e20 4e6f 6e65 2c20 4e6f 6e65  eturn None, None
-000055e0: 2c20 4e6f 6e65 2c20 4e6f 6e65 0a20 2020  , None, None.   
-000055f0: 200a 2020 2020 6465 6620 6175 746f 5f73   .    def auto_s
-00005600: 6361 6e28 7365 6c66 293a 0a20 2020 2020  can(self):.     
-00005610: 2020 2023 2070 7269 6e74 2822 4175 746f     # print("Auto
-00005620: 6d61 7469 6320 7265 6164 696e 6720 7365  matic reading se
-00005630: 7474 696e 6773 2229 0a20 2020 2020 2020  ttings").       
-00005640: 2073 656c 662e 7365 7269 616c 2e77 7269   self.serial.wri
-00005650: 7465 2862 225c 7831 625c 7833 3222 290a  te(b"\x1b\x32").
-00005660: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00005670: 3129 0a20 2020 2020 2020 2074 203d 2073  1).        t = s
-00005680: 656c 662e 7365 7269 616c 2e72 6561 645f  elf.serial.read_
-00005690: 616c 6c28 290a 2020 2020 2020 2020 2320  all().        # 
-000056a0: 7072 696e 7428 7429 0a20 2020 2020 2020  print(t).       
-000056b0: 2072 6574 7572 6e20 740a 2020 2020 0a20   return t.    . 
-000056c0: 2020 2064 6566 2074 7269 6767 6572 5f73     def trigger_s
-000056d0: 746f 705f 7365 7474 696e 6773 2873 656c  top_settings(sel
-000056e0: 6629 3a0a 2020 2020 2020 2020 2320 7072  f):.        # pr
-000056f0: 696e 7428 2254 7269 6767 6572 5f73 746f  int("Trigger_sto
-00005700: 705f 7365 7474 696e 6773 2229 0a20 2020  p_settings").   
-00005710: 2020 2020 2023 2073 6c65 6570 2830 2e31       # sleep(0.1
-00005720: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
-00005730: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
-00005740: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
-00005750: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00005760: 2020 2020 7420 3d20 7365 6c66 2e73 6572      t = self.ser
-00005770: 6961 6c2e 7265 6164 5f61 6c6c 2829 0a20  ial.read_all(). 
-00005780: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
-00005790: 290a 2020 2020 2020 2020 2320 7072 696e  ).        # prin
-000057a0: 7428 7429 0a20 2020 2020 2020 2061 636b  t(t).        ack
-000057b0: 7320 3d20 7374 7228 7429 2e73 706c 6974  s = str(t).split
-000057c0: 2827 3b27 295b 3a2d 315d 0a20 2020 2020  (';')[:-1].     
-000057d0: 2020 2069 7353 7563 6365 7373 203d 2061     isSuccess = a
-000057e0: 6c6c 285b 5472 7565 2069 6620 6163 6b2e  ll([True if ack.
-000057f0: 656e 6473 7769 7468 2827 5c5c 7830 3627  endswith('\\x06'
-00005800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005810: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00005820: 4661 6c73 6520 666f 7220 6163 6b20 696e  False for ack in
-00005830: 2061 636b 735d 290a 2020 2020 2020 2020   acks]).        
-00005840: 7265 7475 726e 2074 2c20 6973 5375 6363  return t, isSucc
-00005850: 6573 730a 0a0a 636c 6173 7320 596f 6374  ess...class Yoct
-00005860: 6f54 656d 7065 7261 7475 7265 5365 6e73  oTemperatureSens
-00005870: 6f72 286f 626a 6563 7429 3a0a 2020 2020  or(object):.    
-00005880: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00005890: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-000058a0: 2e73 656e 736f 7220 3d20 4e6f 6e65 0a20  .sensor = None. 
-000058b0: 2020 2020 2020 2065 7272 6d73 6720 3d20         errmsg = 
-000058c0: 5952 6566 5061 7261 6d28 290a 2020 2020  YRefParam().    
-000058d0: 2020 2020 2320 5365 7475 7020 7468 6520      # Setup the 
-000058e0: 4150 4920 746f 2075 7365 206c 6f63 616c  API to use local
-000058f0: 2055 5342 2064 6576 6963 6573 0a20 2020   USB devices.   
-00005900: 2020 2020 2069 6620 5941 5049 2e52 6567       if YAPI.Reg
-00005910: 6973 7465 7248 7562 2822 7573 6222 2c20  isterHub("usb", 
-00005920: 6572 726d 7367 2920 213d 2059 4150 492e  errmsg) != YAPI.
-00005930: 5355 4343 4553 533a 0a20 2020 2020 2020  SUCCESS:.       
-00005940: 2020 2020 2072 6169 7365 2045 7175 6970       raise Equip
-00005950: 6d65 6e74 4572 726f 7228 2779 6f63 746f  mentError('yocto
-00005960: 2074 656d 7065 7261 7475 7265 2073 656e   temperature sen
-00005970: 736f 7220 676f 7420 696e 6974 2065 7272  sor got init err
-00005980: 6f72 3a20 7b7d 272e 666f 726d 6174 2865  or: {}'.format(e
-00005990: 7272 6d73 672e 7661 6c75 6529 290a 0a20  rrmsg.value)).. 
-000059a0: 2020 2064 6566 2063 6f6e 6e65 6374 2873     def connect(s
-000059b0: 656c 662c 2074 6172 6765 743d 2761 6e79  elf, target='any
-000059c0: 2729 3a0a 2020 2020 2020 2020 6966 2074  '):.        if t
-000059d0: 6172 6765 7420 3d3d 2027 616e 7927 3a0a  arget == 'any':.
-000059e0: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-000059f0: 7472 6965 7665 2061 6e79 2074 656d 7065  trieve any tempe
-00005a00: 7261 7475 7265 2073 656e 736f 720a 2020  rature sensor.  
-00005a10: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00005a20: 656e 736f 7220 3d20 5954 656d 7065 7261  ensor = YTempera
-00005a30: 7475 7265 2e46 6972 7374 5465 6d70 6572  ture.FirstTemper
-00005a40: 6174 7572 6528 290a 2020 2020 2020 2020  ature().        
-00005a50: 656c 6966 2074 6172 6765 7420 3d3d 2027  elif target == '
-00005a60: 273a 0a20 2020 2020 2020 2020 2020 2070  ':.            p
-00005a70: 7269 6e74 2827 7370 6563 6966 6965 6420  rint('specified 
-00005a80: 696e 7661 6c69 6420 7461 7267 6574 2729  invalid target')
-00005a90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005aa0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00005ab0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00005ac0: 2020 2020 7365 6c66 2e73 656e 736f 7220      self.sensor 
-00005ad0: 3d20 5954 656d 7065 7261 7475 7265 2e46  = YTemperature.F
-00005ae0: 696e 6454 656d 7065 7261 7475 7265 2874  indTemperature(t
-00005af0: 6172 6765 7420 2b20 272e 7465 6d70 6572  arget + '.temper
-00005b00: 6174 7572 6527 290a 2020 2020 2020 2020  ature').        
-00005b10: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
-00005b20: 7320 4e6f 6e65 206f 7220 7365 6c66 2e67  s None or self.g
-00005b30: 6574 5f73 656e 736f 725f 6e61 6d65 2829  et_sensor_name()
-00005b40: 203d 3d20 2775 6e72 6573 6f6c 7665 6427   == 'unresolved'
-00005b50: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00005b60: 696e 7428 274e 6f20 6d6f 6475 6c65 2063  int('No module c
-00005b70: 6f6e 6e65 6374 6564 2729 0a20 2020 2020  onnected').     
-00005b80: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00005b90: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
-00005ba0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00005bb0: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
-00005bc0: 6566 2067 6574 5f73 656e 736f 725f 6e61  ef get_sensor_na
-00005bd0: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
-00005be0: 2020 6966 2073 656c 662e 7365 6e73 6f72    if self.sensor
-00005bf0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005c00: 2020 2020 2020 7072 696e 7428 276e 6f20        print('no 
-00005c10: 7365 6e73 6f72 2069 7320 636f 6e6e 6563  sensor is connec
-00005c20: 7465 642e 2074 7279 2074 6f20 6361 6c6c  ted. try to call
-00005c30: 2063 6f6e 6e65 6374 2829 2066 6972 7374   connect() first
-00005c40: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
-00005c50: 6574 7572 6e20 2727 0a0a 2020 2020 2020  eturn ''..      
-00005c60: 2020 7365 6e73 6f72 5f73 7472 203d 2073    sensor_str = s
-00005c70: 656c 662e 7365 6e73 6f72 2e64 6573 6372  elf.sensor.descr
-00005c80: 6962 6528 290a 2020 2020 2020 2020 6e61  ibe().        na
-00005c90: 6d65 5f73 7472 203d 2073 656e 736f 725f  me_str = sensor_
-00005ca0: 7374 722e 7370 6c69 7428 273d 2729 5b31  str.split('=')[1
-00005cb0: 5d2e 7370 6c69 7428 272e 2729 5b30 5d0a  ].split('.')[0].
-00005cc0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00005cd0: 616d 655f 7374 720a 0a20 2020 2064 6566  ame_str..    def
-00005ce0: 2067 6574 5f74 656d 7065 7261 7475 7265   get_temperature
-00005cf0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00005d00: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
-00005d10: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00005d20: 2020 2020 7072 696e 7428 2773 656e 736f      print('senso
-00005d30: 7220 6973 206e 6f74 2063 6f6e 6e65 6374  r is not connect
-00005d40: 6564 2e20 7472 7920 746f 2063 616c 6c20  ed. try to call 
-00005d50: 636f 6e6e 6563 7428 2920 6669 7273 7427  connect() first'
-00005d60: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00005d70: 7475 726e 2066 6c6f 6174 2827 6e61 6e27  turn float('nan'
-00005d80: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00005d90: 2028 7365 6c66 2e73 656e 736f 722e 6973   (self.sensor.is
-00005da0: 4f6e 6c69 6e65 2829 293a 0a20 2020 2020  Online()):.     
-00005db0: 2020 2020 2020 2070 7269 6e74 2827 7365         print('se
-00005dc0: 6e73 6f72 2069 7320 6e6f 7420 636f 6e6e  nsor is not conn
-00005dd0: 6563 7465 6420 6f72 2064 6973 636f 6e6e  ected or disconn
-00005de0: 6563 7465 6420 6475 7269 6e67 2072 756e  ected during run
-00005df0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
-00005e00: 6574 7572 6e20 666c 6f61 7428 276e 616e  eturn float('nan
-00005e10: 2729 0a0a 2020 2020 2020 2020 7265 7475  ')..        retu
-00005e20: 726e 2073 656c 662e 7365 6e73 6f72 2e67  rn self.sensor.g
-00005e30: 6574 5f63 7572 7265 6e74 5661 6c75 6528  et_currentValue(
-00005e40: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
-00005e50: 7468 6f64 0a20 2020 2064 6566 2065 7869  thod.    def exi
-00005e60: 745f 6170 7028 293a 0a20 2020 2020 2020  t_app():.       
-00005e70: 2059 4150 492e 4672 6565 4150 4928 290a   YAPI.FreeAPI().
+00002c10: 7072 696e 7428 7365 6c66 2e6e 6577 5f61  print(self.new_a
+00002c20: 7474 290a 2020 2020 2020 2020 2020 2020  tt).            
+00002c30: 2020 2020 7265 7475 726e 2073 5b31 5d20      return s[1] 
+00002c40: 2b20 735b 325d 202f 2034 0a20 2020 2020  + s[2] / 4.     
+00002c50: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00002c60: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00002c80: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
+00002c90: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
+00002ca0: 6174 7420 3d20 650a 2020 2020 2020 2020  att = e.        
+00002cb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002cc0: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00002cd0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00002ce0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00002cf0: 6465 762e 7365 745f 636f 6e66 6967 7572  dev.set_configur
+00002d00: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+00002d10: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00002d20: 2020 2020 2020 2020 2073 656c 662e 636d           self.cm
+00002d30: 6431 5b30 5d20 3d20 3138 0a20 2020 2020  d1[0] = 18.     
+00002d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002d50: 6465 762e 7772 6974 6528 3078 3031 2c20  dev.write(0x01, 
+00002d60: 7365 6c66 2e63 6d64 3129 2020 2320 4765  self.cmd1)  # Ge
+00002d70: 7420 6174 7465 6e75 6174 7469 6f6e 0a20  t attenuattion. 
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002d90: 203d 2073 656c 662e 6465 762e 7265 6164   = self.dev.read
+00002da0: 2830 7838 312c 2036 3429 0a20 2020 2020  (0x81, 64).     
+00002db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002dc0: 6e65 775f 6174 7420 3d20 2743 7572 7265  new_att = 'Curre
+00002dd0: 6e74 2041 7474 656e 7561 7469 6f6e 203d  nt Attenuation =
+00002de0: 207b 7d64 4220 272e 666f 726d 6174 2873   {}dB '.format(s
+00002df0: 7472 2873 5b31 5d20 2b20 735b 325d 202f  tr(s[1] + s[2] /
+00002e00: 2034 2929 0a20 2020 2020 2020 2020 2020   4)).           
+00002e10: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+00002e20: 6e65 775f 6174 7429 0a20 2020 2020 2020  new_att).       
+00002e30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002e40: 735b 315d 202b 2073 5b32 5d20 2f20 340a  s[1] + s[2] / 4.
+00002e50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002e60: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002e70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002e80: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
+00002e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ea0: 2e6e 6577 5f61 7474 203d 2065 0a20 2020  .new_att = e.   
+00002eb0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00002ec0: 7572 6e20 730a 0a20 2020 2020 2020 2064  urn s..        d
+00002ed0: 6566 2053 656e 645f 5343 5049 2873 656c  ef Send_SCPI(sel
+00002ee0: 662c 2053 4350 4963 6d64 2c20 746d 7029  f, SCPIcmd, tmp)
+00002ef0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002f00: 7365 6e64 2053 4350 4920 636f 6d6d 616e  send SCPI comman
+00002f10: 6473 2028 746f 2073 7570 706f 7274 6564  ds (to supported
+00002f20: 2066 6972 6d77 6172 6520 6f6e 6c79 2129   firmware only!)
+00002f30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002f40: 662e 636d 6431 5b30 5d20 3d20 3432 0a20  f.cmd1[0] = 42. 
+00002f50: 2020 2020 2020 2020 2020 206c 3120 3d20             l1 = 
+00002f60: 300a 2020 2020 2020 2020 2020 2020 6c31  0.            l1
+00002f70: 203d 206c 656e 2853 4350 4963 6d64 290a   = len(SCPIcmd).
+00002f80: 2020 2020 2020 2020 2020 2020 696e 6478              indx
+00002f90: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00002fa0: 2077 6869 6c65 2028 696e 6478 203c 3d20   while (indx <= 
+00002fb0: 6c31 293a 0a20 2020 2020 2020 2020 2020  l1):.           
+00002fc0: 2020 2020 2073 656c 662e 636d 6431 5b69       self.cmd1[i
+00002fd0: 6e64 785d 203d 206f 7264 2853 4350 4963  ndx] = ord(SCPIc
+00002fe0: 6d64 5b69 6e64 7820 2d20 315d 290a 2020  md[indx - 1]).  
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003000: 6478 203d 2069 6e64 7820 2b20 310a 2020  dx = indx + 1.  
+00003010: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003020: 6d64 315b 696e 6478 5d20 3d20 300a 2020  md1[indx] = 0.  
+00003030: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003040: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+00003050: 656c 662e 636d 6431 2920 2023 2053 4350  elf.cmd1)  # SCP
+00003060: 2043 6f6d 6d61 6e64 2075 7020 746f 2036   Command up to 6
+00003070: 3020 6368 6172 733b 0a20 2020 2020 2020  0 chars;.       
+00003080: 2020 2020 2073 203d 2073 656c 662e 6465       s = self.de
+00003090: 762e 7265 6164 2830 7838 312c 2036 3429  v.read(0x81, 64)
+000030a0: 0a20 2020 2020 2020 2020 2020 2069 203d  .            i =
+000030b0: 2031 0a20 2020 2020 2020 2020 2020 2052   1.            R
+000030c0: 6574 5374 7220 3d20 2222 0a20 2020 2020  etStr = "".     
+000030d0: 2020 2020 2020 2077 6869 6c65 2028 735b         while (s[
+000030e0: 695d 203e 2030 293a 0a20 2020 2020 2020  i] > 0):.       
+000030f0: 2020 2020 2020 2020 2052 6574 5374 7220           RetStr 
+00003100: 3d20 5265 7453 7472 202b 2063 6872 2873  = RetStr + chr(s
+00003110: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00003120: 2020 2020 2069 203d 2069 202b 2031 0a20       i = i + 1. 
+00003130: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003140: 6e20 7374 7228 5265 7453 7472 290a 0a20  n str(RetStr).. 
+00003150: 2020 2063 6c61 7373 2041 5049 286f 626a     class API(obj
+00003160: 6563 7429 3a0a 0a20 2020 2020 2020 2064  ect):..        d
+00003170: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00003180: 2c20 636f 6d70 6f72 743d 2241 5554 4f22  , comport="AUTO"
+00003190: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000031a0: 656c 662e 6261 7564 7261 7465 203d 2039  elf.baudrate = 9
+000031b0: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
+000031c0: 6966 2063 6f6d 706f 7274 203d 3d20 2241  if comport == "A
+000031d0: 5554 4f22 3a0a 2020 2020 2020 2020 2020  UTO":.          
+000031e0: 2020 2020 2020 706f 7274 735f 6c69 7374        ports_list
+000031f0: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
+00003200: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003210: 2020 666f 7220 706f 7274 2069 6e20 706f    for port in po
+00003220: 7274 735f 6c69 7374 3a0a 2020 2020 2020  rts_list:.      
+00003230: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003240: 6c66 2e63 6f6d 706f 7274 203d 2070 6f72  lf.comport = por
+00003250: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00003260: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
+00003270: 6572 6961 6c2e 5365 7269 616c 2873 656c  erial.Serial(sel
+00003280: 662e 636f 6d70 6f72 742c 2073 656c 662e  f.comport, self.
+00003290: 6261 7564 7261 7465 2c20 7469 6d65 6f75  baudrate, timeou
+000032a0: 743d 302e 3529 0a20 2020 2020 2020 2020  t=0.5).         
+000032b0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+000032c0: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
+000032d0: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+000032e0: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003310: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003320: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003330: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003340: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
+00003350: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
+00003380: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
+00003390: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
+000033c0: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
+000033d0: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000033e0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000033f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003400: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
+00003410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003420: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
+00003430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003440: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
+00003450: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
+00003460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003470: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
+00003480: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
+00003490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000034a0: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
+000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034c0: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
+000034d0: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
+00003500: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
+00003510: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
+00003580: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003590: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
+000035a0: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035c0: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
+000035d0: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
+000035e0: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
+000035f0: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
+00003600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003610: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003630: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
+00003640: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
+00003650: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
+00003680: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
+00003690: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
+000036a0: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
+000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036e0: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+000036f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003700: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
+00003710: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
+00003720: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
+00003730: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
+00003740: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+00003750: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
+00003760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003770: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
+00003780: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
+00003790: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+000037a0: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
+000037b0: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
+000037c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000037d0: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
+000037e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000037f0: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003820: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003830: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
+00003840: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
+00003850: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003860: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
+00003870: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
+00003880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003890: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000038b0: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
+000038c0: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
+000038d0: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000038f0: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
+00003900: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
+00003910: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
+00003920: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
+00003930: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00003940: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
+00003950: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
+00003960: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
+00003970: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
+00003980: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
+00003990: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
+000039a0: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
+000039b0: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+000039c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
+000039f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003a00: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
+00003a10: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
+00003a20: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
+00003a30: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
+00003a40: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
+00003a50: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00003a60: 0a0a 2020 2020 2020 2020 6465 6620 5772  ..        def Wr
+00003a70: 6974 6528 7365 6c66 2c20 636d 642c 2077  ite(self, cmd, w
+00003a80: 6169 743d 4661 6c73 6529 3a0a 2020 2020  ait=False):.    
+00003a90: 2020 2020 2020 2020 2222 2253 656e 6420          """Send 
+00003aa0: 7468 6520 696e 7075 7420 636d 6420 7374  the input cmd st
+00003ab0: 7269 6e67 2076 6961 2043 4f4d 2053 6f63  ring via COM Soc
+00003ac0: 6b65 7422 2222 0a20 2020 2020 2020 2020  ket""".         
+00003ad0: 2020 2069 6620 7365 6c66 2e73 2e69 734f     if self.s.isO
+00003ae0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00003af0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00003b00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003b20: 6c66 2e73 2e6f 7065 6e28 290a 2020 2020  lf.s.open().    
+00003b30: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+00003b40: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+00003b50: 2020 2020 2020 2020 736c 6565 7028 3129          sleep(1)
+00003b60: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00003b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003b80: 2020 7365 6c66 2e73 2e77 7269 7465 2873    self.s.write(s
+00003b90: 7472 2e65 6e63 6f64 6528 636d 6429 290a  tr.encode(cmd)).
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 736c 6565 7028 302e 3129 2020 2320 436f  sleep(0.1)  # Co
+00003bc0: 6d6d 616e 6473 206d 6179 2062 6520 6c6f  mmands may be lo
+00003bd0: 7374 2077 6865 6e20 7772 6974 696e 6720  st when writing 
+00003be0: 746f 6f20 6661 7374 0a0a 2020 2020 2020  too fast..      
+00003bf0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00003c10: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
+00003c20: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
+00003c30: 0a20 2020 2020 2020 2064 6566 2051 7565  .        def Que
+00003c40: 7279 2873 656c 662c 2063 6d64 293a 0a20  ry(self, cmd):. 
+00003c50: 2020 2020 2020 2020 2020 2022 2222 5365             """Se
+00003c60: 6e64 2074 6865 2069 6e70 7574 2063 6d64  nd the input cmd
+00003c70: 2073 7472 696e 6720 7669 6120 434f 4d20   string via COM 
+00003c80: 536f 636b 6574 2061 6e64 2072 6574 7572  Socket and retur
+00003c90: 6e20 7468 6520 7265 706c 7920 7374 7269  n the reply stri
+00003ca0: 6e67 2222 220a 2020 2020 2020 2020 2020  ng""".          
+00003cb0: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
+00003cc0: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+00003cd0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00003ce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003d00: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
+00003d10: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00003d20: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
+00003d30: 2020 2320 7365 6c66 2e73 2e66 6c75 7368    # self.s.flush
+00003d40: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+00003d50: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
+00003d60: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00003d70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003d80: 6c66 2e73 2e77 7269 7465 2863 6d64 2e65  lf.s.write(cmd.e
+00003d90: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+00003da0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003db0: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003dc0: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
+00003dd0: 5f77 6169 7469 6e67 203e 2030 3a0a 2020  _waiting > 0:.  
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 6461 7461 203d 2073 656c 662e 732e    data = self.s.
+00003e00: 7265 6164 6c69 6e65 2829 2e64 6563 6f64  readline().decod
+00003e10: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00003e20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e40: 2020 2020 2064 6174 6120 3d20 2727 0a20       data = ''. 
+00003e50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00003e60: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00003e70: 2020 2064 6174 6120 3d20 2727 0a20 2020     data = ''.   
+00003e80: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00003e90: 732e 636c 6f73 6528 290a 2020 2020 2020  s.close().      
+00003ea0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00003eb0: 610a 0a20 2020 2020 2020 2064 6566 2063  a..        def c
+00003ec0: 6c6f 7365 5f70 6f72 7428 7365 6c66 293a  lose_port(self):
+00003ed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003ee0: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
+00003ef0: 6e65 2061 6e64 2073 656c 662e 732e 6973  ne and self.s.is
+00003f00: 4f70 656e 2829 3a0a 2020 2020 2020 2020  Open():.        
+00003f10: 2020 2020 2020 2020 7365 6c66 2e73 2e63          self.s.c
+00003f20: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+00003f30: 6465 6620 6973 5f6f 7065 6e28 7365 6c66  def is_open(self
+00003f40: 2c20 6368 6563 6b5f 706f 7274 3d46 616c  , check_port=Fal
+00003f50: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00003f60: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
+00003f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003f80: 2020 2020 2020 2020 6966 2063 6865 636b          if check
+00003f90: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
+00003fa0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fc0: 2020 2020 2020 2020 7365 6c66 2e51 7565          self.Que
+00003fd0: 7279 2822 2a49 444e 3f5c 725c 6e22 290a  ry("*IDN?\r\n").
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 2020 2020 7265 7370 203d 2073          resp = s
+00004000: 656c 662e 5175 6572 7928 222a 4944 4e3f  elf.Query("*IDN?
+00004010: 5c72 5c6e 2229 0a20 2020 2020 2020 2020  \r\n").         
+00004020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004030: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
+00004040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004050: 2020 2020 2020 2020 2069 6620 2822 4165           if ("Ae
+00004060: 726f 666c 6578 2220 696e 2072 6573 7029  roflex" in resp)
+00004070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004080: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004090: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2020 656c 6966 2027 3833 3131 2720 696e    elif '8311' in
+000040c0: 2072 6573 7020 6f72 2027 3833 3331 2720   resp or '8331' 
+000040d0: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00004100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004110: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2073 656c 662e 636c 6f73 655f       self.close_
+00004140: 706f 7274 2829 0a20 2020 2020 2020 2020  port().         
+00004150: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2072 6574 7572 6e20 7365 6c66 2e73 2e69   return self.s.i
+00004180: 734f 7065 6e28 290a 2020 2020 2020 2020  sOpen().        
+00004190: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000041a0: 0a0a 2020 2020 2020 2020 6465 6620 5365  ..        def Se
+000041b0: 7461 7474 6e28 7365 6c66 2c20 6174 746e  tattn(self, attn
+000041c0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000041d0: 6d64 203d 2022 4154 544e 207b 3a2e 3266  md = "ATTN {:.2f
+000041e0: 7d5c 725c 6e22 2e66 6f72 6d61 7428 6174  }\r\n".format(at
+000041f0: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
+00004200: 7365 6c66 2e57 7269 7465 2863 6d64 290a  self.Write(cmd).
+00004210: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00004220: 6520 3d20 7365 6c66 2e47 6574 6174 746e  e = self.Getattn
+00004230: 2829 0a20 2020 2020 2020 2020 2020 2076  ().            v
+00004240: 616c 7565 203d 2066 6c6f 6174 2876 616c  alue = float(val
+00004250: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00004260: 6966 2076 616c 7565 2021 3d20 6174 746e  if value != attn
+00004270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004280: 2020 7072 696e 7428 6627 4572 726f 7220    print(f'Error 
+00004290: 7365 7474 696e 6720 6174 7465 6e75 6174  setting attenuat
+000042a0: 696f 6e3a 206e 6577 203a 207b 6174 746e  ion: new : {attn
+000042b0: 7d20 6375 7272 656e 743a 207b 7661 6c75  } current: {valu
+000042c0: 657d 2729 0a20 2020 2020 2020 2020 2020  e}').           
+000042d0: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
+000042e0: 2020 2020 2020 2064 6566 2047 6574 6174         def Getat
+000042f0: 746e 2873 656c 6629 3a0a 2020 2020 2020  tn(self):.      
+00004300: 2020 2020 2020 636d 6420 3d20 2241 5454        cmd = "ATT
+00004310: 4e3f 5c72 5c6e 220a 2020 2020 2020 2020  N?\r\n".        
+00004320: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00004330: 2e51 7565 7279 2863 6d64 290a 2020 2020  .Query(cmd).    
+00004340: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00004350: 616c 7565 0a0a 0a63 6c61 7373 2054 6573  alue...class Tes
+00004360: 636f 6d3a 0a20 2020 2022 2222 0a20 2020  com:.    """.   
+00004370: 2043 6f6e 7472 6f6c 2054 4553 434f 4d20   Control TESCOM 
+00004380: 7465 7374 696e 6720 6368 616d 6265 7273  testing chambers
+00004390: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
+000043a0: 6e5f 636d 6420 3d20 6227 4f50 454e 5c72  n_cmd = b'OPEN\r
+000043b0: 270a 2020 2020 636c 6f73 655f 636d 6420  '.    close_cmd 
+000043c0: 3d20 6227 434c 4f53 455c 7227 0a20 2020  = b'CLOSE\r'.   
+000043d0: 2063 6f6d 5f70 6f72 745f 6f62 6a20 3d20   com_port_obj = 
+000043e0: 4e6f 6e65 0a20 2020 206d 6f64 656c 735f  None.    models_
+000043f0: 6c69 7374 203d 205b 2754 432d 3530 3634  list = ['TC-5064
+00004400: 4327 2c20 2754 412d 3730 3131 4150 272c  C', 'TA-7011AP',
+00004410: 2027 5443 2d35 3036 3341 272c 2027 5443   'TC-5063A', 'TC
+00004420: 2d35 3937 3043 5027 5d0a 0a20 2020 2064  -5970CP']..    d
+00004430: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00004440: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
+00004450: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
+00004460: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
+00004470: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00004480: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
+00004490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000044a0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+000044b0: 7428 706f 7274 290a 0a20 2020 2020 2020  t(port)..       
+000044c0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000044d0: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+000044e0: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+000044f0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00004500: 5465 7363 6f6d 202d 2043 6f6e 6e65 6374  Tescom - Connect
+00004510: 696f 6e20 6661 696c 6564 2229 0a0a 2020  ion failed")..  
+00004520: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
+00004530: 6c66 2c20 706f 7274 293a 0a20 2020 2020  lf, port):.     
+00004540: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00004550: 7061 7261 6d20 706f 7274 3a20 636f 6d20  param port: com 
+00004560: 706f 7274 2074 6f20 636f 6e6e 6563 740a  port to connect.
+00004570: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00004580: 2063 6f6d 2070 6f72 7420 6f62 6a0a 2020   com port obj.  
+00004590: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000045a0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000045b0: 2020 2063 6f6d 5f70 6f72 745f 6f62 6a20     com_port_obj 
+000045c0: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+000045d0: 6f62 6a20 3d20 7365 7269 616c 2e53 6572  obj = serial.Ser
+000045e0: 6961 6c28 706f 7274 3d70 6f72 742c 2062  ial(port=port, b
+000045f0: 6175 6472 6174 653d 3936 3030 2c20 7469  audrate=9600, ti
+00004600: 6d65 6f75 743d 3129 0a20 2020 2020 2020  meout=1).       
+00004610: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
+00004620: 5f6f 626a 2069 7320 6e6f 7420 4e6f 6e65  _obj is not None
+00004630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004640: 2020 7365 6c66 2e64 6f6f 725f 636d 6420    self.door_cmd 
+00004650: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00004660: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
+00004670: 706f 7274 5f6f 626a 2e77 7269 7465 2862  port_obj.write(b
+00004680: 274d 4f44 454c 3f5c 7227 290a 2020 2020  'MODEL?\r').    
+00004690: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000046a0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000046b0: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+000046c0: 7472 2873 656c 662e 636f 6d5f 706f 7274  tr(self.com_port
+000046d0: 5f6f 626a 2e72 6561 6428 3134 2929 0a20  _obj.read(14)). 
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000046f0: 6172 7473 203d 205b 7020 666f 7220 7020  arts = [p for p 
+00004700: 696e 206d 6f64 656c 2e73 706c 6974 2822  in model.split("
+00004710: 2722 295d 0a20 2020 2020 2020 2020 2020  '")].           
+00004720: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
+00004730: 666f 7220 7020 696e 2070 6172 7473 5b31  for p in parts[1
+00004740: 5d2e 7370 6c69 7428 2220 2229 5d0a 2020  ].split(" ")].  
+00004750: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004760: 6c66 2e6d 6f64 656c 203d 2070 6172 7473  lf.model = parts
+00004770: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00004780: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00004790: 6d6f 6465 6c29 203e 2030 3a0a 2020 2020  model) > 0:.    
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 7072 696e 7428 2252 4620 6368 616d 6265  print("RF chambe
+000047c0: 7220 636f 6e6e 6563 7465 6420 746f 2070  r connected to p
+000047d0: 6f72 7420 2220 2b20 7374 7228 706f 7274  ort " + str(port
+000047e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000047f0: 2020 2020 2020 2070 7269 6e74 2822 5465         print("Te
+00004800: 7363 6f6d 202d 2043 6861 6d62 6572 206d  scom - Chamber m
+00004810: 6f64 656c 3a22 2c20 7365 6c66 2e6d 6f64  odel:", self.mod
+00004820: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+00004830: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00004840: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004850: 696e 7428 2254 6573 636f 6d20 2d20 4572  int("Tescom - Er
+00004860: 726f 7221 204e 6f20 6368 616d 6265 7220  ror! No chamber 
+00004870: 666f 756e 6422 290a 2020 2020 2020 2020  found").        
+00004880: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004890: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
+000048a0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+000048b0: 2069 6e20 7365 6c66 2e6d 6f64 656c 735f   in self.models_
+000048c0: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+000048d0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000048e0: 6f6f 725f 636d 6420 3d20 6227 444f 4f52  oor_cmd = b'DOOR
+000048f0: 3f5c 7227 0a20 2020 2020 2020 2020 2020  ?\r'.           
+00004900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004920: 656c 662e 646f 6f72 5f63 6d64 203d 2062  elf.door_cmd = b
+00004930: 274c 4944 3f5c 7227 0a20 2020 2020 2020  'LID?\r'.       
+00004940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004950: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004960: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
+00004970: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00004980: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
+00004990: 2020 2020 2020 2320 7072 696e 7428 6529        # print(e)
+000049a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000049b0: 6e74 2828 2254 6573 636f 6d20 2d20 436f  nt(("Tescom - Co
+000049c0: 756c 6420 6e6f 7420 636f 6e6e 6563 7420  uld not connect 
+000049d0: 746f 2070 6f72 7420 2220 2b20 706f 7274  to port " + port
+000049e0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+000049f0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00004a00: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
+00004a10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004a20: 220a 2020 2020 2020 2020 636c 6f73 6573  ".        closes
+00004a30: 2063 6f6d 2070 6f72 740a 2020 2020 2020   com port.      
+00004a40: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+00004a50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00004a60: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004a70: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00004a80: 2020 2020 2070 7269 6e74 2822 5246 2063       print("RF c
+00004a90: 6861 6d62 6572 2064 6973 636f 6e6e 6563  hamber disconnec
+00004aa0: 7465 6420 6672 6f6d 2070 6f72 743a 2022  ted from port: "
+00004ab0: 202b 2073 7472 2873 656c 662e 706f 7274   + str(self.port
+00004ac0: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+00004ad0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00004ae0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00004af0: 696e 7428 2243 6f75 6c64 206e 6f74 2064  int("Could not d
+00004b00: 6973 636f 6e6e 6563 7422 290a 0a20 2020  isconnect")..   
+00004b10: 2064 6566 206f 7065 6e5f 6368 616d 6265   def open_chambe
+00004b20: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00004b30: 2022 2222 0a20 2020 2020 2020 206f 7065   """.        ope
+00004b40: 6e73 2063 6861 6d62 6572 0a20 2020 2020  ns chamber.     
+00004b50: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00004b60: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00004b70: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00004b80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00004b90: 6620 7365 6c66 2e69 735f 646f 6f72 5f6f  f self.is_door_o
+00004ba0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00004bb0: 2020 2070 7269 6e74 2822 4368 616d 6265     print("Chambe
+00004bc0: 7220 6973 206f 7065 6e22 290a 2020 2020  r is open").    
+00004bd0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
+00004be0: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
+00004bf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004c00: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
+00004c10: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
+00004c20: 696e 6722 290a 2020 2020 2020 2020 2020  ing").          
+00004c30: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+00004c40: 6f62 6a2e 7265 7365 745f 696e 7075 745f  obj.reset_input_
+00004c50: 6275 6666 6572 2829 0a20 2020 2020 2020  buffer().       
+00004c60: 2020 2020 2073 656c 662e 636f 6d5f 706f       self.com_po
+00004c70: 7274 5f6f 626a 2e72 6573 6574 5f6f 7574  rt_obj.reset_out
+00004c80: 7075 745f 6275 6666 6572 2829 0a20 2020  put_buffer().   
+00004c90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004ca0: 6d5f 706f 7274 5f6f 626a 2e77 7269 7465  m_port_obj.write
+00004cb0: 2873 656c 662e 6f70 656e 5f63 6d64 290a  (self.open_cmd).
+00004cc0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00004cd0: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00004ce0: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00004cf0: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00004d00: 696c 6520 274f 4b27 206e 6f74 2069 6e20  ile 'OK' not in 
+00004d10: 7265 733a 0a20 2020 2020 2020 2020 2020  res:.           
+00004d20: 2020 2020 2069 6620 7761 6974 5f63 6f75       if wait_cou
+00004d30: 6e74 6572 203e 3d20 3135 3a0a 2020 2020  nter >= 15:.    
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00004d60: 6622 4572 726f 7220 696e 206f 7065 6e69  f"Error in openi
+00004d70: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+00004d80: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+00004d90: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+00004da0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004db0: 2e72 6561 6428 3134 292e 6465 636f 6465  .read(14).decode
+00004dc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004dd0: 2020 2020 2020 2775 7466 2d38 2729 2e75        'utf-8').u
+00004de0: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
+00004df0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00004e00: 2020 2020 6966 206c 656e 2873 7472 2872      if len(str(r
+00004e10: 6573 2929 203e 2030 3a0a 2020 2020 2020  es)) > 0:.      
+00004e20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004e30: 696e 7428 6627 4368 616d 6265 7220 7b73  int(f'Chamber {s
+00004e40: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
+00004e50: 3a20 2720 2b20 7374 7228 7265 7329 290a  : ' + str(res)).
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 7761 6974 5f63 6f75 6e74 6572 202b 3d20  wait_counter += 
+00004e80: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00004e90: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
+00004ea0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00004eb0: 7365 6c66 2e69 735f 646f 6f72 5f6f 7065  self.is_door_ope
+00004ec0: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
+00004ed0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00004ee0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00004ef0: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
+00004f00: 662e 706f 7274 7d20 446f 6f72 2073 7461  f.port} Door sta
+00004f10: 7475 7320 646f 6573 6e27 7420 6d61 7463  tus doesn't matc
+00004f20: 6820 636f 6d6d 616e 6420 7365 6e74 2122  h command sent!"
+00004f30: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00004f40: 696e 7428 6622 4368 616d 6265 7220 7b73  int(f"Chamber {s
+00004f50: 656c 662e 706f 7274 7d20 6973 206f 7065  elf.port} is ope
+00004f60: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00004f70: 7265 7475 726e 2027 4f4b 270a 2020 2020  return 'OK'.    
+00004f80: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00004f90: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00004fa0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00004fb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004fc0: 726e 2022 4641 494c 220a 0a20 2020 2064  rn "FAIL"..    d
+00004fd0: 6566 2063 6c6f 7365 5f63 6861 6d62 6572  ef close_chamber
+00004fe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004ff0: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
+00005000: 6573 2063 6861 6d62 6572 0a20 2020 2020  es chamber.     
+00005010: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00005020: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00005030: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00005040: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00005050: 6620 7365 6c66 2e69 735f 646f 6f72 5f63  f self.is_door_c
+00005060: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+00005070: 2020 2020 2070 7269 6e74 2822 4368 616d       print("Cham
+00005080: 6265 7220 636c 6f73 6564 2229 0a20 2020  ber closed").   
+00005090: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000050a0: 274f 4b27 0a20 2020 2020 2020 2074 7279  'OK'.        try
+000050b0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000050c0: 696e 7428 6622 4348 414d 4245 5220 7b73  int(f"CHAMBER {s
+000050d0: 656c 662e 706f 7274 7d20 4953 2043 4c4f  elf.port} IS CLO
+000050e0: 5349 4e47 2c20 434c 4541 5220 4841 4e44  SING, CLEAR HAND
+000050f0: 5321 2121 2229 0a20 2020 2020 2020 2020  S!!!").         
+00005100: 2020 2073 6c65 6570 2832 290a 2020 2020     sleep(2).    
+00005110: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00005120: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
+00005130: 7365 6c66 2e63 6c6f 7365 5f63 6d64 290a  self.close_cmd).
+00005140: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005150: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00005160: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00005170: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00005180: 696c 6520 2752 4541 4459 2720 6e6f 7420  ile 'READY' not 
+00005190: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
+000051a0: 2020 2020 2020 2020 6966 2077 6169 745f          if wait_
+000051b0: 636f 756e 7465 7220 3e3d 2032 303a 0a20  counter >= 20:. 
+000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051d0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+000051e0: 6f6e 2866 2245 7272 6f72 2069 6e20 636c  on(f"Error in cl
+000051f0: 6f73 696e 6720 6368 616d 6265 7220 7b73  osing chamber {s
+00005200: 656c 662e 706f 7274 7d22 290a 2020 2020  elf.port}").    
+00005210: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005220: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+00005230: 6f62 6a2e 7265 6164 2831 3429 2e64 6563  obj.read(14).dec
+00005240: 6f64 6528 0a20 2020 2020 2020 2020 2020  ode(.           
+00005250: 2020 2020 2020 2020 2027 7574 662d 3827           'utf-8'
+00005260: 292e 7570 7065 7228 292e 7273 7472 6970  ).upper().rstrip
+00005270: 2827 5c72 2729 0a20 2020 2020 2020 2020  ('\r').         
+00005280: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
+00005290: 696e 2072 6573 206f 7220 2752 4541 4459  in res or 'READY
+000052a0: 2720 696e 2072 6573 206f 7220 274f 4b27  ' in res or 'OK'
+000052b0: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
+000052c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000052d0: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
+000052e0: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
+000052f0: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
+00005300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005310: 6620 2745 5252 2720 696e 2072 6573 3a0a  f 'ERR' in res:.
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 7265 7475 726e 2022 4641 494c      return "FAIL
+00005340: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00005350: 2020 7761 6974 5f63 6f75 6e74 6572 202b    wait_counter +
+00005360: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00005370: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
+00005380: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00005390: 7420 7365 6c66 2e69 735f 646f 6f72 5f63  t self.is_door_c
+000053a0: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+000053b0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000053c0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+000053d0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000053e0: 7b73 656c 662e 706f 7274 7d20 446f 6f72  {self.port} Door
+000053f0: 2073 7461 7475 7320 646f 6573 6e27 7420   status doesn't 
+00005400: 6d61 7463 6820 636f 6d6d 616e 6420 7365  match command se
+00005410: 6e74 2122 290a 2020 2020 2020 2020 2020  nt!").          
+00005420: 2020 7072 696e 7428 6622 4368 616d 6265    print(f"Chambe
+00005430: 7220 7b73 656c 662e 706f 7274 7d20 636c  r {self.port} cl
+00005440: 6f73 6564 2229 0a20 2020 2020 2020 2020  osed").         
+00005450: 2020 2072 6574 7572 6e20 274f 4b27 0a20     return 'OK'. 
+00005460: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00005470: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00005480: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005490: 6622 4572 726f 7220 696e 2063 6c6f 7369  f"Error in closi
+000054a0: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+000054b0: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+000054c0: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
+000054d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000054e0: 2022 4641 494c 220a 0a20 2020 2064 6566   "FAIL"..    def
+000054f0: 2069 735f 636f 6e6e 6563 7465 6428 7365   is_connected(se
+00005500: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00005510: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+00005520: 6a20 6973 204e 6f6e 653a 0a20 2020 2020  j is None:.     
+00005530: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00005540: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+00005550: 726e 2073 656c 662e 636f 6d5f 706f 7274  rn self.com_port
+00005560: 5f6f 626a 2e69 734f 7065 6e28 290a 0a20  _obj.isOpen().. 
+00005570: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
+00005580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00005590: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+000055a0: 6a2e 7265 7365 745f 696e 7075 745f 6275  j.reset_input_bu
+000055b0: 6666 6572 2829 0a20 2020 2020 2020 2073  ffer().        s
+000055c0: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
+000055d0: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+000055e0: 6f62 6a2e 7772 6974 6528 7365 6c66 2e64  obj.write(self.d
+000055f0: 6f6f 725f 636d 6429 0a20 2020 2020 2020  oor_cmd).       
+00005600: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+00005610: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
+00005620: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
+00005630: 6164 2831 3429 2e64 6563 6f64 6528 2775  ad(14).decode('u
+00005640: 7466 2d38 2729 2e75 7070 6572 2829 2e72  tf-8').upper().r
+00005650: 7374 7269 7028 275c 7227 290a 2020 2020  strip('\r').    
+00005660: 2020 2020 7265 7475 726e 2073 7461 7465      return state
+00005670: 0a0a 2020 2020 6465 6620 6973 5f64 6f6f  ..    def is_doo
+00005680: 725f 6f70 656e 2873 656c 6629 3a0a 2020  r_open(self):.  
+00005690: 2020 2020 2020 7374 6174 6520 3d20 7365        state = se
+000056a0: 6c66 2e67 6574 5f73 7461 7465 2829 0a20  lf.get_state(). 
+000056b0: 2020 2020 2020 2069 6620 274f 5045 4e27         if 'OPEN'
+000056c0: 2069 6e20 7374 6174 653a 0a20 2020 2020   in state:.     
+000056d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000056e0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+000056f0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00005700: 2069 735f 646f 6f72 5f63 6c6f 7365 6428   is_door_closed(
+00005710: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00005720: 7461 7465 203d 2073 656c 662e 6765 745f  tate = self.get_
+00005730: 7374 6174 6528 290a 2020 2020 2020 2020  state().        
+00005740: 6966 2027 434c 4f53 4527 2069 6e20 7374  if 'CLOSE' in st
+00005750: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00005760: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005770: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005780: 650a 0a0a 636c 6173 7320 4261 7263 6f64  e...class Barcod
+00005790: 6553 6361 6e6e 6572 286f 626a 6563 7429  eScanner(object)
+000057a0: 3a0a 2020 2020 7072 6566 6978 203d 2027  :.    prefix = '
+000057b0: 7e01 3030 3030 4027 0a20 2020 2073 7566  ~.0000@'.    suf
+000057c0: 6669 7820 3d20 273b 0327 0a20 2020 2063  fix = ';.'.    c
+000057d0: 6f6d 203d 2027 270a 2020 2020 7365 7269  om = ''.    seri
+000057e0: 616c 203d 204e 6f6e 650a 0a20 2020 2064  al = None..    d
+000057f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00005800: 2c20 636f 6d3d 4e6f 6e65 2c20 6261 7564  , com=None, baud
+00005810: 3d31 3135 3230 302c 2063 6f6e 6669 673d  =115200, config=
+00005820: 5472 7565 2c20 6c6f 675f 7479 7065 3d27  True, log_type='
+00005830: 4e4f 5f4c 4f47 2729 3a0a 2020 2020 2020  NO_LOG'):.      
+00005840: 2020 7365 6c66 2e6c 6f67 5f74 7970 6520    self.log_type 
+00005850: 3d20 6c6f 675f 7479 7065 0a20 2020 2020  = log_type.     
+00005860: 2020 2069 6620 636f 6d20 213d 204e 6f6e     if com != Non
+00005870: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005880: 656c 662e 6f70 656e 5f70 6f72 7428 636f  elf.open_port(co
+00005890: 6d2c 2062 6175 643d 6261 7564 2c20 636f  m, baud=baud, co
+000058a0: 6e66 6967 3d63 6f6e 6669 6729 0a20 2020  nfig=config).   
+000058b0: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+000058c0: 2020 2020 2023 2020 2020 2073 656c 662e       #     self.
+000058d0: 7365 7269 616c 203d 2073 6572 203d 2053  serial = ser = S
+000058e0: 6572 6961 6c28 290a 0a20 2020 2064 6566  erial()..    def
+000058f0: 206f 7065 6e5f 706f 7274 2873 656c 662c   open_port(self,
+00005900: 2063 6f6d 2c20 6261 7564 3d31 3135 3230   com, baud=11520
+00005910: 302c 2063 6f6e 6669 673d 5472 7565 293a  0, config=True):
+00005920: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005930: 2e73 6572 6961 6c20 213d 204e 6f6e 6520  .serial != None 
+00005940: 616e 6420 7365 6c66 2e73 6572 6961 6c2e  and self.serial.
+00005950: 6973 5f6f 7065 6e28 293a 0a20 2020 2020  is_open():.     
+00005960: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005970: 616c 2e63 6c6f 7365 506f 7274 2829 0a20  al.closePort(). 
+00005980: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005990: 616c 203d 2073 6572 203d 2073 6572 6961  al = ser = seria
+000059a0: 6c2e 5365 7269 616c 2863 6f6d 2c20 6261  l.Serial(com, ba
+000059b0: 7564 2c20 7469 6d65 6f75 743d 302e 3529  ud, timeout=0.5)
+000059c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000059d0: 7365 6c66 2e63 6865 636b 5f63 6f6d 5f70  self.check_com_p
+000059e0: 6f72 7428 293a 0a20 2020 2020 2020 2020  ort():.         
+000059f0: 2020 2070 7269 6e74 2866 277b 636f 6d7d     print(f'{com}
+00005a00: 2069 7320 6e6f 7420 6261 7263 6f64 6520   is not barcode 
+00005a10: 7363 616e 6e65 7227 290a 2020 2020 2020  scanner').      
+00005a20: 2020 6966 2073 6572 2021 3d20 4e6f 6e65    if ser != None
+00005a30: 2061 6e64 2073 656c 662e 6c6f 675f 7479   and self.log_ty
+00005a40: 7065 2021 3d20 274e 4f5f 4c4f 4727 3a0a  pe != 'NO_LOG':.
+00005a50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00005a60: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
+00005a70: 6e65 7220 287b 636f 6d7d 2920 636f 6e6e  ner ({com}) conn
+00005a80: 6563 7465 642e 2729 0a20 2020 2020 2020  ected.').       
+00005a90: 2065 6c69 6620 7365 7220 3d3d 204e 6f6e   elif ser == Non
+00005aa0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00005ab0: 7269 6e74 2866 2742 6172 636f 6465 2073  rint(f'Barcode s
+00005ac0: 6361 6e6e 6572 202d 2050 726f 626c 656d  canner - Problem
+00005ad0: 2063 6f6e 6e65 6374 696e 6720 7b63 6f6d   connecting {com
+00005ae0: 7d27 290a 2020 2020 2020 2020 7365 6c66  }').        self
+00005af0: 2e63 6f6d 203d 2063 6f6d 0a20 2020 2020  .com = com.     
+00005b00: 2020 2073 6572 2e74 696d 6572 6f75 7420     ser.timerout 
+00005b10: 3d20 3120 2023 2072 6561 6420 7469 6d65  = 1  # read time
+00005b20: 206f 7574 0a20 2020 2020 2020 2073 6572   out.        ser
+00005b30: 2e77 7269 7465 5469 6d65 6f75 7420 3d20  .writeTimeout = 
+00005b40: 302e 3520 2023 2077 7269 7465 2074 696d  0.5  # write tim
+00005b50: 6520 6f75 742e 0a20 2020 2020 2020 2069  e out..        i
+00005b60: 6620 636f 6e66 6967 3a0a 2020 2020 2020  f config:.      
+00005b70: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00005b80: 6775 7265 2829 0a0a 2020 2020 6465 6620  gure()..    def 
+00005b90: 6669 6e64 5f61 6e64 5f6f 7065 6e5f 706f  find_and_open_po
+00005ba0: 7274 2873 656c 662c 2062 6175 643d 3131  rt(self, baud=11
+00005bb0: 3532 3030 2c20 636f 6e66 6967 3d54 7275  5200, config=Tru
+00005bc0: 6529 3a0a 2020 2020 2020 2020 636f 6d20  e):.        com 
+00005bd0: 3d20 7365 6c66 2e66 696e 645f 636f 6d5f  = self.find_com_
+00005be0: 706f 7274 2862 6175 6429 0a20 2020 2020  port(baud).     
+00005bf0: 2020 2069 6620 636f 6d20 6973 206e 6f74     if com is not
+00005c00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005c10: 2020 2073 656c 662e 6f70 656e 5f70 6f72     self.open_por
+00005c20: 7428 636f 6d2c 2062 6175 642c 2063 6f6e  t(com, baud, con
+00005c30: 6669 6729 0a20 2020 2020 2020 2020 2020  fig).           
+00005c40: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005c50: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005c60: 650a 0a20 2020 2064 6566 2066 696e 645f  e..    def find_
+00005c70: 636f 6d5f 706f 7274 2873 656c 662c 2062  com_port(self, b
+00005c80: 6175 643d 3131 3532 3030 293a 0a20 2020  aud=115200):.   
+00005c90: 2020 2020 2063 6f6d 506f 7274 7320 3d20       comPorts = 
+00005ca0: 7365 7269 616c 5f70 6f72 7473 2829 0a20  serial_ports(). 
+00005cb0: 2020 2020 2020 2063 6f6d 7320 3d20 5b5d         coms = []
+00005cc0: 0a20 2020 2020 2020 2066 6f72 2063 6f6d  .        for com
+00005cd0: 2069 6e20 636f 6d50 6f72 7473 3a0a 2020   in comPorts:.  
+00005ce0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005cf0: 662e 6368 6563 6b5f 636f 6d5f 706f 7274  f.check_com_port
+00005d00: 2863 6f6d 2c20 6261 7564 293a 0a20 2020  (com, baud):.   
+00005d10: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00005d20: 732e 6170 7065 6e64 2863 6f6d 290a 2020  s.append(com).  
+00005d30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005d40: 206c 656e 2863 6f6d 7329 203e 2031 3a0a   len(coms) > 1:.
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2027 5761 726e 696e 6720 2d20 6d6f     'Warning - mo
+00005d90: 7265 2074 6861 6e20 6f6e 6520 6261 7263  re than one barc
+00005da0: 6f64 6520 7363 616e 6e65 7220 666f 756e  ode scanner foun
+00005db0: 642c 2075 7369 6e67 2074 6865 2066 6972  d, using the fir
+00005dc0: 7374 2062 6172 636f 6465 2073 6361 6e6e  st barcode scann
+00005dd0: 6572 2e27 290a 0a20 2020 2020 2020 2069  er.')..        i
+00005de0: 6620 6c65 6e28 636f 6d73 2920 3e20 303a  f len(coms) > 0:
+00005df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005e00: 7572 6e20 636f 6d73 5b30 5d0a 2020 2020  urn coms[0].    
+00005e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005e20: 2020 2020 2020 7072 696e 7428 2745 7272        print('Err
+00005e30: 6f72 202d 2063 6f75 6c64 206e 6f74 2066  or - could not f
+00005e40: 696e 6420 6261 7263 6f64 6520 7363 616e  ind barcode scan
+00005e50: 6e65 722e 2729 0a20 2020 2020 2020 2020  ner.').         
+00005e60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00005e70: 2020 2020 6465 6620 6368 6563 6b5f 636f      def check_co
+00005e80: 6d5f 706f 7274 2873 656c 662c 2063 6f6d  m_port(self, com
+00005e90: 3d4e 6f6e 652c 2062 6175 643d 3131 3532  =None, baud=1152
+00005ea0: 3030 293a 0a20 2020 2020 2020 2069 735f  00):.        is_
+00005eb0: 6261 725f 7363 616e 203d 2054 7275 650a  bar_scan = True.
+00005ec0: 2020 2020 2020 2020 636c 6f73 655f 706f          close_po
+00005ed0: 7274 203d 2046 616c 7365 0a20 2020 2020  rt = False.     
+00005ee0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+00005ef0: 735f 6f70 656e 2829 2061 6e64 2063 6f6d  s_open() and com
+00005f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00005f10: 2020 2020 2020 2020 2020 636c 6f73 655f            close_
+00005f20: 706f 7274 203d 2054 7275 650a 2020 2020  port = True.    
+00005f30: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00005f40: 6961 6c20 3d20 7365 7269 616c 2e53 6572  ial = serial.Ser
+00005f50: 6961 6c28 636f 6d2c 2062 6175 642c 2074  ial(com, baud, t
+00005f60: 696d 656f 7574 3d30 2e35 290a 2020 2020  imeout=0.5).    
+00005f70: 2020 2020 656c 6966 206e 6f74 2073 656c      elif not sel
+00005f80: 662e 6973 5f6f 7065 6e28 293a 0a20 2020  f.is_open():.   
+00005f90: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00005fa0: 4261 7263 6f64 6553 6361 6e6e 6572 202d  BarcodeScanner -
+00005fb0: 2063 6865 636b 5f63 6f6d 5f70 6f72 743a   check_com_port:
+00005fc0: 204d 6973 7369 6e67 2063 6f6d 2070 6f72   Missing com por
+00005fd0: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
+00005fe0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00005ff0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00006000: 6d61 6e75 616c 5f63 6f6e 6669 6775 7265  manual_configure
+00006010: 285b 2751 5259 5044 4e27 5d29 0a20 2020  (['QRYPDN']).   
+00006020: 2020 2020 2069 6620 6e6f 7420 274e 4c53       if not 'NLS
+00006030: 2d4e 3127 2069 6e20 7374 7228 7265 7329  -N1' in str(res)
+00006040: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
+00006050: 5f62 6172 5f73 6361 6e20 3d20 4661 6c73  _bar_scan = Fals
+00006060: 650a 2020 2020 2020 2020 6966 2063 6c6f  e.        if clo
+00006070: 7365 5f70 6f72 743a 0a20 2020 2020 2020  se_port:.       
+00006080: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+00006090: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+000060a0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000060b0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000060c0: 2072 6574 7572 6e20 6973 5f62 6172 5f73   return is_bar_s
+000060d0: 6361 6e0a 0a20 2020 2064 6566 2063 6c6f  can..    def clo
+000060e0: 7365 5f70 6f72 7428 7365 6c66 293a 0a20  se_port(self):. 
+000060f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00006100: 6572 6961 6c2e 6973 4f70 656e 2829 3a0a  erial.isOpen():.
+00006110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006120: 2e73 6572 6961 6c2e 636c 6f73 6528 290a  .serial.close().
+00006130: 0a20 2020 2064 6566 2069 735f 6f70 656e  .    def is_open
+00006140: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006150: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00006160: 2072 6573 203d 2073 656c 662e 6d61 6e75   res = self.manu
+00006170: 616c 5f63 6f6e 6669 6775 7265 285b 2751  al_configure(['Q
+00006180: 5259 5044 4e27 5d29 0a20 2020 2020 2020  RYPDN']).       
+00006190: 2020 2020 2069 6620 274e 4c53 2d4e 3127       if 'NLS-N1'
+000061a0: 2069 6e20 7374 7228 7265 7329 3a0a 2020   in str(res):.  
+000061b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000061c0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000061d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000061e0: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
+000061f0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00006200: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00006210: 2064 6566 2063 6f6e 6669 6775 7265 2873   def configure(s
+00006220: 656c 662c 2069 6c6c 5363 6e3d 2731 272c  elf, illScn='1',
+00006230: 2061 6d6c 456e 613d 2730 272c 2067 7262   amlEna='0', grb
+00006240: 456e 613d 2730 272c 2067 7262 566c 6c3d  Ena='0', grbVll=
+00006250: 2732 272c 2061 7473 456e 613d 2730 272c  '2', atsEna='0',
+00006260: 2061 7473 4475 723d 2733 3630 3030 272c   atsDur='36000',
+00006270: 2073 636e 4d6f 643d 2730 272c 0a20 2020   scnMod='0',.   
+00006280: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00006290: 7762 456e 613d 2730 2729 3a0a 2020 2020  wbEna='0'):.    
+000062a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000062b0: 696c 6c53 636e 202d 2069 6c6c 756d 696e  illScn - illumin
+000062c0: 6174 696f 6e3a 2020 2020 302d 6f66 662c  ation:    0-off,
+000062d0: 2031 2d6e 6f72 6d61 6c2c 2032 2d61 6c77   1-normal, 2-alw
+000062e0: 6179 7320 6f6e 0a20 2020 2020 2020 2061  ays on.        a
+000062f0: 6d6c 456e 6120 2d20 6169 6d69 6e67 3a20  mlEna - aiming: 
+00006300: 2020 2020 2020 2020 2030 2d6f 6666 2c20           0-off, 
+00006310: 312d 6e6f 726d 616c 2c20 322d 616c 7761  1-normal, 2-alwa
+00006320: 7973 206f 6e0a 2020 2020 2020 2020 7077  ys on.        pw
+00006330: 6245 6e61 202d 2070 6f77 6572 206f 6e20  bEna - power on 
+00006340: 6265 6570 2020 2020 302d 6f66 662c 2031  beep    0-off, 1
+00006350: 2d6f 6e0a 2020 2020 2020 2020 6772 6245  -on.        grbE
+00006360: 6e61 202d 2067 6f6f 6420 7265 6164 2062  na - good read b
+00006370: 6565 7020 2020 302d 6f66 662c 2031 2d6f  eep   0-off, 1-o
+00006380: 6e0a 2020 2020 2020 2020 6174 7345 6e61  n.        atsEna
+00006390: 202d 2061 7574 6f20 736c 6565 7020 2020   - auto sleep   
+000063a0: 2020 2020 302d 6469 7361 626c 652c 2031      0-disable, 1
+000063b0: 2d65 6e61 626c 650a 2020 2020 2020 2020  -enable.        
+000063c0: 6174 7344 7572 202d 2073 6c65 6570 2064  atsDur - sleep d
+000063d0: 7572 6174 696f 6e20 2020 312d 3336 3030  uration   1-3600
+000063e0: 3020 5b73 6563 5d0a 2020 2020 2020 2020  0 [sec].        
+000063f0: 7363 6e4d 6f64 202d 2073 6361 6e20 6d6f  scnMod - scan mo
+00006400: 6465 2020 2020 2020 2020 302d 6c65 7665  de        0-leve
+00006410: 6c20 6d6f 6465 2c20 322d 7365 6e73 6520  l mode, 2-sense 
+00006420: 6d6f 6465 2c20 332d 636f 6e74 696e 756f  mode, 3-continuo
+00006430: 7573 206d 6f64 652c 2037 2d62 6174 6368  us mode, 7-batch
+00006440: 206d 6f64 650a 2020 2020 2020 2020 2727   mode.        ''
+00006450: 270a 2020 2020 2020 2020 736c 6565 7028  '.        sleep(
+00006460: 302e 3129 0a20 2020 2020 2020 2070 6172  0.1).        par
+00006470: 616d 7320 3d20 7b27 494c 4c53 434e 273a  ams = {'ILLSCN':
+00006480: 2069 6c6c 5363 6e2c 2027 414d 4c45 4e41   illScn, 'AMLENA
+00006490: 273a 2061 6d6c 456e 612c 2027 4752 4245  ': amlEna, 'GRBE
+000064a0: 4e41 273a 2067 7262 456e 612c 2027 4154  NA': grbEna, 'AT
+000064b0: 5345 4e41 273a 2061 7473 456e 612c 0a20  SENA': atsEna,. 
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064d0: 2027 4752 4256 4c4c 273a 2067 7262 566c   'GRBVLL': grbVl
+000064e0: 6c2c 2027 4154 5344 5552 273a 2061 7473  l, 'ATSDUR': ats
+000064f0: 4475 722c 2027 5343 4e4d 4f44 273a 2073  Dur, 'SCNMOD': s
+00006500: 636e 4d6f 642c 2027 5057 4245 4e41 273a  cnMod, 'PWBENA':
+00006510: 2070 7762 456e 617d 0a20 2020 2020 2020   pwbEna}.       
+00006520: 2070 6172 616d 7320 3d20 5b6b 6579 202b   params = [key +
+00006530: 2076 616c 7565 2066 6f72 206b 6579 2c20   value for key, 
+00006540: 7661 6c75 6520 696e 2070 6172 616d 732e  value in params.
+00006550: 6974 656d 7328 295d 0a20 2020 2020 2020  items()].       
+00006560: 2074 2c20 6973 5375 6363 6573 7320 3d20   t, isSuccess = 
+00006570: 7365 6c66 2e6d 616e 7561 6c5f 636f 6e66  self.manual_conf
+00006580: 6967 7572 6528 7061 7261 6d73 290a 2020  igure(params).  
+00006590: 2020 2020 2020 6966 2069 7353 7563 6365        if isSucce
+000065a0: 7373 2061 6e64 2073 656c 662e 6c6f 675f  ss and self.log_
+000065b0: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
+000065c0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000065d0: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+000065e0: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+000065f0: 7d29 2063 6f6e 6669 6775 7265 6420 7375  }) configured su
+00006600: 6363 6573 7366 756c 6c79 2e27 290a 2020  ccessfully.').  
+00006610: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
+00006620: 7353 7563 6365 7373 3a0a 2020 2020 2020  sSuccess:.      
+00006630: 2020 2020 2020 7072 696e 7428 6627 4261        print(f'Ba
+00006640: 7263 6f64 6520 7363 616e 6e65 7220 287b  rcode scanner ({
+00006650: 7365 6c66 2e63 6f6d 7d29 2063 6f6e 6669  self.com}) confi
+00006660: 6775 7261 7469 6f6e 2066 6169 6c65 642e  guration failed.
+00006670: 2729 0a0a 2020 2020 6465 6620 7265 7374  ')..    def rest
+00006680: 6f72 655f 616c 6c5f 6661 6374 6f72 795f  ore_all_factory_
+00006690: 6465 6661 756c 7473 2873 656c 6629 3a0a  defaults(self):.
+000066a0: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
+000066b0: 3129 0a20 2020 2020 2020 2070 6172 616d  1).        param
+000066c0: 7320 3d20 7b27 4641 4344 4546 273a 2027  s = {'FACDEF': '
+000066d0: 277d 0a20 2020 2020 2020 2070 6172 616d  '}.        param
+000066e0: 7320 3d20 5b6b 6579 202b 2076 616c 7565  s = [key + value
+000066f0: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00006700: 696e 2070 6172 616d 732e 6974 656d 7328  in params.items(
+00006710: 295d 0a20 2020 2020 2020 2074 2c20 6973  )].        t, is
+00006720: 5375 6363 6573 7320 3d20 7365 6c66 2e6d  Success = self.m
+00006730: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006740: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+00006750: 6966 2069 7353 7563 6365 7373 2061 6e64  if isSuccess and
+00006760: 2073 656c 662e 6c6f 675f 7479 7065 2021   self.log_type !
+00006770: 3d20 274e 4f5f 4c4f 4727 3a0a 2020 2020  = 'NO_LOG':.    
+00006780: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00006790: 4261 7263 6f64 6520 7363 616e 6e65 7220  Barcode scanner 
+000067a0: 287b 7365 6c66 2e63 6f6d 7d29 2072 6573  ({self.com}) res
+000067b0: 746f 7265 6420 6661 6374 6f72 7920 6465  tored factory de
+000067c0: 6661 756c 7420 7375 6363 6573 7366 756c  fault successful
+000067d0: 6c79 2e27 290a 2020 2020 2020 2020 656c  ly.').        el
+000067e0: 6966 206e 6f74 2069 7353 7563 6365 7373  if not isSuccess
+000067f0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00006800: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+00006810: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+00006820: 7d29 2072 6573 746f 7265 6420 6661 6374  }) restored fact
+00006830: 6f72 7920 6465 6661 756c 7420 6661 696c  ory default fail
+00006840: 6564 2e27 290a 0a20 2020 2064 6566 206d  ed.')..    def m
+00006850: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006860: 7365 6c66 2c20 7061 7261 6d73 293a 0a20  self, params):. 
+00006870: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006880: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00006890: 7320 3d20 7365 6c66 2e70 7265 6669 7820  s = self.prefix 
+000068a0: 2b20 273b 272e 6a6f 696e 2870 6172 616d  + ';'.join(param
+000068b0: 7329 202b 2073 656c 662e 7375 6666 6978  s) + self.suffix
+000068c0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+000068d0: 7269 616c 2e66 6c75 7368 496e 7075 7428  rial.flushInput(
+000068e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000068f0: 6572 6961 6c2e 666c 7573 684f 7574 7075  erial.flushOutpu
+00006900: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00006910: 2e73 6572 6961 6c2e 7772 6974 6528 7374  .serial.write(st
+00006920: 722e 656e 636f 6465 2863 6f6e 6669 6773  r.encode(configs
+00006930: 2929 0a20 2020 2020 2020 2073 6c65 6570  )).        sleep
+00006940: 2830 2e31 290a 2020 2020 2020 2020 742c  (0.1).        t,
+00006950: 2069 7353 7563 6365 7373 203d 2073 656c   isSuccess = sel
+00006960: 662e 7472 6967 6765 725f 7374 6f70 5f73  f.trigger_stop_s
+00006970: 6574 7469 6e67 7328 290a 2020 2020 2020  ettings().      
+00006980: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00006990: 2020 2020 2072 6574 7572 6e20 742c 2069       return t, i
+000069a0: 7353 7563 6365 7373 0a0a 2020 2020 6465  sSuccess..    de
+000069b0: 6620 7363 616e 2873 656c 6629 3a0a 2020  f scan(self):.  
+000069c0: 2020 2020 2020 2320 7072 696e 7428 2261        # print("a
+000069d0: 6e61 6c6f 675f 7472 6967 6765 725f 7365  nalog_trigger_se
+000069e0: 7474 696e 6722 290a 2020 2020 2020 2020  tting").        
+000069f0: 7365 6c66 2e73 6572 6961 6c2e 7772 6974  self.serial.writ
+00006a00: 6528 6222 5c78 3162 5c78 3331 2229 0a20  e(b"\x1b\x31"). 
+00006a10: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006a20: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+00006a30: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+00006a40: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+00006a50: 2074 203d 2073 656c 662e 7365 7269 616c   t = self.serial
+00006a60: 2e72 6561 645f 616c 6c28 290a 2020 2020  .read_all().    
+00006a70: 2020 2020 2320 7072 696e 7428 7429 0a20      # print(t). 
+00006a80: 2020 2020 2020 2072 6574 7572 6e20 740a         return t.
+00006a90: 0a20 2020 2064 6566 2073 6361 6e5f 616e  .    def scan_an
+00006aa0: 645f 666c 7573 6828 7365 6c66 293a 0a20  d_flush(self):. 
+00006ab0: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00006ac0: 616c 2e66 6c75 7368 496e 7075 7428 290a  al.flushInput().
+00006ad0: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00006ae0: 6961 6c2e 666c 7573 684f 7574 7075 7428  ial.flushOutput(
+00006af0: 290a 2020 2020 2020 2020 7420 3d20 7365  ).        t = se
+00006b00: 6c66 2e73 6361 6e28 290a 2020 2020 2020  lf.scan().      
+00006b10: 2020 7365 6c66 2e73 6572 6961 6c2e 666c    self.serial.fl
+00006b20: 7573 6849 6e70 7574 2829 0a20 2020 2020  ushInput().     
+00006b30: 2020 2073 656c 662e 7365 7269 616c 2e66     self.serial.f
+00006b40: 6c75 7368 4f75 7470 7574 2829 0a20 2020  lushOutput().   
+00006b50: 2020 2020 2074 436c 6561 6e20 3d20 7374       tClean = st
+00006b60: 7228 7429 2e73 706c 6974 2827 5c5c 7827  r(t).split('\\x'
+00006b70: 295b 2d31 5d0a 2020 2020 2020 2020 6966  )[-1].        if
+00006b80: 2074 436c 6561 6e2e 7374 6172 7473 7769   tClean.startswi
+00006b90: 7468 2827 3036 2729 3a0a 2020 2020 2020  th('06'):.      
+00006ba0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bb0: 436c 6561 6e5b 323a 5d0a 2020 2020 2020  Clean[2:].      
+00006bc0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bd0: 436c 6561 6e2e 7374 7269 7028 2227 5c5c  Clean.strip("'\\
+00006be0: 6e5c 5c72 2229 0a20 2020 2020 2020 2020  n\\r").         
+00006bf0: 2020 2074 436c 6561 6e20 3d20 7443 6c65     tClean = tCle
+00006c00: 616e 2e73 706c 6974 2827 5c5c 6e27 295b  an.split('\\n')[
+00006c10: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
+00006c20: 7443 6c65 616e 203d 2074 436c 6561 6e2e  tClean = tClean.
+00006c30: 7370 6c69 7428 275c 5c72 2729 5b2d 315d  split('\\r')[-1]
+00006c40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006c50: 7572 6e20 7443 6c65 616e 0a20 2020 2020  urn tClean.     
+00006c60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006c70: 2020 2020 2070 7269 6e74 2827 5761 726e       print('Warn
+00006c80: 696e 6720 2d20 6e6f 7420 7265 6365 6976  ing - not receiv
+00006c90: 6564 2041 434b 2066 726f 6d20 6261 7263  ed ACK from barc
+00006ca0: 6f64 6520 7363 616e 6e65 722e 2729 0a20  ode scanner.'). 
+00006cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006cc0: 6e20 7374 7228 7429 2e73 706c 6974 2827  n str(t).split('
+00006cd0: 5c5c 7827 295b 2d31 5d0a 0a20 2020 2064  \\x')[-1]..    d
+00006ce0: 6566 2073 6361 6e5f 6578 745f 6964 2873  ef scan_ext_id(s
+00006cf0: 656c 662c 2073 6361 6e44 7572 3d30 2e35  elf, scanDur=0.5
+00006d00: 2c20 5661 6c69 6461 7465 436e 743d 3329  , ValidateCnt=3)
+00006d10: 3a0a 2020 2020 2020 2020 6261 7263 6f64  :.        barcod
+00006d20: 6552 6561 6420 3d20 2727 0a20 2020 2020  eRead = ''.     
+00006d30: 2020 2062 6172 636f 6465 7320 3d20 5b5d     barcodes = []
+00006d40: 0a20 2020 2020 2020 2073 7461 7274 5469  .        startTi
+00006d50: 6d65 203d 2074 696d 6528 290a 2020 2020  me = time().    
+00006d60: 2020 2020 7768 696c 6520 2828 7469 6d65      while ((time
+00006d70: 2829 202d 2073 7461 7274 5469 6d65 2920  () - startTime) 
+00006d80: 3c20 7363 616e 4475 7229 3a0a 2020 2020  < scanDur):.    
+00006d90: 2020 2020 2020 2020 6261 7263 6f64 6552          barcodeR
+00006da0: 6561 6420 3d20 7365 6c66 2e73 6361 6e5f  ead = self.scan_
+00006db0: 616e 645f 666c 7573 6828 290a 2020 2020  and_flush().    
+00006dc0: 2020 2020 2020 2020 2320 6261 7263 6f64          # barcod
+00006dd0: 6552 6561 6420 3d20 7374 7228 7429 0a20  eRead = str(t). 
+00006de0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006df0: 6e28 6261 7263 6f64 6552 6561 6429 203c  n(barcodeRead) <
+00006e00: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
+00006e10: 2020 2020 6261 7263 6f64 6552 6561 6420      barcodeRead 
+00006e20: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00006e30: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00006e40: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006e50: 6e28 6261 7263 6f64 6573 2920 3c20 5661  n(barcodes) < Va
+00006e60: 6c69 6461 7465 436e 743a 0a20 2020 2020  lidateCnt:.     
+00006e70: 2020 2020 2020 2020 2020 2062 6172 636f             barco
+00006e80: 6465 732e 6170 7065 6e64 2862 6172 636f  des.append(barco
+00006e90: 6465 5265 6164 290a 2020 2020 2020 2020  deRead).        
+00006ea0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00006eb0: 0a0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00006ec0: 7263 6f64 6552 6561 6420 3d20 6d6f 6465  rcodeRead = mode
+00006ed0: 2862 6172 636f 6465 7329 0a20 2020 2020  (barcodes).     
+00006ee0: 2020 2020 2020 2066 756c 6c44 6174 6120         fullData 
+00006ef0: 3d20 6375 7249 6420 3d20 7265 656c 4964  = curId = reelId
+00006f00: 203d 2067 7469 6e20 3d20 6261 7263 6f64   = gtin = barcod
+00006f10: 6552 6561 640a 2020 2020 2020 2020 2020  eRead.          
+00006f20: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00006f30: 2020 2020 2020 2069 6620 2729 2720 696e         if ')' in
+00006f40: 2066 756c 6c44 6174 613a 0a20 2020 2020   fullData:.     
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00006f60: 7469 6e20 3d20 2729 272e 6a6f 696e 2866  tin = ')'.join(f
+00006f70: 756c 6c44 6174 612e 7370 6c69 7428 2729  ullData.split(')
+00006f80: 2729 5b3a 325d 2920 2b20 2729 270a 2020  ')[:2]) + ')'.  
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 7461 6744 6174 6120 3d20 6675 6c6c    tagData = full
+00006fb0: 4461 7461 2e73 706c 6974 2827 2927 295b  Data.split(')')[
+00006fc0: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+00006fd0: 2020 2065 6c73 653a 2020 2320 6774 696e     else:  # gtin
+00006fe0: 2077 6974 686f 7574 2070 6172 656e 7468   without parenth
+00006ff0: 6573 6973 0a20 2020 2020 2020 2020 2020  esis.           
+00007000: 2020 2020 2020 2020 2067 7469 6e20 3d20           gtin = 
+00007010: 6675 6c6c 4461 7461 5b30 3a31 385d 0a20  fullData[0:18]. 
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2074 6167 4461 7461 203d 2066 756c     tagData = ful
+00007040: 6c44 6174 615b 3138 3a5d 0a20 2020 2020  lData[18:].     
+00007050: 2020 2020 2020 2020 2020 2063 7572 4964             curId
+00007060: 203d 2074 6167 4461 7461 2e73 706c 6974   = tagData.split
+00007070: 2827 5427 295b 315d 2e73 7472 6970 2822  ('T')[1].strip("
+00007080: 2720 2229 2e73 706c 6974 2827 2827 295b  ' ").split('(')[
+00007090: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+000070a0: 2020 2072 6565 6c49 6420 3d20 7461 6744     reelId = tagD
+000070b0: 6174 612e 7370 6c69 7428 2754 2729 5b30  ata.split('T')[0
+000070c0: 5d2e 7374 7269 7028 2227 2022 290a 2020  ].strip("' ").  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000070e0: 7475 726e 2066 756c 6c44 6174 612c 2063  turn fullData, c
+000070f0: 7572 4964 2c20 7265 656c 4964 2c20 6774  urId, reelId, gt
+00007100: 696e 0a20 2020 2020 2020 2020 2020 2065  in.            e
+00007110: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00007120: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00007130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007140: 6675 6c6c 4461 7461 2c20 6375 7249 642c  fullData, curId,
+00007150: 2072 6565 6c49 642c 2067 7469 6e0a 0a20   reelId, gtin.. 
+00007160: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00007170: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
+00007180: 4e6f 6e65 0a0a 2020 2020 6465 6620 6175  None..    def au
+00007190: 746f 5f73 6361 6e28 7365 6c66 293a 0a20  to_scan(self):. 
+000071a0: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+000071b0: 4175 746f 6d61 7469 6320 7265 6164 696e  Automatic readin
+000071c0: 6720 7365 7474 696e 6773 2229 0a20 2020  g settings").   
+000071d0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000071e0: 2e77 7269 7465 2862 225c 7831 625c 7833  .write(b"\x1b\x3
+000071f0: 3222 290a 2020 2020 2020 2020 736c 6565  2").        slee
+00007200: 7028 302e 3129 0a20 2020 2020 2020 2074  p(0.1).        t
+00007210: 203d 2073 656c 662e 7365 7269 616c 2e72   = self.serial.r
+00007220: 6561 645f 616c 6c28 290a 2020 2020 2020  ead_all().      
+00007230: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00007240: 2020 2020 2072 6574 7572 6e20 740a 0a20       return t.. 
+00007250: 2020 2064 6566 2074 7269 6767 6572 5f73     def trigger_s
+00007260: 746f 705f 7365 7474 696e 6773 2873 656c  top_settings(sel
+00007270: 6629 3a0a 2020 2020 2020 2020 2320 7072  f):.        # pr
+00007280: 696e 7428 2254 7269 6767 6572 5f73 746f  int("Trigger_sto
+00007290: 705f 7365 7474 696e 6773 2229 0a20 2020  p_settings").   
+000072a0: 2020 2020 2023 2073 6c65 6570 2830 2e31       # sleep(0.1
+000072b0: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+000072c0: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+000072d0: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+000072e0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+000072f0: 2020 2020 7420 3d20 7365 6c66 2e73 6572      t = self.ser
+00007300: 6961 6c2e 7265 6164 5f61 6c6c 2829 0a20  ial.read_all(). 
+00007310: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00007320: 290a 2020 2020 2020 2020 2320 7072 696e  ).        # prin
+00007330: 7428 7429 0a20 2020 2020 2020 2061 636b  t(t).        ack
+00007340: 7320 3d20 7374 7228 7429 2e73 706c 6974  s = str(t).split
+00007350: 2827 3b27 295b 3a2d 315d 0a20 2020 2020  (';')[:-1].     
+00007360: 2020 2069 7353 7563 6365 7373 203d 2061     isSuccess = a
+00007370: 6c6c 285b 5472 7565 2069 6620 6163 6b2e  ll([True if ack.
+00007380: 656e 6473 7769 7468 2827 5c5c 7830 3627  endswith('\\x06'
+00007390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000073a0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000073b0: 4661 6c73 6520 666f 7220 6163 6b20 696e  False for ack in
+000073c0: 2061 636b 735d 290a 2020 2020 2020 2020   acks]).        
+000073d0: 7265 7475 726e 2074 2c20 6973 5375 6363  return t, isSucc
+000073e0: 6573 730a 0a0a 636c 6173 7320 596f 6374  ess...class Yoct
+000073f0: 6f54 656d 7065 7261 7475 7265 5365 6e73  oTemperatureSens
+00007400: 6f72 286f 626a 6563 7429 3a0a 2020 2020  or(object):.    
+00007410: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007420: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00007430: 2e73 656e 736f 7220 3d20 4e6f 6e65 0a20  .sensor = None. 
+00007440: 2020 2020 2020 2065 7272 6d73 6720 3d20         errmsg = 
+00007450: 5952 6566 5061 7261 6d28 290a 2020 2020  YRefParam().    
+00007460: 2020 2020 2320 5365 7475 7020 7468 6520      # Setup the 
+00007470: 4150 4920 746f 2075 7365 206c 6f63 616c  API to use local
+00007480: 2055 5342 2064 6576 6963 6573 0a20 2020   USB devices.   
+00007490: 2020 2020 2069 6620 5941 5049 2e52 6567       if YAPI.Reg
+000074a0: 6973 7465 7248 7562 2822 7573 6222 2c20  isterHub("usb", 
+000074b0: 6572 726d 7367 2920 213d 2059 4150 492e  errmsg) != YAPI.
+000074c0: 5355 4343 4553 533a 0a20 2020 2020 2020  SUCCESS:.       
+000074d0: 2020 2020 2072 6169 7365 2045 7175 6970       raise Equip
+000074e0: 6d65 6e74 4572 726f 7228 2779 6f63 746f  mentError('yocto
+000074f0: 2074 656d 7065 7261 7475 7265 2073 656e   temperature sen
+00007500: 736f 7220 676f 7420 696e 6974 2065 7272  sor got init err
+00007510: 6f72 3a20 7b7d 272e 666f 726d 6174 2865  or: {}'.format(e
+00007520: 7272 6d73 672e 7661 6c75 6529 290a 0a20  rrmsg.value)).. 
+00007530: 2020 2064 6566 2063 6f6e 6e65 6374 2873     def connect(s
+00007540: 656c 662c 2074 6172 6765 743d 2761 6e79  elf, target='any
+00007550: 2729 3a0a 2020 2020 2020 2020 6966 2074  '):.        if t
+00007560: 6172 6765 7420 3d3d 2027 616e 7927 3a0a  arget == 'any':.
+00007570: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00007580: 7472 6965 7665 2061 6e79 2074 656d 7065  trieve any tempe
+00007590: 7261 7475 7265 2073 656e 736f 720a 2020  rature sensor.  
+000075a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000075b0: 656e 736f 7220 3d20 5954 656d 7065 7261  ensor = YTempera
+000075c0: 7475 7265 2e46 6972 7374 5465 6d70 6572  ture.FirstTemper
+000075d0: 6174 7572 6528 290a 2020 2020 2020 2020  ature().        
+000075e0: 656c 6966 2074 6172 6765 7420 3d3d 2027  elif target == '
+000075f0: 273a 0a20 2020 2020 2020 2020 2020 2070  ':.            p
+00007600: 7269 6e74 2827 7370 6563 6966 6965 6420  rint('specified 
+00007610: 696e 7661 6c69 6420 7461 7267 6574 2729  invalid target')
+00007620: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007630: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00007640: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007650: 2020 2020 7365 6c66 2e73 656e 736f 7220      self.sensor 
+00007660: 3d20 5954 656d 7065 7261 7475 7265 2e46  = YTemperature.F
+00007670: 696e 6454 656d 7065 7261 7475 7265 2874  indTemperature(t
+00007680: 6172 6765 7420 2b20 272e 7465 6d70 6572  arget + '.temper
+00007690: 6174 7572 6527 290a 2020 2020 2020 2020  ature').        
+000076a0: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000076b0: 7320 4e6f 6e65 206f 7220 7365 6c66 2e67  s None or self.g
+000076c0: 6574 5f73 656e 736f 725f 6e61 6d65 2829  et_sensor_name()
+000076d0: 203d 3d20 2775 6e72 6573 6f6c 7665 6427   == 'unresolved'
+000076e0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000076f0: 696e 7428 274e 6f20 6d6f 6475 6c65 2063  int('No module c
+00007700: 6f6e 6e65 6374 6564 2729 0a20 2020 2020  onnected').     
+00007710: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00007720: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
+00007730: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007740: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
+00007750: 6566 2067 6574 5f73 656e 736f 725f 6e61  ef get_sensor_na
+00007760: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+00007770: 2020 6966 2073 656c 662e 7365 6e73 6f72    if self.sensor
+00007780: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007790: 2020 2020 2020 7072 696e 7428 276e 6f20        print('no 
+000077a0: 7365 6e73 6f72 2069 7320 636f 6e6e 6563  sensor is connec
+000077b0: 7465 642e 2074 7279 2074 6f20 6361 6c6c  ted. try to call
+000077c0: 2063 6f6e 6e65 6374 2829 2066 6972 7374   connect() first
+000077d0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+000077e0: 6574 7572 6e20 2727 0a0a 2020 2020 2020  eturn ''..      
+000077f0: 2020 7365 6e73 6f72 5f73 7472 203d 2073    sensor_str = s
+00007800: 656c 662e 7365 6e73 6f72 2e64 6573 6372  elf.sensor.descr
+00007810: 6962 6528 290a 2020 2020 2020 2020 6e61  ibe().        na
+00007820: 6d65 5f73 7472 203d 2073 656e 736f 725f  me_str = sensor_
+00007830: 7374 722e 7370 6c69 7428 273d 2729 5b31  str.split('=')[1
+00007840: 5d2e 7370 6c69 7428 272e 2729 5b30 5d0a  ].split('.')[0].
+00007850: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00007860: 616d 655f 7374 720a 0a20 2020 2064 6566  ame_str..    def
+00007870: 2067 6574 5f74 656d 7065 7261 7475 7265   get_temperature
+00007880: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007890: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000078a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000078b0: 2020 2020 7072 696e 7428 2773 656e 736f      print('senso
+000078c0: 7220 6973 206e 6f74 2063 6f6e 6e65 6374  r is not connect
+000078d0: 6564 2e20 7472 7920 746f 2063 616c 6c20  ed. try to call 
+000078e0: 636f 6e6e 6563 7428 2920 6669 7273 7427  connect() first'
+000078f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007900: 7475 726e 2066 6c6f 6174 2827 6e61 6e27  turn float('nan'
+00007910: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00007920: 2028 7365 6c66 2e73 656e 736f 722e 6973   (self.sensor.is
+00007930: 4f6e 6c69 6e65 2829 293a 0a20 2020 2020  Online()):.     
+00007940: 2020 2020 2020 2070 7269 6e74 2827 7365         print('se
+00007950: 6e73 6f72 2069 7320 6e6f 7420 636f 6e6e  nsor is not conn
+00007960: 6563 7465 6420 6f72 2064 6973 636f 6e6e  ected or disconn
+00007970: 6563 7465 6420 6475 7269 6e67 2072 756e  ected during run
+00007980: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+00007990: 6574 7572 6e20 666c 6f61 7428 276e 616e  eturn float('nan
+000079a0: 2729 0a0a 2020 2020 2020 2020 7265 7475  ')..        retu
+000079b0: 726e 2073 656c 662e 7365 6e73 6f72 2e67  rn self.sensor.g
+000079c0: 6574 5f63 7572 7265 6e74 5661 6c75 6528  et_currentValue(
+000079d0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+000079e0: 7468 6f64 0a20 2020 2064 6566 2065 7869  thod.    def exi
+000079f0: 745f 6170 7028 293a 0a20 2020 2020 2020  t_app():.       
+00007a00: 2059 4150 492e 4672 6565 4150 4928 290a   YAPI.FreeAPI().
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/tester_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/tester_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 from threading import Event
 import numpy as np
 from queue import Empty
 import sys
 from os.path import dirname
 import PySimpleGUI as SimGUI
 import pathlib
-from wiliot_api.manufacturing.manufacturing import ManufacturingClient, WiliotCloudError
+from wiliot_api import ManufacturingClient, WiliotCloudError
 from wiliot_testers.wiliot_tester_tag_result import *
 from wiliot_core import check_user_config_is_ok
 # TODO: consider to use for cross platform directories
 
 
 ###########################################
 #            Tester Management            #
@@ -264,32 +264,26 @@
         os.makedirs(folder_path)
     
     file_exists = os.path.isfile(file_path)
     if not file_exists:
         # save the default values to json
         with open(file_path, "w") as out_file:
             json.dump(default_values, out_file)
-        f = open(file_path)
-        json_content = json.load(f)
+        with open(file_path, 'r') as f:
+            json_content = json.load(f)
         return json_content
     else:
-        f = open(file_path)
-        # returns JSON object as
-        # a dictionary
-        json_content = json.load(f)
-        
-        if len(json_content['sgtin']) == 0 or len(json_content['reelNumManually']) == 0:
-            f.close()
-            with open(file_path, "w") as out_file:
-                json.dump(default_values, out_file)
-            f = open(file_path)
-            json_content = json.load(f)
-        else:
-            f = open(file_path)
+        with open(file_path, 'r') as f:
             json_content = json.load(f)
+
+        for k, v in default_values.items():
+            if k not in json_content.keys():
+                json_content[k] = v
+        with open(file_path, "w") as out_file:
+            json.dump(json_content, out_file)
         return json_content
 
 
 def printing_func(str_to_print, logging_entity, lock_print=None, do_log=True, logger_type='info', logger_name=None):
     """
     print and log
     :type str_to_print: string
@@ -751,15 +745,15 @@
 
 ###########################################
 #              Cloud Functions            #
 ###########################################
 
 def upload_to_cloud_api(batch_name, tester_type, run_data_csv_name=None, tags_data_csv_name=None, to_logging=False,
                         env='', is_batch_name_inside_logs_folder=True, logger_=None, is_path=False,
-                        client=None, packets_instead_tags=False):
+                        client=None, packets_instead_tags=False, owner_id='wiliot-ops'):
     """
     uploads a tester log to Wiliot cloud
     :type batch_name: string
     :param batch_name: folder name of the relevant log
     :type run_data_csv_name: string
     :param run_data_csv_name: name of desired run_data log to upload,
                               should contain 'run_data' and end with .csv
@@ -789,15 +783,15 @@
         logger.warning('Unsupported run_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
         return
     if tags_data_csv_name is not None and 'packets_data' not in tags_data_csv_name and \
             'tags_data' not in tags_data_csv_name:
         logger.warning('Unsupported tags_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
         return
 
-    file_path, api_key, is_successful = check_user_config_is_ok(env=env)
+    file_path, api_key, is_successful = check_user_config_is_ok(env=env, owner_id=owner_id)
     if env == 'prod':
         env = ''
     if not is_successful:
         logger.warning('could not extract user credentials. please check warnings')
         return
     if client is None:
         client = ManufacturingClient(api_key=api_key, env=env, logger_=logger.name)
@@ -1431,16 +1425,16 @@
                 elif tester_type.value == TesterName.CONVERSION.value:
                     added_headers = []
                 elif tester_type.value == TesterName.SAMPLE.value:
                     added_headers = ['responded', 'responding[%]', 'passed[%]', 'testStatus',
                                      'operator', 'testTime', 'runStartTime', 'runEndTime', 'antennaType',
                                      'surface', 'numChambers', 'gwVersion', 'pyWiliotVersion',
                                      'bleAttenuation', 'loraAttenuation', 'testTimeProfilePeriod',
-                                     'testTimeProfileOnTime', 'ttfpAvg', 'tbpAvg', 'rssiAvg', 'maxTtfp',
-                                     'controlLimits', 'hwVersion']
+                                     'testTimeProfileOnTime', 'ttfpAvg', 'tbpAvg', 'tbpStd', 'rssiAvg', 'maxTtfp',
+                                     'controlLimits', 'hwVersion', 'sub1gFrequency']
                 else:
                     added_headers = []
             elif header_type.value == HeaderType.TAG.value:
                 if tester_type.value == TesterName.OFFLINE.value:
                     added_headers = ['externalId']
                     if self.temperature_sensor_enable:
                         added_headers.append('temperatureFromSensor')
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/utils/get_version.py` & `wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_log.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_tag_result.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,24 +89,14 @@
 
 class ConversionTypes(Enum):
     NOT_CONVERTED = 'Unconverted'
     STANDARD = 'Regular Conversion'
     DURABLE = 'Durable Conversion'
 
 
-class InlayTypes(Enum):
-    TEO_086 = '086'
-    TIKI_096 = '096'
-    TIKI_099 = '099'
-    BATTERY_107 = '107'
-    TIKI_117 = '117'
-    TIKI_121 = '121'
-    TIKI_122_NAP = '122'
-
-
 class SurfaceTypes(Enum):
     AIR = 'air'
     CARDBOARD = 'cardboard'
     RPC = 'RPC'
     ER3 = 'Er3'
     ER3_5 = 'Er3.5'
     ER5 = 'Er5'
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/wiliot_tester_tag_test.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
    (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 """
 import logging
 import time
 import os
 import threading
 import json
-import pandas as pd
 
 from wiliot_core import WiliotDir
 from wiliot_core import WiliotGateway, ActionType, DataType, valid_output_power_vals
 from wiliot_core import PacketList
 from wiliot_testers.wiliot_tester_tag_result import *
 
 supported_gw_version = [3, 5, 2]
@@ -90,15 +89,15 @@
     """
     Wiliot Tags Tester according to configurations provided by user
     """
 
     def __init__(self, selected_test, test_suite=None, gw_obj=None, black_list=None,
                  stop_event_trig=None, tester_name=TesterName.OFFLINE,
                  logger_name=None, logger_result_name=None, logger_gw_name=None,
-                 lock_print=None, inlay=None, verbose=True):
+                 lock_print=None, inlay=None, verbose=True):  # TODO add selected test dict
         """
         :param logger_name: if specified the main logger is based on a predefine logger with the specified name.
                             otherwise the logger is set by the app
         :type logger_name: str
         :param logger_result_name: if specified the results logger is based on a predefine logger with the
                                    specified name. otherwise the logger is set by the app
         :type logger_result_name: str
@@ -237,15 +236,15 @@
                 self.GwObj.reset_buffer()
                 self.GwObj.start_continuous_listener()
                 if self.check_gw_version():
                     self._printing_func('GW obj initialized')
             else:
                 raise Exception('gateway was not detected, please check connection')
         except Exception as e:
-            self._printing_func(e, log_level=logging.WARNING)
+            self._printing_func(str(e), log_level=logging.WARNING)
             raise e
 
     def get_gw_version(self):
         """
         get the gw firmware version
         :return: gw firmware version
         :rtype: str
@@ -316,45 +315,61 @@
                 self._printing_func(msg, log_level=logging.WARNING)
                 raise Exception(msg)
 
     def gw_reset_and_config(self):
         """
         reset gw and config it to tester mode
         """
-        self.GwObj.reset_gw()
-        self.GwObj.close_port()
-        time.sleep(4)
-        self.GwObj.open_port(self.GwObj.port, self.GwObj.baud)
+        self.GwObj.reset_gw(reset_port=False)
+        self.GwObj.reset_listener()
+        if not self.GwObj.is_gw_alive():
+            self._printing_func('gw_reset_and_config: wait more time since gw did not respond')
+            time.sleep(5)
         self.GwObj.write('!set_tester_mode 1', with_ack=True)
         self.GwObj.write('!pl_gw_config 1', with_ack=True)
-        self.GwObj.write('!enable_brg_mgmt 0', with_ack=True)
         self.GwObj.write('!listen_to_tag_only 1', with_ack=True)
-        self.GwObj.write('!energizing_prob_set 100', with_ack=True)
+        self.GwObj.write('!sub1g_sync 1', with_ack=True)
 
         self.GwObj.config_gw(rssi_thr_val=int(self.selected_test['rssiThresholdHW']),
                              time_profile_val=self.selected_test['tests'][0]['timeProfile'],
                              pl_delay_val=self.selected_test['plDelay'], start_gw_app=False, with_ack=True,
                              combined_msg=False)
+        if not self.GwObj.is_gw_alive():
+            raise Exception('Could not get responds from the Gateway, please check connection and re-run')
+
+    def check_if_trigger_was_received(self):
+        n_gw_msg = self.GwObj.com_rsp_str_input_q.qsize()
+        for i in range(n_gw_msg):
+            gw_rsp = self.GwObj.com_rsp_str_input_q.get(timeout=None)
+            if "Start Production Line GW" in gw_rsp['raw']:
+                return True
+        return False
 
     def wait_for_trigger(self, wait_for_gw_trigger):
         """
-        wait for gw trigger, i.e. send 'Start Production Line' msg
+        wait for gw trigger, i.e. send 'Start Production Line' msg.
+        if trigger was not received, gw reset and re-config to make sure there is no gw problem.
         :param wait_for_gw_trigger: the time [seconds] to wait to trigger,
                                     if the elapsed time is larger the function return False
         :type wait_for_gw_trigger: int or float
         :return: if trigger was detected return True
         :rtype: bool
         """
         gw_answer = ''
         gw_trigger_init = datetime.datetime.now()
         dt = datetime.datetime.now() - gw_trigger_init
         while gw_answer == '' and not self.stop_event_trig.isSet() and dt.total_seconds() < wait_for_gw_trigger:
             gw_answer = self.GwObj.read_specific_message(msg="Start Production Line GW", read_timeout=1)
             dt = datetime.datetime.now() - gw_trigger_init
-        return "Start Production Line GW" in gw_answer
+        is_trigger_received = "Start Production Line GW" in gw_answer
+        if not is_trigger_received:
+            self._printing_func('no trigger was detected. reset and config gw again', log_level=logging.INFO)
+            self.gw_reset_and_config()
+            self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
+        return is_trigger_received
 
     def power_index_to_value(self, power_index, abs_power=False, gw_output=False):
         """
         convert gw ouput power index to value according to valid_output_power_vals
         :param power_index: the index of the valid_output_power_vals list
         :type power_index: int
         :param abs_power: true if the desired value is the absolute output power value
@@ -374,15 +389,14 @@
         """
         trigger when the test timers are set (the defined test time was elapsed)
         and reset the timers
         :param timer_type: the timer name
         :type timer_type: str
         """
         self._printing_func('{} time has expired'.format(timer_type), logger_name=LoggerName.RESULTS)
-        self.GwObj.stop_gw_app()
         self.time_expired = True
         self.reset_timers()
 
     def packet_filter(self, packet_list, filter_param='rssi', param_limits=None, ignore_test_mode_packet=False):
         """
         filter the packets from the packet_list according to the filter_param and the param_limits.
         packets that were filtered out of the test does no take into account during the test and considered as noise
@@ -410,15 +424,15 @@
         filtered_packet_list = PacketList()
 
         for p in packet_list:
             # filter packets from black list:
             if p.packet_data['adv_address'] in self.black_list:
                 p.add_custom_data(custom_data={'packet_status': 'blacklist'})
             elif ignore_test_mode_packet and p.packet_data['test_mode'] == 1:
-                p.add_custom_data(custom_data={'packet_status': 'test_mode'})
+                p.add_custom_data(custom_data={'packet_status': 'test_mode'})  # TODO: check if it really help
             else:
                 # filter packets by filter param:
                 packet_param_list = p.extract_packet_data_by_name(filter_param)
                 sprinkler_ids = []
                 for i, param in enumerate(packet_param_list):
                     if param_limits[0] <= param <= param_limits[-1]:
                         update_custom_data(p, 'packet_status', 'good')
@@ -476,41 +490,49 @@
             elif tags_in_tie:
                 pass
             else:
                 self.tag_results.selected_tag = self.tag_results.all_tags.tags[selected_adva]
 
         return self.tag_results.selected_tag
 
-    def get_packets(self, filter_param='rssi', filter_value=0):
+    def get_packets(self, filter_param='rssi', filter_value=0, data_type=DataType.PACKET_LIST):
         """
         receive packets from the gw (via the listener) and filter them according to packet_filter()
         :param filter_param: one of the packet dataframe column names (for packet_filter)
         :type filter_param: str
         :param filter_value: the max valid value of the specified param
         :type filter_value: int
+        :param data_type: data type of the received packets
+        :type data_type: DataType
         :return: True if packet were received
         :rtype: bool
         """
         packets_received_list = None
         if self.GwObj.is_data_available():
             packets_received_list = self.GwObj.get_packets(action_type=ActionType.ALL_SAMPLE,
-                                                           data_type=DataType.PACKET_LIST,
+                                                           data_type=data_type,
                                                            tag_inlay=self.selected_test['inlay'])
         if packets_received_list:
-            self._printing_func('got {} packets'.format([p.get_packet_string() for p in packets_received_list]),
-                                log_level=logging.DEBUG)
+            if packets_received_list.size() > 1:
+                self._printing_func('pulled more than one packet from the queue, check analysis performance')
+
+            self._printing_func('got {} packets'.format(
+                ['ADVA:' + p.get_adva() + ',    FLOW:' + p.get_flow() + ',    RSSI:' +
+                 p.get_rssi() + ',    ' + p.get_packet_string() for p in packets_received_list]),
+                log_level=logging.DEBUG)
             filtered_packets = self.packet_filter(packets_received_list, filter_param=filter_param,
                                                   param_limits=[0, filter_value],
                                                   ignore_test_mode_packet=self.selected_test['ignore_test_mode'])
             self.tag_results.all_packets.__add__(packets_received_list)
             if filtered_packets.size():
                 self.tag_results.filtered_tags = \
                     self.tag_results.add_packets_to_multi_tags(filtered_packets, self.tag_results.filtered_tags)
                 self._printing_func('and {} pass the packet filter'.format(
-                    [p.get_packet_string() for p in filtered_packets]), log_level=logging.DEBUG)
+                    ['ADVA:' + p.get_adva() + ',    FLOW:' + p.get_flow() + ',    RSSI:' + p.get_rssi() + ',    ' +
+                     p.get_packet_string() for p in packets_received_list]), log_level=logging.DEBUG)
             return True
         else:
             return False
 
     def check_stop_criteria(self, stop_criteria_dict=None, check_packet_num_only=False):
         """
         check if the received packet met the stop criteria and the test should be stopped
@@ -540,36 +562,53 @@
                     if all(criteria_status):
                         tags_reached_criteria.append(tag['adv_address'])
                 except Exception as e:
                     raise e
 
         return tags_reached_criteria
 
-    @staticmethod
-    def is_gw_fetal_error(packet_list):
+    def is_gw_fetal_error(self, packet_list=None):
         """
-        check if the gw reset itself for some reason
+        check if the gw reset itself for some reason or if it needs to be reset
         :param packet_list: the received packets list
         :type packet_list: PacketList
         :return:
         :rtype:
         """
-        counter = 0
-        for p in packet_list:
-            if p.gw_data['stat_param'].size > 1:
-                for s in p.gw_data['stat_param']:
-                    if s == 0:
+        if not self.GwObj.is_connected():
+            self._printing_func('GW was disconnected. trying to initiate connection...', log_level=logging.WARNING)
+            self.GwObj.open_port(self.GwObj.port, self.GwObj.baud)
+            return True
+
+        if self.GwObj.get_read_error_status():
+            self._printing_func('A GW reading Error was detected', log_level=logging.WARNING)
+            return True
+
+        if packet_list is None:
+            return False
+        # check if GW's clock was reset (relevant only to GW ver 3.8.14 and lower)
+        try:
+            is_old_gw_ver = int(self.get_gw_version().split('.')[0]) < 4
+        except Exception as e:
+            is_old_gw_ver = True  # do the test next test anyway
+
+        if is_old_gw_ver:
+            counter = 0
+            for p in packet_list:
+                if p.gw_data['stat_param'].size > 1:
+                    for s in p.gw_data['stat_param']:
+                        if s == 0:
+                            counter = counter + 1
+                            if counter > 1:
+                                return True
+                else:
+                    if p.gw_data['stat_param'] == 0:
                         counter = counter + 1
                         if counter > 1:
                             return True
-            else:
-                if p.gw_data['stat_param'] == 0:
-                    counter = counter + 1
-                    if counter > 1:
-                        return True
         return False
 
     def statistics_analyzer(self, test_param=None, test_num=None):
         """
         test the quality of the test according to test_param
         :param test_param: the test parameters including the quality parameters which defines if
                            the tag passed or failed the test (e.g.
@@ -579,24 +618,24 @@
         :return: True if the tag passed the test
         :rtype: bool
         """
 
         # add test num to the packets:
         self.tag_results.add_selected_tag_statistics(custom_data={'test_num': test_num})
         if self.is_gw_fetal_error(self.tag_results.selected_tag):
-            self.logger_results.debug('gw fetal error was detected')
+            self.logger_results.warning('gw fetal error was detected')
             self.gw_reset_and_config()
+            self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
             self.tag_results.test_status = FailureCodes.GW_ERROR
             targets_status = [False]
         elif 'quality_param' in test_param and len(test_param['quality_param']) > 0:
             targets_status = [v[0] <= self.tag_results.selected_tag_statistics[k] <= v[-1]
                               for k, v in test_param['quality_param'].items()]
-            self.logger_results.debug('selected tag values: {}'.format({k: self.tag_results.selected_tag_statistics[k]
-                                                                        for k in test_param['quality_param'].keys()
-                                                                        }))
+            self.logger_results.info('selected tag values: {}'.format({k: self.tag_results.selected_tag_statistics[k]
+                                                                       for k in test_param['quality_param'].keys()}))
             self.tag_results.set_quality_test_failure(test_param['quality_param'], targets_status)
 
         else:
             targets_status = [True]
 
         return all(targets_status)
 
@@ -651,15 +690,16 @@
         :type max_ttfp: float
         :param sub_test: the test parameters according to the test suite
         :type sub_test: dict
         """
         if max_ttfp is not None:
             self.first_packet_timer = threading.Timer(max_ttfp, self.end_of_time, ['First Packet'])
             self.first_packet_timer.start()
-            self.logger.info('Timer for first packet has been set for {} seconds, test time is {} seconds'.format(max_ttfp, sub_test['maxTime']))
+            self.logger.info('Timer for first packet has been set for {} seconds, test time is {} seconds'.format(
+                max_ttfp, sub_test['maxTime']))
         self.test_timer = threading.Timer(sub_test['maxTime'], self.end_of_time, ['Test'])
         self.test_timer.start()
         if max_ttfp is None:
             self.logger.info('Timer for test has been set {} seconds'.format(sub_test['maxTime']))
 
     def reset_timers(self, only_first_packet_timer=False):
         """
@@ -678,15 +718,15 @@
         """
         internal function to print the logs
         :param msg: the message to print
         :type msg: str
         :param logger_name: the logger name
         :type logger_name: LoggerName
         :param log_level: the log level
-        :type log_level: logging
+        :type log_level: logging.INFO
         """
         if self.verbose or log_level != logging.DEBUG:
             with self._lock_print:
                 if logger_name.value == 'main':
                     self.logger.log(log_level, msg)
                 elif logger_name.value == 'gw':
                     self.logger_gw.log(log_level, msg)
@@ -702,15 +742,19 @@
         if isinstance(new_blacklist, list):
             self.black_list += new_blacklist
         elif isinstance(new_blacklist, str):
             self.black_list.append(new_blacklist)
         else:
             raise Exception('trying to add new member to black list of unsupported type: {}'.format(new_blacklist))
 
-    def run(self, wait_for_gw_trigger=None):
+    def init_run(self):
+        self.test_results = WiliotTesterTagResultList()
+        self.tag_results = WiliotTesterTagResult()
+
+    def run(self, wait_for_gw_trigger=None, need_to_manual_trigger=True):
         """
         Flow:
         1. wait for trigger if wait_for_gw_trigger is specified.
         2. Collect filtered packets (e.g. filtered by rssi)
         3. Check if we reached stop criteria - according to stop criteria list
         4. Check if test passed according to performance criteria:
             A. identify the tag under test
@@ -721,44 +765,44 @@
         2. time to first packet expired if max_ttfp is specified
         3. external stop event, is stop_event_trig was specified whn init the class
         4. parameter according to the tests_suite.json (e.g. number of packets)
 
         :param wait_for_gw_trigger: if specified, the test waits the specified seconds for the gw trigger and
                                     starts only when triggered
         :type wait_for_gw_trigger: float or NoneType
-        :param max_ttfp: the maximum time in seconds to wait for the first packet
-        :type max_ttfp: int or NoneType
+        :param need_to_manual_trigger: if True and wait_for_gw_trigger is not specified, a serial command is sent to
+                                       the gw at the start of the test
         :return: the test results including all the tags and test information
         :rtype: WiliotTesterTagResultList
         """
 
         self._printing_func('New tag test starts from API', logger_name=LoggerName.RESULTS)
 
-        self.test_results = WiliotTesterTagResultList()
-        self.tag_results = WiliotTesterTagResult()
+        self.init_run()
 
         # wait for trigger if needed
         if wait_for_gw_trigger is None:
             self.start_test = True
-            self.GwObj.config_gw(start_gw_app=True, with_ack=True)
+            if need_to_manual_trigger:
+                self.GwObj.config_gw(start_gw_app=True, with_ack=True)
         else:
             self._printing_func('Wait for GW trigger for {} second'.format(wait_for_gw_trigger))
             self.start_test = self.wait_for_trigger(wait_for_gw_trigger)
 
         # check if test can be started:
         if self.stop_event_trig.isSet():
             self._printing_func('Run was stopped by the stop event before it started', log_level=logging.INFO)
             return self.test_results
 
         if not self.start_test:
-            self._printing_func('no trigger was detected. Please check GW for input trigger', log_level=logging.INFO)
             return self.test_results
 
+        self.GwObj.reset_start_time()
         self.test_results.set_trigger_time()
-        self.GwObj.reset_listener()
+
         # Test begins
         self._printing_func('Trigger received')
 
         num_of_tests = len(self.selected_test['tests'])
         for test_num in range(num_of_tests):
             sub_test = self.selected_test['tests'][test_num]
             check_packet_num_only = \
@@ -772,49 +816,67 @@
 
             # Begin test timers
             self.init_test_timers(self.max_ttfp, sub_test)
 
             # Start test check
             tags_reached_criteria = []
             while not self.test_end and not self.stop_event_trig.isSet() and not self.time_expired:
+
+                # check if trigger was received during run:
+                if self.check_if_trigger_was_received():
+                    self._printing_func('Gateway got trigger during run. Please check the Machine')
+                    raise Exception('Gateway got trigger during run. Please check the Machine')
+
                 # collect filtered packets
-                is_received_packet = self.get_packets(filter_param='rssi',
-                                                      filter_value=self.selected_test['rssiThresholdSW'])
+                is_received_packet = self.get_packets(filter_value=self.selected_test['rssiThresholdSW'])
                 if is_received_packet:
                     self.reset_timers(only_first_packet_timer=True)
                     # check if we reached stop criteria:
                     tags_reached_criteria = self.check_stop_criteria(stop_criteria_dict=sub_test['stop_criteria'],
                                                                      check_packet_num_only=check_packet_num_only)
 
                     if len(tags_reached_criteria):
                         self._printing_func('test reached stop criteria - starting to analyze the results')
                         self.test_end = True
                 else:
                     time.sleep(0)  # allow time for recovery
+                    # check if GW ERROR occurred and fix it:
+                    if self.is_gw_fetal_error():
+                        self.logger_results.warning('gw fetal error was detected')
+                        if not self.GwObj.is_connected():
+                            raise Exception('Could not reconnect to the GW. please check connections')
+                        self.gw_reset_and_config()
+                        self.init_gw_test(sub_test=sub_test, is_start_gw_app=True)
+                        self.tag_results.test_status = FailureCodes.GW_ERROR
 
             # stop gw from transmitting
             self.GwObj.stop_gw_app()
 
             # check why the test is over
             if self.stop_event_trig.isSet():  # Stop event was triggered
-                self._printing_func('Stop was triggered', log_level=logging.INFO)
+                self._printing_func('Stop was triggered')
                 self._printing_func('Tag marked as Fail', logger_name=LoggerName.RESULTS)
                 self.reset_timers()
                 self.tag_results.test_status = FailureCodes.STOP_BY_USER
                 self.test_results.append(self.tag_results)
 
             elif self.time_expired:  # time expired before reaching stop criteria
                 if sub_test['stop_criteria']:
                     self._printing_func('Stage {} Failed - Timeout'.format(test_num + 1),
                                         logger_name=LoggerName.RESULTS)
-                    if self.tag_results.all_packets.size() == 0:
+                    if self.tag_results.test_status == FailureCodes.GW_ERROR:
+                        pass
+                    elif self.tag_results.all_packets.size() == 0:
                         self.tag_results.test_status = FailureCodes.NO_RESPONSE
                     elif len(self.tag_results.filtered_tags) == 0:
                         self.tag_results.test_status = FailureCodes.NO_PACKETS_UNDER_RSSI_THR
                     else:
+                        self.tag_results.all_tags = self.tag_results.add_packets_to_multi_tags(
+                            packets_in=self.tag_results.all_packets,
+                            multi_tag_out=self.tag_results.all_tags)
                         self.tag_results.test_status = FailureCodes.NOT_ENOUGH_PACKETS
                     self.test_results.append(self.tag_results)
                 else:
                     # no stop criteria:
                     self._printing_func('Stage {} Passed Auto (no stop criteria)'.format(test_num + 1),
                                         logger_name=LoggerName.RESULTS)
                     self.tag_results.test_status = FailureCodes.PASS
@@ -857,31 +919,33 @@
                     dt = datetime.datetime.now() - t_i
             # end of test:
             self.tag_results.test_end = datetime.datetime.now()
             if self.tag_results.test_status != FailureCodes.PASS and not self.run_all:
                 break  # stop the test if one of the stages was failed
 
         # prepare gw for the next run:
-        self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
+        if num_of_tests > 1:
+            self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
         self.reset_timers()
         return self.test_results
 
     def exit_tag_test(self):
         self.reset_timers()
         self.GwObj.close_port(is_reset=True)
         self.GwObj.stop_continuous_listener()
 
 
 if __name__ == '__main__':
     from csv import DictWriter
+    import os
 
     from wiliot_testers.wiliot_tester_log import WiliotTesterLog
-    from wiliot_testers.wiliot_tester_tag_result import ConversionTypes, InlayTypes, SurfaceTypes, FailureCodes
-    from wiliot_testers.utils import get_version
-
+    from wiliot_testers.wiliot_tester_tag_result import ConversionTypes, SurfaceTypes, FailureCodes
+    from wiliot_testers.utils.get_version import get_version
+    from wiliot_core import InlayTypes
 
     def stop_run():
         my_stop_event.set()
 
 
     def dict_to_csv(dict_in, path, append=False, only_titles=False):
         if append:
@@ -968,15 +1032,15 @@
                     save_default_packet_data(summary=r_sum)
 
         else:
             test_data['test_num'] = 0
             save_default_packet_data()
 
 
-    log_path = 'C:\\Users\\shunit\\Downloads'
+    log_path = os.path.join(os.path.expanduser('~'), 'Downloads')
     black_list = ['A', 'B']
     test_suite = {"Dual Band": {
         "plDelay": 100,
         "rssiThresholdHW": 86,
         "rssiThresholdSW": 56,
         "maxTtfp": 3,
         "tests": [
@@ -985,17 +1049,17 @@
              "energizingPattern": 18,
              "timeProfile": [5, 15],
              "absGwTxPowerIndex": -1,
              "maxTime": 3,
              "delayBeforeNextTest": 0,
              "stop_criteria": {"num_packets": [1, 99]},
              "quality_param": {"ttfp": [0, 3]},
-             'gw_commands': ['!set_sub_1_ghz_energizing_frequency 916000',
-                             '!set_dyn_energizing_pattern 6 0 1 2480',
-                             '!set_beacons_pattern 375 3 2402 2426 2478']
+             # 'gw_commands': ['!set_sub_1_ghz_energizing_frequency 916000',
+             #                 '!set_dyn_energizing_pattern 6 0 1 2480',
+             #                 '!set_beacons_pattern 375 3 2402 2426 2478']
              },
             {"name": "sub1G_band",
              "rxChannel": 37,
              "energizingPattern": 52,
              "timeProfile": [5, 15],
              "absGwTxPowerIndex": -1,
              "sub1gGwTxPower": 9,
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/yield/arduino_counter/arduino_counter.ino` & `wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.0/wiliot_testers/yield/configs/inlay_data.py` & `wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 csv_dictionary = {
-    'TEO_086': {'number': '086', 'number_of_rows': 1, 'received_channel': '37', 'energy_pattern_val': 18,
-                'time_profile_val': [5, 15]},
-    'TIKI_096': {'number': '096', 'number_of_rows': 2, 'received_channel': '37', 'energy_pattern_val': 51,
-                 'time_profile_val': [5, 15]},
-    'TIKI_099': {'number': '099', 'number_of_rows': 3, 'received_channel': '37', 'energy_pattern_val': 51,
-                 'time_profile_val': [5, 15]},
-    'BATTERY_107': {'number': '107', 'number_of_rows': 4, 'received_channel': '37', 'energy_pattern_val': 17,
-                    'time_profile_val': [5, 15]},
-    'TIKI_117': {'number': '117', 'number_of_rows': 5, 'received_channel': '37', 'energy_pattern_val': 51,
-                 'time_profile_val': [5, 15]},
-    'TIKI_121': {'number': '121', 'number_of_rows': 6, 'received_channel': '37', 'energy_pattern_val': 51,
-                 'time_profile_val': [5, 15]},
-    'TIKI_122': {'number': '122', 'number_of_rows': 7, 'received_channel': '37', 'energy_pattern_val': 51,
-                 'time_profile_val': [5, 15]}}
+    'TEO_086': {'inlay': 'TEO_086', 'number': '086', 'number_of_rows': 1, 'received_channel': '37',
+                'energy_pattern_val': 18, 'time_profile_val': [5, 15]},
+    'TIKI_096': {'inlay': 'TIKI_096', 'number': '096', 'number_of_rows': 2, 'received_channel': '37',
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
+    'TIKI_099': {'inlay': 'TIKI_099', 'number': '099', 'number_of_rows': 3, 'received_channel': '37',
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
+    'BATTERY_107': {'inlay': 'BATTERY_107', 'number': '107', 'number_of_rows': 4, 'received_channel': '37',
+                    'energy_pattern_val': 17, 'time_profile_val': [5, 15]},
+    'TIKI_117': {'inlay': 'TIKI_117', 'number': '117', 'number_of_rows': 5, 'received_channel': '37',
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
+    'TIKI_121': {'inlay': 'TIKI_121', 'number': '121', 'number_of_rows': 6, 'received_channel': '37',
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
+    'TIKI_122': {'inlay': 'TIKI_122', 'number': '122', 'number_of_rows': 7, 'received_channel': '37',
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
+    '': {'inlay': '', 'number': '', 'number_of_rows': 0, 'received_channel': '', 'energy_pattern_val': 0,
+         'time_profile_val': [0, 0]}}
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers/yield/yield_tester.py` & `wiliot-testers-4.0.6/wiliot_testers/yield/yield_tester.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,23 +66,23 @@
 4)Calculating the Yield fraction according to the results we got from the instances
 5)Creating two threads in MainWindow class in order to calculate the fraction by MultiThreadingCalculation instance
 and to run the GUI function (open_session) at the same time.
 """
 
 from wiliot_core import *
 import csv
-import serial
 import serial.tools.list_ports
 import PySimpleGUI as sg
 from configs.inlay_data import *
 from wiliot_testers.tester_utils import *
 from wiliot_testers.utils.get_version import *
+import serial
+
 
 inlay_types_dict = {item.name: item.value for item in InlayTypes}
-my_path = ''
 today = datetime.date.today()
 formatted_today = today.strftime("%Y%m%d")  # without -
 formatted_date = today.strftime("%Y-%m-%d")
 current_time = datetime.datetime.now()
 cur_time_formatted = current_time.strftime("%I%M%S")  # without :
 time_formatted = current_time.strftime("%I:%M:%S")
 
@@ -169,26 +169,25 @@
         self.ports = self.get_ports_of_arduino()
         try:
             self.comPortObj = serial.Serial(self.ports[0], self.baud, timeout=0.1)
         except serial.SerialException:
             print("NO ARDUINO")
         self.rows = rows
         self.stop = stop_event
-        self.tags_num = 0
         self.tested = 0
 
     def get_ports_of_arduino(self):
         """
         Gets all the ports we have, then chooses Arduino's ports
         """
 
         arduino_ports = []
-        for p in self.available_ports:
-            if 'modem' in str(p):
-                arduino_ports.append(p)
+        for p in serial.tools.list_ports.comports():
+            if 'Arduino' in p.description:
+                arduino_ports.append(p.device)
         if not arduino_ports:
             print('NO ARDUINO')
 
         return arduino_ports
 
     def run(self):
         """
@@ -196,36 +195,36 @@
         """
 
         while not self.stop.is_set():
             time.sleep(1)
             data = ''
             try:
                 data = self.comPortObj.readline()
+
             except e:
                 print("NO READLINE")
             buf = b''
             if data.__len__() > 0:
-                self.tags_num += 1
                 buf += data
                 if b'\n' in buf:
                     try:
                         tmp = buf.decode().strip(' \t\n\r')
                         if "pulses detected" in tmp:
                             self.tested += self.rows
 
                     except e:
                         print('Warning: Could not decode counter data or Warning: Could not decode counter data')
                         continue
         self.comPortObj.close()
 
-    def get_tags_num(self):
+    def get_tested(self):
         """
         returns the number of tags
         """
-        return self.tags_num
+        return self.tested
 
 
 class MultithreadedCalculation(threading.Thread):
     """
     Calculating the yield fraction by multi-threading process
     """
 
@@ -243,17 +242,17 @@
         """
         self.adva_process.start()
         self.count_thread.start()
         while not self.stop.is_set():
             time.sleep(3)
 
             unq_advas = self.adva_process.get_unq_advas()
-            tags_num = self.count_thread.get_tags_num()
+            tags_num = self.count_thread.get_tested()
             if tags_num > 0:
-                self.result = unq_advas / (tags_num * self.rows)
+                self.result = unq_advas / tags_num
                 print(self.result)
 
         self.adva_process.stop.set()
         self.count_thread.stop.set()
         self.adva_process.join()
         self.count_thread.join()
 
@@ -271,20 +270,19 @@
         self.stop = threading.Event()
         self.selected = ''
         self.wafer_lot = ''
         self.wafer_number = ''
         self.operator = ''
         self.run_start_time = ''
         self.run_end_time = ''
-        self.tester_type = 'yield'
+        self.tester_type = 'yield-test'
         self.tester_station_name = ''
         self.comments = ''
         self.gw_version = ''
         self.advas = 0
-        self.tags_num = 0
         self.run_responsive_tags_yield = 0  # still don't have a pass criteria
         self.result = 0
         self.run_passed_tags_yield = 0  # still don't have a pass criteria
         self.rows_number = 1
         self.upload_flag = True
 
     def run(self):
@@ -298,27 +296,27 @@
         self.multi.join()
 
     def run_data_to_csv(self, csv_dict, file_path, cmn_r_name, run_end_time, total_run_tested,
                         total_run_responding_tags, total_run_passed_tags, py_wiliot_version):
         """
         Saves a csv file with all the needed features
         """
-
         with open(file_path, 'w', newline='') as file:
             csv_writer = csv.writer(file)
             csv_writer.writerow([
                 'common_run_name', 'tester_station_name', 'operator',
                 'run_start_time', 'run_end_time', 'wafer_lot', 'wafer_number', 'tester_type',
                 'comments', 'inlay', 'total_run_tested', 'total_run_responding_tags',
                 'total_run_passed_tags', 'run_responsive_tags_yield', 'run_passed_tags_yield',
                 'gw_version',
                 'py_wiliot_version', 'upload_date', 'number_of_rows', 'received_channel', 'energy_pattern_val',
                 'time_profile_val', ])
             if self.selected == '':
-                exit()
+                # exit()
+                pass
             value = csv_dict[self.selected]
             csv_writer.writerow(
                 [
                     cmn_r_name, self.tester_station_name, self.operator,
                     formatted_date + ' ' + self.run_start_time,
                     formatted_date + ' ' + run_end_time,
                     self.wafer_lot, self.wafer_number, self.tester_type, self.comments, self.selected, total_run_tested,
@@ -335,17 +333,17 @@
         """
 
         start_time = datetime.datetime.now()
         self.run_start_time = start_time.strftime("%I:%M:%S")
         yes_or_no = ['Yes', 'No']
         layout = [
             [sg.Text('YIELD Fraction is :', font=4)],
-            # [sg.Output(key='yield', font=4)],
+            [sg.Output(key='yield', font=4, size=(60, 7))],
             [sg.Text('Do you want to stop or upload?')],
-            [sg.Button('Stop'), [sg.Text('Upload:', font=4)],
+            [sg.Button('Stop'), [sg.Text('Upload:', font=6)],
              [sg.Combo(values=yes_or_no, default_value=yes_or_no[0], key='upload', font=4, enable_events=True)]]
         ]
         sub = False
         window = sg.Window('Upload CSV files', layout, modal=True)
         while True:
             event, values = window.read()
             if event == sg.WIN_CLOSED or event in ('Stop', 'upload'):
@@ -355,38 +353,49 @@
                     else:
                         self.upload_flag = True  # if we press No then yes
                 if event == 'Stop':
                     self.stop.set()
                     end_time = datetime.datetime.now()
                     run_end_time = end_time.strftime("%I:%M:%S")
                     advas = self.multi.adva_process.get_unq_advas()
-                    tags_num = self.multi.count_thread.get_tags_num()
+                    tags_num = self.multi.count_thread.get_tested()
                     result = self.multi.get_result()
                     cmn = self.wafer_lot + '.' + self.wafer_number + '_' + formatted_today + '_' + cur_time_formatted
                     py_wiliot_version = get_version()
                     d = WiliotDir()
                     d.create_tester_dir(tester_name='yield_tester')
                     yield_test_app_data = d.get_tester_dir('yield_tester')
                     run_path = os.path.join(yield_test_app_data, cmn)
                     if not os.path.exists(run_path):
                         os.makedirs(run_path)
                     final_path_run_data = os.path.join(run_path, cmn + '@run_data.csv')
-                    self.run_data_to_csv(csv_dictionary, final_path_run_data, cmn, run_end_time,
-                                         tags_num, advas, result, py_wiliot_version)
+
+                    try:
+                        self.run_data_to_csv(csv_dictionary, final_path_run_data, cmn, run_end_time,
+                                             tags_num, advas, result, py_wiliot_version)
+                    except Exception as e:
+                        print(e)
                     try:
                         tag_df = self.multi.adva_process.all_tags.get_df()
                         tag_df.insert(loc=len(tag_df.columns), column='common_run_name', value=cmn)
                         final_path_packets_data = os.path.join(run_path, cmn + '@packets_data.csv')
-                        tag_df.to_csv(final_path_packets_data)
+                        tag_df.to_csv(final_path_packets_data, index=False)
                         if self.upload_flag:
                             try:
-                                upload_to_cloud_api(cmn, self.tester_type, run_data_csv_name=final_path_run_data,
-                                                    tags_data_csv_name=final_path_packets_data,
-                                                    packets_instead_tags=True)
-                            except FileExistsError:
+                                is_uploaded = upload_to_cloud_api(cmn, self.tester_type,
+                                                                  run_data_csv_name=final_path_run_data,
+                                                                  tags_data_csv_name=final_path_packets_data,
+                                                                  env='test',
+                                                                  packets_instead_tags=True, is_path=True)
+                                if is_uploaded:
+                                    print("Successful upload")
+                                else:
+                                    print("Unsuccessful upload")
+                            except Exception as e:
+                                print(e)
                                 print("Upload function failure")
 
                     except Empty:
                         print("NO PACKETS RECEIVED")
 
                     sub = True
                     break
@@ -396,34 +405,35 @@
         window.close()
         return sub
 
     def open_session(self):
         """
         opening a session for the process
         """
-
         if os.path.exists("configs/gui_input_do_not_delete.json"):
             with open("configs/gui_input_do_not_delete.json", "r") as f:
                 previous_input = json.load(f)
+
         else:
-            previous_input = {'wafer_lot': '', 'wafer_num': '', 'inlay': '',
-                              'tester_station_name': '', 'comments': '', 'operator': ''}
-        selected_inlay = csv_dictionary[previous_input["inlay"]]
+            previous_input = {'inlay': '', 'number': '', 'number_of_rows': '', 'received_channel': '',
+                              'energy_pattern_val': '', 'time_profile_val': '', 'tester_station_name': '',
+                              'comments': '', 'operator': '', 'wafer_lot': '', 'wafer_num': ''}
+        selected_inlay = csv_dictionary[previous_input['inlay']]
         self.rows_number = selected_inlay['number_of_rows']
         energy_pat = selected_inlay['energy_pattern_val']
         time_pro = selected_inlay['time_profile_val']
         rec_channel = selected_inlay['received_channel']
         lst_inlay_options = list(inlay_types_dict.keys())
         layout = [
 
             [sg.Text('Wafer Lot:', font=4)],
-            [sg.InputText(key='wafer_lot', font=4)],
+            [sg.InputText(key='wafer_lot', default_text=previous_input['wafer_lot'], font=4)],
 
             [sg.Text('Wafer Number:', font=4)],
-            [sg.InputText(key='wafer_num', font=4)],
+            [sg.InputText(key='wafer_num', default_text=previous_input['wafer_num'], font=4)],
 
             [sg.Text('Inlay:', font=4)],
             [sg.Combo(values=lst_inlay_options, default_value=previous_input['inlay'], key='inlay', font=4,
                       enable_events=True)],
 
             [
                 sg.Column([[sg.Text('Energy Pattern:', font=4),
@@ -472,23 +482,23 @@
                 window.find_element('energy_pattern_val').Update(value=energy_pat)
                 window.find_element('time_profile_val').Update(value=time_pro)
                 window.find_element('received_channel').Update(value=rec_channel)
             if event == 'Submit':  # Button clicked
                 self.comments = values['comments']
                 self.tester_station_name = values['tester_station_name']
                 self.operator = values['operator']
-                self.multi = MultithreadedCalculation(self.stop, self.rows_number, rec_channel,
-                                                      time_pro, energy_pat)
+                self.multi = MultithreadedCalculation(self.stop, rec_channel,
+                                                      time_pro, energy_pat, self.rows_number)
                 self.gw_version = self.multi.adva_process.gw_instance.get_gw_version()[0]
                 self.multi.start()
                 with open("configs/gui_input_do_not_delete.json", "w") as f:
                     json.dump(values, f)
                 break
             elif event == sg.WIN_CLOSED:
                 exit()
 
         window.close()
 
 
 if __name__ == '__main__':
     m = MainWindow()
-    m.run()
+    m.run()
```

### Comparing `wiliot-testers-4.0.0/wiliot_testers.egg-info/SOURCES.txt` & `wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 setup.py
 unittests.dockerfile
 wiliot_testers/API_README.md
 wiliot_testers/__init__.py
 wiliot_testers/requirements.txt
 wiliot_testers/test_equipment.py
 wiliot_testers/tester_utils.py
+wiliot_testers/upload_testers_data.bat
+wiliot_testers/upload_testers_data_to_cloud.py
 wiliot_testers/version.py
 wiliot_testers/wiliot_tester_log.py
 wiliot_testers/wiliot_tester_tag_result.py
 wiliot_testers/wiliot_tester_tag_test.py
 wiliot_testers.egg-info/PKG-INFO
 wiliot_testers.egg-info/SOURCES.txt
 wiliot_testers.egg-info/dependency_links.txt
@@ -36,40 +38,33 @@
 wiliot_testers/offline/env_install.bat
 wiliot_testers/offline/env_install.py
 wiliot_testers/offline/offline_tester.py
 wiliot_testers/offline/offline_utils.py
 wiliot_testers/offline/requirements.txt
 wiliot_testers/offline/run_offline_tester.bat
 wiliot_testers/offline/tadbik_r2r_controller.py
-wiliot_testers/offline/upload_and_serialize_csv_manually.py
-wiliot_testers/offline/upload_and_serialize_offlne_logs.bat
 wiliot_testers/offline/configs/__init__.py
-wiliot_testers/offline/configs/gui_inputs_autotests.json
-wiliot_testers/offline/configs/gui_printer_inputs_4_Test_do_not_delete.json
 wiliot_testers/offline/configs/test_configs.json
 wiliot_testers/offline/configs/tests_suites.json
 wiliot_testers/offline/docs/__init__.py
 wiliot_testers/offline/docs/example_of_timing_diagram.jpg
 wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
 wiliot_testers/offline/docs/offline_tester_run_gui.png
 wiliot_testers/offline/docs/offline_tester_start_gui.png
 wiliot_testers/offline/docs/r2r_communication_diagram.jpg
 wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
 wiliot_testers/offline/docs/wiliot_logo.png
 wiliot_testers/sample/__init__.py
 wiliot_testers/sample/com_connect.py
 wiliot_testers/sample/configs_gui.py
 wiliot_testers/sample/get_temperature_sensor_name.py
-wiliot_testers/sample/sample_test _calib.bat
-wiliot_testers/sample/sample_test _offline.bat
 wiliot_testers/sample/sample_test.bat
 wiliot_testers/sample/sample_test.py
-wiliot_testers/sample/sample_test_calib_offline.bat
-wiliot_testers/sample/configs/.default_configs.json
 wiliot_testers/sample/configs/.default_surfaces.json
+wiliot_testers/sample/configs/.default_test_configs.json
 wiliot_testers/sample/configs/__init__.py
 wiliot_testers/sample/utils/__init__.py
 wiliot_testers/sample/utils/com_connect.ui
 wiliot_testers/sample/utils/comm.gif
 wiliot_testers/sample/utils/configs.gif
 wiliot_testers/sample/utils/configs.ui
 wiliot_testers/sample/utils/edit.gif
```

