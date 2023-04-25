# Comparing `tmp/mobspy-2.0.3.tar.gz` & `tmp/mobspy-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.0.3.tar", last modified: Sun Apr 23 19:15:42 2023, max compression
+gzip compressed data, was "mobspy-2.0.4.tar", last modified: Tue Apr 25 07:34:13 2023, max compression
```

## Comparing `mobspy-2.0.3.tar` & `mobspy-2.0.4.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.269219 mobspy-2.0.3/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.147516 mobspy-2.0.3/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.158559 mobspy-2.0.3/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.3/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.3/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.3/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-23 19:15:42.267710 mobspy-2.0.3/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.3/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.148165 mobspy-2.0.3/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.171569 mobspy-2.0.3/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.3/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.3/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/toggle_switch.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.191472 mobspy-2.0.3/example_models/tutorial_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/01_Getting_Started.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/03_Queries.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/03_Queries.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/04_Characteristic_Restriction.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/05_C_Query.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/06_Round_Robin.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/07_Rates.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/08_Units.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/10_Species_Loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/11_Results.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/12_Hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/13_Born_Species.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      255 2023-04-23 19:10:29.000000 mobspy-2.0.3/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.192835 mobspy-2.0.3/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.3/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.198020 mobspy-2.0.3/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-04-23 19:15:34.000000 mobspy-2.0.3/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.205512 mobspy-2.0.3/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-23 18:41:27.000000 mobspy-2.0.3/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5972 2023-04-20 09:08:12.000000 mobspy-2.0.3/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.218128 mobspy-2.0.3/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.3/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12825 2023-04-21 13:25:09.000000 mobspy-2.0.3/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.3/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    57658 2023-04-23 16:02:06.000000 mobspy-2.0.3/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.3/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.3/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.3/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4088 2023-04-20 15:42:12.000000 mobspy-2.0.3/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.3/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.3/mobspy/modules/unit_handler.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.219619 mobspy-2.0.3/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.3/mobspy/parameter_scripts/parameter_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.223327 mobspy-2.0.3/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.3/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.3/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.227163 mobspy-2.0.3/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1266 2023-04-21 19:43:28.000000 mobspy-2.0.3/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.230023 mobspy-2.0.3/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.3/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14508 2023-04-20 22:03:28.000000 mobspy-2.0.3/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1846 2023-04-20 09:16:42.000000 mobspy-2.0.3/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-20 08:51:56.000000 mobspy-2.0.3/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.234491 mobspy-2.0.3/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.3/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/sbml_simulator/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.3/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.3/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26518 2023-04-23 18:48:25.000000 mobspy-2.0.3/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.236459 mobspy-2.0.3/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.3/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.202456 mobspy-2.0.3/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3635 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.3/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-23 19:15:42.269433 mobspy-2.0.3/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.3/setup.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    20965 2023-04-23 19:13:59.000000 mobspy-2.0.3/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.265261 mobspy-2.0.3/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.3/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.3/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.3/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.3/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.3/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.3/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.3/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.3/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.3/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.3/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.3/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.3/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.3/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.3/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.3/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.3/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.3/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.3/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-04-20 13:29:32.000000 mobspy-2.0.3/test_tools/model_28.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-04-20 13:29:51.000000 mobspy-2.0.3/test_tools/model_29.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-04-21 18:32:12.000000 mobspy-2.0.3/test_tools/model_30.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.3/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.3/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.3/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.152087 mobspy-2.0.4/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.013743 mobspy-2.0.4/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.024525 mobspy-2.0.4/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.4/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.4/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.4/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-25 07:34:13.151251 mobspy-2.0.4/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.4/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.014177 mobspy-2.0.4/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.036653 mobspy-2.0.4/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.4/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.4/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.4/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/application_models/toggle_switch.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.056744 mobspy-2.0.4/example_models/tutorial_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/01_Getting_Started.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/02_Reaction_Inheritance.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/03_Queries.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/03_Queries.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/04_Characteristic_Restriction.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.4/example_models/tutorial_models/05_C_Query.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.4/example_models/tutorial_models/06_Round_Robin.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/07_Rates.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.4/example_models/tutorial_models/08_Units.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/09_Count_Assignment.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/09_Count_Assignment.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/10_Species_Loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/11_Results.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/12_Hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.4/example_models/tutorial_models/13_Born_Species.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      102 2023-04-25 07:25:57.000000 mobspy-2.0.4/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.057771 mobspy-2.0.4/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.4/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.061602 mobspy-2.0.4/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-04-25 07:28:32.000000 mobspy-2.0.4/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.066116 mobspy-2.0.4/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-23 18:41:27.000000 mobspy-2.0.4/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5972 2023-04-20 09:08:12.000000 mobspy-2.0.4/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.084236 mobspy-2.0.4/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.4/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12825 2023-04-21 13:25:09.000000 mobspy-2.0.4/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.4/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    57707 2023-04-24 12:21:50.000000 mobspy-2.0.4/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.4/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.4/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16546 2023-04-24 12:22:42.000000 mobspy-2.0.4/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4088 2023-04-20 15:42:12.000000 mobspy-2.0.4/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.4/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.4/mobspy/modules/unit_handler.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.085650 mobspy-2.0.4/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.4/mobspy/parameter_scripts/parameter_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.088694 mobspy-2.0.4/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.4/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.4/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.092861 mobspy-2.0.4/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1266 2023-04-21 19:43:28.000000 mobspy-2.0.4/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.098947 mobspy-2.0.4/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.4/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14508 2023-04-20 22:03:28.000000 mobspy-2.0.4/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1846 2023-04-20 09:16:42.000000 mobspy-2.0.4/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-20 08:51:56.000000 mobspy-2.0.4/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.103357 mobspy-2.0.4/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.4/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/sbml_simulator/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.4/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12443 2023-04-25 06:36:38.000000 mobspy-2.0.4/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26480 2023-04-25 06:36:38.000000 mobspy-2.0.4/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.104807 mobspy-2.0.4/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.4/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.4/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.064382 mobspy-2.0.4/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-25 07:34:12.000000 mobspy-2.0.4/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3747 2023-04-25 07:34:12.000000 mobspy-2.0.4/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-25 07:34:12.000000 mobspy-2.0.4/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-25 07:34:12.000000 mobspy-2.0.4/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-25 07:34:12.000000 mobspy-2.0.4/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.4/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-25 07:34:13.152276 mobspy-2.0.4/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.4/setup.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.109008 mobspy-2.0.4/test_plot_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11552 2023-04-25 07:28:43.000000 mobspy-2.0.4/test_plot_images/constant_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    47574 2023-04-25 07:28:43.000000 mobspy-2.0.4/test_plot_images/deterministic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    59209 2023-04-25 07:28:43.000000 mobspy-2.0.4/test_plot_images/stochastic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    20606 2023-04-25 07:26:33.000000 mobspy-2.0.4/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-25 07:34:13.148495 mobspy-2.0.4/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.4/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.4/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.4/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.4/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.4/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.4/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.4/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.4/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.4/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.4/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.4/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.4/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.4/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.4/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.4/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.4/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.4/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.4/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-04-20 13:29:32.000000 mobspy-2.0.4/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-04-20 13:29:51.000000 mobspy-2.0.4/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-04-21 18:32:12.000000 mobspy-2.0.4/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.4/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-04-25 07:25:57.000000 mobspy-2.0.4/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.4/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.4/useful_parameters.json
```

### Comparing `mobspy-2.0.3/.github/workflows/python-app.yml` & `mobspy-2.0.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/LICENSE` & `mobspy-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/PKG-INFO` & `mobspy-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.3/README.md` & `mobspy-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/AB_2CD.py` & `mobspy-2.0.4/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/AND_gate.py` & `mobspy-2.0.4/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.0.4/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/For_The_Trees.py` & `mobspy-2.0.4/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/NOR_gate.py` & `mobspy-2.0.4/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/donor_receptor.py` & `mobspy-2.0.4/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/oscillator.py` & `mobspy-2.0.4/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/random_walk.py` & `mobspy-2.0.4/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/simple_repressor.py` & `mobspy-2.0.4/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/application_models/toggle_switch.py` & `mobspy-2.0.4/example_models/application_models/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/01_Getting_Started.py` & `mobspy-2.0.4/example_models/tutorial_models/01_Getting_Started.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance.py` & `mobspy-2.0.4/example_models/tutorial_models/02_Reaction_Inheritance.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt` & `mobspy-2.0.4/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/03_Queries.py` & `mobspy-2.0.4/example_models/tutorial_models/03_Queries.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/03_Queries.txt` & `mobspy-2.0.4/example_models/tutorial_models/03_Queries.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/04_Characteristic_Restriction.py` & `mobspy-2.0.4/example_models/tutorial_models/04_Characteristic_Restriction.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/05_C_Query.py` & `mobspy-2.0.4/example_models/tutorial_models/05_C_Query.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/06_Round_Robin.py` & `mobspy-2.0.4/example_models/tutorial_models/06_Round_Robin.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/07_Rates.py` & `mobspy-2.0.4/example_models/tutorial_models/07_Rates.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/08_Units.py` & `mobspy-2.0.4/example_models/tutorial_models/08_Units.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.py` & `mobspy-2.0.4/example_models/tutorial_models/09_Count_Assignment.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.txt` & `mobspy-2.0.4/example_models/tutorial_models/09_Count_Assignment.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/10_Species_Loop.py` & `mobspy-2.0.4/example_models/tutorial_models/10_Species_Loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/11_Results.py` & `mobspy-2.0.4/example_models/tutorial_models/11_Results.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/12_Hierarchical_plot.py` & `mobspy-2.0.4/example_models/tutorial_models/12_Hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/example_models/tutorial_models/13_Born_Species.py` & `mobspy-2.0.4/example_models/tutorial_models/13_Born_Species.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/images/img.png` & `mobspy-2.0.4/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/data_handler/process_result_data.py` & `mobspy-2.0.4/mobspy/data_handler/process_result_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/data_handler/time_series_object.py` & `mobspy-2.0.4/mobspy/data_handler/time_series_object.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/event_functions.py` & `mobspy-2.0.4/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/function_rate_code.py` & `mobspy-2.0.4/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/logic_operator_objects.py` & `mobspy-2.0.4/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/meta_class.py` & `mobspy-2.0.4/mobspy/modules/meta_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         # BaseSpecies reactions for SBML with theirs respective parameters and rates
         # What do I have so far
         # Species_String_Dict and a set of reaction objects in Reactions_Set
         reactions_for_sbml, parameters_for_sbml = rc.create_all_reactions(reactions_set,
                                                                           meta_species_to_simulate,
                                                                           orthogonal_vector_structure,
                                                                           type_of_model, dimension)
+
         parameters_for_sbml['volume'] = (volume, f'dimensionless')
 
         # O(n^2) reaction check for doubles
         for i, r1 in enumerate(reactions_for_sbml):
             for j, r2 in enumerate(reactions_for_sbml):
                 if i == j:
                     continue
@@ -940,14 +941,16 @@
             Just making addition symmetric check __add__
         """
         return Species.__add__(self, other)
 
     @classmethod
     def _compile_defined_reaction(cls, code_line, line_number):
         n_all = code_line.count('All')
+        code_line = code_line.replace(' ', '')
+
         if 'Rev' in code_line:
             n_all = n_all + 1
 
         n_key = code_line.count(']')
         if n_key != n_all + 1:
             simlog.error(f'At: {code_line} \n' + f'Line number: {line_number} \n'
                         + f'The reaction did not compile. Perhaps there is a missing rate?')
```

### Comparing `mobspy-2.0.3/mobspy/modules/meta_class_utils.py` & `mobspy-2.0.4/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/order_operators.py` & `mobspy-2.0.4/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.0.4/mobspy/modules/reaction_construction_nb.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,17 @@
     """
     for reaction in reactions:
         for reactant in reaction.reactants:
 
             check_for_duplicates = {}
             for cha in reactant['characteristics']:
 
+                if cha == 'all$':
+                    continue
+
                 # Ok I love try catches for checking if something is in a dict. Don't judge me
                 try:
                     check_for_duplicates[ref_characteristics_to_object[cha]]
                     simlog.error(f'Illegal reaction: {reaction}. \n'
                                  'There is a query with two characteristics '
                                  f'{ref_characteristics_to_object[cha].get_characteristics()} from the same'
                                  f' vector axis resulting in an impossible query. \n'
```

### Comparing `mobspy-2.0.3/mobspy/modules/set_counts_module.py` & `mobspy-2.0.4/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/species_string_generator.py` & `mobspy-2.0.4/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/modules/unit_handler.py` & `mobspy-2.0.4/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.0.4/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/parameters/README.md` & `mobspy-2.0.4/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/parameters/default_reader.py` & `mobspy-2.0.4/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/parameters/example_reader.py` & `mobspy-2.0.4/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.0.4/mobspy/plot_params/example_plot_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/plot_scripts/default_plots.py` & `mobspy-2.0.4/mobspy/plot_scripts/default_plots.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.0.4/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.0.4/mobspy/plot_scripts/process_plot_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.0.4/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.0.4/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/sbml_simulator/builder.py` & `mobspy-2.0.4/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy/sbml_simulator/run.py` & `mobspy-2.0.4/mobspy/sbml_simulator/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,14 @@
         if sbml_key not in species_for_sbml.keys():
             continue
 
         if key == 'Time':
             continue
         try:
             # Case of species set
-            if sbml_key in model['assigned_species'] and new_model:
-                continue
             if sim_para["simulation_method"].lower() in check_list:
                 species_for_sbml[sbml_key] = int(list(data[key])[-1])
             else:
                 species_for_sbml[sbml_key] = list(data[key])[-1]
         except KeyError:
             pass
```

### Comparing `mobspy-2.0.3/mobspy/simulation.py` & `mobspy-2.0.4/mobspy/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,14 @@
                 self._reactions_set = self._reactions_set.union(reference.get_reactions())
 
         self._species_counts = []
         for spe_object in self.model:
             for count in spe_object.get_quantities():
                 self._species_counts.append({'object': spe_object, 'characteristics': count['characteristics'],
                                              'quantity': count['quantity']})
-            spe_object.reset_counts()
 
         if not parameters:
             self.parameters = get_default_parameters()
 
         if not plot_parameters:
             self.plot_parameters = get_default_plot_parameters()
```

### Comparing `mobspy-2.0.3/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.0.4/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/mobspy.egg-info/PKG-INFO` & `mobspy-2.0.4/mobspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.3/mobspy.egg-info/SOURCES.txt` & `mobspy-2.0.4/mobspy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 mobspy/plot_scripts/statistics_calculations.py
 mobspy/sbml_simulator/SBMLWriter.py
 mobspy/sbml_simulator/__init__.py
 mobspy/sbml_simulator/builder.py
 mobspy/sbml_simulator/run.py
 mobspy/simulation_logging/__init__.py
 mobspy/simulation_logging/log_scripts.py
+test_plot_images/constant_tree.png
+test_plot_images/deterministic_tree.png
+test_plot_images/stochastic_tree.png
 test_tools/model_1.txt
 test_tools/model_10.txt
 test_tools/model_11.txt
 test_tools/model_12.txt
 test_tools/model_13.txt
 test_tools/model_14.txt
 test_tools/model_15.txt
```

### Comparing `mobspy-2.0.3/setup.py` & `mobspy-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_script.py` & `mobspy-2.0.4/test_script.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,25 +163,24 @@
     MySim.run()
 
 
 def test_hybrid_sim():
     A, B = BaseSpecies(2)
     A >> 2 * A[1]
 
-    A(1)
-    S1 = Simulation(A | B)
+    A(1), B(50)
+    S1 = Simulation(A)
     S1.save_data = False
     S1.plot_data = False
     S1.duration = 3
     S1.level = -1
 
     A.reset_reactions()
     A + B >> Zero[0.01]
 
-    B(50)
     S2 = Simulation(A | B)
     S2.method = 'stochastic'
     S2.duration = (A <= 0) | (B <= 0)
     S2.level = -1
 
     Sim = S1 + S2
     Sim.run()
@@ -283,19 +282,21 @@
 
     A(1), R(1)
     S1 = Simulation(A | R)
     S1.level = -1
     S1.duration = 1
     S1.plot_data = False
 
-    R(0)
     S2 = Simulation(A | R)
     S2.duration = 1
     S2.level = -1
 
+    with S2.event_time(0):
+        R(0)
+
     Sim = S1 + S2
     Sim.run()
     assert Sim.results[A][0] < Sim.results[A][-1] and Sim.results[R][0] == 1 and Sim.results[R][-1] == 0
 
 
 def test_count_assignment():
     A = BaseSpecies(1)
@@ -311,33 +312,14 @@
     S.plot_data = False
     S.duration = 5
     S.run()
     assert compare_model(S.compile(), 'test_tools/model_11.txt') \
            and 150 > S.results[B][-1] > 100 and S.results[A][-1] == 200
 
 
-def test_reaction_deactivation():
-    A, R = BaseSpecies(2)
-    A + R.r1 >> 2 * A + R.r1[1]
-
-    A(1), R(1)
-    S1 = Simulation(A | R)
-    S1.plot_data = False
-    S1.duration = 2
-    S1.level = -1
-
-    R(0)
-    S2 = Simulation(A | R)
-    S2.duration = 2
-    S2.level = -1
-    Sim = S1 + S2
-    Sim.run()
-    assert Sim.results[R][-1] == 0 and Sim.results[R][0] == 1 and Sim.results[A][-2] == Sim.results[A][-1]
-
-
 def test_complex_cell_model():
     Resource, Phage, Infectable = BaseSpecies(3)
     Cell = New(Infectable)
     Cell.t1, Cell.t2, Cell.t3
 
     def reproduction_rate(r):
         if r.t1:
@@ -774,14 +756,15 @@
     Tree = Age * Color * Size
 
     Tree(100), Tree.red.big(150), All[Tree](10), All[Tree.big](100)
     S = Simulation(Tree)
     S.level = -1
     assert compare_model(S.compile(), 'test_tools/model_28.txt')
 
+    Tree.reset_quantities()
     model = set_counts({All[Tree]: 30, 'Tree.blue.old': 100})
     S = Simulation(model)
     S.level = -1
     assert compare_model(S.compile(), 'test_tools/model_29.txt')
 
 
 def test_string_events_assignment():
@@ -838,16 +821,16 @@
     assert os.path.exists('test_plot_images/constant_tree.png')
 
 
 def test_volume_after_sim():
 
     A = BaseSpecies()
 
-    Zero >> A[42]
-    A >> Zero[1]
+    Zero >> A [42]
+    A >> Zero [1]
 
     S = Simulation(A)
     S.plot_data = False
     S.level = -1
     S.volume = 1 * u.milliliter
     S.run()
     assert int(S.results[A][-1]) == 42
```

### Comparing `mobspy-2.0.3/test_tools/model_15.txt` & `mobspy-2.0.4/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_19.txt` & `mobspy-2.0.4/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_21.txt` & `mobspy-2.0.4/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_24.txt` & `mobspy-2.0.4/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_3.txt` & `mobspy-2.0.4/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_4.txt` & `mobspy-2.0.4/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_5.txt` & `mobspy-2.0.4/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_7.txt` & `mobspy-2.0.4/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.3/test_tools/model_9.txt` & `mobspy-2.0.4/test_tools/model_9.txt`

 * *Files identical despite different names*

