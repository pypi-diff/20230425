# Comparing `tmp/control-lab-ly-1.0.1a0.tar.gz` & `tmp/control-lab-ly-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.1a0.tar", last modified: Fri Apr 21 08:38:54 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.1a1.tar", last modified: Tue Apr 25 13:16:49 2023, max compression
```

## Comparing `control-lab-ly-1.0.1a0.tar` & `control-lab-ly-1.0.1a1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:54.105082 control-lab-ly-1.0.1a0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a0/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/MANIFEST.in
--rw-rw-rw-   0        0        0    17492 2023-04-21 08:38:54.109880 control-lab-ly-1.0.1a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.207903 control-lab-ly-1.0.1a0/docs/
--rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a0/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a0/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0     1559 2023-04-21 08:38:54.150031 control-lab-ly-1.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:51.822740 control-lab-ly-1.0.1a0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.236169 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    17492 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.239957 control-lab-ly-1.0.1a0/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.242946 control-lab-ly-1.0.1a0/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.253273 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.267345 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.301990 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.321851 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.333070 control-lab-ly-1.0.1a0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.340050 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.361819 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    16608 2023-04-21 08:35:19.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.374884 control-lab-ly-1.0.1a0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.448785 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.462459 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.491092 control-lab-ly-1.0.1a0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.531957 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10517 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.547863 control-lab-ly-1.0.1a0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.569861 control-lab-ly-1.0.1a0/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.600664 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.659207 control-lab-ly-1.0.1a0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.665311 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.711248 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.755782 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.767824 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.820453 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.861104 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.902106 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8271 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.939190 control-lab-ly-1.0.1a0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.984490 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.000839 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.034499 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.062642 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.071616 control-lab-ly-1.0.1a0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.130251 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.179331 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.229287 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.279847 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30605 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.302152 control-lab-ly-1.0.1a0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.333781 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.364389 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.407515 control-lab-ly-1.0.1a0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.437394 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.462892 control-lab-ly-1.0.1a0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.493863 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.520526 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.532489 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.613079 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.642110 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.741266 control-lab-ly-1.0.1a0/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.753241 control-lab-ly-1.0.1a0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.781965 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.809974 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.863295 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:54.098861 control-lab-ly-1.0.1a0/tests/
--rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.1a0/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      585 2023-04-21 08:33:59.000000 control-lab-ly-1.0.1a0/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a0/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.478120 control-lab-ly-1.0.1a1/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a1/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/MANIFEST.in
+-rw-rw-rw-   0        0        0    17492 2023-04-25 13:16:49.481622 control-lab-ly-1.0.1a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:46.972796 control-lab-ly-1.0.1a1/docs/
+-rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a1/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a1/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a1/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/pyproject.toml
+-rw-rw-rw-   0        0        0     1560 2023-04-25 13:16:49.500329 control-lab-ly-1.0.1a1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:46.656691 control-lab-ly-1.0.1a1/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.020425 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    17492 2023-04-25 13:16:46.000000 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-04-25 13:16:46.000000 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:16:46.000000 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-04-25 13:16:46.000000 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 13:16:46.000000 control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.025610 control-lab-ly-1.0.1a1/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.046667 control-lab-ly-1.0.1a1/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.057403 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.083172 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.131873 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.157770 control-lab-ly-1.0.1a1/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.166771 control-lab-ly-1.0.1a1/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.194719 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.215984 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    16608 2023-04-21 10:10:50.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a1/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.227429 control-lab-ly-1.0.1a1/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.424158 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-25 13:07:43.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3767 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a1/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.533301 control-lab-ly-1.0.1a1/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a1/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.583393 control-lab-ly-1.0.1a1/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.644689 control-lab-ly-1.0.1a1/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-04-21 14:30:09.000000 control-lab-ly-1.0.1a1/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.672544 control-lab-ly-1.0.1a1/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.704561 control-lab-ly-1.0.1a1/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.739524 control-lab-ly-1.0.1a1/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.757547 control-lab-ly-1.0.1a1/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.768541 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.832580 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.873561 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.903932 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.949981 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.974989 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:47.983435 control-lab-ly-1.0.1a1/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8427 2023-04-25 13:14:54.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.014701 control-lab-ly-1.0.1a1/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.113542 control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.143252 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.213168 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.249645 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.296048 control-lab-ly-1.0.1a1/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.339468 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.412014 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.453846 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.493071 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    30605 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.519485 control-lab-ly-1.0.1a1/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.544122 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.584864 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.617518 control-lab-ly-1.0.1a1/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.644202 control-lab-ly-1.0.1a1/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.668619 control-lab-ly-1.0.1a1/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.776962 control-lab-ly-1.0.1a1/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a1/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.808800 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.820369 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.853574 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:48.873371 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a1/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a1/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a1/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.059109 control-lab-ly-1.0.1a1/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a1/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.064320 control-lab-ly-1.0.1a1/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.078092 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.117992 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.158633 control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-25 13:16:49.468197 control-lab-ly-1.0.1a1/tests/
+-rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a1/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      585 2023-04-21 08:33:59.000000 control-lab-ly-1.0.1a1/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a1/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a1/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a1/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.1a0/LICENSE.md` & `control-lab-ly-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/PKG-INFO` & `control-lab-ly-1.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a0
+Version: 1.0.1a1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
```

### Comparing `control-lab-ly-1.0.1a0/docs/CHANGELOG.md` & `control-lab-ly-1.0.1a1/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.1a1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/docs/LICENSE.md` & `control-lab-ly-1.0.1a1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/docs/README.md` & `control-lab-ly-1.0.1a1/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/setup.cfg` & `control-lab-ly-1.0.1a1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e31 2d61 0d0a 6465 7363 7269 7074 696f  .1-a..descriptio
-00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
-00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
-00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
-00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
-00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
-00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
-000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
-000000d0: 0a61 7574 686f 7220 3d20 4368 616e 6720  .author = Chang 
-000000e0: 4a69 6520 4c65 6f6e 670d 0a61 7574 686f  Jie Leong..autho
-000000f0: 725f 656d 6169 6c20 3d20 6368 616e 676a  r_email = changj
-00000100: 6965 2e6c 656f 6e67 406f 7574 6c6f 6f6b  ie.leong@outlook
-00000110: 2e63 6f6d 0d0a 7572 6c20 3d20 6874 7470  .com..url = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00000130: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
-00000140: 7472 6f6c 2d6c 6162 2d6c 650d 0a70 726f  trol-lab-le..pro
-00000150: 6a65 6374 5f75 726c 7320 3d20 0d0a 0947  ject_urls = ...G
-00000160: 6974 4875 6220 3d20 6874 7470 733a 2f2f  itHub = https://
-00000170: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
-00000180: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
-00000190: 2d6c 6162 2d6c 650d 0a09 446f 6375 6d65  -lab-le...Docume
-000001a0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-000001c0: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-000001d0: 6f6c 2d6c 6162 2d6c 652f 626c 6f62 2f6d  ol-lab-le/blob/m
-000001e0: 6169 6e2f 646f 6373 2f52 4541 444d 452e  ain/docs/README.
-000001f0: 6d64 0d0a 0943 6861 6e67 656c 6f67 203d  md...Changelog =
-00000200: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000210: 636f 6d2f 6b79 6c65 6a65 616e 6c65 7769  com/kylejeanlewi
-00000220: 732f 636f 6e74 726f 6c2d 6c61 622d 6c65  s/control-lab-le
-00000230: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
-00000240: 4348 414e 4745 4c4f 472e 6d64 0d0a 0954  CHANGELOG.md...T
-00000250: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000260: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
-00000270: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
-00000280: 6c2d 6c61 622d 6c65 2f69 7373 7565 730d  l-lab-le/issues.
-00000290: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
-000002a0: 6b65 7977 6f72 6473 203d 200d 0a09 7079  keywords = ...py
-000002b0: 7468 6f6e 0d0a 096c 6162 2061 7574 6f6d  thon...lab autom
-000002c0: 6174 696f 6e0d 0a63 6c61 7373 6966 6965  ation..classifie
-000002d0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-000002e0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-000002f0: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
-00000300: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000310: 6576 656c 6f70 6572 730d 0a09 496e 7465  evelopers...Inte
-00000320: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000330: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-00000340: 680d 0a09 4c69 6365 6e73 6520 3a3a 204f  h...License :: O
-00000350: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000360: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000370: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000380: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
-00000390: 6e64 6f77 730d 0a09 5072 6f67 7261 6d6d  ndows...Programm
-000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003b0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-000003c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003e0: 332e 380d 0a09 546f 7069 6320 3a3a 2053  3.8...Topic :: S
-000003f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000400: 6572 696e 670d 0a0d 0a5b 6f70 7469 6f6e  ering....[option
-00000410: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000420: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000430: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000440: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000450: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
-00000460: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000470: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
-00000480: 6972 6573 203d 200d 0a09 6461 7368 3e3d  ires = ...dash>=
-00000490: 322e 370d 0a09 696d 7065 6461 6e63 653e  2.7...impedance>
-000004a0: 3d31 2e34 0d0a 0969 6d75 7469 6c73 3e3d  =1.4...imutils>=
-000004b0: 302e 350d 0a09 6d61 7470 6c6f 746c 6962  0.5...matplotlib
-000004c0: 3e3d 332e 330d 0a09 6e65 7374 5f61 7379  >=3.3...nest_asy
-000004d0: 6e63 696f 3e3d 312e 350d 0a09 6e75 6d70  ncio>=1.5...nump
-000004e0: 793e 3d31 2e31 390d 0a09 6f70 656e 6376  y>=1.19...opencv
-000004f0: 5f70 7974 686f 6e3e 3d34 2e35 2e30 0d0a  _python>=4.5.0..
-00000500: 0970 616e 6461 733e 3d31 2e32 0d0a 0970  .pandas>=1.2...p
-00000510: 6c6f 746c 793e 3d35 2e33 0d0a 0970 794d  lotly>=5.3...pyM
-00000520: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
-00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
-00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
-00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
-00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
-00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
-00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000005a0: 7372 630d 0a65 7863 6c75 6465 203d 2074  src..exclude = t
-000005b0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
-000005c0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000005d0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 7961  * = *.json, *.ya
-000005e0: 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b 6567  ml, *.png....[eg
-000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000610: 3d20 300d 0a0d 0a                        = 0....
+00000030: 2e31 2d61 310d 0a64 6573 6372 6970 7469  .1-a1..descripti
+00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
+00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
+00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
+00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
+00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
+000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000d0: 0d0a 6175 7468 6f72 203d 2043 6861 6e67  ..author = Chang
+000000e0: 204a 6965 204c 656f 6e67 0d0a 6175 7468   Jie Leong..auth
+000000f0: 6f72 5f65 6d61 696c 203d 2063 6861 6e67  or_email = chang
+00000100: 6a69 652e 6c65 6f6e 6740 6f75 746c 6f6f  jie.leong@outloo
+00000110: 6b2e 636f 6d0d 0a75 726c 203d 2068 7474  k.com..url = htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 6b79 6c65 6a65 616e 6c65 7769 732f 636f  kylejeanlewis/co
+00000140: 6e74 726f 6c2d 6c61 622d 6c65 0d0a 7072  ntrol-lab-le..pr
+00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000160: 4769 7448 7562 203d 2068 7474 7073 3a2f  GitHub = https:/
+00000170: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
+00000180: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
+00000190: 6c2d 6c61 622d 6c65 0d0a 0944 6f63 756d  l-lab-le...Docum
+000001a0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
+000001c0: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
+000001d0: 726f 6c2d 6c61 622d 6c65 2f62 6c6f 622f  rol-lab-le/blob/
+000001e0: 6d61 696e 2f64 6f63 732f 5245 4144 4d45  main/docs/README
+000001f0: 2e6d 640d 0a09 4368 616e 6765 6c6f 6720  .md...Changelog 
+00000200: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000210: 2e63 6f6d 2f6b 796c 656a 6561 6e6c 6577  .com/kylejeanlew
+00000220: 6973 2f63 6f6e 7472 6f6c 2d6c 6162 2d6c  is/control-lab-l
+00000230: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
+00000240: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a09  /CHANGELOG.md...
+00000250: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+00000270: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+00000280: 6f6c 2d6c 6162 2d6c 652f 6973 7375 6573  ol-lab-le/issues
+00000290: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
+000002a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
+000002b0: 7974 686f 6e0d 0a09 6c61 6220 6175 746f  ython...lab auto
+000002c0: 6d61 7469 6f6e 0d0a 636c 6173 7369 6669  mation..classifi
+000002d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
+000002e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
+000002f0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
+00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
+00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
+00000340: 6368 0d0a 094c 6963 656e 7365 203a 3a20  ch...License :: 
+00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000360: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000370: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000380: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
+00000390: 696e 646f 7773 0d0a 0950 726f 6772 616d  indows...Program
+000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000003e0: 2033 2e38 0d0a 0954 6f70 6963 203a 3a20   3.8...Topic :: 
+000003f0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+00000400: 6565 7269 6e67 0d0a 0d0a 5b6f 7074 696f  eering....[optio
+00000410: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000420: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
+00000440: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000450: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
+00000460: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000470: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
+00000480: 7569 7265 7320 3d20 0d0a 0964 6173 683e  uires = ...dash>
+00000490: 3d32 2e37 0d0a 0969 6d70 6564 616e 6365  =2.7...impedance
+000004a0: 3e3d 312e 340d 0a09 696d 7574 696c 733e  >=1.4...imutils>
+000004b0: 3d30 2e35 0d0a 096d 6174 706c 6f74 6c69  =0.5...matplotli
+000004c0: 623e 3d33 2e33 0d0a 096e 6573 745f 6173  b>=3.3...nest_as
+000004d0: 796e 6369 6f3e 3d31 2e35 0d0a 096e 756d  yncio>=1.5...num
+000004e0: 7079 3e3d 312e 3139 0d0a 096f 7065 6e63  py>=1.19...openc
+000004f0: 765f 7079 7468 6f6e 3e3d 342e 352e 300d  v_python>=4.5.0.
+00000500: 0a09 7061 6e64 6173 3e3d 312e 320d 0a09  ..pandas>=1.2...
+00000510: 706c 6f74 6c79 3e3d 352e 330d 0a09 7079  plotly>=5.3...py
+00000520: 4d6f 6462 7573 5443 503e 3d30 2e32 0d0a  ModbusTCP>=0.2..
+00000530: 0970 7973 6572 6961 6c3e 3d33 2e35 0d0a  .pyserial>=3.5..
+00000540: 0950 7953 696d 706c 6547 5549 3e3d 342e  .PySimpleGUI>=4.
+00000550: 3630 0d0a 0950 7956 4953 413e 3d31 2e31  60...PyVISA>=1.1
+00000560: 320d 0a09 5079 5941 4d4c 3e3d 362e 300d  2...PyYAML>=6.0.
+00000570: 0a09 7363 6970 793e 3d31 2e36 0d0a 0d0a  ..scipy>=1.6....
+00000580: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000590: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+000005a0: 2073 7263 0d0a 6578 636c 7564 6520 3d20   src..exclude = 
+000005b0: 7465 7374 730d 0a0d 0a5b 6f70 7469 6f6e  tests....[option
+000005c0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+000005d0: 0a2a 203d 202a 2e6a 736f 6e2c 202a 2e79  .* = *.json, *.y
+000005e0: 616d 6c2c 202a 2e70 6e67 0d0a 0d0a 5b65  aml, *.png....[e
+000005f0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000600: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000610: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a0
+Version: 1.0.1a1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
```

### Comparing `control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.1a1/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/_guibuilder.py`

 * *Files 24% similar despite different names*

```diff
@@ -162,126 +162,14 @@
     - text_size: size of body text
     - bg_color: background color
     """
     def __init__(self, theme=THEME, font=FONT, title_size=TITLE_SIZE, text_size=TEXT_SIZE, bg_color=BG_COLOR):
         super().__init__(theme, font, title_size, text_size, bg_color)
         return
 
-    def getCamera(self):
-        """
-        Get camera module with title and current XYZ labels
-        Return: sg.Column object
-        """
-        module = [
-            [self.getTitle("Webcam", (64,1), 'center', bold=True)],
-            [sg.Image(filename='', key='-IMAGE-', enable_events=True)]
-        ]
-        return sg.Column(module, background_color=self.bg_color)
-    
-    def getControl(self, itemsH=[], itemsV=[], padding=(None,None)):
-        """
-        Get movement control module in different linear or cross configurations
-        - itemsH: items in horizontal alignment
-        - itemsV: items in vertical alignment
-        - padding: amount of padding to add
-        
-        Return: list
-        """
-        module = []
-        if len(itemsV) != 0:
-            for item in itemsV:
-                if item != None:
-                    module.append([self.getP(padding), item, self.getP(padding)])
-                elif len(itemsH) != 0:
-                    module.append([self.getP()] + itemsH + [self.getP()])
-        elif len(itemsH) != 0:
-            module = [self.getP()] + itemsH + [self.getP()]
-        return module
-    def getXYControl(self):
-        """
-        Get XY-control module (cross-configuration)
-        Return: sg.Column object
-        """
-        overall_size = int(64/8*7)
-        size_B = (int(overall_size/7), 2)
-        module = [
-            [self.getText("X/Y axis", (overall_size, 1), 'left', bold=True)]
-        ]
-        x_buttons = [ 
-            self.getB("X-10", size_B), self.getB("X-1", size_B), self.getB("X-0.1", size_B), 
-            sg.Button("<XY>", size=size_B, font=(self.font, self.text_size), button_color=('#000000', '#ffffff')), 
-            self.getB("X+0.1", size_B), self.getB("X+1", size_B), self.getB("X+10", size_B)
-        ]
-        y_buttons = [
-            self.getB("Y+10", size_B), self.getB("Y+1", size_B), self.getB("Y+0.1", size_B), None,
-            self.getB("Y-0.1", size_B), self.getB("Y-1", size_B), self.getB("Y-10", size_B)
-        ]
-        module = module + self.getControl(x_buttons, y_buttons, padding=(size_B[0]*3+4, 2))
-        return sg.Column(module, background_color=self.bg_color)
-    def getXControl(self):
-        """
-        Get X-control module (linear, horizontal configuration)
-        Return sg.Column object
-        """
-        overall_size = int(64/8)
-        size_B = (overall_size, 2)
-        module = [
-            [self.getText("X axis", (overall_size,1), 'left', bold=True)]
-        ]
-        x_buttons = [
-            self.getB("X+10", size_B), self.getB("X+1", size_B), self.getB("X+0.1", size_B),
-            sg.Button("<X>", size=size_B, font=(FONT, self.text_size), button_color=('#000000', '#ffffff')),
-            self.getB("X-0.1", size_B), self.getB("X-1", size_B), self.getB("X-10", size_B)
-        ]
-        module = module + [self.getControl(itemsH=x_buttons)]
-        return sg.Column(module, background_color=self.bg_color)
-    def getZControl(self):
-        """
-        Get Z-control module (linear, vertical configuration)
-        Return sg.Column object
-        """
-        overall_size = int(64/8)
-        size_B = (overall_size, 2)
-        module = [
-            [self.getText("Z axis", (overall_size,1), 'left', bold=True)]
-        ]
-        z_buttons = [
-            self.getB("Z+10", size_B), self.getB("Z+1", size_B), self.getB("Z+0.1", size_B),
-            sg.Button("<Z>", size=size_B, font=(FONT, self.text_size), button_color=('#000000', '#ffffff')),
-            self.getB("Z-0.1", size_B), self.getB("Z-1", size_B), self.getB("Z-10", size_B)
-        ]
-        module = module + self.getControl(itemsV=z_buttons)
-        return sg.Column(module, background_color=self.bg_color)
-    def getXYZControls(self):
-        """
-        Get XYz-control module (cross-configuration + linear, vertical)
-        Return: sg.Column object
-        """
-        module = [
-            [self.getTitle("XYZ Position Control", (64,1), 'center', bold=True)], 
-            [self.getXYControl(), self.getZControl()],
-            [self.getTitle("", (64,1))]
-            ]
-        return sg.Column(module, background_color=self.bg_color)
-    def getPositions(self):
-        """
-        Get XYZ-position indicator module
-        Return: sg.Column object
-        """
-        overall_size = 64
-        size = (int(overall_size/8), 1)
-        module = [
-            [self.getText("Current Position", (overall_size,1), bold=True)], 
-            [self.getText("X:  ", size, 'right'), self.getI(0, size, '-X-CURRENT-'),
-            self.getText("Y:  ", size, 'right'), self.getI(0, size, '-Y-CURRENT-'),
-            self.getText("Z:  ", size, 'right'), self.getI(0, size, '-Z-CURRENT-'),
-            self.getB('Go To', size), self.getB('Clear', size)]
-        ]
-        return sg.Column(module, background_color=self.bg_color)
-
     def getFile(self, name, initial_file=''):
         """
         Get file selector module
         - name: name of field
         - initial_file: default file to display
 
         Return: sg.Column object
@@ -306,72 +194,14 @@
             [self.getP()],
             [self.getText(f"Choose {name.lower()} location: ", (20,1)), 
             self.getI(initial_folder, (36,1), f"-{name.upper()} FOLDER-", enable_events=True),
             sg.FolderBrowse(size=(8,1), font=(self.font, self.text_size), key=f"-{name.upper()} BROWSE-", initial_folder=initial_folder)]
         ]
         return sg.Column(module, background_color=self.bg_color)
 
-    def getKeithley(self, name, default_address=0):
-        """
-        Get Keithley control module
-        - name: name of Keithley
-        - default_address: default address of Keithley to be displayed upon starting GUI
-
-        Return: sg.Column object
-        """
-        overall_size = 64
-        size = (int(overall_size/6), 1)
-        name = name.title()
-        module = [
-            [self.getText(f"{name} Settings", (overall_size,1), bold=True)],
-            [self.getP(), self.getText('IP Address:  ', size, 'right'), self.getI(default_address, size, f'--{name[0]}-ADDRESS--'), 
-            self.getText('# Readings:  ', size, 'right'), self.getI(5, size, f'-{name[0]}-NUMREAD-'), 
-            self.getText('Buffer Size:  ', size, 'right'), self.getI(100, size, f'-{name[0]}-BUFFERSIZE-'), self.getP()]
-        ]
-        return sg.Column(module, background_color=self.bg_color)
-    def getKeithleyParams(self, name, default_address=0, default_values=(0,0,0)):
-        """
-        Get Keithley parameters module
-        - name: name of Keithley
-        - default_address: default address of Keithley to be displayed upon starting GUI
-        - default_values: default parameters of measurement to be displayed upon starting GUI
-
-        Return: sg.Column object
-        """
-        overall_size = 64
-        size = (int(overall_size/8), 1)
-        name = name.title()
-        module = [
-            [self.getText(f"{name} Parameters", (overall_size,1), bold=True)],
-            [self.getP(), self.getText('Address:  ', size, 'right'), self.getI(default_address, size, f'-{name[0]}-ADDRESS-'), 
-            self.getText('Start:  ', size, 'right'), self.getI(default_values[0], size, f'-{name[0]}-START-'), 
-            self.getText('Stop:  ', size, 'right'), self.getI(default_values[1], size, f'-{name[0]}-STOP-'), 
-            self.getText('Step:  ', size, 'right'), self.getI(default_values[2], size, f'-{name[0]}-STEP-'), self.getP()]
-        ]
-        return sg.Column(module, background_color=self.bg_color)
-    
-    def getMacros(self, fn_labels=['fn1', 'fn2', 'fn3']):
-        """
-        Get Macro buttons module
-        - fn_labels: labels for the three function buttons
-        
-        Return: sg.Column object
-        """
-        overall_size = 64
-        size_B = (int(overall_size/6), 2)
-        fn_keys = [s.replace(' ', '').upper() for s in fn_labels]
-        module = [
-            [self.getTitle("Macro", (overall_size, 1), 'center', bold=True)],
-            [self.getP((12,1)), self.getB("Default View", size_B), self.getB("Probe", size_B), 
-            self.getB("Cam", size_B), self.getB("Calibrate", size_B), self.getP((12,1))],
-            [self.getP((12,1)), self.getB("Set View", size_B), self.getB(f"{fn_labels[0]}", size_B, f'-{fn_keys[0].upper()}-'), 
-            self.getB(f"{fn_labels[1]}", size_B, f'-{fn_keys[1].upper()}-'), self.getB(f"{fn_labels[2]}", size_B, f'-{fn_keys[2].upper()}-'), self.getP((12,1))]
-        ]
-        return sg.Column(module, background_color=self.bg_color)
-
     def getOpenCV(self):
         """
         Get Open CV control module
         Return: sg.Column object
         """
         overall_size = 64
         size_R = (int(overall_size/8), 1)
@@ -391,69 +221,14 @@
             [self.getText("Min Neighbour  ", (20,0), 'right'), self.getS((0,20), 10, 'h', size_S, "-NEIGHBOR SLIDER-")],
             [self.getText("BG Noise Removal  ", (20,1), 'right'), self.getS((0,5), 0, 'h', size_S, "-OPENING SLIDER-")], 
             [self.getText("FG Noise Removal  ", (20,1), 'right'), self.getS((0,5), 0, 'h', size_S, "-CLOSING SLIDER-")]
         ]
         return sg.Column(module, background_color=self.bg_color)
 
 
-# %%
-class Builder(Modules):
-    """
-    Child class of Modules.
-    Generate layouts from modules.
-    - theme: overall UI theme
-    - font: text font
-    - title_size: size of title text
-    - text_size: size of body text
-    - bg_color: background color
-    """
-    def __init__(self, theme=THEME, font=FONT, title_size=TITLE_SIZE, text_size=TEXT_SIZE, bg_color=BG_COLOR):
-        super().__init__(theme, font, title_size, text_size, bg_color)
-        self.layouts = {}
-        self.layout = []
-        return
-    
-    def addCollapsable(self, name, items, alignV=None, visible=True):
-        """
-        Add a new collapsable layout to collection
-        - name: name of the new layout
-        - items: elements or columns to be added into the layout
-        - alignV: vertial alignment of items
-        - visible: whether layout is visible
-        """
-        layout = items
-        self.layouts[name] = sg.pin(sg.Column(layout, vertical_alignment=alignV, key=name, visible=visible))
-        return
-
-    def addLayout(self, name, items, alignV=None, visible=True):
-        """
-        Add a new layout to collection
-        - name: name of the new layout
-        - items: elements or columns to be added into the layout
-        - alignV: vertial alignment of items
-        - visible: whether layout is visible
-        """
-        if name == '-FINAL-':
-            self.layout = items
-            return
-        layout = items
-        self.layouts[name] = sg.Column(layout, vertical_alignment=alignV, key=name, visible=visible)
-        return
-
-    def getWindow(self, gui_name):
-        """
-        Generate a GUI window from the final layout stored
-        - gui_name: name of window to be displayed
-
-        Return: sg.Window object
-        """
-        window = sg.Window(gui_name, self.layout, enable_close_attempted_event=True, resizable=True, finalize=True)
-        return window
-
-
 class Popups(Elements):
     """
     Child class of Elements.
     Generate Popups from modules.
     - theme: overall UI theme
     - font: text font
     - title_size: size of title text
```

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/GUI/viewer_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 # Standard library imports
 from __future__ import annotations
 import time
 from typing import Protocol
 
 # Third party imports
+import cv2              # pip install opencv-python
 import PySimpleGUI as sg # pip install PySimpleGUI
 
 # Local application imports
 from .gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
 class Viewer(Protocol):
@@ -59,15 +60,15 @@
             name (str, optional): name of panel. Defaults to 'VIEW'.
             group (str, optional): name of group. Defaults to 'viewer'.
         """
         super().__init__(name=name, group=group, **kwargs)
         self.tool = viewer
         
         self.display_box = self._mangle('-IMAGE-')
-        self._last_read_time = time.time()
+        self._last_read_time = time.perf_counter()
         
         self.setFlag(update_display=True)
         return
     
     # Properties
     @property
     def viewer(self) -> Viewer:
@@ -106,15 +107,16 @@
             values (dict[str, str]): dictionary of values from window
 
         Returns:
             dict: dictionary of updates
         """
         updates = {}
         if self.flags['update_display']:
-            frame_interval = time.time() - self._last_read_time
-            fps = round(1/frame_interval, 2)
-            ret, image = self.viewer.getImage()
-            self._last_read_time = time.time()
+            now = time.perf_counter()
+            ret, frame = self.viewer.getImage()
             if ret:
-                image = image.addText(f'FPS: {fps}', position=(0,image.frame.shape[0]-5), inplace=False)
-            updates[self.display_box] = dict(data=image.encode())
+                frame_interval =  now - self._last_read_time
+                self._last_read_time = now
+                fps = round(1/frame_interval, 2)
+                frame = cv2.putText(frame, f'FPS: {fps}', (0,frame.shape[0]-5), cv2.FONT_HERSHEY_PLAIN, 1, (255,255,255), 1)
+            updates[self.display_box] = dict(data=cv2.imencode(".png", frame)[1].tobytes())
         return updates
```

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/Physical/balance_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,16 +126,18 @@
                     value, 
                     self.calibration_factor, 
                     self.baseline, 
                     self._mass
                 ]
                 row = {k:v for k,v in zip(COLUMNS, values)}
                 # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
-                new_row_df = pd.DataFrame(row)
-                self.buffer_df = pd.concat([self.buffer_df, new_row_df])
+                # new_row_df = pd.DataFrame(row)
+                # self.buffer_df = pd.concat([self.buffer_df, new_row_df])
+                new_row_df = pd.DataFrame(row, index=[0])
+                self.buffer_df = pd.concat([self.buffer_df, new_row_df], ignore_index=True)
         return response
   
     def reset(self):
         """Reset the device"""
         super().reset()
         self.baseline = 0
         return
```

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.1a1/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/image_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/image_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,323 +1,28 @@
 # %% -*- coding: utf-8 -*-
 """
 This module holds the base class for image data.
 
-Classes:
-    Image
-    
 Functions:
     addText
     annotate
     blur
-    convertToRGB
     convolve
     crosshair
-    encode
-    grayscale
     process
     removeNoise
-    resize
     rotate
-    save
 """
 # Standard library imports
 from __future__ import annotations
 import numpy as np
-from typing import Optional
 
 # Third party imports
 import cv2              # pip install opencv-python
 print(f"Import: OK <{__name__}>")
-
-class Image:
-    """
-    Image class with image manipulation methods
-
-    ### Constructor
-    Args:
-        `frame` (np.ndarray): frame array
-        
-    ### Attributes
-    - `frame` (np.ndarray): frame array
-    
-    ### Methods
-    - `addText`: add text to the image
-    - `annotate`: annotate the image to label identified targets
-    - `blur`: blur the image
-    - `convertToRGB`: turn the image to RGB
-    - `crosshair`: add crosshair in the middle of image
-    - `encode`: encode the frame into bytes
-    - `grayscale`: turn image to grayscale
-    - `process`: process the image
-    - `removeNoise`: remove noise from image
-    - `resize`: resize the image
-    - `rotate`: rotate the 2D array of multiples of 90 degrees, clockwise
-    - `save`: save image to file
-    """
-    
-    def __init__(self, frame:np.ndarray):
-        """
-        Instantiate the class
-
-        Args:
-            frame (np.ndarray): frame array
-        """
-        self.frame = frame
-        pass
-    
-    def addText(self, text:str, position:tuple[int], inplace:bool = False) -> Optional[Image]:
-        """
-        Add text to the image
-
-        Args:
-            text (str): text to be added
-            position (tuple[int]): x,y position of where to place the text
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = self.frame
-        frame = cv2.putText(frame, text, position, cv2.FONT_HERSHEY_PLAIN, 1, (255,255,255), 1)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def annotate(self, index:int, dimensions:tuple[int], inplace:bool = False) -> Optional[Image]:
-        """
-        Annotate the image to label identified targets
-
-        Args:
-            index (int): index of target
-            dimensions (tuple[int]): list of x,y,w,h
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        x,y,w,h = dimensions
-        frame = self.frame
-        frame = cv2.rectangle(frame, (x,y), (x+w, y+h), (0,255,0), 2)
-        frame = cv2.circle(frame, (int(x+(w/2)), int(y+(h/2))), 3, (0,0,255), -1)
-        frame = cv2.putText(frame, '{}'.format(index+1), (x-8, y-4), cv2.FONT_HERSHEY_PLAIN, 1, (255,255,255), 1)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def blur(self, blur_kernel:int = 3, inplace:bool = False) -> Optional[Image]:
-        """
-        Blur the image
-
-        Args:
-            blur_kernel (int, optional): level of blurring, odd numbers only, minimum value of 3. Defaults to 3.
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = cv2.GaussianBlur(self.frame, (blur_kernel,blur_kernel), 0)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def convertToRGB(self, inplace:bool = False) -> Optional[Image]:
-        """
-        Turn image to RGB
-
-        Args:
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = cv2.cvtColor(self.frame, cv2.COLOR_BGR2RGB)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    # def convolve(self, inplace:bool = False) -> Optional[Image]: # FIXME
-    #     """
-    #     Perform convolution on image
-
-    #     Args:
-    #         inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-    #     Returns:
-    #         Image, or None: Image object, or None (if inplace=True)
-    #     """
-    #     return
-    
-    def crosshair(self, inplace:bool = False) -> Optional[Image]:
-        """
-        Add crosshair in the middle of image
-
-        Args:
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = self.frame
-        center_x = int(frame.shape[1] / 2)
-        center_y = int(frame.shape[0] / 2)
-        cv2.line(frame, (center_x, center_y+50), (center_x, center_y-50), (255,255,255), 1)
-        cv2.line(frame, (center_x+50, center_y), (center_x-50, center_y), (255,255,255), 1)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def encode(self, extension:str = '.png'):
-        """
-        Encode image into byte array
-
-        Args:
-            extension (str, optional): image format to encode to. Defaults to '.png'.
-
-        Returns:
-            bytes: byte array of image
-        """
-        return cv2.imencode(extension, self.frame)[1].tobytes()
-    
-    def grayscale(self, inplace:bool = False) -> Optional[Image]:
-        """
-        Turn image to grayscale
-
-        Args:
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = cv2.cvtColor(self.frame, cv2.COLOR_BGR2GRAY)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def process(self, alpha:float, beta:float, blur_kernel:int = 3, inplace:bool = False) -> Optional[Image]: # FIXME
-        """
-        Process the image
-
-        Args:
-            alpha (float): alpha value
-            beta (float): beta value
-            blur_kernel (int, optional): level of blurring, odd numbers only, minimum value of 3. Defaults to 3.
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = self.frame
-        frame = cv2.addWeighted(frame, alpha, np.zeros(frame.shape, frame.dtype), 0, beta)
-        if blur_kernel > 0:
-            frame = cv2.GaussianBlur(frame, (blur_kernel,blur_kernel), 0)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def removeNoise(self, open_iter:int = 0, close_iter:int = 0, inplace:bool = False) -> Optional[Image]:
-        """
-        Remove noise from image
-
-        Args:
-            open_iter (int, optional): opening iteration. Defaults to 0.
-            close_iter (int, optional): closing iteration. Defaults to 0.
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        kernel = np.ones((3,3),np.uint8)
-        frame = self.frame
-        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-        frame = cv2.morphologyEx(frame,cv2.MORPH_OPEN,kernel,iterations=open_iter)
-        frame = cv2.morphologyEx(frame,cv2.MORPH_CLOSE,kernel,iterations=close_iter)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def resize(self, size:tuple[int], inplace:bool = False) -> Optional[Image]:
-        """
-        Resize the image
-
-        Args:
-            size (tuple[int]): tuple of desired image width and height
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        frame = cv2.resize(self.frame, size)
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-    
-    def rotate(self, angle:int, inplace:bool = False) -> Optional[Image]:
-        """
-        Rotate a 2D array of multiples of 90 degrees, clockwise
-
-        Args:
-            angle (int): 90, 180, or 270 degrees
-            inplace (bool, optional): whether to perform action in place. Defaults to False.
-
-        Returns:
-            Optional[Image]: None if inplace else `Image` object
-        """
-        rotateCodes = {
-            90: cv2.ROTATE_90_CLOCKWISE,
-            180: cv2.ROTATE_180,
-            270: cv2.ROTATE_90_COUNTERCLOCKWISE
-        }
-        frame = self.frame
-        if angle != 0:
-            frame = cv2.rotate(frame, rotateCodes.get(angle))
-        if inplace:
-            self.frame = frame
-            return
-        return Image(frame)
-
-    def save(self, filename:str):
-        """
-        Save image to file
-
-        Args:
-            filename (str): filename to save to
-
-        Returns:
-            bool: whether the image is successfully saved
-        """
-        return cv2.imwrite(filename, self.frame)
-
-
-"""
-Image module with image manipulation functions
-
-### Functions
-- `addText`: add text to the image
-- `annotate`: annotate the image to label identified targets
-- `blur`: blur the image
-- `convertToRGB`: turn the image to RGB
-- `crosshair`: add crosshair in the middle of image
-- `encode`: encode the frame into bytes
-- `grayscale`: turn image to grayscale
-- `process`: process the image
-- `removeNoise`: remove noise from image
-- `resize`: resize the image
-- `rotate`: rotate the 2D array of multiples of 90 degrees, clockwise
-- `save`: save image to file
-"""
     
 def addText(frame:np.ndarray, text:str, position:tuple[int]) -> np.ndarray:
     """
     Add text to the image
 
     Args:
         frame (np.ndarray): frame array
@@ -356,26 +61,14 @@
         blur_kernel (int, optional): level of blurring, odd numbers only, minimum value of 3. Defaults to 3.
 
     Returns:
         np.ndarray: frame array
     """
     return cv2.GaussianBlur(frame, (blur_kernel,blur_kernel), 0)
 
-def convertToRGB(frame:np.ndarray) -> np.ndarray:
-    """
-    Turn image to RGB
-
-    Args:
-        frame (np.ndarray): frame array
-
-    Returns:
-        np.ndarray: frame array
-    """
-    return cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-
 def convolve(frame:np.ndarray) -> np.ndarray: # FIXME
     """
     Perform convolution on image
 
     Args:
         frame (np.ndarray): frame array
 
@@ -396,39 +89,14 @@
     """
     center_x = int(frame.shape[1] / 2)
     center_y = int(frame.shape[0] / 2)
     cv2.line(frame, (center_x, center_y+50), (center_x, center_y-50), (255,255,255), 1)
     cv2.line(frame, (center_x+50, center_y), (center_x-50, center_y), (255,255,255), 1)
     return frame
 
-def encode(frame:np.ndarray, extension:str = '.png') -> bytes:
-    """
-    Encode image into byte array
-
-    Args:
-        frame (np.ndarray): frame array
-        extension (str, optional): image format to encode to. Defaults to '.png'.
-
-    Returns:
-        bytes: byte array of image
-    """
-    return cv2.imencode(extension, frame)[1].tobytes()
-
-def grayscale(frame:np.ndarray) -> np.ndarray:
-    """
-    Turn image to grayscale
-
-    Args:
-        frame (np.ndarray): frame array
-
-    Returns:
-        np.ndarray: frame array
-    """
-    return cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-
 def process(frame:np.ndarray, alpha:float, beta:float, blur_kernel:int = 3) -> np.ndarray: # FIXME
     """
     Process the image
 
     Args:
         frame (np.ndarray): frame array
         alpha (float): alpha value
@@ -457,27 +125,14 @@
     """
     kernel = np.ones((3,3),np.uint8)
     frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
     frame = cv2.morphologyEx(frame,cv2.MORPH_OPEN,kernel,iterations=open_iter)
     frame = cv2.morphologyEx(frame,cv2.MORPH_CLOSE,kernel,iterations=close_iter)
     return frame
 
-def resize(frame:np.ndarray, size:tuple[int]) -> np.ndarray:
-    """
-    Resize the image
-
-    Args:
-        frame (np.ndarray): frame array
-        size (tuple[int]): tuple of desired image width and height
-
-    Returns:
-        np.ndarray: frame array
-    """
-    return cv2.resize(frame, size)
-
 def rotate(frame:np.ndarray, angle:int) -> np.ndarray:
     """
     Rotate a 2D array of multiples of 90 degrees, clockwise
 
     Args:
         frame (np.ndarray): frame array
         angle (int): 90, 180, or 270 degrees
@@ -490,19 +145,341 @@
         180: cv2.ROTATE_180,
         270: cv2.ROTATE_90_COUNTERCLOCKWISE
     }
     if angle != 0:
         frame = cv2.rotate(frame, rotateCodes.get(angle))
     return frame
 
-def save(frame:np.ndarray, filename:str) -> bool:
-    """
-    Save image to file
 
-    Args:
-        frame (np.ndarray): frame array
-        filename (str): filename to save to
 
-    Returns:
-        bool: whether the image is successfully saved
-    """
-    return cv2.imwrite(filename, frame)
+# NOTE: DEPRECATED
+
+# class Image:
+#     """
+#     Image class with image manipulation methods
+
+#     ### Constructor
+#     Args:
+#         `frame` (np.ndarray): frame array
+        
+#     ### Attributes
+#     - `frame` (np.ndarray): frame array
+    
+#     ### Methods
+#     - `addText`: add text to the image
+#     - `annotate`: annotate the image to label identified targets
+#     - `blur`: blur the image
+#     - `convertToRGB`: turn the image to RGB
+#     - `crosshair`: add crosshair in the middle of image
+#     - `encode`: encode the frame into bytes
+#     - `grayscale`: turn image to grayscale
+#     - `process`: process the image
+#     - `removeNoise`: remove noise from image
+#     - `resize`: resize the image
+#     - `rotate`: rotate the 2D array of multiples of 90 degrees, clockwise
+#     - `save`: save image to file
+#     """
+    
+#     def __init__(self, frame:np.ndarray):
+#         """
+#         Instantiate the class
+
+#         Args:
+#             frame (np.ndarray): frame array
+#         """
+#         self.frame = frame
+#         pass
+    
+#     def addText(self, text:str, position:tuple[int], inplace:bool = False) -> Optional[Image]:
+#         """
+#         Add text to the image
+
+#         Args:
+#             text (str): text to be added
+#             position (tuple[int]): x,y position of where to place the text
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = self.frame
+#         frame = cv2.putText(frame, text, position, cv2.FONT_HERSHEY_PLAIN, 1, (255,255,255), 1)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def annotate(self, index:int, dimensions:tuple[int], inplace:bool = False) -> Optional[Image]:
+#         """
+#         Annotate the image to label identified targets
+
+#         Args:
+#             index (int): index of target
+#             dimensions (tuple[int]): list of x,y,w,h
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         x,y,w,h = dimensions
+#         frame = self.frame
+#         frame = cv2.rectangle(frame, (x,y), (x+w, y+h), (0,255,0), 2)
+#         frame = cv2.circle(frame, (int(x+(w/2)), int(y+(h/2))), 3, (0,0,255), -1)
+#         frame = cv2.putText(frame, '{}'.format(index+1), (x-8, y-4), cv2.FONT_HERSHEY_PLAIN, 1, (255,255,255), 1)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def blur(self, blur_kernel:int = 3, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Blur the image
+
+#         Args:
+#             blur_kernel (int, optional): level of blurring, odd numbers only, minimum value of 3. Defaults to 3.
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = cv2.GaussianBlur(self.frame, (blur_kernel,blur_kernel), 0)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def convertToRGB(self, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Turn image to RGB
+
+#         Args:
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = cv2.cvtColor(self.frame, cv2.COLOR_BGR2RGB)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     # def convolve(self, inplace:bool = False) -> Optional[Image]: # FIXME
+#     #     """
+#     #     Perform convolution on image
+
+#     #     Args:
+#     #         inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#     #     Returns:
+#     #         Image, or None: Image object, or None (if inplace=True)
+#     #     """
+#     #     return
+    
+#     def crosshair(self, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Add crosshair in the middle of image
+
+#         Args:
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = self.frame
+#         center_x = int(frame.shape[1] / 2)
+#         center_y = int(frame.shape[0] / 2)
+#         cv2.line(frame, (center_x, center_y+50), (center_x, center_y-50), (255,255,255), 1)
+#         cv2.line(frame, (center_x+50, center_y), (center_x-50, center_y), (255,255,255), 1)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def encode(self, extension:str = '.png'):
+#         """
+#         Encode image into byte array
+
+#         Args:
+#             extension (str, optional): image format to encode to. Defaults to '.png'.
+
+#         Returns:
+#             bytes: byte array of image
+#         """
+#         return cv2.imencode(extension, self.frame)[1].tobytes()
+    
+#     def grayscale(self, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Turn image to grayscale
+
+#         Args:
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = cv2.cvtColor(self.frame, cv2.COLOR_BGR2GRAY)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def process(self, alpha:float, beta:float, blur_kernel:int = 3, inplace:bool = False) -> Optional[Image]: # FIXME
+#         """
+#         Process the image
+
+#         Args:
+#             alpha (float): alpha value
+#             beta (float): beta value
+#             blur_kernel (int, optional): level of blurring, odd numbers only, minimum value of 3. Defaults to 3.
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = self.frame
+#         frame = cv2.addWeighted(frame, alpha, np.zeros(frame.shape, frame.dtype), 0, beta)
+#         if blur_kernel > 0:
+#             frame = cv2.GaussianBlur(frame, (blur_kernel,blur_kernel), 0)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def removeNoise(self, open_iter:int = 0, close_iter:int = 0, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Remove noise from image
+
+#         Args:
+#             open_iter (int, optional): opening iteration. Defaults to 0.
+#             close_iter (int, optional): closing iteration. Defaults to 0.
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         kernel = np.ones((3,3),np.uint8)
+#         frame = self.frame
+#         frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+#         frame = cv2.morphologyEx(frame,cv2.MORPH_OPEN,kernel,iterations=open_iter)
+#         frame = cv2.morphologyEx(frame,cv2.MORPH_CLOSE,kernel,iterations=close_iter)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def resize(self, size:tuple[int], inplace:bool = False) -> Optional[Image]:
+#         """
+#         Resize the image
+
+#         Args:
+#             size (tuple[int]): tuple of desired image width and height
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         frame = cv2.resize(self.frame, size)
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+    
+#     def rotate(self, angle:int, inplace:bool = False) -> Optional[Image]:
+#         """
+#         Rotate a 2D array of multiples of 90 degrees, clockwise
+
+#         Args:
+#             angle (int): 90, 180, or 270 degrees
+#             inplace (bool, optional): whether to perform action in place. Defaults to False.
+
+#         Returns:
+#             Optional[Image]: None if inplace else `Image` object
+#         """
+#         rotateCodes = {
+#             90: cv2.ROTATE_90_CLOCKWISE,
+#             180: cv2.ROTATE_180,
+#             270: cv2.ROTATE_90_COUNTERCLOCKWISE
+#         }
+#         frame = self.frame
+#         if angle != 0:
+#             frame = cv2.rotate(frame, rotateCodes.get(angle))
+#         if inplace:
+#             self.frame = frame
+#             return
+#         return Image(frame)
+
+#     def save(self, filename:str):
+#         """
+#         Save image to file
+
+#         Args:
+#             filename (str): filename to save to
+
+#         Returns:
+#             bool: whether the image is successfully saved
+#         """
+#         return cv2.imwrite(filename, self.frame)
+
+
+# def convertToRGB(frame:np.ndarray) -> np.ndarray:
+#     """
+#     Turn image to RGB
+
+#     Args:
+#         frame (np.ndarray): frame array
+
+#     Returns:
+#         np.ndarray: frame array
+#     """
+#     return cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+
+# def encode(frame:np.ndarray, extension:str = '.png') -> bytes:
+#     """
+#     Encode image into byte array
+
+#     Args:
+#         frame (np.ndarray): frame array
+#         extension (str, optional): image format to encode to. Defaults to '.png'.
+
+#     Returns:
+#         bytes: byte array of image
+#     """
+#     return cv2.imencode(extension, frame)[1].tobytes()
+
+# def grayscale(frame:np.ndarray) -> np.ndarray:
+#     """
+#     Turn image to grayscale
+
+#     Args:
+#         frame (np.ndarray): frame array
+
+#     Returns:
+#         np.ndarray: frame array
+#     """
+#     return cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+
+# def resize(frame:np.ndarray, size:tuple[int]) -> np.ndarray:
+#     """
+#     Resize the image
+
+#     Args:
+#         frame (np.ndarray): frame array
+#         size (tuple[int]): tuple of desired image width and height
+
+#     Returns:
+#         np.ndarray: frame array
+#     """
+#     return cv2.resize(frame, size)
+
+# def save(frame:np.ndarray, filename:str) -> bool:
+#     """
+#     Save image to file
+
+#     Args:
+#         frame (np.ndarray): frame array
+#         filename (str): filename to save to
+
+#     Returns:
+#         bool: whether the image is successfully saved
+#     """
+#     return cv2.imwrite(filename, frame)
```

### Comparing `control-lab-ly-1.0.1a0/src/controllably/View/view_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/View/view_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from typing import Optional, Protocol
 
 # Third party imports
 import cv2              # pip install opencv-python
 
 # Local application imports
 from ..misc import Helper
-from .image_utils import Image
-# from . import image_utils as Image
+from . import image_utils as Image
 print(f"Import: OK <{__name__}>")
 
 DIMENSION_THRESHOLD = 36
 """Minimum width in pixels of target for detection"""
 ROW_DISTANCE = 30
 """Number of pixels between rows of detected targets"""
 
@@ -53,15 +52,15 @@
     - `calibration_unit` (float): calibration from pixels to mm
     - `cam_size` (tuple[int], optional): (width, height) of camera feed
     - `classifier` (Classifier): image classifier object
     - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
     - `device` (Callable): device object that communicates with physical tool
     - `feed` (Callable): connection to image feed
     - `flags` (dict[str, bool]): keywords paired with boolean flags
-    - `placeholder_image` (Image): placeholder image for when there is no feed available
+    - `placeholder_image` (np.ndarray): placeholder image for when there is no feed available
     - `record_folder` (str): filepath at which to store images and data
     - `record_timeout` (int): number of seconds to record images for
     - `rotation` (int): rotation angle for camera feed (multiples of 90 degrees)
     - `verbose` (bool): verbosity of class
     
     ### Methods
     #### Abstract
@@ -78,15 +77,15 @@
     - `isConnected`: checks and returns whether the device is connected
     - `loadClassifier`: load the desired image classifier
     - `loadImage`: load an image from file
     - `resetFlags`: reset all flags to class attribute `_default_flags`
     - `saveImage`: save image to file
     - `setFlag`: set flags by using keyword arguments
     - `shutdown`: shutdown procedure for tool
-    - `toggleRecord`: start or stop data recording
+    - `toggleRecord`: start or stop image capture and recording
     """
     
     _default_flags: dict[str, bool] = {
         'connected': False,
         'pause_record': False,
         'record': False
     }
@@ -149,65 +148,58 @@
 
         Returns:
             tuple[bool, np.ndarray]: (whether frame is obtained, frame array)
         """
     
     def annotateAll(self, 
         df: pd.DataFrame, 
-        image: Optional[Image] = None, 
-        frame: Optional[np.ndarray] = None    
-    ) -> tuple[dict[str,tuple[int]], Image]:
+        frame: np.ndarray
+    ) -> tuple[dict[str,tuple[int]], np.ndarray]:
         """
         Annotate all detected targets
 
         Args:
-            df (pd.DataFrame): dataframe of detected targets details
-            image (Optional[Image], optional): image object. Defaults to None.
-            frame (Optional[np.ndarray], optional): frame array. Defaults to None.
+            df (pd.DataFrame): dataframe of detected targets detail
+            frame (np.ndarray): image array
 
         Returns:
-            tuple[dict[str,tuple[int]], Image]: ({target index: center positions}, image object)
+            tuple[dict[str,tuple[int]], np.ndarray]: ({target index: center positions}, image array)
         """
         data = {}
-        if (frame is None) == (image is None):
-            raise Exception('Please input either image or frame.')
-        elif frame is not None:
-            image = Image(frame)
-            
         for index in range(len(df)):
             dimensions = df.loc[index, ['x','y','w','h']].to_list()
             x,y,w,h = dimensions
             if w*h >= DIMENSION_THRESHOLD**2:                       # Compare area to threshold
-                image.annotate(index, (x,y,w,h), inplace=True)
+                frame = Image.annotate(frame=frame, index=index, dimensions=(x,y,w,h))
                 data[f'C{index+1}'] = (int(x+(w/2)), int(y+(h/2)))  # Center of target
-        return data, image
+        return data, frame
     
     def connect(self):
         """Establish connection with device"""
         return self._connect(**self.connection_details)
 
-    def detect(self, image:Image, scale:int, neighbors:int) -> pd.DataFrame:
+    def detect(self, frame:np.ndarray, scale:int, neighbors:int) -> pd.DataFrame:
         """
         Perform image detection
 
         Args:
-            image (Image): image to detect from
+            frame (np.ndarray): image array to detect from
             scale (int): scale at which to detect targets
             neighbors (int): minimum number of neighbors for targets
 
         Raises:
             RuntimeError: Please load a classifier first.
 
         Returns:
             pd.DataFrame: dataframe of detected targets
         """
         if self.classifier is None:
             raise RuntimeError('Please load a classifier first.')
-        image.grayscale(inplace=True)
-        detected_data = self.classifier.detect(frame=image.frame, scale=scale, neighbors=neighbors)
+        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+        detected_data = self.classifier.detect(frame=frame, scale=scale, neighbors=neighbors)
         return self._data_to_df(detected_data)
     
     def isConnected(self) -> bool:
         """
         Checks and returns whether the device is connected
 
         Returns:
@@ -220,18 +212,15 @@
     def loadClassifier(self, classifier:Classifier):
         """
         Load the desired image classifier
 
         Args:
             classifier (Classifier): desired image classifier
         """
-        # try:
         self.classifier = classifier
-        # except SystemError:
-        #     print('Please select a classifier.')
         return
 
     def resetFlags(self):
         """Reset all flags to class attribute `_default_flags`"""
         self.flags = self._default_flags.copy()
         return
     
@@ -276,121 +265,96 @@
             thread.start()
             self._threads['record_loop'] = thread
         else:
             self._threads['record_loop'].join()
         return
  
     # Image handling
-    def decodeImage(self, array:bytes) -> Image:
+    def decodeImage(self, array:bytes) -> np.ndarray:
         """
         Decode byte array of image
 
         Args:
             array (bytes): byte array of image
 
         Returns:
-            Image: image of decoded byte array
+            np.ndarray: image array of decoded byte array
         """
-        frame = cv2.imdecode(array, cv2.IMREAD_COLOR)
-        return Image(frame)
+        return cv2.imdecode(array, cv2.IMREAD_COLOR)
     
-    def encodeImage(self, 
-        image: Optional[Image] = None, 
-        frame: Optional[np.ndarray] = None, 
-        extension: str = '.png'
-    ) -> bytes:
+    def encodeImage(self, frame:np.ndarray, extension:str = '.png') -> bytes:
         """
         Encode image into byte array
 
         Args:
-            image (Optional[Image], optional): image object to be encoded. Defaults to None.
-            frame (Optional[np.ndarray], optional): frame array to be encoded. Defaults to None.
+            frame (np.ndarray): image array to be encoded
             extension (str, optional): image format to encode to. Defaults to '.png'.
 
-        Raises:
-            ValueError: Please input either image or frame.
-
         Returns:
-            bytes: byte array of image / frame
+            bytes: byte array of image
         """
-        if (frame is None) == (image is None):
-            raise ValueError('Please input either image or frame.')
-        elif image is not None:
-            return image.encode(extension)
         return cv2.imencode(extension, frame)[1].tobytes()
     
     def getImage(self, 
         crosshair: bool = False, 
         resize: bool = False
-    ) -> tuple[bool, Image]:
+    ) -> tuple[bool, np.ndarray]:
         """
         Get image from camera feed
 
         Args:
             crosshair (bool, optional): whether to overlay crosshair on image. Defaults to False.
             resize (bool, optional): whether to resize the image. Defaults to False.
 
         Returns:
-            tuple[bool, Image]: (whether an image is obtained, image object)
+            tuple[bool, np.ndarray]: (whether an image is obtained, image array)
         """
         ret = False
-        image = self.placeholder_image
+        frame = self.placeholder_image
         try:
             ret, frame = self._read()
         except AttributeError:
             pass
         if ret:
-            image = Image(frame)
             if resize:
-                image.resize(self.cam_size, inplace=True)
-            image.rotate(self.rotation, inplace=True)
+                frame = cv2.resize(frame, self.cam_size)
+            frame = Image.rotate(frame=frame, angle=self.rotation)
         if crosshair:
-            image.crosshair(inplace=True)
-        return ret, image
+            frame = Image.crosshair(frame=frame)
+        return ret, frame
 
-    def loadImage(self, filename:str) -> Image:
+    def loadImage(self, filename:str) -> np.ndarray:
         """
-        Load image from file
+        Load an image from file
 
         Args:
             filename (str): image filename
 
         Returns:
-            Image: image from file
+            np.ndarray: image array from file
         """
-        frame = cv2.imread(filename)
-        return Image(frame)
+        return cv2.imread(filename)
     
     def saveImage(self, 
-        image: Optional[Image] = None, 
-        frame: Optional[np.ndarray] = None, 
+        frame: np.ndarray, 
         filename: str = 'image.png'
     ) -> bool:
         """
         Save image to file
 
         Args:
-            image (Optional[Image], optional): image object to be saved. Defaults to None.
-            frame (Optional[np.ndarray], optional): frame array to be saved. Defaults to None.
+            frame (np.ndarray): frame array to be saved
             filename (str, optional): filename to save to. Defaults to 'image.png'.
 
-        Raises:
-            ValueError: Please input either image or frame.
-
         Returns:
-            bool: whether the image is successfully saved
+            bool: whether the image array is successfully saved
         """
         if filename == 'image.png':
             now = datetime.now().strftime("%Y%m%d_%H-%M-%S")
             filename = f'image{now}.png'
-        
-        if (frame is None) == (image is None):
-            raise ValueError('Please input either image or frame.')
-        elif image is not None:
-            return image.save(filename)
         return cv2.imwrite(filename, frame)
     
     # Protected method(s)
     def _data_to_df(self, data:dict) -> pd.DataFrame:
         """
         Convert data dictionary to dataframe
 
@@ -425,18 +389,18 @@
         folder = Helper.create_folder(self.record_folder, 'frames')
         
         start = datetime.now()
         while self.flags['record']:
             if self.flags['pause_record']:
                 continue
             now = datetime.now()
-            _, image = self.getImage()
-            self.saveImage(image, filename=f'{folder}/frames/frame_{frame_num:05}.png')
+            _, frame = self.getImage()
+            self.saveImage(frame=frame, filename=f'{folder}/frames/frame_{frame_num:05}.png')
             timestamps.append(now)
-            # frames.append(image.frame)
+            # frames.append(frame)
             frame_num += 1
             
             # Timer check
             if self.record_timeout is not None and (now - start).seconds > self.record_timeout:
                 break
         end = datetime.now()
         
@@ -462,25 +426,21 @@
         """
         Sets placeholder image for camera, if not  camera is not connected
 
         Args:
             filename (str, optional): name of placeholder image file. Defaults to class attribute `_placeholder_filename`.
             img_bytes (Optional[bytes], optional): byte array of placeholder image. Defaults to None.
             resize (bool, optional): whether to resize the image. Defaults to False.
-
-        Returns:
-            Image: image of placeholder
         """
-        image = None
+        frame = None
         if not len(filename) and img_bytes is None:
             img_bytes = pkgutil.get_data(self._package, self._placeholder_filename)
         if len(filename):
-            image = self.loadImage(filename)
+            frame = self.loadImage(filename)
         elif type(img_bytes) == bytes:
             array = np.asarray(bytearray(img_bytes), dtype="uint8")
-            image = self.decodeImage(array)
-        
+            frame = self.decodeImage(array)
         if resize:
-            image.resize(self.cam_size, inplace=True)
-        self.placeholder_image = image
+            frame = cv2.resize(frame, self.cam_size)
+        self.placeholder_image = frame
         return
```

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/__init__.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/factory.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/helper.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/layout.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/logger.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.1a1/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_compound_liquidmover.py` & `control-lab-ly-1.0.1a1/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_compound_spin_printer.py` & `control-lab-ly-1.0.1a1/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_dobot_m1pro.py` & `control-lab-ly-1.0.1a1/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_dobot_mg400.py` & `control-lab-ly-1.0.1a1/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_heat_peltier.py` & `control-lab-ly-1.0.1a1/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a0/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.0.1a1/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

